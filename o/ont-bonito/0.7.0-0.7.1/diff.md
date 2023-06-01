# Comparing `tmp/ont-bonito-0.7.0.tar.gz` & `tmp/ont-bonito-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ont-bonito-0.7.0.tar", last modified: Mon Apr  3 12:40:06 2023, max compression
+gzip compressed data, was "ont-bonito-0.7.1.tar", last modified: Thu Jun  1 13:10:26 2023, max compression
```

## Comparing `ont-bonito-0.7.0.tar` & `ont-bonito-0.7.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-04-03 12:40:06.654555 ont-bonito-0.7.0/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    14470 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/LICENCE.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      179 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/MANIFEST.in
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     5127 2023-04-03 12:40:06.652191 ont-bonito-0.7.0/PKG-INFO
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4821 2023-04-03 12:37:54.000000 ont-bonito-0.7.0/README.md
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-04-03 12:40:06.521507 ont-bonito-0.7.0/bonito/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      937 2023-04-02 12:07:46.000000 ont-bonito-0.7.0/bonito/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1550 2022-01-09 17:00:34.000000 ont-bonito-0.7.0/bonito/aligner.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-04-03 12:40:06.569299 ont-bonito-0.7.0/bonito/cli/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)        0 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/bonito/cli/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     7983 2023-04-01 22:07:04.000000 ont-bonito-0.7.0/bonito/cli/basecaller.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     5096 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/bonito/cli/convert.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4454 2023-04-03 09:41:00.000000 ont-bonito-0.7.0/bonito/cli/download.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    12570 2023-04-01 22:07:04.000000 ont-bonito-0.7.0/bonito/cli/duplex.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     3647 2022-02-13 12:34:47.000000 ont-bonito-0.7.0/bonito/cli/evaluate.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     6815 2023-04-01 22:07:04.000000 ont-bonito-0.7.0/bonito/cli/export.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4565 2023-04-01 22:07:04.000000 ont-bonito-0.7.0/bonito/cli/train.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      567 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/bonito/cli/view.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-04-03 12:40:06.582274 ont-bonito-0.7.0/bonito/crf/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/bonito/crf/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     2564 2023-01-05 13:16:22.000000 ont-bonito-0.7.0/bonito/crf/basecall.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     8944 2023-01-11 16:32:25.000000 ont-bonito-0.7.0/bonito/crf/model.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-04-03 12:40:06.597098 ont-bonito-0.7.0/bonito/ctc/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/bonito/ctc/__init__.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     2018 2022-02-13 12:34:47.000000 ont-bonito-0.7.0/bonito/ctc/basecall.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     7110 2022-11-17 14:06:33.000000 ont-bonito-0.7.0/bonito/ctc/model.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-04-03 12:40:06.602694 ont-bonito-0.7.0/bonito/data/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       95 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/bonito/data/README.md
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     2868 2023-04-01 22:07:04.000000 ont-bonito-0.7.0/bonito/data.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     6593 2023-04-01 22:07:04.000000 ont-bonito-0.7.0/bonito/fast5.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    19373 2023-04-03 09:38:52.000000 ont-bonito-0.7.0/bonito/io.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     3067 2022-06-11 12:11:56.000000 ont-bonito-0.7.0/bonito/mod_util.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-04-03 12:40:06.610322 ont-bonito-0.7.0/bonito/models/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      115 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/bonito/models/README.md
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-04-03 12:40:06.625270 ont-bonito-0.7.0/bonito/models/configs/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1206 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/bonito/models/configs/dna_r9.4.1@v1.toml
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1289 2021-10-27 17:31:47.000000 ont-bonito-0.7.0/bonito/models/configs/dna_r9.4.1@v2.toml
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      290 2021-10-27 17:31:48.000000 ont-bonito-0.7.0/bonito/models/configs/dna_r9.4.1@v3.toml
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     7948 2021-12-03 16:22:18.000000 ont-bonito-0.7.0/bonito/multiprocessing.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    11194 2023-01-27 13:44:25.000000 ont-bonito-0.7.0/bonito/nn.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4718 2023-04-01 22:07:04.000000 ont-bonito-0.7.0/bonito/pod5.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     4545 2023-04-01 22:07:04.000000 ont-bonito-0.7.0/bonito/reader.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     3330 2021-11-22 13:56:15.000000 ont-bonito-0.7.0/bonito/schedule.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     9608 2022-11-13 23:14:06.000000 ont-bonito-0.7.0/bonito/training.py
--rw-r--r--   0 cseymour  (5744) domain users  (1113)    13024 2023-01-05 13:16:22.000000 ont-bonito-0.7.0/bonito/util.py
-drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-04-03 12:40:06.647760 ont-bonito-0.7.0/ont_bonito.egg-info/
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     5127 2023-04-03 12:40:05.000000 ont-bonito-0.7.0/ont_bonito.egg-info/PKG-INFO
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      987 2023-04-03 12:40:05.000000 ont-bonito-0.7.0/ont_bonito.egg-info/SOURCES.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       39 2023-04-03 12:40:05.000000 ont-bonito-0.7.0/ont_bonito.egg-info/dependency_links.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       40 2023-04-03 12:40:05.000000 ont-bonito-0.7.0/ont_bonito.egg-info/entry_points.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      261 2023-04-03 12:40:05.000000 ont-bonito-0.7.0/ont_bonito.egg-info/requires.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)        7 2023-04-03 12:40:05.000000 ont-bonito-0.7.0/ont_bonito.egg-info/top_level.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)      304 2023-04-03 10:24:52.000000 ont-bonito-0.7.0/requirements.txt
--rw-r--r--   0 cseymour  (5744) domain users  (1113)       38 2023-04-03 12:40:06.655754 ont-bonito-0.7.0/setup.cfg
--rw-r--r--   0 cseymour  (5744) domain users  (1113)     1270 2022-09-05 12:28:38.000000 ont-bonito-0.7.0/setup.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.335109 ont-bonito-0.7.1/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    14470 2023-04-05 10:36:21.000000 ont-bonito-0.7.1/LICENCE.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      179 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/MANIFEST.in
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     5127 2023-06-01 13:10:26.331505 ont-bonito-0.7.1/PKG-INFO
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4821 2023-04-03 12:37:54.000000 ont-bonito-0.7.1/README.md
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.083858 ont-bonito-0.7.1/bonito/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      937 2023-06-01 12:51:57.000000 ont-bonito-0.7.1/bonito/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1550 2022-01-09 17:00:34.000000 ont-bonito-0.7.1/bonito/aligner.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.156103 ont-bonito-0.7.1/bonito/cli/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)        0 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/cli/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     7975 2023-05-31 13:55:48.000000 ont-bonito-0.7.1/bonito/cli/basecaller.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     5096 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/cli/convert.py
+-rwxr-xr-x   0 cseymour  (5744) domain users  (1113)     4773 2023-05-31 13:55:48.000000 ont-bonito-0.7.1/bonito/cli/download.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    12570 2023-04-01 22:07:04.000000 ont-bonito-0.7.1/bonito/cli/duplex.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     3647 2022-02-13 12:34:47.000000 ont-bonito-0.7.1/bonito/cli/evaluate.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     6815 2023-04-01 22:07:04.000000 ont-bonito-0.7.1/bonito/cli/export.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4704 2023-05-05 09:40:35.000000 ont-bonito-0.7.1/bonito/cli/train.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      567 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/cli/view.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.185212 ont-bonito-0.7.1/bonito/crf/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/crf/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     2627 2023-04-04 08:37:25.000000 ont-bonito-0.7.1/bonito/crf/basecall.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     8951 2023-04-13 14:08:39.000000 ont-bonito-0.7.1/bonito/crf/model.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.210045 ont-bonito-0.7.1/bonito/ctc/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       56 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/ctc/__init__.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     2018 2022-02-13 12:34:47.000000 ont-bonito-0.7.1/bonito/ctc/basecall.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     7110 2022-11-17 14:06:33.000000 ont-bonito-0.7.1/bonito/ctc/model.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.221146 ont-bonito-0.7.1/bonito/data/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       95 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/data/README.md
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     2868 2023-04-01 22:07:04.000000 ont-bonito-0.7.1/bonito/data.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     6672 2023-05-31 13:47:00.000000 ont-bonito-0.7.1/bonito/fast5.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    19373 2023-04-03 09:38:52.000000 ont-bonito-0.7.1/bonito/io.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     3067 2022-06-11 12:11:56.000000 ont-bonito-0.7.1/bonito/mod_util.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.232862 ont-bonito-0.7.1/bonito/models/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      115 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/models/README.md
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.264946 ont-bonito-0.7.1/bonito/models/configs/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1206 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/models/configs/dna_r9.4.1@v1.toml
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1289 2021-10-27 17:31:47.000000 ont-bonito-0.7.1/bonito/models/configs/dna_r9.4.1@v2.toml
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      290 2021-10-27 17:31:48.000000 ont-bonito-0.7.1/bonito/models/configs/dna_r9.4.1@v3.toml
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     7948 2021-12-03 16:22:18.000000 ont-bonito-0.7.1/bonito/multiprocessing.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    11194 2023-01-27 13:44:25.000000 ont-bonito-0.7.1/bonito/nn.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4718 2023-04-01 22:07:04.000000 ont-bonito-0.7.1/bonito/pod5.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     4550 2023-04-13 14:08:39.000000 ont-bonito-0.7.1/bonito/reader.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     3330 2021-11-22 13:56:15.000000 ont-bonito-0.7.1/bonito/schedule.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    10481 2023-04-13 14:08:39.000000 ont-bonito-0.7.1/bonito/training.py
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)    13024 2023-01-05 13:16:22.000000 ont-bonito-0.7.1/bonito/util.py
+drwxr-xr-x   0 cseymour  (5744) domain users  (1113)        0 2023-06-01 13:10:26.319405 ont-bonito-0.7.1/ont_bonito.egg-info/
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     5127 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/PKG-INFO
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      987 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/SOURCES.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       39 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/dependency_links.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       40 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/entry_points.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      261 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/requires.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)        7 2023-06-01 13:10:25.000000 ont-bonito-0.7.1/ont_bonito.egg-info/top_level.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)      304 2023-04-13 14:09:16.000000 ont-bonito-0.7.1/requirements.txt
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)       38 2023-06-01 13:10:26.338927 ont-bonito-0.7.1/setup.cfg
+-rw-r--r--   0 cseymour  (5744) domain users  (1113)     1270 2022-09-05 12:28:38.000000 ont-bonito-0.7.1/setup.py
```

### Comparing `ont-bonito-0.7.0/LICENCE.txt` & `ont-bonito-0.7.1/LICENCE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Oxford Nanopore Technologies, Ltd. Public License Version 1.0
+Oxford Nanopore Technologies, plc. Public License Version 1.0
 =============================================================
 
 1. Definitions
 --------------
 
 1.1. “Contributor”
     means each individual or legal entity that creates, contributes to
@@ -283,15 +283,15 @@
 shall not be used to construe this License against a Contributor.
 
 10. Versions of the License
 ---------------------------
 
 10.1. New Versions
 
-Oxford Nanopore Technologies, Ltd. is the license steward. Except as
+Oxford Nanopore Technologies, plc. is the license steward. Except as
 provided in Section 10.3, no one other than the license steward has the
 right to modify or publish new versions of this License. Each version
 will be given a distinguishing version number.
 
 10.2. Effect of New Versions
 
 You may distribute the Covered Software under the terms of the version
@@ -307,15 +307,15 @@
 any references to the name of the license steward (except to note that
 such modified license differs from this License).
 
 Exhibit A - Source Code Form License Notice
 -------------------------------------------
 
   This Source Code Form is subject to the terms of the Oxford Nanopore
-  Technologies, Ltd. Public License, v. 1.0.  Full licence can be found
+  Technologies, plc. Public License, v. 1.0.  Full licence can be found
   at
   https://github.com/nanoporetech/bonito/blob/master/LICENCE.txt
 
 If it is not possible or desirable to put the notice in a particular
 file, then You may include the notice in a location (such as a LICENSE
 file in a relevant directory) where a recipient would be likely to look
 for such a notice.
```

### Comparing `ont-bonito-0.7.0/PKG-INFO` & `ont-bonito-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ont-bonito
-Version: 0.7.0
+Version: 0.7.1
 Summary: UNKNOWN
 Home-page: https://github.com/nanoporetech/bonito
 Author: Oxford Nanopore Technologies, Ltd
 Author-email: support@nanoporetech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ont-bonito-0.7.0/README.md` & `ont-bonito-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/__init__.py` & `ont-bonito-0.7.1/bonito/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
 from bonito.cli import basecaller, train, evaluate, view, convert, download, export, duplex
 
 modules = [
     'basecaller', 'train', 'evaluate', 'view', 'convert', 'download', 'export', 'duplex'
 ]
 
-__version__ = '0.7.0'
+__version__ = '0.7.1'
 
 
 def main():
     parser = ArgumentParser(
         'bonito',
         formatter_class=ArgumentDefaultsHelpFormatter
     )
```

### Comparing `ont-bonito-0.7.0/bonito/aligner.py` & `ont-bonito-0.7.1/bonito/aligner.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/cli/basecaller.py` & `ont-bonito-0.7.1/bonito/cli/basecaller.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     elif args.reference and fmt.name == "fastq":
         sys.stderr.write(f"> warning: did you really want {fmt.aligned} {fmt.name}?\n")
     else:
         sys.stderr.write(f"> outputting {fmt.aligned} {fmt.name}\n")
 
     if args.model_directory in models and args.model_directory not in os.listdir(__models__):
         sys.stderr.write("> downloading model\n")
-        File(__models__, models[args.model_directory]).download()
+        File(__models__, args.model_directory).download()
 
     sys.stderr.write(f"> loading model {args.model_directory}\n")
     try:
         model = load_model(
             args.model_directory,
             args.device,
             weights=args.weights if args.weights > 0 else None,
```

### Comparing `ont-bonito-0.7.0/bonito/cli/convert.py` & `ont-bonito-0.7.1/bonito/cli/convert.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/cli/download.py` & `ont-bonito-0.7.1/bonito/cli/download.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,30 +23,35 @@
     """
     __url__ = "https://cdn.oxfordnanoportal.com/software/analysis/bonito/"
 
     def __init__(self, path, url_frag, force=False):
         self.path = path
         self.force = force
         self.filename = url_frag
-        self.url = os.path.join(self.__url__, "%s.zip" % url_frag)
+        if url_frag.endswith('.hdf5'):
+            self.url = os.path.join(self.__url__, url_frag)
+            self.fname = self.filename
+        else:
+            self.url = os.path.join(self.__url__, "%s.zip" % url_frag)
+            self.fname = "%s.zip" % self.filename
 
     def location(self, filename):
         return os.path.join(self.path, filename)
 
     def exists(self, filename):
         return os.path.exists(self.location(filename))
 
     def download(self):
         """
         Download the remote file
         """
         # create the requests for the file
         req = requests.get(self.url, stream=True)
         total = int(req.headers.get('content-length', 0))
-        fname = "%s.zip" % self.filename
+        fname = self.fname
 
         # skip download if local file is found
         if self.exists(fname.strip('.zip')) and not self.force:
             print("[skipping %s]" % fname, file=sys.stderr)
             return
 
         if self.exists(fname.strip('.zip')) and self.force:
@@ -74,14 +79,17 @@
                 self.location(fname),
                 self.location(fname).strip('.hdf5')
             ])
             convert(args)
 
 
 models = [
+    "dna_r10.4.1_e8.2_400bps_fast@v4.2.0",
+    "dna_r10.4.1_e8.2_400bps_hac@v4.2.0",
+    "dna_r10.4.1_e8.2_400bps_sup@v4.2.0",
 
     "dna_r10.4.1_e8.2_260bps_fast@v4.1.0",
     "dna_r10.4.1_e8.2_260bps_hac@v4.1.0",
     "dna_r10.4.1_e8.2_260bps_sup@v4.1.0",
 
     "dna_r10.4.1_e8.2_400bps_fast@v4.1.0",
     "dna_r10.4.1_e8.2_400bps_hac@v4.1.0",
```

### Comparing `ont-bonito-0.7.0/bonito/cli/duplex.py` & `ont-bonito-0.7.1/bonito/cli/duplex.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/cli/evaluate.py` & `ont-bonito-0.7.1/bonito/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/cli/export.py` & `ont-bonito-0.7.1/bonito/cli/export.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/cli/train.py` & `ont-bonito-0.7.1/bonito/cli/train.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,15 +87,16 @@
 
     trainer = Trainer(
         model, device, train_loader, valid_loader,
         use_amp=half_supported() and not args.no_amp,
         lr_scheduler_fn=lr_scheduler_fn,
         restore_optim=args.restore_optim,
         save_optim_every=args.save_optim_every,
-        grad_accum_split=args.grad_accum_split
+        grad_accum_split=args.grad_accum_split,
+        quantile_grad_clip=args.quantile_grad_clip
     )
 
     if (',' in args.lr):
         lr = [float(x) for x in args.lr.split(',')]
     else:
         lr = float(args.lr)
     trainer.fit(workdir, args.epochs, lr)
@@ -112,15 +113,16 @@
     parser.add_argument("--directory", type=Path)
     parser.add_argument("--device", default="cuda")
     parser.add_argument("--lr", default='2e-3')
     parser.add_argument("--seed", default=25, type=int)
     parser.add_argument("--epochs", default=5, type=int)
     parser.add_argument("--batch", default=64, type=int)
     parser.add_argument("--chunks", default=0, type=int)
-    parser.add_argument("--valid-chunks", default=0, type=int)
+    parser.add_argument("--valid-chunks", default=None, type=int)
     parser.add_argument("--no-amp", action="store_true", default=False)
     parser.add_argument("-f", "--force", action="store_true", default=False)
     parser.add_argument("--restore-optim", action="store_true", default=False)
     parser.add_argument("--nondeterministic", action="store_true", default=False)
     parser.add_argument("--save-optim-every", default=10, type=int)
     parser.add_argument("--grad-accum-split", default=1, type=int)
+    parser.add_argument("--quantile-grad-clip", action="store_true", default=False)
     return parser
```

### Comparing `ont-bonito-0.7.0/bonito/cli/view.py` & `ont-bonito-0.7.1/bonito/cli/view.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/crf/basecall.py` & `ont-bonito-0.7.1/bonito/crf/basecall.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,18 +30,19 @@
     """
     with torch.inference_mode():
         device = next(model.parameters()).device
         dtype = torch.float16 if half_supported() else torch.float32
         scores = model(batch.to(dtype).to(device))
         if reverse:
             scores = model.seqdist.reverse_complement(scores)
-        sequence, qstring, moves = beam_search(
-            scores, beam_width=beam_width, beam_cut=beam_cut,
-            scale=scale, offset=offset, blank_score=blank_score
-        )
+        with torch.cuda.device(scores.device):
+            sequence, qstring, moves = beam_search(
+                scores, beam_width=beam_width, beam_cut=beam_cut,
+                scale=scale, offset=offset, blank_score=blank_score
+            )
         return {
             'moves': moves,
             'qstring': qstring,
             'sequence': sequence,
         }
```

### Comparing `ont-bonito-0.7.0/bonito/crf/model.py` & `ont-bonito-0.7.1/bonito/crf/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,15 +170,15 @@
         self.alphabet = seqdist.alphabet
         if n_pre_post_context_bases is None:
             self.n_pre_context_bases = self.seqdist.state_len - 1
             self.n_post_context_bases = 1
         else:
             self.n_pre_context_bases, self.n_post_context_bases = n_pre_post_context_bases
 
-    def forward(self, x):
+    def forward(self, x, *args):
         return self.encoder(x)
 
     def decode_batch(self, x):
         scores = self.seqdist.posteriors(x.to(torch.float32)) + 1e-8
         tracebacks = self.seqdist.viterbi(scores.log()).to(torch.int16).T
         return [self.seqdist.path_to_str(x) for x in tracebacks.cpu().numpy()]
```

### Comparing `ont-bonito-0.7.0/bonito/ctc/basecall.py` & `ont-bonito-0.7.1/bonito/ctc/basecall.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/ctc/model.py` & `ont-bonito-0.7.1/bonito/ctc/model.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/data.py` & `ont-bonito-0.7.1/bonito/data.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/fast5.py` & `ont-bonito-0.7.1/bonito/fast5.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,18 @@
         self.filename = filename.name
         self.run_id = read.get_run_id()
         if type(self.run_id) in (bytes, np.bytes_):
             self.run_id = self.run_id.decode('ascii')
 
         tracking_id = read.handle[read.global_key + 'tracking_id'].attrs
 
-        self.sample_id = tracking_id['sample_id']
+        try:
+            self.sample_id = tracking_id['sample_id']
+        except KeyError:
+            self.sample_id = 'unset'
         if type(self.sample_id) in (bytes, np.bytes_):
             self.sample_id = self.sample_id.decode()
 
         self.exp_start_time = tracking_id['exp_start_time']
         if type(self.exp_start_time) in (bytes, np.bytes_):
             self.exp_start_time = self.exp_start_time.decode('ascii')
         self.exp_start_time = self.exp_start_time.replace('Z', '')
```

### Comparing `ont-bonito-0.7.0/bonito/io.py` & `ont-bonito-0.7.1/bonito/io.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/mod_util.py` & `ont-bonito-0.7.1/bonito/mod_util.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/models/configs/dna_r9.4.1@v1.toml` & `ont-bonito-0.7.1/bonito/models/configs/dna_r9.4.1@v1.toml`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/models/configs/dna_r9.4.1@v2.toml` & `ont-bonito-0.7.1/bonito/models/configs/dna_r9.4.1@v2.toml`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/multiprocessing.py` & `ont-bonito-0.7.1/bonito/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/nn.py` & `ont-bonito-0.7.1/bonito/nn.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/pod5.py` & `ont-bonito-0.7.1/bonito/pod5.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/reader.py` & `ont-bonito-0.7.1/bonito/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -132,15 +132,15 @@
             if end >= min(max_samples, len(signal)) or end / len(signal) > max_trim:
                 return min_trim
             return end
 
     return min_trim
 
 
-def normalisation(sig, norm_params):
+def normalisation(sig, norm_params=None):
     """
     Calculate signal shift and scale factors for normalisation..
     """
     if norm_params is None:
         norm_params = __default_norm_params__
     qa, qb = np.quantile(sig, [norm_params['quantile_a'], norm_params['quantile_b']])
     shift = max(10, norm_params['shift_multiplier'] * (qa + qb))
```

### Comparing `ont-bonito-0.7.0/bonito/schedule.py` & `ont-bonito-0.7.1/bonito/schedule.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/bonito/training.py` & `ont-bonito-0.7.1/bonito/training.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Bonito train
 """
 
+import math
 import os
 import re
 from glob import glob
 from functools import partial
 from time import perf_counter
 from collections import OrderedDict
 from datetime import datetime
@@ -65,55 +66,81 @@
         epoch = weight_no
     else:
         epoch = 0
 
     return epoch
 
 
+class ClipGrad:
+    def __init__(self, quantile=0.5, factor=2.0, buffer_size=100):
+        self.buffer = np.full(buffer_size, fill_value=1e6)
+        self.quantile = quantile
+        self.factor = factor
+        self.i = 0
+
+    def append(self, grad_norm):
+        self.buffer[self.i] = grad_norm
+        self.i = (self.i + 1) % len(self.buffer)
+
+    def __call__(self, parameters):
+        max_norm = self.factor * np.quantile(self.buffer, self.quantile)
+        grad_norm = torch.nn.utils.clip_grad_norm_(parameters, max_norm=max_norm).item()
+        if not math.isnan(grad_norm):
+            self.append(grad_norm)
+        return grad_norm
+
+
 class Trainer:
     def __init__(
         self, model, device, train_loader, valid_loader, criterion=None,
         use_amp=True, lr_scheduler_fn=None, restore_optim=False,
-        save_optim_every=10, grad_accum_split=1
+        save_optim_every=10, grad_accum_split=1, quantile_grad_clip=False
     ):
         self.model = model.to(device)
         self.device = device
         self.train_loader = train_loader
         self.valid_loader = valid_loader
         self.criterion = criterion or model.loss
         self.use_amp = use_amp
         self.lr_scheduler_fn = lr_scheduler_fn or linear_warmup_cosine_decay()
         self.restore_optim = restore_optim
         self.save_optim_every = save_optim_every
         self.grad_accum_split = grad_accum_split
         self.scaler = torch.cuda.amp.GradScaler(enabled=use_amp)
         self.optimizer = None
+        if quantile_grad_clip:
+            self.clip_grad = ClipGrad()
+        else:
+            self.clip_grad = lambda parameters: torch.nn.utils.clip_grad_norm_(parameters, max_norm=2.0).item()
 
     def train_one_step(self, batch):
         self.optimizer.zero_grad()
 
         losses = None
         with amp.autocast(enabled=self.use_amp):
-            for data_, targets_, lengths_ in zip(*map(lambda t: t.chunk(self.grad_accum_split, dim=0), batch)):
-                data_, targets_, lengths_ = data_.to(self.device), targets_.to(self.device), lengths_.to(self.device)
-                scores_ = self.model(data_)
+            for batch_ in zip(
+                *map(lambda t: t.chunk(self.grad_accum_split, dim=0), batch)
+            ):
+                data_, targets_, lengths_, *args = (x.to(self.device) for x in batch_)
+
+                scores_ = self.model(data_, *args)
                 losses_ = self.criterion(scores_, targets_, lengths_)
 
                 if not isinstance(losses_, dict): losses_ = {'loss': losses_}
 
                 total_loss = losses_.get('total_loss', losses_['loss']) / self.grad_accum_split
                 self.scaler.scale(total_loss).backward()
 
                 losses = {
                     k: ((v.item() / self.grad_accum_split) if losses is None else (v.item() / self.grad_accum_split) + losses[k])
                     for k, v in losses_.items()
                 }
 
         self.scaler.unscale_(self.optimizer)
-        grad_norm = torch.nn.utils.clip_grad_norm_(self.model.parameters(), max_norm=2.0).item()
+        grad_norm = self.clip_grad(self.model.parameters())
         self.scaler.step(self.optimizer)
         self.scaler.update()
 
         return losses, grad_norm
 
     def train_one_epoch(self, loss_log, lr_scheduler):
         t0 = perf_counter()
@@ -152,17 +179,16 @@
                     })
 
                 if lr_scheduler is not None: lr_scheduler.step()
 
         return smoothed_loss, perf_counter() - t0
 
     def validate_one_step(self, batch):
-        data, targets, lengths = batch
-
-        scores = self.model(data.to(self.device))
+        data, targets, lengths, *args = batch
+        scores = self.model(data.to(self.device), *(x.to(self.device) for x in args))
         losses = self.criterion(scores, targets.to(self.device), lengths.to(self.device))
         losses = {k: v.item() for k, v in losses.items()} if isinstance(losses, dict) else losses.item()
         if hasattr(self.model, 'decode_batch'):
             seqs = self.model.decode_batch(scores)
         else:
             seqs = [self.model.decode(x) for x in permute(scores, 'TNC', 'NTC')]
         refs = [decode_ref(target, self.model.alphabet) for target in targets]
```

### Comparing `ont-bonito-0.7.0/bonito/util.py` & `ont-bonito-0.7.1/bonito/util.py`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/ont_bonito.egg-info/PKG-INFO` & `ont-bonito-0.7.1/ont_bonito.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ont-bonito
-Version: 0.7.0
+Version: 0.7.1
 Summary: UNKNOWN
 Home-page: https://github.com/nanoporetech/bonito
 Author: Oxford Nanopore Technologies, Ltd
 Author-email: support@nanoporetech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ont-bonito-0.7.0/ont_bonito.egg-info/SOURCES.txt` & `ont-bonito-0.7.1/ont_bonito.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ont-bonito-0.7.0/setup.py` & `ont-bonito-0.7.1/setup.py`

 * *Files identical despite different names*

