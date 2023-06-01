# Comparing `tmp/nenupy-2.1.0.tar.gz` & `tmp/nenupy-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nenupy-2.1.0.tar", last modified: Mon Jan 31 12:51:29 2022, max compression
+gzip compressed data, was "/Users/aloh/Documents/GitHub/nenupy/dist/.tmp-t2sf1g8j/nenupy-2.2.9.tar", last modified: Thu Jun  1 12:54:02 2023, max compression
```

## Comparing `nenupy-2.1.0.tar` & `nenupy-2.2.9.tar`

### file list

```diff
@@ -1,93 +1,102 @@
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/
--rw-r--r--   0 aloh       (502) staff       (20)      523 2021-11-12 13:44:32.000000 nenupy-2.1.0/MANIFEST.in
--rw-r--r--   0 aloh       (502) staff       (20)      375 2022-01-31 12:51:29.000000 nenupy-2.1.0/PKG-INFO
--rw-r--r--   0 aloh       (502) staff       (20)     1324 2020-04-29 09:51:54.000000 nenupy-2.1.0/README.md
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/bin/
--rw-r--r--   0 aloh       (502) staff       (20)    25281 2021-02-04 12:50:28.000000 nenupy-2.1.0/bin/nenupy_vcr_coordinates
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/
--rw-r--r--   0 aloh       (502) staff       (20)     5532 2022-01-31 12:44:22.000000 nenupy-2.1.0/nenupy/__init__.py
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/astro/
--rw-r--r--   0 aloh       (502) staff       (20)       73 2021-11-05 12:27:43.000000 nenupy-2.1.0/nenupy/astro/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)    22326 2022-01-27 16:22:02.000000 nenupy-2.1.0/nenupy/astro/astro_tools.py
--rw-r--r--   0 aloh       (502) staff       (20)    28036 2022-01-31 10:42:43.000000 nenupy-2.1.0/nenupy/astro/pointing.py
--rw-r--r--   0 aloh       (502) staff       (20)    32462 2022-01-25 16:20:49.000000 nenupy-2.1.0/nenupy/astro/sky.py
--rw-r--r--   0 aloh       (502) staff       (20)     3742 2021-11-05 12:17:04.000000 nenupy-2.1.0/nenupy/astro/skymodel.py
--rw-r--r--   0 aloh       (502) staff       (20)    38445 2021-11-09 13:07:02.000000 nenupy-2.1.0/nenupy/astro/target.py
--rw-r--r--   0 aloh       (502) staff       (20)     2572 2022-01-25 10:41:26.000000 nenupy-2.1.0/nenupy/astro/uvw.py
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/astro_old/
--rw-r--r--   0 aloh       (502) staff       (20)     8618 2020-10-07 15:54:09.000000 nenupy-2.1.0/nenupy/astro_old/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)    39980 2021-11-05 13:00:15.000000 nenupy-2.1.0/nenupy/astro_old/astro.py
--rw-r--r--   0 aloh       (502) staff       (20)    26534 2021-11-05 12:59:47.000000 nenupy-2.1.0/nenupy/astro_old/hpxsky.py
--rw-r--r--   0 aloh       (502) staff       (20)     2709 2020-07-20 16:40:48.000000 nenupy-2.1.0/nenupy/astro_old/radio_sources.json
--rw-r--r--   0 aloh       (502) staff       (20)     4651 2020-10-29 14:40:34.000000 nenupy-2.1.0/nenupy/base.py
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/beam/
--rw-r--r--   0 aloh       (502) staff       (20)      218 2020-05-21 08:35:43.000000 nenupy-2.1.0/nenupy/beam/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)    15725 2021-06-23 15:27:06.000000 nenupy-2.1.0/nenupy/beam/beam.py
--rw-r--r--   0 aloh       (502) staff       (20)    18445 2021-08-05 11:47:25.000000 nenupy-2.1.0/nenupy/beam/hpxbeam.py
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/beamlet/
--rw-r--r--   0 aloh       (502) staff       (20)      308 2020-05-21 08:35:01.000000 nenupy-2.1.0/nenupy/beamlet/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)     2807 2020-11-04 13:45:53.000000 nenupy-2.1.0/nenupy/beamlet/beamlet.py
--rw-r--r--   0 aloh       (502) staff       (20)    20410 2021-09-13 14:32:07.000000 nenupy-2.1.0/nenupy/beamlet/bstdata.py
--rw-r--r--   0 aloh       (502) staff       (20)    19521 2021-12-07 14:42:28.000000 nenupy-2.1.0/nenupy/beamlet/sdata.py
--rw-r--r--   0 aloh       (502) staff       (20)    21329 2021-11-11 09:44:28.000000 nenupy-2.1.0/nenupy/beamlet/sstdata.py
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/instru/
--rw-r--r--   0 aloh       (502) staff       (20)  3156480 2019-10-13 07:36:22.000000 nenupy-2.1.0/nenupy/instru/NenuFAR_Ant_Hpx.fits
--rw-r--r--   0 aloh       (502) staff       (20)      915 2021-11-12 10:51:46.000000 nenupy-2.1.0/nenupy/instru/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)     9389 2022-01-28 16:45:54.000000 nenupy-2.1.0/nenupy/instru/instrument_tools.py
--rw-r--r--   0 aloh       (502) staff       (20)    37703 2022-01-25 09:23:27.000000 nenupy-2.1.0/nenupy/instru/interferometer.py
--rw-r--r--   0 aloh       (502) staff       (20)     2510 2021-11-12 10:22:32.000000 nenupy-2.1.0/nenupy/instru/low_noise_amplifier.json
--rw-r--r--   0 aloh       (502) staff       (20)     1770 2021-10-01 14:40:39.000000 nenupy-2.1.0/nenupy/instru/miniarray_antennas.json
--rw-r--r--   0 aloh       (502) staff       (20)    47735 2022-01-25 09:16:53.000000 nenupy-2.1.0/nenupy/instru/nenufar.py
--rw-r--r--   0 aloh       (502) staff       (20)    26776 2021-10-25 11:00:08.000000 nenupy-2.1.0/nenupy/instru/nenufar_array.json
--rw-r--r--   0 aloh       (502) staff       (20)     4796 2021-11-04 09:34:34.000000 nenupy-2.1.0/nenupy/instru/squint_table.sav
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/instru_old/
--rw-r--r--   0 aloh       (502) staff       (20)       68 2020-10-27 17:06:58.000000 nenupy-2.1.0/nenupy/instru_old/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)  1572887 2019-06-19 15:22:15.000000 nenupy-2.1.0/nenupy/instru_old/cal_pz_2_multi_2019-02-23.dat
--rw-r--r--   0 aloh       (502) staff       (20)    53736 2021-08-04 08:32:42.000000 nenupy-2.1.0/nenupy/instru_old/instru.py
--rw-r--r--   0 aloh       (502) staff       (20)     4796 2019-10-13 07:36:22.000000 nenupy-2.1.0/nenupy/instru_old/squint_table.sav
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/io/
--rw-r--r--   0 aloh       (502) staff       (20)       45 2021-12-01 16:27:12.000000 nenupy-2.1.0/nenupy/io/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)     8710 2022-01-31 12:42:17.000000 nenupy-2.1.0/nenupy/io/bst.py
--rw-r--r--   0 aloh       (502) staff       (20)     3936 2022-01-31 09:14:21.000000 nenupy-2.1.0/nenupy/io/io_tools.py
--rw-r--r--   0 aloh       (502) staff       (20)    49739 2022-01-31 12:43:40.000000 nenupy-2.1.0/nenupy/io/xst.py
--rw-r--r--   0 aloh       (502) staff       (20)     2646 2020-10-07 16:52:55.000000 nenupy-2.1.0/nenupy/miscellaneous.py
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/observation/
--rw-r--r--   0 aloh       (502) staff       (20)      528 2021-11-05 12:59:05.000000 nenupy-2.1.0/nenupy/observation/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)    71982 2022-01-05 11:16:27.000000 nenupy-2.1.0/nenupy/observation/obs_config.py
--rw-r--r--   0 aloh       (502) staff       (20)    38312 2022-01-19 11:54:54.000000 nenupy-2.1.0/nenupy/observation/parset.py
--rw-r--r--   0 aloh       (502) staff       (20)     9708 2022-01-20 11:00:57.000000 nenupy-2.1.0/nenupy/observation/parset_user_options.json
--rw-r--r--   0 aloh       (502) staff       (20)    14669 2021-11-05 12:58:52.000000 nenupy-2.1.0/nenupy/observation/pointing_obs.py
--rw-r--r--   0 aloh       (502) staff       (20)    31747 2021-11-05 12:55:12.000000 nenupy-2.1.0/nenupy/observation/sqldatabase.py
--rw-r--r--   0 aloh       (502) staff       (20)    14616 2020-07-16 11:29:02.000000 nenupy-2.1.0/nenupy/observation/tapdatabase.py
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/schedule/
--rw-r--r--   0 aloh       (502) staff       (20)      432 2021-02-26 12:53:50.000000 nenupy-2.1.0/nenupy/schedule/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)    33101 2022-01-19 11:05:42.000000 nenupy-2.1.0/nenupy/schedule/constraints.py
--rw-r--r--   0 aloh       (502) staff       (20)    12383 2022-01-11 10:31:54.000000 nenupy-2.1.0/nenupy/schedule/contamination.py
--rw-r--r--   0 aloh       (502) staff       (20)    16215 2021-11-13 16:35:22.000000 nenupy-2.1.0/nenupy/schedule/geneticalgo.py
--rw-r--r--   0 aloh       (502) staff       (20)    23271 2021-11-13 17:42:52.000000 nenupy-2.1.0/nenupy/schedule/obsblocks.py
--rw-r--r--   0 aloh       (502) staff       (20)    41201 2021-11-18 08:36:44.000000 nenupy-2.1.0/nenupy/schedule/schedule.py
--rw-r--r--   0 aloh       (502) staff       (20)     9406 2021-03-08 17:26:45.000000 nenupy-2.1.0/nenupy/schedule/targets.py
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/simulation/
--rw-r--r--   0 aloh       (502) staff       (20)      159 2020-05-21 08:35:48.000000 nenupy-2.1.0/nenupy/simulation/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)    19179 2020-04-17 13:49:39.000000 nenupy-2.1.0/nenupy/simulation/hpxsimu.py
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/skymodel/
--rw-r--r--   0 aloh       (502) staff       (20)      268 2021-11-25 14:33:44.000000 nenupy-2.1.0/nenupy/skymodel/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)     5367 2020-05-09 15:34:40.000000 nenupy-2.1.0/nenupy/skymodel/hpxgsm.py
--rw-r--r--   0 aloh       (502) staff       (20)     3739 2020-04-23 15:44:26.000000 nenupy-2.1.0/nenupy/skymodel/hpxlofar.py
--rw-r--r--   0 aloh       (502) staff       (20)  3539520 2020-04-06 16:17:35.000000 nenupy-2.1.0/nenupy/skymodel/lfsky.fits
--rw-r--r--   0 aloh       (502) staff       (20)     8705 2020-10-23 09:47:00.000000 nenupy-2.1.0/nenupy/skymodel/pointsource.py
--rw-r--r--   0 aloh       (502) staff       (20)       99 2021-09-16 09:10:00.000000 nenupy-2.1.0/nenupy/telescopes.json
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy/undysputed/
--rw-r--r--   0 aloh       (502) staff       (20)      217 2020-05-21 08:36:38.000000 nenupy-2.1.0/nenupy/undysputed/__init__.py
--rw-r--r--   0 aloh       (502) staff       (20)    79962 2019-09-11 14:11:38.000000 nenupy-2.1.0/nenupy/undysputed/bandpass_coeffs.dat
--rw-r--r--   0 aloh       (502) staff       (20)    58838 2021-11-18 15:32:52.000000 nenupy-2.1.0/nenupy/undysputed/dynspec.py
--rw-r--r--   0 aloh       (502) staff       (20)     7848 2020-06-24 10:02:05.000000 nenupy-2.1.0/nenupy/undysputed/waveform.py
-drwxr-xr-x   0 aloh       (502) staff       (20)        0 2022-01-31 12:51:29.000000 nenupy-2.1.0/nenupy.egg-info/
--rw-r--r--   0 aloh       (502) staff       (20)      375 2022-01-31 12:51:27.000000 nenupy-2.1.0/nenupy.egg-info/PKG-INFO
--rw-r--r--   0 aloh       (502) staff       (20)     2081 2022-01-31 12:51:28.000000 nenupy-2.1.0/nenupy.egg-info/SOURCES.txt
--rw-r--r--   0 aloh       (502) staff       (20)        1 2022-01-31 12:51:27.000000 nenupy-2.1.0/nenupy.egg-info/dependency_links.txt
--rw-r--r--   0 aloh       (502) staff       (20)        1 2020-04-29 08:15:12.000000 nenupy-2.1.0/nenupy.egg-info/not-zip-safe
--rw-r--r--   0 aloh       (502) staff       (20)      107 2022-01-31 12:51:27.000000 nenupy-2.1.0/nenupy.egg-info/requires.txt
--rw-r--r--   0 aloh       (502) staff       (20)        7 2022-01-31 12:51:27.000000 nenupy-2.1.0/nenupy.egg-info/top_level.txt
--rw-r--r--   0 aloh       (502) staff       (20)       38 2022-01-31 12:51:29.000000 nenupy-2.1.0/setup.cfg
--rw-r--r--   0 aloh       (502) staff       (20)     1421 2021-11-13 18:05:34.000000 nenupy-2.1.0/setup.py
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:54:02.000000 nenupy-2.2.9/
+-rw-r--r--   0 aloh       (502) staff       (20)     1073 2019-10-13 07:36:21.000000 nenupy-2.2.9/LICENSE
+-rw-r--r--   0 aloh       (502) staff       (20)      669 2022-02-01 18:14:22.000000 nenupy-2.2.9/MANIFEST.in
+-rw-r--r--   0 aloh       (502) staff       (20)     1830 2023-06-01 12:54:02.000000 nenupy-2.2.9/PKG-INFO
+-rw-r--r--   0 aloh       (502) staff       (20)     1324 2020-04-29 09:51:54.000000 nenupy-2.2.9/README.md
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:53:58.000000 nenupy-2.2.9/bin/
+-rw-r--r--   0 aloh       (502) staff       (20)     4160 2023-05-25 13:33:25.000000 nenupy-2.2.9/bin/nenupy_parallactic_correction
+-rw-r--r--   0 aloh       (502) staff       (20)    25281 2021-02-04 12:50:28.000000 nenupy-2.2.9/bin/nenupy_vcr_coordinates
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:53:58.000000 nenupy-2.2.9/nenupy/
+-rw-r--r--   0 aloh       (502) staff       (20)     5532 2023-05-30 12:25:59.000000 nenupy-2.2.9/nenupy/__init__.py
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:53:58.000000 nenupy-2.2.9/nenupy/astro/
+-rw-r--r--   0 aloh       (502) staff       (20)      230 2022-02-01 18:08:41.000000 nenupy-2.2.9/nenupy/astro/__init__.py
+-rw-r--r--   0 aloh       (502) staff       (20)    39865 2023-02-02 10:26:44.000000 nenupy-2.2.9/nenupy/astro/astro_tools.py
+-rw-r--r--   0 aloh       (502) staff       (20)     3653 2023-05-25 13:33:44.000000 nenupy-2.2.9/nenupy/astro/beam_correction.py
+-rw-r--r--   0 aloh       (502) staff       (20)      452 2022-02-01 18:18:31.000000 nenupy-2.2.9/nenupy/astro/common_sources.json
+-rw-r--r--   0 aloh       (502) staff       (20)    17680 2023-05-22 16:09:49.000000 nenupy-2.2.9/nenupy/astro/jones_mueller.py
+-rw-r--r--   0 aloh       (502) staff       (20)    30840 2022-11-08 09:51:12.000000 nenupy-2.2.9/nenupy/astro/pointing.py
+-rw-r--r--   0 aloh       (502) staff       (20)    33563 2023-01-24 15:55:44.000000 nenupy-2.2.9/nenupy/astro/sky.py
+-rw-r--r--   0 aloh       (502) staff       (20)     3742 2022-02-09 10:45:35.000000 nenupy-2.2.9/nenupy/astro/skymodel.py
+-rw-r--r--   0 aloh       (502) staff       (20)    40370 2022-05-11 09:12:51.000000 nenupy-2.2.9/nenupy/astro/target.py
+-rw-r--r--   0 aloh       (502) staff       (20)    16531 2022-12-14 13:46:45.000000 nenupy-2.2.9/nenupy/astro/uvw.py
+-rw-r--r--   0 aloh       (502) staff       (20)     4651 2020-10-29 14:40:34.000000 nenupy-2.2.9/nenupy/base.py
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:53:58.000000 nenupy-2.2.9/nenupy/beamlet/
+-rw-r--r--   0 aloh       (502) staff       (20)      308 2020-05-21 08:35:01.000000 nenupy-2.2.9/nenupy/beamlet/__init__.py
+-rw-r--r--   0 aloh       (502) staff       (20)     2807 2020-11-04 13:45:53.000000 nenupy-2.2.9/nenupy/beamlet/beamlet.py
+-rw-r--r--   0 aloh       (502) staff       (20)    20410 2021-09-13 14:32:07.000000 nenupy-2.2.9/nenupy/beamlet/bstdata.py
+-rw-r--r--   0 aloh       (502) staff       (20)    19553 2022-02-14 15:25:28.000000 nenupy-2.2.9/nenupy/beamlet/sdata.py
+-rw-r--r--   0 aloh       (502) staff       (20)    21329 2021-11-11 09:44:28.000000 nenupy-2.2.9/nenupy/beamlet/sstdata.py
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:54:01.000000 nenupy-2.2.9/nenupy/instru/
+-rw-r--r--   0 aloh       (502) staff       (20)  3156480 2019-10-13 07:36:22.000000 nenupy-2.2.9/nenupy/instru/NenuFAR_Ant_Hpx.fits
+-rw-r--r--   0 aloh       (502) staff       (20)      915 2021-11-12 10:51:46.000000 nenupy-2.2.9/nenupy/instru/__init__.py
+-rw-r--r--   0 aloh       (502) staff       (20)  1572887 2019-06-19 15:22:15.000000 nenupy-2.2.9/nenupy/instru/cal_pz_2_multi_2019-02-23.dat
+-rw-r--r--   0 aloh       (502) staff       (20)  1572887 2022-01-19 19:25:30.000000 nenupy-2.2.9/nenupy/instru/cal_table_NDPPP-24sep2021-freq-all-MR6_V1_20220118.dat
+-rw-r--r--   0 aloh       (502) staff       (20)  1572887 2022-01-20 15:59:15.000000 nenupy-2.2.9/nenupy/instru/cal_table_NDPPP-24sep2021-freq-all-MR6_V1_20220120.dat
+-rw-r--r--   0 aloh       (502) staff       (20)    12149 2022-02-14 15:46:18.000000 nenupy-2.2.9/nenupy/instru/instrument_tools.py
+-rw-r--r--   0 aloh       (502) staff       (20)    42028 2023-05-30 14:10:49.000000 nenupy-2.2.9/nenupy/instru/interferometer.py
+-rw-r--r--   0 aloh       (502) staff       (20)     2510 2021-11-12 10:22:32.000000 nenupy-2.2.9/nenupy/instru/low_noise_amplifier.json
+-rw-r--r--   0 aloh       (502) staff       (20)     1770 2021-10-01 14:40:39.000000 nenupy-2.2.9/nenupy/instru/miniarray_antennas.json
+-rw-r--r--   0 aloh       (502) staff       (20)     3420 2022-11-17 16:27:40.000000 nenupy-2.2.9/nenupy/instru/nda.py
+-rw-r--r--   0 aloh       (502) staff       (20)    50480 2023-02-08 16:34:48.000000 nenupy-2.2.9/nenupy/instru/nenufar.py
+-rw-r--r--   0 aloh       (502) staff       (20)    26776 2021-10-25 11:00:08.000000 nenupy-2.2.9/nenupy/instru/nenufar_array.json
+-rw-r--r--   0 aloh       (502) staff       (20)     4796 2021-11-04 09:34:34.000000 nenupy-2.2.9/nenupy/instru/squint_table.sav
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:54:01.000000 nenupy-2.2.9/nenupy/io/
+-rw-r--r--   0 aloh       (502) staff       (20)       45 2021-12-01 16:27:12.000000 nenupy-2.2.9/nenupy/io/__init__.py
+-rw-r--r--   0 aloh       (502) staff       (20)     9749 2022-05-09 15:45:16.000000 nenupy-2.2.9/nenupy/io/bst.py
+-rw-r--r--   0 aloh       (502) staff       (20)    44569 2022-11-17 15:17:21.000000 nenupy-2.2.9/nenupy/io/io_tools.py
+-rw-r--r--   0 aloh       (502) staff       (20)      394 2022-02-04 18:03:32.000000 nenupy-2.2.9/nenupy/io/nenufar_tv_sources.json
+-rw-r--r--   0 aloh       (502) staff       (20)     6216 2022-02-24 14:39:30.000000 nenupy-2.2.9/nenupy/io/sst.py
+-rw-r--r--   0 aloh       (502) staff       (20)    60385 2022-11-17 16:21:01.000000 nenupy-2.2.9/nenupy/io/xst.py
+-rw-r--r--   0 aloh       (502) staff       (20)     2646 2020-10-07 16:52:55.000000 nenupy-2.2.9/nenupy/miscellaneous.py
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:54:01.000000 nenupy-2.2.9/nenupy/observation/
+-rw-r--r--   0 aloh       (502) staff       (20)      530 2022-02-02 10:02:33.000000 nenupy-2.2.9/nenupy/observation/__init__.py
+-rw-r--r--   0 aloh       (502) staff       (20)    71683 2022-04-13 20:13:52.000000 nenupy-2.2.9/nenupy/observation/obs_config.py
+-rw-r--r--   0 aloh       (502) staff       (20)     3341 2022-02-22 10:11:30.000000 nenupy-2.2.9/nenupy/observation/obs_tools.py
+-rw-r--r--   0 aloh       (502) staff       (20)    84438 2022-12-09 15:09:27.000000 nenupy-2.2.9/nenupy/observation/parset.py
+-rw-r--r--   0 aloh       (502) staff       (20)    14503 2023-04-11 09:41:18.000000 nenupy-2.2.9/nenupy/observation/parset_user_options.json
+-rw-r--r--   0 aloh       (502) staff       (20)    31743 2022-02-02 09:58:28.000000 nenupy-2.2.9/nenupy/observation/sqldatabase.py
+-rw-r--r--   0 aloh       (502) staff       (20)    14616 2020-07-16 11:29:02.000000 nenupy-2.2.9/nenupy/observation/tapdatabase.py
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:54:01.000000 nenupy-2.2.9/nenupy/schedule/
+-rw-r--r--   0 aloh       (502) staff       (20)      478 2022-12-04 11:21:57.000000 nenupy-2.2.9/nenupy/schedule/__init__.py
+-rw-r--r--   0 aloh       (502) staff       (20)    38857 2023-05-30 13:09:22.000000 nenupy-2.2.9/nenupy/schedule/constraints.py
+-rw-r--r--   0 aloh       (502) staff       (20)    16325 2023-01-10 09:24:53.000000 nenupy-2.2.9/nenupy/schedule/contamination.py
+-rw-r--r--   0 aloh       (502) staff       (20)    16215 2021-11-13 16:35:22.000000 nenupy-2.2.9/nenupy/schedule/geneticalgo.py
+-rw-r--r--   0 aloh       (502) staff       (20)    25925 2023-05-30 13:02:39.000000 nenupy-2.2.9/nenupy/schedule/obsblocks.py
+-rw-r--r--   0 aloh       (502) staff       (20)    60190 2023-05-30 13:15:50.000000 nenupy-2.2.9/nenupy/schedule/schedule.py
+-rw-r--r--   0 aloh       (502) staff       (20)     9648 2023-05-30 13:02:27.000000 nenupy-2.2.9/nenupy/schedule/targets.py
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:54:01.000000 nenupy-2.2.9/nenupy/skymodel/
+-rw-r--r--   0 aloh       (502) staff       (20)      268 2021-11-25 14:33:44.000000 nenupy-2.2.9/nenupy/skymodel/__init__.py
+-rw-r--r--   0 aloh       (502) staff       (20)     5367 2020-05-09 15:34:40.000000 nenupy-2.2.9/nenupy/skymodel/hpxgsm.py
+-rw-r--r--   0 aloh       (502) staff       (20)     3739 2020-04-23 15:44:26.000000 nenupy-2.2.9/nenupy/skymodel/hpxlofar.py
+-rw-r--r--   0 aloh       (502) staff       (20)  3539520 2020-04-06 16:17:35.000000 nenupy-2.2.9/nenupy/skymodel/lfsky.fits
+-rw-r--r--   0 aloh       (502) staff       (20)     8705 2020-10-23 09:47:00.000000 nenupy-2.2.9/nenupy/skymodel/pointsource.py
+-rw-r--r--   0 aloh       (502) staff       (20)      103 2022-08-25 13:42:22.000000 nenupy-2.2.9/nenupy/telescopes.json
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:54:01.000000 nenupy-2.2.9/nenupy/undysputed/
+-rw-r--r--   0 aloh       (502) staff       (20)      217 2020-05-21 08:36:38.000000 nenupy-2.2.9/nenupy/undysputed/__init__.py
+-rw-r--r--   0 aloh       (502) staff       (20)    79962 2019-09-11 14:11:38.000000 nenupy-2.2.9/nenupy/undysputed/bandpass_coeffs.dat
+-rw-r--r--   0 aloh       (502) staff       (20)    59623 2022-09-13 08:25:59.000000 nenupy-2.2.9/nenupy/undysputed/dynspec.py
+-rw-r--r--   0 aloh       (502) staff       (20)     7848 2020-06-24 10:02:05.000000 nenupy-2.2.9/nenupy/undysputed/waveform.py
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:53:58.000000 nenupy-2.2.9/nenupy.egg-info/
+-rw-r--r--   0 aloh       (502) staff       (20)     1830 2023-06-01 12:53:58.000000 nenupy-2.2.9/nenupy.egg-info/PKG-INFO
+-rw-r--r--   0 aloh       (502) staff       (20)     2447 2023-06-01 12:53:58.000000 nenupy-2.2.9/nenupy.egg-info/SOURCES.txt
+-rw-r--r--   0 aloh       (502) staff       (20)        1 2023-06-01 12:53:58.000000 nenupy-2.2.9/nenupy.egg-info/dependency_links.txt
+-rw-r--r--   0 aloh       (502) staff       (20)       69 2023-06-01 12:53:58.000000 nenupy-2.2.9/nenupy.egg-info/requires.txt
+-rw-r--r--   0 aloh       (502) staff       (20)        7 2023-06-01 12:53:58.000000 nenupy-2.2.9/nenupy.egg-info/top_level.txt
+-rw-r--r--   0 aloh       (502) staff       (20)      988 2023-05-24 11:50:31.000000 nenupy-2.2.9/pyproject.toml
+-rw-r--r--   0 aloh       (502) staff       (20)       38 2023-06-01 12:54:02.000000 nenupy-2.2.9/setup.cfg
+drwxr-xr-x   0 aloh       (502) staff       (20)        0 2023-06-01 12:54:02.000000 nenupy-2.2.9/tests/
+-rw-r--r--   0 aloh       (502) staff       (20)     9584 2022-02-08 14:55:33.000000 nenupy-2.2.9/tests/test_astro_pointing.py
+-rw-r--r--   0 aloh       (502) staff       (20)     7400 2022-02-09 11:55:52.000000 nenupy-2.2.9/tests/test_astro_sky.py
+-rw-r--r--   0 aloh       (502) staff       (20)     2786 2022-02-09 16:34:21.000000 nenupy-2.2.9/tests/test_astro_skymodel.py
+-rw-r--r--   0 aloh       (502) staff       (20)    12513 2022-02-08 16:06:13.000000 nenupy-2.2.9/tests/test_astro_target.py
+-rw-r--r--   0 aloh       (502) staff       (20)    11148 2022-02-08 12:58:47.000000 nenupy-2.2.9/tests/test_astro_tools.py
+-rw-r--r--   0 aloh       (502) staff       (20)     3239 2020-10-01 15:36:39.000000 nenupy-2.2.9/tests/test_database.py
+-rw-r--r--   0 aloh       (502) staff       (20)     3553 2022-02-14 15:56:11.000000 nenupy-2.2.9/tests/test_instru.py
+-rw-r--r--   0 aloh       (502) staff       (20)    10961 2022-12-15 15:48:23.000000 nenupy-2.2.9/tests/test_instru_miniarray.py
+-rw-r--r--   0 aloh       (502) staff       (20)     9019 2022-12-15 15:50:47.000000 nenupy-2.2.9/tests/test_instru_nenufar.py
+-rw-r--r--   0 aloh       (502) staff       (20)     6384 2022-05-20 15:57:48.000000 nenupy-2.2.9/tests/test_io_bst.py
+-rw-r--r--   0 aloh       (502) staff       (20)     6088 2022-11-17 15:20:23.000000 nenupy-2.2.9/tests/test_io_xst.py
+-rw-r--r--   0 aloh       (502) staff       (20)     9661 2022-11-17 15:07:47.000000 nenupy-2.2.9/tests/test_jones_mueller.py
+-rw-r--r--   0 aloh       (502) staff       (20)    16125 2021-09-08 08:59:08.000000 nenupy-2.2.9/tests/test_obsconfig.py
+-rw-r--r--   0 aloh       (502) staff       (20)     4408 2022-03-10 09:32:19.000000 nenupy-2.2.9/tests/test_schedule.py
+-rw-r--r--   0 aloh       (502) staff       (20)    10553 2020-10-23 14:37:33.000000 nenupy-2.2.9/tests/test_sdata.py
```

### Comparing `nenupy-2.1.0/MANIFEST.in` & `nenupy-2.2.9/MANIFEST.in`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 include nenupy/telescopes.json
-include nenupy/instru_old/cal_pz_2_multi_2019-02-23.dat
-include nenupy/instru_old/squint_table.sav
-include nenupy/skymodel/lfsky.fits
-include nenupy/undysputed/bandpass_coeffs.dat
-include nenupy/astro_old/radio_sources.json
-include nenupy/observation/parset_user_options.json
+include nenupy/astro/common_sources.json
+include nenupy/instru/cal_pz_2_multi_2019-02-23.dat
+include nenupy/instru/cal_table_NDPPP-24sep2021-freq-all-MR6_V1_20220118.dat
+include nenupy/instru/cal_table_NDPPP-24sep2021-freq-all-MR6_V1_20220120.dat
 include nenupy/instru/low_noise_amplifier.json
-include nenupy/instru/nenufar_array.json
 include nenupy/instru/miniarray_antennas.json
-include nenupy/instru/squint_table.sav
 include nenupy/instru/NenuFAR_Ant_Hpx.fits
+include nenupy/instru/nenufar_array.json
+include nenupy/instru/squint_table.sav
+include nenupy/io/nenufar_tv_sources.json
+include nenupy/observation/parset_user_options.json
+include nenupy/undysputed/bandpass_coeffs.dat
+include nenupy/skymodel/lfsky.fits
```

### Comparing `nenupy-2.1.0/README.md` & `nenupy-2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/bin/nenupy_vcr_coordinates` & `nenupy-2.2.9/bin/nenupy_vcr_coordinates`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/__init__.py` & `nenupy-2.2.9/nenupy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #! /usr/bin/python3
 # -*- coding: utf-8 -*-
 
 __author__ = 'Alan Loh'
 __copyright__ = 'Copyright 2021, nenupy'
 __credits__ = ['Alan Loh']
 __license__ = 'MIT'
-__version__ = '2.1.0'
+__version__ = '2.2.9'
 __maintainer__ = 'Alan Loh'
 __email__ = 'alan.loh@obspm.fr'
 
 
 import logging
 import sys
 import json
```

### Comparing `nenupy-2.1.0/nenupy/astro/pointing.py` & `nenupy-2.2.9/nenupy/astro/pointing.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 
         .. rubric:: Methods Summary
 
         .. autosummary::
 
             ~Pointing.plot
             ~Pointing.from_file
+            ~Pointing.from_bst
             ~Pointing.target_tracking
             ~Pointing.target_transit
             ~Pointing.zenith_tracking
 
         .. rubric:: Attributes and Methods Documentation
 
     """
@@ -115,16 +116,24 @@
 
 
     def __getitem__(self, time: Time):
         """ """
         starts = (self.time).jd
         stops = (self.time + self.duration).jd
         
+        if time.isscalar:
+            time = time.reshape(1,)
+    
         if self.coordinates.isscalar:
-            coordinates = self.coordinates.reshape(1,)
+            # coordinates = self.coordinates.reshape(1,)
+            coordinates = SkyCoord(
+                np.repeat(self.coordinates.ra.deg, self.time.size),
+                np.repeat(self.coordinates.dec.deg, self.time.size),
+                unit="deg"
+            )
         else:
             coordinates = self.coordinates
         ras = coordinates.ra.deg
         decs = coordinates.dec.deg
 
         ra = []
         dec = []
@@ -151,19 +160,28 @@
                 dec.append(zenith.dec)
 
                 if hasattr(self, "custom_ho_coordinates"):
                     custom_az.append(0*u.deg)
                     custom_el.append(90*u.deg)
             else:
                 # there is a match
-                ra.append(ras[mask][0])
-                dec.append(decs[mask][0])
+                ra.append(ras[mask][-1]) # -1 because there may be several matches
+                dec.append(decs[mask][-1])
                 if hasattr(self, "custom_ho_coordinates"):
-                    custom_az.append(self.custom_ho_coordinates[mask].az[0])
-                    custom_el.append(self.custom_ho_coordinates[mask].alt[0])
+                    if self.custom_ho_coordinates.shape == (1, 1):
+                        # Transit observation
+                        custom_az.append(self.custom_ho_coordinates.az[0, 0].deg*u.deg)
+                        custom_el.append(self.custom_ho_coordinates.alt[0, 0].deg*u.deg)
+                    elif self.custom_ho_coordinates.shape == (1,):
+                        # Transit observation
+                        custom_az.append(self.custom_ho_coordinates.az[0].deg*u.deg)
+                        custom_el.append(self.custom_ho_coordinates.alt[0].deg*u.deg)
+                    else:
+                        custom_az.append(self.custom_ho_coordinates[mask].az[-1].deg*u.deg)
+                        custom_el.append(self.custom_ho_coordinates[mask].alt[-1].deg*u.deg)
 
         pointing = Pointing(
             coordinates=SkyCoord(
                 ra,
                 dec,
                 unit='deg'
             ),
@@ -365,15 +383,34 @@
     @classmethod
     def from_bst(cls,
             bst,
             beam: int = 0,
             analog: bool = True,
             max_points: int = 100
         ):
-        """ """
+        """ Instantiates a class:`~nenupy.astro.pointing.Pointing` object from
+            a :class:`~nenupy.io.bst.BST` object.
+
+            :param bst:
+            :type bst:
+            :param beam:
+            :type beam:
+                `int`
+            :param analog:
+            :type analog:
+                `bool`
+            :param max_points:
+            :type max_points:
+
+            :returns:
+                Pointing derived from a NenuFAR BST file.
+            :rtype:
+                :class:`~nenupy.astro.pointing.Pointing`
+
+        """
         bst.beam = beam
 
         if analog:
             time, az, el = bst.analog_pointing
         else:
             time, az, el = bst.digital_pointing
         
@@ -426,14 +463,19 @@
                 numerical (ending with ``.altazB``).
             :type file_name:
                 `str`
             :param beam_index:
                 Beam number to take into account.
             :type beam_index:
                 `int`
+            :param include_corrections:
+                Include or not the pointing corrections (default is ``True``).
+                Only has an effect on analog beam corrections.
+            :type include_corrections:
+                `bool`
             
             :return:
                 Pointing derived from a NenuFAR pointing file.
             :rtype:
                 :class:`~nenupy.astro.pointing.Pointing`
 
             :Example:
@@ -451,53 +493,69 @@
                     skiprows=3,
                     comments=";",
                     dtype={
                         'names': ('time', 'anabeam', 'az', 'el', 'az_cor', 'el_cor', 'freq', 'el_eff'),
                         'formats': ('U20', 'i4', 'f4', 'f4', 'f4', 'f4', 'U5', 'f4')
                     }
                 )
-                pointing = pointing[pointing["anabeam"] == beam_index]
-                azimuths = pointing["az_cor"][:-1] if include_corrections else pointing["az"][:-1]
-                elevations = pointing["el_eff"][:-1] if include_corrections else pointing["el"][:-1]
+                available_beams = pointing["anabeam"]
+                pointing = pointing[available_beams == beam_index]
+                azimuths = pointing["az_cor"] if include_corrections else pointing["az"]
+                elevations = pointing["el_eff"] if include_corrections else pointing["el"]
             except ValueError:
                 # No correction
                 pointing = np.loadtxt(
                     file_name,
                     skiprows=3,
                     comments=";",
                     dtype={
                         'names': ('time', 'anabeam', 'az', 'el', 'freq', 'el_eff'),
                         'formats': ('U20', 'i4', 'f4', 'f4', 'U5', 'f4')
                     }
                 )
-                pointing = pointing[pointing["anabeam"] == beam_index]
-                azimuths = pointing["az"][:-1]
-                elevations = pointing["el_eff"][:-1] if include_corrections else pointing["el"][:-1]
+                available_beams = pointing["anabeam"]
+                pointing = pointing[available_beams == beam_index]
+                azimuths = pointing["az"]
+                elevations = pointing["el_eff"] if include_corrections else pointing["el"]
             except IndexError:
                 # No beamsquint
                 pointing = np.loadtxt(
                     file_name,
                     skiprows=3,
                     comments=";",
                     dtype={
                         'names': ('time', 'anabeam', 'az', 'el', 'az_cor', 'el_cor'),
                         'formats': ('U20', 'i4', 'f4', 'f4', 'f4', 'f4')
                     }
                 )
-                pointing = pointing[pointing["anabeam"] == beam_index]
-                azimuths = pointing["az_cor"][:-1] if include_corrections else pointing["az"][:-1]
-                elevations = pointing["el_cor"][:-1] if include_corrections else pointing["el"][:-1]
+                available_beams = pointing["anabeam"]
+                pointing = pointing[available_beams == beam_index]
+                azimuths = pointing["az_cor"] if include_corrections else pointing["az"]
+                elevations = pointing["el_cor"] if include_corrections else pointing["el"]
+            
+            if pointing.size == 0:
+                raise ValueError(
+                    f"Empty pointing, check the beam_index={beam_index} value "
+                    f"(avalaible beam indices: {np.unique(available_beams)})."
+                )
 
             times = Time(pointing["time"])
+            azimuths *= u.deg
+            elevations *= u.deg
+            if times.size == 1:
+                # for a transit with multiple ABeams
+                azimuths = np.append(azimuths, [0]*u.deg)
+                elevations = np.append(elevations, [90]*u.deg)
+                times = times.insert(1, times[-1] + TimeDelta(1, format="sec"))
+
             duration = times[1:] - times[:-1]
             times = times[:-1]
             altaz_coords = SkyCoord(
-                azimuths,
-                elevations,
-                unit="deg",
+                azimuths[:-1],
+                elevations[:-1],
                 frame=AltAz(
                     obstime=times,
                     location=nenufar_position
                 )
             )
         elif file_name.endswith('.altazB'):
             pointing = np.loadtxt(
@@ -505,35 +563,35 @@
                 skiprows=2,
                 comments=";",
                 dtype={
                     'names': ('time', 'anabeam', 'digibeam', 'az', 'el', 'l', 'm', 'n'),
                     'formats': ('U20', 'i4', 'i4', 'f4', 'f4', 'f4', 'f4', 'f4')
                 }
             )
-            pointing = pointing[pointing["digibeam"] == beam_index]
+            available_beams = pointing["digibeam"]
+            pointing = pointing[available_beams == beam_index]
+            if pointing.size == 0:
+                raise ValueError(
+                    f"Empty pointing, check the beam_index={beam_index} value "
+                    f"(avalaible beam indices: {np.unique(available_beams)})."
+                )
             times = Time(pointing["time"])
             duration = times[1:] - times[:-1]
             # Add the last duration at the end (supposed to be 10 seconds)
             duration = duration.insert(-1, TimeDelta(10, format="sec", scale=duration.scale))
             altaz_coords = SkyCoord(
                 pointing['az'],
                 pointing["el"],
                 unit="deg",
                 frame=AltAz(
                     obstime=times,
                     location=nenufar_position
                 )
             )
-        
-        # return cls(
-        #     coordinates=altaz_to_radec(altaz=altaz_coords),
-        #     time=times,
-        #     duration=duration,
-        #     observer=nenufar_position
-        # )
+
         pointing = cls(
             coordinates=altaz_to_radec(altaz=altaz_coords),
             time=times,
             duration=duration,
             observer=nenufar_position
         )
         pointing.custom_ho_coordinates = altaz_coords
@@ -663,38 +721,41 @@
         if transit_time.size == 0:
             raise ValueError(
                 f"The selected target does not cross azimuth={azimuth}."
             )
         elif transit_time.size != 1:
             # Possibly 2 crossings if the source is circumpolar
             # get the one at maximal elevation
-            target_altaz = radec_to_altaz(radec=target.coordinates, time=transit_time)[:, 0]
-            transit_time = transit_time[target_altaz.alt.argmax()]
+            # target_altaz = radec_to_altaz(radec=target.coordinates, time=transit_time, fast_compute=True)[:, 0]
+            # transit_time = transit_time[target_altaz.alt.argmax()]
+            transit_time = transit_time[0].reshape((1,))
         
-        transit_altaz = radec_to_altaz(radec=target.coordinates, time=transit_time)
+        transit_altaz = radec_to_altaz(radec=target.coordinates, time=transit_time, fast_compute=True)
         time_steps = np.floor(duration/dt)
         time_steps = time_steps + 1 if time_steps%2 == 0 else time_steps
         dt_shifts = np.arange(time_steps) - (time_steps - 1)/2
 
         pointing_times = transit_time + dt_shifts*dt
 
-        return cls(
+        pointing = cls(
             coordinates=SkyCoord(
                 np.repeat(transit_altaz.az.deg, pointing_times.size),
                 np.repeat(transit_altaz.alt.deg, pointing_times.size),
                 unit="deg",
                 frame=AltAz(
                     obstime=pointing_times,
                     location=nenufar_position
                 )
             ).transform_to(ICRS),
             time=pointing_times,
             duration=dt,
             observer=observer
         )
+        pointing.custom_ho_coordinates = transit_altaz
+        return pointing
 
 
     # @classmethod
     # def snapshot(cls,
     #         target: Target,
     #         time: Time,
     #         duration: TimeDelta = TimeDelta(1, format="sec"),
@@ -788,26 +849,29 @@
 
         """
         az = 0
         el = 90
         if not time.isscalar:
             az = np.repeat(az, time.size)
             el = np.repeat(el, time.size)
-        return cls(
+        altaz = SkyCoord(
+            az,
+            el,
+            unit="deg",
+            frame=AltAz(
+                obstime=time,
+                location=observer
+            )
+        )
+        pointing = cls(
             coordinates=altaz_to_radec(
-                altaz=SkyCoord(
-                    az,
-                    el,
-                    unit="deg",
-                    frame=AltAz(
-                        obstime=time,
-                        location=observer
-                    )
-                ),
+                altaz=altaz,
                 fast_compute=False
             ),
             time=time,
             duration=duration,
             observer=observer
         )
+        pointing.custom_ho_coordinates = altaz.reshape((1,)) if altaz.isscalar else altaz
+        return pointing
 # ============================================================= #
 # ============================================================= #
```

### Comparing `nenupy-2.1.0/nenupy/astro/sky.py` & `nenupy-2.2.9/nenupy/astro/sky.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,14 +130,19 @@
                 `bool`
             :param decibel:
                 If set to ``True``, the data values are displayed at the decibel scale,
                 i.e., :math:`10 \log( \rm{data} )`. 
                 Default is ``False``.
             :type decibel:
                 `bool`
+            :param interpolation:
+                Matplotlib `imshow interpolation <https://matplotlib.org/stable/gallery/images_contours_and_fields/interpolation_methods.html>`_ method.
+                Default is ``'quadric'``.
+            :type interpolation:
+                `str`
 
             .. rubric:: Overplot keywords
 
             :param scatter:
                 Add a scatter plot (as defined in `matplotlib.pyplot.scatter`).
                 Expected syntax is ``(<SkyCoord>, <marker_size>, <color>)``.
                 Default is ``None`` (i.e., no scatter overplot).
@@ -213,14 +218,15 @@
         radius = kwargs.get("radius", None)
         ticks_color = kwargs.get("ticks_color", "0.9")
         colorbar_label = kwargs.get("colorbar_label", "")
         title = kwargs.get("title", f"{self.time.isot.split('.')[0]}, {self.frequency:.2f}")
         visible_sky = kwargs.get("only_visible", True)
         decibel = kwargs.get("decibel", False)
         altaz_overlay = kwargs.get("altaz_overlay", False)
+        alpha = kwargs.get('alpha', None)
 
         # Initialize figure
         wcs, shape = self._compute_wcs(
             center=center,
             resolution=getattr(self, "resolution", resolution),
             radius=radius
         )
@@ -232,30 +238,41 @@
 
         # Get the data projected on fullsky
         data = self._fullsky_projection(
             wcs=wcs,
             shape=shape,
             display_visible_sky=visible_sky
         )
+        if alpha is not None:
+            # Use additional data stored in alpha argument to overlap an oppacity mask
+            alpha_image = self._fullsky_projection(
+                wcs=wcs,
+                shape=shape,
+                display_visible_sky=False,
+                value=alpha
+            )
+            alpha_image[np.isnan(alpha_image)] = 0
+            alpha_image /= alpha_image.max()
 
         # Scale the data in decibel
         if decibel:
             data = 10 * np.log10(data)
 
         vmin = kwargs.get("vmin", np.nanmin(data))
         vmax = kwargs.get("vmax", np.nanmax(data))
 
         # Plot the data
         im = ax.imshow(
             data,
             origin="lower",
-            interpolation="quadric",
+            interpolation=kwargs.get("interpolation", "quadric"),
             cmap=cmap,
             vmin=vmin,
-            vmax=vmax
+            vmax=vmax,
+            alpha=None if alpha is None else alpha_image
         )
 
         # Define ax ticks
         ax.coords.grid(color=ticks_color, alpha=0.5)
         path_effects=[patheffects.withStroke(linewidth=3, foreground='black')]
 
         ra_axis = ax.coords[0]
@@ -443,19 +460,20 @@
                 )
             contour, _ = reproject_from_healpix(
                 (data, ICRS()),
                 wcs,
                 nested=False,
                 shape_out=shape#(ndec, nra)
             )
-            ax.contour(
+            cont = ax.contour(
                 contour,
                 levels=parameters[1],
                 cmap=parameters[2],
             )
+            ax.clabel(cont, inline=1, fontsize=10)
 
         # Other
         im.set_clip_path(ax.coords.frame.patch)
         ax.set_title(title, pad=20)
 
         # Save or show
         if figname is None:
@@ -519,15 +537,15 @@
         wcs.wcs.cdelt = np.array([-dangle/scale, dangle/scale])
         wcs.wcs.crval = [center.ra.deg, center.dec.deg]
         wcs.wcs.ctype = ['RA---AIT', 'DEC--AIT']
 
         return wcs, (ra_dim, dec_dim)
 
 
-    def _fullsky_projection(self, wcs: WCS, shape: tuple, display_visible_sky: bool):
+    def _fullsky_projection(self, wcs: WCS, shape: tuple, display_visible_sky: bool, value: np.ndarray = None):
         """ """
         x, y = wcs.world_to_pixel(self.coordinates)
 
         data = np.zeros(shape, dtype=np.float64)
         data[:, :] = np.nan
         weights = np.zeros(shape, dtype=int)
 
@@ -535,15 +553,19 @@
         x_in_image = (x_int >= 0) & (x_int < shape[0])
         y_int = np.floor(y).astype(int)
         y_in_image = (y_int >= 0) & (y_int < shape[1])
         in_image_mask = x_in_image & y_in_image
         x_int = x_int[in_image_mask]
         y_int = y_int[in_image_mask]
 
-        values = copy.deepcopy(self.value)
+        if value is None:
+            values = copy.deepcopy(self.value)
+        else:
+            values = da.from_array(value)
+
         if display_visible_sky:
             values[~self.visible_sky] = np.nan
         values = values[in_image_mask]
 
         if isinstance(values, da.Array):
             with ProgressBar() if log.getEffectiveLevel() <= logging.INFO else DummyCtMgr():
                 values = values.compute()
@@ -603,17 +625,21 @@
         wcs.wcs.cdelt = np.array([-dangle/scale, dangle/scale])
         wcs.wcs.crval = [center.ra.deg, center.dec.deg]
         wcs.wcs.ctype = ['RA---AIT', 'DEC--AIT']
 
         return wcs, (dec_dim, ra_dim)
 
 
-    def _fullsky_projection(self, wcs: WCS, shape: tuple, display_visible_sky: bool):
+    def _fullsky_projection(self, wcs: WCS, shape: tuple, display_visible_sky: bool, value: np.ndarray = None):
         """ """
-        values = copy.deepcopy(self.value)
+        if value is None:
+            values = copy.deepcopy(self.value)
+        else:
+            values = da.from_array(value)
+
         if display_visible_sky:
             values[~self.visible_sky] = np.nan
         
         if isinstance(values, da.Array):
             with ProgressBar() if log.getEffectiveLevel() <= logging.INFO else DummyCtMgr():
                 values = values.compute()
```

### Comparing `nenupy-2.1.0/nenupy/astro/skymodel.py` & `nenupy-2.2.9/nenupy/astro/skymodel.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/astro/target.py` & `nenupy-2.2.9/nenupy/astro/target.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,17 +38,18 @@
 from typing import Callable
 import numpy as np
 import logging
 log = logging.getLogger(__name__)
 
 import astropy.units as u
 from astropy.time import Time, TimeDelta
-from astropy.coordinates import SkyCoord, EarthLocation, FK5, AltAz
+from astropy.coordinates import SkyCoord, EarthLocation, FK5, AltAz, Angle
 
 from nenupy import nenufar_position
+from nenupy.astro import common_sources
 from nenupy.astro.astro_tools import (
     AstroObject,
     hour_angle,
     solar_system_source
 )
 
 
@@ -70,14 +71,15 @@
             ~Target.is_circumpolar
             ~Target.culmination_azimuth
 
         .. rubric:: Methods Summary
 
         .. autosummary::
 
+            ~Target.separation
             ~Target.meridian_transit
             ~Target.next_meridian_transit
             ~Target.previous_meridian_transit
             ~Target.azimuth_transit
             ~Target.rise_time
             ~Target.next_rise_time
             ~Target.previous_rise_time
@@ -135,14 +137,55 @@
             return 180*u.deg
         else:
             return 0*u.deg
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
+    def separation(self, other: Target) -> Angle:
+        """ Computes the angular separation between two :class:`~nenupy.astro.target.Target`
+            instances.
+            This method is a wrapper around :meth:`astropy.coordinates.SkyCoord.separation`.
+
+            :param other:
+                Other :class:`~nenupy.astro.target.Target` from 
+                which the angular separation should be computed.
+            :type other:
+                :class:`~nenupy.astro.target.Target`
+
+            :returns:
+                Angular separation.
+            :rtype:
+                :class:`~astropy.coordinates.Angle`
+
+            :Example:
+                .. code-block:: python
+
+                    from nenupy.astro.target import FixedTarget, SolarSystemTarget
+                    from astropy.time import Time, TimeDelta
+                    import numpy as np
+
+                    src = FixedTarget.from_name("Cyg A")
+                    times = Time("2022-01-01T12:00:00") + np.arange(180)*TimeDelta(2, format="jd")
+                    seps = src.separation(
+                        SolarSystemTarget.from_name(
+                            "Sun",
+                            time=times
+                        )
+                    )
+
+        """
+        if not isinstance(other, Target):
+            raise TypeError(
+                f"The angular separation should be computed against another {Target} object. "
+                f"Got {type(other)} instead."
+            )
+        return self.coordinates.separation(other.coordinates)
+
+
     def meridian_transit(self,
             t_min: Time = Time.now(),
             duration: TimeDelta = TimeDelta(86400, format='sec'),
             precision: TimeDelta = TimeDelta(5, format='sec'),
             fast_compute: bool = True
         ) -> Time:
         """ Computes the :class:`~nenupy.astro.target.Target` meridian transit time(s).
@@ -288,14 +331,15 @@
                     obstime=times,
                     location=self.observer
                 )
             )
             azimuths = altaz_coordinates.az.rad
             az = azimuth.to(u.rad).value
             if self.is_circumpolar:
+                az = np.angle(np.cos(az) + 1j*np.sin(az))
                 complexAzStarts = np.angle(
                     np.cos(azimuths[:, :-1]) + 1j*np.sin(azimuths[:, :-1])
                 )
                 complexAzStops = np.angle(
                     np.cos(azimuths[:, 1:]) + 1j*np.sin(azimuths[:, 1:])
                 )
                 mask = (complexAzStarts <= az) &\
@@ -891,14 +935,15 @@
             ~Target.culmination_azimuth
 
         .. rubric:: Methods Summary
 
         .. autosummary::
 
             ~FixedTarget.from_name
+            ~Target.separation
             ~Target.meridian_transit
             ~Target.next_meridian_transit
             ~Target.previous_meridian_transit
             ~Target.azimuth_transit
             ~Target.rise_time
             ~Target.next_rise_time
             ~Target.previous_rise_time
@@ -933,15 +978,15 @@
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
     @classmethod
     def from_name(cls,
             name: str,
             time: Time = Time.now(),
             observer: EarthLocation = nenufar_position
-        ) -> SolarSystemTarget:
+        ) -> FixedTarget:
         """ Instantiates a :class:`~nenupy.astro.target.FixedTarget`
             object from a name that could be resolved by `Simbad <http://simbad.u-strasbg.fr/simbad/>`_.
 
             :param name:
                 Source name.
             :type name:
                 `str`
@@ -963,16 +1008,20 @@
             
             :Example:
                 >>> from nenupy.astro.target import FixedTarget
                 >>> cyg_a = FixedTarget.from_name("Cyg A")
 
         """
 
-        # Retrieve the Simbad coordinates
-        source = SkyCoord.from_name(name)
+        if name.lower() in common_sources.keys():
+            src = common_sources[name.lower()]
+            source = SkyCoord(src["ra"], src["dec"], unit="deg")
+        else:
+            # Retrieve the Simbad coordinates
+            source = SkyCoord.from_name(name)
 
         return cls(
             coordinates=source,
             observer=observer,
             time=time
         )
 
@@ -1011,14 +1060,15 @@
             ~Target.culmination_azimuth
 
         .. rubric:: Methods Summary
 
         .. autosummary::
 
             ~SolarSystemTarget.from_name
+            ~Target.separation
             ~Target.meridian_transit
             ~Target.next_meridian_transit
             ~Target.previous_meridian_transit
             ~Target.azimuth_transit
             ~Target.rise_time
             ~Target.next_rise_time
             ~Target.previous_rise_time
```

### Comparing `nenupy-2.1.0/nenupy/astro_old/astro.py` & `nenupy-2.2.9/nenupy/instru/interferometer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,1176 +1,1075 @@
 #! /usr/bin/python3
 # -*- coding: utf-8 -*-
 
 
 """
-    **********************
-    Astronomical Functions
-    **********************
-
-    Below are defined a set of useful astronomical functions
-    summarized as:
-    
-    * :func:`~nenupy.astro.astro.lst`: Sidereal time
-    * :func:`~nenupy.astro.astro.lha`: Local hour angle
-    * :func:`~nenupy.astro.astro.wavelength`: Convert frequency to wavelength
-    * :func:`~nenupy.astro.astro.ho_coord`: Define a :class:`~astropy.coordinates.AltAz` object
-    * :func:`~nenupy.astro.astro.eq_coord`: Define a :class:`~astropy.coordinates.ICRS` object
-    * :func:`~nenupy.astro.astro.to_radec`: Convert :class:`~astropy.coordinates.AltAz` to :class:`~astropy.coordinates.ICRS`
-    * :func:`~nenupy.astro.astro.toAltaz`: Convert equatorial coordinates to horizontal coordinates
-    * :func:`~nenupy.astro.astro.ho_zenith`: Get the local zenith in :class:`~astropy.coordinates.AltAz` coordinates
-    * :func:`~nenupy.astro.astro.eq_zenith`: Get the local zenith in :class:`~astropy.coordinates.ICRS` coordinates
-    * :func:`~nenupy.astro.astro.radio_sources`: Get main radio source positions
-    * :func:`~nenupy.astro.astro.getSource`: Get a particular source coordinates
-    * :func:`~nenupy.astro.astro.altazProfile`: Retrieve horizontal coordinates versus time
-    * :func:`~nenupy.astro.astro.meridianTransit`: Next meridian transit time
-    * :func:`~nenupy.astro.astro.dispersion_delay`: Dispersion delay induced by wave propagation through an electron plasma
-
+    *********************
+    Interferometric Array
+    *********************
 """
 
 
-__author__ = 'Alan Loh'
-__copyright__ = 'Copyright 2020, nenupy'
-__credits__ = ['Alan Loh']
-__maintainer__ = 'Alan'
-__email__ = 'alan.loh@obspm.fr'
-__status__ = 'Production'
+__author__ = "Alan Loh"
+__copyright__ = "Copyright 2021, nenupy"
+__credits__ = ["Alan Loh"]
+__maintainer__ = "Alan"
+__email__ = "alan.loh@obspm.fr"
+__status__ = "Production"
 __all__ = [
-    'lst',
-    'lha',
-    'toFK5',
-    'wavelength',
-    'ho_coord',
-    'eq_coord',
-    'to_radec',
-    'toAltaz',
-    'ho_zenith',
-    'eq_zenith',
-    'radio_sources',
-    'getSource',
-    'altazProfile',
-    'meridianTransit',
-    'dispersion_delay',
-    '_normalizeEarthRadius',
-    'l93_to_etrs',
-    'geo_to_etrs',
-    'etrs_to_geo',
-    'etrs_to_enu',
-    'enu_to_etrs'
-    ]
+    "Baseline",
+    "ObservingMode",
+    "Interferometer"
+]
 
 
+from abc import ABC, ABCMeta, abstractmethod
+import copy
+from enum import Enum, auto
+from functools import lru_cache
+from os import cpu_count
+from typing import Dict, Callable
+import logging
+log = logging.getLogger(__name__)
+
 import numpy as np
-from astropy.time import Time, TimeDelta
-from astropy import units as u
+import matplotlib.pyplot as plt
+
+import astropy.units as u
+from astropy.constants import k_B
 from astropy.coordinates import (
     EarthLocation,
-    Angle,
-    Longitude,
-    SkyCoord,
-    AltAz,
-    Galactic,
-    ICRS,
-    FK5,
-    solar_system_ephemeris,
-    get_body
+    Angle
 )
-from astropy.constants import c as lspeed
-from os.path import dirname, join
-import json
-
-from nenupy.instru_old import nenufar_loc
-import nenupy.miscellaneous as misc
+import dask.array as da
+from dask.diagnostics import ProgressBar
 
-import logging
-log = logging.getLogger(__name__)
+from nenupy import LogMethodMetaClass, DummyCtMgr
+from nenupy.astro.sky import Sky
+from nenupy.astro.astro_tools import sky_temperature
+from nenupy.astro.pointing import Pointing
 
 
 # ============================================================= #
-# ---------------------------- lst ---------------------------- #
+# ---------------- Interferometer class errors ---------------- #
 # ============================================================= #
-@misc.accepts(Time, str, strict=(False, True))
-def lst(time, kind='fast'):
-    """ Computes the Local Sidereal Time at the longitude of the
-        NenuFAR radio telescope.
-        Viewed from NenuFAR, a fixed celestial object seen at one
-        position in the sky will be seen at the same position on
-        another night at the same sidereal time. LST angle
-        indicates the Right Ascension on the sky that is
-        currently crossing the Local Meridian.
-
-        :param time:
-            UT Time to be converted
-        :type time: :class:`~astropy.time.Time`
-        :param kind:
-            ``'fast'`` computes an approximation of local sidereal
-            time, ``'mean'`` accounts for precession and ``'apparent'``
-            accounts for precession and nutation.
-        :type kind: str
-
-        :returns: Local Sidereal Time angle
-        :rtype: :class:`~astropy.coordinates.Longitude`
-
-        :Example:
-            >>> from nenupy.astro import lst
-            >>> from astropy.time import Time
-            >>> lst(time=Time('2020-01-01 12:00:00'), kind='fast')
-            <Longitude 18.85380195 hourangle>
-            >>> lst(time=Time('2020-01-01 12:00:00'), kind='mean')
-            <Longitude 18.85375283 hourangle>
-            >>> lst(time=Time('2020-01-01 12:00:00'), kind='apparent')
-            <Longitude 18.85347225 hourangle>
+class CombinedMeta(LogMethodMetaClass, ABCMeta):
+    """ Intermediate metaclass when inheriting from ABC. """
 
-    """
-    if kind.lower() == 'fast':
-        # http://www.roma1.infn.it/~frasca/snag/GeneralRules.pdf
-        # Number of days since 2000 January 1, 12h UT
-        nDays = time.jd - 2451545.
-        # Greenwich mean sidereal time
-        gmst = 18.697374558 + 24.06570982441908 * nDays
-        gmst %= 24.
-        # Local Sidereal Time
-        lst = gmst + nenufar_loc.lon.hour
-        if np.isscalar(lst):
-            if lst < 0:
-                lst += 24
-        else:
-            lst[lst < 0] += 24.   
-        return Longitude(lst, 'hour')
-    else:
-        location = nenufar_loc
-        lon = location.to_geodetic().lon
-        lst = time.sidereal_time(kind, lon)
-        return lst
-# ============================================================= #
 
+class AntennaNameError(Exception):
+    """ Error raised when the name doesn't match existing antenna names. """
 
-# ============================================================= #
-# ---------------------------- lha ---------------------------- #
-# ============================================================= #
-@misc.accepts(Longitude, (ICRS, SkyCoord, FK5), strict=True)
-def lha(lst, skycoord):
-    r""" Local Hour Angle of an object in the observer's sky. It
-        is defined as the angular distance on the celestial
-        sphere measured westward along the celestial equator from
-        the meridian to the hour circle passing through a point.
-
-        The local hour angle :math:`h` is computed with respect
-        to the local sidereal time ``lst`` :math:`t_{\rm LST}`
-        and the ``skycoord`` astronomical source's right 
-        ascension :math:`\alpha`:
-
-        .. math::
-            h = t_{\rm LST} - \alpha
-
-        with the rule that if :math:`h < 0`, a :math:`2\pi` angle
-        is added or if :math:`h > 2\pi`, a :math:`2\pi` angle
-        is subtracted.
-        
-        :param lst:
-            Local Sidereal Time, such as returned by
-            :func:`~nenupy.astro.astro.lst` for instance.
-        :type lst: :class:`~astropy.coordinates.Longitude`
-        :param skycoord:
-            Sky coordinates to convert to Local Hour Angles. This
-            must be converted to FK5 coordinates with the
-            corresponding equinox in order to give accurate
-            results (see :func:`~nenupy.astro.astro.toFK5`).
-        :type skycoord: :class:`~astropy.coordinates.SkyCoord`
-
-        :returns: LHA time
-        :rtype: :class:`~astropy.coordinates.Angle`
-
-        :Example:
-            >>> from nenupy.astro import lst, lha, toFK5
-            >>> from astropy.time import Time
-            >>> from astropy.coordinates import SkyCoord
-            >>> utcTime = Time(['2020-01-01 12:00:00', '2020-01-01 13:00:00'])
-            >>> lstTime = lst(
-                    time=utcTime,
-                    kind='apparent'
-                )
-            >>> casA = SkyCoord.from_name('Cas A')
-            >>> casA_2020 = toFK5(
-                    skycoord=casA,
-                    time=utcTime
-                )
-            >>> lHA = lha(
-                    lst=lstTime,
-                    skycoord=casA_2020
-                )
-            >>> lHA
-            [19h26m53.9458s 20h27m03.8018s]
+    def __init__(self,
+            input_name: np.ndarray,
+            available_antennas: np.ndarray
+        ):
+        self.input_name = input_name
+        self.message = f"Valid antenna names are {available_antennas}."
+        super().__init__(self.message)
 
-    """
-    if skycoord.equinox is None:
-        log.warning(
-            (
-                'Given skycoord for LHA computation does not '
-                'have an equinox attribute, make sure the '
-                'precession is taken into account.'
-            )
-        )
-    ha = lst - skycoord.ra
-    twopi = Angle(360.000000 * u.deg)
-    if ha.isscalar:
-        if ha.deg < 0:
-            ha += twopi
-        elif ha.deg > 360:
-            ha -= twopi
-    else:
-        ha[ha.deg < 0] += twopi
-        ha[ha.deg > 360] -= twopi
-    return ha
 
-# ============================================================= #
+    def __str__(self):
+        return f"'{self.input_name}'\n{self.message}"
 
 
-# ============================================================= #
-# --------------------------- toFK5 --------------------------- #
-# ============================================================= #
-@misc.accepts((ICRS, SkyCoord, FK5), Time, strict=(True, False))
-def toFK5(skycoord, time):
-    """ Converts sky coordinates ``skycoord`` to FK5 system with
-        equinox given by ``time``.
-
-        :param skycoord:
-            Sky Coordinates to be converted to FK5 system.
-        :type skycoord: :class:`~astropy.coordinates.SkyCoord`
-        :param time:
-            Time that defines the equinox to be accounted for.
-        :type time: :class:`~astropy.time.Time`
+class AntennaIndexError(Exception):
+    """ Error raised when the index doesn't match existing antenna indices. """
 
-        :returns: FK5 sky coordinates
-        :rtype: :class:`~astropy.coordinates.SkyCoord`
-    """
-    return skycoord.transform_to(
-        FK5(equinox=time)
-    )
-# ============================================================= #
+    def __init__(self,
+            input_index: np.ndarray,
+            n_available_antennas: int
+        ):
+        self.input_index = input_index
+        self.message = f"Maximum antenna index is {n_available_antennas - 1}."
+        super().__init__(self.message)
 
 
-# ============================================================= #
-# ------------------------ wavelength ------------------------- #
-# ============================================================= #
-def wavelength(freq):
-    """ Convert radio frequency in wavelength.
+    def __str__(self):
+        return f"{self.input_index}\n{self.message}"
 
-        :param freq:
-            Frequency (assumed in MHz unless a
-            :class:`~astropy.units.Quantity` is provided)
-        :type freq: `float`, :class:`~numpy.ndarray` or
-            :class:`~astropy.units.Quantity`
 
-        :returns: Wavelength in meters
-        :rtype: :class:`~astropy.units.Quantity`
-    """
-    if not isinstance(freq, u.Quantity):
-        freq *= u.MHz
-    freq = freq.to(u.Hz)
-    wavel = lspeed / freq
-    return wavel.to(u.m)
-# ============================================================= #
+class DuplicateAntennaError(Exception):
+    """ Error raised when antennas are duplicated. """
 
+    def __init__(self,
+            input_antenna: np.ndarray,
+        ):
+        self.input_antenna = input_antenna
+        unique, counts = np.unique(self.input_antenna, return_counts=True)
+        duplicate_mask = [counts > 1]
+        dup = unique[tuple(duplicate_mask)]
+        cnt = counts[tuple(duplicate_mask)]
 
-# ============================================================= #
-# ------------------------- ho_coord -------------------------- #
-# ============================================================= #
-def ho_coord(alt, az, time):
-    """ Horizontal coordinates
-    
-        :param alt:
-            Altitude in degrees
-        :type alt: `float` or :class:`~astropy.units.Quantity`
-        :param az:
-            Azimuth in degrees
-        :type az: `float` or :class:`~astropy.units.Quantity`
-        :param time:
-            Time at which the local zenith coordinates should be 
-            computed. It can either be provided as an 
-            :class:`~astropy.time.Time` object or a string in ISO
-            or ISOT format.
-        :type time: str, :class:`~astropy.time.Time`
-
-        :returns: :class:`~astropy.coordinates.AltAz` object
-        :rtype: :class:`~astropy.coordinates.AltAz`
-
-        :Example:
-            >>> from nenupysim.astro import ho_coord
-            >>> altaz = ho_coord(
-                    alt=45,
-                    az=180,
-                    time='2020-01-01 12:00:00'
-                )
-    """
-    if not isinstance(az, u.Quantity):
-        az *= u.deg
-    if not isinstance(alt, u.Quantity):
-        alt *= u.deg
-    if not isinstance(time, Time):
-        time = Time(time)
-    return AltAz(
-        az=az,
-        alt=alt,
-        location=nenufar_loc,
-        obstime=time
-    )
-# ============================================================= #
+        self.message = f"antenna name/index {dup} is duplicated {cnt} times."
+        super().__init__(self.message)
 
 
+    def __str__(self):
+        return f"{self.input_antenna}: {self.message}"
 # ============================================================= #
-# ------------------------- eq_coord -------------------------- #
-# ============================================================= #
-def eq_coord(ra, dec):
-    """ Equatorial coordinates
-        
-        :param ra:
-            Right ascension in degrees
-        :type ra: `float` or :class:`~astropy.units.Quantity`
-        :param dec:
-            Declination in degrees
-        :type dec: `float` or :class:`~astropy.units.Quantity`
-
-        :returns: :class:`~astropy.coordinates.ICRS` object
-        :rtype: :class:`~astropy.coordinates.ICRS`
-
-        :Example:
-            >>> from nenupysim.astro import eq_coord
-            >>> radec = eq_coord(
-                    ra=51,
-                    dec=39,
-                )
-    """
-    if not isinstance(ra, u.Quantity):
-        ra *= u.deg
-    if not isinstance(dec, u.Quantity):
-        dec *= u.deg
-    return ICRS(
-        ra=ra,
-        dec=dec
-    )
 # ============================================================= #
 
 
 # ============================================================= #
-# ------------------------- to_radec -------------------------- #
-# ============================================================= #
-def to_radec(altaz):
-    """ Transform altaz coordinates to ICRS equatorial system
-        
-        :param altaz:
-            Horizontal coordinates
-        :type altaz: :class:`~astropy.coordinates.AltAz`
-
-        :returns: :class:`~astropy.coordinates.ICRS` object
-        :rtype: :class:`~astropy.coordinates.ICRS`
-
-        :Example:
-            >>> from nenupysim.astro import eq_coord
-            >>> radec = eq_coord(
-                    ra=51,
-                    dec=39,
-                )
-    """
-    if not isinstance(altaz, AltAz):
-        raise TypeError(
-            'AltAz object expected.'
-        )
-    return altaz.transform_to(ICRS)
+# ------------------------- Baseline -------------------------- #
 # ============================================================= #
+class Baseline:
+    """ Class to handle interferometric baseline operations. """
 
+    def __init__(self, itrf_positions: np.ndarray):
+        self.itrf_positions = itrf_positions
 
-# ============================================================= #
-# -------------------------- toAltaz -------------------------- #
-# ============================================================= #
-@misc.accepts((SkyCoord, ICRS), Time, str, strict=(True, False, True))
-def toAltaz(skycoord, time, kind='normal'):
-    r""" Convert a celestial object equatorial coordinates
-        ``skycoord`` to horizontal coordinates as seen from
-        NenuFAR's location at a given ``time``.
-
-        If ``kind='fast'`` is selected the computation is
-        accelerated using Local Sidereal Time approximation
-        (see :func:`~nenupy.astro.astro.lst`). The altitude
-        :math:`\theta` and azimuth :math:`\varphi` are computed
-        as follows:
-
-        .. math::
-            \cases{
-                \sin(\theta) = \sin(\delta) \sin(l) + \cos(\delta) \cos(l) \cos(h)\\
-                \cos(\varphi) = \frac{\sin(\delta) - \sin(l) \sin(\theta)}{\cos(l)\cos(\varphi)}
-            }
-
-        with :math:`\delta` the object's declination, :math:`l`
-        the NenuFAR's latitude and :math:`h` the Local Hour Angle
-        (see :func:`~nenupy.astro.astro.lha`).
-        If :math:`\sin(h) \geq 0`, then :math:`\varphi = 2 \pi - \varphi`.
-        Otherwise, :meth:`~astropy.coordinates.SkyCoord.transform_to`
-        is used.
-
-        :param skycoord:
-            Celestial object equatorial coordinates
-        :type skycoord: :class:`~astropy.coordinates.SkyCoord`
-        :param time:
-            Coordinated universal time
-        :type time: :class:`~astropy.time.Time`
-        :param kind:
-            ``'fast'`` enables faster computation time for the
-            conversion, mainly relying on an approximation of the
-            local sidereal time. All other values would lead to
-            accurate coordinates computation. Differences in
-            coordinates values are of the order of :math:`10^{-2}`
-            degrees or less.
-        :type kind: `str`
-
-        :returns:
-            Celestial object's horizontal coordinates
-        :rtype: :class:`~astropy.coordinates.SkyCoord`
-
-        :Example:
-            >>> from nenupy.astro import toAltaz
-            >>> from astropy.time import Time
-            >>> from astropy.coordinates import SkyCoord
-
-            >>> utcTime = Time('2020-10-07 11:16:49')
-            >>> casA_radec = SkyCoord.from_name('Cas A')
-            >>> casA_altaz = toAltaz(
-                    skycoord=casA_radec,
-                    time=utcTime,
-                    kind='fast'
-                )
-            >>> print(casA_altaz.az.deg, casA_altaz.alt.deg)
-            9.024164094317975 17.2063660579154
-
-            >>> casA_altaz = toAltaz(
-                    skycoord=casA_radec,
-                    time=utcTime
-                )
-            >>> print(casA_altaz.az.deg, casA_altaz.alt.deg)
-            9.018801267468616 17.206414428075465
+        if self.itrf_positions.ndim != 2:
+            raise ValueError(
+                "<arg 'itrf_positions'>: instance of "
+                f"{np.ndarray} of dimension 2 expected. "
+                f"Got {self.itrf_positions.shape} instead."
+            )
+        self.antenna_idx = np.arange(self.itrf_positions.shape[0])
+        xyz = self.itrf_positions[..., None]
+        xyz = xyz[:, :, 0][:, None]
+        self.bsl = xyz.transpose(1, 0, 2) - xyz
 
-            >>> utcTime = Time(['2020-01-01', '2020-01-02'])
-            >>> casA_altaz = toAltaz(casA_radec, utcTime, 'fast')
-            >>> print(casA_altaz.az.deg, casA_altaz.alt.deg)
-            [326.15940811 326.56313916] [30.23939922 29.86967785]
 
-    """
-    altazFrame = AltAz(
-        obstime=time,
-        location=nenufar_loc
-    )
-    if kind.lower() == 'fast':
-        lstTime = lst(
-            time=time,
-            kind='fast'
-        )
-        skycoord = toFK5(
-            skycoord=skycoord,
-            time=time
-        )
-        lHA = lha(
-            lst=lstTime,
-            skycoord=skycoord
+    def __getitem__(self, n):
+        pos = self.itrf_positions[n, :]
+        return Baseline(
+            itrf_positions=pos
         )
 
-        decRad = skycoord.dec.rad
-        haRad = lHA.rad
-        latRad = nenufar_loc.lat.rad
-
-        sinDec = np.sin(decRad)
-        cosDec = np.cos(decRad)
-        sinLat = np.sin(latRad)
-        cosLat = np.cos(latRad)
-        sinHa = np.sin(haRad)
-        cosHa = np.cos(haRad)
-
-        # Elevation
-        sinAlt = sinDec * sinLat + cosDec * cosLat * cosHa
-        altRad = np.arcsin(sinAlt)
-
-        # Azimuth
-        cosAz = (sinDec - sinLat * np.sin(altRad))/\
-                (cosLat * np.cos(altRad))
-        azRad = np.arccos(cosAz)
-        if np.isscalar(altRad):
-            if sinHa >= 0.:
-                azRad = 2*np.pi - azRad
-        else:
-            posMask = sinHa >= 0.
-            azRad[posMask] = 2*np.pi - azRad[posMask]
 
-        return SkyCoord(
-            azRad * u.rad,
-            altRad * u.rad,
-            frame=altazFrame
-        )
-    else:
-        return skycoord.transform_to(altazFrame)
-# ============================================================= #
+    # --------------------------------------------------------- #
+    # --------------------- Getter/Setter --------------------- #
+    @property
+    def flatten(self):
+        """
+        """
+        return self.bsl[
+            np.tril_indices(self.antenna_idx.size)
+        ]
 
 
+    @property
+    def distance(self):
+        """
+        """
+        return np.linalg.norm(self.bsl, axis=2) * u.m
 # ============================================================= #
-# ------------------------- ho_zenith ------------------------- #
-# ============================================================= #
-def ho_zenith(time):
-    """ Horizontal coordinates of local zenith above NenuFAR
-
-        :param time:
-            Time at which the local zenith coordinates should be 
-            computed. It can either be provided as an 
-            :class:`~astropy.time.Time` object or a string in ISO
-            or ISOT format.
-        :type time: `str`, :class:`~astropy.time.Time`
-
-        :returns: :class:`~astropy.coordinates.AltAz` object
-        :rtype: :class:`~astropy.coordinates.AltAz`
-
-        :Example:
-            >>> from nenupysim.astro import ho_zenith
-            >>> zen_altaz = ho_zenith(time='2020-01-01 12:00:00')
-    """
-    if not isinstance(time, Time):
-        time = Time(time)
-    if time.isscalar:
-        return ho_coord(
-            az=0.,
-            alt=90.,
-            time=time
-        )
-    else:
-        return ho_coord(
-            az=np.zeros(time.size),
-            alt=np.ones(time.size) * 90.,
-            time=time
-        )
 # ============================================================= #
 
 
 # ============================================================= #
-# ------------------------- eq_zenith ------------------------- #
+# ----------------------- ObservingMode ----------------------- #
 # ============================================================= #
-def eq_zenith(time):
-    """ Equatorial coordinates of local zenith above NenuFAR
-        
-        :param time:
-            Time at which the local zenith coordinates should be 
-            computed. It can either be provided as an 
-            :class:`~astropy.time.Time` object or a string in ISO
-            or ISOT format.
-        :type time: `str`, :class:`~astropy.time.Time`
-        
-        :returns: :class:`~astropy.coordinates.ICRS` object
-        :rtype: :class:`~astropy.coordinates.ICRS`
+class ObservingMode(Enum):
+    """ Enumerator of the different available observing modes of NenuFAR. """
 
-        :Example:
-            >>> from nenupysim.astro import ho_zenith
-            >>> zen_radec = eq_zenith(time='2020-01-01 12:00:00')
-    """
-    altaz_zenith = ho_zenith(
-        time=time
-    )
-    return to_radec(altaz_zenith)
+    BEAMFORMING = auto()
+    IMAGING = auto()
+# ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
-# ----------------------- radio_sources ----------------------- #
+# ---------------------- Interferometer ----------------------- #
 # ============================================================= #
-def radio_sources(time):
-    """ Main low-frequency radio source position in local
-        coordinates frame at time ``time``.
-
-        :param time:
-            Time at which the local zenith coordinates should be 
-            computed. It can either be provided as an 
-            :class:`~astropy.time.Time` object or a string in ISO
-            or ISOT format.
-        :type time: `str`, :class:`~astropy.time.Time`
-
-        :returns:
-            Dictionnary of radio source positions.
-        :rtype: `dict`
-    """
-    if not isinstance(time, Time):
-        time = Time(time)
-    if not time.isscalar:
-        raise ValueError(
-            'Only scalar time allowed.'
-        )
+class Interferometer(ABC, metaclass=CombinedMeta):
+    """ Abstract base class for all phased-array/interferometer classes.
 
-    def solarsyst_eq(src, time):
-        src = get_body(
-            src,
-            time,
-            nenufar_loc
-        )
-        return eq_coord(src.ra.deg, src.dec.deg)
+        .. rubric:: Attributes Summary
 
-    with solar_system_ephemeris.set('builtin'):
-        src_radec = {
-            'vira': eq_coord(187.70593075, +12.39112331),
-            'cyga': eq_coord(299.86815263, +40.73391583),
-            'casa': eq_coord(350.850000, +58.815000),
-            'hera': eq_coord(252.783433, +4.993031),
-            'hyda': eq_coord(139.523546, -12.095553),
-            'taua': eq_coord(83.63308, +22.01450),
-            'sun': solarsyst_eq('sun', time),
-            'moon': solarsyst_eq('moon', time),
-            'jupiter': solarsyst_eq('jupiter', time),
-        }
-    return {
-        key: toAltaz(src_radec[key], time=time) for key in src_radec.keys()
-    }
-# ============================================================= #
+        .. autosummary::
 
+            ~nenupy.instru.interferometer.Interferometer.antenna_gains
+            ~nenupy.instru.interferometer.Interferometer.antenna_names
+            ~nenupy.instru.interferometer.Interferometer.antenna_positions
+            ~nenupy.instru.interferometer.Interferometer.baselines
+            ~nenupy.instru.interferometer.Interferometer.position
+            ~nenupy.instru.interferometer.Interferometer.size
 
-# ============================================================= #
-# ------------------------- getSource ------------------------- #
-# ============================================================= #
-def getSource(name, time=None):
-    """ Retrieve a source equatorial coordinates.
+        .. rubric:: Methods Summary
+
+        .. autosummary::
 
-        :param name:
-            Source name.
-        :type name: `str`
-        :param time:
-            Time at which the coordinates need to be calculated.
-            This is particularly relevant for Solar System objects.
-            Moreover, if ``time`` is not a scalar, the returned
-            source coordinates will have dimensions matching the
-            ``time`` argument.
-        :type time: :class:`~astropy.time.Time`
-
-        :returns:
-            Source equatorial coordinates.
-        :rtype: :class:`~astropy.coordinates.SkyCoord`
-
-        :Example:
-            >>> from nenupy.astro import getSource
-            >>> from astropy.time import Time
-            >>> getSource('Cyg X-3')
-                <SkyCoord (ICRS): (ra, dec) in deg
-                [(308.10741667, 40.95775)]>
-            >>> getSource('Sun', Time(['2020-04-01 12:00:00', '2020-04-01 14:00:00']))
-                <SkyCoord (GCRS:
-                    obstime=['2020-04-01 12:00:00.000' '2020-04-01 14:00:00.000'],
-                    obsgeoloc=[
-                        (4237729.57730929,  917401.20083485, 4662142.24721379),
-                        (3208307.85440129, 2913433.12950414, 4664141.44068417)
-                    ] m,
-                    obsgeovel=[
-                        ( -66.89938865, 308.36222659, 0.13071683),
-                        (-212.45197538, 233.29547849, 0.41179784)
-                    ] m / s): (ra, dec, distance) in (deg, deg, AU)
-                    [(10.983783  , 4.71984404, 0.99938543),
-                     (11.05889498, 4.75192569, 0.99941305)]>
+            ~nenupy.instru.interferometer.Interferometer.angular_resolution
+            ~nenupy.instru.interferometer.Interferometer.array_factor
+            ~nenupy.instru.interferometer.Interferometer.beam
+            ~nenupy.instru.interferometer.Interferometer.confusion_noise
+            ~nenupy.instru.interferometer.Interferometer.plot
+            ~nenupy.instru.interferometer.Interferometer.sefd
+            ~nenupy.instru.interferometer.Interferometer.sensitivity
+            ~nenupy.instru.interferometer.Interferometer.system_temperature
+
+        .. rubric:: Attributes and Methods Documentation
 
-        .. versionadded:: 1.1.0
     """
-    sourceJson = join(
-        dirname(__file__),
-        'radio_sources.json',
-    )
-    with open(sourceJson) as jsonFile:
-        sources = json.load(jsonFile)
-
-    solarSystem = [
-        'sun',
-        'moon',
-        'jupiter',
-        'saturn',
-        'mars',
-        'venus',
-        'uranus',
-        'neptune'
-    ]
-
-    nTime = 1
-
-    if name.upper() in sources.keys():
-        if time is not None:
-            if not time.isscalar:
-                nTime = time.size
-            else:
-                nTime = 1
-        src = sources[name.upper()]
-        src = SkyCoord(
-            ra=[src['ra']] * nTime * u.deg,
-            dec=[src['dec']] * nTime * u.deg,
-            frame='icrs'
-        )
-        log.debug(
-            f'Source {name} found in {sourceJson}.'
-        )
-    elif name.lower() in solarSystem:
-        if not isinstance(time, Time):
-            raise TypeError(
-                'time should be a Time object'
+
+    def __init__(self,
+            position: EarthLocation,
+            antenna_names: np.ndarray,
+            antenna_positions: np.ndarray,
+            antenna_gains: np.ndarray
+        ):
+        self.position = position
+        self.antenna_names = antenna_names
+        self.antenna_positions = antenna_positions
+        self.antenna_gains = antenna_gains
+
+
+    def __getitem__(self, n):
+        if isinstance(n, slice):
+            # Convert the slice into a numpy array
+            n = np.r_[n]
+        elif not isinstance(n, np.ndarray):
+            n = np.array(n)
+            if np.isscalar(n):
+                n = n.reshape((1,))
+
+        # Checking the correct input format
+        if n.ndim > 1:
+            raise ValueError(
+                "<class 'Interferometer'> can only be "
+                f"subscriptable by 1D arrays. Got {n} instead."
             )
-        with solar_system_ephemeris.set('builtin'):
-            src = get_body(name, time, nenufar_loc)
-            if src.ra.isscalar:
-                src = SkyCoord(
-                    ra=[src.ra.deg] * u.deg,
-                    dec=[src.dec.deg] * u.deg
-                )
-            else:
-                src = SkyCoord(
-                    ra=src.ra,
-                    dec=src.dec
+        if np.unique(n).size != n.size:
+            raise DuplicateAntennaError(n)
+
+        # Generating antenna mask
+        if n.dtype.str.startswith('<U'):
+            # Selection based on antenna names
+            antenna_mask = np.isin(self.antenna_names, n)
+            bad_name_index = ~np.isin(n, self.antenna_names)
+            if np.any(bad_name_index):
+                raise AntennaNameError(
+                    n[bad_name_index],
+                    self.antenna_names
                 )
-        log.debug(
-            f'Source {name} found in Solar System Ephemeris.'
-        )
-    else:
-        if time is not None:
-            if not time.isscalar:
-                nTime = time.size
-            else:
-                nTime = 1
-        src = SkyCoord.from_name(name) # ICRS
-        if time is not None:
-            if not time.isscalar:
-                nTime = time.size
         else:
-            nTime = 1
-        src = SkyCoord(
-            ra=[src.ra.deg] * nTime * u.deg,
-            dec=[src.dec.deg] * nTime * u.deg,
-            frame='icrs'
-        )
-        log.debug(
-            f'Source {name} found in Simbad.'
-        )
+            # Selection based on antenna indices
+            if n.max() >= self.size:
+                raise AntennaIndexError(n, self.size)
+            antenna_mask = np.isin(np.arange(self.size), n)
+
+        # Constructing the new instance as a 'cutout' of its parent
+        interfero = copy.deepcopy(self)
+        interfero.antenna_names = self.antenna_names[antenna_mask]
+        interfero.antenna_positions = self.antenna_positions[antenna_mask, :]
+        interfero.antenna_gains = self.antenna_gains[antenna_mask]
+        return interfero
+
+
+    def __repr__(self):
+        return f"{self.__class__}"
+
+
+    def __str__(self):
+        return f"{self.__class__.__name__}"
+
+
+    def __add__(self, other):
+        interferometer = copy.deepcopy(self)
+        to_include = ~np.isin(other.antenna_names, self.antenna_names)
+        interferometer.antenna_names = np.concatenate((self.antenna_names, other.antenna_names[to_include]))
+        interferometer.antenna_positions = np.concatenate((self.antenna_positions, other.antenna_positions[to_include]))
+        interferometer.antenna_gains = np.concatenate((self.antenna_gains, other.antenna_gains[to_include]))
+        return interferometer
+    
 
-    return src
-# ============================================================= #
+    def __sub__(self, other):
+        interferometer = copy.deepcopy(self)
+        to_keep = ~np.isin(self.antenna_names, other.antenna_names)
+        interferometer.antenna_names = self.antenna_names[to_keep]
+        interferometer.antenna_positions = self.antenna_positions[to_keep]
+        interferometer.antenna_gains = self.antenna_gains[to_keep]
+        return interferometer
+
+
+    # --------------------------------------------------------- #
+    # --------------------- Getter/Setter --------------------- #
+    @property
+    def size(self):
+        """ Number of elements belonging to the array. 
 
+            :getter: Size of the array.
 
-# ============================================================= #
-# ----------------------- altazProfile ------------------------ #
-# ============================================================= #
-def altazProfile(sourceName, tMin=None, tMax=None, dt=None):
-    """
-    """
-    if tMin is None:
-        tMin = Time.now()
-    elif not isinstance(tMin, Time):
-        raise TypeError(
-            'tMin should be a Time object'
-        )
+            :type: `int`
+        """
+        return self.antenna_positions.shape[0]
 
-    if tMax is None:
-        tMax = tMin + TimeDelta(24*3600, format='sec')
-    elif not isinstance(tMax, Time):
-        raise TypeError(
-            'tMax should be a Time object'
-        )
 
-    if dt is None:
-        dt = TimeDelta(5*60, format='sec')
-    elif not isinstance(dt, TimeDelta):
-        raise TypeError(
-            'dt should be a TimeDelta object'
-        )
+    @property
+    def baselines(self):
+        """ Instrument baselines.
 
-    tCurrent = tMin
-    times = []
-    elevations = []
-    azimuths = []
-    while tCurrent <= tMax:
-        if 'srcRaDec' not in locals():
-            srcRaDec = getSource(
-                name=sourceName,
-                time=tCurrent
-            )
-        elif srcRaDec.frame.name == 'gcrs':
-            # Solar system source, need to be updated/time
-            srcRaDec = getSource(
-                name=sourceName,
-                time=tCurrent
-            )
-        else:
-            # Do not ask again for same source
-            pass
+            :getter: Baselines.
 
-        srcAltAz = toAltaz(
-            skycoord=srcRaDec,
-            time=tCurrent
-        )
+            :type: :class:`~nenupy.instru.interferometer.Baseline`
+        """
+        try:
+            antenna_position = self._toITRF()
+        except AttributeError:
+            log.error("No method '_toITRF()' is implemented.")
+            raise
+        return Baseline(itrf_positions=antenna_position)
 
-        times.append(tCurrent.isot)
-        azimuths.append(srcAltAz.az.deg)
-        elevations.append(srcAltAz.alt.deg)
-        tCurrent += dt
 
-    return Time(times), np.array(azimuths), np.array(elevations)
-# ============================================================= #
+    @property
+    def antenna_names(self) -> np.ndarray:
+        """ Antenna names.
 
+            :setter: Array of antenna names.
 
-# ============================================================= #
-# ---------------------- meridianTransit ---------------------- #
-# ============================================================= #
-@misc.accepts(SkyCoord, Time, TimeDelta, str, strict=(True, False, False, True))
-def meridianTransit(source, fromTime, duration=TimeDelta(1), kind='fast'):
-    """ Find the ``source`` meridian transit time(s) since the
-        time ``fromTime`` at NenuFAR location within a time period
-        ``duration``.
-
-        :param source:
-            The source instance to look for the transit.
-            See also :func:`~nenupy.astro.astro.eq_coord` or 
-            :meth:`~astropy.coordinates.SkyCoord.from_name`.
-        :type source: :class:`~astropy.coordinates.SkyCoord`
-        :param fromTime:
-            Time from which the next transit should be found.
-        :type fromTime: :class:`~astropy.time.Time`
-        :param duration:
-            Duration to check transits since ``fromTime``
-        :type duration: :class:`~astropy.time.TimeDelta`
-        :param kind:
-            Manner to compute the Local Sidereal Time, allowed
-            values are ``'fast'``, ``'mean'`` and ``'apparent'``,
-            see :func:`~nenupy.astro.astro.lst`.
-        :type kind: str
-        
-        :returns:
-            Next meridian transit time of ``source``.
-        :rtype: :class:`~astropy.time.Time`
-    """
-    def _timeRange(tMin, tMax, dt):
+            :getter: Array of antenna names.
+
+            :type: :class:`~numpy.ndarray`
         """
+        return self._antenna_names
+    @antenna_names.setter
+    def antenna_names(self, n: np.ndarray):
+        self._antenna_names = n
+
+    
+    @property
+    def antenna_positions(self) -> np.ndarray:
+        """ Antenna positions.
+            The positions should be shaped as ``(n_ant, 3)``
+
+            :setter: Array of antenna positions.
+
+            :getter: Array of antenna positions.
+
+            :type: :class:`~numpy.ndarray`
         """
-        if not (isinstance(tMin, Time) and isinstance(tMax, Time)):
-            raise TypeError(
-                'tMin and tMax should be astropy.Time instances.'
-            )
-        if not isinstance(dt, TimeDelta):
-            raise TypeError(
-                'dt should be an astropy.TimeDelta instance.'
-            )
-        nTimes = (tMax - tMin) / dt
-        times = tMin + np.arange(nTimes + 1) * dt
-        return times
-
-    def _jumpIndices(angleArray):
-        """ ``angleArray`` is expected to contain increasing
-            angular values.
-            This function enables to detect the jumps between 360
-            and 0 deg for instance (or 180 and -180 deg).
+        return self._antenna_positions
+    @antenna_positions.setter
+    def antenna_positions(self, p: np.ndarray):
+        self._antenna_positions = p
+
+
+    @property
+    def antenna_gains(self) -> np.ndarray:
+        """ Antenna gains.
+            This is an array of `callable` (methods or functions)
+            defining the radiation pattern of each antenna.
+
+            :setter: Array of antenna gains.
+
+            :getter: Array of antenna gains.
+
+            :type: :class:`~numpy.ndarray` of `callable`
         """
-        indices = np.where(
-            (np.roll(angleArray, -1) - angleArray)[:-1] < 0
-        )[0]
-        return indices
+        return self._antenna_gains
+    @antenna_gains.setter
+    def antenna_gains(self, g: np.ndarray):
+        self._antenna_gains = g
+
+
+    @property
+    def position(self) -> EarthLocation:
+        """ Array's position.
+
+            :setter: Position of the array.
 
-    def _getLHA(times, source, kind):
+            :getter: Position of the array.
+
+            :type: :class:`~astropy.coordinates.EarthLocation`
         """
+        return self._position
+    @position.setter
+    def position(self, p: EarthLocation):
+        self._position = p
+
+
+    # --------------------------------------------------------- #
+    # ------------------------ Methods ------------------------ #
+    def plot(self, **kwargs) -> None:
+        """ Plots the antenna distribution.
+
+            :param figsize:
+                Size of the figure. Default is ``(10, 10)``.
+            :type figsize:
+                `tuple`
+            :param figname:
+                File name of the figure to save. Default is ``''``,
+                i.e. show the figure without saving it.
+            :type figname:
+                `str`
+            :param xlim:
+                X-axis limits. Default is auto-scaling.
+            :type xlim:
+                `tuple`
+            :param ylim:
+                Y-axis limits. Default is auto-scaling.
+            :type ylim:
+                `tuple`
+            :param show_names:
+                Print the antenna names. Default is ``True``.
+            :type show_names:
+                `bool`
+            :param patches:
+                Matplotlib Polygons
+            :type patches:
+                `tuple`(`list`, colors) of Polygons
         """
-        sourcefk5 = toFK5(
-            skycoord=source,
-            time=times
-        )
-        lstTime = lst(
-            time=times,
-            kind=kind
-        )
-        hourAngles = lha(
-            lst=lstTime,
-            skycoord=sourcefk5
+        fig, ax = plt.subplots(
+            figsize=kwargs.get('figsize', (10, 10))
         )
-        return hourAngles
 
-    transitTimes = []
+        positions = self.antenna_positions
 
-    extDuration = TimeDelta(3600, format='sec')
-    largeDt = TimeDelta(1800, format='sec')
-    mediumDt = TimeDelta(60, format='sec')
-    smallDt = TimeDelta(1, format='sec')
-
-    # Broad search
-    times = _timeRange(
-        tMin=fromTime - extDuration,
-        tMax=fromTime + duration + extDuration,
-        dt=largeDt
-    )
-    hourAngles = _getLHA(times, source, kind)
-    indices = _jumpIndices(hourAngles)
-    
-    # Iterate over the transit(s)
-    for index in indices:
-        # Medium search
-        medTimes = _timeRange(
-            tMin=times[index],
-            tMax=times[index + 1],
-            dt=mediumDt
-        )
-        hourAngles = _getLHA(medTimes, source, kind)
-        medIndices = _jumpIndices(hourAngles)
-        medIndex = medIndices[0]
-
-        # Finest search
-        smallTimes = _timeRange(
-            tMin=medTimes[medIndex],
-            tMax=medTimes[medIndex + 1],
-            dt=smallDt
-        )
-        hourAngles = _getLHA(smallTimes, source, kind)
-        smallIndices = _jumpIndices(hourAngles)
+        ax.scatter(positions[:, 0], positions[:, 1], kwargs.get('s', 30))
 
-        transitTimes.append(
-            (smallTimes[smallIndices[0]] + smallDt/2.).isot
-        )
+        if kwargs.get("patches", None) is not None:
+            from matplotlib.collections import PatchCollection
+            patches, colors = kwargs.get("patches")
+            p = PatchCollection(patches, alpha=0.5)
+            p.set_array(colors)
+            ax.add_collection(p)
+
+        ax.set_xlim(kwargs.get('xlim', ax.get_xlim()))
+        ax.set_ylim(kwargs.get('ylim', ax.get_ylim()))
+
+        ax.set_xlabel(kwargs.get('x_label', ''))
+        ax.set_ylabel(kwargs.get('y_label', ''))
+
+        if kwargs.get("show_names", True):
+            for i, antenna_name in enumerate(self.antenna_names):
+                ax.annotate(
+                    antenna_name,
+                    (
+                        positions[i, 0],
+                        positions[i, 1]
+                    ),
+                    ha='center'
+                )
+        ax.set_aspect('equal', adjustable='datalim')
 
-    return Time(transitTimes)
-# ============================================================= #
+        if kwargs.get('figname', '') != '':
+            plt.savefig(
+                kwargs.get('figname'),
+                dpi=300,
+                transparent=True,
+                bbox_inches='tight'
+            )
+        else:
+            plt.show()
+        plt.close('all')
 
+        # from nenupy.instru import miniarray_antennas, MiniArray
+        # from nenupy.astro import l93_to_etrs
+        # from pyproj import Transformer
+        # def ma_antenna_positions(ma_index: int = 0):
+        #     ma_name = f'MA{ma_index:03}'
+        #     ma = MiniArray(index=ma_index)
+        #     ant_pos = ma.antenna_positions
+        #     rotation = np.radians(0)##360-ma.rotation.value)#ma.rotation.value +90)
+        #     rot_matrix = np.array(
+        #         [
+        #             [-np.cos(rotation), -np.sin(rotation), 0],
+        #             [-np.sin(rotation), np.cos(rotation), 0],
+        #             [0,           0,           1]
+        #         ]
+        #     )
+        #     ant_pos = np.dot(ant_pos, rot_matrix).astype(np.float32)
+        #     lambert_positions = ant_pos#nenufar_miniarrays[ma_name]['position'] + ant_pos
+        #     return lambert_positions
+        #     #etrs_positions = l93_to_etrs(lambert_positions)
+        #     #return etrs_positions
+        # with open('/Users/aloh/Desktop/antenna_positions.csv', 'w') as wfile:
+        #     wfile.write('Mini-Array,Antenna,x(m),y(m),height(m)')
+        #     for ma_index in range(96):
+        #         positions = ma_antenna_positions(ma_index)
+        #         # plt.scatter(pos[:, 0], pos[:, 1])
+        #         # for i in range(19):
+        #         #     plt.text(pos[i, 0], pos[i, 1], f'{i+1}')
+        #         # plt.gca().set_aspect('equal', adjustable='box')
+        #         # plt.show()
+        #         #plt.savefig('/Users/aloh/Desktop/ma7dist.png', transparent=True)
+        #         # for i, ant in enumerate(pos):
+        #         #     #print(f'{i} {ant[0]:3f} {ant[1]:3f}')
+        #         #     print(f'{ant[0]:3f}')
+        #         # for i, ant in enumerate(pos):
+        #         #     #print(f'{i} {ant[0]:3f} {ant[1]:3f}')
+        #         #     print(f'{ant[1]:3f}')
+        #         # t = Transformer.from_crs(
+        #         #     crs_from="EPSG:2154", # RGF93
+        #         #     crs_to="EPSG:4326" # World Geodetic System 1984, used in GPS
+        #         # )
+        #         # ws84 = t.transform(
+        #         #     xx=positions[:, 0],
+        #         #     yy=positions[:, 1],
+        #         #     zz=positions[:, 2]
+        #         # )
+        #         # lat0 = [47.376595,47.376596,47.376596,47.376552,47.376553,47.376553,47.376554,47.376509,47.376509,47.376510,47.376510,47.376511,47.376466,47.376467,47.376467,47.376468,47.376424,47.376424,47.376425]
+        #         # lon0 = [2.193005,2.193077,2.193150,2.192969,2.193042,2.193115,2.193187,2.192933,2.193006,2.193079,2.193152,2.193224,2.192970,2.193043,2.193116,2.193189,2.193007,2.193080,2.193153]
+        #         # lat7 = [47.376085,47.376123,47.376160,47.376094,47.376132,47.376169,47.376207,47.376103,47.376141,47.376178,47.376216,47.376254,47.376150,47.376187,47.376225,47.376263,47.376197,47.376234,47.376272]
+        #         # lon7 = [2.191337,2.191289,2.191242,2.191408,2.191361,2.191314,2.191266,2.191480,2.191433,2.191385,2.191338,2.191290,2.191504,2.191457,2.191409,2.191362,2.191528,2.191481,2.191434]
+        #         # plt.scatter(lat0, lon0)
+        #         #plt.gca().set_aspect('equal', adjustable='box')
+        #         lon, lat, height = ws84
+        #         for ia, ant in enumerate(positions):
+        #             wfile.write(f'\n{ma_index},{ia+1},{ant[0]:.4f},{ant[1]:.4f},{ant[2]:.4f}')
+
+
+
+    def array_factor(self, sky: Sky, pointing: Pointing, return_complex: bool = False) -> da.Array:
+        r""" Computes the array factor of the antenna distribution.
+
+            .. math::
+                \mathcal{F}(\nu, \phi, \theta) = \sum_{\rm ant} e^{ i \mathbf{k}(\nu, \phi, \theta) \cdot \mathbf{r}_{\rm ant}}
+
+            where :math:`\mathbf{k} = \frac{2\pi}{\lambda} (\cos \phi \cos \theta, \sin \phi \cos \theta, \sin \theta )`
+            is the wave vector for a wave propagation in a direction described by spherical coordinates,
+            :math:`\lambda` is the wavelength, :math:`\phi` is the azimuth,
+            :math:`\theta` is the elevation, :math:`\mathbf{r}_{\rm ant}`
+            is the antenna position matrix.
+
+            This method considers the ``sky`` as the desired output (in terms of
+            time, frequency and sky positions). It evaluates the effective 
+            pointing directions for every time step defined in ``sky`` regarding
+            the ``pointing`` input.
+
+            :param sky:
+                Desired output contained in a :class:`~nenupy.astro.sky.Sky` instance.
+                (:attr:`~nenupy.astro.sky.Sky.time`, :attr:`~nenupy.astro.sky.Sky.frequency` and
+                :attr:`~nenupy.astro.sky.Sky.coordinates` are used as inputs for the computation).
+            :type sky:
+                :class:`~nenupy.astro.sky.Sky`
+            :param pointing:
+                Instance of :class:`~nenupy.astro.pointing.Pointing` that defines
+                the targeted pointing directions over the time.
+            :type pointing:
+                :class:`~nenupy.astro.pointing.Pointing`
+
+            :return:
+                Array factor of the antenna distribution shaped as ``(time, frequency, 1, coordinates)``.
+            :rtype:
+                :class:`~dask.array.Array`                
 
-# ============================================================= #
-# --------------------- dispersion_delay ---------------------- #
-# ============================================================= #
-def dispersion_delay(freq, dm):
-    r""" Dispersion delay induced to a radio wave of frequency
-        ``freq`` (:math:`\nu`) propagating through an electron
-        plasma of uniform density :math:`n_e`.
-        
-        The pulse travel time :math:`\Delta t_p` emitted at a
-        distance :math:`d` is:
+            .. seealso::
+                :class:`~nenupy.astro.sky.Sky` and :class:`~nenupy.astro.pointing.Pointing`
+        """
 
-        .. math::
-            \Delta t_p = \frac{d}{c} + \frac{e^2}{2\pi m_e c} \frac{\int_0^d n_e\, dl}{\nu^2}
-    
-        where :math:`\mathcal{D}\mathcal{M} = \int_0^d n_e\, dl`
-        is the *Dispersion Measure*.
+        # Determine the effective pointing based on the time
+        # informations contained in the sky instance.
+        effective_pointing = pointing[sky.time]
+
+        # Compute the geometric delays as the dot product of the
+        # antenna position and the difference between sky and
+        # pointing ground projections.
+        geometric_delays = self._geometric_delays(sky, effective_pointing)
+
+        # Use the sky frequency attribute to compute the wavelength
+        # and prepare the coefficient of the exponential with
+        # the correct dimensions.
+        wavelength = sky.frequency.to(u.m, equivalencies=u.spectral())
+        coeff = 2j * np.pi / wavelength.value
+        coeff = coeff.reshape(
+            (1, 1, wavelength.size, 1, 1)
+        ) # (antenna, time, frequency, polar, coord)
+
+        exponent = coeff * geometric_delays
+        # coord_chunk = exponent.shape[-1]//cpu_count()
+        # coord_chunk = 1 if coord_chunk == 0 else coord_chunk
+        # exponent = da.rechunk(
+        #     exponent,
+        #     chunks=exponent.shape[:-1] + (coord_chunk,)
+        # )
+        complex_array_factor = np.sum(
+            np.exp(exponent),
+            axis=0
+        )/exponent.shape[0] # normalized
 
-        Therefore, the time delay :math:`\Delta t_d` due to the
-        dispersion is:
+        if return_complex:
+            return complex_array_factor
+        else:
+            return np.sqrt(np.real(complex_array_factor * np.conjugate(complex_array_factor)))
 
-        .. math::
-            \Delta t_d = \frac{e^2}{2 \pi m_e c} \frac{\mathcal{D}\mathcal{M}}{\nu^2} 
 
-        and computed as:
-
-        .. math::
-            \Delta t_d = 4140 \left( \frac{\mathcal{D}\mathcal{M}}{\rm{pc}\,\rm{cm}^{-3}} \right) \left( \frac{\nu}{1\, \rm{MHz}} \right)^{-2}\, \rm{sec}
-
-        :param freq:
-            Observation frequency (assumed to be in MHz if no
-            unit is provided).
-        :type freq: `float` or :class:`~numpy.ndarray` or :class:`~astropy.units.Quantity`
-        :param dm:
-            Dispersion Measure (assumed to be in pc/cm^-3 if no
-            unit is provided.
-        :type dm: `float` or :class:`~astropy.units.Quantity`
-
-        :returns: Dispersion delay in seconds.
-        :rtype: :class:`~astropy.units.Quantity`
-
-        :Example:
-            >>> from nenupy.astro import dispersion_delay
-            >>> import astropy.units as u
-            >>> dispersion_delay(
-                    freq=50*u.MHz,
-                    dm=12.4*u.pc/(u.cm**3)
-                )
-            20.5344 s
+    def beam(self, sky: Sky, pointing: Pointing, return_complex: bool = False) -> Sky:
+        r""" Computes the phased-array response :math:`\mathcal{G}` over the ``sky`` for a given
+            ``pointing``.
+
+            .. math::
+                \mathcal{G}(\nu, \phi, \theta) = \sum_{\rm ant} \mathcal{F}(\nu, \phi, \theta) \mathcal{G}_{\rm ant} (\nu, \phi, \theta)
+
+            where :math:`\nu` is the frequency, :math:`\phi` is the azimuth,
+            :math:`\theta` is the elevation,
+            :math:`\mathcal{G}_{\rm ant}` is the individual array element radiation pattern and
+            :math:`\mathcal{F}` is the array factor.
+
+            This method considers the ``sky`` as the desired output (in terms of
+            time, frequency, polarization and sky positions). It evaluates the effective 
+            pointing directions for every time step defined in ``sky`` regarding
+            the ``pointing`` input.
+
+            :param sky:
+                Desired output contained in a :class:`~nenupy.astro.sky.Sky` instance.
+            :type sky:
+                :class:`~nenupy.astro.sky.Sky`
+            :param pointing:
+                Instance of :class:`~nenupy.astro.pointing.Pointing` that defines
+                the targeted pointing directions over the time.
+            :type pointing:
+                :class:`~nenupy.astro.pointing.Pointing`
+
+            :return:
+                The instance of :class:`~nenupy.astro.sky.Sky`
+                given as input is returned, its attribute
+                :attr:`~nenupy.astro.sky.Sky.value` is updated
+                with the result of the beam computation (stored as
+                an :class:`~dask.array.Array`) and shaped as 
+                ``(time, frequency, polarization, coordinates)``.
+            :rtype:
+                :class:`~nenupy.astro.sky.Sky`
 
-        .. versionadded:: 1.1.0
-    """
-    if not isinstance(dm, u.Quantity):
-        dm *= u.pc / (u.cm**3)
-    else:
-        dm = dm.to(u.pc / (u.cm**3))
-    if not isinstance(freq, u.Quantity):
-        freq *= u.MHz
-    else:
-        freq = freq.to(u.MHz)
-    dm_ref = 1. * u.pc / (u.cm**3)
-    freq_ref = 1. * u.MHz
-    delay = 4140. * (dm/dm_ref) / ((freq/freq_ref)**2) * u.s
-    return delay
-# ============================================================= #
+            .. seealso::
+                :meth:`~nenupy.instru.interferometer.Interferometer.array_factor`
 
+        """
 
-# ============================================================= #
-# ------------------------ l93_to_etrs ------------------------ #
-# ============================================================= #
-def l93_to_etrs(positions):
-    """
-    """
-    from pyproj import Transformer
-    t = Transformer.from_crs(
-        crs_from='EPSG:2154', # RGF93
-        crs_to='EPSG:4896'# ITRF2005 / ETRS used in MS
-    )
-    positions[:, 0], positions[:, 1], positions[:, 2] = t.transform(
-        xx=positions[:, 0],
-        yy=positions[:, 1],
-        zz=positions[:, 2]
-    )
-    return positions
-# ============================================================= #
+        # Compute the array factor
+        array_factor = self.array_factor(
+            sky=sky,
+            pointing=pointing,
+            return_complex=return_complex
+        )
+
+        # Compute the total antenna gain, i.e. the sum of all
+        # antenna gains for beamforming.
+        antenna_gain = np.sum(
+            np.array([gain(
+                sky=sky,
+                pointing=pointing
+            ) for gain in self.antenna_gains]),
+            axis=0
+        ) / len(self.antenna_gains) # normalized
+
+        # Rechunk the Dask Array before the computation
+        # coord_chunk = array_factor.shape[-1]//cpu_count()
+        # coord_chunk = 1 if coord_chunk == 0 else coord_chunk
+        # array_factor = array_factor.rechunk(array_factor.shape[:-1] + (coord_chunk,))
+
+        # Perform the Dask computation of array factor times antenna
+        # gains. Update the sky instance values.
+        if return_complex:
+            sky.value = array_factor * np.sqrt(antenna_gain)
+        else:
+            sky.value = array_factor * antenna_gain
 
+        return sky
 
-# ============================================================= #
-# ------------------- _normalizeEarthRadius ------------------- #
-# ============================================================= #
-def _normalizeEarthRadius(lat):
-    """ Normalized radius of the WGS84 ellipsoid at a given latitude
-        From https://github.com/brentjens/lofar-antenna-positions/blob/master/lofarantpos/geo.py
-        lat in radians
-    """
-    wgs84_f = 1./298.257223563
-    cosLat = np.cos(lat)
-    sinlat = np.sin(lat)
-    return 1./np.sqrt(cosLat**2 + ((1. - wgs84_f)**2) * (sinlat**2))
-# ============================================================= #
 
+    @lru_cache(maxsize=1)
+    @abstractmethod
+    def effective_area(self,
+            frequency: u.Quantity = 50*u.MHz,
+            elevation: u.Quantity = 90*u.deg
+        ) -> u.Quantity:
+        """ This method needs to be defined in child classes. """
+        return
+
+
+    @abstractmethod
+    def instrument_temperature(self, frequency: u.Quantity = 50*u.MHz, **kwargs) -> u.Quantity:
+        """ This method needs to be defined in child classes. """
+        return
+
+
+    def system_temperature(self,
+            frequency: u.Quantity = 50*u.MHz,
+            source_spectrum: Dict[str, Callable] = {},
+            efficiency: float = 1.,
+            elevation: u.Quantity = 90*u.deg,
+            **kwargs
+        ) -> u.Quantity:
+        r""" Computes the System Noise Temperature :math:`T_{\rm sys}`.
+            It is computed as follows:
+
+            .. math::
+                T_{\rm sys} = T_{\rm sky} + T_{\rm inst} + \sum_{\rm src} T_{\rm src}
+
+            where :math:`T_{\rm sky}` is an approximation of the
+            low-frequency sky temperature dominated by Galactic
+            emission and :math:`T_{\rm inst}` is the instrumental
+            noise temperature (which depends on the current
+            instrument instance).
+            :math:`T_{\rm src}` is the antenna temperature induced by a given source
+            whose spectrum is defined in the ``source_spectrum`` argument computed as:
+
+            .. math::
+                T_{\rm src} = \frac{F_{\rm src} \eta A_{\rm eff}}{2 k_{\rm B}}
+            
+            where :math:`F_{\rm src}` is the source spectrum, :math:`\eta` is the
+            ``efficiency`` of the effective area :math:`A_{\rm eff}}`.
+
+            :param frequency: 
+                Frequency for the System Temperature computation.
+                Default is ``50 MHz``.
+            :type frequency:
+                :class:`~astropy.units.Quantity`
+            :param elevation:
+                Pointing elevation impacting the :meth:`~nenupy.instru.interferometer.Interferometer.effective_area`.
+                Default is ``90 deg``.
+            :type elevation:
+                :class:`~astropy.units.Quantity`
+            :param efficiency:
+                Effective area reducing factor. Default is ``1.``, it cannot be greater than ``1.``.
+            :type efficiency:
+                `float`
+            :param source_spectrum:
+                By default the system temperature is evaluated using a mean Galactic temperature.
+                However, if a bright source is targeted, the noise introduced can be under-estimated.
+                Therefore, one can provide a `callable` object that takes as inputs a frequency array (of type :class:`~astropy.units.Quantity`) and
+                returns the source flux density in Jansky (of type :class:`~astropy.units.Quantity`).
+            :type source_spectrum:
+                `dict` of `callable`
+
+            :returns:
+                System Temperature in Kelvins.
+            :rtype:
+                :class:`~astropy.units.Quantity`
 
-# ============================================================= #
-# ------------------------ geo_to_xyz ------------------------- #
-# ============================================================= #
-@misc.accepts(EarthLocation, strict=True)
-def geo_to_etrs(earthlocation=nenufar_loc):
-    """
-    """
-    gps_b = 6356752.31424518
-    gps_a = 6378137
-    e_squared = 6.69437999014e-3
-    latRad = earthlocation.lat.rad
-    lonRad = earthlocation.lon.rad
-    alt = earthlocation.height.value
-    if earthlocation.isscalar:
-        xyz = np.zeros((1, 3))
-    else:
-        xyz = np.zeros((earthlocation.size, 3))
-    gps_n = gps_a / np.sqrt(1 - e_squared * np.sin(latRad) ** 2)
-    xyz[:, 0] = (gps_n + alt) * np.cos(latRad) * np.cos(lonRad)
-    xyz[:, 1] = (gps_n + alt) * np.cos(latRad) * np.sin(lonRad)
-    xyz[:, 2] = (gps_b**2/gps_a**2*gps_n + alt) * np.sin(latRad)
-    return xyz
-# ============================================================= #
+            .. seealso::
+                :func:`~nenupy.astro.astro_tools.sky_temperature`
 
+        """
+        t_gal = sky_temperature(frequency)
+        t_inst = self.instrument_temperature(frequency, **kwargs)
+        t_src = np.zeros(frequency.shape)*u.K
+        for _, spectrum in source_spectrum.items():
+            src_flux = spectrum(frequency)
+            t_src += (src_flux*self.effective_area(frequency, elevation)*efficiency/(2*k_B)).to(u.K)
+        return (t_gal + t_inst + t_src).to(u.K)
+
+
+    def sefd(self,
+            frequency: u.Quantity = 50*u.MHz,
+            elevation: u.Quantity = 90*u.deg,
+            efficiency: float = 1.,
+            decoherence: float = 1.,
+            source_spectrum: Dict[str, Callable] = {},
+            **kwargs
+        ) -> u.Quantity:
+        r""" Computes the System Equivalent Flux Density (SEFD or
+            system sensitivity).
+            
+            .. math::
+                S_{\rm sys} = \xi \frac{2 k_{\rm B}}{ \eta A_{\rm eff}(\nu, \theta)} T_{\rm sys} (\nu)
+            
+            with :math:`T_{\rm sys}` the :meth:`~nenupy.instru.interferometer.Interferometer.system_temperature`,
+            the efficiency :math:`\eta`, :math:`\nu` the frequency, :math:`\theta` the elevation,
+            :math:`\xi` the decoherence factor, and :math:`k_{\rm B}` the
+            Boltzmann constant.
+
+            :param frequency:
+                Frequency at which the SEFD will be computed.
+                If an array is given as input, the output will be of same shape.
+                Default if ``50 MHz``.
+            :type frequency:
+                :class:`~astropy.units.Quantity`
+            :param elevation:
+                Pointing elevation impacting the :meth:`~nenupy.instru.interferometer.Interferometer.effective_area`.
+                Default is ``90 deg``.
+            :type elevation:
+                :class:`~astropy.units.Quantity`
+            :param efficiency:
+                Effective area reducing factor. Default is ``1.``, it cannot be greater than ``1.``.
+            :type efficiency:
+                `float`
+            :param decoherence:
+                Parameter that reflects other uncertainties (particularly the unperfect phasing system).
+                Default is ``1.``.
+            :type decoherence:
+                `float`
+            :param source_spectrum:
+                By default the system temperature is evaluated using a mean Galactic temperature.
+                However, if a bright source is targeted, the noise introduced can be under-estimated.
+                Therefore, one can provide a `callable` object that takes as inputs a frequency array (of type :class:`~astropy.units.Quantity`) and
+                returns the source flux density in Jansky (of type (as :class:`~astropy.units.Quantity`).
+            :type source_spectrum:
+                `dict` of `callable`
+
+            :returns:
+                SEFD in Janskys.
+            :rtype:
+                :class:`~astropy.units.Quantity`
+        
+            .. seealso::
+                `LOFAR website <http://old.astron.nl/radio-observatory/astronomers/lofar-imaging-capabilities-sensitivity/sensitivity-lofar-array/sensiti>`_, :meth:`nenupy.instru.interferometer.Interferometer.system_temperature`
 
-# ============================================================= #
-# ------------------------ etrs_to_geo ------------------------ #
-# ============================================================= #
-@misc.accepts(np.ndarray, strict=True)
-def etrs_to_geo(positions):
-    """
-    """
-    assert (len(positions.shape)==2) and positions.shape[1]==3,\
-        'positions should be an array of shape (n, 3)'
+        """
+        effective_area = self.effective_area(frequency, elevation)
+        t_sys = self.system_temperature(frequency, source_spectrum, **kwargs)
+        sefd = decoherence*2*k_B*t_sys/(efficiency*effective_area)
+        return sefd.to(u.Jy)
+
+
+    def sensitivity(self,
+            frequency: u.Quantity = 50*u.MHz,
+            mode: ObservingMode = ObservingMode.BEAMFORMING,
+            dt: u.Quantity = 1.*u.s,
+            df: u.Quantity = 195.3125*u.kHz,
+            elevation: u.Quantity = 90*u.deg,
+            efficiency: float = 1.,
+            decoherence: float = 1.,
+            source_spectrum: Dict[str, Callable] = {},
+            **kwargs
+        ) -> u.Quantity:
+        r""" Computes the sensititivy of the array with respect to the observing configuration.
+            The sensitivity computation depends on the observing mode of the instrument:
+
+            * for the imaging mode:
+
+                .. math::
+                    \sigma_{\rm im} = \frac{S_{\rm sys}(\nu, \theta, \eta, \xi)}{
+                        \sqrt{N(N-1) 2 \Delta \nu\, \Delta t}
+                    }
+
+            * for the beamforming mode:
+
+                .. math::
+                    \sigma_{\rm bf} = \frac{S_{\rm sys}(\nu, \theta, \eta, \xi)}{
+                        \sqrt{2 \Delta \nu\, \Delta t}
+                    }
+            
+            where :math:`\nu` is the frequency, :math:`\theta` is the elevation,
+            :math:`\eta` is the effective area efficiency,
+            :math:`\xi` is the decoherence factor,
+            :math:`\Delta t` is the integration time,
+            :math:`\Delta \nu` is the bandwidth, :math:`N` is the antenna number,
+            and :math:`S_{\rm sys}` is the System Equivalent Flux Density (which also depends
+            on the ``source_spectrum`` argument, see :meth:`~nenupy.instru.interferometer.Interferometer.sefd`).
+
+            :param frequency:
+                Frequency at which the sensitivity will be evaluated.
+                If an array is given as input, the output will be of same shape.
+                Default if ``50 MHz``.
+            :type frequency:
+                :class:`~astropy.units.Quantity`
+            :param mode:
+                Observing mode, either ``ObservingMode.BEAMFORMING`` or ``ObservingMode.IMAGING``, default is the former.
+            :type mode:
+                :class:`~nenupy.instru.interferometer.ObservingMode`
+            :param dt:
+                Integration time. Default is ``1 sec``.
+            :type dt:
+                :class:`~astropy.units.Quantity`
+            :param df:
+                Observing bandwidth. Default is ``195.3125 kHz``.
+            :type df:
+                :class:`~astropy.units.Quantity`
+            :param elevation:
+                Pointing elevation impacting the :meth:`~nenupy.instru.interferometer.Interferometer.effective_area`.
+                Default is ``90 deg``.
+            :type elevation:
+                :class:`~astropy.units.Quantity`
+            :param efficiency:
+                Effective area reducing factor. Default is ``1.``, it cannot be greater than ``1.``.
+            :type efficiency:
+                `float`
+            :param decoherence:
+                Parameter that reflects other uncertainties (particularly the unperfect phasing system).
+                Default is ``1.``.
+            :type decoherence:
+                `float`
+            :param source_spectrum:
+                By default the system temperature is evaluated using a mean Galactic temperature.
+                However, if a bright source is targeted, the noise introduced can be under-estimated.
+                Therefore, one can provide a `callable` object that takes as inputs a frequency array (of type :class:`~astropy.units.Quantity`) and
+                returns the source flux density in Jansky (of type :class:`~astropy.units.Quantity`).
+            :type source_spectrum:
+                `dict` of `callable`
+
+            :return:
+                Array sensitivity.
+            :rtype:
+                :class:`~astropy.units.Quantity`
+
+            :Example:
+                >>> from nenupy.instru.interferometer import ObservingMode
+                >>> import astropy.units as u
+                >>> <instrument>.sensitivity(
+                        frequency=50*u.MHz,
+                        mode=ObservingMode.IMAGING,
+                        dt=1*u.s,
+                        df=3*u.kHz
+                    )
 
-    wgs84_a = 6378137.0
-    wgs84_f = 1./298.257223563
-    wgs84_e2 = wgs84_f*(2.0 - wgs84_f)
-    
-    x, y, z = np.transpose(positions)
-    lonRad = np.arctan2(y, x)
-    r = np.sqrt(x**2 + y**2)
-    # Iterate to latitude solution
-    phi_previous = 1e4
-    phi = np.arctan2(z, r)
-    while (np.abs(phi - phi_previous) > 1.6e-12).any():
-        phi_previous = phi
-        earthRadius = _normalizeEarthRadius(phi)
-        sinPhi = np.sin(phi)
-        phi = np.arctan2(
-            z + wgs84_e2*wgs84_a*earthRadius*sinPhi,
-            r
-        )
-    latRad = phi
-    cosLat = np.cos(latRad)
-    sinLat = np.sin(latRad)
-    heightM = r*cosLat + z*sinLat - wgs84_a*np.sqrt(1. - wgs84_e2*sinLat**2)
-
-    return EarthLocation(
-        lon=lonRad*u.rad,
-        lat=latRad*u.rad,
-        height=heightM*u.m
-    )
-# ============================================================= #
+            .. seealso::
+                :meth:`~nenupy.instru.interferometer.Interferometer.sefd` and :ref:`instrument_properties_doc`.
+
+        """
+        s_sys = self.sefd(
+            frequency=frequency,
+            elevation=elevation,
+            decoherence=decoherence,
+            efficiency=efficiency,
+            source_spectrum=source_spectrum,
+            **kwargs
+        )
+        n_ant = self.antenna_names.size
+        if mode is ObservingMode.IMAGING:
+            sensitivity = s_sys/np.sqrt(n_ant*(n_ant - 1)*2*dt*df)
+        elif mode is ObservingMode.BEAMFORMING:
+            sensitivity = s_sys/np.sqrt(2*dt*df)
+        else:
+            raise ValueError(
+                'Invalid observation mode.'
+            )
+        return sensitivity.to(u.Jy)
 
 
-# ============================================================= #
-# ------------------------ etrs_to_enu ------------------------ #
-# ============================================================= #
-@misc.accepts(np.ndarray, EarthLocation, strict=True)
-def etrs_to_enu(positions, earthlocation=nenufar_loc):
-    r""" Local east, north, up (ENU) coordinates centered on the 
-        position ``earthlocation`` (default is at the location of
-        NenuFAR).
-
-        The conversion from cartesian coordinates :math:`(x, y, z)`
-        to ENU :math:`(e, n, u)` is done as follows:
-
-        .. math::
-                \pmatrix{
-                    e \\
-                    n \\
-                    u
-                } =
-                \pmatrix{
-                    -\sin(b) & \cos(l) & 0\\
-                    -\sin(l) \cos(b) & -\sin(l) \sin(b) & \cos(l)\\
-                    \cos(l)\cos(b) & \cos(l) \sin(b) & \sin(l)
-                }
-                \pmatrix{
-                    \delta x\\
-                    \delta y\\
-                    \delta z
-                }
-
-        where :math:`b` is the longitude, :math:`l` is the
-        latitude and :math:`(\delta x, \delta y, \delta z)` are
-        the cartesian coordinates with respect to the center
-        ``earthlocation``.
-    """
-    assert (len(positions.shape)==2) and positions.shape[1]==3,\
-        'positions should be an array of shape (n, 3)'
-    xyz = positions.copy()
-    xyzCenter = geo_to_etrs(earthlocation)
-    xyz -= xyzCenter
-
-    cosLat = np.cos(earthlocation.lat.rad)
-    sinLat = np.sin(earthlocation.lat.rad)
-    cosLon = np.cos(earthlocation.lon.rad)
-    sinLon = np.sin(earthlocation.lon.rad)
-    transformation = np.array([
-        [       -sinLon,          cosLon,      0],
-        [-sinLat*cosLon, - sinLat*sinLon, cosLat],
-        [ cosLat*cosLon,   cosLat*sinLon, sinLat]
-    ])
+    def angular_resolution(self,
+            frequency: u.Quantity = 50*u.MHz
+        ) -> u.Quantity:
+        r""" Computes the angular resolution of the antenna array.
+
+            The full width at half maximum (FWHM) :math:`\theta` is approximated as follows:
+
+            .. math::
+                \theta = \frac{\lambda}{D}
+            
+            where :math:`\lambda` is the wavelength and :math:`D` is
+            is the length of the maximum physical separation of the antennas
+            in the array.
+
+            :param frequency:
+                Frequency at which the angular resolution is evaluated.
+            :type frequency:
+                :class:`~astropy.units.Quantity`
+            
+            :return:
+                Angular resolution (FWHM) of the instrument.
+            :rtype:
+                :class:`~astropy.units.Quantity`
+            
+            :Example:
+
+                >>> import astropy.units as u
+                >>> <instrument>.angular_resolution(
+                        frequency=50*u.MHz
+                    )
 
-    return np.matmul(xyz, transformation.T)
-# ============================================================= #
+        """
+        if self.size == 1:
+            raise Exception(
+                "Angular resolution is not defined for an interferometer of 1 element."
+            )
+        wavelength = frequency.to(
+            u.m,
+            equivalencies=u.spectral()
+        )
+        diameter = np.max(self.baselines.distance)
+        return (wavelength / diameter * u.rad).to(u.deg)
+
+
+    def confusion_noise(self,
+            frequency: u.Quantity = 50*u.MHz,
+            lofar: bool = True
+        ) -> u.Quantity:
+        r""" Confusion rms noise :math:`\sigma_{\rm c}` (parameter
+            used for specifying the width of the confusion
+            distribution) computed as:
+
+            .. math::
+                \left( \frac{\sigma_{\rm c}}{\rm{mJy}\, \rm{beam}^{-1}} \right) \simeq
+                0.2 \left( \frac{\nu}{\rm GHz} \right)^{-0.7} 
+                \left( \frac{\theta}{\rm arcmin} \right)^{2}
+            
+            or (if ``lofar=True``):
+            
+            .. math::
+                \left( \frac{\sigma_{\rm c}}{\mu\rm{Jy}\, \rm{beam}^{-1}} \right) \simeq
+                30 \left( \frac{\nu}{74 {\rm MHz}} \right)^{-0.7} 
+                \left( \frac{\theta}{\rm arcsec} \right)^{1.54}
+            
+            where :math:`\nu` is the frequency and :math:`\theta` is
+            the radiotelescope FWHM (see :meth:`~nenupy.instru.interferometer.Interferometer.angular_resolution`).
+            
+            Individual sources fainter than about 
+            :math:`5\sigma_{\rm c}` cannot be detected reliably.
+
+            :param freq:
+                Frequency at which computing the confusion noise.
+                In MHz if no unit is provided. Default is ``50 MHz``.
+            :type freq: `float` or :class:`~astropy.units.Quantity`
+            :param miniarrays:
+                Mini-Array indices to take into account.
+                Default is ``None`` (all available MAs).
+            :type miniarrays: `int`, `list` or :class:`~numpy.ndarray`
+            :param lofar:
+                If set to ``True`` (recommended), the confusion noise
+                is estimated using Eq. 6 of `van Haarlem et al. (2013) <https://arxiv.org/pdf/1305.3550.pdf>`_.
+            :type:
+                `bool`
+
+            :returns:
+                Confusion rms noise in Jy/beam
+            :rtype:
+                :class:`~astropy.units.Quantity`
+
+            :Example:
+                >>> import astropy.units as u
+                >>> <instrument>.confusion_noise(
+                        frequency=50*u.MHz
+                    )
+
+            .. see also::
+                `NRAO lecture <https://www.cv.nrao.edu/course/astr534/Radiometers.html>`_ (eq. 3E6),
+                `Takeuchi and Ishii, 2004 <https://ui.adsabs.harvard.edu/abs/2004ApJ...604...40T/abstract>`_.
+        """
+        resolution = self.angular_resolution(frequency=frequency)
+        if lofar: # https://arxiv.org/pdf/1305.3550.pdf
+            freq_at_74mHz = (frequency.to(u.MHz)/(74*u.MHz)).value
+            res_in_asec = resolution.to(u.arcsec).value
+            conf = 30 * res_in_asec**1.54 * freq_at_74mHz**(-0.7) * u.uJy
+        else:
+            # freq_in_ghz = frequency.to(u.GHz).value
+            # res_in_asec = resolution.to(u.arcsec).value
+            # conf = 1.2 * (freq_in_ghz/3.02)**(-0.7) * (res_in_asec/8)**(10/3) * u.uJy # condon 2012
+            freq_in_ghz = frequency.to(u.GHz).value
+            res_in_amin = resolution.to(u.arcmin).value
+            conf = 0.2 * freq_in_ghz**(-0.7) * res_in_amin**2 * u.mJy # Condon 2002
+
+        return conf.to(u.Jy) # Jy/beam
 
 
-# ============================================================= #
-# ------------------------ enu_to_etrs ------------------------ #
-# ============================================================= #
-@misc.accepts(np.ndarray, EarthLocation, strict=True)
-def enu_to_etrs(positions, earthlocation=nenufar_loc):
-    """
-    """
-    assert (len(positions.shape)==2) and positions.shape[1]==3,\
-        'positions should be an array of shape (n, 3)'
-    enu = positions.copy()
-
-    cosLat = np.cos(earthlocation.lat.rad)
-    sinLat = np.sin(earthlocation.lat.rad)
-    cosLon = np.cos(earthlocation.lon.rad)
-    sinLon = np.sin(earthlocation.lon.rad)
-    transformation = np.array([
-        [       -sinLon,          cosLon,      0],
-        [-sinLat*cosLon, - sinLat*sinLon, cosLat],
-        [ cosLat*cosLon,   cosLat*sinLon, sinLat]
-    ])
-
-    xyz = np.matmul(enu, np.linalg.inv(transformation).T)
-    xyzCenter = geo_to_etrs(earthlocation)
-    xyz += xyzCenter
+    # --------------------------------------------------------- #
+    # ----------------------- Internal ------------------------ #
+    def _geometric_delays(self, sky: Sky, pointing: Pointing) -> da.Array:
+        """ Computes the geometric delays between the sky and the pointing direction(s).
+        """
+        sky_projection = sky.ground_projection
+        pointing_projection = pointing.ground_projection
 
-    return xyz
+        # coord_chunk = sky_projection.shape[-1]//cpu_count()
+        # coord_chunk = 1 if coord_chunk == 0 else coord_chunk
+        # chunk_shape = sky_projection.shape[:-1] + (coord_chunk,)
+        chunk_shape = (1, 1, 1, 3,) + (sky_projection.shape[-1],)
+
+        sky_projection = da.from_array(
+            sky_projection,
+            chunks=chunk_shape
+        )
+        pointing_projection = da.from_array(
+            pointing_projection,
+            chunks=chunk_shape
+        )
+
+        # Put the ground antennas in the sky
+        angle = np.pi/2
+        rot_90 = np.array(
+            [
+                [np.cos(angle), -np.sin(angle), 0],
+                [np.sin(angle), np.cos(angle), 0],
+                [0,           0,           1]
+            ]
+        )
+
+        return np.dot(
+            np.dot(self.antenna_positions, rot_90),
+            sky_projection - pointing_projection
+        )
+# ============================================================= #
 # ============================================================= #
-
```

### Comparing `nenupy-2.1.0/nenupy/base.py` & `nenupy-2.2.9/nenupy/base.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/beamlet/beamlet.py` & `nenupy-2.2.9/nenupy/beamlet/beamlet.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/beamlet/bstdata.py` & `nenupy-2.2.9/nenupy/beamlet/bstdata.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/beamlet/sdata.py` & `nenupy-2.2.9/nenupy/beamlet/sdata.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,14 +571,15 @@
                 kwargs['vmax'] = np.nanpercentile(dynspec, 95)
             else:
                 pass
             plt.pcolormesh(
                 self.datetime,
                 self.freq.to(u.MHz).value,
                 dynspec,
+                shading='auto',
                 cmap=kwargs['cmap'],
                 vmin=kwargs['vmin'],
                 vmax=kwargs['vmax']
             )
             if 'altaza' in kwargs.keys():
                     ptimes = kwargs['altaza'].pointingTimes
                     for ptime in ptimes:
```

### Comparing `nenupy-2.1.0/nenupy/beamlet/sstdata.py` & `nenupy-2.2.9/nenupy/beamlet/sstdata.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/instru/NenuFAR_Ant_Hpx.fits` & `nenupy-2.2.9/nenupy/instru/NenuFAR_Ant_Hpx.fits`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/instru/__init__.py` & `nenupy-2.2.9/nenupy/instru/__init__.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/instru/instrument_tools.py` & `nenupy-2.2.9/nenupy/instru/instrument_tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,22 +17,24 @@
 __email__ = "alan.loh@obspm.fr"
 __status__ = "Production"
 __all__ = [
     "freq2sb",
     "sb2freq",
     "instrument_temperature",
     "miniarrays_rotated_like",
-    "read_cal_table"
+    "read_cal_table",
+    "generate_nenufar_subarrays"
 ]
 
 
 import numpy as np
 import astropy.units as u
 from typing import List
 from os.path import join, dirname
+from scipy.interpolate import interp2d
 
 from nenupy.instru import lna_gain
 from nenupy.astro.astro_tools import sky_temperature
 from nenupy.instru import nenufar_miniarrays
 
 import logging
 log = logging.getLogger(__name__)
@@ -57,21 +59,27 @@
 
         :returns:
             Sub-band index, same shape as ``frequency``.
         :rtype:
             `int` or :class:`~numpy.ndarray`
 
         :example:
-            >>> from nenupy.instru import freq2sb
-            >>> freq2sb(frequency=50.5*u.MHz)
-            259
-            >>> freq2sb(frequency=[50.5, 51]*u.MHz)
-            array([259, 261])
+            .. code-block:: python
+                
+                from nenupy.instru import freq2sb
+                import astropy.units as u
+
+                freq2sb(frequency=50.5*u.MHz)
+                freq2sb(frequency=[50.5, 51]*u.MHz)
 
     """
+    if not isinstance(frequency, u.Quantity):
+        raise TypeError(
+            f"`frequency` - {u.Quantity} expected."
+        )
     if (frequency.min() < 0 * u.MHz) or (frequency.max() > 100 * u.MHz):
         raise ValueError(
             "'frequency' should be between 0 and 100 MHz."
         )
     frequency = frequency.to(u.MHz)
     sb_width = 100. * u.MHz / 512
     sb_idx = np.floor(frequency/sb_width + 0.5)
@@ -101,32 +109,34 @@
             `int` or :class:`~numpy.ndarray` of `int`
 
         :returns:
             Sub-band start frequency :math:`\nu_{\rm start}` in MHz.
         :rtype:
             :class:`~astropy.units.Quantity`
 
-        :example:
-            >>> from nenupy.instru import sb2freq
-            >>> sb2freq(subband=1)
-            [0.09765625] MHz
-            >>> sb2freq(subband=[1, 2, 3, 4])
-            [0.09765625, 0.29296875, 0.48828125, 0.68359375] MHz
+        :Example:
+            .. code-block:: python
+            
+                from nenupy.instru import sb2freq
+
+                sb2freq(subband=1)
+                sb2freq(subband=[1, 2, 3, 4])
+
     """
     if np.isscalar(subband):
         subband = np.array([subband])
     else:
         subband = np.array(subband)
     if subband.dtype.name not in ['int32', 'int64']:
         raise TypeError(
-            "'subband' should be integers."
+            "`subband` - Integer(s) expected."
         )
     if (subband.min() < 0) or (subband.max() > 511):
         raise ValueError(
-            "'sb' should be between 0 and 511."
+            "`subband` - Values should be between 0 and 511."
         )
     sb_width = 100.*u.MHz/512 #200e6*192/1024# + 195312.5/2
     freq_start = subband*sb_width - sb_width/2
     return freq_start
 # ============================================================= #
 # ============================================================= #
 
@@ -152,21 +162,25 @@
         :type lna_filter:
             `int`
 
         :returns:
             Instrument temperature in Kelvins
         :rtype:
             :class:`~astropy.units.Quantity`
+        
+        .. warning::
+            For the time being, only ``lna_filter`` values ``0`` and ``3`` are available.
 
         :Example:
+            .. code-block:: python
+            
+                from nenupy.instru import instrument_temperature
+                import astropy.units as u
 
-            >>> from nenupy.instru import instrument_temperature
-            >>> import astropy.units as u
-            >>> instrument_temperature(frequency=70*u.MHz)
-            526.11213 K
+                instrument_temperature(frequency=70*u.MHz)
 
         .. seealso::
             :func:`~nenupy.astro.astro_tools.sky_temperature`
 
     """
     # Available filters
     filters = {0: "no_filter", 3: "25mhz_filter"}
@@ -198,18 +212,19 @@
 
         :returns:
             Mini-Array indices.
         :rtype:
             :class:`~numpy.ndarray`
 
         :Example:
-
-            >>> from nenupy.instru import miniarrays_rotated_like
-            >>> miniarrays_rotated_like([10])
-            array([11, 12, 18, 22, 43, 47, 54, 56, 60, 66, 70, 77])
+            .. code-block:: python
+            
+                from nenupy.instru import miniarrays_rotated_like
+                
+                miniarrays_rotated_like([10])
 
     """
     # Check that the rotation format is correct
     if not all([rot%10 == 0 for rot in rotations]):
         raise ValueError(
             f"Syntax error: miniarray_rotations={rotations}. It should be a list of integers, multiples of 10."
         )
@@ -220,15 +235,15 @@
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
 # ---------------------- read_cal_table ----------------------- #
 # ============================================================= #
-def read_cal_table(calibration_file=None):
+def read_cal_table(calibration_file: str = None) -> np.ndarray:
     """ Reads NenuFAR antenna delays calibration file.
 
         :param calibration_file: 
             Name of the calibration file to read. If ``None`` or
             ``'default'`` the standard calibration file is read.
         :type calibration_file: `str`
 
@@ -268,7 +283,76 @@
     )
     decoded = tmp.view(dtype)[0]["data"]
     data = decoded[..., 0] + 1.j*decoded[..., 1]
     return data
 # ============================================================= #
 # ============================================================= #
 
+
+# ============================================================= #
+# ---------------- generate_nenufar_subarrays ----------------- #
+# ============================================================= #
+def generate_nenufar_subarrays(
+        n_subarrays: int = 2,
+        include_remote_mas: bool = False
+    ):
+    """ Generates NenuFAR sub-arrays of Mini-Arrays. The sub-arraying
+        is done completely randomly.
+
+        :param n_subarrays:
+            Number of sub-arrays to generate from the NenuFAR
+            Mini-Array distribution. Default is `2`.
+        :type n_subarrays:
+            `int`
+        :param include_remote_mas:
+            Include or not the remote Mini-Arrays.
+        :type include_remote_mas:
+            `bool`
+        
+        :returns:
+            A list of Mini-Array names for each sub-array.
+        :rtype:
+            `list` of `~numpy.ndarray`
+
+        :Example:
+            .. code-block:: python
+
+                from nenupy.instru import generate_nenufar_subarrays
+                from nenupy.instru import NenuFAR
+
+                sub_arrays = generate_nenufar_subarrays(n_subarrays=2)
+                sub_array_1 = NenuFAR()[sub_arrays[0]]
+                sub_array_2 = NenuFAR()[sub_arrays[1]]
+
+    """
+
+    if n_subarrays < 2:
+        raise ValueError(
+            "`n_subarrays` should be at least equal to 2."
+        )
+
+    # Number of Mini-Arrays
+    n_mas = 96
+    if include_remote_mas:
+        n_mas = 102
+
+    # Mini-Arrays names
+    ma_names = np.array([ma_name for ma_name in nenufar_miniarrays.keys()])
+    ma_names = ma_names[:n_mas]
+
+    # Generate random values
+    rng = np.random.default_rng()
+    ma_values = rng.random(n_mas) # floats between [0, 1[
+
+    # Create mask by evaluating the random value per MA
+    edge_values = np.linspace(0, 1, n_subarrays + 1)
+    subarray_masks = (edge_values[:-1][:, None] <= ma_values[None, :]) & (ma_values[None, :] < edge_values[1:][:, None]) 
+
+    # Check that each Mini-Array is counted once
+    if not np.all(np.sum(subarray_masks, axis=0)==1):
+        raise ValueError("Something's wrong.")
+
+    # Return a list of sub-arrays (numpy arrays of Mini-Array names)
+    return [ma_names[subarray_masks[i]] for i in range(n_subarrays)]
+# ============================================================= #
+# ============================================================= #
+
```

### Comparing `nenupy-2.1.0/nenupy/instru/interferometer.py` & `nenupy-2.2.9/nenupy/io/io_tools.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,999 +1,1216 @@
 #! /usr/bin/python3
 # -*- coding: utf-8 -*-
 
 
 """
-    *********************
-    Interferometric Array
-    *********************
+    ********
+    BST file
+    ********
 """
 
 
-__author__ = "Alan Loh"
-__copyright__ = "Copyright 2021, nenupy"
-__credits__ = ["Alan Loh"]
-__maintainer__ = "Alan"
-__email__ = "alan.loh@obspm.fr"
-__status__ = "Production"
+__author__ = 'Alan Loh'
+__copyright__ = 'Copyright 2021, nenupy'
+__credits__ = ['Alan Loh']
+__maintainer__ = 'Alan'
+__email__ = 'alan.loh@obspm.fr'
+__status__ = 'Production'
 __all__ = [
-    "Baseline",
-    "ObservingMode",
-    "Interferometer"
+    "StatisticsData",
+    "ST_Slice"
 ]
 
 
-from abc import ABC, ABCMeta, abstractmethod
-import copy
-from enum import Enum, auto
-from functools import lru_cache
-from os import cpu_count
-from typing import Dict, Callable
-import logging
-log = logging.getLogger(__name__)
-
+from abc import ABC
+import operator
+import re
+from typing import Callable
+from astropy.io import fits
+from astropy.time import Time, TimeDelta
+from scipy.signal import find_peaks
+from astropy.modeling import fitting
+from astropy.modeling.models import custom_model
+import astropy.units as u
 import numpy as np
 import matplotlib.pyplot as plt
+import matplotlib.dates as mdates
+from mpl_toolkits.axes_grid1.inset_locator import inset_axes
+from scipy import ndimage
 
-import astropy.units as u
-from astropy.constants import k_B
-from astropy.coordinates import (
-    EarthLocation,
-    Angle
-)
-import dask.array as da
-from dask.diagnostics import ProgressBar
-
-from nenupy import LogMethodMetaClass, DummyCtMgr
-from nenupy.astro.sky import Sky
-from nenupy.astro.astro_tools import sky_temperature
-from nenupy.astro.pointing import Pointing
-
-
-# ============================================================= #
-# ---------------- Interferometer class errors ---------------- #
-# ============================================================= #
-class CombinedMeta(LogMethodMetaClass, ABCMeta):
-    """ Intermediate metaclass when inheriting from ABC. """
-
-
-class AntennaNameError(Exception):
-    """ Error raised when the name doesn't match existing antenna names. """
-
-    def __init__(self,
-            input_name: np.ndarray,
-            available_antennas: np.ndarray
-        ):
-        self.input_name = input_name
-        self.message = f"Valid antenna names are {available_antennas}."
-        super().__init__(self.message)
-
-
-    def __str__(self):
-        return f"'{self.input_name}'\n{self.message}"
+from nenupy.instru.instrument_tools import sb2freq
 
+import logging
+log = logging.getLogger(__name__)
 
-class AntennaIndexError(Exception):
-    """ Error raised when the index doesn't match existing antenna indices. """
-
-    def __init__(self,
-            input_index: np.ndarray,
-            n_available_antennas: int
-        ):
-        self.input_index = input_index
-        self.message = f"Maximum antenna index is {n_available_antennas - 1}."
-        super().__init__(self.message)
-
-
-    def __str__(self):
-        return f"{self.input_index}\n{self.message}"
-
-
-class DuplicateAntennaError(Exception):
-    """ Error raised when antennas are duplicated. """
-
-    def __init__(self,
-            input_antenna: np.ndarray,
-        ):
-        self.input_antenna = input_antenna
-        unique, counts = np.unique(self.input_antenna, return_counts=True)
-        duplicate_mask = [counts > 1]
-        dup = unique[tuple(duplicate_mask)]
-        cnt = counts[tuple(duplicate_mask)]
 
-        self.message = f"antenna name/index {dup} is duplicated {cnt} times."
-        super().__init__(self.message)
+ops = {
+    '>': operator.gt,
+    '<': operator.lt,
+    '>=': operator.ge,
+    '<=': operator.le,
+    '==': operator.eq,
+}
 
 
-    def __str__(self):
-        return f"{self.input_antenna}: {self.message}"
 # ============================================================= #
+# ---------------------- StatisticsData ----------------------- #
 # ============================================================= #
+class StatisticsData(ABC):
+    """ """
 
+    def __init__(self, file_name: str):
+        self.file_name = file_name
+        #self.instrument = None
+        #self.pointing = None
 
-# ============================================================= #
-# ------------------------- Baseline -------------------------- #
-# ============================================================= #
-class Baseline:
-    """ Class to handle interferometric baseline operations. """
+        self._meta_data = {}
+        self._lazy_load()
+    
 
-    def __init__(self, itrf_positions: np.ndarray):
-        self.itrf_positions = itrf_positions
+    def _lazy_load(self):
+        """ """
+        with fits.open(self.file_name,
+            mode='readonly',
+            ignore_missing_end=True,
+            memmap=True
+        ) as f:
+            # Metadata loading
+            # self.meta['hea'] = f[0].header
+            self._meta_data['ins'] = f[1].data
+            self._meta_data['obs'] = f[2].data
+            self._meta_data['ana'] = f[3].data
+            self._meta_data['bea'] = f[4].data
+            self._meta_data['pan'] = f[5].data
+            self._meta_data['pbe'] = f[6].data
+
+            # # Data loading 
+            self.time = Time(f[7].data['JD'], format='jd')
+            self.data = f[7].data['data']
+            try:
+                # For XST data, the frequencies are in the data extension
+                # self.frequencies = sb2freq(
+                #     np.unique(f[7].data['xstsubband']).astype("int")
+                # ) + 195.3125*u.kHz/2 # mid frequency
+                self.frequencies = sb2freq(
+                    f[7].data['xstsubband'].astype("int")
+                ) + 195.3125*u.kHz/2 # mid frequency
+            except KeyError:
+                pass
 
-        if self.itrf_positions.ndim != 2:
-            raise ValueError(
-                "<arg 'itrf_positions'>: instance of "
-                f"{np.ndarray} of dimension 2 expected. "
-                f"Got {self.itrf_positions.shape} instead."
-            )
-        self.antenna_idx = np.arange(self.itrf_positions.shape[0])
-        xyz = self.itrf_positions[..., None]
-        xyz = xyz[:, :, 0][:, None]
-        self.bsl = xyz.transpose(1, 0, 2) - xyz
+        return
 
 
-    def __getitem__(self, n):
-        pos = self.itrf_positions[n, :]
-        return Baseline(
-            itrf_positions=pos
-        )
+    @staticmethod
+    def _parse_condition(conditions, converter):
+        """ """
+        condition_list = conditions.replace(" ", "").split("&")
+
+        cond = []
+        for condition in condition_list:
+            try:
+                op = re.search('((>=)|(<=)|(==)|(<)|(>))', condition).group(0)
+                val = re.search(f'(?<={op})(.*)', condition).group(0)
+            except AttributeError:
+                log.error(
+                    f"Selection syntax '{condition}' not understood."
+                )
+                raise
+            val = converter(val)
+            op = ops[op]
+            cond.append( lambda x, op=op, val=val: op(converter(x), val) )
+
+        if len(cond) == 2:
+            return lambda x, cond1=cond[0], cond2=cond[1]: operator.and_(cond1(x), cond2(x))
+        elif len(cond) == 1:
+            return cond[0]
+        else:
+            raise Exception
 
 
-    # --------------------------------------------------------- #
-    # --------------------- Getter/Setter --------------------- #
-    @property
-    def flatten(self):
-        """
-        """
-        return self.bsl[
-            np.tril_indices(self.antenna_idx.size)
-        ]
+    def _parse_time_condition(self, conditions):
+        """ """
+        return self._parse_condition(conditions, lambda t: Time(t).jd)
 
 
-    @property
-    def distance(self):
-        """
-        """
-        return np.linalg.norm(self.bsl, axis=2) * u.m
+    def _parse_frequency_condition(self, conditions):
+        """ """
+        return self._parse_condition(conditions, lambda f: u.Quantity(f))
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
-# ----------------------- ObservingMode ----------------------- #
+# ------------------------- ST_Slice -------------------------- #
 # ============================================================= #
-class ObservingMode(Enum):
-    """ Enumerator of the different available observing modes of NenuFAR. """
+class InconsistentShapeError(Exception):
+    """ Error raised when an operation between two ST_Slice
+        objects is performed although they have different time
+        and freequency axes.
+    """
 
-    BEAMFORMING = auto()
-    IMAGING = auto()
-# ============================================================= #
-# ============================================================= #
+    def __init__(self):
+        self.message = (
+            "Operation between two ST_Slice instances with "
+            "un-identical time and frequency axes is prohibited."
+        )
+        super().__init__(self.message)
 
+    def __str__(self):
+        return f"{self.message}"
 
-# ============================================================= #
-# ---------------------- Interferometer ----------------------- #
-# ============================================================= #
-class Interferometer(ABC, metaclass=CombinedMeta):
-    """ Abstract base class for all phased-array/interferometer classes.
+
+class ST_Slice:
+    """ Class to handle data sub-set from Statistical data.
 
         .. rubric:: Attributes Summary
 
         .. autosummary::
 
-            ~nenupy.instru.interferometer.Interferometer.antenna_gains
-            ~nenupy.instru.interferometer.Interferometer.antenna_names
-            ~nenupy.instru.interferometer.Interferometer.antenna_positions
-            ~nenupy.instru.interferometer.Interferometer.baselines
-            ~nenupy.instru.interferometer.Interferometer.position
-            ~nenupy.instru.interferometer.Interferometer.size
+            ~ST_Slice.time
+            ~ST_Slice.frequency
+            ~ST_Slice.value
+            ~ST_Slice.analog_pointing_times
+            ~ST_Slice.digital_pointing_times
 
         .. rubric:: Methods Summary
 
         .. autosummary::
 
-            ~nenupy.instru.interferometer.Interferometer.angular_resolution
-            ~nenupy.instru.interferometer.Interferometer.array_factor
-            ~nenupy.instru.interferometer.Interferometer.beam
-            ~nenupy.instru.interferometer.Interferometer.confusion_noise
-            ~nenupy.instru.interferometer.Interferometer.plot
-            ~nenupy.instru.interferometer.Interferometer.sefd
-            ~nenupy.instru.interferometer.Interferometer.sensitivity
-            ~nenupy.instru.interferometer.Interferometer.system_temperature
+            ~ST_Slice.plot
+            ~ST_Slice.rebin
+            ~ST_Slice.fit_transit
+            ~ST_Slice.flatten_frequency
+            ~ST_Slice.flatten_time
+            ~ST_Slice.clear_pointing_switch
 
         .. rubric:: Attributes and Methods Documentation
 
     """
 
     def __init__(self,
-            position: EarthLocation,
-            antenna_names: np.ndarray,
-            antenna_positions: np.ndarray,
-            antenna_gains: np.ndarray
+            time: Time,
+            frequency: u.Quantity,
+            value: np.ndarray,
+            analog_pointing_times: Time = Time([], format='jd'),
+            digital_pointing_times: Time = Time([], format='jd')
         ):
-        self.position = position
-        self.antenna_names = antenna_names
-        self.antenna_positions = antenna_positions
-        self.antenna_gains = antenna_gains
-
-
-    def __getitem__(self, n):
-        if isinstance(n, slice):
-            # Convert the slice into a numpy array
-            n = np.r_[n]
-        elif not isinstance(n, np.ndarray):
-            n = np.array(n)
-            if np.isscalar(n):
-                n = n.reshape((1,))
+        self._time = time
+        self._frequency = frequency
+        self._value = value
+        self._analog_pointing_times = analog_pointing_times
+        self._digital_pointing_times = digital_pointing_times
+
 
-        # Checking the correct input format
-        if n.ndim > 1:
+    def __and__(self, other):
+        """ Concatenates two ST_Slice in frequency.
+        """
+        if not all(self.time == other.time):
             raise ValueError(
-                "<class 'Interferometer'> can only be "
-                f"subscriptable by 1D arrays. Got {n} instead."
+                f"The {ST_Slice} objects to concatenate in "
+                "frequency do not have equal time axes."
             )
-        if np.unique(n).size != n.size:
-            raise DuplicateAntennaError(n)
 
-        # Generating antenna mask
-        if n.dtype.str.startswith('<U'):
-            # Selection based on antenna names
-            antenna_mask = np.isin(self.antenna_names, n)
-            bad_name_index = ~np.isin(n, self.antenna_names)
-            if np.any(bad_name_index):
-                raise AntennaNameError(
-                    n[bad_name_index],
-                    self.antenna_names
-                )
+        log.info(
+            f"Concatenating in frequency ({self.frequency.size}, {other.frequency.size})."
+        )
+
+        if self.frequency.max() < other.frequency.min():
+            new_data = np.hstack((self.value, other.value))
+            new_freq = np.concatenate((self.frequency, other.frequency))
         else:
-            # Selection based on antenna indices
-            if n.max() >= self.size:
-                raise AntennaIndexError(n, self.size)
-            antenna_mask = np.isin(np.arange(self.size), n)
-
-        # Constructing the new instance as a 'cutout' of its parent
-        interfero = copy.deepcopy(self)
-        interfero.antenna_names = self.antenna_names[antenna_mask]
-        interfero.antenna_positions = self.antenna_positions[antenna_mask, :]
-        interfero.antenna_gains = self.antenna_gains[antenna_mask]
-        return interfero
+            new_data = np.hstack((other.value, self.value))
+            new_freq = np.concatenate((other.frequency, self.frequency))
+        
+        unique_freqs_nb = np.unique(new_freq).size
+        if unique_freqs_nb != new_freq.size:
+            log.warning(
+                f"There are {new_freq.size - unique_freqs_nb} overlaps in the frequency axis."
+            )
+
+        return ST_Slice(
+            time=self.time,
+            frequency=new_freq,
+            value=new_data,
+            analog_pointing_times=self.analog_pointing_times,
+            digital_pointing_times=self.digital_pointing_times
+        )
+
+
+    def __or__(self, other):
+        """ Concatenates two ST_Slice in time.
+        """
+        if not all(self.frequency == other.frequency):
+            raise ValueError(
+                f"The {ST_Slice} objects to concatenate in "
+                "time do not have equal frequency axes."
+            )
 
+        log.info(
+            f"Concatenating in time ({self.time.size}, {other.time.size})."
+        )
 
-    def __repr__(self):
-        return f"{self.__class__}"
+        if self.time.max() < other.time.min():
+            new_data = np.hstack((self.value, other.value))
+            new_time = Time(np.hstack((self.time.jd, other.time.jd)), format='jd')
+            new_ana_times = Time(np.hstack((self.analog_pointing_times.jd, other.analog_pointing_times.jd)), format='jd')
+            new_digi_times = Time(np.hstack((self.digital_pointing_times.jd, other.digital_pointing_times.jd)), format='jd')
+        else:
+            new_data = np.hstack((other.value, self.value))
+            new_time = Time(np.hstack((other.time.jd, self.time.jd)), format='jd')
+            new_ana_times = Time(np.hstack((other.analog_pointing_times.jd, self.analog_pointing_times.jd)), format='jd')
+            new_digi_times = Time(np.hstack((other.digital_pointing_times.jd, self.digital_pointing_times.jd)), format='jd')
+
+        # unique_times_nb = np.unique(new_time).size
+        # if unique_times_nb != new_time.size:
+        #     log.warning(
+        #         f"There are {new_time.size - unique_times_nb} overlaps in the time axis."
+        #     )
+
+        return ST_Slice(
+            time=new_time,
+            frequency=self.frequency,
+            value=new_data,
+            analog_pointing_times=new_ana_times,
+            digital_pointing_times=new_digi_times
+        )
 
 
-    def __str__(self):
-        return f"{self.__class__.__name__}"
+    def __getitem__(self, slice_tuple):
+        """ (time, frequency) """
+        # Expects an explicit tuple of length 2
+        if not (isinstance(slice_tuple, tuple) and\
+                (len(slice_tuple) == 2) and\
+                all([isinstance(s, slice) for s in slice_tuple])
+            ):
+            raise IndexError("Only tuple of two slices allowed.")
+        return ST_Slice(
+            time=self.time[slice_tuple[0]],
+            frequency=self.frequency[slice_tuple[1]],
+            value=self.value[slice_tuple],
+            analog_pointing_times=self.analog_pointing_times,
+            digital_pointing_times=self.digital_pointing_times
+        )
 
 
     def __add__(self, other):
-        interferometer = copy.deepcopy(self)
-        to_include = ~np.isin(other.antenna_names, self.antenna_names)
-        interferometer.antenna_names = np.concatenate((self.antenna_names, other.antenna_names[to_include]))
-        interferometer.antenna_positions = np.concatenate((self.antenna_positions, other.antenna_positions[to_include]))
-        interferometer.antenna_gains = np.concatenate((self.antenna_gains, other.antenna_gains[to_include]))
-        return interferometer
-    
+        """ """
+        return self._operation_with_other(other, np.add)
+
 
     def __sub__(self, other):
-        interferometer = copy.deepcopy(self)
-        to_keep = ~np.isin(self.antenna_names, other.antenna_names)
-        interferometer.antenna_names = self.antenna_names[to_keep]
-        interferometer.antenna_positions = self.antenna_positions[to_keep]
-        interferometer.antenna_gains = self.antenna_gains[to_keep]
-        return interferometer
+        """ """
+        return self._operation_with_other(other, np.subtract)
+
+
+    def __mul__(self, other):
+        """ """
+        return self._operation_with_other(other, np.multiply)
+    
+
+    def __truediv__(self, other):
+        """ """
+        return self._operation_with_other(other, np.divide)
 
 
     # --------------------------------------------------------- #
     # --------------------- Getter/Setter --------------------- #
     @property
-    def size(self):
-        """ Number of elements belonging to the array. 
+    def time(self) -> Time:
+        """ Data record times.
+            
+            :getter: Time array.
+            
+            :type: :class:`~astropy.time.Time`
+        """
+        return self._time
 
-            :getter: Size of the array.
 
-            :type: `int`
+    @property
+    def frequency(self) -> u.Quantity:
+        """ Data record frequencies.
+            
+            :getter: Frequency array.
+            
+            :type: :class:`~astropy.units.Quantity`
         """
-        return self.antenna_positions.shape[0]
+        return self._frequency
 
 
     @property
-    def baselines(self):
-        """ Instrument baselines.
+    def value(self) -> np.ndarray:
+        """ Data values.
+            
+            :getter: Values array.
+            
+            :type: :class:`~numpy.ndarray`
+        """
+        return self._value
 
-            :getter: Baselines.
 
-            :type: :class:`~nenupy.instru.interferometer.Baseline`
+    @property
+    def analog_pointing_times(self) -> Time:
+        """ Analog pointing start times corresponding to this data set.
+            
+            :getter: Starting times array.
+            
+            :type: :class:`~astropy.time.Time`
         """
-        try:
-            antenna_position = self._toITRF()
-        except AttributeError:
-            log.error("No method '_toITRF()' is implemented.")
-            raise
-        return Baseline(itrf_positions=antenna_position)
+        return self._analog_pointing_times
 
 
     @property
-    def antenna_names(self) -> np.ndarray:
-        """ Antenna names.
+    def digital_pointing_times(self) -> Time:
+        """ Digital pointing start times corresponding to this data set.
+            
+            :getter: Starting times array.
+            
+            :type: :class:`~astropy.time.Time`
+        """
+        return self._digital_pointing_times
+
+
+    # --------------------------------------------------------- #
+    # ------------------------ Methods ------------------------ #
+    def plot(self, fig_ax=None, **kwargs):
+        r""" Plots the data, while automatically taking into account
+            its shape (lightcurve, spectrum or dynamic spectrum). 
+
+            Several parameters, listed below, can be tuned to adapt the plot
+            to the user requirements:
+
+            .. rubric:: Data display keywords
+
+            :param decibel:
+                If set to ``True``, the data will be displayed in
+                a decibel scale (i.e., :math:`{\rm dB} = 10 \log_{10}({\rm data})`).
+                Default is ``True``.
+            :type decibel:
+                `bool`
+            :param xmin:
+                Minimal x-axis value (could be either time or
+                frequency units depending on the data shape).
+                Default is automatic scaling.
+            :type xmin:
+                :class:`~astropy.units.Quantity` or :class:`~astropy.time.TimeDatetime`
+            :param xmax:
+                Maximal x-axis value (could be either time or
+                frequency units depending on the data shape).
+                Default is automatic scaling.
+            :type xmax:
+                :class:`~astropy.units.Quantity` or :class:`~astropy.time.TimeDatetime`
+            :param ymin:
+                Minimal y-axis value (could be either data amplitude or
+                frequency units depending on the data shape).
+                Default is automatic scaling.
+            :type ymin:
+                `float` or :class:`~astropy.units.Quantity`
+            :param ymax:
+                Maximal y-axis value (could be either data amplitude or
+                frequency units depending on the data shape).
+                Default is automatic scaling.
+            :type ymax:
+                `float` or :class:`~astropy.units.Quantity`
+            :param vmin:
+                *Dynamic spectrum plot only*.
+                Minimal data value to display.
+            :type vmin:
+                `float`
+            :param vmax:
+                *Dynamic spectrum plot only*.
+                Maximal data value to display.
+            :type vmax:
+                `float`
 
-            :setter: Array of antenna names.
+            .. rubric:: Overplot keywords
 
-            :getter: Array of antenna names.
+            :param vlines:
+                *Temporal plot only*.
+                Adds vertical lines at specific times.
+                The expected format is an array of :class:`~astropy.time.TimeDatetime`.
+                Default is ``[]``.
+            :type vlines:
+                [:class:`~astropy.time.TimeDatetime`]
+            :param analog_pointing:
+                *Temporal plot only*.
+                Overplots vertical dot-dashed black lines at analog pointing start times.
+                Default is ``False``.
+            :type analog_pointing:
+                `bool`
+            :param digital_pointing:
+                *Temporal plot only*.
+                Overplots vertical dotted black lines at analog pointing start times.
+                Default is ``False``.
+            :type digital_pointing:
+                `bool`
+            :param hatched_overlay:
+                *Dynamic spectrum plot only*.
+                Produces a hatched overlay on top of the dynamic spectrum.
+                The expected format is ``(time, frequency, hatched_array)``
+                where ``hatched_array`` is a boolean :class:`~numpy.ndarray`,
+                shaped as (frequency, time),
+                set to ``True`` where a hatched cell should be drawn.
+                Default is ``None``.
+            :type hatched_overlay:
+                (:class:`~astropy.time.Time`, :class:`~astropy.units.Quantity`, :class:`~numpy.ndarray`)
 
-            :type: :class:`~numpy.ndarray`
-        """
-        return self._antenna_names
-    @antenna_names.setter
-    def antenna_names(self, n: np.ndarray):
-        self._antenna_names = n
+            .. rubric:: Plotting layout keywords
 
-    
-    @property
-    def antenna_positions(self) -> np.ndarray:
-        """ Antenna positions.
-            The positions should be shaped as ``(n_ant, 3)``
+            :param figname:
+                Name of the file (absolute or relative path) to save the figure.
+                Default is ``''`` (i.e., only show the figure).
+            :type figname:
+                `str`
+            :param figsize:
+                Set the figure size.
+                Default is ``(15, 7)``.
+            :type figsize:
+                `tuple`
+            :param title:
+                Set the figure title.
+                Default is ``''``.
+            :type title:
+                `str`
+            :param colorbar_label:
+                *Dynamic spectrum plot only*.
+                Label of the color bar.
+                Default is ``'Amp'`` if ``decibel=False`` and ``'dB'`` otherwise.
+            :type colorbar_label:
+                `str`
+            :param cmap:
+                *Dynamic spectrum plot only*.
+                Color map used to represent the data.
+                Default is ``'YlGnBu_r'``.
+            :type cmap:
+                `str`
 
-            :setter: Array of antenna positions.
+            :Example:
+                .. code-block:: python
 
-            :getter: Array of antenna positions.
+                    from nenupy.io.bst import BST
+                    from astropy.time import Time, TimeDelta
+                    import astropy.units as u
+                    import numpy as np
+
+                    # Select BST data
+                    bst = BST("/path/to/BST.fits")
+                    data = bst.get()
+                    
+                    # Prepare a boolean array to overlay a hatched pattern
+                    hatch_array = np.zeros((30, 300), dtype=bool)
+                    hatch_array[5:20, 100:200] = True
+                    # Specify time and frequency arrays
+                    time_dts = np.arange(300)*TimeDelta(1, format='sec')
+                    times = Time("2022-01-24T11:01:00") + time_dts
+                    frequencies = np.linspace(47, 52, 30)*u.MHz
+
+                    # Plot
+                    data.plot(
+                        hatched_overlay=(
+                            times,
+                            frequencies,
+                            hatch_array
+                        )
+                    )
 
-            :type: :class:`~numpy.ndarray`
         """
-        return self._antenna_positions
-    @antenna_positions.setter
-    def antenna_positions(self, p: np.ndarray):
-        self._antenna_positions = p
+        # Initialize the figure
+        if fig_ax is None:
+            fig = plt.figure(figsize=kwargs.get("figsize", (15, 7)))
+            ax = fig.add_subplot(111)
+        else:
+            fig, ax = fig_ax
 
+        data = self.value.T
+        if kwargs.get("decibel", True):
+            data = 10*np.log10(data)
+
+        if len(data.shape) == 2:
+            self._plot_dynamic_spectrum(data, ax, fig, **kwargs)
+        elif (len(data.shape) == 1) and (data.size == self.frequency.size):
+            self._plot_spectrum(data, ax, fig, **kwargs)
+        elif (len(data.shape) == 1) and (data.size == self.time.size):
+            self._plot_lightcurve(data, ax, fig, **kwargs)
+        else:
+            raise ValueError("Problem...")
 
-    @property
-    def antenna_gains(self) -> np.ndarray:
-        """ Antenna gains.
-            This is an array of `callable` (methods or functions)
-            defining the radiation pattern of each antenna.
+        # Axes limits
+        xmin, xmax = ax.get_xlim()
+        ymin, ymax = ax.get_ylim()
+        ax.set_xlim(kwargs.get("xmin", xmin), kwargs.get("xmax", xmax))
+        ax.set_ylim(kwargs.get("ymin", ymin), kwargs.get("ymax", ymax))
+
+        # Title
+        ax.set_title(kwargs.get("title", ""))
+
+        # Add minor ticks
+        ax.minorticks_on()
+
+        # Save or show the figure
+        figname = kwargs.get("figname", "")
+        if figname != "":
+            plt.savefig(
+                figname,
+                dpi=300,
+                bbox_inches="tight",
+                transparent=True
+            )
+            log.info(f"Figure '{figname}' saved.")
+        elif fig_ax is not None:
+            return
+        else:
+            plt.show()
+        plt.close("all")
+
+
+    def rebin(self, dt: u.Quantity = None, df: u.Quantity = None, method: str = "mean"):
+        """ Rebins the data in time and frequency.
+
+            :param dt:
+                Time bin widths.
+                Default is ``None`` (i.e., no rebin in time).
+            :type dt:
+                :class:`~astropy.units.Quantity`
+            :param df:
+                Frequency bin widths.
+                Default is ``None`` (i.e., no rebin in frequency).
+            :type df:
+                :class:`~astropy.units.Quantity`
+            :param method:
+                Type of method for rebin purpose (either ``'mean'`` or ``'median'``).
+                Default is ``'mean'``.
+            :type method:
+                `str`
+
+            :returns:
+                Rebinned data.
+            :rtype:
+                :class:`~nenupy.io.bst.ST_Slice`
+            
+            :Example:
+                .. code-block:: python
 
-            :setter: Array of antenna gains.
+                    from nenupy.io.bst import BST
+                    import astropy.units as u
 
-            :getter: Array of antenna gains.
+                    bst = BST("/path/to/BST.fits")
+                    data = bst.get()
+                    rebin_data = data.rebin(
+                        dt=3*u.s,
+                        df=2*u.MHz
+                    )
 
-            :type: :class:`~numpy.ndarray` of `callable`
         """
-        return self._antenna_gains
-    @antenna_gains.setter
-    def antenna_gains(self, g: np.ndarray):
-        self._antenna_gains = g
+        time = self.time.copy()
+        frequency = self.frequency.copy()
+        value = self.value.copy()
+
+        # Define the type of rebin
+        if method.lower() == "mean":
+            rebin_method = np.nanmean
+        elif method.lower() == "median":
+            rebin_method = np.nanmedian
+        else:
+            raise ValueError("`method` should either be 'mean' or 'median'.")
 
+        # Dynamic spectrum
+        if len(value.shape) == 2:
+            rebin_t_indices = self._rebin_time_indices(dt=dt)
+            if rebin_t_indices is not None:
+                value = rebin_method(
+                    value[rebin_t_indices, :],
+                    axis=1
+                )
+                time = Time(np.nanmean(time.jd[rebin_t_indices], axis=1), format='jd')
+            rebin_f_indices = self._rebin_frequency_indices(df=df)
+            if rebin_f_indices is not None:
+                value = rebin_method(
+                    value[:, rebin_f_indices],
+                    axis=2
+                )
+                frequency = np.nanmean(frequency[rebin_f_indices], axis=1)
+            value = value.squeeze()
 
-    @property
-    def position(self) -> EarthLocation:
-        """ Array's position.
+        # Spectrum
+        elif (len(value.shape) == 1) and (value.size == frequency.size):
+            rebin_indices = self._rebin_frequency_indices(df=df)
+            if rebin_indices is not None:
+                value = rebin_method(value[rebin_indices], axis=1)
+                frequency = np.nanmean(frequency[rebin_indices], axis=1)
+
+        # Light curve
+        elif (len(value.shape) == 1) and (value.size == time.size):
+            rebin_indices = self._rebin_time_indices(dt=dt)
+            if rebin_indices is not None:
+                value = rebin_method(value[rebin_indices], axis=1)
+                time = Time(np.nanmean(time.jd[rebin_indices], axis=1), format='jd')
+        else:
+            raise ValueError("Problem...")
+        
+        return ST_Slice(
+            time=time,
+            frequency=frequency,
+            value=value,
+            analog_pointing_times=self.analog_pointing_times,
+            digital_pointing_times=self.digital_pointing_times
+        )
+
+    # def rebin(array, x_step: int = None, y_step: int = None) -> np.ndarray:
+    #     """
+    #         array: 2D array dimensions=(x, y)
+    #         x_step: integer value such that x//x_step = 0 
+    #         y_step: integer value such that y//y_step = 0 
+    #     """
+
+    #     if x_step is not None:
+    #         x_size_final = array.shape[0]/x_step
+    #         if not x_size_final.is_integer():
+    #             raise ValueError(f'Array x dimension {array.shape[0]} is not divisible by {x_step}.')
+    #         if array.ndim == 2:
+    #             array = np.nanmean(
+    #                 array.reshape((int(x_size_final), x_step, array.shape[1])),
+    #                 axis=1
+    #             )
+    #         elif array.ndim == 1:
+    #             array = np.nanmean(
+    #                 array.reshape((int(x_size_final), x_step)),
+    #                 axis=1
+    #             )
+    #         else:
+    #             raise ValueError(f'Array dimension {array.ndim} is not supported.')
+
+    #     if y_step is not None:
+    #         if array.ndim != 2:
+    #             raise ValueError('Only 2D arrays.')
+    #         y_size_final = array.shape[1]/y_step
+    #         if not y_size_final.is_integer():
+    #             raise ValueError(f'Array y dimension {array.shape[1]} is not divisible by {y_step}.')
+    #         array = np.nanmean(
+    #             array.reshape((array.shape[0], int(y_size_final), y_step)),
+    #             axis=2
+    #         )
+
+    #     return array
+
+    # def rebin(array: np.ndarray, new_shape: tuple):
+    #     def get_compressor(old_dimension, new_dimension):
+    #         dim_compressor = np.zeros((new_dimension, old_dimension))
+    #         bin_size = float(old_dimension) / new_dimension
+    #         next_bin_break = bin_size
+    #         row_i = 0
+    #         column_i = 0
+    #         while row_i < dim_compressor.shape[0] and column_i < dim_compressor.shape[1]:
+    #             if round(next_bin_break - column_i, 10) >= 1:
+    #                 dim_compressor[row_i, column_i] = 1
+    #                 column_i += 1
+    #             elif next_bin_break == column_i:
+    #                 row_i += 1
+    #                 next_bin_break += bin_size
+    #             else:
+    #                 partial_credit = next_bin_break - column_i
+    #                 dim_compressor[row_i, column_i] = partial_credit
+    #                 row_i += 1
+    #                 dim_compressor[row_i, column_i] = 1 - partial_credit
+    #                 column_i += 1
+    #                 next_bin_break += bin_size
+    #         dim_compressor /= bin_size
+    #         return dim_compressor
+    #     row_compressor = get_compressor(array.shape[0], new_shape[0])
+    #     if array.ndim == 2:
+    #         column_compressor = get_compressor(array.shape[1], new_shape[1]).T
+    #         return np.matmul(np.matmul(row_compressor, array), column_compressor)
+    #     elif array.ndim == 1:
+    #         return np.matmul(row_compressor, array)
+    #     else:
+    #         raise ValueError('Only 1D or 2D arrays are allowed.')   
+
+    def clean_rfi(self, t_sigma: float = 1, f_sigma: float = 1):
+        """ """
+        cleaned_values = self.value.copy()
+        std = np.nanstd(cleaned_values)
+        frequency_median = np.nanmedian(cleaned_values, axis=0)
+        time_median = np.nanmedian(cleaned_values, axis=1)
+        cleaned_values[cleaned_values >= frequency_median[None, :] + std*f_sigma] = np.nan
+        cleaned_values[cleaned_values >= time_median[:, None] + std*t_sigma] = np.nan
+        return ST_Slice(
+            time=self.time,
+            frequency=self.frequency,
+            value=cleaned_values,
+            analog_pointing_times=self.analog_pointing_times,
+            digital_pointing_times=self.digital_pointing_times
+        )
 
-            :setter: Position of the array.
 
-            :getter: Position of the array.
+    def fit_transit(self, only_gaussian: bool = False, upper_threshold=None, **kwargs):
+        """ Do a fit.
 
-            :type: :class:`~astropy.coordinates.EarthLocation`
+            kwargs
+                filter_window (default (200))
         """
-        return self._position
-    @position.setter
-    def position(self, p: EarthLocation):
-        self._position = p
+        from scipy.optimize import curve_fit
 
+        def analog_switch_load(t, coeff_a=1., coeff_b=1.):
+            """
+                f(t) = a log_10(t) + b
+            """
+            return coeff_a*np.log10(t) + coeff_b
+
+        def gaussian(t, amp=1., mu=1., sig=1.):
+            return amp*np.exp(-np.power(t - mu, 2.) / (2*np.power(sig, 2.)))
+
+        def poly(t, c1=1.):#, c2=1.):#, c3):
+            return c1*t#, c1*np.power(t, 2.)# + c3
+
+        def combined(t, coeff_a, coeff_b, amp, mu, sig, c1):
+            return analog_switch_load(t, coeff_a, coeff_b) + gaussian(t, amp, mu, sig) + poly(c1)
+
+        data = self.value.copy()
+        x_data_to_fit = np.arange(data.size) + 1
+        if upper_threshold is not None:
+            data_mask = data < upper_threshold
+            data = data[data_mask]
+            x_data_to_fit = x_data_to_fit[data_mask]
+        else:
+            data_mask = np.ones(data.size, dtype=bool)
+        data[np.isnan(data)] = np.nanmedian(data)
 
-    # --------------------------------------------------------- #
-    # ------------------------ Methods ------------------------ #
-    def plot(self, **kwargs) -> None:
-        """ Plots the antenna distribution.
+        if only_gaussian:
+            filtered_data = ndimage.median_filter(
+                data,
+                size=kwargs.get("filter_window", (100))
+            )
+            max_data = filtered_data.max()
 
-            :param figsize:
-                Size of the figure. Default is ``(10, 10)``.
-            :type figsize:
-                `tuple`
-            :param figname:
-                File name of the figure to save. Default is ``''``,
-                i.e. show the figure without saving it.
-            :type figname:
-                `str`
-            :param xlim:
-                X-axis limits. Default is auto-scaling.
-            :type xlim:
-                `tuple`
-            :param ylim:
-                Y-axis limits. Default is auto-scaling.
-            :type ylim:
-                `tuple`
-        """
-        fig, ax = plt.subplots(
-            figsize=kwargs.get('figsize', (10, 10))
-        )
-        ax.scatter(
-            self.antenna_positions[:, 0],
-            self.antenna_positions[:, 1],
-            kwargs.get('s', 30)
-        )
-        ax.set_xlim(kwargs.get('xlim', ax.get_xlim()))
-        ax.set_ylim(kwargs.get('ylim', ax.get_ylim()))
-        for i, antenna_name in enumerate(self.antenna_names):
-            ax.annotate(
-                antenna_name,
-                (
-                    self.antenna_positions[i, 0],
-                    self.antenna_positions[i, 1]
-                ),
-                ha='center'
+            # Cut around the maximum (and only conserve the values around the peak)
+            # The maximum is computed over a median-smoothed version of the data to get rid of the RFIs.
+            mask = filtered_data >= max_data/2.
+            groups = np.split(np.arange(data.size), np.where(np.diff(mask) != 0)[0]+1)
+            max_in_group_mask = [np.argmax(filtered_data) in group for group in groups]
+            indices = groups[np.argwhere(max_in_group_mask)[0][0]]
+            data = data[indices]
+
+            data /= data.max()#max_data
+
+            popt, pcov = curve_fit(
+                gaussian,
+                x_data_to_fit,
+                data,
+                p0=[1, np.mean(x_data_to_fit), 10],
+                method="trf",
+                bounds=(
+                    [0.5,            0,          0.1],
+                    [1.2, x_data_to_fit.max(), x_data_to_fit.max()])
             )
-        ax.set_aspect('equal', adjustable='datalim')
 
-        if kwargs.get('figname', '') != '':
-            plt.savefig(
-                kwargs.get('figname'),
-                dpi=300,
-                transparent=True,
-                bbox_inches='tight'
+            x_data = np.arange(self.value.size) + 1
+            fitted_values = max_data*gaussian(x_data - indices[0], *popt)
+            interpolated_time_jd = np.interp(
+                popt[1] + indices[0],
+                x_data,
+                self.time.jd
             )
+
+            # Chi square
+            # stdev = np.std(data)
+            expected = gaussian(x_data_to_fit, *popt)
+            chi_square = np.sum(
+                (data - expected)**2/expected
+            )
+            # p value
+            # from scipy.stats import chi2, ttest_ind
+            # df = x_data_to_fit.size-1 # or dof of the gaussian? 
+            # chi2.sf(chi_2, df)
+
+
         else:
-            plt.show()
-        plt.close('all')
+            max_data = data.max()
+            data /= max_data
 
+            popt, pcov = curve_fit(
+                combined,
+                x_data_to_fit,
+                data,
+                p0=[1e-3, np.nanmin(data), 1., np.mean(x_data_to_fit), x_data_to_fit.max()/20, 0.],
+                method="trf",
+                bounds=( #coeff_a, coeff_b, amp, mu, sig, c1
+                    [1e-5,   0, 1e-3,            0,              x_data_to_fit.max()/35, -1e3],
+                    [1e3, np.nanmin(data), 1.5, x_data_to_fit.max(), x_data_to_fit.max()/20,  1e3])
+            )
 
-    def array_factor(self, sky: Sky, pointing: Pointing) -> da.Array:
-        r""" Computes the array factor of the antenna distribution.
+            fitted_values = max_data*combined(np.arange(self.time.size) + 1, *popt)
+            interpolated_time_jd = np.interp(popt[3], x_data_to_fit, self.time.jd[data_mask])
 
-            .. math::
-                \mathcal{F}(\nu, \phi, \theta) = \sum_{\rm ant} e^{ i \mathbf{k}(\nu, \phi, \theta) \cdot \mathbf{r}_{\rm ant}}
+            # Chi square
+            # Evaluate the chis2 on a reduce interval around the transit peak
+            peak_index = int(np.floor(popt[3]))
+            mask = fitted_values >= fitted_values[peak_index] - (fitted_values[peak_index]-max_data*popt[1])/2.
+            groups = np.split(np.arange(fitted_values.size), np.where(np.diff(mask) != 0)[0]+1)
+            peak_in_group_mask = [peak_index in group for group in groups]
+            indices = groups[np.argwhere(peak_in_group_mask)[0][0]]
+            
+            #chi_square = np.sum((self.value - fitted_values)**2/fitted_values)
+            # plt.plot(data[indices]*max_data, label="data")
+            # plt.plot(fitted_values[indices], label="fit")
+            # plt.legend()
+            # plt.show()
+            # stop
+            expected = combined(x_data_to_fit, *popt)
+            chi_square = np.sum(
+                (data[indices] - expected[indices])**2/expected[indices]
+            )
+            # chi_square = np.sum(
+            #     (self.value[indices] - fitted_values[indices])**2/fitted_values[indices]
+            # )
+            #degree_of_freedom = self.value.size - 6
 
-            where :math:`\mathbf{k} = \frac{2\pi}{\lambda} (\cos \phi \cos \theta, \sin \phi \cos \theta, \sin \theta )`
-            is the wave vector for a wave propagation in a direction described by spherical coordinates,
-            :math:`\lambda` is the wavelength, :math:`\phi` is the azimuth,
-            :math:`\theta` is the elevation, :math:`\mathbf{r}_{\rm ant}`
-            is the antenna position matrix.
-
-            This method considers the ``sky`` as the desired output (in terms of
-            time, frequency and sky positions). It evaluates the effective 
-            pointing directions for every time step defined in ``sky`` regarding
-            the ``pointing`` input.
-
-            :param sky:
-                Desired output contained in a :class:`~nenupy.astro.sky.Sky` instance.
-                (:attr:`~nenupy.astro.sky.Sky.time`, :attr:`~nenupy.astro.sky.Sky.frequency` and
-                :attr:`~nenupy.astro.sky.Sky.coordinates` are used as inputs for the computation).
-            :type sky:
-                :class:`~nenupy.astro.sky.Sky`
-            :param pointing:
-                Instance of :class:`~nenupy.astro.pointing.Pointing` that defines
-                the targeted pointing directions over the time.
-            :type pointing:
-                :class:`~nenupy.astro.pointing.Pointing`
+        # Compute the fitted transit time
+        transit_time = Time(interpolated_time_jd, format="jd")
 
-            :return:
-                Array factor of the antenna distribution shaped as ``(time, frequency, 1, coordinates)``.
-            :rtype:
-                :class:`~dask.array.Array`                
+        return ST_Slice(
+            time=self.time,
+            frequency=self.frequency,
+            value=fitted_values,
+            analog_pointing_times=self.analog_pointing_times,
+            digital_pointing_times=self.digital_pointing_times
+        ), transit_time, chi_square, popt
 
-            .. seealso::
-                :class:`~nenupy.astro.sky.Sky` and :class:`~nenupy.astro.pointing.Pointing`
-        """
 
-        # Determine the effective pointing based on the time
-        # informations contained in the sky instance.
-        effective_pointing = pointing[sky.time]
-
-        # Compute the geometric delays as the dot product of the
-        # antenna position and the difference between sky and
-        # pointing ground projections.
-        geometric_delays = self._geometric_delays(sky, effective_pointing)
-
-        # Use the sky frequency attribute to compute the wavelength
-        # and prepare the coefficient of the exponential with
-        # the correct dimensions.
-        wavelength = sky.frequency.to(u.m, equivalencies=u.spectral())
-        coeff = 2j * np.pi / wavelength.value
-        coeff = coeff.reshape(
-            (1, 1, wavelength.size, 1, 1)
-        ) # (antenna, time, frequency, polar, coord)
-    
-        exponent = coeff * geometric_delays
-        # coord_chunk = exponent.shape[-1]//cpu_count()
-        # coord_chunk = 1 if coord_chunk == 0 else coord_chunk
-        # exponent = da.rechunk(
-        #     exponent,
-        #     chunks=exponent.shape[:-1] + (coord_chunk,)
-        # )
-
-        complex_array_factor = np.sum(
-            np.exp(exponent),
-            axis=0
-        )
-        return (np.real(complex_array_factor * np.conjugate(complex_array_factor)))
-
-
-    def beam(self, sky: Sky, pointing: Pointing) -> Sky:
-        r""" Computes the phased-array response :math:`\mathcal{G}` over the ``sky`` for a given
-            ``pointing``.
-
-            .. math::
-                \mathcal{G}(\nu, \phi, \theta) = \sum_{\rm ant} \mathcal{F}(\nu, \phi, \theta) \mathcal{G}_{\rm ant} (\nu, \phi, \theta)
-
-            where :math:`\nu` is the frequency, :math:`\phi` is the azimuth,
-            :math:`\theta` is the elevation,
-            :math:`\mathcal{G}_{\rm ant}` is the individual array element radiation pattern and
-            :math:`\mathcal{F}` is the array factor.
-
-            This method considers the ``sky`` as the desired output (in terms of
-            time, frequency, polarization and sky positions). It evaluates the effective 
-            pointing directions for every time step defined in ``sky`` regarding
-            the ``pointing`` input.
-
-            :param sky:
-                Desired output contained in a :class:`~nenupy.astro.sky.Sky` instance.
-            :type sky:
-                :class:`~nenupy.astro.sky.Sky`
-            :param pointing:
-                Instance of :class:`~nenupy.astro.pointing.Pointing` that defines
-                the targeted pointing directions over the time.
-            :type pointing:
-                :class:`~nenupy.astro.pointing.Pointing`
-
-            :return:
-                The instance of :class:`~nenupy.astro.sky.Sky`
-                given as input is returned, its attribute
-                :attr:`~nenupy.astro.sky.Sky.value` is updated
-                with the result of the beam computation (stored as
-                an :class:`~dask.array.Array`) and shaped as 
-                ``(time, frequency, polarization, coordinates)``.
-            :rtype:
-                :class:`~nenupy.astro.sky.Sky`
+    def flatten_frequency(self):
+        """ """
+        return self/np.nanmedian(self.value, axis=0)[None, :]
 
-            .. seealso::
-                :meth:`~nenupy.instru.interferometer.Interferometer.array_factor`
 
-        """
+    def flatten_time(self):
+        """ """
+        return self/np.nanmedian(self.value, axis=1)[:, None]
 
-        # Compute the array factor
-        array_factor = self.array_factor(
-            sky=sky,
-            pointing=pointing
-        )
 
-        # Compute the total antenna gain, i.e. the sum of all
-        # antenna gains for beamforming.
-        antenna_gain = np.sum(
-            gain(
-                sky=sky,
-                pointing=pointing
-            ) for gain in self.antenna_gains
+    def median_filter(self,
+            filter_size=None
+        ):
+        """ """
+        if filter_size is None:
+            filter_size = tuple((np.array(self.value.shape)/10).astype(int).tolist())
+        return ST_Slice(
+            time=self.time,
+            frequency=self.frequency,
+            value=ndimage.median_filter(self.value, size=filter_size),
+            analog_pointing_times=self.analog_pointing_times,
+            digital_pointing_times=self.digital_pointing_times
         )
-        # antenna_gain = np.sum(
-        #     np.fromiter(
-        #         gain(
-        #             sky=sky,
-        #             pointing=pointing
-        #         ) for gain in self.antenna_gains
-        #     )
-        # )
 
-        # Rechunk the Dask Array before the computation
-        # coord_chunk = array_factor.shape[-1]//cpu_count()
-        # coord_chunk = 1 if coord_chunk == 0 else coord_chunk
-        # array_factor = array_factor.rechunk(array_factor.shape[:-1] + (coord_chunk,))
-
-        # Perform the Dask computation of array factor times antenna
-        # gains. Update the sky instance values.
-        sky.value = array_factor * antenna_gain
-
-        return sky
-
-
-    @lru_cache(maxsize=1)
-    @abstractmethod
-    def effective_area(self,
-            frequency: u.Quantity = 50*u.MHz,
-            elevation: u.Quantity = 90*u.deg
-        ) -> u.Quantity:
-        """ This method needs to be defined in child classes. """
-        return
 
+    def clear_pointing_switch(self,
+            flatten_frequency: bool = True,
+            pointing_dt: TimeDelta = TimeDelta(6*60, format="sec"),
+            peak_sample_error: int = 2,
+            return_correction: bool = False
+        ):
+        r"""
 
-    @abstractmethod
-    def instrument_temperature(self, frequency: u.Quantity = 50*u.MHz, **kwargs) -> u.Quantity:
-        """ This method needs to be defined in child classes. """
-        return
+        .. math::
+            p(t) = a \log(t) + bt^2 + ct + d
 
 
-    def system_temperature(self,
-            frequency: u.Quantity = 50*u.MHz,
-            source_spectrum: Dict[str, Callable] = {},
-            efficiency: float = 1.,
-            elevation: u.Quantity = 90*u.deg,
-            **kwargs
-        ) -> u.Quantity:
-        r""" Computes the System Noise Temperature :math:`T_{\rm sys}`.
-            It is computed as follows:
-
-            .. math::
-                T_{\rm sys} = T_{\rm sky} + T_{\rm inst} + \sum_{\rm src} T_{\rm src}
-
-            where :math:`T_{\rm sky}` is an approximation of the
-            low-frequency sky temperature dominated by Galactic
-            emission and :math:`T_{\rm inst}` is the instrumental
-            noise temperature (which depends on the current
-            instrument instance).
-            :math:`T_{\rm src}` is the antenna temperature induced by a given source
-            whose spectrum is defined in the ``source_spectrum`` argument computed as:
-
-            .. math::
-                T_{\rm src} = \frac{F_{\rm src} \eta A_{\rm eff}}{2 k_{\rm B}}
-            
-            where :math:`F_{\rm src}` is the source spectrum, :math:`\eta` is the
-            ``efficiency`` of the effective area :math:`A_{\rm eff}}`.
-
-            :param frequency: 
-                Frequency for the System Temperature computation.
-                Default is ``50 MHz``.
-            :type frequency:
-                :class:`~astropy.units.Quantity`
-            :param elevation:
-                Pointing elevation impacting the :meth:`~nenupy.instru.interferometer.Interferometer.effective_area`.
-                Default is ``90 deg``.
-            :type elevation:
-                :class:`~astropy.units.Quantity`
-            :param efficiency:
-                Effective area reducing factor. Default is ``1.``, it cannot be greater than ``1.``.
-            :type efficiency:
-                `float`
-            :param source_spectrum:
-                By default the system temperature is evaluated using a mean Galactic temperature.
-                However, if a bright source is targeted, the noise introduced can be under-estimated.
-                Therefore, one can provide a `callable` object that takes as inputs a frequency array (of type :class:`~astropy.units.Quantity`) and
-                returns the source flux density in Jansky (of type :class:`~astropy.units.Quantity`).
-            :type source_spectrum:
-                `dict` of `callable`
+        """
 
-            :returns:
-                System Temperature in Kelvins.
-            :rtype:
-                :class:`~astropy.units.Quantity`
+        # Prepare the data by computing the median time profile
+        if flatten_frequency:
+            # The median time profile is computed after the data have been flattened in frequency.
+            # This decreases fit domination by the most sensitive part of the spectrum.
+            median_frequency_profile = np.nanmedian(self.value, axis=0)
+            median_time_profile = np.nanmedian(self.value/median_frequency_profile[None, :], axis=1)
+        else:
+            # Keep the frequency responce while performing the median in time.
+            median_time_profile = np.nanmedian(self.value, axis=1)
+        time_profile_max = median_time_profile.max()
+        median_time_profile_normalized = median_time_profile/time_profile_max
+
+        # ------ Find fixed analog pointing time slots ------
+        # NenuFar analog pointing is applied once every `pointing_dt` (usually 6 min).
+        # Find the minimal distance, in sample unit, between two peaks.
+        data_dt_sec = (self.time[1] - self.time[0]).sec
+        pointing_dt_sec = pointing_dt.sec
+        pointing_dstance = int(np.round(pointing_dt_sec/data_dt_sec))
+        # The minimal distance is taken `peak_sample_error` samples short to give an error margin
+        minimal_sample_distance_between_peaks = pointing_dstance - peak_sample_error
+        # Find peaks over the gradient of the time profile
+        time_profile_gradient = np.gradient(median_time_profile_normalized)
+        peak_indices, _ = find_peaks(
+            -time_profile_gradient,
+            height=np.std(time_profile_gradient)*2,
+            distance=minimal_sample_distance_between_peaks
+        )
+        # The gradient shift the peak indices by -1
+        peak_indices += 1
+        # Add first and last indices if they have not been picked up
+        peak_indices = np.insert(peak_indices, 0, 0)
+        peak_indices = np.append(peak_indices, self.value.shape[0])
+        peak_indices = np.unique(peak_indices)
+
+        # ------ Fit each pointing interval ------
+        # Define the fitting function
+        @custom_model
+        def nenufar_switch_load(time, a=1., b=1., c=1., d=1.):
+            """ """
+            return a*np.log10(time) + b + c*time**2 + d*time
+        # Loop over each pointing slot to fit the function
+        switch_correction = np.ones(self.time.size)
+        for start_idx, stop_idx in zip(peak_indices[:-1], peak_indices[1:]):
+            # Select the time profile portion between two peaks
+            interval_profile = median_time_profile_normalized[start_idx:stop_idx]
+            # Perform the fitting
+            switch_model = nenufar_switch_load(1., interval_profile.min())
+            fitter = fitting.LevMarLSQFitter()
+            times = 1 + np.arange(interval_profile.size)
+            switch_model_fit = fitter(switch_model, times, interval_profile)
+            # Update the fit correction
+            switch_correction[start_idx:stop_idx] *= switch_model_fit(times)
+
+        # ------ Return the corrected data ------
+        new_st_slice = self/switch_correction[:, None]
+        if return_correction:
+            return new_st_slice, switch_correction
+        else:
+            return new_st_slice
 
-            .. seealso::
-                :func:`~nenupy.astro.astro_tools.sky_temperature`
 
+    # --------------------------------------------------------- #
+    # ----------------------- Internal ------------------------ #
+    def _overplot_pointings(self, ax, **kwargs):
+        """ Overplot vertical lines
         """
-        t_gal = sky_temperature(frequency)
-        t_inst = self.instrument_temperature(frequency, **kwargs)
-        t_src = np.zeros(frequency.shape)*u.K
-        for _, spectrum in source_spectrum.items():
-            src_flux = spectrum(frequency)
-            t_src += (src_flux*self.effective_area(frequency, elevation)*efficiency/(2*k_B)).to(u.K)
-        return (t_gal + t_inst + t_src).to(u.K)
-
-
-    def sefd(self,
-            frequency: u.Quantity = 50*u.MHz,
-            elevation: u.Quantity = 90*u.deg,
-            efficiency: float = 1.,
-            decoherence: float = 1.,
-            source_spectrum: Dict[str, Callable] = {},
-            **kwargs
-        ) -> u.Quantity:
-        r""" Computes the System Equivalent Flux Density (SEFD or
-            system sensitivity).
-            
-            .. math::
-                S_{\rm sys} = \xi \frac{2 k_{\rm B}}{ \eta A_{\rm eff}(\nu, \theta)} T_{\rm sys} (\nu)
-            
-            with :math:`T_{\rm sys}` the :meth:`~nenupy.instru.interferometer.Interferometer.system_temperature`,
-            the efficiency :math:`\eta`, :math:`\nu` the frequency, :math:`\theta` the elevation,
-            :math:`\xi` the decoherence factor, and :math:`k_{\rm B}` the
-            Boltzmann constant.
-
-            :param frequency:
-                Frequency at which the SEFD will be computed.
-                If an array is given as input, the output will be of same shape.
-                Default if ``50 MHz``.
-            :type frequency:
-                :class:`~astropy.units.Quantity`
-            :param elevation:
-                Pointing elevation impacting the :meth:`~nenupy.instru.interferometer.Interferometer.effective_area`.
-                Default is ``90 deg``.
-            :type elevation:
-                :class:`~astropy.units.Quantity`
-            :param efficiency:
-                Effective area reducing factor. Default is ``1.``, it cannot be greater than ``1.``.
-            :type efficiency:
-                `float`
-            :param decoherence:
-                Parameter that reflects other uncertainties (particularly the unperfect phasing system).
-                Default is ``1.``.
-            :type decoherence:
-                `float`
-            :param source_spectrum:
-                By default the system temperature is evaluated using a mean Galactic temperature.
-                However, if a bright source is targeted, the noise introduced can be under-estimated.
-                Therefore, one can provide a `callable` object that takes as inputs a frequency array (of type :class:`~astropy.units.Quantity`) and
-                returns the source flux density in Jansky (of type (as :class:`~astropy.units.Quantity`).
-            :type source_spectrum:
-                `dict` of `callable`
+        if kwargs.get("analog_pointing", False):
+            for time_i in self.analog_pointing_times:
+                ax.axvline(time_i.datetime, color="black", linestyle="-.", alpha=0.5)
+        if kwargs.get("digital_pointing", False):
+            for time_i in self.digital_pointing_times:
+                ax.axvline(time_i.datetime, color="black", linestyle=":", alpha=0.5)
 
-            :returns:
-                SEFD in Janskys.
-            :rtype:
-                :class:`~astropy.units.Quantity`
-        
-            .. seealso::
-                `LOFAR website <http://old.astron.nl/radio-observatory/astronomers/lofar-imaging-capabilities-sensitivity/sensitivity-lofar-array/sensiti>`_, :meth:`nenupy.instru.interferometer.Interferometer.system_temperature`
 
+    def _plot_spectrum(self, data, ax, fig, **kwargs):
+        """ Plots a spectrum.
         """
-        effective_area = self.effective_area(frequency, elevation)
-        t_sys = self.system_temperature(frequency, source_spectrum, **kwargs)
-        sefd = decoherence*2*k_B*t_sys/(efficiency*effective_area)
-        return sefd.to(u.Jy)
-
-
-    def sensitivity(self,
-            frequency: u.Quantity = 50*u.MHz,
-            mode: ObservingMode = ObservingMode.BEAMFORMING,
-            dt: u.Quantity = 1.*u.s,
-            df: u.Quantity = 195.3125*u.kHz,
-            elevation: u.Quantity = 90*u.deg,
-            efficiency: float = 1.,
-            decoherence: float = 1.,
-            source_spectrum: Dict[str, Callable] = {},
-            **kwargs
-        ) -> u.Quantity:
-        r""" Computes the sensititivy of the array with respect to the observing configuration.
-            The sensitivity computation depends on the observing mode of the instrument:
-
-            * for the imaging mode:
-
-                .. math::
-                    \sigma_{\rm im} = \frac{S_{\rm sys}(\nu, \theta, \eta, \xi)}{
-                        \sqrt{N(N-1) 2 \Delta \nu\, \Delta t}
-                    }
-
-            * for the beamforming mode:
-
-                .. math::
-                    \sigma_{\rm bf} = \frac{S_{\rm sys}(\nu, \theta, \eta, \xi)}{
-                        \sqrt{2 \Delta \nu\, \Delta t}
-                    }
-            
-            where :math:`\nu` is the frequency, :math:`\theta` is the elevation,
-            :math:`\eta` is the effective area efficiency,
-            :math:`\xi` is the decoherence factor,
-            :math:`\Delta t` is the integration time,
-            :math:`\Delta \nu` is the bandwidth, :math:`N` is the antenna number,
-            and :math:`S_{\rm sys}` is the System Equivalent Flux Density (which also depends
-            on the ``source_spectrum`` argument, see :meth:`~nenupy.instru.interferometer.Interferometer.sefd`).
-
-            :param frequency:
-                Frequency at which the sensitivity will be evaluated.
-                If an array is given as input, the output will be of same shape.
-                Default if ``50 MHz``.
-            :type frequency:
-                :class:`~astropy.units.Quantity`
-            :param mode:
-                Observing mode, either ``ObservingMode.BEAMFORMING`` or ``ObservingMode.IMAGING``, default is the former.
-            :type mode:
-                :class:`~nenupy.instru.interferometer.ObservingMode`
-            :param dt:
-                Integration time. Default is ``1 sec``.
-            :type dt:
-                :class:`~astropy.units.Quantity`
-            :param df:
-                Observing bandwidth. Default is ``195.3125 kHz``.
-            :type df:
-                :class:`~astropy.units.Quantity`
-            :param elevation:
-                Pointing elevation impacting the :meth:`~nenupy.instru.interferometer.Interferometer.effective_area`.
-                Default is ``90 deg``.
-            :type elevation:
-                :class:`~astropy.units.Quantity`
-            :param efficiency:
-                Effective area reducing factor. Default is ``1.``, it cannot be greater than ``1.``.
-            :type efficiency:
-                `float`
-            :param decoherence:
-                Parameter that reflects other uncertainties (particularly the unperfect phasing system).
-                Default is ``1.``.
-            :type decoherence:
-                `float`
-            :param source_spectrum:
-                By default the system temperature is evaluated using a mean Galactic temperature.
-                However, if a bright source is targeted, the noise introduced can be under-estimated.
-                Therefore, one can provide a `callable` object that takes as inputs a frequency array (of type :class:`~astropy.units.Quantity`) and
-                returns the source flux density in Jansky (of type :class:`~astropy.units.Quantity`).
-            :type source_spectrum:
-                `dict` of `callable`
+        ax.plot(
+            self.frequency.to(u.MHz).value,
+            data,
+            color=kwargs.get("color", None),
+            label=kwargs.get("label", None)
+        )
 
-            :return:
-                Array sensitivity.
-            :rtype:
-                :class:`~astropy.units.Quantity`
+        # X label
+        ax.set_xlabel("Frequency (MHz)")
 
-            :Example:
-                >>> from nenupy.instru.interferometer import ObservingMode
-                >>> import astropy.units as u
-                >>> <instrument>.sensitivity(
-                        frequency=50*u.MHz,
-                        mode=ObservingMode.IMAGING,
-                        dt=1*u.s,
-                        df=3*u.kHz
-                    )
+        # Y label
+        ax.set_ylabel("dB" if kwargs.get("decibel", True) else "Amp")
 
-            .. seealso::
-                :meth:`~nenupy.instru.interferometer.Interferometer.sefd` and :ref:`instrument_properties_doc`.
 
+    def _plot_lightcurve(self, data, ax, fig, **kwargs):
+        """ Plots a ligthcurve.
         """
-        s_sys = self.sefd(
-            frequency=frequency,
-            elevation=elevation,
-            decoherence=decoherence,
-            efficiency=efficiency,
-            source_spectrum=source_spectrum,
-            **kwargs
-        )
-        n_ant = self.antenna_names.size
-        if mode is ObservingMode.IMAGING:
-            sensitivity = s_sys/np.sqrt(n_ant*(n_ant - 1)*2*dt*df)
-        elif mode is ObservingMode.BEAMFORMING:
-            sensitivity = s_sys/np.sqrt(2*dt*df)
-        else:
-            raise ValueError(
-                'Invalid observation mode.'
-            )
-        return sensitivity.to(u.Jy)
-
-
-    def angular_resolution(self,
-            frequency: u.Quantity = 50*u.MHz
-        ) -> u.Quantity:
-        r""" Computes the angular resolution of the antenna array.
+        ax.plot(
+            self.time.datetime,
+            data,
+            label=kwargs.get("label", None),
+            color=kwargs.get("color", None)
+        )
 
-            The full width at half maximum (FWHM) :math:`\theta` is approximated as follows:
+        # Display pointings
+        self._overplot_pointings(ax, **kwargs)
+        
+        for vline in kwargs.get("vlines", []):
+            ax.axvline(vline, linestyle="--")
 
-            .. math::
-                \theta = \frac{\lambda}{D}
-            
-            where :math:`\lambda` is the wavelength and :math:`D` is
-            is the length of the maximum physical separation of the antennas
-            in the array.
+        # X label
+        ax.xaxis.set_major_formatter(
+            mdates.DateFormatter("%H:%M:%S")
+        )
+        fig.autofmt_xdate()
+        ax.set_xlabel(f"Time (UTC since {self.time[0].isot})")
 
-            :param frequency:
-                Frequency at which the angular resolution is evaluated.
-            :type frequency:
-                :class:`~astropy.units.Quantity`
-            
-            :return:
-                Angular resolution (FWHM) of the instrument.
-            :rtype:
-                :class:`~astropy.units.Quantity`
-            
-            :Example:
+        # Y label
+        ax.set_ylabel("dB" if kwargs.get("decibel", True) else "Amp")
 
-                >>> import astropy.units as u
-                >>> <instrument>.angular_resolution(
-                        frequency=50*u.MHz
-                    )
 
+    def _plot_dynamic_spectrum(self, data, ax, fig, **kwargs):
+        """ Plots a dynamic spectrum.
         """
-        if self.size == 1:
-            raise Exception(
-                "Angular resolution is not defined for an interferometer of 1 element."
-            )
-        wavelength = frequency.to(
-            u.m,
-            equivalencies=u.spectral()
-        )
-        diameter = np.max(self.baselines.distance)
-        return (wavelength / diameter * u.rad).to(u.deg)
-
-
-    def confusion_noise(self,
-            frequency: u.Quantity = 50*u.MHz,
-            lofar: bool = True
-        ) -> u.Quantity:
-        r""" Confusion rms noise :math:`\sigma_{\rm c}` (parameter
-            used for specifying the width of the confusion
-            distribution) computed as:
-
-            .. math::
-                \left( \frac{\sigma_{\rm c}}{\rm{mJy}\, \rm{beam}^{-1}} \right) \simeq
-                0.2 \left( \frac{\nu}{\rm GHz} \right)^{-0.7} 
-                \left( \frac{\theta}{\rm arcmin} \right)^{2}
-            
-            or (if ``lofar=True``):
-            
-            .. math::
-                \left( \frac{\sigma_{\rm c}}{\mu\rm{Jy}\, \rm{beam}^{-1}} \right) \simeq
-                30 \left( \frac{\nu}{74 {\rm MHz}} \right)^{-0.7} 
-                \left( \frac{\theta}{\rm arcsec} \right)^{1.54}
-            
-            where :math:`\nu` is the frequency and :math:`\theta` is
-            the radiotelescope FWHM (see :meth:`~nenupy.instru.interferometer.Interferometer.angular_resolution`).
-            
-            Individual sources fainter than about 
-            :math:`5\sigma_{\rm c}` cannot be detected reliably.
-
-            :param freq:
-                Frequency at which computing the confusion noise.
-                In MHz if no unit is provided. Default is ``50 MHz``.
-            :type freq: `float` or :class:`~astropy.units.Quantity`
-            :param miniarrays:
-                Mini-Array indices to take into account.
-                Default is ``None`` (all available MAs).
-            :type miniarrays: `int`, `list` or :class:`~numpy.ndarray`
-            :param lofar:
-                If set to ``True`` (recommended), the confusion noise
-                is estimated using Eq. 6 of `van Haarlem et al. (2013) <https://arxiv.org/pdf/1305.3550.pdf>`_.
-            :type:
-                `bool`
+        im = ax.pcolormesh(
+            self.time.datetime,
+            self.frequency.to(u.MHz).value,
+            data,
+            shading="auto",
+            cmap=kwargs.get("cmap", "YlGnBu_r"),
+            vmin=kwargs.get("vmin", np.nanpercentile(data, 5)),
+            vmax=kwargs.get("vmax", np.nanpercentile(data, 95))
+        )
 
-            :returns:
-                Confusion rms noise in Jy/beam
-            :rtype:
-                :class:`~astropy.units.Quantity`
+        # Display pointings
+        self._overplot_pointings(ax, **kwargs)
+            
+        for vline in kwargs.get("vlines", []):
+            ax.axvline(vline, linestyle="--")
 
-            :Example:
-                >>> import astropy.units as u
-                >>> <instrument>.confusion_noise(
-                        frequency=50*u.MHz
-                    )
+        if kwargs.get("hatched_overlay", None) is not None:
+            xlim = ax.get_xlim()
+            ylim = ax.get_ylim()
+            overlay_time, overlay_frequency, overlay_values = kwargs["hatched_overlay"]
+            ax.contourf(
+                overlay_time.datetime,
+                overlay_frequency.to(u.MHz).value,
+                overlay_values,
+                levels=[0, 1],
+                hatches=[None, '/'],
+                colors='none',
+                extend='both',
+            )
+            ax.set_xlim(xlim)
+            ax.set_ylim(ylim)
 
-            .. see also::
-                `NRAO lecture <https://www.cv.nrao.edu/course/astr534/Radiometers.html>`_ (eq. 3E6),
-                `Takeuchi and Ishii, 2004 <https://ui.adsabs.harvard.edu/abs/2004ApJ...604...40T/abstract>`_.
-        """
-        resolution = self.angular_resolution(frequency=frequency)
-        if lofar: # https://arxiv.org/pdf/1305.3550.pdf
-            freq_at_74mHz = (frequency.to(u.MHz)/(74*u.MHz)).value
-            res_in_asec = resolution.to(u.arcsec).value
-            conf = 30 * res_in_asec**1.54 * freq_at_74mHz**(-0.7) * u.uJy
-        else:
-            # freq_in_ghz = frequency.to(u.GHz).value
-            # res_in_asec = resolution.to(u.arcsec).value
-            # conf = 1.2 * (freq_in_ghz/3.02)**(-0.7) * (res_in_asec/8)**(10/3) * u.uJy # condon 2012
-            freq_in_ghz = frequency.to(u.GHz).value
-            res_in_amin = resolution.to(u.arcmin).value
-            conf = 0.2 * freq_in_ghz**(-0.7) * res_in_amin**2 * u.mJy # Condon 2002
+        cax = inset_axes(
+            ax,
+            width='3%',
+            height='100%',
+            loc='lower left',
+            bbox_to_anchor=(1.03, 0., 1, 1),
+            bbox_transform=ax.transAxes,
+            borderpad=0,
+        )
+        cbar = plt.colorbar(im, cax=cax)
+        # cbar = plt.colorbar(im, pad=0.03)
+        cbar.set_label(kwargs.get("colorbar_label", "dB" if kwargs.get("decibel", True) else "Amp"))
+
+        # X label
+        ax.xaxis.set_major_formatter(
+            mdates.DateFormatter("%H:%M:%S")
+        )
+        fig.autofmt_xdate()
+        ax.set_xlabel(f"Time (UTC since {self.time[0].isot})")
 
-        return conf.to(u.Jy) # Jy/beam
+        # Y label
+        ax.set_ylabel(f"Frequency (MHz)")
 
 
-    # --------------------------------------------------------- #
-    # ----------------------- Internal ------------------------ #
-    def _geometric_delays(self, sky: Sky, pointing: Pointing) -> da.Array:
-        """ Computes the geometric delays between the sky and the pointing direction(s).
+    def _rebin_frequency_indices(self, df: u.Quantity) -> np.ndarray:
+        """ Get the indices of self.value to rebin in frequencies.
         """
-        sky_projection = sky.ground_projection
-        pointing_projection = pointing.ground_projection
+        # Check that there is an even distribution of frequencies
+        if df is None:
+            return None
+        elif not np.unique(np.diff(self.frequency)).size == 1:
+            log.error(
+                "Impossible to rebin, the frequency range is not uniformly distributed."
+            )
+            raise Exception()
+        df_mhz = df.to(u.MHz).value
+        data_df = self.frequency[1] - self.frequency[0]
+        data_df_mhz = data_df.to(u.MHz).value
+        n_bins = int(np.floor(df_mhz/data_df_mhz))
+        if n_bins > self.frequency.size:
+            n_bins = self.frequency.size
+        elif n_bins == 0:
+            log.warning(
+                f"No frequency rebin applied, {df.to(u.MHz)} <= {data_df.to(u.MHz)}."
+            )
+            return None
+        return np.arange(n_bins)[None, :] + n_bins*np.arange(self.frequency.size//n_bins)[:, None]
 
-        # coord_chunk = sky_projection.shape[-1]//cpu_count()
-        # coord_chunk = 1 if coord_chunk == 0 else coord_chunk
-        # chunk_shape = sky_projection.shape[:-1] + (coord_chunk,)
-        chunk_shape = (1, 1, 1, 3,) + (sky_projection.shape[-1],)
-
-        sky_projection = da.from_array(
-            sky_projection,
-            chunks=chunk_shape
-        )
-        pointing_projection = da.from_array(
-            pointing_projection,
-            chunks=chunk_shape
-        )
-
-        # Put the ground antennas in the sky
-        angle = np.pi/2
-        rot_90 = np.array(
-            [
-                [np.cos(angle), -np.sin(angle), 0],
-                [np.sin(angle), np.cos(angle), 0],
-                [0,           0,           1]
-            ]
-        )
-
-        return np.dot(
-            np.dot(self.antenna_positions, rot_90),
-            sky_projection - pointing_projection
+
+    def _rebin_time_indices(self, dt: u.Quantity = None) -> np.ndarray:
+        """ Get the indices of self.value to rebin in times.
+        """
+        # TO DO IN DASK but not optimized yet...
+        # import dask.array as da
+        # arr = da.from_array(np.arange(100))
+        # nbins = 9
+        # bins = da.from_array(np.arange(nbins))[None, :] + da.from_array(nbins*np.arange(arr.size//nbins))[:, None]
+        # arr.vindex[bins].compute()
+        if dt is None:
+            return None
+        obs_dt = (self.time[1] - self.time[0]).sec * u.s
+        n_bins = int(
+            np.floor(
+                (dt/obs_dt).to(u.dimensionless_unscaled).value
+            )
         )
+        if n_bins > self.time.size:
+            n_bins = self.time.size
+        elif n_bins == 0:
+            log.warning(
+                f"No time rebin applied, {dt.to(u.s)} <= {obs_dt.to(u.s)}."
+            )
+            return None
+        return np.arange(n_bins)[None, :] + n_bins*np.arange(self.time.size//n_bins)[:, None]
+
+
+    def _operation_with_other(self, other, operation: Callable):
+        """ """
+        if type(other) is type(self):
+            # If `other` is a ST_Slice
+
+            # Check if they have the same frequency and time axes
+            same_frequency_size = self.frequency.size == other.frequency.size
+            same_time_size = self.time.size == other.time.size
+            if (not same_frequency_size) or (not same_time_size):
+                raise InconsistentShapeError
+
+            # Check if they have the same frequency and time axes
+            same_frequencies = np.all(self.frequency == other.frequency)
+            same_times = np.all(self.time == other.time)
+            if (not same_frequencies) or (not same_times):
+                raise InconsistentShapeError
+            
+            # Find out if any of the instances have their pointings filled up
+            analog_pointings = [self.analog_pointing_times, other.analog_pointing_times]
+            digital_pointings = [self.digital_pointing_times, other.digital_pointing_times]
+            analog_id_max = np.argmax(list(map(len, analog_pointings)))
+            digital_id_max = np.argmax(list(map(len, digital_pointings)))
+    
+            # Return a new object, while performing a numpy operation
+            return ST_Slice(
+                time=self.time,
+                frequency=self.frequency,
+                value=operation(self.value, other.value),
+                analog_pointing_times=analog_pointings[analog_id_max],
+                digital_pointing_times=digital_pointings[digital_id_max]
+            )
+        else:
+            # Perform a normal numpy operation
+            return ST_Slice(
+                time=self.time,
+                frequency=self.frequency,
+                value=operation(self.value, other),
+                analog_pointing_times=self.analog_pointing_times,
+                digital_pointing_times=self.digital_pointing_times
+            )
+    
+    @staticmethod
+    def _smooth_data(x, window_length=150, sigma_clip=1.5, iterations=2):
+        data = x.copy()
+        if window_length > data.size:
+            raise IndexError(
+                f"window_length: {window_length} > data size: {data.size}."
+            )
+        while iterations != 0:
+            window_indices = np.arange(window_length)
+            slide_indices = np.arange(data.size - window_length + 1)
+            sliding_window_indices = window_indices[None, :] + slide_indices[:, None]
+            windows_stds = np.nanstd(data[sliding_window_indices], axis=1)
+            windows_medians = np.nanmedian(data[sliding_window_indices], axis=1)
+            thresholds = windows_medians + sigma_clip*windows_stds
+            problems_indices = data[sliding_window_indices] >= thresholds[:, None]
+
+            index_problems = np.unique(sliding_window_indices[problems_indices])
+            for pb_idx in index_problems:
+                sliding_windows_affected = np.any(
+                    np.isin(sliding_window_indices, pb_idx),
+                    axis=1
+                )
+                data[pb_idx] = np.median(windows_medians[sliding_windows_affected])
+
+            iterations -= 1
+            window_length = int(window_length//2)
+        
+        return data
 # ============================================================= #
 # ============================================================= #
+
```

### Comparing `nenupy-2.1.0/nenupy/instru/low_noise_amplifier.json` & `nenupy-2.2.9/nenupy/instru/low_noise_amplifier.json`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/instru/miniarray_antennas.json` & `nenupy-2.2.9/nenupy/instru/miniarray_antennas.json`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/instru/nenufar.py` & `nenupy-2.2.9/nenupy/instru/nenufar.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,41 +64,46 @@
 from enum import Enum
 
 
 class _AntennaGain:
     """ NenuFAR antenna gain class. """
 
 
-    def __init__(self, polarization='NW'):
+    def __init__(self, polarization: str = 'NW'):
         self.polarization = polarization
 
-        if self.polarization == 'NW':
+        if self.polarization == 'NE':#'NW':
             fields = np.arange(8)
-        elif self.polarization == 'NE':
+        elif self.polarization == 'NW':#'NE':
             fields = 8 + np.arange(8)
+        else:
+            raise Exception(f"Polarization '{self.polarization}' unknown.")
 
         # Read the gain
         gain = hp.read_map(
             filename=os.path.join(os.path.dirname(__file__), './NenuFAR_Ant_Hpx.fits'),
             hdu=1,
             field=fields,
             memmap=True,
             dtype=float
         )
+        gain /= gain.max()
 
         # Interpolate the antenna gain on the frequency axis
         freqs = np.arange(10, 90, 10)
         self.healpix_coords = np.arange(hp.pixelfunc.nside2npix(64))
         self.interpolated_gain = interp2d(
             x=self.healpix_coords,
             y=freqs,
             z=gain,
             kind='linear'
         )
 
+        log.info(f'NenuFAR antenna model (polarization={polarization}) loaded.')
+
 
     @lru_cache(maxsize=1)
     def __getitem__(self, sky: Sky) -> np.ndarray:
         """ Return an antenna gain array shaped like (sky.time, sky.frequency, sky.coord)
         """
 
         horizontal_coordinates = sky.horizontal_coordinates
@@ -165,14 +170,52 @@
             )
         self._beamsquint_frequency = freq
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
+# ------------------ MiniArray class errors ------------------- #
+# ============================================================= #
+class MiniArrayUnknownIndex(Exception):
+    """ Error raised when the index doesn't exist. """
+
+    def __init__(self,
+            input_index: int
+        ):
+        self.input_index = input_index
+        self.error_message = f"Mini-Array index {self.input_index} does not exist..."
+        available_mini_arrays = [entry["id"] for entry in nenufar_miniarrays.values()]
+        self.help = f"Valid Mini-Array indices are: {available_mini_arrays}."
+        super().__init__(self.help)
+
+
+    def __str__(self):
+        return f"{self.error_message}\n{self.help}"
+
+
+class MiniArrayBadIndexFormat(Exception):
+    """ Error raised when the index cannot be read. """
+
+    def __init__(self,
+            input_index
+        ):
+        self.input_index = input_index
+        self.error_message = f"No support for {type(self.input_index)} format as a Mini-Array index..."
+        self.help = f"The index should be an integer value."
+        super().__init__(self.help)
+
+
+    def __str__(self):
+        return f"{self.error_message}\n{self.help}"
+# ============================================================= #
+# ============================================================= #
+
+
+# ============================================================= #
 # ------------------------- MiniArray ------------------------- #
 # ============================================================= #
 class MiniArray(Interferometer):
     """ Main class to handle a NenuFAR Mini-Array antenna distribution.
 
         .. versionadded:: 2.0.0
 
@@ -232,17 +275,16 @@
 
         .. autosummary::
 
             ~MiniArray.beam
             ~MiniArray.effective_area
             ~MiniArray.instrument_temperature
             ~MiniArray.attenuation_from_zenith
-            ~MiniArray.order_to_skycoord
-            ~MiniArray.skycoord_to_order
             ~MiniArray.analog_pointing
+            ~MiniArray.beamsquint_correction
             ~nenupy.instru.interferometer.Interferometer.plot
             ~nenupy.instru.interferometer.Interferometer.array_factor
             ~nenupy.instru.interferometer.Interferometer.system_temperature
             ~nenupy.instru.interferometer.Interferometer.sefd
             ~nenupy.instru.interferometer.Interferometer.sensitivity
             ~nenupy.instru.interferometer.Interferometer.angular_resolution
             ~nenupy.instru.interferometer.Interferometer.confusion_noise
@@ -250,26 +292,33 @@
         .. rubric:: Attributes and Methods Documentation
 
     """
 
     def __init__(self, index: int = 0):
         self.index = index
 
-        ma_name = f'MA{self.index:03d}'
+        try:
+            ma_name = f'MA{self.index:03d}'
+
+            position = EarthLocation(
+                lat=nenufar_miniarrays[ma_name]['lat'] * u.deg,
+                lon=nenufar_miniarrays[ma_name]['lon'] * u.deg,
+                height=nenufar_miniarrays[ma_name]['height'] * u.m
+            )
+        except KeyError:
+            raise MiniArrayUnknownIndex(self.index)
+        except:
+            raise MiniArrayBadIndexFormat(self.index)
 
-        position = EarthLocation(
-            lat=nenufar_miniarrays[ma_name]['lat'] * u.deg,
-            lon=nenufar_miniarrays[ma_name]['lon'] * u.deg,
-            height=nenufar_miniarrays[ma_name]['height'] * u.m
-        )
         antenna_names = np.array([ant for ant in miniarray_antennas.keys()])
         antPos = np.array([ant['position'] for ant in miniarray_antennas.values()])
         self.rotation = nenufar_miniarrays[ma_name]['rotation'] * u.deg
-        #rotation = np.radians(self.rotation.value - 90)
-        rotation = np.radians(self.rotation.value)
+        #rotation = np.radians(self.rotation.value + 180)
+        rotation = np.radians(360-self.rotation.value)
+        #rotation = np.radians(self.rotation.value)
         rotMatrix = np.array(
             [
                 [np.cos(rotation), -np.sin(rotation), 0],
                 [-np.sin(rotation), -np.cos(rotation), 0],
                 [0,           0,           1]
             ]
         )
@@ -335,15 +384,16 @@
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
     def beam(self,
             sky: Sky,
             pointing: Pointing,
-            configuration: NenuFAR_Configuration = NenuFAR_Configuration()
+            configuration: NenuFAR_Configuration = NenuFAR_Configuration(),
+            return_complex: bool = False
         ) -> Sky:
         r""" Computes the Mini-Array beam over the ``sky`` for a given
             ``pointing``.
 
             .. math::
                 \mathcal{G}_{\rm MA}(\nu, \phi, \theta) = \mathcal{F}_{\rm MA}(\nu, \phi, \theta) \mathcal{G}_{\rm ant} (\nu, \phi, \theta)
 
@@ -455,15 +505,16 @@
         # Computing the Mini-Array effective area.
         # aeff = self.effective_area(sky.frequency).to(u.m**2).value
 
         # The beam is computed thanks to the Interferometer super method.
         # The returned value is only divided by Aeff.
         return super().beam(
             sky=sky,
-            pointing=self.analog_pointing(pointing, configuration=configuration)
+            pointing=self.analog_pointing(pointing, configuration=configuration),
+            return_complex=return_complex
         )# / aeff[None, :, None, None]
 
 
     def effective_area(self,
             frequency: u.Quantity = 50*u.MHz,
             elevation: u.Quantity = 90*u.deg
         ) -> u.Quantity:
@@ -693,14 +744,17 @@
                 `int`
 
             :returns:
                 Instrument temperature in Kelvins
             :rtype:
                 :class:`~astropy.units.Quantity`
 
+            .. warning::
+                For the time being, only ``lna_filter`` values ``0`` and ``3`` are available.
+
             :Example:
 
                 >>> from nenupy.instru import MiniArray
                 >>> import astropy.units as u
                 >>> ma = MiniArray()
                 >>> ma.instrument_temperature(frequency=70*u.MHz)
                 526.11213 K
@@ -767,30 +821,30 @@
         )
         azimuths = coords.az
         elevations = coords.alt
         elevations = np.interp(elevations.deg, squint_table['elev_desiree'][freq_idx, :], squint_table['elev_a_pointer'])
         # Squint is limited at 20 deg elevation, otherwise the
         # pointing can vary drasticaly as the available pointing
         # positions become sparse at low elevation.
-        elevations[elevations < 20] = 20
+        # elevations[elevations < 20] = 20
 
         return SkyCoord(
             azimuths,
             elevations * u.deg,
             frame=coords.frame
         )
 
 
     def analog_pointing(self, pointing: Pointing, configuration: NenuFAR_Configuration) -> Pointing:
         """ Converts the desired pointing to the effective pointing
             which depends on the available pointing positions defined
             on a grid due to analog cable delays.
         """
         # Put the horizontal coordinates in a good shape
-        pointing_ho_coords = pointing.horizontal_coordinates
+        pointing_ho_coords = pointing.horizontal_coordinates # TODO try to copy instead of using a pointer which modifies the top object
         if pointing_ho_coords.isscalar:
             pointing_ho_coords = pointing_ho_coords.reshape((1,))
 
         # Correct the pointing for beamsquint effect, that is, point at a
         # lower elevation than the one desired
         if configuration.beamsquint_correction:
             pointing_ho_coords = self.beamsquint_correction(
@@ -837,15 +891,14 @@
         for i, pol in enumerate(sky.polarization):
             if not isinstance(pol, Polarization):
                 log.warning(
                     f"Invalid value encountered in <attr 'Sky.polarization'>: '{pol}'. "
                     f"Polarization has been set to '{Polarization.NW}' by default."
                 )
                 pol = Polarization.NW
-            t0 = Time.now()
             gain[:, :, i, :] = pol.value[sky]
         return gain
 
 
     def _toITRF(self):
         """
         """
@@ -1025,29 +1078,43 @@
         """
         return f"{self.__class__.__name__}"
 
 
     # --------------------------------------------------------- #
     # --------------------- Getter/Setter --------------------- #
     @property
-    def miniarray_rotations(self):
+    def miniarray_rotations(self) -> u.Quantity:
         """
         """
         return np.array([
             nenufar_miniarrays[ma]['rotation'] for ma in self.antenna_names
-        ])
+        ])*u.deg
+    
+
+    @property
+    def include_remote_mas(self) -> bool:
+        """ """
+        return self._include_remote_mas
+    @include_remote_mas.setter
+    def include_remote_mas(self, include):
+        if not isinstance(include, bool):
+            raise TypeError(
+                "`include_remote_mas` - Boolean value expected."
+            )
+        self._include_remote_mas = include
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
     def beam(self,
             sky: Sky,
             pointing: Pointing,
             analog_pointing: Pointing = None,
-            configuration: NenuFAR_Configuration = NenuFAR_Configuration()
+            configuration: NenuFAR_Configuration = NenuFAR_Configuration(),
+            return_complex: bool = False
         ) -> Sky:
         r""" Computes the NenuFAR beam over the ``sky`` for a given
             ``pointing``.
 
             .. math::
                 \mathcal{G}_{\rm NenuFAR}(\nu, \phi, \theta) = \mathcal{F}_{\rm NenuFAR} (\nu, \phi, \theta) \sum_{\rm MA} \mathcal{G}_{\rm MA}(\nu, \phi, \theta)
 
@@ -1113,37 +1180,42 @@
             log.info(
                 "Analog pointing is set according to the numerical pointing."
             )
 
         # Computing the Array Factor of the whole NenuFAR array.
         array_factor = self.array_factor(
             sky=sky,
-            pointing=pointing
+            pointing=pointing,
+            return_complex=return_complex
         )
 
         # Finding the unique Mini-Array rotations and the number
         # of MAs corresponding to each rotation.
         rots, indices, counts = np.unique(
-            self.miniarray_rotations%60,
+            self.miniarray_rotations.to(u.deg).value%60,
             return_counts=True,
             return_index=True
         )
 
         # Summing all different (due to rotation) Mini-Array beam
         # patterns, although only executing it at most 6 times
         # because there could only be 6 different rotations.
         # Even though antGain updates the same sky instance, the
         # value attr * count creates new memeory allocations.
         antenna_gain = np.sum(
-            gain(
-                sky=sky,
-                pointing=analog_pointing,
-                configuration=configuration
-            ).value*count for gain, count in zip(self.antenna_gains[indices], counts)
-        )
+            np.array([
+                gain(
+                    sky=sky,
+                    pointing=analog_pointing,
+                    configuration=configuration,
+                    return_complex=return_complex
+                ).value*count for gain, count in zip(self.antenna_gains[indices], counts)
+            ]),
+            axis=0
+        )/np.sum(counts) # TODO check that this is correct to normalize
 
         # Updating the sky object value array where the the sky
         # is above the horizon as the product of the NenuFAR array
         # factor and the combined Mini-Array gain patterns.
         sky.value = array_factor * antenna_gain
 
         return sky
```

### Comparing `nenupy-2.1.0/nenupy/instru/nenufar_array.json` & `nenupy-2.2.9/nenupy/instru/nenufar_array.json`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/instru/squint_table.sav` & `nenupy-2.2.9/nenupy/instru/squint_table.sav`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/instru_old/cal_pz_2_multi_2019-02-23.dat` & `nenupy-2.2.9/nenupy/instru/cal_pz_2_multi_2019-02-23.dat`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/instru_old/instru.py` & `nenupy-2.2.9/nenupy/undysputed/dynspec.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,1364 +1,1782 @@
 #! /usr/bin/python3
 # -*- coding: utf-8 -*-
 
 
-"""
-    ********************
-    Instrument functions
-    ********************
+r"""
+    *******
+    Dynspec
+    *******
+
+    :mod:`~nenupy.undysputed.Dynspec` is the module designed to
+    read and analyze *UnDySPuTeD* DynSpec high-rate data. It
+    benefits from `Dask <https://docs.dask.org/en/latest/>`_, with
+    the possibility of reading and applying complex pipelines
+    to larger-than-memory data sets.
+    It replaces the original `nenupy-tf <https://github.com/AlanLoh/nenupy-tf>`_
+    module.
+
+    .. note::
+        `nenupy` logger could be activated at will to enhance the verbosity:
+
+        >>> import logging
+        >>> logging.getLogger('nenupy').setLevel(logging.INFO)
+
+    UnDySPuTeD receiver
+    -------------------
+
+    *UnDySPuTeD* (stands for Unified Dynamic Spectrum Pulsar and
+    Time Domain receiver) is the receiver of the NenuFAR
+    beamformer mode, fed by the (up-to-)96 core Mini-Arrays (2
+    polarizations) from the *LANewBa* backend. 
+
+    DynSpec data
+    ------------
+
+    The raw data flow from *LANewBa* consists of 195312.5 pairs
+    of complex X and Y values per second per beamlet. These data
+    are downsampled in channels per subband (of 195.3125 kHz)
+    numbered from 16 to 2048 channels, ``fftlen``, (to achieve a
+    frequency resolution of :math:`\delta \nu = 12 - 0.1\, \rm{kHz}`
+    respectively). After computation of cross and auto-correlations,
+    the data are downsampled again in time, integrating from 4 to 1024
+    spectra, ``nfft2int`` (implying a time resolution :math:`195312.5^{-1} \times \rm{fftlen} \times \rm{fft2int}`,
+    :math:`\delta t = 0.3 - 83.9\, \rm{ms}`).
+
+    .. seealso::
+        `DynSpec data product <https://nenufar.obs-nancay.fr/en/astronomer/#data-products>`_
+
+    DynSpec data files
+    ------------------
+
+    Each NenuFAR/*UnDySPuTeD*/DynSpec observation results in the
+    production of several proprietary formatted files (``'*.spectra'``),
+    each corresponding to an individual lane of the *UnDySPuTeD* receiver.
+    Depending on the observation configuration, the bandwidth and/or
+    the different observed beams (i.e., beamforming in different sky
+    directions) can be spread accross these files.
+
+    The class :class:`~nenupy.undysputed.dynspec.Dynspec` offers
+    the possibility to read and analyze all these observation files
+    at once, through an API aimed at minimizing user interaction
+    over complicated settings.
+    
+    For the purpose of the following 'how-to' guide, a 1h-observation
+    of the famous pulsar `PSR B1919+21 <https://en.wikipedia.org/wiki/PSR_B1919%2B21>`_
+    is analyzed. :mod:`~nenupy.undysputed.dynspec.Dynspec` needs
+    first to be imported, as well as :mod:`~astropy.units` in order
+    to use physcial units (to avoid mistakes).
+    Attribute :attr:`~nenupy.undysputed.dynspec.Dynspec.lanefiles`
+    is filled with a `list` of all the available lane files (up to four)
+    in order to create ``ds``, an instance of
+    :class:`~nenupy.undysputed.dynspec.Dynspec`:
+
+    >>> from nenupy.undysputed import Dynspec
+    >>> import astropy.units as u
+    >>> ds = Dynspec(
+            lanefiles=[
+                'B1919+21_TRACKING_20200214_090835_0.spectra',
+                'B1919+21_TRACKING_20200214_090835_1.spectra'
+            ]
+        )
+    
+    .. note::
+        :attr:`~nenupy.undysputed.dynspec.Dynspec.lanefiles` must contain
+        files related to one specific observation (otherwise, a ``ValueError``
+        is raised). It can be practical to automatically find all
+        *DynSpec* files if they are stored within an observation folder:
+
+        >>> from glob import glob
+        >>> from os.path import join
+        >>> obs_path = '/path/to/observation'
+        >>> dynspec_files = glob(
+                join(obs_path, '*.spectra')
+            )
+
+        and then filling in :attr:`~nenupy.undysputed.dynspec.Dynspec.lanefiles`
+        with ``dynspec_files``.
+    
+    Observation properties
+    ----------------------
+    
+    Once the two *DynSpec* files 'lazy'-read/loaded (i.e., without
+    being directly stored in memory), and before any data
+    selection to occur, it might be handy to check the data
+    properties.
+    Several getter attributes of :class:`~nenupy.undysputed.dynspec.Dynspec`
+    allow for taking an overall look at the data.
+
+    Time
+    ^^^^
+
+    :attr:`~nenupy.undysputed.dynspec.Dynspec.tmin` and
+    :attr:`~nenupy.undysputed.dynspec.Dynspec.tmax` both return
+    :class:`~astropy.time.Time` object instances and give the
+    start and stop times of the observation (time can thus be
+    expressed in ISOT format, for example, simply by querying the
+    ``.isot`` attribute of the :class:`~astropy.time.Time`
+    instance):
+
+    >>> ds.tmin.isot
+    '2020-02-14T09:08:55.0000000'
+    >>> ds.tmax.isot
+    '2020-02-14T10:07:54.9506330'
+
+    Native time resolution of the data can also be accessed
+    as a :class:`~astropy.units.Quantity` instance by querying
+    the :attr:`~nenupy.undysputed.dynspec.Dynspec.dt` attribute 
+    (wich can then be converted to any desired equivalent
+    unit):  
+    
+    >>> ds.dt
+    0.04194304 s
+    >>> ds.dt.to(u.ms)
+    41.94304 ms
+
+    Frequency
+    ^^^^^^^^^
+
+    :attr:`~nenupy.undysputed.dynspec.Dynspec.fmin` and
+    :attr:`~nenupy.undysputed.dynspec.Dynspec.fmax` are the
+    minimal and maximal recorded frequencies, independently of
+    the beam selection.
+
+    >>> ds.fmin
+    11.816406 MHz
+    >>> ds.fmax
+    83.691406 MHz
+    
+    Native frequency resolution 
+    :attr:`~nenupy.undysputed.dynspec.Dynspec.df` is also an
+    instance of :class:`~astropy.units.Quantity` and can thus
+    be converted to any matching unit:
+
+    >>> ds.df
+    12207.031 Hz
+    >>> ds.df.to(u.MHz)
+    0.012207031 MHz
+
+    Beam
+    ^^^^
+    
+    Depending on the observation configuration, several beams may
+    be spread accross lane files. There could be as many beams as
+    available beamlet (i.e. 768 if the full 150 MHz bandwidth is
+    used, see `NenuFAR receivers <https://nenufar.obs-nancay.fr/en/astronomer/#receivers>`_).
+    They are recorded by their indices and summarized within the
+    :attr:`~nenupy.undysputed.dynspec.Dynspec.beams` atribute:
 
-    Below are defined a set of useful NenuFAR instrumental
-    functions, hereafter summarized:
+    >>> ds.beams
+    array([0])
     
-    * :func:`~nenupy.instru.instru.analog_pointing`: NenuFAR real analog pointing conversion
-    * :func:`~nenupy.instru.instru.desquint_elevation`: Correct for beamsquint
-    * :func:`~nenupy.instru.instru.nenufar_ant_gain`: NenuFAR antenna gain in HEALPix
-    * :func:`~nenupy.instru.instru.read_cal_table`: Read the antenna delay calibration table
-    * :func:`~nenupy.instru.instru.effective_area`: NenuFAR effective area
-    * :func:`~nenupy.instru.instru.sky_temperature`: Compute sky temperature at a given frequency
-    * :func:`~nenupy.instru.instru.inst_temperature`: NenuFAR temperature
-    * :func:`~nenupy.instru.instru.sefd`: NenuFAR SEFD
-    * :func:`~nenupy.instru.instru.sensitivity`: NenuFAR sensitivity
-    * :func:`~nenupy.instru.instru.resolution`: NenuFAR resolution
-    * :func:`~nenupy.instru.instru.confusion_noise`: NenuFAR confusion noise
-    * :func:`~nenupy.instru.instru.data_rate`: NenuFAR data rate estimation
-    * :func:`~nenupy.instru.instru.freq2sb`: Conversion from frequency to sub-band index
-    * :func:`~nenupy.instru.instru.sb2freq`: Conversion sub-band index to sub-band start frequency
-    * :func:`~nenupy.instru.instru.lnaGain`: Low Noise Amplifier gain
+    to help selecting available beam indices. On the current example,
+    only one beam has been recorded, hence the single index ``0``.
 
+    Data selection
+    --------------
+
+    >>> ds.time_range = [
+            '2020-02-14T09:08:55.0000000',
+            '2020-02-14T09:30:30.9506330'
+        ]
+    >>> ds.freq_range = [
+            10*u.MHz,
+            90*u.MHz
+        ]
+    >>> ds.beam = 0
+
+    Pipeline setup
+    --------------
+
+    Before getting the data, several processes may be set up and
+    therefore being used for converting raw data ('L0') to cleaned
+    and reduced data ('L1').
+    
+    Bandpass correction
+    ^^^^^^^^^^^^^^^^^^^
+
+    Reconstructed sub-bands may not display a flat bandpass due
+    to polyphase filter response. It may be usefull to correct
+    for this effect and reduce dynamic spectrum artefacts.
+    Several types of correction are implemented and can be set
+    with the :attr:`~nenupy.undysputed.dynspec.Dynspec.bp_correction`
+    attribute (see :attr:`~nenupy.undysputed.dynspec.Dynspec.bp_correction`
+    for more information regarding each correction efficiency).
+    
+    >>> ds.bp_correction = 'standard'
+
+    Pointing jump correction
+    ^^^^^^^^^^^^^^^^^^^^^^^^
+    
+    Instrumental components used during analogical Mini-Array
+    introduction of antenna delays for pointing purposes may
+    induce < 1dB gain jumps. To ease correction of this effect,
+    analogical pointing orders are set to occur every 6 minutes.
+
+    A correction of these 6-minute jumps is implemented within
+    :mod:`~nenupy.undysputed.dynspec` and only requires the
+    boolean setting of the :attr:`~nenupy.undysputed.dynspec.Dynspec.jump_correction`
+    attribute:
+
+    >>> ds.jump_correction = True
+
+    The jumps are fitted with a function of the form:
+    
+    .. math::
+        f(t) = a \log_{10} (t) + b
+
+    .. image:: ./_images/jumps.png
+        :width: 800
+
+    Dedispersion
+    ^^^^^^^^^^^^
+    
+    `Pulsar <https://en.wikipedia.org/wiki/Pulsar>`_ or 
+    `Fast Radio Burst <https://en.wikipedia.org/wiki/Fast_radio_burst>`_
+    studies may require de-dispersion of the signal before averaging
+    and/or summing over the frequency axis.
+
+    A `Dispersion Measure <https://astronomy.swin.edu.au/cosmos/P/Pulsar+Dispersion+Measure>`_
+    value other than ``None`` input to the
+    :attr:`~nenupy.undysputed.dynspec.Dynspec.dispersion_measure` attribute
+    triggers the de-dispersion process of the dynamic spectrum by
+    correcting the data for frequency-dependent pulse delay
+    (see :func:`~nenupy.astro.astro.dispersion_delay`).
+
+    >>> ds.dispersion_measure = 12.4 * u.pc / (u.cm**3)
+
+    .. warning::
+        Dedispersion cannot benefit from `Dask <https://docs.dask.org/en/latest/>`_
+        computing performances by construction (it would require
+        smart n-dimensional array indexing which is not currently
+        a Dask feature).
+        Therefore, depending on data native sampling in time and
+        frequency, a too large selection may lead to memory error.
+        Users are encouraged to ask for smaller data chunks and
+        combine them afterward.
+    
+    Averaging
+    ^^^^^^^^^
+
+    Averaging data might be quite useful in order to handle them
+    in an easier way by reducing their size. Data can be averaged
+    in time (with a :math:`\Delta t` given as input to the
+    :attr:`~nenupy.undysputed.dynspec.Dynspec.rebin_dt` attribute)
+    or in frequency (with a :math:`\Delta \nu` given as input to the
+    :attr:`~nenupy.undysputed.dynspec.Dynspec.rebin_df` attribute):
+
+    >>> ds.rebin_dt = 0.2 * u.s
+    >>> ds.rebin_df = 195.3125 * u.kHz
+
+    Either of these attribute can be set to ``None``, in which case
+    the data are not averaged on the corresponding dimension. 
+
+    Result examples
+    ---------------
+
+    Raw data averaged
+    ^^^^^^^^^^^^^^^^^
+    
+    The first example follows exactly the previous steps,
+    although, aiming for raw data visulaization, the gain jump
+    correction and the de-dispersion processes are deactivated.
+    Stokes I data are averaged and returned thanks to the
+    :meth:`~nenupy.undysputed.dynspec.Dynspec.get` method and
+    stored in the ``result`` variable, which is a
+    :class:`~nenupy.beamlet.sdata.SData` instance.
+    The dynamic spectrum is displayed with `matplotlib` after
+    subtraction by a median background to enhance the features.
+    
+    .. code-block:: python
+        :emphasize-lines: 12,13
+        
+        >>> from nenupy.undysputed import Dynspec
+        >>> import astropy.units as u
+        >>> import matplotlib.pyplot as plt
+
+        >>> ds = Dynspec(lanefiles=dysnpec_files)
+
+        >>> ds.time_range = ['2020-02-14T09:08:55.0000000', '2020-02-14T09:30:30.9506330']
+        >>> ds.freq_range = [10*u.MHz, 90*u.MHz]
+        >>> ds.beam = 0
+
+        >>> ds.bp_correction = 'standard'
+        >>> ds.jump_correction = False
+        >>> ds.dispersion_measure = None
+        >>> ds.rebin_dt = 0.2 * u.s
+        >>> ds.rebin_df = 195.3125 * u.kHz
+        
+        >>> result = ds.get(stokes='i')
+
+        >>> background = np.nanmedian(result.amp, axis=0)
+        >>> plt.pcolormesh(
+                result.time.datetime,
+                result.freq.to(u.MHz).value,
+                result.amp.T - background[:, np.newaxis],
+            )
+
+    .. image:: ./_images/psrb1919_nojump.png
+        :width: 800
+    
+    Gain jump correction
+    ^^^^^^^^^^^^^^^^^^^^
+
+    The previous example three significant 6-min jumps. They can
+    simply be corrected by setting :attr:`~nenupy.undysputed.dynspec.Dynspec.jump_correction`
+    to ``True``:
+    
+    .. code-block:: python
+        :emphasize-lines: 12
+        
+        >>> from nenupy.undysputed import Dynspec
+        >>> import astropy.units as u
+        >>> import matplotlib.pyplot as plt
+
+        >>> ds = Dynspec(lanefiles=dysnpec_files)
+
+        >>> ds.time_range = ['2020-02-14T09:08:55.0000000', '2020-02-14T09:30:30.9506330']
+        >>> ds.freq_range = [10*u.MHz, 90*u.MHz]
+        >>> ds.beam = 0
+
+        >>> ds.bp_correction = 'standard'
+        >>> ds.jump_correction = True
+        >>> ds.dispersion_measure = None
+        >>> ds.rebin_dt = 0.2 * u.s
+        >>> ds.rebin_df = 195.3125 * u.kHz
+        
+        >>> result = ds.get(stokes='i')
+
+        >>> background = np.nanmedian(result.amp, axis=0)
+        >>> plt.pcolormesh(
+                result.time.datetime,
+                result.freq.to(u.MHz).value,
+                result.amp.T - background[:, np.newaxis],
+            )
+
+    .. image:: ./_images/psrb1919.png
+        :width: 800
+
+    De-dispersion
+    ^^^^^^^^^^^^^
+
+    Finally, as these are `PSR B1919+21 <https://en.wikipedia.org/wiki/PSR_B1919%2B21>`_
+    data, with a known dispersion measure of
+    :math:`\mathcal{D}\mathcal{M} = 12.4\, \rm{pc}\,\rm{cm}^{-3}`,
+    they can be de-dispersed by setting
+    :attr:`~nenupy.undysputed.dynspec.Dynspec.dispersion_measure`
+    to the pulsar's value:
+
+    .. code-block:: python
+        :emphasize-lines: 13
+
+        >>> from nenupy.undysputed import Dynspec
+        >>> import astropy.units as u
+        >>> import matplotlib.pyplot as plt
+
+        >>> ds = Dynspec(lanefiles=dysnpec_files)
+
+        >>> ds.time_range = ['2020-02-14T09:08:55.0000000', '2020-02-14T09:30:30.9506330']
+        >>> ds.freq_range = [10*u.MHz, 90*u.MHz]
+        >>> ds.beam = 0
+
+        >>> ds.bp_correction = 'standard'
+        >>> ds.jump_correction = False
+        >>> ds.dispersion_measure = 12.4 *u.pc / (u.cm**3)
+        >>> ds.rebin_dt = 0.2 * u.s
+        >>> ds.rebin_df = 195.3125 * u.kHz
+        
+        >>> result = ds.get(stokes='i')
+
+        >>> background = np.nanmedian(result.amp, axis=0)
+        >>> plt.pcolormesh(
+                result.time.datetime,
+                result.freq.to(u.MHz).value,
+                result.amp.T - background[:, np.newaxis],
+            )
+
+    .. image:: ./_images/psrb1919_dedispersed.png
+        :width: 800
+
+    The dynamic spectrum is now de-dispersed with two visible effects:
+
+    * The pulsar's pulses are now visible as vertical lines,
+    * The 'right-hand' part of the spectrum contains `~numpy.nan` values as data were shifted to compensate for the dispersion delay. 
+
+    Dynspec class
+    -------------
 """
 
 
 __author__ = 'Alan Loh'
 __copyright__ = 'Copyright 2020, nenupy'
 __credits__ = ['Alan Loh']
 __maintainer__ = 'Alan'
 __email__ = 'alan.loh@obspm.fr'
 __status__ = 'Production'
 __all__ = [
-    'ma_antpos',
-    'ma_info',
-    'ma_pos',
-    '_HiddenPrints',
-    'getMAL93',
-    'nenufar_loc',
-    'analog_pointing',
-    'desquint_elevation',
-    'nenufar_ant_gain',
-    'read_cal_table',
-    'effective_area',
-    'sky_temperature',
-    'inst_temperature',
-    'sefd',
-    'sensitivity',
-    'resolution',
-    'confusion_noise',
-    'data_rate',
-    'freq2sb',
-    'sb2freq',
-    'lnaGain'
+    '_Lane',
+    'Dynspec'
 ]
 
 
-from astropy.io.fits import getdata
-from astropy.units import Quantity
-from astropy.time import Time
-from astropy.coordinates import (
-    ICRS,
-    AltAz,
-    EarthLocation
-)
-import astropy.units as u
-from astropy import constants as const
+from os.path import isfile, abspath, join, dirname, basename
 import numpy as np
-import os, sys
-from os.path import join, dirname
-from scipy.io.idl import readsav
-from scipy.interpolate import interp1d
+import astropy.units as u
+from astropy.time import Time
+from astropy.modeling import models, fitting
+from astropy.modeling.models import custom_model
+import dask.array as da
+from dask.diagnostics import ProgressBar
+
+from nenupy.beamlet import SData
+from nenupy.astro import dispersion_delay
 
 import logging
 log = logging.getLogger(__name__)
+#log.setLevel(logging.INFO)
 
 
 # ============================================================= #
-# ------------------------- ma_antpos ------------------------- #
+# --------------------------- Lane ---------------------------- #
 # ============================================================= #
-def ma_antpos(rot):
-    """ MiniArray rotation in degrees
+class _Lane(object):
+    """
     """
-    nenufar_antpos = np.array(
-        [
-            -5.50000000e+00, -9.52627850e+00,  0.00000000e+00,
-             0.00000000e+00, -9.52627850e+00,  0.00000000e+00,
-             5.50000000e+00, -9.52627850e+00,  0.00000000e+00,
-            -8.25000000e+00, -4.76313877e+00,  0.00000000e+00,
-            -2.75000000e+00, -4.76313877e+00,  0.00000000e+00,
-             2.75000000e+00, -4.76313877e+00,  0.00000000e+00,
-             8.25000000e+00, -4.76313877e+00,  0.00000000e+00,
-            -1.10000000e+01,  9.53674316e-07,  0.00000000e+00,
-            -5.50000000e+00,  9.53674316e-07,  0.00000000e+00,
-             0.00000000e+00,  9.53674316e-07,  0.00000000e+00,
-             5.50000000e+00,  9.53674316e-07,  0.00000000e+00,
-             1.10000000e+01,  9.53674316e-07,  0.00000000e+00,
-            -8.25000000e+00,  4.76314068e+00,  0.00000000e+00,
-            -2.75000000e+00,  4.76314068e+00,  0.00000000e+00,
-             2.75000000e+00,  4.76314068e+00,  0.00000000e+00,
-             8.25000000e+00,  4.76314068e+00,  0.00000000e+00,
-            -5.50000000e+00,  9.52628040e+00,  0.00000000e+00,
-             0.00000000e+00,  9.52628040e+00,  0.00000000e+00,
-             5.50000000e+00,  9.52628040e+00,  0.00000000e+00
-        ]
-    ).reshape(19, 3)
-    rot = np.radians(rot - 90)
-    rotation = np.array(
-        [
-            [ np.cos(rot), np.sin(rot), 0],
-            [-np.sin(rot), np.cos(rot), 0],
-            [ 0,           0,           1]
-        ]
-    )
-    return np.dot(nenufar_antpos, rotation)
-# ============================================================= #
 
+    def __init__(self, lanefile):
+        self.lane_index = None
+        self.data = None
+        self.dt = None
+        self.df = None
+        self.fft0 = None
+        self.fft1 = None
+        self.beam_arr = None
+        self.chan = None
+        # self.unix = None
+        self.lanefile = lanefile
+
+
+    # --------------------------------------------------------- #
+    # --------------------- Getter/Setter --------------------- #
+    @property
+    def lanefile(self):
+        """
+        """
+        return self._lanefile
+    @lanefile.setter
+    def lanefile(self, l):
+        l = abspath(l)
+        if not isfile(l):
+            raise FileNotFoundError(
+                f'{l} not found.'
+            )
+        if not l.endswith('spectra'):
+            raise ValueError(
+                'Wrong file type, expected *.spectra'
+            )
+        self._lanefile = l
+        self._load()
+        return
+
+
+    @property
+    def data(self):
+        return self._data
+    @data.setter
+    def data(self, d):
+        if d is None:
+            self._data = d
+            return
+
+
+    @property
+    def subband_width(self):
+        """
+            Should be equal to 0.1953125 MHz
+        """
+        return self.df * self.fftlen
+
+
+    @property
+    def tmin(self):
+        """
+        """
+        return Time(self._times[0], format='unix', precision=7)
+
+
+    @property
+    def tmax(self):
+        """
+        """
+        return Time(self._times[-1], format='unix', precision=7)
+
+
+    @property
+    def fmin(self):
+        """
+        """
+        half_sb = self.subband_width/2
+        channels = self.chan[0, :] # Assumed all identical!
+        return np.min(channels).compute()*self.subband_width - half_sb
+
+
+    @property
+    def fmax(self):
+        """
+        """
+        half_sb = self.subband_width/2
+        channels = self.chan[0, :] # Assumed all identical!
+        return np.max(channels).compute()*self.subband_width + half_sb
+    
 
-# ============================================================= #
-# -------------------------- ma_info -------------------------- #
-# ============================================================= #
-ma_info = np.array(
-    [
-        (0 , 0  , np.array([6.39113316e+05, 6.69766347e+06, 1.81735000e+02]), 440.5 , 29.5),
-        (1 , 30 , np.array([6.39094578e+05, 6.69764471e+06, 1.81750000e+02]), 364   , 30  ),
-        (2 , 300, np.array([6.39069472e+05, 6.69763443e+06, 1.81761000e+02]), 150   , 31  ),
-        (3 , 200, np.array([6.39038120e+05, 6.69761975e+06, 1.81757000e+02]), 145.5 , 31  ),
-        (4 , 20 , np.array([6.39020122e+05, 6.69759892e+06, 1.81762000e+02]), 464.5 , 28.5),
-        (5 , 180, np.array([6.39062298e+05, 6.69765911e+06, 1.81671000e+02]), 384.5 , 30  ),
-        (6 , 180, np.array([6.39039218e+05, 6.69764638e+06, 1.81718000e+02]), 276.5 , 31  ),
-        (7 , 230, np.array([6.38985155e+05, 6.69762795e+06, 1.81620000e+02]), 471   , 28.5),
-        (8 , 150, np.array([6.39002711e+05, 6.69764788e+06, 1.81677000e+02]), 411.5 , 29.5),
-        (9 , 240, np.array([6.39006567e+05, 6.69767471e+06, 1.81737000e+02]), 428.5 , 29.5),
-        (10, 290, np.array([6.39033717e+05, 6.69769736e+06, 1.81762000e+02]), 496   , 28.5),
-        (11, 310, np.array([6.39040955e+05, 6.69772821e+06, 1.81813000e+02]), 663   , 27.5),
-        (12, 250, np.array([6.39061482e+05, 6.69770986e+06, 1.81727000e+02]), 659.5 , 25  ),
-        (13, 40 , np.array([6.39081586e+05, 6.69774800e+06, 1.81997000e+02]), 958   , 24.5),
-        (14, 330, np.array([6.39099636e+05, 6.69778020e+06, 1.82152000e+02]), 1032  , 24.5),
-        (15, 280, np.array([6.39098493e+05, 6.69772636e+06, 1.81912000e+02]), 793   , 26.5),
-        (16, 60 , np.array([6.39128375e+05, 6.69774506e+06, 1.82005000e+02]), 1054.5, 24  ),
-        (17, 110, np.array([6.39153064e+05, 6.69776096e+06, 1.82062000e+02]), 1233  , 23  ),
-        (18, 10 , np.array([6.39201475e+05, 6.69776774e+06, 1.82083000e+02]), 1355  , 22  ),
-        (19, 210, np.array([6.39146673e+05, 6.69779044e+06, 1.82199000e+02]), 1249.5, 22.5),
-        (20, 320, np.array([6.39191912e+05, 6.69780784e+06, 1.82057000e+02]), 1352.5, 21.5),
-        (21, 260, np.array([6.39158373e+05, 6.69784497e+06, 1.82201000e+02]), 1461  , 21.5),
-        (22, 250, np.array([6.39007359e+05, 6.69773473e+06, 1.81967000e+02]), 662   , 27.5),
-        (23, 170, np.array([6.38994637e+05, 6.69778006e+06, 1.82016000e+02]), 969.5 , 25  ),
-        (24, 180, np.array([6.38974900e+05, 6.69779771e+06, 1.82057000e+02]), 1082.5, 24.5),
-        (25, 50 , np.array([6.39039664e+05, 6.69779603e+06, 1.82092000e+02]), 1052  , 23.5),
-        (26, 300, np.array([6.39051439e+05, 6.69782833e+06, 1.82133000e+02]), 1112  , 23.5),
-        (27, 210, np.array([6.39037314e+05, 6.69786239e+06, 1.82535000e+02]), 1387  , 21  ),
-        (28, 320, np.array([6.39106516e+05, 6.69788052e+06, 1.82416000e+02]), 1527.5, 20.5),
-        (29, 330, np.array([6.39085345e+05, 6.69782694e+06, 1.82164000e+02]), 1226  , 22  ),
-        (30, 60 , np.array([6.39124407e+05, 6.69781362e+06, 1.82277000e+02]), 1530.5, 20.5),
-        (31, 20 , np.array([6.39118449e+05, 6.69784678e+06, 1.82334000e+02]), 1462  , 21  ),
-        (32, 290, np.array([6.38980493e+05, 6.69766162e+06, 1.81773000e+02]), 573   , 28  ),
-        (33, 240, np.array([6.38955067e+05, 6.69765390e+06, 1.81787000e+02]), 616.5 , 27.5),
-        (34, 230, np.array([6.38917110e+05, 6.69764246e+06, 1.81723000e+02]), 770.5 , 26  ),
-        (35, 340, np.array([6.38901511e+05, 6.69766562e+06, 1.81722000e+02]), 1024  , 24.5),
-        (36, 170, np.array([6.38842551e+05, 6.69768422e+06, 1.81915000e+02]), 1182.5, 23  ),
-        (37, 350, np.array([6.38881893e+05, 6.69770613e+06, 1.81971000e+02]), 1231  , 23  ),
-        (38, 260, np.array([6.38828310e+05, 6.69773150e+06, 1.82165000e+02]), 1365  , 21.5),
-        (39, 160, np.array([6.38798998e+05, 6.69767696e+06, 1.82180000e+02]), 1472  , 21  ),
-        (40, 220, np.array([6.38828026e+05, 6.69764418e+06, 1.82034000e+02]), 1115.5, 24  ),
-        (41, 120, np.array([6.38994603e+05, 6.69769938e+06, 1.81819000e+02]), 661.5 , 26.5),
-        (42, 140, np.array([6.38973994e+05, 6.69773127e+06, 1.81940000e+02]), 802.5 , 25.5),
-        (43, 130, np.array([6.38963888e+05, 6.69775682e+06, 1.82315000e+02]), 932   , 24.5),
-        (44, 110, np.array([6.38907143e+05, 6.69775707e+06, 1.82406000e+02]), 1187  , 23  ),
-        (45, 150, np.array([6.38934310e+05, 6.69776276e+06, 1.82306000e+02]), 1030  , 23.5),
-        (46, 300, np.array([6.38947300e+05, 6.69779542e+06, 1.82257000e+02]), 1096  , 23.5),
-        (47, 190, np.array([6.38957218e+05, 6.69768346e+06, 1.81905000e+02]), 721.5 , 26.5),
-        (48, 100, np.array([6.38932724e+05, 6.69769106e+06, 1.81967000e+02]), 898   , 26  ),
-        (49, 340, np.array([6.38924357e+05, 6.69772908e+06, 1.82312000e+02]), 1029  , 23.5),
-        (50, 160, np.array([6.38865831e+05, 6.69778298e+06, 1.82415000e+02]), 1339.5, 23  ),
-        (51, 240, np.array([6.38881847e+05, 6.69776009e+06, 1.82376000e+02]), 1138.5, 23.5),
-        (52, 270, np.array([6.39169242e+05, 6.69769247e+06, 1.82180000e+02]), 1014,   23.5),
-        (53, 340, np.array([6.39199806e+05, 6.69768286e+06, 1.82226000e+02]), 1014,   23.5),
-        (54, 310, np.array([6.39223589e+05, 6.69770809e+06, 1.82158000e+02]), 1106,   23.5),
-        (55, 90,  np.array([6.39216821e+05, 6.69765166e+06, 1.82178000e+02]), 1106,   23.5),
-        (56, 10 , np.array([639166.449,  6697659.027, 182.023]), 0, 0),
-        (57, 350 , np.array([639215.343,  6697624.231, 182.616]), 0, 0),
-        (58, 50 , np.array([639212.511,  6697596.767, 182.589]), 0, 0),
-        (59, 270 , np.array([639172.087,  6697554.41 , 182.618]), 0, 0),
-        (60, 310 , np.array([639195.287,  6697539.278, 182.613]), 0, 0),
-        (61, 220 , np.array([639149.311,  6697537.968, 182.608]), 0, 0),
-        (62, 40 , np.array([639213.407,  6697485.116, 182.655]), 0, 0),
-        (63, 80 , np.array([639199.459,  6697454.733, 182.642]), 0, 0),
-        (64, 140 , np.array([638925.579,  6697597.428, 181.486]), 0, 0),
-        (65, 200 , np.array([638863.841,  6697563.347, 181.296]), 0, 0),
-        (66, 190 , np.array([638821.425,  6697535.168, 181.236]), 0, 0),
-        (67, 60 , np.array([638970.031,  6697540.574, 181.772]), 0, 0),
-        (68, 50 , np.array([638951.341,  6697490.638, 181.764]), 0, 0),
-        (69, 170 , np.array([638902.989,  6697486.95 , 181.178]), 0, 0),
-        (70, 70 , np.array([638924.864,  6697452.932, 181.232]), 0, 0),
-        (71, 0 , np.array([638987.56 ,  6697461.71 , 181.782]), 0, 0),
-        (72, 90 , np.array([638997.129,  6697545.429, 181.801]), 0, 0),
-        (73, 140 , np.array([639004.298,  6697518.733, 181.772]), 0, 0),
-        (74, 350 , np.array([639081.531,  6697491.281, 182.587]), 0, 0),
-        (75, 120 , np.array([639042.344,  6697460.205, 181.792]), 0, 0),
-        (76, 30 , np.array([639120.224,  6697452.406, 182.605]), 0, 0),
-        (77, 190 , np.array([639046.268,  6697413.41 , 181.881]), 0, 0),
-        (78, 270 , np.array([639114.382,  6697512.751, 182.602]), 0, 0),
-        (79, 40 , np.array([639158.051,  6697404.906, 182.415]), 0, 0),
-    ],
-    np.dtype(
-        [
-            ('ma', int),
-            ('rot', float),
-            ('pos', np.ndarray),
-            ('delay', float),
-            ('att', float),
+    # --------------------------------------------------------- #
+    # ------------------------ Methods ------------------------ #
+    def get_stokes(self, stokes='I'):
+        """ fft0[..., :] = [XX, YY]
+            fft1[..., :] = [Re(XY*), Im(XY*)]
+            XX=I+Q YY=I-Q XY=U+iV YX=U-iV
+        """
+        stokes_data = {
+            'i': np.sum(self.fft0, axis=4),
+            'q': self.fft0[..., 0] - self.fft0[..., 1],
+            'u': self.fft1[..., 0] * 2,
+            'v': - self.fft1[..., 1] * 2,
+            'l': np.sqrt((self.fft0[..., 0] - self.fft0[..., 1])**2 + (self.fft1[..., 0] * 2)**2),
+            'xx': self.fft0[..., 0],
+            'yy': self.fft0[..., 1]
+        }
+        try:
+            selected_stokes = stokes_data[stokes.lower()]
+        except KeyError:
+            log.error(
+                f'Available Stokes: {stokes_data.keys()}'
+            )
+            raise
+        selected_stokes = self._to2d(selected_stokes)
+        # selected_stokes = self._bp_correct(
+        #     data=selected_stokes,
+        #     method=bpcorr
+        # )
+        return selected_stokes
+
+
+    # --------------------------------------------------------- #
+    # ----------------------- Internal ------------------------ #
+    def _load(self):
+        """
+        """
+        # Lane index just before '.spectra', warning: hardcoded!
+        self.lane_index = self._lanefile[-9]
+        # Header structure to decode it:
+        header_struct = [
+            ('idx', 'uint64'),
+            ('TIMESTAMP', 'uint64'),
+            ('BLOCKSEQNUMBER', 'uint64'),
+            ('fftlen', 'int32'),
+            ('nfft2int', 'int32'),
+            ('fftovlp', 'int32'),
+            ('apodisation', 'int32'),
+            ('nffte', 'int32'),
+            ('nbchan', 'int32')
         ]
-    )
-)
-# ============================================================= #
-
+        with open(self._lanefile, 'rb') as rf:
+            header_dtype = np.dtype(header_struct)
+            header = np.frombuffer(
+                rf.read(header_dtype.itemsize),
+                count=1,
+                dtype=header_dtype,
+            )[0]
+        # Storing metadata
+        for key in [h[0] for h in header_struct]:
+            setattr(self, key.lower(), header[key])
+        self.dt = 5.12e-6 * self.fftlen * self.nfft2int * u.s
+        self.block_dt = self.dt * self.nffte
+        self.df = (1.0 / 5.12e-6 / self.fftlen) * u.Hz
+        log.debug(
+            f'Header of {self._lanefile} correctly parsed.'
+        )
+        # Read data
+        beamlet_dtype = np.dtype([
+            ('lane', 'int32'),
+            ('beam', 'int32'),
+            ('channel', 'int32'),
+            ('fft0', 'float32', (self.nffte, self.fftlen, 2)),
+            ('fft1', 'float32', (self.nffte, self.fftlen, 2))
+        ])
+        global_struct = header_struct +\
+            [('data', beamlet_dtype, (self.nbchan))]
+        global_dtype = np.dtype(global_struct)
+        itemsize = global_dtype.itemsize
+        with open(self._lanefile, 'rb') as rf:
+            tmp = np.memmap(rf, dtype='int8', mode='r')
+        n_blocks = tmp.size * tmp.itemsize // (itemsize)
+        data = da.from_array(
+            tmp[: n_blocks * itemsize].view(global_dtype)
+        )['data'] # dask powered
+        # Store data in appropriated attributes
+        self.fft0 = data['fft0']
+        self.fft1 = data['fft1']
+        self.beam_arr = data['beam'][0].compute() # asummed same for all time step
+        self.chan = data['channel']
+        ntb, nfb = data['lane'].shape # time blocks, freq blocks
+        # self.unix = np.arange(ntb, dtype='float64')
+        # self.unix *= self.block_dt.to(u.s).value
+        # self.unix += self.timestamp # Maybe I dont need .unix...
+        log.debug(
+            f'Data of {self._lanefile} correctly parsed.'
+        )
+        # Time array
+        n_times = ntb * self.nffte
+        self._times = da.from_array(
+            np.arange(n_times, dtype='float64')
+        )
+        self._times *= self.dt.value
+        self._times += self.timestamp + self.blockseqnumber/195312.5
+        # Frequency array
+        n_freqs = nfb * self.fftlen
+        self._freqs = da.from_array(
+            np.tile(np.arange(self.fftlen) - self.fftlen/2, nfb)
+        )
+        self._freqs = self._freqs.reshape((nfb, self.fftlen))
+        self._freqs *= self.df.to(u.Hz).value
+        self._freqs += self.chan[0, :][:, np.newaxis] * self.subband_width.value # assumed constant over time
+        self._freqs = self._freqs.ravel()
+        # Beam indices
+        unique_b = np.unique(self.beam_arr)
+        self.beam_idx = {}
+        for b in unique_b:
+            b_idx = np.where(self.beam_arr == b)[0]
+            self.beam_idx[str(b)] = (
+                b_idx[0] * self.fftlen, # freq start of beam
+                (b_idx[-1] + 1) * self.fftlen # freq stop of beam
+            )
+        return
 
-# ============================================================= #
-# -------------------------- ma_pos --------------------------- #
-# ============================================================= #
-rot = np.radians(-90)
-rotation = np.array(
-    [
-        [ np.cos(rot), np.sin(rot), 0],
-        [-np.sin(rot), np.cos(rot), 0],
-        [ 0,           0,           1]
-    ]
-)
-ma_pos = np.dot(
-    np.array([aa.tolist() for aa in ma_info['pos']]),
-    rotation
-)
-# ============================================================= #
 
+    def _to2d(self, data):
+        """ Inverts the halves of each beamlet and reshape the
+            array in 2D (time, frequency).
+        """
+        ntb, nfb = data.shape[:2]
+        data = np.swapaxes(data, 1, 2)
+        n_times = ntb * self.nffte
+        n_freqs = nfb * self.fftlen
+        # Invert the halves of the beamlet
+        if self.fftlen % 2. != 0.0:
+            raise ValueError(
+                f'Problem with fftlen value: {self.fftlen}!'
+            )
+        data = data.reshape(
+            (
+                n_times,
+                int(n_freqs/self.fftlen),
+                2,
+                int(self.fftlen/2)
+            )
+        )
+        # data = data[:, :, ::-1, :].reshape((n_times, n_freqs-nfb))
+        data = data[:, :, ::-1, :].reshape((n_times, n_freqs))
+        return data
+
+
+    # def _bandpass(self):
+    #     """ Computes the bandpass correction for a beamlet.
+    #     """
+    #     kaiser_file = join(
+    #         dirname(abspath(__file__)),
+    #         'bandpass_coeffs.dat'
+    #     )
+    #     kaiser = np.loadtxt(kaiser_file)
+
+    #     n_tap = 16
+    #     over_sampling = self.fftlen // n_tap
+    #     n_fft = over_sampling * kaiser.size
+
+    #     g_high_res = np.fft.fft(kaiser, n_fft)
+    #     mid = self.fftlen // 2
+    #     middle = np.r_[g_high_res[-mid:], g_high_res[:mid]]
+    #     right = g_high_res[mid:mid + self.fftlen]
+    #     left = g_high_res[-mid - self.fftlen:-mid]
+
+    #     midsq = np.abs(middle)**2
+    #     leftsq = np.abs(left)**2
+    #     rightsq = np.abs(right)**2
+    #     g = 2**25/np.sqrt(midsq + leftsq + rightsq)
+    #     return g**2.
+
+
+    # def _bp_correct(self, data, method='standard'):
+    #     """ Applies the bandpass correction to each beamlet
+    #     """
+    #     if method.lower() == 'standard':
+    #         bp = self._bandpass()
+    #         ntimes, nfreqs = data.shape
+    #         data = data.reshape(
+    #             (
+    #                 ntimes,
+    #                 int(nfreqs/bp.size),
+    #                 bp.size
+    #             )
+    #         )
+    #         data *= bp[np.newaxis, np.newaxis]
+    #         return data.reshape((ntimes, nfreqs))
+    #     elif method.lower() == 'median':
+    #         ntimes, nfreqs = data.shape
+    #         spectrum = np.median(data, axis=0)
+    #         folded = spectrum.reshape(
+    #             (int(spectrum.size / self.fftlen), self.fftlen)
+    #             )
+    #         broadband = np.median(folded, axis=1)
+    #         data = data.reshape(
+    #             (
+    #                 ntimes,
+    #                 int(spectrum.size / self.fftlen),
+    #                 self.fftlen
+    #             )
+    #         )
+    #         data *= broadband[np.newaxis, :, np.newaxis]
+    #         return data.reshape((ntimes, nfreqs)) / spectrum
+    #     elif method.lower() == 'none':
+    #         return data
+
+    def _polarization_correction(fft0, fft1, jones):
+        """
+            fft0[..., :] = [XX, YY]
+            fft1[..., :] = [Re(XY*), Im(XY*)]
+            XX=I+Q YY=I-Q XY=U+iV YX=U-iV
+        """
+        # fft0.shape = (time_blocks, subbands, time_per_blocks, channels, 2)
+        # jones.shape = (time, frequency, 2, 2)
+        xx = fft0[..., 0]
+        yy = fft1[..., 1]
+        xy = fft1[..., 0] + 1j*fft1[..., 1]
+        yx = fft1[..., 0] - 1j*fft1[..., 1]
 
 # ============================================================= #
-# ----------------------- HiddenPrints ------------------------ #
-# ============================================================= #
-class _HiddenPrints:
-    def __enter__(self):
-        self._original_stdout = sys.stdout
-        sys.stdout = open(os.devnull, 'w')
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        sys.stdout.close()
-        sys.stdout = self._original_stdout
-# ============================================================= #
 
 
 # ============================================================= #
-# ------------------------ nenufar_loc ------------------------ #
-# ============================================================= #
-nenufar_loc = EarthLocation(
-    lat=47.376511 * u.deg,
-    lon=2.1924002 * u.deg,
-    height=135.834 * u.m
-)
-# ============================================================= #
+# -------------------------- Dynspec -------------------------- #
+# ============================================================= #
+class Dynspec(object):
+    """ Main class to read and analyze UnDySPuTeD high-rate data.
+
+        :param lanefiles:
+            List of ``*.spctra`` files (see :attr:`~nenupy.undysputed.dynspec.Dynspec.lanefiles`).
+        :type lanefiles: `list`
 
-
-# ============================================================= #
-# -------------------------- getMAL93 ------------------------- #
-# ============================================================= #
-def getMAL93(m):
-    """
+        .. versionadded:: 1.1.0
     """
-    ma_pos = np.array([a.tolist() for a in ma_info['pos']])
-    available_mas = np.arange(ma_pos.shape[0])
-    antpos = ma_pos[np.isin(available_mas, m)]
-    return antpos
-# ============================================================= #
 
+    def __init__(self, lanefiles=[]):
+        self.lanes = []
+        self.lanefiles = lanefiles
+        log.info(
+            'Observation properties:'\
+            f'\n\tTime : {self.tmin.isot} --> {self.tmax.isot}'\
+            f'\n\tFrequency : {self.fmin} --> {self.fmax}'\
+            f'\n\tTime step : {self.dt}'\
+            f'\n\tFrequency step : {self.df}'
+        )
+        self.beam = 0
+        self.dispersion_measure = None
+        self.rebin_dt = None
+        self.rebin_df = None
+        self.jump_correction = False
+        self.bp_correction = 'none'
+        self.freq_flat = False
+        self.clean_rfi = False
+
+
+    # --------------------------------------------------------- #
+    # --------------------- Getter/Setter --------------------- #
+    @property
+    def lanefiles(self):
+        """ UnDySPuTeD time-frequency files input (i.e. one file
+            per lane) that are stored in the attribute 
+            :attr:`~nenupy.undysputed.dynspec.Dynspec.lanes` as
+            :class:`~nenupy.undysputed.dynspec._Lane` instances.
+
+            Subsequent selections in time, frequency, beam and
+            data operation processes will be run on these files
+            while querying only those required. It means that any
+            file listed in input is not necessarily read, and
+            therefore having more files in input than needed
+            does not increase memory usage or computing time.
+
+            :setter: `list` of ``'*.spectra'`` files.
+
+            :getter: `list` of ``'*.spectra'`` files.
+
+            :type: `list`
+
+            :Example:
+                >>> from nenupy.undysputed import Dynspec
+                >>> ds = Dynspec(
+                        lanefiles=['lane_0.spectra', 'lane_0.spectra']
+                    )
+                >>> ds.lanefiles
+                ['/path/to/lane_0.spectra', '/path/to/lane_0.spectra']
+
+            .. warning::
+                Files are checked to belong to the same
+                observation based on their prefix.
+    
+            .. versionadded:: 1.1.0
+        """
+        return list(self._lanefiles)
+    @lanefiles.setter
+    def lanefiles(self, l):
+        if not isinstance(l, list):
+            l = [l]
+        l = list(map(abspath, l))
+        # Check that all the input files belong to the same obs TO REDO
+        # names = list(map(basename,l))
+        # obsname = [ni[::-1].split('_', 1)[1] for ni in names]
+        # if obsname != obsname[::-1]:
+        #     raise ValueError(
+        #         'Input files seem not to belong to the same observation.'
+        #     )
+        for li in map(abspath, l):
+            if not isfile(li):
+                raise FileNotFoundError(
+                    f'{li} not found.'
+                )
+            else:
+                log.debug(f'Found {li}')
+                self.lanes.append(
+                    _Lane(li)
+                )
+        self._lanefiles = l
+        return
 
-# ============================================================= #
-# ---------------------- analog_pointing ---------------------- #
-# ============================================================= #
-def analog_pointing(azimuth, elevation):
-    """ NenuFAR Mini-Array pointing is performed using analogical
-        delays between antennas. Therefore, the pointing directions
-        follow a discrete distribution. This function allows for
-        finding the actual pointing order given an aziumuth and
-        an elevation as requests.
-
-        .. image:: ./_images/analog_pointing.png
-            :width: 800
-
-        :param azimuth:
-            Requested azimuth (in degrees if `float`).
-        :type azimuth: `float` or :class:`astropy.units.Quantity`
-        :param elevation:
-            Requested elevation (in degrees if `float`).
-        :type elevation: `float` or :class:`astropy.units.Quantity`
 
-        :returns: (Azimuth, Elevation)
-        :rtype: :class:`astropy.units.Quantity`
-        
-        :Example:
-            >>> from nenupysim.instru import analog_pointing
-            >>> import astropy.units as u
-            >>> analog_pointing(180*u.deg, 45*u.deg)
-            (<Quantity 180. deg>, <Quantity 45.17045975 deg>)
-    """
-    if not isinstance(azimuth, Quantity):
-        azimuth *= u.deg
-    if not isinstance(elevation, Quantity):
-        elevation *= u.deg
-    azimuth = azimuth.to(u.deg)
-    elevation = elevation.to(u.deg)
-    file = join(
-        dirname(__file__),
-        'NenuFAR_thph.fits'
-    )
-    thph = getdata(file) # azimuth, zenith angle
-    if np.isscalar(azimuth) and np.isscalar(elevation):
-        phi_idx = int(azimuth.value/0.05 - 0.5)
-        theta_idx = int((90. - elevation.value)/0.05 - 0.5)
-    else:
-        phi_idx = (azimuth.value/0.05 - 0.5).astype(int)
-        theta_idx = ((90. - elevation.value)/0.05 - 0.5).astype(int)
-    t, p = thph[:, theta_idx, phi_idx]
-    azimuth = p * u.deg
-    elevation = (90. - t) * u.deg
-    return azimuth, elevation
-# ============================================================= #
+    @property
+    def time_range(self):
+        """ Time range selection.
+
+            :setter: Time range expressed as ``[t_min, t_max]``
+                where ``t_min`` and ``t_max`` could either be
+                `str` (ISO or ISOT formats) or :class:`~astropy.time.Time`
+                instances.
+
+            :getter: Time range in UNIX unit.
+
+            :type: `list`
+
+            .. versionadded:: 1.1.0
+        """
+        if not hasattr(self, '_time_range'):
+            return [self.tmin.unix, self.tmax.unix]
+        return self._time_range
+    @time_range.setter
+    def time_range(self, t):
+        if not isinstance(t, list):
+            raise TypeError(
+                'time_range expects a list.'
+            )
+        if not len(t) == 2:
+            raise ValueError(
+                'time_range should be a length-2 list.'
+            )
+        if not all([isinstance(ti, Time) for ti in t]):
+            t = [Time(ti, precision=7) for ti in t]
+        if t[0] >= t[1]:
+            raise ValueError(
+                'time_range start >= stop.'
+            )
+        log.info(
+            f'Time-range set: {t[0].isot} to {t[1].isot}.'
+        )
+        self._time_range = [t[0].unix, t[1].unix]
+        return
 
 
-# ============================================================= #
-# -------------------- desquint_elevation --------------------- #
-# ============================================================= #
-def desquint_elevation(elevation, opt_freq=30):
-    """ Radio phased array are affected by beam squint. Combination
-        of antenna response (maximal at zenith) and array factor
-        of antenna distribution can shift maximal sensitivity
-        towards greater elevations.
-        This function allows for correcting this effect by shifting
-        pointing elevation a little bit lower.
-        The correction is limited to elevation greater than 20 
-        deg, otherwise, analog pointing can shift drastically if
-        a low elevation is required
-        (see :func:`~nenupy.instru.instru.analog_pointing`).
-
-        .. image:: ./_images/desquint.png
-            :width: 800
-
-        :param elevation:
-            Requested elevation (in degrees if `float`).
-        :type elevation: `float` or :class:`astropy.units.Quantity`
-        :param opt_freq:
-            Beam squint optimization frequency (in MHz if `float`)
-        :type opt_freq: `float` or :class:`astropy.units.Quantity`
-
-        :returns: Beamsquint-corrected elevation to point
-        :rtype: :class:`~astropy.units.Quantity`
-
-        :Example:
-            >>> from nenupy.instru import desquint_elevation
-            >>> desquint_elevation(
-                    elevation=45,
-                    opt_freq=80
-                )
-            44.359063°
-    """
-    if not isinstance(elevation, Quantity):
-        elevation *= u.deg
-    if not isinstance(opt_freq, Quantity):
-        opt_freq *= u.MHz
-    elevation = elevation.to(u.deg)
-    opt_freq = opt_freq.to(u.MHz)
-    squint = readsav(
-        join(
-            dirname(__file__),
-            'squint_table.sav'
+    @property
+    def freq_range(self):
+        """ Frequency range selection.
+
+            :setter: Frequency range expressed as ``[f_min, f_max]``
+                where ``f_min`` and ``f_max`` could either be
+                `float` (understood as MHz) or :class:`~astropy.units.Quantity`
+                instances.
+
+            :getter: Frequency range in Hz.
+
+            :type: `list`
+
+            .. versionadded:: 1.1.0
+        """
+        if not hasattr(self, '_freq_range'):
+            return [self.fmin.to(u.Hz), self.fmax.to(u.Hz)]
+        return self._freq_range
+    @freq_range.setter
+    def freq_range(self, f):
+        if not isinstance(f, list):
+            raise TypeError(
+                'freq_range expects a list.'
+            )
+        if not len(f) == 2:
+            raise ValueError(
+                'freq_range should be a length-2 list.'
+            )
+        if not all([isinstance(fi, u.Quantity) for fi in f]):
+            f = [fi*u.MHz for fi in f]
+        if f[0] >= f[1]:
+            raise ValueError(
+                'freq_range min >= max.'
+            )
+        log.info(
+            f'Freq-range set: {f[0].to(u.MHz)} to {f[1].to(u.MHz)}.'
         )
-    )
-    freq_idx = np.argmin(
-        np.abs(squint['freq'] - opt_freq.value)
-    )
-    elevation = interp1d(
-        squint['elev_desiree'][freq_idx, :],
-        squint['elev_a_pointer']
-    )(elevation.value)
-    # Squint is limited at 20 deg elevation, otherwise the
-    # pointing can vary drasticaly as the available pointing
-    # positions become sparse at low elevation.
-    if np.isscalar(elevation):
-        if elevation < 20.:
-            elevation = 20
-    else:
-        elevation[elevation < 20] = 20
-    return elevation * u.deg
-# ============================================================= #
+        self._freq_range = [f[0].to(u.Hz), f[1].to(u.Hz)]
+        return
 
 
-# ============================================================= #
-# --------------------- nenufar_ant_gain ---------------------- #
-# ============================================================= #
-def nenufar_ant_gain(freq, polar='NW', nside=64, time=None, normalize=True):
-    """ Get NenuFAR elementary antenna gain with respect to the
-        frequency ``freq``, the polarization ``polar`` and
-        convert it to HEALPix representation with a given
-        ``nside`` that defines pixel number. The map is initially
-        in horizontal coordinates, conversion to equatorial
-        coordinates requires to set the ``time`` at which the 
-        computation should occur.
-
-        :param freq:
-            Frequency of the returned antenna gain. Its value
-            must be comprised between 10 and 80 MHz, because
-            available antenna models are constrained to these
-            frequencies. If the frequency value exceeds 80 MHz,
-            an extrapolation is made using polynomial fits.
-        :type freq: `float` or :class:`~astropy.units.Quantity`
-        :param polar:
-            Antenna polarization to take into account (either
-            ``'NW'`` or ``'NE'``).
-        :type polar: `str`
-        :param nside:
-            HEALPix nside parameter, must be a power of 2, less
-            than 2**30 (see :func:`~healpy.pixelfunc.nside2resol`
-            for corresponding angular pixel resolution).
-        :type nside: `int`
-        :param time:
-            Time at which the computation occurs, in order to
-            have the right antenna gain pattern on the sky above
-            NenuFAR. If ``None`` the map is not rotated to 
-            equatorial coordinates.
-        :type time: `str` or :class:`~astropy.time.Time`
-        :param normalize:
-            Returns the normalized gain or not.
-        :type normalize: `bool`
-
-        :returns:
-            Sky map in HEALPix representation of normalized
-            antenna gain.
-        :rtype: :class:`~numpy.ndarray`
-
-        :Example:
-            Get the antenna gain and plot it (using
-            :class:`~nenupy.astro.hpxsky.HpxSky`):
-
-            >>> from nenupy.instru import nenufar_ant_gain
-            >>> from nenupy.astro import HpxSky
-            >>> ant_sky = HpxSky(resolution=0.5)
-            >>> ant_sky.skymap = nenufar_ant_gain(
-                    freq=60,
-                    polar='NW',
-                    nside=ant_sky.nside,
-                    time='2020-04-01 12:00:00'
-                )
-            >>> ant_sky.plot()
+    @property
+    def beam(self):
+        """ Select a beam index among available beams
+            :attr:`~nenupy.undysputed.dynspec.Dynspec.beams`.
 
-            .. image:: ./_images/antgain.png
-                :width: 800
-
-        .. seealso::
-            :class:`~nenupy.beam.hpxbeam.HpxABeam`
-    """
-    from healpy import (
-        read_map,
-        ud_grade,
-        nside2npix,
-        pix2ang,
-        Rotator
-    )
-
-    # Parameter checks
-    if not isinstance(freq, Quantity):
-        freq *= u.MHz
-    freq = freq.to(u.MHz).value
-    if polar.lower() not in ['nw', 'ne']:
-        raise ValueError(
-            'Polar should be either NW or NE'
-        )
-    polar = polar.upper()
-    # Correspondance between polar/freq and field index in FITS
-    gain_freqs = np.arange(10, 90, 10, dtype=int)
-    count = 0
-    cols = {}
-    for p in ['NE', 'NW']:#['NW', 'NE']:
-        for f in gain_freqs:
-            cols['{}_{}'.format(p, f)] = count
-            count += 1
-    antgain_file = join(
-        dirname(__file__),
-        'NenuFAR_Ant_Hpx.fits',
-    )
-    if freq < 10:
-        raise ValueError(
-            'No antenna model < 10 MHz.'
-        )
-    elif freq > 80:
-        log.warning(
-            'NenuFAR antenna response is extrapolated > 80 MHz.'
-        )
-        # Will fit a polynomial along the high end of frequencies
-        freq_to_fit = np.arange(40, 90, 10, dtype=int)
-        gains = np.zeros((freq_to_fit.size, nside2npix(64)))
-        # Construct the gain map (freqs, npix)
-        for i, f in enumerate(freq_to_fit):
-            gains[i, :] = read_map(
-                filename=antgain_file,
-                hdu=1,
-                field=cols['{}_{}'.format(polar, f)],
-                verbose=False,
-                memmap=True,
-                dtype=float
-            )
-        # Get the polynomial coefficients
-        coeffs = np.polyfit(freq_to_fit, gains, 3)
-        def poly(x, coeffs):
-            """ Retrieve the polynomial from coefficients
-            """
-            na = np.newaxis
-            order = coeffs.shape[0]
-            poly = np.zeros((x.size, coeffs.shape[1]))
-            for deg in range(order):
-                poly += (x**deg)[:, na] * coeffs[order-deg-1, :][na, :]
-            return poly
-        gain = poly(np.array([freq]), coeffs).ravel()
-    else:
-        # Get Low and High ant gain bounding freq
-        f_low = gain_freqs[gain_freqs <= freq].max()
-        f_high = gain_freqs[gain_freqs >= freq].min()
-        gain_low = read_map(
-            filename=antgain_file,
-            hdu=1,
-            field=cols['{}_{}'.format(polar, f_low)],
-            verbose=False,
-            memmap=True,
-            dtype=float
-        )
-        gain_high = read_map(
-            filename=antgain_file,
-            hdu=1,
-            field=cols['{}_{}'.format(polar, f_high)],
-            verbose=False,
-            memmap=True,
-            dtype=float
-        )
-        # Make interpolation
-        if f_low != f_high:
-            gain = gain_low * (f_high - freq)/10. +\
-                gain_high * (freq - f_low)/10.
-        else:
-            gain = gain_low
-    # Rotate the map to equatorial coordinates
-    if time is not None:
-        if not isinstance(time, Time):
-            time = Time(time)
-        altaz_origin = AltAz(
-            0*u.deg,
-            0*u.deg,
-            location=nenufar_loc,
-            obstime=time
-        )
-        radec_origin = altaz_origin.transform_to(ICRS)
-        rot = Rotator(
-            deg=True,
-            rot=[radec_origin.ra.deg, radec_origin.dec.deg], 
-            coord=['C', 'C'],
-            inv=True
-        )
-        with _HiddenPrints():
-            gain = rot.rotate_map_alms(gain)
-    # Convert HEALPix map to required nside
-    gain = ud_grade(gain, nside_out=nside)
-    return gain / gain.max() if normalize else gain
-# ============================================================= #
+            :setter: Selected beam index. Default is ``0``.
 
+            :getter: Selected beam index.
 
-# ============================================================= #
-# ---------------------- read_cal_table ----------------------- #
-# ============================================================= #
-def read_cal_table(calfile=None):
-    """ Reads NenuFAR antenna delays calibration file.
+            :type: `int`
 
-        :param calfile: 
-            Name of the calibration file to read. If ``None`` or
-            ``'default'`` the standard calibration file is read.
-        :type calfile: `str`
-
-        :returns: 
-            Antenna delays shaped as 
-            (frequency, mini-arrays, polarizations).
-        :rtype: :class:`~numpy.ndarray`
-    """
-    if (calfile is None) or (calfile.lower() == 'default'):
-        calfile = join(
-            dirname(__file__),
-            'cal_pz_2_multi_2019-02-23.dat',
-        )
-    with open(calfile, 'rb') as f:
-        log.info(
-            'Loading calibration table {}'.format(
-                calfile
+            .. versionadded:: 1.1.0
+        """
+        return self._beam
+    @beam.setter
+    def beam(self, b):
+        if not isinstance(b, (int, np.integer)):
+            raise TypeError(
+                'beam should be an integer.'
+            )
+        if b not in self.beams:
+            log.warning(
+                f'Available beam indices are {self.beams}. Setting default to {self.beams[0]}'
             )
+            b = self.beams[0]
+        self._beam = b
+        log.info(
+            f'Beam index set: {b}.'
         )
-        header = []
-        while True:
-            line = f.readline()
-            header.append(line)
-            if line.startswith(b'HeaderStop'):
-                break
-    hd_size = sum([len(s) for s in header])
-    dtype = np.dtype(
-        [
-            ('data', 'float64', (512, 96, 2, 2))
-        ]
-    )
-    tmp = np.memmap(
-        filename=calfile,
-        dtype='int8',
-        mode='r',
-        offset=hd_size
-    )
-    decoded = tmp.view(dtype)[0]['data']
-    data = decoded[..., 0] + 1.j*decoded[..., 1]
-    return data
-# ============================================================= #
+        return
 
 
-# ============================================================= #
-# ---------------------- effective_area ----------------------- #
-# ============================================================= #
-def effective_area(freq=50, antennas=None, miniarrays=None):
-    """ Computes the NenuFAR array effective area.
+    @property
+    def dispersion_measure(self):
+        r""" Apply (if other than ``None``) de-dispersion
+            process to the data in order to compensate for
+            the dispersion delay.
+
+            :setter: Dispersion Measure :math:`\mathcal{D}\mathcal{M}`
+                either as `float` (understood as :math:`\rm{pc}\,\rm{cm}^{-3}`
+                unit) or :class:`~astropy.units.Quantity`.
+
+            :getter: Dispersion Measure :math:`\mathcal{D}\mathcal{M}` in :math:`\rm{pc}\,\rm{cm}^{-3}`.
+
+            :type: :class:`~astropy.units.Quantity` or `float`
+
+            .. versionadded:: 1.1.0
+        """
+        return self._dispersion_measure
+    @dispersion_measure.setter
+    def dispersion_measure(self, dm):
+        if not (dm is None):
+            if not isinstance(dm, u.Quantity):
+                dm *= u.pc / (u.cm**3)
+            dm = dm.to(u.pc / (u.cm**3))
+            log.info(
+                f'DM set to {dm}'
+            )
+        self._dispersion_measure = dm
+        return
 
-        :param freq: 
-            Frequency at which computing the effective area.
-            In MHz if no unit is provided. Default is ``50 MHz``.
-        :type freq: `float` or :class:`~astropy.units.Quantity`
-        :param antennas:
-            Mini-Array antenna indices to take into account.
-            Default is ``None`` (all 19 antennas).
-        :type antennas: `int`, `list` or :class:`~numpy.ndarray`
-        :param miniarrays:
-            Mini-Array indices to take into account.
-            Default is ``None`` (all available MAs).
-        :type miniarrays: `int`, `list` or :class:`~numpy.ndarray`
-
-        :returns: Effective area in squared meters
-        :rtype: :class:`~astropy.units.Quantity`
-
-        :Example:
-            * Effective area of a single antenna from ``MA 0``:
-
-            >>> from nenupy.instru import effective_area
-            >>> effective_area(
-                    freq=50,
-                    antennas=10,
-                    miniarrays=0
-                )
-            11.982422 m2
 
-            * Effective area of ``MA 0``:
-            
-            >>> from nenupy.instru import effective_area
-            >>> effective_area(
-                    freq=50,
-                    antennas=np.arange(19),
-                    miniarrays=0
-                )
-            227.60482 m2
+    @property
+    def rebin_dt(self):
+        """ Averaged data time step. If ``None`` data will not
+            be time-averaged.
+
+            :setter: Time step  (in sec if no unit is provided).
+
+            :getter: Time step in seconds.
+
+            :type: :class:`~astropy.units.Quantity` or `float`
+
+            .. versionadded:: 1.1.0
+        """
+        return self._rebin_dt
+    @rebin_dt.setter
+    def rebin_dt(self, dt):
+        if not (dt is None):
+            if not isinstance(dt, u.Quantity):
+                dt *= u.s
+            dt = dt.to(u.s)
+            log.info(
+                f'Time averaging on {dt}'
+            )
+        self._rebin_dt = dt
+        return
 
-            * Effective area of NenuFAR with 56 MAs:
-            
-            >>> from nenupy.instru import effective_area
-            >>> effective_area(
-                    freq=50,
-                    antennas=np.arange(19),
-                    miniarrays=np.arange(56)
-                )
-            12745.87 m2
 
-        .. seealso::
-            NenuFAR Mini-Arrays `characteristics
-            <https://nenufar.obs-nancay.fr/en/astronomer/#mini-arrays>`_.
+    @property
+    def rebin_df(self):
+        """ Averaged data frequency step. If ``None`` data will not
+            be frequency-averaged.
+
+            :setter: Frequency step (in MHz is not unit is provided).
+
+            :getter: Frequency step in Hz.
+
+            :type: 
+
+            .. versionadded:: 1.1.0
+        """
+        return self._rebin_df
+    @rebin_df.setter
+    def rebin_df(self, df):
+        if not (df is None):
+            if not isinstance(df, u.Quantity):
+                df *= u.MHz
+            df = df.to(u.Hz)
+            log.info(
+                f'Frequency averaging on {df}'
+            )
+        self._rebin_df = df
+        return
 
-    """
-    if not isinstance(freq, u.Quantity):
-        freq *= u.MHz
-    if antennas is None:
-        antennas = np.arange(19)
-    else:
-        if np.isscalar(antennas):
-            antennas = np.array([antennas])
-        elif isinstance(antennas, list):
-            antennas = np.array(antennas)
-        if max(antennas) > 18:
-            raise ValueError(
-                'Only 19 antennas in NenuFAR MA'
+
+    @property
+    def bp_correction(self):
+        """ Polyphase-filter introduces a band-pass response
+            that may be corrected using one of the following
+            methods:
+
+            * ``'none'``: no band-pass correction is applied,
+            * ``'standard'``: pre-computed coefficients are used to correct the bandpass,
+            * ``'median'``: the band-pass correction is actively corrected (this lead to the best results but it is the slowest method).
+
+            :setter: Band-pass correction method (default is
+                ``'none'``).
+
+            :getter: Band-pass correction method.
+
+            :type: `str`
+
+            .. warning::
+                Effects of bandpass correction may depend
+                on data quality.
+
+                .. image:: ./_images/bandpass_corr.png
+                    :width: 800
+
+            .. versionadded:: 1.1.0
+        """
+        return self._bp_correction
+    @bp_correction.setter
+    def bp_correction(self, b):
+        available = ['standard', 'median', 'none', 'adjusted']
+        if not isinstance(b, str):
+            raise TypeError(
+                'bp_correction must be a string.'
             )
-    if miniarrays is None:
-        miniarrays = np.arange(ma_info['ma'].size)
-    else:
-        if np.isscalar(miniarrays):
-            miniarrays = np.array([miniarrays])
-        elif isinstance(miniarrays, list):
-            miniarrays = np.array(miniarrays)
-        if max(miniarrays) > ma_info.size:
+        b = b.lower()
+        if not b in available:
             raise ValueError(
-                'Only {} Mini-Arrays'.format(ma_info.size)
+                f'Available bandpass corrections are {available}.'
             )
+        log.info(
+            f'Bandpass correction set: {b}.'
+        )
+        self._bp_correction = b
+        return    
 
-    # Antenna Effective Area
-    k = 3
-    wavelength = const.c.to(u.m/u.s) / freq.to(u.Hz)
-    ant_ea = (wavelength**2 / k).to(u.m**2)
-
-    # Mini-Array Effective Area
-    n = 1000 # grid resolution
-    grid = np.zeros(
-        (n, n),
-        dtype=np.int32
-    )
-    ant_ea_radius = np.sqrt(ant_ea/np.pi).to(u.m).value
-    antpos = ma_antpos(rot=0)[antennas]
-    x_grid = np.linspace(
-        antpos[:, 0].min() - ant_ea_radius,
-        antpos[:, 0].max() + ant_ea_radius,
-        n
-    )
-    dx = x_grid[1] - x_grid[0]
-    y_grid = np.linspace(
-        antpos[:, 1].min() - ant_ea_radius,
-        antpos[:, 1].max() + ant_ea_radius,
-        n
-    )
-    dy = y_grid[1] - y_grid[0]
-    xx_grid, yy_grid = np.meshgrid(x_grid, y_grid)
-    for xi, yi, zi in antpos:
-        dist = np.sqrt((xx_grid - xi)**2. + (yy_grid - yi)**2.)
-        grid[dist <= ant_ea_radius] += 1
-    grid[grid != 0] = 1
-    ma_ea = (grid * dx * dy).sum() * (u.m**2)
 
-    # NenuFAR Effective Area
-    return ma_ea * miniarrays.size
-# ============================================================= #
+    @property
+    def jump_correction(self):
+        """ Correct or not the known 6-minute gain jumps
+            due to analogical Mini-Array pointing orders.
 
+            :setter: 6-min jump correction.
 
-# ============================================================= #
-# ---------------------- sky_temperature ---------------------- #
-# ============================================================= #
-def sky_temperature(freq=50):
-    r""" Sky temperature at a given frequency ``freq`` (strongly
-        dominated by Galactic emission).
-
-        .. math::
-            T_{\rm sky} = T_0 \lambda^{2.55}
-
-        with :math:`T_0 = 60 \pm 20\,\rm{K}` for Galactic
-        latitudes between 10 and 90 degrees.
-
-        :param freq:
-            Frequency at which computing the esky temperature.
-            In MHz if no unit is provided. Default is ``50 MHz``.
-        :type freq: `float` or :class:`~astropy.units.Quantity`
-
-        :returns: Sky temperature in Kelvins
-        :rtype: :class:`~astropy.units.Quantity`
-
-        .. seealso::
-            `LOFAR website <http://old.astron.nl/radio-observatory/astronomers/lofar-imaging-capabilities-sensitivity/sensitivity-lofar-array/sensiti>`_, 
-            Haslam et al. (1982) and Mozdzen et al. (2017, 2019)
-    """
-    if not isinstance(freq, u.Quantity):
-        freq *= u.MHz
-    wavelength = (const.c/freq).to(u.m).value
-    t0 = 60. * u.K
-    tsky = t0 * wavelength**2.55
-    return tsky
-# ============================================================= #
+            :getter: 6-min jump correction.
 
+            :type: `bool`
 
-# ============================================================= #
-# --------------------- inst_temperature ---------------------- #
-# ============================================================= #
-def inst_temperature(freq=50):
-    """ Instrument temperature at a given frequency ``freq``.
-        This depends on the Low Noise Amplifier characteristics.
-
-        :param freq:
-            Frequency at which computing the esky temperature.
-            In MHz if no unit is provided. Default is ``50 MHz``.
-        :type freq: `float` or :class:`~astropy.units.Quantity`
+            .. versionadded:: 1.1.0
+        """
+        return self._jump_correction
+    @jump_correction.setter
+    def jump_correction(self, j):
+        if not isinstance(j, bool):
+            raise TypeError(
+                'jump_correction must be a boolean.'
+            )
+        log.info(
+            f'6-min jump correction set: {j}.'
+        )
+        self._jump_correction = j
+        return
 
-        :returns: Instrument temperature in Kelvins
-        :rtype: :class:`~astropy.units.Quantity`
 
-        .. seealso::
-            :func:`~nenupy.instru.instru.sky_temperature`
-    """
-    if isinstance(freq, u.Quantity):
-        freq = freq.to(u.MHz).value
-    lna_sky = np.array([
-        5.0965,2.3284,1.0268,0.4399,0.2113,0.1190,0.0822,0.0686,
-        0.0656,0.0683,0.0728,0.0770,0.0795,0.0799,0.0783,0.0751,
-        0.0710,0.0667,0.0629,0.0610,0.0614,0.0630,0.0651,0.0672,
-        0.0694,0.0714,0.0728,0.0739,0.0751,0.0769,0.0797,0.0837,
-        0.0889,0.0952,0.1027,0.1114,0.1212,0.1318,0.1434,0.1562,
-        0.1700,0.1841,0.1971,0.2072,0.2135,0.2168,0.2175,0.2159,
-        0.2121,0.2070,0.2022,0.1985,0.1974,0.2001,0.2063,0.2148,
-        0.2246,0.2348,0.2462,0.2600,0.2783,0.3040,0.3390,0.3846,
-        0.4425,0.5167,0.6183,0.7689,1.0086,1.4042,2.0732
-    ])
-    freqs = (np.arange(71) + 15) # MHz
-    tsky = sky_temperature(freq=freq)
-    tinst = tsky * lna_sky[ np.abs(freqs - freq).argmin() ]
-    return tinst
-# ============================================================= #
+    @property
+    def tmin(self):
+        """ Start time of the whole observation.
 
+            :getter: Minimal observation time.
 
-# ============================================================= #
-# --------------------------- sefd ---------------------------- #
-# ============================================================= #
-def sefd(freq=50, antennas=None, miniarrays=None):
-    r""" Computes the System Equivalent Flux Density (SEFD or
-        system sensitivity).
-        
-        .. math::
-            S_{\rm sys} = \frac{2 \eta k_{\rm B}}{ A_{\rm eff}} T_{\rm sys}
-        
-        with :math:`T_{\rm sys} = T_{\rm sky} + T_{\rm inst}`,
-        the efficiency :math:`\eta = 1` and :math:`k_{\rm B}` the
-        Boltzmann constant.
-
-        :param freq: 
-            Frequency at which computing the SEFD.
-            In MHz if no unit is provided. Default is ``50 MHz``.
-        :type freq: `float` or :class:`~astropy.units.Quantity`
-        :param antennas:
-            Mini-Array antenna indices to take into account.
-            Default is ``None`` (all 19 antennas).
-        :type antennas: `int`, `list` or :class:`~numpy.ndarray`
-        :param miniarrays:
-            Mini-Array indices to take into account.
-            Default is ``None`` (all available MAs).
-        :type miniarrays: `int`, `list` or :class:`~numpy.ndarray`
+            :type: :class:`~astropy.time.Time`
 
-        :returns: SEFD in Janskys
-        :rtype: :class:`~astropy.units.Quantity`
-    
-        .. seealso::
-            `LOFAR website <http://old.astron.nl/radio-observatory/astronomers/lofar-imaging-capabilities-sensitivity/sensitivity-lofar-array/sensiti>`_, 
-            :func:`~nenupy.instru.instru.sky_temperature` for :math:`T_{\rm sky}`,
-            :func:`~nenupy.instru.instru.inst_temperature` for :math:`T_{\rm inst}`,
-            :func:`~nenupy.instru.instru.effective_area` for :math:`A_{\rm eff}`.
-    """
-    efficiency = 1.
-    aeff = effective_area(
-        freq=freq,
-        antennas=antennas,
-        miniarrays=miniarrays)
-    tsky = sky_temperature(freq=freq)
-    tinst = inst_temperature(freq=freq)
-    tsys = tsky + tinst
-    sefd = 2 * efficiency * const.k_B * tsys / aeff
-    return sefd.to(u.Jy)
-# ============================================================= #
+            .. versionadded:: 1.1.0
+        """
+        return min(li.tmin for li in self.lanes)
 
 
-# ============================================================= #
-# ------------------------ sensitivity ------------------------ #
-# ============================================================= #
-def sensitivity(mode='imaging', freq=50, antennas=None, miniarrays=None, dt=1, df=1):
-    r""" Returns the sensitivity of NenuFAR.
+    @property
+    def tmax(self):
+        """ End-time of the whole observation.
 
-        For the imaging mode:
+            :getter: Maximal observation time.
 
-        .. math::
-            \Delta S_{\rm im} = \frac{S_{\rm sys}}{
-                \sqrt{N(N-1) 2 \delta \nu \delta t}
-            }
-
-        For the beamforming mode:
-
-        .. math::
-            \Delta S_{\rm bf} = \frac{S_{\rm sys}}{
-                \sqrt{\delta \nu \delta t}
-            }
-
-        where :math:`S_{\rm sys}` is the System Equivalent Flux
-        Density, :math:`N` is the number of Mini-Arrays involved,
-        :math:`\delta t` is the integration time and
-        :math:`\delta \nu` is the bandwidth.
-
-        :param mode:
-            Observation mode (either ``'imaging'`` or
-            ``'beamforming'``)
-        :type mode: `str`
-        :param freq: 
-            Frequency at which computing the sensitivity.
-            In MHz if no unit is provided. Default is ``50 MHz``.
-        :type freq: `float` or :class:`~astropy.units.Quantity`
-        :param antennas:
-            Mini-Array antenna indices to take into account.
-            Default is ``None`` (all 19 antennas).
-        :type antennas: `int`, `list` or :class:`~numpy.ndarray`
-        :param miniarrays:
-            Mini-Array indices to take into account.
-            Default is ``None`` (all available MAs).
-        :type miniarrays: `int`, `list` or :class:`~numpy.ndarray`
-        :param dt:
-            Integration time (in sec if `float`)
-        :type dt: `float` or class:`~astropy.units.Quantity`
-        :param df:
-            Bandwidth (in MHz if `float`)
-        :type df: `float` or :class:`~astropy.units.Quantity`
+            :type: :class:`~astropy.time.Time`
 
-        :returns: Sensitivity in Janskys
-        :rtype: :class:`~astropy.units.Quantity`
+            .. versionadded:: 1.1.0
+        """
+        return max(li.tmax for li in self.lanes)
 
-        .. seealso::
-            :func:`~nenupy.instru.instru.sefd` for :math:`S_{\rm sys}`.
-    """
-    if not isinstance(dt, u.Quantity):
-        dt *= u.s
-    if not isinstance(df, u.Quantity):
-        df *= u.MHz
-    ssys = sefd(
-        freq=freq,
-        antennas=antennas,
-        miniarrays=miniarrays
-    )
-    if miniarrays is None:
-        miniarrays = np.arange(ma_info['ma'].size)
-    else:
-        if np.isscalar(miniarrays):
-            miniarrays = np.array([miniarrays])
-        elif isinstance(miniarrays, list):
-            miniarrays = np.array(miniarrays)
-        if max(miniarrays) > ma_info.size:
-            raise ValueError(
-                'Only {} Mini-Arrays'.format(ma_info.size)
-            )
-    nant = miniarrays.size
-    if mode.lower() == 'imaging':
-        sensitivity = ssys / np.sqrt(nant*(nant-1) * 2 * dt * df)
-    elif mode.lower() == 'beamforming':
-        sensitivity = ssys / np.sqrt(dt * df)
-    else:
-        raise ValueError(
-            'Observation mode not understood'
-        )
-    return sensitivity.to(u.Jy)
-# ============================================================= #
 
+    @property
+    def dt(self):
+        """ Native time resolution.
 
-# ============================================================= #
-# ------------------------ resolution ------------------------- #
-# ============================================================= #
-def resolution(freq=50, miniarrays=None):
-    """ Returns the resolution for a given NenuFAR configuration.
+            :getter: Time resolution in seconds.
 
-        :param freq: 
-            Frequency at which computing the resolution.
-            In MHz if no unit is provided. Default is ``50 MHz``.
-        :type freq: `float` or :class:`~astropy.units.Quantity`
-        :param miniarrays:
-            Mini-Array indices to take into account.
-            Default is ``None`` (all available MAs).
-        :type miniarrays: `int`, `list` or :class:`~numpy.ndarray`
-
-        :returns: Resolution in degrees
-        :rtype: :class:`~astropy.units.Quantity`
-
-        :Example:
-            Resolution of the full NenuFAR array:
-
-            >>> from nenupy.instru import resolution
-            >>> resolution(freq=50, miniarrays=None)
-            0.89189836°
-
-            Resolution of a single Mini-Array:
-
-            >>> from nenupy.instru import resolution
-            >>> resolution(freq=50, miniarrays=0)
-            13.741474°
-
-        .. seealso::
-            `NenuFAR characteristics <https://nenufar.obs-nancay.fr/en/astronomer/#mini-arrays>`_.
-
-        .. warning::
-            A 25m diameter is used for a Mini-Array maximum
-            baseline.
-    """
-    if not isinstance(freq, u.Quantity):
-        freq *= u.MHz
-    wavelength = (const.c / freq).to(u.m)
+            :type: :class:`~astropy.units.Quantity`
 
-    if miniarrays is None:
-        miniarrays = np.arange(ma_info['ma'].size)
-    
-    if np.isscalar(miniarrays):
-        # size = np.sqrt(
-        #     np.sum(
-        #         (ma_antpos(0) - np.mean(ma_antpos(0), axis=0))**2,
-        #         axis=-1
-        #     )
-        # ).max()*2* u.m
-        size = 25 * u.m
-    else:
-        if isinstance(miniarrays, list):
-            miniarrays = np.array(miniarrays)
-        if max(miniarrays) > ma_info.size:
-            raise ValueError(
-                'Only {} Mini-Arrays'.format(ma_info.size)
+            .. versionadded:: 1.1.0
+        """
+        dts = np.array([li.dt.value for li in self.lanes])
+        if not all(dts == dts[0]):
+            log.warning(
+                'Lanes have different dt values.'
             )
-        positions = ma_pos[miniarrays]
-        size = np.sqrt(
-            np.sum(
-                (positions - np.mean(positions, axis=0))**2,
-                axis=-1
-            )
-        ).max()*2 * u.m / 1.2
-    psf = wavelength / size
-    return (psf.value * u.rad).to(u.deg)
-# ============================================================= #
+        return self.lanes[0].dt
 
 
-# ============================================================= #
-# ---------------------- confusion_noise ---------------------- #
-# ============================================================= #
-def confusion_noise(freq=50, miniarrays=None):
-    r""" Confusion rms noise :math:`\sigma_{\rm c}` (parameter
-        used for specifying the width of the confusion
-        distribution) computed as:
-
-        .. math::
-            \left( \frac{\sigma_{\rm c}}{\rm{mJy}\, \rm{beam}^{-1}} \right) \simeq
-            0.2 \left( \frac{\nu}{\rm GHz} \right)^{-0.7} 
-            \left( \frac{\theta}{\rm arcmin} \right)^{2}
-        
-        where :math:`\nu` is the frequency and :math:`\theta` is
-        the radiotelescope FWHM.
-        
-        Individual sources fainter than about 
-        :math:`5\sigma_{\rm c}` cannot be detected reliably.
+    @property
+    def fmin(self):
+        """ Minimal frequency recorded for the observation,
+            over all lane file.
 
-        :param freq:
-            Frequency at which computing the confusion noise.
-            In MHz if no unit is provided. Default is ``50 MHz``.
-        :type freq: `float` or :class:`~astropy.units.Quantity`
-        :param miniarrays:
-            Mini-Array indices to take into account.
-            Default is ``None`` (all available MAs).
-        :type miniarrays: `int`, `list` or :class:`~numpy.ndarray`
-
-        :returns: Confusion rms noise in mJy/beam
-        :rtype: :class:`~astropy.units.Quantity`
-
-        :Example:
-            >>> from nenupy.instru import confusion_noise
-            >>> confusion_noise(
-                    freq=50,
-                    miniarrays=None
-                )
-            4663.202 mJy
+            :getter: Minimal frequency in MHz.
 
-        .. see also::
-            `NRAO lecture <https://www.cv.nrao.edu/course/astr534/Radiometers.html>`_ (eq. 3E6),
-            `Takeuchi and Ishii, 2004 <https://ui.adsabs.harvard.edu/abs/2004ApJ...604...40T/abstract>`_.
-    """
-    if not isinstance(freq, u.Quantity):
-        freq *= u.MHz
-    resol = resolution(
-        freq=freq,
-        miniarrays=miniarrays
-    )
-    norm_freq = freq.to(u.GHz).value
-    norm_res = resol.to(u.arcmin).value
-    conf = 0.2 * norm_freq**(-0.7) * norm_res**2
+            :type: :class:`~astropy.units.Quantity`
 
-    return conf * u.mJy # mJy/beam
-# ============================================================= #
+            .. versionadded:: 1.1.0
+        """
+        fm = min(li.fmin for li in self.lanes)
+        return fm.to(u.MHz)
 
 
-# ============================================================= #
-# ------------------------- data_rate ------------------------- #
-# ============================================================= #
-def data_rate(mode='imaging', mas=96, dt=1, nchan=64, bandwidth=75, nb=1):
-    r""" Estimates the NenuFAR data rate product. To get the total
-        observation size, a simple multiplication with a
-        :class:`~astropy.units.Quantity` time instance,
-        corresponding to total exposure time, is needed. To convert
-        bytes in binary base (i.e. 1 kB = 1024 B), use `astropy`
-        unit conversions (with prefixes ``Ki``, ``Mi``, ``Gi`` or
-        ``Ti`` for KiloBytes MegaBytes, GigaBytes and TeraBytes,
-        see `astropy unit prefixes <https://docs.astropy.org/en/stable/units/standard_units.html#prefixes>`_).
-
-        Data rates (in bytes/s) are computed as follows:
-
-        * Imaging mode (*NICKEL* correlator): :math:`r_{\rm im} = n_{\rm correlations} d_{\rm complex\, 64\, bits} n_{\rm channels} n_{\rm baselines} n_{\rm subbands} / \delta t`;
-        * Beamforming mode (*UnDySPuTeD* backend): :math:`r_{\rm bf} = n_{\rm correlations} d_{\rm float\, 32\, bits} n_{\rm channels} n_{\rm subbands} / \delta t`;
-        * Waveform mode (*LaNewBa* backend): :math:`r_{\rm wf} = 195312.5 \times n_{\rm raw} n_{\rm b} n_{\rm subbands}`;
-        * Transient Buffer mode (*LaNewBa* backend): :math:`r_{\rm tbb} = 195312.5 \times 1024 \times n_{\rm raw} n_{\rm b} n_{\rm mas}`;
-        
-        where :math:`n_{\rm correlations} = 4` (XX, XY, YX, YY),
-        :math:`n_{\rm baselines} = n_{\rm mas}*(n_{\rm mas}-1)/2 + n_{\rm mas}`,
-        :math:`n_{\rm subbands} = \Delta \nu / 195.3125\, \rm{kHz}`,
-        :math:`n_{\rm raw} = 4` (Re(X), Im(X), Re(Y), Im(Y)),
-        :math:`d_{\rm complex\, 64\, bits}` and :math:`d_{\rm float\, 32\, bits}`
-        are data sizes in bytes.
-        
-        :param mode:
-            Observation mode (either ``'imaging'`` or
-            ``'beamforming'`` or ``'waveform'`` or ``'tbb'``).
-        :type mode: `str`
-        :param mas: Number of Mini-Arrays to take into account
-            :math:`n_{\rm mas}`. Default is ``96``.
-        :type mas: `int`
-        :param dt: Observation time step :math:`\delta t` (in
-            seconds if no unit is provided). Default is ``1 sec``.
-        :type dt: `float` or :class:`~astropy.units.Quantity`
-        :param nchan: Number of channels per subband :math:`n_{\rm channels}`.
-            Each subband is 195.3125 kHz. Default is ``64``.
-        :type nchan: `int`
-        :param bandwidth: Observation bandwidth :math:`\Delta \nu`
-            (in MHz if no unit is provided). Default is ``75 MHz``.
-        :type bandwidth: `float` or :class:`~astropy.units.Quantity`
-        :param nb: Number of bytes of raw data samples :math:`n_{\rm b}`
-            (``1 = 8 bits``, ``2 = 16 bits``).
-        :type nb: `int`
-
-        :returns: Data rate in bytes/s.
-        :rtype: :class:`~astropy.units.Quantity`
-
-        :example:
-            Imaging data rate and total size for a 1h exposure, converted in TB:
-
-            >>> from nenupy.instru import data_rate
-            >>> import astropy.units as u
-            >>> rate = data_rate(
-                    mode='imaging',
-                    mas=96,
-                    dt=1*u.s,
-                    nchan=64,
-                    bandwidth=75*u.MHz
-                )
-            >>> print(rate)
-            3.6616274×10^9 byte/s
-            >>> exposure = 3600*u.s
-            >>> size = rate * exposure
-            >>> print(size)
-            1.3181859×10^13 byte
-            >>> print(size.to(u.Tibyte))
-            11.988831 Tibyte
-
-        .. note::
-            IDL original version v1, PZ, 2019-03-19
-            
-            PYTHON transcript v1, JG, 2020-05-09
-            
-            Pythonized for `nenupy`, AL, 2020-05-11
+    @property
+    def fmax(self):
+        """ Maximal frequency recorded for the observation,
+            over all lane file.
 
-        .. versionadded:: 1.1.0
-    """
-    # Input checks
-    available_modes = ['imaging', 'beamforming', 'waveform', 'tbb']
-    if not mode in available_modes:
-        raise ValueError(
-            'mode should be one of {}'.format(available_modes)
-        )
-    if not isinstance(mas, int):
-        raise TypeError(
-            'mas should be an integer'
-        )
-    if not isinstance(dt, u.Quantity):
-        dt *= u.s
-    if not isinstance(nchan, int):
-        raise TypeError(
-            'nchan should be an integer'
-        )
-    if nchan > 64:
-        raise ValueError(
-            'NenuFAR maximal number of channels per subband is 64'
-        )
-    if not isinstance(bandwidth, u.Quantity):
-        bandwidth *= u.MHz
-    if bandwidth > 150*u.MHz:
-        raise ValueError(
-            'NenuFAR maximal bandwidth is 150 MHz.'
-        )
+            :getter: Maximal frequency in MHz.
 
-    # NenuFAR backend properties
-    sb_width = 195.3125*u.kHz # subband bandwidth
-    n_sb_max = 768 # maximal number of subbands
-    n_corr = 4 # XX, XY, YX, YY 
-
-    # Number of sub-bands involved
-    n_sb = int(np.round(bandwidth.to(u.kHz)/sb_width))
-
-    if mode == 'imaging':
-        # Complex in bytes
-        nenucomplex = np.complex64().itemsize * u.byte
-        n_baselines = mas*(mas - 1)/2 + mas
-        rate_sb = n_corr*nenucomplex*nchan*n_baselines/dt
-        rate = rate_sb * n_sb
-    elif mode == 'beamforming':
-        # Floats as bytes in NenuFAR calculators
-        nenufloat = np.float32().itemsize * u.byte
-        rate_sb = n_corr*nenufloat*nchan/dt
-        rate = rate_sb * n_sb
-    elif mode == 'waveform':
-        rate_sb = 4*nb*sb_width.to(u.Hz).value
-        rate = rate_sb * n_sb * u.byte / u.s
-    elif mode == 'tbb':
-        rate = 4*nb*sb_width.to(u.Hz).value*1024*mas  * u.byte / u.s
+            :type: :class:`~astropy.units.Quantity`
 
-    return rate
-# ============================================================= #
+            .. versionadded:: 1.1.0
+        """
+        fm = max(li.fmax for li in self.lanes)
+        return fm.to(u.MHz)
 
 
-# ============================================================= #
-# ------------------------- freq2sb --------------------------- #
-# ============================================================= #
-def freq2sb(freq):
-    r""" Conversion between the frequency :math:`\nu` and the
-        NenuFAR sub-band index :math:`n_{\rm SB}`.
-        Each NenuFAR sub-band has a bandwidth of
-        :math:`\Delta \nu = 195.3125\, \rm{kHz}`:
-
-        .. math::
-            n_{\rm SB} = \frac{512 \times \nu}{\Delta \nu}
-
-        :param freq:
-            Frequency to convert in sub-band index (assumed in
-            MHz if no unit is provided).
-        :type freq:
-            `float`, :class:`~numpy.ndarray` or :class:`~astropy.units.Quantity`
-
-        :returns:
-            Sub-band index, same dimension as ``freq``.
-        :rtype: `int` or :class:`~numpy.ndarray`
-
-        :example:
-            >>> from nenupy.instru import freq2sb
-            >>> freq2sb(freq=50.5)
-            258
-            >>> freq2sb(freq=[50.5, 51])
-            array([258, 261])
+    @property
+    def df(self):
+        """ Native frequency resolution.
 
-        .. versionadded:: 1.1.0
-    """
-    if not isinstance(freq, u.Quantity):
-        freq *= u.MHz
-    if (freq.min() < 0 * u.MHz) or (freq.max() > 100 * u.MHz):
-        raise ValueError(
-            'freq should be between 0 and 100 MHz.'
-        )
-    freq = freq.to(u.MHz)
-    sb_width = 100. * u.MHz
-    sb_idx = np.floor((freq * 512) / sb_width)
-    return sb_idx.astype(int).value
-# ============================================================= #
+            :getter: Frequency resolution in Hz.
 
+            :type: :class:`~astropy.units.Quantity`
 
-# ============================================================= #
-# ------------------------- freq2sb --------------------------- #
-# ============================================================= #
-def sb2freq(sb):
-    r""" Conversion between NenuFAR sub-band index :math:`n_{\rm SB}`
-        to sub-band starting frequency :math:`\nu_{\rm start}`:
-
-        .. math::
-            \nu_{\rm start} = \frac{n_{\rm SB} \times \Delta \nu}{512}
-
-        Each NenuFAR sub-band has a bandwidth of
-        :math:`\Delta \nu = 195.3125\, \rm{kHz}`, therefore, the
-        sub-band :math:`n_{\rm SB}` goes from :math:`\nu_{\rm start}`
-        to :math:`\nu_{\rm stop} = \nu_{\rm start} + \Delta \nu`.
-
-        :param sb:
-            Sub-band index (from 0 to 511).
-        :type sb: `int` or :class:`~numpy.ndarray` of `int`
-
-        :returns:
-            Sub-band start frequency :math:`\nu_{\rm start}` in MHz.
-        :rtype: :class:`~astropy.units.Quantity`
-
-        :example:
-            >>> from nenupy.instru import sb2freq
-            >>> sb2freq(sb=1)
-            [0.1953125] MHz
-            >>> sb2freq(sb=[1, 2, 3, 4])
-            [0.1953125, 0.390625, 0.5859375, 0.78125] MHz
+            .. versionadded:: 1.1.0
+        """
+        dfs = np.array([li.df.value for li in self.lanes])
+        if not all(dfs == dfs[0]):
+            log.warning(
+                'Lanes have different df values.'
+            )
+        return self.lanes[0].df
 
-        .. versionadded:: 1.1.0
-    """
-    if np.isscalar(sb):
-        sb = np.array([sb])
-    else:
-        sb = np.array(sb)
-    if sb.dtype.name not in ['int32', 'int64']:
-        raise TypeError(
-            'sb should be integers.'
+
+    @property
+    def beams(self):
+        """ Array of unique beam indices recorded during the
+            observation over the different lane files.
+
+            :getter: Available beam indices.
+
+            :type: :class:`~numpy.ndarray`
+
+            .. versionadded:: 1.1.0
+        """
+        un_beams = []
+        for li in self.lanes:
+            lane_beams = [int(lbi) for lbi in li.beam_idx.keys()]
+            un_beams += lane_beams
+        return np.unique(un_beams)
+
+
+    # --------------------------------------------------------- #
+    # ------------------------ Methods ------------------------ #
+    def get(self, stokes='I'):
+        r""" *UnDySPuTeD* produces four quantities: 
+            :math:`|\rm{XX}|^2`,
+            :math:`|\rm{YY}|^2`,
+            :math:`\operatorname{Re}(\rm{XY}^*)`,
+            :math:`\operatorname{Im}(\rm{XY}^*)`. They are used
+            to compute the four `Stokes <https://en.wikipedia.org/wiki/Stokes_parameters>`_
+            parameters (:math:`\rm{I}`, :math:`\rm{Q}`,
+            :math:`\rm{U}`, :math:`\rm{V}`) and the linear
+            polarization :math:`\rm{L}`:
+
+            .. math::
+                \rm{I} = |\rm{XX}|^2 + |\rm{YY}|^2
+
+            .. math::
+                \rm{Q} = |\rm{XX}|^2 - |\rm{YY}|^2
+
+            .. math::
+                \rm{U} =  2 \operatorname{Re}(\rm{XY}^*)
+
+            .. math::
+                \rm{V} =  2 \operatorname{Im}(\rm{XY}^*)
+
+            .. math::
+                \rm{L} = \sqrt{\rm{Q}^2 + \rm{U}^2}
+
+            :param stokes:
+                Stokes parameter to return (case insensitive).
+                Allowed values are ``'I'``, ``'Q'``, ``'U'``,
+                ``'V'``, ``'L'``, ``'XX'``, ``'YY'``. Default
+                is ``'I'``.
+            :type stokes: `str`
+
+            :returns:
+            :rtype: `~nenupy.beamlet.sdata.SData`
+
+            .. versionadded:: 1.1.0
+        """
+        for li in self.lanes:
+            try:
+                beam_start, beam_stop = li.beam_idx[str(self.beam)]
+            except KeyError:
+                # No beam 'self.beam' found on this lane
+                continue
+            data = li.get_stokes(
+                stokes=stokes#,
+                #bpcorr=self.bp_correction
+            )
+            # Time selection
+            # way more efficient to compute indices than masking
+            tmin_idx = np.argmin(
+                np.abs(li._times - self.time_range[0])
+            ).compute()
+            tmax_idx = np.argmin(
+                np.abs(li._times - self.time_range[1])
+            ).compute()
+            # Freq/beam selection
+            # way more efficient to compute indices than masking
+            fmin_idx = np.argmin(
+                np.abs(li._freqs[beam_start:beam_stop] - self.freq_range[0].value)
+            ).compute()
+            fmax_idx = np.argmin(
+                np.abs(li._freqs[beam_start:beam_stop] - self.freq_range[1].value)
+            ).compute()
+            if (fmin_idx - fmax_idx) == 0:
+                # No data selected on this lane
+                continue
+            # Ensure that frequency indices are at the bottom and top
+            # of a subband (to ease bandpass computation)
+            fmin_idx = (fmin_idx//li.fftlen)*li.fftlen
+            fmax_idx = (fmax_idx//li.fftlen+1)*li.fftlen
+
+            log.info(
+                f'Retrieving data selection from lane {li.lane_index}...'
+            )
+            # High-rate data selection
+            data = data[:, beam_start:beam_stop][
+                tmin_idx:tmax_idx,
+                fmin_idx:fmax_idx
+            ]
+            # Bandpass correction
+            data = self._bp_correct(
+                data=data,
+                fftlen=li.fftlen
+            )
+            selfreqs = li._freqs[beam_start:beam_stop][fmin_idx:fmax_idx].compute()*u.Hz
+            # Remove channels
+            # mask = np.ones(a.size, dtype=bool)
+            # mask::4] = 0
+            # data = data[:, ]
+            # RFI mitigation
+            data = self._clean(
+                data=data
+            )
+            # Correct 6 min jumps
+            data = self._correct_jumps(
+                data=data,
+                dt=li.dt
+            )
+            # Dedispersion if FRB or Pulsar
+            data = self._dedisperse(
+                data=data,
+                freqs=selfreqs,
+                dt=li.dt
+            )
+            # Rebin data to downweight the output
+            data, seltimes, selfreqs = self._rebin(
+                data=data,
+                times=li._times[tmin_idx:tmax_idx],
+                freqs=selfreqs,
+                dt=li.dt,
+                df=li.df,
+            )
+            with ProgressBar():
+                data = data.compute()
+            # Build a SData instance
+            sd = SData(
+                data=data[..., np.newaxis],
+                time=seltimes,
+                freq=selfreqs,
+                polar=stokes,
+            )
+            # Stack in frequency the SData instances at
+            # each lane reading
+            if not 'spec' in locals():
+                spec = sd
+            else:
+                spec = spec & sd
+        log.info(
+            f'Stokes {stokes} data gathered.'
+        )
+        return spec
+
+
+    # --------------------------------------------------------- #
+    # ----------------------- Internal ------------------------ #
+    def _bandpass(self, fftlen):
+        """ Computes the bandpass correction for a beamlet.
+        """
+        kaiser_file = join(
+            dirname(abspath(__file__)),
+            'bandpass_coeffs.dat'
         )
-    if (sb.min() < 0) or (sb.max() > 511):
-        raise ValueError(
-            'sb should be between 0 and 511.'
+        kaiser = np.loadtxt(kaiser_file)
+
+        n_tap = 16
+        over_sampling = fftlen // n_tap
+        n_fft = over_sampling * kaiser.size
+
+        g_high_res = np.fft.fft(kaiser, n_fft)
+        mid = fftlen // 2
+        middle = np.r_[g_high_res[-mid:], g_high_res[:mid]]
+        right = g_high_res[mid:mid + fftlen]
+        left = g_high_res[-mid - fftlen:-mid]
+
+        midsq = np.abs(middle)**2
+        leftsq = np.abs(left)**2
+        rightsq = np.abs(right)**2
+        g = 2**25/np.sqrt(midsq + leftsq + rightsq)
+        return g**2.
+
+
+    def _bp_correct(self, data, fftlen):
+        """ Applies the bandpass correction to each beamlet
+        """
+        if self.bp_correction == 'standard':
+            bp = self._bandpass(fftlen=fftlen)
+            ntimes, nfreqs = data.shape
+            data = data.reshape(
+                (
+                    ntimes,
+                    int(nfreqs/bp.size),
+                    bp.size
+                )
+            )
+            data *= bp[np.newaxis, np.newaxis]
+            return data.reshape((ntimes, nfreqs))
+        elif self.bp_correction == 'median':
+            ntimes, nfreqs = data.shape
+            spectrum = np.median(data, axis=0)
+            folded = spectrum.reshape(
+                (int(spectrum.size / fftlen), fftlen)
+                )
+            broadband = np.median(folded, axis=1)
+            data = data.reshape(
+                (
+                    ntimes,
+                    int(spectrum.size / fftlen),
+                    fftlen
+                )
+            )
+            data *= broadband[np.newaxis, :, np.newaxis]
+            return data.reshape((ntimes, nfreqs)) / spectrum
+        elif self.bp_correction == 'adjusted':
+            ntimes, nfreqs = data.shape
+            data = data.reshape(
+                (
+                    ntimes,
+                    int(nfreqs/fftlen),
+                    fftlen
+                )
+            )
+            freqProfile = np.median(data, axis=0)
+            medianPerSubband = np.median(freqProfile, axis=1)
+            subbandProfileNormalized = freqProfile / medianPerSubband[:, None]
+            subbandProfile = np.median(subbandProfileNormalized, axis=0)
+            data /= subbandProfile[None, None, :]
+            return data.reshape((ntimes, nfreqs))
+        elif self.bp_correction == 'none':
+            return data
+
+
+    def _freqFlattening(self, data):
+        """ Flatten the sub-band response
+        """
+        return data
+
+
+    def _clean(self, data):
+        """
+        """
+        if self.clean_rfi:
+            pass
+        return data
+
+
+    def _dedisperse(self, data, freqs, dt):
+        """
+            This cannot be done properly with dask...
+
+            .. versionadded:: 1.1.0
+        """
+        if not (self.dispersion_measure is None):
+            log.info(
+                'Starting de-dispersion...'
+            )
+            with ProgressBar():
+                data = data.compute()
+            if data.shape[1] != freqs.size:
+                raise ValueError(
+                    'Problem with frequency axis.'
+                )
+            dm = self.dispersion_measure.value # pc/cm^3
+            delays = dispersion_delay(
+                frequency=freqs,
+                dispersion_measure=self.dispersion_measure
+            )
+            delays -= dispersion_delay( # relative delays
+                frequency=self.freq_range[1],
+                dispersion_measure=self.dispersion_measure
+            )
+            cell_delays = np.round((delays/dt)).astype(int)
+            for i in range(freqs.size):
+                data[:, i] = np.roll(data[:, i], -cell_delays[i], 0)
+                # mask right edge of dynspec
+                data[-cell_delays[i]:, i] = np.nan
+            log.info(
+                'Data are de-dispersed.'
+            )
+            data = da.from_array(data)
+        return data
+
+    # def _dedisperse(self, data, freqs, dt):
+    #     """
+    #         .. versionadded:: 1.1.0
+    #     """
+    #     if not (self.dispersion_measure is None):
+    #         log.info(
+    #             'Starting de-dispersion...'
+    #         )
+    #         if data.shape[1] != freqs.size:
+    #             raise ValueError(
+    #                 'Problem with frequency axis.'
+    #             )
+    #         dm = self.dispersion_measure.value # pc/cm^3
+    #         delays = dispersion_delay(
+    #             freq=freqs,
+    #             dm=self.dispersion_measure)
+    #         delays -= dispersion_delay( # relative delays
+    #             freq=self.freq_range[1],
+    #             dm=self.dispersion_measure
+    #         )
+    #         cell_delays = np.round((delays/dt).value).astype(int)
+    #         #nans = np.ones(data.shape[0])
+    #         rows = []
+    #         for i in range(freqs.size):
+    #             # No item assignement in dask (https://github.com/dask/dask/issues/4399)
+    #             # data[:, i] = np.roll(data[:, i], -cell_delays[i], 0)
+    #             #data[:, i] = np.roll(data[:, i], -cell_delays[i], 0)/data[:, i]
+    #             # mask right edge of dynspec
+    #             #data[-cell_delays[i]:, i] = np.nan
+    #             #data[-cell_delays[i]:, i] *= np.nan
+
+    #             dedispersed_row = da.roll(data[:, i], -cell_delays[i], 0)
+    #             #nans[-cell_delays[i]:] = np.nan
+    #             #dedispersed_row *= nans
+                
+    #             # if 'dedispersed_data' in locals():
+    #             #     dedispersed_data = np.vstack((dedispersed_data, dedispersed_row))
+    #             # else:
+    #             #     dedispersed_data = dedispersed_row
+                
+    #             rows.append(dedispersed_row)
+
+    #         data = da.stack(rows, axis=1)
+    #         log.info(
+    #             'Data are de-dispersed.'
+    #         )
+    #     return data
+
+
+    def _rebin(self, data, times, freqs, dt, df):
+        """
+            .. versionadded:: 1.1.0
+        """
+        ntimes_i, nfreqs_i = data.shape
+        if not (self.rebin_dt is None):
+            # Rebin in time
+            tbins = int(np.floor(self.rebin_dt/dt))
+            log.info(
+                f'Time-averaging {tbins} spectra, dt={tbins*dt}...'
+            )
+            ntimes = int(np.floor(ntimes_i/tbins))
+            tleftover = ntimes_i % ntimes
+            log.info(
+                f'Last {tleftover} spectra are left over for time-averaging.'
+            )
+            data = data[:-tleftover if tleftover != 0 else ntimes_i, :].reshape(
+                (ntimes, int((ntimes_i - tleftover)/ntimes), nfreqs_i)
+            )
+            times = times[:-tleftover if tleftover != 0 else ntimes_i].reshape(
+                (ntimes, int((ntimes_i - tleftover)/ntimes))
+            )
+            data = np.mean(data, axis=1)
+            times = np.mean(times, axis=1)
+            ntimes_i, nfreqs_i = data.shape
+            log.info(
+                'Data are time-averaged.'
+            )
+        if not (self.rebin_df is None):
+            # Rebin in frequency
+            fbins = int(np.floor(self.rebin_df/df))
+            log.info(
+                f'Frequency-averaging {fbins} channels: df={fbins*df}...'
+            )
+            nfreqs = int(np.floor(nfreqs_i/fbins))
+            fleftover = nfreqs_i % nfreqs
+            log.info(
+                f'Last {fleftover} channels are left over for frequency-averaging.'
+            )
+            data = data[:, :-fleftover if fleftover != 0 else nfreqs_i].reshape(
+                (ntimes_i, nfreqs, int((nfreqs_i - fleftover)/nfreqs))
+            )
+            freqs = freqs[:-fleftover if fleftover != 0 else nfreqs_i].reshape(
+                (nfreqs, int((nfreqs_i - fleftover)/nfreqs))
+            )
+            data = np.mean(data, axis=2)
+            freqs = np.mean(freqs, axis=1)
+            log.info(
+                'Data are frequency-averaged.'
+            )
+        times = Time(
+            times,
+            format='unix',
+            precision=7
         )
-    sb_width = 100. * u.MHz
-    freq_start = (sb * sb_width) / 512
-    return freq_start
-# ============================================================= #
+        return data, times, freqs
 
 
-# ============================================================= #
-# ------------------------- lnaGain --------------------------- #
-# ============================================================= #
-def lnaGain(freq, filter25=False):
-    """ Returns the NenuFAR Low Noise Amplifier (LNA) gains
-        at given frequencies ``freq``. LNA gains values are linearly
-        interpolated between 15 and 85 MHz.
-
-        :param freq:
-            Frequency at which the LNA gain must be returned.
-        :type freq:
-            `int`, `float`, :class:`~np.ndarray` or :class:`~astropy.units.Quantity`
-        :param filter25:
-            Take into account or not the LNA gain for which a 25 MHz
-            high-pass filter has been applied. Default is ``False``.
-        :type filter25: `bool`
-
-        :returns:
-            Interpolated LNA gain values over ``freq``.
-        :rtype: :class:`~np.ndarray` or :class:`~astropy.units.Quantity`
-
-        :example:
-            >>> from nenupy.instru import lnaGain
-            >>> lnaGain(freq=50)
-            1893.637660993468
-
-            >>> from nenupy.instru import lnaGain
-            >>> import numpy as np
-            >>> lnaGain(freq=np.linspace(20, 22, 2), filter25=True)
-            array([ 41.40509095, 190.31974857])
-
-            >>> from nenupy.instru import lnaGain
-            >>> import numpy as np
-            >>> import astropy.units as u
-            >>> lnaGain(freq=np.linspace(30, 40, 3)*u.MHz)
-            array([ 807.5866613 , 1176.55665449, 1681.93892233])
+    # def _correct_jumps(self, data, dt):
+    #     """ Dask version
+    #     """
+    #     if not self.jump_correction:
+    #         return data
+    #     log.info(
+    #         'Correcting for 6 min pointing jumps...'
+    #     )
+    #     # Work on cleanest profile
+    #     profile = np.median(data, axis=1).compute()
+    #     # detect jumps
+    #     dt = dt.to(u.s).value
+    #     deriv = np.gradient(profile, dt)
+    #     low_threshold = np.nanmedian(deriv) - 8 * np.nanstd(deriv)
+    #     lower_thr_indices = np.where(deriv < low_threshold)[0] # detection
+    #     # Sort jump indices
+    #     jump_idx = [0]
+    #     for idx in lower_thr_indices:
+    #         if idx > jump_idx[-1] + 10:
+    #             jump_idx.append(idx)
+    #     jump_idx.append(data.shape[0] - 1)
+    #     # Make sure there are no > 6min gaps
+    #     sixmin = 6*60.000000 + dt
+    #     for idx in range(1, len(jump_idx)):
+    #         delta_t = dt * (jump_idx[idx] - jump_idx[idx-1])
+    #         if delta_t > sixmin:
+    #             missing_idx = int(np.round(sixmin/dt))
+    #             jump_idx.insert(idx, missing_idx + jump_idx[idx-1])
+    #     # flatten
+    #     boundaries = list(map(list, zip(jump_idx, jump_idx[1:])))
+    #     previous_endpoint = 1.
+    #     flattening = np.ones(data.shape[0])
+    #     for i, boundary in enumerate(boundaries):
+    #         idi, idf = boundary
+    #         med_data_freq = profile[idi:idf]
+    #         flattening[idi:idf] /= med_data_freq
+    #         if i == 0:
+    #             flattening[idi:idf] *= np.median(med_data_freq)
+    #         else:
+    #             flattening[idi:idf] *= previous_endpoint
+    #         previous_endpoint = profile[idf-1] * flattening[idf-1]
+    #     log.info(
+    #         f'Found and corrected {i+1} jump(s).'
+    #     )
+    #     return data*flattening[:, np.newaxis]
+
+
+    # def _correct_jumps_v0(self, data, dt):
+    #     """ Dask version
+    #     """
+    #     if not self.jump_correction:
+    #         return data
+    #     log.info(
+    #         'Correcting for 6 min pointing jumps...'
+    #     )
+    #     six_min = 6*60.000000 * u.s
+    #     seven_min = 7*60.000000 * u.s
+    #     # Find first jump
+    #     log.info(
+    #         'Computing median time-profile...'
+    #     )
+    #     with ProgressBar():
+    #         tprofile = np.median(
+    #             data,
+    #             axis=1
+    #         ).compute()
+    #     from scipy.signal import savgol_filter
+    #     tprofile_smoothed = savgol_filter(
+    #         x=tprofile[:int(seven_min/dt)],
+    #         window_length=11,
+    #         polyorder=2,
+    #         deriv=0
+    #     )
+    #     deriv = np.gradient(tprofile_smoothed, dt.value)
+    #     jump_idx = [0] # start of the time
+    #     jump_idx.append(np.argmin(deriv)) # first jump
+    #     # Deduce next jump indices
+    #     while True:
+    #         next_jump_idx = jump_idx[-1] + int(six_min/dt)
+    #         if next_jump_idx >= data.shape[0]:
+    #             break
+    #         jump_idx.append(next_jump_idx)
+    #     jump_idx.append(data.shape[0] - 1)
+    #     # flatten
+    #     boundaries = list(map(list, zip(jump_idx, jump_idx[1:])))
+    #     previous_endpoint = 1.
+    #     flattening = np.ones(data.shape[0])
+    #     for i, boundary in enumerate(boundaries):
+    #         idi, idf = boundary
+    #         med_data_freq = tprofile[idi:idf]
+    #         flattening[idi:idf] /= med_data_freq
+    #         if i == 0:
+    #             flattening[idi:idf] *= np.median(med_data_freq)
+    #         else:
+    #             flattening[idi:idf] *= previous_endpoint
+    #         previous_endpoint = tprofile[idf-1] * flattening[idf-1]
+    #     log.info(
+    #         f'Found and corrected {i+1} jump(s).'
+    #     )
+    #     return data*flattening[:, np.newaxis]
+
+
+    def _correct_jumps(self, data, dt):
+        """ Dask version
+        """
+        if not self.jump_correction:
+            return data
+        log.info(
+            'Correcting for 6 min pointing jumps...'
+        )
 
-        .. versionadded:: 1.2.0
-    """
-    if isinstance(freq, u.Quantity):
-        freq = freq.to(u.MHz).value
-    file = join(
-        dirname(__file__),
-        'LNA_25MHzFilter.fits' if filter25 else 'LNA_NoFilter.fits'
-    )
-    lnagain = getdata(file)
-    freqs = lnagain['freq'] # MHz
-    gains = lnagain['gain']
-    return np.interp(freq, freqs, gains)
+        freqProfile = np.median(
+            data,
+            axis=0
+        ).compute()
+        timeProfile = np.median(
+            data / freqProfile[None, :],
+            axis=1
+        ).compute()
+
+        duration = timeProfile.size * dt.value
+        sixMin = 6*60.000000
+        nIntervals = int(np.ceil(duration / sixMin))
+        nJumps = nIntervals - 1
+        nPointsJump = int(sixMin / dt.value)
+        nPointsTotal = timeProfile.size
+
+        # Finding interval indices
+        meanTProfile = np.mean(timeProfile)
+        stdTProfile = np.std(timeProfile)
+        timeProfile[timeProfile > meanTProfile + 4*stdTProfile] = meanTProfile # Get rid of strong RFI
+        derivativeTProfile = np.gradient(timeProfile)
+        jumpIndex = np.argmin(derivativeTProfile)
+        firstJumpIndex = jumpIndex%nPointsJump
+        jumpIndices = firstJumpIndex + np.arange(nJumps) * nPointsJump
+        intervalEdges = np.insert(jumpIndices, 0, 0)
+        intervalEdges = np.append(intervalEdges, nPointsTotal - 1)
+
+        # Model fitting for each interval
+        @custom_model
+        def switchLoadFunc(t, a=1., b=1.):
+            """
+                f(t) = a log_10(t) + b
+            """
+            return a*np.log10(t) + b
+        jumpsFitted = np.ones(timeProfile.size)
+        for i in range(intervalEdges.size - 1):
+            lowEdge = intervalEdges[i]
+            highEdge = intervalEdges[i+1]
+            intervalProfile = timeProfile[lowEdge:highEdge+1]
+            switchModel = switchLoadFunc(1e4, np.mean(intervalProfile))
+            fitter = fitting.LevMarLSQFitter()
+            times = 1 + np.arange(intervalProfile.size)
+            switchModel_fit = fitter(switchModel, times, intervalProfile)
+            jumpsFitted[lowEdge:highEdge+1] *= switchModel_fit(times)
+
+        # Model fitting for each interval
+        # @custom_model
+        # def switchLoadFunc(t, a=1., b=1., c=1., d=1., e=1.):
+        #     """
+        #         f(t) = a log_10(t) + b
+        #     """
+        #     return (a*np.log10(t) + b) * (d * t**2 + c * t + e)
+        # jumpsFitted = np.ones(timeProfile.size)
+        # for i in range(intervalEdges.size - 1):
+        #     lowEdge = intervalEdges[i]
+        #     highEdge = intervalEdges[i+1]
+        #     intervalProfile = timeProfile[lowEdge:highEdge+1]
+        #     switchModel = switchLoadFunc(1e4, np.mean(intervalProfile), (intervalProfile[-1]-intervalProfile[0])/sixMin**2, (intervalProfile[-1]-intervalProfile[0])/sixMin, np.mean(intervalProfile))
+        #     fitter = fitting.LevMarLSQFitter()
+        #     times = 1 + np.arange(intervalProfile.size)
+        #     switchModel_fit = fitter(switchModel, times, intervalProfile)
+        #     jumpsFitted[lowEdge:highEdge+1] = switchModel_fit.a.value * np.log10(times) + switchModel_fit.b.value
+        #     jumpsFitted[lowEdge:highEdge+1] /= switchModel_fit.a.value * np.log10(times[-1]) + switchModel_fit.b.value
+
+        return data / jumpsFitted[:, None]
 # ============================================================= #
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `nenupy-2.1.0/nenupy/io/bst.py` & `nenupy-2.2.9/nenupy/io/bst.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 # -*- coding: utf-8 -*-
 
 
 """
     ********
     BST file
     ********
+
+    .. inheritance-diagram:: nenupy.io.bst.BST
+        :parts: 3
+
+    .. autosummary::
+
+        ~BST
+
 """
 
 
 __author__ = 'Alan Loh'
 __copyright__ = 'Copyright 2021, nenupy'
 __credits__ = ['Alan Loh']
 __maintainer__ = 'Alan'
@@ -19,253 +27,237 @@
     "BST"
 ]
 
 
 from astropy.time import Time
 import astropy.units as u
 import numpy as np
-import matplotlib.pyplot as plt
-import matplotlib.dates as mdates
 
-from nenupy.io.io_tools import StatisticsData
+from nenupy.io.io_tools import StatisticsData, ST_Slice
 
 import logging
 log = logging.getLogger(__name__)
 
 
-
 # ============================================================= #
-# ------------------ AnalogBeamConfiguration ------------------ #
-# ============================================================= #
-class AnalogBeamConfiguration:
-    """ """
-
-    def __init__(self, pointing=None):
-        self.pointing = pointing
-
-    @classmethod
-    def from_statistics_metadata(cls, metadata: dict):
-        """ """
-        metadata["pan"]
-        return cls()
-
-# ============================================================= #
-# ============================================================= #
-
-
-# ============================================================= #
-# ------------------------- BST_Slice ------------------------- #
+# ---------------------------- BST ---------------------------- #
 # ============================================================= #
-class BST_Slice:
-    """ """
-
-    def __init__(self, time, frequency, value):
-        self.time = time
-        self.frequency = frequency
-        self.value = value
-
-    
-
-
-    def plot(self, **kwargs):
-        """ """
-        fig = plt.figure(figsize=kwargs.get("figsize", (15, 7)))
-        ax = fig.add_subplot(111)
-        
-        data = self.value.T
-        if kwargs.get("decibel", True):
-            data = 10*np.log10(data)
-        
-        if len(data.shape) == 2:
-            self._plot_dynamic_spectrum(data, ax, fig)
-        elif (len(data.shape) == 1) and (data.size == self.frequency.size):
-            self._plot_spectrum(data, ax, fig)
-        elif (len(data.shape) == 1) and (data.size == self.time.size):
-            self._plot_lightcurve(data, ax, fig)
-        else:
-            raise ValueError("Problem...")
-
-        # Title
-        ax.set_title(kwargs.get("title", ""))
-
-        # Add minor ticks
-        ax.minorticks_on()
-
-        # Save or show the figure
-        figname = kwargs.get("figname", "")
-        if figname != "":
-            plt.savefig(
-                figname,
-                dpi=300,
-                bbox_inches="tight",
-                transparent=True
-            )
-            log.info(f"Figure '{figname}' saved.")
-        else:
-            plt.show()
-        plt.close("all")
-    
-
-    # --------------------------------------------------------- #
-    # ----------------------- Internal ------------------------ #
-    def _plot_spectrum(self, data, ax, fig, **kwargs):
-        """ """
-        ax.plot(self.frequency.to(u.MHz).value, data)
-
-        # X label
-        ax.xaxis.set_major_formatter(
-            mdates.DateFormatter("%H:%M:%S")
-        )
-        fig.autofmt_xdate()
-        ax.set_xlabel("Frequency (MHz)")
-
-        # Y label
-        ax.set_ylabel("dB" if kwargs.get("decibel", True) else "Amp")
-
-
-    def _plot_lightcurve(self, data, ax, fig, **kwargs):
-        """ """
-        ax.plot(self.time.datetime, data)
+class BST(StatisticsData):
+    """ Beamlet STatistics reading class.
 
-        # X label
-        ax.xaxis.set_major_formatter(
-            mdates.DateFormatter("%H:%M:%S")
-        )
-        fig.autofmt_xdate()
-        ax.set_xlabel(f"Time (UTC since {self.time[0].isot})")
+        .. rubric:: Attributes Summary
 
-        # Y label
-        ax.set_ylabel("dB" if kwargs.get("decibel", True) else "Amp")
+        .. autosummary::
 
+            ~BST.analog_beams
+            ~BST.digital_beams
+            ~BST.analog_beam
+            ~BST.beam
+            ~BST.analog_pointing
+            ~BST.digital_pointing
+            ~BST.frequencies
+            ~BST.mini_arrays
 
-    def _plot_dynamic_spectrum(self, data, ax, fig, **kwargs):
-        """ """
-        im = ax.pcolormesh(
-            self.time.datetime,
-            self.frequency.to(u.MHz).value,
-            data,
-            shading="auto",
-            cmap=kwargs.get("cmap", "YlGnBu_r"),
-            vmin=kwargs.get("vmin", np.nanpercentile(data, 5)),
-            vmax=kwargs.get("vmax", np.nanpercentile(data, 95))
-        )
+        .. rubric:: Methods Summary
 
-        if kwargs.get("hatched_overlay", None) is not None:
-            xlim = ax.get_xlim()
-            ylim = ax.get_ylim()
-            overlay_time, overlay_frequency, overlay_values = kwargs["hatched_overlay"]
-            ax.contourf(
-                overlay_time.datetime,
-                overlay_frequency.to(u.MHz).value,
-                overlay_values,
-                levels=[0, 1],
-                hatches=[None, '/'],
-                colors='none',
-                extend='both',
-            )
-            ax.set_xlim(xlim)
-            ax.set_ylim(ylim)
+        .. autosummary::
 
-        cbar = plt.colorbar(im, pad=0.03)
-        cbar.set_label(kwargs.get("colorbar_label", "dB" if kwargs.get("decibel", True) else "Amp"))
-        
-        # X label
-        ax.xaxis.set_major_formatter(
-            mdates.DateFormatter("%H:%M:%S")
-        )
-        fig.autofmt_xdate()
-        ax.set_xlabel(f"Time (UTC since {self.time[0].isot})")
+            ~BST.get
 
-        # Y label
-        ax.set_ylabel(f"Frequency (MHz)")
-# ============================================================= #
-# ============================================================= #
+        .. rubric:: Attributes and Methods Documentation
 
-
-# ============================================================= #
-# ---------------------------- BST ---------------------------- #
-# ============================================================= #
-class BST(StatisticsData):
-    """ """
+    """
 
     def __init__(self, file_name, beam=0):
         super().__init__(file_name=file_name)
         self.beam = beam
-    
 
+
+    # --------------------------------------------------------- #
+    # --------------------- Getter/Setter --------------------- #
     @property
     def analog_beams(self):
-        """ """
+        """ Lists the analog beam indices used for the recording of BST data.
+
+            :getter: List of analog beam indices.
+
+            :type: :class:`~numpy.ndarray`
+        """
         return np.arange(self._meta_data["ana"].size)
 
 
     @property
     def digital_beams(self):
-        """ """
+        """ Lists the digital beam indices used for the recording of BST data.
+
+            :getter: List of digital beam indices.
+
+            :type: :class:`~numpy.ndarray`
+        """
         return np.arange(self._meta_data["bea"].size)
 
 
     @property
     def analog_beam(self):
-        """ """
+        """ Prints the analog beam index currently corresponding to the digital
+            :attr:`~nenupy.io.bst.BST.beam` index.
+
+            :getter: Analog beam index.
+
+            :type: `int`
+        """
+        log.debug(
+            f"Retrieving analog beam index associated with beam #{self.beam}."
+        )
         return self._meta_data["bea"]["NoAnaBeam"][self.beam]
 
 
     @property
     def analog_pointing(self):
-        """ """
-        analog_mask = self._meta_data["pan"]["noAnaBeam"] == self.analog_beam
+        """ Retrieves the analog pointing associated to the current :attr:`~nenupy.io.bst.BST.analog_beam` selected.
+
+            :getter: Analog pointing (time, azimuth, elevation).
+
+            :type:
+                `tuple`(:class:`~astropy.time.Time`, :class:`~astropy.units.Quantity`, :class:`~astropy.units.Quantity`)
+        """
+        analog_beam = self.analog_beam
+        log.debug(
+            f"Retrieving analog pointing associated with analog beam #{analog_beam}."
+        )
+        analog_mask = self._meta_data["pan"]["noAnaBeam"] == analog_beam
         pointing = self._meta_data["pan"][analog_mask]
         return Time(pointing["timestamp"]), pointing["az"]*u.deg, pointing["el"]*u.deg
 
 
     @property
     def digital_pointing(self):
-        """ """
+        """ Retrieves the digital pointing associated to the current :attr:`~nenupy.io.bst.BST.beam` selected.
+
+            :getter: Digital pointing (time, azimuth, elevation).
+
+            :type:
+                `tuple`(:class:`~astropy.time.Time`, :class:`~astropy.units.Quantity`, :class:`~astropy.units.Quantity`)
+        """
+        log.debug(
+            f"Retrieving digital pointing associated with beam #{self.beam}."
+        )
         digital_mask = self._meta_data["pbe"]["noBeam"] == self.beam
         pointing = self._meta_data["pbe"][digital_mask]
         return Time(pointing["timestamp"]), pointing["az"]*u.deg, pointing["el"]*u.deg
 
 
     @property
-    def frequencies(self):
-        """ """
+    def frequencies(self) -> u.Quantity:
+        """ Retrieves the sub-band middle frequency of all the sub-bands recorded for the selected :attr:`~nenupy.io.bst.BST.beam`.
+
+            :getter: Sub-band mid frequencies.
+
+            :type: :class:`~astropy.units.Quantity`
+        """
+        log.debug(
+            f"Retrieving frequencies associated with beam #{self.beam}."
+        )
         beamlets = self._meta_data["bea"]["nbBeamlet"][self.beam]
         subband_half_width = 195.3125*u.kHz
         freqs = self._meta_data["bea"]["freqList"][self.beam][:beamlets]*u.MHz
         return freqs - subband_half_width/2
-    
+
 
     @property
-    def mini_arrays(self):
-        """ """
-        analog_config = self._meta_data["ana"][self.analog_beam]
+    def mini_arrays(self) -> np.ndarray:
+        """ Retrieves the list of Mini-Arrays used to record BST data for the selected :attr:`~nenupy.io.bst.BST.analog_beam`.
+
+            :getter: Mini-Arrays list.
+
+            :type: :class:`~numpy.ndarray`
+        """
+        analog_beam = self.analog_beam
+        log.debug(
+            f"Retrieving Mini-Arrays associated with analog beam #{analog_beam}."
+        )
+        analog_config = self._meta_data["ana"][analog_beam]
         nb_mini_arrays = analog_config["nbMRUsed"]
         return analog_config["MRList"][:nb_mini_arrays]
 
 
     @property
-    def beam(self):
-        """ """
+    def beam(self) -> int:
+        """ Digital beam index.
+
+            :setter: Beam index.
+            
+            :getter: Beam index.
+            
+            :type: `int`
+        """
         return self._beam
     @beam.setter
-    def beam(self, b):
+    def beam(self, b: int):
         if b not in self.digital_beams:
-            log.error(f"Selected beam {b} should be one of {self.digital_beams}.")
+            log.error(
+                f"Selected beam #{b} should be one of {self.digital_beams}."
+            )
             raise IndexError()
         self._beam = b
 
 
+    # --------------------------------------------------------- #
+    # ------------------------ Methods ------------------------ #
     def get(self,
             frequency_selection: str = None,
             time_selection: str = None,
             polarization: str = "NW",
             beam: int = 0
-        ):
-        """ """
+        ) -> ST_Slice:
+        """ Sub-selects BST data.
+            ``frequency_selection`` and ``time_selection``
+            arguments accept `str` values formatted as, e.g.,
+            ``'>={value}'`` or ``'>={value_1} & <{value_2}'`` or ``'=={value}'``.
+
+            :param frequency_selection:
+                Frequency selection. The expected ``'{value}'`` format is frequency units, e.g. ``'>=50MHz'`` or ``'< 1 GHz'``.
+                Default is ``None`` (i.e., no selection upon frequency).
+            :type frequency_selection:
+                `str`
+            :param time_selection:
+                Time selection. The expected ``'{value}'`` format is ISOT, e.g. ``'>=2022-01-01T12:00:00'``.
+                Default is ``None`` (i.e., no selection upon time).
+            :type time_selection:
+                `str`
+            :param polarization:
+                Polarization selection, must be either ``'NW'`` or ``'NE'``.
+                Default is ``'NW'``.
+            :type polarization:
+                `str`
+            :param beam:
+                Digital beam index selection.
+                Default is ``0``.
+            :type beam:
+                `int`
+            
+            :returns:
+                BST data subset.
+            :rtype:
+                :class:`~nenupy.io.io_tools.ST_Slice`
+            
+            :Example:
+                .. code-block:: python
+
+                    from nenupy.io.bst import BST
+
+                    bst = BST("/path/to/BST.fits")
+                    data = bst.get(
+                        frequency_selection="<=52MHz",
+                        time_selection='>=2022-01-24T11:08:10 & <2022-01-24T11:14:08',
+                        polarization="NW",
+                        beam=8
+                    )
+
+        """
         self.beam = beam
 
         # Frequency selection
         frequencies = self.frequencies
         if frequency_selection is None:
             frequency_selection = f">={frequencies.min()} & <= {frequencies.max()}"
         frequency_mask = self._parse_frequency_condition(frequency_selection)(frequencies)
@@ -276,23 +268,38 @@
         # Time selection
         if time_selection is None:
             time_selection = f">={self.time[0].isot} & <= {self.time[-1].isot}"
         time_mask = self._parse_time_condition(time_selection)(self.time)
 
         # Polarization selection
         polars = self._meta_data['ins']['spol'][0]
+        if polarization not in polars:
+            log.warning(
+                f"`polarization` - unknown '{polarization}', setting default value ('NW')."
+            )
+            polarization = "NW"
         polar_idx = np.where(polars == polarization)[0]
-    
-        return BST_Slice(
+
+        log.info(
+            "BST selection applied\n"
+            f"\t- time ({np.sum(time_mask)},): '{time_selection}'\n"
+            f"\t- frequency ({np.sum(frequency_mask)},): '{frequency_selection}'\n"
+            f"\t- polarization (1,): '{polarization}'\n"
+            f"\t- beam (1,): {self.beam}"
+        )
+
+        return ST_Slice(
             time=self.time[time_mask],
             frequency=frequencies[frequency_mask],
             value=np.squeeze(self.data[
                 np.ix_(
                     time_mask,
                     polar_idx,
                     freq_idx
                 )
-            ])
+            ]),
+            analog_pointing_times=self.analog_pointing[0],
+            digital_pointing_times=self.digital_pointing[0]
         )
 # ============================================================= #
 # ============================================================= #
```

### Comparing `nenupy-2.1.0/nenupy/io/xst.py` & `nenupy-2.2.9/nenupy/io/xst.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,42 @@
 #! /usr/bin/python3
 # -*- coding: utf-8 -*-
 
 
 """
     ********
-    BST file
+    XST file
     ********
+
+    .. inheritance-diagram:: nenupy.io.xst.XST nenupy.io.xst.NenufarTV
+        :parts: 3
+
+    .. autosummary::
+
+        ~XST
+        ~NenufarTV
+        TV_Image
+        TV_Nearfield
+
 """
 
 
 __author__ = 'Alan Loh'
 __copyright__ = 'Copyright 2021, nenupy'
 __credits__ = ['Alan Loh']
 __maintainer__ = 'Alan'
 __email__ = 'alan.loh@obspm.fr'
 __status__ = 'Production'
 __all__ = [
-    "XST"
+    "XST_Slice",
+    "Crosslet",
+    "XST",
+    "TV_Image",
+    "TV_Nearfield",
+    "NenufarTV"
 ]
 
 from abc import ABC
 import os
 from itertools import islice
 from astropy.time import Time, TimeDelta
 from astropy.coordinates import SkyCoord, AltAz, Angle
@@ -39,16 +55,15 @@
 from mpl_toolkits.axes_grid1.inset_locator import inset_axes
 import dask.array as da
 from dask.diagnostics import ProgressBar
 
 import nenupy
 from os.path import join, dirname
 from nenupy.astro.target import FixedTarget, SolarSystemTarget
-from nenupy.io.io_tools import StatisticsData
-from nenupy.io.bst import BST_Slice
+from nenupy.io.io_tools import StatisticsData, ST_Slice
 from nenupy.astro import wavelength, altaz_to_radec, l93_to_etrs, etrs_to_enu
 from nenupy.astro.uvw import compute_uvw
 from nenupy.astro.sky import HpxSky
 from nenupy.astro.pointing import Pointing
 from nenupy.instru import NenuFAR, MiniArray, read_cal_table, freq2sb, nenufar_miniarrays
 from nenupy import nenufar_position, DummyCtMgr
 
@@ -56,27 +71,108 @@
 log = logging.getLogger(__name__)
 
 
 # ============================================================= #
 # ------------------------- XST_Slice ------------------------- #
 # ============================================================= #
 class XST_Slice:
-    """ """
+    """ Class to handle the result of selection upon XST-like data.
+
+        .. rubric:: Methods Summary
+
+        .. autosummary::
+
+            ~XST_Slice.plot_correlaton_matrix
+            ~XST_Slice.rephase_visibilities
+            ~XST_Slice.make_image
+            ~XST_Slice.make_nearfield
+
+        .. rubric:: Attributes and Methods Documentation
+
+    """
 
     def __init__(self, mini_arrays, time, frequency, value):
         self.mini_arrays = mini_arrays
         self.time = time
         self.frequency = frequency
         self.value = value
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
     def plot_correlaton_matrix(self, mask_autocorrelations: bool = False, **kwargs):
-        """
+        """ Plots the cross-correlation matrix.
+
+            :param mask_autocorrelations:
+                If set to ``True``, the auto-correlation diagnoal
+                is hidden.
+                Default is ``False``.
+            :type mask_autocorrelations:
+                `bool`
+            
+            Several parameters, listed below, can be tuned to adapt the plot
+            to the user requirements:
+
+            .. rubric:: Data display keywords
+
+            :param decibel:
+                If set to ``True``, the data will be displayed in
+                a decibel scale (i.e., :math:`{\rm dB} = 10 \log_{10}({\rm data})`).
+                Default is ``True``.
+            :type decibel:
+                `bool`
+            :param vmin:
+                *Dynamic spectrum plot only*.
+                Minimal data value to display.
+            :type vmin:
+                `float`
+            :param vmax:
+                *Dynamic spectrum plot only*.
+                Maximal data value to display.
+            :type vmax:
+                `float`
+
+            .. rubric:: Plotting layout keywords
+
+            :param figname:
+                Name of the file (absolute or relative path) to save the figure.
+                Default is ``''`` (i.e., only show the figure).
+            :type figname:
+                `str`
+            :param figsize:
+                Set the figure size.
+                Default is ``(10, 10)``.
+            :type figsize:
+                `tuple`
+            :param title:
+                Set the figure title.
+                Default is ``''``.
+            :type title:
+                `str`
+            :param colorbar_label:
+                *Dynamic spectrum plot only*.
+                Label of the color bar.
+                Default is ``'Amp'`` if ``decibel=False`` and ``'dB'`` otherwise.
+            :type colorbar_label:
+                `str`
+            :param cmap:
+                *Dynamic spectrum plot only*.
+                Color map used to represent the data.
+                Default is ``'YlGnBu_r'``.
+            :type cmap:
+                `str`
+            
+            :Example:
+                .. code-block:: python
+
+                    from nenupy.io.xst import XST
+
+                    xst = XST("/path/to/XST.fits")
+                    data = xst.get....
+
         """
         max_ma_index = self.mini_arrays.max() + 1
         all_mas = np.arange(max_ma_index)
         matrix = np.full([max_ma_index, max_ma_index], np.nan, "complex")
         ma1, ma2 = np.tril_indices(self.mini_arrays.size, 0)
         for ma in all_mas:
             if ma not in self.mini_arrays:
@@ -135,14 +231,18 @@
             plt.show()
         plt.close("all")
 
 
     def rephase_visibilities(self, phase_center, uvw):
         """ """
 
+        log.info(
+            f"Rephasing the visibilities towards {phase_center}..."
+        )
+
         # Compute the zenith original phase center
         zenith = SkyCoord(
             np.zeros(self.time.size),
             np.ones(self.time.size)*90,
             unit="deg",
             frame=AltAz(
                 obstime=self.time,
@@ -210,15 +310,15 @@
 
 
     def make_image(self,
             resolution: u.Quantity = 1*u.deg,
             fov_radius: u.Quantity = 25*u.deg,
             phase_center: SkyCoord = None,
             stokes: str = "I"
-        ):
+        ) -> HpxSky:
         """
             :Example:
 
                 xst = XST("XST.fits")
                 data = xst.get_stokes("I")
                 sky = data.make_image(
                     resolution=0.5*u.deg,
@@ -234,21 +334,31 @@
         exposure = self.time[-1] - self.time[0]
 
         # Compute XST UVW coordinates (zenith phased)
         uvw = compute_uvw(
             interferometer=NenuFAR()[self.mini_arrays],
             phase_center=None, # will be zenith
             time=self.time,
-        )
+        ).to(u.m).value
 
         # Prepare visibilities rephasing
-        rephase_matrix, uvw = self.rephase_visibilities(
-            phase_center=phase_center,
-            uvw=uvw
-        )
+        if phase_center is None:
+            phase_center = SkyCoord(
+                0, 90, unit="deg",
+                frame=AltAz(
+                    obstime=self.time[0] + exposure/2,
+                    location=nenufar_position
+                )
+            ).transform_to("icrs")
+            rephase_matrix = 1.
+        else:
+            rephase_matrix, uvw = self.rephase_visibilities(
+                phase_center=phase_center,
+                uvw=uvw
+            )
 
         # Mask auto-correlations
         ma1, ma2 = np.tril_indices(self.mini_arrays.size, 0)
         cross_mask = ma1 != ma2
         uvw = uvw[:, cross_mask, :]
         # Transform to lambda units
         wvl = wavelength(self.frequency).to(u.m).value
@@ -262,26 +372,37 @@
             time=self.time[0] + exposure/2,
             frequency=np.mean(self.frequency),
             polarization=np.array([stokes]),
             value=np.nan
         )
 
         # Compute LMN coordinates
+        log.info(
+            "Preparing the sky..."
+        )
         image_mask = sky.visible_mask[0, 0, 0]
         image_mask *= sky.coordinates.separation(phase_center) <= fov_radius
         l, m, n = sky.compute_lmn(
             phase_center=phase_center,
             coordinate_mask=image_mask
         )
         lmn = np.array([l, m, (n - 1)], dtype=np.float32).T
+        n_pix = l.size
+        lmn = da.from_array(
+            lmn,
+            chunks=(np.floor(n_pix/os.cpu_count()), 3)
+        )
 
         # Transform to Dask array
+        n_bsl = uvw.shape[1]
+        n_freq = self.frequency.size
+        n_pix = l.size
         uvw = da.from_array(
             uvw.astype(np.float32),
-            chunks=np.floor(l.size/os.cpu_count())#( (1, 1,) + uvw.shape[2:])
+            chunks=(n_freq, max(1, np.floor(n_bsl/os.cpu_count())), 3)
         )
 
         # Compute the phase
         uvwlmn = np.sum(uvw[:, :, None, :] * lmn[None, None, :, :], axis=-1)
         phase = np.exp( -2j * np.pi * uvwlmn ) # (f, bsl, npix)
 
         # Rephase and average visibilites
@@ -316,15 +437,15 @@
             npix: int = 64,
             sources: list = []
         ):
         r""" Computes the Near-field image from the cross-correlation
             statistics data :math:`\mathcal{V}`.
 
             The distances between each Mini-Array :math:`{\rm MA}_i`
-            and the ground positions :math:`Delta` is:
+            and the ground positions :math:`\Delta` is:
 
             .. math::
                 d_{\rm{MA}_i} (x, y) = \sqrt{
                     ({\rm MA}_{i, x} - \Delta_x)^2 + ({\rm MA}_{i, y} - \Delta_y)^2 + \left( {\rm MA}_{i, z} - \sum_j \frac{{\rm MA}_{j, z}}{n_{\rm MA}} - 1 \right)^2
                 } 
 
             Then, the near-field image :math:`n_f` can be retrieved
@@ -364,21 +485,24 @@
             :type sources:
                 `list`
 
             :returns:
                 Tuple of near-field image and a dictionnary 
                 containing all source footprints. 
             :rtype:
-                `tuple`(:class:`~numpy.ndarray`, `dict`)
+                (:class:`~numpy.ndarray`, `dict`)
 
             :Example:
+                .. code-block:: python
+
+                    from nenupy.io.xst import XST
+
+                    xst = XST("xst_file.fits")
+                    nearfield, src_dict = xst.make_nearfield(sources=["Cas A", "Sun"])
 
-                from nenupy.io.xst import XST
-                xst = XST("xst_file.fits")
-                nearfield, src_dict = xst.make_nearfield(sources=["Cas A", "Sun"])
 
             .. versionadded:: 1.1.0
 
         """
 
         def compute_nearfield_imprint(visibilities, phase):
             # Phase and average in frequency
@@ -412,77 +536,123 @@
         ground_distances = np.sqrt(
             np.sum(
                 (ma_enu[:, None, None, :] - ground_grid[None])**2,
                 axis=-1
             )
         )
         grid_delays = ground_distances[ma1] - ground_distances[ma2] # (nvis, npix, npix)
-        grid_delays = da.from_array(grid_delays[cross_mask])
+        n_bsl = ma1[cross_mask].size
+        grid_delays = da.from_array(
+            grid_delays[cross_mask],
+            chunks=(max(1, np.floor(n_bsl/os.cpu_count())), npix, npix)
+        )
     
         # Mean in time the visibilities
         vis = np.mean(
             self.value,
             axis=0
         )[..., cross_mask] # (nfreqs, nvis)
-        vis = da.from_array(vis, chunks=self.frequency.size)
+        vis = da.from_array(
+            vis,
+            chunks=(1, max(1, np.floor(n_bsl/os.cpu_count())))#(self.frequency.size, np.floor(n_bsl/os.cpu_count()))
+        )
 
         # Make the nearfield image
+        log.info(
+            f"Computing nearfield (time: {self.time.size}, frequency: {self.frequency.size}, baselines: {vis.shape[1]}, pixels: {posx.size})... "
+        )
         wvl = wavelength(self.frequency).to(u.m).value
         phase = np.exp(2.j * np.pi * (grid_delays[None, ...]/wvl[:, None, None, None]))
         log.debug("Computing the phase term...")
         with ProgressBar() if log.getEffectiveLevel() <= logging.INFO else DummyCtMgr():
             phase = phase.compute()
+        log.debug("Computing the nearf-field...")
         nearfield = compute_nearfield_imprint(vis, phase)
 
         # Compute nearfield imprints for other sources
-        wvl = wavelength(self.frequency).to(u.m).value # (nfreqs,)
         simu_sources = {}
         for src_name in sources:
 
             # Check that the source is visible
-            try:
-                src = FixedTarget.from_name(name=src_name, time=obs_time)
-            except:
+            if src_name.lower() in ["sun", "moon", "venus", "mars", "jupiter", "saturn", "uranus", "neptune"]:
                 src = SolarSystemTarget.from_name(name=src_name, time=obs_time)
+            else:
+                src = FixedTarget.from_name(name=src_name, time=obs_time)
             altaz = src.horizontal_coordinates#[0]
             if altaz.alt.deg <= 10:
-                log.debug(f"{src_name}'s elevation {altaz.alt.deg}<=10deg, not considered for nearfield imprint.")
+                log.debug(f"{src_name}'s elevation {altaz[0].alt.deg}<=10deg, not considered for nearfield imprint.")
                 continue
 
             # Projection from AltAz to ENU vector
-            cos_az = np.cos(altaz.az.rad)
-            sin_az = np.sin(altaz.az.rad)
-            cos_el = np.cos(altaz.alt.rad)
-            sin_el = np.sin(altaz.alt.rad)
+            az_rad = altaz.az.rad
+            el_rad = altaz.alt.rad
+            cos_az = np.cos(az_rad)
+            sin_az = np.sin(az_rad)
+            cos_el = np.cos(el_rad)
+            sin_el = np.sin(el_rad)
             to_enu = np.array(
                 [cos_el*sin_az, cos_el*cos_az, sin_el]
             )
+            # src_delays = np.matmul(
+            #     ma_enu[ma1] - ma_enu[ma2],
+            #     to_enu
+            # )
+            # src_delays = da.from_array(
+            #     src_delays[cross_mask, :],
+            #     chunks=((np.floor(n_bsl/os.cpu_count()), npix, npix), 1)
+            # )
+            
+            ma1_enu = da.from_array(
+                ma_enu[ma1[cross_mask]],
+                chunks=max(1, np.floor(n_bsl/os.cpu_count()))
+            )
+            ma2_enu = da.from_array(
+                ma_enu[ma2[cross_mask]],
+                chunks=max(1, np.floor(n_bsl/os.cpu_count()))
+            )
             src_delays = np.matmul(
-                ma_enu[ma1] - ma_enu[ma2],
+                ma1_enu - ma2_enu,
                 to_enu
             )
-            src_delays = da.from_array(
-                src_delays[cross_mask, :]
-            )
 
             # Simulate visibilities
             src_vis = np.exp(2.j * np.pi * (src_delays/wvl))
             src_vis = np.swapaxes(src_vis, 1, 0)
+            log.debug(f"Computing the nearf-field imprint of {src_name}...")
             simu_sources[src_name] = compute_nearfield_imprint(src_vis, phase)
 
         return nearfield, simu_sources
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
 # ------------------------- Crosslet -------------------------- #
 # ============================================================= #
 class Crosslet(ABC):
-    """ """
+    """ Crosslet abstract class (both for XST and NenuFAR TV dat files).
+
+        .. rubric:: Attributes Summary
+
+        .. autosummary::
+
+            ~Crosslet.frequencies
+            ~Crosslet.mini_arrays
+
+        .. rubric:: Methods Summary
+
+        .. autosummary::
+
+            ~Crosslet.get
+            ~Crosslet.get_stokes
+            ~Crosslet.get_beamform
+
+        .. rubric:: Attributes and Methods Documentation
+
+    """
 
     # def __init__(self,
     #         mini_arrays: np.ndarray,
     #         frequency: u.Quantity,
     #         time: Time,
     #         visibilities: np.ndarray
     #     ):
@@ -494,75 +664,77 @@
     # --------------------------------------------------------- #
     # --------------------- Getter/Setter --------------------- #
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
     def get(self,
-            frequency_selection: str = None,
-            time_selection: str = None,
             polarization: str = "XX",
-        ):
-        """ """
-        # Polarization selection
-        allowed_polarizations = ["XX", "XY", "YX", "YY"]
-        if polarization not in allowed_polarizations:
-            raise ValueError(
-                f"'polarization' argument must be equal to one of the following: {allowed_polarizations}."
-            )
-
-        # Frequency selection
+            miniarray_selection: np.ndarray = None,
+            frequency_selection: str = None,
+            time_selection: str = None
+        ) -> XST_Slice:
+        """
+        """
+        mas = self._select_mini_arrays(miniarray_selection)
         frequency_mask = self._get_freq_mask(frequency_selection)
-
-        # Time selection
         time_mask = self._get_time_mask(time_selection)
 
-        ma1, ma2 = np.tril_indices(self.mini_arrays.size, 0)
-        auto_mask = ma1 == ma2
-        cross_mask = ~auto_mask
-
-        if polarization == "XY":
-            # Deal with lack of auto XY cross in XST-like data
-            yx = self.data[
-                np.ix_(
-                    time_mask,
-                    frequency_mask,
-                    self._get_cross_idx("Y", "X")
-                )
-            ]
-            _xy = np.zeros(
-                (list(yx.shape[:-1]) + [ma1.size]),
-                dtype=np.complex
+        return XST_Slice(
+            mini_arrays=mas,
+            time=self.time[time_mask],
+            frequency=self.frequencies[frequency_mask],
+            value=self._get(
+                frequency_selection=frequency_selection,
+                time_selection=time_selection,
+                polarization=polarization,
+                mini_arrays=mas
             )
-            _xy[:, :, auto_mask] = yx[:, :, auto_mask].conj()
-            # Get XY correlations
-            _xy[:, :, cross_mask] = self.data[
-                np.ix_(
-                    time_mask,
-                    frequency_mask,
-                    self._get_cross_idx("X", "Y")
-                )
-            ]
-            return _xy
-        else:
-            return self.data[
-                np.ix_(
-                    time_mask,
-                    frequency_mask,
-                    self._get_cross_idx(*list(polarization))
-                )
-            ]
+        )
 
 
     def get_stokes(self,
             stokes: str = "I",
+            miniarray_selection: np.ndarray = None,
             frequency_selection: str = None,
             time_selection: str = None
-        ):
-        """ """
+        ) -> XST_Slice:
+        r""" 
+             ``frequency_selection`` and ``time_selection``
+            arguments accept `str` values formatted as, e.g.,
+            ``'>={value}'`` or ``'>={value_1} & <{value_2}'`` or ``'=={value}'``.
+
+            :param frequency_selection:
+                Frequency selection. The expected ``'{value}'`` format is frequency units, e.g. ``'>=50MHz'`` or ``'< 1 GHz'``.
+                Default is ``None`` (i.e., no selection upon frequency).
+            :type frequency_selection:
+                `str`
+            :param time_selection:
+                Time selection. The expected ``'{value}'`` format is ISOT, e.g. ``'>=2022-01-01T12:00:00'``.
+                Default is ``None`` (i.e., no selection upon time).
+            :type time_selection:
+                `str`
+            :param stokes:
+                Stokes parameters to return
+            :type stokes:
+                `str`
+
+            .. math::
+
+                \begin{cases}
+                    \rm{I} = \frac{1}{2}(\rm{XX} + \rm{YY})\\
+                    \rm{Q} = \frac{1}{2}(\rm{XX} - \rm{YY})\\
+                    \rm{U} = \frac{1}{2}(\rm{XY} + \rm{YX})\\
+                    \rm{V} = \frac{-i}{2}(\rm{XY} - \rm{YX})\\
+                    \frac{\rm{L}}{\rm{I}} = \frac{\sqrt{\rm{Q}^2 + \rm{U}^2}}{\rm{I}}\\
+                    \frac{\rm{V}}{\rm{I}} = \frac{\rm{V}}{\rm{I}}\\
+                \end{cases}
+
+        """
+        mas = self._select_mini_arrays(miniarray_selection)
         frequency_mask = self._get_freq_mask(frequency_selection)
         time_mask = self._get_time_mask(time_selection)
 
         stokes_parameters = {
             "I": {
                 "cross": ["XX", "YY"],
                 "compute": lambda xx, yy: 0.5*(xx + yy)
@@ -589,40 +761,42 @@
             }
         }
 
         try:
             selected_stokes = stokes_parameters[stokes]
         except KeyError:
             log.warning(f"Available polarizations are: {stokes_parameters.keys()}.")
+            raise
 
         return XST_Slice(
-            mini_arrays=self.mini_arrays,
+            mini_arrays=mas,
             time=self.time[time_mask],
             frequency=self.frequencies[frequency_mask],
             value=selected_stokes["compute"](
                 *map(
-                    lambda pol: self.get(
+                    lambda pol: self._get(
                         frequency_selection=frequency_selection,
                         time_selection=time_selection,
-                        polarization=pol
+                        polarization=pol,
+                        mini_arrays=mas
                     ),
                     selected_stokes["cross"]
                 )
             )
         )
 
 
     def get_beamform(self,
             pointing: Pointing,
             frequency_selection: str = None,
             time_selection: str = None,
             mini_arrays: np.ndarray = np.array([0, 1]),
             polarization: str = "NW",
             calibration: str = "default"
-        ):
+        ) -> ST_Slice:
         """
             :Example:
 
                 from nenupy.io.bst import BST, XST
                 bst = BST("20191129_141900_BST.fits")
                 xst = XST("20191129_141900_XST.fits")
                 bf_cal = xst.get_beamform(
@@ -661,30 +835,30 @@
             cal = cal[np.ix_(
                 freq2sb(self.frequencies[frequency_mask]),
                 ma_real_indices,
                 pol_idx[polarization]
             )].squeeze(axis=2)
 
         # Load and filter the data
-        vis = self.get(
+        vis = self._get(
             frequency_selection=frequency_selection,
             time_selection=time_selection,
             polarization= "XX" if polarization.upper() == "NW" else "YY",
         )[:, :, mask]
 
         # Insert the data in a matrix
         tri_x, tri_y = np.tril_indices(ma_indices.size, 0)
         vis_matrix = np.zeros(
             (
                 self.time[time_mask].size,
                 self.frequencies[frequency_mask].size,
                 ma_indices.size,
                 ma_indices.size
             ),
-            dtype=np.complex
+            dtype=complex
         )
         vis_matrix[:, :, tri_x, tri_y] = vis
         vis_matrix[:, :, tri_y, tri_x] = vis_matrix[:, :, tri_x, tri_y].conj()
 
         # Calibrate the Xcorr with the caltable
         for fi in range(vis_matrix.shape[1]):
             cal_i = np.expand_dims(cal[fi], axis=1)
@@ -696,15 +870,15 @@
         phase = np.ones(
             (
                 self.time[time_mask].size,
                 self.frequencies[frequency_mask].size,
                 ma_indices.size,
                 ma_indices.size
             ),
-            dtype=np.complex
+            dtype=complex
         )
         altaz_pointing = pointing.horizontal_coordinates
         if altaz_pointing.size == 1:
             # Transit
             pass
         else:
             # Multiple pointings, get the correct value for all times
@@ -739,23 +913,34 @@
         wvl = wavelength(self.frequencies[frequency_mask]).to(u.m).value
         phase[:, :, tri_x, tri_y] = np.exp(
             -2.j*np.pi/wvl[None, :, None] * dphi[:, None, :]
         )
         phase[:, :, tri_y, tri_x] = phase[:, :, tri_x, tri_y].conj().copy()
         data = np.sum((vis_matrix * phase).real, axis=(2, 3))
 
-        return BST_Slice(
+        return ST_Slice(
             time=self.time[time_mask],
             frequency=self.frequencies[frequency_mask],
             value=data.squeeze()
         )
 
 
     # --------------------------------------------------------- #
     # ----------------------- Internal ------------------------ #
+    def _select_mini_arrays(self, mini_arrays):
+        """ """
+        if mini_arrays is None:
+            mini_arrays = self.mini_arrays
+        if np.any( ~np.isin(mini_arrays, self.mini_arrays) ):
+            raise IndexError(
+                f"Selected Mini-Arrays {mini_arrays} are outside possible values: {self.mini_arrays}."
+            )
+        return mini_arrays
+
+
     def _get_freq_mask(self, frequency_selection=None):
         """ """
         # Frequency selection
         frequencies = self.frequencies
         if frequency_selection is None:
             frequency_selection = f">={frequencies.min()} & <= {frequencies.max()}"
         frequency_mask = self._parse_frequency_condition(frequency_selection)(frequencies)
@@ -779,37 +964,154 @@
                 "Empty time selection, input values should fall "
                 f"between {self.time[0].isot} and {self.time[-1].isot}, "
                 f"i.e.: '>={self.time[0].isot} & <= {self.time[-1].isot}'"
             )
         return time_mask
 
 
-    def _get_cross_idx(self, c1='X', c2='X'):
+    def _get_cross_idx(self, c1="X", c2="X", mini_arrays=None):
         """ Retrieves visibilities indices for the given cross polarizations
         """
+
         mini_arrays_size = self.mini_arrays.size
-        corr = np.array(['X', 'Y']*mini_arrays_size)
+
+        # Mini-arrays selection
+        ma_indices = np.arange(mini_arrays_size, dtype="int")[np.isin(self.mini_arrays, mini_arrays)]
+
+        # Polarization array
+        corr = np.array(["X", "Y"]*mini_arrays_size)
         i_ant1, i_ant2 = np.tril_indices(mini_arrays_size*2, 0)
+        
+        # Define polarization and mini-arrays masks
         corr_mask = (corr[i_ant1] == c1) & (corr[i_ant2] == c2)
-        indices = np.arange(i_ant1.size)[corr_mask]
+        ma_mask = np.isin(i_ant1//2, ma_indices) & np.isin(i_ant2//2, ma_indices)
+
+        indices = np.arange(i_ant1.size)[corr_mask & ma_mask]
+
         return indices
+
+
+    def _get(self,
+            frequency_selection: str = None,
+            time_selection: str = None,
+            polarization: str = "XX",
+            mini_arrays: np.ndarray = None,
+        ) -> np.ndarray:
+        """ """
+        # Polarization selection
+        allowed_polarizations = ['XX', 'XY', 'YX', 'YY']
+        if polarization not in allowed_polarizations:
+            raise ValueError(
+                f"'polarization' argument must be one of the following: {allowed_polarizations}."
+            )
+
+        # Frequency selection
+        frequency_mask = self._get_freq_mask(frequency_selection)
+
+        # Time selection
+        time_mask = self._get_time_mask(time_selection)
+
+        # Combined mask
+        time_freq_mask = time_mask[:, None] * frequency_mask
+
+        # Final shape
+        if mini_arrays is None:
+            mini_arrays = self.mini_arrays
+        ma1, ma2 = np.tril_indices(mini_arrays.size, 0)
+        # final_shape = (np.sum(time_mask), np.sum(frequency_mask), ma1.size)
+        final_shape = (np.any(time_freq_mask, axis=1).sum(), np.any(time_freq_mask, axis=0).sum(), ma1.size)
+
+        if polarization == 'XY':
+            # Deal with lack of auto XY cross in XST-like data
+            auto_mask = ma1 == ma2
+            cross_mask = ~auto_mask
+            
+            data_tf_selected =  self.data[time_freq_mask]
+            # Deal with dimension cut in case of True over an entire axis
+            if final_shape[0] == 1:
+                data_tf_selected = np.expand_dims(data_tf_selected, axis=0)
+            if final_shape[1] == 1:
+                data_tf_selected = np.expand_dims(data_tf_selected, axis=1)
+
+            yx = data_tf_selected[
+                :,
+                :,
+                self._get_cross_idx('Y', 'X', mini_arrays)
+            ]
+
+            _xy = np.zeros(
+                (list(yx.shape[:-1]) + [ma1.size]),
+                dtype=complex
+            )
+            _xy[:, :, auto_mask] = yx[:, :, auto_mask].conj()
+
+            # Get XY correlations
+            _xy[:, :, cross_mask] = data_tf_selected[
+                :,
+                :,
+                self._get_cross_idx('X', 'Y', mini_arrays)
+            ]
+            return _xy.reshape(final_shape)
+        else:
+            return self.data[
+                time_freq_mask[:, :]
+            ][
+                :,
+                self._get_cross_idx(*list(polarization), mini_arrays)
+            ].reshape(final_shape)
+            # return self.data[
+            #     np.ix_(
+            #         time_mask,
+            #         frequency_mask,
+            #         self._get_cross_idx(*list(polarization), mini_arrays)
+            #     )
+            # ].reshape(final_shape)
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
 # ---------------------------- XST ---------------------------- #
 # ============================================================= #
 class XST(StatisticsData, Crosslet):
-    """ """
+    """ Crosslet STatistics reading class.
+
+        .. rubric:: Attributes Summary
+
+        .. autosummary::
+
+            ~XST.mini_arrays
+
+        .. rubric:: Methods Summary
+
+        .. autosummary::
+
+            ~Crosslet.get
+            ~Crosslet.get_stokes
+            ~Crosslet.get_beamform
+
+        .. rubric:: Attributes and Methods Documentation
+
+    """
 
     def __init__(self, file_name):
         super().__init__(file_name=file_name)
-        self.mini_arrays = self._meta_data['ins']['noMROn'][0]
 
+
+    # --------------------------------------------------------- #
+    # --------------------- Getter/Setter --------------------- #
+    @property
+    def mini_arrays(self):
+        """ Retrieves the list of Mini-Arrays used to get the cross-correlations.
+
+            :getter: Mini-Arrays list.
+
+            :type: :class:`~numpy.ndarray`
+        """
+        return self._meta_data['ins']['noMROn'][0]
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
 # ------------------------- TV_Image -------------------------- #
 # ============================================================= #
@@ -907,28 +1209,28 @@
                 map2write.size,
                 self.tv_image.nside,
                 file_name
             )
         )
 
 
-    def save_png(self, figname: str, beam_contours: bool = True, show_sources: bool = True):
+    def save_png(self, figname: str = "", beam_contours: bool = True, show_sources: bool = True, **kwargs):
         """ """
         image_center = altaz_to_radec(
             SkyCoord(
                 self.analog_pointing.az,
                 self.analog_pointing.alt,
                 frame=AltAz(
                     obstime=self.tv_image.time[0],
                     location=nenufar_position
                 )
             )
         )
 
-        kwargs = {}
+        #kwargs = {}
 
         if show_sources:
             src_names = []
             src_position = []
 
             with open(join(dirname(__file__), "nenufar_tv_sources.json")) as src_file:
                 sources = json.load(src_file)
@@ -940,15 +1242,16 @@
                     src_position.append(src.coordinates)
             for name in sources["SolarSystemSources"]:
                 src = SolarSystemTarget.from_name(name, time=self.tv_image.time[0])
                 if src.coordinates.separation(image_center) <= 0.8*self.fov_radius:
                     src_names.append(name)
                     src_position.append(src.coordinates)
 
-            kwargs["text"] = (SkyCoord(src_position), src_names, "white")
+            if len(src_position) != 0:
+                kwargs["text"] = (SkyCoord(src_position), src_names, "white")
 
         if beam_contours:
             # Simulate the array factor
             ma = MiniArray()
             af_sky = ma.array_factor(
                 sky=HpxSky(
                     resolution=0.2*u.deg,
@@ -969,15 +1272,14 @@
         self.tv_image[0, 0, 0].plot(
             center=image_center,
             radius=self.fov_radius - 2.5*u.deg,
             figname=figname,
             colorbar_label=f"Stokes {self.tv_image.polarization[0]}",
             **kwargs
         )
-        return
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
 # ----------------------- TV_Nearfield ------------------------ #
 # ============================================================= #
@@ -1302,30 +1604,54 @@
 # ============================================================= #
 
 
 # ============================================================= #
 # ------------------------- NenufarTV ------------------------- #
 # ============================================================= #
 class NenufarTV(StatisticsData, Crosslet):
-    """ """
+    """ Crosslet abstract class (both for XST and NenuFAR TV dat files).
+
+        .. rubric:: Attributes Summary
+
+        .. autosummary::
+
+            ~Crosslet.frequencies
+            ~Crosslet.mini_arrays
+
+        .. rubric:: Methods Summary
+
+        .. autosummary::
+
+            ~Crosslet.get
+            ~Crosslet.get_stokes
+            ~Crosslet.get_beamform
+
+        .. rubric:: Attributes and Methods Documentation
+
+    """
 
     def __init__(self, file_name):
         self.file_name = file_name
         self.mini_arrays = None
         self.time = None
         self.dt = None
         self.frequencies = None
         self.data = None
         self.load_tv_data()
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
     def compute_nenufar_tv(self, analog_pointing_file: str = None, **kwargs):
-        """ """
+        """
+            kwargs
+            fov_radius
+            resolution
+            stokes
+        """
 
         obs_time = self.time[0] + (self.time[-1] - self.time[0])/2
         fov_radius = kwargs.get("fov_radius", 27*u.deg)
         resolution = kwargs.get("resolution", 0.5*u.deg)
         stokes = kwargs.get("stokes", "I")
 
         if analog_pointing_file is None:
@@ -1355,14 +1681,19 @@
             analog_pointing=phase_center_altaz,
             fov_radius=fov_radius,
         )
 
 
     def compute_nearfield_tv(self, sources: list = [], **kwargs):
         """ 
+            kwargs
+                stokes
+                radius
+                npix
+
             :Example:
 
                 from nenupy.io.xst import NenufarTV
                 tv = NenufarTV("20191204_132113_nenufarTV.dat")
                 nf_object = tv.compute_nearfield_tv(
                     sources=["Cyg A", "Cas A", "Vir A", "Tau A", "Sun"],
                     npix=64
```

### Comparing `nenupy-2.1.0/nenupy/miscellaneous.py` & `nenupy-2.2.9/nenupy/miscellaneous.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/observation/__init__.py` & `nenupy-2.2.9/nenupy/observation/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,9 +9,9 @@
     for field in PARSET_OPTIONS:
         for key in PARSET_OPTIONS[field]:
             PARSET_OPTIONS[field][key]["modified"] = False
 
 # from .tapdatabase import ObsDatabase
 from .sqldatabase import ParsetDataBase
 from .parset import Parset, ParsetUser
-from .pointing_obs import *
+# from .pointing_obs import *
 from .obs_config import *
```

### Comparing `nenupy-2.1.0/nenupy/observation/obs_config.py` & `nenupy-2.2.9/nenupy/observation/obs_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,22 +346,22 @@
             'min': 1,
             'max': 4,
             'default': 4,
             'type': '`int`',
             'desc': 'Number of polarizations'
         },
         'timeRes': {
-            'min': (0.30*u.ms).to(u.s).value,
+            'min': (0.32*u.ms).to(u.s).value,
             'max': (83.89*u.ms).to(u.s).value,
             'default': (5.00*u.ms).to(u.s).value,
             'type': '`float` or :class:`~astropy.time.TimeDelta`',
             'desc': 'Time resolution in seconds'
         },
         'freqRes': {
-            'min': (0.10*u.kHz).to(u.Hz).value,
+            'min': (0.095*u.kHz).to(u.Hz).value,
             'max': (12.21*u.kHz).to(u.Hz).value,
             'default': (6.10*u.kHz).to(u.Hz).value,
             'type': '`float` or :class:`~astropy.units.Quantity`',
             'desc': 'Frequency resolution in Hz'
         },
         'nSubBands': {
             'min': 1,
@@ -739,30 +739,20 @@
     def _checkAttr(self, key, value, name):
         attrProp = backendProperties[self._backend][key]
         minVal = attrProp['min']
         maxVal = attrProp['max']
         defaultVal = attrProp['default']
         if value > maxVal:
             log.warning(
-                "Maximal value of {0} is {1}. Setting to default '{2}={3}'.".format(
-                    name,
-                    maxVal,
-                    key,
-                    defaultVal
-                )
+                f"Maximal value of {name} is {maxVal} (<{value}). Setting to default '{key}={defaultVal}'."
             )
             value = defaultVal
         elif value < minVal:
             log.warning(
-                "Minimal value for {0} is {1}. Setting to default '{2}={3}'.".format(
-                    name,
-                    minVal,
-                    key,
-                    defaultVal
-                )
+                f"Minimal value for {name} is {minVal} (>{value}). Setting to default '{key}={defaultVal}'."
             )
             value = defaultVal
         return value
 # ============================================================= #
 # ============================================================= #
 
 
@@ -1093,15 +1083,14 @@
     # --------------------------------------------------------- #
     # --------------------- Getter/Setter --------------------- #
     @property
     def volume(self):
         """
         """
         log.debug(str(self))
-        print(self.nPolars, self.freqRes, self.timeRes, self.nSubBands, self.durationSec)
         ratePerSB = self.nPolars * float32 * (200.e6/1024./self.freqRes) / self.timeRes
         rateObs = ratePerSB * self.nSubBands
         return (rateObs * self.durationSec).to(u.Gibyte)
 # ============================================================= #
 # ============================================================= #
```

### Comparing `nenupy-2.1.0/nenupy/observation/sqldatabase.py` & `nenupy-2.2.9/nenupy/observation/sqldatabase.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     Float,
     Boolean,
     DateTime,
     create_engine,
 )
 from sqlalchemy.orm import Session, sessionmaker, relationship
 
-from nenupy.instru_old import sb2freq
+from nenupy.instru import sb2freq
 from nenupy import nenufar_position
 
 import logging
 log = logging.getLogger(__name__)
 
 
 Base = declarative_base()
```

### Comparing `nenupy-2.1.0/nenupy/observation/tapdatabase.py` & `nenupy-2.2.9/nenupy/observation/tapdatabase.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/schedule/constraints.py` & `nenupy-2.2.9/nenupy/schedule/constraints.py`

 * *Files 10% similar despite different names*

```diff
@@ -153,26 +153,29 @@
 __all__ = [
     'Constraint',
     'TargetConstraint',
     'ScheduleConstraint',
     'ElevationCnst',
     'MeridianTransitCnst',
     'AzimuthCnst',
+    'LocalSiderealTimeCnst',
     'LocalTimeCnst',
     'TimeRangeCnst',
+    'NightTimeCnst',
     'Constraints'
 ]
 
 
-from abc import ABC, abstractmethod
+from abc import ABC
 import numpy as np
 from astropy.time import Time, TimeDelta
-from astropy.coordinates import Angle
+from astropy.coordinates import Angle, Longitude
 import pytz
 import matplotlib.pyplot as plt
+from copy import copy
 
 from nenupy.schedule.targets import _Target
 
 import logging
 log = logging.getLogger(__name__)
 
 
@@ -310,15 +313,15 @@
 # ============================================================= #
 
 
 # ============================================================= #
 # --------------------- TargetConstraint ---------------------- #
 # ============================================================= #
 class TargetConstraint(Constraint):
-    """ Base class for constraints involving target propertiy checks.
+    """ Base class for constraints involving target property checks.
 
         .. warning::
             :class:`~nenupy.schedule.constraints.TargetConstraint`
             should not be used on its own.
 
         .. versionadded:: 1.2.0
     """
@@ -506,14 +509,15 @@
         """
         self._is_target_instance(target)
 
         elevation = target.elevation.deg
         elevMean = (elevation[1:] + elevation[:-1])/2
         # elevMean[elevMean <= self.elevationMin.deg] = 0.
         elevMean[elevMean <= self.elevationMin.deg] = np.nan
+
         # if elevMax == 0.:
         if all(np.isnan(elevMean)):
             log.warning(
                 "Constraint <ElevationConstraint(elevationMin="
                 f"{self.elevationMin})> evaluated for target "
                 f"'{target.target}' cannot be satisfied over the "
                 "given time range."
@@ -521,14 +525,15 @@
             # self.score = elevation[1:]*0.
             self.score = elevation[1:]*np.nan
         elif not self.scale_elevation:
             self.score = elevMean/elevMean
         else:
             elevMax = np.nanmax(elevMean)
             self.score = elevMean/elevMax
+
         return self.score
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
 # -------------------- MeridianTransitCnst -------------------- #
@@ -678,14 +683,18 @@
             mask = (az >= azimuths[:-1]) &\
                 (az <= azimuths[1:])
 
         scores = np.zeros(mask.size)
         azIndices = np.where(mask)[0]
         # Set neighbor slots to non-zero to maximize centering
         slotShifts = np.arange(nslots) - int(np.floor(nslots/2))
+        if nslots%2 == 0:
+            # if nslots is even, we have to think which slot to include in addition to the max one.
+            # print(np.abs(azimuths[azIndices] - az))
+            pass
         neighborIdx = (azIndices[:, None] + slotShifts[None, :]).ravel()
         outOfBounds = (neighborIdx < 0) + (neighborIdx >= scores.size)
         neighborIdx = np.delete(
             neighborIdx,
             np.argwhere(outOfBounds)
         )
         scores = np.where(
@@ -703,14 +712,105 @@
         # self.score = mask.astype(float)
         return self.score
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
+# ------------------- LocalSiderealTimeCnst ------------------- #
+# ============================================================= #
+class LocalSiderealTimeCnst(TargetConstraint):
+
+    def __init__(self, lst: Longitude, strict_crossing: bool = True, weight: float = 1):
+        super().__init__(weight=weight)
+        self.lst = lst
+        self.strict_crossing = strict_crossing
+
+
+    # --------------------------------------------------------- #
+    # ------------------------ Methods ------------------------ #
+    def get_score(self, indices):
+        """
+        """
+        self._is_numpy_instance(indices)
+        return np.mean(self.score[indices], axis=-1)
+
+
+    # --------------------------------------------------------- #
+    # ----------------------- Internal ------------------------ #
+    def _evaluate(self, target, nslots):
+        """ time: dim + 1
+        """
+        self._is_target_instance(target)
+
+        pi_lon = Longitude(180, unit='deg')
+        lst_starts = copy(target._lst[:-1])
+        lst_stops = copy(target._lst[1:])
+        lst_desired = np.repeat(self.lst, lst_starts.size)
+
+        # Deal with crossing 360/0 case
+        tricky_mask = lst_starts > lst_stops
+        lst_starts[tricky_mask] = (lst_starts[tricky_mask] - pi_lon).wrap_at('360d')
+        lst_stops[tricky_mask] = (lst_stops[tricky_mask] - pi_lon).wrap_at('360d')
+        lst_desired[tricky_mask] = (lst_desired[tricky_mask] - pi_lon).wrap_at('360d')
+
+        mask = (lst_desired >= lst_starts) & (lst_desired <= lst_stops)
+
+        # Compute the score
+        scores = np.zeros(mask.size)
+        lst_crossing_indices = np.where(mask)[0]
+
+        if self.strict_crossing:
+            # Set neighbor slots to non-zero to maximize centering
+            slot_shifts = np.arange(nslots) - int(np.floor(nslots/2))
+            if nslots%2 == 0:
+                # if nslots is even, we have to think which slot to include in addition to the max one.
+                pass
+            neighbor_idx = (lst_crossing_indices[:, None] + slot_shifts[None, :]).ravel()
+            outOfBounds = (neighbor_idx < 0) + (neighbor_idx >= scores.size)
+            neighbor_idx = np.delete(
+                neighbor_idx,
+                np.argwhere(outOfBounds)
+            )
+            scores = np.where(
+                np.isin(
+                    np.arange(scores.size, dtype=int),
+                    neighbor_idx
+                ),
+                0.5,
+                scores
+            )
+
+            # Set azimuth found slots to maximal score
+            scores[lst_crossing_indices] = 1.
+        else:
+            # Number of consecutive false in the array
+            scores[lst_crossing_indices] = 1 
+            bool_array = ~scores.astype(bool)
+            consecutive_falses = np.diff(
+                np.where(
+                    np.concatenate(
+                        ([bool_array[0]],
+                        bool_array[:-1] != bool_array[1:],
+                        [True])
+                    )
+                )[0]
+            )[::2].max()
+            kernel_size = consecutive_falses + 1 if consecutive_falses%2==0 else consecutive_falses
+            kernel = np.arange(kernel_size) - int(np.floor(kernel_size/2))
+            kernel = 1. - np.abs(kernel)/kernel.max()
+            scores = np.convolve(scores, kernel, mode='same')
+
+        self.score = scores
+        # self.score = mask.astype(float)
+        return self.score
+# ============================================================= #
+# ============================================================= #
+
+# ============================================================= #
 # ----------------------- LocalTimeCnst ----------------------- #
 # ============================================================= #
 class LocalTimeCnst(ScheduleConstraint):
     """
         .. versionadded:: 1.2.0
     """
 
@@ -869,14 +969,63 @@
         self.score = np.where(score==0, np.nan, score)
         return self.score
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
+# ----------------------- NightTimeCnst ----------------------- #
+# ============================================================= #
+class NightTimeCnst(Constraint):
+    """ """
+
+    def __init__(self, sun_elevation_max=0., scale_elevation=True, weight=1):
+        super().__init__(weight=weight)
+        self.sun_elevation_max = sun_elevation_max
+        self.scale_elevation = scale_elevation
+
+
+    # --------------------------------------------------------- #
+    # ------------------------ Methods ------------------------ #
+    def get_score(self, indices):
+        """ """
+        return np.mean(
+            np.where(
+                self.score[indices]>0.,
+                1,
+                0
+            )
+        )
+
+
+    # --------------------------------------------------------- #
+    # ----------------------- Internal ------------------------ #
+    def _evaluate(self, sun_elevation):
+        """
+        """
+        sun_elevation[sun_elevation > self.sun_elevation_max] = np.nan
+
+        if all(np.isnan(sun_elevation)):
+            log.warning(
+                "Constraint <NightTimeCnst(sun_elevation_max="
+                f"{self.sun_elevation_max})> cannot be satisfied"
+                "over the given time range."
+            )
+            self.score = sun_elevation[1:]*np.nan
+        elif not self.scale_elevation:
+            self.score = sun_elevation/sun_elevation
+        else:
+            elevation_min = np.nanmin(sun_elevation)
+            self.score = sun_elevation/elevation_min
+        return self.score
+# ============================================================= #
+# ============================================================= #
+
+
+# ============================================================= #
 # ------------------------ Constraints ------------------------ #
 # ============================================================= #
 class Constraints(object):
     """
         .. versionadded:: 1.2.0
     """
 
@@ -962,24 +1111,26 @@
         """
         return np.array([cnt.weight for cnt in self])
     
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
-    def evaluate(self, target, time, nslots=1):
+    def evaluate(self, target, time, nslots=1, sun_elevation=None):
         """
         """
         cnts = np.zeros((self.size, time.size - 1))
         unEvaluatedCnst = 0
         for i, cnt in enumerate(self):
             if isinstance(cnt, TargetConstraint) and (target is not None):
                 cnts[i, :] = cnt(target, nslots)
             elif isinstance(cnt, ScheduleConstraint):
-                cnts[i, :] = cnt(time, nslots)
+                cnts[i, :] = cnt(tuple(time), nslots)
+            elif isinstance(cnt, NightTimeCnst):
+                cnts[i, :] = cnt(sun_elevation)
             else:
                 unEvaluatedCnst += 1
         if unEvaluatedCnst == self.size:
             cnts += 1.
             log.debug(
                 'No defined constraint could be used. Schedule '
                 'slot scores have been set to 1...'
```

### Comparing `nenupy-2.1.0/nenupy/schedule/contamination.py` & `nenupy-2.2.9/nenupy/schedule/contamination.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,26 +23,27 @@
 
 import logging
 log = logging.getLogger(__name__)
 
 import numpy as np
 from astropy.time import Time
 import astropy.units as u
+from astropy.io import fits
 from astropy.coordinates import SkyCoord
 from dask.diagnostics import ProgressBar
 from typing import List
 import matplotlib.pyplot as plt
 import matplotlib.dates as mdates
 
 from mocpy import MOC
 
 from nenupy import DummyCtMgr
 from nenupy.astro.pointing import Pointing
 from nenupy.astro.sky import HpxSky
-from nenupy.astro.astro_tools import SolarSystemSource, solar_system_source
+from nenupy.astro.astro_tools import SolarSystemSource, solar_system_source, local_sidereal_time
 from nenupy.instru import MiniArray, NenuFAR_Configuration
 
 
 # Mini-Array indices that present a different orientation.
 MA_INDICES = np.array([0, 1, 3, 7, 11, 13])
 MA_ROTATIONS = np.array([0, 30, 20, 50, 10, 40])
 
@@ -55,14 +56,37 @@
 
     def __init__(self, time: Time, frequency: u.Quantity, value: np.ndarray):
         self.time = time
         self.frequency = frequency
         self.value = value
 
 
+    def __add__(self, other):
+        """ Adds two SourceInLobes objects. """
+        same_frequencies = np.all(self.frequency.to(u.MHz) == other.frequency.to(u.MHz))
+        same_times = np.all(self.time.jd == other.time.jd)
+        if (not same_frequencies) or (not same_times):
+            raise Exception(
+                f"Addition of {SourceInLobes} objects with different time and/or frequency ranges."
+            )
+        return SourceInLobes(
+            time=self.time.copy(),
+            frequency=self.frequency.copy(),
+            value=self.value + other.value 
+        )
+
+
+    @property
+    def lst_time(self):
+        """ Returns the times associated with the SourceInLobe object in Local Sidereal Time."""
+        return local_sidereal_time(self.time)
+
+
+    # --------------------------------------------------------- #
+    # ------------------------ Methods ------------------------ #
     def plot(self, **kwargs):
         """ """
         fig = plt.figure(figsize=kwargs.get("figsize", (10, 6)))
 
         plt.pcolormesh(
             self.time.datetime,
             self.frequency.to(u.MHz).value,
@@ -96,29 +120,72 @@
                 bbox_inches="tight",
                 transparent=True
             )
             log.info(f"Figure '{figname}' saved.")
         else:
             plt.show()
         plt.close("all")
+
+
+    def export(self, filename: str):
+        """ Exports the time-frequency contamination array in FITS.
+            
+            :param filename:
+                FITS file name.
+            :type filename:
+                `str`
+        """
+        t_size, f_size = self.time.size, self.frequency.size
+        dtype = [
+            ('time_jd', 'f8', (t_size,)),
+            ('time_lst_deg', 'f8', (t_size,)),
+            ('frequency_mhz', 'f8'),
+            ('contamination', 'i8' if self.value.dtype==np.int32 else 'f8', (t_size,))
+        ]
+        data = np.zeros(f_size, dtype=dtype)
+        data["time_jd"] = self.time.jd
+        data["time_lst_deg"] = local_sidereal_time(self.time).deg
+        data["frequency_mhz"] = self.frequency.to(u.MHz).value
+        data["contamination"] = self.value
+        hdu = fits.BinTableHDU(data)
+        hdu.writeto(filename, overwrite=True)
+        log.info(
+            f"{SourceInLobes} object saved in {filename}."
+        )
+
+
+    @classmethod
+    def from_fits(cls, filename: str):
+        """ """
+        with fits.open(filename) as hdus:
+            time_jd = hdus[1].data["time_jd"][0, :]
+            frequency_mhz = hdus[1].data["frequency_mhz"]
+            values = hdus[1].data["contamination"]
+
+        return cls(
+            time=Time(time_jd, format="jd"),
+            frequency=frequency_mhz*u.MHz,
+            value=values
+        )
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
 # ------------------------- BeamLobes ------------------------- #
 # ============================================================= #
 class BeamLobes:
     """ """
 
     def __init__(self,
             time: Time,
             frequency: u.Quantity,
             pointing: Pointing,
-            miniarray_rotations: List[int] = None
+            miniarray_rotations: List[int] = None,
+            use_antenna_gain: bool = True
         ):
         self.time = time
         self.frequency = frequency
         self.pointing = pointing
         self.configuration=NenuFAR_Configuration(
             beamsquint_correction=False
         )
@@ -142,15 +209,15 @@
             f"(time steps: {self.sky.time.size}, "
             f"frequency steps: {self.sky.frequency.size}, "
             f"coordinates: {self.sky.coordinates.size})."
         )
 
         # Fill in the value attribute with the array factor
         # computed over the 6 different MA orientations.
-        self.sky.value = self._compute_array_factor()
+        self.sky.value = self._compute_array_factor(use_antenna_gain=use_antenna_gain)
         # self._array_factor = self._compute_array_factor()
         # self.sky.value = np.sum(self._array_factor, axis=0)
 
 
     # --------------------------------------------------------- #
     # --------------------- Getter/Setter --------------------- #
     @property
@@ -172,15 +239,48 @@
             mr = np.unique(np.array(mr)%60)
         self._miniarray_rotations = mr
 
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
-    def compute_moc(self, maximum_ratio: float = 0.5):
+    def compute_weight_moc(self, sources: List[str], cuts_number: int = 10) -> np.ndarray:
+        """ Compute moc with arrays of values between 0 and 1."""
+
+        # Get an array of sky positions (including all sources, all times)
+        sky_positions = self._get_skycoord_array(sources)
+
+        thresholds = np.linspace(0, 1, cuts_number + 1)
+
+        threshold_moc = np.zeros((cuts_number, self.frequency.size, self.time.size), dtype=bool)
+
+        for i, thr in enumerate(thresholds[1:]):
+
+            moc = self.compute_moc(maximum_ratio=thr, return_array=True)
+            
+            source_in_grating_lobes = np.zeros(moc.shape, dtype=int)
+            for f_idx in range(self.frequency.size):
+                for t_idx in range(self.time.size):
+                    source_in_grating_lobes[f_idx, t_idx] = np.sum(
+                        moc[f_idx, t_idx].contains(
+                            sky_positions[:, t_idx].ra,
+                            sky_positions[:, t_idx].dec
+                        )
+                    )
+            
+            threshold_moc[i, :, :] = source_in_grating_lobes.astype(bool)
+
+        return SourceInLobes(
+            time=self.time,
+            frequency=self.frequency,
+            value=np.sum(threshold_moc, axis=0)/cuts_number
+        )
+
+
+    def compute_moc(self, maximum_ratio: float = 0.5, return_array: bool = False):
         r"""
             Computes the MOC as sky patches where the array factor
             is above :math:`{\rm max}(\mathcal{F}_{\rm MA}) \times r`.
             :math:`\mathcal{F}_{\rm MA}` is the Mini-Array(s)
             array factor and :math:`r` is the ``maximum_ratio``.
         """
         # Number of Mini-Array that have been summed
@@ -201,15 +301,18 @@
             # Update the array in time
             mocs.append([
                 MOC.from_skycoords(
                     self.sky.coordinates[cells_in_lobes[1][cells_in_lobes[0]==t_idx]],
                     max_norder=5
                 ) for t_idx in range(self.time.size)
             ])
-    
+
+        if return_array:
+            return np.array(mocs)
+
         self.moc = np.array(mocs)
         log.debug("MOC computed (stored in '.moc' attribute).")
 
 
     def gsm_in_lobes(self, temperature_threshold: float = 15000) -> SourceInLobes:
         """ """
         from nenupy.astro.skymodel import HpxGSM
@@ -312,29 +415,33 @@
                 scatter=self._src_display["positions"][t_idx],
                 **kwargs
             )
 
 
     # --------------------------------------------------------- #
     # ----------------------- Internal ------------------------ #
-    def _compute_array_factor(self) -> np.ndarray:
+    def _compute_array_factor(self, use_antenna_gain: bool = True) -> np.ndarray:
         """ Computes the array factor, summed over the 6 different NenuFAR Mini-Array rotations. """
         # Mini-Array selection
         ma_mask = np.isin(MA_ROTATIONS, self.miniarray_rotations)
         af = 0
         # Compute the array factor for each Mini-Array
         for m in MA_INDICES[ma_mask]:
             ma = MiniArray(index=m)
             af += ma.array_factor(
                 sky=self.sky,
                 pointing=ma.analog_pointing(
                     self.pointing,
                     configuration=self.configuration
                 )#self.pointing
             )
+        
+        if use_antenna_gain:
+            af *= ma._antenna_gain(sky=self.sky, pointing=self.pointing)
+
         log.info("Computing the array factor...")
         with ProgressBar() if log.getEffectiveLevel() <= logging.INFO else DummyCtMgr():
             return af.compute()
 
 
     def _get_skycoord_array(self, sources: List[str]) -> SkyCoord:
         """ """
```

### Comparing `nenupy-2.1.0/nenupy/schedule/geneticalgo.py` & `nenupy-2.2.9/nenupy/schedule/geneticalgo.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/schedule/obsblocks.py` & `nenupy-2.2.9/nenupy/schedule/obsblocks.py`

 * *Files 10% similar despite different names*

```diff
@@ -43,75 +43,147 @@
         'name': 'Comissioning',
         'color': '#7DCEA0'
     },
     'es01': {
         'name': 'Cosmic Dawn',
         'color': '#825A2C'
     },
-    'es02':  {
+    'es02': {
         'name': 'Exoplanets and stars',
         'color': '#87794E'
     },
-    'es03':  {
+    'es03': {
         'name': 'Pulsars',
         'color': '#3F729C'
     },
-    'es04':  {
+    'es04': {
         'name': 'Transients',
         'color': '#8800CC'
     },
-    'es05':  {
+    'es05': {
         'name': 'Fast Radio Bursts',
         'color': '#00ABA9'
     },
-    'es06':  {
+    'es06': {
         'name': 'Planetary Lightning',
         'color': '#D80073'
     },
-    'es07':  {
+    'es07': {
         'name': 'Jupiter',
         'color': '#B8860B'
     },
-    'es08':  {
+    'es08': {
         'name': 'Galaxy clusters and AGNs',
         'color': '#0050EF'
     },
-    'es09':  {
+    'es09': {
         'name': 'Cluster filament and cosmic magnetism',
         'color': '#CC66FF'
     },
-    'es10':  {
+    'es10': {
         'name': 'Recombination Lines',
         'color': '#FA6800'
     },
-    'es11':  {
+    'es11': {
         'name': 'Sun',
         'color': '#008A00'
     },
-    'es12':  {
+    'es12': {
         'name': 'Radio Gamma',
         'color': '#A20025'
     },
-    'es13':  {
+    'es13': {
         'name': 'SETI',
         'color': '#F4A460'
     },
-    'es14':  {
+    'es14': {
         'name': 'Cas A',
         'color': '#517A7A'
     },
-    'es15':  {
+    'es15': {
         'name': 'Large Survey',
         'color': '#6699FF'
     },
-    'es16':  {
+    'es16': {
         'name': 'LOFAR-NenuFAR',
         'color': '#708D23'
     },
-    'es17':  {
+    'es17': {
+        'name': 'Radio-Amateurs',
+        'color': '#424242'
+    },
+    'lt00': {
+        'name': 'Comissioning',
+        'color': '#7DCEA0'
+    },
+    'lt01': {
+        'name': 'Cosmic Dawn',
+        'color': '#825A2C'
+    },
+    'lt02': {
+        'name': 'Exoplanets and stars',
+        'color': '#87794E'
+    },
+    'lt03': {
+        'name': 'Pulsars',
+        'color': '#3F729C'
+    },
+    'lt04': {
+        'name': 'Transients',
+        'color': '#8800CC'
+    },
+    'lt05': {
+        'name': 'Fast Radio Bursts',
+        'color': '#00ABA9'
+    },
+    'lt06': {
+        'name': 'Planetary Lightning',
+        'color': '#D80073'
+    },
+    'lt07': {
+        'name': 'Jupiter joint studies',
+        'color': '#B8860B'
+    },
+    'lt09': {
+        'name': 'Galaxies',
+        'color': '#CC66FF'
+    },
+    'lt10': {
+        'name': 'Recombination Lines',
+        'color': '#FA6800'
+    },
+    'lt11': {
+        'name': 'Sun',
+        'color': '#008A00'
+    },
+    'lt12': {
+        'name': 'Radio Gamma',
+        'color': '#A20025'
+    },
+    'lt13': {
+        'name': 'SETI',
+        'color': '#F4A460'
+    },
+    'rp1a': {
+        'name' : 'Faraday tomography of 3C196 field',
+        'color': '#000000' # TO BE DEFINED
+    },
+    'rp1b': {
+        'name': 'NenuFAR Low-Frequency Sky Survey',
+        'color': '#6699FF'
+    },
+    'rp1c': {
+        'name': 'Free-free absorption in Cassiopeia A',
+        'color': '#517A7A'
+    },
+    'sp16': {
+        'name': 'Student training',
+        'color': '#708D23'
+    },
+    'sp17': {
         'name': 'Radio-Amateurs',
         'color': '#424242'
     }
 }
 
 
 STATUS = {
@@ -129,15 +201,15 @@
 class Block(object):
     """
         .. versionadded:: 1.2.0
     """
 
     def __init__(self, *blocks):
         self._blocks = blocks
-        self._assignIndices()
+        self._assign_indices()
 
 
     def __len__(self):
         """
         """
         return len(self._blocks)
 
@@ -145,25 +217,25 @@
     def __mul__(self, n):
         """ Duplicates the :class:`~nenupy.schedule.obsblock.Block`
             ``n`` times.
         """
         blocks = []
         for block in self._blocks:
             for i in range(n):
-                copiedBlock = deepcopy(block)
+                copied_block = deepcopy(block)
                 try:
                     # Do not get a copy of the target attribute
                     # if it exists. Therefore any costly computation
                     # on target coordinates will not happen n times.
-                    copiedBlock.target = block.target
-                    copiedBlock.constraints = block.constraints
+                    copied_block.target = block.target
+                    copied_block.constraints = block.constraints
                 except AttributeError:
                     # Attribute target is not found for ReservedBlock
                     pass
-                blocks.append(copiedBlock)
+                blocks.append(copied_block)
         return Block(*blocks)
 
 
     def __add__(self, other):
         """
         """
         if not isinstance(other, Block):
@@ -172,14 +244,22 @@
                 'instances. Instead one instance is of type '
                 f'`{type(other)}`.'
             )
         blocks = self._blocks + other._blocks
         return Block(*blocks)
 
 
+    def __radd__(self, other):
+        if other == 0:
+            return self
+        else:
+            print(other)
+            return self.__add__(other)
+
+
     def __getitem__(self, n):
         """
         """
         return self._blocks[n]
 
 
     # --------------------------------------------------------- #
@@ -214,15 +294,15 @@
         """
         for block in self._blocks:
             block.constraints = None
 
 
     # --------------------------------------------------------- #
     # ----------------------- Internal ------------------------ #
-    def _assignIndices(self):
+    def _assign_indices(self):
         """
         """
         for i, block in enumerate(self._blocks):
             block.blockIdx = i
 # ============================================================= #
 # ============================================================= #
 
@@ -249,14 +329,20 @@
             The observing constraints to apply.
         :type constraints:
             :class:`~nenupy.schedule.constraints.Constraints`
         :param duration:
             The requested duration of the observation.
         :type duration:
             :class:`~astropy.time.TimeDelta`
+        :param processing_delay:
+            Time delay needed after the observation for the processing to take place.
+            Only :class:`~nenupy.schedule.obsblocks.ObsBlock`s with this parameter set are compared with each other while computing the scheduling.
+            This parameter particularly suits the imaging data.
+        :type processing_delay:
+            :class:`~astropy.time.TimeDelta`
 
         .. seealso::
             :ref:`observation_request_sec`
         
         .. rubric:: Attributes Summary
         
         .. autosummary::
@@ -268,21 +354,23 @@
         .. rubric:: Attributes and Methods Documentation
 
     """
 
     def __init__(
         self, name, program, target,
         constraints=None,
-        duration=TimeDelta(3600, format='sec')
+        duration=TimeDelta(3600, format='sec'),
+        processing_delay: TimeDelta = None
     ):
         self.name = name
         self.program = program
         self.target = target
         self.constraints = constraints
         self.duration = duration
+        self.processing_delay = processing_delay
 
         self.blockIdx = 0
         
         super().__init__(self)
 
 
     # --------------------------------------------------------- #
@@ -308,14 +396,17 @@
     def target(self, src):
         if src is None:
             pass
         elif not isinstance(src, _Target):
             raise TypeError(
                 f'`target` should be of type {_Target}.'
             )
+        elif src._lst is not None:
+            # Clear the target from previous computations
+            src.reset()
         self._target = src
 
 
     @property
     def constraints(self):
         """
         """
@@ -335,25 +426,23 @@
         return KPS[self.program]['color']
 
 
     @property
     def title(self):
         """
         """
-        _charLimit = 23
-        blkId = f'ID: {self.blockIdx}'
-        kpInfos = ' - '.join(
-            [
-                self.program.upper(),
-                KPS[self.program]['name']
-            ]
-        )
-        kpInfos = kpInfos[:_charLimit]
-        obsName = self.name[:_charLimit]
-        return f'{blkId}\n{kpInfos}\n{obsName}'
+        _char_limit = 23
+        block_id = f'ID: {self.blockIdx}'
+        kp_infos = ' - '.join([
+            self.program.upper(),
+            KPS[self.program]['name']
+        ])
+        kp_infos = kp_infos[:_char_limit]
+        obs_name = self.name[:_char_limit]
+        return f'{block_id}\n{kp_infos}\n{obs_name}'
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
     # @classmethod
     # def fromJson(self, jsonFile):
     #     """
@@ -839,14 +928,23 @@
     # @classmethod
     # def fromBookingFile(cls, fileName):
     #     """ Parse VCR booking.
     #     """
     #     blocks = []
     #     return cls()
 
+
+    def is_within(self, start: Time, stop: Time) -> bool:
+        """ """
+        return (self.time_min >= start)*(self.time_max < stop)\
+            + (self.time_min < start)*(self.time_max > start)*(self.time_max < stop)\
+            + (self.time_max > stop)*(self.time_min > start)*(self.time_min < stop)\
+            + (self.time_min < start)*(self.time_max > stop)
+
+
     # --------------------------------------------------------- #
     # ----------------------- Internal ------------------------ #
     def _display(self, ax):
         """
         """
         # Show the block rectangle
         ax.axvspan(
```

### Comparing `nenupy-2.1.0/nenupy/schedule/schedule.py` & `nenupy-2.2.9/nenupy/schedule/schedule.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,16 +25,17 @@
 from astropy.table import Table
 import numpy as np
 from copy import deepcopy, copy
 
 from nenupy.schedule.obsblocks import (
     Block,
     ObsBlock,
-    ReservedBlock
+    ReservedBlock,
 )
+from nenupy.schedule.targets import SSTarget
 from nenupy.schedule.geneticalgo import GeneticAlgorithm
 
 import logging
 log = logging.getLogger(__name__)
 
 
 # ============================================================= #
@@ -69,29 +70,35 @@
 class ScheduleBlock(ObsBlock):
     def __init__(self,
         name,
         program,
         target,
         constraints,
         duration,
-        dt
+        dt,
+        processing_delay
     ):
         super().__init__(
             name=name,
             program=program,
             target=target,
             constraints=constraints,
-            duration=duration
+            duration=duration,
+            processing_delay=processing_delay
         )
 
         self.dt = dt
         self.startIdx = None
         self.time_min = None
         self.time_max = None
         self.nSlots = int(np.ceil(self.duration/self.dt))
+        if self.processing_delay is None:
+            self.n_delay_slots = 0
+        else:
+            self.n_delay_slots = int(np.ceil(self.processing_delay/self.dt))
 
 
     def __del__(self):
         pass
 
 
     # --------------------------------------------------------- #
@@ -122,17 +129,20 @@
     def score(self):
         """
         """
         if self.indices is None:
             return 0.
         else:
             scores = []
+            weights = []
             for constraint in self.constraints:
                 scores.append(constraint.get_score(self.indices))
-            return np.nanmean(scores, axis=0)
+                weights.append(constraint.weight)
+            #return np.nanmean(scores, axis=0)
+            return np.average(scores, weights=weights, axis=0)
 
 
     @property
     def statusColor(self):
         """
         """
         if 0 <= self.score < 0.5:
@@ -144,36 +154,44 @@
         else:
             log.warning('Strange...')
             return STATUS['bad']
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
-    def evaluateScore(self, time):
+    def evaluate_score(self, time, sun_elevation):
         """
         """
         # Evaluate the target positions over time and compute the
         # score (product of each contraint score)
         # If it has already been evaluated do not do twice
         if (self.target is not None) and (self.target._lst is None):
             self.target.computePosition(time)
 
         if self.constraints.score is None:
             # Compute the weighted mean score for all constraints
             self.constraints.evaluate(
                 target=self.target,
                 time=time,
-                nslots=self.nSlots
+                nslots=self.nSlots,
+                sun_elevation=sun_elevation
             )
 
             log.debug(
                 f"<ObsBlock> #{self.blockIdx} named '{self.name}': "
                 "Constraint score evaluated."
             )
 
+    def is_within(self, start: Time, stop: Time) -> bool:
+        """ """
+        return (self.time_min >= start)*(self.time_max < stop)\
+            + (self.time_min < start)*(self.time_max > start)*(self.time_max < stop)\
+            + (self.time_max > stop)*(self.time_min > start)*(self.time_min < stop)\
+            + (self.time_min < start)*(self.time_max > stop)
+
 
     def plot(self, **kwargs):
         """
             kwargs
                 figsize
                 nPoints
                 figname
@@ -324,14 +342,15 @@
         .. versionadded:: 1.2.0
     """
 
     def __init__(self, dt):
         self.dt = dt
         self.blocks = []
         self._nSlots = []
+        self._n_delay_slots = []
         self._indices = []
         self._idxCounter = 0
 
 
     def __len__(self):
         """
         """
@@ -361,14 +380,21 @@
     @property
     def nSlots(self):
         """
         """
         return np.array(self._nSlots, dtype=int)
 
 
+    @property
+    def n_delay_slots(self):
+        """
+        """
+        return np.array(self._n_delay_slots, dtype=int)
+
+
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
     def insert(self, block):
         """
         """
         if not isinstance(block, (ObsBlock, Block)):
             raise TypeError(
@@ -378,19 +404,21 @@
         for blk in block:
             sb = ScheduleBlock(
                     name=blk.name,
                     program=blk.program,
                     target=blk.target,
                     constraints=blk.constraints,
                     duration=blk.duration,
-                    dt=self.dt 
+                    dt=self.dt,
+                    processing_delay=blk.processing_delay
                 )
             sb.blockIdx = self._idxCounter
             self.blocks.append(sb)
             self._nSlots.append(sb.nSlots)
+            self._n_delay_slots.append(sb.n_delay_slots)
             self._indices.append(0)
             self._idxCounter += 1
 # ============================================================= #
 # ============================================================= #
 
 
 # ============================================================= #
@@ -399,39 +427,41 @@
 class _TimeSlots(object):
     """
         .. versionadded:: 1.2.0
     """
 
     def __init__(
         self,
-        time_min, #tMin
-        time_max, #tMax,
+        time_min,
+        time_max,
         dt=TimeDelta(3600, format='sec')
     ):
         if not (_isTime(time_min, time_max) and _isTDelta(dt)):
             raise TypeError(
                 f'Wrong types in `_TimeSlots({type(time_min)}, '
                 f'{type(time_max)}, {type(dt)})`.'
             )
 
         self.dt = dt
         
         # Compute the time slots
-        self.starts, self.stops = self._computeTimeSlots(
+        self.starts, self.stops = self._compute_slots_time_range(
             time_min=time_min,
             time_max=time_max,
             dt=dt
         )
         self._startsJD = self.starts.jd
         self._stopsJD = self.stops.jd
 
         self.size = self.starts.size
 
         # Initialize array of free time slots
         self.freeSlots = np.ones(self.size, dtype=bool)
+        # Initialize array of free processing time slots
+        self.free_processing_slots = np.ones(self.size, dtype=bool)
         # Initialize array of slot indices
         self.idxSlots = np.arange(self.size, dtype=int)
         self._freeIndices = self.idxSlots
 
         log.debug(
             f'{self.__class__} instance created with '
             f'{self.size} time slots.'
@@ -477,25 +507,26 @@
     def dt(self, d):
         self._dt = d
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
     def time2idx(self, *time):
-        """
+        """ Converts times to schedule indices.
+            This method expects either one or two :class:`~astropy.time.Time` object(s).
         """
         if not _isTime(*time):
             raise TypeError(
                 f'<time2idx> expects a {Time} object.'
             )
 
         if len(time) == 1:
             # Find the unique corresponding slot index
-            mask = (self._startsJD <= time.jd) &\
-                (self._stopsJD > time.jd)
+            mask = (self._startsJD <= time[0].jd) &\
+                (self._stopsJD > time[0].jd)
         elif len(time) == 2:
             if time[1] < time[0]:
                 raise ValueError(
                     f'start>stop ({time[1].isot} < {time[0].isot})'
                     ' in <time2idx(start, stop)>.'
                 )
             # Find all indices within the time range
@@ -505,15 +536,15 @@
             raise Exception(
                 '<time2idx()> not properly called.'
             )
 
         return self.idxSlots[mask]
 
 
-    def addBooking(self, time_min, time_max):
+    def add_booking(self, time_min: Time, time_max: Time) -> None:
         """ Changes the status of the time slots comprised
             between ``time_min`` and ``time_max`` to 'booked' (i.e., not
             available anymore).
             In particular, the attribute 
             :attr:`~nenupy.schedule._TimeSlots.freeSlots` is set
             to ``False`` at the corresponding indices.
 
@@ -532,26 +563,26 @@
                 f"Booking on reserved slots from '{time_min.isot}' "
                 f"to '{time_max.isot}'."
             )
         self.freeSlots[indices] = False
         self._freeIndices = self.idxSlots[self.freeSlots]
 
 
-    def delBooking(self, time_min, time_max):
+    def remove_booking(self, time_min: Time, time_max: Time) -> None:
         """
         """
         indices = self.time2idx(time_min, time_max)
         self.freeSlots[indices] = True
         self._freeIndices = self.idxSlots[self.freeSlots]
 
 
     # --------------------------------------------------------- #
     # ----------------------- Internal ------------------------ #
     @staticmethod
-    def _computeTimeSlots(time_min, time_max, dt):
+    def _compute_slots_time_range(time_min: Time, time_max: Time, dt: TimeDelta):
         """
         """
         if time_max <= time_min:
             raise ValueError(
                 f'Schedule time_max={time_max.isot} <= '
                 f'time_min={time_min.isot}.'
             )
@@ -610,19 +641,22 @@
             ~Schedule.observation_blocks
             ~Schedule.reserved_blocks
 
         .. rubric:: Methods Summary
 
         .. autosummary::
 
+            ~Schedule.set_free_slots
+            ~Schedule.match_booking
             ~Schedule.insert
             ~Schedule.plot
+            ~Schedule.plot_range
             ~Schedule.book
             ~Schedule.export
-            
+
         .. rubric:: Attributes and Methods Documentation
 
     """
 
     def __init__(
         self,
         time_min,
@@ -635,14 +669,28 @@
             dt=dt
         )
 
         # self.observation_blocks = None
         self.observation_blocks = ScheduleBlocks(dt=self.dt)
         self.reserved_blocks = None
 
+        # Store the Sun's elevation
+        sun = SSTarget.fromName('Sun')
+        sun.computePosition(
+            Time(
+                np.append(
+                    self._startsJD,
+                    self._startsJD[-1] + self.dt.jd
+                ),
+                format='jd'
+            )
+        )
+        elevation = sun.elevation.deg
+        self.sun_elevation = (elevation[1:] + elevation[:-1])/2
+
 
     def __getitem__(self, n):
         """
         """
         return self.observation_blocks[n]
 
 
@@ -677,14 +725,19 @@
         """
         return self._reserved_blocks
     @reserved_blocks.setter
     def reserved_blocks(self, res):
         self._reserved_blocks = res
 
 
+    @property
+    def score(self) -> float:
+        """ Returns the current schedule score. """
+        return np.mean([block.score for block in self.observation_blocks])
+
     # @property
     # def scheduledBlocks(self):
     #     """
     #     """
     # list(map(schedule.observation_blocks.__getitem__, [i for i, blk in enumerate(schedule.observation_blocks) if blk.isBooked]))
     #     return self._scheduledBlocks
     
@@ -696,53 +749,159 @@
         
             :param \*blocks:
                 Observation blocks or reserved blocks.
             :type \*blocks:
                 :class:`~nenupy.schedule.obsblocks.Block`, :class:`~nenupy.schedule.obsblocks.ObsBlock` or :class:`~nenupy.schedule.obsblocks.ReservedBlock`
 
             :Example:
-                >>> from nenupy.schedule import Schedule, ESTarget, ObsBlock
-                >>> from astropy.time import Time, TimeDelta
-                >>> schedule = Schedule(
-                >>>     time_min=Time('2021-01-11 00:00:00'),
-                >>>     time_max=Time('2021-01-15 00:00:00'),
-                >>>     dt=TimeDelta(3600, format='sec')
-                >>> )
-                >>> cas_a = ObsBlock(
-                >>>     name="Cas A",
-                >>>     program="ES00",
-                >>>     target=ESTarget.fromName("Cas A"),
-                >>>     duration=TimeDelta(2*3600, format='sec'),
-                >>> )
-                >>> schedule.insert(cas_a)
+                .. code-block:: python
+
+                    from nenupy.schedule import Schedule, ESTarget, ObsBlock
+                    from astropy.time import Time, TimeDelta
+
+                    schedule = Schedule(
+                        time_min=Time('2021-01-11 00:00:00'),
+                        time_max=Time('2021-01-15 00:00:00'),
+                        dt=TimeDelta(3600, format='sec')
+                    )
+
+                    cas_a = ObsBlock(
+                        name="Cas A",
+                        program="ES00",
+                        target=ESTarget.fromName("Cas A"),
+                        duration=TimeDelta(2*3600, format='sec'),
+                    )
+
+                    schedule.insert(cas_a)
 
         """
         for blocks_i in blocks:
             # if not isinstance(blocks_i, Block):
             #     raise TypeError(
             #         f'Expected input of type {Block}>'
             #         f', got <{blocks_i.__class__}> instead.'
             #     )
             if all([blk.__class__ is ObsBlock for blk in blocks_i]):
                 self.observation_blocks.insert(blocks_i)
             elif all([blk.__class__ is ReservedBlock for blk in blocks_i]):
                 for blk in blocks_i:
-                    self.addBooking(blk.time_min, blk.time_max)
+                    self.add_booking(blk.time_min, blk.time_max)
+                    log.debug(f'ReservedBlock added from {blk.time_min.isot} to {blk.time_max.isot}.')
                 if self.reserved_blocks is None:
                     self.reserved_blocks = blocks_i
                 else:
                     self.reserved_blocks += blocks_i
             else:
                 raise Exception(
                     f'Not supposed to happen for type {blocks_i.__class__}!'
                 )
 
         self._toSchedule = np.ones(self.observation_blocks.size, dtype=bool)
 
 
+    def set_free_slots(self, start_times: Time, stop_times: Time) -> None:
+        """ Assign a :class:`~nenupy.schedule.obsblocks.ReservedBlock`
+            to every Schedule time interval that is not comprised bewteen
+            ``start_times`` and ``stop_times``.
+        """
+        if start_times.size != stop_times.size:
+            raise ValueError(
+                "start_times and stop_times should have the same length."
+            )
+        elif start_times.isscalar and stop_times.isscalar:
+            start_times = start_times.reshape((1,))
+            stop_times = stop_times.reshape((1,))
+        elif (start_times.ndim != 1) or (stop_times.ndim != 1):
+            raise ValueError(
+                f"start_times ({start_times.ndim}D) and "
+                f"stop_times ({stop_times.ndim}D) should be 1D."
+            )
+        # Treat the first booking
+        if start_times[0] > self.time_min:
+            self.insert(
+                ReservedBlock(
+                    time_min=self.time_min,
+                    time_max=start_times[0]
+                )
+            )
+        # Treat the rest
+        for blk_start, blk_stop in zip(stop_times[:-1], start_times[1:]):
+            self.insert(
+                ReservedBlock(
+                    time_min=blk_start,
+                    time_max=blk_stop
+                )
+            )
+        # Treat the last booking
+        if stop_times[-1] < self.time_max:
+            self.insert(
+                ReservedBlock(
+                    time_min=stop_times[-1],
+                    time_max=self.time_max
+                )
+            )
+
+
+    def match_booking(self, booking_file: str, key_program: str) -> None:
+        """ """
+        bookings = np.loadtxt(
+            booking_file,
+            skiprows=1,
+            delimiter=',',
+            dtype={
+                'names': ('start', 'stop', 'kp', 'comment'),
+                'formats': ('U19', 'U19', 'U4', 'U50')
+            }
+        )
+
+        # Check that the selected Key program is valid
+        kp_names = np.unique(bookings['kp'])
+        if key_program not in kp_names:
+            raise ValueError(
+                f'Key program {key_program} does not have any entry in {booking_file}, select a value in {kp_names}.'
+            )
+        valid_booking = bookings[bookings['kp'] == key_program]
+        booking_starts = Time(valid_booking['start'])
+        booking_stops = Time(valid_booking['stop'])
+
+        # Find each time period not in the valid booking range
+        within_schedule_mask = (booking_starts >= self.time_min)*(booking_stops <= self.time_max)\
+            + (booking_starts < self.time_min)*(booking_stops > self.time_min)\
+            + (booking_starts < self.time_max)*(booking_stops > self.time_max)
+        log.debug(f'{np.sum(within_schedule_mask)} bookings are within the schedule.')
+
+        # Insert corresponding reserved blocks in between the booking periods
+        starts = booking_starts[within_schedule_mask]
+        stops = booking_stops[within_schedule_mask]
+        # # Treat the first booking
+        # if starts[0] > self.time_min:
+        #     self.insert(
+        #         ReservedBlock(
+        #             time_min=self.time_min,
+        #             time_max=starts[0]
+        #         )
+        #     )
+        # for reserve_block_start, reserve_block_stop in zip(stops[:-1], starts[1:]):
+        #     self.insert(
+        #         ReservedBlock(
+        #             time_min=reserve_block_start,
+        #             time_max=reserve_block_stop
+        #         )
+        #     )
+        # # Treat the first booking
+        # if stops[-1] < self.time_max:
+        #     self.insert(
+        #         ReservedBlock(
+        #             time_min=stops[-1],
+        #             time_max=self.time_max
+        #         )
+        #     )
+        self.set_free_slots(start_times=starts, stop_times=stops)
+
+
     def book(self, optimize=False, **kwargs):
         r""" Distributes the :attr:`~nenupy.schedule.schedule.Schedule.observation_blocks` over the schedule time slots.
             The observing constraints are evaluated over the whole schedule.
 
             :param optimize:
                 If set to ``False`` an heuristic algorithm is used to perfom the booking.
                 However faster, this could result in sub-optimized time slots filling.
@@ -808,102 +967,247 @@
                 If ``optimize`` is set to ``False``, nothing is returned.
                 If ``optimize`` is set to ``True``, the :class:`~nenupy.schedule.geneticalgo.GeneticAlgorithm` instance is returned.
                 The method :class:`~nenupy.schedule.geneticalgo.GeneticAlgorithm.plot` can then be called to visualize the evolution of the solution populations.
             :rtype:
                 ``None`` or :class:`~nenupy.schedule.geneticalgo.GeneticAlgorithm`
 
         """
-        self._evaluateCnst(**kwargs)
+        # Ré-initialize the booking, in case the user calls this method several times
+        self._reset_observation_block_bookings()
 
-        nBlocksUnScheduled = 0
+        # Pre-compute the constraints scores
+        self._compute_block_constraint_scores(**kwargs)
 
+        n_unscheduled_blocks = 0
+
+        # Raise warning if the observation block are impossible to fit
         if sum(self._toSchedule) == 0:
             log.warning(
                 'Required observation blocks have constraints '
                 'unfitted for this schedule.'
             )
+            return
         else:
             log.info(
                 f'Fitting {sum(self._toSchedule)} observation blocks...'
             )
 
         if optimize:
             # All the observation blocks are booked at
-            # once with the genetic agorithm.
+            # once with the genetic algorithm.
             ga = GeneticAlgorithm(
                 populate=self._populate,
                 fitness=self._fitness,
                 mutation=self._mutation,
                 populationSize=kwargs.get('population_size', 20)
             )
 
+            # Find out the best observation schedule
             ga.evolve(
                 **kwargs
             )
 
+            # Book the observation_blocks on the schedule
             k = 0
             for i, blk in enumerate(self.observation_blocks):
                 if not self._toSchedule[i]:
+                    # The observation had a null score over the schedule
                     continue
-                bestStartIdx = ga.bestGenome[k]
-                bestStopIdx = bestStartIdx + blk.nSlots - 1
+                best_start_index = ga.bestGenome[k]
+                best_stop_index = best_start_index + blk.nSlots - 1
                 k += 1
-                if all(self._cnstScores[i, bestStartIdx:bestStopIdx + 1]==0):
-                    nBlocksUnScheduled += 1
+                if all(self._cnstScores[i, best_start_index:best_stop_index + 1] == 0):
+                    n_unscheduled_blocks += 1
                     log.warning(
                         f"<ObsBlock> #{blk.blockIdx} '{blk.name}' cannot be scheduled."
                     )
                     continue
-                blk.startIdx = bestStartIdx
-                blk.time_min = self.starts[bestStartIdx]
-                blk.time_max = self.stops[bestStartIdx + blk.nSlots-1]
+                blk.startIdx = best_start_index
+                blk.time_min = self.starts[best_start_index]
+                blk.time_max = self.stops[best_start_index + blk.nSlots-1]
+
+            score = self.fine_tune(max_it=kwargs.get("fine_tune_max_iterations", 1000))
+
+            # Remove blocks that are overlapping
+            # Lowest scores are removed in priority
+            scores = [blk.score for blk in self.observation_blocks]
+            for _, blk in sorted(zip(scores, self.observation_blocks), key=lambda pair: pair[0]):
+                if blk.startIdx is None: continue
+                start_idx = blk.startIdx
+                stop_idx = blk.startIdx + blk.nSlots
+                if not all(self.freeSlots[start_idx:stop_idx]):
+                    n_unscheduled_blocks += 1
+                    blk.startIdx = None # unbook the block
+                    log.warning(f"<ObsBlock> #{blk.blockIdx} is overlapping other blocks.")
+                    continue
+                self.freeSlots[start_idx:stop_idx] = False
 
             log.info(
-                f'{sum(self._toSchedule) - nBlocksUnScheduled}/'
+                f'{sum(self._toSchedule) - n_unscheduled_blocks}/'
                 f'{sum(self._toSchedule)} observation blocks scheduled '
                 f'({sum(~self._toSchedule)} impossible to fit).'
             )
 
             return ga
 
         else:
+            block_indices = np.arange(self.observation_blocks.size)
+            if kwargs.get('sort_by_difficulty', False):
+                sort_idx = np.argsort(np.sum(self._cnstScores, axis=1))
+                block_indices = block_indices[sort_idx]
+
             # Block are booked iteratively 
-            for i, blk in enumerate(self.observation_blocks):
-                if not self._toSchedule[i]:
+            # for i, blk in enumerate(self.observation_blocks):
+            for i in block_indices:
+                blk = self.observation_blocks[i]
+
+                if (not self._toSchedule[i]) or (blk.isBooked):
                     continue
                 # Construct a mask to avoid setting the obsblock where it cannot fit
-                freeSlotsShifted = self.freeSlots.copy()
-                for j in range(blk.nSlots):
-                    freeSlotsShifted *= np.roll(self.freeSlots, -j)
-                freeSlotsShifted[-blk.nSlots:] = self.freeSlots[-blk.nSlots:]
+                if blk.n_delay_slots != 0:
+                    freeSlotsShifted = self.freeSlots.copy() * self.free_processing_slots
+                else:
+                    freeSlotsShifted = self.freeSlots.copy()
+                
+                # for j in range(blk.nSlots):
+                #     freeSlotsShifted *= np.roll(self.freeSlots, -j)
+                # freeSlotsShifted[-blk.nSlots:] = self.freeSlots[-blk.nSlots:]
+                mask_idx = (np.where(~freeSlotsShifted)[0][:, None] - np.arange(blk.nSlots)[None, ::-1]).ravel()
+                mask_idx = np.unique(mask_idx)
+                mask_idx = mask_idx[mask_idx >= 0]
+                freeSlotsShifted[mask_idx] = False
+                
                 # Find the best spot
                 score = self._cnstScores[i, :] * self.freeSlots * freeSlotsShifted
                 if all(score==0):
-                    nBlocksUnScheduled += 1
+                    n_unscheduled_blocks += 1
                     log.warning(
                         f"<ObsBlock> #{i} '{blk.name}' cannot be scheduled."
                     )
                     continue
                 bestStartIdx = np.argmax(
                     score
                 )
                 # Assign a start and stop time to the block and update the free slots
                 blk.startIdx = bestStartIdx
                 bestStopIdx = bestStartIdx + blk.nSlots - 1
                 self.freeSlots[bestStartIdx:bestStopIdx + 1] = False
+                if blk.n_delay_slots != 0:
+                    # Update the processing reserved slots
+                    start_proc = bestStartIdx - blk.n_delay_slots
+                    start_proc = 0 if start_proc < 0 else start_proc
+                    stop_proc = bestStopIdx + blk.n_delay_slots + 1
+                    stop_proc = self.size if stop_proc > self.size else stop_proc
+                    self.free_processing_slots[start_proc:stop_proc] = False
+
                 blk.time_min = self.starts[bestStartIdx]
                 blk.time_max = self.stops[bestStopIdx]
 
             log.info(
-                f'{sum(self._toSchedule) - nBlocksUnScheduled}/'
+                f'{sum(self._toSchedule) - n_unscheduled_blocks}/'
                 f'{sum(self._toSchedule)} observation blocks scheduled '
                 f'({sum(~self._toSchedule)} impossible to fit).'
             )
 
 
+    def fine_tune(self, max_it: int = 1000) -> None:
+        """ 
+        """
+        log.info("(Fine tunning) Launching...")
+
+        scores = []
+
+        # Loop until the score drops
+        while len(scores) < max_it:
+            # Gather starting index and size of each schedule obsblock
+            start_indices = []
+            nslots = []
+            delay_nslots = []
+            indices = []
+            for block in self.observation_blocks:
+                if not block.isBooked:
+                    continue
+                start_indices.append(block.startIdx)
+                nslots.append(block.nSlots)
+                indices.append(block.blockIdx)
+                delay_nslots.append(block.n_delay_slots)
+
+            # Sort the by increasing index
+            start_indices_sorted = np.argsort(start_indices)
+            start_indices = np.array(start_indices, dtype=int)[start_indices_sorted]
+            nslots = np.array(nslots, dtype=int)[start_indices_sorted]
+            indices = np.array(indices, dtype=int)[start_indices_sorted]
+            delay_nslots = np.array(delay_nslots, dtype=int)[start_indices_sorted]
+
+            # Associate each observation blocks with its score before and after
+            max_scores = np.zeros((len(indices), 2)) # (number of booked blocks, score just before/score just after)
+            for i in range(start_indices_sorted.size):
+                block_index = indices[i]
+                block_score = self._cnstScores[block_index, start_indices[i]]
+                id1 = i - 1 # index of previous before
+                gap1 = np.arange(start_indices[id1] + nslots[id1] if id1 > 0 else 0, start_indices[i])
+                score1 = -1 if gap1.size == 0 else self._cnstScores[block_index, gap1[-1]] - block_score
+                id2 = i + 1 # index of next block
+                gap2 = np.arange(start_indices[i] + 1, start_indices[id2] - nslots[i] + 1 if id2 <= (len(indices) - 1) else self.size - 1)
+                score2 = -1 if gap2.size == 0 else self._cnstScores[block_index, gap2[0]] - block_score
+
+                if delay_nslots[i] != 0:
+                    # If this is requires a processing delay, we must check for the previous and next similar
+                    # observation, which may not be the very previous or very next.
+                    # Override immediate left/right slot if a similar observation is too close.
+                    delay_obs = np.argwhere(delay_nslots != 0)
+                    # Left
+                    prev_delay_idx = delay_obs[np.roll(delay_obs == i, -1)][0]
+                    if prev_delay_idx > i:
+                        # This is the first observation block with a delay constraint
+                        pass
+                    elif start_indices[prev_delay_idx] + nslots[prev_delay_idx] + delay_nslots[prev_delay_idx] >= start_indices[i]:
+                        score1 = -1
+                    # Right
+                    next_delay_idx = delay_obs[np.roll(delay_obs == i, +1)][0]
+                    if next_delay_idx < i:
+                        # This is the last observation block with delay constraint
+                        pass
+                    elif start_indices[i] + nslots[i] + delay_nslots[i] >= start_indices[next_delay_idx]:
+                        score2 = -1
+
+                # Score 'gradients'
+                max_scores[i, :] = np.array([
+                    score1,
+                    score2
+                ])
+
+            # Find out the maximal score difference
+            left_right_max = np.argmax(max_scores, axis=1)
+            max_score_diff = np.max(max_scores[np.arange(left_right_max.size), left_right_max])
+            max_score_block_idx = np.argmax(max_scores[np.arange(left_right_max.size), left_right_max])
+            if max_score_diff <= 0:
+                log.info("(Fine tunning) No positive gradient available. End of fine-tunning loop.")
+                break
+
+            # Shift the block 1dt left or right
+            block = self.observation_blocks[indices[max_score_block_idx]]
+            block.startIdx += -1 if left_right_max[max_score_block_idx] == 0 else 1
+            block.time_min = self.starts[block.startIdx]
+            block.time_max = self.stops[block.startIdx + block.nSlots - 1]
+
+            direction = 'left' if left_right_max[max_score_block_idx] == 0 else 'right'
+            log.debug(f'Shifting block #{indices[max_score_block_idx]} to the {direction}.')
+
+            # Compute the score
+            scores.append(self.score)
+
+        else:
+            log.info("(Fine tunning) Maximum number of iterations reached.")
+
+        log.info(f"(Fine tunning) End after {len(scores)} iterations.")
+
+        return scores
+
+
     def export(self, score_min=0):
         """ Exports the current schedule once :meth:`~nenupy.schedule.schedule.Schedule.book` has been called.
             Every observation with a ``score`` higher than ``score_min`` is included in the export.
 
             :param score_min:
                 Minimal :attr:`~nenupy.schedule.schedule.Schedule.obervation_blocks`'s score to be exported.
                 Default is ``0``.
@@ -946,27 +1250,120 @@
                 continue
             scores.append(score)
             names.append(blk.name)
             index.append(blk.blockIdx)
             starts.append(blk.time_min.isot)
             stops.append(blk.time_max.isot)
             programs.append(blk.program)
-        startArray = Time(starts, format='isot')
-        chron = np.argsort(startArray)
+        start_array = Time(starts, format='isot')
+        chron = np.argsort(start_array)
 
         tab = Table()
         tab['obsid'] = np.array(index, dtype=int)[chron]
         tab['name'] = np.array(names, dtype=str)[chron]
         tab['program'] = np.array(programs, dtype=str)[chron]
-        tab['start'] = startArray[chron]
+        tab['start'] = start_array[chron]
         tab['stop'] = Time(stops, format='isot')[chron]
         tab['score'] = np.array(scores)[chron]
 
         return tab
 
+    
+    def plot_range(self, start_time: Time, stop_time: Time, **kwargs) -> None:
+        """ Plots the current schedule.
+
+            .. rubric:: Data display keywords
+
+            :param start_time:
+                Minimal time to display.
+            :type start_time:
+                :class:`~astropy.time.Time`
+            :param stop_time:
+                Maximal time to display.
+            :type stop_time:
+                :class:`~astropy.time.Time`
+
+            .. rubric:: Plotting layout keywords
+
+            :param grid:
+                If set to ``True``, the time slots are separated by vertical lines.
+                Default is ``True``.
+            :type grid:
+                `bool`
+            :param figname:
+                Name of the file (absolute or relative path) to save the figure.
+                Default is ``''`` (i.e., only show the figure).
+            :type figname:
+                `str`
+            :param figsize:
+                Set the figure size.
+                Default is ``(15, 3)``.
+            :type figsize:
+                `tuple`
+
+        """
+        import matplotlib.pyplot as plt
+        import matplotlib.dates as mdates
+
+        # Initialize the figure
+        _, ax = plt.subplots(
+            figsize=kwargs.get("figsize", (15, 3))
+        )
+
+        # Display granularity
+        if kwargs.get("grid", True):
+            time_mask = (self._startsJD >= start_time.jd)*(self._stopsJD <= stop_time.jd)
+            for slot_start in self.starts[time_mask]:
+                ax.axvline(
+                    slot_start.datetime,
+                    color="gray",
+                    linestyle="-",
+                    linewidth=0.5
+                )
+
+        # Display unavailable slots
+        if self.reserved_blocks is not None:
+            for booked_block in self.reserved_blocks:
+                if not booked_block.is_within(start_time, stop_time):
+                    continue
+                booked_block._display(ax=ax)
+
+        # Display observation blocks
+        if self.observation_blocks is not None:
+            for obs_block in self.observation_blocks:
+                if not obs_block.isBooked:
+                    continue
+                if not obs_block.is_within(start_time, stop_time):
+                    continue
+                obs_block._display(ax=ax)
+
+        ax.set_xlim(
+                left=start_time.datetime,
+                right=stop_time.datetime
+            )
+
+        # Formating
+        ax.yaxis.set_visible(False)
+        h_fmt = mdates.DateFormatter("%y-%m-%d\n%H")
+        ax.xaxis.set_major_formatter(h_fmt)
+
+        # Save or show the figure
+        figname = kwargs.get("figname", "")
+        if figname != "":
+            plt.savefig(
+                figname,
+                dpi=300,
+                bbox_inches="tight",
+                transparent=True
+            )
+            log.info(f"Figure '{figname}' saved.")
+        else:
+            plt.show()
+        plt.close("all")
+
 
     def plot(self, days_per_line=1, **kwargs):
         """ Plots the current schedule.
 
             .. rubric:: Data display keywords
 
             :param days_per_line:
@@ -1003,21 +1400,21 @@
 
         # Find the number of sub-plots to display the schedule
         if not isinstance(days_per_line, TimeDelta):
             days_per_line = TimeDelta(
                 days_per_line,
                 format='jd'
             )
-        nSubPlots = int(np.ceil((time_max - time_min)/days_per_line))
+        n_subplots = int(np.ceil((time_max - time_min)/days_per_line))
 
         # Initialize the figure
         fig, axs = plt.subplots(
-            nrows=nSubPlots,
+            nrows=n_subplots,
             ncols=1,
-            figsize=kwargs.get('figsize', (15, 3*nSubPlots))
+            figsize=kwargs.get('figsize', (15, 3*n_subplots))
         )
 
         # Iterate over the sub-plots
         try:
             isIterable = iter(axs)
         except:
             axs = [axs]
@@ -1030,30 +1427,32 @@
                 right=tiMax.datetime
             )
 
             # Display granularity
             if kwargs.get('grid', True):
                 tMask = (self._startsJD >= tiMin.jd) *\
                     (self._stopsJD <= tiMax.jd)
-                for slotStart in self.starts[tMask]:
+                for slot_start in self.starts[tMask]:
                     ax.axvline(
-                        slotStart.datetime,
+                        slot_start.datetime,
                         color='gray',
                         linestyle='-',
                         linewidth=0.5
                     )
 
             # Display unavailable slots
             if self.reserved_blocks is not None:
                 for bookedBlock in self.reserved_blocks:
                     bookedBlock._display(ax=ax)
 
             # Display observation blocks
             if self.observation_blocks is not None:
                 for obsBlock in self.observation_blocks:
+                    if not obsBlock.isBooked:
+                        continue
                     obsBlock._display(ax=ax)
 
             # Formating
             ax.yaxis.set_visible(False)
             h_fmt = mdates.DateFormatter('%y-%m-%d\n%H')
             ax.xaxis.set_major_formatter(h_fmt)
 
@@ -1070,72 +1469,88 @@
         else:
             plt.show()
         plt.close('all')
 
 
     # --------------------------------------------------------- #
     # ----------------------- Internal ------------------------ #
-    def _evaluateCnst(self, **kwargs):
+    def _compute_block_constraint_scores(self, **kwargs):
         """
         """
         log.info(
             'Evaluating observation block constraints over '
             'the schedule...'
         )
         self._cnstScores = np.zeros(
             (self.observation_blocks.size, self.size)
         )
         self._maxScores = np.zeros(self.observation_blocks.size)
 
         # Compute the constraint score over the schedule if it
         # has not been previously been done
+        times = Time(
+            np.append(
+                self._startsJD,
+                self._startsJD[-1] + self.dt.jd
+            ),
+            format='jd'
+        )
         for i, blk in enumerate(self.observation_blocks):
             if blk.constraints.score is None:
                 # If != 1, the constraint score has already been computed
                 # Append the last time slot to get the last slot top
-                blk.evaluateScore(
-                    time=Time(
-                        np.append(
-                            self._startsJD,
-                            self._startsJD[-1] + self.dt.jd
-                        ),
-                        format='jd'
-                    )
-                )
+                blk.evaluate_score(time=times, sun_elevation=self.sun_elevation)
 
             # Set other attributes relying on the schedule
             blk.nSlots = int(np.ceil(blk.duration/self.dt))
 
             # Get the constraint and maximum possible score
-            slidingIdx = np.arange(blk.nSlots)[None, :] +\
+            sliding_indices = np.arange(blk.nSlots)[None, :] +\
                 np.arange(self.size - blk.nSlots)[:, None]
             self._cnstScores[i, :-blk.nSlots] = np.mean(
-                blk.constraints.score[slidingIdx],
+                blk.constraints.score[sliding_indices],
                 axis=1
             )
             # Set constraint score to zero if forbidden index
-            forbiddenMask = np.any(~self.freeSlots[slidingIdx], axis=1)
-            self._cnstScores[i, :-blk.nSlots][forbiddenMask] *= 0
+            forbidden_mask = np.any(~self.freeSlots[sliding_indices], axis=1)
+            self._cnstScores[i, :-blk.nSlots][forbidden_mask] *= 0
             self._maxScores[i] = np.max(self._cnstScores[i, :])
 
             # Check that the constraints are non zero
             if self._maxScores[i] == 0:
                 self._toSchedule[i] = False
-                log.info(
+                log.warning(
                     f"<ObsBlock> #{blk.blockIdx} '{blk.name}'"
                     " has a null score over the schedule."
                 )
 
         log.info(
             f'{self.observation_blocks.size} observation blocks have been '
             'successfully evaluated.'
         )        
 
 
-    def _bounds(self, indices):
+    def _reset_observation_block_bookings(self) -> None:
+        """ Loops through all observation_blocks,
+            if they are booked, set them as brand new and
+            release the corresponding schedule booking slots.
+        """
+        for block in self.observation_blocks:
+            if block.startIdx is None:
+                # The observation block has not been booked, skip
+                continue
+            # Free the schedule slots
+            self.freeSlots[block.startIdx:block.startIdx + block.nSlots] = True
+            if block.n_delay_slots != 0:
+                self.free_processing_slots[block.startIdx - block.n_delay_slots - 1: block.startIdx + block.nSlots + block.n_delay_slots] = True
+            # Reset the observation block as un-booked
+            block.startIdx = None
+
+
+    def _bound_to_schedule(self, indices: np.ndarray) -> np.ndarray:
         """
             startIndices = (schedule_size)
             
             return startIndices = (schedule_size)
         """
         indices[indices < 0] = 0
         beyond = (indices + self.observation_blocks.nSlots[self._toSchedule]) >= self.idxSlots.size
@@ -1151,82 +1566,120 @@
         #     randGen.integers(
         #         low=0,
         #         high=self.idxSlots.size,
         #         size=(n, self.observation_blocks.size),
         #         dtype=np.int64
         #     )
         # )
-        nBlocks = np.sum(self._toSchedule)
+        n_obs_blocks = np.sum(self._toSchedule)
         # population = np.zeros(
         #     (n, self.observation_blocks.size),
         #     dtype=int
         # )
         population = np.zeros(
-            (n, nBlocks),
+            (n, n_obs_blocks),
             dtype=int
         )
-        # for i in range(self.observation_blocks.size):
-        for i in range(nBlocks):
+        for i in range(n_obs_blocks):
             population[:, i] = randGen.choice(
                 np.where(self._cnstScores[self._toSchedule][i] != 0)[0],
                 # replace=False,
                 size=n,
             )
 
-        return self._bounds(population)
+        return self._bound_to_schedule(population)
 
 
     def _fitness(self, population):
         """
             population : np.array((children, genome))
         """
         # Evaluate the fitness of all the observation blocks over
-        # the cumulative (on nSlots) constraint scores and noormalize
+        # the cumulative (on nSlots) constraint scores and normalize
         # by the maximum available score within the schedule
+        genome_fitness = np.diagonal(
+            self._cnstScores[self._toSchedule].T[population],
+            axis1=1,
+            axis2=2
+        )/self._maxScores[self._toSchedule]
+        #has_zeros = np.any(genome_fitness==0., axis=1)
         fitness = np.mean(
-            np.diagonal(
-                self._cnstScores[self._toSchedule].T[population],
-                axis1=1,
-                axis2=2
-            )/self._maxScores[self._toSchedule],
+            genome_fitness,
             axis=1
         )
-        # Find out which inidicual in the population contains blocks
+        #fitness[has_zeros] = 0.
+        # Find out which individual in the population contains blocks
         # that overlaps with one another.
         # Sort the population block indices because we don't care
         # about the last one 
+        # sortedIdx = np.argsort(population)
+        # overlaps = np.any(
+        #     np.diff(
+        #         np.take_along_axis(
+        #             population,
+        #             sortedIdx,
+        #             axis=1
+        #         ),
+        #         axis=1
+        #     ) - self.observation_blocks.nSlots[self._toSchedule][sortedIdx][:, :-1] < 0,
+        #     axis=1
+        # )
+        # # The fitness is the product of the constraint score and
+        # # is set to 0 whenever there are overlapping blocks.
+        # return fitness * ~overlaps
+
+       
+        # Reduce the fitness if blocks with n_delay_slots != 0 overlap
+        are_delay_constrained = self.observation_blocks.n_delay_slots[self._toSchedule] > 0
+        population_delay = population[:, are_delay_constrained]
+        sorted_indices = np.argsort(population_delay)
+        delays = self.observation_blocks.n_delay_slots[self._toSchedule][sorted_indices][:, :-1]
+        nslots = self.observation_blocks.nSlots[self._toSchedule][sorted_indices][:, :-1]
+        overlaps_delay = np.sum(
+            np.diff(
+                np.take_along_axis(
+                    population_delay,
+                    sorted_indices,
+                    axis=1
+                ),
+                axis=1
+            ) - (delays + nslots) < 0,
+            axis=1
+        )        
+
+        # Reduce the fitness if observations temporally overlap
         sortedIdx = np.argsort(population)
-        overlaps = np.any(
+        overlaps = np.sum(
             np.diff(
                 np.take_along_axis(
                     population,
                     sortedIdx,
                     axis=1
                 ),
                 axis=1
             ) - self.observation_blocks.nSlots[self._toSchedule][sortedIdx][:, :-1] < 0,
             axis=1
         )
         # The fitness is the product of the constraint score and
-        # is set to 0 whenever there are overlapping blocks.
-        return fitness * ~overlaps
+        # is reduced whenever there are overlapping blocks.
+        return fitness/(overlaps + overlaps_delay + 1)
 
 
     def _mutation(self, genome):#, scaleOnFitness=False):
         """
         """
         idx = randGen.integers(
             low=0,
             high=genome.size
         )
         genome[idx] = randGen.integers(
             low=0,
             high=self.idxSlots.size
         )
-        return self._bounds(genome)
+        return self._bound_to_schedule(genome)
         # if scaleOnFitness:
         #     fitness = self._fitness(genome[None, :])[0]
         #     nMutations = int(np.ceil(genome.size * (1 - fitness)))
         #     idx = randGen.choice(
         #         np.arange(genome.size),
         #         replace=False,
         #         size=nMutations
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nenupy-2.1.0/nenupy/schedule/targets.py` & `nenupy-2.2.9/nenupy/schedule/targets.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,14 +114,23 @@
         if self._azimuth is None:
             self._attrWarning('azimuth')
         return self._azimuth
 
 
     # --------------------------------------------------------- #
     # ------------------------ Methods ------------------------ #
+    def reset(self) -> None:
+        """ Clear the Target instance from previous computations. """
+        self._lst = None
+        self._fk5 = None
+        self._hourAngle = None
+        self._elevation = None
+        self._azimuth = None
+
+
     def computePosition(self, time):
         """
         """
         if not isinstance(time, Time):
             raise TypeError(
                 f'<time> should be a {Time} object.'
             )
```

### Comparing `nenupy-2.1.0/nenupy/skymodel/hpxgsm.py` & `nenupy-2.2.9/nenupy/skymodel/hpxgsm.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/skymodel/hpxlofar.py` & `nenupy-2.2.9/nenupy/skymodel/hpxlofar.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/skymodel/lfsky.fits` & `nenupy-2.2.9/nenupy/skymodel/lfsky.fits`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/skymodel/pointsource.py` & `nenupy-2.2.9/nenupy/skymodel/pointsource.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/undysputed/bandpass_coeffs.dat` & `nenupy-2.2.9/nenupy/undysputed/bandpass_coeffs.dat`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy/undysputed/waveform.py` & `nenupy-2.2.9/nenupy/undysputed/waveform.py`

 * *Files identical despite different names*

### Comparing `nenupy-2.1.0/nenupy.egg-info/SOURCES.txt` & `nenupy-2.2.9/nenupy.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,88 @@
+LICENSE
 MANIFEST.in
 README.md
-setup.py
+pyproject.toml
+setup.cfg
+bin/nenupy_parallactic_correction
 bin/nenupy_vcr_coordinates
 nenupy/__init__.py
 nenupy/base.py
 nenupy/miscellaneous.py
 nenupy/telescopes.json
 nenupy.egg-info/PKG-INFO
 nenupy.egg-info/SOURCES.txt
 nenupy.egg-info/dependency_links.txt
-nenupy.egg-info/not-zip-safe
 nenupy.egg-info/requires.txt
 nenupy.egg-info/top_level.txt
 nenupy/astro/__init__.py
 nenupy/astro/astro_tools.py
+nenupy/astro/beam_correction.py
+nenupy/astro/common_sources.json
+nenupy/astro/jones_mueller.py
 nenupy/astro/pointing.py
 nenupy/astro/sky.py
 nenupy/astro/skymodel.py
 nenupy/astro/target.py
 nenupy/astro/uvw.py
-nenupy/astro_old/__init__.py
-nenupy/astro_old/astro.py
-nenupy/astro_old/hpxsky.py
-nenupy/astro_old/radio_sources.json
-nenupy/beam/__init__.py
-nenupy/beam/beam.py
-nenupy/beam/hpxbeam.py
 nenupy/beamlet/__init__.py
 nenupy/beamlet/beamlet.py
 nenupy/beamlet/bstdata.py
 nenupy/beamlet/sdata.py
 nenupy/beamlet/sstdata.py
 nenupy/instru/NenuFAR_Ant_Hpx.fits
 nenupy/instru/__init__.py
+nenupy/instru/cal_pz_2_multi_2019-02-23.dat
+nenupy/instru/cal_table_NDPPP-24sep2021-freq-all-MR6_V1_20220118.dat
+nenupy/instru/cal_table_NDPPP-24sep2021-freq-all-MR6_V1_20220120.dat
 nenupy/instru/instrument_tools.py
 nenupy/instru/interferometer.py
 nenupy/instru/low_noise_amplifier.json
 nenupy/instru/miniarray_antennas.json
+nenupy/instru/nda.py
 nenupy/instru/nenufar.py
 nenupy/instru/nenufar_array.json
 nenupy/instru/squint_table.sav
-nenupy/instru_old/__init__.py
-nenupy/instru_old/cal_pz_2_multi_2019-02-23.dat
-nenupy/instru_old/instru.py
-nenupy/instru_old/squint_table.sav
 nenupy/io/__init__.py
 nenupy/io/bst.py
 nenupy/io/io_tools.py
+nenupy/io/nenufar_tv_sources.json
+nenupy/io/sst.py
 nenupy/io/xst.py
 nenupy/observation/__init__.py
 nenupy/observation/obs_config.py
+nenupy/observation/obs_tools.py
 nenupy/observation/parset.py
 nenupy/observation/parset_user_options.json
-nenupy/observation/pointing_obs.py
 nenupy/observation/sqldatabase.py
 nenupy/observation/tapdatabase.py
 nenupy/schedule/__init__.py
 nenupy/schedule/constraints.py
 nenupy/schedule/contamination.py
 nenupy/schedule/geneticalgo.py
 nenupy/schedule/obsblocks.py
 nenupy/schedule/schedule.py
 nenupy/schedule/targets.py
-nenupy/simulation/__init__.py
-nenupy/simulation/hpxsimu.py
 nenupy/skymodel/__init__.py
 nenupy/skymodel/hpxgsm.py
 nenupy/skymodel/hpxlofar.py
 nenupy/skymodel/lfsky.fits
 nenupy/skymodel/pointsource.py
 nenupy/undysputed/__init__.py
 nenupy/undysputed/bandpass_coeffs.dat
 nenupy/undysputed/dynspec.py
-nenupy/undysputed/waveform.py
+nenupy/undysputed/waveform.py
+tests/test_astro_pointing.py
+tests/test_astro_sky.py
+tests/test_astro_skymodel.py
+tests/test_astro_target.py
+tests/test_astro_tools.py
+tests/test_database.py
+tests/test_instru.py
+tests/test_instru_miniarray.py
+tests/test_instru_nenufar.py
+tests/test_io_bst.py
+tests/test_io_xst.py
+tests/test_jones_mueller.py
+tests/test_obsconfig.py
+tests/test_schedule.py
+tests/test_sdata.py
```

