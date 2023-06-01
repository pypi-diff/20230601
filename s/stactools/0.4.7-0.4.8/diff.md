# Comparing `tmp/stactools-0.4.7.tar.gz` & `tmp/stactools-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactools-0.4.7.tar", last modified: Mon May  8 19:54:46 2023, max compression
+gzip compressed data, was "stactools-0.4.8.tar", last modified: Thu Jun  1 15:10:00 2023, max compression
```

## Comparing `stactools-0.4.7.tar` & `stactools-0.4.8.tar`

### file list

```diff
@@ -1,67 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.140977 stactools-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-08 19:54:24.000000 stactools-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-08 19:54:46.140977 stactools-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-08 19:54:24.000000 stactools-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-08 19:54:24.000000 stactools-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-08 19:54:46.140977 stactools-0.4.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.128977 stactools-0.4.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.132977 stactools-0.4.7/src/stactools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.132977 stactools-0.4.7/src/stactools/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.136977 stactools-0.4.7/src/stactools/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/add_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/add_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3018 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/update_extent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/update_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/validate.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/cli/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.140977 stactools-0.4.7/src/stactools/core/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/add_asset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/add_raster.py
--rw-r--r--   0 runner    (1001) docker     (123)     8711 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/create.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/geometry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.140977 stactools-0.4.7/src/stactools/core/io/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/io/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.140977 stactools-0.4.7/src/stactools/core/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11624 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/antimeridian.py
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)    40595 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/raster_footprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/round.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/core/utils/subprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.140977 stactools-0.4.7/src/stactools/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/testing/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/testing/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/testing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-05-08 19:54:24.000000 stactools-0.4.7/src/stactools/testing/test_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 19:54:46.132977 stactools-0.4.7/src/stactools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9153 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 19:54:45.000000 stactools-0.4.7/src/stactools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 19:54:46.000000 stactools-0.4.7/src/stactools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.200767 stactools-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-01 15:09:38.000000 stactools-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-06-01 15:10:00.200767 stactools-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-01 15:09:38.000000 stactools-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-06-01 15:09:38.000000 stactools-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 15:10:00.200767 stactools-0.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.192767 stactools-0.4.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.192767 stactools-0.4.8/src/stactools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.192767 stactools-0.4.8/src/stactools/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.196767 stactools-0.4.8/src/stactools/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/add_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/add_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/update_extent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3492 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/update_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/cli/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.196767 stactools-0.4.8/src/stactools/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/add_asset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/add_raster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8925 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/geometry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.196767 stactools-0.4.8/src/stactools/core/io/
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5801 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/io/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/projection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.200767 stactools-0.4.8/src/stactools/core/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9221 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/antimeridian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40585 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/raster_footprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/round.py
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/core/utils/subprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.200767 stactools-0.4.8/src/stactools/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/testing/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/testing/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-01 15:09:38.000000 stactools-0.4.8/src/stactools/testing/test_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 15:10:00.192767 stactools-0.4.8/src/stactools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9236 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 15:10:00.000000 stactools-0.4.8/src/stactools.egg-info/top_level.txt
```

### Comparing `stactools-0.4.7/LICENSE` & `stactools-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/PKG-INFO` & `stactools-0.4.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: stactools
-Version: 0.4.7
+Version: 0.4.8
 Summary: Command line tool and Python library for working with STAC
-Home-page: https://github.com/stac-utils/stactools
-Author: stac-utils
-Author-email: stac@radiant.earth
-Project-URL: Documentation, https://stactools.readthedocs.io/en/latest/
-Project-URL: Issues, https://github.com/stac-utils/stactools/issues
-Keywords: stactools,pystac,imagery,raster,catalog,STAC
+Author-email: Rob Emanuele <rdemanuele@gmail.com>, Pete Gadomski <pete.gadomski@gmail.com>
+Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
+License: Apache-2.0
+Project-URL: homepage, https://github.com/stac-utils/stactools
+Project-URL: documentation, https://stactools.readthedocs.io/
+Project-URL: repository, https://github.com/stac-utils/stactools.git
+Project-URL: changelog, https://github.com/stac-utils/stactools/blob/main/CHANGELOG.md
+Project-URL: discussions, https://github.com/radiantearth/stac-spec/discussions/categories/stac-software
+Keywords: pystac,imagery,raster,catalog,STAC
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: all
+Provides-Extra: dev
 Provides-Extra: s3
 License-File: LICENSE
 
 # stactools
 
 ![Build Status](https://github.com/stac-utils/stactools/workflows/CI/badge.svg)
 [![Documentation](https://readthedocs.org/projects/stactools/badge/?version=latest)](https://stactools.readthedocs.io/en/latest/)
@@ -90,23 +93,23 @@
 
 ## Running
 
 ```sh
 stac --help
 ```
 
-### Docker
+### Running from docker
 
 ```sh
 docker run --rm ghcr.io/stac-utils/stactools:latest --help
 ```
 
 ## Documentation
 
-See the [documentation page](https://stactools.readthedocs.io/en/latest/) for the latest docs.
+See the [documentation page](https://stactools.readthedocs.io/) for the latest docs.
 
 ## Packages
 
 `stactools` is comprised of many other sub-packages that provide library and CLI functionality.
 Officially supported packages are hosted in the Github [`stactools-packages` organization](https://github.com/stactools-packages/stactools-packages.github.io), and other subpackages may be available from other sources.
 
 There are over 25 packages that translate specific types of data into STAC,
@@ -136,23 +139,20 @@
 For the list of officially supported packages see the [list of STAC packages](https://github.com/stactools-packages/stactools-packages.github.io#list-of-stac-packages)
 on the [stactools-packages GitHub organization](https://github.com/stactools-packages).
 Each package can be installed via `pip install stactools-{package}`, e.g. `pip install stactools-landsat`.
 Third-party packages can be installed in the same way, or, if they are not on PyPI, directly from the source repository, e.g. `pip install /path/to/my/code/stactools-greatdata`.
 
 ## Developing
 
-Basic development can be done with your system's default Python, though it it recommended to use a virtual environment.
-E.g.:
+Clone the repository and install it in editable mode with the `dev` optional dependencies:
 
 ```sh
 git clone https://github.com/stac-utils/stactools.git
 cd stactools
-python -m venv venv
-pip install -e .  # install stactools into the virtual environment in editable mode
-pip install -r requirements-dev.txt  # install development requirements
+pip install -e '.[dev]'
 ```
 
 Linting and formatting are handled with [pre-commit](https://pre-commit.com/).
 You will need to install pre-commit before committing any changes:
 
 ```sh
 pre-commit install
@@ -223,21 +223,20 @@
 ```sh
 conda activate stactools
 ```
 
 Finally, install `stactools` in editable mode and all development requirements:
 
 ```sh
-pip install -e .
-pip install -r requirements-dev.txt
+pip install -e '.[dev]'
 ```
 
-### Documentation
+### Developing the docs
 
-To build and serve the docs, the development requirements must be installed with `pip install -r requirements-dev.txt`.
+To build and serve the docs, the development requirements must be installed with `pip install -e '.[dev]'`.
 To build the docs, you can use `make html` from inside of the docs directory, and to build the docs and start a server that watches for changes, use `make livehtml`:
 
 ```sh
 cd docs
 make html
 make livehtml
 ```
```

### Comparing `stactools-0.4.7/README.md` & `stactools-0.4.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -68,23 +68,23 @@
 
 ## Running
 
 ```sh
 stac --help
 ```
 
-### Docker
+### Running from docker
 
 ```sh
 docker run --rm ghcr.io/stac-utils/stactools:latest --help
 ```
 
 ## Documentation
 
-See the [documentation page](https://stactools.readthedocs.io/en/latest/) for the latest docs.
+See the [documentation page](https://stactools.readthedocs.io/) for the latest docs.
 
 ## Packages
 
 `stactools` is comprised of many other sub-packages that provide library and CLI functionality.
 Officially supported packages are hosted in the Github [`stactools-packages` organization](https://github.com/stactools-packages/stactools-packages.github.io), and other subpackages may be available from other sources.
 
 There are over 25 packages that translate specific types of data into STAC,
@@ -114,23 +114,20 @@
 For the list of officially supported packages see the [list of STAC packages](https://github.com/stactools-packages/stactools-packages.github.io#list-of-stac-packages)
 on the [stactools-packages GitHub organization](https://github.com/stactools-packages).
 Each package can be installed via `pip install stactools-{package}`, e.g. `pip install stactools-landsat`.
 Third-party packages can be installed in the same way, or, if they are not on PyPI, directly from the source repository, e.g. `pip install /path/to/my/code/stactools-greatdata`.
 
 ## Developing
 
-Basic development can be done with your system's default Python, though it it recommended to use a virtual environment.
-E.g.:
+Clone the repository and install it in editable mode with the `dev` optional dependencies:
 
 ```sh
 git clone https://github.com/stac-utils/stactools.git
 cd stactools
-python -m venv venv
-pip install -e .  # install stactools into the virtual environment in editable mode
-pip install -r requirements-dev.txt  # install development requirements
+pip install -e '.[dev]'
 ```
 
 Linting and formatting are handled with [pre-commit](https://pre-commit.com/).
 You will need to install pre-commit before committing any changes:
 
 ```sh
 pre-commit install
@@ -201,21 +198,20 @@
 ```sh
 conda activate stactools
 ```
 
 Finally, install `stactools` in editable mode and all development requirements:
 
 ```sh
-pip install -e .
-pip install -r requirements-dev.txt
+pip install -e '.[dev]'
 ```
 
-### Documentation
+### Developing the docs
 
-To build and serve the docs, the development requirements must be installed with `pip install -r requirements-dev.txt`.
+To build and serve the docs, the development requirements must be installed with `pip install -e '.[dev]'`.
 To build the docs, you can use `make html` from inside of the docs directory, and to build the docs and start a server that watches for changes, use `make livehtml`:
 
 ```sh
 cd docs
 make html
 make livehtml
 ```
```

### Comparing `stactools-0.4.7/src/stactools/cli/__init__.py` & `stactools-0.4.8/src/stactools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/cli/cli.py` & `stactools-0.4.8/src/stactools/cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 from typing import Union
 
 import click
-
 from stactools.cli import registry
 
 
 def setup_logging(level: Union[str, int]) -> None:
     logger = logging.getLogger("stactools")
     logger.setLevel(level)
```

### Comparing `stactools-0.4.7/src/stactools/cli/commands/add.py` & `stactools-0.4.8/src/stactools/cli/commands/add.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Optional
 
 import click
 from pystac import Catalog, Item, read_file
-
 from stactools.core import add_item
 
 
 def add(
     source_item: str,
     target_catalog: str,
     collection_id: Optional[str] = None,
```

### Comparing `stactools-0.4.7/src/stactools/cli/commands/add_asset.py` & `stactools-0.4.8/src/stactools/cli/commands/add_asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import List, Optional
 
 import click
 import pystac
 import pystac.utils
-
 from stactools.core import add_asset_to_item
 
 
 def _add_asset(
     item_path: str,
     asset_key: str,
     asset_path: str,
```

### Comparing `stactools-0.4.7/src/stactools/cli/commands/add_raster.py` & `stactools-0.4.8/src/stactools/cli/commands/add_raster.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import click
 import pystac
-
 from stactools.core import add_raster_to_item
 
 
 def add_raster(item_path: str) -> None:
     item = pystac.read_file(item_path)
     if not isinstance(item, pystac.Item):
         raise click.BadArgumentUsage(f"{item_path} is not a STAC Item")
```

### Comparing `stactools-0.4.7/src/stactools/cli/commands/copy.py` & `stactools-0.4.8/src/stactools/cli/commands/copy.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Optional
 
 import click
 import pystac
 from pystac.utils import make_absolute_href
-
 from stactools.core.copy import copy_catalog, move_all_assets
 
 
 def create_move_assets_command(cli: click.Group) -> click.Command:
     @cli.command(
         "move-assets", short_help="Move or copy assets in a STAC to the Item locations."
     )
@@ -65,34 +64,50 @@
             case_sensitive=False,
         ),
     )
     @click.option(
         "--copy-assets",
         "-a",
         is_flag=True,
-        help=("Copy all item assets to " "be alongside the new item location."),
+        help="Copy all item assets to be alongside the new item location.",
     )
     @click.option(
         "-l",
         "--publish-location",
         help=(
             "Location to use for resolving HREF links "
             "instead of the destination folder."
         ),
     )
+    @click.option(
+        "--resolve-links/--no-resolve-links",
+        default=True,
+        help=(
+            "Whether to resolve HREF links. Defaults to --resolve-links. "
+            "Use --no-resolve-links to avoid writing external child objects locally."
+        ),
+    )
     def copy_command(
         src: str,
         dst: str,
         catalog_type: pystac.CatalogType,
         copy_assets: bool,
         publish_location: Optional[str],
+        resolve_links: bool,
     ) -> None:
         """Copy a STAC Catalog or Collection at SRC to the directory at DST.
 
         Note: Copying a catalog will upgrade it to the latest version of STAC.
         """
         source_catalog = pystac.read_file(make_absolute_href(src))
         if not isinstance(source_catalog, pystac.Catalog):
             raise click.BadArgumentUsage(f"{src} is not a STAC Catalog")
-        copy_catalog(source_catalog, dst, catalog_type, copy_assets, publish_location)
+        copy_catalog(
+            source_catalog,
+            dst,
+            catalog_type,
+            copy_assets,
+            publish_location,
+            resolve_links,
+        )
 
     return copy_command
```

### Comparing `stactools-0.4.7/src/stactools/cli/commands/create.py` & `stactools-0.4.8/src/stactools/cli/commands/create.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import json
 import sys
 
 import click
-
 from stactools.core import create
 
 
 def create_create_item_command(cli: click.Group) -> click.Command:
     @cli.command("create-item", short_help="Creates an item from an asset")
     @click.argument("href")
     def create_item_command(href: str) -> None:
```

### Comparing `stactools-0.4.7/src/stactools/cli/commands/info.py` & `stactools-0.4.8/src/stactools/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/cli/commands/layout.py` & `stactools-0.4.8/src/stactools/cli/commands/layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import click
 import pystac
-
 from stactools.core import layout_catalog
 
 
 def create_layout_command(cli: click.Group) -> click.Command:
     @cli.command(
         "layout", short_help="Reformat the layout of a STAC based on templating."
     )
```

### Comparing `stactools-0.4.7/src/stactools/cli/commands/lint.py` & `stactools-0.4.8/src/stactools/cli/commands/lint.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 from typing import Optional
 
 import click
-from stac_check.lint import Linter  # type: ignore
+from stac_check.lint import Linter
 
 
 def create_lint_command(cli: click.Group) -> click.Command:
     @cli.command("lint", short_help="Lint a stac object with stac-check.")
     @click.option(
         "--quiet",
         is_flag=True,
```

### Comparing `stactools-0.4.7/src/stactools/cli/commands/merge.py` & `stactools-0.4.8/src/stactools/cli/commands/merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from typing import Optional
 
 import click
 import pystac
-
 from stactools.core import merge_all_items
 
 
 def merge(
     source_catalog: str,
     target_catalog: str,
     collection_id: Optional[str] = None,
```

### Comparing `stactools-0.4.7/src/stactools/cli/commands/summary.py` & `stactools-0.4.8/src/stactools/cli/commands/summary.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/cli/commands/update_extent.py` & `stactools-0.4.8/src/stactools/cli/commands/update_extent.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/cli/commands/update_geometry.py` & `stactools-0.4.8/src/stactools/cli/commands/update_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import List, Optional
 
 import click
 from click import Command, Group
 from pystac import Item
-
 from stactools.core.utils import raster_footprint
 
 
 def create_update_geometry_command(cli: Group) -> Command:
     @cli.command(
         "update-geometry", short_help="Update an item geometry from an asset footprint"
     )
```

### Comparing `stactools-0.4.7/src/stactools/cli/commands/validate.py` & `stactools-0.4.8/src/stactools/cli/commands/validate.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/cli/commands/version.py` & `stactools-0.4.8/src/stactools/cli/commands/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import pystac
 from click import echo
 from click.core import Command, Group
 from pystac.version import get_stac_version
-
 from stactools.core import __version__
 
 
 def create_version_command(cli: Group) -> Command:
     @cli.command("version", short_help="Display version info.")
     def version_command() -> None:
         """Display version info."""
```

### Comparing `stactools-0.4.7/src/stactools/cli/registry.py` & `stactools-0.4.8/src/stactools/cli/registry.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/core/__init__.py` & `stactools-0.4.8/src/stactools/core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,8 @@
     "merge_all_items",
     "merge_items",
     "move_asset_file_to_item",
     "move_assets",
     "move_all_assets",
     "use_fsspec",
 ]
-__version__ = "0.4.7"
+__version__ = "0.4.8"
```

### Comparing `stactools-0.4.7/src/stactools/core/add.py` & `stactools-0.4.8/src/stactools/core/add.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Add items to catalogs."""
 
 import os
 
 from pystac import Catalog, Collection, Item
 from pystac.layout import BestPracticesLayoutStrategy
-
 from stactools.core.copy import move_assets as do_move_assets
 
 
 def add_item(
     source_item: Item, target_catalog: Catalog, move_assets: bool = False
 ) -> None:
     """Adds an item to a catalog.
```

### Comparing `stactools-0.4.7/src/stactools/core/add_asset.py` & `stactools-0.4.8/src/stactools/core/add_asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import logging
 
 from pystac import Asset, Item
 from pystac.utils import is_absolute_href, make_relative_href
-
 from stactools.core.copy import move_asset_file_to_item
 
 logger = logging.getLogger(__name__)
 
 
 def add_asset_to_item(
     item: Item,
```

### Comparing `stactools-0.4.7/src/stactools/core/add_raster.py` & `stactools-0.4.8/src/stactools/core/add_raster.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/core/copy.py` & `stactools-0.4.8/src/stactools/core/copy.py`

 * *Files 3% similar despite different names*

```diff
@@ -226,20 +226,26 @@
 
 def copy_catalog(
     source_catalog: Catalog,
     dest_directory: str,
     catalog_type: Optional[CatalogType] = None,
     copy_assets: bool = False,
     publish_location: Optional[str] = None,
+    resolve_links: bool = True,
 ) -> None:
-    catalog = source_catalog.full_copy()
+    if resolve_links:
+        catalog = source_catalog.full_copy()
+    else:
+        catalog = source_catalog.clone()
+        catalog.set_root(catalog)
+
     dest_directory = make_absolute_href(dest_directory)
 
     if copy_assets:
         catalog = move_all_assets(catalog, copy=True, make_hrefs_relative=True)
 
     if publish_location is not None:
-        catalog.normalize_hrefs(publish_location)
+        catalog.normalize_hrefs(publish_location, skip_unresolved=not resolve_links)
         catalog.save(catalog_type, dest_directory)
     else:
-        catalog.normalize_hrefs(dest_directory)
+        catalog.normalize_hrefs(dest_directory, skip_unresolved=not resolve_links)
         catalog.save(catalog_type)
```

### Comparing `stactools-0.4.7/src/stactools/core/create.py` & `stactools-0.4.8/src/stactools/core/create.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import datetime
 import os.path
 from typing import Optional
 
 import rasterio
 import shapely.geometry
+import stactools.core.projection
 from pystac import Asset, Item
 from pystac.extensions.projection import ProjectionExtension
 
-import stactools.core.projection
-
 from .io import ReadHrefModifier
 
 
 def item(href: str, read_href_modifier: Optional[ReadHrefModifier] = None) -> Item:
     """Creates a STAC Item from the asset at the provided href.
 
     The ``read_href_modifer`` argument can be used to modify the href for the
```

### Comparing `stactools-0.4.7/src/stactools/core/geometry.py` & `stactools-0.4.8/src/stactools/core/geometry.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/core/io/__init__.py` & `stactools-0.4.8/src/stactools/core/io/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import os
 from typing import Any, Callable, Optional
 
 import fsspec
 from pystac.link import HREF
 from pystac.stac_io import StacIO
-
 from stactools.core import utils
 
 ReadHrefModifier = Callable[[str], str]
 """Type alias for a function parameter that allows users to manipulate HREFs.
 
 Used for reading, e.g. appending an Azure SAS Token or translating to a
 signed URL.
```

### Comparing `stactools-0.4.7/src/stactools/core/io/xml.py` & `stactools-0.4.8/src/stactools/core/io/xml.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from functools import lru_cache
 from typing import Any, Callable, List, Optional, cast
 
 from lxml import etree
 from lxml.etree import _Element as lxmlElement
-
 from stactools.core.io import ReadHrefModifier, read_text
 
 
 class XmlElement:
     """Thin wrapper around `lxml <https://lxml.de/>`_ etree.Element with some
     convenience functions."""
 
@@ -25,15 +24,15 @@
 
         Args:
             xpath (str): The xpath to use for search.
 
         Returns:
             Optional[XmlElement]: The found element, or None if not found.
         """
-        node = self.element.find(xpath, self.element.nsmap)  # type: ignore
+        node = self.element.find(xpath, self.element.nsmap)
         return None if node is None else XmlElement(node)
 
     def find_or_throw(
         self, xpath: str, get_exception: Callable[[str], Exception]
     ) -> "XmlElement":
         """Find a child ``XmlElement`` by xpath, or throw an exception if not
         found.
@@ -61,18 +60,15 @@
 
         Args:
             xpath (str): The xpath to use for search.
 
         Returns:
             list[XmlElement]: The found elements.
         """
-        return [
-            XmlElement(e)
-            for e in self.element.findall(xpath, self.element.nsmap)  # type: ignore
-        ]
+        return [XmlElement(e) for e in self.element.findall(xpath, self.element.nsmap)]
 
     @lru_cache(maxsize=100)
     def find_text(self, xpath: str) -> Optional[str]:
         """Finds an element by xpath and returns its contained text.
 
         Args:
             xpath (str): The xpath to use for search.
```

### Comparing `stactools-0.4.7/src/stactools/core/layout.py` & `stactools-0.4.8/src/stactools/core/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
 
 from pystac import Catalog
 from pystac.layout import TemplateLayoutStrategy
-
 from stactools.core import move_all_assets
 
 
 def layout_catalog(
     catalog: Catalog,
     item_path_template: str,
     create_subcatalogs: bool = False,
```

### Comparing `stactools-0.4.7/src/stactools/core/merge.py` & `stactools-0.4.8/src/stactools/core/merge.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 from typing import Optional
 
 import pystac
 from pystac.layout import BestPracticesLayoutStrategy
 from pystac.utils import is_absolute_href, make_relative_href
 from shapely.geometry import mapping, shape
-
 from stactools.core.copy import copy_catalog, move_asset_file_to_item
 from stactools.core.copy import move_assets as do_move_assets
 
 
 def merge_items(
     source_item: pystac.Item,
     target_item: pystac.Item,
```

### Comparing `stactools-0.4.7/src/stactools/core/projection.py` & `stactools-0.4.8/src/stactools/core/projection.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/core/utils/__init__.py` & `stactools-0.4.8/src/stactools/core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/core/utils/convert.py` & `stactools-0.4.8/src/stactools/core/utils/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import os
 from typing import Any, Dict, List, Optional, Tuple, cast
 
 import rasterio
 import rasterio.shutil
 from rasterio.errors import DriverRegistrationError
-
 from stactools.core import utils
 
 DEFAULT_PROFILE = {
     "compress": "deflate",
     "driver": "COG",
     "blocksize": 512,
 }
```

### Comparing `stactools-0.4.7/src/stactools/core/utils/raster_footprint.py` & `stactools-0.4.8/src/stactools/core/utils/raster_footprint.py`

 * *Files 0% similar despite different names*

```diff
@@ -255,15 +255,15 @@
         assert self.data_array.ndim == 3
         shape = self.data_array.shape
         if self.no_data is not None:
             mask: npt.NDArray[np.uint8] = np.full(shape, 0, dtype=np.uint8)
             if np.isnan(self.no_data):
                 mask[~np.isnan(self.data_array)] = 1
             else:
-                mask[np.where(self.data_array != self.no_data)] = 1
+                mask[self.data_array != self.no_data] = 1
             mask = np.sum(mask, axis=0, dtype=np.uint8)
             mask[mask > 0] = 1
         else:
             mask = np.full(shape, 1, dtype=np.uint8)
         return mask
 
     def data_extent(self, mask: npt.NDArray[np.uint8]) -> Optional[Polygon]:
```

### Comparing `stactools-0.4.7/src/stactools/core/utils/round.py` & `stactools-0.4.8/src/stactools/core/utils/round.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/core/utils/subprocess.py` & `stactools-0.4.8/src/stactools/core/utils/subprocess.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/testing/cli.py` & `stactools-0.4.8/src/stactools/testing/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """CLI for test data maintenance and generation."""
 import logging
 import os
 import shutil
 from tempfile import TemporaryDirectory
 
 import click
-
 from stactools.core.utils.subprocess import call
 
 logger = logging.getLogger(__name__)
 
 
 @click.group()
 def cli() -> None:
```

### Comparing `stactools-0.4.7/src/stactools/testing/cli_test.py` & `stactools-0.4.8/src/stactools/testing/cli_test.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools/testing/test_data.py` & `stactools-0.4.8/src/stactools/testing/test_data.py`

 * *Files identical despite different names*

### Comparing `stactools-0.4.7/src/stactools.egg-info/PKG-INFO` & `stactools-0.4.8/src/stactools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 Metadata-Version: 2.1
 Name: stactools
-Version: 0.4.7
+Version: 0.4.8
 Summary: Command line tool and Python library for working with STAC
-Home-page: https://github.com/stac-utils/stactools
-Author: stac-utils
-Author-email: stac@radiant.earth
-Project-URL: Documentation, https://stactools.readthedocs.io/en/latest/
-Project-URL: Issues, https://github.com/stac-utils/stactools/issues
-Keywords: stactools,pystac,imagery,raster,catalog,STAC
+Author-email: Rob Emanuele <rdemanuele@gmail.com>, Pete Gadomski <pete.gadomski@gmail.com>
+Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
+License: Apache-2.0
+Project-URL: homepage, https://github.com/stac-utils/stactools
+Project-URL: documentation, https://stactools.readthedocs.io/
+Project-URL: repository, https://github.com/stac-utils/stactools.git
+Project-URL: changelog, https://github.com/stac-utils/stactools/blob/main/CHANGELOG.md
+Project-URL: discussions, https://github.com/radiantearth/stac-spec/discussions/categories/stac-software
+Keywords: pystac,imagery,raster,catalog,STAC
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: all
+Provides-Extra: dev
 Provides-Extra: s3
 License-File: LICENSE
 
 # stactools
 
 ![Build Status](https://github.com/stac-utils/stactools/workflows/CI/badge.svg)
 [![Documentation](https://readthedocs.org/projects/stactools/badge/?version=latest)](https://stactools.readthedocs.io/en/latest/)
@@ -90,23 +93,23 @@
 
 ## Running
 
 ```sh
 stac --help
 ```
 
-### Docker
+### Running from docker
 
 ```sh
 docker run --rm ghcr.io/stac-utils/stactools:latest --help
 ```
 
 ## Documentation
 
-See the [documentation page](https://stactools.readthedocs.io/en/latest/) for the latest docs.
+See the [documentation page](https://stactools.readthedocs.io/) for the latest docs.
 
 ## Packages
 
 `stactools` is comprised of many other sub-packages that provide library and CLI functionality.
 Officially supported packages are hosted in the Github [`stactools-packages` organization](https://github.com/stactools-packages/stactools-packages.github.io), and other subpackages may be available from other sources.
 
 There are over 25 packages that translate specific types of data into STAC,
@@ -136,23 +139,20 @@
 For the list of officially supported packages see the [list of STAC packages](https://github.com/stactools-packages/stactools-packages.github.io#list-of-stac-packages)
 on the [stactools-packages GitHub organization](https://github.com/stactools-packages).
 Each package can be installed via `pip install stactools-{package}`, e.g. `pip install stactools-landsat`.
 Third-party packages can be installed in the same way, or, if they are not on PyPI, directly from the source repository, e.g. `pip install /path/to/my/code/stactools-greatdata`.
 
 ## Developing
 
-Basic development can be done with your system's default Python, though it it recommended to use a virtual environment.
-E.g.:
+Clone the repository and install it in editable mode with the `dev` optional dependencies:
 
 ```sh
 git clone https://github.com/stac-utils/stactools.git
 cd stactools
-python -m venv venv
-pip install -e .  # install stactools into the virtual environment in editable mode
-pip install -r requirements-dev.txt  # install development requirements
+pip install -e '.[dev]'
 ```
 
 Linting and formatting are handled with [pre-commit](https://pre-commit.com/).
 You will need to install pre-commit before committing any changes:
 
 ```sh
 pre-commit install
@@ -223,21 +223,20 @@
 ```sh
 conda activate stactools
 ```
 
 Finally, install `stactools` in editable mode and all development requirements:
 
 ```sh
-pip install -e .
-pip install -r requirements-dev.txt
+pip install -e '.[dev]'
 ```
 
-### Documentation
+### Developing the docs
 
-To build and serve the docs, the development requirements must be installed with `pip install -r requirements-dev.txt`.
+To build and serve the docs, the development requirements must be installed with `pip install -e '.[dev]'`.
 To build the docs, you can use `make html` from inside of the docs directory, and to build the docs and start a server that watches for changes, use `make livehtml`:
 
 ```sh
 cd docs
 make html
 make livehtml
 ```
```

### Comparing `stactools-0.4.7/src/stactools.egg-info/SOURCES.txt` & `stactools-0.4.8/src/stactools.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 LICENSE
 README.md
 pyproject.toml
-setup.cfg
 src/stactools.egg-info/PKG-INFO
 src/stactools.egg-info/SOURCES.txt
 src/stactools.egg-info/dependency_links.txt
 src/stactools.egg-info/entry_points.txt
-src/stactools.egg-info/not-zip-safe
 src/stactools.egg-info/requires.txt
 src/stactools.egg-info/top_level.txt
 src/stactools/cli/__init__.py
 src/stactools/cli/__main__.py
 src/stactools/cli/cli.py
-src/stactools/cli/py.typed
 src/stactools/cli/registry.py
 src/stactools/cli/commands/__init__.py
 src/stactools/cli/commands/add.py
 src/stactools/cli/commands/add_asset.py
 src/stactools/cli/commands/add_raster.py
 src/stactools/cli/commands/copy.py
 src/stactools/cli/commands/create.py
@@ -36,21 +33,19 @@
 src/stactools/core/add_raster.py
 src/stactools/core/copy.py
 src/stactools/core/create.py
 src/stactools/core/geometry.py
 src/stactools/core/layout.py
 src/stactools/core/merge.py
 src/stactools/core/projection.py
-src/stactools/core/py.typed
 src/stactools/core/io/__init__.py
 src/stactools/core/io/xml.py
 src/stactools/core/utils/__init__.py
 src/stactools/core/utils/antimeridian.py
 src/stactools/core/utils/convert.py
 src/stactools/core/utils/raster_footprint.py
 src/stactools/core/utils/round.py
 src/stactools/core/utils/subprocess.py
 src/stactools/testing/__init__.py
 src/stactools/testing/cli.py
 src/stactools/testing/cli_test.py
-src/stactools/testing/py.typed
 src/stactools/testing/test_data.py
```

