# Comparing `tmp/interva-0.0.4.tar.gz` & `tmp/interva-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "interva-0.0.4.tar", last modified: Tue Mar 14 00:44:21 2023, max compression
+gzip compressed data, was "interva-0.0.5.tar", last modified: Thu Jun  1 14:44:20 2023, max compression
```

## Comparing `interva-0.0.4.tar` & `interva-0.0.5.tar`

### file list

```diff
@@ -1,99 +1,102 @@
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.505934 interva-0.0.4/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    35149 2022-07-29 15:44:16.000000 interva-0.0.4/LICENSE
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      114 2022-07-29 16:28:38.000000 interva-0.0.4/MANIFEST.in
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4213 2023-03-14 00:44:21.505470 interva-0.0.4/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3462 2023-03-13 22:54:59.000000 interva-0.0.4/README.md
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.432516 interva-0.0.4/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.439467 interva-0.0.4/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.432877 interva-0.0.4/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.438514 interva-0.0.4/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.433254 interva-0.0.4/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.437737 interva-0.0.4/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.433575 interva-0.0.4/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.436696 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.433889 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.435837 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.434231 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.434896 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.450792 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.452520 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.454432 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.456991 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.457870 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.460703 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.463520 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.464837 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.467332 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.469462 interva-0.0.4/build/lib/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.470595 interva-0.0.4/build/lib/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.4/build/lib/build/lib/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.472542 interva-0.0.4/build/lib/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.4/build/lib/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.4/build/lib/build/lib/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.475297 interva-0.0.4/build/lib/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.476927 interva-0.0.4/build/lib/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.4/build/lib/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.479296 interva-0.0.4/build/lib/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.4/build/lib/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.4/build/lib/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.482099 interva-0.0.4/build/lib/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.4/build/lib/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.483432 interva-0.0.4/build/lib/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.4/build/lib/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.485510 interva-0.0.4/build/lib/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.4/build/lib/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.4/build/lib/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.4/build/lib/tests/test_interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.487414 interva-0.0.4/interva/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.4/interva/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-13 22:16:04.000000 interva-0.0.4/interva/__version__.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.496160 interva-0.0.4/interva/data/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.4/interva/data/causetext.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   459264 2022-07-29 17:06:50.000000 interva-0.0.4/interva/data/probbase.xls
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   164661 2022-07-29 16:52:08.000000 interva-0.0.4/interva/data/probbaseV5_19.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088   286521 2022-11-03 17:23:26.000000 interva-0.0.4/interva/data/randomva5.csv
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    37287 2023-03-13 23:50:57.000000 interva-0.0.4/interva/interva5.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.504320 interva-0.0.4/interva.egg-info/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     4213 2023-03-14 00:44:21.000000 interva-0.0.4/interva.egg-info/PKG-INFO
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     3100 2023-03-14 00:44:21.000000 interva-0.0.4/interva.egg-info/SOURCES.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        1 2023-03-14 00:44:21.000000 interva-0.0.4/interva.egg-info/dependency_links.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       26 2023-03-14 00:44:21.000000 interva-0.0.4/interva.egg-info/requires.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       25 2023-03-14 00:44:21.000000 interva-0.0.4/interva.egg-info/top_level.txt
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       87 2022-07-29 15:51:31.000000 interva-0.0.4/pyproject.toml
--rw-r--r--   0 thomas.3912 (1583608718) 444659088       38 2023-03-14 00:44:21.506072 interva-0.0.4/setup.cfg
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     1367 2023-03-13 22:54:59.000000 interva-0.0.4/setup.py
-drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-03-14 00:44:21.501031 interva-0.0.4/tests/
--rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.4/tests/__init__.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088     2186 2023-03-13 23:42:11.000000 interva-0.0.4/tests/test_compare_r.py
--rw-r--r--   0 thomas.3912 (1583608718) 444659088    10728 2023-03-13 23:16:48.000000 interva-0.0.4/tests/test_interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.746485 interva-0.0.5/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    35149 2022-07-29 15:44:16.000000 interva-0.0.5/LICENSE
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      114 2022-07-29 16:28:38.000000 interva-0.0.5/MANIFEST.in
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4213 2023-06-01 14:44:20.746164 interva-0.0.5/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3462 2023-03-13 22:54:59.000000 interva-0.0.5/README.md
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.688978 interva-0.0.5/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.694603 interva-0.0.5/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.689223 interva-0.0.5/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.693873 interva-0.0.5/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.689473 interva-0.0.5/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.693293 interva-0.0.5/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.689719 interva-0.0.5/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.692689 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.689969 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.691881 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.690393 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.691169 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.700483 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.701522 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.703277 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.705399 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.706148 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.707967 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.709855 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.710948 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.712441 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.714404 interva-0.0.5/build/lib/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.715061 interva-0.0.5/build/lib/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/build/lib/build/lib/interva/interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.717046 interva-0.0.5/build/lib/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/build/lib/build/lib/tests/test_interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.719309 interva-0.0.5/build/lib/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.720178 interva-0.0.5/build/lib/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/build/lib/interva/interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.721792 interva-0.0.5/build/lib/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/build/lib/tests/test_interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.723993 interva-0.0.5/build/lib/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-02-09 17:14:38.000000 interva-0.0.5/build/lib/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.724718 interva-0.0.5/build/lib/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5725 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    36035 2022-08-29 17:52:11.000000 interva-0.0.5/build/lib/interva/interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.726689 interva-0.0.5/build/lib/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/build/lib/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     2148 2022-08-29 16:27:41.000000 interva-0.0.5/build/lib/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10738 2022-08-29 17:49:16.000000 interva-0.0.5/build/lib/tests/test_interva5.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.730946 interva-0.0.5/interva/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      150 2023-02-09 17:14:38.000000 interva-0.0.5/interva/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      290 2023-03-22 19:51:39.000000 interva-0.0.5/interva/__version__.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.738060 interva-0.0.5/interva/data/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     5724 2023-05-12 20:38:51.000000 interva-0.0.5/interva/data/causetext.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   459264 2023-03-22 19:50:10.000000 interva-0.0.5/interva/data/probbase.xls
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   164661 2022-07-29 16:52:08.000000 interva-0.0.5/interva/data/probbaseV5_19.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088   286521 2022-11-03 17:23:26.000000 interva-0.0.5/interva/data/randomva5.csv
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088      518 2023-05-11 15:53:16.000000 interva-0.0.5/interva/exceptions.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    40925 2023-05-12 19:03:30.000000 interva-0.0.5/interva/interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    18966 2023-05-31 17:21:29.000000 interva-0.0.5/interva/utils.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.745234 interva-0.0.5/interva.egg-info/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4213 2023-06-01 14:44:20.000000 interva-0.0.5/interva.egg-info/PKG-INFO
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3185 2023-06-01 14:44:20.000000 interva-0.0.5/interva.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        1 2023-06-01 14:44:20.000000 interva-0.0.5/interva.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       26 2023-06-01 14:44:20.000000 interva-0.0.5/interva.egg-info/requires.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       25 2023-06-01 14:44:20.000000 interva-0.0.5/interva.egg-info/top_level.txt
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       87 2022-07-29 15:51:31.000000 interva-0.0.5/pyproject.toml
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088       38 2023-06-01 14:44:20.746605 interva-0.0.5/setup.cfg
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     1367 2023-03-13 22:54:59.000000 interva-0.0.5/setup.py
+drwxr-xr-x   0 thomas.3912 (1583608718) 444659088        0 2023-06-01 14:44:20.742959 interva-0.0.5/tests/
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088        0 2022-07-29 15:44:16.000000 interva-0.0.5/tests/__init__.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     3814 2023-05-12 18:14:23.000000 interva-0.0.5/tests/test_compare_r.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088    10772 2023-05-12 16:39:17.000000 interva-0.0.5/tests/test_interva5.py
+-rw-r--r--   0 thomas.3912 (1583608718) 444659088     4519 2023-05-31 18:06:53.000000 interva-0.0.5/tests/test_utils.py
```

### Comparing `interva-0.0.4/LICENSE` & `interva-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/PKG-INFO` & `interva-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interva
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python implementation of the InterVA Algorithm.
 Home-page: https://github.com/verbal-autopsy-software/interva
 Author: Sherry Zhao & Jason Thomas
 Author-email: zhao.3248@buckeyemail.osu.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `interva-0.0.4/README.md` & `interva-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/interva/interva5.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.5/build/lib/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.5/build/lib/build/lib/build/lib/interva/data/causetext.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/interva/interva5.py` & `interva-0.0.5/build/lib/build/lib/build/lib/interva/interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.5/build/lib/build/lib/build/lib/tests/test_compare_r.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.5/build/lib/build/lib/build/lib/tests/test_interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/interva/data/causetext.py` & `interva-0.0.5/build/lib/build/lib/interva/data/causetext.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/interva/interva5.py` & `interva-0.0.5/build/lib/build/lib/interva/interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/tests/test_compare_r.py` & `interva-0.0.5/build/lib/build/lib/tests/test_compare_r.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/build/lib/tests/test_interva5.py` & `interva-0.0.5/build/lib/build/lib/tests/test_interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/interva/data/causetext.py` & `interva-0.0.5/build/lib/interva/data/causetext.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/interva/interva5.py` & `interva-0.0.5/build/lib/interva/interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/tests/test_compare_r.py` & `interva-0.0.5/build/lib/tests/test_compare_r.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/build/lib/tests/test_interva5.py` & `interva-0.0.5/build/lib/tests/test_interva5.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/interva/data/causetext.py` & `interva-0.0.5/interva/data/causetext.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 CAUSETEXTV5 = {
     "a_nrp": {"cause": "Not pregnant or recently delivered",
               "code": "Not pregnant or recently delivered"},
     "a_pend_6w": {"cause": "Pregnancy ended within 6 weeks of death",
                   "code": "Pregnancy ended within 6 weeks of death"},
     "a_preg": {"cause": "Pregnant at death",
                "code": "Pregnant at death"},
-    "b_0101": {"cause": "Sepsis (non-obstetric)", 
+    "b_0101": {"cause": "Sepsis (non-obstetric)",
                "code": 1.01},
     "b_0102": {"cause": "Acute resp infect incl pneumonia",
                "code": 1.02},
     "b_0103": {"cause": "HIV/AIDS related death",
                "code": 1.03},
     "b_0104": {"cause": "Diarrhoeal diseases",
                "code": 1.04},
```

### Comparing `interva-0.0.4/interva/data/probbase.xls` & `interva-0.0.5/interva/data/probbase.xls`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 000001b0: ffff ffff ffff ffff ffff ffff ffff ffff  ................
 000001c0: ffff ffff ffff ffff ffff ffff ffff ffff  ................
 000001d0: ffff ffff ffff ffff ffff ffff ffff ffff  ................
 000001e0: ffff ffff ffff ffff ffff ffff ffff ffff  ................
 000001f0: ffff ffff ffff ffff ffff ffff ffff ffff  ................
 00000200: 0908 0800 0005 0500 0a54 cd07 e100 0000  .........T......
 00000210: c100 0200 0000 bf00 0000 c000 0000 e200  ................
-00000220: 0000 5c00 7000 154d 6963 726f 736f 6674  ..\.p..Microsoft
-00000230: 204f 6666 6963 6520 5573 6572 2020 2020   Office User    
+00000220: 0000 5c00 7000 0550 6574 6572 2020 2020  ..\.p..Peter    
+00000230: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000240: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000250: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000260: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000280: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000290: 2020 2020 2020 4200 0200 e404 9c00 0200        B.........
 000002a0: 1100 1900 0200 0000 1200 0200 0000 1300  ................
@@ -28672,16 +28672,16 @@
 0006fff0: fdff ffff fdff ffff fdff ffff feff ffff  ................
 00070000: 5200 6f00 6f00 7400 2000 4500 6e00 7400  R.o.o.t. .E.n.t.
 00070010: 7200 7900 0000 0000 0000 0000 0000 0000  r.y.............
 00070020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00070030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00070040: 1600 0501 ffff ffff ffff ffff 0200 0000  ................
 00070050: 1008 0200 0000 0000 c000 0000 0000 0046  ...............F
-00070060: 0000 0000 0000 0000 0000 0000 60d9 99e2  ............`...
-00070070: a7ef d801 feff ffff 0000 0000 0000 0000  ................
+00070060: 0000 0000 0000 0000 0000 0000 0091 3894  ..............8.
+00070070: 610e d601 feff ffff 0000 0000 0000 0000  a...............
 00070080: 4200 6f00 6f00 6b00 0000 0000 0000 0000  B.o.o.k.........
 00070090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000700a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000700b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000700c0: 0a00 0201 ffff ffff ffff ffff ffff ffff  ................
 000700d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000700e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `interva-0.0.4/interva/data/probbaseV5_19.csv` & `interva-0.0.5/interva/data/probbaseV5_19.csv`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/interva/data/randomva5.csv` & `interva-0.0.5/interva/data/randomva5.csv`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/interva/interva5.py` & `interva-0.0.5/interva/interva5.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 from logging import INFO, FileHandler, getLogger
 from csv import writer
 import datetime
 from pkgutil import get_data
 from io import BytesIO
 
 from interva.data.causetext import CAUSETEXTV5
+from interva.utils import _get_dem_groups
 from vacheck.datacheck5 import datacheck5
 
 
 class InterVA5:
     """InterVA5 algorithm for assigning cause of death.
 
     :param va_input: Verbal Autopsy data
@@ -76,30 +77,88 @@
     def __init__(self, va_input: Union[DataFrame, str], hiv: str, malaria: str,
                  write: bool = True, directory: str = None,
                  filename: str = "VA5_result", output: str = "classic",
                  append: bool = False, groupcode: bool = False,
                  sci: DataFrame = None,
                  return_checked_data: bool = False,
                  openva_app: Union[None,
-                                   PyQt5.QtWidgets.QWidget] = None) -> dict:
+                                   PyQt5.QtWidgets.QWidget] = None,
+                 gui_ctrl: dict = {"break": False}) -> dict:
 
         self.va_input = va_input
         self.hiv = hiv
         self.malaria = malaria
         self.write = write
         self.directory = directory
         self.filename = filename
         self.output = output
         self.append = append
         self.groupcode = groupcode
         self.sci = sci
         self.return_checked_data = return_checked_data
         self.openva_app = openva_app
         self.checked_data: Union[DataFrame, str] = ""
-        self.out = {}
+        self.results: dict = {}
+        self.gui_ctrl = gui_ctrl
+        self.dem_group: DataFrame = DataFrame({})
+
+    def __repr__(self):
+        sci_msg = "None\n"
+        if self.sci is not None:
+            sci_msg = "\n\n" + repr(self.sci) + "\n\n"
+        msg = ("interva.interva5.InterVA5(\n"
+               f"va_input = \n{self.va_input}\n"
+               f"hiv = {self.hiv}\n"
+               f"malaria = {self.malaria}\n"
+               f"write = {self.write}\n"
+               f"directory = {self.directory}\n"
+               f"filename = {self.filename}\n"
+               f"output = {self.output}\n"
+               f"append = {self.append}\n"
+               f"groupcode = {self.groupcode}\n"
+               f"sci = " + sci_msg +
+               f"return_checked_data = {self.return_checked_data}\n"
+               f"openva_app = {self.openva_app}\n"
+               f"gui_ctrl = {self.gui_ctrl}\n" + ")")
+        return msg
+
+    def __str__(self):
+        if len(self.results) == 0:
+            if isinstance(self.va_input, DataFrame):
+                data_msg = f"{self.va_input.shape[0]} VA records loaded\n"
+            elif isinstance(self.va_input, DataFrame):
+                data_msg = f"VA records from {self.va_input}\n"
+            else:
+                data_msg = "No VA records!\n"
+            msg = "InterVA5:\n" + data_msg
+            msg = msg + (f"HIV parameter is {self.hiv}\n"
+                         f"Malaria parameter is {self.malaria}\n"
+                         "No results (need to use run() method).")
+            return msg
+        else:
+            n_processed = self.results["VA5"].shape[0]
+            n_undetermined = sum(
+                self.results["VA5"]["CAUSE1"] == "Undetermined")
+            n_miss = n_processed - self.results["VA5"].shape[0]
+            n_male = sum(self.dem_group["sex"] == "male")
+            n_female = sum(self.dem_group["sex"] == "female")
+            n_adult = sum(self.dem_group["age"] == "adult")
+            n_child = sum(self.dem_group["age"] == "child")
+            n_neo = sum(self.dem_group["age"] == "neonate")
+            msg = ("InterVA5:\n"
+                   f"{self.va_input.shape[0]} VA records loaded\n"
+                   f"HIV parameter is {self.hiv}\n"
+                   f"Malaria parameter is {self.malaria}\n\n"
+                   f"{n_processed} VA records processed:\n"
+                   f"  {n_undetermined} causes are Undetermined\n"
+                   f"  {n_miss} records have missing info for age and/or sex\n"
+                   "Demographic Summary:\n"
+                   f"  Female: {n_female}, Male: {n_male}\n"
+                   f"  Adult: {n_adult}, Child: {n_child}, Neonate: {n_neo}")
+            return msg
 
     @staticmethod
     def _check_data(va_input: Series, va_id: str,
                     insilico_check: bool = False) -> dict:
         """Run data check."""
 
         return datacheck5(va_input, va_id, insilico_check)
@@ -139,30 +198,32 @@
         filename = filename + ".csv"
         x = concatenate((x, prob))
         with open(filename, "a", newline="") as csvfile:
             csv_writer = writer(csvfile)
             csv_writer.writerow(x)
 
     def run(self) -> None:
-        """Assign causes of death.
+        """Assign causes of death to valid VA records.
 
-        :return: ids of VA input,
-         VA results with cause assignments and likelihoods,
-         likelihood of malaria and HIV as causes of death, and
-         cleaned data from data consistency checks.
-        :rtype: dictionary with keys
-         ID (pandas.series),
-         VA5 (pandas DataFrame),
-         Malaria (str),
-         HIV (str), and
-         checked_data (pandas DataFrame).
-        """
+        Results are stored as a dictionary in the attribute out, which includes
+        the keys: (ID) pandas.Series of VA input IDs; (VA5) pandas.DataFrame
+        of VA results with cause assignments and likelihoods for valid VA
+        records (or None if there are no valid records); (Malaria) a str
+        indicating the likelihood of malaria as causes of death; (HIV) a str
+        indicating the likelihood of HIV as causes of death; and (checked_data)
+        a pandas.DataFrame containing the cleaned data from data consistency
+        checks.
+
+        If there are no valid VA records then the out["VA5"] value is None.
+        Note that the data checks identify records as invalid (if the age or
+        sex indicators are missing, or if all the symptoms have missing
+        values).
 
-        if self.openva_app:
-            from PyQt5.QtWidgets import QApplication
+        :return: None
+        """
 
         if self.directory is None and self.write:
             raise IOError(
                 "error: please provide a directory " +
                 "(required when write = True)")
         if self.directory is None:
             self.directory = getcwd()
@@ -312,23 +373,25 @@
             with open(self.filename + ".csv", "w", newline="") as write_obj:
                 csv_writer = writer(write_obj)
                 csv_writer.writerow(header)
         nd = max(1, round(N/100))
         np = max(1, round(N/10))
 
         if self.write:
-            logger.info("\n\nthe following records are incomplete and "
-                        "excluded from further processing: \n\n")
+            logger.info("\nThe following records are incomplete and "
+                        "excluded from further processing:\n")
 
         first_pass = []
         second_pass = []
-        errors = ""
         list_checked_data = []
+        list_dem_group = []
 
         for i in range(N):
+            if self.gui_ctrl["break"]:
+                raise RuntimeError
             k = i + 1
             if k % nd == 0:
                 print(".", end="")
             if k % np == 0:
                 print(round(k/N * 100), "% completed", sep="")
             if k == N:
                 print("100% completed")
@@ -344,32 +407,34 @@
             input_current = copy(va_data[i, :])
             input_current[:][input_current[:] == "0"] = 0
             input_current[:][input_current[:] == "1"] = 1
 
             input_current[0] = 0
             if nansum(input_current[5:12]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in age indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in age indicator: Not Specified")
                 continue
             if nansum(input_current[3:5]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in sex indicator: Not Specified")
+                    logger.info(index_current +
+                                " Error in sex indicator: Not Specified")
                 continue
             if nansum(input_current[20:328]) < 1:
                 if self.write:
-                    errors = (errors + index_current +
-                              " Error in indicators: No symptoms specified")
+                    logger.info(index_current +
+                                " Error in indicators: No symptoms specified")
                 continue
 
             input_current = Series(input_current, index=va_input_names)
             tmp = datacheck5(va_input=input_current, va_id=index_current,
                              probbase=pb_for_datacheck)
 
+            list_dem_group.append(_get_dem_groups(tmp["output"]))
+
             if self.return_checked_data:
                 list_checked_data.append(
                     [id_inputs[i]] + list(tmp["output"][1:S]))
 
             input_current = copy(tmp["output"])
             first_pass.append(tmp["first_pass"])
             second_pass.append(tmp["second_pass"])
@@ -495,18 +560,17 @@
                                    write=self.write)
             if self.output == "extended":
                 InterVA5._save_va5_prob(VA_result[i].copy(),
                                         filename=self.filename,
                                         write=self.write)
             if self.openva_app:
                 progress = int(100 * k / N)
-                self.openva_app.interva_pbar.setValue(progress)
-                QApplication.processEvents()
+                self.openva_app.emit(progress)
         if self.write:
-            logger.info("the following data discrepancies were identified "
+            logger.info("\nThe following data discrepancies were identified "
                         "and handled:\n")
             for j in range(len(first_pass)):
                 item = first_pass[j]
                 if item:
                     for k in item:
                         logger.info(k)
             logger.info("\nSecond pass\n")
@@ -522,25 +586,32 @@
             self.checked_data = DataFrame(list_checked_data)
             self.checked_data.columns = va_input_names
 
         ID_list = Series(ID_list, name="ID")
         nan_indices = where(ID_list.isna())[0]
         ID_list.drop(nan_indices, inplace=True)
 
-        VA_result = DataFrame(VA_result)
-        VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
-                             "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
-                             "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
-        VA_result.drop(nan_indices, axis=0, inplace=True)
-
-        self.out = {"ID": ID_list,
-                    "VA5": VA_result,
-                    "Malaria": self.malaria,
-                    "HIV": self.hiv,
-                    "checked_data": self.checked_data}
+        if len(ID_list) > 0:
+            VA_result = DataFrame(VA_result)
+            VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT",
+                                 "PREGLIK", "CAUSE1", "LIK1", "CAUSE2", "LIK2",
+                                 "CAUSE3", "LIK3", "INDET", "COMCAT", "COMNUM",
+                                 "WHOLEPROB"]
+            VA_result.drop(nan_indices, axis=0, inplace=True)
+        else:
+            VA_result = None
+
+        dem_group = DataFrame(list_dem_group)
+        self.dem_group = dem_group.set_index("ID")
+
+        self.results = {"ID": ID_list,
+                        "VA5": VA_result,
+                        "Malaria": self.malaria,
+                        "HIV": self.hiv,
+                        "checked_data": self.checked_data}
 
     def get_hiv(self) -> str:
         """Get HIV parameter."""
 
         print(f"HIV parameter is {self.hiv}")
         return self.hiv
 
@@ -576,31 +647,32 @@
         """Return pandas series of ID column in data."""
 
         va_df = self.va_input
         if isinstance(va_df, str) and va_df[-4:] == ".csv":
             va_df = read_csv(va_df)
         return va_df.loc[:, "ID"]
 
-    def plot_csmf(self, top: int = 10, file: str = None) -> None:
-        """Plot cause-specific mortality fraction (CSMF)."""
-        pass
+    # def plot_csmf(self, top: int = 10, file: str = None) -> None:
+    #     """Plot cause-specific mortality fraction (CSMF)."""
+    #     pass
 
-    def get_csmf(self, top: int = 10, groupcode: bool = False) -> Series:
+    def get_csmf(self, top: int = 10,
+                 groupcode: bool = False) -> Union[Series, None]:
         """Return top causes in cause-specific mortality fraction (CSMF).
 
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
-        :param groupcode: a logical value indicating whether or not the
-         group code will be included in the cause names.
-        :type groupcode: boolean
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
         :return: the top causes in CSMF with their values.
         :rtype: pandas.series
         """
 
-        va = self.out["VA5"]
+        va = self.results["VA5"]
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
 
         # for future compatibility with non-standard input
         causenames = causeindex = []
         for i in range(va.shape[0]):
             if va.loc[i, "WHOLEPROB"] is not None:
@@ -646,15 +718,15 @@
                     code = str(self.causetextV5.iloc[i, 1])
                     temp_names[i] = code + " " + cause
             causenames = Index(temp_names)
 
         # Check if there is a valid va object
         if len(va) < 1:
             print("No va5 object found")
-            return()
+            return None
         # Initialize the population distribution
         dist = None
         for i in range(len(va)):
             if va.iloc[i, 14] is not None:
                 dist = [[0 for _ in range(len(va.iloc[i, 14]))]]
                 break
         undeter = 0
@@ -734,22 +806,25 @@
             b = dist_cod_sorted[show_top-1]
             while show_top < len(dist_cod_sorted) and \
                     (abs(a-b) < (a+b) * 1e-5):
                 show_top = show_top + 1
                 a = dist_cod_sorted[show_top]
                 b = dist_cod_sorted[show_top-1]
         top_csmf = dist_cod_sorted.head(show_top)
-        return(top_csmf)
+        return top_csmf
 
     def write_csmf(self, top: int = 10, groupcode: bool = False,
                    filename: str = "csmf") -> None:
         """Write cause-specific mortality fraction (CSMF) to CSV file.
 
         :param top: number of top causes in the CSMF to be determined.
         :type top: integer
+        :param groupcode: a logical value indicating if the group code will be
+        included in the cause names.
+        :type groupcode: bool
         :param filename: the filename the user wishes to save the CSMF.
          No extension needed. The output is in .csv format by default.
         :type filename: string
         """
 
         set_option("display.max_rows", None)
         set_option("display.max_columns", None)
@@ -758,24 +833,24 @@
         csmf.to_csv(filename, header=False)
 
     def get_indiv_prob(self, top: int = 0,
                        include_propensities: bool = False) -> DataFrame:
         """Get individual causes of death distribution.
 
         :param top: number of top causes to be determined. If top is 0 or none,
-         all propensities and no top causes will be be returned.
+         all propensities and no top causes will be returned.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :return: the individual causes of death distribution.
         :rtype: pandas DataFrame
         """
 
-        VA5 = self.out["VA5"]
+        VA5 = self.results["VA5"]
         num_indiv = VA5.shape[0]
         cod_list = [[] for _ in range(num_indiv)]
         column_names = []
         if top == 0 or top is None:
             column_names = VA5.loc[0, "WHOLEPROB"].iloc[3:64].index
         else:
             for i in range(top):
@@ -815,24 +890,24 @@
                         if include_propensities:
                             if cause == " ":
                                 cod_list[indiv].append(" ")
                             else:
                                 cod_list[indiv].append(nanmax(prob_temp))
                         prob_temp = delete(prob_temp, max_loc)
         cod_df = DataFrame(cod_list, columns=column_names)
-        cod_df.insert(loc=0, column='ID', value=self.out["ID"])
+        cod_df.insert(loc=0, column='ID', value=self.results["ID"])
         return cod_df
 
     def write_indiv_prob(self, top: int = 0,
                          include_propensities: bool = False,
                          filename: str = "indiv_prob") -> None:
         """Write individual cause of death distribution to CSV file.
 
         :param top: number of top causes to be determined. If top is 0 or none,
-         no causes and all propensities will be be displayed.
+         no causes and all propensities will be displayed.
         :type top: integer
         :param include_propensities: a logical value indicating whether the
          propensities of top causes should be included. If top is 0 or none,
          this boolean is automatically set to true.
         :type include_propensities: boolean
         :param filename: the filename the user wishes to save the individual
          cause distribution. No extension needed. The output is in .csv
```

### Comparing `interva-0.0.4/interva.egg-info/PKG-INFO` & `interva-0.0.5/interva.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: interva
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python implementation of the InterVA Algorithm.
 Home-page: https://github.com/verbal-autopsy-software/interva
 Author: Sherry Zhao & Jason Thomas
 Author-email: zhao.3248@buckeyemail.osu.edu
 License: GPLv3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `interva-0.0.4/interva.egg-info/SOURCES.txt` & `interva-0.0.5/interva.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -43,26 +43,30 @@
 ./build/lib/interva/interva5.py
 ./build/lib/interva/data/causetext.py
 ./build/lib/tests/__init__.py
 ./build/lib/tests/test_compare_r.py
 ./build/lib/tests/test_interva5.py
 ./interva/__init__.py
 ./interva/__version__.py
+./interva/exceptions.py
 ./interva/interva5.py
+./interva/utils.py
 ./interva/data/causetext.py
 ./interva/data/probbase.xls
 ./interva/data/probbaseV5_19.csv
 ./interva/data/randomva5.csv
 ./tests/__init__.py
 ./tests/test_compare_r.py
 ./tests/test_interva5.py
+./tests/test_utils.py
 interva.egg-info/PKG-INFO
 interva.egg-info/SOURCES.txt
 interva.egg-info/dependency_links.txt
 interva.egg-info/requires.txt
 interva.egg-info/top_level.txt
 interva/data/causetext.py
 interva/data/probbase.xls
 interva/data/probbaseV5_19.csv
 interva/data/randomva5.csv
 tests/test_compare_r.py
-tests/test_interva5.py
+tests/test_interva5.py
+tests/test_utils.py
```

### Comparing `interva-0.0.4/setup.py` & `interva-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `interva-0.0.4/tests/test_compare_r.py` & `interva-0.0.5/tests/test_compare_r.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # # -*- coding: utf-8 -*-
 
 from interva.interva5 import InterVA5, get_example_input
+from interva.utils import csmf
 from rpy2.robjects.packages import data, importr
 import rpy2.robjects as robjects
 from rpy2.robjects.conversion import get_conversion, localconverter
 from rpy2.robjects import pandas2ri
 
 r_iva5 = importr("InterVA5")
 randomva5 = data(r_iva5).fetch("RandomVA5")["RandomVA5"]
@@ -18,31 +19,42 @@
                     groupcode=FALSE)$VA5
   prob <- matrix(NA, nrow=nrow(ra5), ncol=length(r_va5[[1]]$wholeprob))
   r_prob_names <- colnames(r_va5[[1]]$wholeprob)
   for (i in 1:nrow(ra5)) {
     prob[i,] <- r_va5[[i]]$wholeprob
   }
   csmf <- InterVA5::CSMF.interVA5(r_va5)
+  csmf5_no_rule <- InterVA5::CSMF5(r_va5, noplot=TRUE)
+  csmf5_no_rule2 <- InterVA5::CSMF5(r_va5, top.aggregate = 8, noplot=TRUE)
 
   r_prob_df <- as.data.frame(prob, colnames=r_prob_names)
   csmf_top15 <- as.data.frame(csmf[order(csmf, decreasing=TRUE)[1:15]])
+  df_csmf5_1 <- as.data.frame(csmf5_no_rule)
+  df_csmf5_2 <- as.data.frame(csmf5_no_rule2)
 ''')
 r_prob_df = robjects.globalenv["r_prob_df"]
 csmf_top15 = robjects.globalenv["csmf_top15"]
+df_csmf5_1 = robjects.globalenv["df_csmf5_1"]
+df_csmf5_2 = robjects.globalenv["df_csmf5_2"]
 
 with localconverter(robjects.default_converter + pandas2ri.converter):
     r_prob_check = get_conversion().rpy2py(r_prob_df)
     r_csmf_top15_check = get_conversion().rpy2py(csmf_top15)
+    r_csmf5_1 = get_conversion().rpy2py(df_csmf5_1)
+    r_csmf5_2 = get_conversion().rpy2py(df_csmf5_2)
 
 va_data = get_example_input()
 iv5out = InterVA5(va_data, hiv="h", malaria="l", directory=".",
                   groupcode=False)
 iv5out.run()
-py_prob_check = iv5out.out["VA5"].loc[:, "WHOLEPROB"]
+py_prob_check = iv5out.results["VA5"].loc[:, "WHOLEPROB"]
 py_csmf_top15_check = iv5out.get_csmf(top=15, groupcode=False)
+py_csmf5_1 = csmf(iv5out, interva_rule=False, top=15)
+py_csmf5_2 = csmf(iv5out, interva_rule=False,
+                  top=15, top_aggregate=8)
 
 
 def test_r_va5_comparison():
     for i in range(r_prob_check.shape[0]):
         for j in range(r_prob_check.shape[1]):
             a = round(r_prob_check.iloc[i, j], 10)
             b = round(py_prob_check[i][j], 10)
@@ -53,7 +65,33 @@
     assert (py_csmf_top15_check.index == r_csmf_top15_check.index).all()
     py_csmf_top15 = py_csmf_top15_check.to_numpy()
     r_csmf_top15 = r_csmf_top15_check.to_numpy()
     for i in range(len(r_csmf_top15_check)):
         a = round(float(py_csmf_top15[i]), 10)
         b = round(float(r_csmf_top15[i]), 10)
         assert a == b
+
+
+def tests_utils_csmf_1():
+    r_csmf5_1_top15 = r_csmf5_1.sort_values(
+        by="csmf5_no_rule", ascending=False)[0:15]
+    py_csmf5_1_top15 = py_csmf5_1.sort_values(ascending=False)
+    assert (r_csmf5_1_top15.index == py_csmf5_1_top15.index).all()
+    py_csmf5_1_top15 = py_csmf5_1_top15.to_numpy()
+    r_csmf5_1_top15 = r_csmf5_1_top15.to_numpy()
+    for i in range(len(r_csmf5_1_top15)):
+        a = round(float(py_csmf5_1_top15[i]), 10)
+        b = round(float(r_csmf5_1_top15[i]), 10)
+        assert a == b
+
+
+def tests_utils_csmf_2():
+    r_csmf5_2_top15 = r_csmf5_2.sort_values(
+        by="csmf5_no_rule2", ascending=False)[0:15]
+    py_csmf5_2_top15 = py_csmf5_2.sort_values(ascending=False)
+    assert (r_csmf5_2_top15.index == py_csmf5_2_top15.index).all()
+    py_csmf5_2_top15 = py_csmf5_2_top15.to_numpy()
+    r_csmf5_2_top15 = r_csmf5_2_top15.to_numpy()
+    for i in range(len(r_csmf5_2_top15)):
+        a = round(float(py_csmf5_2_top15[i]), 4)
+        b = round(float(r_csmf5_2_top15[i]), 4)
+        assert a == b
```

### Comparing `interva-0.0.4/tests/test_interva5.py` & `interva-0.0.5/tests/test_interva5.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,28 +74,28 @@
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # id_output = run_output["ID"]
     iv5out.run()
-    id_output = iv5out.out["ID"]
+    id_output = iv5out.results["ID"]
     assert isinstance(id_output, Series)
     assert (id_output == example_va_ids).all()
 
 
 def test_run_correct_VA5_output(example_va_data, example_va_ids):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # va5_output = run_output["VA5"]
     iv5out.run()
-    va5_output = iv5out.out["VA5"]
+    va5_output = iv5out.results["VA5"]
     # VA_result.columns = ["ID", "MALPREV", "HIVPREV", "PREGSTAT", "PREGLIK",
     #                      "CAUSE1", "LIK1", "CAUSE2", "LIK2", "CAUSE3",
     #                      "LIK3", "INDET", "COMCAT", "COMNUM", "WHOLEPROB"]
     assert isinstance(va5_output, DataFrame)
     assert (va5_output.loc[:, "ID"] == example_va_ids).all()
     assert (va5_output.loc[:, "MALPREV"] == "l").all()
     assert (va5_output.loc[:, "HIVPREV"] == "h").all()
@@ -120,52 +120,52 @@
 def test_run_correct_malaria_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # malaria_output = run_output["Malaria"]
     iv5out.run()
-    malaria_output = iv5out.out["Malaria"]
+    malaria_output = iv5out.results["Malaria"]
     assert isinstance(malaria_output, str)
     assert malaria_output == "l"
 
 
 def test_run_correct_hiv_output(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     # hiv_output = run_output["HIV"]
     iv5out.run()
-    hiv_output = iv5out.out["HIV"]
+    hiv_output = iv5out.results["HIV"]
     assert isinstance(hiv_output, str)
     assert hiv_output == "h"
 
 
 def test_run_correct_checked_data_output_if_true_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=True)
     # run_output = iv5out.run()
     # checked_data_output = run_output["checked_data"]
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, DataFrame)
     assert (checked_data_output.columns == va_data.columns).all()
 
 
 def test_run_correct_checked_data_output_if_false_return(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended",
                       return_checked_data=False)
     # run_output = iv5out.run()
     iv5out.run()
-    checked_data_output = iv5out.out["checked_data"]
+    checked_data_output = iv5out.results["checked_data"]
     assert isinstance(checked_data_output, str)
     assert checked_data_output == "return_checked_data = False"
 
 
 # get hiv/malaria function tests
 def test_get_hiv(example_va_data):
     va_data = example_va_data
@@ -219,16 +219,16 @@
     ids_output = iv5out.get_ids()
     expected = Series(["d" + str(x+1) for x in range(len(va_data))], name="ID")
     assert isinstance(ids_output, Series)
     assert (ids_output == expected).all()
 
 
 # plot function tests
-def test_plot_csmf():
-    pass
+# def test_plot_csmf():
+#     pass
 
 
 # get csmf function tests
 def test_get_csmf_shape(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
@@ -255,29 +255,29 @@
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=0)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # length of prob_B + 1 (ID)
     assert indiv_prob.shape[1] == len(
-        iv5out.out["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
+        iv5out.results["VA5"].loc[0, "WHOLEPROB"].iloc[3:64]) + 1
 
 
 def test_get_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
                       directory=".", output="extended")
     # run_output = iv5out.run()
     iv5out.run()
     indiv_prob = iv5out.get_indiv_prob(top=5, include_propensities=True)
     assert isinstance(indiv_prob, DataFrame)
-    assert (indiv_prob.loc[:, "ID"] == iv5out.out["ID"]).all()
+    assert (indiv_prob.loc[:, "ID"] == iv5out.results["ID"]).all()
     # 5 causes * 2 (for propensities) + 1 ID
     assert indiv_prob.shape[1] == 5*2 + 1
 
 
 def test_write_indiv_prob_top_5(example_va_data):
     va_data = example_va_data
     iv5out = InterVA5(va_data, hiv="h", malaria="l", write=False,
@@ -286,8 +286,8 @@
     iv5out.run()
     iv5out.write_indiv_prob(top=5, filename="indiv_prob_top_5")
     assert isfile('indiv_prob_top_5.csv')
     rowcount = 0
     for _ in open("indiv_prob_top_5.csv"):
         rowcount = rowcount + 1
     # account for column headers
-    assert rowcount == len(iv5out.out["ID"]) + 1
+    assert rowcount == len(iv5out.results["ID"]) + 1
```

