# Comparing `tmp/pyxel_sim-1.8.tar.gz` & `tmp/pyxel_sim-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxel_sim-1.8.tar", last modified: Thu Mar 30 09:27:05 2023, max compression
+gzip compressed data, was "pyxel_sim-1.9.tar", last modified: Thu Jun  1 10:40:29 2023, max compression
```

## Comparing `pyxel_sim-1.8.tar` & `pyxel_sim-1.9.tar`

### file list

```diff
@@ -1,339 +1,343 @@
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.495271 pyxel_sim-1.8/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      552 2023-03-29 16:35:58.000000 pyxel_sim-1.8/AUTHORS.rst
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1085 2022-08-02 12:27:04.000000 pyxel_sim-1.8/LICENSE.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      244 2023-03-29 16:35:58.000000 pyxel_sim-1.8/MANIFEST.in
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6923 2023-03-30 09:27:05.494547 pyxel_sim-1.8/PKG-INFO
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5492 2023-03-29 16:35:58.000000 pyxel_sim-1.8/README.md
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.080749 pyxel_sim-1.8/continuous_integration/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.120990 pyxel_sim-1.8/continuous_integration/scripts/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   126320 2023-03-29 17:56:34.000000 pyxel_sim-1.8/continuous_integration/scripts/auto_generated.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   125532 2023-01-30 18:33:41.000000 pyxel_sim-1.8/continuous_integration/scripts/copy_auto_generated.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    29757 2023-03-29 16:35:58.000000 pyxel_sim-1.8/continuous_integration/scripts/create_json_schema.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2421 2023-03-29 16:35:58.000000 pyxel_sim-1.8/continuous_integration/scripts/download_last_environment_artifact.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.083775 pyxel_sim-1.8/docs/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.082278 pyxel_sim-1.8/docs/html/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.122087 pyxel_sim-1.8/docs/html/_static/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2022-08-02 12:27:04.000000 pyxel_sim-1.8/docs/html/_static/dummy.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.083258 pyxel_sim-1.8/docs/jupyter_execute/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.123321 pyxel_sim-1.8/docs/jupyter_execute/howto/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2357 2022-11-15 08:58:01.000000 pyxel_sim-1.8/docs/jupyter_execute/howto/detector_import_export.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.124759 pyxel_sim-1.8/docs/source/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.125926 pyxel_sim-1.8/docs/source/_static/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2022-08-02 12:27:04.000000 pyxel_sim-1.8/docs/source/_static/dummy.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10759 2023-03-29 16:35:58.000000 pyxel_sim-1.8/docs/source/conf.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4800 2023-03-30 07:08:14.000000 pyxel_sim-1.8/pyproject.toml
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.496185 pyxel_sim-1.8/pyxel/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1013 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      653 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/__main__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      495 2023-03-30 09:27:05.496342 pyxel_sim-1.8/pyxel/_version.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.140315 pyxel_sim-1.8/pyxel/backends/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      478 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/backends/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2551 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/backends/asdf.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5726 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/backends/hdf5.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.151638 pyxel_sim-1.8/pyxel/calibration/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1002 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/calibration/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    14665 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/calibration/algorithm.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20608 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/calibration/archipelago.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17109 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/calibration/calibration.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2027 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/calibration/fitness.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16927 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/calibration/fitting.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2036 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/calibration/protocols.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5999 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/calibration/user_defined.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7533 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/calibration/util.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.154197 pyxel_sim-1.8/pyxel/configuration/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      511 2023-03-29 16:35:58.000000 pyxel_sim-1.8/pyxel/configuration/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15218 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/configuration/configuration.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.170156 pyxel_sim-1.8/pyxel/data_structure/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      707 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4823 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/array.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15980 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/charge.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1154 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4900 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/persistence.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      952 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/phase.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1909 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/photon.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1132 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/pixel.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2101 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/processed_data.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4412 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/scene.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1049 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/signal.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1340 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/data_structure/util.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.183101 pyxel_sim-1.8/pyxel/detectors/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      867 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.188085 pyxel_sim-1.8/pyxel/detectors/apd/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      516 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/apd/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5285 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/apd/apd.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15836 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/apd/apd_characteristics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      875 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/apd/apd_geometry.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.192186 pyxel_sim-1.8/pyxel/detectors/ccd/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      464 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/ccd/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4950 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/ccd/ccd.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      869 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/ccd/ccd_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8926 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/characteristics.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.197230 pyxel_sim-1.8/pyxel/detectors/cmos/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      468 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/cmos/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4977 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/cmos/cmos.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      877 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/cmos/cmos_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    21426 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/detector.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2385 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/environment.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8253 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/geometry.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.200908 pyxel_sim-1.8/pyxel/detectors/mkid/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      468 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/mkid/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6702 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/mkid/mkid.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      877 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/mkid/mkid_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      472 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/optics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2829 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/detectors/readout_properties.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4046 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/evaluator.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.204576 pyxel_sim-1.8/pyxel/exposure/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      518 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/exposure/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5480 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/exposure/exposure.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4690 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/exposure/readout.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.206697 pyxel_sim-1.8/pyxel/inputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      463 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/inputs/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8487 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/inputs/loader.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.209027 pyxel_sim-1.8/pyxel/models/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      450 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.219633 pyxel_sim-1.8/pyxel/models/charge_collection/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      643 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_collection/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      696 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_collection/collection.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9200 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_collection/diffusion.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4897 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_collection/fixed_pattern_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1488 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_collection/full_well.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3215 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_collection/inter_pixel_capacitance.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15939 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_collection/persistence.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.234199 pyxel_sim-1.8/pyxel/models/charge_generation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      859 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1774 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/apd_gain.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16820 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/charge_deposition.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2546 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/charge_injection.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.243942 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16105 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/cosmix.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.092963 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.256741 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13511 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/particle.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    23219 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/plotting.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20020 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/simulation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3672 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/util.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12505 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/dark_current.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6040 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/dark_current_rule07.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.263548 pyxel_sim-1.8/pyxel/models/charge_generation/data/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1875 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/data/mct-stopping-power.csv
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    51083 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    50826 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2524 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1948 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/load_charge.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4986 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_generation/photoelectrons.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.275833 pyxel_sim-1.8/pyxel/models/charge_measurement/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      853 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_measurement/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16384 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_measurement/linearity.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1636 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_measurement/measurement.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.281072 pyxel_sim-1.8/pyxel/models/charge_measurement/nghxrg/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_measurement/nghxrg/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13385 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_measurement/nghxrg/nghxrg.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    33375 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8678 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_measurement/non_linearity_calculation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3089 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_measurement/offset.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5633 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_measurement/readout_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2497 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_measurement/reset_noise.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.284839 pyxel_sim-1.8/pyxel/models/charge_transfer/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2677 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_transfer/EMCCD_poisson.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      496 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_transfer/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.288552 pyxel_sim-1.8/pyxel/models/charge_transfer/arctic_cti/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_transfer/arctic_cti/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8693 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    18700 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/charge_transfer/cdm.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.292050 pyxel_sim-1.8/pyxel/models/data_processing/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      565 2023-03-30 07:08:14.000000 pyxel_sim-1.8/pyxel/models/data_processing/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4798 2023-03-30 07:08:14.000000 pyxel_sim-1.8/pyxel/models/data_processing/source_extractor.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1735 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/data_processing/statistics.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.295576 pyxel_sim-1.8/pyxel/models/optics/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      662 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/optics/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2009 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/optics/point_spread_function.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12706 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/optics/poppy.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.297997 pyxel_sim-1.8/pyxel/models/phasing/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      450 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/phasing/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2126 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/phasing/pulse_processing.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.306584 pyxel_sim-1.8/pyxel/models/photon_collection/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      630 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_collection/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7898 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_collection/illumination.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2958 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_collection/load_image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1794 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_collection/point_spread_function.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12492 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_collection/poppy.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2572 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_collection/shot_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3663 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_collection/stripe_pattern.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.312409 pyxel_sim-1.8/pyxel/models/photon_generation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      750 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_generation/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8124 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_generation/illumination.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3157 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_generation/load_image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2772 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_generation/shot_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3893 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/photon_generation/stripe_pattern.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.327741 pyxel_sim-1.8/pyxel/models/readout_electronics/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      716 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/readout_electronics/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1413 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/readout_electronics/amplification.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9440 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/readout_electronics/amplifier_crosstalk.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3552 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/readout_electronics/dead_time.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      916 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/readout_electronics/phase_conversion.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2348 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/readout_electronics/sar_adc.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7135 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/readout_electronics/sar_adc_with_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2274 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/readout_electronics/simple_adc.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.329660 pyxel_sim-1.8/pyxel/models/scene_generation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/scene_generation/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.331362 pyxel_sim-1.8/pyxel/models/signal_transfer/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      403 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/signal_transfer/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1272 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/models/util.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.336409 pyxel_sim-1.8/pyxel/notebook/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      784 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/notebook/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16272 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/notebook/calibration.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5202 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/notebook/html_representation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10379 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/notebook/jupyxel.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.340184 pyxel_sim-1.8/pyxel/observation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      532 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/observation/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    46903 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/observation/observation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5320 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/observation/parameter_values.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3876 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/options.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.346372 pyxel_sim-1.8/pyxel/outputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      621 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/outputs/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4853 2023-03-30 07:05:09.000000 pyxel_sim-1.8/pyxel/outputs/calibration_outputs.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3294 2023-03-30 06:58:42.000000 pyxel_sim-1.8/pyxel/outputs/exposure_outputs.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4504 2023-03-30 07:05:09.000000 pyxel_sim-1.8/pyxel/outputs/observation_outputs.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16253 2023-03-30 07:05:09.000000 pyxel_sim-1.8/pyxel/outputs/outputs.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.352841 pyxel_sim-1.8/pyxel/pipelines/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      668 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/pipelines/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6086 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/pipelines/model_function.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3068 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/pipelines/model_group.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8181 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/pipelines/pipeline.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9076 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/pipelines/processor.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17591 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/run.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4485 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/show_versions.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6107 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/state.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.353882 pyxel_sim-1.8/pyxel/templates/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4045 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/templates/_TEMPLATE.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.363155 pyxel_sim-1.8/pyxel/util/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3015 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/util/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3892 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/util/add_model.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1973 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/util/examples.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6178 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/util/image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7475 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/util/materials.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2314 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/util/memory.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      999 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/util/random.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2202 2023-03-29 16:35:59.000000 pyxel_sim-1.8/pyxel/util/timing.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.374652 pyxel_sim-1.8/pyxel_sim.egg-info/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6923 2023-03-30 09:27:04.000000 pyxel_sim-1.8/pyxel_sim.egg-info/PKG-INFO
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10393 2023-03-30 09:27:05.000000 pyxel_sim-1.8/pyxel_sim.egg-info/SOURCES.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        1 2023-03-30 09:27:04.000000 pyxel_sim-1.8/pyxel_sim.egg-info/dependency_links.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       41 2023-03-30 09:27:04.000000 pyxel_sim-1.8/pyxel_sim.egg-info/entry_points.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      392 2023-03-30 09:27:04.000000 pyxel_sim-1.8/pyxel_sim.egg-info/requires.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       91 2023-03-30 09:27:04.000000 pyxel_sim-1.8/pyxel_sim.egg-info/top_level.txt
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       38 2023-03-30 09:27:05.495439 pyxel_sim-1.8/setup.cfg
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      266 2023-03-29 16:35:59.000000 pyxel_sim-1.8/setup.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.383993 pyxel_sim-1.8/tests/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      375 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/__init__.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.386441 pyxel_sim-1.8/tests/calibration/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7424 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/calibration/test_check_ranges.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2171 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/calibration/test_slice_to_range.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.388945 pyxel_sim-1.8/tests/configuration/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15979 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/configuration/test_load.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1589 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/configuration/test_schema.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1485 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/conftest.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.391059 pyxel_sim-1.8/tests/data_structure/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    11580 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/data_structure/test_charge.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3890 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/data_structure/test_processed_data.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.406369 pyxel_sim-1.8/tests/detectors/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15075 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_ccd.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4861 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_ccd_characteristics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4295 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_ccd_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    11922 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_cmos.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4590 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_cmos_characteristics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4359 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_cmos_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7061 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_detectors.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2367 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_environment.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6977 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_geometry.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12315 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_mkid.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4583 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_mkid_characteristics.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4308 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/detectors/test_mkid_geometry.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.407420 pyxel_sim-1.8/tests/exposure/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1827 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/exposure/test_readout.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.410738 pyxel_sim-1.8/tests/functional_tests/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2022-08-02 12:27:05.000000 pyxel_sim-1.8/tests/functional_tests/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3700 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/functional_tests/test_parametric.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5386 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/functional_tests/test_yaml.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.411800 pyxel_sim-1.8/tests/inputs/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    21926 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/inputs/test_image.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.103219 pyxel_sim-1.8/tests/model_tests/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.413010 pyxel_sim-1.8/tests/model_tests/amplifier_crosstalk/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1060 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/model_tests/amplifier_crosstalk/test_crosstalk.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.414082 pyxel_sim-1.8/tests/models/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.423061 pyxel_sim-1.8/tests/models/charge_collection/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3046 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_collection/test_fixed_pattern_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5563 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_collection/test_persistence.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1946 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_collection/test_simple_full_well.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9628 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_collection/test_simple_ipc.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3609 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_collection/test_simple_persistence.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.435719 pyxel_sim-1.8/tests/models/charge_generation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2551 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_generation/test_apd_gain.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2867 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_generation/test_charge_deposition_in_MCT.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3528 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_generation/test_charge_injection.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5033 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_generation/test_dark_current.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1843 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_generation/test_dark_current_rule07.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4309 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_generation/test_load_charge.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3366 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_generation/test_photoelectrons.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.442187 pyxel_sim-1.8/tests/models/charge_measurement/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2659 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_measurement/test_nghxrg.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5942 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_measurement/test_non_linearity.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3793 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_measurement/test_offset.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4752 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_measurement/test_readout_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2723 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_measurement/test_reset_noise.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.447313 pyxel_sim-1.8/tests/models/charge_transfer/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2265 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_transfer/arctic_remove.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1680 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_transfer/test_arctic_add.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8612 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_transfer/test_cdm.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      718 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/charge_transfer/test_emccd_poisson.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.448429 pyxel_sim-1.8/tests/models/data_processing/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1332 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/data_processing/test_statistics.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.449643 pyxel_sim-1.8/tests/models/phasing/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3187 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/phasing/test_pulse_processing.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.458016 pyxel_sim-1.8/tests/models/photon_collection/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2887 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/photon_collection/test_illumination.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3899 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/photon_collection/test_load_image.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2042 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/photon_collection/test_load_psf.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5001 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/photon_collection/test_optical_psf.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5640 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/photon_collection/test_shot_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2081 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/photon_collection/test_stripe_pattern.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.471346 pyxel_sim-1.8/tests/models/readout_electronics/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3384 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/readout_electronics/test_ac_crosstalk.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3384 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/readout_electronics/test_dc_crosstalk.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2924 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/readout_electronics/test_dead_time_filter.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      720 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/readout_electronics/test_get_matrix.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1069 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/readout_electronics/test_phase_conversion.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1071 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/readout_electronics/test_sar_adc.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3229 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/readout_electronics/test_sar_adc_with_noise.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2161 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/readout_electronics/test_simple_adc.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2029 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/models/test_save_load_detector.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.473050 pyxel_sim-1.8/tests/pipelines/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.474576 pyxel_sim-1.8/tests/pipelines/observation/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2360 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/pipelines/observation/test_validate_steps.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1925 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/pipelines/test_pipelines.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.477654 pyxel_sim-1.8/tests/running_mode/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    21242 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/running_mode/test_observation.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1772 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/test_evaluator.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1914 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/test_options.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      486 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/test_show_versions.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.487803 pyxel_sim-1.8/tests/unittests/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      375 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/unittests/__init__.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1654 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/unittests/test_arguments.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4832 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/unittests/test_calibration.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3908 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/unittests/test_detector.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6789 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/unittests/test_environment.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15913 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/unittests/test_fitting.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2463 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/unittests/test_model_function.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.491617 pyxel_sim-1.8/tests/util/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10118 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/util/test_fit_into_array.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1375 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/util/test_memory.py
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2362 2023-03-29 16:35:59.000000 pyxel_sim-1.8/tests/util/test_random.py
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.109062 pyxel_sim-1.8/venv/
-drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-03-30 09:27:05.493055 pyxel_sim-1.8/venv/bin/
--rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1176 2023-01-04 09:36:07.000000 pyxel_sim-1.8/venv/bin/activate_this.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:29.105435 pyxel_sim-1.9/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      552 2023-03-29 16:35:58.000000 pyxel_sim-1.9/AUTHORS.rst
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1085 2022-08-02 12:27:04.000000 pyxel_sim-1.9/LICENSE.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      244 2023-03-29 16:35:58.000000 pyxel_sim-1.9/MANIFEST.in
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6924 2023-06-01 10:40:29.103587 pyxel_sim-1.9/PKG-INFO
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5492 2023-05-15 05:35:04.000000 pyxel_sim-1.9/README.md
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.675500 pyxel_sim-1.9/continuous_integration/
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.066278 pyxel_sim-1.9/continuous_integration/scripts/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   130300 2023-05-24 09:13:19.000000 pyxel_sim-1.9/continuous_integration/scripts/auto_generated.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   128772 2023-05-08 19:38:26.000000 pyxel_sim-1.9/continuous_integration/scripts/before_auto_generated.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    29848 2023-05-24 04:59:59.000000 pyxel_sim-1.9/continuous_integration/scripts/create_json_schema.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2421 2023-03-29 16:35:58.000000 pyxel_sim-1.9/continuous_integration/scripts/download_last_environment_artifact.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      249 2023-04-18 08:58:54.000000 pyxel_sim-1.9/continuous_integration/scripts/dummy.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.687646 pyxel_sim-1.9/docs/
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.684401 pyxel_sim-1.9/docs/html/
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.070375 pyxel_sim-1.9/docs/html/_static/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2022-08-02 12:27:04.000000 pyxel_sim-1.9/docs/html/_static/dummy.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.073493 pyxel_sim-1.9/docs/source/
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.077008 pyxel_sim-1.9/docs/source/_static/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2022-08-02 12:27:04.000000 pyxel_sim-1.9/docs/source/_static/dummy.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10728 2023-05-24 04:59:59.000000 pyxel_sim-1.9/docs/source/conf.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5669 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyproject.toml
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:29.107892 pyxel_sim-1.9/pyxel/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1013 2023-03-29 16:35:58.000000 pyxel_sim-1.9/pyxel/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      653 2023-03-29 16:35:58.000000 pyxel_sim-1.9/pyxel/__main__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      495 2023-06-01 10:40:29.108292 pyxel_sim-1.9/pyxel/_version.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.320146 pyxel_sim-1.9/pyxel/backends/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      478 2023-03-29 16:35:58.000000 pyxel_sim-1.9/pyxel/backends/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2840 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/backends/asdf.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6324 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/backends/hdf5.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.634432 pyxel_sim-1.9/pyxel/calibration/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1087 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/calibration/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    14707 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/calibration/algorithm.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20616 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/calibration/archipelago.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17840 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/calibration/archipelago_datatree.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    18051 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/calibration/calibration.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2065 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/calibration/fitness.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16917 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/calibration/fitting.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    17657 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/calibration/fitting_datatree.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2056 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/calibration/protocols.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5992 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/calibration/user_defined.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13610 2023-05-25 05:43:54.000000 pyxel_sim-1.9/pyxel/calibration/util.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.691558 pyxel_sim-1.9/pyxel/configuration/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      511 2023-03-29 16:35:58.000000 pyxel_sim-1.9/pyxel/configuration/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15239 2023-05-24 09:17:19.000000 pyxel_sim-1.9/pyxel/configuration/configuration.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:23.888254 pyxel_sim-1.9/pyxel/data_structure/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      707 2023-04-15 09:29:03.000000 pyxel_sim-1.9/pyxel/data_structure/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4914 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/data_structure/array.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16476 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/data_structure/charge.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1154 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/data_structure/image.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4902 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/data_structure/persistence.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      952 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/data_structure/phase.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1940 2023-05-17 07:08:29.000000 pyxel_sim-1.9/pyxel/data_structure/photon.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1132 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/data_structure/pixel.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2101 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/data_structure/processed_data.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4439 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/data_structure/scene.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1049 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/data_structure/signal.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1340 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/data_structure/util.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.063362 pyxel_sim-1.9/pyxel/detectors/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      867 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/__init__.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.118015 pyxel_sim-1.9/pyxel/detectors/apd/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      516 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/apd/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5666 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/apd/apd.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15856 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/apd/apd_characteristics.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      875 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/apd/apd_geometry.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.173248 pyxel_sim-1.9/pyxel/detectors/ccd/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      464 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/ccd/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5496 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/ccd/ccd.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      869 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/ccd/ccd_geometry.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9216 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/characteristics.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.199785 pyxel_sim-1.9/pyxel/detectors/cmos/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      468 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/cmos/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5358 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/cmos/cmos.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      877 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/cmos/cmos_geometry.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    22369 2023-05-24 08:35:07.000000 pyxel_sim-1.9/pyxel/detectors/detector.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2412 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/environment.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8273 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/detectors/geometry.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.247063 pyxel_sim-1.9/pyxel/detectors/mkid/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      468 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/mkid/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7083 2023-05-24 08:34:39.000000 pyxel_sim-1.9/pyxel/detectors/mkid/mkid.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      877 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/mkid/mkid_geometry.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      472 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/detectors/optics.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2824 2023-05-24 08:35:07.000000 pyxel_sim-1.9/pyxel/detectors/readout_properties.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4085 2023-05-24 08:35:07.000000 pyxel_sim-1.9/pyxel/evaluator.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.300724 pyxel_sim-1.9/pyxel/exposure/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      532 2023-05-17 07:08:29.000000 pyxel_sim-1.9/pyxel/exposure/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10011 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/exposure/exposure.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4710 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/exposure/readout.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.327623 pyxel_sim-1.9/pyxel/inputs/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      479 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/inputs/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9604 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/inputs/loader.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.390809 pyxel_sim-1.9/pyxel/models/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      450 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/__init__.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.535819 pyxel_sim-1.9/pyxel/models/charge_collection/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      643 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_collection/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      696 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_collection/collection.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9200 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_collection/diffusion.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4890 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_collection/fixed_pattern_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1488 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_collection/full_well.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3229 2023-05-17 07:08:29.000000 pyxel_sim-1.9/pyxel/models/charge_collection/inter_pixel_capacitance.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15959 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_collection/persistence.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.678669 pyxel_sim-1.9/pyxel/models/charge_generation/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      859 2023-05-30 12:18:54.000000 pyxel_sim-1.9/pyxel/models/charge_generation/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1165 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/charge_generation/apd_gain.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16775 2023-05-24 04:59:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/charge_deposition.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2539 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/charge_injection.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.835229 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16084 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/cosmix.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.740004 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:24.976460 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)   657923 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13498 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/particle.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    23212 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/plotting.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20041 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/simulation.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3672 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/util.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12524 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/dark_current.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6059 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/dark_current_rule07.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.069638 pyxel_sim-1.9/pyxel/models/charge_generation/data/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1875 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/data/mct-stopping-power.csv
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    51083 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    50826 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2524 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1941 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/load_charge.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4979 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_generation/photoelectrons.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.264847 pyxel_sim-1.9/pyxel/models/charge_measurement/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      853 2023-05-25 08:34:10.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16977 2023-05-25 08:34:10.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/linearity.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1636 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/measurement.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.350327 pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    13399 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/nghxrg.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    33333 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8678 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/non_linearity_calculation.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3063 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/offset.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5626 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/readout_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2490 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_measurement/reset_noise.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.462156 pyxel_sim-1.9/pyxel/models/charge_transfer/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2677 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_transfer/EMCCD_poisson.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      496 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_transfer/__init__.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.517357 pyxel_sim-1.9/pyxel/models/charge_transfer/arctic_cti/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/charge_transfer/arctic_cti/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8702 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    18727 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/charge_transfer/cdm.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.637538 pyxel_sim-1.9/pyxel/models/data_processing/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      647 2023-05-24 08:35:07.000000 pyxel_sim-1.9/pyxel/models/data_processing/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6055 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/models/data_processing/linear_regression.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5397 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/models/data_processing/mean_variance.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4798 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/data_processing/source_extractor.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3882 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/models/data_processing/statistics.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.671692 pyxel_sim-1.9/pyxel/models/optics/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      662 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/optics/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2009 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/optics/point_spread_function.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12726 2023-05-22 12:43:55.000000 pyxel_sim-1.9/pyxel/models/optics/poppy.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.730350 pyxel_sim-1.9/pyxel/models/phasing/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      450 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/phasing/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2126 2023-05-24 08:34:39.000000 pyxel_sim-1.9/pyxel/models/phasing/pulse_processing.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.884241 pyxel_sim-1.9/pyxel/models/photon_collection/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      630 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/photon_collection/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7918 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_collection/illumination.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2951 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_collection/load_image.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1794 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_collection/point_spread_function.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12512 2023-05-22 12:43:55.000000 pyxel_sim-1.9/pyxel/models/photon_collection/poppy.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2611 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_collection/shot_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3657 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/photon_collection/stripe_pattern.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:25.988669 pyxel_sim-1.9/pyxel/models/photon_generation/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      750 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/photon_generation/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8144 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_generation/illumination.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3150 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_generation/load_image.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2811 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/photon_generation/shot_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3887 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/photon_generation/stripe_pattern.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.210492 pyxel_sim-1.9/pyxel/models/readout_electronics/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      716 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1413 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/amplification.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9454 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/amplifier_crosstalk.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3552 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/dead_time.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      916 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/phase_conversion.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2348 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/sar_adc.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7109 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/sar_adc_with_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2267 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/models/readout_electronics/simple_adc.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.232095 pyxel_sim-1.9/pyxel/models/scene_generation/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      387 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/scene_generation/__init__.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.259567 pyxel_sim-1.9/pyxel/models/signal_transfer/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      403 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/models/signal_transfer/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1272 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/models/util.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.346727 pyxel_sim-1.9/pyxel/notebook/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      784 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/notebook/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16292 2023-05-31 14:39:03.000000 pyxel_sim-1.9/pyxel/notebook/calibration.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5202 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/notebook/html_representation.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10431 2023-05-24 08:34:39.000000 pyxel_sim-1.9/pyxel/notebook/jupyxel.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.422174 pyxel_sim-1.9/pyxel/observation/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      532 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/observation/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    43007 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/observation/observation.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5340 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/observation/parameter_values.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3903 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/options.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.565094 pyxel_sim-1.9/pyxel/outputs/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      621 2023-04-19 20:35:04.000000 pyxel_sim-1.9/pyxel/outputs/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4847 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/outputs/calibration_outputs.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3146 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/outputs/exposure_outputs.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4488 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/outputs/observation_outputs.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    16300 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/outputs/outputs.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.696763 pyxel_sim-1.9/pyxel/pipelines/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      681 2023-05-31 10:39:46.000000 pyxel_sim-1.9/pyxel/pipelines/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6107 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/pipelines/model_function.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3089 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/pipelines/model_group.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8201 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/pipelines/pipeline.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9320 2023-05-31 10:39:47.000000 pyxel_sim-1.9/pyxel/pipelines/processor.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    20958 2023-05-31 14:38:11.000000 pyxel_sim-1.9/pyxel/run.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4567 2023-05-30 05:42:20.000000 pyxel_sim-1.9/pyxel/show_versions.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6124 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/state.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.748908 pyxel_sim-1.9/pyxel/templates/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4039 2023-05-24 04:59:59.000000 pyxel_sim-1.9/pyxel/templates/_TEMPLATE.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.938172 pyxel_sim-1.9/pyxel/util/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3015 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/util/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3867 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/util/add_model.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1973 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/util/examples.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6171 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/util/image.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7475 2023-03-29 16:35:59.000000 pyxel_sim-1.9/pyxel/util/materials.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2308 2023-05-15 05:35:04.000000 pyxel_sim-1.9/pyxel/util/memory.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      999 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/util/random.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2202 2023-05-22 12:44:18.000000 pyxel_sim-1.9/pyxel/util/timing.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:26.960083 pyxel_sim-1.9/pyxel_sim.egg-info/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6924 2023-06-01 10:40:13.000000 pyxel_sim-1.9/pyxel_sim.egg-info/PKG-INFO
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10638 2023-06-01 10:40:22.000000 pyxel_sim-1.9/pyxel_sim.egg-info/SOURCES.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        1 2023-06-01 10:40:13.000000 pyxel_sim-1.9/pyxel_sim.egg-info/dependency_links.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       41 2023-06-01 10:40:13.000000 pyxel_sim-1.9/pyxel_sim.egg-info/entry_points.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      425 2023-06-01 10:40:13.000000 pyxel_sim-1.9/pyxel_sim.egg-info/requires.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      101 2023-06-01 10:40:13.000000 pyxel_sim-1.9/pyxel_sim.egg-info/top_level.txt
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)       38 2023-06-01 10:40:29.105879 pyxel_sim-1.9/setup.cfg
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      266 2023-03-29 16:35:59.000000 pyxel_sim-1.9/setup.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.052468 pyxel_sim-1.9/tests/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      375 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/__init__.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.112009 pyxel_sim-1.9/tests/calibration/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7424 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/calibration/test_check_ranges.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2932 2023-05-31 10:39:47.000000 pyxel_sim-1.9/tests/calibration/test_fitness.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2171 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/calibration/test_slice_to_range.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.166710 pyxel_sim-1.9/tests/configuration/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15979 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/configuration/test_load.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1589 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/configuration/test_schema.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1485 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/conftest.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.174528 pyxel_sim-1.9/tests/data_structure/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12924 2023-05-24 08:35:07.000000 pyxel_sim-1.9/tests/data_structure/test_charge.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3890 2023-04-15 09:29:03.000000 pyxel_sim-1.9/tests/data_structure/test_processed_data.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.419458 pyxel_sim-1.9/tests/detectors/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15278 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/detectors/test_ccd.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4861 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_ccd_characteristics.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4295 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_ccd_geometry.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    11767 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/detectors/test_cmos.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4590 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_cmos_characteristics.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4359 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_cmos_geometry.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     7061 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/detectors/test_detectors.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2367 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_environment.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6977 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/detectors/test_geometry.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    12053 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/detectors/test_mkid.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4583 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_mkid_characteristics.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4308 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/detectors/test_mkid_geometry.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.465334 pyxel_sim-1.9/tests/exposure/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1827 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/exposure/test_readout.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.536674 pyxel_sim-1.9/tests/functional_tests/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2022-08-02 12:27:05.000000 pyxel_sim-1.9/tests/functional_tests/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3369 2023-05-17 07:08:30.000000 pyxel_sim-1.9/tests/functional_tests/test_basic_exposure.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4076 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/functional_tests/test_parametric.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5386 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/functional_tests/test_yaml.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.583129 pyxel_sim-1.9/tests/inputs/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    21926 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/inputs/test_image.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.792841 pyxel_sim-1.9/tests/model_tests/
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.611553 pyxel_sim-1.9/tests/model_tests/amplifier_crosstalk/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1060 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/model_tests/amplifier_crosstalk/test_crosstalk.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.649427 pyxel_sim-1.9/tests/models/
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.774176 pyxel_sim-1.9/tests/models/charge_collection/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3046 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/charge_collection/test_fixed_pattern_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5572 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/models/charge_collection/test_persistence.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1946 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_collection/test_simple_full_well.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     9628 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_collection/test_simple_ipc.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3609 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_collection/test_simple_persistence.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:27.932761 pyxel_sim-1.9/tests/models/charge_generation/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2551 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_apd_gain.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2867 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_charge_deposition_in_MCT.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3528 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_charge_injection.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5033 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_dark_current.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1843 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_dark_current_rule07.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4309 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_generation/test_load_charge.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3366 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/charge_generation/test_photoelectrons.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.244769 pyxel_sim-1.9/tests/models/charge_measurement/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2659 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_measurement/test_nghxrg.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5951 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/models/charge_measurement/test_non_linearity.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3793 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_measurement/test_offset.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4752 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/charge_measurement/test_readout_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2723 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/charge_measurement/test_reset_noise.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.299909 pyxel_sim-1.9/tests/models/charge_transfer/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2265 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_transfer/arctic_remove.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1680 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_transfer/test_arctic_add.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     8639 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/charge_transfer/test_cdm.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      718 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/charge_transfer/test_emccd_poisson.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.317423 pyxel_sim-1.9/tests/models/data_processing/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1916 2023-05-17 07:08:30.000000 pyxel_sim-1.9/tests/models/data_processing/test_statistics.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.336552 pyxel_sim-1.9/tests/models/phasing/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3187 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/phasing/test_pulse_processing.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.532086 pyxel_sim-1.9/tests/models/photon_collection/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2914 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/photon_collection/test_illumination.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3899 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/models/photon_collection/test_load_image.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2042 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/photon_collection/test_load_psf.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5010 2023-05-15 05:35:04.000000 pyxel_sim-1.9/tests/models/photon_collection/test_optical_psf.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     5640 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/photon_collection/test_shot_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2081 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/photon_collection/test_stripe_pattern.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.708821 pyxel_sim-1.9/tests/models/readout_electronics/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3384 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_ac_crosstalk.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3384 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_dc_crosstalk.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2924 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_dead_time_filter.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      720 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_get_matrix.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1069 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_phase_conversion.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1071 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_sar_adc.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3229 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_sar_adc_with_noise.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2161 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/readout_electronics/test_simple_adc.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2029 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/models/test_save_load_detector.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.716014 pyxel_sim-1.9/tests/pipelines/
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.741396 pyxel_sim-1.9/tests/pipelines/observation/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2360 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/pipelines/observation/test_validate_steps.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1925 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/pipelines/test_pipelines.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.772580 pyxel_sim-1.9/tests/running_mode/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    21242 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/running_mode/test_observation.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1772 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/test_evaluator.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1914 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/test_options.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      486 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/test_show_versions.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:28.983777 pyxel_sim-1.9/tests/unittests/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)      375 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/__init__.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1654 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/test_arguments.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     4832 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/test_calibration.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     3908 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/test_detector.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     6789 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/test_environment.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    15920 2023-05-31 10:39:47.000000 pyxel_sim-1.9/tests/unittests/test_fitting.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2463 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/unittests/test_model_function.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:29.081576 pyxel_sim-1.9/tests/util/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)    10118 2023-05-22 12:44:18.000000 pyxel_sim-1.9/tests/util/test_fit_into_array.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1375 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/util/test_memory.py
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     2362 2023-03-29 16:35:59.000000 pyxel_sim-1.9/tests/util/test_random.py
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:22.820615 pyxel_sim-1.9/venv/
+drwxr-xr-x   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)        0 2023-06-01 10:40:29.100325 pyxel_sim-1.9/venv/bin/
+-rw-r--r--   0 frederic lemmel (1604465057) ESAAD\Domain Users (1276952531)     1176 2023-01-04 09:36:07.000000 pyxel_sim-1.9/venv/bin/activate_this.py
```

### Comparing `pyxel_sim-1.8/AUTHORS.rst` & `pyxel_sim-1.9/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/LICENSE.txt` & `pyxel_sim-1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/PKG-INFO` & `pyxel_sim-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel_sim
-Version: 1.8
+Version: 1.9
 Summary: Pyxel detector simulation framework.
 Author-email: The Pyxel development team <pyxel@esa.int>
 License: MIT
 Project-URL: homepage, https://esa.gitlab.io/pyxel/
 Project-URL: documentation, https://esa.gitlab.io/pyxel/doc/
 Project-URL: repository, https://gitlab.com/esa/pyxel
 Project-URL: changelog, https://gitlab.com/esa/pyxel/-/releases
@@ -13,22 +13,22 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: calibration
 Provides-Extra: model
 Provides-Extra: io
 Provides-Extra: all
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
@@ -53,15 +53,15 @@
 ## What is it?
 
 *Pyxel* is a general detector simulation framework.
 An easy-to-use framework that can simulate a variety of imaging detector
 effects combined on images (e.g. radiation and optical effects, noises)
 made by CCD or CMOS-based detectors.
 
-*Pyxel* is tested on Python 3.8+.
+*Pyxel* is tested on Python 3.9+.
 
 If you'd like to contribute to *Pyxel* you're most welcome.
 Please read [the little guide](https://esa.gitlab.io/pyxel/doc/stable/references/contributing.html) to get you started.
 
 ## Documentation
 
 Learn more about *Pyxel* in its offical [blog](https://esa.gitlab.io/pyxel) and its official documentation at [https://esa.gitlab.io/pyxel/doc](https://esa.gitlab.io/pyxel/doc).
```

### Comparing `pyxel_sim-1.8/README.md` & `pyxel_sim-1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 ## What is it?
 
 *Pyxel* is a general detector simulation framework.
 An easy-to-use framework that can simulate a variety of imaging detector
 effects combined on images (e.g. radiation and optical effects, noises)
 made by CCD or CMOS-based detectors.
 
-*Pyxel* is tested on Python 3.8+.
+*Pyxel* is tested on Python 3.9+.
 
 If you'd like to contribute to *Pyxel* you're most welcome.
 Please read [the little guide](https://esa.gitlab.io/pyxel/doc/stable/references/contributing.html) to get you started.
 
 ## Documentation
 
 Learn more about *Pyxel* in its offical [blog](https://esa.gitlab.io/pyxel) and its official documentation at [https://esa.gitlab.io/pyxel/doc](https://esa.gitlab.io/pyxel/doc).
```

### Comparing `pyxel_sim-1.8/continuous_integration/scripts/auto_generated.py` & `pyxel_sim-1.9/continuous_integration/scripts/auto_generated.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,52 +6,56 @@
 #  the terms contained in the file ‘LICENCE.txt’.
 
 ######################################
 # Note: This code is auto-generated. #
 #       Don't modify it !            #
 ######################################
 
+import collections
 import json
 import pathlib
 import sys
 from dataclasses import dataclass, field
 from pathlib import Path
 from pprint import pprint
 from typing import Any, Iterator, Literal, Mapping, Optional, Sequence, Tuple, Union
 
 import click
 from apischema import schema
 from apischema.json_schema import JsonSchemaVersion, deserialization_schema
 
 
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelLoadSaveDetectorArguments(Mapping[str, Any]):
     filename: float = field(
-    metadata=schema(title='filename', description='Filename to load/save.')
-)
+        metadata=schema(title="filename", description="Filename to load/save.")
+    )
+
 
 @dataclass
 class ModelLoadDetector:
     name: str
     arguments: ModelLoadSaveDetectorArguments
-    func: Literal['pyxel.models.load_detector'] = 'pyxel.models.load_detector'
+    func: Literal["pyxel.models.load_detector"] = "pyxel.models.load_detector"
     enabled: bool = True
 
+
 @dataclass
 class ModelSaveDetector:
     name: str
     arguments: ModelLoadSaveDetectorArguments
-    func: Literal['pyxel.models.save_detector'] = 'pyxel.models.save_detector'
+    func: Literal["pyxel.models.save_detector"] = "pyxel.models.save_detector"
     enabled: bool = True
 
+
 @dataclass
 class ModelFunction:
     name: str
-    func: str = field(metadata=schema(pattern='^(?!pyxel\.models\.)'))
+    func: str = field(metadata=schema(pattern="^(?!pyxel\.models\.)"))
     arguments: Optional[Mapping[str, Any]] = None
     enabled: bool = True
 
 
 @dataclass
 class ModelGroup:
     models: Sequence[ModelFunction]
@@ -73,3713 +77,4004 @@
     readout_electronics: Optional[Sequence[ModelFunction]] = None
     data_processing: Optional[Sequence[ModelFunction]] = None
 
 
 #
 # Model: Photon Collection / Illumination
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhotonCollectionIlluminationArguments(Mapping[str, Any]):
     level: float = field(
-        metadata=schema(
-            title='level'
-            ,description='Flux of photon per pixel.'
-        )
+        metadata=schema(title="level", description="Flux of photon per pixel.")
     )
-    option: Literal['uniform', 'rectangular', 'elliptic'] = field(
-        default='uniform',
+    option: Literal["uniform", "rectangular", "elliptic"] = field(
+        default="uniform",
         metadata=schema(
-            title='option'
-            ,description=(
-                    'A string indicating the type of illumination: - ``uniform`` Uniformly'
-                    'fill the entire array with photon. (Default) - ``elliptic`` Mask with'
-                    'elliptic object. - ``rectangular`` Mask with rectangular object.'
-                )
-        )
+            title="option",
+            description=(
+                "A string indicating the type of illumination: - ``uniform`` Uniformly"
+                "fill the entire array with photon. (Default) - ``elliptic`` Mask with"
+                "elliptic object. - ``rectangular`` Mask with rectangular object."
+            ),
+        ),
     )
-    object_size: Optional[Sequence[int]] = field(
+    object_size: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
-            title='object_size'
-            ,description=(
-                    'List or tuple of length 2, integers defining the diameters of the'
-                    'elliptic or rectangular object in vertical and horizontal directions.'
-                )
-        )
+            title="object_size",
+            description=(
+                "List or tuple of length 2, integers defining the diameters of the"
+                "elliptic or rectangular object in vertical and horizontal directions."
+            ),
+        ),
     )
-    object_center: Optional[Sequence[int]] = field(
+    object_center: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
-            title='object_center'
-            ,description=(
-                    'List or tuple of length 2, two integers (row and column number),'
-                    'defining the coordinates of the center of the elliptic or rectangular'
-                    'object.'
-                )
-        )
+            title="object_center",
+            description=(
+                "List or tuple of length 2, two integers (row and column number),"
+                "defining the coordinates of the center of the elliptic or rectangular"
+                "object."
+            ),
+        ),
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title='time_scale'
-            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
-        )
+            title="time_scale",
+            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('level', 'option', 'object_size', 'object_center', 'time_scale'))
+        return iter(("level", "option", "object_size", "object_center", "time_scale"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'illumination'"
-    ,description=(
-        'Generate photon uniformly over the entire array or over an elliptic or'
-        'rectangular object.'
-    )
+    title="Model 'illumination'",
+    description=(
+        "Generate photon uniformly over the entire array or over an elliptic or"
+        "rectangular object."
+    ),
 )
 @dataclass
 class ModelPhotonCollectionIllumination:
     name: str
     arguments: ModelPhotonCollectionIlluminationArguments
-    func: Literal['pyxel.models.photon_collection.illumination'] = 'pyxel.models.photon_collection.illumination'
+    func: Literal[
+        "pyxel.models.photon_collection.illumination"
+    ] = "pyxel.models.photon_collection.illumination"
     enabled: bool = True
 
 
 #
 # Model: Photon Collection / Load Image
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhotonCollectionLoadImageArguments(Mapping[str, Any]):
     image_file: str = field(
-        metadata=schema(
-            title='image_file'
-            ,description='Path to image file.'
-        )
+        metadata=schema(title="image_file", description="Path to image file.")
     )
-    position: Tuple[int, int] = field(
+    position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title='position'
-            ,description=(
-                    'Indices of starting row and column, used when fitting image to'
-                    'detector.'
-                )
-        )
+            title="position",
+            description=(
+                "Indices of starting row and column, used when fitting image to"
+                "detector."
+            ),
+        ),
     )
-    align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
+    align: Optional[
+        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
+    ] = field(
         default=None,
         metadata=schema(
-            title='align'
-            ,description=(
-                    'Keyword to align the image to detector. Can be any from: ("center",'
-                    '"top_left", "top_right", "bottom_left", "bottom_right")'
-                )
-        )
+            title="align",
+            description=(
+                'Keyword to align the image to detector. Can be any from: ("center",'
+                '"top_left", "top_right", "bottom_left", "bottom_right")'
+            ),
+        ),
     )
     convert_to_photons: bool = field(
         default=False,
         metadata=schema(
-            title='convert_to_photons'
-            ,description=(
-                    'If ``True``, the model converts the values of loaded image array from'
-                    'ADU to photon numbers for each pixel using the Photon Transfer'
-                    'Function: :math:`\\mathit{PTF} = \\mathit{quantum\\_efficiency} \\cdot'
-                    '\\mathit{charge\\_to\\_voltage\\_conversion} \\cdot'
-                    '\\mathit{pre\\_amplification} \\cdot \\mathit{adc\\_factor}`.'
-                )
-        )
+            title="convert_to_photons",
+            description=(
+                "If ``True``, the model converts the values of loaded image array from"
+                "ADU to photon numbers for each pixel using the Photon Transfer"
+                "Function: :math:`\\mathit{PTF} = \\mathit{quantum\\_efficiency} \\cdot"
+                "\\mathit{charge\\_to\\_voltage\\_conversion} \\cdot"
+                "\\mathit{pre\\_amplification} \\cdot \\mathit{adc\\_factor}`."
+            ),
+        ),
     )
     multiplier: float = field(
         default=1.0,
         metadata=schema(
-            title='multiplier'
-            ,description='Multiply photon array level with a custom number.'
-        )
+            title="multiplier",
+            description="Multiply photon array level with a custom number.",
+        ),
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title='time_scale'
-            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
-        )
+            title="time_scale",
+            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
+        ),
     )
     bit_resolution: Optional[int] = field(
         default=None,
         metadata=schema(
-            title='bit_resolution'
-            ,description='Bit resolution of the loaded image.'
-        )
+            title="bit_resolution", description="Bit resolution of the loaded image."
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('image_file', 'position', 'align', 'convert_to_photons', 'multiplier', 'time_scale', 'bit_resolution'))
+        return iter(
+            (
+                "image_file",
+                "position",
+                "align",
+                "convert_to_photons",
+                "multiplier",
+                "time_scale",
+                "bit_resolution",
+            )
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 7
 
 
 @schema(
-    title="Model 'load_image'"
-    ,description=(
-        'Load :term:`FITS` file as a numpy array and add to the detector as'
-        'input image.'
-    )
+    title="Model 'load_image'",
+    description=(
+        "Load :term:`FITS` file as a numpy array and add to the detector as"
+        "input image."
+    ),
 )
 @dataclass
 class ModelPhotonCollectionLoadImage:
     name: str
     arguments: ModelPhotonCollectionLoadImageArguments
-    func: Literal['pyxel.models.photon_collection.load_image'] = 'pyxel.models.photon_collection.load_image'
+    func: Literal[
+        "pyxel.models.photon_collection.load_image"
+    ] = "pyxel.models.photon_collection.load_image"
     enabled: bool = True
 
 
 #
 # Model: Photon Collection / Load Psf
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhotonCollectionLoadPsfArguments(Mapping[str, Any]):
     filename: Union[str, pathlib.Path] = field(
         metadata=schema(
-            title='filename'
-            ,description='Input filename of the point spread function.'
+            title="filename", description="Input filename of the point spread function."
         )
     )
     normalize_kernel: bool = field(
         default=True,
-        metadata=schema(
-            title='normalize_kernel'
-            ,description='Normalize kernel.'
-        )
+        metadata=schema(title="normalize_kernel", description="Normalize kernel."),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('filename', 'normalize_kernel'))
+        return iter(("filename", "normalize_kernel"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'load_psf'"
-    ,description=(
-        'Load a point spread function from file and convolve the photon array'
-        'with the PSF.'
-    )
+    title="Model 'load_psf'",
+    description=(
+        "Load a point spread function from file and convolve the photon array"
+        "with the PSF."
+    ),
 )
 @dataclass
 class ModelPhotonCollectionLoadPsf:
     name: str
     arguments: ModelPhotonCollectionLoadPsfArguments
-    func: Literal['pyxel.models.photon_collection.load_psf'] = 'pyxel.models.photon_collection.load_psf'
+    func: Literal[
+        "pyxel.models.photon_collection.load_psf"
+    ] = "pyxel.models.photon_collection.load_psf"
     enabled: bool = True
 
 
 #
 # Model: Photon Collection / Optical Psf
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhotonCollectionOpticalPsfArguments(Mapping[str, Any]):
     wavelength: float = field(
         metadata=schema(
-            title='wavelength'
-            ,description='Wavelength of incoming light in meters.'
+            title="wavelength", description="Wavelength of incoming light in meters."
         )
     )
     fov_arcsec: float = field(
         metadata=schema(
-            title='fov_arcsec'
-            ,description='Field Of View on detector plane in arcsec.'
+            title="fov_arcsec", description="Field Of View on detector plane in arcsec."
         )
     )
     pixelscale: float = field(
         metadata=schema(
-            title='pixelscale'
-            ,description=(
-                    'Pixel scale on detector plane (arcsec/pixel). Defines sampling'
-                    'resolution of :term:`PSF`.'
-                )
+            title="pixelscale",
+            description=(
+                "Pixel scale on detector plane (arcsec/pixel). Defines sampling"
+                "resolution of :term:`PSF`."
+            ),
         )
     )
-    optical_system: Sequence[Mapping[str, Any]] = field(
+    optical_system: collections.abc.Sequence[collections.abc.Mapping[str, Any]] = field(
         metadata=schema(
-            title='optical_system'
-            ,description=(
-                    'List of optical elements before detector with their specific'
-                    'arguments.'
-                )
+            title="optical_system",
+            description=(
+                "List of optical elements before detector with their specific"
+                "arguments."
+            ),
         )
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('wavelength', 'fov_arcsec', 'pixelscale', 'optical_system'))
+        return iter(("wavelength", "fov_arcsec", "pixelscale", "optical_system"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 4
 
 
 @schema(
-    title="Model 'optical_psf'"
-    ,description='Model function for poppy optics model: convolve photon array with psf.'
+    title="Model 'optical_psf'",
+    description="Model function for poppy optics model: convolve photon array with psf.",
 )
 @dataclass
 class ModelPhotonCollectionOpticalPsf:
     name: str
     arguments: ModelPhotonCollectionOpticalPsfArguments
-    func: Literal['pyxel.models.photon_collection.optical_psf'] = 'pyxel.models.photon_collection.optical_psf'
+    func: Literal[
+        "pyxel.models.photon_collection.optical_psf"
+    ] = "pyxel.models.photon_collection.optical_psf"
     enabled: bool = True
 
 
 #
 # Model: Photon Collection / Shot Noise
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhotonCollectionShotNoiseArguments(Mapping[str, Any]):
-    type: Literal['poisson', 'normal'] = field(
-        default='poisson',
+    type: Literal["poisson", "normal"] = field(
+        default="poisson",
         metadata=schema(
-            title='type'
-            ,description="Choose either 'poisson' or 'normal'. Default is Poisson noise."
-        )
+            title="type",
+            description="Choose either 'poisson' or 'normal'. Default is Poisson noise.",
+        ),
     )
     seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-            ,description='Random seed.'
-        )
+        default=None, metadata=schema(title="seed", description="Random seed.")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('type', 'seed'))
+        return iter(("type", "seed"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'shot_noise'"
-    ,description=(
-        'Add shot noise to the flux of photon per pixel. It can be either'
-        'Poisson noise or Gaussian.'
-    )
+    title="Model 'shot_noise'",
+    description=(
+        "Add shot noise to the flux of photon per pixel. It can be either"
+        "Poisson noise or Gaussian."
+    ),
 )
 @dataclass
 class ModelPhotonCollectionShotNoise:
     name: str
-    arguments: ModelPhotonCollectionShotNoiseArguments = field(default_factory=ModelPhotonCollectionShotNoiseArguments)
-    func: Literal['pyxel.models.photon_collection.shot_noise'] = 'pyxel.models.photon_collection.shot_noise'
+    arguments: ModelPhotonCollectionShotNoiseArguments = field(
+        default_factory=ModelPhotonCollectionShotNoiseArguments
+    )
+    func: Literal[
+        "pyxel.models.photon_collection.shot_noise"
+    ] = "pyxel.models.photon_collection.shot_noise"
     enabled: bool = True
 
 
 #
 # Model: Photon Collection / Stripe Pattern
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhotonCollectionStripePatternArguments(Mapping[str, Any]):
     period: int = field(
         default=10,
         metadata=schema(
-            title='period'
-            ,description='Period of the periodic pattern in pixels.'
-        )
+            title="period", description="Period of the periodic pattern in pixels."
+        ),
     )
     level: float = field(
         default=1.0,
         metadata=schema(
-            title='level'
-            ,description='Amplitude of the periodic pattern.'
-        )
+            title="level", description="Amplitude of the periodic pattern."
+        ),
     )
     angle: int = field(
         default=0,
-        metadata=schema(
-            title='angle'
-            ,description='Angle of the pattern in degrees.'
-        )
+        metadata=schema(title="angle", description="Angle of the pattern in degrees."),
     )
     startwith: int = field(
         default=0,
         metadata=schema(
-            title='startwith'
-            ,description='1 to start with high level or 0 for 0.'
-        )
+            title="startwith", description="1 to start with high level or 0 for 0."
+        ),
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title='time_scale'
-            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
-        )
+            title="time_scale",
+            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('period', 'level', 'angle', 'startwith', 'time_scale'))
+        return iter(("period", "level", "angle", "startwith", "time_scale"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 5
 
 
-@schema(
-    title="Model 'stripe_pattern'"
-    ,description='Stripe pattern model.'
-)
+@schema(title="Model 'stripe_pattern'", description="Stripe pattern model.")
 @dataclass
 class ModelPhotonCollectionStripePattern:
     name: str
-    arguments: ModelPhotonCollectionStripePatternArguments = field(default_factory=ModelPhotonCollectionStripePatternArguments)
-    func: Literal['pyxel.models.photon_collection.stripe_pattern'] = 'pyxel.models.photon_collection.stripe_pattern'
+    arguments: ModelPhotonCollectionStripePatternArguments = field(
+        default_factory=ModelPhotonCollectionStripePatternArguments
+    )
+    func: Literal[
+        "pyxel.models.photon_collection.stripe_pattern"
+    ] = "pyxel.models.photon_collection.stripe_pattern"
     enabled: bool = True
 
 
 #
 # Model: Photon Generation / Illumination
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhotonGenerationIlluminationArguments(Mapping[str, Any]):
     level: float = field(
-        metadata=schema(
-            title='level'
-            ,description='Flux of photon per pixel.'
-        )
+        metadata=schema(title="level", description="Flux of photon per pixel.")
     )
-    option: Literal['uniform', 'rectangular', 'elliptic'] = field(
-        default='uniform',
+    option: Literal["uniform", "rectangular", "elliptic"] = field(
+        default="uniform",
         metadata=schema(
-            title='option'
-            ,description=(
-                    'A string indicating the type of illumination: - ``uniform`` Uniformly'
-                    'fill the entire array with photon. (Default) - ``elliptic`` Mask with'
-                    'elliptic object. - ``rectangular`` Mask with rectangular object.'
-                )
-        )
+            title="option",
+            description=(
+                "A string indicating the type of illumination: - ``uniform`` Uniformly"
+                "fill the entire array with photon. (Default) - ``elliptic`` Mask with"
+                "elliptic object. - ``rectangular`` Mask with rectangular object."
+            ),
+        ),
     )
-    object_size: Optional[Sequence[int]] = field(
+    object_size: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
-            title='object_size'
-            ,description=(
-                    'List or tuple of length 2, integers defining the diameters of the'
-                    'elliptic or rectangular object in vertical and horizontal directions.'
-                )
-        )
+            title="object_size",
+            description=(
+                "List or tuple of length 2, integers defining the diameters of the"
+                "elliptic or rectangular object in vertical and horizontal directions."
+            ),
+        ),
     )
-    object_center: Optional[Sequence[int]] = field(
+    object_center: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
-            title='object_center'
-            ,description=(
-                    'List or tuple of length 2, two integers (row and column number),'
-                    'defining the coordinates of the center of the elliptic or rectangular'
-                    'object.'
-                )
-        )
+            title="object_center",
+            description=(
+                "List or tuple of length 2, two integers (row and column number),"
+                "defining the coordinates of the center of the elliptic or rectangular"
+                "object."
+            ),
+        ),
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title='time_scale'
-            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
-        )
+            title="time_scale",
+            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('level', 'option', 'object_size', 'object_center', 'time_scale'))
+        return iter(("level", "option", "object_size", "object_center", "time_scale"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'illumination'"
-    ,description=(
-        'Generate photon uniformly over the entire array or over an elliptic or'
-        'rectangular object.'
-    )
+    title="Model 'illumination'",
+    description=(
+        "Generate photon uniformly over the entire array or over an elliptic or"
+        "rectangular object."
+    ),
 )
 @dataclass
 class ModelPhotonGenerationIllumination:
     name: str
     arguments: ModelPhotonGenerationIlluminationArguments
-    func: Literal['pyxel.models.photon_generation.illumination'] = 'pyxel.models.photon_generation.illumination'
+    func: Literal[
+        "pyxel.models.photon_generation.illumination"
+    ] = "pyxel.models.photon_generation.illumination"
     enabled: bool = True
 
 
 #
 # Model: Photon Generation / Load Image
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhotonGenerationLoadImageArguments(Mapping[str, Any]):
     image_file: str = field(
-        metadata=schema(
-            title='image_file'
-            ,description='Path to image file.'
-        )
+        metadata=schema(title="image_file", description="Path to image file.")
     )
-    position: Tuple[int, int] = field(
+    position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title='position'
-            ,description=(
-                    'Indices of starting row and column, used when fitting image to'
-                    'detector.'
-                )
-        )
+            title="position",
+            description=(
+                "Indices of starting row and column, used when fitting image to"
+                "detector."
+            ),
+        ),
     )
-    align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
+    align: Optional[
+        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
+    ] = field(
         default=None,
         metadata=schema(
-            title='align'
-            ,description=(
-                    'Keyword to align the image to detector. Can be any from: ("center",'
-                    '"top_left", "top_right", "bottom_left", "bottom_right")'
-                )
-        )
+            title="align",
+            description=(
+                'Keyword to align the image to detector. Can be any from: ("center",'
+                '"top_left", "top_right", "bottom_left", "bottom_right")'
+            ),
+        ),
     )
     convert_to_photons: bool = field(
         default=False,
         metadata=schema(
-            title='convert_to_photons'
-            ,description=(
-                    'If ``True``, the model converts the values of loaded image array from'
-                    'ADU to photon numbers for each pixel using the Photon Transfer'
-                    'Function: :math:`\\mathit{PTF} = \\mathit{quantum\\_efficiency} \\cdot'
-                    '\\mathit{charge\\_to\\_voltage\\_conversion} \\cdot'
-                    '\\mathit{pre\\_amplification} \\cdot \\mathit{adc\\_factor}`.'
-                )
-        )
+            title="convert_to_photons",
+            description=(
+                "If ``True``, the model converts the values of loaded image array from"
+                "ADU to photon numbers for each pixel using the Photon Transfer"
+                "Function: :math:`\\mathit{PTF} = \\mathit{quantum\\_efficiency} \\cdot"
+                "\\mathit{charge\\_to\\_voltage\\_conversion} \\cdot"
+                "\\mathit{pre\\_amplification} \\cdot \\mathit{adc\\_factor}`."
+            ),
+        ),
     )
     multiplier: float = field(
         default=1.0,
         metadata=schema(
-            title='multiplier'
-            ,description='Multiply photon array level with a custom number.'
-        )
+            title="multiplier",
+            description="Multiply photon array level with a custom number.",
+        ),
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title='time_scale'
-            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
-        )
+            title="time_scale",
+            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
+        ),
     )
     bit_resolution: Optional[int] = field(
         default=None,
         metadata=schema(
-            title='bit_resolution'
-            ,description='Bit resolution of the loaded image.'
-        )
+            title="bit_resolution", description="Bit resolution of the loaded image."
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('image_file', 'position', 'align', 'convert_to_photons', 'multiplier', 'time_scale', 'bit_resolution'))
+        return iter(
+            (
+                "image_file",
+                "position",
+                "align",
+                "convert_to_photons",
+                "multiplier",
+                "time_scale",
+                "bit_resolution",
+            )
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 7
 
 
 @schema(
-    title="Model 'load_image'"
-    ,description=(
-        'Load :term:`FITS` file as a numpy array and add to the detector as'
-        'input image.'
-    )
+    title="Model 'load_image'",
+    description=(
+        "Load :term:`FITS` file as a numpy array and add to the detector as"
+        "input image."
+    ),
 )
 @dataclass
 class ModelPhotonGenerationLoadImage:
     name: str
     arguments: ModelPhotonGenerationLoadImageArguments
-    func: Literal['pyxel.models.photon_generation.load_image'] = 'pyxel.models.photon_generation.load_image'
+    func: Literal[
+        "pyxel.models.photon_generation.load_image"
+    ] = "pyxel.models.photon_generation.load_image"
     enabled: bool = True
 
 
 #
 # Model: Photon Generation / Shot Noise
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhotonGenerationShotNoiseArguments(Mapping[str, Any]):
-    type: Literal['poisson', 'normal'] = field(
-        default='poisson',
+    type: Literal["poisson", "normal"] = field(
+        default="poisson",
         metadata=schema(
-            title='type'
-            ,description="Choose either 'poisson' or 'normal'. Default is Poisson noise."
-        )
+            title="type",
+            description="Choose either 'poisson' or 'normal'. Default is Poisson noise.",
+        ),
     )
     seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-            ,description='Random seed.'
-        )
+        default=None, metadata=schema(title="seed", description="Random seed.")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('type', 'seed'))
+        return iter(("type", "seed"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'shot_noise'"
-    ,description=(
-        'Add shot noise to the flux of photon per pixel. It can be either'
-        'Poisson noise or Gaussian.'
-    )
+    title="Model 'shot_noise'",
+    description=(
+        "Add shot noise to the flux of photon per pixel. It can be either"
+        "Poisson noise or Gaussian."
+    ),
 )
 @dataclass
 class ModelPhotonGenerationShotNoise:
     name: str
-    arguments: ModelPhotonGenerationShotNoiseArguments = field(default_factory=ModelPhotonGenerationShotNoiseArguments)
-    func: Literal['pyxel.models.photon_generation.shot_noise'] = 'pyxel.models.photon_generation.shot_noise'
+    arguments: ModelPhotonGenerationShotNoiseArguments = field(
+        default_factory=ModelPhotonGenerationShotNoiseArguments
+    )
+    func: Literal[
+        "pyxel.models.photon_generation.shot_noise"
+    ] = "pyxel.models.photon_generation.shot_noise"
     enabled: bool = True
 
 
 #
 # Model: Photon Generation / Stripe Pattern
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhotonGenerationStripePatternArguments(Mapping[str, Any]):
     period: int = field(
         default=10,
         metadata=schema(
-            title='period'
-            ,description='Period of the periodic pattern in pixels.'
-        )
+            title="period", description="Period of the periodic pattern in pixels."
+        ),
     )
     level: float = field(
         default=1.0,
         metadata=schema(
-            title='level'
-            ,description='Amplitude of the periodic pattern.'
-        )
+            title="level", description="Amplitude of the periodic pattern."
+        ),
     )
     angle: int = field(
         default=0,
-        metadata=schema(
-            title='angle'
-            ,description='Angle of the pattern in degrees.'
-        )
+        metadata=schema(title="angle", description="Angle of the pattern in degrees."),
     )
     startwith: int = field(
         default=0,
         metadata=schema(
-            title='startwith'
-            ,description='1 to start with high level or 0 for 0.'
-        )
+            title="startwith", description="1 to start with high level or 0 for 0."
+        ),
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title='time_scale'
-            ,description='Time scale of the photon flux, default is 1 second. 0.001 would be ms.'
-        )
+            title="time_scale",
+            description="Time scale of the photon flux, default is 1 second. 0.001 would be ms.",
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('period', 'level', 'angle', 'startwith', 'time_scale'))
+        return iter(("period", "level", "angle", "startwith", "time_scale"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 5
 
 
-@schema(
-    title="Model 'stripe_pattern'"
-    ,description='Stripe pattern model.'
-)
+@schema(title="Model 'stripe_pattern'", description="Stripe pattern model.")
 @dataclass
 class ModelPhotonGenerationStripePattern:
     name: str
-    arguments: ModelPhotonGenerationStripePatternArguments = field(default_factory=ModelPhotonGenerationStripePatternArguments)
-    func: Literal['pyxel.models.photon_generation.stripe_pattern'] = 'pyxel.models.photon_generation.stripe_pattern'
+    arguments: ModelPhotonGenerationStripePatternArguments = field(
+        default_factory=ModelPhotonGenerationStripePatternArguments
+    )
+    func: Literal[
+        "pyxel.models.photon_generation.stripe_pattern"
+    ] = "pyxel.models.photon_generation.stripe_pattern"
     enabled: bool = True
 
 
 #
 # Model: Optics / Load Psf
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelOpticsLoadPsfArguments(Mapping[str, Any]):
     filename: Union[str, pathlib.Path] = field(
         metadata=schema(
-            title='filename'
-            ,description='Input filename of the point spread function.'
+            title="filename", description="Input filename of the point spread function."
         )
     )
     normalize_kernel: bool = field(
         default=True,
-        metadata=schema(
-            title='normalize_kernel'
-            ,description='Normalize kernel.'
-        )
+        metadata=schema(title="normalize_kernel", description="Normalize kernel."),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('filename', 'normalize_kernel'))
+        return iter(("filename", "normalize_kernel"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'load_psf'"
-    ,description=(
-        'Load a point spread function from file and convolve the photon array'
-        'with the PSF.'
-    )
+    title="Model 'load_psf'",
+    description=(
+        "Load a point spread function from file and convolve the photon array"
+        "with the PSF."
+    ),
 )
 @dataclass
 class ModelOpticsLoadPsf:
     name: str
     arguments: ModelOpticsLoadPsfArguments
-    func: Literal['pyxel.models.optics.load_psf'] = 'pyxel.models.optics.load_psf'
+    func: Literal["pyxel.models.optics.load_psf"] = "pyxel.models.optics.load_psf"
     enabled: bool = True
 
 
 #
 # Model: Optics / Optical Psf
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelOpticsOpticalPsfArguments(Mapping[str, Any]):
     wavelength: float = field(
         metadata=schema(
-            title='wavelength'
-            ,description='Wavelength of incoming light in meters.'
+            title="wavelength", description="Wavelength of incoming light in meters."
         )
     )
     fov_arcsec: float = field(
         metadata=schema(
-            title='fov_arcsec'
-            ,description='Field Of View on detector plane in arcsec.'
+            title="fov_arcsec", description="Field Of View on detector plane in arcsec."
         )
     )
     pixelscale: float = field(
         metadata=schema(
-            title='pixelscale'
-            ,description=(
-                    'Pixel scale on detector plane (arcsec/pixel). Defines sampling'
-                    'resolution of :term:`PSF`.'
-                )
+            title="pixelscale",
+            description=(
+                "Pixel scale on detector plane (arcsec/pixel). Defines sampling"
+                "resolution of :term:`PSF`."
+            ),
         )
     )
-    optical_system: Sequence[Mapping[str, Any]] = field(
+    optical_system: collections.abc.Sequence[collections.abc.Mapping[str, Any]] = field(
         metadata=schema(
-            title='optical_system'
-            ,description=(
-                    'List of optical elements before detector with their specific'
-                    'arguments.'
-                )
+            title="optical_system",
+            description=(
+                "List of optical elements before detector with their specific"
+                "arguments."
+            ),
         )
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('wavelength', 'fov_arcsec', 'pixelscale', 'optical_system'))
+        return iter(("wavelength", "fov_arcsec", "pixelscale", "optical_system"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 4
 
 
 @schema(
-    title="Model 'optical_psf'"
-    ,description='Model function for poppy optics model: convolve photon array with psf.'
+    title="Model 'optical_psf'",
+    description="Model function for poppy optics model: convolve photon array with psf.",
 )
 @dataclass
 class ModelOpticsOpticalPsf:
     name: str
     arguments: ModelOpticsOpticalPsfArguments
-    func: Literal['pyxel.models.optics.optical_psf'] = 'pyxel.models.optics.optical_psf'
+    func: Literal["pyxel.models.optics.optical_psf"] = "pyxel.models.optics.optical_psf"
     enabled: bool = True
 
 
 #
 # Model: Phasing / Pulse Processing
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelPhasingPulseProcessingArguments(Mapping[str, Any]):
     wavelength: float = field(
-        metadata=schema(
-            title='wavelength'
-            ,description='Wavelength.'
-        )
+        metadata=schema(title="wavelength", description="Wavelength.")
     )
     responsivity: float = field(
-        metadata=schema(
-            title='responsivity'
-            ,description='Responsivity of the pixel.'
-        )
+        metadata=schema(title="responsivity", description="Responsivity of the pixel.")
     )
     scaling_factor: float = field(
         default=250.0,
         metadata=schema(
-            title='scaling_factor'
-            ,description=(
-                    'Scaling factor taking into account the missing pieces of'
-                    'superconducting physics, as well as the resonator quality factor, the'
-                    'bias power, the quasi-particle losses, etc.'
-                )
-        )
+            title="scaling_factor",
+            description=(
+                "Scaling factor taking into account the missing pieces of"
+                "superconducting physics, as well as the resonator quality factor, the"
+                "bias power, the quasi-particle losses, etc."
+            ),
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('wavelength', 'responsivity', 'scaling_factor'))
+        return iter(("wavelength", "responsivity", "scaling_factor"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 3
 
 
-@schema(
-    title="Model 'pulse_processing'"
-    ,description='TBW.'
-)
+@schema(title="Model 'pulse_processing'", description="TBW.")
 @dataclass
 class ModelPhasingPulseProcessing:
     name: str
     arguments: ModelPhasingPulseProcessingArguments
-    func: Literal['pyxel.models.phasing.pulse_processing'] = 'pyxel.models.phasing.pulse_processing'
+    func: Literal[
+        "pyxel.models.phasing.pulse_processing"
+    ] = "pyxel.models.phasing.pulse_processing"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Apd Gain
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationApdGainArguments(Mapping[str, Any]):
     def __iter__(self) -> Iterator[str]:
         return iter(())
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 0
 
 
-@schema(
-    title="Model 'apd_gain'"
-    ,description='Apply APD gain.'
-)
+@schema(title="Model 'apd_gain'", description="Apply APD gain.")
 @dataclass
 class ModelChargeGenerationApdGain:
     name: str
-    arguments: ModelChargeGenerationApdGainArguments = field(default_factory=ModelChargeGenerationApdGainArguments)
-    func: Literal['pyxel.models.charge_generation.apd_gain'] = 'pyxel.models.charge_generation.apd_gain'
+    arguments: ModelChargeGenerationApdGainArguments = field(
+        default_factory=ModelChargeGenerationApdGainArguments
+    )
+    func: Literal[
+        "pyxel.models.charge_generation.apd_gain"
+    ] = "pyxel.models.charge_generation.apd_gain"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Charge Blocks
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationChargeBlocksArguments(Mapping[str, Any]):
     charge_level: float = field(
-        metadata=schema(
-            title='charge_level'
-            ,description='Value of charges.'
-        )
+        metadata=schema(title="charge_level", description="Value of charges.")
     )
     block_start: int = field(
         default=0,
         metadata=schema(
-            title='block_start'
-            ,description='Starting row of the injected charge.'
-        )
+            title="block_start", description="Starting row of the injected charge."
+        ),
     )
     block_end: Optional[int] = field(
         default=None,
         metadata=schema(
-            title='block_end'
-            ,description='Ending row for the injected charge.'
-        )
+            title="block_end", description="Ending row for the injected charge."
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('charge_level', 'block_start', 'block_end'))
+        return iter(("charge_level", "block_start", "block_end"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'charge_blocks'"
-    ,description='Inject a block of charge into the :term:`CCD` detector.'
+    title="Model 'charge_blocks'",
+    description="Inject a block of charge into the :term:`CCD` detector.",
 )
 @dataclass
 class ModelChargeGenerationChargeBlocks:
     name: str
     arguments: ModelChargeGenerationChargeBlocksArguments
-    func: Literal['pyxel.models.charge_generation.charge_blocks'] = 'pyxel.models.charge_generation.charge_blocks'
+    func: Literal[
+        "pyxel.models.charge_generation.charge_blocks"
+    ] = "pyxel.models.charge_generation.charge_blocks"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Charge Deposition
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationChargeDepositionArguments(Mapping[str, Any]):
     flux: float = field(
         metadata=schema(
-            title='flux'
-            ,description='the flux of incoming particles in particle/s'
+            title="flux", description="the flux of incoming particles in particle/s"
         )
     )
     step_size: float = field(
         default=1.0,
         metadata=schema(
-            title='step_size'
-            ,description=(
-                    'the size of the considered unitary step in unit length along which'
-                    'energy is deposited'
-                )
-        )
+            title="step_size",
+            description=(
+                "the size of the considered unitary step in unit length along which"
+                "energy is deposited"
+            ),
+        ),
     )
     energy_mean: float = field(
         default=1.0,
         metadata=schema(
-            title='energy_mean'
-            ,description='the mean energy of the incoming ionizing particles in MeV'
-        )
+            title="energy_mean",
+            description="the mean energy of the incoming ionizing particles in MeV",
+        ),
     )
     energy_spread: float = field(
         default=0.1,
         metadata=schema(
-            title='energy_spread'
-            ,description='the spread in energy of the incoming ionizing particles in MeV'
-        )
+            title="energy_spread",
+            description="the spread in energy of the incoming ionizing particles in MeV",
+        ),
     )
     energy_spectrum: Union[str, pathlib.Path, None] = field(
         default=None,
         metadata=schema(
-            title='energy_spectrum'
-            ,description=(
-                    'the location of the file describing the energy spectrum of incident'
-                    'particles if no spectrum is provided energies are randomly drawn from'
-                    'a normal distribution with mean and spread defined above note that the'
-                    'energy spectrum is assumed to be a txt file with two columns [energy,'
-                    'flux] with the energy in MeV'
-                )
-        )
-    )
-    energy_spectrum_sampling: Optional[Literal['linear', 'log', None]] = field(
-        default='log',
-        metadata=schema(
-            title='energy_spectrum_sampling'
-            ,description=(
-                    '"log" or None: the energy spectrum is sampled in log space "linear" :'
-                    'the energy spectrum is sampled in linear space'
-                )
-        )
+            title="energy_spectrum",
+            description=(
+                "the location of the file describing the energy spectrum of incident"
+                "particles if no spectrum is provided energies are randomly drawn from"
+                "a normal distribution with mean and spread defined above note that the"
+                "energy spectrum is assumed to be a txt file with two columns [energy,"
+                "flux] with the energy in MeV"
+            ),
+        ),
+    )
+    energy_spectrum_sampling: Literal["linear", "log"] = field(
+        default="log",
+        metadata=schema(
+            title="energy_spectrum_sampling",
+            description=(
+                '"log" or None: the energy spectrum is sampled in log space "linear" :'
+                "the energy spectrum is sampled in linear space"
+            ),
+        ),
     )
     ehpair_creation: float = field(
         default=3.65,
         metadata=schema(
-            title='ehpair_creation'
-            ,description=(
-                    'the energy required to generate a electron-hole pair in eV by default'
-                    'the Si value at room temperature is parsed i.e. 3.65 eV'
-                )
-        )
+            title="ehpair_creation",
+            description=(
+                "the energy required to generate a electron-hole pair in eV by default"
+                "the Si value at room temperature is parsed i.e. 3.65 eV"
+            ),
+        ),
     )
     material_density: float = field(
         default=2.329,
         metadata=schema(
-            title='material_density'
-            ,description=(
-                    'the material density in g/cm3 by default he Si value at room'
-                    'temperature is parsed i.e. 2.3290 g/cm3'
-                )
-        )
-    )
-    particle_direction: Optional[Literal['isotropic', 'orthogonal', None]] = field(
-        default='isotropic',
-        metadata=schema(
-            title='particle_direction'
-            ,description=(
-                    '"isotropic" : particles are coming from all directions (outside of the'
-                    'sensor) "orthogonal" : particles are coming from the top of the sensor'
-                    '(thickness = 0) and orthogonal to its surface'
-                )
-        )
+            title="material_density",
+            description=(
+                "the material density in g/cm3 by default he Si value at room"
+                "temperature is parsed i.e. 2.3290 g/cm3"
+            ),
+        ),
     )
-    stopping_power_curve: Union[str, pathlib.Path, None] = field(
-        default=None,
+    particle_direction: Literal["isotropic", "orthogonal"] = field(
+        default="isotropic",
         metadata=schema(
-            title='stopping_power_curve'
-            ,description=(
-                    'the location of the file describing the total massive stopping power'
-                    'energetic loss per mass of material and per unit path length versus'
-                    'particle energy note that the the stopping power curve is assumed to'
-                    'be a csv file with two columns [energy, stopping power] energy in MeV,'
-                    'stopping power in MeV cm2/g'
-                )
-        )
+            title="particle_direction",
+            description=(
+                '"isotropic" : particles are coming from all directions (outside of the'
+                'sensor) "orthogonal" : particles are coming from the top of the sensor'
+                "(thickness = 0) and orthogonal to its surface"
+            ),
+        ),
     )
-    seed: Optional[int] = field(
+    stopping_power_curve: Union[str, pathlib.Path, None] = field(
         default=None,
         metadata=schema(
-            title='seed'
+            title="stopping_power_curve",
+            description=(
+                "the location of the file describing the total massive stopping power"
+                "energetic loss per mass of material and per unit path length versus"
+                "particle energy note that the the stopping power curve is assumed to"
+                "be a csv file with two columns [energy, stopping power] energy in MeV,"
+                "stopping power in MeV cm2/g"
+            ),
+        ),
+    )
+    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(
+            (
+                "flux",
+                "step_size",
+                "energy_mean",
+                "energy_spread",
+                "energy_spectrum",
+                "energy_spectrum_sampling",
+                "ehpair_creation",
+                "material_density",
+                "particle_direction",
+                "stopping_power_curve",
+                "seed",
+            )
         )
-    )
-    def __iter__(self) -> Iterator[str]:
-        return iter(('flux', 'step_size', 'energy_mean', 'energy_spread', 'energy_spectrum', 'energy_spectrum_sampling', 'ehpair_creation', 'material_density', 'particle_direction', 'stopping_power_curve', 'seed'))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 11
 
 
 @schema(
-    title="Model 'charge_deposition'"
-    ,description=(
-        'Simulate charge deposition by ionizing particles using a stopping'
-        'power curve.'
-    )
+    title="Model 'charge_deposition'",
+    description=(
+        "Simulate charge deposition by ionizing particles using a stopping"
+        "power curve."
+    ),
 )
 @dataclass
 class ModelChargeGenerationChargeDeposition:
     name: str
     arguments: ModelChargeGenerationChargeDepositionArguments
-    func: Literal['pyxel.models.charge_generation.charge_deposition'] = 'pyxel.models.charge_generation.charge_deposition'
+    func: Literal[
+        "pyxel.models.charge_generation.charge_deposition"
+    ] = "pyxel.models.charge_generation.charge_deposition"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Charge Deposition In Mct
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationChargeDepositionInMctArguments(Mapping[str, Any]):
     flux: float = field(
         metadata=schema(
-            title='flux'
-            ,description='the flux of incoming particles in particle/s'
+            title="flux", description="the flux of incoming particles in particle/s"
         )
     )
     step_size: float = field(
         default=1.0,
         metadata=schema(
-            title='step_size'
-            ,description=(
-                    'the size of the considered unitary step in unit length along which'
-                    'energy is deposited'
-                )
-        )
+            title="step_size",
+            description=(
+                "the size of the considered unitary step in unit length along which"
+                "energy is deposited"
+            ),
+        ),
     )
     energy_mean: float = field(
         default=1.0,
         metadata=schema(
-            title='energy_mean'
-            ,description='the mean energy of the incoming ionizing particles in MeV'
-        )
+            title="energy_mean",
+            description="the mean energy of the incoming ionizing particles in MeV",
+        ),
     )
     energy_spread: float = field(
         default=0.1,
         metadata=schema(
-            title='energy_spread'
-            ,description='the spread in energy of the incoming ionizing particles in MeV'
-        )
+            title="energy_spread",
+            description="the spread in energy of the incoming ionizing particles in MeV",
+        ),
     )
     energy_spectrum: Union[str, pathlib.Path, None] = field(
         default=None,
         metadata=schema(
-            title='energy_spectrum'
-            ,description=(
-                    'the location of the file describing the energy spectrum of incident'
-                    'particles if no spectrum is provided energies are randomly drawn from'
-                    'a normal distribution with mean and spread defined above note that the'
-                    'energy spectrum is assumed to be a txt file with two columns [energy,'
-                    'flux] with the energy in MeV'
-                )
-        )
-    )
-    energy_spectrum_sampling: Optional[Literal['linear', 'log', None]] = field(
-        default='log',
-        metadata=schema(
-            title='energy_spectrum_sampling'
-            ,description=(
-                    '"log" or None: the energy spectrum is sampled in log space "linear" :'
-                    'the energy spectrum is sampled in linear space'
-                )
-        )
+            title="energy_spectrum",
+            description=(
+                "the location of the file describing the energy spectrum of incident"
+                "particles if no spectrum is provided energies are randomly drawn from"
+                "a normal distribution with mean and spread defined above note that the"
+                "energy spectrum is assumed to be a txt file with two columns [energy,"
+                "flux] with the energy in MeV"
+            ),
+        ),
+    )
+    energy_spectrum_sampling: Literal["linear", "log"] = field(
+        default="log",
+        metadata=schema(
+            title="energy_spectrum_sampling",
+            description=(
+                '"log" : the energy spectrum is sampled in log space "linear" : the'
+                "energy spectrum is sampled in linear space"
+            ),
+        ),
     )
     cutoff_wavelength: float = field(
         default=2.5,
         metadata=schema(
-            title='cutoff_wavelength'
-            ,description=(
-                    'the longest wavelength in micrometer at which the QE reaches 50% of'
-                    'its maximum, used to compute the bandgap energy, and the corresponding'
-                    'fraction of cadmium'
-                )
-        )
-    )
-    particle_direction: Optional[Literal['isotropic', 'orthogonal', None]] = field(
-        default='isotropic',
-        metadata=schema(
-            title='particle_direction'
-            ,description=(
-                    '"isotropic" : particles are coming from all directions (outside of the'
-                    'sensor) "orthogonal" : particles are coming from the top of the sensor'
-                    '(thickness = 0) and orthogonal to its surface'
-                )
-        )
+            title="cutoff_wavelength",
+            description=(
+                "the longest wavelength in micrometer at which the QE reaches 50% of"
+                "its maximum, used to compute the bandgap energy, and the corresponding"
+                "fraction of cadmium"
+            ),
+        ),
     )
-    stopping_power_curve: Union[str, pathlib.Path, None] = field(
-        default=None,
+    particle_direction: Literal["isotropic", "orthogonal"] = field(
+        default="isotropic",
         metadata=schema(
-            title='stopping_power_curve'
-            ,description=(
-                    'the location of the file describing the total massive stopping power'
-                    'energetic loss per mass of material and per unit path length versus'
-                    'particle energy note that the the stopping power curve is assumed to'
-                    'be a csv file with two columns [energy, stopping power] energy in MeV,'
-                    'stopping power in MeV cm2/g'
-                )
-        )
+            title="particle_direction",
+            description=(
+                '"isotropic" : particles are coming from all directions (outside of the'
+                'sensor) "orthogonal" : particles are coming from the top of the sensor'
+                "(thickness = 0) and orthogonal to its surface"
+            ),
+        ),
     )
-    seed: Optional[int] = field(
+    stopping_power_curve: Union[str, pathlib.Path, None] = field(
         default=None,
         metadata=schema(
-            title='seed'
+            title="stopping_power_curve",
+            description=(
+                "the location of the file describing the total massive stopping power"
+                "energetic loss per mass of material and per unit path length versus"
+                "particle energy note that the the stopping power curve is assumed to"
+                "be a csv file with two columns [energy, stopping power] energy in MeV,"
+                "stopping power in MeV cm2/g"
+            ),
+        ),
+    )
+    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(
+            (
+                "flux",
+                "step_size",
+                "energy_mean",
+                "energy_spread",
+                "energy_spectrum",
+                "energy_spectrum_sampling",
+                "cutoff_wavelength",
+                "particle_direction",
+                "stopping_power_curve",
+                "seed",
+            )
         )
-    )
-    def __iter__(self) -> Iterator[str]:
-        return iter(('flux', 'step_size', 'energy_mean', 'energy_spread', 'energy_spectrum', 'energy_spectrum_sampling', 'cutoff_wavelength', 'particle_direction', 'stopping_power_curve', 'seed'))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 10
 
 
 @schema(
-    title="Model 'charge_deposition_in_mct'"
-    ,description=(
-        'Simulate charge deposition by ionizing particles using a stopping'
-        'power curve.'
-    )
+    title="Model 'charge_deposition_in_mct'",
+    description=(
+        "Simulate charge deposition by ionizing particles using a stopping"
+        "power curve."
+    ),
 )
 @dataclass
 class ModelChargeGenerationChargeDepositionInMct:
     name: str
     arguments: ModelChargeGenerationChargeDepositionInMctArguments
-    func: Literal['pyxel.models.charge_generation.charge_deposition_in_mct'] = 'pyxel.models.charge_generation.charge_deposition_in_mct'
+    func: Literal[
+        "pyxel.models.charge_generation.charge_deposition_in_mct"
+    ] = "pyxel.models.charge_generation.charge_deposition_in_mct"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Conversion With Qe Map
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationConversionWithQeMapArguments(Mapping[str, Any]):
     filename: Union[str, pathlib.Path] = field(
-        metadata=schema(
-            title='filename'
-            ,description='File path.'
-        )
+        metadata=schema(title="filename", description="File path.")
     )
-    position: Tuple[int, int] = field(
+    position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title='position'
-            ,description=(
-                    'Indices of starting row and column, used when fitting :term:`QE` map'
-                    'to detector.'
-                )
-        )
-    )
-    align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
-        default=None,
-        metadata=schema(
-            title='align'
-            ,description=(
-                    'Keyword to align the :term:`QE` map to detector. Can be any from:'
-                    '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
-                )
-        )
+            title="position",
+            description=(
+                "Indices of starting row and column, used when fitting :term:`QE` map"
+                "to detector."
+            ),
+        ),
     )
-    seed: Optional[int] = field(
+    align: Optional[
+        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
+    ] = field(
         default=None,
         metadata=schema(
-            title='seed'
-        )
+            title="align",
+            description=(
+                "Keyword to align the :term:`QE` map to detector. Can be any from:"
+                '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
+            ),
+        ),
     )
+    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
     binomial_sampling: bool = field(
         default=True,
         metadata=schema(
-            title='binomial_sampling'
-            ,description='Binomial sampling. Default is True.'
-        )
+            title="binomial_sampling", description="Binomial sampling. Default is True."
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('filename', 'position', 'align', 'seed', 'binomial_sampling'))
+        return iter(("filename", "position", "align", "seed", "binomial_sampling"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'conversion_with_qe_map'"
-    ,description=(
-        'Generate charge from incident photon via photoelectric effect, simple'
-        'model with custom :term:`QE` map.'
-    )
+    title="Model 'conversion_with_qe_map'",
+    description=(
+        "Generate charge from incident photon via photoelectric effect, simple"
+        "model with custom :term:`QE` map."
+    ),
 )
 @dataclass
 class ModelChargeGenerationConversionWithQeMap:
     name: str
     arguments: ModelChargeGenerationConversionWithQeMapArguments
-    func: Literal['pyxel.models.charge_generation.conversion_with_qe_map'] = 'pyxel.models.charge_generation.conversion_with_qe_map'
+    func: Literal[
+        "pyxel.models.charge_generation.conversion_with_qe_map"
+    ] = "pyxel.models.charge_generation.conversion_with_qe_map"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Cosmix
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationCosmixArguments(Mapping[str, Any]):
-    simulation_mode: Optional[Literal['cosmic_ray', 'cosmics', 'radioactive_decay', 'snowflakes']] = field(
+    simulation_mode: Optional[
+        Literal["cosmic_ray", "cosmics", "radioactive_decay", "snowflakes"]
+    ] = field(
         default=None,
         metadata=schema(
-            title='simulation_mode'
-            ,description='Simulation mode: ``cosmic_rays``, ``radioactive_decay``.'
-        )
+            title="simulation_mode",
+            description="Simulation mode: ``cosmic_rays``, ``radioactive_decay``.",
+        ),
     )
-    running_mode: Optional[Literal['stopping', 'stepsize', 'geant4', 'plotting']] = field(
+    running_mode: Optional[
+        Literal["stopping", "stepsize", "geant4", "plotting"]
+    ] = field(
         default=None,
         metadata=schema(
-            title='running_mode'
-            ,description='Mode: ``stopping``, ``stepsize``, ``geant4``, ``plotting``.'
-        )
+            title="running_mode",
+            description="Mode: ``stopping``, ``stepsize``, ``geant4``, ``plotting``.",
+        ),
     )
-    particle_type: Optional[Literal['proton', 'alpha', 'ion']] = field(
+    particle_type: Optional[Literal["proton", "alpha", "ion"]] = field(
         default=None,
         metadata=schema(
-            title='particle_type'
-            ,description='Type of particle: ``proton``, ``alpha``, ``ion``.'
-        )
+            title="particle_type",
+            description="Type of particle: ``proton``, ``alpha``, ``ion``.",
+        ),
     )
-    initial_energy: Union[int, float, Literal['random'], None] = field(
+    initial_energy: Union[int, float, Literal["random"], None] = field(
         default=None,
         metadata=schema(
-            title='initial_energy'
-            ,description='Kinetic energy of particle, set `random` for random.'
-        )
+            title="initial_energy",
+            description="Kinetic energy of particle, set `random` for random.",
+        ),
     )
     particles_per_second: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='particles_per_second'
-            ,description='Number of particles per second.'
-        )
+            title="particles_per_second", description="Number of particles per second."
+        ),
     )
-    incident_angles: Optional[Tuple[str, str]] = field(
+    incident_angles: Optional[tuple[str, str]] = field(
         default=None,
         metadata=schema(
-            title='incident_angles'
-            ,description='Incident angles: ``(α, β)``.'
-        )
+            title="incident_angles", description="Incident angles: ``(α, β)``."
+        ),
     )
-    starting_position: Optional[Tuple[str, str, str]] = field(
+    starting_position: Optional[tuple[str, str, str]] = field(
         default=None,
         metadata=schema(
-            title='starting_position'
-            ,description='Starting position: ``(x, y, z)``.'
-        )
+            title="starting_position", description="Starting position: ``(x, y, z)``."
+        ),
     )
     spectrum_file: Optional[str] = field(
         default=None,
-        metadata=schema(
-            title='spectrum_file'
-            ,description='Path to input spectrum'
-        )
+        metadata=schema(title="spectrum_file", description="Path to input spectrum"),
     )
     seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-            ,description='Random seed.'
-        )
+        default=None, metadata=schema(title="seed", description="Random seed.")
     )
     ionization_energy: float = field(
         default=3.6,
         metadata=schema(
-            title='ionization_energy'
-            ,description='Mean ionization energy of the semiconductor lattice.'
-        )
+            title="ionization_energy",
+            description="Mean ionization energy of the semiconductor lattice.",
+        ),
     )
     progressbar: bool = field(
-        default=True,
-        metadata=schema(
-            title='progressbar'
-            ,description='Progressbar.'
-        )
+        default=True, metadata=schema(title="progressbar", description="Progressbar.")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('simulation_mode', 'running_mode', 'particle_type', 'initial_energy', 'particles_per_second', 'incident_angles', 'starting_position', 'spectrum_file', 'seed', 'ionization_energy', 'progressbar'))
+        return iter(
+            (
+                "simulation_mode",
+                "running_mode",
+                "particle_type",
+                "initial_energy",
+                "particles_per_second",
+                "incident_angles",
+                "starting_position",
+                "spectrum_file",
+                "seed",
+                "ionization_energy",
+                "progressbar",
+            )
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 11
 
 
-@schema(
-    title="Model 'cosmix'"
-    ,description='Apply CosmiX model.'
-)
+@schema(title="Model 'cosmix'", description="Apply CosmiX model.")
 @dataclass
 class ModelChargeGenerationCosmix:
     name: str
-    arguments: ModelChargeGenerationCosmixArguments = field(default_factory=ModelChargeGenerationCosmixArguments)
-    func: Literal['pyxel.models.charge_generation.cosmix'] = 'pyxel.models.charge_generation.cosmix'
+    arguments: ModelChargeGenerationCosmixArguments = field(
+        default_factory=ModelChargeGenerationCosmixArguments
+    )
+    func: Literal[
+        "pyxel.models.charge_generation.cosmix"
+    ] = "pyxel.models.charge_generation.cosmix"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Dark Current
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationDarkCurrentArguments(Mapping[str, Any]):
     figure_of_merit: float = field(
         metadata=schema(
-            title='figure_of_merit'
-            ,description='Dark current figure of merit. Unit: nA/cm^2'
+            title="figure_of_merit",
+            description="Dark current figure of merit. Unit: nA/cm^2",
         )
     )
     spatial_noise_factor: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='spatial_noise_factor'
-            ,description='Dark current fixed pattern noise factor.'
-        )
+            title="spatial_noise_factor",
+            description="Dark current fixed pattern noise factor.",
+        ),
     )
     band_gap: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='band_gap'
-            ,description='Semiconductor band_gap. If none, the one for silicon is used. Unit: eV'
-        )
+            title="band_gap",
+            description="Semiconductor band_gap. If none, the one for silicon is used. Unit: eV",
+        ),
     )
     band_gap_room_temperature: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='band_gap_room_temperature'
-            ,description=(
-                    'Semiconductor band gap at 300K. If none, the one for silicon is used.'
-                    'Unit: eV'
-                )
-        )
+            title="band_gap_room_temperature",
+            description=(
+                "Semiconductor band gap at 300K. If none, the one for silicon is used."
+                "Unit: eV"
+            ),
+        ),
     )
     seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-            ,description='Random seed.'
-        )
+        default=None, metadata=schema(title="seed", description="Random seed.")
     )
     temporal_noise: bool = field(
-        default=True,
-        metadata=schema(
-            title='temporal_noise'
-            ,description='Shot noise.'
-        )
+        default=True, metadata=schema(title="temporal_noise", description="Shot noise.")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('figure_of_merit', 'spatial_noise_factor', 'band_gap', 'band_gap_room_temperature', 'seed', 'temporal_noise'))
+        return iter(
+            (
+                "figure_of_merit",
+                "spatial_noise_factor",
+                "band_gap",
+                "band_gap_room_temperature",
+                "seed",
+                "temporal_noise",
+            )
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 6
 
 
 @schema(
-    title="Model 'dark_current'"
-    ,description='Add dark current to the detector charge.'
+    title="Model 'dark_current'", description="Add dark current to the detector charge."
 )
 @dataclass
 class ModelChargeGenerationDarkCurrent:
     name: str
     arguments: ModelChargeGenerationDarkCurrentArguments
-    func: Literal['pyxel.models.charge_generation.dark_current'] = 'pyxel.models.charge_generation.dark_current'
+    func: Literal[
+        "pyxel.models.charge_generation.dark_current"
+    ] = "pyxel.models.charge_generation.dark_current"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Dark Current Rule07
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationDarkCurrentRule07Arguments(Mapping[str, Any]):
     cutoff_wavelength: float = field(
         default=2.5,
         metadata=schema(
-            title='cutoff_wavelength'
-            ,description='Cutoff wavelength. Unit: um'
-        )
+            title="cutoff_wavelength", description="Cutoff wavelength. Unit: um"
+        ),
     )
     spatial_noise_factor: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='spatial_noise_factor'
-            ,description='Dark current fixed pattern noise factor.'
-        )
-    )
-    seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-        )
+            title="spatial_noise_factor",
+            description="Dark current fixed pattern noise factor.",
+        ),
     )
+    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
     temporal_noise: bool = field(
-        default=True,
-        metadata=schema(
-            title='temporal_noise'
-            ,description='Shot noise.'
-        )
+        default=True, metadata=schema(title="temporal_noise", description="Shot noise.")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('cutoff_wavelength', 'spatial_noise_factor', 'seed', 'temporal_noise'))
+        return iter(
+            ("cutoff_wavelength", "spatial_noise_factor", "seed", "temporal_noise")
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 4
 
 
 @schema(
-    title="Model 'dark_current_rule07'"
-    ,description='Generate charge from dark current process.'
+    title="Model 'dark_current_rule07'",
+    description="Generate charge from dark current process.",
 )
 @dataclass
 class ModelChargeGenerationDarkCurrentRule07:
     name: str
-    arguments: ModelChargeGenerationDarkCurrentRule07Arguments = field(default_factory=ModelChargeGenerationDarkCurrentRule07Arguments)
-    func: Literal['pyxel.models.charge_generation.dark_current_rule07'] = 'pyxel.models.charge_generation.dark_current_rule07'
+    arguments: ModelChargeGenerationDarkCurrentRule07Arguments = field(
+        default_factory=ModelChargeGenerationDarkCurrentRule07Arguments
+    )
+    func: Literal[
+        "pyxel.models.charge_generation.dark_current_rule07"
+    ] = "pyxel.models.charge_generation.dark_current_rule07"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Dark Current Saphira
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationDarkCurrentSaphiraArguments(Mapping[str, Any]):
-    seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-        )
-    )
+    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('seed',))
+        return iter(("seed",))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'dark_current_saphira'"
-    ,description='Simulate dark current in a Saphira APD detector.'
+    title="Model 'dark_current_saphira'",
+    description="Simulate dark current in a Saphira APD detector.",
 )
 @dataclass
 class ModelChargeGenerationDarkCurrentSaphira:
     name: str
-    arguments: ModelChargeGenerationDarkCurrentSaphiraArguments = field(default_factory=ModelChargeGenerationDarkCurrentSaphiraArguments)
-    func: Literal['pyxel.models.charge_generation.dark_current_saphira'] = 'pyxel.models.charge_generation.dark_current_saphira'
+    arguments: ModelChargeGenerationDarkCurrentSaphiraArguments = field(
+        default_factory=ModelChargeGenerationDarkCurrentSaphiraArguments
+    )
+    func: Literal[
+        "pyxel.models.charge_generation.dark_current_saphira"
+    ] = "pyxel.models.charge_generation.dark_current_saphira"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Load Charge
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationLoadChargeArguments(Mapping[str, Any]):
     filename: Union[str, pathlib.Path] = field(
-        metadata=schema(
-            title='filename'
-            ,description='File path.'
-        )
+        metadata=schema(title="filename", description="File path.")
     )
-    position: Tuple[int, int] = field(
+    position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title='position'
-            ,description=(
-                    'Indices of starting row and column, used when fitting charge to'
-                    'detector.'
-                )
-        )
+            title="position",
+            description=(
+                "Indices of starting row and column, used when fitting charge to"
+                "detector."
+            ),
+        ),
     )
-    align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
+    align: Optional[
+        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
+    ] = field(
         default=None,
         metadata=schema(
-            title='align'
-            ,description=(
-                    'Keyword to align the charge to detector. Can be any from: ("center",'
-                    '"top_left", "top_right", "bottom_left", "bottom_right")'
-                )
-        )
+            title="align",
+            description=(
+                'Keyword to align the charge to detector. Can be any from: ("center",'
+                '"top_left", "top_right", "bottom_left", "bottom_right")'
+            ),
+        ),
     )
     time_scale: float = field(
         default=1.0,
         metadata=schema(
-            title='time_scale'
-            ,description=(
-                    'Time scale of the input charge, default is 1 second. 0.001 would be'
-                    'ms.'
-                )
-        )
+            title="time_scale",
+            description=(
+                "Time scale of the input charge, default is 1 second. 0.001 would be"
+                "ms."
+            ),
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('filename', 'position', 'align', 'time_scale'))
+        return iter(("filename", "position", "align", "time_scale"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 4
 
 
 @schema(
-    title="Model 'load_charge'"
-    ,description=(
-        'Load charge from txt file for detector, mostly for but not limited to'
-        ':term:`CCDs<CCD>`.'
-    )
+    title="Model 'load_charge'",
+    description=(
+        "Load charge from txt file for detector, mostly for but not limited to"
+        ":term:`CCDs<CCD>`."
+    ),
 )
 @dataclass
 class ModelChargeGenerationLoadCharge:
     name: str
     arguments: ModelChargeGenerationLoadChargeArguments
-    func: Literal['pyxel.models.charge_generation.load_charge'] = 'pyxel.models.charge_generation.load_charge'
+    func: Literal[
+        "pyxel.models.charge_generation.load_charge"
+    ] = "pyxel.models.charge_generation.load_charge"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Simple Conversion
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationSimpleConversionArguments(Mapping[str, Any]):
     quantum_efficiency: Optional[float] = field(
         default=None,
-        metadata=schema(
-            title='quantum_efficiency'
-            ,description='Quantum efficiency.'
-        )
-    )
-    seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-        )
+        metadata=schema(title="quantum_efficiency", description="Quantum efficiency."),
     )
+    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
     binomial_sampling: bool = field(
         default=True,
         metadata=schema(
-            title='binomial_sampling'
-            ,description='Binomial sampling. Default is True.'
-        )
+            title="binomial_sampling", description="Binomial sampling. Default is True."
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('quantum_efficiency', 'seed', 'binomial_sampling'))
+        return iter(("quantum_efficiency", "seed", "binomial_sampling"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'simple_conversion'"
-    ,description=(
-        'Generate charge from incident photon via photoelectric effect, simple'
-        'model.'
-    )
+    title="Model 'simple_conversion'",
+    description=(
+        "Generate charge from incident photon via photoelectric effect, simple" "model."
+    ),
 )
 @dataclass
 class ModelChargeGenerationSimpleConversion:
     name: str
-    arguments: ModelChargeGenerationSimpleConversionArguments = field(default_factory=ModelChargeGenerationSimpleConversionArguments)
-    func: Literal['pyxel.models.charge_generation.simple_conversion'] = 'pyxel.models.charge_generation.simple_conversion'
+    arguments: ModelChargeGenerationSimpleConversionArguments = field(
+        default_factory=ModelChargeGenerationSimpleConversionArguments
+    )
+    func: Literal[
+        "pyxel.models.charge_generation.simple_conversion"
+    ] = "pyxel.models.charge_generation.simple_conversion"
     enabled: bool = True
 
 
 #
 # Model: Charge Generation / Simple Dark Current
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationSimpleDarkCurrentArguments(Mapping[str, Any]):
     dark_rate: float = field(
         metadata=schema(
-            title='dark_rate'
-            ,description=(
-                    'Dark current, in electrons/pixel/second, which is the way'
-                    'manufacturers typically report it.'
-                )
-        )
-    )
-    seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
+            title="dark_rate",
+            description=(
+                "Dark current, in electrons/pixel/second, which is the way"
+                "manufacturers typically report it."
+            ),
         )
     )
+    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('dark_rate', 'seed'))
+        return iter(("dark_rate", "seed"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'simple_dark_current'"
-    ,description='Simulate dark current in a detector.'
+    title="Model 'simple_dark_current'",
+    description="Simulate dark current in a detector.",
 )
 @dataclass
 class ModelChargeGenerationSimpleDarkCurrent:
     name: str
     arguments: ModelChargeGenerationSimpleDarkCurrentArguments
-    func: Literal['pyxel.models.charge_generation.simple_dark_current'] = 'pyxel.models.charge_generation.simple_dark_current'
+    func: Literal[
+        "pyxel.models.charge_generation.simple_dark_current"
+    ] = "pyxel.models.charge_generation.simple_dark_current"
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Fixed Pattern Noise
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeCollectionFixedPatternNoiseArguments(Mapping[str, Any]):
     filename: Union[pathlib.Path, str, None] = field(
         default=None,
         metadata=schema(
-            title='filename'
-            ,description='Path to a file with an array or an image.'
-        )
+            title="filename", description="Path to a file with an array or an image."
+        ),
     )
-    position: Tuple[int, int] = field(
+    position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title='position'
-            ,description=(
-                    'Indices of starting row and column, used when fitting noise to'
-                    'detector.'
-                )
-        )
+            title="position",
+            description=(
+                "Indices of starting row and column, used when fitting noise to"
+                "detector."
+            ),
+        ),
     )
-    align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
+    align: Optional[
+        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
+    ] = field(
         default=None,
         metadata=schema(
-            title='align'
-            ,description=(
-                    'Keyword to align the noise to detector. Can be any from: ("center",'
-                    '"top_left", "top_right", "bottom_left", "bottom_right")'
-                )
-        )
+            title="align",
+            description=(
+                'Keyword to align the noise to detector. Can be any from: ("center",'
+                '"top_left", "top_right", "bottom_left", "bottom_right")'
+            ),
+        ),
     )
     fixed_pattern_noise_factor: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='fixed_pattern_noise_factor'
-            ,description='Fixed pattern noise factor.'
-        )
+            title="fixed_pattern_noise_factor",
+            description="Fixed pattern noise factor.",
+        ),
     )
     seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-            ,description='Random seed.'
-        )
+        default=None, metadata=schema(title="seed", description="Random seed.")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('filename', 'position', 'align', 'fixed_pattern_noise_factor', 'seed'))
+        return iter(
+            ("filename", "position", "align", "fixed_pattern_noise_factor", "seed")
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'fixed_pattern_noise'"
-    ,description=(
-        'Add fixed pattern noise caused by pixel non-uniformity during charge'
-        'collection.'
-    )
+    title="Model 'fixed_pattern_noise'",
+    description=(
+        "Add fixed pattern noise caused by pixel non-uniformity during charge"
+        "collection."
+    ),
 )
 @dataclass
 class ModelChargeCollectionFixedPatternNoise:
     name: str
-    arguments: ModelChargeCollectionFixedPatternNoiseArguments = field(default_factory=ModelChargeCollectionFixedPatternNoiseArguments)
-    func: Literal['pyxel.models.charge_collection.fixed_pattern_noise'] = 'pyxel.models.charge_collection.fixed_pattern_noise'
+    arguments: ModelChargeCollectionFixedPatternNoiseArguments = field(
+        default_factory=ModelChargeCollectionFixedPatternNoiseArguments
+    )
+    func: Literal[
+        "pyxel.models.charge_collection.fixed_pattern_noise"
+    ] = "pyxel.models.charge_collection.fixed_pattern_noise"
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Persistence
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeCollectionPersistenceArguments(Mapping[str, Any]):
-    trap_time_constants: Sequence[float] = field(
+    trap_time_constants: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title='trap_time_constants'
-            ,description='A list of trap time constants.'
+            title="trap_time_constants", description="A list of trap time constants."
         )
     )
-    trap_proportions: Sequence[float] = field(
+    trap_proportions: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title='trap_proportions'
-            ,description='A list of trap proportions.'
+            title="trap_proportions", description="A list of trap proportions."
         )
     )
     trap_densities_filename: Union[pathlib.Path, str] = field(
         metadata=schema(
-            title='trap_densities_filename'
-            ,description='Path to densities file.'
+            title="trap_densities_filename", description="Path to densities file."
         )
     )
     trap_capacities_filename: Union[pathlib.Path, str, None] = field(
         default=None,
         metadata=schema(
-            title='trap_capacities_filename'
-            ,description='Path to capacities file.'
-        )
+            title="trap_capacities_filename", description="Path to capacities file."
+        ),
     )
-    trap_densities_position: Tuple[int, int] = field(
+    trap_densities_position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title='trap_densities_position'
-            ,description=(
-                    'Indices of starting row and column, used when fitting densities to'
-                    'detector.'
-                )
-        )
+            title="trap_densities_position",
+            description=(
+                "Indices of starting row and column, used when fitting densities to"
+                "detector."
+            ),
+        ),
     )
-    trap_densities_align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
+    trap_densities_align: Optional[
+        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
+    ] = field(
         default=None,
         metadata=schema(
-            title='trap_densities_align'
-            ,description=(
-                    'Keyword to align the densities to detector. Can be any from:'
-                    '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
-                )
-        )
+            title="trap_densities_align",
+            description=(
+                "Keyword to align the densities to detector. Can be any from:"
+                '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
+            ),
+        ),
     )
-    trap_capacities_position: Tuple[int, int] = field(
+    trap_capacities_position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
-            title='trap_capacities_position'
-            ,description=(
-                    'Indices of starting row and column, used when fitting capacities to'
-                    'detector.'
-                )
-        )
+            title="trap_capacities_position",
+            description=(
+                "Indices of starting row and column, used when fitting capacities to"
+                "detector."
+            ),
+        ),
     )
-    trap_capacities_align: Optional[Literal['center', 'top_left', 'top_right', 'bottom_left', 'bottom_right']] = field(
+    trap_capacities_align: Optional[
+        Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
+    ] = field(
         default=None,
         metadata=schema(
-            title='trap_capacities_align'
-            ,description=(
-                    'Keyword to align the capacities to detector. Can be any from:'
-                    '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
-                )
-        )
+            title="trap_capacities_align",
+            description=(
+                "Keyword to align the capacities to detector. Can be any from:"
+                '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
+            ),
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('trap_time_constants', 'trap_proportions', 'trap_densities_filename', 'trap_capacities_filename', 'trap_densities_position', 'trap_densities_align', 'trap_capacities_position', 'trap_capacities_align'))
+        return iter(
+            (
+                "trap_time_constants",
+                "trap_proportions",
+                "trap_densities_filename",
+                "trap_capacities_filename",
+                "trap_densities_position",
+                "trap_densities_align",
+                "trap_capacities_position",
+                "trap_capacities_align",
+            )
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 8
 
 
-@schema(
-    title="Model 'persistence'"
-    ,description='Apply persistence model.'
-)
+@schema(title="Model 'persistence'", description="Apply persistence model.")
 @dataclass
 class ModelChargeCollectionPersistence:
     name: str
     arguments: ModelChargeCollectionPersistenceArguments
-    func: Literal['pyxel.models.charge_collection.persistence'] = 'pyxel.models.charge_collection.persistence'
+    func: Literal[
+        "pyxel.models.charge_collection.persistence"
+    ] = "pyxel.models.charge_collection.persistence"
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Simple Collection
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeCollectionSimpleCollectionArguments(Mapping[str, Any]):
     def __iter__(self) -> Iterator[str]:
         return iter(())
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 0
 
 
 @schema(
-    title="Model 'simple_collection'"
-    ,description='Associate charge with the closest pixel.'
+    title="Model 'simple_collection'",
+    description="Associate charge with the closest pixel.",
 )
 @dataclass
 class ModelChargeCollectionSimpleCollection:
     name: str
-    arguments: ModelChargeCollectionSimpleCollectionArguments = field(default_factory=ModelChargeCollectionSimpleCollectionArguments)
-    func: Literal['pyxel.models.charge_collection.simple_collection'] = 'pyxel.models.charge_collection.simple_collection'
+    arguments: ModelChargeCollectionSimpleCollectionArguments = field(
+        default_factory=ModelChargeCollectionSimpleCollectionArguments
+    )
+    func: Literal[
+        "pyxel.models.charge_collection.simple_collection"
+    ] = "pyxel.models.charge_collection.simple_collection"
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Simple Full Well
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeCollectionSimpleFullWellArguments(Mapping[str, Any]):
-    fwc: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='fwc'
-        )
-    )
+    fwc: Optional[int] = field(default=None, metadata=schema(title="fwc"))
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('fwc',))
+        return iter(("fwc",))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'simple_full_well'"
-    ,description='Limit the amount of charge in pixel due to full well capacity.'
+    title="Model 'simple_full_well'",
+    description="Limit the amount of charge in pixel due to full well capacity.",
 )
 @dataclass
 class ModelChargeCollectionSimpleFullWell:
     name: str
-    arguments: ModelChargeCollectionSimpleFullWellArguments = field(default_factory=ModelChargeCollectionSimpleFullWellArguments)
-    func: Literal['pyxel.models.charge_collection.simple_full_well'] = 'pyxel.models.charge_collection.simple_full_well'
+    arguments: ModelChargeCollectionSimpleFullWellArguments = field(
+        default_factory=ModelChargeCollectionSimpleFullWellArguments
+    )
+    func: Literal[
+        "pyxel.models.charge_collection.simple_full_well"
+    ] = "pyxel.models.charge_collection.simple_full_well"
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Simple Ipc
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeCollectionSimpleIpcArguments(Mapping[str, Any]):
-    coupling: float = field(
-        metadata=schema(
-            title='coupling'
-        )
-    )
+    coupling: float = field(metadata=schema(title="coupling"))
     diagonal_coupling: float = field(
-        default=0.0,
-        metadata=schema(
-            title='diagonal_coupling'
-        )
+        default=0.0, metadata=schema(title="diagonal_coupling")
     )
     anisotropic_coupling: float = field(
-        default=0.0,
-        metadata=schema(
-            title='anisotropic_coupling'
-        )
+        default=0.0, metadata=schema(title="anisotropic_coupling")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('coupling', 'diagonal_coupling', 'anisotropic_coupling'))
+        return iter(("coupling", "diagonal_coupling", "anisotropic_coupling"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'simple_ipc'"
-    ,description='Convolve pixel array with the IPC kernel.'
+    title="Model 'simple_ipc'", description="Convolve pixel array with the IPC kernel."
 )
 @dataclass
 class ModelChargeCollectionSimpleIpc:
     name: str
     arguments: ModelChargeCollectionSimpleIpcArguments
-    func: Literal['pyxel.models.charge_collection.simple_ipc'] = 'pyxel.models.charge_collection.simple_ipc'
+    func: Literal[
+        "pyxel.models.charge_collection.simple_ipc"
+    ] = "pyxel.models.charge_collection.simple_ipc"
     enabled: bool = True
 
 
 #
 # Model: Charge Collection / Simple Persistence
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeCollectionSimplePersistenceArguments(Mapping[str, Any]):
-    trap_time_constants: Sequence[float] = field(
+    trap_time_constants: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title='trap_time_constants'
-            ,description='List of trap time constants.'
+            title="trap_time_constants", description="List of trap time constants."
         )
     )
-    trap_densities: Sequence[float] = field(
-        metadata=schema(
-            title='trap_densities'
-            ,description='List of trap densities.'
-        )
+    trap_densities: collections.abc.Sequence[float] = field(
+        metadata=schema(title="trap_densities", description="List of trap densities.")
     )
-    trap_capacities: Optional[Sequence[float]] = field(
+    trap_capacities: Optional[collections.abc.Sequence[float]] = field(
         default=None,
         metadata=schema(
-            title='trap_capacities'
-            ,description='List of trap capacities.'
-        )
+            title="trap_capacities", description="List of trap capacities."
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('trap_time_constants', 'trap_densities', 'trap_capacities'))
+        return iter(("trap_time_constants", "trap_densities", "trap_capacities"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'simple_persistence'"
-    ,description='Apply simple persistence model.'
+    title="Model 'simple_persistence'", description="Apply simple persistence model."
 )
 @dataclass
 class ModelChargeCollectionSimplePersistence:
     name: str
     arguments: ModelChargeCollectionSimplePersistenceArguments
-    func: Literal['pyxel.models.charge_collection.simple_persistence'] = 'pyxel.models.charge_collection.simple_persistence'
+    func: Literal[
+        "pyxel.models.charge_collection.simple_persistence"
+    ] = "pyxel.models.charge_collection.simple_persistence"
     enabled: bool = True
 
 
 #
 # Model: Charge Transfer / Arctic Add
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeTransferArcticAddArguments(Mapping[str, Any]):
-    well_fill_power: float = field(
-        metadata=schema(
-            title='well_fill_power'
-        )
-    )
-    trap_densities: Sequence[float] = field(
+    well_fill_power: float = field(metadata=schema(title="well_fill_power"))
+    trap_densities: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title='trap_densities'
-            ,description='A 1D arrays of all trap species densities for serial clocking.'
+            title="trap_densities",
+            description="A 1D arrays of all trap species densities for serial clocking.",
         )
     )
-    trap_release_timescales: Sequence[float] = field(
+    trap_release_timescales: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title='trap_release_timescales'
-            ,description='A 1D arrays of all trap release timescales for serial clocking.'
+            title="trap_release_timescales",
+            description="A 1D arrays of all trap release timescales for serial clocking.",
         )
     )
     express: int = field(
         default=0,
         metadata=schema(
-            title='express'
-            ,description=(
-                    'As described in more detail in :cite:p:`2014:massey` section 2.1.5,'
-                    'the effects of each individual pixel-to-pixel transfer can be very'
-                    'similar, so multiple transfers can be computed at once for efficiency.'
-                    'The ``express`` input sets the number of times the transfers are'
-                    'calculated.      * ``express = 1`` is the fastest and least accurate.'
-                    '* ``express = 2`` means the transfers are re-computed half-way through'
-                    'readout.     * ``express = N`` where ``N`` is the total number of'
-                    'pixels.  Default ``express = 0`` is a convenient input for automatic'
-                    '``express = N``.'
-                )
-        )
+            title="express",
+            description=(
+                "As described in more detail in :cite:p:`2014:massey` section 2.1.5,"
+                "the effects of each individual pixel-to-pixel transfer can be very"
+                "similar, so multiple transfers can be computed at once for efficiency."
+                "The ``express`` input sets the number of times the transfers are"
+                "calculated.      * ``express = 1`` is the fastest and least accurate."
+                "* ``express = 2`` means the transfers are re-computed half-way through"
+                "readout.     * ``express = N`` where ``N`` is the total number of"
+                "pixels.  Default ``express = 0`` is a convenient input for automatic"
+                "``express = N``."
+            ),
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('well_fill_power', 'trap_densities', 'trap_release_timescales', 'express'))
+        return iter(
+            ("well_fill_power", "trap_densities", "trap_release_timescales", "express")
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 4
 
 
 @schema(
-    title="Model 'arctic_add'"
-    ,description=(
-        'Add :term:`CTI` trails to an image by trapping, releasing and moving'
-        'electrons.'
-    )
+    title="Model 'arctic_add'",
+    description=(
+        "Add :term:`CTI` trails to an image by trapping, releasing and moving"
+        "electrons."
+    ),
 )
 @dataclass
 class ModelChargeTransferArcticAdd:
     name: str
     arguments: ModelChargeTransferArcticAddArguments
-    func: Literal['pyxel.models.charge_transfer.arctic_add'] = 'pyxel.models.charge_transfer.arctic_add'
+    func: Literal[
+        "pyxel.models.charge_transfer.arctic_add"
+    ] = "pyxel.models.charge_transfer.arctic_add"
     enabled: bool = True
 
 
 #
 # Model: Charge Transfer / Arctic Remove
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeTransferArcticRemoveArguments(Mapping[str, Any]):
-    well_fill_power: float = field(
-        metadata=schema(
-            title='well_fill_power'
-        )
-    )
-    trap_densities: Sequence[float] = field(
-        metadata=schema(
-            title='trap_densities'
-        )
+    well_fill_power: float = field(metadata=schema(title="well_fill_power"))
+    trap_densities: collections.abc.Sequence[float] = field(
+        metadata=schema(title="trap_densities")
     )
-    trap_release_timescales: Sequence[float] = field(
-        metadata=schema(
-            title='trap_release_timescales'
-        )
+    trap_release_timescales: collections.abc.Sequence[float] = field(
+        metadata=schema(title="trap_release_timescales")
     )
     num_iterations: int = field(
         metadata=schema(
-            title='num_iterations'
-            ,description=(
-                    'Number of iterations for the forward modelling. More iterations'
-                    'provide higher accuracy at the cost of longer runtime. In practice,'
-                    'just 1 to 3 iterations are usually sufficient.'
-                )
+            title="num_iterations",
+            description=(
+                "Number of iterations for the forward modelling. More iterations"
+                "provide higher accuracy at the cost of longer runtime. In practice,"
+                "just 1 to 3 iterations are usually sufficient."
+            ),
         )
     )
     express: int = field(
         default=0,
         metadata=schema(
-            title='express'
-            ,description=(
-                    'As described in more detail in :cite:p:`2014:massey` section 2.1.5,'
-                    'the effects of each individual pixel-to-pixel transfer can be very'
-                    'similar, so multiple transfers can be computed at once for efficiency.'
-                    'The ``express`` input sets the number of times the transfers are'
-                    'calculated.      * ``express = 1`` is the fastest and least accurate.'
-                    '* ``express = 2`` means the transfers are re-computed half-way through'
-                    'readout.     * ``express = N`` where ``N`` is the total number of'
-                    'pixels.  Default ``express = 0`` is a convenient input for automatic'
-                    '``express = N``.'
-                )
-        )
+            title="express",
+            description=(
+                "As described in more detail in :cite:p:`2014:massey` section 2.1.5,"
+                "the effects of each individual pixel-to-pixel transfer can be very"
+                "similar, so multiple transfers can be computed at once for efficiency."
+                "The ``express`` input sets the number of times the transfers are"
+                "calculated.      * ``express = 1`` is the fastest and least accurate."
+                "* ``express = 2`` means the transfers are re-computed half-way through"
+                "readout.     * ``express = N`` where ``N`` is the total number of"
+                "pixels.  Default ``express = 0`` is a convenient input for automatic"
+                "``express = N``."
+            ),
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('well_fill_power', 'trap_densities', 'trap_release_timescales', 'num_iterations', 'express'))
+        return iter(
+            (
+                "well_fill_power",
+                "trap_densities",
+                "trap_release_timescales",
+                "num_iterations",
+                "express",
+            )
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'arctic_remove'"
-    ,description=(
-        'Remove :term:`CTI` trails from an image by first modelling the'
-        'addition of :term:`CTI`.'
-    )
+    title="Model 'arctic_remove'",
+    description=(
+        "Remove :term:`CTI` trails from an image by first modelling the"
+        "addition of :term:`CTI`."
+    ),
 )
 @dataclass
 class ModelChargeTransferArcticRemove:
     name: str
     arguments: ModelChargeTransferArcticRemoveArguments
-    func: Literal['pyxel.models.charge_transfer.arctic_remove'] = 'pyxel.models.charge_transfer.arctic_remove'
+    func: Literal[
+        "pyxel.models.charge_transfer.arctic_remove"
+    ] = "pyxel.models.charge_transfer.arctic_remove"
     enabled: bool = True
 
 
 #
 # Model: Charge Transfer / Cdm
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeTransferCdmArguments(Mapping[str, Any]):
-    direction: Literal['parallel', 'serial'] = field(
+    direction: Literal["parallel", "serial"] = field(
         metadata=schema(
-            title='direction'
-            ,description=(
-                    'Set ``"parallel"`` for :term:`CTI` in parallel direction or'
-                    '``"serial"`` for :term:`CTI` in serial register.'
-                )
+            title="direction",
+            description=(
+                'Set ``"parallel"`` for :term:`CTI` in parallel direction or'
+                '``"serial"`` for :term:`CTI` in serial register.'
+            ),
         )
     )
     beta: float = field(
         metadata=schema(
-            title='beta'
-            ,description='Electron cloud expansion coefficient :math:`\\beta`.'
+            title="beta",
+            description="Electron cloud expansion coefficient :math:`\\beta`.",
         )
     )
-    trap_release_times: Sequence[float] = field(
+    trap_release_times: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title='trap_release_times'
-            ,description='Trap release time constants :math:`\\tau_r`. Unit: :math:`s`.'
+            title="trap_release_times",
+            description="Trap release time constants :math:`\\tau_r`. Unit: :math:`s`.",
         )
     )
-    trap_densities: Sequence[float] = field(
+    trap_densities: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title='trap_densities'
-            ,description='Absolute trap densities :math:`n_t`. Unit: :math:`cm^{-3}`.'
+            title="trap_densities",
+            description="Absolute trap densities :math:`n_t`. Unit: :math:`cm^{-3}`.",
         )
     )
-    sigma: Sequence[float] = field(
+    sigma: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title='sigma'
-            ,description='Trap capture cross section :math:`\\sigma`. Unit: :math:`cm^2`.'
+            title="sigma",
+            description="Trap capture cross section :math:`\\sigma`. Unit: :math:`cm^2`.",
         )
     )
     full_well_capacity: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='full_well_capacity'
-            ,description='Full well capacity :math:`FWC`. Unit: :math:`e^-`.'
-        )
+            title="full_well_capacity",
+            description="Full well capacity :math:`FWC`. Unit: :math:`e^-`.",
+        ),
     )
     max_electron_volume: float = field(
         default=0.0,
         metadata=schema(
-            title='max_electron_volume'
-            ,description=(
-                    'Maximum geometrical volume :math:`V_g` that electrons can occupy'
-                    'within a pixel. Unit: :math:`cm^3`.'
-                )
-        )
+            title="max_electron_volume",
+            description=(
+                "Maximum geometrical volume :math:`V_g` that electrons can occupy"
+                "within a pixel. Unit: :math:`cm^3`."
+            ),
+        ),
     )
     transfer_period: float = field(
         default=0.0,
         metadata=schema(
-            title='transfer_period'
-            ,description='Transfer period :math:`t` (TDI period). Unit: :math:`s`.'
-        )
+            title="transfer_period",
+            description="Transfer period :math:`t` (TDI period). Unit: :math:`s`.",
+        ),
     )
     charge_injection: bool = field(
         default=False,
         metadata=schema(
-            title='charge_injection'
-            ,description='Enable charge injection (only used in ``"parallel"`` mode).'
-        )
+            title="charge_injection",
+            description='Enable charge injection (only used in ``"parallel"`` mode).',
+        ),
     )
     electron_effective_mass: float = field(
         default=0.5,
         metadata=schema(
-            title='electron_effective_mass'
-            ,description=(
-                    'Electron effective mass in the semiconductor lattice. Unit: 1 electron'
-                    'mass'
-                )
-        )
+            title="electron_effective_mass",
+            description=(
+                "Electron effective mass in the semiconductor lattice. Unit: 1 electron"
+                "mass"
+            ),
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('direction', 'beta', 'trap_release_times', 'trap_densities', 'sigma', 'full_well_capacity', 'max_electron_volume', 'transfer_period', 'charge_injection', 'electron_effective_mass'))
+        return iter(
+            (
+                "direction",
+                "beta",
+                "trap_release_times",
+                "trap_densities",
+                "sigma",
+                "full_well_capacity",
+                "max_electron_volume",
+                "transfer_period",
+                "charge_injection",
+                "electron_effective_mass",
+            )
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 10
 
 
-@schema(
-    title="Model 'cdm'"
-    ,description='Charge Distortion Model (CDM) model wrapper.'
-)
+@schema(title="Model 'cdm'", description="Charge Distortion Model (CDM) model wrapper.")
 @dataclass
 class ModelChargeTransferCdm:
     name: str
     arguments: ModelChargeTransferCdmArguments
-    func: Literal['pyxel.models.charge_transfer.cdm'] = 'pyxel.models.charge_transfer.cdm'
+    func: Literal[
+        "pyxel.models.charge_transfer.cdm"
+    ] = "pyxel.models.charge_transfer.cdm"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Dc Offset
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementDcOffsetArguments(Mapping[str, Any]):
     offset: float = field(
-        metadata=schema(
-            title='offset'
-            ,description='DC offset voltage. Unit: V'
-        )
+        metadata=schema(title="offset", description="DC offset voltage. Unit: V")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('offset',))
+        return iter(("offset",))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 1
 
 
-@schema(
-    title="Model 'dc_offset'"
-    ,description='Apply DC voltage to the detector.'
-)
+@schema(title="Model 'dc_offset'", description="Apply DC voltage to the detector.")
 @dataclass
 class ModelChargeMeasurementDcOffset:
     name: str
     arguments: ModelChargeMeasurementDcOffsetArguments
-    func: Literal['pyxel.models.charge_measurement.dc_offset'] = 'pyxel.models.charge_measurement.dc_offset'
+    func: Literal[
+        "pyxel.models.charge_measurement.dc_offset"
+    ] = "pyxel.models.charge_measurement.dc_offset"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Ktc Noise
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementKtcNoiseArguments(Mapping[str, Any]):
     node_capacitance: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='node_capacitance'
-            ,description='Node capacitance. Unit: F'
-        )
+            title="node_capacitance", description="Node capacitance. Unit: F"
+        ),
     )
     seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-            ,description='Random seed.'
-        )
+        default=None, metadata=schema(title="seed", description="Random seed.")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('node_capacitance', 'seed'))
+        return iter(("node_capacitance", "seed"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'ktc_noise'"
-    ,description='Apply KTC reset noise to detector signal array.'
+    title="Model 'ktc_noise'",
+    description="Apply KTC reset noise to detector signal array.",
 )
 @dataclass
 class ModelChargeMeasurementKtcNoise:
     name: str
-    arguments: ModelChargeMeasurementKtcNoiseArguments = field(default_factory=ModelChargeMeasurementKtcNoiseArguments)
-    func: Literal['pyxel.models.charge_measurement.ktc_noise'] = 'pyxel.models.charge_measurement.ktc_noise'
+    arguments: ModelChargeMeasurementKtcNoiseArguments = field(
+        default_factory=ModelChargeMeasurementKtcNoiseArguments
+    )
+    func: Literal[
+        "pyxel.models.charge_measurement.ktc_noise"
+    ] = "pyxel.models.charge_measurement.ktc_noise"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Nghxrg
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementNghxrgArguments(Mapping[str, Any]):
-    noise: Sequence[Mapping[Literal['ktc_bias_noise', 'white_read_noise', 'corr_pink_noise', 'uncorr_pink_noise', 'acn_noise', 'pca_zero_noise'], Mapping[str, float]]] = field(
-        metadata=schema(
-            title='noise'
-        )
-    )
-    window_position: Optional[Tuple[int, int]] = field(
-        default=None,
-        metadata=schema(
-            title='window_position'
-            ,description='[x0 (columns), y0 (rows)].'
-        )
-    )
-    window_size: Optional[Tuple[int, int]] = field(
+    noise: collections.abc.Sequence[
+        collections.abc.Mapping[
+            Literal[
+                "ktc_bias_noise",
+                "white_read_noise",
+                "corr_pink_noise",
+                "uncorr_pink_noise",
+                "acn_noise",
+                "pca_zero_noise",
+            ],
+            collections.abc.Mapping[str, float],
+        ]
+    ] = field(metadata=schema(title="noise"))
+    window_position: Optional[tuple[int, int]] = field(
         default=None,
         metadata=schema(
-            title='window_size'
-            ,description='[x (columns), y (rows)].'
-        )
+            title="window_position", description="[x0 (columns), y0 (rows)]."
+        ),
     )
-    seed: Optional[int] = field(
+    window_size: Optional[tuple[int, int]] = field(
         default=None,
-        metadata=schema(
-            title='seed'
-        )
+        metadata=schema(title="window_size", description="[x (columns), y (rows)]."),
     )
+    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
     n_output: int = field(
         default=1,
-        metadata=schema(
-            title='n_output'
-            ,description='Number of detector outputs.'
-        )
+        metadata=schema(title="n_output", description="Number of detector outputs."),
     )
     n_row_overhead: int = field(
         default=0,
         metadata=schema(
-            title='n_row_overhead'
-            ,description=(
-                    'New row overhead in pixel. This allows for a short wait at the end of'
-                    'a row before starting the next row.'
-                )
-        )
+            title="n_row_overhead",
+            description=(
+                "New row overhead in pixel. This allows for a short wait at the end of"
+                "a row before starting the next row."
+            ),
+        ),
     )
     n_frame_overhead: int = field(
         default=0,
         metadata=schema(
-            title='n_frame_overhead'
-            ,description=(
-                    'New frame overhead in rows. This allows for a short wait at the end of'
-                    'a frame before starting the next frame.'
-                )
-        )
+            title="n_frame_overhead",
+            description=(
+                "New frame overhead in rows. This allows for a short wait at the end of"
+                "a frame before starting the next frame."
+            ),
+        ),
     )
     reverse_scan_direction: bool = field(
         default=False,
         metadata=schema(
-            title='reverse_scan_direction'
-            ,description=(
-                    'Set this True to reverse the fast scanner readout directions. This'
-                    'capability was added to support Teledyne’s programmable fast scan'
-                    'readout directions. The default setting (False) corresponds to what'
-                    'HxRG detectors default to upon power up.'
-                )
-        )
+            title="reverse_scan_direction",
+            description=(
+                "Set this True to reverse the fast scanner readout directions. This"
+                "capability was added to support Teledyne’s programmable fast scan"
+                "readout directions. The default setting (False) corresponds to what"
+                "HxRG detectors default to upon power up."
+            ),
+        ),
     )
     reference_pixel_border_width: int = field(
         default=4,
         metadata=schema(
-            title='reference_pixel_border_width'
-            ,description='Width of reference pixel border around image area.'
-        )
+            title="reference_pixel_border_width",
+            description="Width of reference pixel border around image area.",
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('noise', 'window_position', 'window_size', 'seed', 'n_output', 'n_row_overhead', 'n_frame_overhead', 'reverse_scan_direction', 'reference_pixel_border_width'))
+        return iter(
+            (
+                "noise",
+                "window_position",
+                "window_size",
+                "seed",
+                "n_output",
+                "n_row_overhead",
+                "n_frame_overhead",
+                "reverse_scan_direction",
+                "reference_pixel_border_width",
+            )
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 9
 
 
 @schema(
-    title="Model 'nghxrg'"
-    ,description='Generate fourier noise power spectrum on HXRG detector.'
+    title="Model 'nghxrg'",
+    description="Generate fourier noise power spectrum on HXRG detector.",
 )
 @dataclass
 class ModelChargeMeasurementNghxrg:
     name: str
     arguments: ModelChargeMeasurementNghxrgArguments
-    func: Literal['pyxel.models.charge_measurement.nghxrg'] = 'pyxel.models.charge_measurement.nghxrg'
+    func: Literal[
+        "pyxel.models.charge_measurement.nghxrg"
+    ] = "pyxel.models.charge_measurement.nghxrg"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Output Node Linearity Poly
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementOutputNodeLinearityPolyArguments(Mapping[str, Any]):
-    coefficients: Sequence[float] = field(
+    coefficients: collections.abc.Sequence[float] = field(
         metadata=schema(
-            title='coefficients'
-            ,description='Coefficient of the polynomial function.'
+            title="coefficients", description="Coefficient of the polynomial function."
         )
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('coefficients',))
+        return iter(("coefficients",))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'output_node_linearity_poly'"
-    ,description=(
-        'Add non-linearity to signal array to simulate the non-linearity of the'
-        'output node circuit.'
-    )
+    title="Model 'output_node_linearity_poly'",
+    description=(
+        "Add non-linearity to signal array to simulate the non-linearity of the"
+        "output node circuit."
+    ),
 )
 @dataclass
 class ModelChargeMeasurementOutputNodeLinearityPoly:
     name: str
     arguments: ModelChargeMeasurementOutputNodeLinearityPolyArguments
-    func: Literal['pyxel.models.charge_measurement.output_node_linearity_poly'] = 'pyxel.models.charge_measurement.output_node_linearity_poly'
+    func: Literal[
+        "pyxel.models.charge_measurement.output_node_linearity_poly"
+    ] = "pyxel.models.charge_measurement.output_node_linearity_poly"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Output Node Noise
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementOutputNodeNoiseArguments(Mapping[str, Any]):
     std_deviation: float = field(
         metadata=schema(
-            title='std_deviation'
-            ,description='Standard deviation. Unit: V'
+            title="std_deviation", description="Standard deviation. Unit: V"
         )
     )
     seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-            ,description='Random seed.'
-        )
+        default=None, metadata=schema(title="seed", description="Random seed.")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('std_deviation', 'seed'))
+        return iter(("std_deviation", "seed"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'output_node_noise'"
-    ,description=(
-        'Add noise to signal array of detector output node using normal random'
-        'distribution.'
-    )
+    title="Model 'output_node_noise'",
+    description=(
+        "Add noise to signal array of detector output node using normal random"
+        "distribution."
+    ),
 )
 @dataclass
 class ModelChargeMeasurementOutputNodeNoise:
     name: str
     arguments: ModelChargeMeasurementOutputNodeNoiseArguments
-    func: Literal['pyxel.models.charge_measurement.output_node_noise'] = 'pyxel.models.charge_measurement.output_node_noise'
+    func: Literal[
+        "pyxel.models.charge_measurement.output_node_noise"
+    ] = "pyxel.models.charge_measurement.output_node_noise"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Output Node Noise Cmos
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementOutputNodeNoiseCmosArguments(Mapping[str, Any]):
     readout_noise: float = field(
         metadata=schema(
-            title='readout_noise'
-            ,description='Mean readout noise for the array in units of electrons. Unit: electron'
+            title="readout_noise",
+            description="Mean readout noise for the array in units of electrons. Unit: electron",
         )
     )
     readout_noise_std: float = field(
         metadata=schema(
-            title='readout_noise_std'
-            ,description='Readout noise standard deviation in units of electrons. Unit: electron'
+            title="readout_noise_std",
+            description="Readout noise standard deviation in units of electrons. Unit: electron",
         )
     )
     seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-            ,description='Random seed.'
-        )
+        default=None, metadata=schema(title="seed", description="Random seed.")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('readout_noise', 'readout_noise_std', 'seed'))
+        return iter(("readout_noise", "readout_noise_std", "seed"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'output_node_noise_cmos'"
-    ,description=(
-        'Output node noise model for :term:`CMOS` detectors where readout is'
-        'statistically independent for each pixel.'
-    )
+    title="Model 'output_node_noise_cmos'",
+    description=(
+        "Output node noise model for :term:`CMOS` detectors where readout is"
+        "statistically independent for each pixel."
+    ),
 )
 @dataclass
 class ModelChargeMeasurementOutputNodeNoiseCmos:
     name: str
     arguments: ModelChargeMeasurementOutputNodeNoiseCmosArguments
-    func: Literal['pyxel.models.charge_measurement.output_node_noise_cmos'] = 'pyxel.models.charge_measurement.output_node_noise_cmos'
+    func: Literal[
+        "pyxel.models.charge_measurement.output_node_noise_cmos"
+    ] = "pyxel.models.charge_measurement.output_node_noise_cmos"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Output Pixel Reset Voltage Apd
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementOutputPixelResetVoltageApdArguments(Mapping[str, Any]):
     roic_drop: float = field(
         metadata=schema(
-            title='roic_drop'
-            ,description='Readout circuit drop voltage. Unit: V'
+            title="roic_drop", description="Readout circuit drop voltage. Unit: V"
         )
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('roic_drop',))
+        return iter(("roic_drop",))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'output_pixel_reset_voltage_apd'"
-    ,description='Apply output pixel reset voltage to APD detector.'
+    title="Model 'output_pixel_reset_voltage_apd'",
+    description="Apply output pixel reset voltage to APD detector.",
 )
 @dataclass
 class ModelChargeMeasurementOutputPixelResetVoltageApd:
     name: str
     arguments: ModelChargeMeasurementOutputPixelResetVoltageApdArguments
-    func: Literal['pyxel.models.charge_measurement.output_pixel_reset_voltage_apd'] = 'pyxel.models.charge_measurement.output_pixel_reset_voltage_apd'
+    func: Literal[
+        "pyxel.models.charge_measurement.output_pixel_reset_voltage_apd"
+    ] = "pyxel.models.charge_measurement.output_pixel_reset_voltage_apd"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Physical Non Linearity
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementPhysicalNonLinearityArguments(Mapping[str, Any]):
     cutoff: float = field(
-        metadata=schema(
-            title='cutoff'
-            ,description='Cutoff wavelength. unit: um'
-        )
+        metadata=schema(title="cutoff", description="Cutoff wavelength. unit: um")
     )
     n_donor: float = field(
-        metadata=schema(
-            title='n_donor'
-            ,description='Donor density. Unit: atoms/cm^3'
-        )
+        metadata=schema(title="n_donor", description="Donor density. Unit: atoms/cm^3")
     )
     n_acceptor: float = field(
         metadata=schema(
-            title='n_acceptor'
-            ,description='Acceptor density. Unit: atoms/cm^3'
+            title="n_acceptor", description="Acceptor density. Unit: atoms/cm^3"
         )
     )
     diode_diameter: float = field(
-        metadata=schema(
-            title='diode_diameter'
-            ,description='Diode diameter. Unit: um'
-        )
+        metadata=schema(title="diode_diameter", description="Diode diameter. Unit: um")
     )
     v_bias: float = field(
-        metadata=schema(
-            title='v_bias'
-            ,description='Initial bias voltage. Unit: V.'
-        )
+        metadata=schema(title="v_bias", description="Initial bias voltage. Unit: V.")
     )
     fixed_capacitance: float = field(
         metadata=schema(
-            title='fixed_capacitance'
-            ,description='Additional fixed capacitance. Unit: F'
+            title="fixed_capacitance",
+            description="Additional fixed capacitance. Unit: F",
         )
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('cutoff', 'n_donor', 'n_acceptor', 'diode_diameter', 'v_bias', 'fixed_capacitance'))
+        return iter(
+            (
+                "cutoff",
+                "n_donor",
+                "n_acceptor",
+                "diode_diameter",
+                "v_bias",
+                "fixed_capacitance",
+            )
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 6
 
 
 @schema(
-    title="Model 'physical_non_linearity'"
-    ,description='Apply physical non-linearity.'
+    title="Model 'physical_non_linearity'", description="Apply physical non-linearity."
 )
 @dataclass
 class ModelChargeMeasurementPhysicalNonLinearity:
     name: str
     arguments: ModelChargeMeasurementPhysicalNonLinearityArguments
-    func: Literal['pyxel.models.charge_measurement.physical_non_linearity'] = 'pyxel.models.charge_measurement.physical_non_linearity'
+    func: Literal[
+        "pyxel.models.charge_measurement.physical_non_linearity"
+    ] = "pyxel.models.charge_measurement.physical_non_linearity"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Physical Non Linearity With Saturation
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
-class ModelChargeMeasurementPhysicalNonLinearityWithSaturationArguments(Mapping[str, Any]):
+class ModelChargeMeasurementPhysicalNonLinearityWithSaturationArguments(
+    Mapping[str, Any]
+):
     cutoff: float = field(
-        metadata=schema(
-            title='cutoff'
-            ,description='Cutoff wavelength. unit: um'
-        )
+        metadata=schema(title="cutoff", description="Cutoff wavelength. unit: um")
     )
     n_donor: float = field(
-        metadata=schema(
-            title='n_donor'
-            ,description='Donor density. Unit: atoms/cm^3'
-        )
+        metadata=schema(title="n_donor", description="Donor density. Unit: atoms/cm^3")
     )
     n_acceptor: float = field(
         metadata=schema(
-            title='n_acceptor'
-            ,description='Acceptor density. Unit: atoms/cm^3'
+            title="n_acceptor", description="Acceptor density. Unit: atoms/cm^3"
         )
     )
     phi_implant: float = field(
         metadata=schema(
-            title='phi_implant'
-            ,description='Diameter of the implantation. Unit: um'
+            title="phi_implant", description="Diameter of the implantation. Unit: um"
         )
     )
     d_implant: float = field(
         metadata=schema(
-            title='d_implant'
-            ,description='Depth of the implamantation. Unit: um'
+            title="d_implant", description="Depth of the implamantation. Unit: um"
         )
     )
     saturation_current: float = field(
         metadata=schema(
-            title='saturation_current'
-            ,description='Saturation current: e-/s/pix.'
+            title="saturation_current", description="Saturation current: e-/s/pix."
         )
     )
     ideality_factor: float = field(
-        metadata=schema(
-            title='ideality_factor'
-            ,description='Ideality factor.'
-        )
+        metadata=schema(title="ideality_factor", description="Ideality factor.")
     )
     v_reset: float = field(
-        metadata=schema(
-            title='v_reset'
-            ,description='VRESET. Unit: V.'
-        )
-    )
-    d_sub: float = field(
-        metadata=schema(
-            title='d_sub'
-            ,description='DSUB. Unit: V.'
-        )
+        metadata=schema(title="v_reset", description="VRESET. Unit: V.")
     )
+    d_sub: float = field(metadata=schema(title="d_sub", description="DSUB. Unit: V."))
     fixed_capacitance: float = field(
         metadata=schema(
-            title='fixed_capacitance'
-            ,description='Additional fixed capacitance. Unit: F.'
+            title="fixed_capacitance",
+            description="Additional fixed capacitance. Unit: F.",
         )
     )
     euler_points: int = field(
         metadata=schema(
-            title='euler_points'
-            ,description='Number of points in the euler method.'
+            title="euler_points", description="Number of points in the euler method."
         )
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('cutoff', 'n_donor', 'n_acceptor', 'phi_implant', 'd_implant', 'saturation_current', 'ideality_factor', 'v_reset', 'd_sub', 'fixed_capacitance', 'euler_points'))
+        return iter(
+            (
+                "cutoff",
+                "n_donor",
+                "n_acceptor",
+                "phi_implant",
+                "d_implant",
+                "saturation_current",
+                "ideality_factor",
+                "v_reset",
+                "d_sub",
+                "fixed_capacitance",
+                "euler_points",
+            )
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 11
 
 
 @schema(
-    title="Model 'physical_non_linearity_with_saturation'"
-    ,description='Apply physical non-linearity with saturation.'
+    title="Model 'physical_non_linearity_with_saturation'",
+    description="Apply physical non-linearity with saturation.",
 )
 @dataclass
 class ModelChargeMeasurementPhysicalNonLinearityWithSaturation:
     name: str
     arguments: ModelChargeMeasurementPhysicalNonLinearityWithSaturationArguments
-    func: Literal['pyxel.models.charge_measurement.physical_non_linearity_with_saturation'] = 'pyxel.models.charge_measurement.physical_non_linearity_with_saturation'
+    func: Literal[
+        "pyxel.models.charge_measurement.physical_non_linearity_with_saturation"
+    ] = "pyxel.models.charge_measurement.physical_non_linearity_with_saturation"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Readout Noise Saphira
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementReadoutNoiseSaphiraArguments(Mapping[str, Any]):
     roic_readout_noise: float = field(
         metadata=schema(
-            title='roic_readout_noise'
-            ,description='Readout integrated circuit noise in volts RMS. Unit: V'
+            title="roic_readout_noise",
+            description="Readout integrated circuit noise in volts RMS. Unit: V",
         )
     )
     controller_noise: float = field(
         default=0.0,
         metadata=schema(
-            title='controller_noise'
-            ,description='Controller noise in volts RMS. Unit: V'
-        )
-    )
-    seed: Optional[int] = field(
-        default=None,
-        metadata=schema(
-            title='seed'
-        )
+            title="controller_noise",
+            description="Controller noise in volts RMS. Unit: V",
+        ),
     )
+    seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('roic_readout_noise', 'controller_noise', 'seed'))
+        return iter(("roic_readout_noise", "controller_noise", "seed"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'readout_noise_saphira'"
-    ,description='Apply Saphira specific readout noise to the APD detector.'
+    title="Model 'readout_noise_saphira'",
+    description="Apply Saphira specific readout noise to the APD detector.",
 )
 @dataclass
 class ModelChargeMeasurementReadoutNoiseSaphira:
     name: str
     arguments: ModelChargeMeasurementReadoutNoiseSaphiraArguments
-    func: Literal['pyxel.models.charge_measurement.readout_noise_saphira'] = 'pyxel.models.charge_measurement.readout_noise_saphira'
+    func: Literal[
+        "pyxel.models.charge_measurement.readout_noise_saphira"
+    ] = "pyxel.models.charge_measurement.readout_noise_saphira"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Simple Measurement
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementSimpleMeasurementArguments(Mapping[str, Any]):
     gain: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='gain'
-            ,description=(
-                    'Gain to apply. By default, this is the sensitivity of charge readout.'
-                    'Unit: V/e-'
-                )
-        )
+            title="gain",
+            description=(
+                "Gain to apply. By default, this is the sensitivity of charge readout."
+                "Unit: V/e-"
+            ),
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('gain',))
+        return iter(("gain",))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'simple_measurement'"
-    ,description='Convert the pixel array into signal array.'
+    title="Model 'simple_measurement'",
+    description="Convert the pixel array into signal array.",
 )
 @dataclass
 class ModelChargeMeasurementSimpleMeasurement:
     name: str
-    arguments: ModelChargeMeasurementSimpleMeasurementArguments = field(default_factory=ModelChargeMeasurementSimpleMeasurementArguments)
-    func: Literal['pyxel.models.charge_measurement.simple_measurement'] = 'pyxel.models.charge_measurement.simple_measurement'
+    arguments: ModelChargeMeasurementSimpleMeasurementArguments = field(
+        default_factory=ModelChargeMeasurementSimpleMeasurementArguments
+    )
+    func: Literal[
+        "pyxel.models.charge_measurement.simple_measurement"
+    ] = "pyxel.models.charge_measurement.simple_measurement"
     enabled: bool = True
 
 
 #
 # Model: Charge Measurement / Simple Physical Non Linearity
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementSimplePhysicalNonLinearityArguments(Mapping[str, Any]):
     cutoff: float = field(
-        metadata=schema(
-            title='cutoff'
-            ,description='Cutoff wavelength. unit: um'
-        )
+        metadata=schema(title="cutoff", description="Cutoff wavelength. unit: um")
     )
     n_donor: float = field(
-        metadata=schema(
-            title='n_donor'
-            ,description='Donor density. Unit: atoms/cm^3'
-        )
+        metadata=schema(title="n_donor", description="Donor density. Unit: atoms/cm^3")
     )
     n_acceptor: float = field(
         metadata=schema(
-            title='n_acceptor'
-            ,description='Acceptor density. Unit: atoms/cm^3'
+            title="n_acceptor", description="Acceptor density. Unit: atoms/cm^3"
         )
     )
     diode_diameter: float = field(
-        metadata=schema(
-            title='diode_diameter'
-            ,description='Diode diameter. Unit: um'
-        )
+        metadata=schema(title="diode_diameter", description="Diode diameter. Unit: um")
     )
     v_bias: float = field(
-        metadata=schema(
-            title='v_bias'
-            ,description='Initial bias voltage. Unit: V.'
-        )
+        metadata=schema(title="v_bias", description="Initial bias voltage. Unit: V.")
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('cutoff', 'n_donor', 'n_acceptor', 'diode_diameter', 'v_bias'))
+        return iter(("cutoff", "n_donor", "n_acceptor", "diode_diameter", "v_bias"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 5
 
 
 @schema(
-    title="Model 'simple_physical_non_linearity'"
-    ,description='Apply simple physical non-linearity.'
+    title="Model 'simple_physical_non_linearity'",
+    description="Apply simple physical non-linearity.",
 )
 @dataclass
 class ModelChargeMeasurementSimplePhysicalNonLinearity:
     name: str
     arguments: ModelChargeMeasurementSimplePhysicalNonLinearityArguments
-    func: Literal['pyxel.models.charge_measurement.simple_physical_non_linearity'] = 'pyxel.models.charge_measurement.simple_physical_non_linearity'
+    func: Literal[
+        "pyxel.models.charge_measurement.simple_physical_non_linearity"
+    ] = "pyxel.models.charge_measurement.simple_physical_non_linearity"
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Ac Crosstalk
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsAcCrosstalkArguments(Mapping[str, Any]):
-    coupling_matrix: Union[str, pathlib.Path, Sequence] = field(
-        metadata=schema(
-            title='coupling_matrix'
-        )
-    )
-    channel_matrix: Sequence = field(
-        metadata=schema(
-            title='channel_matrix'
-        )
-    )
-    readout_directions: Sequence = field(
-        metadata=schema(
-            title='readout_directions'
-        )
+    coupling_matrix: Union[str, pathlib.Path, collections.abc.Sequence] = field(
+        metadata=schema(title="coupling_matrix")
     )
+    channel_matrix: Sequence = field(metadata=schema(title="channel_matrix"))
+    readout_directions: Sequence = field(metadata=schema(title="readout_directions"))
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('coupling_matrix', 'channel_matrix', 'readout_directions'))
+        return iter(("coupling_matrix", "channel_matrix", "readout_directions"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'ac_crosstalk'"
-    ,description='Apply AC crosstalk signal to detector signal.'
+    title="Model 'ac_crosstalk'",
+    description="Apply AC crosstalk signal to detector signal.",
 )
 @dataclass
 class ModelReadoutElectronicsAcCrosstalk:
     name: str
     arguments: ModelReadoutElectronicsAcCrosstalkArguments
-    func: Literal['pyxel.models.readout_electronics.ac_crosstalk'] = 'pyxel.models.readout_electronics.ac_crosstalk'
+    func: Literal[
+        "pyxel.models.readout_electronics.ac_crosstalk"
+    ] = "pyxel.models.readout_electronics.ac_crosstalk"
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Dc Crosstalk
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsDcCrosstalkArguments(Mapping[str, Any]):
-    coupling_matrix: Union[str, pathlib.Path, Sequence] = field(
-        metadata=schema(
-            title='coupling_matrix'
-        )
-    )
-    channel_matrix: Sequence = field(
-        metadata=schema(
-            title='channel_matrix'
-        )
-    )
-    readout_directions: Sequence = field(
-        metadata=schema(
-            title='readout_directions'
-        )
+    coupling_matrix: Union[str, pathlib.Path, collections.abc.Sequence] = field(
+        metadata=schema(title="coupling_matrix")
     )
+    channel_matrix: Sequence = field(metadata=schema(title="channel_matrix"))
+    readout_directions: Sequence = field(metadata=schema(title="readout_directions"))
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('coupling_matrix', 'channel_matrix', 'readout_directions'))
+        return iter(("coupling_matrix", "channel_matrix", "readout_directions"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 3
 
 
 @schema(
-    title="Model 'dc_crosstalk'"
-    ,description='Apply DC crosstalk signal to detector signal.'
+    title="Model 'dc_crosstalk'",
+    description="Apply DC crosstalk signal to detector signal.",
 )
 @dataclass
 class ModelReadoutElectronicsDcCrosstalk:
     name: str
     arguments: ModelReadoutElectronicsDcCrosstalkArguments
-    func: Literal['pyxel.models.readout_electronics.dc_crosstalk'] = 'pyxel.models.readout_electronics.dc_crosstalk'
+    func: Literal[
+        "pyxel.models.readout_electronics.dc_crosstalk"
+    ] = "pyxel.models.readout_electronics.dc_crosstalk"
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Dead Time Filter
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsDeadTimeFilterArguments(Mapping[str, Any]):
     tau_0: float = field(
         default=4.4e-07,
         metadata=schema(
-            title='tau_0'
-            ,description=(
-                    'Material dependent characteristic time for the electron-phonon'
-                    'coupling. Unit: s'
-                )
-        )
+            title="tau_0",
+            description=(
+                "Material dependent characteristic time for the electron-phonon"
+                "coupling. Unit: s"
+            ),
+        ),
     )
     n_0: float = field(
         default=17200000000.0,
         metadata=schema(
-            title='n_0'
-            ,description=(
-                    'Material dependent single spin density of states at the Fermi-level.'
-                    'Unit: um^-3 eV^-1'
-                )
-        )
+            title="n_0",
+            description=(
+                "Material dependent single spin density of states at the Fermi-level."
+                "Unit: um^-3 eV^-1"
+            ),
+        ),
     )
     t_c: float = field(
         default=1.26,
         metadata=schema(
-            title='t_c'
-            ,description='Material dependent critical temperature. Unit: K'
-        )
+            title="t_c", description="Material dependent critical temperature. Unit: K"
+        ),
     )
     v: float = field(
         default=30.0,
-        metadata=schema(
-            title='v'
-            ,description='Superconducting volume. Unit: um^3'
-        )
+        metadata=schema(title="v", description="Superconducting volume. Unit: um^3"),
     )
     t_op: float = field(
-        default=0.3,
-        metadata=schema(
-            title='t_op'
-            ,description='Temperature. Unit: K'
-        )
+        default=0.3, metadata=schema(title="t_op", description="Temperature. Unit: K")
     )
     tau_pb: float = field(
         default=2.8e-10,
         metadata=schema(
-            title='tau_pb'
-            ,description='Phonon pair-breaking time. Unit: s'
-        )
+            title="tau_pb", description="Phonon pair-breaking time. Unit: s"
+        ),
     )
     tau_esc: float = field(
         default=1.4e-10,
-        metadata=schema(
-            title='tau_esc'
-            ,description='Phonon escape time. Unit: s'
-        )
+        metadata=schema(title="tau_esc", description="Phonon escape time. Unit: s"),
     )
     tau_sat: float = field(
         default=0.001,
-        metadata=schema(
-            title='tau_sat'
-            ,description='Saturation time. Unit: s'
-        )
+        metadata=schema(title="tau_sat", description="Saturation time. Unit: s"),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('tau_0', 'n_0', 't_c', 'v', 't_op', 'tau_pb', 'tau_esc', 'tau_sat'))
+        return iter(
+            ("tau_0", "n_0", "t_c", "v", "t_op", "tau_pb", "tau_esc", "tau_sat")
+        )
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 8
 
 
-@schema(
-    title="Model 'dead_time_filter'"
-    ,description='Dead time filter.'
-)
+@schema(title="Model 'dead_time_filter'", description="Dead time filter.")
 @dataclass
 class ModelReadoutElectronicsDeadTimeFilter:
     name: str
-    arguments: ModelReadoutElectronicsDeadTimeFilterArguments = field(default_factory=ModelReadoutElectronicsDeadTimeFilterArguments)
-    func: Literal['pyxel.models.readout_electronics.dead_time_filter'] = 'pyxel.models.readout_electronics.dead_time_filter'
+    arguments: ModelReadoutElectronicsDeadTimeFilterArguments = field(
+        default_factory=ModelReadoutElectronicsDeadTimeFilterArguments
+    )
+    func: Literal[
+        "pyxel.models.readout_electronics.dead_time_filter"
+    ] = "pyxel.models.readout_electronics.dead_time_filter"
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Sar Adc
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsSarAdcArguments(Mapping[str, Any]):
     def __iter__(self) -> Iterator[str]:
         return iter(())
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 0
 
 
 @schema(
-    title="Model 'sar_adc'"
-    ,description=(
-        'Digitize signal array using :term:`SAR` (Successive Approximation'
-        'Register) :term:`ADC` logic.'
-    )
+    title="Model 'sar_adc'",
+    description=(
+        "Digitize signal array using :term:`SAR` (Successive Approximation"
+        "Register) :term:`ADC` logic."
+    ),
 )
 @dataclass
 class ModelReadoutElectronicsSarAdc:
     name: str
-    arguments: ModelReadoutElectronicsSarAdcArguments = field(default_factory=ModelReadoutElectronicsSarAdcArguments)
-    func: Literal['pyxel.models.readout_electronics.sar_adc'] = 'pyxel.models.readout_electronics.sar_adc'
+    arguments: ModelReadoutElectronicsSarAdcArguments = field(
+        default_factory=ModelReadoutElectronicsSarAdcArguments
+    )
+    func: Literal[
+        "pyxel.models.readout_electronics.sar_adc"
+    ] = "pyxel.models.readout_electronics.sar_adc"
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Sar Adc With Noise
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsSarAdcWithNoiseArguments(Mapping[str, Any]):
-    strengths: Tuple[float, ...] = field(
+    strengths: tuple[float, ...] = field(
         metadata=schema(
-            title='strengths'
-            ,description=(
-                    'Sequence of ``detector.characteristics.adc_bit_resolution`` number(s).'
-                    'Unit: V'
-                )
+            title="strengths",
+            description=(
+                "Sequence of ``detector.characteristics.adc_bit_resolution`` number(s)."
+                "Unit: V"
+            ),
         )
     )
-    noises: Tuple[float, ...] = field(
+    noises: tuple[float, ...] = field(
         metadata=schema(
-            title='noises'
-            ,description=(
-                    'Sequence of ``detector.characteristics.adc_bit_resolution`` number(s).'
-                    'Unit: V'
-                )
+            title="noises",
+            description=(
+                "Sequence of ``detector.characteristics.adc_bit_resolution`` number(s)."
+                "Unit: V"
+            ),
         )
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('strengths', 'noises'))
+        return iter(("strengths", "noises"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'sar_adc_with_noise'"
-    ,description=(
-        'Digitize signal array using :term:`SAR` (Successive Approximation'
-        'Register) :term:`ADC` logic with noise.'
-    )
+    title="Model 'sar_adc_with_noise'",
+    description=(
+        "Digitize signal array using :term:`SAR` (Successive Approximation"
+        "Register) :term:`ADC` logic with noise."
+    ),
 )
 @dataclass
 class ModelReadoutElectronicsSarAdcWithNoise:
     name: str
     arguments: ModelReadoutElectronicsSarAdcWithNoiseArguments
-    func: Literal['pyxel.models.readout_electronics.sar_adc_with_noise'] = 'pyxel.models.readout_electronics.sar_adc_with_noise'
+    func: Literal[
+        "pyxel.models.readout_electronics.sar_adc_with_noise"
+    ] = "pyxel.models.readout_electronics.sar_adc_with_noise"
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Simple Adc
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsSimpleAdcArguments(Mapping[str, Any]):
-    data_type: Literal['uint16', 'uint32', 'uint64', 'uint'] = field(
-        default='uint32',
+    data_type: Literal["uint16", "uint32", "uint64", "uint"] = field(
+        default="uint32",
         metadata=schema(
-            title='data_type'
-            ,description=(
-                    'The desired data-type for the Image array. The data-type must be an'
-                    "unsigned integer. Valid values: 'uint16', 'uint32', 'uint64', 'uint'"
-                    "Invalid values: 'int16', 'int32', 'int64', 'int', 'float'..."
-                )
-        )
+            title="data_type",
+            description=(
+                "The desired data-type for the Image array. The data-type must be an"
+                "unsigned integer. Valid values: 'uint16', 'uint32', 'uint64', 'uint'"
+                "Invalid values: 'int16', 'int32', 'int64', 'int', 'float'..."
+            ),
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('data_type',))
+        return iter(("data_type",))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'simple_adc'"
-    ,description='Apply simple Analog to Digital conversion.'
+    title="Model 'simple_adc'", description="Apply simple Analog to Digital conversion."
 )
 @dataclass
 class ModelReadoutElectronicsSimpleAdc:
     name: str
-    arguments: ModelReadoutElectronicsSimpleAdcArguments = field(default_factory=ModelReadoutElectronicsSimpleAdcArguments)
-    func: Literal['pyxel.models.readout_electronics.simple_adc'] = 'pyxel.models.readout_electronics.simple_adc'
+    arguments: ModelReadoutElectronicsSimpleAdcArguments = field(
+        default_factory=ModelReadoutElectronicsSimpleAdcArguments
+    )
+    func: Literal[
+        "pyxel.models.readout_electronics.simple_adc"
+    ] = "pyxel.models.readout_electronics.simple_adc"
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Simple Amplifier
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsSimpleAmplifierArguments(Mapping[str, Any]):
     def __iter__(self) -> Iterator[str]:
         return iter(())
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 0
 
 
 @schema(
-    title="Model 'simple_amplifier'"
-    ,description=(
-        'Amplify signal using gain from the output amplifier and the signal'
-        'processor.'
-    )
+    title="Model 'simple_amplifier'",
+    description=(
+        "Amplify signal using gain from the output amplifier and the signal"
+        "processor."
+    ),
 )
 @dataclass
 class ModelReadoutElectronicsSimpleAmplifier:
     name: str
-    arguments: ModelReadoutElectronicsSimpleAmplifierArguments = field(default_factory=ModelReadoutElectronicsSimpleAmplifierArguments)
-    func: Literal['pyxel.models.readout_electronics.simple_amplifier'] = 'pyxel.models.readout_electronics.simple_amplifier'
+    arguments: ModelReadoutElectronicsSimpleAmplifierArguments = field(
+        default_factory=ModelReadoutElectronicsSimpleAmplifierArguments
+    )
+    func: Literal[
+        "pyxel.models.readout_electronics.simple_amplifier"
+    ] = "pyxel.models.readout_electronics.simple_amplifier"
     enabled: bool = True
 
 
 #
 # Model: Readout Electronics / Simple Phase Conversion
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsSimplePhaseConversionArguments(Mapping[str, Any]):
     phase_conversion: float = field(
         default=1.0,
         metadata=schema(
-            title='phase_conversion'
-            ,description='Phase conversion factor'
-        )
+            title="phase_conversion", description="Phase conversion factor"
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('phase_conversion',))
+        return iter(("phase_conversion",))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 1
 
 
 @schema(
-    title="Model 'simple_phase_conversion'"
-    ,description='Create an image array from phase array.'
+    title="Model 'simple_phase_conversion'",
+    description="Create an image array from phase array.",
 )
 @dataclass
 class ModelReadoutElectronicsSimplePhaseConversion:
     name: str
-    arguments: ModelReadoutElectronicsSimplePhaseConversionArguments = field(default_factory=ModelReadoutElectronicsSimplePhaseConversionArguments)
-    func: Literal['pyxel.models.readout_electronics.simple_phase_conversion'] = 'pyxel.models.readout_electronics.simple_phase_conversion'
+    arguments: ModelReadoutElectronicsSimplePhaseConversionArguments = field(
+        default_factory=ModelReadoutElectronicsSimplePhaseConversionArguments
+    )
+    func: Literal[
+        "pyxel.models.readout_electronics.simple_phase_conversion"
+    ] = "pyxel.models.readout_electronics.simple_phase_conversion"
     enabled: bool = True
 
 
 #
-# Model: Data Processing / Compute Statistics
+# Model: Data Processing / Extract Roi To Xarray
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
-class ModelDataProcessingComputeStatisticsArguments(Mapping[str, Any]):
-    data_structure: Literal['pixel', 'photon', 'image', 'signal'] = field(
-        default='pixel',
+class ModelDataProcessingExtractRoiToXarrayArguments(Mapping[str, Any]):
+    thresh: int = field(
+        default=50,
         metadata=schema(
-            title='data_structure'
-            ,description=(
-                    'Keyword to choose data structure. Can be any from: ("pixel", "photon",'
-                    '"image", "signal")'
-                )
-        )
+            title="thresh",
+            description="threshold above which information from the image array is extracted",
+        ),
     )
-    dimensions: Union[str, Sequence[str]] = field(
-        default=('x', 'y'),
+    minarea: int = field(
+        default=5,
         metadata=schema(
-            title='dimensions'
-            ,description='Dimensions.'
-        )
+            title="minarea",
+            description=(
+                "minimum area of elements required that are above the threshold for the"
+                "extractor to extract information"
+            ),
+        ),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('data_structure', 'dimensions'))
+        return iter(("thresh", "minarea"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'compute_statistics'"
-    ,description='Compute basic statistics.'
+    title="Model 'extract_roi_to_xarray'",
+    description=(
+        "Extract the roi data converts it to xarray dataset and saves the"
+        "information to the final result."
+    ),
 )
 @dataclass
-class ModelDataProcessingComputeStatistics:
+class ModelDataProcessingExtractRoiToXarray:
     name: str
-    arguments: ModelDataProcessingComputeStatisticsArguments = field(default_factory=ModelDataProcessingComputeStatisticsArguments)
-    func: Literal['pyxel.models.data_processing.compute_statistics'] = 'pyxel.models.data_processing.compute_statistics'
+    arguments: ModelDataProcessingExtractRoiToXarrayArguments = field(
+        default_factory=ModelDataProcessingExtractRoiToXarrayArguments
+    )
+    func: Literal[
+        "pyxel.models.data_processing.extract_roi_to_xarray"
+    ] = "pyxel.models.data_processing.extract_roi_to_xarray"
     enabled: bool = True
 
 
 #
-# Model: Data Processing / Extract Roi To Xarray
+# Model: Data Processing / Linear Regression
 #
-@schema(title='Parameters')
+@schema(title="Parameters")
 @dataclass
-class ModelDataProcessingExtractRoiToXarrayArguments(Mapping[str, Any]):
-    thresh: int = field(
-        default=50,
+class ModelDataProcessingLinearRegressionArguments(Mapping[str, Any]):
+    data_structure: Literal["pixel", "photon", "image", "signal"] = field(
+        default="image",
         metadata=schema(
-            title='thresh'
-            ,description='threshold above which information from the image array is extracted'
-        )
+            title="data_structure",
+            description="Data bucket to use for the linear regression.",
+        ),
     )
-    minarea: int = field(
-        default=5,
-        metadata=schema(
-            title='minarea'
-            ,description=(
-                    'minimum area of elements required that are above the threshold for the'
-                    'extractor to extract information'
-                )
-        )
+    name: Optional[str] = field(
+        default=None,
+        metadata=schema(title="name", description="Name to use for the result."),
     )
+
     def __iter__(self) -> Iterator[str]:
-        return iter(('thresh', 'minarea'))
+        return iter(("data_structure", "name"))
+
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
+
     def __len__(self) -> int:
         return 2
 
 
 @schema(
-    title="Model 'extract_roi_to_xarray'"
-    ,description=(
-        'Extract the roi data converts it to xarray dataset and saves the'
-        'information to the final result.'
+    title="Model 'linear_regression'",
+    description=(
+        "Compute a linear regression along 'readout_time' and store it in"
+        "'.data' bucket."
+    ),
+)
+@dataclass
+class ModelDataProcessingLinearRegression:
+    name: str
+    arguments: ModelDataProcessingLinearRegressionArguments = field(
+        default_factory=ModelDataProcessingLinearRegressionArguments
     )
+    func: Literal[
+        "pyxel.models.data_processing.linear_regression"
+    ] = "pyxel.models.data_processing.linear_regression"
+    enabled: bool = True
+
+
+#
+# Model: Data Processing / Mean Variance
+#
+@schema(title="Parameters")
+@dataclass
+class ModelDataProcessingMeanVarianceArguments(Mapping[str, Any]):
+    data_structure: Literal["pixel", "photon", "image", "signal"] = field(
+        default="image",
+        metadata=schema(
+            title="data_structure",
+            description="Data bucket to use for the linear regression.",
+        ),
+    )
+    name: Optional[str] = field(
+        default=None,
+        metadata=schema(title="name", description="Name to use for the result."),
+    )
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(("data_structure", "name"))
+
+    def __getitem__(self, item: Any) -> Any:
+        if item in tuple(self):
+            return getattr(self, item)
+        else:
+            raise KeyError
+
+    def __len__(self) -> int:
+        return 2
+
+
+@schema(
+    title="Model 'mean_variance'",
+    description="Compute mean-variance and store it in '.data' bucket.",
 )
 @dataclass
-class ModelDataProcessingExtractRoiToXarray:
+class ModelDataProcessingMeanVariance:
     name: str
-    arguments: ModelDataProcessingExtractRoiToXarrayArguments = field(default_factory=ModelDataProcessingExtractRoiToXarrayArguments)
-    func: Literal['pyxel.models.data_processing.extract_roi_to_xarray'] = 'pyxel.models.data_processing.extract_roi_to_xarray'
+    arguments: ModelDataProcessingMeanVarianceArguments = field(
+        default_factory=ModelDataProcessingMeanVarianceArguments
+    )
+    func: Literal[
+        "pyxel.models.data_processing.mean_variance"
+    ] = "pyxel.models.data_processing.mean_variance"
+    enabled: bool = True
+
+
+#
+# Model: Data Processing / Statistics
+#
+@schema(title="Parameters")
+@dataclass
+class ModelDataProcessingStatisticsArguments(Mapping[str, Any]):
+    data_structure: Literal["pixel", "photon", "signal", "image", "all"] = field(
+        default="all",
+        metadata=schema(
+            title="data_structure",
+            description=(
+                'Keyword to choose data structure. Can be any from: ("pixel", "photon",'
+                '"signal", "image", "all"). Default is "all" and computes the'
+                'statistics on "pixel", "photon", "signal" and "image".'
+            ),
+        ),
+    )
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(("data_structure",))
+
+    def __getitem__(self, item: Any) -> Any:
+        if item in tuple(self):
+            return getattr(self, item)
+        else:
+            raise KeyError
+
+    def __len__(self) -> int:
+        return 1
+
+
+@schema(title="Model 'statistics'", description="Compute basic statistics.")
+@dataclass
+class ModelDataProcessingStatistics:
+    name: str
+    arguments: ModelDataProcessingStatisticsArguments = field(
+        default_factory=ModelDataProcessingStatisticsArguments
+    )
+    func: Literal[
+        "pyxel.models.data_processing.statistics"
+    ] = "pyxel.models.data_processing.statistics"
     enabled: bool = True
 
 
 #
 # Detection pipeline
 #
 @dataclass
 class DetailedDetectionPipeline(DetectionPipeline):
     scene_generation: Optional[
         Sequence[Union[ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Scene Generation'))
+    ] = field(default=None, metadata=schema(title="Scene Generation"))
     photon_collection: Optional[
-        Sequence[Union[ModelPhotonCollectionIllumination, ModelPhotonCollectionLoadImage, ModelPhotonCollectionLoadPsf, ModelPhotonCollectionOpticalPsf, ModelPhotonCollectionShotNoise, ModelPhotonCollectionStripePattern, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Photon Collection'))
+        Sequence[
+            Union[
+                ModelPhotonCollectionIllumination,
+                ModelPhotonCollectionLoadImage,
+                ModelPhotonCollectionLoadPsf,
+                ModelPhotonCollectionOpticalPsf,
+                ModelPhotonCollectionShotNoise,
+                ModelPhotonCollectionStripePattern,
+                ModelLoadDetector,
+                ModelSaveDetector,
+                ModelFunction,
+            ]
+        ]
+    ] = field(default=None, metadata=schema(title="Photon Collection"))
     photon_generation: Optional[
-        Sequence[Union[ModelPhotonGenerationIllumination, ModelPhotonGenerationLoadImage, ModelPhotonGenerationShotNoise, ModelPhotonGenerationStripePattern, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Photon Generation'))
+        Sequence[
+            Union[
+                ModelPhotonGenerationIllumination,
+                ModelPhotonGenerationLoadImage,
+                ModelPhotonGenerationShotNoise,
+                ModelPhotonGenerationStripePattern,
+                ModelLoadDetector,
+                ModelSaveDetector,
+                ModelFunction,
+            ]
+        ]
+    ] = field(default=None, metadata=schema(title="Photon Generation"))
     optics: Optional[
-        Sequence[Union[ModelOpticsLoadPsf, ModelOpticsOpticalPsf, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Optics'))
+        Sequence[
+            Union[
+                ModelOpticsLoadPsf,
+                ModelOpticsOpticalPsf,
+                ModelLoadDetector,
+                ModelSaveDetector,
+                ModelFunction,
+            ]
+        ]
+    ] = field(default=None, metadata=schema(title="Optics"))
     phasing: Optional[
-        Sequence[Union[ModelPhasingPulseProcessing, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Phasing'))
+        Sequence[
+            Union[
+                ModelPhasingPulseProcessing,
+                ModelLoadDetector,
+                ModelSaveDetector,
+                ModelFunction,
+            ]
+        ]
+    ] = field(default=None, metadata=schema(title="Phasing"))
     charge_generation: Optional[
-        Sequence[Union[ModelChargeGenerationApdGain, ModelChargeGenerationChargeBlocks, ModelChargeGenerationChargeDeposition, ModelChargeGenerationChargeDepositionInMct, ModelChargeGenerationConversionWithQeMap, ModelChargeGenerationCosmix, ModelChargeGenerationDarkCurrent, ModelChargeGenerationDarkCurrentRule07, ModelChargeGenerationDarkCurrentSaphira, ModelChargeGenerationLoadCharge, ModelChargeGenerationSimpleConversion, ModelChargeGenerationSimpleDarkCurrent, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Charge Generation'))
+        Sequence[
+            Union[
+                ModelChargeGenerationApdGain,
+                ModelChargeGenerationChargeBlocks,
+                ModelChargeGenerationChargeDeposition,
+                ModelChargeGenerationChargeDepositionInMct,
+                ModelChargeGenerationConversionWithQeMap,
+                ModelChargeGenerationCosmix,
+                ModelChargeGenerationDarkCurrent,
+                ModelChargeGenerationDarkCurrentRule07,
+                ModelChargeGenerationDarkCurrentSaphira,
+                ModelChargeGenerationLoadCharge,
+                ModelChargeGenerationSimpleConversion,
+                ModelChargeGenerationSimpleDarkCurrent,
+                ModelLoadDetector,
+                ModelSaveDetector,
+                ModelFunction,
+            ]
+        ]
+    ] = field(default=None, metadata=schema(title="Charge Generation"))
     charge_collection: Optional[
-        Sequence[Union[ModelChargeCollectionFixedPatternNoise, ModelChargeCollectionPersistence, ModelChargeCollectionSimpleCollection, ModelChargeCollectionSimpleFullWell, ModelChargeCollectionSimpleIpc, ModelChargeCollectionSimplePersistence, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Charge Collection'))
+        Sequence[
+            Union[
+                ModelChargeCollectionFixedPatternNoise,
+                ModelChargeCollectionPersistence,
+                ModelChargeCollectionSimpleCollection,
+                ModelChargeCollectionSimpleFullWell,
+                ModelChargeCollectionSimpleIpc,
+                ModelChargeCollectionSimplePersistence,
+                ModelLoadDetector,
+                ModelSaveDetector,
+                ModelFunction,
+            ]
+        ]
+    ] = field(default=None, metadata=schema(title="Charge Collection"))
     charge_transfer: Optional[
-        Sequence[Union[ModelChargeTransferArcticAdd, ModelChargeTransferArcticRemove, ModelChargeTransferCdm, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Charge Transfer'))
+        Sequence[
+            Union[
+                ModelChargeTransferArcticAdd,
+                ModelChargeTransferArcticRemove,
+                ModelChargeTransferCdm,
+                ModelLoadDetector,
+                ModelSaveDetector,
+                ModelFunction,
+            ]
+        ]
+    ] = field(default=None, metadata=schema(title="Charge Transfer"))
     charge_measurement: Optional[
-        Sequence[Union[ModelChargeMeasurementDcOffset, ModelChargeMeasurementKtcNoise, ModelChargeMeasurementNghxrg, ModelChargeMeasurementOutputNodeLinearityPoly, ModelChargeMeasurementOutputNodeNoise, ModelChargeMeasurementOutputNodeNoiseCmos, ModelChargeMeasurementOutputPixelResetVoltageApd, ModelChargeMeasurementPhysicalNonLinearity, ModelChargeMeasurementPhysicalNonLinearityWithSaturation, ModelChargeMeasurementReadoutNoiseSaphira, ModelChargeMeasurementSimpleMeasurement, ModelChargeMeasurementSimplePhysicalNonLinearity, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Charge Measurement'))
+        Sequence[
+            Union[
+                ModelChargeMeasurementDcOffset,
+                ModelChargeMeasurementKtcNoise,
+                ModelChargeMeasurementNghxrg,
+                ModelChargeMeasurementOutputNodeLinearityPoly,
+                ModelChargeMeasurementOutputNodeNoise,
+                ModelChargeMeasurementOutputNodeNoiseCmos,
+                ModelChargeMeasurementOutputPixelResetVoltageApd,
+                ModelChargeMeasurementPhysicalNonLinearity,
+                ModelChargeMeasurementPhysicalNonLinearityWithSaturation,
+                ModelChargeMeasurementReadoutNoiseSaphira,
+                ModelChargeMeasurementSimpleMeasurement,
+                ModelChargeMeasurementSimplePhysicalNonLinearity,
+                ModelLoadDetector,
+                ModelSaveDetector,
+                ModelFunction,
+            ]
+        ]
+    ] = field(default=None, metadata=schema(title="Charge Measurement"))
     signal_transfer: Optional[
         Sequence[Union[ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Signal Transfer'))
+    ] = field(default=None, metadata=schema(title="Signal Transfer"))
     readout_electronics: Optional[
-        Sequence[Union[ModelReadoutElectronicsAcCrosstalk, ModelReadoutElectronicsDcCrosstalk, ModelReadoutElectronicsDeadTimeFilter, ModelReadoutElectronicsSarAdc, ModelReadoutElectronicsSarAdcWithNoise, ModelReadoutElectronicsSimpleAdc, ModelReadoutElectronicsSimpleAmplifier, ModelReadoutElectronicsSimplePhaseConversion, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Readout Electronics'))
+        Sequence[
+            Union[
+                ModelReadoutElectronicsAcCrosstalk,
+                ModelReadoutElectronicsDcCrosstalk,
+                ModelReadoutElectronicsDeadTimeFilter,
+                ModelReadoutElectronicsSarAdc,
+                ModelReadoutElectronicsSarAdcWithNoise,
+                ModelReadoutElectronicsSimpleAdc,
+                ModelReadoutElectronicsSimpleAmplifier,
+                ModelReadoutElectronicsSimplePhaseConversion,
+                ModelLoadDetector,
+                ModelSaveDetector,
+                ModelFunction,
+            ]
+        ]
+    ] = field(default=None, metadata=schema(title="Readout Electronics"))
     data_processing: Optional[
-        Sequence[Union[ModelDataProcessingComputeStatistics, ModelDataProcessingExtractRoiToXarray, ModelLoadDetector, ModelSaveDetector, ModelFunction]]
-    ] = field(default=None, metadata=schema(title='Data Processing'))
-@schema(
-    title='Environment',
-    description='Environmental attributes of the detector.'
-)
+        Sequence[
+            Union[
+                ModelDataProcessingExtractRoiToXarray,
+                ModelDataProcessingLinearRegression,
+                ModelDataProcessingMeanVariance,
+                ModelDataProcessingStatistics,
+                ModelLoadDetector,
+                ModelSaveDetector,
+                ModelFunction,
+            ]
+        ]
+    ] = field(default=None, metadata=schema(title="Data Processing"))
+
+
+@schema(title="Environment", description="Environmental attributes of the detector.")
 @dataclass(kw_only=True)  # Python 3.10+
 class Environment:
     temperature: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='temperature',
-            description='Temperature of the detector. Unit: K'
-        )
+            title="temperature", description="Temperature of the detector. Unit: K"
+        ),
     )
 
 
 @schema(
-    title='Characteristics',
-    description='Characteristic attributes of the detector.'
+    title="Characteristics", description="Characteristic attributes of the detector."
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class Characteristics:
     quantum_efficiency: Optional[float] = field(
         default=None,
-        metadata=schema(
-            title='quantum_efficiency',
-            description='Quantum efficiency.'
-        )
+        metadata=schema(title="quantum_efficiency", description="Quantum efficiency."),
     )
     charge_to_volt_conversion: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='charge_to_volt_conversion',
-            description='Sensitivity of charge readout. Unit: V/e-'
-        )
+            title="charge_to_volt_conversion",
+            description="Sensitivity of charge readout. Unit: V/e-",
+        ),
     )
     pre_amplification: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='pre_amplification',
-            description='Gain of pre-amplifier. Unit: V/V'
-        )
+            title="pre_amplification", description="Gain of pre-amplifier. Unit: V/V"
+        ),
     )
     full_well_capacity: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='full_well_capacity',
-            description='Full well capacity. Unit: e-'
-        )
+            title="full_well_capacity", description="Full well capacity. Unit: e-"
+        ),
     )
-    adc_voltage_range: Optional[Tuple[float, float]] = field(
+    adc_voltage_range: Optional[tuple[float, float]] = field(
         default=None,
         metadata=schema(
-            title='adc_voltage_range',
-            description='ADC voltage range. Unit: V'
-        )
+            title="adc_voltage_range", description="ADC voltage range. Unit: V"
+        ),
     )
     adc_bit_resolution: Optional[int] = field(
         default=None,
-        metadata=schema(
-            title='adc_bit_resolution',
-            description='ADC bit resolution.'
-        )
+        metadata=schema(title="adc_bit_resolution", description="ADC bit resolution."),
     )
 
 
-@schema(
-    title='Geometry',
-    description='Geometrical attributes of the detector.'
-)
+@schema(title="Geometry", description="Geometrical attributes of the detector.")
 @dataclass(kw_only=True)  # Python 3.10+
 class Geometry:
-    row: int = field(
-        metadata=schema(
-            title='row',
-            description='Number of pixel rows.'
-        )
-    )
+    row: int = field(metadata=schema(title="row", description="Number of pixel rows."))
     col: int = field(
-        metadata=schema(
-            title='col',
-            description='Number of pixel columns.'
-        )
+        metadata=schema(title="col", description="Number of pixel columns.")
     )
     total_thickness: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='total_thickness',
-            description='Thickness of detector. Unit: um'
-        )
+            title="total_thickness", description="Thickness of detector. Unit: um"
+        ),
     )
     pixel_vert_size: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='pixel_vert_size',
-            description='Vertical dimension of pixel. Unit: um'
-        )
+            title="pixel_vert_size", description="Vertical dimension of pixel. Unit: um"
+        ),
     )
     pixel_horz_size: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='pixel_horz_size',
-            description='Horizontal dimension of pixel. Unit: um'
-        )
+            title="pixel_horz_size",
+            description="Horizontal dimension of pixel. Unit: um",
+        ),
     )
 
 
 @schema(
-    title='APDCharacteristics',
-    description='Characteristic attributes of the APD detector.'
+    title="APDCharacteristics",
+    description="Characteristic attributes of the APD detector.",
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class APDCharacteristics:
     roic_gain: float = field(
         metadata=schema(
-            title='roic_gain',
-            description='Gain of the read-out integrated circuit. Unit: V/V'
+            title="roic_gain",
+            description="Gain of the read-out integrated circuit. Unit: V/V",
         )
     )
     quantum_efficiency: Optional[float] = field(
         default=None,
-        metadata=schema(
-            title='quantum_efficiency',
-            description='Quantum efficiency.'
-        )
+        metadata=schema(title="quantum_efficiency", description="Quantum efficiency."),
     )
     full_well_capacity: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='full_well_capacity',
-            description='Full well capacity. Unit: e-'
-        )
+            title="full_well_capacity", description="Full well capacity. Unit: e-"
+        ),
     )
     adc_bit_resolution: Optional[int] = field(
         default=None,
-        metadata=schema(
-            title='adc_bit_resolution',
-            description='ADC bit resolution.'
-        )
+        metadata=schema(title="adc_bit_resolution", description="ADC bit resolution."),
     )
-    adc_voltage_range: Optional[Tuple[float, float]] = field(
+    adc_voltage_range: Optional[tuple[float, float]] = field(
         default=None,
         metadata=schema(
-            title='adc_voltage_range',
-            description='ADC voltage range. Unit: V'
-        )
+            title="adc_voltage_range", description="ADC voltage range. Unit: V"
+        ),
     )
     avalanche_gain: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='avalanche_gain',
-            description='APD gain. Unit: electron/electron'
-        )
+            title="avalanche_gain", description="APD gain. Unit: electron/electron"
+        ),
     )
     pixel_reset_voltage: Optional[float] = field(
         default=None,
         metadata=schema(
-            title='pixel_reset_voltage',
+            title="pixel_reset_voltage",
             description=(
-                    'DC voltage going into the detector, not the voltage of a reset pixel.'
-                    'Unit: V'
-                )
-        )
+                "DC voltage going into the detector, not the voltage of a reset pixel."
+                "Unit: V"
+            ),
+        ),
     )
     common_voltage: Optional[float] = field(
         default=None,
-        metadata=schema(
-            title='common_voltage',
-            description='Common voltage. Unit: V'
-        )
+        metadata=schema(title="common_voltage", description="Common voltage. Unit: V"),
     )
 
 
-@schema(
-    title='Detector',
-    description='The detector class.'
-)
+@schema(title="Detector", description="The detector class.")
 @dataclass(kw_only=True)  # Python 3.10+
 class Detector:
     environment: Optional[Environment] = field(
-        default=None,
-        metadata=schema(
-            title='environment'
-        )
+        default=None, metadata=schema(title="environment")
     )
 
 
 @schema(
-    title='CCDGeometry',
-    description='Geometrical attributes of a :term:`CCD` detector.'
+    title="CCDGeometry", description="Geometrical attributes of a :term:`CCD` detector."
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class CCDGeometry(Geometry):
     pass
 
 
 @schema(
-    title='CMOSGeometry',
-    description='Geometrical attributes of a :term:`CMOS`-based detector.'
+    title="CMOSGeometry",
+    description="Geometrical attributes of a :term:`CMOS`-based detector.",
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class CMOSGeometry(Geometry):
     pass
 
 
 @schema(
-    title='MKIDGeometry',
-    description='Geometrical attributes of a :term:`MKID`-based detector.'
+    title="MKIDGeometry",
+    description="Geometrical attributes of a :term:`MKID`-based detector.",
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class MKIDGeometry(Geometry):
     pass
 
 
 @schema(
-    title='APDGeometry',
-    description='Geometrical attributes of a :term:`APD`-based detector.'
+    title="APDGeometry",
+    description="Geometrical attributes of a :term:`APD`-based detector.",
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class APDGeometry(Geometry):
     pass
 
 
 @schema(
-    title='CCD',
+    title="CCD",
     description=(
-        'Charge-Coupled Device class containing all detector attributes and'
-        'data.'
-        )
+        "Charge-Coupled Device class containing all detector attributes and" "data."
+    ),
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class CCD(Detector):
-    geometry: CCDGeometry = field(
-        metadata=schema(
-            title='geometry'
-        )
-    )
-    characteristics: Characteristics = field(
-        metadata=schema(
-            title='characteristics'
-        )
-    )
+    geometry: CCDGeometry = field(metadata=schema(title="geometry"))
+    characteristics: Characteristics = field(metadata=schema(title="characteristics"))
 
 
 @schema(
-    title='CMOS',
+    title="CMOS",
     description=(
-        ':term:`CMOS`-based detector class containing all detector attributes'
-        'and data.'
-        )
+        ":term:`CMOS`-based detector class containing all detector attributes"
+        "and data."
+    ),
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class CMOS(Detector):
-    geometry: CMOSGeometry = field(
-        metadata=schema(
-            title='geometry'
-        )
-    )
-    characteristics: Characteristics = field(
-        metadata=schema(
-            title='characteristics'
-        )
-    )
+    geometry: CMOSGeometry = field(metadata=schema(title="geometry"))
+    characteristics: Characteristics = field(metadata=schema(title="characteristics"))
 
 
 @schema(
-    title='MKID',
+    title="MKID",
     description=(
-        ':term:`MKID`-based detector class containing all detector attributes'
-        'and data.'
-        )
+        ":term:`MKID`-based detector class containing all detector attributes"
+        "and data."
+    ),
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class MKID(Detector):
-    geometry: MKIDGeometry = field(
-        metadata=schema(
-            title='geometry'
-        )
-    )
-    characteristics: Characteristics = field(
-        metadata=schema(
-            title='characteristics'
-        )
-    )
+    geometry: MKIDGeometry = field(metadata=schema(title="geometry"))
+    characteristics: Characteristics = field(metadata=schema(title="characteristics"))
 
 
 @schema(
-    title='APD',
+    title="APD",
     description=(
-        ':term:`CMOS`-based detector class containing all detector attributes'
-        'and data.'
-        )
+        ":term:`CMOS`-based detector class containing all detector attributes"
+        "and data."
+    ),
 )
 @dataclass(kw_only=True)  # Python 3.10+
 class APD(Detector):
-    geometry: APDGeometry = field(
-        metadata=schema(
-            title='geometry'
-        )
-    )
+    geometry: APDGeometry = field(metadata=schema(title="geometry"))
     characteristics: APDCharacteristics = field(
-        metadata=schema(
-            title='characteristics'
-        )
+        metadata=schema(title="characteristics")
     )
 
 
-
 #
 # Outputs
 #
 ValidName = Literal[
-    'detector.image.array', 'detector.signal.array', 'detector.pixel.array'
+    "detector.image.array", "detector.signal.array", "detector.pixel.array"
 ]
-ValidFormat = Literal['fits', 'hdf', 'npy', 'txt', 'csv', 'png', 'jpg', 'jpeg']
+ValidFormat = Literal["fits", "hdf", "npy", "txt", "csv", "png", "jpg", "jpeg"]
 
 
 @dataclass
 class Outputs:
     output_folder: pathlib.Path
     save_data_to_file: Optional[
         Sequence[Mapping[ValidName, Sequence[ValidFormat]]]
@@ -3787,177 +4082,196 @@
 
 
 #
 # Exposure
 #
 @dataclass
 class ExposureOutputs(Outputs):
-    save_exposure_data: Optional[
-        Sequence[Mapping[str, Sequence[str]]]
-    ] = None
+    save_exposure_data: Optional[Sequence[Mapping[str, Sequence[str]]]] = None
+
+
 @dataclass
 class Readout:
     times: Union[Sequence, str, None] = None
     times_from_file: Optional[str] = None
     start_time: float = 0.0
     non_destructive: bool = False
 
 
-@schema(title='Exposure')
+@schema(title="Exposure")
 @dataclass
 class Exposure:
     outputs: ExposureOutputs
     readout: Readout = field(default_factory=Readout)
-    result_type: Literal['image', 'signal', 'pixel', 'all'] = 'all'
+    result_type: Literal["image", "signal", "pixel", "all"] = "all"
     pipeline_seed: Optional[int] = None
 
 
 #
 # Observation
 #
 
 
 @dataclass
 class ObservationOutputs(Outputs):
-    save_observation_data: Optional[
-        Sequence[Mapping[str, Sequence[str]]]
-    ] = None
+    save_observation_data: Optional[Sequence[Mapping[str, Sequence[str]]]] = None
 
 
 @dataclass
 class ParameterValues:
     key: str
     values: Union[
-        Literal['_'],
-        Sequence[Literal['_']],
+        Literal["_"],
+        Sequence[Literal["_"]],
         Sequence[Union[int, float]],
         Sequence[Sequence[Union[int, float]]],
         Sequence[Sequence[Sequence[Union[int, float]]]],
         Sequence[str],
-        str, # e.g. 'numpy.unique(...)'
+        str,  # e.g. 'numpy.unique(...)'
     ]
     boundaries: Union[Tuple[float, float], Sequence[Tuple[float, float]], None] = None
     enabled: bool = True
     logarithmic: bool = False
 
 
-@schema(title='Observation')
+@schema(title="Observation")
 @dataclass
 class Observation:
     outputs: ObservationOutputs
     parameters: Sequence[ParameterValues]
     readout: Optional[Readout] = None
-    mode: Literal['product', 'sequential', 'custom'] = 'product'
+    mode: Literal["product", "sequential", "custom"] = "product"
     from_file: Optional[str] = None
     column_range: Optional[Tuple[int, int]] = None
     with_dask: bool = False
-    result_type: Literal['image', 'signal', 'pixel', 'all'] = 'all'
+    result_type: Literal["image", "signal", "pixel", "all"] = "all"
     pipeline_seed: Optional[int] = None
 
 
 #
 # Calibration
 #
 @dataclass
 class CalibrationOutputs(Outputs):
-    save_calibration_data: Optional[
-        Sequence[Mapping[str, Sequence[str]]]
-    ] = None
+    save_calibration_data: Optional[Sequence[Mapping[str, Sequence[str]]]] = None
 
 
 @dataclass
 class Algorithm:
-    type: Literal['sade', 'sga', 'nlopt'] = 'sade'
+    type: Literal["sade", "sga", "nlopt"] = "sade"
     generations: int = 1
     population_size: int = 1
     # SADE #####
     variant: int = 2
     variant_adptv: int = 1
     ftol: float = 1e-6
     xtol: float = 1e-6
     memory: bool = False
     # SGA #####
     cr: float = 0.9
     eta_c: float = 1.0
     m: float = 0.02
     param_m: float = 1.0
     param_s: int = 2
-    crossover: Literal['single', 'exponential', 'binominal', 'sbx'] = 'exponential'
-    mutation: Literal['uniform', 'gaussian', 'polynomial'] = 'polynomial'
-    selection: Literal['tournament', 'truncated'] = 'tournament'
+    crossover: Literal["single", "exponential", "binominal", "sbx"] = "exponential"
+    mutation: Literal["uniform", "gaussian", "polynomial"] = "polynomial"
+    selection: Literal["tournament", "truncated"] = "tournament"
     # NLOPT #####
     nlopt_solver: Literal[
-        'cobyla', 'bobyqa', 'newuoa', 'newuoa_bound', 'praxis', 'neldermead',
-        'sbplx', 'mma', 'ccsaq', 'slsqp', 'lbfgs', 'tnewton_precond_restart',
-        'tnewton_precond', 'tnewton_restart', 'tnewton', 'var2', 'var1', 'auglag',
-        'auglag_eq'
-    ] = 'neldermead'
+        "cobyla",
+        "bobyqa",
+        "newuoa",
+        "newuoa_bound",
+        "praxis",
+        "neldermead",
+        "sbplx",
+        "mma",
+        "ccsaq",
+        "slsqp",
+        "lbfgs",
+        "tnewton_precond_restart",
+        "tnewton_precond",
+        "tnewton_restart",
+        "tnewton",
+        "var2",
+        "var1",
+        "auglag",
+        "auglag_eq",
+    ] = "neldermead"
     maxtime: int = 0
     maxeval: int = 0
     xtol_rel: float = 1.0e-8
     xtol_abs: float = 0.0
     ftol_rel: float = 0.0
     ftol_abs: float = 0.0
     stopval: Optional[float] = None
     # local_optimizer: Optional['pg.nlopt'] = None
-    replacement: Literal['best', 'worst', 'random'] = 'best'
-    nlopt_selection: Literal['best', 'worst', 'random'] = 'best'
+    replacement: Literal["best", "worst", "random"] = "best"
+    nlopt_selection: Literal["best", "worst", "random"] = "best"
 
 
-@schema(title='Fitness function')
+@schema(title="Fitness function")
 @dataclass
 class FitnessFunction:
     func: str
 
 
-@schema(title='Calibration')
+@schema(title="Calibration")
 @dataclass
 class Calibration:
     outputs: CalibrationOutputs
     target_data_path: Sequence[pathlib.Path]
     fitness_function: FitnessFunction
     algorithm: Algorithm
     parameters: Sequence[ParameterValues]
     readout: Optional[Readout] = None
-    mode: Literal['pipeline', 'single_model'] = 'pipeline'
-    result_type: Literal['image', 'signal', 'pixel'] = 'image'
+    mode: Literal["pipeline", "single_model"] = "pipeline"
+    result_type: Literal["image", "signal", "pixel"] = "image"
     result_fit_range: Optional[Sequence[int]] = None
     result_input_arguments: Optional[Sequence[ParameterValues]] = None
     target_fit_range: Optional[Sequence[int]] = None
     pygmo_seed: Optional[int] = None
     pipeline_seed: Optional[int] = None
     num_islands: int = 1
     num_evolutions: int = 1
     num_best_decisions: Optional[int] = None
-    topology: Literal['unconnected', 'ring', 'fully_connected'] = 'unconnected'
+    topology: Literal["unconnected", "ring", "fully_connected"] = "unconnected"
     type_islands: Literal[
-        'multiprocessing', 'multithreading', 'ipyparallel'
-    ] = 'multiprocessing'
+        "multiprocessing", "multithreading", "ipyparallel"
+    ] = "multiprocessing"
     weights_from_file: Optional[Sequence[pathlib.Path]] = None
     weights: Optional[Sequence[float]] = None
 
 
-
 @dataclass
 class Configuration:
     pipeline: DetailedDetectionPipeline
 
     # Running modes
-    exposure: Optional[Exposure] = field(default=None, metadata=schema(title='Exposure'))
-    observation: Optional[Observation] = field(default=None, metadata=schema(title='Observation'))
-    calibration: Optional[Calibration] = field(default=None, metadata=schema(title='Calibration'))
+    exposure: Optional[Exposure] = field(
+        default=None, metadata=schema(title="Exposure")
+    )
+    observation: Optional[Observation] = field(
+        default=None, metadata=schema(title="Observation")
+    )
+    calibration: Optional[Calibration] = field(
+        default=None, metadata=schema(title="Calibration")
+    )
 
     # Detectors
-    ccd_detector: Optional[CCD] = field(default=None, metadata=schema(title='CCD'))
-    cmos_detector: Optional[CMOS] = field(default=None, metadata=schema(title='CMOS'))
-    mkid_detector: Optional[MKID] = field(default=None, metadata=schema(title='MKID'))
-    apd_detector: Optional[APD] = field(default=None, metadata=schema(title='APD'))
+    ccd_detector: Optional[CCD] = field(default=None, metadata=schema(title="CCD"))
+    cmos_detector: Optional[CMOS] = field(default=None, metadata=schema(title="CMOS"))
+    mkid_detector: Optional[MKID] = field(default=None, metadata=schema(title="MKID"))
+    apd_detector: Optional[APD] = field(default=None, metadata=schema(title="APD"))
+
+
 class NotEqualError(Exception):
     ...
 
+
 def compare(first, second) -> None:
     if type(first) != type(second):
         raise NotEqualError
 
     if isinstance(first, dict) and isinstance(second, dict):
         if set(first) != set(second):
             raise NotEqualError
@@ -3978,55 +4292,59 @@
     else:
         if first != second:
             raise NotEqualError
 
 
 @click.command()
 @click.option(
-    '-f',
-    '--filename',
-    default='../../static/pyxel_schema.json',
+    "-f",
+    "--filename",
+    default="../../static/pyxel_schema.json",
     type=click.Path(),
-    help='JSON schema filename',
+    help="JSON schema filename",
     show_default=True,
 )
-@click.option('--check', is_flag=True,
-     help="Don't write the JSON Schema back, just return the status.")
+@click.option(
+    "--check",
+    is_flag=True,
+    help="Don't write the JSON Schema back, just return the status.",
+)
 def create_json_schema(filename: pathlib.Path, check: bool):
     if sys.version_info < (3, 10):
-        raise NotImplementedError('This script must run on Python 3.10+')
+        raise NotImplementedError("This script must run on Python 3.10+")
 
     # Manually define a 'format' for JSON Schema for 'Path'
-    schema(format='uri')(Path)
+    schema(format="uri")(Path)
 
     dct_schema = deserialization_schema(
-        Configuration, version=JsonSchemaVersion.DRAFT_7, all_refs=True,
+        Configuration,
+        version=JsonSchemaVersion.DRAFT_7,
+        all_refs=True,
     )
 
-
     full_filename = pathlib.Path(filename).resolve()
 
     if check:
         with full_filename.open() as fh:
             dct_reference = json.load(fh)
 
         new_dct_schema: Mapping[str, Any] = json.loads(json.dumps(dct_schema))
 
         try:
-           compare(dct_reference, new_dct_schema)
+            compare(dct_reference, new_dct_schema)
         except NotEqualError:
             print(
                 f"Error, JSON Schema file: {full_filename} is not the newest version. "
                 f"Please run 'tox -e json_schema'"
-             )
+            )
             pprint(result)
             sys.exit(1)
         else:
             sys.exit(0)
     else:
         print(json.dumps(dct_schema))
-        with full_filename.open('w') as fh:
+        with full_filename.open("w") as fh:
             json.dump(obj=dct_schema, fp=fh, indent=2, sort_keys=True)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     create_json_schema()
```

### Comparing `pyxel_sim-1.8/continuous_integration/scripts/copy_auto_generated.py` & `pyxel_sim-1.9/continuous_integration/scripts/before_auto_generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 #  the terms contained in the file ‘LICENCE.txt’.
 
 ######################################
 # Note: This code is auto-generated. #
 #       Don't modify it !            #
 ######################################
 
+import collections
 import json
 import pathlib
 import sys
 from dataclasses import dataclass, field
 from pathlib import Path
 from pprint import pprint
 from typing import Any, Iterator, Literal, Mapping, Optional, Sequence, Tuple, Union
 
-import attrs
 import click
 from apischema import schema
 from apischema.json_schema import JsonSchemaVersion, deserialization_schema
-from deepdiff import DeepDiff
 
 
 @schema(title="Parameters")
 @dataclass
 class ModelLoadSaveDetectorArguments(Mapping[str, Any]):
     filename: float = field(
         metadata=schema(title="filename", description="Filename to load/save.")
@@ -61,14 +60,15 @@
 class ModelGroup:
     models: Sequence[ModelFunction]
     name: str
 
 
 @dataclass
 class DetectionPipeline:
+    scene_generation: Optional[Sequence[ModelFunction]] = None
     photon_collection: Optional[Sequence[ModelFunction]] = None
     photon_generation: Optional[Sequence[ModelFunction]] = None
     optics: Optional[Sequence[ModelFunction]] = None
     phasing: Optional[Sequence[ModelFunction]] = None
     charge_generation: Optional[Sequence[ModelFunction]] = None
     charge_collection: Optional[Sequence[ModelFunction]] = None
     charge_transfer: Optional[Sequence[ModelFunction]] = None
@@ -94,25 +94,25 @@
             description=(
                 "A string indicating the type of illumination: - ``uniform`` Uniformly"
                 "fill the entire array with photon. (Default) - ``elliptic`` Mask with"
                 "elliptic object. - ``rectangular`` Mask with rectangular object."
             ),
         ),
     )
-    object_size: Optional[Sequence[int]] = field(
+    object_size: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
             title="object_size",
             description=(
                 "List or tuple of length 2, integers defining the diameters of the"
                 "elliptic or rectangular object in vertical and horizontal directions."
             ),
         ),
     )
-    object_center: Optional[Sequence[int]] = field(
+    object_center: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
             title="object_center",
             description=(
                 "List or tuple of length 2, two integers (row and column number),"
                 "defining the coordinates of the center of the elliptic or rectangular"
                 "object."
@@ -162,15 +162,15 @@
 #
 @schema(title="Parameters")
 @dataclass
 class ModelPhotonCollectionLoadImageArguments(Mapping[str, Any]):
     image_file: str = field(
         metadata=schema(title="image_file", description="Path to image file.")
     )
-    position: Tuple[int, int] = field(
+    position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
             title="position",
             description=(
                 "Indices of starting row and column, used when fitting image to"
                 "detector."
             ),
@@ -329,15 +329,15 @@
             title="pixelscale",
             description=(
                 "Pixel scale on detector plane (arcsec/pixel). Defines sampling"
                 "resolution of :term:`PSF`."
             ),
         )
     )
-    optical_system: Sequence[Mapping[str, Any]] = field(
+    optical_system: collections.abc.Sequence[collections.abc.Mapping[str, Any]] = field(
         metadata=schema(
             title="optical_system",
             description=(
                 "List of optical elements before detector with their specific"
                 "arguments."
             ),
         )
@@ -497,25 +497,25 @@
             description=(
                 "A string indicating the type of illumination: - ``uniform`` Uniformly"
                 "fill the entire array with photon. (Default) - ``elliptic`` Mask with"
                 "elliptic object. - ``rectangular`` Mask with rectangular object."
             ),
         ),
     )
-    object_size: Optional[Sequence[int]] = field(
+    object_size: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
             title="object_size",
             description=(
                 "List or tuple of length 2, integers defining the diameters of the"
                 "elliptic or rectangular object in vertical and horizontal directions."
             ),
         ),
     )
-    object_center: Optional[Sequence[int]] = field(
+    object_center: Optional[collections.abc.Sequence[int]] = field(
         default=None,
         metadata=schema(
             title="object_center",
             description=(
                 "List or tuple of length 2, two integers (row and column number),"
                 "defining the coordinates of the center of the elliptic or rectangular"
                 "object."
@@ -565,15 +565,15 @@
 #
 @schema(title="Parameters")
 @dataclass
 class ModelPhotonGenerationLoadImageArguments(Mapping[str, Any]):
     image_file: str = field(
         metadata=schema(title="image_file", description="Path to image file.")
     )
-    position: Tuple[int, int] = field(
+    position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
             title="position",
             description=(
                 "Indices of starting row and column, used when fitting image to"
                 "detector."
             ),
@@ -841,15 +841,15 @@
             title="pixelscale",
             description=(
                 "Pixel scale on detector plane (arcsec/pixel). Defines sampling"
                 "resolution of :term:`PSF`."
             ),
         )
     )
-    optical_system: Sequence[Mapping[str, Any]] = field(
+    optical_system: collections.abc.Sequence[collections.abc.Mapping[str, Any]] = field(
         metadata=schema(
             title="optical_system",
             description=(
                 "List of optical elements before detector with their specific"
                 "arguments."
             ),
         )
@@ -1053,15 +1053,17 @@
                 "particles if no spectrum is provided energies are randomly drawn from"
                 "a normal distribution with mean and spread defined above note that the"
                 "energy spectrum is assumed to be a txt file with two columns [energy,"
                 "flux] with the energy in MeV"
             ),
         ),
     )
-    energy_spectrum_sampling: Optional[Literal["linear", "log", None]] = field(
+    energy_spectrum_sampling: Literal[
+        "linear", "log", None
+    ] = field(  # TODO: Check this
         default="log",
         metadata=schema(
             title="energy_spectrum_sampling",
             description=(
                 '"log" or None: the energy spectrum is sampled in log space "linear" :'
                 "the energy spectrum is sampled in linear space"
             ),
@@ -1300,15 +1302,15 @@
 #
 @schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationConversionWithQeMapArguments(Mapping[str, Any]):
     filename: Union[str, pathlib.Path] = field(
         metadata=schema(title="filename", description="File path.")
     )
-    position: Tuple[int, int] = field(
+    position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
             title="position",
             description=(
                 "Indices of starting row and column, used when fitting :term:`QE` map"
                 "to detector."
             ),
@@ -1404,21 +1406,21 @@
     )
     particles_per_second: Optional[float] = field(
         default=None,
         metadata=schema(
             title="particles_per_second", description="Number of particles per second."
         ),
     )
-    incident_angles: Optional[Tuple[str, str]] = field(
+    incident_angles: Optional[tuple[str, str]] = field(
         default=None,
         metadata=schema(
             title="incident_angles", description="Incident angles: ``(α, β)``."
         ),
     )
-    starting_position: Optional[Tuple[str, str, str]] = field(
+    starting_position: Optional[tuple[str, str, str]] = field(
         default=None,
         metadata=schema(
             title="starting_position", description="Starting position: ``(x, y, z)``."
         ),
     )
     spectrum_file: Optional[str] = field(
         default=None,
@@ -1653,15 +1655,15 @@
 #
 @schema(title="Parameters")
 @dataclass
 class ModelChargeGenerationLoadChargeArguments(Mapping[str, Any]):
     filename: Union[str, pathlib.Path] = field(
         metadata=schema(title="filename", description="File path.")
     )
-    position: Tuple[int, int] = field(
+    position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
             title="position",
             description=(
                 "Indices of starting row and column, used when fitting charge to"
                 "detector."
             ),
@@ -1821,15 +1823,15 @@
 class ModelChargeCollectionFixedPatternNoiseArguments(Mapping[str, Any]):
     filename: Union[pathlib.Path, str, None] = field(
         default=None,
         metadata=schema(
             title="filename", description="Path to a file with an array or an image."
         ),
     )
-    position: Tuple[int, int] = field(
+    position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
             title="position",
             description=(
                 "Indices of starting row and column, used when fitting noise to"
                 "detector."
             ),
@@ -1894,20 +1896,20 @@
 
 #
 # Model: Charge Collection / Persistence
 #
 @schema(title="Parameters")
 @dataclass
 class ModelChargeCollectionPersistenceArguments(Mapping[str, Any]):
-    trap_time_constants: Sequence[float] = field(
+    trap_time_constants: collections.abc.Sequence[float] = field(
         metadata=schema(
             title="trap_time_constants", description="A list of trap time constants."
         )
     )
-    trap_proportions: Sequence[float] = field(
+    trap_proportions: collections.abc.Sequence[float] = field(
         metadata=schema(
             title="trap_proportions", description="A list of trap proportions."
         )
     )
     trap_densities_filename: Union[pathlib.Path, str] = field(
         metadata=schema(
             title="trap_densities_filename", description="Path to densities file."
@@ -1915,15 +1917,15 @@
     )
     trap_capacities_filename: Union[pathlib.Path, str, None] = field(
         default=None,
         metadata=schema(
             title="trap_capacities_filename", description="Path to capacities file."
         ),
     )
-    trap_densities_position: Tuple[int, int] = field(
+    trap_densities_position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
             title="trap_densities_position",
             description=(
                 "Indices of starting row and column, used when fitting densities to"
                 "detector."
             ),
@@ -1937,15 +1939,15 @@
             title="trap_densities_align",
             description=(
                 "Keyword to align the densities to detector. Can be any from:"
                 '("center", "top_left", "top_right", "bottom_left", "bottom_right")'
             ),
         ),
     )
-    trap_capacities_position: Tuple[int, int] = field(
+    trap_capacities_position: tuple[int, int] = field(
         default=(0, 0),
         metadata=schema(
             title="trap_capacities_position",
             description=(
                 "Indices of starting row and column, used when fitting capacities to"
                 "detector."
             ),
@@ -2113,23 +2115,23 @@
 
 #
 # Model: Charge Collection / Simple Persistence
 #
 @schema(title="Parameters")
 @dataclass
 class ModelChargeCollectionSimplePersistenceArguments(Mapping[str, Any]):
-    trap_time_constants: Sequence[float] = field(
+    trap_time_constants: collections.abc.Sequence[float] = field(
         metadata=schema(
             title="trap_time_constants", description="List of trap time constants."
         )
     )
-    trap_densities: Sequence[float] = field(
+    trap_densities: collections.abc.Sequence[float] = field(
         metadata=schema(title="trap_densities", description="List of trap densities.")
     )
-    trap_capacities: Optional[Sequence[float]] = field(
+    trap_capacities: Optional[collections.abc.Sequence[float]] = field(
         default=None,
         metadata=schema(
             title="trap_capacities", description="List of trap capacities."
         ),
     )
 
     def __iter__(self) -> Iterator[str]:
@@ -2161,21 +2163,21 @@
 #
 # Model: Charge Transfer / Arctic Add
 #
 @schema(title="Parameters")
 @dataclass
 class ModelChargeTransferArcticAddArguments(Mapping[str, Any]):
     well_fill_power: float = field(metadata=schema(title="well_fill_power"))
-    trap_densities: Sequence[float] = field(
+    trap_densities: collections.abc.Sequence[float] = field(
         metadata=schema(
             title="trap_densities",
             description="A 1D arrays of all trap species densities for serial clocking.",
         )
     )
-    trap_release_timescales: Sequence[float] = field(
+    trap_release_timescales: collections.abc.Sequence[float] = field(
         metadata=schema(
             title="trap_release_timescales",
             description="A 1D arrays of all trap release timescales for serial clocking.",
         )
     )
     express: int = field(
         default=0,
@@ -2230,16 +2232,18 @@
 #
 # Model: Charge Transfer / Arctic Remove
 #
 @schema(title="Parameters")
 @dataclass
 class ModelChargeTransferArcticRemoveArguments(Mapping[str, Any]):
     well_fill_power: float = field(metadata=schema(title="well_fill_power"))
-    trap_densities: Sequence[float] = field(metadata=schema(title="trap_densities"))
-    trap_release_timescales: Sequence[float] = field(
+    trap_densities: collections.abc.Sequence[float] = field(
+        metadata=schema(title="trap_densities")
+    )
+    trap_release_timescales: collections.abc.Sequence[float] = field(
         metadata=schema(title="trap_release_timescales")
     )
     num_iterations: int = field(
         metadata=schema(
             title="num_iterations",
             description=(
                 "Number of iterations for the forward modelling. More iterations"
@@ -2321,27 +2325,27 @@
     )
     beta: float = field(
         metadata=schema(
             title="beta",
             description="Electron cloud expansion coefficient :math:`\\beta`.",
         )
     )
-    trap_release_times: Sequence[float] = field(
+    trap_release_times: collections.abc.Sequence[float] = field(
         metadata=schema(
             title="trap_release_times",
             description="Trap release time constants :math:`\\tau_r`. Unit: :math:`s`.",
         )
     )
-    trap_densities: Sequence[float] = field(
+    trap_densities: collections.abc.Sequence[float] = field(
         metadata=schema(
             title="trap_densities",
             description="Absolute trap densities :math:`n_t`. Unit: :math:`cm^{-3}`.",
         )
     )
-    sigma: Sequence[float] = field(
+    sigma: collections.abc.Sequence[float] = field(
         metadata=schema(
             title="sigma",
             description="Trap capture cross section :math:`\\sigma`. Unit: :math:`cm^2`.",
         )
     )
     full_well_capacity: Optional[float] = field(
         default=None,
@@ -2503,34 +2507,34 @@
 
 #
 # Model: Charge Measurement / Nghxrg
 #
 @schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementNghxrgArguments(Mapping[str, Any]):
-    noise: Sequence[
-        Mapping[
+    noise: collections.abc.Sequence[
+        collections.abc.Mapping[
             Literal[
                 "ktc_bias_noise",
                 "white_read_noise",
                 "corr_pink_noise",
                 "uncorr_pink_noise",
                 "acn_noise",
                 "pca_zero_noise",
             ],
-            Mapping[str, float],
+            collections.abc.Mapping[str, float],
         ]
     ] = field(metadata=schema(title="noise"))
-    window_position: Optional[Tuple[int, int]] = field(
+    window_position: Optional[tuple[int, int]] = field(
         default=None,
         metadata=schema(
             title="window_position", description="[x0 (columns), y0 (rows)]."
         ),
     )
-    window_size: Optional[Tuple[int, int]] = field(
+    window_size: Optional[tuple[int, int]] = field(
         default=None,
         metadata=schema(title="window_size", description="[x (columns), y (rows)]."),
     )
     seed: Optional[int] = field(default=None, metadata=schema(title="seed"))
     n_output: int = field(
         default=1,
         metadata=schema(title="n_output", description="Number of detector outputs."),
@@ -2616,15 +2620,15 @@
 
 #
 # Model: Charge Measurement / Output Node Linearity Poly
 #
 @schema(title="Parameters")
 @dataclass
 class ModelChargeMeasurementOutputNodeLinearityPolyArguments(Mapping[str, Any]):
-    coefficients: Sequence[float] = field(
+    coefficients: collections.abc.Sequence[float] = field(
         metadata=schema(
             title="coefficients", description="Coefficient of the polynomial function."
         )
     )
 
     def __iter__(self) -> Iterator[str]:
         return iter(("coefficients",))
@@ -3098,15 +3102,15 @@
 
 #
 # Model: Readout Electronics / Ac Crosstalk
 #
 @schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsAcCrosstalkArguments(Mapping[str, Any]):
-    coupling_matrix: Union[str, pathlib.Path, Sequence] = field(
+    coupling_matrix: Union[str, pathlib.Path, collections.abc.Sequence] = field(
         metadata=schema(title="coupling_matrix")
     )
     channel_matrix: Sequence = field(metadata=schema(title="channel_matrix"))
     readout_directions: Sequence = field(metadata=schema(title="readout_directions"))
 
     def __iter__(self) -> Iterator[str]:
         return iter(("coupling_matrix", "channel_matrix", "readout_directions"))
@@ -3137,15 +3141,15 @@
 
 #
 # Model: Readout Electronics / Dc Crosstalk
 #
 @schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsDcCrosstalkArguments(Mapping[str, Any]):
-    coupling_matrix: Union[str, pathlib.Path, Sequence] = field(
+    coupling_matrix: Union[str, pathlib.Path, collections.abc.Sequence] = field(
         metadata=schema(title="coupling_matrix")
     )
     channel_matrix: Sequence = field(metadata=schema(title="channel_matrix"))
     readout_directions: Sequence = field(metadata=schema(title="readout_directions"))
 
     def __iter__(self) -> Iterator[str]:
         return iter(("coupling_matrix", "channel_matrix", "readout_directions"))
@@ -3296,24 +3300,24 @@
 
 #
 # Model: Readout Electronics / Sar Adc With Noise
 #
 @schema(title="Parameters")
 @dataclass
 class ModelReadoutElectronicsSarAdcWithNoiseArguments(Mapping[str, Any]):
-    strengths: Tuple[float, ...] = field(
+    strengths: tuple[float, ...] = field(
         metadata=schema(
             title="strengths",
             description=(
                 "Sequence of ``detector.characteristics.adc_bit_resolution`` number(s)."
                 "Unit: V"
             ),
         )
     )
-    noises: Tuple[float, ...] = field(
+    noises: tuple[float, ...] = field(
         metadata=schema(
             title="noises",
             description=(
                 "Sequence of ``detector.characteristics.adc_bit_resolution`` number(s)."
                 "Unit: V"
             ),
         )
@@ -3472,65 +3476,161 @@
     func: Literal[
         "pyxel.models.readout_electronics.simple_phase_conversion"
     ] = "pyxel.models.readout_electronics.simple_phase_conversion"
     enabled: bool = True
 
 
 #
-# Model: Data Processing / Compute Statistics
+# Model: Data Processing / Extract Roi To Xarray
+#
+@schema(title="Parameters")
+@dataclass
+class ModelDataProcessingExtractRoiToXarrayArguments(Mapping[str, Any]):
+    thresh: int = field(
+        default=50,
+        metadata=schema(
+            title="thresh",
+            description="threshold above which information from the image array is extracted",
+        ),
+    )
+    minarea: int = field(
+        default=5,
+        metadata=schema(
+            title="minarea",
+            description=(
+                "minimum area of elements required that are above the threshold for the"
+                "extractor to extract information"
+            ),
+        ),
+    )
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(("thresh", "minarea"))
+
+    def __getitem__(self, item: Any) -> Any:
+        if item in tuple(self):
+            return getattr(self, item)
+        else:
+            raise KeyError
+
+    def __len__(self) -> int:
+        return 2
+
+
+@schema(
+    title="Model 'extract_roi_to_xarray'",
+    description=(
+        "Extract the roi data converts it to xarray dataset and saves the"
+        "information to the final result."
+    ),
+)
+@dataclass
+class ModelDataProcessingExtractRoiToXarray:
+    name: str
+    arguments: ModelDataProcessingExtractRoiToXarrayArguments = field(
+        default_factory=ModelDataProcessingExtractRoiToXarrayArguments
+    )
+    func: Literal[
+        "pyxel.models.data_processing.extract_roi_to_xarray"
+    ] = "pyxel.models.data_processing.extract_roi_to_xarray"
+    enabled: bool = True
+
+
+#
+# Model: Data Processing / Mean Variance
 #
 @schema(title="Parameters")
 @dataclass
-class ModelDataProcessingComputeStatisticsArguments(Mapping[str, Any]):
+class ModelDataProcessingMeanVarianceArguments(Mapping[str, Any]):
     data_structure: Literal["pixel", "photon", "image", "signal"] = field(
-        default="pixel",
+        default="image", metadata=schema(title="data_structure")
+    )
+    name: Optional[str] = field(default=None, metadata=schema(title="name"))
+
+    def __iter__(self) -> Iterator[str]:
+        return iter(("data_structure", "name"))
+
+    def __getitem__(self, item: Any) -> Any:
+        if item in tuple(self):
+            return getattr(self, item)
+        else:
+            raise KeyError
+
+    def __len__(self) -> int:
+        return 2
+
+
+@schema(
+    title="Model 'mean_variance'",
+    description="Compute mean-variance and store it in '.data' bucket.",
+)
+@dataclass
+class ModelDataProcessingMeanVariance:
+    name: str
+    arguments: ModelDataProcessingMeanVarianceArguments = field(
+        default_factory=ModelDataProcessingMeanVarianceArguments
+    )
+    func: Literal[
+        "pyxel.models.data_processing.mean_variance"
+    ] = "pyxel.models.data_processing.mean_variance"
+    enabled: bool = True
+
+
+#
+# Model: Data Processing / Statistics
+#
+@schema(title="Parameters")
+@dataclass
+class ModelDataProcessingStatisticsArguments(Mapping[str, Any]):
+    data_structure: Literal["pixel", "photon", "signal", "image", "all"] = field(
+        default="all",
         metadata=schema(
             title="data_structure",
             description=(
                 'Keyword to choose data structure. Can be any from: ("pixel", "photon",'
-                '"image", "signal")'
+                '"signal", "image", "all"). Default is "all" and computes the'
+                'statistics on "pixel", "photon", "signal" and "image".'
             ),
         ),
     )
-    dimensions: Union[str, Sequence[str]] = field(
-        default=("x", "y"),
-        metadata=schema(title="dimensions", description="Dimensions."),
-    )
 
     def __iter__(self) -> Iterator[str]:
-        return iter(("data_structure", "dimensions"))
+        return iter(("data_structure",))
 
     def __getitem__(self, item: Any) -> Any:
         if item in tuple(self):
             return getattr(self, item)
         else:
             raise KeyError
 
     def __len__(self) -> int:
-        return 2
+        return 1
 
 
-@schema(title="Model 'compute_statistics'", description="Compute basic statistics.")
+@schema(title="Model 'statistics'", description="Compute basic statistics.")
 @dataclass
-class ModelDataProcessingComputeStatistics:
+class ModelDataProcessingStatistics:
     name: str
-    arguments: ModelDataProcessingComputeStatisticsArguments = field(
-        default_factory=ModelDataProcessingComputeStatisticsArguments
+    arguments: ModelDataProcessingStatisticsArguments = field(
+        default_factory=ModelDataProcessingStatisticsArguments
     )
     func: Literal[
-        "pyxel.models.data_processing.compute_statistics"
-    ] = "pyxel.models.data_processing.compute_statistics"
+        "pyxel.models.data_processing.statistics"
+    ] = "pyxel.models.data_processing.statistics"
     enabled: bool = True
 
 
 #
 # Detection pipeline
 #
 @dataclass
 class DetailedDetectionPipeline(DetectionPipeline):
+    scene_generation: Optional[
+        Sequence[Union[ModelLoadDetector, ModelSaveDetector, ModelFunction]]
+    ] = field(default=None, metadata=schema(title="Scene Generation"))
     photon_collection: Optional[
         Sequence[
             Union[
                 ModelPhotonCollectionIllumination,
                 ModelPhotonCollectionLoadImage,
                 ModelPhotonCollectionLoadPsf,
                 ModelPhotonCollectionOpticalPsf,
@@ -3664,15 +3764,17 @@
                 ModelFunction,
             ]
         ]
     ] = field(default=None, metadata=schema(title="Readout Electronics"))
     data_processing: Optional[
         Sequence[
             Union[
-                ModelDataProcessingComputeStatistics,
+                ModelDataProcessingExtractRoiToXarray,
+                ModelDataProcessingMeanVariance,
+                ModelDataProcessingStatistics,
                 ModelLoadDetector,
                 ModelSaveDetector,
                 ModelFunction,
             ]
         ]
     ] = field(default=None, metadata=schema(title="Data Processing"))
 
@@ -3712,15 +3814,15 @@
     )
     full_well_capacity: Optional[float] = field(
         default=None,
         metadata=schema(
             title="full_well_capacity", description="Full well capacity. Unit: e-"
         ),
     )
-    adc_voltage_range: Optional[Tuple[float, float]] = field(
+    adc_voltage_range: Optional[tuple[float, float]] = field(
         default=None,
         metadata=schema(
             title="adc_voltage_range", description="ADC voltage range. Unit: V"
         ),
     )
     adc_bit_resolution: Optional[int] = field(
         default=None,
@@ -3778,15 +3880,15 @@
             title="full_well_capacity", description="Full well capacity. Unit: e-"
         ),
     )
     adc_bit_resolution: Optional[int] = field(
         default=None,
         metadata=schema(title="adc_bit_resolution", description="ADC bit resolution."),
     )
-    adc_voltage_range: Optional[Tuple[float, float]] = field(
+    adc_voltage_range: Optional[tuple[float, float]] = field(
         default=None,
         metadata=schema(
             title="adc_voltage_range", description="ADC voltage range. Unit: V"
         ),
     )
     avalanche_gain: Optional[float] = field(
         default=None,
@@ -3929,15 +4031,15 @@
 @dataclass
 class ExposureOutputs(Outputs):
     save_exposure_data: Optional[Sequence[Mapping[str, Sequence[str]]]] = None
 
 
 @dataclass
 class Readout:
-    times: Optional[Union[Sequence, str]] = None
+    times: Union[Sequence, str, None] = None
     times_from_file: Optional[str] = None
     start_time: float = 0.0
     non_destructive: bool = False
 
 
 @schema(title="Exposure")
 @dataclass
@@ -3966,26 +4068,26 @@
         Sequence[Literal["_"]],
         Sequence[Union[int, float]],
         Sequence[Sequence[Union[int, float]]],
         Sequence[Sequence[Sequence[Union[int, float]]]],
         Sequence[str],
         str,  # e.g. 'numpy.unique(...)'
     ]
-    boundaries: Optional[Tuple[float, float]] = None
+    boundaries: Union[Tuple[float, float], Sequence[Tuple[float, float]], None] = None
     enabled: bool = True
     logarithmic: bool = False
 
 
 @schema(title="Observation")
 @dataclass
 class Observation:
     outputs: ObservationOutputs
     parameters: Sequence[ParameterValues]
     readout: Optional[Readout] = None
-    mode: str = "product"
+    mode: Literal["product", "sequential", "custom"] = "product"
     from_file: Optional[str] = None
     column_range: Optional[Tuple[int, int]] = None
     with_dask: bool = False
     result_type: Literal["image", "signal", "pixel", "all"] = "all"
     pipeline_seed: Optional[int] = None
 
 
@@ -4106,38 +4208,35 @@
     apd_detector: Optional[APD] = field(default=None, metadata=schema(title="APD"))
 
 
 class NotEqualError(Exception):
     ...
 
 
-def comparison(first, second) -> bool:
+def compare(first, second) -> None:
     if type(first) != type(second):
         raise NotEqualError
 
     if isinstance(first, dict) and isinstance(second, dict):
         if set(first) != set(second):
             raise NotEqualError
 
         for key in first:
-            comparison(first[key], second[key])
+            compare(first[key], second[key])
 
     elif isinstance(first, list) and isinstance(second, list):
         if len(first) != len(second):
             raise NotEqualError
 
         if first != second:
             sorted_first = sorted(first)
             sorted_second = sorted(second)
 
             if sorted_first != sorted_second:
                 raise NotEqualError
-
-        # for key1, key2 in zip(sorted(first), sorted(second)):
-        #     comparison(key1, key2)
     else:
         if first != second:
             raise NotEqualError
 
 
 @click.command()
 @click.option(
@@ -4170,27 +4269,25 @@
 
     if check:
         with full_filename.open() as fh:
             dct_reference = json.load(fh)
 
         new_dct_schema: Mapping[str, Any] = json.loads(json.dumps(dct_schema))
 
-        result = comparison(dct_reference, new_dct_schema)
-
-        if dct_reference == new_dct_schema:
-            sys.exit(0)
-        else:
-            result = DeepDiff(dct_reference, new_dct_schema)
-
+        try:
+            compare(dct_reference, new_dct_schema)
+        except NotEqualError:
             print(
                 f"Error, JSON Schema file: {full_filename} is not the newest version. "
                 f"Please run 'tox -e json_schema'"
             )
             pprint(result)
             sys.exit(1)
+        else:
+            sys.exit(0)
     else:
         print(json.dumps(dct_schema))
         with full_filename.open("w") as fh:
             json.dump(obj=dct_schema, fp=fh, indent=2, sort_keys=True)
 
 
 if __name__ == "__main__":
```

### Comparing `pyxel_sim-1.8/continuous_integration/scripts/create_json_schema.py` & `pyxel_sim-1.9/continuous_integration/scripts/create_json_schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -665,15 +665,15 @@
     yield "    weights: Optional[Sequence[float]] = None"
 
     yield ""
     yield ""
     yield ""
 
     # Create wrappers for the detectors
-    detector_classes: Sequence[str] = ("CCD", "CMOS", "MKID", "APD")
+    # detector_classes: Sequence[str] = ("CCD", "CMOS", "MKID", "APD")
     # for klass_name in detector_classes:
     #     yield f"#@schema(title='{klass_name}')"
     #     yield "#@dataclass"
     #     yield f"#class Wrapper{klass_name}:"
     #     yield f"#    {klass_name.lower()}: {klass_name}"
     #     yield ""
     #     yield ""
@@ -700,15 +700,16 @@
     yield ""
     yield "    # Running modes"
     for klass_name in mode_classes:
         yield f"    {klass_name.lower()}: Optional[{klass_name}] = field(default=None, metadata=schema(title={klass_name!r}))"
 
     yield ""
     yield "    # Detectors"
-    for klass_name in detector_classes:
+    for detector_klass in registered_detectors:
+        klass_name: str = detector_klass.__name__
         yield f"    {klass_name.lower()}_detector: Optional[{klass_name}] = field(default=None, metadata=schema(title={klass_name!r}))"
 
 
 def generate_all_models() -> Iterator[str]:
     lst = get_model_group_info()
     yield "#  Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022."
     yield "#"
@@ -719,14 +720,15 @@
     yield ""
     yield "######################################"
     yield "# Note: This code is auto-generated. #"
     yield "#       Don't modify it !            #"
     yield "######################################"
     yield ""
 
+    yield "import collections"
     yield "import json"
     yield "import pathlib"
     yield "import sys"
     yield "from dataclasses import dataclass, field"
     yield "from pathlib import Path"
     yield "from pprint import pprint"
     yield "from typing import Any, Iterator, Literal, Mapping, Optional, Sequence, Tuple, Union"
```

### Comparing `pyxel_sim-1.8/continuous_integration/scripts/download_last_environment_artifact.py` & `pyxel_sim-1.9/continuous_integration/scripts/download_last_environment_artifact.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/docs/source/conf.py` & `pyxel_sim-1.9/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,14 @@
 # of the sidebar.
 html_logo = "_static/pyxel-logo.png"
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
-html_css_files = ["style.css"]
 
 # configuration for sphinxext.opengraph
 ogp_site_url = "https://esa.gitlab.io/pyxel/doc/"
 ogp_image = "https://esa.gitlab.io/pyxel/doc/_static/esa-logo.png"
 ogp_custom_meta_tags = [
     # '<meta name="twitter:card" content="summary_large_image" />',
     '<meta name="image" property="og:image" content="https://esa.gitlab.io/pyxel/doc/_static/esa-logo.png">',
```

### Comparing `pyxel_sim-1.8/pyproject.toml` & `pyxel_sim-1.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -3,46 +3,46 @@
 # Build project       : python -m build . --wheel --sdist
 [build-system]
 requires = ["setuptools>=63", "versioneer[toml]==0.28", "wheel"]
 build-backend = "setuptools.build_meta"
 
 # https://peps.python.org/pep-0621
 [project]
-requires-python = ">= 3.8"
+requires-python = ">= 3.9"
 name = "pyxel_sim"
 description = "Pyxel detector simulation framework."
 readme = "README.md"
 authors = [{"name" = "The Pyxel development team", "email" = "pyxel@esa.int" }]
 license = { text = "MIT" }
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-#    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Astronomy",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Scientific/Engineering :: Physics",
     "Typing :: Typed",
 ]
 keywords = ["ESA", "data modeling", "sensors", "calibration", "CCD",
     "CMOS", "active sensors", "electronics"]
 dependencies = [
     # Scientific computing
     "numba",
     "numpy>=1.21",
     "pandas",
     "scipy",
     "xarray>=2022.06",
+    "xarray-datatree>=0.0.12",
     "sep",
 
     # Plotting
     "matplotlib>=3.1",
     "seaborn",
     "holoviews>=1.15.0",
     "bokeh",
@@ -54,14 +54,15 @@
     # Jupyter notebook
     "ipywidgets>=7.5",
 
     # Input/Output
     "astropy>=4.3",
     "fsspec[http]>=2021",
     "h5py",
+    "h5netcdf",
     "pyyaml",
     "xlrd",
     "openpyxl",
     "netcdf4",
 
     # Others
     "attrs>=21.3.0",
@@ -79,15 +80,15 @@
 documentation = "https://esa.gitlab.io/pyxel/doc/"
 repository = "https://gitlab.com/esa/pyxel"
 changelog = "https://gitlab.com/esa/pyxel/-/releases"
 tracker = "https://gitlab.com/esa/pyxel/issues"
 
 [project.optional-dependencies]
 calibration = [ "pygmo>=2.16.1" ]
-model = [ "poppy>=1.0.2" ]
+model = [ "poppy>=1.1.0" ]
 io = [ "asdf" ]
 all = [
     "pyxel-sim[calibration]",
     "pyxel-sim[model]",
     "pyxel-sim[io]",
 ]
 
@@ -195,15 +196,15 @@
 ignore = ["D001", "D002", "D004", "D005"]
 
 [tool.bandit]
 exclude_dirs = ["pyxel/_version.py"]
 
 [tool.codespell]
 ignore-words-list = "acn,sade,te"
-skip = "pyxel/_version.py"
+skip = "pyxel/_version.py,*.fits"
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "debug",
     "raise NotImplementedError",
 ]
@@ -212,11 +213,36 @@
 omit = [
     "pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py",
     "pyxel/models/charge_generation/tars/plotting.py",
 ]
 
 [tool.ruff]
 ignore = [
-    "E501", # Omit 'Line too long'
+    "E501",     # Omit 'Line too long'
+    "D102",     # Missing docstring in public method
+    "D103",     # Missing docstring in public function
+    "D105",     # Missing docstring in magic method
+    "D202",     # No blank lines
+    "RUF002",   # Docstring contains ambiguous unicode character
+    "RUF003",   # ambiguous unicode character
+    "TRY003",   # Avoid specifying long messages outside the exception class
+    "TRY301",   # Abstract `raise` to an inner function
+]
+
+select = [
+    "A",        # flake8-builtins
+    "B",        # flake8-bugbear
+    "E",        # pycodestyle
+    "F",        # pyflakes
+    "D",        # pydocstyle
+    # "SIM",      # flake8-simplify
+    "W",        # pycodestyle
+    # "PD",       # pandas-vet
+    # "S",        # bandit
+    "RUF",      # Ruff-specific rules
+    "TRY",      # Tryceratops
 ]
 
-exclude = ["_TEMPLATE.py"]
+exclude = ["_TEMPLATE.py", "_version.py"]
+
+[tool.ruff.pydocstyle]
+convention = "numpy"
```

### Comparing `pyxel_sim-1.8/pyxel/__init__.py` & `pyxel_sim-1.9/pyxel/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/__main__.py` & `pyxel_sim-1.9/pyxel/__main__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/backends/asdf.py` & `pyxel_sim-1.9/pyxel/backends/asdf.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Module to read/write ASDF files."""
 
+from collections.abc import Iterator, Mapping, Sequence
 from contextlib import contextmanager
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, Iterator, Mapping, Sequence, Union
+from typing import TYPE_CHECKING, Any, Union
 
 if TYPE_CHECKING:
     import pandas as pd
+    import xarray as xr
 
 
 def to_asdf(filename: Union[str, Path], dct: Mapping[str, Any]) -> None:
     """Write data to a ASDF file."""
     try:
         import asdf
     except ImportError as exc:
@@ -31,14 +33,22 @@
 
     # Convert a 'DataFrame' into a `dict`
     df: pd.DataFrame = dct["data"]["charge"]["frame"]
     frame_dct: Mapping[str, Sequence[float]] = df.to_dict(orient="list")
 
     dct["data"]["charge"]["frame"] = frame_dct
 
+    # Convert 'Dataset(s)' into a 'dict(s)'
+    data: Mapping[str, xr.Dataset] = dct["data"]["data"]
+    dct_data: Mapping[str, Mapping] = {
+        key: value.to_dict() for key, value in data.items()
+    }
+
+    dct["data"]["data"] = dct_data
+
     with asdf.AsdfFile(dct) as af:
         af.write_to(filename)
 
 
 @contextmanager
 def from_asdf(filename: Union[str, Path]) -> Iterator[Mapping[str, Any]]:
     """Read data from a HDF5 file."""
@@ -49,15 +59,15 @@
     except ImportError as exc:
         raise ImportError(
             "Missing optional package 'asdf'.\n"
             "Please install it with 'pip install pyxel-sim[io]' "
             "or 'pip install pyxel-sim[all]'"
         ) from exc
 
-    dct: Dict[str, Any] = {}
+    dct: dict[str, Any] = {}
 
     with asdf.open(filename, copy_arrays=True) as af:
         # TODO: Use a JSON schema to validate 'dct'
         if "version" not in af:
             raise ValueError("Missing 'version' !")
 
         version: int = af["version"]
```

### Comparing `pyxel_sim-1.8/pyxel/backends/hdf5.py` & `pyxel_sim-1.9/pyxel/backends/hdf5.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 
 from collections import abc
+from collections.abc import Iterator, Mapping
 from contextlib import contextmanager
 from pathlib import Path
-from typing import Any, Iterator, Mapping, Optional, Union
+from typing import Any, Optional, Union
 
 import h5py as h5
 import numpy as np
 import pandas as pd
+import xarray as xr
 
 from pyxel import __version__
 
 ATTRIBUTES: Mapping[str, Mapping[str, str]] = {
     "photon": {"name": "Photon", "unit": "photon/s"},
     "charge": {"name": "Charge", "unit": "electron"},
     "pixel": {"name": "Pixel", "unit": "electron"},
@@ -26,15 +28,17 @@
     "image": {"name": "Image", "unit": "adu"},
 }
 
 
 def _store(
     h5file: h5.File,
     name: str,
-    dct: Mapping[str, Union[int, float, pd.DataFrame, pd.Series, np.ndarray, dict]],
+    dct: Mapping[
+        str, Union[int, float, pd.DataFrame, pd.Series, xr.Dataset, np.ndarray, dict]
+    ],
     attributes: Optional[Mapping[str, Mapping[str, str]]] = None,
 ) -> None:
     """Write data into a new HDF5 group.
 
     Parameters
     ----------
     h5file : h5.File
@@ -43,14 +47,16 @@
         Name of the HDF5 group to create. (e.g. '/' or '/geometry')
     dct : dict
         Data to write into a HDF5 dataset.
     attributes : dict
         Attributes to store.
     """
     for key, value in dct.items():
+        key = key.removeprefix("/")
+
         new_name = f"{name}/{key}"
 
         if isinstance(value, (int, float)) or value is None:
             if value is None:
                 value = np.nan
 
             dataset: h5.Dataset = h5file.create_dataset(
@@ -63,19 +69,26 @@
         elif isinstance(value, pd.DataFrame):
             new_group: h5.Group = h5file.create_group(name=new_name)
             new_group.attrs["type"] = "DataFrame"
 
             _store(h5file, name=new_name, dct=value.to_dict(orient="series"))
 
         elif isinstance(value, (pd.Series, np.ndarray, abc.Sequence)):
-            dataset = h5file.create_dataset(name=new_name, data=np.asarray(value))
+            dataset = h5file.create_dataset(name=new_name, data=value)
 
             if attributes is not None and key in attributes:
                 dataset.attrs.update(attributes[key])
 
+        elif isinstance(value, xr.Dataset):
+            if value:
+                _store(h5file, name=new_name, dct=value.to_dict())
+            else:
+                # Do nothing
+                pass
+
         elif isinstance(value, dict):
             new_group = h5file.create_group(name=new_name)
 
             if attributes is not None and key in attributes:
                 new_group.attrs.update(attributes[key])
 
             _store(h5file, name=new_name, dct=value)
@@ -102,15 +115,15 @@
         )
 
         _store(h5file, name="/data", dct=dct["data"], attributes=ATTRIBUTES)
 
 
 def _load(
     h5file: h5.File, name: str
-) -> Union[None, int, float, Mapping[str, Any], np.ndarray, pd.DataFrame]:
+) -> Union[None, int, float, str, Mapping[str, Any], np.ndarray, pd.DataFrame]:
     """Write data from a HDF5 group.
 
     Parameters
     ----------
     h5file : h5.File
         Readable HDF5 file object.
     name : str
@@ -133,26 +146,32 @@
         if name.endswith("frame"):
             return pd.DataFrame.from_dict(dct)
         else:
             return dct
 
     elif isinstance(dataset, h5.Dataset):
         if dataset.ndim == 0:
-            value = np.array(dataset)
+            value = np.array(dataset, dtype=dataset.dtype)
 
-            if np.isnan(value):
+            if dataset.dtype == np.dtype(object):
+                value_converted = value.astype(str)
+                return str(value_converted)
+            elif np.isnan(value):
                 return None
             elif np.issubdtype(dataset.dtype, np.integer):
                 return int(value)
             elif np.issubdtype(dataset.dtype, np.floating):
                 return float(value)
             else:
                 raise TypeError
         else:
-            return np.array(dataset)
+            if dataset.dtype == np.dtype(object):
+                return np.array(dataset, dtype=str)
+            else:
+                return np.array(dataset)
     else:
         raise NotImplementedError
 
 
 @contextmanager
 def from_hdf5(filename: Union[str, Path]) -> Iterator[Mapping[str, Any]]:
     """Read data from a HDF5 file."""
```

### Comparing `pyxel_sim-1.8/pyxel/calibration/__init__.py` & `pyxel_sim-1.9/pyxel/calibration/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,12 +16,16 @@
     CalibrationMode,
     Island,
     check_ranges,
     list_to_slice,
     read_data,
     read_datacubes,
     list_to_3d_slice,
+    FitRange2D,
+    FitRange3D,
+    to_fit_range,
+    check_fit_ranges,
 )
-from ..pipelines.processor import ResultType
 from .archipelago import MyArchipelago
+from .archipelago_datatree import ArchipelagoDataTree
 from .calibration import Calibration, CalibrationMode
 from .fitness import sum_of_abs_residuals, sum_of_squared_residuals, reduced_chi_squared
```

### Comparing `pyxel_sim-1.8/pyxel/calibration/algorithm.py` & `pyxel_sim-1.9/pyxel/calibration/algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # TODO: Use a class `Sade`, `SGA` and `NLOPT`. See #334
 class Algorithm:
     """TBW."""
 
     def __init__(
         self,
         # TODO: Rename 'type' into 'algorithm_type'. See #334
-        type: Literal["sade", "sga", "nlopt"] = "sade",
+        type: Literal["sade", "sga", "nlopt"] = "sade",  # noqa: A002
         generations: int = 1,
         population_size: int = 1,
         # SADE #####
         variant: int = 2,
         variant_adptv: int = 1,
         ftol: float = 1e-6,
         xtol: float = 1e-6,
@@ -131,20 +131,20 @@
         self._ftol_abs = ftol_abs
         self._stopval: float = -math.inf if stopval is None else stopval
         self._local_optimizer: Optional[pg.nlopt] = local_optimizer
         self._replacement = replacement
         self._nlopt_selection = nlopt_selection
 
     @property
-    def type(self) -> AlgorithmType:
+    def type(self) -> AlgorithmType:  # noqa: A003
         """TBW."""
         return self._type
 
     @type.setter
-    def type(self, value: AlgorithmType) -> None:
+    def type(self, value: AlgorithmType) -> None:  # noqa: A003
         """TBW."""
         self._type = AlgorithmType(value)
 
     @property
     def generations(self) -> int:
         """TBW."""
         return self._generations
```

### Comparing `pyxel_sim-1.8/pyxel/calibration/archipelago.py` & `pyxel_sim-1.9/pyxel/calibration/archipelago.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,18 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Sub-package to create 'archipelagos'."""
 import logging
+from collections.abc import Mapping, Sequence
 from concurrent.futures.thread import ThreadPoolExecutor
 from timeit import default_timer as timer
-from typing import (
-    TYPE_CHECKING,
-    Callable,
-    List,
-    Mapping,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-)
+from typing import TYPE_CHECKING, Callable, Optional, Union
 
 import dask.array as da
 import numpy as np
 import pandas as pd
 import xarray as xr
 from dask.delayed import Delayed
 from tqdm.auto import tqdm
@@ -34,14 +26,15 @@
 if TYPE_CHECKING:
     import pygmo as pg
     from numpy.typing import ArrayLike
 
     from pyxel.exposure import Readout
 
 
+# TODO: Deprecate this class ?
 class ArchipelagoLogs:
     """Keep log information from all algorithms in an archipelago."""
 
     def __init__(self, algo_type: AlgorithmType, num_generations: int):
         try:
             import pygmo as pg
         except ImportError as exc:
@@ -78,15 +71,15 @@
         # Put the logging information from pygmo into a `DataFrame`
         df = pd.DataFrame(logs, columns=self._columns)
 
         return df
 
     def _from_archi(self, archi: "pg.archipelago") -> pd.DataFrame:
         """Get logging information from an archipelago."""
-        lst: List[pd.DataFrame] = []
+        lst: list[pd.DataFrame] = []
 
         for id_island, island in enumerate(archi):
             # Extract the Pygmo algorithm from an island
             df_island = self._from_algo(algo=island.get_algorithm())
             df_island["id_island"] = id_island + 1
 
             lst.append(df_island)
@@ -123,15 +116,15 @@
     df_results: pd.DataFrame,
     rows: int,
     cols: int,
     times: int,
     readout_times: np.ndarray,
 ) -> xr.Dataset:
     """Extract 'photon', 'charge', 'pixel', 'signal' and 'image' arrays from several delayed dynamic results."""
-    lst: List[xr.Dataset] = []
+    lst: list[xr.Dataset] = []
     for _, row in df_results.iterrows():
         island: int = row["island"]
         id_processor: int = row["id_processor"]
         result: Mapping[str, Delayed] = row["processor"].result
 
         photon_delayed: Delayed = result["photon"]
         charge_delayed: Delayed = result["charge"]
@@ -298,15 +291,15 @@
         logging.info("Create a new archipelago in %.2f s", stop_time - start_time)
 
     def run_evolve(
         self,
         readout: "Readout",
         num_evolutions: int = 1,
         num_best_decisions: Optional[int] = None,
-    ) -> Tuple[xr.Dataset, pd.DataFrame, pd.DataFrame]:
+    ) -> tuple[xr.Dataset, pd.DataFrame, pd.DataFrame]:
         """Run evolution(s) several time.
 
         Parameters
         ----------
         readout
         num_evolutions : int
             Number of time to run the evolutions.
@@ -328,15 +321,15 @@
 
         with tqdm(
             total=total_num_generations,
             desc=f"Evolve with {self.num_islands} islands",
             unit=" generations",
             disable=not self.with_bar,
         ) as progress:
-            champions_lst: List[xr.Dataset] = []
+            champions_lst: list[xr.Dataset] = []
             # Run an evolution im the archipelago several times
             for id_evolution in range(num_evolutions):
                 # If the evolution on this archipelago was already run before, then
                 # the migration process between the islands is automatically executed
                 # Call all 'evolve()' methods on all islands
                 self._pygmo_archi.evolve()
                 # self._log.info(self._pygmo_archi)  # TODO: Remove this
```

### Comparing `pyxel_sim-1.8/pyxel/calibration/calibration.py` & `pyxel_sim-1.9/pyxel/calibration/calibration.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,51 +3,48 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 import logging
+from collections.abc import Mapping, Sequence
 from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Literal,
-    Mapping,
-    Optional,
-    Sequence,
-    Tuple,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Literal, Optional, Union
 
 import numpy as np
 from dask.delayed import Delayed
 
 from pyxel.calibration import (
     Algorithm,
+    ArchipelagoDataTree,
     CalibrationMode,
     DaskBFE,
     DaskIsland,
+    FitRange3D,
     Island,
     MyArchipelago,
+    to_fit_range,
 )
 from pyxel.calibration.fitting import ModelFitting
+from pyxel.calibration.fitting_datatree import ModelFittingDataTree
 from pyxel.exposure import Readout
 from pyxel.observation import ParameterValues
-from pyxel.pipelines import FitnessFunction, Processor, ResultType
+from pyxel.pipelines import FitnessFunction, Processor, ResultId, get_result_id
 
 if TYPE_CHECKING:
     import pandas as pd
     import xarray as xr
+    from datatree import DataTree
 
     from pyxel.outputs import CalibrationOutputs
 
 
 def to_path_list(values: Sequence[Union[str, Path]]) -> Sequence[Path]:
-    """TBW."""
+    """Convert a sequence of ``Path``-like into a sequence of ``Path``."""
     return [Path(obj).resolve() for obj in values]
 
 
 class Calibration:
     """TBW."""
 
     def __init__(
@@ -56,17 +53,25 @@
         target_data_path: Sequence[Union[str, Path]],
         fitness_function: FitnessFunction,
         algorithm: Algorithm,
         parameters: Sequence[ParameterValues],
         readout: Optional["Readout"] = None,
         mode: Literal["pipeline", "single_model"] = "pipeline",
         result_type: Literal["image", "signal", "pixel"] = "image",
-        result_fit_range: Optional[Sequence[int]] = None,
+        result_fit_range: Union[
+            tuple[int, int, int, int],
+            tuple[int, int, int, int, int, int],
+            None,
+        ] = None,
         result_input_arguments: Optional[Sequence[ParameterValues]] = None,
-        target_fit_range: Optional[Sequence[int]] = None,
+        target_fit_range: Union[
+            tuple[int, int, int, int],
+            tuple[int, int, int, int, int, int],
+            None,
+        ] = None,
         pygmo_seed: Optional[int] = None,
         pipeline_seed: Optional[int] = None,
         num_islands: int = 1,
         num_evolutions: int = 1,
         num_best_decisions: Optional[int] = None,
         topology: Literal["unconnected", "ring", "fully_connected"] = "unconnected",
         type_islands: Literal[
@@ -84,15 +89,15 @@
         self._log = logging.getLogger(__name__)
 
         self.outputs = outputs
         self.readout: Readout = readout or Readout()
 
         self._calibration_mode = CalibrationMode(mode)
 
-        self._result_type: ResultType = ResultType(result_type)
+        self._result_type: ResultId = get_result_id(result_type)
 
         self._result_fit_range: Sequence[int] = result_fit_range or []
 
         self._result_input_arguments: Sequence[ParameterValues] = (
             result_input_arguments or []
         )
 
@@ -134,20 +139,20 @@
 
     @calibration_mode.setter
     def calibration_mode(self, value: CalibrationMode) -> None:
         """TBW."""
         self._calibration_mode = value
 
     @property
-    def result_type(self) -> ResultType:
+    def result_type(self) -> ResultId:
         """TBW."""
         return self._result_type
 
     @result_type.setter
-    def result_type(self, value: ResultType) -> None:
+    def result_type(self, value: ResultId) -> None:
         """TBW."""
         self._result_type = value
 
     @property
     def result_fit_range(self) -> Sequence[int]:
         """TBW."""
         return self._result_fit_range
@@ -308,142 +313,157 @@
         return self._weights
 
     @weights.setter
     def weights(self, value: Sequence[float]) -> None:
         """TBW."""
         self._weights = value
 
+    def get_problem(self, processor: Processor, output_dir: Path) -> ModelFitting:
+        """Convert a 'processor' object into a Pygmo Problem.
+
+        Examples
+        --------
+        Create a 'Pygmo Problem'
+        >>> calibration = Calibration(...)
+        >>> problem = calibration.get_problem(processor=..., output_dir=...)
+
+        Create a decision vector
+        >>> problem.get_bounds()
+        >>> decision_vector = [...]
+
+        Compute fitness
+        >>> problem.fitness(decision_vector)
+        """
+        problem = ModelFitting(
+            processor=processor,
+            variables=self.parameters,
+            readout=self.readout,
+            calibration_mode=CalibrationMode(self.calibration_mode),
+            simulation_output=self.result_type,
+            generations=self.algorithm.generations,
+            population_size=self.algorithm.population_size,
+            fitness_func=self.fitness_function,
+            file_path=output_dir,
+        )
+
+        problem.configure(
+            target_output=self.target_data_path,
+            target_fit_range=self.target_fit_range,
+            out_fit_range=self.result_fit_range,
+            input_arguments=self.result_input_arguments,
+            weights=self.weights,
+            weights_from_file=self.weights_from_file,
+        )
+
+        return problem
+
     # TODO: This function will be deprecated (see #563)
     def run_calibration(
         self,
         processor: Processor,
         output_dir: Path,
         with_progress_bar: bool = True,
-    ) -> Tuple["xr.Dataset", "pd.DataFrame", "pd.DataFrame"]:
+    ) -> tuple["xr.Dataset", "pd.DataFrame", "pd.DataFrame"]:
         """Run calibration pipeline."""
         try:
             import pygmo as pg
         except ImportError as exc:
             raise ImportError(
                 "Missing optional package 'pygmo'.\n"
                 "Please install it with 'pip install pyxel-sim[calibration]' "
                 "or 'pip install pyxel-sim[all]'"
             ) from exc
 
         pg.set_global_rng_seed(seed=self.pygmo_seed)
         self._log.info("Pygmo seed: %d", self.pygmo_seed)
 
-        fitting = ModelFitting(
-            processor=processor,
-            variables=self.parameters,
-            readout=self.readout,
-            calibration_mode=CalibrationMode(self.calibration_mode),
-            simulation_output=ResultType(self.result_type),
-            generations=self.algorithm.generations,
-            population_size=self.algorithm.population_size,
-            fitness_func=self.fitness_function,
-            file_path=output_dir,
+        # Create a Pygmo problem
+        fitting: ModelFitting = self.get_problem(
+            processor=processor, output_dir=output_dir
         )
 
-        fitting.configure(
-            target_output=self.target_data_path,
-            target_fit_range=self.target_fit_range,
-            out_fit_range=self.result_fit_range,
-            input_arguments=self.result_input_arguments,
-            weights=self.weights,
-            weights_from_file=self.weights_from_file,
-        )
+        # Create an archipelago
+        user_defined_island = DaskIsland()
+        user_defined_bfe = DaskBFE()
 
-        if self.num_islands > 1:  # default
-            # Create an archipelago
-            user_defined_island = DaskIsland()
-            user_defined_bfe = DaskBFE()
-
-            if self.topology == "unconnected":
-                topo = pg.unconnected()
-            elif self.topology == "ring":
-                topo = pg.ring()
-            elif self.topology == "fully_connected":
-                topo = pg.fully_connected()
-            else:
-                raise NotImplementedError(f"topology {self.topology!r}")
-
-            # Create a new archipelago
-            # This operation takes some time ...
-            my_archipelago = MyArchipelago(
-                num_islands=self.num_islands,
-                udi=user_defined_island,
-                algorithm=self.algorithm,
-                problem=fitting,
-                pop_size=self.algorithm.population_size,
-                bfe=user_defined_bfe,
-                topology=topo,
-                pygmo_seed=self.pygmo_seed,
-                with_bar=with_progress_bar,
-            )
+        if self.topology == "unconnected":
+            topo = pg.unconnected()
+        elif self.topology == "ring":
+            topo = pg.ring()
+        elif self.topology == "fully_connected":
+            topo = pg.fully_connected()
+        else:
+            raise NotImplementedError(f"topology {self.topology!r}")
 
-            # Run several evolutions in the archipelago
-            ds, df_processors, df_all_logs = my_archipelago.run_evolve(
-                readout=self.readout,
-                num_evolutions=self._num_evolutions,
-                num_best_decisions=self._num_best_decisions,
-            )
+        # Create a new archipelago
+        # This operation takes some time ...
+        archipelago = MyArchipelago(
+            num_islands=self.num_islands,
+            udi=user_defined_island,
+            algorithm=self.algorithm,
+            problem=fitting,
+            pop_size=self.algorithm.population_size,
+            bfe=user_defined_bfe,
+            topology=topo,
+            pygmo_seed=self.pygmo_seed,
+            with_bar=with_progress_bar,
+        )
 
-            ds.attrs["topology"] = self.topology
-            ds.attrs["result_type"] = str(fitting.sim_output)
+        # Run several evolutions in the archipelago
+        ds, df_processors, df_all_logs = archipelago.run_evolve(
+            readout=self.readout,
+            num_evolutions=self._num_evolutions,
+            num_best_decisions=self._num_best_decisions,
+        )
 
-        else:
-            raise NotImplementedError("Not implemented for 1 island.")
+        ds.attrs["topology"] = self.topology
+        ds.attrs["result_type"] = str(fitting.sim_output)
 
         self._log.info("Calibration ended.")
         return ds, df_processors, df_all_logs
 
     def run_calibration_new(
         self,
         processor: Processor,
         output_dir: Path,
         with_progress_bar: bool = True,
-    ) -> "xr.Dataset":
+    ) -> "DataTree":
         """Run calibration pipeline."""
         try:
             import pygmo as pg
         except ImportError as exc:
             raise ImportError(
                 "Missing optional package 'pygmo'.\n"
                 "Please install it with 'pip install pyxel-sim[calibration]' "
                 "or 'pip install pyxel-sim[all]'"
             ) from exc
 
         pg.set_global_rng_seed(seed=self.pygmo_seed)
         self._log.info("Pygmo seed: %d", self.pygmo_seed)
 
-        fitting = ModelFitting(
+        target_fit_range = to_fit_range(self.target_fit_range)
+        result_fit_range = FitRange3D.from_sequence(self.result_fit_range)
+
+        fitting: ModelFittingDataTree = ModelFittingDataTree(
             processor=processor,
             variables=self.parameters,
             readout=self.readout,
-            calibration_mode=CalibrationMode(self.calibration_mode),
-            simulation_output=ResultType(self.result_type),
+            simulation_output=self.result_type,
             generations=self.algorithm.generations,
             population_size=self.algorithm.population_size,
             fitness_func=self.fitness_function,
             file_path=output_dir,
-        )
-
-        fitting.configure(
-            target_output=self.target_data_path,
-            target_fit_range=self.target_fit_range,
-            out_fit_range=self.result_fit_range,
+            target_filenames=self.target_data_path,
+            target_fit_range=target_fit_range,
+            out_fit_range=result_fit_range,
             input_arguments=self.result_input_arguments,
             weights=self.weights,
             weights_from_file=self.weights_from_file,
         )
 
-        if self.num_islands <= 1:
-            raise NotImplementedError("Not implemented for 1 island.")
-
         # Create an archipelago
         user_defined_island = DaskIsland()
         user_defined_bfe = DaskBFE()
 
         if self.topology == "unconnected":
             topo = pg.unconnected()
         elif self.topology == "ring":
@@ -451,46 +471,48 @@
         elif self.topology == "fully_connected":
             topo = pg.fully_connected()
         else:
             raise NotImplementedError(f"topology {self.topology!r}")
 
         # Create a new archipelago
         # This operation takes some time ...
-        my_archipelago = MyArchipelago(
+        archipelago = ArchipelagoDataTree(
             num_islands=self.num_islands,
             udi=user_defined_island,
             algorithm=self.algorithm,
             problem=fitting,
             pop_size=self.algorithm.population_size,
             bfe=user_defined_bfe,
             topology=topo,
             pygmo_seed=self.pygmo_seed,
             with_bar=with_progress_bar,
         )
 
         # Run several evolutions in the archipelago
-        ds, _, _ = my_archipelago.run_evolve(
+        data_tree: "DataTree" = archipelago.run_evolve(
             readout=self.readout,
+            num_rows=processor.detector.geometry.row,
+            num_cols=processor.detector.geometry.col,
             num_evolutions=self._num_evolutions,
             num_best_decisions=self._num_best_decisions,
         )
 
-        ds.attrs["topology"] = self.topology
-        ds.attrs["result_type"] = str(fitting.sim_output)
+        data_tree.attrs["topology"] = self.topology
+        data_tree.attrs["result_type"] = str(fitting.sim_output)
 
         self._log.info("Calibration ended.")
-        return ds
+        return data_tree
 
-    def post_processing(
+    # TODO: This function will be deprecated (see #563)
+    def _post_processing(
         self,
         ds: "xr.Dataset",
         df_processors: "pd.DataFrame",
         output: "CalibrationOutputs",
     ) -> Sequence[Delayed]:
-        """TBW."""
         filenames: Sequence[Delayed] = output.save_processors(processors=df_processors)
 
         # TODO: Use output.fitting_plot ?
         # TODO: Use output.fitting_plot_close ?
         # TODO: Use output.calibration_plots ?
 
         return filenames
```

### Comparing `pyxel_sim-1.8/pyxel/calibration/fitness.py` & `pyxel_sim-1.9/pyxel/calibration/fitness.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     -------
     array
         TBW.
     """
     diff = target - simulated
     diff *= weighting
 
-    result = float(np.sum(np.abs(diff)))
+    result = float(np.nansum(np.abs(diff)))
     return result
 
 
 @numba.njit
 def sum_of_squared_residuals(
     simulated: np.ndarray,
     target: np.ndarray,
@@ -56,15 +56,15 @@
     array
         TBW.
     """
     diff = target - simulated
     diff_square = diff * diff
     diff_square *= weighting
 
-    result = float(np.sum(diff_square))
+    result = float(np.nansum(diff_square))
     return result
 
 
 @numba.njit
 def reduced_chi_squared(
     simulated: np.ndarray,
     target: np.ndarray,
@@ -90,11 +90,13 @@
     -------
     float
         The reduced :math:`\chi^{2}`.
     """
     diff = target - simulated
     deviation2 = np.square(diff / weighting)
 
-    degrees_of_freedom = target.size - free_parameters
-    reduced_chi2 = float(np.sum(deviation2)) / degrees_of_freedom
+    size = np.isfinite(diff).sum()
+
+    degrees_of_freedom = size - free_parameters
+    reduced_chi2 = float(np.nansum(deviation2)) / degrees_of_freedom
 
     return reduced_chi2
```

### Comparing `pyxel_sim-1.8/pyxel/calibration/fitting.py` & `pyxel_sim-1.9/pyxel/calibration/fitting.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 """:term:`CDM` model calibration with PYGMO.
 
 https://esa.github.io/pagmo2/index.html
 """
 import copy
 import logging
 import math
+from collections.abc import Sequence
 from copy import deepcopy
 from numbers import Number
 from pathlib import Path
-from typing import TYPE_CHECKING, Dict, List, Literal, Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 from dask.delayed import delayed
 from numpy.typing import NDArray
 
 from pyxel.calibration import (
@@ -30,15 +31,15 @@
     list_to_3d_slice,
     list_to_slice,
     read_data,
     read_datacubes,
 )
 from pyxel.exposure import run_exposure_pipeline
 from pyxel.observation import ParameterValues
-from pyxel.pipelines import Processor, ResultType
+from pyxel.pipelines import Processor, ResultId
 
 if TYPE_CHECKING:
     import xarray as xr
     from numpy.typing import ArrayLike
 
     from pyxel.exposure import Readout
 
@@ -48,15 +49,15 @@
 
     def __init__(
         self,
         processor: Processor,
         variables: Sequence[ParameterValues],
         readout: "Readout",
         calibration_mode: CalibrationMode,
-        simulation_output: ResultType,
+        simulation_output: ResultId,
         generations: int,
         population_size: int,
         fitness_func: FittingCallable,
         file_path: Path,
         pipeline_seed: Optional[int] = None,
     ):
         self.processor: Processor = processor
@@ -64,45 +65,45 @@
 
         self.calibration_mode: CalibrationMode = calibration_mode
         self.original_processor: Optional[Processor] = None
         self.generations: int = generations
         self.pop: int = population_size
         self.readout: Readout = readout
 
-        self.all_target_data: List[np.ndarray] = []
+        self.all_target_data: list[np.ndarray] = []
         self.weighting: Optional[np.ndarray] = None
         self.weighting_from_file: Optional[Sequence[np.ndarray]] = None
         self.fitness_func: FittingCallable = fitness_func
-        self.sim_output: ResultType = simulation_output
-        self.param_processor_list: List[Processor] = []
+        self.sim_output: ResultId = simulation_output
+        self.param_processor_list: list[Processor] = []
 
         self.file_path: Path = file_path
         self.pipeline_seed: Optional[int] = pipeline_seed
 
         self.fitness_array: Optional[np.ndarray] = None
         self.population: Optional[np.ndarray] = None
         self.champion_f_list: Optional[np.ndarray] = None
         self.champion_x_list: Optional[np.ndarray] = None
 
-        self.lbd: List[float] = []  # lower boundary
-        self.ubd: List[float] = []  # upper boundary
+        self.lbd: list[float] = []  # lower boundary
+        self.ubd: list[float] = []  # upper boundary
 
-        self.sim_fit_range: Tuple[slice, slice, slice] = (
+        self.sim_fit_range: tuple[slice, slice, slice] = (
             slice(None),
             slice(None),
             slice(None),
         )
-        self.targ_fit_range: Union[Tuple[slice, slice], Tuple[slice, slice, slice]] = (
+        self.targ_fit_range: Union[tuple[slice, slice], tuple[slice, slice, slice]] = (
             slice(None),
             slice(None),
         )
 
-        self.match: Dict[int, List[str]] = {}
+        self.match: dict[int, list[str]] = {}
 
-    def get_bounds(self) -> Tuple[Sequence[float], Sequence[float]]:
+    def get_bounds(self) -> tuple[Sequence[float], Sequence[float]]:
         """Get the box bounds of the problem (lower_boundary, upper_boundary).
 
         It also implicitly defines the dimension of the problem.
 
         Returns
         -------
         tuple of lower boundaries and upper boundaries
@@ -189,15 +190,17 @@
             check_ranges(
                 target_fit_range=target_fit_range,
                 out_fit_range=out_fit_range,
                 rows=rows,
                 cols=cols,
             )
             self.targ_fit_range = list_to_slice(target_fit_range)
-            out_fit_range = [None, None] + out_fit_range  # type: ignore
+
+            # TODO: remove 'type: ignore' and fix the issue
+            out_fit_range = [None, None, *out_fit_range]  # type: ignore
             self.sim_fit_range = list_to_3d_slice(out_fit_range)
 
             target_2d: np.ndarray
             for target_2d in target_list_2d:
                 self.all_target_data += [target_2d[self.targ_fit_range]]
 
             self._configure_weights(
@@ -287,26 +290,23 @@
                 raise ValueError(
                     'Character "_" (or a list of it) should be used to '
                     "indicate variables need to be calibrated"
                 )
 
     def get_simulated_data(self, processor: Processor) -> np.ndarray:
         """Extract 2D data from a processor."""
-        if self.sim_output == ResultType.Image:
-            simulated_data: np.ndarray = processor.result["image"][self.sim_fit_range]
-
-        elif self.sim_output == ResultType.Signal:
-            simulated_data = processor.result["signal"][self.sim_fit_range]
-        elif self.sim_output == ResultType.Pixel:
-            simulated_data = processor.result["pixel"][self.sim_fit_range]
-        else:
+        if self.sim_output not in ("image", "signal", "pixel"):
             raise NotImplementedError(
                 f"Simulation mode: {self.sim_output!r} not implemented"
             )
 
+        simulated_data: np.ndarray = processor.result[self.sim_output][
+            self.sim_fit_range
+        ]
+
         return simulated_data
 
     def calculate_fitness(
         self,
         simulated_data: np.ndarray,
         target_data: np.ndarray,
         weighting: Optional[np.ndarray] = None,
@@ -393,14 +393,16 @@
                             processor.detector.geometry.row,
                             processor.detector.geometry.col,
                         )
                     )
                 elif self.weighting_from_file is not None:
                     weighting = self.weighting_from_file[i]
 
+                # TODO: Create a multi-objective problem and use
+                #       pygmo.decompose to convert it into a single-objective problem
                 overall_fitness += self.calculate_fitness(
                     simulated_data=simulated_data,
                     target_data=target_data,
                     weighting=weighting,
                 )
 
         except Exception:
```

### Comparing `pyxel_sim-1.8/pyxel/calibration/protocols.py` & `pyxel_sim-1.9/pyxel/calibration/protocols.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Subpackage containing ``typing.Protocol`` definition."""
 
-from typing import TYPE_CHECKING, Protocol, Sequence, Tuple
+from collections.abc import Sequence
+from typing import TYPE_CHECKING, Protocol
 
 import numpy as np
 
 if TYPE_CHECKING:
     import pygmo as pg
 
 __all__ = ["IslandProtocol", "ProblemSingleObjective", "FittingCallable"]
 
 
 class IslandProtocol(Protocol):
     """Protocol for a User Define Island."""
 
     def run_evolve(
         self, algo: "pg.algorithm", pop: "pg.population"
-    ) -> Tuple["pg.algorithm", "pg.population"]:
+    ) -> tuple["pg.algorithm", "pg.population"]:
         """Run 'evolve' method."""
         ...
 
 
 class ProblemSingleObjective(Protocol):
     """Create a `Protocol` for a user defined Single Objective `Problem` for Pygmo2.
 
@@ -39,15 +40,15 @@
     def fitness(self, parameter: np.ndarray) -> Sequence[float]:
         """Return the fitness of the input decision vector.
 
         Concatenate the objectives, the equality and the inequality constraints.
         """
         ...
 
-    def get_bounds(self) -> Tuple[Sequence[float], Sequence[float]]:
+    def get_bounds(self) -> tuple[Sequence[float], Sequence[float]]:
         """Get the box bounds of the problem (lower_boundary, upper_boundary).
 
         It also implicitly defines the dimension of the problem.
         """
         ...
 
     # TODO: Add something about 'batch_fitness'
```

### Comparing `pyxel_sim-1.8/pyxel/calibration/user_defined.py` & `pyxel_sim-1.9/pyxel/calibration/user_defined.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Subpackage containing user defined Island and Batch Fitness evaluator using Dask."""
 
 import logging
-from typing import TYPE_CHECKING, Optional, Tuple
+from typing import TYPE_CHECKING, Optional
 
 import numpy as np
 from dask import array as da
 from dask.delayed import Delayed, delayed
 
 if TYPE_CHECKING:
     import pygmo as pg
@@ -147,15 +147,15 @@
 
 
 class DaskIsland:
     """User Defined Island using `Dask`."""
 
     def run_evolve(
         self, algo: "pg.algorithm", pop: "pg.population"
-    ) -> Tuple["pg.algorithm", "pg.population"]:
+    ) -> tuple["pg.algorithm", "pg.population"]:
         """Run 'evolve' method from the input `algorithm` to evolve the input `population`.
 
         Once the evolution is finished, it will return the algorithm used for the
         evolution and the evolved `population`.
 
         Parameters
         ----------
```

### Comparing `pyxel_sim-1.8/pyxel/configuration/configuration.py` & `pyxel_sim-1.9/pyxel/configuration/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 """Configuration loader."""
 
+from collections.abc import Iterator, Sequence
 from dataclasses import dataclass
 from pathlib import Path
 from shutil import copy2
-from typing import IO, TYPE_CHECKING, Any, Dict, Iterator, Optional, Sequence, Union
+from typing import IO, TYPE_CHECKING, Any, Optional, Union
 
 import yaml
 
 from pyxel import __version__ as version
 from pyxel.detectors import (
     APD,
     CCD,
@@ -602,25 +603,25 @@
         "apd_detector",
     ]
     num_detector: int = sum(key in dct for key in keys_detectors)
     if num_detector != 1:
         keys = ", ".join(map(repr, keys_detectors))
         raise ValueError(f"Expecting only one detector: {keys}")
 
-    running_mode: Dict[str, Union[Exposure, Observation, "Calibration"]] = {}
+    running_mode: dict[str, Union[Exposure, Observation, "Calibration"]] = {}
     if "exposure" in dct:
         running_mode["exposure"] = to_exposure(dct["exposure"])
     elif "observation" in dct:
         running_mode["observation"] = to_observation(dct["observation"])
     elif "calibration" in dct:
         running_mode["calibration"] = to_calibration(dct["calibration"])
     else:
         raise ValueError("No mode configuration provided.")
 
-    detector: Dict[str, Union[CCD, CMOS, MKID, APD]] = {}
+    detector: dict[str, Union[CCD, CMOS, MKID, APD]] = {}
     if "ccd_detector" in dct:
         detector["ccd_detector"] = to_ccd(dct["ccd_detector"])
     elif "cmos_detector" in dct:
         detector["cmos_detector"] = to_cmos(dct["cmos_detector"])
     elif "mkid_detector" in dct:
         detector["mkid_detector"] = to_mkid_array(dct["mkid_detector"])
     elif "apd_detector" in dct:
```

### Comparing `pyxel_sim-1.8/pyxel/data_structure/__init__.py` & `pyxel_sim-1.9/pyxel/data_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/data_structure/array.py` & `pyxel_sim-1.9/pyxel/data_structure/array.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel Array class."""
 
-from typing import TYPE_CHECKING, Optional, Tuple, Type, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 import numpy as np
 
 from pyxel.util.memory import get_size
 
 if TYPE_CHECKING:
     import xarray as xr
@@ -21,16 +21,16 @@
 # TODO: Does it make sense to force 'self._array' to be read-only ?
 #       It could be done with:
 #       ... self._array = np.array(value)
 #       ... self._array.setflags(write=False)
 class Array:
     """Array class."""
 
-    EXP_TYPE: Union[Type, np.dtype] = type(None)
-    TYPE_LIST: Tuple[np.dtype, ...] = ()
+    EXP_TYPE: Union[type, np.dtype] = type(None)
+    TYPE_LIST: tuple[np.dtype, ...] = ()
     NAME: str = ""
     UNIT: str = ""
 
     # TODO: Add units ?
     def __init__(self, value: np.ndarray):
         if value.ndim != 2:
             raise ValueError(
@@ -78,15 +78,15 @@
 
     def __array__(self, dtype: Optional[np.dtype] = None):
         if not isinstance(self._array, np.ndarray):
             raise TypeError("Array not initialized.")
         return np.asarray(self._array, dtype=dtype)
 
     @property
-    def shape(self) -> Tuple[int, int]:
+    def shape(self) -> tuple[int, int]:
         """Return array shape."""
         num_cols, num_rows = self._array.shape
         return num_cols, num_rows
 
     @property
     def ndim(self) -> int:
         """Return number of dimensions of the array."""
@@ -128,21 +128,22 @@
         -------
         int
             Size of the object in bytes.
         """
         self._numbytes = get_size(self)
         return self._numbytes
 
-    def to_xarray(self) -> "xr.DataArray":
+    def to_xarray(self, dtype: Optional[np.typing.DTypeLike] = None) -> "xr.DataArray":
         """Convert into a `DataArray` object."""
         import xarray as xr
 
         num_rows, num_cols = self.shape
         return xr.DataArray(
-            self.array,
+            np.array(self.array, dtype=dtype),
+            name=self.NAME.lower(),
             dims=["y", "x"],
             coords={"y": range(num_rows), "x": range(num_cols)},
             attrs={"units": self.UNIT, "long_name": self.NAME},
         )
 
     def plot(self, robust: bool = True) -> None:
         """Plot the array using Matplotlib.
```

### Comparing `pyxel_sim-1.8/pyxel/data_structure/charge.py` & `pyxel_sim-1.9/pyxel/data_structure/charge.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,25 +3,28 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel Charge class to generate electrons or holes inside detector."""
 
-from typing import TYPE_CHECKING, Literal, Mapping, Optional, Sequence, Tuple, Union
+from collections.abc import Mapping, Sequence
+from typing import TYPE_CHECKING, Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from pyxel.detectors.geometry import (
     get_horizontal_pixel_center_pos,
     get_vertical_pixel_center_pos,
 )
 
 if TYPE_CHECKING:
+    import xarray as xr
+
     from pyxel.detectors import Geometry
 
 
 class Charge:
     """TBW."""
 
     EXP_TYPE = float
@@ -32,15 +35,15 @@
     )
 
     def __init__(self, geo: "Geometry"):
         self._array: np.ndarray = np.zeros((geo.row, geo.col), dtype=self.EXP_TYPE)
         self._geo = geo
         self.nextid: int = 0
 
-        self.columns: Tuple[str, ...] = (
+        self.columns: tuple[str, ...] = (
             "charge",
             "number",
             "init_energy",
             "energy",
             "init_pos_ver",
             "init_pos_hor",
             "init_pos_z",
@@ -363,14 +366,28 @@
     # TODO : Try to optimize function
     def array(self) -> np.ndarray:
         """Get charge in a numpy array."""
         if not self._frame.empty:
             self._array = self.convert_df_to_array()
         return self._array
 
+    def to_xarray(self) -> "xr.DataArray":
+        """Convert into a `DataArray` object."""
+        import xarray as xr
+
+        data_2d: np.ndarray = self.array
+        num_rows, num_cols = data_2d.shape
+        return xr.DataArray(
+            data_2d,
+            name="charge",
+            dims=["y", "x"],
+            coords={"y": range(num_rows), "x": range(num_cols)},
+            attrs={"units": "electron", "long_name": "Charge"},
+        )
+
     def __array__(self, dtype: Optional[np.dtype] = None):
         if not isinstance(self._array, np.ndarray):
             raise TypeError("Array not initialized.")
         return np.asarray(self._array, dtype=dtype)
 
     @property
     def frame(self) -> pd.DataFrame:
```

### Comparing `pyxel_sim-1.8/pyxel/data_structure/image.py` & `pyxel_sim-1.9/pyxel/data_structure/image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/data_structure/persistence.py` & `pyxel_sim-1.9/pyxel/data_structure/persistence.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 #
 #
 """Persistence classes."""
 
+from collections.abc import Sequence
 from dataclasses import dataclass
-from typing import Sequence, Tuple
 
 import numpy as np
 
 
 @dataclass
 class Trap:
     """Trap dataclass."""
@@ -26,15 +26,15 @@
 class Persistence:
     """Persistence class."""
 
     def __init__(
         self,
         trap_time_constants: Sequence[float],
         trap_proportions: Sequence[float],
-        geometry: Tuple[int, int],
+        geometry: tuple[int, int],
     ):
         traps: Sequence[Trap] = [
             Trap(
                 time_constant=time_constant,
                 proportion=trap_proportion,
                 charge=np.zeros(geometry),
             )
@@ -97,15 +97,15 @@
 class SimplePersistence:
     """Simple persistence dataclass."""
 
     def __init__(
         self,
         trap_time_constants: Sequence[float],
         trap_densities: Sequence[float],
-        geometry: Tuple[int, int],
+        geometry: tuple[int, int],
     ):
         traps: Sequence[SimpleTrap] = [
             SimpleTrap(
                 time_constant=time_constant,
                 density=trap_density,
                 charge=np.zeros(geometry),
             )
```

### Comparing `pyxel_sim-1.8/pyxel/data_structure/phase.py` & `pyxel_sim-1.9/pyxel/data_structure/phase.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/data_structure/photon.py` & `pyxel_sim-1.9/pyxel/data_structure/photon.py`

 * *Files 9% similar despite different names*

```diff
@@ -56,11 +56,12 @@
         """
         self.validate_type(value)
         self.validate_shape(value)
 
         if np.any(value < 0):
             value[value < 0] = 0.0
             warnings.warn(
-                "Trying to set negative values in the Photon array! Negative values clipped to 0."
+                "Trying to set negative values in the Photon array! Negative values clipped to 0.",
+                stacklevel=2,
             )
 
         self._array = value
```

### Comparing `pyxel_sim-1.8/pyxel/data_structure/pixel.py` & `pyxel_sim-1.9/pyxel/data_structure/pixel.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/data_structure/processed_data.py` & `pyxel_sim-1.9/pyxel/data_structure/processed_data.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/data_structure/scene.py` & `pyxel_sim-1.9/pyxel/data_structure/scene.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel Scene class to track multi-wavelength photon."""
 
-from typing import TYPE_CHECKING, Mapping, Sequence
+from collections.abc import Mapping, Sequence
+from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import numpy as np
     from astropy.io.fits import ImageHDU
     from astropy.table import Table
     from scopesim import Source
```

### Comparing `pyxel_sim-1.8/pyxel/data_structure/signal.py` & `pyxel_sim-1.9/pyxel/data_structure/signal.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/data_structure/util.py` & `pyxel_sim-1.9/pyxel/data_structure/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/detectors/__init__.py` & `pyxel_sim-1.9/pyxel/detectors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/detectors/apd/__init__.py` & `pyxel_sim-1.9/pyxel/detectors/apd/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/detectors/apd/apd.py` & `pyxel_sim-1.9/pyxel/detectors/apd/apd.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """:term:`APD` detector modeling class."""
 
-from typing import TYPE_CHECKING, Mapping, Optional
+from collections.abc import Mapping
+from typing import TYPE_CHECKING, Optional
 
 from pyxel.detectors import Detector
 
 if TYPE_CHECKING:
     import pandas as pd
 
     from pyxel.detectors import APDCharacteristics, APDGeometry, Environment
@@ -76,14 +77,15 @@
                 "signal": None if self._signal is None else self._signal.array.copy(),
                 "image": None if self._image is None else self._image.array.copy(),
                 "processed_data": (
                     None
                     if self._processed_data is None
                     else self._processed_data.data.to_dict()
                 ),
+                "data": None if self._data is None else self._data.to_dict(),
                 "charge": (
                     None
                     if self._charge is None
                     else {
                         "array": self._charge.array.copy(),
                         "frame": self._charge.frame.copy(),
                     }
@@ -96,14 +98,15 @@
     # TODO: Refactor this
     @classmethod
     def from_dict(cls, dct: Mapping) -> "APD":
         """Create a new instance of `APD` from a `dict`."""
         # TODO: This is a simplistic implementation. Improve this.
         import numpy as np
         import xarray as xr
+        from datatree import DataTree
 
         from pyxel.data_structure import Scene
         from pyxel.detectors import APDCharacteristics, APDGeometry, Environment
 
         if dct["type"] != "APD":
             raise ValueError
 
@@ -134,14 +137,21 @@
             detector.pixel.array = np.asarray(data["pixel"])
         if "signal" in data:
             detector.signal.array = np.asarray(data["signal"])
         if "image" in data:
             detector.image.array = np.asarray(data["image"])
         if "processed_data" in data:
             detector.processed_data._data = xr.Dataset.from_dict(data["processed_data"])
+        if "data" in data:
+            detector._data = DataTree.from_dict(
+                {
+                    key: xr.Dataset.from_dict(value)
+                    for key, value in data["data"].items()
+                }
+            )
         if "charge" in data and data["charge"] is not None:
             charge_dct = data["charge"]
             detector.charge._array = np.asarray(charge_dct["array"])
 
             new_frame: pd.DataFrame = charge_dct["frame"]
             previous_frame: pd.DataFrame = detector.charge._frame
             detector.charge._frame = new_frame[previous_frame.columns]
```

### Comparing `pyxel_sim-1.8/pyxel/detectors/apd/apd_characteristics.py` & `pyxel_sim-1.9/pyxel/detectors/apd/apd_characteristics.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 [5] I. M. Baker et al., Linear-mode avalanche photodiode arrays in HgCdTe at Leonardo, UK: the
 current status, in Image Sensing Technologies: Materials, Devices, Systems, and Applications VI,
 2019, vol. 10980, no. May, p. 20.
 """
 
 import math
-from typing import Mapping, Optional, Tuple
+from collections.abc import Mapping
+from typing import Optional
 
 import numpy as np
 from toolz import dicttoolz
 
 from pyxel.util.memory import get_size
 
 
@@ -62,15 +63,15 @@
 
     def __init__(
         self,
         roic_gain: float,  # unit: V
         quantum_efficiency: Optional[float] = None,  # unit: NA
         full_well_capacity: Optional[float] = None,  # unit: electron
         adc_bit_resolution: Optional[int] = None,
-        adc_voltage_range: Optional[Tuple[float, float]] = None,  # unit: V
+        adc_voltage_range: Optional[tuple[float, float]] = None,  # unit: V
         avalanche_gain: Optional[float] = None,  # unit: electron/electron
         pixel_reset_voltage: Optional[float] = None,  # unit: V
         common_voltage: Optional[float] = None,  # unit: V
     ):
         self._avalanche_gain = avalanche_gain
         self._common_voltage = common_voltage
         self._pixel_reset_voltage = pixel_reset_voltage
@@ -238,25 +239,25 @@
 
     @adc_bit_resolution.setter
     def adc_bit_resolution(self, value: int) -> None:
         """Set bit resolution of the Analog-Digital Converter."""
         self._adc_bit_resolution = value
 
     @property
-    def adc_voltage_range(self) -> Tuple[float, float]:
+    def adc_voltage_range(self) -> tuple[float, float]:
         """Get voltage range of the Analog-Digital Converter."""
         if self._adc_voltage_range:
             return self._adc_voltage_range
         else:
             raise ValueError(
                 "'adc_voltage_range' not specified in detector characteristics."
             )
 
     @adc_voltage_range.setter
-    def adc_voltage_range(self, value: Tuple[float, float]) -> None:
+    def adc_voltage_range(self, value: tuple[float, float]) -> None:
         """Set voltage range of the Analog-Digital Converter."""
         self._adc_voltage_range = value
 
     @property
     def full_well_capacity(self) -> float:
         """Get Full well capacity."""
         if self._full_well_capacity:
```

### Comparing `pyxel_sim-1.8/pyxel/detectors/apd/apd_geometry.py` & `pyxel_sim-1.9/pyxel/detectors/apd/apd_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/detectors/ccd/ccd.py` & `pyxel_sim-1.9/pyxel/detectors/ccd/ccd.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """CCD detector modeling class."""
 
-from typing import TYPE_CHECKING, Mapping, Optional
+from collections.abc import Mapping
+from typing import TYPE_CHECKING, Optional
 
 from pyxel.detectors import Detector
 
 if TYPE_CHECKING:
     import pandas as pd
 
     from pyxel.detectors import CCDGeometry, Characteristics, Environment
@@ -69,14 +70,20 @@
                 "signal": None if self._signal is None else self._signal.array.copy(),
                 "image": None if self._image is None else self._image.array.copy(),
                 "processed_data": (
                     None
                     if self._processed_data is None
                     else self._processed_data.data.to_dict()
                 ),
+                "data": None
+                if self._data is None
+                else {
+                    key.replace("/", "#"): value
+                    for key, value in self._data.to_dict().items()
+                },
                 "charge": (
                     None
                     if self._charge is None
                     else {
                         "array": self._charge.array.copy(),
                         "frame": self._charge.frame.copy(),
                     }
@@ -89,14 +96,15 @@
     # TODO: Refactor this
     @classmethod
     def from_dict(cls, dct: Mapping) -> "CCD":
         """Create a new instance of `CCD` from a `dict`."""
         # TODO: This is a simplistic implementation. Improve this.
         import numpy as np
         import xarray as xr
+        from datatree import DataTree
 
         from pyxel.data_structure import Scene
         from pyxel.detectors import CCDGeometry, Characteristics, Environment
 
         if dct["type"] != "CCD":
             raise ValueError
 
@@ -127,14 +135,21 @@
             detector.pixel.array = np.asarray(data["pixel"])
         if "signal" in data:
             detector.signal.array = np.asarray(data["signal"])
         if "image" in data:
             detector.image.array = np.asarray(data["image"])
         if "processed_data" in data:
             detector.processed_data._data = xr.Dataset.from_dict(data["processed_data"])
+        if "data" in data:
+            detector._data = DataTree.from_dict(
+                {
+                    key.replace("#", "/"): xr.Dataset.from_dict(value)
+                    for key, value in data["data"].items()
+                }
+            )
         if "charge" in data and data["charge"] is not None:
             charge_dct = data["charge"]
             detector.charge._array = np.asarray(charge_dct["array"])
 
             new_frame: pd.DataFrame = charge_dct["frame"]
             previous_frame: pd.DataFrame = detector.charge._frame
             detector.charge._frame = new_frame[previous_frame.columns]
```

### Comparing `pyxel_sim-1.8/pyxel/detectors/ccd/ccd_geometry.py` & `pyxel_sim-1.9/pyxel/detectors/ccd/ccd_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/detectors/characteristics.py` & `pyxel_sim-1.9/pyxel/detectors/characteristics.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 
-from typing import Iterable, Mapping, Optional, Tuple
+from collections.abc import Iterable, Mapping
+from typing import Optional
 
 import numpy as np
 from toolz import dicttoolz
 
 from pyxel.util.memory import get_size
 
 
@@ -37,15 +38,15 @@
     def __init__(
         self,
         quantum_efficiency: Optional[float] = None,  # unit: NA
         charge_to_volt_conversion: Optional[float] = None,  # unit: volt/electron
         pre_amplification: Optional[float] = None,  # unit: V/V
         full_well_capacity: Optional[float] = None,  # unit: electron
         adc_bit_resolution: Optional[int] = None,
-        adc_voltage_range: Optional[Tuple[float, float]] = None,  # unit: V
+        adc_voltage_range: Optional[tuple[float, float]] = None,  # unit: V
     ):
         if quantum_efficiency and not (0.0 <= quantum_efficiency <= 1.0):
             raise ValueError("'quantum_efficiency' must be between 0.0 and 1.0.")
         if charge_to_volt_conversion and not (
             0.0 <= charge_to_volt_conversion <= 100.0
         ):
             raise ValueError(
@@ -60,15 +61,23 @@
         if adc_voltage_range and not len(adc_voltage_range) == 2:
             raise ValueError("Voltage range must have length of 2.")
 
         self._quantum_efficiency = quantum_efficiency
         self._charge_to_volt_conversion = charge_to_volt_conversion
         self._pre_amplification = pre_amplification
         self._full_well_capacity = full_well_capacity
-        self._adc_voltage_range = adc_voltage_range
+
+        if adc_voltage_range is None:
+            volt_range: Optional[tuple[float, float]] = None
+        else:
+            # Force 'volt_range' to be a tuple of 2 elements
+            start_volt, end_volt = adc_voltage_range
+            volt_range = (start_volt, end_volt)
+
+        self._adc_voltage_range = volt_range
         self._adc_bit_resolution = adc_bit_resolution
 
         self._numbytes = 0
 
     def __eq__(self, other) -> bool:
         return (
             type(self) == type(other)
@@ -147,25 +156,25 @@
 
     @adc_bit_resolution.setter
     def adc_bit_resolution(self, value: int) -> None:
         """Set bit resolution of the Analog-Digital Converter."""
         self._adc_bit_resolution = value
 
     @property
-    def adc_voltage_range(self) -> Tuple[float, float]:
+    def adc_voltage_range(self) -> tuple[float, float]:
         """Get voltage range of the Analog-Digital Converter."""
         if self._adc_voltage_range:
             return self._adc_voltage_range
         else:
             raise ValueError(
                 "'adc_voltage_range' not specified in detector characteristics."
             )
 
     @adc_voltage_range.setter
-    def adc_voltage_range(self, value: Tuple[float, float]) -> None:
+    def adc_voltage_range(self, value: tuple[float, float]) -> None:
         """Set voltage range of the Analog-Digital Converter."""
         self._adc_voltage_range = value
 
     @property
     def full_well_capacity(self) -> float:
         """Get Full well capacity."""
         if self._full_well_capacity:
@@ -222,13 +231,13 @@
         # TODO: This is a simplistic implementation. Improve this.
 
         # Extract param 'adc_voltage_range'
         param: Optional[Iterable[float]] = dct.get("adc_voltage_range")
         new_dct: Mapping = dicttoolz.dissoc(dct, "adc_voltage_range")
 
         if param is None:
-            adc_voltage_range: Optional[Tuple[float, float]] = None
+            adc_voltage_range: Optional[tuple[float, float]] = None
         else:
             adc_voltage_min, adc_voltage_max = tuple(param)
             adc_voltage_range = adc_voltage_min, adc_voltage_max
 
         return cls(adc_voltage_range=adc_voltage_range, **new_dct)
```

### Comparing `pyxel_sim-1.8/pyxel/detectors/cmos/cmos.py` & `pyxel_sim-1.9/pyxel/detectors/cmos/cmos.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """:term:`CMOS` detector modeling class."""
 
-from typing import TYPE_CHECKING, Mapping, Optional
+from collections.abc import Mapping
+from typing import TYPE_CHECKING, Optional
 
 from pyxel.detectors import Detector
 
 if TYPE_CHECKING:
     import pandas as pd
 
     from pyxel.detectors import Characteristics, CMOSGeometry, Environment
@@ -69,14 +70,15 @@
                 "signal": None if self._signal is None else self._signal.array.copy(),
                 "image": None if self._image is None else self._image.array.copy(),
                 "processed_data": (
                     None
                     if self._processed_data is None
                     else self._processed_data.data.to_dict()
                 ),
+                "data": None if self._data is None else self._data.to_dict(),
                 "charge": (
                     None
                     if self._charge is None
                     else {
                         "array": self._charge.array.copy(),
                         "frame": self._charge.frame.copy(),
                     }
@@ -89,14 +91,15 @@
     # TODO: Refactor this
     @classmethod
     def from_dict(cls, dct: Mapping) -> "CMOS":
         """Create a new instance of `CMOS` from a `dict`."""
         # TODO: This is a simplistic implementation. Improve this.
         import numpy as np
         import xarray as xr
+        from datatree import DataTree
 
         from pyxel.data_structure import Scene
         from pyxel.detectors import Characteristics, CMOSGeometry, Environment
 
         if dct["type"] != "CMOS":
             raise ValueError
 
@@ -127,14 +130,21 @@
             detector.pixel.array = np.asarray(data["pixel"])
         if "signal" in data:
             detector.signal.array = np.asarray(data["signal"])
         if "image" in data:
             detector.image.array = np.asarray(data["image"])
         if "processed_data" in data:
             detector.processed_data._data = xr.Dataset.from_dict(data["processed_data"])
+        if "data" in data:
+            detector._data = DataTree.from_dict(
+                {
+                    key: xr.Dataset.from_dict(value)
+                    for key, value in data["data"].items()
+                }
+            )
         if "charge" in data and data["charge"] is not None:
             charge_dct = data["charge"]
             detector.charge._array = np.asarray(charge_dct["array"])
 
             new_frame: pd.DataFrame = charge_dct["frame"]
             previous_frame: pd.DataFrame = detector.charge._frame
             detector.charge._frame = new_frame[previous_frame.columns]
```

### Comparing `pyxel_sim-1.8/pyxel/detectors/cmos/cmos_geometry.py` & `pyxel_sim-1.9/pyxel/detectors/cmos/cmos_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/detectors/detector.py` & `pyxel_sim-1.9/pyxel/detectors/detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Detector class."""
 import collections
+from collections.abc import Mapping
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, Mapping, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 import numpy as np
 
 from pyxel import __version__, backends
 from pyxel.data_structure import (
     Charge,
     Image,
@@ -25,38 +26,40 @@
     SimplePersistence,
 )
 from pyxel.detectors import Environment, ReadoutProperties
 from pyxel.util.memory import get_size, memory_usage_details
 
 if TYPE_CHECKING:
     import xarray as xr
+    from datatree import DataTree
 
 
 __all__ = ["Detector"]
 
 
 # TODO: Add methods to save/load a `Detector` instance to the filesystem. See #329
 class Detector:
     """The detector class."""
 
     def __init__(self, environment: Optional[Environment] = None):
         self.environment: Environment = environment or Environment()
 
-        self.header: Dict[str, object] = collections.OrderedDict()
+        self.header: dict[str, object] = collections.OrderedDict()
 
         self._photon: Optional[Photon] = None
         self._scene: Optional[Scene] = None
         self._charge: Optional[Charge] = None
         self._pixel: Optional[Pixel] = None
         self._signal: Optional[Signal] = None
         self._image: Optional[Image] = None
         self._processed_data: Optional[ProcessedData] = None
+        self._data: Optional[DataTree] = None
 
         # This will be the memory of the detector where trapped charges will be saved
-        self._memory: Dict = {}
+        self._memory: dict = {}
         self._persistence: Optional[Union[Persistence, SimplePersistence]] = None
 
         self.input_image: Optional[np.ndarray] = None
         self._output_dir: Optional[Path] = None  # TODO: See #330
 
         self._readout_properties: Optional["ReadoutProperties"] = None
 
@@ -68,14 +71,22 @@
             and self._photon == other._photon
             and self._scene == other._scene
             and self._charge == other._charge
             and self._pixel == other._pixel
             and self._signal == other._signal
             and self._image == other._image
             and self._processed_data == other._processed_data
+            and (
+                (self._data is None and other._data is None)
+                or (
+                    self._data is not None
+                    and other._data is not None
+                    and self._data.equals(other._data)
+                )
+            )
         )
 
     @property
     def geometry(self):
         """TBW."""
         raise NotImplementedError
 
@@ -135,22 +146,31 @@
     def image(self) -> Image:
         """TBW."""
         if not self._image:
             raise RuntimeError("'image' not initialized.")
 
         return self._image
 
+    # TODO: This will be deprecated
     @property
     def processed_data(self) -> ProcessedData:
         """TBW."""
         if not self._processed_data:
             raise RuntimeError("'processed_data' not initialized.")
 
         return self._processed_data
 
+    @property
+    def data(self) -> "DataTree":
+        """TBW."""
+        if self._data is None:
+            raise RuntimeError("'data' not initialized.")
+
+        return self._data
+
     def to_xarray(self) -> "xr.Dataset":
         """Create a new ``Dataset`` from all data containers.
 
         Examples
         --------
         >>> detector.to_xarray()
         <xarray.Dataset>
@@ -179,31 +199,30 @@
 
         ds.attrs.update({"detector": type(self).__name__, "pyxel version": __version__})
 
         return ds
 
     def reset(self) -> None:
         """TBW."""
+        from datatree import DataTree
+
         self._photon = Photon(geo=self.geometry)
         self._scene = None
         self._charge = Charge(geo=self.geometry)
         self._pixel = Pixel(geo=self.geometry)
         self._signal = Signal(geo=self.geometry)
         self._image = Image(geo=self.geometry)
 
         if self._processed_data is None:
             self._processed_data = ProcessedData()
 
-    def empty(self, empty_all: bool = True) -> None:
-        """Empty the data in the detector.
+        self._data = DataTree()
 
-        Returns
-        -------
-        None
-        """
+    def empty(self, empty_all: bool = True) -> None:
+        """Empty the data in the detector."""
         if self._photon:
             self.photon.array *= 0
 
         self._scene = None
 
         if self._signal:
             self.signal.array *= 0
@@ -315,15 +334,15 @@
         """TBW."""
         if self._readout_properties is not None:
             return self._readout_properties.num_steps
         else:
             raise ValueError("No readout defined.")
 
     @property
-    def pipeline_count(self) -> float:
+    def pipeline_count(self) -> int:
         """TBW."""
         if self._readout_properties is not None:
             return self._readout_properties.pipeline_count
         else:
             raise ValueError("No readout defined.")
 
     @pipeline_count.setter
@@ -331,14 +350,24 @@
         """TBW."""
         if self._readout_properties is not None:
             self._readout_properties.pipeline_count = value
         else:
             raise ValueError("No readout defined.")
 
     @property
+    def is_first_readout(self) -> bool:
+        """Check if this is the first readout time."""
+        return bool(self.pipeline_count == 0)
+
+    @property
+    def is_last_readout(self) -> bool:
+        """Check if this is the last readout time."""
+        return bool(self.pipeline_count == (self.num_steps - 1))
+
+    @property
     def read_out(self) -> bool:
         """TBW."""
         if self._readout_properties is not None:
             return self._readout_properties.read_out
         else:
             raise ValueError("No readout defined.")
```

### Comparing `pyxel_sim-1.8/pyxel/detectors/environment.py` & `pyxel_sim-1.9/pyxel/detectors/environment.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 
-from typing import Mapping, Optional
+from collections.abc import Mapping
+from typing import Optional
 
 from pyxel.util.memory import get_size
 
 
 class Environment:
     """Environmental attributes of the detector.
```

### Comparing `pyxel_sim-1.8/pyxel/detectors/geometry.py` & `pyxel_sim-1.9/pyxel/detectors/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Geometry class for detector."""
 
-from typing import Mapping, Optional, Tuple
+from collections.abc import Mapping
+from typing import Optional
 
 import numpy as np
 
 from pyxel.util.memory import get_size
 
 
 def get_vertical_pixel_center_pos(
@@ -137,15 +138,15 @@
         """Set Number of pixel columns."""
         if value <= 0:
             raise ValueError("'col' must be strictly greater than 0.")
 
         self._col = value
 
     @property
-    def shape(self) -> Tuple[int, int]:
+    def shape(self) -> tuple[int, int]:
         """Return detector shape."""
         return self.row, self.col
 
     @property
     def total_thickness(self) -> float:
         """Get Thickness of detector."""
         if self._total_thickness:
```

### Comparing `pyxel_sim-1.8/pyxel/detectors/mkid/mkid.py` & `pyxel_sim-1.9/pyxel/detectors/mkid/mkid.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """:term:`MKID`-array detector modeling class."""
 
-from typing import TYPE_CHECKING, Mapping, Optional
+from collections.abc import Mapping
+from typing import TYPE_CHECKING, Optional
 
 from pyxel.data_structure import Phase
 from pyxel.detectors import Detector
 from pyxel.util.memory import memory_usage_details
 
 if TYPE_CHECKING:
     import pandas as pd
@@ -132,14 +133,15 @@
                 "image": None if self._image is None else self._image.array.copy(),
                 "phase": None if self._phase is None else self._phase.array.copy(),
                 "processed_data": (
                     None
                     if self._processed_data is None
                     else self._processed_data.data.to_dict()
                 ),
+                "data": None if self._data is None else self._data.to_dict(),
                 "charge": (
                     None
                     if self._charge is None
                     else {
                         "array": self._charge.array.copy(),
                         "frame": self._charge.frame.copy(),
                     }
@@ -152,14 +154,15 @@
     # TODO: Refactor this
     @classmethod
     def from_dict(cls, dct: Mapping) -> "MKID":
         """Create a new instance of `MKID` from a `dict`."""
         # TODO: This is a simplistic implementation. Improve this.
         import numpy as np
         import xarray as xr
+        from datatree import DataTree
 
         from pyxel.data_structure import Scene
         from pyxel.detectors import Characteristics, Environment, MKIDGeometry
 
         if dct["type"] != "MKID":
             raise ValueError
 
@@ -190,14 +193,21 @@
             detector.pixel.array = np.asarray(data["pixel"])
         if "signal" in data:
             detector.signal.array = np.asarray(data["signal"])
         if "image" in data:
             detector.image.array = np.asarray(data["image"])
         if "processed_data" in data:
             detector.processed_data._data = xr.Dataset.from_dict(data["processed_data"])
+        if "data" in data:
+            detector._data = DataTree.from_dict(
+                {
+                    key: xr.Dataset.from_dict(value)
+                    for key, value in data["data"].items()
+                }
+            )
         if "charge" in data and data["charge"] is not None:
             charge_dct = data["charge"]
             detector.charge._array = np.asarray(charge_dct["array"])
 
             new_frame: pd.DataFrame = charge_dct["frame"]
             previous_frame: pd.DataFrame = detector.charge._frame
             detector.charge._frame = new_frame[previous_frame.columns]
```

### Comparing `pyxel_sim-1.8/pyxel/detectors/mkid/mkid_geometry.py` & `pyxel_sim-1.9/pyxel/detectors/mkid/mkid_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/detectors/readout_properties.py` & `pyxel_sim-1.9/pyxel/detectors/readout_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #  Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022.
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
-#
-#
+
 """Sampling detector properties class."""
 
 
 class ReadoutProperties:
     """Sampling detector properties.
 
     Parameters
@@ -104,15 +103,15 @@
 
     @read_out.setter
     def read_out(self, value: bool) -> None:
         """TBW."""
         self._read_out = value
 
     @property
-    def pipeline_count(self) -> float:
+    def pipeline_count(self) -> int:
         """TBW."""
         return self._pipeline_count
 
     @pipeline_count.setter
     def pipeline_count(self, value: int) -> None:
         """TBW."""
         self._pipeline_count = value
```

### Comparing `pyxel_sim-1.8/pyxel/evaluator.py` & `pyxel_sim-1.9/pyxel/evaluator.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 import importlib
 from ast import literal_eval
 from collections import abc
+from collections.abc import Sequence
 from numbers import Number
-from typing import Callable, Sequence, Union
+from typing import Callable, Union
 
 import numpy as np
 
 __all__ = ["evaluate_reference", "eval_range", "eval_entry"]
 
 
 def evaluate_reference(reference_str: str) -> Callable:
@@ -66,15 +67,15 @@
             globals_dict = None
             values_array: np.ndarray = eval(values, globals_dict, locals_dict)
 
             # NOTE: the following casting is to ensure JSON serialization works
             # JSON does not accept numpy.int* or numpy.float* types.
             if values_array.dtype == float:
                 values_lst: list = [float(value) for value in values_array]
-            elif values_array.dtype == int:
+            elif values_array.dtype in (int, np.int64):
                 values_lst = [int(value) for value in values_array]
             else:
                 raise NotImplementedError(
                     f"numpy data type is not a float or int: {values_array!r}"
                 )
         # Preventing any problems with evaluating _ as a variable in outer scope.
         elif values == "_":
```

### Comparing `pyxel_sim-1.8/pyxel/exposure/__init__.py` & `pyxel_sim-1.9/pyxel/observation/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 #  Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022.
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
-#
-#
-"""Observation classes and function."""
+
+"""TBW."""
 
 # flake8: noqa
-from .readout import Readout
-from .exposure import Exposure, run_exposure_pipeline
+from .observation import (
+    Observation,
+    ParameterValues,
+    ParameterMode,
+    ObservationResult,
+    log_parameters,
+)
```

### Comparing `pyxel_sim-1.8/pyxel/exposure/readout.py` & `pyxel_sim-1.9/pyxel/exposure/readout.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 #
 #
 """TBW."""
 
-from typing import Iterator, Optional, Sequence, Tuple, Union
+from collections.abc import Iterator, Sequence
+from typing import Optional, Union
 
 import numpy as np
 
 from pyxel import load_table
 from pyxel.evaluator import eval_range
 
 
@@ -71,15 +72,15 @@
 
     def _set_steps(self) -> None:
         """TBW."""
         self._times, self._steps = calculate_steps(self._times, self._start_time)
         self._times_linear = bool(np.all(self._steps == self._steps[0]))
         self._num_steps = len(self._times)
 
-    def time_step_it(self) -> Iterator[Tuple[float, float]]:
+    def time_step_it(self) -> Iterator[tuple[float, float]]:
         """TBW."""
         return zip(self._times, self._steps)
 
     @property
     def start_time(self) -> float:
         """Return start time."""
         return self._start_time
@@ -131,15 +132,15 @@
     def non_destructive(self, value: bool) -> None:
         """Set non-destructive mode."""
         self._non_destructive = value
 
 
 def calculate_steps(
     times: np.ndarray, start_time: float
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Calculate time differences for a given array and start time.
 
     Parameters
     ----------
     times: ndarray
     start_time: float
```

### Comparing `pyxel_sim-1.8/pyxel/inputs/loader.py` & `pyxel_sim-1.9/pyxel/inputs/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,42 +4,44 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Subpackage to load images and tables."""
 
 import csv
+from collections.abc import Sequence
 from contextlib import suppress
 from io import BytesIO, StringIO
 from pathlib import Path
-from typing import TYPE_CHECKING, Sequence, Union
+from typing import TYPE_CHECKING, Union
 
 import fsspec
 import numpy as np
 from numpy.typing import DTypeLike
 from PIL import Image
 
 from pyxel.options import global_options
 
 if TYPE_CHECKING:
     import pandas as pd
+    import xarray as xr
 
 
 def load_image(filename: Union[str, Path]) -> np.ndarray:
     """Load a 2D image.
 
     Parameters
     ----------
     filename : str or Path
         Filename to read an image.
         {.npy, .fits, .txt, .data, .jpg, .jpeg, .bmp, .png, .tiff} are accepted.
 
     Returns
     -------
-    array : ndarray
+    ndarray
         A 2D array.
 
     Raises
     ------
     FileNotFoundError
         If an image is not found.
     ValueError
@@ -215,14 +217,57 @@
 
     else:
         raise ValueError("Only .npy, .xlsx, .csv, .txt and .data implemented.")
 
     return table
 
 
+def load_dataarray(filename: Union[str, Path]) -> "xr.DataArray":
+    """Load a ``DataArray`` image.
+
+    Parameters
+    ----------
+    filename : str of Path
+
+    Returns
+    -------
+    DataArray
+        A multi-dimensional array.
+
+    Raises
+    ------
+    FileNotFoundError
+        If an image is not found.
+    """
+    if isinstance(filename, Path):
+        full_filename: Path = filename.expanduser().resolve()
+        if not full_filename.exists():
+            raise FileNotFoundError(f"Input file '{full_filename}' can not be found.")
+
+        url_path: str = str(full_filename)
+
+    else:
+        url_path = filename
+
+    # Define extra parameters to use with 'fsspec'
+    extras = {}
+    if global_options.cache_enabled:
+        url_path = f"simplecache::{url_path}"
+
+        if global_options.cache_folder:
+            extras["simplecache"] = {"cache_storage": global_options.cache_folder}
+
+    import xarray as xr
+
+    with fsspec.open(url_path, mode="rb", **extras) as file_handler:
+        data_array = xr.load_dataarray(file_handler)
+
+    return data_array
+
+
 def load_datacube(filename: Union[str, Path]) -> np.ndarray:
     """Load a 3D datacube.
 
     Parameters
     ----------
     filename : str or Path
         Filename to read a datacube.
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_collection/__init__.py` & `pyxel_sim-1.9/pyxel/models/charge_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_collection/collection.py` & `pyxel_sim-1.9/pyxel/models/charge_collection/collection.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_collection/diffusion.py` & `pyxel_sim-1.9/pyxel/models/charge_collection/diffusion.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_collection/fixed_pattern_noise.py` & `pyxel_sim-1.9/pyxel/models/charge_collection/fixed_pattern_noise.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Fix pattern noise model."""
 
 from pathlib import Path
-from typing import Literal, Optional, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 
 from pyxel.detectors import Detector, Geometry
 from pyxel.util import load_cropped_and_aligned_image, set_random_seed
 
 
 def fpn_from_file(
     geometry: Geometry,
     filename: Union[Path, str],
-    position: Tuple[int, int] = (0, 0),
+    position: tuple[int, int] = (0, 0),
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ] = None,
 ) -> np.ndarray:
     """Get fixed pattern noise caused by pixel non-uniformity during charge collection from a file.
 
     Parameters
@@ -64,15 +64,15 @@
         align=align,
     )
 
     return prnu_2d
 
 
 def compute_simple_prnu(
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     quantum_efficiency: float,
     fixed_pattern_noise_factor: float,
 ) -> np.ndarray:
     """Compute fixed pattern noise caused by pixel non-uniformity during charge collection.
 
     Parameters
     ----------
@@ -95,15 +95,15 @@
 
     return prnu_2
 
 
 def fixed_pattern_noise(
     detector: Detector,
     filename: Union[Path, str, None] = None,
-    position: Tuple[int, int] = (0, 0),
+    position: tuple[int, int] = (0, 0),
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ] = None,
     fixed_pattern_noise_factor: Optional[float] = None,
     seed: Optional[int] = None,
 ) -> None:
     """Add fixed pattern noise caused by pixel non-uniformity during charge collection.
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_collection/full_well.py` & `pyxel_sim-1.9/pyxel/models/charge_collection/full_well.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_collection/inter_pixel_capacitance.py` & `pyxel_sim-1.9/pyxel/models/charge_collection/inter_pixel_capacitance.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         dtype=float,
     )
 
     return kernel
 
 
 def compute_ipc_convolution(
-    input: np.ndarray,
+    input: np.ndarray,  # noqa: A002
     coupling: float,
     diagonal_coupling: float,
     anisotropic_coupling: float,
 ) -> np.ndarray:
     """Compute convolution of the array with IPC kernel.
 
     Parameters
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_collection/persistence.py` & `pyxel_sim-1.9/pyxel/models/charge_collection/persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,16 +72,17 @@
 
 TO DO:
    - Add temperature dependency
    - Add default -flat?- trap maps
 
 """
 
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Literal, Optional, Sequence, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numba
 import numpy as np
 
 from pyxel.data_structure import Persistence, SimplePersistence
 from pyxel.detectors import CMOS
 from pyxel.util import load_cropped_and_aligned_image
@@ -158,15 +159,15 @@
 def compute_simple_persistence(
     pixel_array: np.ndarray,
     all_trapped_charge: np.ndarray,
     trap_densities: np.ndarray,
     trap_time_constants: np.ndarray,
     delta_t: float,
     trap_capacities: Optional[np.ndarray] = None,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Compute simple persistence.
 
     Parameters
     ----------
     pixel_array : ndarray
     all_trapped_charge : ndarray
     trap_densities : ndarray
@@ -226,19 +227,19 @@
 
 def persistence(
     detector: CMOS,
     trap_time_constants: Sequence[float],
     trap_proportions: Sequence[float],
     trap_densities_filename: Union[Path, str],
     trap_capacities_filename: Optional[Union[Path, str]] = None,
-    trap_densities_position: Tuple[int, int] = (0, 0),
+    trap_densities_position: tuple[int, int] = (0, 0),
     trap_densities_align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ] = None,
-    trap_capacities_position: Tuple[int, int] = (0, 0),
+    trap_capacities_position: tuple[int, int] = (0, 0),
     trap_capacities_align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ] = None,
 ) -> None:
     """Apply persistence model.
 
     Parameters
@@ -345,15 +346,15 @@
     pixel_array: np.ndarray,
     all_trapped_charge: np.ndarray,
     trap_proportions: np.ndarray,
     trap_time_constants: np.ndarray,
     trap_densities_2d: np.ndarray,
     delta_t: float,
     trap_capacities_2d: Optional[np.ndarray] = None,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Compute persistence.
 
     Parameters
     ----------
     pixel_array : ndarray
     all_trapped_charge : ndarray
     trap_proportions : ndarray
@@ -418,15 +419,15 @@
 @numba.njit(fastmath=True)
 def clip_trapped_charge(
     trapped_charge: np.ndarray,
     pixel: np.ndarray,
     available_traps: np.ndarray,
     pixel_diff: np.ndarray,
     trap_capacities: Optional[np.ndarray] = None,
-) -> Tuple[np.ndarray, np.ndarray]:
+) -> tuple[np.ndarray, np.ndarray]:
     """Clip trapped charge between arrays of max and min value.
 
     Parameters
     ----------
     trapped_charge : ndarray
     pixel : ndarray
     available_traps : ndarray
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/__init__.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/apd_gain.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/apd_gain.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,14 @@
 #  Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022.
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
-#
-#
-#
-#  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
-#  is part of this Pyxel package. No part of the package, including
-#  this file, may be copied, modified, propagated, or distributed except according to
-#  the terms contained in the file ‘LICENCE.txt’.
-#
-#
-#
-#  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
-#  is part of this Pyxel package. No part of the package, including
-#  this file, may be copied, modified, propagated, or distributed except according to
-#  the terms contained in the file ‘LICENCE.txt’.
-#
-#
+
 """Avalanche gain model."""
 from pyxel.detectors import APD
 
 
 def apd_gain(detector: APD) -> None:
     """Apply APD gain.
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/charge_deposition.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/charge_deposition.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 #   This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #   is part of this Pyxel package. No part of the package, including
 #   this file, may be copied, modified, propagated, or distributed except according to
 #   the terms contained in the file ‘LICENCE.txt’.
 
 """Simple models to simulate charge deposition by ionizing particles (e.g. cosmic rays)."""
 
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Literal, Optional, Sequence, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from pyxel.data_structure import Charge
 from pyxel.detectors import Detector
 from pyxel.util import materials, set_random_seed
@@ -21,20 +22,18 @@
 def charge_deposition(
     detector: Detector,
     flux: float,
     step_size: float = 1.0,
     energy_mean: float = 1.0,
     energy_spread: float = 0.1,
     energy_spectrum: Union[str, Path, None] = None,
-    energy_spectrum_sampling: Optional[Literal["linear", "log", None]] = "log",
+    energy_spectrum_sampling: Literal["linear", "log"] = "log",
     ehpair_creation: float = 3.65,
     material_density: float = 2.3290,
-    particle_direction: Optional[
-        Literal["isotropic", "orthogonal", None]
-    ] = "isotropic",
+    particle_direction: Literal["isotropic", "orthogonal"] = "isotropic",
     stopping_power_curve: Union[str, Path, None] = None,
     seed: Optional[int] = None,
 ) -> None:
     """Simulate charge deposition by ionizing particles using a stopping power curve.
 
     Parameters
     ----------
@@ -97,19 +96,17 @@
 def charge_deposition_in_mct(
     detector: Detector,
     flux: float,
     step_size: float = 1.0,
     energy_mean: float = 1.0,
     energy_spread: float = 0.1,
     energy_spectrum: Union[str, Path, None] = None,
-    energy_spectrum_sampling: Optional[Literal["linear", "log", None]] = "log",
+    energy_spectrum_sampling: Literal["linear", "log"] = "log",
     cutoff_wavelength: float = 2.5,
-    particle_direction: Optional[
-        Literal["isotropic", "orthogonal", None]
-    ] = "isotropic",
+    particle_direction: Literal["isotropic", "orthogonal"] = "isotropic",
     stopping_power_curve: Union[str, Path, None] = None,
     seed: Optional[int] = None,
 ) -> None:
     """Simulate charge deposition by ionizing particles using a stopping power curve.
 
     Parameters
     ----------
@@ -125,21 +122,21 @@
         the spread in energy of the incoming ionizing particles in MeV
     energy_spectrum : str
         the location of the file describing the energy spectrum of incident particles
         if no spectrum is provided energies are randomly drawn from a normal distribution
         with mean and spread defined above
         note that the energy spectrum is assumed to be a txt file with two columns [energy, flux]
         with the energy in MeV
-    energy_spectrum_sampling : str
-        "log" or None: the energy spectrum is sampled in log space
+    energy_spectrum_sampling : str. Default: 'log'
+        "log" : the energy spectrum is sampled in log space
         "linear" : the energy spectrum is sampled in linear space
     cutoff_wavelength : float
         the longest wavelength in micrometer at which the QE reaches 50% of its maximum,
         used to compute the bandgap energy, and the corresponding fraction of cadmium
-    particle_direction : str
+    particle_direction : str. Default: 'isotropic'
         "isotropic" : particles are coming from all directions (outside of the sensor)
         "orthogonal" : particles are coming from the top of the sensor (thickness = 0) and orthogonal to its surface
     stopping_power_curve : str
         the location of the file describing the total massive stopping power
         energetic loss per mass of material and per unit path length versus particle energy
         note that the the stopping power curve is assumed to be a csv file with two columns [energy, stopping power]
         energy in MeV, stopping power in MeV cm2/g
@@ -209,18 +206,18 @@
     x_lim: float,
     y_lim: float,
     z_lim: float,
     step_size: float = 1.0,
     energy_mean: float = 1.0,
     energy_spread: float = 0.1,
     energy_spectrum: Union[str, Path, None] = None,
-    energy_spectrum_sampling: Optional[Literal["linear", "log"]] = "log",
+    energy_spectrum_sampling: Literal["linear", "log"] = "log",
     ehpair_creation: float = 3.65,
     material_density: float = 2.3290,
-    particle_direction: Optional[Literal["isotropic", "orthogonal"]] = "isotropic",
+    particle_direction: Literal["isotropic", "orthogonal"] = "isotropic",
     stopping_power_curve: Union[str, Path, None] = None,
 ) -> list:
     """Simulate charge deposition of incident ionizing particles inside a detector.
 
     Parameters
     ----------
     flux : float
@@ -241,16 +238,16 @@
         the spread in energy of the incoming ionizing particles
     energy_spectrum : str
         the location of the file describing the energy spectrum of incident particles
         if no spectrum is provided energies are randomly drawn from a normal distribution
         with mean and spread defined above
         note that the energy spectrum is assumed to be a txt file with two columns [energy, flux]
         with the energy in MeV
-    energy_spectrum_sampling : str
-        "log" or None: the energy spectrum is sampled in log space
+    energy_spectrum_sampling : str. Default: 'log'
+        "log" : the energy spectrum is sampled in log space
         "linear" : the energy spectrum is sampled in linear space
     ehpair_creation : float
         the energy required to generate a electron-hole pair in eV
         by default the Si value at room temperature is parsed i.e. 3.65 eV
     material_density : float
         the material density in g/cm3
         by default he Si value at room temperature is parsed i.e. 2.3290 g/cm3
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/charge_injection.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/charge_injection.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel charge injection functions for CCDs."""
 
-from typing import Optional, Tuple
+from typing import Optional
 
 import numpy as np
 
 from pyxel.detectors import CCD
 
 
 def compute_charge_blocks(
-    output_shape: Tuple[int, int],
+    output_shape: tuple[int, int],
     charge_level: float,
     block_start: int = 0,
     block_end: Optional[int] = None,
 ) -> np.ndarray:
     """Compute a block of charges to be injected in the detector.
 
     Parameters
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/cosmix.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/cosmix.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel CosmiX model to generate charge by ionization."""
 
 import logging
 import math
-
-# noqa: F401
 from pathlib import Path
-from typing import Literal, Optional, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 from tqdm.auto import tqdm
 
 from pyxel.detectors import Detector
 from pyxel.models.charge_generation.cosmix.plotting import PlottingCosmix
@@ -37,16 +35,16 @@
     ] = None,
     running_mode: Optional[
         Literal["stopping", "stepsize", "geant4", "plotting"]
     ] = None,
     particle_type: Optional[Literal["proton", "alpha", "ion"]] = None,
     initial_energy: Optional[Union[int, float, Literal["random"]]] = None,
     particles_per_second: Optional[float] = None,
-    incident_angles: Optional[Tuple[str, str]] = None,
-    starting_position: Optional[Tuple[str, str, str]] = None,
+    incident_angles: Optional[tuple[str, str]] = None,
+    starting_position: Optional[tuple[str, str, str]] = None,
     # step_size_file: str = None,
     # stopping_file: str = None,
     spectrum_file: Optional[str] = None,
     seed: Optional[int] = None,
     ionization_energy: float = 3.6,
     progressbar: bool = True,
 ) -> None:
@@ -210,21 +208,21 @@
         self.init_energy = energy
 
     # TODO: Is it still used ?
     def set_particle_number(self, number: int) -> None:
         self.particle_number = number
 
     # TODO: Is it still used ?
-    def set_incident_angles(self, angles: Tuple[str, str]) -> None:
+    def set_incident_angles(self, angles: tuple[str, str]) -> None:
         alpha, beta = angles
         self.angle_alpha = alpha
         self.angle_beta = beta
 
     # TODO: Is it still used ?
-    def set_starting_position(self, start_position: Tuple[str, str, str]) -> None:
+    def set_starting_position(self, start_position: tuple[str, str, str]) -> None:
         position_vertical, position_horizontal, position_z = start_position
         self.position_ver = position_vertical
         self.position_hor = position_horizontal
         self.position_z = position_z
 
     def set_particle_spectrum(self, file_name: Path) -> None:
         """Set up the particle specs according to a spectrum.
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii` & `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_100um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii` & `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_40um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii` & `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_50um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii` & `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_60um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii` & `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/data/inputs/stepsize_proton_100MeV_70um_Si_10k.ascii`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/particle.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/particle.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel CosmiX model to generate charge by ionization."""
 
-from typing import List, Literal, Optional, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 
 from pyxel.detectors import Detector
 from pyxel.models.charge_generation.cosmix.util import sampling_distribution
 
 
@@ -155,28 +155,28 @@
 
         else:
             raise ValueError("Given particle type can not be simulated")
 
     def get_surface_point(self) -> np.ndarray:
         geo = self.detector.geometry
 
-        norm_vectors: List[np.ndarray] = [
+        norm_vectors: list[np.ndarray] = [
             np.array(
                 [0.0, 0.0, -1.0]
             ),  # top plane (usually particle enters vol. via this)
             np.array(
                 [0.0, 0.0, 1.0]
             ),  # bottom plane (usually particle leaves vol. via this)
             np.array([0.0, 1.0, 0.0]),
             np.array([-1.0, 0.0, 0.0]),
             np.array([0.0, -1.0, 0.0]),
             np.array([1.0, 0.0, 0.0]),
         ]
 
-        points: List[np.ndarray] = [
+        points: list[np.ndarray] = [
             np.array(
                 [0.0, 0.0, 0.0]
             ),  # top plane (usually particle enters vol. via this)
             np.array(
                 [0.0, 0.0, -1 * geo.total_thickness]
             ),  # bottom plane (usually particle leaves vol. via this)
             np.array([0.0, 0.0, 0.0]),
@@ -236,15 +236,15 @@
         if surface_start_point is None:
             raise ValueError("This should not happen")
         if surface_end_point is None:
             raise ValueError("This should not happen")
 
         return surface_start_point
 
-    def get_angles(self) -> Tuple[float, float]:
+    def get_angles(self) -> tuple[float, float]:
         beta = np.arccos(
             np.dot(np.array([1.0, 0.0]), np.array([self.dir_ver, self.dir_hor]))
         )
 
         alpha = np.arccos(
             np.dot(
                 np.array([0.0, 0.0, 1.0]),
@@ -329,23 +329,23 @@
         return None
     else:
         d = np.dot((p0 - ls), n) / np.dot(lv, n)
         p: np.ndarray = d * lv + ls
         return p
 
 
-def isotropic_direction() -> Tuple[float, float, float]:
+def isotropic_direction() -> tuple[float, float, float]:
     u = 2 * np.random.random() - 1
     r = np.sqrt(1 - u**2)
     kszi = np.random.random()
     v = r * np.cos(2 * np.pi * kszi)
     w = r * np.sin(2 * np.pi * kszi)
     return u, v, w
 
 
-def non_isotropic_direction(n: int) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+def non_isotropic_direction(n: int) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
     alpha = 2 * np.pi * np.random.random(n)
     beta = 2 * np.pi * np.random.random(n)
     x = np.cos(alpha) * np.sin(beta)
     y = np.cos(alpha) * np.cos(beta)
     z = np.sin(alpha)
     return x, y, z
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/plotting.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel CosmiX model to generate charge by ionization."""
 
 from contextlib import suppress
 from pathlib import Path
-from typing import TYPE_CHECKING, Optional, Tuple, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 with suppress(ImportError):
     from matplotlib import pyplot as plt
 
@@ -578,15 +578,15 @@
     def plot_electron_hist(
         self,
         data1: Union[str, np.ndarray],
         data2: Optional[np.ndarray] = None,
         data3: Optional[np.ndarray] = None,
         title: str = "",
         hist_bins: int = 500,
-        hist_range: Tuple[int, int] = (0, 15000),
+        hist_range: tuple[int, int] = (0, 15000),
         normalize: bool = False,
     ) -> None:
         labels = [
             "TARS (David), 40um"
             # 'secondary e-',
             # 'tertiary e-'
         ]
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/simulation.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel CosmiX model to generate charge by ionization."""
 
 import subprocess
 from bisect import bisect
+from collections.abc import Sequence
 from pathlib import Path
-from typing import List, Literal, Optional, Sequence, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 import pandas as pd
 
 from pyxel.detectors import Detector
 from pyxel.models.charge_generation.cosmix.particle import Particle
 from pyxel.models.charge_generation.cosmix.util import (
@@ -71,36 +72,36 @@
         self.angle_beta: Optional[str] = None
         self.step_length = (
             1.0  # fix, all the other data/parameters should be adjusted to this
         )
         self.energy_cut = 1.0e-5  # MeV
         self.ionization_energy = 3.6
 
-        self.e_num_lst_per_step: List[int] = []
-        self.e_energy_lst: List[float] = []
-        self.e_pos0_lst: List[float] = []
-        self.e_pos1_lst: List[float] = []
-        self.e_pos2_lst: List[float] = []
+        self.e_num_lst_per_step: list[int] = []
+        self.e_energy_lst: list[float] = []
+        self.e_pos0_lst: list[float] = []
+        self.e_pos1_lst: list[float] = []
+        self.e_pos2_lst: list[float] = []
         self.e_vel0_lst: np.ndarray = np.array([])
         self.e_vel1_lst: np.ndarray = np.array([])
         self.e_vel2_lst: np.ndarray = np.array([])
 
-        self.electron_number_from_eloss: List[int] = []
-        self.secondaries_from_eloss: List[int] = []
-        self.tertiaries_from_eloss: List[int] = []
-
-        self.track_length_lst_per_event: List[float] = []
-        self.e_num_lst_per_event: List[int] = []
-        self.sec_lst_per_event: List[int] = []
-        self.ter_lst_per_event: List[int] = []
-        self.edep_per_step: List[float] = []
-        self.total_edep_per_particle: List[float] = []
-        self.p_energy_lst_per_event: List[float] = []
-        self.alpha_lst_per_event: List[float] = []
-        self.beta_lst_per_event: List[float] = []
+        self.electron_number_from_eloss: list[int] = []
+        self.secondaries_from_eloss: list[int] = []
+        self.tertiaries_from_eloss: list[int] = []
+
+        self.track_length_lst_per_event: list[float] = []
+        self.e_num_lst_per_event: list[int] = []
+        self.sec_lst_per_event: list[int] = []
+        self.ter_lst_per_event: list[int] = []
+        self.edep_per_step: list[float] = []
+        self.total_edep_per_particle: list[float] = []
+        self.p_energy_lst_per_event: list[float] = []
+        self.alpha_lst_per_event: list[float] = []
+        self.beta_lst_per_event: list[float] = []
 
     def parameters(
         self,
         sim_mode: Literal["cosmic_ray", "cosmics", "radioactive_decay", "snowflakes"],
         part_type: Literal[
             "proton", "ion", "alpha", "beta", "electron", "gamma", "x-ray"
         ],
@@ -412,18 +413,18 @@
             "data", "geant4", "tars_geant4.data"
         )
         g4data = read_data(g4_data_path)  # mm (!)
 
         if g4data.shape == (
             3,
         ):  # alternative running mode, only all electron number without proton step size data
-            electron_number_vector: Union[List, np.ndarray] = [g4data[0].astype(int)]
+            electron_number_vector: Union[list, np.ndarray] = [g4data[0].astype(int)]
             secondaries = g4data[1].astype(int)
             tertiaries = g4data[2].astype(int)
-            step_size_vector: Union[List, np.ndarray] = [0]
+            step_size_vector: Union[list, np.ndarray] = [0]
         elif g4data.shape == (0,):
             step_size_vector = []  # um
             electron_number_vector = []
         elif g4data.shape == (2,):
             step_size_vector = [g4data[0] * 1e3]  # um
             electron_number_vector = [g4data[1].astype(int)]
         else:
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/cosmix/util.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/cosmix/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/dark_current.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/dark_current.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #   This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #   is part of this Pyxel package. No part of the package, including
 #   this file, may be copied, modified, propagated, or distributed except according to
 #   the terms contained in the file ‘LICENCE.txt’.
 
 """Models to generate charge due to dark current process."""
 import warnings
-from typing import Optional, Tuple
+from typing import Optional
 
 import numpy as np
 from astropy import constants as const
 
 from pyxel.detectors import APD, Detector
 from pyxel.util import set_random_seed
 
@@ -113,15 +113,15 @@
         * (1 / room_temperature_factor)
     )  # Unit: e-/s/pixel
 
     return avg_dark_current
 
 
 def compute_dark_current(
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     time_step: float,
     temperature: float,
     pixel_area: float,
     figure_of_merit: float,
     band_gap: float,
     band_gap_room_temperature: float,
     spatial_noise_factor: Optional[float] = None,
@@ -189,14 +189,15 @@
         )
 
     if np.isinf(dark_current_2d).any():
         warnings.warn(
             "Unphysical high value for dark current from fixed pattern noise distribution"
             " will result in inf values. Enable a FWC model to ensure a physical limit.",
             RuntimeWarning,
+            stacklevel=2,
         )
 
     return dark_current_2d
 
 
 def dark_current(
     detector: Detector,
@@ -321,15 +322,15 @@
 
     detector.charge.add_charge_array(dark_current_array)
 
 
 def calculate_dark_current_saphira(
     temperature: float,
     avalanche_gain: float,
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     exposure_time: float,
 ) -> np.ndarray:
     """Simulate dark current in a Saphira :term:`APD`.
 
     From: I. M. Baker et al., Linear-mode avalanche photodiode arrays in HgCdTe at Leonardo, UK: the
     current status, in Image Sensing Technologies: Materials, Devices, Systems, and Applications VI,
     2019, vol. 10980, no. May, p. 20.
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/dark_current_rule07.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/dark_current_rule07.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Simple models to generate charge due to dark current process."""
 import warnings
-from typing import Optional, Tuple
+from typing import Optional
 
 import numpy as np
 
 from pyxel.detectors import CMOS
 from pyxel.util import set_random_seed
 
 
@@ -79,15 +79,15 @@
     factor = amp_to_eps * pitch * pitch * um2_to_cm2  # to convert Amp/cm2 in e/pixel/s
     avg_dark_current_rule07 = rule07 * factor
 
     return avg_dark_current_rule07
 
 
 def compute_mct_dark_rule07(
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     pitch: float,
     time_step: float,
     temperature: float,
     cut_off: float,
     spatial_noise_factor: Optional[float] = None,
     temporal_noise: bool = True,
 ) -> np.ndarray:
@@ -143,14 +143,15 @@
         )
 
     if np.isinf(dark_current_2d_rule07).any():
         warnings.warn(
             "Unphysical high value for dark current from fixed pattern noise distribution"
             " will result in inf values. Enable a FWC model to ensure a physical limit.",
             RuntimeWarning,
+            stacklevel=2,
         )
 
     return dark_current_2d_rule07
 
 
 def dark_current_rule07(
     detector: CMOS,
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/data/mct-stopping-power.csv` & `pyxel_sim-1.9/pyxel/models/charge_generation/data/mct-stopping-power.csv`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt` & `pyxel_sim-1.9/pyxel/models/charge_generation/data/proton_L2_solarMax_11mm_Shielding.txt`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt` & `pyxel_sim-1.9/pyxel/models/charge_generation/data/proton_L2_solarMax_NoShielding.txt`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv` & `pyxel_sim-1.9/pyxel/models/charge_generation/data/protons-in-silicon_stopping-power.csv`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/load_charge.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/load_charge.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,26 +4,26 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Simple model to load charge profiles."""
 
 from pathlib import Path
-from typing import Literal, Optional, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 
 from pyxel.detectors import Detector, Geometry
 from pyxel.util import load_cropped_and_aligned_image
 
 
 def load_charge(
     detector: Detector,
     filename: Union[str, Path],
-    position: Tuple[int, int] = (0, 0),
+    position: tuple[int, int] = (0, 0),
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ] = None,
     time_scale: float = 1.0,
 ) -> None:
     """Load charge from txt file for detector, mostly for but not limited to :term:`CCDs<CCD>`.
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_generation/photoelectrons.py` & `pyxel_sim-1.9/pyxel/models/charge_generation/photoelectrons.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Simple model to convert photon into photo-electrons inside detector."""
 
 from pathlib import Path
-from typing import Literal, Optional, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 
 from pyxel.detectors import Detector
 from pyxel.util import load_cropped_and_aligned_image, set_random_seed
 
 
@@ -74,15 +74,15 @@
         )
     detector.charge.add_charge_array(detector_charge)
 
 
 def conversion_with_qe_map(
     detector: Detector,
     filename: Union[str, Path],
-    position: Tuple[int, int] = (0, 0),
+    position: tuple[int, int] = (0, 0),
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ] = None,
     seed: Optional[int] = None,
     binomial_sampling: bool = True,
 ) -> None:
     """Generate charge from incident photon via photoelectric effect, simple model with custom :term:`QE` map.
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_measurement/__init__.py` & `pyxel_sim-1.9/pyxel/models/charge_measurement/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_measurement/linearity.py` & `pyxel_sim-1.9/pyxel/models/charge_measurement/linearity.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Linearity models."""
 
-from typing import Sequence
+from collections.abc import Sequence
 
 import numpy as np
 from astropy import constants as const
 
 from pyxel.detectors import CMOS, Detector
 from pyxel.models.charge_measurement.non_linearity_calculation import (
     euler,
@@ -115,23 +115,25 @@
     # Here we are considering the case where the detector is operated at its nominal temperature,
     # it might not be always the case
     # cutoff = 2.1
     e_g_targeted = 1.24 / cutoff  # cutoff is um and Eg in eV
     xcd = np.linspace(0.2, 0.6, 1000)
     targeted_operating_temperature = temperature
     e_g_calculated = hgcdte_bandgap(
-        xcd, targeted_operating_temperature
+        x_cd=xcd,
+        temperature=targeted_operating_temperature,
     )  # Expected bandgap
+
     index = np.where(e_g_calculated > e_g_targeted)[0][0]
     x_cd = xcd[index]  # Targeted cadmium concentration in the HgCdTe alloy
 
     if not (0.2 <= x_cd <= 0.6):
         raise ValueError(
-            "Hansen bangap expression used out of its nominal application range. \
-                x_cd must be between 0.2 and 0.6"
+            "Hansen bangap expression used out of its nominal application range. "
+            "x_cd must be between 0.2 and 0.6"
         )
 
     ni = ni_hansen(x_cd=x_cd, temperature=temperature)
 
     # Build in potential
     vbi = (
         const.k_B.value
@@ -189,16 +191,16 @@
         Diode diameter. Unit: um
     v_bias : float
         Initial bias voltage. Unit: V.
     """
 
     if not (4 <= detector.environment.temperature <= 300):
         raise ValueError(
-            "Hansen bangap expression used out of its nominal application range. \
-                temperature must be between 4K and 300K"
+            "Hansen bangap expression used out of its nominal application range. "
+            "temperature must be between 4K and 300K"
         )
 
     if not isinstance(detector, CMOS):
         raise TypeError("Expecting a 'CMOS' detector object.")
 
     signal_mean_array = detector.charge.array.astype("float64")
     signal_non_linear = compute_simple_physical_non_linearity(
@@ -260,16 +262,16 @@
         xcd, targeted_operating_temperature
     )  # Expected band-gap
     index = np.where(e_g_calculated > e_g_targeted)[0][0]
     x_cd = xcd[index]  # Targeted cadmium concentration in the HgCdTe alloy
 
     if not (0.2 <= x_cd <= 0.6):
         raise ValueError(
-            "Hansen bangap expression used out of its nominal application range. \
-                x_cd must be between 0.2 and 0.6"
+            "Hansen bangap expression used out of its nominal application range. "
+            "x_cd must be between 0.2 and 0.6"
         )
 
     # Calculate the effective band-gap value at the temperature at which simulations are performed.
     ni = ni_hansen(x_cd=x_cd, temperature=temperature)
 
     # Build in potential
     vbi = (
@@ -338,16 +340,16 @@
     v_bias : float
         Initial bias voltage. Unit: V.
     fixed_capacitance : float
         Additional fixed capacitance. Unit: F
     """
     if not (4 <= detector.environment.temperature <= 300):
         raise ValueError(
-            "Hansen bangap expression used out of its nominal application range. \
-                temperature must be between 4K and 300K"
+            "Hansen bangap expression used out of its nominal application range. "
+            "temperature must be between 4K and 300K"
         )
 
     if not isinstance(detector, CMOS):
         raise TypeError("Expecting a 'CMOS' detector object.")
 
     signal_mean_array = detector.pixel.array.astype("float64")
     signal_non_linear = compute_physical_non_linearity(
@@ -364,14 +366,15 @@
     detector.signal.array = signal_non_linear
 
 
 def compute_physical_non_linearity_with_saturation(
     signal_array_2d: np.ndarray,
     photon_array_2d: np.ndarray,
     time_step: float,
+    step_number: int,
     temperature: float,
     cutoff: float,
     n_donor: float,
     n_acceptor: float,
     phi_implant: float,
     d_implant: float,
     saturation_current: float,
@@ -387,14 +390,16 @@
     ----------
     signal_array_2d : ndarray
         Input signal array.
     photon_array_2d : ndarray
         Input photon array.
     time_step
         Time step. Unit: s.
+    step_number : int
+        Step number.
     temperature : float
         Temperature. Unit: K.
     cutoff : float
         Cutoff wavelength. unit: um.
     n_donor : float
         Donor density. Unit: atoms/cm^3.
     n_acceptor : float
@@ -430,24 +435,24 @@
     e_g_calculated = hgcdte_bandgap(xcd, temperature)  # Expected bandgap
     index = np.where(e_g_calculated > e_g_targeted)[0][0]
     x_cd = xcd[index]  # Targeted cadmium concentration in the HgCdTe alloy
     # Calculate the effective bandgap value at the temperature at which simulations are performed.
 
     if not (0.2 <= x_cd <= 0.6):
         raise ValueError(
-            "Hansen bangap expression used out of its nominal application range. \
-                x_cd must be between 0.2 and 0.6"
+            "Hansen bangap expression used out of its nominal application range. "
+            "x_cd must be between 0.2 and 0.6"
         )
 
     row, col = signal_array_2d.shape
 
     phi_implant = phi_implant * 1e-6  # in m
     d_implant = d_implant * 1e-6  # in m
 
-    if signal_array_2d[3, 3] == 0:
+    if step_number == 0:
         signal_array_2d = v_reset * np.ones((row, col))
 
     # detector.signal.array should be expressed in unit of mV. It is the bias at the gate of the pixel SFD ????
     det_polar = euler(
         time_step=time_step,
         nb_pts=euler_points,
         v_bias=np.ravel(signal_array_2d) - d_sub,
@@ -510,33 +515,47 @@
     fixed_capacitance : float
         Additional fixed capacitance. Unit: F.
     euler_points : int
         Number of points in the euler method.
     """
     if not (4 <= detector.environment.temperature <= 300):
         raise ValueError(
-            "Hansen bangap expression used out of its nominal application range. \
-                temperature must be between 4K and 300K"
+            "Hansen bangap expression used out of its nominal application range. "
+            "temperature must be between 4K and 300K"
         )
 
     if not isinstance(detector, CMOS):
         raise TypeError("Expecting a 'CMOS' detector object.")
 
+    if detector.is_first_readout:
+        # This is the first step
+        signal_2d = detector.signal.array
+    else:
+        signal_2d = np.array(detector.data["/non_linearity_with_saturation/previous"])
+
+        if detector.is_last_readout:
+            # This is the last step. Remove the previous value
+            detector.data["/non_linearity_with_saturation"].orphan()
+
     signal_non_linear = compute_physical_non_linearity_with_saturation(
-        signal_array_2d=detector.signal.array,
+        signal_array_2d=signal_2d,
         photon_array_2d=detector.photon.array,
         time_step=detector.time_step,
+        step_number=detector.pipeline_count,
         temperature=detector.environment.temperature,
         cutoff=cutoff,
         n_donor=n_donor,
         n_acceptor=n_acceptor,
         phi_implant=phi_implant,
         d_implant=d_implant,
         saturation_current=saturation_current,
         ideality_factor=ideality_factor,
         v_reset=v_reset,
         d_sub=d_sub,
         fixed_capacitance=fixed_capacitance,
         euler_points=euler_points,
     )
 
+    # Update previous value
+    detector.data["/non_linearity_with_saturation/previous"] = signal_non_linear
+
     detector.signal.array = signal_non_linear
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_measurement/measurement.py` & `pyxel_sim-1.9/pyxel/models/charge_measurement/measurement.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_measurement/nghxrg/nghxrg.py` & `pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/nghxrg.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel wrapper class for NGHXRG - Teledyne HxRG Noise Generator model."""
 
 import logging
+from collections.abc import Mapping, Sequence
 from dataclasses import dataclass
-from typing import List, Literal, Mapping, Optional, Sequence, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 
 from pyxel.detectors import CMOS, CMOSGeometry
 from pyxel.models.charge_measurement.nghxrg.nghxrg_beta import HXRGNoise
 from pyxel.util import set_random_seed
 
@@ -75,17 +76,17 @@
 
 
 # TODO: Use function `simcado.nghxrg.HXRGNoise` instead of
 #       `pyxel.models.charge_measurement.nghxrg.nghxrg.HXRGNoise`
 def compute_nghxrg(
     pixel_2d: np.ndarray,
     noise: Sequence[NoiseType],
-    detector_shape: Tuple[int, int],
-    window_pos: Tuple[int, int],
-    window_size: Tuple[int, int],
+    detector_shape: tuple[int, int],
+    window_pos: tuple[int, int],
+    window_size: tuple[int, int],
     num_outputs: int,
     time_step: int,
     num_rows_overhead: int,
     num_frames_overhead: int,
     reverse_scan_direction: bool,
     reference_pixel_border_width: int,
 ) -> np.ndarray:
@@ -197,16 +198,16 @@
                 "uncorr_pink_noise",
                 "acn_noise",
                 "pca_zero_noise",
             ],
             Mapping[str, float],
         ]
     ],
-    window_position: Optional[Tuple[int, int]] = None,
-    window_size: Optional[Tuple[int, int]] = None,
+    window_position: Optional[tuple[int, int]] = None,
+    window_size: Optional[tuple[int, int]] = None,
     n_output: int = 1,
     n_row_overhead: int = 0,
     n_frame_overhead: int = 0,
     reverse_scan_direction: bool = False,
     reference_pixel_border_width: int = 4,
     seed: Optional[int] = None,
 ) -> None:
@@ -247,15 +248,15 @@
     if n_frame_overhead not in range(101):
         raise ValueError("'n_frame_overhead' must be between 0 and 100.")
 
     if reference_pixel_border_width not in range(33):
         raise ValueError("'reference_pixel_border_width' must be between 0 and 32.")
 
     # Converter
-    params: List[NoiseType] = []
+    params: list[NoiseType] = []
     for item in noise:
         if "ktc_bias_noise" in item:
             sub_item: Mapping[str, float] = item["ktc_bias_noise"]
             param: NoiseType = KTCBiasNoise(
                 ktc_noise=sub_item["ktc_noise"],
                 bias_offset=sub_item["bias_offset"],
                 bias_amp=sub_item["bias_amp"],
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py` & `pyxel_sim-1.9/pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py`

 * *Files 0% similar despite different names*

```diff
@@ -598,27 +598,27 @@
             w = self.ref_all
             r = reference_pixel_noise_ratio  # Easier to work with
             for z in np.arange(self.naxis3):
                 here = np.zeros((self.naxis2, self.naxis1))
 
                 # Noisy reference pixel for each side of detector
                 if w[0] > 0:  # lower
-                    here[: w[0], :] = (  # noqa: E203
+                    here[: w[0], :] = (
                         r * rd_noise * np.random.standard_normal((w[0], self.naxis1))
                     )
                 if w[1] > 0:  # upper
-                    here[-w[1] :, :] = (  # noqa: E203
+                    here[-w[1] :, :] = (
                         r * rd_noise * np.random.standard_normal((w[1], self.naxis1))
                     )
                 if w[2] > 0:  # left
                     here[:, : w[2]] = (
                         r * rd_noise * np.random.standard_normal((self.naxis2, w[2]))
                     )
                 if w[3] > 0:  # right
-                    here[:, -w[3] :] = (  # noqa: E203
+                    here[:, -w[3] :] = (
                         r * rd_noise * np.random.standard_normal((self.naxis2, w[3]))
                     )
 
                 # Noisy regular pixel
                 if np.sum(w) > 0:  # Ref. pixel exist in frame
                     start_y_idx = w[0]
                     end_y_idx = self.naxis2 - w[1]
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_measurement/non_linearity_calculation.py` & `pyxel_sim-1.9/pyxel/models/charge_measurement/non_linearity_calculation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_measurement/offset.py` & `pyxel_sim-1.9/pyxel/models/charge_measurement/offset.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 #
 #
 """Voltage offset models."""
 
-from typing import Tuple
-
 import numpy as np
 
 from pyxel.detectors import APD, Detector
 
 
-def compute_dc_offset(offset: float, shape: Tuple[int, int]) -> np.ndarray:
+def compute_dc_offset(offset: float, shape: tuple[int, int]) -> np.ndarray:
     """Compute DC offset voltage array.
 
     Parameters
     ----------
     offset : float
         DC voltage offset. Unit: V
     shape : tuple
@@ -53,15 +51,15 @@
     detector.signal.array += compute_dc_offset(offset, detector.geometry.shape)
 
 
 def compute_output_pixel_reset_voltage_apd(
     roic_drop: float,
     roic_gain: float,
     pixel_reset_voltage: float,
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
 ) -> np.ndarray:
     """Compute output pixel reset voltage.
 
     Parameters
     ----------
     roic_drop : float
         Readout circuit drop voltage. Unit: V
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_measurement/readout_noise.py` & `pyxel_sim-1.9/pyxel/models/charge_measurement/readout_noise.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Readout noise model."""
 
-from typing import Optional, Tuple
+from typing import Optional
 
 import numpy as np
 
 from pyxel.detectors import APD, CMOS, Detector
 from pyxel.util import set_random_seed
 
 
@@ -138,15 +138,15 @@
 
     detector.signal.array = noise_2d
 
 
 def compute_readout_noise_saphira(
     roic_readout_noise: float,
     avalanche_gain: float,
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     controller_noise: float = 0.0,
 ) -> np.ndarray:
     """Compute Saphira specific readout noise.
 
     Parameters
     ----------
     roic_readout_noise : float
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_measurement/reset_noise.py` & `pyxel_sim-1.9/pyxel/models/charge_measurement/reset_noise.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,25 +4,25 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 #
 #
 """Reset noise models."""
 
-from typing import Optional, Tuple
+from typing import Optional
 
 import astropy.constants as const
 import numpy as np
 
 from pyxel.detectors import Detector
 from pyxel.util import set_random_seed
 
 
 def compute_ktc_noise(
-    temperature: float, capacitance: float, shape: Tuple[int, int]
+    temperature: float, capacitance: float, shape: tuple[int, int]
 ) -> np.ndarray:
     """Compute KTC noise array.
 
     Parameters
     ----------
     temperature : float
         Temperature. Unit: K
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_transfer/EMCCD_poisson.py` & `pyxel_sim-1.9/pyxel/models/charge_transfer/EMCCD_poisson.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py` & `pyxel_sim-1.9/pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 
+from collections.abc import Sequence
 from dataclasses import dataclass
-from typing import Sequence
 
 import numpy as np
 
 from pyxel.detectors import CCD
 
 try:
     import arcticpy as ac
```

### Comparing `pyxel_sim-1.8/pyxel/models/charge_transfer/cdm.py` & `pyxel_sim-1.9/pyxel/models/charge_transfer/cdm.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,17 @@
 Nr - number of electrons released into the sample during a transit along the column
 vg: assumed maximum geometrical volume electrons can occupy within a pixel (parallel)
 svg: assumed maximum geometrical volume electrons can occupy within a pixel (serial)
 t: constant TDI period (parallel)
 st: constant TDI period (serial)
 """
 
+from collections.abc import Sequence
 from enum import Enum
-from typing import Literal, Optional, Sequence
+from typing import Literal, Optional
 
 import astropy.constants as const
 import numba
 import numpy as np
 
 from pyxel.detectors import CCD
```

### Comparing `pyxel_sim-1.8/pyxel/models/data_processing/__init__.py` & `pyxel_sim-1.9/pyxel/models/data_processing/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,9 +4,11 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Subpackage with all models related to the 'DataProcessing' model group."""
 
 # flake8: noqa
-from .statistics import compute_statistics
+from .statistics import statistics
 from .source_extractor import extract_roi_to_xarray
+from .mean_variance import mean_variance
+from .linear_regression import linear_regression
```

### Comparing `pyxel_sim-1.8/pyxel/models/data_processing/source_extractor.py` & `pyxel_sim-1.9/pyxel/models/data_processing/source_extractor.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/data_processing/statistics.py` & `pyxel_sim-1.9/pyxel/models/readout_electronics/sar_adc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,54 +1,85 @@
 #  Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022.
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
-"""Simple model to compute basic statistics."""
-from typing import Literal, Sequence, Union
-
-import xarray as xr
+""":term:`SAR` :term:`ADC` model."""
+import numpy as np
 
 from pyxel.detectors import Detector
 
 
-def compute_statistics(
+def apply_sar_adc(
+    signal_2d: np.ndarray,
+    num_rows: int,
+    num_cols: int,
+    min_volt: float,
+    max_volt: float,
+    adc_bits: int,
+) -> np.ndarray:
+    """Apply :term:`SAR` :term:`ADC`.
+
+    Parameters
+    ----------
+    signal_2d : ndarray
+    num_rows : int
+    num_cols : int
+    min_volt : float
+    max_volt : float
+    adc_bits : int
+
+    Returns
+    -------
+    ndarray
+    """
+    data_digitized_2d = np.zeros((num_rows, num_cols))
+
+    signal_normalized_2d = signal_2d.copy()
+
+    # Set the reference voltage of the ADC to half the max
+    ref: float = max_volt / 2.0
+
+    # For each bits, compare the value of the ref to the capacitance value
+    for i in np.arange(adc_bits):
+        # digital value associated with this step
+        digital_value = 2 ** (adc_bits - (i + 1))
+
+        # All data that is higher than the ref is equal to the dig. value
+        data_digitized_2d[signal_normalized_2d >= ref] += digital_value
+
+        # Subtract ref value from the data
+        signal_normalized_2d[signal_normalized_2d >= ref] -= ref
+
+        # Divide reference voltage by 2 for next step
+        ref /= 2.0
+
+    return data_digitized_2d
+
+
+# TODO: documentation, range volt - only max is used
+def sar_adc(
     detector: Detector,
-    data_structure: Literal["pixel", "photon", "image", "signal"] = "pixel",
-    dimensions: Union[str, Sequence[str]] = ("x", "y"),
 ) -> None:
-    """Compute basic statistics.
+    """Digitize signal array using :term:`SAR` (Successive Approximation Register) :term:`ADC` logic.
 
     Parameters
     ----------
     detector : Detector
         Pyxel Detector object.
-    data_structure : Literal
-        Keyword to choose data structure. Can be any from:
-        ("pixel", "photon", "image", "signal")
-    dimensions : str or Sequence of str
-        Dimensions.
     """
-    data_2d: xr.DataArray = getattr(detector, data_structure).to_xarray()
-    var = data_2d.var(dim=dimensions)
-    mean = data_2d.mean(dim=dimensions)
-    min_array = data_2d.min(dim=dimensions)
-    max_array = data_2d.max(dim=dimensions)
-    count = data_2d.count(dim=dimensions)
-
-    # Get current absolute time
-    absolute_time = xr.DataArray(
-        [detector.absolute_time],
-        dims=["time"],
-        attrs={"units": "s"},
-    )
 
-    dataset = xr.Dataset().assign_coords(time=absolute_time)
-    dataset["var"] = var
-    dataset["mean"] = mean
-    dataset["min"] = min_array
-    dataset["max"] = max_array
-    dataset["count"] = count
+    min_volt, max_volt = detector.characteristics.adc_voltage_range
+    adc_bits = detector.characteristics.adc_bit_resolution
+
+    image_2d: np.ndarray = apply_sar_adc(
+        signal_2d=detector.signal.array,
+        num_rows=detector.geometry.row,
+        num_cols=detector.geometry.col,
+        min_volt=min_volt,
+        max_volt=max_volt,
+        adc_bits=adc_bits,
+    )
 
-    detector.processed_data.append(dataset)
+    detector.image.array = image_2d
```

### Comparing `pyxel_sim-1.8/pyxel/models/optics/__init__.py` & `pyxel_sim-1.9/pyxel/models/optics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/optics/point_spread_function.py` & `pyxel_sim-1.9/pyxel/models/optics/point_spread_function.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/optics/poppy.py` & `pyxel_sim-1.9/pyxel/models/optics/poppy.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Poppy model."""
 
 import logging
+from collections.abc import Mapping, Sequence
 from dataclasses import dataclass
-from typing import Any, Mapping, Sequence, Tuple, Union
+from typing import Any, Union
 
 import numpy as np
 from astropy.convolution import convolve_fft
 from astropy.io import fits
 
 from pyxel.detectors import Detector
 from pyxel.util import deprecated
@@ -334,15 +335,15 @@
 
 
 def calc_psf(
     wavelength: float,
     fov_arcsec: float,
     pixelscale: float,
     optical_parameters: Sequence[OpticalParameter],
-) -> Tuple[Sequence[fits.hdu.image.PrimaryHDU], Sequence["op.Wavefront"]]:
+) -> tuple[Sequence[fits.hdu.image.PrimaryHDU], Sequence["op.Wavefront"]]:
     """Calculate the point spread function for the given optical system.
 
     Parameters
     ----------
     wavelength : float
         Wavelength of incoming light in meters.
     fov_arcsec : float, optional
```

### Comparing `pyxel_sim-1.8/pyxel/models/phasing/pulse_processing.py` & `pyxel_sim-1.9/pyxel/models/phasing/pulse_processing.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/photon_collection/__init__.py` & `pyxel_sim-1.9/pyxel/models/photon_collection/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/photon_collection/illumination.py` & `pyxel_sim-1.9/pyxel/models/photon_collection/illumination.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,24 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel photon generator models."""
 
-from typing import Literal, Optional, Sequence, Tuple
+from collections.abc import Sequence
+from typing import Literal, Optional
 
 import numpy as np
 
 from pyxel.detectors import Detector
 
 
 def rectangular(
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     level: float,
     object_size: Optional[Sequence[int]] = None,
     object_center: Optional[Sequence[int]] = None,
 ) -> np.ndarray:
     """Calculate an image of a rectangular object.
 
     Parameters
@@ -63,15 +64,15 @@
     q0 = int(np.clip(q, a_min=0, a_max=shape[1]))
     photon_array[slice(p0, p + object_size[0]), slice(q0, q + object_size[1])] = level
 
     return photon_array
 
 
 def elliptic(
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     level: float,
     object_size: Optional[Sequence[int]] = None,
     object_center: Optional[Sequence[int]] = None,
 ) -> np.ndarray:
     """Calculate an image of an elliptic object.
 
     Parameters
@@ -115,15 +116,15 @@
         + ((y - object_center[0]) / float(object_size[0] / 2)) ** 2
     )
     photon_array[dist_from_center < 1] = level
     return photon_array
 
 
 def calculate_illumination(
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     level: float,
     option: Literal["uniform", "rectangular", "elliptic"] = "uniform",
     object_size: Optional[Sequence[int]] = None,
     object_center: Optional[Sequence[int]] = None,
 ) -> np.ndarray:
     """Calculate the array of photons uniformly over the entire array or over a object.
```

### Comparing `pyxel_sim-1.8/pyxel/models/photon_collection/load_image.py` & `pyxel_sim-1.9/pyxel/models/photon_collection/load_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel photon generator models."""
 
-from typing import Literal, Optional, Tuple
+from typing import Literal, Optional
 
 from pyxel.detectors import Detector
 from pyxel.util import load_cropped_and_aligned_image
 
 
 def load_image(
     detector: Detector,
     image_file: str,
-    position: Tuple[int, int] = (0, 0),
+    position: tuple[int, int] = (0, 0),
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ] = None,
     convert_to_photons: bool = False,
     multiplier: float = 1.0,
     time_scale: float = 1.0,
     bit_resolution: Optional[int] = None,
```

### Comparing `pyxel_sim-1.8/pyxel/models/photon_collection/point_spread_function.py` & `pyxel_sim-1.9/pyxel/models/photon_collection/point_spread_function.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/photon_collection/poppy.py` & `pyxel_sim-1.9/pyxel/models/photon_collection/poppy.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Poppy model."""
 
 import logging
+from collections.abc import Mapping, Sequence
 from dataclasses import dataclass
-from typing import Any, Mapping, Sequence, Tuple, Union
+from typing import Any, Union
 
 import numpy as np
 from astropy.convolution import convolve_fft
 from astropy.io import fits
 
 from pyxel.detectors import Detector
 
@@ -333,15 +334,15 @@
 
 
 def calc_psf(
     wavelength: float,
     fov_arcsec: float,
     pixelscale: float,
     optical_parameters: Sequence[OpticalParameter],
-) -> Tuple[Sequence[fits.hdu.image.PrimaryHDU], Sequence["op.Wavefront"]]:
+) -> tuple[Sequence[fits.hdu.image.PrimaryHDU], Sequence["op.Wavefront"]]:
     """Calculate the point spread function for the given optical system.
 
     Parameters
     ----------
     wavelength : float
         Wavelength of incoming light in meters.
     fov_arcsec : float, optional
```

### Comparing `pyxel_sim-1.8/pyxel/models/photon_collection/shot_noise.py` & `pyxel_sim-1.9/pyxel/models/photon_generation/shot_noise.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel photon generator models: photon shot noise."""
-
 from typing import Literal, Optional
 
 import numpy as np
 
 from pyxel.detectors import Detector
-from pyxel.util import set_random_seed
+from pyxel.util import deprecated, set_random_seed
 
 
 def compute_poisson_noise(array: np.ndarray) -> np.ndarray:
     """Compute Poisson noise using the input array.
 
     Parameters
     ----------
@@ -45,15 +44,18 @@
     output: ndarray
         Output array.
     """
     output = np.random.normal(loc=array, scale=np.sqrt(array))
     return output
 
 
-def compute_noise(array: np.ndarray, type: str = "poisson") -> np.ndarray:
+def compute_noise(
+    array: np.ndarray,
+    type: str = "poisson",  # noqa: A002
+) -> np.ndarray:
     """Compute shot noise for an input array. It can be either Poisson noise or Gaussian.
 
     Parameters
     ----------
     array : ndarray
         Input array.
     type : str, optional
@@ -70,17 +72,21 @@
     elif type == "normal":
         output = compute_gaussian_noise(array)
         return output
     else:
         raise ValueError("Invalid noise type!")
 
 
+@deprecated(
+    "Model 'pyxel.models.photon_generation.shot_noise' is deprecated and will be removed in version 2. "
+    "Use model 'pyxel.models.photon_collection.shot_noise' instead."
+)
 def shot_noise(
     detector: Detector,
-    type: Literal["poisson", "normal"] = "poisson",
+    type: Literal["poisson", "normal"] = "poisson",  # noqa: A002
     seed: Optional[int] = None,
 ) -> None:
     """Add shot noise to the flux of photon per pixel. It can be either Poisson noise or Gaussian.
 
     Parameters
     ----------
     detector : Detector
```

### Comparing `pyxel_sim-1.8/pyxel/models/photon_collection/stripe_pattern.py` & `pyxel_sim-1.9/pyxel/models/photon_collection/stripe_pattern.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 
 """Stripe pattern illumination model."""
 
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING
 
 import numpy as np
 import skimage.transform as tr
 
 if TYPE_CHECKING:
     from pyxel.detectors import Detector
 
 
-def square_signal(n: int, lw: int, start_with: int = 0) -> List[int]:
+def square_signal(n: int, lw: int, start_with: int = 0) -> list[int]:
     """Compute a 1D periodic square signal.
 
     Parameters
     ----------
     n : int
         Length of the signal.
     lw
@@ -32,16 +32,16 @@
     Returns
     -------
     list
         Output list.
     """
     if lw > n // 2:
         raise ValueError("Line too wide.")
-    start: List[int] = [start_with] * lw
-    second: List[int] = [1 - start_with] * lw
+    start: list[int] = [start_with] * lw
+    second: list[int] = [1 - start_with] * lw
     pair = start + second
     num = n // len(pair)
     out = pair * num
     return out
 
 
 def compute_pattern(
@@ -83,16 +83,16 @@
 
     n = max(y, x) * 2
     m = max(y, x) * 2
 
     sx = slice(n // 2 - y // 2, n // 2 + y // 2)
     sy = slice(m // 2 - x // 2, m // 2 + x // 2)
 
-    signal_lst: List[int] = square_signal(n=n, lw=period // 2, start_with=start_with)
-    new_signal_lst: List[int] = signal_lst + ([1] * (n - len(signal_lst)))
+    signal_lst: list[int] = square_signal(n=n, lw=period // 2, start_with=start_with)
+    new_signal_lst: list[int] = signal_lst + ([1] * (n - len(signal_lst)))
     signal = np.array(new_signal_lst)[::-1]
 
     out = np.ones((n, m))
 
     for i in range(m):
         out[:, i] = signal
```

### Comparing `pyxel_sim-1.8/pyxel/models/photon_generation/__init__.py` & `pyxel_sim-1.9/pyxel/models/photon_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/photon_generation/illumination.py` & `pyxel_sim-1.9/pyxel/models/photon_generation/illumination.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel photon generator models."""
-from typing import Literal, Optional, Sequence, Tuple
+from collections.abc import Sequence
+from typing import Literal, Optional
 
 import numpy as np
 
 from pyxel.detectors import Detector
 from pyxel.util import deprecated
 
 
 def rectangular(
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     level: float,
     object_size: Optional[Sequence[int]] = None,
     object_center: Optional[Sequence[int]] = None,
 ) -> np.ndarray:
     """Calculate an image of a rectangular object.
 
     Parameters
@@ -63,15 +64,15 @@
     q0 = int(np.clip(q, a_min=0, a_max=shape[1]))
     photon_array[slice(p0, p + object_size[0]), slice(q0, q + object_size[1])] = level
 
     return photon_array
 
 
 def elliptic(
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     level: float,
     object_size: Optional[Sequence[int]] = None,
     object_center: Optional[Sequence[int]] = None,
 ) -> np.ndarray:
     """Calculate an image of an elliptic object.
 
     Parameters
@@ -115,15 +116,15 @@
         + ((y - object_center[0]) / float(object_size[0] / 2)) ** 2
     )
     photon_array[dist_from_center < 1] = level
     return photon_array
 
 
 def calculate_illumination(
-    shape: Tuple[int, int],
+    shape: tuple[int, int],
     level: float,
     option: Literal["uniform", "rectangular", "elliptic"] = "uniform",
     object_size: Optional[Sequence[int]] = None,
     object_center: Optional[Sequence[int]] = None,
 ) -> np.ndarray:
     """Calculate the array of photons uniformly over the entire array or over a object.
```

### Comparing `pyxel_sim-1.8/pyxel/models/photon_generation/load_image.py` & `pyxel_sim-1.9/pyxel/models/photon_generation/load_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel photon generator models."""
-from typing import Literal, Optional, Tuple
+from typing import Literal, Optional
 
 from pyxel.detectors import Detector
 from pyxel.util import deprecated, load_cropped_and_aligned_image
 
 
 @deprecated(
     "Model 'pyxel.models.photon_generation.load_image' is deprecated and will be removed in version 2. "
     "Use model 'pyxel.models.photon_collection.load_image' instead."
 )
 def load_image(
     detector: Detector,
     image_file: str,
-    position: Tuple[int, int] = (0, 0),
+    position: tuple[int, int] = (0, 0),
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ] = None,
     convert_to_photons: bool = False,
     multiplier: float = 1.0,
     time_scale: float = 1.0,
     bit_resolution: Optional[int] = None,
```

### Comparing `pyxel_sim-1.8/pyxel/models/photon_generation/shot_noise.py` & `pyxel_sim-1.9/pyxel/models/photon_collection/shot_noise.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Pyxel photon generator models: photon shot noise."""
+
 from typing import Literal, Optional
 
 import numpy as np
 
 from pyxel.detectors import Detector
-from pyxel.util import deprecated, set_random_seed
+from pyxel.util import set_random_seed
 
 
 def compute_poisson_noise(array: np.ndarray) -> np.ndarray:
     """Compute Poisson noise using the input array.
 
     Parameters
     ----------
@@ -44,15 +45,18 @@
     output: ndarray
         Output array.
     """
     output = np.random.normal(loc=array, scale=np.sqrt(array))
     return output
 
 
-def compute_noise(array: np.ndarray, type: str = "poisson") -> np.ndarray:
+def compute_noise(
+    array: np.ndarray,
+    type: str = "poisson",  # noqa: A002
+) -> np.ndarray:
     """Compute shot noise for an input array. It can be either Poisson noise or Gaussian.
 
     Parameters
     ----------
     array : ndarray
         Input array.
     type : str, optional
@@ -69,21 +73,17 @@
     elif type == "normal":
         output = compute_gaussian_noise(array)
         return output
     else:
         raise ValueError("Invalid noise type!")
 
 
-@deprecated(
-    "Model 'pyxel.models.photon_generation.shot_noise' is deprecated and will be removed in version 2. "
-    "Use model 'pyxel.models.photon_collection.shot_noise' instead."
-)
 def shot_noise(
     detector: Detector,
-    type: Literal["poisson", "normal"] = "poisson",
+    type: Literal["poisson", "normal"] = "poisson",  # noqa: A002
     seed: Optional[int] = None,
 ) -> None:
     """Add shot noise to the flux of photon per pixel. It can be either Poisson noise or Gaussian.
 
     Parameters
     ----------
     detector : Detector
```

### Comparing `pyxel_sim-1.8/pyxel/models/photon_generation/stripe_pattern.py` & `pyxel_sim-1.9/pyxel/models/photon_generation/stripe_pattern.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 
 """Stripe pattern illumination model."""
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING
 
 import numpy as np
 import skimage.transform as tr
 
 from pyxel.util import deprecated
 
 if TYPE_CHECKING:
     from pyxel.detectors import Detector
 
 
-def square_signal(n: int, lw: int, start_with: int = 0) -> List[int]:
+def square_signal(n: int, lw: int, start_with: int = 0) -> list[int]:
     """Compute a 1D periodic square signal.
 
     Parameters
     ----------
     n : int
         Length of the signal.
     lw
@@ -33,16 +33,16 @@
     Returns
     -------
     list
         Output list.
     """
     if lw > n // 2:
         raise ValueError("Line too wide.")
-    start: List[int] = [start_with] * lw
-    second: List[int] = [1 - start_with] * lw
+    start: list[int] = [start_with] * lw
+    second: list[int] = [1 - start_with] * lw
     pair = start + second
     num = n // len(pair)
     out = pair * num
     return out
 
 
 def compute_pattern(
@@ -84,16 +84,16 @@
 
     n = max(y, x) * 2
     m = max(y, x) * 2
 
     sx = slice(n // 2 - y // 2, n // 2 + y // 2)
     sy = slice(m // 2 - x // 2, m // 2 + x // 2)
 
-    signal_lst: List[int] = square_signal(n=n, lw=period // 2, start_with=start_with)
-    new_signal_lst: List[int] = signal_lst + ([1] * (n - len(signal_lst)))
+    signal_lst: list[int] = square_signal(n=n, lw=period // 2, start_with=start_with)
+    new_signal_lst: list[int] = signal_lst + ([1] * (n - len(signal_lst)))
     signal = np.array(new_signal_lst)[::-1]
 
     out = np.ones((n, m))
 
     for i in range(m):
         out[:, i] = signal
```

### Comparing `pyxel_sim-1.8/pyxel/models/readout_electronics/__init__.py` & `pyxel_sim-1.9/pyxel/models/readout_electronics/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/readout_electronics/amplification.py` & `pyxel_sim-1.9/pyxel/models/readout_electronics/amplification.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/readout_electronics/amplifier_crosstalk.py` & `pyxel_sim-1.9/pyxel/models/readout_electronics/amplifier_crosstalk.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Amplifier crosstalk model: https://arxiv.org/abs/1808.00790."""
 
+from collections.abc import Sequence
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, List, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Any, Union
 
 import numba
 import numpy as np
 
 from pyxel import load_table
 
 if TYPE_CHECKING:
@@ -46,15 +47,15 @@
 
     return result
 
 
 @numba.njit
 def get_channel_slices(
     shape: tuple, channel_matrix: np.ndarray
-) -> List[List[Tuple[Any, Any]]]:
+) -> list[list[tuple[Any, Any]]]:
     """Get pairs of slices that correspond to the given channel matrix in numerical order of channels.
 
     Parameters
     ----------
     shape : tuple
     channel_matrix : ndarray
 
@@ -127,15 +128,15 @@
 
     Returns
     -------
     ndarray
     """
     amp_number = channel_matrix.size  # number of amplifiers
 
-    slices: List[List[Tuple[Any, Any]]] = get_channel_slices(
+    slices: list[list[tuple[Any, Any]]] = get_channel_slices(
         shape=array.shape, channel_matrix=channel_matrix
     )
 
     array_copy = array.copy()
 
     for k in range(amp_number):
         for j in range(amp_number):
@@ -177,15 +178,15 @@
 
     Returns
     -------
     ndarray
     """
     amp_number = channel_matrix.size  # number of amplifiers
 
-    slices: List[List[Tuple[Any, Any]]] = get_channel_slices(
+    slices: list[list[tuple[Any, Any]]] = get_channel_slices(
         shape=array.shape, channel_matrix=channel_matrix
     )
 
     array_copy = array.copy()
 
     for k in range(amp_number):
         for j in range(amp_number):
```

### Comparing `pyxel_sim-1.8/pyxel/models/readout_electronics/dead_time.py` & `pyxel_sim-1.9/pyxel/models/readout_electronics/dead_time.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/readout_electronics/phase_conversion.py` & `pyxel_sim-1.9/pyxel/models/readout_electronics/phase_conversion.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/models/readout_electronics/sar_adc_with_noise.py` & `pyxel_sim-1.9/pyxel/models/readout_electronics/sar_adc_with_noise.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """:term:`SAR` :term:`ADC` model with noise."""
 
-from typing import Tuple
-
 import numpy as np
 
 from pyxel.detectors import Detector
 
 
 def apply_sar_adc_with_noise(
     signal_2d: np.ndarray,
@@ -71,16 +69,16 @@
 
     return data_digitized_2d
 
 
 # TODO: documentation, range volt - only max is used
 def sar_adc_with_noise(
     detector: Detector,
-    strengths: Tuple[float, ...],
-    noises: Tuple[float, ...],
+    strengths: tuple[float, ...],
+    noises: tuple[float, ...],
 ) -> None:
     r"""Digitize signal array using :term:`SAR` (Successive Approximation Register) :term:`ADC` logic with noise.
 
     Successive-approximation-register (:term:`SAR`) analog-to-digital converters (:term:`ADC`)
     for each bit, will compare the randomly perturbated **reference voltage** to
     the voltage of the pixel, adding the corresponding digital value if it is superior.
     The perturbations are generated randomly for each pixel.
```

### Comparing `pyxel_sim-1.8/pyxel/models/readout_electronics/simple_adc.py` & `pyxel_sim-1.9/pyxel/models/readout_electronics/simple_adc.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 
 """Simple ADC model functions."""
 
-from typing import Literal, Tuple
+from typing import Literal
 
 import numpy as np
 
 from pyxel.detectors import Detector
 
 
 def apply_simple_adc(
-    signal: np.ndarray, bit_resolution: int, voltage_range: Tuple[float, float]
+    signal: np.ndarray, bit_resolution: int, voltage_range: tuple[float, float]
 ) -> np.ndarray:
     """Apply digitization.
 
     Parameters
     ----------
     signal : np.ndarray
         Input signal.
```

### Comparing `pyxel_sim-1.8/pyxel/models/util.py` & `pyxel_sim-1.9/pyxel/models/util.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/notebook/__init__.py` & `pyxel_sim-1.9/pyxel/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/notebook/calibration.py` & `pyxel_sim-1.9/pyxel/notebook/calibration.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 if TYPE_CHECKING:
     import holoviews as hv
     import xarray as xr
 
     from pyxel.calibration import Calibration
     from pyxel.detectors import Detector
+    from pyxel.pipelines import ResultId
 
 
 def display_calibration_inputs(
     calibration: "Calibration", detector: "Detector"
 ) -> "hv.Layout":
     """Display calibration inputs and target data based on configuration file.
 
@@ -169,20 +170,20 @@
     import holoviews as hv
     import xarray as xr
 
     # Apply an extension to Holoviews (if needed)
     if not hv.Store.renderers:
         hv.extension("bokeh")
 
-    result_type = ds.attrs["result_type"]
+    result_type: "ResultId" = ds.attrs["result_type"]
 
     var_name = {
-        "ResultType.Image": "simulated_image",
-        "ResultType.Signal": "simulated_signal",
-        "ResultType.Pixel": "simulated_pixel",
+        "image": "simulated_image",
+        "signal": "simulated_signal",
+        "pixel": "simulated_pixel",
     }[result_type]
 
     simulated_data = ds[var_name]
     target_data = ds["target"]
 
     output_data = xr.Dataset()
     output_data["simulated"] = simulated_data
```

### Comparing `pyxel_sim-1.8/pyxel/notebook/html_representation.py` & `pyxel_sim-1.9/pyxel/notebook/html_representation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/notebook/jupyxel.py` & `pyxel_sim-1.9/pyxel/notebook/jupyxel.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Tools for jupyter notebook visualization."""
 
-from typing import TYPE_CHECKING, Any, Dict, Sequence, Union
+from collections.abc import Sequence
+from typing import TYPE_CHECKING, Any, Union
 
 import numpy as np
 
 from pyxel.data_structure import Persistence, SimplePersistence
 
 if TYPE_CHECKING:
     import matplotlib.pyplot as plt
@@ -154,27 +155,27 @@
     import holoviews as hv
 
     # Apply an extension to Holoviews (if needed)
     if not hv.Store.renderers:
         hv.extension("bokeh")
 
     # Container for detector data, leave out where there is none.
-    det: Dict[str, np.ndarray] = {}
+    det: dict[str, np.ndarray] = {}
     if detector.input_image is not None:
-        det["Input"] = detector.input_image
+        det["Input Image"] = detector.input_image
     if detector._photon is not None:
-        det["Photon"] = detector.photon.array
+        det["Photon [ph]"] = detector.photon.array
     if detector._charge is not None:
-        det["Charge"] = detector.charge.array
+        det["Charge [e-]"] = detector.charge.array
     if detector._pixel is not None:
-        det["Pixel"] = detector.pixel.array
+        det["Pixel [e-]"] = detector.pixel.array
     if detector._signal is not None:
-        det["Signal"] = detector.signal.array
+        det["Signal [V]"] = detector.signal.array
     if detector._image is not None:
-        det["Image"] = detector.image.array
+        det["Image [ADU]"] = detector.image.array
 
     def get_image(name):
         data: np.ndarray = det[name]
 
         if detector.geometry.row == 1:
             im = hv.Curve((range(len(data[0, :])), data[0, :])).opts(
                 tools=["hover"], aspect=1.5, xlabel="x", ylabel="z"
```

### Comparing `pyxel_sim-1.8/pyxel/observation/observation.py` & `pyxel_sim-1.9/pyxel/observation/observation.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,51 +4,47 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Parametric mode class and helper functions."""
 import itertools
 import logging
-import sys
 from collections import Counter
+from collections.abc import Iterable, Iterator, Mapping, Sequence
 from copy import deepcopy
 from dataclasses import dataclass
 from enum import Enum
-from functools import partial
+from functools import partial, reduce
 from numbers import Number
 from typing import (
     TYPE_CHECKING,
     Any,
-    Dict,
-    Iterable,
-    Iterator,
-    List,
+    Callable,
     Literal,
-    Mapping,
     NamedTuple,
     Optional,
-    Sequence,
     Tuple,
     Union,
 )
 
 import dask.bag as db
 import numpy as np
 import pandas as pd
 import toolz
 from numpy.typing import ArrayLike
 from tqdm.auto import tqdm
 
-from pyxel.exposure import Readout, run_exposure_pipeline
+from pyxel.exposure import Readout, run_exposure_pipeline, run_pipeline
 from pyxel.observation.parameter_values import ParameterType, ParameterValues
-from pyxel.pipelines import ResultType
+from pyxel.pipelines import ResultId, get_result_id
 from pyxel.state import get_obj_att, get_value
 
 if TYPE_CHECKING:
     import xarray as xr
+    from datatree import DataTree
 
     from pyxel.outputs import ObservationOutputs
     from pyxel.pipelines import Processor
 
 
 class ParameterMode(Enum):
     """Parameter mode class."""
@@ -57,25 +53,25 @@
     Sequential = "sequential"
     Custom = "custom"
 
 
 class ObservationResult(NamedTuple):
     """Result class for observation class."""
 
-    dataset: Union["xr.Dataset", Dict[str, "xr.Dataset"]]
+    dataset: Union["xr.Dataset", dict[str, "xr.Dataset"]]
     parameters: "xr.Dataset"
     logs: "xr.Dataset"
 
 
 @dataclass(frozen=True)
 class ParameterItem:
     """Internal Parameter Item."""
 
     # TODO: Merge 'index' and 'parameters'
-    index: Tuple[int, ...]
+    index: tuple[int, ...]
     parameters: Mapping[str, Any]
     run_index: int
 
 
 @dataclass(frozen=True)
 class CustomParameterItem:
     """Internal Parameter Item."""
@@ -100,15 +96,15 @@
     else:
         raise NotImplementedError
 
 
 # TODO: This function will be deprecated (see #563)
 def _get_short_dimension_names(types: Mapping[str, ParameterType]) -> Mapping[str, str]:
     # Create potential names for the dimensions
-    potential_dim_names: Dict[str, str] = {}
+    potential_dim_names: dict[str, str] = {}
     for param_name, param_type in types.items():
         short_name: str = short(param_name)
 
         potential_dim_names[param_name] = _get_final_short_name(
             name=short_name, param_type=param_type
         )
 
@@ -116,15 +112,15 @@
     count_dim_names: Mapping[str, int] = Counter(potential_dim_names.values())
 
     duplicate_dim_names: Sequence[str] = [
         name for name, freq in count_dim_names.items() if freq > 1
     ]
 
     if duplicate_dim_names:
-        dim_names: Dict[str, str] = {}
+        dim_names: dict[str, str] = {}
         for param_name, param_type in types.items():
             short_name = potential_dim_names[param_name]
 
             if short_name in duplicate_dim_names:
                 new_short_name: str = _get_short_name_with_model(param_name)
                 dim_names[param_name] = _get_final_short_name(
                     name=new_short_name, param_type=param_type
@@ -139,29 +135,29 @@
 
 
 # TODO: Add unit tests
 def _get_short_dimension_names_new(
     types: Mapping[str, ParameterType]
 ) -> Mapping[str, str]:
     # Create potential names for the dimensions
-    potential_dim_names: Dict[str, str] = {}
+    potential_dim_names: dict[str, str] = {}
     for param_name in types:
         short_name: str = short(param_name)
 
         potential_dim_names[param_name] = short_name
 
     # Find possible duplicates
     count_dim_names: Mapping[str, int] = Counter(potential_dim_names.values())
 
     duplicate_dim_names: Sequence[str] = [
         name for name, freq in count_dim_names.items() if freq > 1
     ]
 
     if duplicate_dim_names:
-        dim_names: Dict[str, str] = {}
+        dim_names: dict[str, str] = {}
         for param_name in types:
             short_name = potential_dim_names[param_name]
 
             if short_name in duplicate_dim_names:
                 new_short_name: str = _get_short_name_with_model(param_name)
                 dim_names[param_name] = new_short_name
 
@@ -179,17 +175,17 @@
     def __init__(
         self,
         outputs: "ObservationOutputs",
         parameters: Sequence[ParameterValues],
         readout: Optional[Readout] = None,
         mode: Literal["product", "sequential", "custom"] = "product",
         from_file: Optional[str] = None,  # Note: Only For 'custom' mode
-        column_range: Optional[Tuple[int, int]] = None,  # Note: Only For 'custom' mode
+        column_range: Optional[tuple[int, int]] = None,  # Note: Only For 'custom' mode
         with_dask: bool = False,
-        result_type: Literal["image", "signal", "pixel", "all"] = "all",
+        result_type: str = "all",
         pipeline_seed: Optional[int] = None,
     ):
         self.outputs = outputs
         self.readout: Readout = readout or Readout()
         self.parameter_mode: ParameterMode = ParameterMode(mode)
         self._parameters: Sequence[ParameterValues] = parameters
 
@@ -197,32 +193,32 @@
         self._custom_file: Optional[str] = from_file
         self._custom_data: Optional[pd.DataFrame] = None
         self._custom_columns: Optional[slice] = (
             slice(*column_range) if column_range else None
         )
 
         self.with_dask = with_dask
-        self.parameter_types: Dict[str, ParameterType] = {}
-        self._result_type = ResultType(result_type)
+        self.parameter_types: dict[str, ParameterType] = {}
+        self._result_type: ResultId = get_result_id(result_type)
         self._pipeline_seed = pipeline_seed
 
         if self.parameter_mode == ParameterMode.Custom:
             self._load_custom_parameters()
 
     def __repr__(self):
         cls_name: str = self.__class__.__name__
         return f"{cls_name}<mode={self.parameter_mode!s}>"
 
     @property
-    def result_type(self) -> ResultType:
+    def result_type(self) -> ResultId:
         """TBW."""
         return self._result_type
 
     @result_type.setter
-    def result_type(self, value: ResultType) -> None:
+    def result_type(self, value: ResultId) -> None:
         """TBW."""
         self._result_type = value
 
     @property
     def pipeline_seed(self) -> Optional[int]:
         """TBW."""
         return self._pipeline_seed
@@ -251,17 +247,17 @@
         filtered_data: pd.DataFrame = all_data.loc[:, self._custom_columns]
 
         self._custom_data = filtered_data
 
     def _custom_parameters(
         self,
     ) -> Iterator[
-        Tuple[
+        tuple[
             int,
-            Dict[str, Union[Number, str, Sequence[Union[Number, str]]]],
+            dict[str, Union[Number, str, Sequence[Union[Number, str]]]],
         ]
     ]:
         """Generate custom mode parameters based on input file.
 
         Yields
         ------
         index: int
@@ -272,15 +268,15 @@
 
         index: int
         row_serie: pd.Series
         for index, row_serie in self._custom_data.iterrows():
             row: Sequence[Union[Number, str]] = row_serie.to_list()
 
             i: int = 0
-            parameter_dict: Dict[
+            parameter_dict: dict[
                 str, Union[Number, str, Sequence[Union[Number, str]]]
             ] = {}
             for step in self.enabled_steps:
                 key: str = step.key
 
                 # TODO: this is confusing code. Fix this.
                 #       Furthermore 'step.values' should be a `List[int, float]` and not a `str`
@@ -296,27 +292,27 @@
                         raise ValueError(
                             'Only "_" characters (or a list of them) should be used to '
                             "indicate parameters updated from file in custom mode"
                         )
 
                     value: Sequence[Union[Number, str]] = row[
                         i : i + len(values_flattened)
-                    ]  # noqa: E203
+                    ]
                     assert len(value) == len(step.values)
 
                     parameter_dict[key] = value
 
                 else:
                     raise NotImplementedError
 
                 i += len(step.values)
 
             yield index, parameter_dict
 
-    def _sequential_parameters(self) -> Iterator[Tuple[int, dict]]:
+    def _sequential_parameters(self) -> Iterator[tuple[int, dict]]:
         """Generate sequential mode parameters.
 
         Yields
         ------
         index: int
         parameter_dict: dict
         """
@@ -336,15 +332,15 @@
         """
         step_ranges = [range(len(step)) for step in self.enabled_steps]
         out = itertools.product(*step_ranges)
         return out
 
     def _product_parameters(
         self,
-    ) -> Iterator[Tuple[Tuple, Dict[str, Any]]]:
+    ) -> Iterator[tuple[tuple, dict[str, Any]]]:
         """Generate product mode parameters.
 
         Yields
         ------
         indices: tuple
         parameter_dict: dict
         """
@@ -355,30 +351,74 @@
         ):
             parameter_dict = {}
             for key, value in zip(keys, params):
                 parameter_dict.update({key: value})
             yield indices, parameter_dict
 
     # TODO: This function will be deprecated (see #563)
-    def _parameter_it(self) -> Iterator[Tuple]:
+    def _parameter_it(self) -> Iterator[tuple]:
         """Return the method for generating parameters based on parametric mode."""
         if self.parameter_mode == ParameterMode.Product:
             yield from self._product_parameters()
 
         elif self.parameter_mode == ParameterMode.Sequential:
             yield from self._sequential_parameters()
 
         elif self.parameter_mode == ParameterMode.Custom:
             yield from self._custom_parameters()
         else:
             raise NotImplementedError
 
+    def _get_parameters_item(
+        self, processor: "Processor"
+    ) -> Sequence[Union[ParameterItem, CustomParameterItem]]:
+        if self.parameter_mode == ParameterMode.Product:
+            params_it: Iterator = self._product_parameters()
+
+            return [
+                ParameterItem(index=index, parameters=parameter_dict, run_index=n)
+                for n, (index, parameter_dict) in enumerate(params_it)
+            ]
+
+        elif self.parameter_mode == ParameterMode.Sequential:
+            # Get default values for all unique parameters
+            params_all_keys: Sequence[str] = [
+                param_value.key for param_value in self.enabled_steps
+            ]
+            params_unique_keys: Iterator[str] = toolz.unique(params_all_keys)
+
+            params_defaults: Mapping[str, np.ndarray] = {
+                key: processor.get(key) for key in params_unique_keys
+            }
+
+            params_it = self._sequential_parameters()
+
+            return [
+                CustomParameterItem(
+                    index=index,
+                    parameters=params_defaults | parameter_dict,
+                    run_index=n,
+                )
+                for n, (index, parameter_dict) in enumerate(params_it)
+            ]
+
+        elif self.parameter_mode == ParameterMode.Custom:
+            params_it = self._custom_parameters()
+
+            return [
+                CustomParameterItem(index=index, parameters=parameter_dict, run_index=n)
+                for n, (index, parameter_dict) in enumerate(params_it)
+            ]
+
+        else:
+            raise ValueError("Parametric mode not specified.")
+
     def _processors_it(
         self, processor: "Processor"
-    ) -> Iterator[Tuple["Processor", Union[int, Tuple[int]], Dict]]:
+    ) -> Iterator[tuple["Processor", Union[int, tuple[int]], dict]]:
         """Generate processors with different product parameters.
 
         Parameters
         ----------
         processor: Processor
 
         Yields
@@ -399,15 +439,15 @@
         """Check for each step if parameters can be used as dataset coordinates (1D, simple) or not (multi)."""
         for step in self.enabled_steps:
             self.parameter_types.update({step.key: step.type})
         return self.parameter_types
 
     def run_debug_mode(
         self, processor: "Processor"
-    ) -> Tuple[List["Processor"], "xr.Dataset"]:
+    ) -> tuple[list["Processor"], "xr.Dataset"]:
         """Run observation pipelines in debug mode and return list of processors and parameter logs.
 
         Parameters
         ----------
         processor: Processor
 
         Returns
@@ -415,15 +455,15 @@
         processors: list
         final_logs: Dataset
         """
         # Late import to speedup start-up time
         import xarray as xr
 
         processors = []
-        logs: List[xr.Dataset] = []
+        logs: list[xr.Dataset] = []
 
         for processor_id, (proc, _index, parameter_dict) in enumerate(
             tqdm(self._processors_it(processor))
         ):
             log: xr.Dataset = log_parameters(
                 processor_id=processor_id, parameter_dict=parameter_dict
             )
@@ -482,20 +522,21 @@
                 and self.parameter_mode != ParameterMode.Custom
             ):
                 raise ValueError(
                     "Either define 'custom' as parametric mode or "
                     "do not use '_' character in 'values' field"
                 )
 
+    # TODO: This method will be deprecated (see #563)
     def run_observation(self, processor: "Processor") -> ObservationResult:
         """Run the observation pipelines.
 
         Parameters
         ----------
-        processor: Processor
+        processor : Processor
 
         Returns
         -------
         Result
         """
         # Late import to speedup start-up time
         import xarray as xr
@@ -528,15 +569,15 @@
 
             if self.with_dask:
                 dataset_list = db.from_sequence(lst).map(apply_pipeline).compute()
             else:
                 dataset_list = list(map(apply_pipeline, tqdm(lst)))
 
             # prepare lists for to-be-merged datasets
-            parameters: List[List[xr.Dataset]] = [
+            parameters: list[list[xr.Dataset]] = [
                 [] for _ in range(len(self.enabled_steps))
             ]
             logs = []
 
             for processor_id, (indices, parameter_dict, _) in enumerate(lst):
                 # log parameters for this pipeline
                 log = log_parameters(
@@ -551,15 +592,15 @@
                         dimension_names=dim_names,
                         index=indices[i],
                         coordinate_name=coordinate,
                     )
                     parameters[i].append(parameter_ds)
 
             # merging/combining the outputs
-            final_parameters_list: List[xr.Dataset] = []
+            final_parameters_list: list[xr.Dataset] = []
             for p in parameters:
                 # See issue #276
                 new_dataset = xr.combine_by_coords(p)
                 if not isinstance(new_dataset, xr.Dataset):
                     raise TypeError("Expecting 'Dataset'.")
 
                 final_parameters_list.append(new_dataset)
@@ -708,160 +749,68 @@
                 dataset=final_ds, parameters=final_parameters, logs=final_log
             )
             return result
 
         else:
             raise ValueError("Parametric mode not specified.")
 
-    def run_observation_new(self, processor: "Processor") -> "xr.Dataset":
+    def run_observation_datatree(self, processor: "Processor") -> "DataTree":
         """Run the observation pipelines."""
         # Late import to speedup start-up time
-        import xarray as xr
+        from datatree import DataTree
 
         # validation
         self.validate_steps(processor)
 
         types: Mapping[str, ParameterType] = self._get_parameter_types()
-
         dim_names: Mapping[str, str] = _get_short_dimension_names_new(types)
 
-        y = range(processor.detector.geometry.row)
-        x = range(processor.detector.geometry.col)
-        times = self.readout.times
-
-        if self.parameter_mode == ParameterMode.Product:
-            apply_pipeline = partial(
-                self._apply_exposure_pipeline_product_new,
-                dimension_names=dim_names,
-                x=x,
-                y=y,
-                processor=processor,
-                times=times,
-                types=types,
-            )
-
-            params_it: Iterator = self._product_parameters()
-
-            lst: Sequence[ParameterItem] = [
-                ParameterItem(index=index, parameters=parameter_dict, run_index=n)
-                for n, (index, parameter_dict) in enumerate(params_it)
-            ]
-
-            if self.with_dask:
-                dataset_bag: db.Bag = db.from_sequence(lst).map(apply_pipeline)
-                dataset_list: Sequence[xr.Dataset] = dataset_bag.compute()
-            else:
-                dataset_list = [apply_pipeline(el) for el in tqdm(lst)]
-
-            # See issue #276
-            final_dataset = xr.combine_by_coords(dataset_list)
-            if not isinstance(final_dataset, xr.Dataset):
-                raise TypeError("Expecting 'Dataset'.")
-
-            return final_dataset
+        apply_pipeline: Callable[
+            [Union[ParameterItem, CustomParameterItem]], DataTree
+        ] = partial(
+            self._apply_exposure_pipeline_new,
+            dimension_names=dim_names,
+            processor=processor,
+            types=types,
+        )
 
-        elif self.parameter_mode == ParameterMode.Sequential:
-            apply_pipeline = partial(
-                self._apply_exposure_pipeline_sequential_new,
-                dimension_names=dim_names,
-                x=x,
-                y=y,
-                processor=processor,
-                times=times,
-                types=types,
+        parameters: Sequence[
+            Union[ParameterItem, CustomParameterItem]
+        ] = self._get_parameters_item(processor=processor)
+
+        if self.with_dask:
+            datatree_bag: db.Bag = (
+                db.from_sequence(parameters)
+                .map(apply_pipeline)
+                .fold(binop=DataTree.combine_first, combine=DataTree.combine_first)  # type: ignore
             )
-
-            # Get default values for all unique parameters
-            params_all_keys: Sequence[str] = [
-                param_value.key for param_value in self.enabled_steps
-            ]
-            params_unique_keys: Iterator[str] = toolz.unique(params_all_keys)
-
-            params_defaults: Mapping[str, np.ndarray] = {
-                key: processor.get(key) for key in params_unique_keys
-            }
-
-            params_it = self._sequential_parameters()
-
-            if sys.version_info >= (3, 9):
-                lst_sequence = [
-                    CustomParameterItem(
-                        index=index,
-                        parameters=params_defaults | parameter_dict,
-                        run_index=n,
-                    )
-                    for n, (index, parameter_dict) in enumerate(params_it)
-                ]
-            else:
-                lst_sequence = [
-                    CustomParameterItem(
-                        index=index,
-                        parameters={**params_defaults, **parameter_dict},
-                        run_index=n,
-                    )
-                    for n, (index, parameter_dict) in enumerate(params_it)
-                ]
-
-            if self.with_dask:
-                dataset_list = (
-                    db.from_sequence(lst_sequence).map(apply_pipeline).compute()
-                )
-            else:
-                dataset_list = list(map(apply_pipeline, tqdm(lst_sequence)))
-
-            # See issue #276
-            final_dataset = xr.combine_by_coords(dataset_list)
-            if not isinstance(final_dataset, xr.Dataset):
-                raise TypeError("Expecting 'Dataset'.")
-
-            return final_dataset
-
-        elif self.parameter_mode == ParameterMode.Custom:
-            apply_pipeline = partial(
-                self._apply_exposure_pipeline_custom_new,
-                dimension_names=dim_names,
-                x=x,
-                y=y,
-                processor=processor,
-                times=times,
-                types=types,
+            final_datatree: DataTree = datatree_bag.compute()
+        else:
+            datatree_list: Iterator[DataTree] = (
+                apply_pipeline(el) for el in tqdm(parameters)
             )
+            final_datatree = reduce(DataTree.combine_first, datatree_list)  # type: ignore
 
-            params_it = self._custom_parameters()
-
-            lst_custom = [
-                CustomParameterItem(index=index, parameters=parameter_dict, run_index=n)
-                for n, (index, parameter_dict) in enumerate(params_it)
-            ]
-
-            if self.with_dask:
-                dataset_list = (
-                    db.from_sequence(lst_custom).map(apply_pipeline).compute()
-                )
-            else:
-                dataset_list = list(map(apply_pipeline, tqdm(lst_custom)))
-
-            # See issue #276
-            final_dataset = xr.combine_by_coords(dataset_list)
-            if not isinstance(final_dataset, xr.Dataset):
-                raise TypeError("Expecting 'Dataset'.")
+        parameter_name: str = self.parameter_mode.name
+        final_datatree.attrs["running mode"] = f"Observation - {parameter_name}"
 
-            return final_dataset
+        # See issue #276. TODO: Is this still valid ?
+        # if not isinstance(final_dataset, xr.Dataset):
+        #     raise TypeError("Expecting 'Dataset'.")
 
-        else:
-            raise ValueError("Parametric mode not specified.")
+        return final_datatree
 
     # TODO: This function will be deprecated (see #563)
     def _apply_exposure_pipeline_product(
         self,
-        index_and_parameter: Tuple[
-            Tuple[int, ...],
+        index_and_parameter: tuple[
+            tuple[int, ...],
             Mapping[
                 str,
-                Union[str, Number, np.ndarray, List[Union[str, Number, np.ndarray]]],
+                Union[str, Number, np.ndarray, list[Union[str, Number, np.ndarray]]],
             ],
             int,
         ],
         dimension_names: Mapping[str, str],
         processor: "Processor",
         x: range,
         y: range,
@@ -900,70 +849,68 @@
             types=types,
         )
 
         ds.attrs.update({"running mode": "Observation - Product"})
 
         return ds
 
-    def _apply_exposure_pipeline_product_new(
+    def _apply_exposure_pipeline_new(
         self,
-        param_item: ParameterItem,
+        param_item: Union[ParameterItem, CustomParameterItem],
         dimension_names: Mapping[str, str],
         processor: "Processor",
-        x: range,
-        y: range,
-        times: np.ndarray,
         types: Mapping[str, ParameterType],
-    ) -> "xr.Dataset":
+    ) -> "DataTree":
         new_processor = create_new_processor(
             processor=processor,
             parameter_dict=param_item.parameters,
         )
 
         # run the pipeline
-        _ = run_exposure_pipeline(
+        data_tree: "DataTree" = run_pipeline(
             processor=new_processor,
             readout=self.readout,
             result_type=self.result_type,
             pipeline_seed=self.pipeline_seed,
         )
 
         _ = self.outputs.save_to_file(
             processor=new_processor,
             run_number=param_item.run_index,
         )
 
-        ds: xr.Dataset = new_processor.result_to_dataset(
-            x=x,
-            y=y,
-            times=times,
-            result_type=self.result_type,
-        )
-
         # Can also be done outside dask in a loop
-        ds = _add_product_parameters_new(
-            ds=ds,
-            parameter_dict=param_item.parameters,
-            indexes=param_item.index,
-            dimension_names=dimension_names,
-            types=types,
-        )
+        if isinstance(param_item, ParameterItem):
+            final_data_tree = _add_product_parameters_datatree(
+                data_tree=data_tree,
+                parameter_dict=param_item.parameters,
+                indexes=param_item.index,
+                dimension_names=dimension_names,
+                types=types,
+            )
 
-        ds.attrs.update({"running mode": "Observation - Product"})
+        else:
+            final_data_tree = _add_custom_parameters_datatree(
+                data_tree=data_tree,
+                parameter_dict=param_item.parameters,
+                index=param_item.index,
+                dimension_names=dimension_names,
+                types=types,
+            )
 
-        return ds
+        return final_data_tree
 
     # TODO: This function will be deprecated (see #563)
     def _apply_exposure_pipeline_custom(
         self,
-        index_and_parameter: Tuple[
+        index_and_parameter: tuple[
             int,
             Mapping[
                 str,
-                Union[str, Number, np.ndarray, List[Union[str, Number, np.ndarray]]],
+                Union[str, Number, np.ndarray, list[Union[str, Number, np.ndarray]]],
             ],
             int,
         ],
         processor: "Processor",
         x: range,
         y: range,
         times: np.ndarray,
@@ -994,69 +941,22 @@
             ds=ds,
             index=index,
         )
         ds.attrs.update({"running mode": "Observation - Custom"})
 
         return ds
 
-    def _apply_exposure_pipeline_custom_new(
-        self,
-        param_item: CustomParameterItem,
-        dimension_names: Mapping[str, str],
-        processor: "Processor",
-        x: range,
-        y: range,
-        times: np.ndarray,
-        types: Mapping[str, ParameterType],
-    ):
-        new_processor = create_new_processor(
-            processor=processor,
-            parameter_dict=param_item.parameters,
-        )
-
-        # run the pipeline
-        _ = run_exposure_pipeline(
-            processor=new_processor,
-            readout=self.readout,
-            result_type=self.result_type,
-            pipeline_seed=self.pipeline_seed,
-        )
-
-        _ = self.outputs.save_to_file(
-            processor=new_processor,
-            run_number=param_item.run_index,
-        )
-
-        ds: xr.Dataset = new_processor.result_to_dataset(
-            x=x,
-            y=y,
-            times=times,
-            result_type=self.result_type,
-        )
-
-        # Can also be done outside dask in a loop
-        ds = _add_custom_parameters_new(
-            ds=ds,
-            parameter_dict=param_item.parameters,
-            index=param_item.index,
-            dimension_names=dimension_names,
-            types=types,
-        )
-        ds.attrs.update({"running mode": "Observation - Custom"})
-
-        return ds
-
     # TODO: This function will be deprecated (see #563)
     def _apply_exposure_pipeline_sequential(
         self,
-        index_and_parameter: Tuple[
+        index_and_parameter: tuple[
             int,
             Mapping[
                 str,
-                Union[str, Number, np.ndarray, List[Union[str, Number, np.ndarray]]],
+                Union[str, Number, np.ndarray, list[Union[str, Number, np.ndarray]]],
             ],
             int,
         ],
         dimension_names: Mapping[str, str],
         processor: "Processor",
         x: range,
         y: range,
@@ -1096,62 +996,14 @@
             types=types,
         )
 
         ds.attrs.update({"running mode": "Observation - Sequential"})
 
         return ds
 
-    def _apply_exposure_pipeline_sequential_new(
-        self,
-        param_item: CustomParameterItem,
-        dimension_names: Mapping[str, str],
-        processor: "Processor",
-        x: range,
-        y: range,
-        times: np.ndarray,
-        types: Mapping[str, ParameterType],
-    ):
-        new_processor = create_new_processor(
-            processor=processor,
-            parameter_dict=param_item.parameters,
-        )
-
-        # run the pipeline
-        _ = run_exposure_pipeline(
-            processor=new_processor,
-            readout=self.readout,
-            result_type=self.result_type,
-            pipeline_seed=self.pipeline_seed,
-        )
-
-        _ = self.outputs.save_to_file(
-            processor=new_processor,
-            run_number=param_item.run_index,
-        )
-
-        ds: xr.Dataset = new_processor.result_to_dataset(
-            x=x,
-            y=y,
-            times=times,
-            result_type=self.result_type,
-        )
-
-        # Can also be done outside dask in a loop
-        ds = _add_custom_parameters_new(
-            ds=ds,
-            parameter_dict=param_item.parameters,
-            index=param_item.index,
-            dimension_names=dimension_names,
-            types=types,
-        )
-
-        ds.attrs.update({"running mode": "Observation - Sequential"})
-
-        return ds
-
     def debug_parameters(self, processor: "Processor") -> list:
         """List the parameters using processor parameters in processor generator.
 
         Parameters
         ----------
         processor: Processor
 
@@ -1171,15 +1023,15 @@
             result.append((i, values))
         return result
 
 
 def create_new_processor(
     processor: "Processor",
     parameter_dict: Mapping[
-        str, Union[str, Number, np.ndarray, List[Union[str, Number, np.ndarray]]]
+        str, Union[str, Number, np.ndarray, list[Union[str, Number, np.ndarray]]]
     ],
 ) -> "Processor":
     """Create a copy of processor and set new attributes from a dictionary before returning it.
 
     Parameters
     ----------
     processor: Processor
@@ -1292,76 +1144,78 @@
 
     ds = ds.assign_coords({"id": index})
     ds = ds.expand_dims(dim="id")
 
     return ds
 
 
-def _add_custom_parameters_new(
-    ds: "xr.Dataset",
+def _add_custom_parameters_datatree(
+    data_tree: "DataTree",
     parameter_dict: Mapping[str, Union[str, Number, ArrayLike]],
     index: int,
     dimension_names: Mapping[str, str],
     types: Mapping[str, ParameterType],
-) -> "xr.Dataset":
+) -> "DataTree":
     """Add coordinate "index" to the dataset.
 
     Parameters
     ----------
-    ds: Dataset
+    data_tree: Dataset
     index: int
 
     Returns
     -------
-    Dataset
+    DataTree
     """
     import pandas as pd
     import xarray as xr
 
-    ds = ds.expand_dims({"id": [index]})
+    data_tree = data_tree.expand_dims({"id": [index]})
 
     for coordinate_name, param_value in parameter_dict.items():
         short_name: str = dimension_names[coordinate_name]
 
         #  assigning the right coordinates based on type
         if types[coordinate_name] == ParameterType.Simple:
-            ds = ds.assign_coords({short_name: ("id", pd.Index([param_value]))})
+            data_tree = data_tree.assign_coords(
+                {short_name: ("id", pd.Index([param_value]))}
+            )
 
         elif types[coordinate_name] == ParameterType.Multi:
             data = np.array(param_value)
             data_array = xr.DataArray(data).expand_dims({"id": [index]})
-            ds = ds.assign_coords({short_name: data_array})
+            data_tree = data_tree.assign_coords({short_name: data_array})
 
         else:
             raise NotImplementedError
 
-    return ds
+    return data_tree
 
 
 # TODO: This function will be deprecated (see #563)
 def _add_sequential_parameters(
     ds: "xr.Dataset",
     parameter_dict: Mapping[
-        str, Union[str, Number, np.ndarray, List[Union[str, Number, np.ndarray]]]
+        str, Union[str, Number, np.ndarray, list[Union[str, Number, np.ndarray]]]
     ],
     dimension_names: Mapping[str, str],
     index: int,
     coordinate_name: str,
     types: Mapping[str, ParameterType],
 ) -> "xr.Dataset":
     """Add true coordinates or index to sequential mode dataset.
 
     Parameters
     ----------
-    ds: Dataset
-    parameter_dict: dict
+    ds : Dataset
+    parameter_dict : dict
     dimension_names
-    index: int
-    coordinate_name: str
-    types: dict
+    index : int
+    coordinate_name : str
+    types : dict
 
     Returns
     -------
     Dataset
     """
 
     #  assigning the right coordinates based on type
@@ -1378,18 +1232,18 @@
     return ds
 
 
 # TODO: This function will be deprecated (see #563)
 def _add_product_parameters(
     ds: "xr.Dataset",
     parameter_dict: Mapping[
-        str, Union[str, Number, np.ndarray, List[Union[str, Number, np.ndarray]]]
+        str, Union[str, Number, np.ndarray, list[Union[str, Number, np.ndarray]]]
     ],
     dimension_names: Mapping[str, str],
-    indices: Tuple[int, ...],
+    indices: tuple[int, ...],
     types: Mapping[str, ParameterType],
 ) -> "xr.Dataset":
     """Add true coordinates or index to product mode dataset.
 
     Parameters
     ----------
     ds: Dataset
@@ -1416,76 +1270,74 @@
 
         else:
             raise NotImplementedError
 
     return ds
 
 
-def to_tuples(data: Iterable) -> Tuple:
-    lst: List = []
+def to_tuples(data: Iterable) -> tuple:
+    lst: list = []
     for el in data:
         if isinstance(el, Iterable) and not isinstance(el, str):
             lst.append(to_tuples(el))
         else:
             lst.append(el)
 
     return tuple(lst)
 
 
-def _add_product_parameters_new(
-    ds: "xr.Dataset",
+def _add_product_parameters_datatree(
+    data_tree: "DataTree",
     parameter_dict: Mapping[str, Union[str, Number, ArrayLike]],
-    indexes: Tuple[int, ...],
+    indexes: tuple[int, ...],
     dimension_names: Mapping[str, str],
     types: Mapping[str, ParameterType],
-) -> "xr.Dataset":
+) -> "DataTree":
     """Add true coordinates or index to product mode dataset.
 
     Parameters
     ----------
-    ds: Dataset
-    parameter_dict: dict
-    types: dict
+    data_tree : DataTree
+    parameter_dict : dict
+    types : dict
 
     Returns
     -------
-    Dataset
+    DataTree
     """
     import xarray as xr
 
     # TODO: join 'indexes' and 'parameter_dict'
     for index, (coordinate_name, param_value) in zip(indexes, parameter_dict.items()):
         short_name: str = dimension_names[coordinate_name]
 
         #  assigning the right coordinates based on type
         if types[coordinate_name] == ParameterType.Simple:
-            ds = ds.expand_dims(dim={short_name: [param_value]})
+            data_tree = data_tree.expand_dims(dim={short_name: [param_value]})
 
         elif types[coordinate_name] == ParameterType.Multi:
             data = np.array(param_value)
             data_array = xr.DataArray(data).expand_dims(
                 dim={f"{short_name}_id": [index]}
             )
-            ds = ds.expand_dims({f"{short_name}_id": [index]}).assign_coords(
-                {short_name: data_array}
-            )
+            data_tree = data_tree.expand_dims(
+                {f"{short_name}_id": [index]}
+            ).assign_coords({short_name: data_array})
 
         else:
             raise NotImplementedError
 
-    # new_ds = ds.expand_dims(new_dimensions)
-    # return new_ds
-    return ds
+    return data_tree
 
 
 def compute_final_sequential_dataset(
     list_of_index_and_parameter: list,
     list_of_datasets: list,
     dimension_names: Mapping[str, str],
-) -> Dict[str, "xr.Dataset"]:
+) -> dict[str, "xr.Dataset"]:
     """Return a dictionary of result datasets where keys are different parameters.
 
     Parameters
     ----------
     list_of_index_and_parameter: list
     list_of_datasets: list
     dimension_names
@@ -1493,27 +1345,27 @@
     Returns
     -------
     dict
     """
     # Late import to speedup start-up time
     import xarray as xr
 
-    final_dict: Dict[str, List[xr.Dataset]] = {}
+    final_dict: dict[str, list[xr.Dataset]] = {}
 
     for _, parameter_dict, n in list_of_index_and_parameter:
         coordinate = str(list(parameter_dict)[0])
         coordinate_short: str = dimension_names[coordinate]
 
         if short(coordinate) not in final_dict:
             final_dict.update({coordinate_short: []})
             final_dict[coordinate_short].append(list_of_datasets[n])
         else:
             final_dict[coordinate_short].append(list_of_datasets[n])
 
-    final_datasets: Dict[str, xr.Dataset] = {}
+    final_datasets: dict[str, xr.Dataset] = {}
     for key, value in final_dict.items():
         ds = xr.combine_by_coords(value)
         # see issue #276
         if not isinstance(ds, xr.Dataset):
             raise TypeError("Expecting 'Dataset'.")
 
         final_datasets.update({key: ds})
```

### Comparing `pyxel_sim-1.8/pyxel/observation/parameter_values.py` & `pyxel_sim-1.9/pyxel/observation/parameter_values.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,17 +4,18 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 
 from collections import abc
+from collections.abc import Iterator, Sequence
 from enum import Enum
 from numbers import Number
-from typing import Iterator, Literal, Optional, Sequence, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 from numpy.typing import NDArray
 
 from pyxel.evaluator import eval_range
 
 
@@ -37,16 +38,16 @@
         values: Union[
             Literal["_"],
             Sequence[Literal["_"]],
             Sequence[Number],
             Sequence[str],
         ],
         boundaries: Union[
-            Tuple[float, float],
-            Sequence[Tuple[float, float]],
+            tuple[float, float],
+            Sequence[tuple[float, float]],
             None,
         ] = None,
         enabled: bool = True,
         logarithmic: bool = False,
     ):
         # TODO: maybe use numpy to check multi-dimensional input lists
         # Check YAML input (not real values yet) and define parameter type
```

### Comparing `pyxel_sim-1.8/pyxel/options.py` & `pyxel_sim-1.9/pyxel/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Subpackage to define options in Pyxel."""
 
+from collections.abc import Mapping
 from pathlib import Path
-from typing import Any, Mapping, Optional, Union
+from typing import Any, Optional, Union
 
 import attrs
 
 
 @attrs.define(on_setattr=[attrs.setters.convert, attrs.setters.validate])
 class GlobalOptions:
     """Define a container class for all available options."""
```

### Comparing `pyxel_sim-1.8/pyxel/outputs/__init__.py` & `pyxel_sim-1.9/pyxel/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/outputs/calibration_outputs.py` & `pyxel_sim-1.9/pyxel/outputs/calibration_outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,26 +4,17 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 
 """TBW."""
 
+from collections.abc import Mapping, Sequence
 from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Dict,
-    List,
-    Mapping,
-    Optional,
-    Protocol,
-    Sequence,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Optional, Protocol, Union
 
 import pandas as pd
 from dask.delayed import Delayed, delayed
 
 from pyxel.outputs import Outputs, ValidFormat, ValidName
 
 if TYPE_CHECKING:
@@ -73,15 +64,15 @@
         # Parameter(s) specific for 'Calibration'
         self.save_calibration_data: Optional[
             Sequence[Mapping[str, Sequence[str]]]
         ] = save_calibration_data
 
     def save_processors(self, processors: pd.DataFrame) -> Sequence[Delayed]:
         """TBW."""
-        lst: List[Delayed] = []
+        lst: list[Delayed] = []
 
         if self.save_data_to_file:
             for _, series in processors.iterrows():
                 id_island: int = series["island"]
                 id_processor: int = series["id_processor"]
                 processor: Delayed = series["processor"]
 
@@ -102,33 +93,33 @@
 
         Parameters
         ----------
         dataset: Dataset
         logs: DataFrame
         """
 
-        save_methods: Dict[str, SaveToFile] = {"nc": self.save_to_netcdf}
+        save_methods: dict[str, SaveToFile] = {"nc": self.save_to_netcdf}
 
         if self.save_calibration_data is not None:
             dct: Mapping[str, Sequence[str]]
             for dct in self.save_calibration_data:
                 first_item, *_ = dct.items()
                 obj, format_list = first_item
 
                 if obj == "logs":
-                    for format in format_list:
-                        if format == "csv":
+                    for formal_file in format_list:
+                        if formal_file == "csv":
                             filename = self.output_dir.joinpath("logs.csv")
                             logs.to_csv(filename)
-                        elif format == "xlsx":
+                        elif formal_file == "xlsx":
                             filename = self.output_dir.joinpath("logs.xlsx")
                             logs.to_excel(filename)
                         else:
                             raise NotImplementedError(
-                                f"Saving to format {format} not implemented"
+                                f"Saving to format {formal_file} not implemented"
                             )
 
                 elif obj == "dataset":
                     if format_list is not None:
                         for out_format in format_list:
                             if out_format not in save_methods:
                                 raise ValueError(
```

### Comparing `pyxel_sim-1.8/pyxel/outputs/exposure_outputs.py` & `pyxel_sim-1.9/pyxel/outputs/exposure_outputs.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,30 +4,23 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 
 """Single outputs."""
 
+from collections.abc import Mapping, Sequence
 from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Dict,
-    Mapping,
-    Optional,
-    Protocol,
-    Sequence,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Optional, Protocol, Union
 
 from pyxel.outputs import Outputs, ValidFormat, ValidName
 
 if TYPE_CHECKING:
     import xarray as xr
+    from datatree import DataTree
 
     class SaveToFile(Protocol):
         """TBW."""
 
         def __call__(self, data: Any, name: str, with_auto_suffix: bool = True) -> Path:
             """TBW."""
             ...
@@ -66,36 +59,35 @@
             save_data_to_file=save_data_to_file,
         )
 
         self.save_exposure_data: Optional[
             Sequence[Mapping[str, Sequence[str]]]
         ] = save_exposure_data
 
-    def save_exposure_outputs(self, dataset: "xr.Dataset") -> None:
+    def save_exposure_outputs(self, dataset: Union["xr.Dataset", "DataTree"]) -> None:
         """Save the observation outputs such as the dataset.
 
         Parameters
         ----------
         dataset: Dataset
         """
 
-        save_methods: Dict[str, SaveToFile] = {"nc": self.save_to_netcdf}
+        save_methods: dict[str, SaveToFile] = {"nc": self.save_to_netcdf}
 
-        if self.save_exposure_data is not None:
-            dct: Mapping[str, Sequence[str]]
-            for dct in self.save_exposure_data:
-                first_item, *_ = dct.items()
-                obj, format_list = first_item
-
-                if obj == "dataset":
-                    if format_list is not None:
-                        for out_format in format_list:
-                            if out_format not in save_methods:
-                                raise ValueError(
-                                    "Format " + out_format + " not a valid save method!"
-                                )
+        if self.save_exposure_data is None:
+            return
 
-                            func = save_methods[out_format]
-                            func(data=dataset, name=obj)
+        dct: Mapping[str, Sequence[str]]
+        for dct in self.save_exposure_data:
+            first_item, *_ = dct.items()
+            obj, format_list = first_item
+
+            if obj != "dataset":
+                raise NotImplementedError(f"Object {obj} unknown.")
+
+            out_format: str
+            for out_format in format_list:
+                if out_format not in save_methods:
+                    raise ValueError(f"Format {out_format} not a valid save method!")
 
-                else:
-                    raise NotImplementedError(f"Object {obj} unknown.")
+                func = save_methods[out_format]
+                func(data=dataset, name=obj)
```

### Comparing `pyxel_sim-1.8/pyxel/outputs/observation_outputs.py` & `pyxel_sim-1.9/pyxel/outputs/observation_outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,17 @@
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 
 """TBW."""
 
 import operator
+from collections.abc import Mapping, Sequence
 from pathlib import Path
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Dict,
-    Mapping,
-    Optional,
-    Protocol,
-    Sequence,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Optional, Protocol, Union
 
 from pyxel.observation import ParameterMode
 from pyxel.outputs import Outputs, ValidFormat, ValidName
 
 if TYPE_CHECKING:
     from pyxel.observation import ObservationResult
 
@@ -82,15 +74,15 @@
         ----------
         result: Result
         mode: ParameterMode
         """
 
         dataset_names = ("dataset", "parameters", "logs")
 
-        save_methods: Dict[str, SaveToFile] = {"nc": self.save_to_netcdf}
+        save_methods: dict[str, SaveToFile] = {"nc": self.save_to_netcdf}
 
         if self.save_observation_data is not None:
             dct: Mapping[str, Sequence[str]]
             for dct in self.save_observation_data:
                 first_item, *_ = dct.items()
                 obj, format_list = first_item
```

### Comparing `pyxel_sim-1.8/pyxel/outputs/outputs.py` & `pyxel_sim-1.9/pyxel/outputs/outputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,39 +4,30 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """Classes for creating outputs."""
 import logging
 import re
+from collections.abc import Mapping, Sequence
 from glob import glob
 from pathlib import Path
 from time import strftime
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    List,
-    Literal,
-    Mapping,
-    Optional,
-    Protocol,
-    Sequence,
-    Tuple,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Literal, Optional, Protocol, Union
 
 import h5py as h5
 import numpy as np
 import pandas as pd
 from PIL import Image
 
 from pyxel import __version__ as version
 
 if TYPE_CHECKING:
     import xarray as xr
+    from datatree import DataTree
 
     from pyxel.detectors import Detector
     from pyxel.pipelines import Processor
 
     class SaveToFile(Protocol):
         """TBW."""
 
@@ -363,22 +354,22 @@
             "txt": self.save_to_txt,
             "csv": self.save_to_csv,
             "png": self.save_to_png,
             "jpg": self.save_to_jpg,
             "jpeg": self.save_to_jpeg,
         }
 
-        filenames: List[Path] = []
+        filenames: list[Path] = []
 
         dct: Mapping[ValidName, Sequence[ValidFormat]]
         if self.save_data_to_file:
             for dct in self.save_data_to_file:
                 # TODO: Why looking at first entry ? Check this !
                 # Get first entry of `dict` 'item'
-                first_item: Tuple[ValidName, Sequence[ValidFormat]]
+                first_item: tuple[ValidName, Sequence[ValidFormat]]
                 first_item, *_ = dct.items()
 
                 obj: ValidName
                 format_list: Sequence[ValidFormat]
                 obj, format_list = first_item
 
                 data: np.ndarray = np.array(processor.get(obj))
@@ -421,15 +412,18 @@
                         )
 
                         filenames.append(filename)
 
         return filenames
 
     def save_to_netcdf(
-        self, data: "xr.Dataset", name: str, with_auto_suffix: bool = False
+        self,
+        data: Union["xr.Dataset", "DataTree"],
+        name: str,
+        with_auto_suffix: bool = False,
     ) -> Path:
         """Write Xarray dataset to NetCDF file.
 
         Parameters
         ----------
         data: Dataset
         name: str
@@ -470,15 +464,15 @@
     if "?" in template_str:
         if run_number is not None:
             path_str = template_str.replace("?", "{}")
             output_str = path_str.format(run_number + 1)
         else:
             path_str_for_glob = template_str.replace("?", "*")
             dir_list = glob(path_str_for_glob)
-            num_list: List[int] = sorted(get_number(d) for d in dir_list)
+            num_list: list[int] = sorted(get_number(d) for d in dir_list)
             if num_list:
                 next_num = num_list[-1] + 1
             else:
                 next_num = 1
             path_str = template_str.replace("?", "{}")
             output_str = path_str.format(next_num)
```

### Comparing `pyxel_sim-1.8/pyxel/pipelines/__init__.py` & `pyxel_sim-1.9/pyxel/pipelines/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 
 """The pipeline code for the different detector simulation routines."""
 
 # flake8: noqa
 from .model_function import ModelFunction, Arguments, FitnessFunction
 from .model_group import ModelGroup
 from .pipeline import DetectionPipeline
-from .processor import Processor, ResultType, result_keys
+from .processor import Processor, ResultId, get_result_id, result_keys
```

### Comparing `pyxel_sim-1.8/pyxel/pipelines/model_function.py` & `pyxel_sim-1.9/pyxel/pipelines/model_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 import inspect
 import warnings
-from typing import TYPE_CHECKING, Any, Callable, Dict, MutableMapping, Optional
+from collections.abc import MutableMapping
+from typing import TYPE_CHECKING, Any, Callable, Optional
 
 from pyxel.evaluator import evaluate_reference
 
 if TYPE_CHECKING:
     import numpy as np
 
     from pyxel.calibration import FittingCallable
@@ -50,16 +51,16 @@
     Non existing arguments
     >>> arguments["three"] = 3
     KeyError: 'No argument named three !'
     >>> arguments.three = 3
     AttributeError: 'No argument named three !'
     """
 
-    def __init__(self, input_arguments: Dict[str, Any]):
-        self._arguments: Dict[str, Any] = input_arguments
+    def __init__(self, input_arguments: dict[str, Any]):
+        self._arguments: dict[str, Any] = input_arguments
 
     def __setitem__(self, key, value):
         if key not in self._arguments:
             raise KeyError(f"No argument named {key} !")
 
         self._arguments[key] = value
```

### Comparing `pyxel_sim-1.8/pyxel/pipelines/model_group.py` & `pyxel_sim-1.9/pyxel/pipelines/model_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,17 @@
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 import logging
+from collections.abc import Iterator, Mapping, Sequence
 from copy import deepcopy
-from typing import TYPE_CHECKING, Iterator, List, Mapping, Optional, Sequence
+from typing import TYPE_CHECKING, Optional
 
 from pyxel import util
 from pyxel.pipelines import ModelFunction
 
 if TYPE_CHECKING:
     from pyxel.detectors import Detector
     from pyxel.pipelines import DetectionPipeline
@@ -28,15 +29,15 @@
         self._log = logging.getLogger(__name__)
         self._name = name
         self.models: Sequence[ModelFunction] = models
 
     def __repr__(self):
         cls_name: str = self.__class__.__name__
 
-        all_models: List[str] = [model.name for model in self.models if model.name]
+        all_models: list[str] = [model.name for model in self.models if model.name]
 
         return f"{cls_name}<name={self._name!r}, models={all_models!r}>"
 
     def __deepcopy__(self, memo: dict) -> "ModelGroup":
         copied_models = deepcopy(self.models)
         return ModelGroup(models=copied_models, name=self._name)
```

### Comparing `pyxel_sim-1.8/pyxel/pipelines/pipeline.py` & `pyxel_sim-1.9/pyxel/pipelines/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 
 import warnings
-from typing import Iterable, Optional, Sequence, Tuple
+from collections.abc import Iterable, Sequence
+from typing import Optional
 
 from pyxel.pipelines import ModelFunction, ModelGroup
 
 
 class DetectionPipeline:
     """TBW."""
 
     # Define the order of steps in the pipeline.
-    MODEL_GROUPS: Tuple[str, ...] = (
+    MODEL_GROUPS: tuple[str, ...] = (
         "scene_generation",
         "photon_collection",
         "photon_generation",  # Deprecated. It will be removed in version 2.0
         "optics",  # Deprecated. It will be removed in version 2.0
         "phasing",
         "charge_generation",
         "charge_collection",
@@ -203,15 +204,15 @@
 
     @property
     def data_processing(self) -> Optional[ModelGroup]:
         """Get group 'data processing'."""
         return self._data_processing
 
     @property
-    def model_group_names(self) -> Tuple[str, ...]:
+    def model_group_names(self) -> tuple[str, ...]:
         """TBW."""
         return self.MODEL_GROUPS
 
     @property
     def is_running(self) -> bool:
         """Return the running state of this pipeline."""
         return self._is_running
```

### Comparing `pyxel_sim-1.8/pyxel/pipelines/processor.py` & `pyxel_sim-1.9/pyxel/pipelines/processor.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,27 +4,18 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
 import logging
 import operator
+from collections.abc import Sequence
 from copy import deepcopy
-from enum import Enum
 from numbers import Number
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    Callable,
-    List,
-    Literal,
-    Optional,
-    Sequence,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, Callable, NewType, Optional, Union
 
 import numpy as np
 
 from pyxel import __version__
 from pyxel.evaluator import eval_entry
 from pyxel.pipelines import DetectionPipeline, ModelGroup
 from pyxel.state import get_obj_att
@@ -32,64 +23,77 @@
 
 if TYPE_CHECKING:
     import xarray as xr
 
     from pyxel.detectors import Detector
 
 
-class ResultType(Enum):
-    """Result type class."""
+# class ResultType(Enum):
+#     """Result type class."""
+#
+#     Photon = "photon"
+#     Charge = "charge"
+#     Pixel = "pixel"
+#     Signal = "signal"
+#     Image = "image"
+#     Data = "data"
+#     All = "all"
+
+ResultId = NewType("ResultId", str)
+
+
+def get_result_id(name: str) -> ResultId:
+    """Convert to a 'ResultId' object."""
+    if name not in (
+        "photon",
+        "charge",
+        "pixel",
+        "signal",
+        "image",
+        "all",
+    ) and not name.startswith("data"):
+        raise ValueError(f"Result type: {name!r} unknown !")
 
-    Photon = "photon"
-    Charge = "charge"
-    Pixel = "pixel"
-    Signal = "signal"
-    Image = "image"
-    All = "all"
+    return ResultId(name)
 
 
-def result_keys(
-    result_type: ResultType = ResultType.All,
-) -> Sequence[Literal["photon", "charge", "pixel", "signal", "image"]]:
+def result_keys(result_type: ResultId) -> Sequence[ResultId]:
     """Return result keys based on result type.
 
     Parameters
     ----------
     result_type
 
     Returns
     -------
     list
     """
-    if result_type == ResultType.Photon:
-        return ["photon"]
-    elif result_type == ResultType.Charge:
-        return ["charge"]
-    elif result_type == ResultType.Pixel:
-        return ["pixel"]
-    elif result_type == ResultType.Signal:
-        return ["signal"]
-    elif result_type == ResultType.Image:
-        return ["image"]
-    elif result_type == ResultType.All:
-        return ["photon", "charge", "pixel", "signal", "image"]
+    if result_type == "all":
+        return [
+            ResultId("photon"),
+            ResultId("charge"),
+            ResultId("pixel"),
+            ResultId("signal"),
+            ResultId("image"),
+            ResultId("data"),
+        ]
     else:
-        raise ValueError("Result type unknown.")
+        return [ResultId(result_type)]
 
 
 # TODO: Is this class needed ?
 class Processor:
     """TBW."""
 
     def __init__(self, detector: "Detector", pipeline: DetectionPipeline):
         self._log = logging.getLogger(__name__)
 
         self.detector = detector
         self.pipeline = pipeline
-        self._result: Optional[dict] = None
+        self._result: Optional[dict] = None  # TODO: Deprecate this variable ?
 
         self._numbytes = 0
 
     def __repr__(self) -> str:
         cls_name: str = self.__class__.__name__
         return f"{cls_name}<detector={self.detector!r}, pipeline={self.pipeline!r}>"
 
@@ -135,41 +139,41 @@
         """
         func: Callable = operator.attrgetter(key)
         result = func(self)
 
         return result
 
     # TODO: Could it be renamed '__setitem__' ?
-    def set(
+    def set(  # noqa: A003
         self,
         key: str,
-        value: Union[str, Number, np.ndarray, List[Union[str, Number, np.ndarray]]],
+        value: Union[str, Number, np.ndarray, list[Union[str, Number, np.ndarray]]],
         convert_value: bool = True,
     ) -> None:
         """TBW.
 
         Parameters
         ----------
         key : str
         value
         convert_value : bool
         """
         if convert_value:  # and value:
             # TODO: Refactor this
             # convert the string based value to a number
             if isinstance(value, list):
-                new_value_lst: List[Union[str, Number, np.ndarray]] = []
+                new_value_lst: list[Union[str, Number, np.ndarray]] = []
 
                 val: Union[str, Number, np.ndarray]
                 for val in value:
                     new_val = eval_entry(val) if val else val
                     new_value_lst.append(new_val)
 
                 new_value: Union[
-                    str, Number, np.ndarray, List[Union[str, Number, np.ndarray]]
+                    str, Number, np.ndarray, list[Union[str, Number, np.ndarray]]
                 ] = new_value_lst
 
             else:
                 converted_value: Union[str, Number, np.ndarray] = eval_entry(value)
 
                 new_value = converted_value
         else:
@@ -221,50 +225,56 @@
                     break
 
         self.pipeline._is_running = False
 
         # TODO: Is is necessary to return 'self' ??
         return self
 
-    # TODO: Refactor '.result'. See #524
+    # TODO: Refactor '.result'. See #524. Deprecate this method ?
     @property
     def result(self) -> dict:
         """Return exposure pipeline final result in a dictionary."""
         if not self._result:
             raise ValueError("No result saved in the processor.")
         return self._result
 
-    # TODO: Refactor '.result'. See #524
+    # TODO: Refactor '.result'. See #524. Deprecate this method ?
     @result.setter
     def result(self, result_to_save: dict) -> None:
         """Set result."""
         self._result = result_to_save
 
     # TODO: Refactor '.result'. See #524
     def result_to_dataset(
-        self, y: range, x: range, times: np.ndarray, result_type: ResultType
+        self,
+        y: range,
+        x: range,
+        times: np.ndarray,
+        result_type: ResultId,
     ) -> "xr.Dataset":
         """Return the result in a xarray dataset."""
         # Late import to speedup start-up time
         import xarray as xr
 
         if not self._result:
             raise ValueError("No result saved in the processor.")
 
         readout_time = xr.DataArray(
             times,
             dims=("readout_time",),
             attrs={"units": "s", "standard_name": "Readout time"},
         )
 
-        lst: List[xr.DataArray] = []
+        lst: list[xr.DataArray] = []
 
-        key: Literal["photon", "charge", "pixel", "signal", "image"]
+        key: ResultId
         for key in result_keys(result_type):
-            if key == "photon":
+            if key.startswith("data"):
+                continue
+            elif key == "photon":
                 standard_name = "Photon"
                 unit = "photon"
             elif key == "charge":
                 standard_name = "Charge"
                 unit = "electron"
             elif key == "pixel":
                 standard_name = "Pixel"
@@ -273,16 +283,16 @@
                 standard_name = "Signal"
                 unit = "volt"
             elif key == "image":
                 standard_name = "Image"
                 unit = "adu"
             else:
                 raise NotImplementedError
-                standard_name = key
-                unit = ""
+                # standard_name = key
+                # unit = ""
 
             da = xr.DataArray(
                 self.result[key],
                 dims=("readout_time", "y", "x"),
                 name=key,
                 coords={"readout_time": readout_time, "y": y, "x": x},
                 attrs={"units": unit, "standard_name": standard_name},
```

### Comparing `pyxel_sim-1.8/pyxel/run.py` & `pyxel_sim-1.9/pyxel/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,16 +5,17 @@
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """CLI to run Pyxel."""
 import logging
 import sys
 import time
+from collections.abc import Sequence
 from pathlib import Path
-from typing import TYPE_CHECKING, Optional, Sequence, Tuple, Union
+from typing import TYPE_CHECKING, Optional, Union
 
 import click
 import dask
 import pandas as pd
 
 from pyxel import Configuration
 from pyxel import __version__ as version
@@ -23,14 +24,15 @@
 from pyxel.exposure import Exposure
 from pyxel.observation import Observation, ObservationResult
 from pyxel.pipelines import DetectionPipeline, Processor
 from pyxel.util import create_model, download_examples
 
 if TYPE_CHECKING:
     import xarray as xr
+    from datatree import DataTree
 
     from pyxel.calibration import Calibration
     from pyxel.outputs import CalibrationOutputs, ExposureOutputs, ObservationOutputs
 
 
 # TODO: This function will be deprecated (see #563)
 def exposure_mode(
@@ -93,14 +95,78 @@
 
     if exposure_outputs.save_exposure_data:
         exposure_outputs.save_exposure_outputs(dataset=result)
 
     return result
 
 
+def _run_exposure_mode(
+    exposure: "Exposure",
+    detector: Detector,
+    pipeline: "DetectionPipeline",
+) -> "DataTree":
+    """Run an 'exposure' pipeline.
+
+    For more information, see :ref:`exposure_mode`.
+
+    Parameters
+    ----------
+    exposure: Exposure
+    detector: Detector
+    pipeline: DetectionPipeline
+
+    Returns
+    -------
+    Dataset
+        An multi-dimensional array database from `xarray <https://xarray.pydata.org>`_.
+
+    Examples
+    --------
+    Load a configuration file
+
+    >>> import pyxel
+    >>> config = pyxel.load("configuration.yaml")
+    >>> config
+    Configuration(...)
+
+    Run an exposure pipeline
+
+    >>> dataset = pyxel.exposure_mode(
+    ...     exposure=config.exposure,
+    ...     detector=config.detector,
+    ...     pipeline=config.pipeline,
+    ... )
+    >>> dataset
+    <xarray.Dataset>
+    Dimensions:       (readout_time: 1, y: 450, x: 450)
+    Coordinates:
+      * readout_time  (readout_time) int64 1
+      * y             (y) int64 0 1 2 3 4 5 6 7 ... 442 443 444 445 446 447 448 449
+      * x             (x) int64 0 1 2 3 4 5 6 7 ... 442 443 444 445 446 447 448 449
+    Data variables:
+        image         (readout_time, y, x) uint16 9475 9089 8912 ... 9226 9584 10079
+        signal        (readout_time, y, x) float64 3.159 3.03 2.971 ... 3.195 3.36
+        pixel         (readout_time, y, x) float64 1.053e+03 1.01e+03 ... 1.12e+03
+    """
+
+    logging.info("Mode: Exposure")
+
+    exposure_outputs: ExposureOutputs = exposure.outputs
+    detector.set_output_dir(exposure_outputs.output_dir)  # TODO: Remove this
+
+    processor = Processor(detector=detector, pipeline=pipeline)
+
+    result: DataTree = exposure.run_exposure_new(processor=processor)
+
+    if exposure_outputs.save_exposure_data:
+        exposure_outputs.save_exposure_outputs(dataset=result)
+
+    return result
+
+
 # TODO: This function will be deprecated (see #563)
 def observation_mode(
     observation: "Observation",
     detector: Detector,
     pipeline: "DetectionPipeline",
 ) -> "ObservationResult":
     """Run an 'observation' pipeline.
@@ -159,15 +225,15 @@
 
 # TODO: This function will be deprecated (see #563)
 def calibration_mode(
     calibration: "Calibration",
     detector: Detector,
     pipeline: "DetectionPipeline",
     compute_and_save: bool = True,
-) -> Tuple["xr.Dataset", pd.DataFrame, pd.DataFrame, Sequence]:
+) -> tuple["xr.Dataset", pd.DataFrame, pd.DataFrame, Sequence]:
     """Run a 'calibration' pipeline.
 
     For more information, see :ref:`calibration_mode`.
 
     Parameters
     ----------
     calibration: Calibration
@@ -217,15 +283,15 @@
         target               (id_processor, y, x) >f8 4.834e+03 ... 4.865e+03
     Attributes:
         num_islands:      2
         population_size:  20
         num_evolutions:   2
         generations:      5
         topology:         unconnected
-        result_type:      ResultType.Image
+        result_type:      image
 
     >>> processors
            island  id_processor                                          processor
     0       0             0  Delayed('apply_parameters-c5da1649-766f-4ecb-a...
     1       1             0  Delayed('apply_parameters-c16f998f-f52f-4beb-b...
 
     >>> logs
@@ -270,15 +336,15 @@
     # geometry = processor.detector.geometry
     # calibration.post_processing(
     #     champions=champions,
     #     output=calibration_outputs,
     #     row=geometry.row,
     #     col=geometry.col,
     # )
-    filenames = calibration.post_processing(
+    filenames = calibration._post_processing(
         ds=ds_results, df_processors=df_processors, output=calibration_outputs
     )
 
     if compute_and_save:
         computed_ds, df_processors, df_logs, filenames = dask.compute(
             ds_results, df_processors, df_all_logs, filenames
         )
@@ -307,73 +373,72 @@
     return result
 
 
 def _run_calibration_mode(
     calibration: "Calibration",
     detector: Detector,
     pipeline: "DetectionPipeline",
-) -> "xr.Dataset":
+) -> "DataTree":
     logging.info("Mode: Calibration")
 
     calibration_outputs: CalibrationOutputs = calibration.outputs
     detector.set_output_dir(calibration_outputs.output_dir)  # TODO: Remove this
 
     processor = Processor(detector=detector, pipeline=pipeline)
 
-    ds = calibration.run_calibration_new(
+    data_tree = calibration.run_calibration_new(
         processor=processor,
         output_dir=calibration_outputs.output_dir,
     )
 
-    return ds
+    return data_tree
 
 
 def _run_observation_mode(
     observation: Observation,
     detector: Detector,
     pipeline: DetectionPipeline,
-) -> "xr.Dataset":
+) -> "DataTree":
     logging.info("Mode: Observation")
 
     observation_outputs: ObservationOutputs = observation.outputs
     detector.set_output_dir(observation_outputs.output_dir)  # TODO: Remove this
 
     processor = Processor(detector=detector, pipeline=pipeline)
 
-    ds = observation.run_observation_new(processor=processor)
+    result = observation.run_observation_datatree(processor=processor)
 
     if observation_outputs.save_observation_data:
         raise NotImplementedError
     #     observation_outputs.save_observation_datasets(
     #         result=result, mode=observation.parameter_mode
     #     )
 
-    return ds
+    return result
 
 
 def run_mode(
     mode: Union[Exposure, Observation, "Calibration"],
     detector: Detector,
     pipeline: DetectionPipeline,
-) -> "xr.Dataset":
+) -> "DataTree":
     """Run a pipeline.
 
     Parameters
     ----------
     mode : Exposure, Observation or Calibration
         Mode to execute.
     detector : Detector
         This object is the container for all the data used for the models.
     pipeline : DetectionPipeline
         This is the core algorithm of Pyxel. This pipeline contains all the models to run.
 
     Returns
     -------
-    Dataset
-        Multi-dimensional result.
+    DataTree
 
     Raises
     ------
     TypeError
         Raised if the ``mode`` is not valid.
 
     Examples
@@ -388,48 +453,74 @@
 
     >>> data = pyxel.run_mode(
     ...     mode=config.exposure,
     ...     detector=config.detector,
     ...     pipeline=config.pipeline,
     ... )
     >>> data
-    <xarray.Dataset>
-    Dimensions:       (readout_time: 1, y: 450, x: 450)
-    Coordinates:
-      * readout_time  (readout_time) int64 1
-      * y             (y) int64 0 1 2 3 4 5 6 7 ... 442 443 444 445 446 447 448 449
-      * x             (x) int64 0 1 2 3 4 5 6 7 ... 442 443 444 445 446 447 448 449
-    Data variables:
-        image         (readout_time, y, x) uint16 9475 9089 8912 ... 9226 9584 10079
-        signal        (readout_time, y, x) float64 3.159 3.03 2.971 ... 3.195 3.36
-        pixel         (readout_time, y, x) float64 1.053e+03 1.01e+03 ... 1.12e+03
+    DataTree('None', parent=None)
+    │   Dimensions:            (period: 5, angle: 3, trap_densities_id: 7, dim_0: 2)
+    │   Coordinates:
+    │     * period             (period) int64 4 8 12 16 20
+    │     * angle              (angle) int64 0 10 20
+    │     * trap_densities_id  (trap_densities_id) int64 0 1 2 3 4 5 6
+    │       trap_densities     (trap_densities_id, dim_0) float64 nan nan ... 70.0 80.0
+    │   Dimensions without coordinates: dim_0
+    │   Data variables:
+    │       *empty*
+    │   Attributes:
+    │       pyxel version:  1.8+141.gb470c395
+    │       running mode:   Observation - Product
+    ├── DataTree('bucket')
+    │       Dimensions:            (trap_densities_id: 7, angle: 3, period: 5, time: 1,
+    │                               y: 100, x: 100, dim_0: 2)
+    │       Coordinates:
+    │         * time               (time) float64 1.0
+    │         * y                  (y) int64 0 1 2 3 4 5 6 7 8 ... 92 93 94 95 96 97 98 99
+    │         * x                  (x) int64 0 1 2 3 4 5 6 7 8 ... 92 93 94 95 96 97 98 99
+    │         * period             (period) int64 4 8 12 16 20
+    │         * angle              (angle) int64 0 10 20
+    │         * trap_densities_id  (trap_densities_id) int64 0 1 2 3 4 5 6
+    │           trap_densities     (trap_densities_id, dim_0) float64 nan nan ... 70.0 80.0
+    │       Dimensions without coordinates: dim_0
+    │       Data variables:
+    │           photon             (trap_densities_id, angle, period, time, y, x) float64 ...
+    │           charge             (trap_densities_id, angle, period, time, y, x) float64 ...
+    │           pixel              (trap_densities_id, angle, period, time, y, x) float64 ...
+    │           signal             (trap_densities_id, angle, period, time, y, x) float64 ...
+    │           image              (trap_densities_id, angle, period, time, y, x) float64 ...
+    └── DataTree('data')
     """
     from pyxel.calibration import Calibration
 
     if isinstance(mode, Exposure):
-        ds = exposure_mode(exposure=mode, detector=detector, pipeline=pipeline)
+        data_tree = _run_exposure_mode(
+            exposure=mode,
+            detector=detector,
+            pipeline=pipeline,
+        )
 
     elif isinstance(mode, Observation):
-        ds = _run_observation_mode(
+        data_tree = _run_observation_mode(
             observation=mode,
             detector=detector,
             pipeline=pipeline,
         )
 
     elif isinstance(mode, Calibration):
-        ds = _run_calibration_mode(
+        data_tree = _run_calibration_mode(
             calibration=mode,
             detector=detector,
             pipeline=pipeline,
         )
 
     else:
         raise TypeError("Please provide a valid simulation mode !")
 
-    return ds
+    return data_tree
 
 
 def output_directory(configuration: Configuration) -> Path:
     """Return the output directory from the configuration.
 
     Parameters
     ----------
```

### Comparing `pyxel_sim-1.8/pyxel/show_versions.py` & `pyxel_sim-1.9/pyxel/show_versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 """Subpackage used to display the versions of all dependencies."""
 import importlib
 import locale
 import os
 import platform
 import struct
 import sys
-from typing import Any, Dict, Mapping, Optional, Tuple
+from collections.abc import Mapping
+from typing import Any, Optional
 
 from ._version import get_versions
 
 __all__ = ["show_versions"]
 
 
 def get_system_info() -> Mapping[str, Any]:
@@ -89,18 +90,20 @@
     isort      : 5.5.2
     mypy       : installed
     pytest     : 6.0.1
     sphinx     : None
     """
     system_info: Mapping[str, Any] = get_system_info()
 
-    dependencies_lst: Tuple[str, ...] = (
+    dependencies_lst: tuple[str, ...] = (
         "pyxel",
         # required
         "astropy",
+        "asdf",
+        "attrs",
         "bokeh",
         "cloudpickle",
         "dask",
         "dask_jobqueue",
         "distributed",
         "fsspec",
         "h5py",
@@ -115,19 +118,21 @@
         "pandas",
         "PIL",
         "poppy",
         "pygmo",
         "pympler",
         "scipy",
         "seaborn",
+        "sep",
         "skimage",
         "tqdm",
         "typing-extensions",
         "yaml",
         "xarray",
+        "datatree",
         "xlrd",
         "openpyxl",
         "netcdf4",
         # Install / build
         "setuptools",
         "pip",
         "conda",
@@ -139,15 +144,15 @@
         "mypy",
         "pytest",
         "tox",
         # Docs
         "sphinx",
     )
 
-    dependencies: Dict[str, Optional[str]] = {}
+    dependencies: dict[str, Optional[str]] = {}
 
     for module_name in dependencies_lst:
         try:
             # Try to get a module
             module = importlib.import_module(module_name)
         except Exception:
             dependencies[module_name] = None
```

### Comparing `pyxel_sim-1.8/pyxel/state.py` & `pyxel_sim-1.9/pyxel/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 """TBW."""
-from typing import Any, Dict, Mapping, Optional, Sequence, Tuple, Type
+from collections.abc import Mapping, Sequence
+from typing import Any, Optional
 
 __all__ = ["get_obj_att", "get_obj_by_type", "get_value", "get_state_ids", "copy_state"]
 
 
 # TODO: Remove this function ? See issue #230.
-def get_obj_by_type(obj: Any, key: str, obj_type: Optional[Type] = None) -> Any:
+def get_obj_by_type(obj: Any, key: str, obj_type: Optional[type] = None) -> Any:
     """Get the object associated with the class type following the key chain.
 
     :param obj:
     :param key:
     :param obj_type:
     :return:
     """
     obj, att = get_obj_att(obj, key, obj_type)
     if obj_type is not None:
         if isinstance(obj, obj_type):
             return obj
 
 
 # TODO: Remove this function ? See issue #230.
-def get_obj_att(obj: Any, key: str, obj_type: Optional[Type] = None) -> Tuple[Any, str]:
+def get_obj_att(obj: Any, key: str, obj_type: Optional[type] = None) -> tuple[Any, str]:
     """Get the object associated with the key.
 
     Example::
 
         >>> obj = {"processor": {"pipeline": {"models": [1, 2, 3]}}}
         >>> om.get_obj_att(obj, "processor.pipeline.models")
         ({'models': [1, 2, 3]}, 'models')
@@ -103,15 +104,15 @@
     return result
 
 
 # TODO: Remove this function ? See issue #230.
 def get_state_ids(
     obj: Any,
     parent_key_list: Optional[Sequence[str]] = None,
-    result: Optional[Dict[str, Any]] = None,
+    result: Optional[dict[str, Any]] = None,
 ) -> Any:
     """Retrieve a flat dictionary of the object attribute hierarchy.
 
     The dot-format is used as the key representation.
 
     :param obj:
     :param parent_key_list:
@@ -128,25 +129,25 @@
 
     if isinstance(obj, dict):
         for key, value in obj.items():
             if isinstance(value, (str, int, float)):
                 key = ".".join(parent_key_list) + "." + key
                 result[key] = value
             else:
-                list(parent_key_list) + [key]
-                get_state_ids(value, list(parent_key_list) + [key], result)
+                _ = [*parent_key_list, key]  # TODO: Is it used ??
+                get_state_ids(value, [*parent_key_list, key], result)
 
     elif isinstance(obj, list):
         is_primitive = all([isinstance(value, (str, int, float)) for value in obj])
         if is_primitive:
             key = ".".join(parent_key_list)
             result[key] = obj
         else:
             for i, value in enumerate(obj):
-                get_state_ids(value, list(parent_key_list) + [str(i)], result)
+                get_state_ids(value, [*parent_key_list, str(i)], result)
     return result
 
 
 # TODO: Remove this function ? See issue #230.
 def get_value(obj: Any, key: str) -> Any:
     """Retrieve the attribute value of the object given the attribute dot formatted key chain.
```

### Comparing `pyxel_sim-1.8/pyxel/templates/_TEMPLATE.py` & `pyxel_sim-1.9/pyxel/templates/_TEMPLATE.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
 
    Write the documentation for _TEMPLATE
 
 """
 
 
 # One or the other
-from pyxel.detectors import CCD, CMOS
+from pyxel.detectors import CCD
 
 
 def model(detector: CCD, arg1: str, arg2: bool = True, arg3: int = 42) -> None:
     """Do nothing.
 
     Parameters
     ----------
```

### Comparing `pyxel_sim-1.8/pyxel/util/__init__.py` & `pyxel_sim-1.9/pyxel/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/util/add_model.py` & `pyxel_sim-1.9/pyxel/util/add_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 import logging
 import os
 import shutil
 import sys
 import time
 from pathlib import Path
-from typing import Tuple
 
 
 def create_model(newmodel: str) -> None:
     """Create a new module using pyxel/templates/MODELTEMPLATE.py.
 
     Parameters
     ----------
@@ -90,15 +89,15 @@
         raise
     # Any error saying that the directory doesn't exist
     except OSError as e:
         logging.critical(model_name + " not created. Error: %s" % e)
         raise
 
 
-def get_name_and_location(newmodel: str) -> Tuple[str, str]:
+def get_name_and_location(newmodel: str) -> tuple[str, str]:
     """Get name and location of new model from string modeltype/modelname.
 
     Parameters
     ----------
     newmodel: str
 
     Returns
```

### Comparing `pyxel_sim-1.8/pyxel/util/examples.py` & `pyxel_sim-1.9/pyxel/util/examples.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/util/image.py` & `pyxel_sim-1.9/pyxel/util/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 """Utility functions for images."""
 
 from enum import Enum
 from functools import lru_cache
 from pathlib import Path
-from typing import Literal, Optional, Tuple, Union
+from typing import Literal, Optional, Union
 
 import numpy as np
 
 from pyxel.inputs import load_image
 
 
 class Alignment(Enum):
@@ -30,15 +30,15 @@
 
 def _set_relative_position(
     array_x: int,
     array_y: int,
     output_x: int,
     output_y: int,
     alignment: Alignment,
-) -> Tuple[int, int]:
+) -> tuple[int, int]:
     """Calculate relative position of (0, 0) pixels for two different array shapes based on desired alignment.
 
     Parameters
     ----------
     output_y: int
     output_x: int
     array_y: int
@@ -61,16 +61,16 @@
         return output_y - array_y, output_x - array_x
     else:
         raise NotImplementedError
 
 
 def fit_into_array(
     array: np.ndarray,
-    output_shape: Tuple[int, ...],
-    relative_position: Tuple[int, int] = (0, 0),
+    output_shape: tuple[int, ...],
+    relative_position: tuple[int, int] = (0, 0),
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ] = None,
     allow_smaller_array: bool = True,
 ) -> np.ndarray:
     """Fit input array into an output array of specified output shape.
 
@@ -147,15 +147,15 @@
     ] = cropped_array
 
     return output
 
 
 @lru_cache(maxsize=128)  # One must add parameter 'maxsize' for Python 3.7
 def load_cropped_and_aligned_image(
-    shape: Tuple[int, ...],
+    shape: tuple[int, ...],
     filename: Union[str, Path],
     position_x: int = 0,
     position_y: int = 0,
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ] = None,
     allow_smaller_array: bool = True,
```

### Comparing `pyxel_sim-1.8/pyxel/util/materials.py` & `pyxel_sim-1.9/pyxel/util/materials.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/util/memory.py` & `pyxel_sim-1.9/pyxel/util/memory.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 
 """Object memory consumption utilities."""
 
-from typing import Any, List
+from typing import Any
 
 import numpy as np
 from pympler.asizeof import asizeof
 
 
 def get_size(obj: Any) -> int:
     """Recursively calculates object size in bytes using Pympler library.
@@ -47,15 +47,15 @@
                 print(f"{k:<20}{np.round(v,decimals=1):<7}{unit}")
                 break
             v /= 1024.0
 
 
 def memory_usage_details(
     obj: Any,
-    *attr_kw: List[str],
+    *attr_kw: list[str],
     print_result: bool = True,
     human_readable: bool = True,
 ) -> dict:
     """TBW.
 
     Parameters
     ----------
```

### Comparing `pyxel_sim-1.8/pyxel/util/random.py` & `pyxel_sim-1.9/pyxel/util/random.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel/util/timing.py` & `pyxel_sim-1.9/pyxel/util/timing.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/pyxel_sim.egg-info/PKG-INFO` & `pyxel_sim-1.9/pyxel_sim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxel-sim
-Version: 1.8
+Version: 1.9
 Summary: Pyxel detector simulation framework.
 Author-email: The Pyxel development team <pyxel@esa.int>
 License: MIT
 Project-URL: homepage, https://esa.gitlab.io/pyxel/
 Project-URL: documentation, https://esa.gitlab.io/pyxel/doc/
 Project-URL: repository, https://gitlab.com/esa/pyxel
 Project-URL: changelog, https://gitlab.com/esa/pyxel/-/releases
@@ -13,22 +13,22 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: calibration
 Provides-Extra: model
 Provides-Extra: io
 Provides-Extra: all
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
@@ -53,15 +53,15 @@
 ## What is it?
 
 *Pyxel* is a general detector simulation framework.
 An easy-to-use framework that can simulate a variety of imaging detector
 effects combined on images (e.g. radiation and optical effects, noises)
 made by CCD or CMOS-based detectors.
 
-*Pyxel* is tested on Python 3.8+.
+*Pyxel* is tested on Python 3.9+.
 
 If you'd like to contribute to *Pyxel* you're most welcome.
 Please read [the little guide](https://esa.gitlab.io/pyxel/doc/stable/references/contributing.html) to get you started.
 
 ## Documentation
 
 Learn more about *Pyxel* in its offical [blog](https://esa.gitlab.io/pyxel) and its official documentation at [https://esa.gitlab.io/pyxel/doc](https://esa.gitlab.io/pyxel/doc).
```

### Comparing `pyxel_sim-1.8/pyxel_sim.egg-info/SOURCES.txt` & `pyxel_sim-1.9/pyxel_sim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 AUTHORS.rst
 LICENSE.txt
 MANIFEST.in
 README.md
 pyproject.toml
 setup.py
 continuous_integration/scripts/auto_generated.py
-continuous_integration/scripts/copy_auto_generated.py
+continuous_integration/scripts/before_auto_generated.py
 continuous_integration/scripts/create_json_schema.py
 continuous_integration/scripts/download_last_environment_artifact.py
+continuous_integration/scripts/dummy.py
 docs/html/_static/dummy.py
-docs/jupyter_execute/howto/detector_import_export.py
 docs/source/conf.py
 docs/source/_static/dummy.py
 pyxel/__init__.py
 pyxel/__main__.py
 pyxel/_version.py
 pyxel/evaluator.py
 pyxel/options.py
@@ -22,17 +22,19 @@
 pyxel/state.py
 pyxel/backends/__init__.py
 pyxel/backends/asdf.py
 pyxel/backends/hdf5.py
 pyxel/calibration/__init__.py
 pyxel/calibration/algorithm.py
 pyxel/calibration/archipelago.py
+pyxel/calibration/archipelago_datatree.py
 pyxel/calibration/calibration.py
 pyxel/calibration/fitness.py
 pyxel/calibration/fitting.py
+pyxel/calibration/fitting_datatree.py
 pyxel/calibration/protocols.py
 pyxel/calibration/user_defined.py
 pyxel/calibration/util.py
 pyxel/configuration/__init__.py
 pyxel/configuration/configuration.py
 pyxel/data_structure/__init__.py
 pyxel/data_structure/array.py
@@ -115,14 +117,16 @@
 pyxel/models/charge_measurement/nghxrg/nghxrg_beta.py
 pyxel/models/charge_transfer/EMCCD_poisson.py
 pyxel/models/charge_transfer/__init__.py
 pyxel/models/charge_transfer/cdm.py
 pyxel/models/charge_transfer/arctic_cti/__init__.py
 pyxel/models/charge_transfer/arctic_cti/models_arctic_vanilla.py
 pyxel/models/data_processing/__init__.py
+pyxel/models/data_processing/linear_regression.py
+pyxel/models/data_processing/mean_variance.py
 pyxel/models/data_processing/source_extractor.py
 pyxel/models/data_processing/statistics.py
 pyxel/models/optics/__init__.py
 pyxel/models/optics/point_spread_function.py
 pyxel/models/optics/poppy.py
 pyxel/models/phasing/__init__.py
 pyxel/models/phasing/pulse_processing.py
@@ -182,14 +186,15 @@
 pyxel_sim.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_evaluator.py
 tests/test_options.py
 tests/test_show_versions.py
 tests/calibration/test_check_ranges.py
+tests/calibration/test_fitness.py
 tests/calibration/test_slice_to_range.py
 tests/configuration/test_load.py
 tests/configuration/test_schema.py
 tests/data_structure/test_charge.py
 tests/data_structure/test_processed_data.py
 tests/detectors/test_ccd.py
 tests/detectors/test_ccd_characteristics.py
@@ -201,14 +206,15 @@
 tests/detectors/test_environment.py
 tests/detectors/test_geometry.py
 tests/detectors/test_mkid.py
 tests/detectors/test_mkid_characteristics.py
 tests/detectors/test_mkid_geometry.py
 tests/exposure/test_readout.py
 tests/functional_tests/__init__.py
+tests/functional_tests/test_basic_exposure.py
 tests/functional_tests/test_parametric.py
 tests/functional_tests/test_yaml.py
 tests/inputs/test_image.py
 tests/model_tests/amplifier_crosstalk/test_crosstalk.py
 tests/models/test_save_load_detector.py
 tests/models/charge_collection/test_fixed_pattern_noise.py
 tests/models/charge_collection/test_persistence.py
```

### Comparing `pyxel_sim-1.8/tests/calibration/test_check_ranges.py` & `pyxel_sim-1.9/tests/calibration/test_check_ranges.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/calibration/test_slice_to_range.py` & `pyxel_sim-1.9/tests/calibration/test_slice_to_range.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/configuration/test_load.py` & `pyxel_sim-1.9/tests/configuration/test_load.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/configuration/test_schema.py` & `pyxel_sim-1.9/tests/configuration/test_schema.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/conftest.py` & `pyxel_sim-1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/data_structure/test_charge.py` & `pyxel_sim-1.9/tests/data_structure/test_charge.py`

 * *Files 21% similar despite different names*

```diff
@@ -84,14 +84,20 @@
             "position_z": np.array([3.3]),
             "velocity_ver": np.array([4.4]),
             "velocity_hor": np.array([-5.5]),
             "velocity_z": np.array([6.6]),
         }
     )
 
+    # ensure that the integer types are consistent
+    exp_df_charges["charge"] = exp_df_charges["charge"].astype(np.int64)
+    exp_df_charges["number"] = exp_df_charges["number"].astype(np.int64)
+    charge.frame["charge"] = charge.frame["charge"].astype(np.int64)
+    charge.frame["number"] = charge.frame["number"].astype(np.int64)
+
     assert charge.nextid == 1
     pd.testing.assert_frame_equal(charge.frame, exp_df_charges)
 
 
 def test_add_one_hole(geo: Geometry):
     """Test with one hole."""
     charge = Charge(geo=geo)
@@ -122,14 +128,20 @@
             "position_z": [3.3],
             "velocity_ver": [4.4],
             "velocity_hor": [-5.5],
             "velocity_z": [6.6],
         }
     )
 
+    # ensure that the integer types are consistent
+    exp_df_charges["charge"] = exp_df_charges["charge"].astype(np.int64)
+    exp_df_charges["number"] = exp_df_charges["number"].astype(np.int64)
+    charge.frame["charge"] = charge.frame["charge"].astype(np.int64)
+    charge.frame["number"] = charge.frame["number"].astype(np.int64)
+
     assert charge.nextid == 1
     pd.testing.assert_frame_equal(charge.frame, exp_df_charges)
 
 
 @dataclass
 class ChargeInfo:
     """Define one charge.
@@ -280,14 +292,20 @@
             "position_z": [3.31, 3.32],
             "velocity_ver": [4.41, 4.42],
             "velocity_hor": [-5.51, 5.52],
             "velocity_z": [6.61, 6.62],
         }
     )
 
+    # ensure that the integer types are consistent
+    exp_df_charges["charge"] = exp_df_charges["charge"].astype(np.int64)
+    exp_df_charges["number"] = exp_df_charges["number"].astype(np.int64)
+    charge.frame["charge"] = charge.frame["charge"].astype(np.int64)
+    charge.frame["number"] = charge.frame["number"].astype(np.int64)
+
     assert charge.nextid == 2
     pd.testing.assert_frame_equal(charge.frame, exp_df_charges)
 
 
 def test_add_two_charges_one_hole(geo: Geometry):
     """Test when adding two charges and then one hole."""
     charge = Charge(geo=geo)
@@ -332,14 +350,20 @@
             "position_z": [3.31, 3.32, 3.33],
             "velocity_ver": [4.41, 4.42, 4.43],
             "velocity_hor": [-5.51, 5.52, 5.53],
             "velocity_z": [6.61, 6.62, 6.63],
         }
     )
 
+    # ensure that the integer types are consistent
+    exp_df_charges["charge"] = exp_df_charges["charge"].astype(np.int64)
+    exp_df_charges["number"] = exp_df_charges["number"].astype(np.int64)
+    charge.frame["charge"] = charge.frame["charge"].astype(np.int64)
+    charge.frame["number"] = charge.frame["number"].astype(np.int64)
+
     assert charge.nextid == 3
     pd.testing.assert_frame_equal(charge.frame, exp_df_charges)
 
 
 def test_invalid_add_charge_dataframe(geo: Geometry):
     """Test method `Charge.add_charge_dataframe` with an invalid input."""
     charge = Charge(geo=geo)
```

### Comparing `pyxel_sim-1.8/tests/data_structure/test_processed_data.py` & `pyxel_sim-1.9/tests/data_structure/test_processed_data.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/detectors/test_ccd.py` & `pyxel_sim-1.9/tests/detectors/test_ccd.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,24 @@
     assert dct["version"] == other_dct["version"]
     assert dct["type"] == other_dct["type"]
     assert dct["properties"] == other_dct["properties"]
 
     assert (
         set(dct["data"])
         == set(other_dct["data"])
-        == {"photon", "scene", "pixel", "signal", "image", "charge", "processed_data"}
+        == {
+            "photon",
+            "scene",
+            "pixel",
+            "signal",
+            "image",
+            "charge",
+            "processed_data",
+            "data",
+        }
     )
     np.testing.assert_equal(dct["data"]["photon"], other_dct["data"]["photon"])
     np.testing.assert_equal(dct["data"]["pixel"], other_dct["data"]["pixel"])
     np.testing.assert_equal(dct["data"]["signal"], other_dct["data"]["signal"])
     np.testing.assert_equal(dct["data"]["image"], other_dct["data"]["image"])
 
     assert (
@@ -230,14 +239,15 @@
                     },
                     "processed_data": {
                         "coords": {},
                         "attrs": {},
                         "dims": {},
                         "data_vars": {},
                     },
+                    "data": {},
                 },
             },
             id="Default parameters",
         ),
         pytest.param(
             CCD(
                 geometry=CCDGeometry(
@@ -307,14 +317,15 @@
                     },
                     "processed_data": {
                         "coords": {},
                         "attrs": {},
                         "dims": {},
                         "data_vars": {},
                     },
+                    "data": {},
                 },
             },
             id="CCD fully defined",
         ),
     ],
 )
 def test_to_and_from_dict(klass, obj, exp_dict):
@@ -404,14 +415,15 @@
                         "velocity_hor",
                         "velocity_z",
                     ],
                     dtype=float,
                 ),
             },
             "processed_data": {"coords": {}, "attrs": {}, "dims": {}, "data_vars": {}},
+            "data": {},
         },
     }
 
     comparison(dct, exp_dict)
 
     # Copy 'exp_dict'
     copied_dct = deepcopy(exp_dict)  # create a new dict
```

### Comparing `pyxel_sim-1.8/tests/detectors/test_ccd_characteristics.py` & `pyxel_sim-1.9/tests/detectors/test_ccd_characteristics.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/detectors/test_ccd_geometry.py` & `pyxel_sim-1.9/tests/detectors/test_ccd_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/detectors/test_cmos.py` & `pyxel_sim-1.9/tests/detectors/test_cmos.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,27 +140,36 @@
 def comparison(dct, other_dct):
     assert set(dct) == set(other_dct) == {"version", "type", "data", "properties"}
     assert dct["version"] == other_dct["version"]
     assert dct["type"] == other_dct["type"]
     assert dct["properties"] == other_dct["properties"]
 
     assert (
-        set(dct["data"])
-        == set(other_dct["data"])
-        == {"photon", "scene", "pixel", "signal", "image", "charge", "processed_data"}
+        sorted(dct["data"])
+        == sorted(other_dct["data"])
+        == [
+            "charge",
+            "data",
+            "image",
+            "photon",
+            "pixel",
+            "processed_data",
+            "scene",
+            "signal",
+        ]
     )
     np.testing.assert_equal(dct["data"]["photon"], other_dct["data"]["photon"])
     np.testing.assert_equal(dct["data"]["pixel"], other_dct["data"]["pixel"])
     np.testing.assert_equal(dct["data"]["signal"], other_dct["data"]["signal"])
     np.testing.assert_equal(dct["data"]["image"], other_dct["data"]["image"])
 
     assert (
-        set(dct["data"]["charge"])
-        == set(other_dct["data"]["charge"])
-        == {"array", "frame"}
+        sorted(dct["data"]["charge"])
+        == sorted(other_dct["data"]["charge"])
+        == ["array", "frame"]
     )
     np.testing.assert_equal(
         dct["data"]["charge"]["array"], other_dct["data"]["charge"]["array"]
     )
     pd.testing.assert_frame_equal(
         dct["data"]["charge"]["frame"], other_dct["data"]["charge"]["frame"]
     )
@@ -220,20 +229,16 @@
                                 "velocity_ver",
                                 "velocity_hor",
                                 "velocity_z",
                             ],
                             dtype=float,
                         ),
                     },
-                    "processed_data": {
-                        "coords": {},
-                        "attrs": {},
-                        "dims": {},
-                        "data_vars": {},
-                    },
+                    "data": {},
+                    "processed_data": {},
                 },
             },
             id="Default parameters",
         ),
         pytest.param(
             CMOS(
                 geometry=CMOSGeometry(
@@ -297,20 +302,16 @@
                                 "velocity_ver",
                                 "velocity_hor",
                                 "velocity_z",
                             ],
                             dtype=float,
                         ),
                     },
-                    "processed_data": {
-                        "coords": {},
-                        "attrs": {},
-                        "dims": {},
-                        "data_vars": {},
-                    },
+                    "data": {},
+                    "processed_data": {},
                 },
             },
             id="CMOS fully defined",
         ),
     ],
 )
 def test_to_and_from_dict(klass, obj, exp_dict):
```

### Comparing `pyxel_sim-1.8/tests/detectors/test_cmos_characteristics.py` & `pyxel_sim-1.9/tests/detectors/test_cmos_characteristics.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/detectors/test_cmos_geometry.py` & `pyxel_sim-1.9/tests/detectors/test_cmos_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/detectors/test_detectors.py` & `pyxel_sim-1.9/tests/detectors/test_detectors.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/detectors/test_environment.py` & `pyxel_sim-1.9/tests/detectors/test_environment.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/detectors/test_geometry.py` & `pyxel_sim-1.9/tests/detectors/test_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
             Parameters(row=1, col=3, pixel_vert_size=0.1, pixel_horz_size=0.2),
             np.array([0.05, 0.05, 0.05]),
             id="1x3",
         ),
     ],
 )
 def test_vertical_pixel_center_pos(
-    geometry_cls: Type[Geometry], parameters: Parameters, exp_values: np.ndarray
+    geometry_cls: type[Geometry], parameters: Parameters, exp_values: np.ndarray
 ):
     """Test method '.vertical_pixel_center_pos_list'."""
     # Create the geometry object
     geometry = geometry_cls(
         row=parameters.row,
         col=parameters.col,
         pixel_vert_size=parameters.pixel_vert_size,
@@ -83,15 +83,15 @@
             Parameters(row=1, col=3, pixel_vert_size=0.1, pixel_horz_size=0.2),
             np.array([0.1, 0.3, 0.5]),
             id="1x3",
         ),
     ],
 )
 def test_horizontal_pixel_center_pos(
-    geometry_cls: Type[Geometry], parameters: Parameters, exp_values: np.ndarray
+    geometry_cls: type[Geometry], parameters: Parameters, exp_values: np.ndarray
 ):
     """Test method '.horizontal_pixel_center_pos_list'."""
     # Create the geometry object
     geometry = geometry_cls(
         row=parameters.row,
         col=parameters.col,
         pixel_vert_size=parameters.pixel_vert_size,
```

### Comparing `pyxel_sim-1.8/tests/detectors/test_mkid.py` & `pyxel_sim-1.9/tests/detectors/test_mkid.py`

 * *Files 11% similar despite different names*

```diff
@@ -154,14 +154,15 @@
             "scene",
             "pixel",
             "signal",
             "image",
             "phase",
             "charge",
             "processed_data",
+            "data",
         }
     )
     np.testing.assert_equal(dct["data"]["photon"], other_dct["data"]["photon"])
     np.testing.assert_equal(dct["data"]["pixel"], other_dct["data"]["pixel"])
     np.testing.assert_equal(dct["data"]["signal"], other_dct["data"]["signal"])
     np.testing.assert_equal(dct["data"]["image"], other_dct["data"]["image"])
     np.testing.assert_equal(dct["data"]["phase"], other_dct["data"]["phase"])
@@ -234,20 +235,16 @@
                                 "velocity_ver",
                                 "velocity_hor",
                                 "velocity_z",
                             ],
                             dtype=float,
                         ),
                     },
-                    "processed_data": {
-                        "coords": {},
-                        "attrs": {},
-                        "dims": {},
-                        "data_vars": {},
-                    },
+                    "data": {},
+                    "processed_data": {},
                 },
             },
             id="Default Parameters",
         ),
         pytest.param(
             MKID(
                 geometry=MKIDGeometry(
@@ -311,20 +308,16 @@
                                 "velocity_ver",
                                 "velocity_hor",
                                 "velocity_z",
                             ],
                             dtype=float,
                         ),
                     },
-                    "processed_data": {
-                        "coords": {},
-                        "attrs": {},
-                        "dims": {},
-                        "data_vars": {},
-                    },
+                    "data": {},
+                    "processed_data": {},
                 },
             },
             id="MKID fully defined",
         ),
     ],
 )
 def test_to_and_from_dict(klass, obj, exp_dict):
```

### Comparing `pyxel_sim-1.8/tests/detectors/test_mkid_characteristics.py` & `pyxel_sim-1.9/tests/detectors/test_mkid_characteristics.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/detectors/test_mkid_geometry.py` & `pyxel_sim-1.9/tests/detectors/test_mkid_geometry.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/exposure/test_readout.py` & `pyxel_sim-1.9/tests/exposure/test_readout.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/functional_tests/test_parametric.py` & `pyxel_sim-1.9/tests/functional_tests/test_parametric.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+#  Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022.
+#
+#  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
+#  is part of this Pyxel package. No part of the package, including
+#  this file, may be copied, modified, propagated, or distributed except according to
+#  the terms contained in the file ‘LICENCE.txt’.
+
 from collections import abc
 from pathlib import Path
 
 import pytest
 
 import pyxel
 from pyxel import Configuration
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyxel_sim-1.8/tests/functional_tests/test_yaml.py` & `pyxel_sim-1.9/tests/functional_tests/test_yaml.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/inputs/test_image.py` & `pyxel_sim-1.9/tests/inputs/test_image.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/model_tests/amplifier_crosstalk/test_crosstalk.py` & `pyxel_sim-1.9/tests/model_tests/amplifier_crosstalk/test_crosstalk.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_collection/test_fixed_pattern_noise.py` & `pyxel_sim-1.9/tests/models/charge_collection/test_fixed_pattern_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_collection/test_persistence.py` & `pyxel_sim-1.9/tests/models/charge_collection/test_persistence.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 
+from collections.abc import Sequence
 from pathlib import Path
-from typing import Sequence
 
 import numpy as np
 import pytest
 
 from pyxel.detectors import (
     CCD,
     CMOS,
```

### Comparing `pyxel_sim-1.8/tests/models/charge_collection/test_simple_full_well.py` & `pyxel_sim-1.9/tests/models/charge_collection/test_simple_full_well.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_collection/test_simple_ipc.py` & `pyxel_sim-1.9/tests/models/charge_collection/test_simple_ipc.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_collection/test_simple_persistence.py` & `pyxel_sim-1.9/tests/models/charge_collection/test_simple_persistence.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_generation/test_apd_gain.py` & `pyxel_sim-1.9/tests/models/charge_generation/test_apd_gain.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_generation/test_charge_deposition_in_MCT.py` & `pyxel_sim-1.9/tests/models/charge_generation/test_charge_deposition_in_MCT.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_generation/test_charge_injection.py` & `pyxel_sim-1.9/tests/models/charge_generation/test_charge_injection.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_generation/test_dark_current.py` & `pyxel_sim-1.9/tests/models/charge_generation/test_dark_current.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_generation/test_dark_current_rule07.py` & `pyxel_sim-1.9/tests/models/charge_generation/test_dark_current_rule07.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_generation/test_load_charge.py` & `pyxel_sim-1.9/tests/models/charge_generation/test_load_charge.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_generation/test_photoelectrons.py` & `pyxel_sim-1.9/tests/models/charge_generation/test_photoelectrons.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_measurement/test_nghxrg.py` & `pyxel_sim-1.9/tests/models/charge_measurement/test_nghxrg.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_measurement/test_non_linearity.py` & `pyxel_sim-1.9/tests/models/charge_measurement/test_non_linearity.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 
-from typing import Sequence
+from collections.abc import Sequence
 
 import numpy as np
 import pytest
 
 from pyxel.detectors import (
     CCD,
     CMOS,
```

### Comparing `pyxel_sim-1.8/tests/models/charge_measurement/test_offset.py` & `pyxel_sim-1.9/tests/models/charge_measurement/test_offset.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_measurement/test_readout_noise.py` & `pyxel_sim-1.9/tests/models/charge_measurement/test_readout_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_measurement/test_reset_noise.py` & `pyxel_sim-1.9/tests/models/charge_measurement/test_reset_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_transfer/arctic_remove.py` & `pyxel_sim-1.9/tests/models/charge_transfer/arctic_remove.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_transfer/test_arctic_add.py` & `pyxel_sim-1.9/tests/models/charge_transfer/test_arctic_add.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/charge_transfer/test_cdm.py` & `pyxel_sim-1.9/tests/models/charge_transfer/test_cdm.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
 
-from typing import Literal, Optional, Sequence
+from collections.abc import Sequence
+from typing import Literal, Optional
 
 import numpy as np
 import pytest
 
 from pyxel.detectors import (
     CCD,
     CMOS,
```

### Comparing `pyxel_sim-1.8/tests/models/charge_transfer/test_emccd_poisson.py` & `pyxel_sim-1.9/tests/models/charge_transfer/test_emccd_poisson.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/data_processing/test_statistics.py` & `pyxel_sim-1.9/tests/models/readout_electronics/test_sar_adc.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,34 @@
-#   Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022.
-#  #
-#   This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
-#   is part of this Pyxel package. No part of the package, including
-#   this file, may be copied, modified, propagated, or distributed except according to
-#   the terms contained in the file ‘LICENCE.txt’.
+#  Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022.
+#
+#  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
+#  is part of this Pyxel package. No part of the package, including
+#  this file, may be copied, modified, propagated, or distributed except according to
+#  the terms contained in the file ‘LICENCE.txt’.
 
 import pytest
 
-from pyxel.detectors import (
-    CCD,
-    CCDGeometry,
-    Characteristics,
-    Environment,
-    ReadoutProperties,
-)
-from pyxel.models.data_processing import compute_statistics
+from pyxel.detectors import CCD, CCDGeometry, Characteristics, Environment
+from pyxel.models.readout_electronics import sar_adc
 
 
 @pytest.fixture
-def ccd_10x10() -> CCD:
+def ccd_10x3() -> CCD:
     """Create a valid CCD detector."""
-    detector = CCD(
+    return CCD(
         geometry=CCDGeometry(
             row=10,
-            col=10,
+            col=3,
             total_thickness=40.0,
             pixel_vert_size=10.0,
             pixel_horz_size=10.0,
         ),
         environment=Environment(),
-        characteristics=Characteristics(),
+        characteristics=Characteristics(
+            adc_bit_resolution=16, adc_voltage_range=(0.0, 10.0)
+        ),
     )
-    detector._readout_properties = ReadoutProperties(num_steps=1)
-    return detector
 
 
-def test_statistics(ccd_10x10: CCD):
-    """Test input parameters for function 'statistics'."""
-    detector = ccd_10x10
-    compute_statistics(detector=detector)
-    dataset = detector.processed_data.data
-    assert "time" in dataset.coords
-    assert list(dataset.coords["time"].values) == [0.0]
+def test_sar_adc(ccd_10x3: CCD):
+    """Test model 'sar_adc' with valid inputs."""
+    sar_adc(detector=ccd_10x3)
```

### Comparing `pyxel_sim-1.8/tests/models/phasing/test_pulse_processing.py` & `pyxel_sim-1.9/tests/models/phasing/test_pulse_processing.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/photon_collection/test_illumination.py` & `pyxel_sim-1.9/tests/models/photon_collection/test_illumination.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 #  Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022.
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
-from typing import Literal, Optional, Sequence
+from collections.abc import Sequence
+from typing import Literal, Optional
 
 import pytest
 
 from pyxel.detectors import (
     CCD,
     CCDGeometry,
     Characteristics,
```

### Comparing `pyxel_sim-1.8/tests/models/photon_collection/test_load_image.py` & `pyxel_sim-1.9/tests/models/photon_collection/test_load_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         pytest.param("img.npy", (0, 0), None, True, 1.0, 1.0, 16, id="valid"),
     ],
 )
 def test_load_image(
     ccd_10x10: CCD,
     valid_data2d: str,
     image_file: str,
-    position: Tuple[int, int],
+    position: tuple[int, int],
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ],
     convert_to_photons: bool,
     multiplier: float,
     time_scale: float,
     bit_resolution: int,
@@ -110,15 +110,15 @@
         ),
     ],
 )
 def test_load_image_with_invalid_params(
     ccd_10x10: CCD,
     valid_data2d: str,
     image_file: str,
-    position: Tuple[int, int],
+    position: tuple[int, int],
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ],
     convert_to_photons: bool,
     multiplier: float,
     time_scale: float,
     bit_resolution: int,
```

### Comparing `pyxel_sim-1.8/tests/models/photon_collection/test_load_psf.py` & `pyxel_sim-1.9/tests/models/photon_collection/test_load_psf.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/photon_collection/test_optical_psf.py` & `pyxel_sim-1.9/tests/models/photon_collection/test_optical_psf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #  Copyright (c) European Space Agency, 2017, 2018, 2019, 2020, 2021, 2022.
 #
 #  This file is subject to the terms and conditions defined in file 'LICENCE.txt', which
 #  is part of this Pyxel package. No part of the package, including
 #  this file, may be copied, modified, propagated, or distributed except according to
 #  the terms contained in the file ‘LICENCE.txt’.
 
-from typing import Mapping, Sequence
+from collections.abc import Mapping, Sequence
 
 import pytest
 
 from pyxel.detectors import CCD, CCDGeometry, Characteristics, Environment
 from pyxel.models.photon_collection import optical_psf
 from pyxel.models.photon_collection.poppy import (
     CircularAperture,
```

### Comparing `pyxel_sim-1.8/tests/models/photon_collection/test_shot_noise.py` & `pyxel_sim-1.9/tests/models/photon_collection/test_shot_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/photon_collection/test_stripe_pattern.py` & `pyxel_sim-1.9/tests/models/photon_collection/test_stripe_pattern.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/readout_electronics/test_ac_crosstalk.py` & `pyxel_sim-1.9/tests/models/readout_electronics/test_ac_crosstalk.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/readout_electronics/test_dc_crosstalk.py` & `pyxel_sim-1.9/tests/models/readout_electronics/test_dc_crosstalk.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/readout_electronics/test_dead_time_filter.py` & `pyxel_sim-1.9/tests/models/readout_electronics/test_dead_time_filter.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/readout_electronics/test_get_matrix.py` & `pyxel_sim-1.9/tests/models/readout_electronics/test_get_matrix.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/readout_electronics/test_phase_conversion.py` & `pyxel_sim-1.9/tests/models/readout_electronics/test_phase_conversion.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/readout_electronics/test_sar_adc_with_noise.py` & `pyxel_sim-1.9/tests/models/readout_electronics/test_sar_adc_with_noise.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/readout_electronics/test_simple_adc.py` & `pyxel_sim-1.9/tests/models/readout_electronics/test_simple_adc.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/models/test_save_load_detector.py` & `pyxel_sim-1.9/tests/models/test_save_load_detector.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/pipelines/observation/test_validate_steps.py` & `pyxel_sim-1.9/tests/pipelines/observation/test_validate_steps.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/pipelines/test_pipelines.py` & `pyxel_sim-1.9/tests/pipelines/test_pipelines.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/running_mode/test_observation.py` & `pyxel_sim-1.9/tests/running_mode/test_observation.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/test_evaluator.py` & `pyxel_sim-1.9/tests/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/test_options.py` & `pyxel_sim-1.9/tests/test_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,12 +48,12 @@
             {"non_sense": "foo"}, KeyError, "Wrong option", id="Unknown option"
         ),
         pytest.param({"cache_enabled": "Hello"}, TypeError, None, id="Wrong type"),
         pytest.param({"cache_folder": 42}, TypeError, None, id="Wrong type"),
     ],
 )
 def test_with_wrong_inputs(
-    dct: dict, exp_error: Type[TypeError], exp_msg: Optional[str]
+    dct: dict, exp_error: type[TypeError], exp_msg: Optional[str]
 ):
     """Test with a bad input."""
     with pytest.raises(exp_error, match=exp_msg):
         pyxel.set_options(**dct)
```

### Comparing `pyxel_sim-1.8/tests/unittests/test_arguments.py` & `pyxel_sim-1.9/tests/unittests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/unittests/test_calibration.py` & `pyxel_sim-1.9/tests/unittests/test_calibration.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/unittests/test_detector.py` & `pyxel_sim-1.9/tests/unittests/test_detector.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/unittests/test_environment.py` & `pyxel_sim-1.9/tests/unittests/test_environment.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/unittests/test_fitting.py` & `pyxel_sim-1.9/tests/unittests/test_fitting.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 import pyxel
 from pyxel.calibration import Calibration
 from pyxel.calibration.fitting import ModelFitting
 from pyxel.calibration.util import CalibrationMode
 from pyxel.detectors import CCD
 from pyxel.pipelines import DetectionPipeline, Processor
-from pyxel.pipelines.processor import ResultType
+
+# from pyxel.pipelines.processor import ResultType
 
 try:
     import pygmo as pg
 
     WITH_PYGMO = True
 except ImportError:
     WITH_PYGMO = False
@@ -73,15 +74,15 @@
     assert mf.calibration_mode == CalibrationMode.Pipeline
     assert mf.sim_fit_range == (
         slice(None, None, None),
         slice(0, 4, None),
         slice(2, 4, None),
     )
     assert mf.targ_fit_range == (slice(1, 5, None), slice(0, 2, None))
-    assert mf.sim_output == ResultType.Image
+    # assert mf.sim_output == ResultType.Image
 
 
 @pytest.mark.skipif(not WITH_PYGMO, reason="Package 'pygmo' is not installed.")
 @pytest.mark.parametrize("yaml", ["tests/data/calibrate_fits.yaml"])
 def test_configure_fits_target(yaml):
     """Test"""
     cfg = pyxel.load(yaml)
@@ -103,15 +104,15 @@
     configure(mf, cfg)
     assert mf.sim_fit_range == (
         slice(None, None, None),
         slice(0, 4, None),
         slice(2, 4, None),
     )
     assert mf.targ_fit_range == (slice(1, 5, None), slice(0, 2, None))
-    assert mf.sim_output == ResultType.Image
+    # assert mf.sim_output == ResultType.Image
     expected = np.array(
         [
             [4173.6434, 4203.6883],
             [4468.6537, 4517.2588],
             [4683.7958, 4594.2287],
             [4520.4915, 4315.9494],
         ]
```

### Comparing `pyxel_sim-1.8/tests/unittests/test_model_function.py` & `pyxel_sim-1.9/tests/unittests/test_model_function.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/util/test_fit_into_array.py` & `pyxel_sim-1.9/tests/util/test_fit_into_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,16 +161,16 @@
                 ]
             ),
         ),
     ],
 )
 def test_fit_into_array_2d(
     array_2d,
-    output_shape: Tuple[int, int],
-    relative_position: Tuple[int, int],
+    output_shape: tuple[int, int],
+    relative_position: tuple[int, int],
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ],
     allow_smaller_array: bool,
     expected_output: np.ndarray,
 ):
     """Test function 'fit_into_array' with some valid inputs."""
@@ -226,16 +226,16 @@
                 ]
             ),
         ),
     ],
 )
 def test_fit_into_array_1d_col(
     array_1d_col,
-    output_shape: Tuple[int, int],
-    relative_position: Tuple[int, int],
+    output_shape: tuple[int, int],
+    relative_position: tuple[int, int],
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ],
     allow_smaller_array: bool,
     expected_output: np.ndarray,
 ):
     """Test function 'fit_into_array' with some valid inputs."""
@@ -289,16 +289,16 @@
                 ]
             ),
         ),
     ],
 )
 def test_fit_into_array_1d_row(
     array_1d_row,
-    output_shape: Tuple[int, int],
-    relative_position: Tuple[int, int],
+    output_shape: tuple[int, int],
+    relative_position: tuple[int, int],
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ],
     allow_smaller_array: bool,
     expected_output: np.ndarray,
 ):
     """Test function 'fit_into_array' with some valid inputs."""
@@ -356,16 +356,16 @@
             True,
             ValueError,
             "No overlap of array and target in X dimension.",
         ),
     ],
 )
 def test_fit_into_array_bad_inputs(
-    output_shape: Tuple[int, int],
-    relative_position: Tuple[int, int],
+    output_shape: tuple[int, int],
+    relative_position: tuple[int, int],
     align: Optional[
         Literal["center", "top_left", "top_right", "bottom_left", "bottom_right"]
     ],
     allow_smaller_array: bool,
     exp_exc,
     exp_error,
 ):
```

### Comparing `pyxel_sim-1.8/tests/util/test_memory.py` & `pyxel_sim-1.9/tests/util/test_memory.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/tests/util/test_random.py` & `pyxel_sim-1.9/tests/util/test_random.py`

 * *Files identical despite different names*

### Comparing `pyxel_sim-1.8/venv/bin/activate_this.py` & `pyxel_sim-1.9/venv/bin/activate_this.py`

 * *Files identical despite different names*

