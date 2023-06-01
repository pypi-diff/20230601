# Comparing `tmp/yang-vlp-0.2.19.tar.gz` & `tmp/yang-vlp-0.2.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-de3eu8l2\yang-vlp-0.2.19.tar", last modified: Tue May 16 07:20:44 2023, max compression
+gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-uzht8j2i\yang-vlp-0.2.20.tar", last modified: Thu Jun  1 13:05:58 2023, max compression
```

## Comparing `yang-vlp-0.2.19.tar` & `yang-vlp-0.2.20.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.891974 yang-vlp-0.2.19/
--rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.19/LICENSE
--rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.19/MANIFEST.in
--rw-rw-rw-   0        0        0     2686 2023-05-16 07:20:44.890979 yang-vlp-0.2.19/PKG-INFO
--rw-rw-rw-   0        0        0      847 2023-05-06 06:53:58.000000 yang-vlp-0.2.19/README.md
--rw-rw-rw-   0        0        0      639 2023-05-09 12:15:04.000000 yang-vlp-0.2.19/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-16 07:20:44.891974 yang-vlp-0.2.19/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-05-09 12:15:10.000000 yang-vlp-0.2.19/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.700493 yang-vlp-0.2.19/vlppy/
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.704475 yang-vlp-0.2.19/vlppy/.vscode/
--rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.19/vlppy/.vscode/settings.json
--rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.19/vlppy/LICENSE.txt
--rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.19/vlppy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.721475 yang-vlp-0.2.19/vlppy/demo/
--rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.19/vlppy/demo/README.md
--rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.19/vlppy/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.730473 yang-vlp-0.2.19/vlppy/demo/__pycache__/
--rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.19/vlppy/demo/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.19/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
--rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.19/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
--rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 yang-vlp-0.2.19/vlppy/demo/demo_filter.py
--rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.19/vlppy/demo/demo_main.py
--rw-rw-rw-   0        0        0     2950 2023-05-16 06:59:59.000000 yang-vlp-0.2.19/vlppy/demo/vlp_model.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.738497 yang-vlp-0.2.19/vlppy/error/
--rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.19/vlppy/error/__init__.py
--rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.19/vlppy/error/error.py
--rw-rw-rw-   0        0        0      108 2023-05-09 12:14:50.000000 yang-vlp-0.2.19/vlppy/info.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.743473 yang-vlp-0.2.19/vlppy/io/
--rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.19/vlppy/io/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.19/vlppy/io/io.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.799613 yang-vlp-0.2.19/vlppy/model/
--rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.19/vlppy/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.816477 yang-vlp-0.2.19/vlppy/model/__pycache__/
--rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.19/vlppy/model/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.19/vlppy/model/__pycache__/filter.cpython-39.pyc
--rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.19/vlppy/model/__pycache__/led.cpython-39.pyc
--rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.19/vlppy/model/__pycache__/pd.cpython-39.pyc
--rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.19/vlppy/model/__pycache__/room.cpython-39.pyc
--rw-rw-rw-   0        0        0     6303 2023-05-16 07:19:55.000000 yang-vlp-0.2.19/vlppy/model/led.py
--rw-rw-rw-   0        0        0    18199 2023-05-16 07:07:32.000000 yang-vlp-0.2.19/vlppy/model/pd.py
--rw-rw-rw-   0        0        0    17948 2023-05-16 06:59:05.000000 yang-vlp-0.2.19/vlppy/model/room.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.841688 yang-vlp-0.2.19/vlppy/setting/
--rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.19/vlppy/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.846675 yang-vlp-0.2.19/vlppy/setting/__pycache__/
--rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.19/vlppy/setting/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.19/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
--rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.19/vlppy/setting/json_setting.py
--rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.19/vlppy/setting/settings.json
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.856676 yang-vlp-0.2.19/vlppy/signal/
--rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.19/vlppy/signal/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.19/vlppy/signal/filter.py
--rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 yang-vlp-0.2.19/vlppy/signal/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.861698 yang-vlp-0.2.19/vlppy/tools/
--rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.19/vlppy/tools/__init__.py
--rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.19/vlppy/tools/decorator.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.868682 yang-vlp-0.2.19/vlppy/vis/
--rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.19/vlppy/vis/__init__.py
--rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.19/vlppy/vis/vis.py
-drwxrwxrwx   0        0        0        0 2023-05-16 07:20:44.885991 yang-vlp-0.2.19/yang_vlp.egg-info/
--rw-rw-rw-   0        0        0     2686 2023-05-16 07:20:44.000000 yang-vlp-0.2.19/yang_vlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2023-05-16 07:20:44.000000 yang-vlp-0.2.19/yang_vlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 07:20:44.000000 yang-vlp-0.2.19/yang_vlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-16 07:20:44.000000 yang-vlp-0.2.19/yang_vlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-16 07:20:44.000000 yang-vlp-0.2.19/yang_vlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.953498 yang-vlp-0.2.20/
+-rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.20/LICENSE
+-rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.20/MANIFEST.in
+-rw-rw-rw-   0        0        0     2686 2023-06-01 13:05:58.950497 yang-vlp-0.2.20/PKG-INFO
+-rw-rw-rw-   0        0        0      847 2023-05-06 06:53:58.000000 yang-vlp-0.2.20/README.md
+-rw-rw-rw-   0        0        0      639 2023-06-01 06:17:34.000000 yang-vlp-0.2.20/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-01 13:05:58.954497 yang-vlp-0.2.20/setup.cfg
+-rw-rw-rw-   0        0        0      943 2023-06-01 06:17:22.000000 yang-vlp-0.2.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.736496 yang-vlp-0.2.20/vlppy/
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.739497 yang-vlp-0.2.20/vlppy/.vscode/
+-rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.20/vlppy/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.20/vlppy/LICENSE.txt
+-rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.20/vlppy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.757498 yang-vlp-0.2.20/vlppy/demo/
+-rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.20/vlppy/demo/README.md
+-rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.20/vlppy/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.783493 yang-vlp-0.2.20/vlppy/demo/__pycache__/
+-rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.20/vlppy/demo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.20/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.20/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 yang-vlp-0.2.20/vlppy/demo/demo_filter.py
+-rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.20/vlppy/demo/demo_main.py
+-rw-rw-rw-   0        0        0     2950 2023-05-16 06:59:59.000000 yang-vlp-0.2.20/vlppy/demo/vlp_model.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.799493 yang-vlp-0.2.20/vlppy/error/
+-rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.20/vlppy/error/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.20/vlppy/error/error.py
+-rw-rw-rw-   0        0        0      108 2023-06-01 06:17:48.000000 yang-vlp-0.2.20/vlppy/info.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.805493 yang-vlp-0.2.20/vlppy/io/
+-rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.20/vlppy/io/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.20/vlppy/io/io.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.818509 yang-vlp-0.2.20/vlppy/model/
+-rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.20/vlppy/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.860525 yang-vlp-0.2.20/vlppy/model/__pycache__/
+-rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.20/vlppy/model/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.20/vlppy/model/__pycache__/filter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.20/vlppy/model/__pycache__/led.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.20/vlppy/model/__pycache__/pd.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.20/vlppy/model/__pycache__/room.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6303 2023-05-16 07:19:55.000000 yang-vlp-0.2.20/vlppy/model/led.py
+-rw-rw-rw-   0        0        0    18237 2023-05-22 02:50:09.000000 yang-vlp-0.2.20/vlppy/model/pd.py
+-rw-rw-rw-   0        0        0    17966 2023-06-01 06:04:36.000000 yang-vlp-0.2.20/vlppy/model/room.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.880491 yang-vlp-0.2.20/vlppy/setting/
+-rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.20/vlppy/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.894491 yang-vlp-0.2.20/vlppy/setting/__pycache__/
+-rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.20/vlppy/setting/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.20/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.20/vlppy/setting/json_setting.py
+-rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.20/vlppy/setting/settings.json
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.916491 yang-vlp-0.2.20/vlppy/signal/
+-rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.20/vlppy/signal/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.20/vlppy/signal/filter.py
+-rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 yang-vlp-0.2.20/vlppy/signal/plot.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.922491 yang-vlp-0.2.20/vlppy/tools/
+-rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.20/vlppy/tools/__init__.py
+-rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.20/vlppy/tools/decorator.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.929491 yang-vlp-0.2.20/vlppy/vis/
+-rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.20/vlppy/vis/__init__.py
+-rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.20/vlppy/vis/vis.py
+drwxrwxrwx   0        0        0        0 2023-06-01 13:05:58.946494 yang-vlp-0.2.20/yang_vlp.egg-info/
+-rw-rw-rw-   0        0        0     2686 2023-06-01 13:05:58.000000 yang-vlp-0.2.20/yang_vlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-06-01 13:05:58.000000 yang-vlp-0.2.20/yang_vlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 13:05:58.000000 yang-vlp-0.2.20/yang_vlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-06-01 13:05:58.000000 yang-vlp-0.2.20/yang_vlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-01 13:05:58.000000 yang-vlp-0.2.20/yang_vlp.egg-info/top_level.txt
```

### Comparing `yang-vlp-0.2.19/LICENSE` & `yang-vlp-0.2.20/LICENSE`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/PKG-INFO` & `yang-vlp-0.2.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.19
+Version: 0.2.20
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `yang-vlp-0.2.19/README.md` & `yang-vlp-0.2.20/README.md`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/pyproject.toml` & `yang-vlp-0.2.20/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yang-vlp"
-version = "0.2.19"
+version = "0.2.20"
 authors = [
   { name="yangwuju", email="1424134319@qq.com" },
 ]
 description = "Construction of visible light positioning model"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
```

### Comparing `yang-vlp-0.2.19/setup.py` & `yang-vlp-0.2.20/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,24 +6,25 @@
 path = os.path.join(CUR_PATH, 'build')
 if os.path.isdir(path):
     print('INFO del dir ', path) 
     shutil.rmtree(path)
 
 setup(
     name = 'yang-vlp', #应用名
-    version = '0.2.19',  #版本号
+    version = '0.2.20',  #版本号
     description = 'Construction of visible light positioning model', 
     packages = find_packages(),  #包括在安装包内的Python包
     include_package_data = True, #启用清单文件MANIFEST.in,包含数据文件
     # exclude_package_data = {'docs':['1.txt']},  #排除文件
     install_requires = [#自动安装依赖
         'numpy>=1.19.0',
         'matplotlib>=3.5.0',
         'scipy>=1.8.0',
-        'pandas>=1.3.0'
+        'pandas>=1.3.0',
+        
     ],
     author = 'yangwuju',
     author_email = '1424134319@qq.com',
     url = 'https://gitee.com/yangwuju/yang_vlp',
 )
```

### Comparing `yang-vlp-0.2.19/vlppy/LICENSE.txt` & `yang-vlp-0.2.20/vlppy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/demo/__pycache__/demo_main.cpython-39.pyc` & `yang-vlp-0.2.20/vlppy/demo/__pycache__/demo_main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc` & `yang-vlp-0.2.20/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/demo/demo_filter.py` & `yang-vlp-0.2.20/vlppy/demo/demo_filter.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/demo/demo_main.py` & `yang-vlp-0.2.20/vlppy/demo/demo_main.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/demo/vlp_model.py` & `yang-vlp-0.2.20/vlppy/demo/vlp_model.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/error/error.py` & `yang-vlp-0.2.20/vlppy/error/error.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/io/io.py` & `yang-vlp-0.2.20/vlppy/io/io.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/model/__pycache__/filter.cpython-39.pyc` & `yang-vlp-0.2.20/vlppy/model/__pycache__/filter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/model/__pycache__/led.cpython-39.pyc` & `yang-vlp-0.2.20/vlppy/model/__pycache__/led.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/model/__pycache__/pd.cpython-39.pyc` & `yang-vlp-0.2.20/vlppy/model/__pycache__/pd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/model/__pycache__/room.cpython-39.pyc` & `yang-vlp-0.2.20/vlppy/model/__pycache__/room.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/model/led.py` & `yang-vlp-0.2.20/vlppy/model/led.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/model/pd.py` & `yang-vlp-0.2.20/vlppy/model/pd.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,16 @@
             pos: 倾斜PD位置
             Nv: 倾斜PD的法向量
         """
         if len(center_tp_pos) == 3:
             x0, y0, z0 = center_tp_pos
         else:
             x0, y0, z0 = np.split(center_tp_pos, indices_or_sections=3, axis=-1)
-        x0, y0, z0 = x0.flatten(), y0.flatten(), z0.flatten()
-
+        x0, y0, z0 = np.reshape(x0,-1), np.reshape(y0,-1), np.reshape(z0,-1)
+        
         # 角度制转弧度制
         alpha_rad, beta_rad = np.radians([alpha, beta])
 
         # 倾斜PD和中心参考点位置关系
         xr = x0 + l * np.cos(alpha_rad) * np.cos(beta_rad) 
         yr = y0 + l * np.sin(alpha_rad) * np.cos(beta_rad)
         zr = z0 + l * np.sin(beta_rad)
@@ -97,15 +97,15 @@
         if not 0 <= beta_rad <= 90: # 限定
             raise VLPValueRangeError(beta, 0, 90)
         
         if len(center_tp_pos) == 3:
             x0, y0, z0 = center_tp_pos
         else:
             x0, y0, z0 = np.split(center_tp_pos, indices_or_sections=3, axis=-1)
-        x0, y0, z0 = x0.flatten(), y0.flatten(), z0.flatten()
+        x0, y0, z0 = np.reshape(x0,-1), np.reshape(y0,-1), np.reshape(z0,-1)
         
         # 倾斜PD位置
         xr = x0 + a * np.cos(alpha_rad) * np.sin(beta_rad)
         yr = y0 + b * np.sin(alpha_rad) * np.sin(beta_rad)
         zr = z0 - c * (1 - np.cos(beta_rad))
 
         # alpha_rad: PD的方位角和PD倾斜面的摆放角相等
```

### Comparing `yang-vlp-0.2.19/vlppy/model/room.py` & `yang-vlp-0.2.20/vlppy/model/room.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,20 +58,20 @@
         """
         if wall not in (0,1,2,3,4,5):
             raise VLPValueError(wall,0,1,2,3,4,5)
         (xo, yo, zo) = self.origin # 原点
         gx, gy, gz = gap # 墙壁网格划分的间隔
 
         if wall in (0,5):    # 地板或天花板
-            x = np.arange(gx, self.length-gx+1e-3, gx)  # 不取靠近墙壁的点（符合实际环境）
+            x = np.arange(gx, self.length-gx+1e-3, gx)  # 不取靠近墙壁的点 
             y = np.arange(gy, self.width-gy+1e-3, gy) 
             z = 0 if wall == 0 else self.height 
             Xw, Yw, Zw = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 地板和天花板平面建立二维网格矩阵 
-        elif wall in (1,3): #前后墙  
-            x = np.arange(0, self.length+1e-3, gx) 
+        elif wall in (1,3): #前后墙    
+            x = np.arange(0, self.length+1e-3, gx)  
             y = 0 if wall == 1 else self.width 
             z = np.arange(self.rp_height[0], self.rp_height[1]+1e-3, gz) 
             Xw, Yw, Zw = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 前后墙面建立二维网格矩阵 
         else:  #左右墙
             x = self.length if wall == 2 else 0
             y = np.arange(0, self.width+1e-3, gy) 
             z = np.arange(self.rp_height[0], self.rp_height[1]+1e-3, gz) 
@@ -232,15 +232,15 @@
     def height(self, h):
         """设置房间高度
         """
         self._height = h
 
     @property
     def size(self) -> tuple:
-        """获取房间大小
+        """获取房间大小(length, width, height)
         """
         return (self.length, self.width, self.height)
 
     @size.setter
     def size(self, s:tuple):
         """设置房间大小
         """
@@ -329,15 +329,15 @@
 
     @property
     def tp_raw_pos(self) -> tuple:
         """获取测试点位置
             shape:(l*w*h)、(l*w*h)、(l*w*h)
         """
         xr, yr, zr = self.tp_grid
-        xr, yr, zr = xr.flatten(), yr.flatten(), zr.flatten()
+        xr, yr, zr = np.reshape(xr,-1), np.reshape(yr,-1), np.reshape(zr,-1)
         return (xr, yr, zr) 
 
     @property
     def wall_gap(self):
         """获取墙壁划分网格的间隔 
         """
         return self._wall_gap
```

### Comparing `yang-vlp-0.2.19/vlppy/setting/__pycache__/json_setting.cpython-39.pyc` & `yang-vlp-0.2.20/vlppy/setting/__pycache__/json_setting.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/setting/json_setting.py` & `yang-vlp-0.2.20/vlppy/setting/json_setting.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/setting/settings.json` & `yang-vlp-0.2.20/vlppy/setting/settings.json`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/signal/filter.py` & `yang-vlp-0.2.20/vlppy/signal/filter.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/signal/plot.py` & `yang-vlp-0.2.20/vlppy/signal/plot.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/vlppy/vis/vis.py` & `yang-vlp-0.2.20/vlppy/vis/vis.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.19/yang_vlp.egg-info/PKG-INFO` & `yang-vlp-0.2.20/yang_vlp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.19
+Version: 0.2.20
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `yang-vlp-0.2.19/yang_vlp.egg-info/SOURCES.txt` & `yang-vlp-0.2.20/yang_vlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

