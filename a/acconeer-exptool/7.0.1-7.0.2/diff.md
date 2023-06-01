# Comparing `tmp/acconeer-exptool-7.0.1.tar.gz` & `tmp/acconeer-exptool-7.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acconeer-exptool-7.0.1.tar", last modified: Mon May 15 15:25:01 2023, max compression
+gzip compressed data, was "acconeer-exptool-7.0.2.tar", last modified: Thu Jun  1 13:03:48 2023, max compression
```

## Comparing `acconeer-exptool-7.0.1.tar` & `acconeer-exptool-7.0.2.tar`

### file list

```diff
@@ -1,608 +1,609 @@
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.336519 acconeer-exptool-7.0.1/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/.gitattributes
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.288519 acconeer-exptool-7.0.1/.github/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.292519 acconeer-exptool-7.0.1/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/.readthedocs.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14313 2023-05-15 15:24:30.000000 acconeer-exptool-7.0.1/CHANGELOG.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-04-04 07:09:09.000000 acconeer-exptool-7.0.1/Jenkinsfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/LICENSE.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-05-15 15:25:01.336519 acconeer-exptool-7.0.1/PKG-INFO
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-04-04 08:04:53.000000 acconeer-exptool-7.0.1/README.md
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       73 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.1/UNRELEASED_CHANGELOG.md
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.292519 acconeer-exptool-7.0.1/docker/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/docker/Dockerfile
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/docker/requirements-dev.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-03-28 13:52:52.000000 acconeer-exptool-7.0.1/dodo.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.288519 acconeer-exptool-7.0.1/examples/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.292519 acconeer-exptool-7.0.1/examples/a111/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/basic.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/basic_continuous.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a111/plotting/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/plotting/plot_with_matplotlib.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/plotting/plot_with_pyqtgraph.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a111/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/record_data/long_duration_split_files.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/record_data/with_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a111/services/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/services/envelope.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/services/iq.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/services/power_bins.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/services/sparse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a111/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/utils/ping.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a111/utils/test_throughput.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/basic.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/bilateration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/bilateration/bilaterator.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6340 2023-05-15 15:00:18.000000 acconeer-exptool-7.0.1/examples/a121/breathing/breathing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/distance/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/distance/detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/distance/processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      776 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/extended_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a121/load_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/examples/a121/load_record_h5.m
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-04-11 14:12:51.000000 acconeer-exptool-7.0.1/examples/a121/phase_tracking/phase_tracking.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/plot.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/presence/detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/presence/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/record_data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      975 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/examples/a121/record_data/barebones.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1017 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/examples/a121/record_data/with_cli.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/reuse_calibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/smart_presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/smart_presence/processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9497 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/smart_presence/ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/stress.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      946 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/subsweeps.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/surface_velocity/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-04-17 09:00:21.000000 acconeer-exptool-7.0.1/examples/a121/surface_velocity/example_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-04-17 09:00:21.000000 acconeer-exptool-7.0.1/examples/a121/surface_velocity/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/touchless_button/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/examples/a121/touchless_button/processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/examples/a121/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-04-28 09:00:19.000000 acconeer-exptool-7.0.1/examples/a121/vibration/vibration.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/gui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/gui/main.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7005 2023-04-17 09:00:21.000000 acconeer-exptool-7.0.1/noxfile.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/portable/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/portable/.gitignore
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/portable/make.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/portable/package/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/portable/package/cmd_with_path.bat
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/portable/package/run_app.bat
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/portable/package/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/portable/package/tools/update.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/portable/package/update.bat
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2515 2023-04-04 07:09:09.000000 acconeer-exptool-7.0.1/pyproject.toml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2433 2023-05-15 15:25:01.336519 acconeer-exptool-7.0.1/setup.cfg
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.292519 acconeer-exptool-7.0.1/src/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.288519 acconeer-exptool-7.0.1/src/acconeer/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/src/acconeer/exptool/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_bs_thread.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.296519 acconeer-exptool-7.0.1/src/acconeer/exptool/_pyusb/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_pyusb/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-01-20 14:07:33.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_pyusb/pyusbcomm.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/_structs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_structs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_structs/configbase.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_structs/qtpidgets.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/_tests/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_tests/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_tests/test_rig.py
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-05-15 15:25:01.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_version.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/LICENSE
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-27 07:26:03.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/usb_cdc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/winusb.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/winusbclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/winusberror.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/winusbpy.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/winusbutils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      438 2023-04-04 07:09:09.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/client_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/common.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/json/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/json/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/json/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/links.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/mock/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/mock/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/mock/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/multiwrap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/data/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/protocol.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-04-04 07:09:09.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/regmap.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_modes.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/_base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/_base/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/_base/module_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/_standalone_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.300519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.304519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.304519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.304519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.304519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2022-12-29 10:05:03.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.304519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/iq/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/iq/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.304519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.304519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/parking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/parking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/parking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/parking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/parking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/parking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.304519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.304519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/power_bins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/power_bins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/power_bins/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/power_bins/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/power_bins/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/power_bins/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.308519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-21 12:30:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-21 12:30:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-21 12:30:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-21 12:30:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-21 12:30:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.308519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.308519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sleep_breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.308519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.308519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.308519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.308519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/speed_sparse/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.308519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.308519 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/wave_to_exit/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a111/recording.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.308519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1136 2023-03-31 13:21:19.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_cli.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.312519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.312519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.312519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-08 08:37:30.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    22033 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10267 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11137 2023-04-28 09:00:19.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.312519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      607 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-04-17 12:38:00.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8216 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/result.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/dtypes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.312519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/mediators/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/mediators/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/mediators/link.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1265 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/mediators/recorder.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.312519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      401 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/__init__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.312519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      439 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7119 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15568 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.312519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-10 15:31:42.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-10 15:31:42.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11369 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      276 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3012 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12719 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/im_record/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3543 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18035 2023-04-28 09:00:19.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core_ext/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core_ext/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4903 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_h5_utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4840 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_perf_calc.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_rate_calc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      646 2023-04-28 09:00:19.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-04-17 12:38:00.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_base.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7322 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/_a121.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/processor/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8305 2023-05-15 15:24:30.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6492 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7327 2023-05-15 15:00:18.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/bilateration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-06 10:47:50.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/bilateration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:17.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/bilateration/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24956 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/bilateration/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/breathing/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      192 2023-05-15 15:00:18.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/breathing/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-05-15 15:00:18.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/breathing/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8723 2023-05-15 15:00:18.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/breathing/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7401 2023-05-15 15:00:18.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/breathing/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      507 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      855 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_aggregator.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:17.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    59448 2023-05-15 15:24:30.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24143 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-04-28 09:00:19.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_processors.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.316519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/phase_tracking/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-03-31 11:49:15.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.320519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-03-22 15:48:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2175 2023-03-22 15:48:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14489 2023-05-15 15:24:30.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/_detector.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25715 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-04-28 09:00:19.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/_processors.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.320519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-02-21 12:30:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2223 2023-03-22 15:48:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-03-23 12:16:45.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7165 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21740 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6835 2023-03-22 15:48:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.320519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/sparse_iq/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-06 10:47:50.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-06 10:47:50.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.320519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/surface_velocity/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      130 2023-03-27 10:18:02.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11611 2023-05-15 15:24:30.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21725 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14090 2023-04-28 09:00:19.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.320519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-03-22 21:29:48.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27271 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-03-22 15:48:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-03-22 21:29:48.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.320519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-01-27 07:26:03.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-31 08:16:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14570 2023-04-11 12:00:20.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-03-29 14:55:09.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.320519 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/vibration/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/vibration/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/vibration/__main__,py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 09:00:19.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/vibration/_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7398 2023-04-28 09:00:19.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/vibration/_processor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/a121/py.typed
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.320519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-03-31 11:49:15.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/launcher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.320519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      959 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/_argument_parser.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-02-21 12:30:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/_enums.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/_exceptions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/_version_checker.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2022-12-29 10:05:03.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.324519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27938 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/app_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/app_model_listener.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/file_detective.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/port_updater.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.324519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      452 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2737 2023-05-15 11:15:58.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_application_client.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5135 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_backend.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_backend_logger.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1857 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_backend_plugin.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_message.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4896 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_model.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1558 2023-05-15 15:00:18.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/plugin_loader.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.324519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2222 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/qt_subclasses.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/storage.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.324519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      495 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/app_model_viewer.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-04-11 13:26:43.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/device_comboboxes.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.324519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/flash_tab/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       94 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14023 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4635 2023-04-19 08:17:48.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15274 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/help_tab.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2052 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/icons.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3600 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/main_window.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1968 2023-04-11 13:26:43.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/misc.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.324519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      783 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6615 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-22 15:48:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6166 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-03-27 09:24:07.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3557 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.324519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-20 12:36:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      499 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3814 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25494 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-04-28 09:00:19.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12975 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6474 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7963 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1887 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      294 2023-04-19 08:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/types.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      865 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9480 2023-04-11 13:26:43.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/status_bar.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.328519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       98 2023-04-11 13:27:02.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10441 2023-04-11 13:27:02.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5853 2023-04-11 13:27:02.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12245 2023-04-11 13:27:02.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4551 2023-04-11 13:27:02.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2636 2023-04-21 07:00:24.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1382 2023-04-26 12:00:23.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.328519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    84006 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/app.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/data_processing.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.328519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/elements/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/elements/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-29 10:05:03.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/elements/helper.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-21 12:30:25.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/elements/modules.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-12 21:00:22.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/elements/qt_subclasses.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.328519 acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/a111_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/a121_gui.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/icon-black.svg
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/icon.png
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/loader.gif
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.292519 acconeer-exptool-7.0.1/src/acconeer/exptool/data/
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.328519 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/LICENSE.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.328519 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/aarch64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.328519 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/amd64/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.328519 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/armv6/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.332519 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/armv7/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.332519 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/i386/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.332519 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/x86_64/
--rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.332519 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/__main__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5844 2023-04-03 11:06:12.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_bin_fetcher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3625 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_dev_license.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_dev_license_tui.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_device_flasher_base.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-04-04 08:00:22.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_flasher.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-01-27 07:26:03.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_products.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.332519 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_stm32uart/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_stm32uart/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_stm32uart/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-03-30 11:28:28.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.332519 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_xc120/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-27 07:26:03.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_xc120/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-01-27 07:26:03.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-04-19 12:00:17.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-27 07:26:03.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_xc120/_meta.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/libft4222.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/mpl_process.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/pg_process.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.336519 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/__main__.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.336519 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/platform_install.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/prompts.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/setup_group.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/setup_step.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.336519 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/cli/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/cli/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/cli/argument_parser.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.336519 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/platforms/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/platforms/__init__.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/platforms/how_to.txt
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/platforms/linux.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/setup/py.typed
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-03-22 21:29:48.000000 acconeer-exptool-7.0.1/src/acconeer/exptool/utils.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.336519 acconeer-exptool-7.0.1/src/acconeer_exptool.egg-info/
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-05-15 15:25:01.000000 acconeer-exptool-7.0.1/src/acconeer_exptool.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25483 2023-05-15 15:25:01.000000 acconeer-exptool-7.0.1/src/acconeer_exptool.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-15 15:25:01.000000 acconeer-exptool-7.0.1/src/acconeer_exptool.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-05-15 15:25:00.000000 acconeer-exptool-7.0.1/src/acconeer_exptool.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)      475 2023-05-15 15:25:01.000000 acconeer-exptool-7.0.1/src/acconeer_exptool.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-05-15 15:25:01.000000 acconeer-exptool-7.0.1/src/acconeer_exptool.egg-info/top_level.txt
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.336519 acconeer-exptool-7.0.1/tools/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3715 2023-05-04 12:49:41.000000 acconeer-exptool-7.0.1/tools/check_changelog.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/tools/check_copyright.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/tools/check_line_length.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/tools/check_permissions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-04-04 07:09:09.000000 acconeer-exptool-7.0.1/tools/check_sdk_mentions.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/tools/check_whitespace.py
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/tools/update_regmap.py
-drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-05-15 15:25:01.336519 acconeer-exptool-7.0.1/utils/
--rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14756 2022-12-22 13:53:10.000000 acconeer-exptool-7.0.1/utils/convert_to_csv.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.774839 acconeer-exptool-7.0.2/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/.gitattributes
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.722839 acconeer-exptool-7.0.2/.github/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      877 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      368 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      158 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/.readthedocs.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14372 2023-06-01 12:49:58.000000 acconeer-exptool-7.0.2/CHANGELOG.md
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    13663 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/Jenkinsfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1881 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/LICENSE.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      217 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-06-01 13:03:48.774839 acconeer-exptool-7.0.2/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7948 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/README.md
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       73 2023-05-31 10:00:02.000000 acconeer-exptool-7.0.2/UNRELEASED_CHANGELOG.md
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/docker/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1865 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/docker/Dockerfile
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       82 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/docker/requirements-dev.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1604 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/dodo.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.726839 acconeer-exptool-7.0.2/examples/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/examples/a111/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3247 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/basic.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1819 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/basic_continuous.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2657 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1273 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/examples/a111/plotting/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1999 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/plotting/plot_with_matplotlib.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2551 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/plotting/plot_with_pyqtgraph.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/examples/a111/record_data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1156 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/record_data/barebones.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2541 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/record_data/long_duration_split_files.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1958 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/record_data/with_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a111/services/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2251 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/services/envelope.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3013 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/services/iq.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2277 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/services/power_bins.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2861 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/services/sparse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a111/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      802 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/utils/ping.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      805 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a111/utils/test_throughput.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1222 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/basic.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/bilateration/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8174 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/bilateration/bilaterator.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6340 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/examples/a121/breathing/breathing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/distance/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4522 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/distance/detector.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/distance/processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      776 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/extended_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1518 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a121/load_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1405 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/examples/a121/load_record_h5.m
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/phase_tracking/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5808 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/phase_tracking/phase_tracking.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4538 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/plot.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/presence/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11241 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/presence/detector.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11026 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/presence/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/record_data/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      975 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/record_data/barebones.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1017 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/record_data/with_cli.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1140 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/reuse_calibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/smart_presence/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10430 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/smart_presence/processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9497 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/smart_presence/ref_app.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4253 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/stress.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      946 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/subsweeps.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/surface_velocity/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8515 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/surface_velocity/example_app.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8864 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/surface_velocity/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/touchless_button/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3927 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/touchless_button/processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/examples/a121/vibration/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4410 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/examples/a121/vibration/vibration.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/gui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1254 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/gui/main.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7005 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/noxfile.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/portable/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       27 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/.gitignore
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1571 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/make.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/portable/package/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      108 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/package/cmd_with_path.bat
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      346 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/package/run_app.bat
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/portable/package/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      989 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/package/tools/update.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      168 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/portable/package/update.bat
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2515 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/pyproject.toml
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2433 2023-06-01 13:03:48.774839 acconeer-exptool-7.0.2/setup.cfg
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/src/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.726839 acconeer-exptool-7.0.2/src/acconeer/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/src/acconeer/exptool/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      295 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3212 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_bs_thread.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/src/acconeer/exptool/_pyusb/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      100 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_pyusb/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5890 2023-01-24 10:54:24.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_pyusb/pyusbcomm.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15542 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/configbase.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15673 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/qtpidgets.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.734839 acconeer-exptool-7.0.2/src/acconeer/exptool/_tests/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_tests/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4259 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_tests/test_rig.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       22 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_version.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1071 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/LICENSE
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      190 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2847 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6837 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/usb_cdc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2021 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusb.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3466 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      231 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusberror.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10029 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbpy.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12307 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbutils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      438 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      119 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7940 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5916 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5513 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/client_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      517 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/common.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/json/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/json/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18330 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/json/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14209 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/links.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/mock/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/mock/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7621 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/mock/client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1496 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/multiwrap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    24884 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/data/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/data/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8068 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6351 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/protocol.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9853 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/regmap.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7176 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_conf_to_rss_sdk.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    28007 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      587 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_modes.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3710 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      242 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2708 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_base/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      860 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_base/module_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1695 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_standalone_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      538 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7469 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4554 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.738839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      618 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6054 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5308 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11319 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4931 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      948 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21416 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2204 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6126 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      862 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2022-12-29 10:02:50.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5280 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      565 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1985 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3928 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      939 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27784 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9166 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      104 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    16847 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      890 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9162 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8503 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      110 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      576 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2599 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4172 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       99 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      612 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1400 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.742839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15250 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13885 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      917 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14079 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10519 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      615 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10381 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4623 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      577 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5079 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      552 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1341 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4454 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      557 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5185 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     5472 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      824 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12380 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      186 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/constants.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7812 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/ui.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10409 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1517 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3125 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2560 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      135 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      153 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      545 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4662 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6099 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9009 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a111/recording.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1136 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1790 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_cli.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.746839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      989 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      690 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2023-02-08 08:58:10.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4195 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    22033 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10267 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/session_config.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11137 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1035 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      607 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8821 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/client_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4798 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/metadata.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8216 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2192 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/result.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1351 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2906 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/server_info.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/server_log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2189 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1675 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      144 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/dtypes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      150 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      931 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/link.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1265 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/recorder.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      401 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/__init__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      439 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7119 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/client.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5053 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1324 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15568 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      403 2023-02-13 09:23:57.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1023 2023-02-13 09:23:57.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6512 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      985 2023-02-13 09:23:57.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1037 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      840 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.750839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      521 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      687 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1150 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       96 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/parse_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4314 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1123 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      752 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2836 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1045 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      791 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       97 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/server_error.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1998 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/links.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      643 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/message.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11369 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3996 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      276 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8225 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3012 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12719 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1526 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      928 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/im_record/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       95 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/im_record/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3543 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18035 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core_ext/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      118 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core_ext/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4868 2023-05-31 21:00:21.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core_ext/_replaying_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      318 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_h5_utils.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4840 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_perf_calc.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2516 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_rate_calc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      681 2023-06-01 09:17:45.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4086 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_base.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      367 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7933 2023-06-01 12:45:39.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_a121.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      434 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      617 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3783 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      446 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8320 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1276 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6579 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    10386 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      175 2023-02-06 10:51:29.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      395 2023-03-28 07:00:16.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24946 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/_plugin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    17474 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      192 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8723 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7401 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      507 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      855 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5471 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_aggregator.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      307 2023-03-28 07:00:16.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_configs.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    59448 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    24079 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    30450 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_processors.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    15812 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.754839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7575 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7141 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      213 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2175 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    13856 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_detector.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    25707 2023-06-01 12:48:59.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    18288 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_processors.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4717 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      182 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2223 2023-05-31 10:00:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6607 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7165 2023-05-31 10:00:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21729 2023-06-01 12:48:59.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6835 2023-05-31 10:00:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      220 2023-02-06 16:11:19.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8167 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3116 2023-02-06 16:11:19.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7245 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      130 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    11611 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21732 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14090 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      219 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1658 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27152 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7290 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     6265 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4229 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_serializer.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      306 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      486 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1100 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1738 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_configs.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7687 2023-03-31 08:16:11.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14754 2023-06-01 09:17:45.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_processor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2896 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      187 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      376 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/__main__,py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8514 2023-04-28 09:00:18.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     7628 2023-06-01 09:17:45.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/_processor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/a121/py.typed
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      333 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4475 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/launcher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.758839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      959 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/__main__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      994 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_argument_parser.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1718 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_enums.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      102 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_exceptions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      983 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_version_checker.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2698 2022-12-29 10:02:50.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      239 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    27076 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/app_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/app_model_listener.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      981 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/file_detective.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      428 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/plugin_protocols.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2074 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/port_updater.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      478 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2737 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_application_client.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4985 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1610 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend_logger.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2040 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend_plugin.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1559 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_message.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4770 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_model.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2786 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_tasks.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1558 2023-06-01 11:00:34.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/plugin_loader.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      241 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      973 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      431 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1404 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1024 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1836 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      470 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/qt_subclasses.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      804 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/storage.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      495 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2141 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/app_model_viewer.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2641 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/device_comboboxes.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       94 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    14023 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4635 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/threads.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    15274 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1802 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/help_tab.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2052 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/icons.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3600 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/main_window.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1968 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/misc.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.762839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      783 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6615 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1290 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1026 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6166 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1432 2023-03-27 09:23:51.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3557 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      769 2023-03-30 13:00:17.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      499 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/common.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     3814 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2082 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25494 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2004 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12975 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6474 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     7963 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1887 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      294 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/types.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      865 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/utils.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9480 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/status_bar.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)       98 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/__init__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10441 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5853 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/hints.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12245 2023-06-01 12:00:03.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4551 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     2636 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     1382 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       79 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      116 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    84006 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/app.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4735 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/data_processing.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     8476 2022-12-29 10:02:50.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/helper.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2346 2023-02-23 12:52:28.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/modules.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    10745 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/qt_subclasses.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    90184 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/a111_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    57036 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/a121_gui.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4162 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/icon-black.svg
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    35706 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/icon.png
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3208 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/loader.gif
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.730839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1245 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/LICENSE.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/aarch64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   513305 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/amd64/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   209008 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   314552 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv6/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   484176 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.766839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv7/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   399731 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/i386/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   160256 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)   271672 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/x86_64/
+-rwxrwxr-x   0 jenkins   (1000) jenkins   (1000)   504389 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      338 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      115 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/__main__.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     5844 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_bin_fetcher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3625 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_dev_license.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     4284 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_dev_license_tui.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      416 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_device_flasher_base.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    12868 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_flasher.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      828 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_products.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_stm32uart/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      150 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_stm32uart/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      274 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_stm32uart/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     6665 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      258 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     9147 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     9417 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      224 2023-01-24 14:05:20.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/_meta.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    11051 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/libft4222.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3338 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/mpl_process.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3185 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/pg_process.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/__main__.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      244 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1431 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/platform_install.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      980 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/prompts.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      690 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/setup_group.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2880 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/setup_step.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      520 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/cli/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      106 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/cli/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      684 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/cli/argument_parser.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)       91 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/__init__.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)      329 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/how_to.txt
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1867 2022-12-22 15:03:13.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/linux.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1191 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)        0 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/setup/py.typed
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    21469 2023-04-03 13:53:22.000000 acconeer-exptool-7.0.2/src/acconeer/exptool/utils.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.770839 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     8990 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)    25530 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        1 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)      475 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)        9 2023-06-01 13:03:48.000000 acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/top_level.txt
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.774839 acconeer-exptool-7.0.2/tools/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     3943 2023-06-01 09:17:45.000000 acconeer-exptool-7.0.2/tools/check_changelog.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    12005 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/tools/check_copyright.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1388 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/tools/check_line_length.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1495 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/tools/check_permissions.py
+-rw-r--r--   0 jenkins   (1000) jenkins   (1000)     4237 2023-05-30 21:08:02.000000 acconeer-exptool-7.0.2/tools/check_sdk_mentions.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     1801 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/tools/check_whitespace.py
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)     2064 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/tools/update_regmap.py
+drwxr-xr-x   0 jenkins   (1000) jenkins   (1000)        0 2023-06-01 13:03:48.774839 acconeer-exptool-7.0.2/utils/
+-rw-rw-r--   0 jenkins   (1000) jenkins   (1000)    14756 2022-12-21 10:06:47.000000 acconeer-exptool-7.0.2/utils/convert_to_csv.py
```

### Comparing `acconeer-exptool-7.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `acconeer-exptool-7.0.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/CHANGELOG.md` & `acconeer-exptool-7.0.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## v7.0.2
+
+### Fixed
+- A121: Fix replaying issues in apps
+
 ## v7.0.1
 
 ### Fixed
 - Recording bug introduced in v7.0.0 that broke all algorithms.
 
 ## v7.0.0
 This release is not fully backwards compatibility,
```

### Comparing `acconeer-exptool-7.0.1/Jenkinsfile` & `acconeer-exptool-7.0.2/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/LICENSE.md` & `acconeer-exptool-7.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/PKG-INFO` & `acconeer-exptool-7.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 7.0.1
+Version: 7.0.2
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
```

### Comparing `acconeer-exptool-7.0.1/README.md` & `acconeer-exptool-7.0.2/README.md`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/docker/Dockerfile` & `acconeer-exptool-7.0.2/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/dodo.py` & `acconeer-exptool-7.0.2/dodo.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/basic.py` & `acconeer-exptool-7.0.2/examples/a111/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/basic_continuous.py` & `acconeer-exptool-7.0.2/examples/a111/basic_continuous.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/load_record.py` & `acconeer-exptool-7.0.2/examples/a111/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/load_record_h5.m` & `acconeer-exptool-7.0.2/examples/a111/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/plotting/plot_with_matplotlib.py` & `acconeer-exptool-7.0.2/examples/a111/plotting/plot_with_matplotlib.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/plotting/plot_with_pyqtgraph.py` & `acconeer-exptool-7.0.2/examples/a111/plotting/plot_with_pyqtgraph.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/record_data/barebones.py` & `acconeer-exptool-7.0.2/examples/a111/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/record_data/long_duration_split_files.py` & `acconeer-exptool-7.0.2/examples/a111/record_data/long_duration_split_files.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/record_data/with_cli.py` & `acconeer-exptool-7.0.2/examples/a111/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/services/envelope.py` & `acconeer-exptool-7.0.2/examples/a111/services/envelope.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/services/iq.py` & `acconeer-exptool-7.0.2/examples/a111/services/iq.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/services/power_bins.py` & `acconeer-exptool-7.0.2/examples/a111/services/power_bins.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/services/sparse.py` & `acconeer-exptool-7.0.2/examples/a111/services/sparse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/utils/ping.py` & `acconeer-exptool-7.0.2/examples/a111/utils/ping.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a111/utils/test_throughput.py` & `acconeer-exptool-7.0.2/examples/a111/utils/test_throughput.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/basic.py` & `acconeer-exptool-7.0.2/examples/a121/basic.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/bilateration/bilaterator.py` & `acconeer-exptool-7.0.2/examples/a121/bilateration/bilaterator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/breathing/breathing.py` & `acconeer-exptool-7.0.2/examples/a121/breathing/breathing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/distance/detector.py` & `acconeer-exptool-7.0.2/examples/a121/distance/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/distance/processor.py` & `acconeer-exptool-7.0.2/examples/a121/distance/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/extended_config.py` & `acconeer-exptool-7.0.2/examples/a121/extended_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/load_record.py` & `acconeer-exptool-7.0.2/examples/a121/load_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/load_record_h5.m` & `acconeer-exptool-7.0.2/examples/a121/load_record_h5.m`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/phase_tracking/phase_tracking.py` & `acconeer-exptool-7.0.2/examples/a121/phase_tracking/phase_tracking.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/plot.py` & `acconeer-exptool-7.0.2/examples/a121/plot.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/presence/detector.py` & `acconeer-exptool-7.0.2/examples/a121/presence/detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/presence/processor.py` & `acconeer-exptool-7.0.2/examples/a121/presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/record_data/barebones.py` & `acconeer-exptool-7.0.2/examples/a121/record_data/barebones.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/record_data/with_cli.py` & `acconeer-exptool-7.0.2/examples/a121/record_data/with_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/reuse_calibration.py` & `acconeer-exptool-7.0.2/examples/a121/reuse_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/smart_presence/processor.py` & `acconeer-exptool-7.0.2/examples/a121/smart_presence/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/smart_presence/ref_app.py` & `acconeer-exptool-7.0.2/examples/a121/smart_presence/ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/stress.py` & `acconeer-exptool-7.0.2/examples/a121/stress.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/subsweeps.py` & `acconeer-exptool-7.0.2/examples/a121/subsweeps.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/surface_velocity/example_app.py` & `acconeer-exptool-7.0.2/examples/a121/surface_velocity/example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/surface_velocity/processor.py` & `acconeer-exptool-7.0.2/examples/a121/surface_velocity/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/touchless_button/processor.py` & `acconeer-exptool-7.0.2/examples/a121/touchless_button/processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/examples/a121/vibration/vibration.py` & `acconeer-exptool-7.0.2/examples/a121/vibration/vibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/gui/main.py` & `acconeer-exptool-7.0.2/gui/main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/noxfile.py` & `acconeer-exptool-7.0.2/noxfile.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/portable/make.py` & `acconeer-exptool-7.0.2/portable/make.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/portable/package/tools/update.py` & `acconeer-exptool-7.0.2/portable/package/tools/update.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/pyproject.toml` & `acconeer-exptool-7.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/setup.cfg` & `acconeer-exptool-7.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_bs_thread.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_bs_thread.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_pyusb/pyusbcomm.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_pyusb/pyusbcomm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_structs/configbase.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/configbase.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_structs/qtpidgets.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_structs/qtpidgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_tests/test_rig.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_tests/test_rig.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/LICENSE` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/LICENSE`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/__main__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/usb_cdc.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/usb_cdc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/winusb.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusb.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/winusbclasses.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/winusbpy.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbpy.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/_winusbcdc/winusbutils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/_winusbcdc/winusbutils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/base.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/client.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/client_factory.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/client_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/common.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/common.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/json/client.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/json/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/links.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/mock/client.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/mock/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/multiwrap.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/multiwrap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/client.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/data/regmap.yaml`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/protocol.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_clients/reg/regmap.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_clients/reg/regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_conf_to_rss_sdk.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_conf_to_rss_sdk.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_configs.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_modes.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_modes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/_utils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/_utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/_base/calibration.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_base/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/_base/module_info.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_base/module_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/_standalone_main.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/_standalone_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/breathing/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/breathing/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/breathing/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/button_press_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/calibration.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/distance_detector/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/distance_detector/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/calibration.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/envelope/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/envelope/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/iq/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/iq/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/iq/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/iq/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/obstacle_detection/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/parking/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/parking/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/parking/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/parking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/phase_tracking/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/phase_tracking/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/power_bins/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/power_bins/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/power_bins/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detect_human_only/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/presence_detection_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sleep_breathing/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_fft/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/sparse_inter_fft/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/speed_sparse/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/speed_sparse/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/tank_level_short/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/tank_level_short/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/utils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/_meta.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/algo/wave_to_exit/ui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a111/recording.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a111/recording.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/__init__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_cli.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_cli.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/__init__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/__init__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/config_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/sensor_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/session_config.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/session_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/subsweep_config.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/configs/validation_error.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/__init__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/client_info.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/client_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/metadata.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/metadata.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/record.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/result.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/result.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/sensor_calibration.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/server_info.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/server_info.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/stacked_results.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/entities/containers/utils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/entities/containers/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/mediators/link.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/link.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/mediators/recorder.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/mediators/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/client.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/common_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/communication_protocol.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_factory.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_latest.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_15_6_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_5_2_mhz.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/_no_calibration_reuse.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/erroneus_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/log_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/result_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/sensor_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/set_baudrate_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/setup_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/streaming_responses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/exploration_protocol/messages/system_info_response.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/links.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/links.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/message.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/mock_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/communication/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/record_io.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/recorder.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/session_schema.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/h5_record/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/peripherals/im_record/im_record.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core/utils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_core_ext/_replaying_client.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_core_ext/_replaying_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,18 +123,18 @@
         else:
             warnings.warn(f"Results of session {self._actual_session_idx} were not exhausted.")
 
         self._session_idx += 1
         self._is_started = False
 
     def attach_recorder(self, recorder: Recorder) -> None:
-        raise NotImplementedError
+        pass
 
     def detach_recorder(self) -> Optional[Recorder]:
-        raise NotImplementedError
+        return None
 
     def close(self) -> None:
         pass
 
     @property
     def connected(self) -> bool:
         return True
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_perf_calc.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_perf_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/_rate_calc.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/_rate_calc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/__init__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 )
 from ._utils import (
     APPROX_BASE_STEP_LENGTH_M,
     ENVELOPE_FWHM_M,
     NOISE_TEMPERATURE_MODEL_PARAMETER,
     PERCEIVED_WAVELENGTH,
     SIGNAL_TEMPERATURE_MODEL_PARAMETER,
+    double_buffering_frame_filter,
     find_peaks,
     get_approx_fft_vels,
     get_distance_filter_coeffs,
     get_distance_filter_edge_margin,
     get_distances_m,
     get_temperature_adjustment_factors,
     interpolate_peaks,
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_base.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/_a121.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_a121.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,22 @@
         self._replaying_client = None
         self._opened_record = None
 
     @is_task
     def load_from_file(self, *, path: Path) -> None:
         try:
             self._opened_record = a121.H5Record(h5py.File(path, mode="r"))
-            replaying_client = a121._ReplayingClient(self._opened_record)
+
+            # This is to be able to replay files recorded before v7.0.0
+            # when there were only one session per file
+            if self._opened_record.num_sessions <= 1:
+                replaying_client = a121._ReplayingClient(self._opened_record, cycled_session_idx=0)
+            else:
+                replaying_client = a121._ReplayingClient(self._opened_record)
+
             self.load_from_record_setup(record=self._opened_record)
         except Exception as exc:
             self._opened_record = None
             self._replaying_client = None
 
             self.callback(PluginStateMessage(state=PluginState.LOADED_IDLE))
             raise HandledException("Could not load from file") from exc
@@ -211,15 +218,22 @@
 
     @abc.abstractmethod
     def save_to_cache(self, file: h5py.File) -> None:
         pass
 
 
 class A121ViewPluginBase(ViewPluginBase):
-    pass
+    def _send_start_request(self) -> None:
+        A121BackendPluginBase.start_session.rpc(
+            self.app_model.put_task,
+            with_recorder=self.app_model.recording_enabled,
+        )
+
+    def _send_stop_request(self) -> None:
+        A121BackendPluginBase.stop_session.rpc(self.app_model.put_task)
 
 
 class A121PlotPluginBase(PlotPluginBase):
     def __init__(self, *, plot_layout: pg.GraphicsLayout, app_model: AppModel) -> None:
         super().__init__(plot_layout=plot_layout, app_model=app_model)
         self._is_setup = False
         self._plot_job: Optional[GeneralMessage] = None
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_null_app_model.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/_processor_main.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/backend_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     PLUGIN_PRESETS: Mapping[int, Callable[[], ProcessorPluginPreset[ProcessorConfigT]]] = {}
 
     def __init__(
         self, callback: Callable[[Message], None], generation: PluginGeneration, key: str
     ):
         super().__init__(callback=callback, generation=generation, key=key)
         self._processor_instance = None
-        self._log = BackendLogger.getLogger(__name__)
+        self._log: BackendLogger = BackendLogger.getLogger(__name__)
         self.restore_defaults()
 
     def _load_from_cache(self, file: h5py.File) -> None:
         self.shared_state.session_config = a121.SessionConfig.from_json(file["session_config"][()])
         self.shared_state.processor_config = self.get_processor_config_cls().from_json(
             file["processor_config"][()]
         )
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/plot_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/_plugins/processor/view_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import abc
 import logging
-from typing import Generic, Optional, Type
+from typing import Any, Generic, Optional, Type
 
 from PySide6.QtWidgets import QPushButton, QVBoxLayout, QWidget
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121.algo._base import ProcessorConfigT
 from acconeer.exptool.a121.algo._plugins._a121 import A121ViewPluginBase
 from acconeer.exptool.app.new import (
@@ -21,15 +21,15 @@
     PluginState,
     SessionConfigEditor,
     SmartMetadataView,
     SmartPerfCalcView,
     icons,
 )
 
-from .backend_plugin import ProcessorBackendPluginSharedState
+from .backend_plugin import ProcessorBackendPluginBase, ProcessorBackendPluginSharedState
 
 
 log = logging.getLogger(__name__)
 
 
 class ProcessorViewPluginBase(A121ViewPluginBase, Generic[ProcessorConfigT]):
     def __init__(self, app_model: AppModel, view_widget: QWidget) -> None:
@@ -78,21 +78,22 @@
         self.session_config_editor.sig_update.connect(self._on_session_config_update)
         scrolly_layout.addWidget(self.session_config_editor)
 
         self.sticky_widget.setLayout(sticky_layout)
         self.scrolly_widget.setLayout(scrolly_layout)
 
     def _on_session_config_update(self, session_config: a121.SessionConfig) -> None:
-        self.app_model.put_backend_plugin_task(
-            "update_session_config", {"session_config": session_config}
+        ProcessorBackendPluginBase.update_session_config.rpc(
+            self.app_model.put_task, session_config=session_config
         )
 
     def _on_processor_config_update(self, processor_config: ProcessorConfigT) -> None:
-        self.app_model.put_backend_plugin_task(
-            "update_processor_config", {"processor_config": processor_config}
+        ProcessorBackendPluginBase[ProcessorConfigT, Any].update_processor_config.rpc(
+            self.app_model.put_task,
+            processor_config=processor_config,
         )
 
     def on_backend_state_update(
         self,
         backend_plugin_state: Optional[
             ProcessorBackendPluginSharedState[ProcessorConfigT, a121.Metadata]
         ],
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/bilateration/_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -592,27 +592,27 @@
         )
         self.start_button.setEnabled(
             ready_for_session and detector_status.ready_to_start and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
     def _on_config_update(self, config: DetectorConfig) -> None:
-        self.app_model.put_backend_plugin_task("update_config", {"config": config})
+        BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
     def _on_processor_config_update(self, config: ProcessorConfig) -> None:
-        self.app_model.put_backend_plugin_task("update_processor_config", {"config": config})
+        BackendPlugin.update_processor_config.rpc(self.app_model.put_task, config=config)
 
     def _on_sensor_ids_update(self, sensor_ids: list[int]) -> None:
-        self.app_model.put_backend_plugin_task("update_sensor_ids", {"sensor_ids": sensor_ids})
+        BackendPlugin.update_sensor_ids.rpc(self.app_model.put_task, sensor_ids=sensor_ids)
 
     def _on_calibrate_detector(self) -> None:
-        self.app_model.put_backend_plugin_task("calibrate_detector")
+        BackendPlugin.calibrate_detector.rpc(self.app_model.put_task)
 
     def _send_defaults_request(self) -> None:
-        self.app_model.put_backend_plugin_task("restore_defaults")
+        BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
 
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
         return BackendPlugin(callback, generation=self.generation, key=key)
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/bilateration/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/bilateration/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/breathing/_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/breathing/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/breathing/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/__main__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_aggregator.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_aggregator.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_detector.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_detector.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_detector_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -568,26 +568,24 @@
             and config_valid
             and detector_status.ready_to_start
             and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
-        self.app_model.put_backend_plugin_task("update_sensor_ids", {"sensor_ids": [sensor_id]})
+        BackendPlugin.update_sensor_ids.rpc(self.app_model.put_task, sensor_ids=[sensor_id])
 
     def _on_config_update(self, config: DetectorConfig) -> None:
-        self.app_model.put_backend_plugin_task("update_config", {"config": config})
+        BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
     def _on_calibrate_detector(self) -> None:
-        self.app_model.put_backend_plugin_task(
-            "calibrate_detector", on_error=self.app_model.emit_error
-        )
+        BackendPlugin.calibrate_detector.rpc(self.app_model.put_task)
 
     def _send_defaults_request(self) -> None:
-        self.app_model.put_backend_plugin_task("restore_defaults")
+        BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
 
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
         return BackendPlugin(callback, generation=self.generation, key=key)
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_processors.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/distance/_serializers.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/distance/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/phase_tracking/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/_configs.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/_detector.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 
 import attrs
 import h5py
 import numpy as np
 import numpy.typing as npt
 
 from acconeer.exptool import a121
-from acconeer.exptool.a121._core.entities import Result
 from acconeer.exptool.a121._core.entities.configs.config_enums import IdleState, Profile
 from acconeer.exptool.a121._core.utils import is_divisor_of, is_multiple_of
 from acconeer.exptool.a121._h5_utils import _create_h5_string_dataset
 from acconeer.exptool.a121.algo import ENVELOPE_FWHM_M, AlgoConfigBase, Controller, select_prf
+from acconeer.exptool.a121.algo._utils import estimate_frame_rate
 
 from ._processors import Processor, ProcessorConfig, ProcessorContext, ProcessorExtraResult
 
 
 SPARSE_IQ_PPC = 24
 
 
@@ -200,51 +200,27 @@
     ) -> None:
         super().__init__(client=client, config=detector_config)
         self.sensor_id = sensor_id
         self.detector_metadata: Optional[DetectorMetadata] = None
 
         self.started = False
 
-    def _estimate_frame_rate(self) -> float:
-        delta_times = np.full(2, np.nan)
-
-        self.client.setup_session(self.session_config)
-        self.client.start_session()
-
-        for i in range(4):
-            result = self.client.get_next()
-            assert isinstance(result, Result)
-
-            if i < 2:
-                last_time = result.tick_time
-                continue
-
-            time = result.tick_time
-            delta = time - last_time
-            last_time = time
-            delta_times = np.roll(delta_times, -1)
-            delta_times[-1] = delta
-
-        self.client.stop_session()
-
-        return float(1.0 / np.nanmean(delta_times))
-
     def start(
         self, recorder: Optional[a121.Recorder] = None, _algo_group: Optional[h5py.Group] = None
     ) -> None:
         if self.started:
             raise RuntimeError("Already started")
 
         sensor_config = self._get_sensor_config(self.config)
         self.session_config = a121.SessionConfig(
             {self.sensor_id: sensor_config},
             extended=False,
         )
 
-        self.estimated_frame_rate = self._estimate_frame_rate()
+        self.estimated_frame_rate = estimate_frame_rate(self.client, self.session_config)
         # Add estimated frame rate to context if it differs more than 10% from the set frame rate
         if (
             np.abs(self.config.frame_rate - self.estimated_frame_rate) / self.config.frame_rate
             > 0.1
         ):
             context = ProcessorContext(estimated_frame_rate=self.estimated_frame_rate)
         else:
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_detector_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 class PluginPresetId(Enum):
     SHORT_RANGE = auto()
     MEDIUM_RANGE = auto()
     LONG_RANGE = auto()
 
 
 class BackendPlugin(DetectorBackendPluginBase[SharedState]):
-
     PLUGIN_PRESETS: Mapping[int, Callable[[], DetectorConfig]] = {
         PluginPresetId.SHORT_RANGE.value: lambda: get_short_range_config(),
         PluginPresetId.MEDIUM_RANGE.value: lambda: get_medium_range_config(),
         PluginPresetId.LONG_RANGE.value: lambda: get_long_range_config(),
     }
 
     def __init__(
@@ -624,21 +623,21 @@
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
     def _on_config_update(self, config: DetectorConfig) -> None:
-        self.app_model.put_backend_plugin_task("update_config", {"config": config})
+        BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
     def _send_defaults_request(self) -> None:
-        self.app_model.put_backend_plugin_task("restore_defaults")
+        BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
-        self.app_model.put_backend_plugin_task("update_sensor_id", {"sensor_id": sensor_id})
+        BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
 
 
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
         return BackendPlugin(callback=callback, generation=self.generation, key=key)
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/_processors.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_processors.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/presence/_serializers.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/presence/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/_configs.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_ref_app_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -506,24 +506,24 @@
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
     def _on_config_update(self, config: RefAppConfig) -> None:
-        self.app_model.put_backend_plugin_task("update_config", {"config": config})
+        BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
     def _on_plot_config_update(self, config: PlotConfig) -> None:
-        self.app_model.put_backend_plugin_task("update_plot_config", {"config": config})
+        BackendPlugin.update_plot_config.rpc(self.app_model.put_task, config=config)
 
     def _send_defaults_request(self) -> None:
-        self.app_model.put_backend_plugin_task("restore_defaults")
+        BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
-        self.app_model.put_backend_plugin_task("update_sensor_id", {"sensor_id": sensor_id})
+        BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
 
 
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
         return BackendPlugin(callback=callback, generation=self.generation, key=key)
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/smart_presence/_serializer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/sparse_iq/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_example_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_example_app_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,16 +283,16 @@
 
         self.upper_std_history = np.roll(self.upper_std_history, -1)
         self.upper_std_history[-1] = (
             example_app_result.velocity - 0.5 * processor_extra_result.peak_width
         )
         self.upper_std_curve.setData(xs, self.upper_std_history)
 
-        lim = self.psd_smooth_max.update(processor_extra_result.psd)
-        self.psd_plot.setYRange(np.log(0.5), np.log(lim))
+        lim = self.psd_smooth_max.update(processor_extra_result.psd_threshold)
+        self.psd_plot.setYRange(np.log10(0.2), np.log10(lim))
         self.psd_plot.setXRange(
             processor_extra_result.max_bin_vertical_vs[0],
             processor_extra_result.max_bin_vertical_vs[-1],
         )
         self.psd_curve.setData(
             processor_extra_result.vertical_velocities, processor_extra_result.psd
         )
@@ -533,21 +533,21 @@
 
         self.start_button.setEnabled(
             app_model.is_ready_for_session() and self.config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
     def _on_config_update(self, config: ExampleAppConfig) -> None:
-        self.app_model.put_backend_plugin_task("update_config", {"config": config})
+        BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
     def _send_defaults_request(self) -> None:
-        self.app_model.put_backend_plugin_task("restore_defaults")
+        BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
-        self.app_model.put_backend_plugin_task("update_sensor_id", {"sensor_id": sensor_id})
+        BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
 
 
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
         return BackendPlugin(callback=callback, generation=self.generation, key=key)
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/surface_velocity/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/_configs.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,14 @@
 
         self._recorder = None
         self._ref_app_instance: Optional[RefApp] = None
         self._log = BackendLogger.getLogger(__name__)
 
         self.restore_defaults()
 
-    @is_task
     def _load_from_cache(self, file: h5py.File) -> None:
         self.shared_state.config = RefAppConfig.from_json(file["config"][()])
         self.shared_state.context = RefAppContext.from_h5(file["context"])
 
     @is_task
     def restore_defaults(self) -> None:
         self.shared_state = SharedState(config=get_small_config())
@@ -674,36 +673,34 @@
             and config_valid
             and self.config_editor.is_ready
             and self.tank_level_config_editor.is_ready
         )
         self.stop_button.setEnabled(app_model.plugin_state == PluginState.LOADED_BUSY)
 
     def _on_sensor_id_update(self, sensor_id: int) -> None:
-        self.app_model.put_backend_plugin_task("update_sensor_id", {"sensor_id": sensor_id})
+        BackendPlugin.update_sensor_id.rpc(self.app_model.put_task, sensor_id=sensor_id)
 
     def _on_config_update(self, config: RefAppConfig) -> None:
-        self.app_model.put_backend_plugin_task("update_config", {"config": config})
+        BackendPlugin.update_config.rpc(self.app_model.put_task, config=config)
 
     # TODO: move to detector base (?)
     def _send_start_request(self) -> None:
-        self.app_model.put_backend_plugin_task(
-            "start_session",
-            {"with_recorder": self.app_model.recording_enabled},
-            on_error=self.app_model.emit_error,
+        BackendPlugin.start_session.rpc(
+            self.app_model.put_task, with_recorder=self.app_model.recording_enabled
         )
 
     # TODO: move to detector base (?)
     def _send_stop_request(self) -> None:
-        self.app_model.put_backend_plugin_task("stop_session", on_error=self.app_model.emit_error)
+        BackendPlugin.stop_session.rpc(self.app_model.put_task)
 
     def _on_calibrate_detector(self) -> None:
-        self.app_model.put_backend_plugin_task("calibrate_detector")
+        BackendPlugin.calibrate_detector.rpc(self.app_model.put_task)
 
     def _send_defaults_request(self) -> None:
-        self.app_model.put_backend_plugin_task("restore_defaults")
+        BackendPlugin.restore_defaults.rpc(self.app_model.put_task)
 
 
 class PluginSpec(PluginSpecBase):
     def create_backend_plugin(
         self, callback: Callable[[Message], None], key: str
     ) -> BackendPlugin:
         return BackendPlugin(callback, generation=self.generation, key=key)
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_processor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_ref_app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/tank_level/_serializer.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/tank_level/_serializer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_blinkstick_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/_configs.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_configs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,20 @@
 from typing import Optional
 
 import attrs
 import numpy as np
 import numpy.typing as npt
 
 from acconeer.exptool import a121
-from acconeer.exptool.a121.algo import AlgoParamEnum, AlgoProcessorConfigBase, ProcessorBase
+from acconeer.exptool.a121.algo import (
+    AlgoParamEnum,
+    AlgoProcessorConfigBase,
+    ProcessorBase,
+    double_buffering_frame_filter,
+)
 
 
 class MeasurementType(AlgoParamEnum):
     CLOSE_RANGE = enum.auto()
     FAR_RANGE = enum.auto()
     CLOSE_AND_FAR_RANGE = enum.auto()
 
@@ -158,15 +163,19 @@
 
         self._sig_count = np.zeros((2,))
         self._nonsig_count = np.array(
             [processor_config.patience_close + 1, processor_config.patience_far + 1],
         )
 
     def process(self, result: a121.Result) -> ProcessorResult:
-        frame = result.frame
+        if self._sensor_config.double_buffering:
+            frame = double_buffering_frame_filter(result.frame)
+        else:
+            frame = result.frame
+
         y = np.zeros_like(frame, dtype=float)
 
         sensitivity = self._get_sensitivity()
 
         if self._frames_since_last_cal > self._cal_interval_frames:
             self._calibrate()
         elif not np.any(np.isnan(self._cfar_ref_buf)):
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/touchless_button/_serializers.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/vibration/_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/_plugin.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/a121/algo/vibration/_processor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/a121/algo/vibration/_processor.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import numpy.typing as npt
 
 from acconeer.exptool import a121
 from acconeer.exptool.a121.algo import (
     APPROX_BASE_STEP_LENGTH_M,
     AlgoProcessorConfigBase,
     ProcessorBase,
+    double_buffering_frame_filter,
 )
 
 
 @attrs.mutable(kw_only=True)
 class ProcessorConfig(AlgoProcessorConfigBase):
     time_series_length: int = attrs.field(default=1024)
     """Length of time series."""
@@ -109,14 +110,15 @@
     ) -> None:
 
         processor_config.validate(sensor_config)
 
         # Should never happen, checked in validate
         assert sensor_config.sweep_rate is not None
 
+        self.double_buffering = sensor_config.double_buffering
         self.spf = sensor_config.sweeps_per_frame
         self.lp_coeffs = processor_config.lp_coeff
         self.sensitivity = processor_config.sensitivity
         self.time_series_length = processor_config.time_series_length
         self.amplitude_threshold = processor_config.amplitude_threshold
 
         self.time_series = np.zeros(shape=processor_config.time_series_length)
@@ -126,25 +128,30 @@
         )[1:]
         self.lp_z_abs_db = np.zeros_like(self.freq)
         self.window_length = self._WINDOW_BASE_LENGTH * self._OVER_SAMPLING_FACTOR
         self.half_guard_length = self._HALF_GUARD_BASE_LENGTH * self._OVER_SAMPLING_FACTOR
 
     def process(self, result: a121.Result) -> ProcessorResult:
 
-        max_amplitude = float(np.max(np.abs(result.frame)))
+        if self.double_buffering:
+            frame = double_buffering_frame_filter(result.frame)
+        else:
+            frame = result.frame
+
+        max_amplitude = float(np.max(np.abs(frame)))
 
         if max_amplitude < self.amplitude_threshold:
             return ProcessorResult(
                 result_available=False,
                 max_amplitude=max_amplitude,
                 amplitude_threshold=self.amplitude_threshold,
                 freqs=self.freq,
             )
 
-        new_data_segment = np.angle(result.frame.squeeze(axis=1))
+        new_data_segment = np.angle(frame.squeeze(axis=1))
 
         self.time_series = np.roll(self.time_series, -self.spf)
         self.time_series[-self.spf :] = new_data_segment
         self.time_series = np.unwrap(self.time_series)
 
         z_abs = np.abs(
             np.fft.rfft(
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/launcher.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/launcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/__init__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/_argument_parser.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/_enums.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_enums.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/_version_checker.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/_version_checker.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/app_model.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/app_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
+import functools
 import json
 import logging
 import queue
 import shutil
 import time
 from enum import Enum
 from pathlib import Path
@@ -35,16 +36,18 @@
     BackendPlugin,
     BackendPluginStateMessage,
     ClosedTask,
     ConnectionStateMessage,
     GeneralMessage,
     LogMessage,
     Message,
+    Model,
     PluginStateMessage,
     StatusMessage,
+    Task,
 )
 from acconeer.exptool.app.new.storage import get_config_dir, remove_temp_dir
 from acconeer.exptool.utils import CommDevice, SerialDevice, USBDevice  # type: ignore[import]
 
 from .plugin_protocols import PlotPluginInterface, ViewPluginInterface
 from .port_updater import PortUpdater
 
@@ -298,50 +301,30 @@
     def broadcast_backend_state(self) -> None:
         self.sig_backend_state_changed.emit(self.backend_plugin_state)
 
     def emit_error(self, exception: Exception, traceback_format_exc: Optional[str] = None) -> None:
         log.debug("Emitting error")
         self.sig_error.emit(exception, traceback_format_exc)
 
-    def _put_backend_task(
+    def put_task(
         self,
-        name: str,
-        kwargs: Optional[dict[str, Any]] = None,
+        task: Task,
         *,
-        plugin: bool = False,
         on_ok: Optional[Callable[[], None]] = None,
         on_error: Optional[Callable[[Exception, Optional[str]], None]] = None,
     ) -> None:
-        if kwargs is None:
-            kwargs = {}
-
-        key = self._backend.put_task((name, kwargs, plugin))
+        key = self._backend.put_task(task)
         self._backend_task_callbacks[key] = {
             "on_ok": on_ok,
             "on_error": on_error,
         }
 
+        (name, _) = task
         log.debug(f"Put backend task with name: '{name}', key: {key.time_low}")
 
-    def put_backend_plugin_task(
-        self,
-        name: str,
-        kwargs: Optional[dict[str, Any]] = None,
-        *,
-        on_ok: Optional[Callable[[], None]] = None,
-        on_error: Optional[Callable[[Exception, Optional[str]], None]] = None,
-    ) -> None:
-        self._put_backend_task(
-            name,
-            kwargs,
-            plugin=True,
-            on_ok=on_ok,
-            on_error=on_error or self.emit_error,
-        )
-
     def _handle_backend_closed_task(self, closed_task: ClosedTask) -> None:
         log.debug(f"Got backend closed task: {closed_task.key.time_low}")
 
         callbacks = self._backend_task_callbacks.pop(closed_task.key)
 
         if closed_task.exception:
             f = callbacks["on_error"]
@@ -581,28 +564,25 @@
             else:
                 open_client_parameters = {"usb_device": True}
         else:
             raise RuntimeError
 
         log.debug(f"Connecting client with {open_client_parameters}")
 
-        on_error = self.emit_error
-        if auto:
-            on_error = self._failed_autoconnect
-
-        self._put_backend_task(
-            "connect_client",
-            {"open_client_parameters": open_client_parameters},
-            on_error=on_error,
+        Model.connect_client.rpc(
+            functools.partial(
+                self.put_task, on_error=self._failed_autoconnect if auto else self.emit_error
+            ),
+            open_client_parameters=open_client_parameters,
         )
         self.connection_warning = None
         self.broadcast()
 
     def disconnect_client(self) -> None:
-        self._put_backend_task("disconnect_client", {})
+        Model.disconnect_client.rpc(self.put_task)
         self.connection_warning = None
         self._a121_server_info = None
         self.broadcast()
 
     def is_connect_ready(self) -> bool:
         return (
             (self.connection_interface == ConnectionInterface.SOCKET)
@@ -703,48 +683,38 @@
     def _unload_current_plugin(self) -> None:
         log.debug("AppModel is unloading its current plugin")
         self.sig_load_plugin.emit(None)
         self._update_saveable_file(None)
         self.backend_plugin_state = None
         self.broadcast()
 
-        self._put_backend_task("unload_plugin", {}, on_error=self.emit_error)
+        Model.unload_plugin.rpc(self.put_task)
 
     def load_plugin(self, plugin: Optional[PluginSpec]) -> None:
         log.debug(f"AppModel is loading the plugin {plugin}")
         if plugin == self.plugin:
             return
 
         self._unload_current_plugin()
 
         if plugin is not None:
-            self._put_backend_task(
-                "load_plugin",
-                {
-                    "plugin_factory": plugin.create_backend_plugin,
-                    "key": plugin.key,
-                },
-                on_error=self.emit_error,
+            Model.load_plugin.rpc(
+                self.put_task,
+                plugin_factory=plugin.create_backend_plugin,
+                key=plugin.key,
             )
-            self.put_backend_plugin_task("load_from_cache", {})
+            BackendPlugin.load_from_cache.rpc(self.put_task)
 
         self.sig_load_plugin.emit(plugin)
         self.plugin = plugin
         self.broadcast()
         self.broadcast_backend_state()
 
     def set_plugin_preset(self, preset_id: Enum) -> None:
-        self._put_backend_task(
-            "set_preset",
-            {
-                "preset_id": preset_id.value,
-            },
-            plugin=True,
-            on_error=self.emit_error,
-        )
+        BackendPlugin.set_preset.rpc(self.put_task, preset_id=preset_id.value)
 
     def save_to_file(self, path: Path) -> None:
         log.debug(f"{self.__class__.__name__} saving to file '{path}'")
 
         if self.saveable_file is None:
             raise RuntimeError
 
@@ -768,15 +738,15 @@
         except Exception:
             log.debug(f"Could not find plugin '{findings.key}'")
 
             # TODO: Don't hardcode
             plugin = self._find_plugin("sparse_iq")  # noqa: F841
 
         self.load_plugin(plugin)
-        self.put_backend_plugin_task("load_from_file", {"path": path}, on_error=self.emit_error)
+        BackendPlugin.load_from_file.rpc(self.put_task, path=path)
 
     def _find_plugin(self, find_key: Optional[str]) -> PluginSpec:  # TODO: Also find by generation
         if find_key is None:
             raise Exception
 
         return next(plugin for plugin in self.plugins if plugin.key == find_key)
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/app_model_listener.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/app_model_listener.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/file_detective.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/file_detective.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/app_model/port_updater.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/app_model/port_updater.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_application_client.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_application_client.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_backend.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,41 @@
-# Copyright (c) Acconeer AB, 2022
+# Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import logging
 import multiprocessing as mp
 import queue
 import time
 import traceback
 import uuid
 from multiprocessing.synchronize import Event as mp_EventType  # NOTE! this is not mp.Event.
-from typing import Any, Dict, Optional, Tuple, Union
+from typing import Optional, Tuple, Union
 
 import attrs
 import psutil
 from typing_extensions import Literal
 
 from ._backend_logger import BackendLogger
 from ._message import GeneralMessage, Message
 from ._model import Model
+from ._tasks import Task
 
 
 log = logging.getLogger(__name__)
 
 
 @attrs.frozen
 class ClosedTask:
     key: uuid.UUID = attrs.field()
     exception: Optional[Exception] = attrs.field(default=None)
     traceback_format_exc: Optional[str] = attrs.field(default=None)
 
 
-TaskName = str
-TaskPlugin = bool
-TaskKwargs = Dict[str, Any]
-Task = Tuple[TaskName, TaskKwargs, TaskPlugin]
-
 ToBackendQueueItem = Union[
     Tuple[Literal["stop"], None],
     Tuple[Literal["task"], Tuple[uuid.UUID, Task]],
 ]
 FromBackendQueueItem = Union[Message, ClosedTask]
 
 
@@ -156,18 +152,17 @@
 
             if cmd == "stop":
                 break
             elif cmd == "task":
                 assert maybe_key_and_task is not None
 
                 key, task = maybe_key_and_task
-                name, kwargs, plugin = task
 
                 try:
-                    model.execute_task(name, kwargs, plugin)
+                    model.execute_task(task)
                 except Exception as exc:
                     send_queue.put(ClosedTask(key, exc, traceback.format_exc()))
                 else:
                     send_queue.put(ClosedTask(key))
 
                 model_wants_to_idle = True
             else:
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_backend_logger.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend_logger.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_backend_plugin.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_backend_plugin.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Copyright (c) Acconeer AB, 2022-2023
 # All rights reserved
 
 from __future__ import annotations
 
 import abc
 from contextlib import contextmanager
+from pathlib import Path
 from typing import Any, Callable, Generic, Optional, TypeVar
 
 import h5py
 
 from acconeer.exptool.app.new import PluginGeneration
 from acconeer.exptool.app.new.storage import get_config_dir
 
 from ._message import BackendPluginStateMessage, Message, StatusMessage
+from ._tasks import is_task
 
 
 StateT = TypeVar("StateT")
 
 
 class BackendPlugin(abc.ABC, Generic[StateT]):
     shared_state: StateT
@@ -38,18 +40,29 @@
             file_path.parent.mkdir(parents=True, exist_ok=True)
 
         file_mode = "w" if write else "r"
         h5_file = h5py.File(file_path, file_mode)
         yield h5_file
         h5_file.close()
 
+    @is_task
     @abc.abstractmethod
     def load_from_cache(self) -> None:
         pass
 
+    @is_task
+    @abc.abstractmethod
+    def load_from_file(self, *, path: Path) -> None:
+        pass
+
+    @is_task
+    @abc.abstractmethod
+    def set_preset(self, preset_id: int) -> None:
+        pass
+
     @abc.abstractmethod
     def idle(self) -> bool:
         pass
 
     @abc.abstractmethod
     def attach_client(self, *, client: Any) -> None:
         pass
@@ -58,16 +71,12 @@
     def detach_client(self) -> None:
         pass
 
     @abc.abstractmethod
     def teardown(self) -> None:
         pass
 
-    @abc.abstractmethod
-    def set_preset(self, preset_id: int) -> None:
-        pass
-
     def broadcast(self) -> None:
         self.callback(BackendPluginStateMessage(state=self.shared_state))
 
     def send_status_message(self, message: Optional[str]) -> None:
         self.callback(StatusMessage(status=message))
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_message.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_message.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/backend/_model.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/backend/_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,29 +10,25 @@
 
 from acconeer.exptool import a121
 from acconeer.exptool.app.new._enums import ConnectionState, PluginState
 from acconeer.exptool.app.new._exceptions import HandledException
 
 from ._backend_plugin import BackendPlugin
 from ._message import ConnectionStateMessage, GeneralMessage, Message, PluginStateMessage
+from ._tasks import Task, get_task, is_task
 
 
 log = logging.getLogger(__name__)
 
 
 T = TypeVar("T")
 MessageHandler = Callable[[Message], None]
 BackendPluginFactory = Callable[[MessageHandler, str], BackendPlugin]
 
 
-def is_task(func: T) -> T:
-    setattr(func, "is_task", True)
-    return func
-
-
 class Model:
     backend_plugin: Optional[BackendPlugin[Any]]
     client: Optional[a121.Client]
 
     def __init__(self, task_callback: Callable[[Message], None]) -> None:
         self.backend_plugin = None
         self.client = None
@@ -40,31 +36,28 @@
 
     def idle(self) -> bool:
         if self.backend_plugin is None:
             return False
 
         return self.backend_plugin.idle()
 
-    def execute_task(self, name: str, kwargs: dict[str, Any], plugin: bool) -> None:
-        if plugin:
-            if self.backend_plugin is None:
-                raise RuntimeError
-
-            obj: Any = self.backend_plugin
-        else:
-            obj = self
-
-        try:
-            method = getattr(obj, name)
-            if not getattr(method, "is_task"):
-                raise Exception
-        except Exception:
-            raise RuntimeError(f"'{name}' is not a task")
+    def execute_task(self, task: Task) -> None:
+        (name, kwargs) = task
+
+        builtin_task = get_task(self, name)
+        if builtin_task is not None:
+            builtin_task(**kwargs)
+            return
+
+        plugin_task = get_task(self.backend_plugin, name)
+        if plugin_task is not None:
+            plugin_task(**kwargs)
+            return
 
-        method(**kwargs)
+        raise RuntimeError(f"'{name}' is not a task")
 
     @is_task
     def connect_client(self, open_client_parameters: Dict[str, Any]) -> None:
         if self.client is not None:
             raise RuntimeError(
                 "Model already has a Client. The current Client needs to be disconnected first."
             )
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/plugin_loader.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/plugin_loader.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -48,17 +48,7 @@
     @property
     def scrolly_widget(self) -> QWidget:
         """The scrolly widget. The scrolly area is located below the sticky area"""
         return self._scrolly_widget
 
     def handle_message(self, message: GeneralMessage) -> None:
         raise RuntimeError("ViewPlugins does not expect any messages ATM.")
-
-    def _send_start_request(self) -> None:
-        self.app_model.put_backend_plugin_task(
-            "start_session",
-            {"with_recorder": self.app_model.recording_enabled},
-            on_error=self.app_model.emit_error,
-        )
-
-    def _send_stop_request(self) -> None:
-        self.app_model.put_backend_plugin_task("stop_session", on_error=self.app_model.emit_error)
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/storage.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/storage.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/app_model_viewer.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/app_model_viewer.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/device_comboboxes.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/device_comboboxes.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/dialogs.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/flash_tab/threads.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/threads.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/flash_tab/widgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/help_tab.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/help_tab.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/icons.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/icons.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/main_window.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/main_window.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/misc.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/misc.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/attrs_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/collapsible_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/data_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/metadata_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/misc_error_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/perf_calc_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/hooks.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidget_groups.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/pidgets/pidgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/range_help_view.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/sensor_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/session_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/subsweep_config_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/two_sensor_ids_editor.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/plugin_components/utils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/plugin_components/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/status_bar.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/status_bar.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/connection_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/hints.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/hints.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/plugin_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/recording_widget.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/stream_tab/widgets.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/new/ui/utils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/new/ui/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/app.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/app.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/data_processing.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/data_processing.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/elements/helper.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/helper.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/elements/modules.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/modules.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/old/elements/qt_subclasses.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/old/elements/qt_subclasses.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/a111_gui.png` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/a111_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/a121_gui.png` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/a121_gui.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/icon-black.svg` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/icon-black.svg`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/icon.png` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/icon.png`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/app/resources/loader.gif` & `acconeer-exptool-7.0.2/src/acconeer/exptool/app/resources/loader.gif`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/LICENSE.txt` & `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/aarch64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll` & `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/amd64/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll` & `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/amd64/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44` & `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv6/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44` & `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/armv7/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll` & `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/i386/LibFT4222.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll` & `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/i386/ftd2xx.dll`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44` & `acconeer-exptool-7.0.2/src/acconeer/exptool/data/libft4222/x86_64/libft4222.so.1.4.4.44`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_bin_fetcher.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_bin_fetcher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_dev_license.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_dev_license.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_dev_license_tui.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_dev_license_tui.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_flasher.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_products.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_products.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_stm32uart/_stm32flasher.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/_bootloader_comm.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/flash/_xc120/_bootloader_tool.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/libft4222.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/libft4222.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/mpl_process.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/mpl_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/pg_process.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/pg_process.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/setup/__main__.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/__main__.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/platform_install.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/platform_install.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/prompts.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/prompts.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/setup_group.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/setup_group.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/setup_step.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/setup_step.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/setup/base/utils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/base/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/setup/cli/argument_parser.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/cli/argument_parser.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/setup/platforms/linux.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/linux.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/setup/platforms/ubuntu_20_04.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer/exptool/utils.py` & `acconeer-exptool-7.0.2/src/acconeer/exptool/utils.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/src/acconeer_exptool.egg-info/PKG-INFO` & `acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acconeer-exptool
-Version: 7.0.1
+Version: 7.0.2
 Summary: Acconeer Exploration Tool
 Home-page: https://github.com/acconeer/acconeer-python-exploration
 Author: Acconeer AB
 Author-email: tools@acconeer.com
 License: BSD 3-Clause Clear License
 Project-URL: Tracker, https://github.com/acconeer/acconeer-python-exploration/issues
 Project-URL: Documentation, https://acconeer-python-exploration.readthedocs.io
```

### Comparing `acconeer-exptool-7.0.1/src/acconeer_exptool.egg-info/SOURCES.txt` & `acconeer-exptool-7.0.2/src/acconeer_exptool.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -373,14 +373,15 @@
 src/acconeer/exptool/app/new/backend/__init__.py
 src/acconeer/exptool/app/new/backend/_application_client.py
 src/acconeer/exptool/app/new/backend/_backend.py
 src/acconeer/exptool/app/new/backend/_backend_logger.py
 src/acconeer/exptool/app/new/backend/_backend_plugin.py
 src/acconeer/exptool/app/new/backend/_message.py
 src/acconeer/exptool/app/new/backend/_model.py
+src/acconeer/exptool/app/new/backend/_tasks.py
 src/acconeer/exptool/app/new/pluginbase/__init__.py
 src/acconeer/exptool/app/new/pluginbase/plot_plugin_base.py
 src/acconeer/exptool/app/new/pluginbase/plugin_preset_base.py
 src/acconeer/exptool/app/new/pluginbase/plugin_spec_base.py
 src/acconeer/exptool/app/new/pluginbase/ui_plugin_base.py
 src/acconeer/exptool/app/new/pluginbase/view_plugin_base.py
 src/acconeer/exptool/app/new/ui/__init__.py
```

### Comparing `acconeer-exptool-7.0.1/tools/check_changelog.py` & `acconeer-exptool-7.0.2/tools/check_changelog.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,30 +83,39 @@
     if (
         get_number_of_matches_in_string(r"## " + VERSION_PATTERN, unreleased_changelog.read_text())
         > 0
     ):
         print("Unreleased Changelog contains illegal version tag headline")
         status = False
 
-    # First, we check if this is a "Prepare release" commit.
-    # If it's not, we check if the current commit is tagged.
-    current_tag = get_current_commit_prepare_release_version() or get_current_commit_tag()
+    # The version if this is a "Prepare release" commit.
+    prepare_release_version = get_current_commit_prepare_release_version()
 
-    if current_tag is None or Version(current_tag).is_prerelease:
+    # The current git tag
+    git_tag = get_current_commit_tag()
+
+    version_tag = prepare_release_version or git_tag
+
+    if version_tag is None or Version(version_tag).is_prerelease:
         exit(0 if status else 1)
 
-    print(f"Current commit is tagged ({current_tag}).")
+    if prepare_release_version is not None:
+        print(f"Current commit is a prepare commit for {prepare_release_version}.")
+    elif git_tag is not None:
+        print(f"Current commit is tagged ({git_tag}).")
+    else:
+        assert False
 
     first_match = get_first_match_in_string(VERSION_PATTERN, changelog.read_text())
     print(f'Found "{first_match}" in {FILE_PATH}', end=" ... ")
 
-    if first_match == current_tag:
-        print(f"Which matches {current_tag} exactly.")
+    if first_match == version_tag:
+        print(f"Which matches {version_tag} exactly.")
     else:
-        print(f'Which does not match "{current_tag}".')
+        print(f'Which does not match "{version_tag}".')
         status = False
 
     empty_unreleased_changelog = (
         "# Unreleased Changelog\n\n## Unreleased\n\n### Added\n\n### Changed\n\n### Fixed\n"
     )
 
     if unreleased_changelog.read_text() != empty_unreleased_changelog:
```

### Comparing `acconeer-exptool-7.0.1/tools/check_copyright.py` & `acconeer-exptool-7.0.2/tools/check_copyright.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/tools/check_line_length.py` & `acconeer-exptool-7.0.2/tools/check_line_length.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/tools/check_permissions.py` & `acconeer-exptool-7.0.2/tools/check_permissions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/tools/check_sdk_mentions.py` & `acconeer-exptool-7.0.2/tools/check_sdk_mentions.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/tools/check_whitespace.py` & `acconeer-exptool-7.0.2/tools/check_whitespace.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/tools/update_regmap.py` & `acconeer-exptool-7.0.2/tools/update_regmap.py`

 * *Files identical despite different names*

### Comparing `acconeer-exptool-7.0.1/utils/convert_to_csv.py` & `acconeer-exptool-7.0.2/utils/convert_to_csv.py`

 * *Files identical despite different names*

