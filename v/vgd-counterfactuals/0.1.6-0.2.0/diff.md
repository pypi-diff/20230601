# Comparing `tmp/vgd_counterfactuals-0.1.6.tar.gz` & `tmp/vgd_counterfactuals-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vgd_counterfactuals-0.1.6.tar", max compression
+gzip compressed data, was "vgd_counterfactuals-0.2.0.tar", max compression
```

## Comparing `vgd_counterfactuals-0.1.6.tar` & `vgd_counterfactuals-0.2.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.1.6/LICENSE
--rwxr-xr-x   0        0        0     6577 2023-05-26 18:55:18.237103 vgd_counterfactuals-0.1.6/README.rst
--rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.1.6/banner.png
--rwxr-xr-x   0        0        0     1514 2023-05-26 18:55:18.229103 vgd_counterfactuals-0.1.6/pyproject.toml
--rwxr-xr-x   0        0        0        5 2023-05-26 18:55:18.237103 vgd_counterfactuals-0.1.6/vgd_counterfactuals/VERSION
--rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.1.6/vgd_counterfactuals/__init__.py
--rw-r--r--   0        0        0    11840 2023-05-26 18:53:16.524275 vgd_counterfactuals-0.1.6/vgd_counterfactuals/base.py
--rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/cli.py
--rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/00_quickstart.py
--rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/01_visualization.py
--rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/README.rst
--rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/__init__.py
--rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
--rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
--rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
--rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
--rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
--rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
--rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
--rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
--rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
--rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
--rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
--rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
--rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
--rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
--rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
--rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
--rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
--rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
--rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
--rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
--rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
--rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
--rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
--rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
--rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
--rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
--rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
--rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/README.rst
--rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/results/README.rst
--rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/template_experiment.py
--rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/template_experiment_sub.py
--rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/__init__.py
--rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     8355 2023-05-26 08:30:52.863182 vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
--rw-r--r--   0        0        0    11111 2023-05-26 08:30:51.243165 vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/molecules.py
--rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/smiles_one_step_changes.py
--rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.1.6/vgd_counterfactuals/templates/article.tex.j2
--rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.1.6/vgd_counterfactuals/testing.py
--rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.1.6/vgd_counterfactuals/utils.py
--rw-r--r--   0        0        0     3370 2023-05-01 16:09:36.020519 vgd_counterfactuals-0.1.6/vgd_counterfactuals/visualization.py
--rw-r--r--   0        0        0     7622 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.1.6/PKG-INFO
+-rwxr-xr-x   0        0        0     1070 2023-04-28 11:58:50.318682 vgd_counterfactuals-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0     6577 2023-06-01 13:25:42.788509 vgd_counterfactuals-0.2.0/README.rst
+-rw-r--r--   0        0        0    75715 2023-04-30 10:49:40.133365 vgd_counterfactuals-0.2.0/banner.png
+-rwxr-xr-x   0        0        0     1540 2023-06-01 13:25:42.776508 vgd_counterfactuals-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0        5 2023-06-01 13:25:42.788509 vgd_counterfactuals-0.2.0/vgd_counterfactuals/VERSION
+-rwxr-xr-x   0        0        0       39 2023-04-30 10:06:54.410920 vgd_counterfactuals-0.2.0/vgd_counterfactuals/__init__.py
+-rw-r--r--   0        0        0    12166 2023-06-01 10:10:57.254190 vgd_counterfactuals-0.2.0/vgd_counterfactuals/base.py
+-rwxr-xr-x   0        0        0     5290 2023-04-28 11:58:50.338682 vgd_counterfactuals-0.2.0/vgd_counterfactuals/cli.py
+-rw-r--r--   0        0        0     1950 2023-05-01 15:19:29.825180 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/00_quickstart.py
+-rw-r--r--   0        0        0     3422 2023-05-01 15:37:09.041204 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/01_visualization.py
+-rw-r--r--   0        0        0      471 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/README.rst
+-rw-r--r--   0        0        0        0 2023-05-01 14:39:31.031283 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/__init__.py
+-rw-r--r--   0        0        0      847 2023-05-01 15:19:38.033191 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py
+-rw-r--r--   0        0        0     2191 2023-05-01 15:19:38.025191 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/code.py
+-rw-r--r--   0        0        0      778 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json
+-rw-r--r--   0        0        0    17914 2023-05-01 15:19:39.289193 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json
+-rw-r--r--   0        0        0    17705 2023-05-01 15:19:38.169191 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png
+-rw-r--r--   0        0        0      968 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json
+-rw-r--r--   0        0        0    18723 2023-05-01 15:19:38.281191 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png
+-rw-r--r--   0        0        0      975 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json
+-rw-r--r--   0        0        0    19578 2023-05-01 15:19:38.393192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png
+-rw-r--r--   0        0        0      974 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json
+-rw-r--r--   0        0        0    18471 2023-05-01 15:19:38.501192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png
+-rw-r--r--   0        0        0      972 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json
+-rw-r--r--   0        0        0    19414 2023-05-01 15:19:38.617192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png
+-rw-r--r--   0        0        0      978 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json
+-rw-r--r--   0        0        0    20003 2023-05-01 15:19:38.729192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png
+-rw-r--r--   0        0        0      971 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json
+-rw-r--r--   0        0        0    23908 2023-05-01 15:19:38.841192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png
+-rw-r--r--   0        0        0      970 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json
+-rw-r--r--   0        0        0    19642 2023-05-01 15:19:38.953192 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png
+-rw-r--r--   0        0        0      977 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json
+-rw-r--r--   0        0        0    19682 2023-05-01 15:19:39.065193 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png
+-rw-r--r--   0        0        0      969 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json
+-rw-r--r--   0        0        0    20380 2023-05-01 15:19:39.177193 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png
+-rw-r--r--   0        0        0   221293 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf
+-rw-r--r--   0        0        0        2 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_data.json
+-rw-r--r--   0        0        0      555 2023-05-01 15:19:40.353194 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json
+-rw-r--r--   0        0        0     1328 2023-05-01 15:19:40.357194 vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log
+-rw-r--r--   0        0        0     1334 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.2.0/vgd_counterfactuals/experiments/README.rst
+-rw-r--r--   0        0        0      209 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.2.0/vgd_counterfactuals/experiments/results/README.rst
+-rwxr-xr-x   0        0        0      729 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.2.0/vgd_counterfactuals/experiments/template_experiment.py
+-rw-r--r--   0        0        0      614 2023-04-28 11:58:50.342682 vgd_counterfactuals-0.2.0/vgd_counterfactuals/experiments/template_experiment_sub.py
+-rw-r--r--   0        0        0        0 2023-04-28 12:00:41.971495 vgd_counterfactuals-0.2.0/vgd_counterfactuals/generate/__init__.py
+-rw-r--r--   0        0        0      176 2023-04-30 07:11:09.422132 vgd_counterfactuals-0.2.0/vgd_counterfactuals/generate/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     9194 2023-06-01 10:01:20.429985 vgd_counterfactuals-0.2.0/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc
+-rw-r--r--   0        0        0    13613 2023-06-01 10:01:19.881981 vgd_counterfactuals-0.2.0/vgd_counterfactuals/generate/molecules.py
+-rwxr-xr-x   0        0        0    19773 2023-04-14 06:32:11.000000 vgd_counterfactuals-0.2.0/vgd_counterfactuals/generate/smiles_one_step_changes.py
+-rwxr-xr-x   0        0        0      997 2023-04-28 11:58:50.346682 vgd_counterfactuals-0.2.0/vgd_counterfactuals/templates/article.tex.j2
+-rw-r--r--   0        0        0      490 2023-05-01 15:26:26.262286 vgd_counterfactuals-0.2.0/vgd_counterfactuals/testing.py
+-rwxr-xr-x   0        0        0     5201 2023-05-01 15:30:16.327226 vgd_counterfactuals-0.2.0/vgd_counterfactuals/utils.py
+-rw-r--r--   0        0        0     3931 2023-06-01 08:03:40.743915 vgd_counterfactuals-0.2.0/vgd_counterfactuals/visualization.py
+-rw-r--r--   0        0        0     7661 1970-01-01 00:00:00.000000 vgd_counterfactuals-0.2.0/PKG-INFO
```

### Comparing `vgd_counterfactuals-0.1.6/LICENSE` & `vgd_counterfactuals-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/README.rst` & `vgd_counterfactuals-0.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.6-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.2.0-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

### Comparing `vgd_counterfactuals-0.1.6/banner.png` & `vgd_counterfactuals-0.2.0/banner.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/pyproject.toml` & `vgd_counterfactuals-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.2.0b2"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vgd_counterfactuals"
-version = "0.1.6"
+version = "0.2.0"
 description = "Counterfactual explanations for GNNs based on the visual graph dataset format"
 license = "MIT license"
 authors = ["Jonas Teufel <jonseb1998@gmail.com>"]
 maintainers = ["Jonas Teufel <jonseb1998@gmail.com>"]
 readme = "README.rst"
 keywords = ["graph neural networks", "counterfactuals", "explainable AI"]
 packages = [
@@ -34,14 +34,15 @@
 matplotlib = ">=3.5.3"
 numpy = ">=1.23.2"
 python-decouple = ">=3.6"
 poetry-bumpversion = ">=0.3.0"
 rdkit = ">=2022.9.5"
 pycomex = ">=0.9.2"
 visual_graph_datasets = ">=0.11.0"
+dimorphite-dl = ">=1.3.2"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=7.1.3"
 poetry-bumpversion = ">=0.3.0"
 
 [tool.poetry_bumpversion.file."vgd_counterfactuals/VERSION"]
 search = "{current_version}"
```

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/base.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -102,16 +102,16 @@
         graph = self.processing.process(original)
         original_prediction = self.model.predict_graph(graph)
 
         # 26.05.23 - Instead of having the implementation here, it is now in its own function which will
         # return a list of all the valid k-edit neighbors.
         # Moving this had two purposes: (1) it's cleaner code and (2) now I have the potential to cache
         # the results, which I have realized is a functionality I'll need in the future.
-        neighbors: t.List[tv.DomainRepr] = self.get_neighbors(original, k_neighborhood)
-        graphs = [self.processing.process(value) for value in neighbors]
+        neighbors: t.List[dict] = self.get_neighbors(original, k_neighborhood)
+        graphs = [self.processing.process(data['value']) for data in neighbors]
 
         # 16.05.23 - I have noticed that for larger neighborhood sizes there can be A LOT of counterfactuals
         # so many that a model cannot possibly predict them all at once without causing a memory overflow
         # for the resulting vector. This is why we need to process this in a batched manner now!
         # NOTE: One might think that this could be parallelized as well, like the counterfactual generation
         # itself, but that would actually not work because we cant serialize the model to send it to another
         # process and loading the model from memory takes so long that it would not make sense to do that
@@ -137,25 +137,28 @@
         # If there are less neighbors in total than the desired number of results, we can only
         # provide as many as there are.
         num = min(len(sorted_results), k_results)
         top_results = sorted_results[:num]
 
         # For these top results we now want to create a visual graph dataset folder so that they can be
         # visualized and processed further
-        for index, (distance, value, prediction, graph) in enumerate(top_results):
+        for index, (distance, data, prediction, graph) in enumerate(top_results):
             self.processing.create(
-                value,
+                data['value'],
                 index=str(index),
-                name=value,
+                name=data['value'],
                 output_path=path,
                 width=image_width,
                 height=image_height,
                 additional_metadata={
-                    'distance': distance,
-                    'prediction': prediction
+                    'distance':             distance,
+                    'prediction':           prediction,
+                    'modification_type':    data['type'],
+                    'original_indices':     data['org'],
+                    'modified_indices':     data['mod'],
                 },
                 additional_graph_data={},
             )
 
         metadata_map, index_data_map = load_visual_graph_dataset(
             path=path,
             logger=self.logger,
@@ -164,27 +167,31 @@
         return index_data_map
 
     def get_neighbors(self, original: tv.DomainRepr, k_neighborhood):
         # Based on the original we need ALL possible neighbors of this in a k-neighborhood
         # 16.05.23 - For a larger neighborhood size the number of counterfactuals increases exponentially
         # and generating them takes forever. That is why we use multiprocessing to do the generation in
         # parallel and hopefully be a bit faster.
-        neighbors_set = {original}
+        neighbors = [{'value': original, 'type': 'none', 'org': (0, 0), 'mod': (0, 0)}]
         if self.num_processes is not None:
             with multiprocessing.Pool(processes=self.num_processes) as pool:
                 for i in range(k_neighborhood):
-                    neighbors_set = set(itertools.chain(*pool.map(self.neighborhood_func, neighbors_set)))
+                    neighbors += list(itertools.chain.from_iterable(
+                        pool.map(self.neighborhood_func, [data['value'] for data in neighbors])
+                    ))
+
         else:
             for i in range(k_neighborhood):
-                neighbors = []
-                for value in neighbors_set:
-                    neighbors += self.neighborhood_func(value)
-                neighbors_set = neighbors_set.union(set(neighbors))
+                neighbors_local = []
+                for data in neighbors:
+                    neighbors_local += self.neighborhood_func(data['value'])
+
+                neighbors += neighbors_local
 
-        return list(neighbors_set)
+        return neighbors
 
     def create(self,
                value: tv.DomainRepr,
                path: str,
                index: str,
                image_width=DEFAULT_IMAGE_WIDTH,
                image_height=DEFAULT_IMAGE_HEIGHT,
```

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/cli.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/cli.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/00_quickstart.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/00_quickstart.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/01_visualization.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/01_visualization.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/analysis.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/code.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/code.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/-1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/0.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/1.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/2.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/3.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/4.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/5.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/6.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/7.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/8.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals/9.png`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/counterfactuals.pdf`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_meta.json`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/examples/results/01_visualization/debug/experiment_out.log`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/README.rst` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/experiments/README.rst`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/template_experiment.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/experiments/template_experiment.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/experiments/template_experiment_sub.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/experiments/template_experiment_sub.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/generate/__pycache__/molecules.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 08:30:51 2023 UTC, .py size: 11111 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 24% similar despite different names*

```diff
@@ -1,523 +1,575 @@
-00000000: 6f0d 0d0a 0000 0000 3b6e 7064 672b 0000  o.......;npdg+..
+00000000: 6f0d 0d0a 0000 0000 6f6c 7864 2d35 0000  o.......olxd-5..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000b 0000 0040 0000 0073 8601 0000 6400  .....@...s....d.
+00000020: 000e 0000 0040 0000 0073 a401 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c05 6d07 5a07  m.Z...d.d.l.m.Z.
-00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6406  ..d.d.l.m.Z...d.
-00000070: 6407 6408 6409 640a 6408 640b 9c06 5a0a  d.d.d.d.d.d...Z.
-00000080: 0900 642a 640c 6504 6a0b 640d 6504 6a0b  ..d*d.e.j.d.e.j.
-00000090: 640e 650c 640f 6502 6a0d 650e 650e 6602  d.e.d.e.j.e.e.f.
-000000a0: 1900 6608 6410 6411 8405 5a0f 642b 6413  ..f.d.d...Z.d+d.
-000000b0: 6504 6a0b 6414 650e 6604 6415 6416 8405  e.j.d.e.f.d.d...
-000000c0: 5a10 642c 6413 6504 6a0b 6414 650e 6604  Z.d,d.e.j.d.e.f.
-000000d0: 6418 6419 8405 5a11 650a 6510 6511 6602  d.d...Z.e.e.e.f.
-000000e0: 6602 641a 650e 641b 6502 6a12 6502 6a13  f.d.e.d.e.j.e.j.
-000000f0: 6504 6a0b 6701 6514 6602 1900 1900 640f  e.j.g.e.f.....d.
-00000100: 6502 6a15 650e 1900 6606 641c 641d 8405  e.j.e...f.d.d...
-00000110: 5a16 642d 6413 6504 6a0b 641f 650c 640f  Z.d-d.e.j.d.e.d.
-00000120: 6517 6606 6420 6421 8405 5a18 6413 6504  e.f.d d!..Z.d.e.
-00000130: 6a0b 6422 6502 6a19 650e 650c 6602 1900  j.d"e.j.e.e.f...
-00000140: 6423 6502 6a19 650c 6502 6a15 650c 1900  d#e.j.e.e.j.e...
-00000150: 6602 1900 640f 6502 6a1a 650e 1900 6608  f...d.e.j.e...f.
-00000160: 6424 6425 8404 5a1b 6413 6504 6a0b 6423  d$d%..Z.d.e.j.d#
-00000170: 6502 6a19 650c 6502 6a15 650c 1900 6602  e.j.e.e.j.e...f.
-00000180: 1900 640f 6502 6a1a 650e 1900 6606 6426  ..d.e.j.e...f.d&
-00000190: 6427 8404 5a1c 6413 6504 6a0b 640f 6502  d'..Z.d.e.j.d.e.
-000001a0: 6a1a 650e 1900 6604 6428 6429 8404 5a1d  j.e...f.d(d)..Z.
-000001b0: 6401 5300 292e e900 0000 004e 2901 da04  d.S.)......N)...
-000001c0: 4368 656d 2901 da06 7264 464d 4353 2901  Chem)...rdFMCS).
-000001d0: da07 416c 6c43 6865 6d29 01da 0b69 6e76  ..AllChem)...inv
-000001e0: 6572 745f 6469 6374 e904 0000 00e9 0500  ert_dict........
-000001f0: 0000 e906 0000 00e9 0100 0000 e907 0000  ................
-00000200: 0029 06da 0143 da01 4eda 014f da01 46da  .)...C..N..O..F.
-00000210: 0243 6cda 0153 da04 6d6f 6c31 da04 6d6f  .Cl..S..mol1..mo
-00000220: 6c32 da06 7261 6469 7573 da06 7265 7475  l2..radius..retu
-00000230: 726e 6303 0000 0000 0000 0000 0000 000d  rnc.............
-00000240: 0000 0007 0000 0003 0000 0073 2c01 0000  ...........s,...
-00000250: 7c00 7c01 6602 4400 5d19 7d03 7c03 a000  |.|.f.D.].}.|...
-00000260: a100 4400 5d12 7d04 7401 6401 6402 8400  ..D.].}.t.d.d...
-00000270: 7c04 a002 a100 4400 8301 8301 7d05 7c04  |.....D.....}.|.
-00000280: a003 7c05 a101 0100 710a 7104 7404 6a05  ..|.....q.q.t.j.
-00000290: 7c00 7c01 6702 7404 6a06 6a07 6403 8d02  |.|.g.t.j.j.d...
-000002a0: 7d06 7408 a009 7c06 6a0a a101 7d07 6700  }.t...|.j...}.g.
-000002b0: 7d08 7c00 7c01 6602 4400 5d5e 7d03 7c03  }.|.|.f.D.]^}.|.
-000002c0: a00b 7c07 a101 8901 740c 8700 8701 6602  ..|.....t.....f.
-000002d0: 6404 6405 8408 7c03 a000 a100 4400 8301  d.d...|.....D...
-000002e0: 8301 7d09 740d 7c02 8301 4400 5d20 7d0a  ..}.t.|...D.] }.
-000002f0: 6700 7d0b 7c09 4400 5d12 7d0c 7c03 a00e  g.}.|.D.].}.|...
-00000300: 7c0c a101 7d04 7c0b 6406 6405 8400 7c04  |...}.|.d.d...|.
-00000310: a00f a100 4400 8301 3700 7d0b 7154 7c09  ....D...7.}.qT|.
-00000320: a010 740c 7c0b 8301 a101 0100 714e 7c03  ..t.|.......qN|.
-00000330: a000 a100 4400 5d07 7d04 7c04 a003 6407  ....D.].}.|...d.
-00000340: a101 0100 7173 7411 7c09 8301 6407 6b03  ....qst.|...d.k.
-00000350: 728e 7c08 a012 7408 6a13 7c03 7414 7c09  r.|...t.j.|.t.|.
-00000360: 8301 6408 8d02 a101 0100 7135 7c08 a012  ..d.......q5|...
-00000370: 6409 a101 0100 7135 7c08 5300 290a 7a05  d.....q5|.S.).z.
-00000380: 0a20 2020 2063 0100 0000 0000 0000 0000  .    c..........
-00000390: 0000 0200 0000 0400 0000 7300 0000 7320  ..........s...s 
-000003a0: 0000 0081 007c 005d 0b7d 017c 01a0 00a1  .....|.].}.|....
-000003b0: 007c 01a0 01a1 0017 0056 0001 0071 0264  .|.......V...q.d
-000003c0: 0053 00a9 014e 2902 da0b 4765 7442 6f6e  .S...N)...GetBon
-000003d0: 6454 7970 65da 0a47 6574 426f 6e64 4469  dType..GetBondDi
-000003e0: 7229 02da 022e 30da 0462 6f6e 64a9 0072  r)....0..bond..r
-000003f0: 1a00 0000 fa54 2f6d 6564 6961 2f73 7364  .....T/media/ssd
-00000400: 2f50 726f 6772 616d 6d69 6e67 2f76 6764  /Programming/vgd
-00000410: 5f63 6f75 6e74 6572 6661 6374 7561 6c73  _counterfactuals
-00000420: 2f76 6764 5f63 6f75 6e74 6572 6661 6374  /vgd_counterfact
-00000430: 7561 6c73 2f67 656e 6572 6174 652f 6d6f  uals/generate/mo
-00000440: 6c65 6375 6c65 732e 7079 da09 3c67 656e  lecules.py..<gen
-00000450: 6578 7072 3e1e 0000 0073 0400 0000 0280  expr>....s......
-00000460: 1e00 7a27 6d6f 6c65 6375 6c65 5f64 6966  ..z'molecule_dif
-00000470: 6665 7265 6e63 6573 2e3c 6c6f 6361 6c73  ferences.<locals
-00000480: 3e2e 3c67 656e 6578 7072 3e29 01da 0b61  >.<genexpr>)...a
-00000490: 746f 6d43 6f6d 7061 7265 6301 0000 0000  tomComparec.....
-000004a0: 0000 0000 0000 0002 0000 0004 0000 0013  ................
-000004b0: 0000 0073 2000 0000 6700 7c00 5d0c 7d01  ...s ...g.|.].}.
-000004c0: 7c01 a000 a100 0400 8900 8801 7601 7202  |...........v.r.
-000004d0: 8800 9102 7102 5300 721a 0000 00a9 01da  ....q.S.r.......
-000004e0: 0647 6574 4964 78a9 0272 1800 0000 da04  .GetIdx..r......
-000004f0: 6174 6f6d a902 da05 696e 6465 78da 056d  atom....index..m
-00000500: 6174 6368 721a 0000 0072 1b00 0000 da0a  atchr....r......
-00000510: 3c6c 6973 7463 6f6d 703e 2a00 0000 7302  <listcomp>*...s.
-00000520: 0000 0020 007a 286d 6f6c 6563 756c 655f  ... .z(molecule_
-00000530: 6469 6666 6572 656e 6365 732e 3c6c 6f63  differences.<loc
-00000540: 616c 733e 2e3c 6c69 7374 636f 6d70 3e63  als>.<listcomp>c
-00000550: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000560: 0400 0000 5300 0000 7314 0000 0067 007c  ....S...s....g.|
-00000570: 005d 067d 017c 01a0 00a1 0091 0271 0253  .].}.|.......q.S
-00000580: 0072 1a00 0000 721e 0000 0029 0272 1800  .r....r....).r..
-00000590: 0000 da01 6172 1a00 0000 721a 0000 0072  ....ar....r....r
-000005a0: 1b00 0000 7225 0000 002f 0000 00f3 0200  ....r%.../......
-000005b0: 0000 1400 7201 0000 0029 01da 0a61 746f  ....r....)...ato
-000005c0: 6d73 546f 5573 65da 0029 15da 0847 6574  msToUse..)...Get
-000005d0: 4174 6f6d 73da 0373 756d da08 4765 7442  Atoms..sum..GetB
-000005e0: 6f6e 6473 da0a 5365 7449 736f 746f 7065  onds..SetIsotope
-000005f0: 7203 0000 00da 0746 696e 644d 4353 da0b  r......FindMCS..
-00000600: 4174 6f6d 436f 6d70 6172 65da 0f43 6f6d  AtomCompare..Com
-00000610: 7061 7265 4973 6f74 6f70 6573 7202 0000  pareIsotopesr...
-00000620: 00da 0d4d 6f6c 4672 6f6d 536d 6172 7473  ...MolFromSmarts
-00000630: da0c 736d 6172 7473 5374 7269 6e67 da11  ..smartsString..
-00000640: 4765 7453 7562 7374 7275 6374 4d61 7463  GetSubstructMatc
-00000650: 68da 0373 6574 da05 7261 6e67 65da 0e47  h..set..range..G
-00000660: 6574 4174 6f6d 5769 7468 4964 78da 0c47  etAtomWithIdx..G
-00000670: 6574 4e65 6967 6862 6f72 73da 0675 7064  etNeighbors..upd
-00000680: 6174 65da 036c 656e da06 6170 7065 6e64  ate..len..append
-00000690: da13 4d6f 6c46 7261 676d 656e 7454 6f53  ..MolFragmentToS
-000006a0: 6d69 6c65 73da 046c 6973 7429 0d72 1100  miles..list).r..
-000006b0: 0000 7212 0000 0072 1300 0000 da03 6d6f  ..r....r......mo
-000006c0: 6c72 2100 0000 da05 7661 6c75 65da 036d  lr!.....value..m
-000006d0: 6373 da13 636f 6d6d 6f6e 5f73 7562 7374  cs..common_subst
-000006e0: 7275 6374 7572 65da 0772 6573 756c 7473  ructure..results
-000006f0: da0b 6e6f 6e5f 6d61 7463 6865 73da 0172  ..non_matches..r
-00000700: da09 6e65 6967 6862 6f72 73da 0a61 746f  ..neighbors..ato
-00000710: 6d5f 696e 6465 7872 1a00 0000 7222 0000  m_indexr....r"..
-00000720: 0072 1b00 0000 da14 6d6f 6c65 6375 6c65  .r......molecule
-00000730: 5f64 6966 6665 7265 6e63 6573 1600 0000  _differences....
-00000740: 7334 0000 000c 060c 0116 010c 0102 fe04  s4..............
-00000750: 0406 0106 0106 fe0c 0404 020c 010a 011c  ................
-00000760: 010c 0104 0108 010a 0118 0110 020c 020c  ................
-00000770: 010c 021a 010c 0204 0272 4600 0000 fa0e  .........rF.....
-00000780: 2a31 3d2a 2a32 3d2a 2a3d 2a31 2a32 723d  *1=**2=**=*1*2r=
-00000790: 0000 00da 0770 6174 7465 726e 6302 0000  .....patternc...
-000007a0: 0000 0000 0000 0000 0004 0000 0003 0000  ................
-000007b0: 0043 0000 00f3 1800 0000 7400 a001 7c01  .C........t...|.
-000007c0: a101 7d02 7c00 a002 7c02 a101 7d03 7c03  ..}.|...|...}.|.
-000007d0: 5300 2901 7a83 0a20 2020 2043 6865 636b  S.).z..    Check
-000007e0: 7320 6966 2074 6865 2067 6976 656e 206d  s if the given m
-000007f0: 6f6c 6563 756c 6520 6060 6d6f 6c60 6020  olecule ``mol`` 
-00000800: 6973 2061 2062 7269 6467 6520 6865 6164  is a bridge head
-00000810: 2063 6172 626f 6e20 7374 7275 6374 7572   carbon structur
-00000820: 6520 7768 6963 6820 6170 7061 7265 6e74  e which apparent
-00000830: 6c79 2064 6f65 7320 6e6f 740a 2020 2020  ly does not.    
-00000840: 6170 7065 6172 2069 6e20 6368 656d 6973  appear in chemis
-00000850: 7472 792e 0a20 2020 20a9 0372 0200 0000  try..    ..r....
-00000860: 7231 0000 00da 1148 6173 5375 6273 7472  r1.....HasSubstr
-00000870: 7563 744d 6174 6368 a904 723d 0000 0072  uctMatch..r=...r
-00000880: 4800 0000 da06 736d 6172 7473 da08 6973  H.....smarts..is
-00000890: 5f6d 6174 6368 721a 0000 0072 1a00 0000  _matchr....r....
-000008a0: 721b 0000 00da 1569 735f 6272 6964 6765  r......is_bridge
-000008b0: 5f68 6561 645f 6361 7262 6f6e 3e00 0000  _head_carbon>...
-000008c0: 7306 0000 000a 050a 0104 0172 4f00 0000  s..........rO...
-000008d0: da03 534e 4e63 0200 0000 0000 0000 0000  ..SNNc..........
-000008e0: 0000 0400 0000 0300 0000 4300 0000 7249  ..........C...rI
-000008f0: 0000 0072 1500 0000 724a 0000 0072 4c00  ...r....rJ...rL.
-00000900: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
-00000910: 00da 1b69 735f 6e69 7472 6f67 656e 5f6e  ...is_nitrogen_n
-00000920: 6974 726f 6765 6e5f 7375 6c66 7572 4800  itrogen_sulfurH.
-00000930: 0000 7306 0000 000a 010a 0104 0172 5100  ..s..........rQ.
-00000940: 0000 da06 736d 696c 6573 da0b 6d6f 6c5f  ....smiles..mol_
-00000950: 6669 6c74 6572 7363 0300 0000 0000 0000  filtersc........
-00000960: 0000 0000 0600 0000 0700 0000 0300 0000  ................
-00000970: 738c 0000 0074 0083 007d 0374 01a0 027c  s....t...}.t...|
-00000980: 00a1 0189 0074 0388 0083 017d 047c 03a0  .....t.....}.|..
-00000990: 0474 0588 007c 017c 0464 018d 03a1 0101  .t...|.|.d......
-000009a0: 007c 03a0 0474 0688 007c 0464 028d 02a1  .|...t...|.d....
-000009b0: 0101 007c 03a0 0474 0788 0064 038d 01a1  ...|...t...d....
-000009c0: 0101 0067 007d 057c 0344 005d 187d 0074  ...g.}.|.D.].}.t
-000009d0: 01a0 027c 00a1 0189 0074 0887 0066 0164  ...|.....t...f.d
-000009e0: 0464 0584 087c 0244 0083 0183 0172 3e71  .d...|.D.....r>q
-000009f0: 2b7c 05a0 097c 00a1 0101 0071 2b7c 0553  +|...|.....q+|.S
-00000a00: 0029 0661 b103 0000 0a20 2020 2047 6976  .).a.....    Giv
-00000a10: 656e 2061 2060 6073 6d69 6c65 7360 6020  en a ``smiles`` 
-00000a20: 7265 7072 6573 656e 7461 7469 6f6e 206f  representation o
-00000a30: 6620 6120 6d6f 6c65 6375 6c65 2c20 7468  f a molecule, th
-00000a40: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
-00000a50: 2072 6574 7572 6e20 6120 6c69 7374 206f   return a list o
-00000a60: 6620 7468 6520 534d 494c 4553 0a20 2020  f the SMILES.   
-00000a70: 2072 6570 7265 7365 6e74 6174 696f 6e73   representations
-00000a80: 206f 6620 616c 6c20 7468 6520 7661 6c69   of all the vali
-00000a90: 6420 6d6f 6c65 6375 6c65 7320 7769 7468  d molecules with
-00000aa0: 696e 2061 2031 2d65 6469 7420 6e65 6967  in a 1-edit neig
-00000ab0: 6862 6f72 686f 6f64 2e20 4f70 7469 6f6e  hborhood. Option
-00000ac0: 616c 6c79 2c20 6120 6c69 7374 206f 6620  ally, a list of 
-00000ad0: 626f 6f6c 6561 6e0a 2020 2020 6675 6e63  boolean.    func
-00000ae0: 7469 6f6e 7320 6361 6e20 6265 2070 726f  tions can be pro
-00000af0: 7669 6465 6420 666f 7220 6060 6d6f 6c5f  vided for ``mol_
-00000b00: 6669 6c74 6572 7360 6020 746f 2066 7572  filters`` to fur
-00000b10: 7468 6572 206c 696d 6974 2074 6865 206b  ther limit the k
-00000b20: 696e 6473 206f 6620 6d6f 6c65 6375 6c65  inds of molecule
-00000b30: 7320 696e 636c 7564 6564 2069 6e20 7468  s included in th
-00000b40: 650a 2020 2020 7265 7375 6c74 2e0a 0a20  e.    result... 
-00000b50: 2020 203a 7061 7261 6d20 736d 696c 6573     :param smiles
-00000b60: 3a20 5468 6520 534d 494c 4553 2073 7472  : The SMILES str
-00000b70: 696e 6720 7265 7072 6573 656e 7461 7469  ing representati
-00000b80: 6f6e 206f 660a 2020 2020 3a70 6172 616d  on of.    :param
-00000b90: 2061 746f 6d5f 7661 6c65 6e63 655f 6d61   atom_valence_ma
-00000ba0: 703a 2041 2064 6963 7469 6f6e 6172 792c  p: A dictionary,
-00000bb0: 2077 686f 7365 206b 6579 7320 6172 6520   whose keys are 
-00000bc0: 7374 7269 6e67 7320 7468 6174 2069 6465  strings that ide
-00000bd0: 6e74 6966 7920 6174 6f6d 2074 7970 6573  ntify atom types
-00000be0: 206f 6620 7468 6520 534d 494c 4553 0a20   of the SMILES. 
-00000bf0: 2020 2020 2020 206e 6f74 6174 696f 6e20         notation 
-00000c00: 284f 2c20 4e2c 2043 6c20 2e2e 2e29 2061  (O, N, Cl ...) a
-00000c10: 6e64 2074 6865 2076 616c 7565 7320 6172  nd the values ar
-00000c20: 6520 7468 6520 696e 7465 6765 7220 7661  e the integer va
-00000c30: 6c65 6e63 6520 6f66 2074 6865 2063 6f72  lence of the cor
-00000c40: 7265 7370 6f6e 6469 6e67 2061 746f 6d2e  responding atom.
-00000c50: 204f 6e6c 790a 2020 2020 2020 2020 6174   Only.        at
-00000c60: 6f6d 7320 7468 6174 2061 7265 206c 6973  oms that are lis
-00000c70: 7465 6420 696e 2074 6869 7320 6469 6374  ted in this dict
-00000c80: 2077 696c 6c20 6265 2063 6f6e 7369 6465   will be conside
-00000c90: 7265 6420 666f 7220 6564 6974 206f 7065  red for edit ope
-00000ca0: 7261 7469 6f6e 7320 7375 6368 2061 7320  rations such as 
-00000cb0: 6164 6469 6e67 206f 720a 2020 2020 2020  adding or.      
-00000cc0: 2020 7265 706c 6163 696e 6720 616e 6420    replacing and 
-00000cd0: 6174 6f6d 210a 2020 2020 3a70 6172 616d  atom!.    :param
-00000ce0: 206d 6f6c 5f66 696c 7465 7273 3a20 4120   mol_filters: A 
-00000cf0: 6c69 7374 206f 6620 6675 6e63 7469 6f6e  list of function
-00000d00: 7320 7768 6963 6820 6561 6368 2074 616b  s which each tak
-00000d10: 6520 6120 4d6f 6c20 6f62 6a65 6374 2061  e a Mol object a
-00000d20: 7320 696e 7075 7420 616e 6420 7265 7475  s input and retu
-00000d30: 726e 2061 2062 6f6f 6c65 616e 2076 616c  rn a boolean val
-00000d40: 7565 0a20 2020 2020 2020 2074 6f20 6465  ue.        to de
-00000d50: 7465 726d 696e 6520 7768 6574 6865 7220  termine whether 
-00000d60: 7468 6174 2061 746f 6d20 7368 6f75 6c64  that atom should
-00000d70: 2062 6520 6578 636c 7564 6564 2028 5472   be excluded (Tr
-00000d80: 7565 2920 6f72 206e 6f74 2028 4661 6c73  ue) or not (Fals
-00000d90: 6529 2e0a 0a20 2020 203a 7265 7475 726e  e)...    :return
-00000da0: 733a 2041 206c 6973 7420 6f66 2073 7472  s: A list of str
-00000db0: 696e 6773 0a20 2020 2029 0372 3d00 0000  ings.    ).r=...
-00000dc0: da10 6174 6f6d 5f76 616c 656e 6365 5f6d  ..atom_valence_m
-00000dd0: 6170 da18 6672 6565 5f76 616c 656e 6365  ap..free_valence
-00000de0: 5f69 6e64 6963 6573 5f6d 6170 2902 723d  _indices_map).r=
-00000df0: 0000 0072 5500 0000 a901 723d 0000 0063  ...rU.....r=...c
-00000e00: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000e10: 0400 0000 1300 0000 7314 0000 0067 007c  ........s....g.|
-00000e20: 005d 067d 017c 0188 0083 0191 0271 0253  .].}.|.......q.S
-00000e30: 0072 1a00 0000 721a 0000 0029 0272 1800  .r....r....).r..
-00000e40: 0000 da04 6675 6e63 7256 0000 0072 1a00  ....funcrV...r..
-00000e50: 0000 721b 0000 0072 2500 0000 8000 0000  ..r....r%.......
-00000e60: 7227 0000 007a 2467 6574 5f6e 6569 6768  r'...z$get_neigh
-00000e70: 626f 7268 6f6f 642e 3c6c 6f63 616c 733e  borhood.<locals>
-00000e80: 2e3c 6c69 7374 636f 6d70 3e29 0a72 3400  .<listcomp>).r4.
-00000e90: 0000 7202 0000 00da 0d4d 6f6c 4672 6f6d  ..r......MolFrom
-00000ea0: 536d 696c 6573 da14 6765 745f 6672 6565  Smiles..get_free
-00000eb0: 5f76 616c 656e 6365 5f6d 6170 7238 0000  _valence_mapr8..
-00000ec0: 00da 1867 6574 5f76 616c 6964 5f61 746f  ...get_valid_ato
-00000ed0: 6d5f 6164 6469 7469 6f6e 73da 1867 6574  m_additions..get
-00000ee0: 5f76 616c 6964 5f62 6f6e 645f 6164 6469  _valid_bond_addi
-00000ef0: 7469 6f6e 73da 1767 6574 5f76 616c 6964  tions..get_valid
-00000f00: 5f62 6f6e 645f 7265 6d6f 7661 6c73 da03  _bond_removals..
-00000f10: 616e 7972 3a00 0000 2906 7252 0000 0072  anyr:...).rR...r
-00000f20: 5400 0000 7253 0000 00da 0d6e 6569 6768  T...rS.....neigh
-00000f30: 626f 7273 5f73 6574 7255 0000 00da 126e  bors_setrU.....n
-00000f40: 6569 6768 626f 7273 5f66 696c 7465 7265  eighbors_filtere
-00000f50: 6472 1a00 0000 7256 0000 0072 1b00 0000  dr....rV...r....
-00000f60: da10 6765 745f 6e65 6967 6862 6f72 686f  ..get_neighborho
-00000f70: 6f64 4e00 0000 732c 0000 0006 170a 0208  odN...s,........
-00000f80: 0106 0202 0102 0102 0108 fd06 0602 0102  ................
-00000f90: 0108 fe06 0502 0108 ff04 0808 010a 0116  ................
-00000fa0: 0102 010c 0204 0272 6000 0000 e908 0000  .......r`.......
-00000fb0: 00da 0b6d 6178 5f76 616c 656e 6365 6302  ...max_valencec.
-00000fc0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000fd0: 0000 0003 0000 0073 3200 0000 6900 7d02  .......s2...i.}.
-00000fe0: 7400 6401 7c01 8302 4400 5d0f 8900 8700  t.d.|...D.].....
-00000ff0: 6601 6402 6403 8408 7c00 a001 a100 4400  f.d.d...|.....D.
-00001000: 8301 7c02 8800 3c00 7107 7c02 5300 2904  ..|...<.q.|.S.).
-00001010: 4e72 0900 0000 6301 0000 0000 0000 0000  Nr....c.........
-00001020: 0000 0002 0000 0004 0000 0013 0000 0073  ...............s
-00001030: 2000 0000 6700 7c00 5d0c 7d01 7c01 a000   ...g.|.].}.|...
-00001040: a100 8800 6b05 7202 7c01 a001 a100 9102  ....k.r.|.......
-00001050: 7102 5300 721a 0000 0029 02da 1047 6574  q.S.r....)...Get
-00001060: 4e75 6d49 6d70 6c69 6369 7448 7372 1f00  NumImplicitHsr..
-00001070: 0000 7220 0000 00a9 01da 0169 721a 0000  ..r .......ir...
-00001080: 0072 1b00 0000 7225 0000 008b 0000 0073  .r....r%.......s
-00001090: 0c00 0000 0600 0202 0a01 02fd 0601 06ff  ................
-000010a0: 7a28 6765 745f 6672 6565 5f76 616c 656e  z(get_free_valen
-000010b0: 6365 5f6d 6170 2e3c 6c6f 6361 6c73 3e2e  ce_map.<locals>.
-000010c0: 3c6c 6973 7463 6f6d 703e 2902 7235 0000  <listcomp>).r5..
-000010d0: 0072 2a00 0000 2903 723d 0000 0072 6200  .r*...).r=...rb.
-000010e0: 0000 da06 7265 7375 6c74 721a 0000 0072  ....resultr....r
-000010f0: 6400 0000 721b 0000 0072 5900 0000 8800  d...r....rY.....
-00001100: 0000 730c 0000 0004 010e 010a 0106 020c  ..s.............
-00001110: fe04 0672 5900 0000 7254 0000 0072 5500  ...rY...rT...rU.
-00001120: 0000 6303 0000 0000 0000 0000 0000 000e  ..c.............
-00001130: 0000 0008 0000 0043 0000 0073 a400 0000  .......C...s....
-00001140: 7400 8300 7d03 7401 6a02 6a03 7401 6a02  t...}.t.j.j.t.j.
-00001150: 6a04 7401 6a02 6a05 6401 9c03 7d04 7c04  j.t.j.j.d...}.|.
-00001160: a006 a100 4400 5d3c 5c02 7d05 7d06 7c02  ....D.]<\.}.}.|.
-00001170: 7c05 1900 4400 5d33 7d07 7c01 a006 a100  |...D.]3}.|.....
-00001180: 4400 5d2c 5c02 7d08 7d09 7401 a007 7c00  D.],\.}.}.t...|.
-00001190: a101 7d0a 7c0a a008 7401 a009 7c08 a101  ..}.|...t...|...
-000011a0: a101 7d0b 7c0a a00a 7c07 7c0b 7c06 a103  ..}.|...|.|.|...
-000011b0: 0100 7401 6a0b 7c0a 6402 6403 8d02 7d0c  ..t.j.|.d.d...}.
-000011c0: 7c0c 7243 7121 7401 a00c 7c0a a101 7d0d  |.rCq!t...|...}.
-000011d0: 7c03 a00d 7c0d a101 0100 7121 711b 7113  |...|.....q!q.q.
-000011e0: 7c03 5300 2904 7ab6 0a20 2020 2047 6976  |.S.).z..    Giv
-000011f0: 656e 2061 206d 6f6c 6563 756c 6520 6060  en a molecule ``
-00001200: 6d6f 6c60 602c 2074 6869 7320 6675 6e63  mol``, this func
-00001210: 7469 6f6e 2077 696c 6c20 7265 7475 726e  tion will return
-00001220: 2061 206c 6973 7420 6f66 2053 4d49 4c45   a list of SMILE
-00001230: 5320 7374 7269 6e67 7320 7468 6174 2072  S strings that r
-00001240: 6570 7265 7365 6e74 2076 616c 6964 0a20  epresent valid. 
-00001250: 2020 2061 746f 6d20 6164 6469 7469 6f6e     atom addition
-00001260: 7320 746f 2074 6865 2062 6173 6520 6d6f  s to the base mo
-00001270: 6c65 6375 6c65 2e0a 0a20 2020 203a 7265  lecule...    :re
-00001280: 7475 726e 733a 2041 206c 6973 7420 6f66  turns: A list of
-00001290: 2073 7472 696e 6773 2e0a 2020 2020 a903   strings..    ..
-000012a0: 7209 0000 00e9 0200 0000 e903 0000 0054  r..............T
-000012b0: a901 da0b 6361 7463 6845 7272 6f72 7329  ....catchErrors)
-000012c0: 0e72 3400 0000 7202 0000 00da 0842 6f6e  .r4...r......Bon
-000012d0: 6454 7970 65da 0653 494e 474c 45da 0644  dType..SINGLE..D
-000012e0: 4f55 424c 45da 0654 5249 504c 45da 0569  OUBLE..TRIPLE..i
-000012f0: 7465 6d73 da05 5257 4d6f 6cda 0741 6464  tems..RWMol..Add
-00001300: 4174 6f6d da04 4174 6f6d da07 4164 6442  Atom..Atom..AddB
-00001310: 6f6e 64da 0b53 616e 6974 697a 654d 6f6c  ond..SanitizeMol
-00001320: da0b 4d6f 6c54 6f53 6d69 6c65 73da 0361  ..MolToSmiles..a
-00001330: 6464 290e 723d 0000 0072 5400 0000 7255  dd).r=...rT...rU
-00001340: 0000 0072 4100 0000 da13 7661 6c75 655f  ...rA.....value_
-00001350: 626f 6e64 5f74 7970 655f 6d61 7072 6500  bond_type_mapre.
-00001360: 0000 da09 626f 6e64 5f74 7970 6572 2100  ....bond_typer!.
-00001370: 0000 da07 656c 656d 656e 74da 0776 616c  ....element..val
-00001380: 656e 6365 da07 6e65 775f 6d6f 6cda 0369  ence..new_mol..i
-00001390: 6478 da13 7361 6e69 7469 7a61 7469 6f6e  dx..sanitization
-000013a0: 5f72 6573 756c 7472 5200 0000 721a 0000  _resultrR...r...
-000013b0: 0072 1a00 0000 721b 0000 0072 5a00 0000  .r....r....rZ...
-000013c0: 9400 0000 7326 0000 0006 0a06 0306 0106  ....s&..........
-000013d0: 0106 fd10 050c 0210 010a 0110 010e 010e  ................
-000013e0: 0104 0102 010a 020c 0102 f702 ff04 0c72  ...............r
-000013f0: 5a00 0000 6302 0000 0000 0000 0000 0000  Z...c...........
-00001400: 0010 0000 0007 0000 0043 0000 0073 3601  .........C...s6.
-00001410: 0000 7400 8300 7d02 6401 7401 6a02 6a03  ..t...}.d.t.j.j.
-00001420: 7401 6a02 6a04 7401 6a02 6a05 6402 9c04  t.j.j.t.j.j.d...
-00001430: 7d03 7406 7c03 8301 7d04 7c01 a007 a100  }.t.|...}.|.....
-00001440: 4400 5d80 5c02 7d05 7d06 7408 a009 7c06  D.].\.}.}.t...|.
-00001450: 6403 a102 4400 5d75 5c02 7d07 7d08 7c00  d...D.]u\.}.}.|.
-00001460: a00a 7c07 a101 a00b a100 7235 7c00 a00a  ..|.......r5|...
-00001470: 7c08 a101 a00b a100 7235 7122 7401 a00c  |.......r5q"t...
-00001480: 7c00 a101 a00d 7c07 7c08 a102 7d09 7401  |.....|.|...}.t.
-00001490: a00e 7c00 a101 7d0a 7401 6a0f 7c0a 6404  ..|...}.t.j.|.d.
-000014a0: 6405 8d02 0100 7c09 6401 7501 7278 7c09  d.....|.d.u.rx|.
-000014b0: a010 a100 7d0b 7c0b 7c03 a011 a100 7601  ....}.|.|.....v.
-000014c0: 7259 7122 7c04 7c0b 1900 7d0c 7c0c 7c05  rYq"|.|...}.|.|.
-000014d0: 3700 7d0c 7c0c 6406 6b04 7266 7122 7c09  7.}.|.d.k.rfq"|.
-000014e0: a012 a100 7d0d 7c09 a013 7c03 7c0c 1900  ....}.|...|.|...
-000014f0: a101 0100 7c0a a014 7c0d 7c09 a102 0100  ....|...|.|.....
-00001500: 6e0b 7c03 7c05 1900 7d0b 7c0a a015 7c07  n.|.|...}.|...|.
-00001510: 7c08 7c0b a103 0100 7401 6a16 7c0a 6404  |.|.....t.j.|.d.
-00001520: 6407 8d02 7d0e 7c0e 728d 7122 7401 a017  d...}.|.r.q"t...
-00001530: 7c0a a101 7d0f 7c02 a018 7c0f a101 0100  |...}.|...|.....
-00001540: 7122 7118 7c02 5300 2908 6140 0300 000a  q"q.|.S.).a@....
-00001550: 2020 2020 4769 7665 6e20 6120 6d6f 6c65      Given a mole
-00001560: 6375 6c65 2060 606d 6f6c 6060 2c20 7468  cule ``mol``, th
-00001570: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
-00001580: 2072 6574 7572 6e20 6120 6c69 7374 206f   return a list o
-00001590: 6620 534d 494c 4553 2073 7472 696e 6773  f SMILES strings
-000015a0: 2077 6869 6368 2072 6573 756c 7473 2066   which results f
-000015b0: 726f 6d20 7661 6c69 640a 2020 2020 626f  rom valid.    bo
-000015c0: 6e64 2061 6464 6974 696f 6e73 2074 6f20  nd additions to 
-000015d0: 7468 6174 2062 6173 6520 6d6f 6c65 6375  that base molecu
-000015e0: 6c65 2e20 5661 6c69 6420 626f 6e64 2061  le. Valid bond a
-000015f0: 6464 6974 696f 6e73 2069 6e20 7468 6973  dditions in this
-00001600: 2063 6173 6520 6172 6520 6465 6669 6e65   case are define
-00001610: 6420 6173 2061 6c6c 6f77 6564 2069 6e0a  d as allowed in.
-00001620: 2020 2020 7465 726d 7320 6f66 2074 6865      terms of the
-00001630: 2061 746f 6d20 7661 6c65 6e63 6573 2e20   atom valences. 
-00001640: 626f 6e64 2061 6464 6974 696f 6e73 206d  bond additions m
-00001650: 6179 2063 6f6e 6e65 6374 2074 776f 2061  ay connect two a
-00001660: 746f 6d73 2077 6869 6368 2061 7265 206e  toms which are n
-00001670: 6f74 2079 6574 2064 6972 6563 746c 7920  ot yet directly 
-00001680: 636f 6e6e 6563 7465 640a 2020 2020 6f72  connected.    or
-00001690: 2075 7067 7261 6465 2061 6e20 6578 6973   upgrade an exis
-000016a0: 7469 6e67 2062 6f6e 6420 2873 696e 676c  ting bond (singl
-000016b0: 6520 746f 2064 6f75 626c 6529 2e0a 0a20  e to double)... 
-000016c0: 2020 2041 6c73 6f20 6469 7361 6c6c 6f77     Also disallow
-000016d0: 6564 2061 7265 2062 6f6e 6473 2062 6574  ed are bonds bet
-000016e0: 7765 656e 2074 776f 2061 746f 6d73 2077  ween two atoms w
-000016f0: 6869 6368 2061 7265 2074 6865 6d73 656c  hich are themsel
-00001700: 7665 7320 616c 7265 6164 7920 7061 7274  ves already part
-00001710: 206f 6620 6120 7269 6e67 2e0a 0a20 2020   of a ring...   
-00001720: 203a 7061 7261 6d20 6d6f 6c3a 2054 6865   :param mol: The
-00001730: 2062 6173 6520 6d6f 6c65 6375 6c65 0a20   base molecule. 
-00001740: 2020 203a 7061 7261 6d20 6672 6565 5f76     :param free_v
-00001750: 616c 656e 6365 5f69 6e64 6963 6573 5f6d  alence_indices_m
-00001760: 6170 3a20 4120 6469 6374 2077 686f 7365  ap: A dict whose
-00001770: 206b 6579 7320 6172 6520 696e 7465 6765   keys are intege
-00001780: 7273 2073 7461 7274 696e 6720 6672 6f6d  rs starting from
-00001790: 2030 2e20 5448 6520 6b65 7920 7661 6c75   0. THe key valu
-000017a0: 6573 0a20 2020 2020 2020 2072 6570 7265  es.        repre
-000017b0: 7365 6e74 2074 6865 202a 6672 6565 206e  sent the *free n
-000017c0: 756d 6265 7220 6f66 2076 616c 656e 6365  umber of valence
-000017d0: 732a 2e20 5468 6520 7661 6c75 6573 2061  s*. The values a
-000017e0: 7265 206c 6973 7473 206f 6620 6174 6f6d  re lists of atom
-000017f0: 2069 6e64 6963 6573 2077 6865 7265 2065   indices where e
-00001800: 6163 6820 6174 6f6d 2069 6e0a 2020 2020  ach atom in.    
-00001810: 2020 2020 7468 6520 6c69 7374 2068 6173      the list has
-00001820: 2074 6f20 6861 7665 2074 6865 2063 6f72   to have the cor
-00001830: 7265 7370 6f6e 6469 6e67 206e 756d 6265  responding numbe
-00001840: 7220 6f66 2066 7265 6520 7661 6c65 6e63  r of free valenc
-00001850: 6573 2067 6976 656e 2062 7920 7468 6520  es given by the 
-00001860: 6469 6374 206b 6579 2e0a 0a20 2020 203a  dict key...    :
-00001870: 7265 7475 726e 733a 2041 206c 6973 7420  returns: A list 
-00001880: 6f66 2073 7472 696e 6773 0a20 2020 204e  of strings.    N
-00001890: a904 7201 0000 0072 0900 0000 7268 0000  ..r....r....rh..
-000018a0: 0072 6900 0000 7268 0000 0054 a901 da12  .ri...rh...T....
-000018b0: 636c 6561 7241 726f 6d61 7469 6346 6c61  clearAromaticFla
-000018c0: 6773 7269 0000 0072 6a00 0000 2919 7234  gsri...rj...).r4
-000018d0: 0000 0072 0200 0000 726c 0000 0072 6d00  ...r....rl...rm.
-000018e0: 0000 726e 0000 0072 6f00 0000 7205 0000  ..rn...ro...r...
-000018f0: 0072 7000 0000 da09 6974 6572 746f 6f6c  .rp.....itertool
-00001900: 73da 0c63 6f6d 6269 6e61 7469 6f6e 7372  s..combinationsr
-00001910: 3600 0000 da08 4973 496e 5269 6e67 da03  6.....IsInRing..
-00001920: 4d6f 6cda 1347 6574 426f 6e64 4265 7477  Mol..GetBondBetw
-00001930: 6565 6e41 746f 6d73 7271 0000 00da 084b  eenAtomsrq.....K
-00001940: 656b 756c 697a 6572 1600 0000 da06 7661  ekulizer......va
-00001950: 6c75 6573 721f 0000 00da 0b53 6574 426f  luesr......SetBo
-00001960: 6e64 5479 7065 da0b 5265 706c 6163 6542  ndType..ReplaceB
-00001970: 6f6e 6472 7400 0000 7275 0000 0072 7600  ondrt...ru...rv.
-00001980: 0000 7277 0000 0029 1072 3d00 0000 7255  ..rw...).r=...rU
-00001990: 0000 0072 4100 0000 7278 0000 00da 1362  ...rA...rx.....b
-000019a0: 6f6e 645f 7479 7065 5f76 616c 7565 5f6d  ond_type_value_m
-000019b0: 6170 727b 0000 00da 0561 746f 6d73 da05  apr{.....atoms..
-000019c0: 6174 6f6d 31da 0561 746f 6d32 7219 0000  atom1..atom2r...
-000019d0: 0072 7c00 0000 7279 0000 00da 0a62 6f6e  .r|...ry.....bon
-000019e0: 645f 7661 6c75 6572 2300 0000 727e 0000  d_valuer#...r~..
-000019f0: 0072 5200 0000 721a 0000 0072 1a00 0000  .rR...r....r....
-00001a00: 721b 0000 0072 5b00 0000 b600 0000 7344  r....r[.......sD
-00001a10: 0000 0006 1202 0306 0106 0106 0106 fc08  ................
-00001a20: 0610 0214 011c 0302 0112 020a 010e 0208  ................
-00001a30: 0108 010c 0102 0108 0208 0108 0102 0108  ................
-00001a40: 020e 010e 0108 030e 010e 0204 0102 010a  ................
-00001a50: 020c 0102 df04 2372 5b00 0000 6301 0000  ......#r[...c...
-00001a60: 0000 0000 0000 0000 000f 0000 0007 0000  ................
-00001a70: 0043 0000 0073 6201 0000 7400 8300 7d01  .C...sb...t...}.
-00001a80: 6401 7401 6a02 6a03 7401 6a02 6a04 7401  d.t.j.j.t.j.j.t.
-00001a90: 6a02 6a05 6402 9c04 7d02 7406 7c02 8301  j.j.d...}.t.|...
-00001aa0: 7d03 6403 4400 5d98 7d04 7c00 a007 a100  }.d.D.].}.|.....
-00001ab0: 4400 5d91 7d05 7c05 a008 a100 7c05 a009  D.].}.|.....|...
-00001ac0: a100 0202 7d06 7d07 7401 a00a 7c00 a101  ....}.}.t...|...
-00001ad0: a00b 7c06 7c07 a102 7d05 7c05 a00c a100  ..|.|...}.|.....
-00001ae0: 7d08 7c08 7c02 a00d a100 7601 723b 711c  }.|.|.....v.r;q.
-00001af0: 7401 a00e 7c00 a101 7d09 7401 6a0f 7c09  t...|...}.t.j.|.
-00001b00: 6404 6405 8d02 0100 7c03 7c08 1900 7d0a  d.d.....|.|...}.
-00001b10: 7c0a 7c04 3800 7d0a 7c0a 6406 6b02 725a  |.|.8.}.|.d.k.rZ
-00001b20: 7c09 a010 7c06 7c07 a102 0100 6e17 7c0a  |...|.|.....n.|.
-00001b30: 6406 6b04 7270 7c05 a011 7c02 7c0a 1900  d.k.rp|...|.|...
-00001b40: a101 0100 7c05 a012 a100 7d0b 7c09 a013  ....|.....}.|...
-00001b50: 7c0b 7c05 a102 0100 6e01 711c 7401 6a14  |.|.....n.q.t.j.
-00001b60: 7c09 6404 6407 8d02 7d0c 7c0c 727b 711c  |.d.d...}.|.r{q.
-00001b70: 7401 a015 7c09 a101 7d0d 6408 7c0d 7600  t...|...}.d.|.v.
-00001b80: 72a8 7416 7c0d a017 6408 a101 7418 6409  r.t.|...d...t.d.
-00001b90: 8d02 7d0e 7418 7c0e 6406 1900 8301 640a  ..}.t.|.d.....d.
-00001ba0: 6b04 7296 711c 7418 7401 a019 7c0e 640a  k.r.q.t.t...|.d.
-00001bb0: 1900 a101 a01a a100 8301 640b 6b00 72a4  ..........d.k.r.
-00001bc0: 711c 7c0e 640a 1900 7d0d 7c01 a01b 7c0d  q.|.d...}.|...|.
-00001bd0: a101 0100 711c 7116 7c01 5300 290c 61a2  ....q.q.|.S.).a.
-00001be0: 0100 000a 2020 2020 4769 7665 6e20 6120  ....    Given a 
-00001bf0: 6d6f 6c65 6375 6c65 2060 606d 6f6c 6060  molecule ``mol``
-00001c00: 2c20 7468 6973 2066 756e 6374 696f 6e20  , this function 
-00001c10: 7769 6c6c 2072 6574 7572 6e20 6120 6c69  will return a li
-00001c20: 7374 206f 6620 534d 494c 4553 2073 7472  st of SMILES str
-00001c30: 696e 6773 2077 6869 6368 2072 6570 7265  ings which repre
-00001c40: 7365 6e74 2076 616c 6964 0a20 2020 2062  sent valid.    b
-00001c50: 6f6e 6420 7265 6d6f 7661 6c73 2e20 4120  ond removals. A 
-00001c60: 626f 6e64 2072 656d 6f76 616c 2069 7320  bond removal is 
-00001c70: 6569 7468 6572 2061 2064 6f77 6e67 7261  either a downgra
-00001c80: 6465 206f 6620 616e 2065 7869 7374 696e  de of an existin
-00001c90: 6720 626f 6e64 2028 652e 672e 2064 6f75  g bond (e.g. dou
-00001ca0: 626c 6520 746f 2073 696e 676c 6529 206f  ble to single) o
-00001cb0: 7220 7468 650a 2020 2020 7265 6d6f 7661  r the.    remova
-00001cc0: 6c20 6f66 2061 2073 696e 676c 6520 626f  l of a single bo
-00001cd0: 6e64 2077 6869 6368 2077 6f75 6c64 206d  nd which would m
-00001ce0: 6561 6e20 746f 2064 6973 636f 6e6e 6563  ean to disconnec
-00001cf0: 7420 6174 206d 6f73 7420 6120 7369 6e67  t at most a sing
-00001d00: 6c65 2061 746f 6d20 6672 6f6d 2074 6865  le atom from the
-00001d10: 2072 6573 7420 6f66 2074 6865 0a20 2020   rest of the.   
-00001d20: 206d 6f6c 6563 756c 6521 0a0a 2020 2020   molecule!..    
-00001d30: 3a70 6172 616d 206d 6f6c 3a20 5468 6520  :param mol: The 
-00001d40: 6261 7365 206d 6f6c 6563 756c 6520 666f  base molecule fo
-00001d50: 7220 7468 6520 7265 6d6f 7661 6c73 2e0a  r the removals..
-00001d60: 0a20 2020 203a 7265 7475 726e 733a 2041  .    :returns: A
-00001d70: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
-00001d80: 0a20 2020 204e 727f 0000 0072 6700 0000  .    Nr....rg...
-00001d90: 5472 8000 0000 7201 0000 0072 6a00 0000  Tr....r....rj...
-00001da0: da01 2e29 01da 036b 6579 7209 0000 0072  ...)...keyr....r
-00001db0: 6800 0000 291c 7234 0000 0072 0200 0000  h...).r4...r....
-00001dc0: 726c 0000 0072 6d00 0000 726e 0000 0072  rl...rm...rn...r
-00001dd0: 6f00 0000 7205 0000 0072 2c00 0000 da0f  o...r....r,.....
-00001de0: 4765 7442 6567 696e 4174 6f6d 4964 78da  GetBeginAtomIdx.
-00001df0: 0d47 6574 456e 6441 746f 6d49 6478 7285  .GetEndAtomIdxr.
-00001e00: 0000 0072 8600 0000 7216 0000 0072 8800  ...r....r....r..
-00001e10: 0000 7271 0000 0072 8700 0000 da0a 5265  ..rq...r......Re
-00001e20: 6d6f 7665 426f 6e64 7289 0000 0072 1f00  moveBondr....r..
-00001e30: 0000 728a 0000 0072 7500 0000 7276 0000  ..r....ru...rv..
-00001e40: 00da 0673 6f72 7465 64da 0573 706c 6974  ...sorted..split
-00001e50: 7239 0000 0072 5800 0000 722a 0000 0072  r9...rX...r*...r
-00001e60: 7700 0000 290f 723d 0000 0072 4100 0000  w...).r=...rA...
-00001e70: 7278 0000 0072 8b00 0000 727b 0000 0072  rx...r....r{...r
-00001e80: 1900 0000 728d 0000 0072 8e00 0000 7279  ....r....r....ry
-00001e90: 0000 0072 7c00 0000 728f 0000 0072 2300  ...r|...r....r#.
-00001ea0: 0000 727e 0000 0072 5200 0000 da05 7061  ..r~...rR.....pa
-00001eb0: 7274 7372 1a00 0000 721a 0000 0072 1b00  rtsr....r....r..
-00001ec0: 0000 725c 0000 00f9 0000 0073 4e00 0000  ..r\.......sN...
-00001ed0: 060c 0203 0601 0601 0601 06fc 0806 0802  ................
-00001ee0: 0c01 1201 1201 0802 0c01 0201 0a02 0e01  ................
-00001ef0: 0802 0801 0802 0e01 0802 0e01 0801 0e01  ................
-00001f00: 0203 0e02 0401 0201 0a02 0801 1201 1001  ................
-00001f10: 0201 1a06 0201 0802 0c02 02d4 042e 725c  ..............r\
-00001f20: 0000 0029 0172 0100 0000 2901 7247 0000  ...).r....).rG..
-00001f30: 0029 0172 5000 0000 2901 7261 0000 0029  .).rP...).ra...)
-00001f40: 1e72 8200 0000 da06 7479 7069 6e67 da01  .r......typing..
-00001f50: 74da 0572 646b 6974 7202 0000 00da 0a72  t..rdkitr......r
-00001f60: 646b 6974 2e43 6865 6d72 0300 0000 7204  dkit.Chemr....r.
-00001f70: 0000 00da 1976 6764 5f63 6f75 6e74 6572  .....vgd_counter
-00001f80: 6661 6374 7561 6c73 2e75 7469 6c73 7205  factuals.utilsr.
-00001f90: 0000 00da 1844 4546 4155 4c54 5f41 544f  .....DEFAULT_ATO
-00001fa0: 4d5f 5641 4c45 4e43 455f 4d41 5072 8500  M_VALENCE_MAPr..
-00001fb0: 0000 da03 696e 74da 0554 7570 6c65 da03  ....int..Tuple..
-00001fc0: 7374 7272 4600 0000 724f 0000 0072 5100  strrF...rO...rQ.
-00001fd0: 0000 da08 5365 7175 656e 6365 da08 4361  ....Sequence..Ca
-00001fe0: 6c6c 6162 6c65 da04 626f 6f6c da04 4c69  llable..bool..Li
-00001ff0: 7374 7260 0000 00da 0464 6963 7472 5900  str`.....dictrY.
-00002000: 0000 da04 4469 6374 da03 5365 7472 5a00  ....Dict..SetrZ.
-00002010: 0000 725b 0000 0072 5c00 0000 721a 0000  ..r[...r\...r...
-00002020: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00002030: da08 3c6d 6f64 756c 653e 0100 0000 7360  ..<module>....s`
-00002040: 0000 0008 0008 010c 010c 010c 010c 0202  ................
-00002050: 0402 0102 0202 0102 0102 0106 f902 0e0a  ................
-00002060: fe04 0102 ff02 0202 fe0c 030a fd16 2816  ..............(.
-00002070: 0a02 0702 0202 0102 fe08 fe16 0202 fe08  ................
-00002080: 060a fa1a 3a08 0c0c 0102 ff12 0202 fe08  ....:...........
-00002090: 030a fd08 2212 0102 ff08 020a fe08 4308  ....".........C.
-000020a0: 010e ff                                  ...
+00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
+00000070: 6406 6c0a 6d0b 5a0b 0100 6407 6408 6409  d.l.m.Z...d.d.d.
+00000080: 640a 640b 6409 640c 9c06 5a0c 642e 640e  d.d.d.d...Z.d.d.
+00000090: 6504 6a0d 640f 650e 6604 6410 6411 8405  e.j.d.e.f.d.d...
+000000a0: 5a0f 642f 640e 6504 6a0d 640f 650e 6604  Z.d/d.e.j.d.e.f.
+000000b0: 6413 6414 8405 5a10 6415 6502 6a11 650e  d.d...Z.d.e.j.e.
+000000c0: 1900 6416 6512 6417 6512 6418 6502 6a11  ..d.e.d.e.d.e.j.
+000000d0: 650e 1900 6608 6419 641a 8404 5a13 650c  e...f.d.d...Z.e.
+000000e0: 650f 6510 6602 641b 641c 641c 6605 641d  e.e.f.d.d.d.f.d.
+000000f0: 650e 641e 6502 6a14 6502 6a15 6504 6a0d  e.d.e.j.e.j.e.j.
+00000100: 6701 6502 6a11 650e 1900 6602 1900 1900  g.e.j.e...f.....
+00000110: 641f 6516 6417 6512 6416 6512 6418 6502  d.e.d.e.d.e.d.e.
+00000120: 6a11 650e 1900 660c 6420 6421 8405 5a17  j.e...f.d d!..Z.
+00000130: 6430 640e 6504 6a0d 6423 6518 6418 6519  d0d.e.j.d#e.d.e.
+00000140: 6606 6424 6425 8405 5a1a 640e 6504 6a0d  f.d$d%..Z.d.e.j.
+00000150: 6426 6502 6a1b 650e 6518 6602 1900 6427  d&e.j.e.e.f...d'
+00000160: 6502 6a1b 6518 6502 6a11 6518 1900 6602  e.j.e.e.j.e...f.
+00000170: 1900 6418 6502 6a11 6519 1900 6608 6428  ..d.e.j.e...f.d(
+00000180: 6429 8404 5a1c 640e 6504 6a0d 6427 6502  d)..Z.d.e.j.d'e.
+00000190: 6a1b 6518 6502 6a11 6518 1900 6602 1900  j.e.e.j.e...f...
+000001a0: 6418 6502 6a11 6519 1900 6606 642a 642b  d.e.j.e...f.d*d+
+000001b0: 8404 5a1d 640e 6504 6a0d 6418 6502 6a11  ..Z.d.e.j.d.e.j.
+000001c0: 6519 1900 6604 642c 642d 8404 5a1e 6401  e...f.d,d-..Z.d.
+000001d0: 5300 2931 e900 0000 004e 2901 da04 4368  S.)1.....N)...Ch
+000001e0: 656d 2901 da06 7264 464d 4353 2901 da07  em)...rdFMCS)...
+000001f0: 416c 6c43 6865 6d29 01da 0c44 696d 6f72  AllChem)...Dimor
+00000200: 7068 6974 6544 4c29 01da 0b69 6e76 6572  phiteDL)...inver
+00000210: 745f 6469 6374 e904 0000 00e9 0500 0000  t_dict..........
+00000220: e906 0000 00e9 0100 0000 e907 0000 0029  ...............)
+00000230: 06da 0143 da01 4eda 014f da01 46da 0243  ...C..N..O..F..C
+00000240: 6cda 0153 fa0e 2a31 3d2a 2a32 3d2a 2a3d  l..S..*1=**2=**=
+00000250: 2a31 2a32 da03 6d6f 6cda 0770 6174 7465  *1*2..mol..patte
+00000260: 726e 6302 0000 0000 0000 0000 0000 0004  rnc.............
+00000270: 0000 0003 0000 0043 0000 00f3 1800 0000  .......C........
+00000280: 7400 a001 7c01 a101 7d02 7c00 a002 7c02  t...|...}.|...|.
+00000290: a101 7d03 7c03 5300 2901 7a83 0a20 2020  ..}.|.S.).z..   
+000002a0: 2043 6865 636b 7320 6966 2074 6865 2067   Checks if the g
+000002b0: 6976 656e 206d 6f6c 6563 756c 6520 6060  iven molecule ``
+000002c0: 6d6f 6c60 6020 6973 2061 2062 7269 6467  mol`` is a bridg
+000002d0: 6520 6865 6164 2063 6172 626f 6e20 7374  e head carbon st
+000002e0: 7275 6374 7572 6520 7768 6963 6820 6170  ructure which ap
+000002f0: 7061 7265 6e74 6c79 2064 6f65 7320 6e6f  parently does no
+00000300: 740a 2020 2020 6170 7065 6172 2069 6e20  t.    appear in 
+00000310: 6368 656d 6973 7472 792e 0a20 2020 20a9  chemistry..    .
+00000320: 0372 0200 0000 da0d 4d6f 6c46 726f 6d53  .r......MolFromS
+00000330: 6d61 7274 73da 1148 6173 5375 6273 7472  marts..HasSubstr
+00000340: 7563 744d 6174 6368 a904 7213 0000 0072  uctMatch..r....r
+00000350: 1400 0000 da06 736d 6172 7473 da08 6973  ......smarts..is
+00000360: 5f6d 6174 6368 a900 721c 0000 00fa 542f  _match..r.....T/
+00000370: 6d65 6469 612f 7373 642f 5072 6f67 7261  media/ssd/Progra
+00000380: 6d6d 696e 672f 7667 645f 636f 756e 7465  mming/vgd_counte
+00000390: 7266 6163 7475 616c 732f 7667 645f 636f  rfactuals/vgd_co
+000003a0: 756e 7465 7266 6163 7475 616c 732f 6765  unterfactuals/ge
+000003b0: 6e65 7261 7465 2f6d 6f6c 6563 756c 6573  nerate/molecules
+000003c0: 2e70 79da 1569 735f 6272 6964 6765 5f68  .py..is_bridge_h
+000003d0: 6561 645f 6361 7262 6f6e 1600 0000 7306  ead_carbon....s.
+000003e0: 0000 000a 050a 0104 0172 1e00 0000 da03  .........r......
+000003f0: 534e 4e63 0200 0000 0000 0000 0000 0000  SNNc............
+00000400: 0400 0000 0300 0000 4300 0000 7215 0000  ........C...r...
+00000410: 0029 014e 7216 0000 0072 1900 0000 721c  .).Nr....r....r.
+00000420: 0000 0072 1c00 0000 721d 0000 00da 1b69  ...r....r......i
+00000430: 735f 6e69 7472 6f67 656e 5f6e 6974 726f  s_nitrogen_nitro
+00000440: 6765 6e5f 7375 6c66 7572 2000 0000 7306  gen_sulfur ...s.
+00000450: 0000 000a 010a 0104 0172 2000 0000 da0b  .........r .....
+00000460: 736d 696c 6573 5f6c 6973 74da 066d 696e  smiles_list..min
+00000470: 5f70 68da 066d 6178 5f70 68da 0672 6574  _ph..max_ph..ret
+00000480: 7572 6e63 0300 0000 0000 0000 0000 0000  urnc............
+00000490: 0400 0000 0700 0000 0300 0000 7334 0000  ............s4..
+000004a0: 0074 007c 017c 0264 0164 0264 0364 048d  .t.|.|.d.d.d.d..
+000004b0: 0589 0074 0174 026a 03a0 0487 0066 0164  ...t.t.j.....f.d
+000004c0: 0564 0684 087c 0044 0083 01a1 0183 017d  .d...|.D.......}
+000004d0: 037c 0353 0029 074e e90a 0000 0046 e700  .|.S.).N.....F..
+000004e0: 0000 0000 00f0 3fa9 0572 2200 0000 7223  ......?..r"...r#
+000004f0: 0000 00da 0c6d 6178 5f76 6172 6961 6e74  .....max_variant
+00000500: 73da 0c6c 6162 656c 5f73 7461 7465 73da  s..label_states.
+00000510: 0d70 6b61 5f70 7265 6369 7369 6f6e 6301  .pka_precisionc.
+00000520: 0000 0000 0000 0000 0000 0002 0000 0005  ................
+00000530: 0000 0013 0000 0073 1600 0000 6700 7c00  .......s....g.|.
+00000540: 5d07 7d01 8800 a000 7c01 a101 9102 7102  ].}.....|.....q.
+00000550: 5300 721c 0000 0029 01da 0970 726f 746f  S.r....)...proto
+00000560: 6e61 7465 2902 da02 2e30 da06 736d 696c  nate)....0..smil
+00000570: 6573 a901 da04 646d 7068 721c 0000 0072  es....dmphr....r
+00000580: 1d00 0000 da0a 3c6c 6973 7463 6f6d 703e  ......<listcomp>
+00000590: 3200 0000 7302 0000 0016 007a 2e66 6978  2...s......z.fix
+000005a0: 5f70 726f 746f 6e61 7469 6f6e 5f64 696d  _protonation_dim
+000005b0: 6f72 7068 6974 652e 3c6c 6f63 616c 733e  orphite.<locals>
+000005c0: 2e3c 6c69 7374 636f 6d70 3e29 0572 0500  .<listcomp>).r..
+000005d0: 0000 da04 6c69 7374 da09 6974 6572 746f  ....list..iterto
+000005e0: 6f6c 73da 0563 6861 696e da0d 6672 6f6d  ols..chain..from
+000005f0: 5f69 7465 7261 626c 6529 0472 2100 0000  _iterable).r!...
+00000600: 7222 0000 0072 2300 0000 da06 7265 7375  r"...r#.....resu
+00000610: 6c74 721c 0000 0072 2e00 0000 721d 0000  ltr....r....r...
+00000620: 00da 1a66 6978 5f70 726f 746f 6e61 7469  ...fix_protonati
+00000630: 6f6e 5f64 696d 6f72 7068 6974 6526 0000  on_dimorphite&..
+00000640: 0073 1600 0000 0204 0201 0201 0201 0201  .s..............
+00000650: 0201 06fb 0807 1001 06ff 0404 7236 0000  ............r6..
+00000660: 0046 679a 9999 9999 9919 4072 2d00 0000  .Fg.......@r-...
+00000670: da0b 6d6f 6c5f 6669 6c74 6572 73da 0f66  ..mol_filters..f
+00000680: 6978 5f70 726f 746f 6e61 7469 6f6e 6306  ix_protonationc.
+00000690: 0000 0000 0000 0000 0000 000d 0000 0007  ................
+000006a0: 0000 0003 0000 0073 dc00 0000 6700 7d06  .......s....g.}.
+000006b0: 7400 a001 7c00 a101 8900 7402 8800 8301  t...|.....t.....
+000006c0: 7d07 7c06 7403 8800 7c01 7c07 6401 8d03  }.|.t...|.|.d...
+000006d0: 3700 7d06 7c06 7404 8800 7c07 6402 8d02  7.}.|.t...|.d...
+000006e0: 3700 7d06 7c06 7405 8800 6403 8d01 3700  7.}.|.t...d...7.
+000006f0: 7d06 6700 7d08 7c06 4400 5d17 7d09 7c09  }.g.}.|.D.].}.|.
+00000700: 6404 1900 8900 7406 8700 6601 6405 6406  d.....t...f.d.d.
+00000710: 8408 7c02 4400 8301 8301 7239 7127 7c08  ..|.D.....r9q'|.
+00000720: a007 7c09 a101 0100 7127 7c08 7d06 7c03  ..|.....q'|.}.|.
+00000730: 726c 6700 7d0a 7408 7c05 7c04 6407 6408  rlg.}.t.|.|.d.d.
+00000740: 6409 640a 8d05 7d0b 7c06 4400 5d19 7d09  d.d...}.|.D.].}.
+00000750: 7c0b a009 7c09 640b 1900 a101 7d0c 7c0c  |...|.d.....}.|.
+00000760: 4400 5d0d 7d00 7c0a a007 6900 7c09 a501  D.].}.|...i.|...
+00000770: 640b 7c00 6901 a501 a101 0100 715b 7150  d.|.i.......q[qP
+00000780: 7c0a 7d06 7c06 5300 290c 61b1 0300 000a  |.}.|.S.).a.....
+00000790: 2020 2020 4769 7665 6e20 6120 6060 736d      Given a ``sm
+000007a0: 696c 6573 6060 2072 6570 7265 7365 6e74  iles`` represent
+000007b0: 6174 696f 6e20 6f66 2061 206d 6f6c 6563  ation of a molec
+000007c0: 756c 652c 2074 6869 7320 6675 6e63 7469  ule, this functi
+000007d0: 6f6e 2077 696c 6c20 7265 7475 726e 2061  on will return a
+000007e0: 206c 6973 7420 6f66 2074 6865 2053 4d49   list of the SMI
+000007f0: 4c45 530a 2020 2020 7265 7072 6573 656e  LES.    represen
+00000800: 7461 7469 6f6e 7320 6f66 2061 6c6c 2074  tations of all t
+00000810: 6865 2076 616c 6964 206d 6f6c 6563 756c  he valid molecul
+00000820: 6573 2077 6974 6869 6e20 6120 312d 6564  es within a 1-ed
+00000830: 6974 206e 6569 6768 626f 7268 6f6f 642e  it neighborhood.
+00000840: 204f 7074 696f 6e61 6c6c 792c 2061 206c   Optionally, a l
+00000850: 6973 7420 6f66 2062 6f6f 6c65 616e 0a20  ist of boolean. 
+00000860: 2020 2066 756e 6374 696f 6e73 2063 616e     functions can
+00000870: 2062 6520 7072 6f76 6964 6564 2066 6f72   be provided for
+00000880: 2060 606d 6f6c 5f66 696c 7465 7273 6060   ``mol_filters``
+00000890: 2074 6f20 6675 7274 6865 7220 6c69 6d69   to further limi
+000008a0: 7420 7468 6520 6b69 6e64 7320 6f66 206d  t the kinds of m
+000008b0: 6f6c 6563 756c 6573 2069 6e63 6c75 6465  olecules include
+000008c0: 6420 696e 2074 6865 0a20 2020 2072 6573  d in the.    res
+000008d0: 756c 742e 0a0a 2020 2020 3a70 6172 616d  ult...    :param
+000008e0: 2073 6d69 6c65 733a 2054 6865 2053 4d49   smiles: The SMI
+000008f0: 4c45 5320 7374 7269 6e67 2072 6570 7265  LES string repre
+00000900: 7365 6e74 6174 696f 6e20 6f66 0a20 2020  sentation of.   
+00000910: 203a 7061 7261 6d20 6174 6f6d 5f76 616c   :param atom_val
+00000920: 656e 6365 5f6d 6170 3a20 4120 6469 6374  ence_map: A dict
+00000930: 696f 6e61 7279 2c20 7768 6f73 6520 6b65  ionary, whose ke
+00000940: 7973 2061 7265 2073 7472 696e 6773 2074  ys are strings t
+00000950: 6861 7420 6964 656e 7469 6679 2061 746f  hat identify ato
+00000960: 6d20 7479 7065 7320 6f66 2074 6865 2053  m types of the S
+00000970: 4d49 4c45 530a 2020 2020 2020 2020 6e6f  MILES.        no
+00000980: 7461 7469 6f6e 2028 4f2c 204e 2c20 436c  tation (O, N, Cl
+00000990: 202e 2e2e 2920 616e 6420 7468 6520 7661   ...) and the va
+000009a0: 6c75 6573 2061 7265 2074 6865 2069 6e74  lues are the int
+000009b0: 6567 6572 2076 616c 656e 6365 206f 6620  eger valence of 
+000009c0: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
+000009d0: 6720 6174 6f6d 2e20 4f6e 6c79 0a20 2020  g atom. Only.   
+000009e0: 2020 2020 2061 746f 6d73 2074 6861 7420       atoms that 
+000009f0: 6172 6520 6c69 7374 6564 2069 6e20 7468  are listed in th
+00000a00: 6973 2064 6963 7420 7769 6c6c 2062 6520  is dict will be 
+00000a10: 636f 6e73 6964 6572 6564 2066 6f72 2065  considered for e
+00000a20: 6469 7420 6f70 6572 6174 696f 6e73 2073  dit operations s
+00000a30: 7563 6820 6173 2061 6464 696e 6720 6f72  uch as adding or
+00000a40: 0a20 2020 2020 2020 2072 6570 6c61 6369  .        replaci
+00000a50: 6e67 2061 6e64 2061 746f 6d21 0a20 2020  ng and atom!.   
+00000a60: 203a 7061 7261 6d20 6d6f 6c5f 6669 6c74   :param mol_filt
+00000a70: 6572 733a 2041 206c 6973 7420 6f66 2066  ers: A list of f
+00000a80: 756e 6374 696f 6e73 2077 6869 6368 2065  unctions which e
+00000a90: 6163 6820 7461 6b65 2061 204d 6f6c 206f  ach take a Mol o
+00000aa0: 626a 6563 7420 6173 2069 6e70 7574 2061  bject as input a
+00000ab0: 6e64 2072 6574 7572 6e20 6120 626f 6f6c  nd return a bool
+00000ac0: 6561 6e20 7661 6c75 650a 2020 2020 2020  ean value.      
+00000ad0: 2020 746f 2064 6574 6572 6d69 6e65 2077    to determine w
+00000ae0: 6865 7468 6572 2074 6861 7420 6174 6f6d  hether that atom
+00000af0: 2073 686f 756c 6420 6265 2065 7863 6c75   should be exclu
+00000b00: 6465 6420 2854 7275 6529 206f 7220 6e6f  ded (True) or no
+00000b10: 7420 2846 616c 7365 292e 0a0a 2020 2020  t (False)...    
+00000b20: 3a72 6574 7572 6e73 3a20 4120 6c69 7374  :returns: A list
+00000b30: 206f 6620 7374 7269 6e67 730a 2020 2020   of strings.    
+00000b40: 2903 7213 0000 00da 1061 746f 6d5f 7661  ).r......atom_va
+00000b50: 6c65 6e63 655f 6d61 70da 1866 7265 655f  lence_map..free_
+00000b60: 7661 6c65 6e63 655f 696e 6469 6365 735f  valence_indices_
+00000b70: 6d61 7029 0272 1300 0000 723a 0000 00a9  map).r....r:....
+00000b80: 0172 1300 0000 7213 0000 0063 0100 0000  .r....r....c....
+00000b90: 0000 0000 0000 0000 0200 0000 0400 0000  ................
+00000ba0: 1300 0000 7314 0000 0067 007c 005d 067d  ....s....g.|.].}
+00000bb0: 017c 0188 0083 0191 0271 0253 0072 1c00  .|.......q.S.r..
+00000bc0: 0000 721c 0000 0029 0272 2c00 0000 da04  ..r....).r,.....
+00000bd0: 6675 6e63 723b 0000 0072 1c00 0000 721d  funcr;...r....r.
+00000be0: 0000 0072 3000 0000 6d00 0000 7302 0000  ...r0...m...s...
+00000bf0: 0014 007a 2467 6574 5f6e 6569 6768 626f  ...z$get_neighbo
+00000c00: 7268 6f6f 642e 3c6c 6f63 616c 733e 2e3c  rhood.<locals>.<
+00000c10: 6c69 7374 636f 6d70 3e72 2500 0000 4672  listcomp>r%...Fr
+00000c20: 2600 0000 7227 0000 00da 0576 616c 7565  &...r'.....value
+00000c30: 290a 7202 0000 00da 0d4d 6f6c 4672 6f6d  ).r......MolFrom
+00000c40: 536d 696c 6573 da14 6765 745f 6672 6565  Smiles..get_free
+00000c50: 5f76 616c 656e 6365 5f6d 6170 da18 6765  _valence_map..ge
+00000c60: 745f 7661 6c69 645f 6174 6f6d 5f61 6464  t_valid_atom_add
+00000c70: 6974 696f 6e73 da18 6765 745f 7661 6c69  itions..get_vali
+00000c80: 645f 626f 6e64 5f61 6464 6974 696f 6e73  d_bond_additions
+00000c90: da17 6765 745f 7661 6c69 645f 626f 6e64  ..get_valid_bond
+00000ca0: 5f72 656d 6f76 616c 73da 0361 6e79 da06  _removals..any..
+00000cb0: 6170 7065 6e64 7205 0000 0072 2b00 0000  appendr....r+...
+00000cc0: 290d 722d 0000 0072 3900 0000 7237 0000  ).r-...r9...r7..
+00000cd0: 0072 3800 0000 7223 0000 0072 2200 0000  .r8...r#...r"...
+00000ce0: da09 6e65 6967 6862 6f72 7372 3a00 0000  ..neighborsr:...
+00000cf0: da12 6e65 6967 6862 6f72 735f 6669 6c74  ..neighbors_filt
+00000d00: 6572 6564 da04 6461 7461 da14 6e65 6967  ered..data..neig
+00000d10: 6862 6f72 735f 7072 6f74 6f6e 6174 6564  hbors_protonated
+00000d20: 722f 0000 00da 1173 6d69 6c65 735f 7072  r/.....smiles_pr
+00000d30: 6f74 6f6e 6174 6564 721c 0000 0072 3b00  otonatedr....r;.
+00000d40: 0000 721d 0000 00da 1067 6574 5f6e 6569  ..r......get_nei
+00000d50: 6768 626f 7268 6f6f 6438 0000 0073 4c00  ghborhood8...sL.
+00000d60: 0000 041a 0a02 0801 0402 0201 0201 0201  ................
+00000d70: 08fd 0406 0201 0201 08fe 0405 0201 08ff  ................
+00000d80: 0408 0801 0801 1601 0201 0c02 0402 0406  ................
+00000d90: 0401 0201 0201 0201 0201 0201 0201 06fb  ................
+00000da0: 0807 0e01 0801 1801 02ff 0403 0402 724a  ..............rJ
+00000db0: 0000 00e9 0800 0000 da0b 6d61 785f 7661  ..........max_va
+00000dc0: 6c65 6e63 6563 0200 0000 0000 0000 0000  lencec..........
+00000dd0: 0000 0300 0000 0400 0000 0300 0000 7332  ..............s2
+00000de0: 0000 0069 007d 0274 0064 017c 0183 0244  ...i.}.t.d.|...D
+00000df0: 005d 0f89 0087 0066 0164 0264 0384 087c  .].....f.d.d...|
+00000e00: 00a0 01a1 0044 0083 017c 0288 003c 0071  .....D...|...<.q
+00000e10: 077c 0253 0029 044e 720a 0000 0063 0100  .|.S.).Nr....c..
+00000e20: 0000 0000 0000 0000 0000 0200 0000 0400  ................
+00000e30: 0000 1300 0000 7320 0000 0067 007c 005d  ......s ...g.|.]
+00000e40: 0c7d 017c 01a0 00a1 0088 006b 0572 027c  .}.|.......k.r.|
+00000e50: 01a0 01a1 0091 0271 0253 0072 1c00 0000  .......q.S.r....
+00000e60: 2902 da10 4765 744e 756d 496d 706c 6963  )...GetNumImplic
+00000e70: 6974 4873 da06 4765 7449 6478 2902 722c  itHs..GetIdx).r,
+00000e80: 0000 00da 0461 746f 6da9 01da 0169 721c  .....atom....ir.
+00000e90: 0000 0072 1d00 0000 7230 0000 008e 0000  ...r....r0......
+00000ea0: 0073 0c00 0000 0600 0202 0a01 02fd 0601  .s..............
+00000eb0: 06ff 7a28 6765 745f 6672 6565 5f76 616c  ..z(get_free_val
+00000ec0: 656e 6365 5f6d 6170 2e3c 6c6f 6361 6c73  ence_map.<locals
+00000ed0: 3e2e 3c6c 6973 7463 6f6d 703e 2902 da05  >.<listcomp>)...
+00000ee0: 7261 6e67 65da 0847 6574 4174 6f6d 7329  range..GetAtoms)
+00000ef0: 0372 1300 0000 724c 0000 0072 3500 0000  .r....rL...r5...
+00000f00: 721c 0000 0072 5000 0000 721d 0000 0072  r....rP...r....r
+00000f10: 3f00 0000 8b00 0000 730c 0000 0004 010e  ?.......s.......
+00000f20: 010a 0106 020c fe04 0672 3f00 0000 7239  .........r?...r9
+00000f30: 0000 0072 3a00 0000 6303 0000 0000 0000  ...r:...c.......
+00000f40: 0000 0000 000e 0000 000b 0000 0043 0000  .............C..
+00000f50: 0073 bc00 0000 6700 7d03 7400 6a01 6a02  .s....g.}.t.j.j.
+00000f60: 7400 6a01 6a03 7400 6a01 6a04 6401 9c03  t.j.j.t.j.j.d...
+00000f70: 7d04 7c04 a005 a100 4400 5d49 5c02 7d05  }.|.....D.]I\.}.
+00000f80: 7d06 7c02 7c05 1900 4400 5d40 7d07 7c01  }.|.|...D.]@}.|.
+00000f90: a005 a100 4400 5d39 5c02 7d08 7d09 7400  ....D.]9\.}.}.t.
+00000fa0: a006 7c00 a101 7d0a 7c0a a007 7400 a008  ..|...}.|...t...
+00000fb0: 7c08 a101 a101 7d0b 7c0a a009 7c07 7c0b  |.....}.|...|.|.
+00000fc0: 7c06 a103 0100 7400 6a0a 7c0a 6402 6403  |.....t.j.|.d.d.
+00000fd0: 8d02 7d0c 7c0c 7242 7120 7400 6a0b 7c0a  ..}.|.rBq t.j.|.
+00000fe0: 6404 6405 6406 8d03 7d0d 7c03 a00c 6407  d.d.d...}.|...d.
+00000ff0: 7c0a 7c0d 7c07 7c07 6602 7c07 7c0b 6602  |.|.|.|.f.|.|.f.
+00001000: 6408 9c05 a101 0100 7120 711a 7112 7c03  d.......q q.q.|.
+00001010: 5300 2909 611b 0400 000a 2020 2020 4769  S.).a.....    Gi
+00001020: 7665 6e20 6120 6d6f 6c65 6375 6c65 2060  ven a molecule `
+00001030: 606d 6f6c 6060 2c20 7468 6973 2066 756e  `mol``, this fun
+00001040: 6374 696f 6e20 7769 6c6c 2072 6574 7572  ction will retur
+00001050: 6e20 6120 6c69 7374 206f 6620 534d 494c  n a list of SMIL
+00001060: 4553 2073 7472 696e 6773 2074 6861 7420  ES strings that 
+00001070: 7265 7072 6573 656e 7420 7661 6c69 640a  represent valid.
+00001080: 2020 2020 6174 6f6d 2061 6464 6974 696f      atom additio
+00001090: 6e73 2074 6f20 7468 6520 6261 7365 206d  ns to the base m
+000010a0: 6f6c 6563 756c 652e 0a0a 2020 2020 3a70  olecule...    :p
+000010b0: 6172 616d 206d 6f6c 3a20 5468 6520 6f72  aram mol: The or
+000010c0: 6967 696e 616c 206d 6f6c 6563 756c 6520  iginal molecule 
+000010d0: 666f 7220 7768 6963 6820 746f 2063 616c  for which to cal
+000010e0: 6375 6c61 7465 2074 6865 206d 6f64 6966  culate the modif
+000010f0: 6963 6174 696f 6e73 0a20 2020 203a 7061  ications.    :pa
+00001100: 7261 6d20 6174 6f6d 5f76 616c 656e 6365  ram atom_valence
+00001110: 5f6d 6170 3a20 4120 6469 6374 2077 686f  _map: A dict who
+00001120: 7365 206b 6579 7320 6172 6520 7374 7269  se keys are stri
+00001130: 6e67 2069 6465 6e74 6966 6965 7273 206f  ng identifiers o
+00001140: 6620 6174 6f6d 2074 7970 6573 2028 4f2c  f atom types (O,
+00001150: 204e 2c20 532e 2e2e 2920 616e 6420 7468   N, S...) and th
+00001160: 650a 2020 2020 2020 2020 7661 6c75 6573  e.        values
+00001170: 2061 7265 2074 6865 2069 6e74 6567 6572   are the integer
+00001180: 2076 616c 656e 6365 7320 6173 736f 6369   valences associ
+00001190: 6174 6564 2077 6974 6820 7468 6573 6520  ated with these 
+000011a0: 6174 6f6d 2074 7970 6573 2e0a 2020 2020  atom types..    
+000011b0: 3a70 6172 616d 2066 7265 655f 7661 6c65  :param free_vale
+000011c0: 6e63 655f 696e 6469 6365 735f 6d61 703a  nce_indices_map:
+000011d0: 2041 2064 6963 7420 7768 6f73 6520 6b65   A dict whose ke
+000011e0: 7973 2061 7265 2069 6e74 6567 6572 2076  ys are integer v
+000011f0: 616c 7565 7320 666f 7220 706f 7373 6962  alues for possib
+00001200: 6c65 2061 746f 6d20 7661 6c65 6e63 6573  le atom valences
+00001210: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
+00001220: 6d6f 6c65 6375 6c65 2061 6e64 2074 6865  molecule and the
+00001230: 2076 616c 7565 7320 6172 6520 6c69 7374   values are list
+00001240: 7320 636f 6e74 6169 6e69 6e67 2069 6e74  s containing int
+00001250: 6567 6572 206e 6f64 6520 696e 6469 6365  eger node indice
+00001260: 7320 6f66 2061 6c6c 2074 6865 2061 746f  s of all the ato
+00001270: 6d73 2077 6869 6368 2068 6176 6520 7468  ms which have th
+00001280: 6174 0a20 2020 2020 2020 2063 6f72 7265  at.        corre
+00001290: 7370 6f6e 6469 6e67 2076 616c 656e 6365  sponding valence
+000012a0: 2e0a 0a20 2020 203a 7265 7475 726e 733a  ...    :returns:
+000012b0: 2041 206c 6973 7420 6f66 2064 6963 7469   A list of dicti
+000012c0: 6f6e 6172 6965 7320 7768 6963 6820 6465  onaries which de
+000012d0: 6669 6e65 2074 6865 2076 616c 6964 206d  fine the valid m
+000012e0: 6f64 6966 6963 6174 696f 6e73 2e20 4561  odifications. Ea
+000012f0: 6368 2064 6963 7469 6f6e 6172 7920 6861  ch dictionary ha
+00001300: 7320 7468 6520 6b65 7973 0a20 2020 2020  s the keys.     
+00001310: 2020 202d 206d 6f6c 3a20 5468 6520 6d6f     - mol: The mo
+00001320: 6c20 6f62 6a65 6374 206f 6620 7468 6520  l object of the 
+00001330: 4e45 5720 6d6f 6c65 6375 6c65 0a20 2020  NEW molecule.   
+00001340: 2020 2020 202d 2073 6d69 6c65 733a 2054       - smiles: T
+00001350: 6865 2053 4d49 4c45 5320 7374 7269 6e67  he SMILES string
+00001360: 206f 6620 7468 6520 4e45 5720 6d6f 6c65   of the NEW mole
+00001370: 6375 6c65 0a20 2020 2020 2020 202d 206f  cule.        - o
+00001380: 7267 3a20 5468 6520 696e 7465 6765 7220  rg: The integer 
+00001390: 6174 6f6d 2069 6e64 6578 206f 6620 7468  atom index of th
+000013a0: 6520 4f52 4947 494e 414c 206d 6f6c 6563  e ORIGINAL molec
+000013b0: 756c 6520 7768 6572 6520 7468 6520 6d6f  ule where the mo
+000013c0: 6469 6669 6361 7469 6f6e 206f 7269 6769  dification origi
+000013d0: 6e61 7465 730a 2020 2020 2020 2020 2d20  nates.        - 
+000013e0: 6d6f 643a 2054 6865 2069 6e74 6567 6572  mod: The integer
+000013f0: 2061 746f 6d20 696e 6465 7820 6f66 2074   atom index of t
+00001400: 6865 204e 4557 206d 6f6c 6563 756c 6520  he NEW molecule 
+00001410: 7768 6572 6520 7468 6520 6d6f 6469 6669  where the modifi
+00001420: 6361 7469 6f6e 206f 6363 7572 7265 640a  cation occurred.
+00001430: 2020 2020 a903 720a 0000 00e9 0200 0000      ..r.........
+00001440: e903 0000 0054 a901 da0b 6361 7463 6845  .....T....catchE
+00001450: 7272 6f72 7346 7201 0000 00a9 02da 0963  rrorsFr........c
+00001460: 616e 6f6e 6963 616c da0c 726f 6f74 6564  anonical..rooted
+00001470: 4174 4174 6f6d da08 6164 645f 6e6f 6465  AtAtom..add_node
+00001480: a905 da04 7479 7065 7213 0000 0072 3d00  ....typer....r=.
+00001490: 0000 da03 6f72 67da 036d 6f64 290d 7202  ....org..mod).r.
+000014a0: 0000 00da 0842 6f6e 6454 7970 65da 0653  .....BondType..S
+000014b0: 494e 474c 45da 0644 4f55 424c 45da 0654  INGLE..DOUBLE..T
+000014c0: 5249 504c 45da 0569 7465 6d73 da05 5257  RIPLE..items..RW
+000014d0: 4d6f 6cda 0741 6464 4174 6f6d da04 4174  Mol..AddAtom..At
+000014e0: 6f6d da07 4164 6442 6f6e 64da 0b53 616e  om..AddBond..San
+000014f0: 6974 697a 654d 6f6c da0b 4d6f 6c54 6f53  itizeMol..MolToS
+00001500: 6d69 6c65 7372 4400 0000 290e 7213 0000  milesrD...).r...
+00001510: 0072 3900 0000 723a 0000 00da 0772 6573  .r9...r:.....res
+00001520: 756c 7473 da13 7661 6c75 655f 626f 6e64  ults..value_bond
+00001530: 5f74 7970 655f 6d61 7072 5100 0000 da09  _type_maprQ.....
+00001540: 626f 6e64 5f74 7970 6572 4f00 0000 da07  bond_typerO.....
+00001550: 656c 656d 656e 74da 0776 616c 656e 6365  element..valence
+00001560: da07 6e65 775f 6d6f 6cda 0369 6478 da13  ..new_mol..idx..
+00001570: 7361 6e69 7469 7a61 7469 6f6e 5f72 6573  sanitization_res
+00001580: 756c 7472 2d00 0000 721c 0000 0072 1c00  ultr-...r....r..
+00001590: 0000 721d 0000 0072 4000 0000 9700 0000  ..r....r@.......
+000015a0: 7332 0000 0004 1506 0306 0106 0106 fd10  s2..............
+000015b0: 050c 0210 010a 0110 010e 010e 0104 0102  ................
+000015c0: 0110 0204 0102 0102 0102 0106 0106 010a  ................
+000015d0: fb02 f702 ff04 1272 4000 0000 6302 0000  .......r@...c...
+000015e0: 0000 0000 0000 0000 0010 0000 000a 0000  ................
+000015f0: 0043 0000 0073 4e01 0000 6700 7d02 6401  .C...sN...g.}.d.
+00001600: 7400 6a01 6a02 7400 6a01 6a03 7400 6a01  t.j.j.t.j.j.t.j.
+00001610: 6a04 6402 9c04 7d03 7405 7c03 8301 7d04  j.d...}.t.|...}.
+00001620: 7c01 a006 a100 4400 5d8d 5c02 7d05 7d06  |.....D.].\.}.}.
+00001630: 7407 a008 7c06 6403 a102 4400 5d82 5c02  t...|.d...D.].\.
+00001640: 7d07 7d08 7c00 a009 7c07 a101 a00a a100  }.}.|...|.......
+00001650: 7234 7c00 a009 7c08 a101 a00a a100 7234  r4|...|.......r4
+00001660: 7121 7400 a00b 7c00 a101 a00c 7c07 7c08  q!t...|.....|.|.
+00001670: a102 7d09 7400 a00d 7c00 a101 7d0a 7400  ..}.t...|...}.t.
+00001680: 6a0e 7c0a 6404 6405 8d02 0100 7c09 6401  j.|.d.d.....|.d.
+00001690: 7501 7277 7c09 a00f a100 7d0b 7c0b 7c03  u.rw|.....}.|.|.
+000016a0: a010 a100 7601 7258 7121 7c04 7c0b 1900  ....v.rXq!|.|...
+000016b0: 7d0c 7c0c 7c05 3700 7d0c 7c0c 6406 6b04  }.|.|.7.}.|.d.k.
+000016c0: 7265 7121 7c09 a011 a100 7d0d 7c09 a012  req!|.....}.|...
+000016d0: 7c03 7c0c 1900 a101 0100 7c0a a013 7c0d  |.|.......|...|.
+000016e0: 7c09 a102 0100 6e0b 7c03 7c05 1900 7d0b  |.....n.|.|...}.
+000016f0: 7c0a a014 7c07 7c08 7c0b a103 0100 7400  |...|.|.|.....t.
+00001700: 6a15 7c0a 6404 6407 8d02 7d0e 7c0e 728c  j.|.d.d...}.|.r.
+00001710: 7121 7400 6a16 7c0a 6408 6409 640a 8d03  q!t.j.|.d.d.d...
+00001720: 7d0f 7c02 a017 640b 7c0a 7c0f 7c07 7c08  }.|...d.|.|.|.|.
+00001730: 6602 7c07 7c08 6602 640c 9c05 a101 0100  f.|.|.f.d.......
+00001740: 7121 7117 7c02 5300 290d 6140 0300 000a  q!q.|.S.).a@....
+00001750: 2020 2020 4769 7665 6e20 6120 6d6f 6c65      Given a mole
+00001760: 6375 6c65 2060 606d 6f6c 6060 2c20 7468  cule ``mol``, th
+00001770: 6973 2066 756e 6374 696f 6e20 7769 6c6c  is function will
+00001780: 2072 6574 7572 6e20 6120 6c69 7374 206f   return a list o
+00001790: 6620 534d 494c 4553 2073 7472 696e 6773  f SMILES strings
+000017a0: 2077 6869 6368 2072 6573 756c 7473 2066   which results f
+000017b0: 726f 6d20 7661 6c69 640a 2020 2020 626f  rom valid.    bo
+000017c0: 6e64 2061 6464 6974 696f 6e73 2074 6f20  nd additions to 
+000017d0: 7468 6174 2062 6173 6520 6d6f 6c65 6375  that base molecu
+000017e0: 6c65 2e20 5661 6c69 6420 626f 6e64 2061  le. Valid bond a
+000017f0: 6464 6974 696f 6e73 2069 6e20 7468 6973  dditions in this
+00001800: 2063 6173 6520 6172 6520 6465 6669 6e65   case are define
+00001810: 6420 6173 2061 6c6c 6f77 6564 2069 6e0a  d as allowed in.
+00001820: 2020 2020 7465 726d 7320 6f66 2074 6865      terms of the
+00001830: 2061 746f 6d20 7661 6c65 6e63 6573 2e20   atom valences. 
+00001840: 626f 6e64 2061 6464 6974 696f 6e73 206d  bond additions m
+00001850: 6179 2063 6f6e 6e65 6374 2074 776f 2061  ay connect two a
+00001860: 746f 6d73 2077 6869 6368 2061 7265 206e  toms which are n
+00001870: 6f74 2079 6574 2064 6972 6563 746c 7920  ot yet directly 
+00001880: 636f 6e6e 6563 7465 640a 2020 2020 6f72  connected.    or
+00001890: 2075 7067 7261 6465 2061 6e20 6578 6973   upgrade an exis
+000018a0: 7469 6e67 2062 6f6e 6420 2873 696e 676c  ting bond (singl
+000018b0: 6520 746f 2064 6f75 626c 6529 2e0a 0a20  e to double)... 
+000018c0: 2020 2041 6c73 6f20 6469 7361 6c6c 6f77     Also disallow
+000018d0: 6564 2061 7265 2062 6f6e 6473 2062 6574  ed are bonds bet
+000018e0: 7765 656e 2074 776f 2061 746f 6d73 2077  ween two atoms w
+000018f0: 6869 6368 2061 7265 2074 6865 6d73 656c  hich are themsel
+00001900: 7665 7320 616c 7265 6164 7920 7061 7274  ves already part
+00001910: 206f 6620 6120 7269 6e67 2e0a 0a20 2020   of a ring...   
+00001920: 203a 7061 7261 6d20 6d6f 6c3a 2054 6865   :param mol: The
+00001930: 2062 6173 6520 6d6f 6c65 6375 6c65 0a20   base molecule. 
+00001940: 2020 203a 7061 7261 6d20 6672 6565 5f76     :param free_v
+00001950: 616c 656e 6365 5f69 6e64 6963 6573 5f6d  alence_indices_m
+00001960: 6170 3a20 4120 6469 6374 2077 686f 7365  ap: A dict whose
+00001970: 206b 6579 7320 6172 6520 696e 7465 6765   keys are intege
+00001980: 7273 2073 7461 7274 696e 6720 6672 6f6d  rs starting from
+00001990: 2030 2e20 5448 6520 6b65 7920 7661 6c75   0. THe key valu
+000019a0: 6573 0a20 2020 2020 2020 2072 6570 7265  es.        repre
+000019b0: 7365 6e74 2074 6865 202a 6672 6565 206e  sent the *free n
+000019c0: 756d 6265 7220 6f66 2076 616c 656e 6365  umber of valence
+000019d0: 732a 2e20 5468 6520 7661 6c75 6573 2061  s*. The values a
+000019e0: 7265 206c 6973 7473 206f 6620 6174 6f6d  re lists of atom
+000019f0: 2069 6e64 6963 6573 2077 6865 7265 2065   indices where e
+00001a00: 6163 6820 6174 6f6d 2069 6e0a 2020 2020  ach atom in.    
+00001a10: 2020 2020 7468 6520 6c69 7374 2068 6173      the list has
+00001a20: 2074 6f20 6861 7665 2074 6865 2063 6f72   to have the cor
+00001a30: 7265 7370 6f6e 6469 6e67 206e 756d 6265  responding numbe
+00001a40: 7220 6f66 2066 7265 6520 7661 6c65 6e63  r of free valenc
+00001a50: 6573 2067 6976 656e 2062 7920 7468 6520  es given by the 
+00001a60: 6469 6374 206b 6579 2e0a 0a20 2020 203a  dict key...    :
+00001a70: 7265 7475 726e 733a 2041 206c 6973 7420  returns: A list 
+00001a80: 6f66 2073 7472 696e 6773 0a20 2020 204e  of strings.    N
+00001a90: a904 7201 0000 0072 0a00 0000 7255 0000  ..r....r....rU..
+00001aa0: 0072 5600 0000 7255 0000 0054 a901 da12  .rV...rU...T....
+00001ab0: 636c 6561 7241 726f 6d61 7469 6346 6c61  clearAromaticFla
+00001ac0: 6773 7256 0000 0072 5700 0000 4672 0100  gsrV...rW...Fr..
+00001ad0: 0000 7259 0000 00da 0b6d 6f64 6966 795f  ..rY.....modify_
+00001ae0: 6564 6765 725d 0000 0029 1872 0200 0000  edger]...).r....
+00001af0: 7261 0000 0072 6200 0000 7263 0000 0072  ra...rb...rc...r
+00001b00: 6400 0000 7206 0000 0072 6500 0000 7232  d...r....re...r2
+00001b10: 0000 00da 0c63 6f6d 6269 6e61 7469 6f6e  .....combination
+00001b20: 73da 0e47 6574 4174 6f6d 5769 7468 4964  s..GetAtomWithId
+00001b30: 78da 0849 7349 6e52 696e 67da 034d 6f6c  x..IsInRing..Mol
+00001b40: da13 4765 7442 6f6e 6442 6574 7765 656e  ..GetBondBetween
+00001b50: 4174 6f6d 7372 6600 0000 da08 4b65 6b75  Atomsrf.....Keku
+00001b60: 6c69 7a65 da0b 4765 7442 6f6e 6454 7970  lize..GetBondTyp
+00001b70: 65da 0676 616c 7565 7372 4e00 0000 da0b  e..valuesrN.....
+00001b80: 5365 7442 6f6e 6454 7970 65da 0b52 6570  SetBondType..Rep
+00001b90: 6c61 6365 426f 6e64 7269 0000 0072 6a00  laceBondri...rj.
+00001ba0: 0000 726b 0000 0072 4400 0000 2910 7213  ..rk...rD...).r.
+00001bb0: 0000 0072 3a00 0000 726c 0000 0072 6d00  ...r:...rl...rm.
+00001bc0: 0000 da13 626f 6e64 5f74 7970 655f 7661  ....bond_type_va
+00001bd0: 6c75 655f 6d61 7072 7000 0000 da05 6174  lue_maprp.....at
+00001be0: 6f6d 73da 0561 746f 6d31 da05 6174 6f6d  oms..atom1..atom
+00001bf0: 32da 0462 6f6e 6472 7100 0000 726e 0000  2..bondrq...rn..
+00001c00: 00da 0a62 6f6e 645f 7661 6c75 65da 0569  ...bond_value..i
+00001c10: 6e64 6578 7273 0000 0072 2d00 0000 721c  ndexrs...r-...r.
+00001c20: 0000 0072 1c00 0000 721d 0000 0072 4100  ...r....r....rA.
+00001c30: 0000 ca00 0000 7350 0000 0004 1202 0306  ......sP........
+00001c40: 0106 0106 0106 fc08 0610 0214 011c 0302  ................
+00001c50: 0112 020a 010e 0208 0108 010c 0102 0108  ................
+00001c60: 0208 0108 0102 0108 020e 010e 0108 030e  ................
+00001c70: 010e 0204 0102 0110 0204 0102 0102 0102  ................
+00001c80: 0106 0106 010a fb02 df04 2972 4100 0000  ..........)rA...
+00001c90: 6301 0000 0000 0000 0000 0000 0012 0000  c...............
+00001ca0: 000a 0000 0043 0000 0073 e801 0000 6700  .....C...s....g.
+00001cb0: 7d01 6401 7400 6a01 6a02 7400 6a01 6a03  }.d.t.j.j.t.j.j.
+00001cc0: 7400 6a01 6a04 6402 9c04 7d02 7405 7c02  t.j.j.d...}.t.|.
+00001cd0: 8301 7d03 6403 4400 5ddc 7d04 7c00 a006  ..}.d.D.].}.|...
+00001ce0: a100 4400 5dd5 7d05 6401 7d06 7c05 a007  ..D.].}.d.}.|...
+00001cf0: a100 7c05 a008 a100 0202 7d07 7d08 7400  ..|.......}.}.t.
+00001d00: a009 7c00 a101 a00a 7c07 7c08 a102 7d05  ..|.....|.|...}.
+00001d10: 7c05 a00b a100 7d09 7c09 7c02 a00c a100  |.....}.|.|.....
+00001d20: 7601 723c 711b 7400 a00d 7c00 a101 7d0a  v.r<q.t...|...}.
+00001d30: 7400 6a0e 7c0a 6404 6405 8d02 0100 7c03  t.j.|.d.d.....|.
+00001d40: 7c09 1900 7d0b 7c0b 7c04 3800 7d0b 7c0b  |...}.|.|.8.}.|.
+00001d50: 6406 6b02 727c 7c0a a00f 7c07 7c08 a102  d.k.r||...|.|...
+00001d60: 0100 7c0a a010 7c07 a101 a011 a100 6406  ..|...|.......d.
+00001d70: 6b02 726b 7c0a a012 7c07 a101 0100 7c07  k.rk|...|.....|.
+00001d80: 7d06 6e28 7c0a a010 7c08 a101 a011 a100  }.n(|...|.......
+00001d90: 6406 6b02 727b 7c0a a012 7c08 a101 0100  d.k.r{|...|.....
+00001da0: 7c08 7d06 6e17 7c0b 6406 6b04 7292 7c05  |.}.n.|.d.k.r.|.
+00001db0: a013 7c02 7c0b 1900 a101 0100 7c05 a014  ..|.|.......|...
+00001dc0: a100 7d0c 7c0a a015 7c0c 7c05 a102 0100  ..}.|...|.|.....
+00001dd0: 6e01 711b 7400 6a16 7c0a 6404 6407 8d02  n.q.t.j.|.d.d...
+00001de0: 7d0d 7c0d 729d 711b 7400 6a17 7c0a 6408  }.|.r.q.t.j.|.d.
+00001df0: 6406 6409 8d03 7d0e 640a 7c0e 7600 72cd  d.d...}.d.|.v.r.
+00001e00: 7418 7c0e a019 640a a101 741a 640b 8d02  t.|...d...t.d...
+00001e10: 7d0f 741a 7c0f 6406 1900 8301 640c 6b04  }.t.|.d.....d.k.
+00001e20: 72bb 711b 741a 7400 a01b 7c0f 640c 1900  r.q.t.t...|.d...
+00001e30: a101 a01c a100 8301 640d 6b00 72c9 711b  ........d.k.r.q.
+00001e40: 7c0f 640c 1900 7d0e 7c07 7c06 6b03 72d3  |.d...}.|.|.k.r.
+00001e50: 7c07 6e01 7c08 7d10 7c08 7c06 6b03 72db  |.n.|.}.|.|.k.r.
+00001e60: 7c08 6e01 7c07 7d11 7c01 a01d 7c06 72e3  |.n.|.}.|...|.r.
+00001e70: 640e 6e01 640f 7c0a 7c0e 7c07 7c08 6602  d.n.d.|.|.|.|.f.
+00001e80: 7c10 7c11 6602 6410 9c05 a101 0100 711b  |.|.f.d.......q.
+00001e90: 7115 7c01 5300 2911 61a2 0100 000a 2020  q.|.S.).a.....  
+00001ea0: 2020 4769 7665 6e20 6120 6d6f 6c65 6375    Given a molecu
+00001eb0: 6c65 2060 606d 6f6c 6060 2c20 7468 6973  le ``mol``, this
+00001ec0: 2066 756e 6374 696f 6e20 7769 6c6c 2072   function will r
+00001ed0: 6574 7572 6e20 6120 6c69 7374 206f 6620  eturn a list of 
+00001ee0: 534d 494c 4553 2073 7472 696e 6773 2077  SMILES strings w
+00001ef0: 6869 6368 2072 6570 7265 7365 6e74 2076  hich represent v
+00001f00: 616c 6964 0a20 2020 2062 6f6e 6420 7265  alid.    bond re
+00001f10: 6d6f 7661 6c73 2e20 4120 626f 6e64 2072  movals. A bond r
+00001f20: 656d 6f76 616c 2069 7320 6569 7468 6572  emoval is either
+00001f30: 2061 2064 6f77 6e67 7261 6465 206f 6620   a downgrade of 
+00001f40: 616e 2065 7869 7374 696e 6720 626f 6e64  an existing bond
+00001f50: 2028 652e 672e 2064 6f75 626c 6520 746f   (e.g. double to
+00001f60: 2073 696e 676c 6529 206f 7220 7468 650a   single) or the.
+00001f70: 2020 2020 7265 6d6f 7661 6c20 6f66 2061      removal of a
+00001f80: 2073 696e 676c 6520 626f 6e64 2077 6869   single bond whi
+00001f90: 6368 2077 6f75 6c64 206d 6561 6e20 746f  ch would mean to
+00001fa0: 2064 6973 636f 6e6e 6563 7420 6174 206d   disconnect at m
+00001fb0: 6f73 7420 6120 7369 6e67 6c65 2061 746f  ost a single ato
+00001fc0: 6d20 6672 6f6d 2074 6865 2072 6573 7420  m from the rest 
+00001fd0: 6f66 2074 6865 0a20 2020 206d 6f6c 6563  of the.    molec
+00001fe0: 756c 6521 0a0a 2020 2020 3a70 6172 616d  ule!..    :param
+00001ff0: 206d 6f6c 3a20 5468 6520 6261 7365 206d   mol: The base m
+00002000: 6f6c 6563 756c 6520 666f 7220 7468 6520  olecule for the 
+00002010: 7265 6d6f 7661 6c73 2e0a 0a20 2020 203a  removals...    :
+00002020: 7265 7475 726e 733a 2041 206c 6973 7420  returns: A list 
+00002030: 6f66 2073 7472 696e 6773 0a20 2020 204e  of strings.    N
+00002040: 7274 0000 0072 5400 0000 5472 7500 0000  rt...rT...Tru...
+00002050: 7201 0000 0072 5700 0000 4672 5900 0000  r....rW...FrY...
+00002060: da01 2e29 01da 036b 6579 720a 0000 0072  ...)...keyr....r
+00002070: 5500 0000 da0b 7265 6d6f 7665 5f65 6467  U.....remove_edg
+00002080: 6572 7700 0000 725d 0000 0029 1e72 0200  erw...r]...).r..
+00002090: 0000 7261 0000 0072 6200 0000 7263 0000  ..ra...rb...rc..
+000020a0: 0072 6400 0000 7206 0000 00da 0847 6574  .rd...r......Get
+000020b0: 426f 6e64 73da 0f47 6574 4265 6769 6e41  Bonds..GetBeginA
+000020c0: 746f 6d49 6478 da0d 4765 7445 6e64 4174  tomIdx..GetEndAt
+000020d0: 6f6d 4964 7872 7b00 0000 727c 0000 0072  omIdxr{...r|...r
+000020e0: 7e00 0000 727f 0000 0072 6600 0000 727d  ~...r....rf...r}
+000020f0: 0000 00da 0a52 656d 6f76 6542 6f6e 6472  .....RemoveBondr
+00002100: 7900 0000 da09 4765 7444 6567 7265 65da  y.....GetDegree.
+00002110: 0a52 656d 6f76 6541 746f 6d72 8000 0000  .RemoveAtomr....
+00002120: 724e 0000 0072 8100 0000 726a 0000 0072  rN...r....rj...r
+00002130: 6b00 0000 da06 736f 7274 6564 da05 7370  k.....sorted..sp
+00002140: 6c69 74da 036c 656e 723e 0000 0072 5300  lit..lenr>...rS.
+00002150: 0000 7244 0000 0029 1272 1300 0000 726c  ..rD...).r....rl
+00002160: 0000 0072 6d00 0000 7282 0000 0072 7000  ...rm...r....rp.
+00002170: 0000 7286 0000 00da 0c61 746f 6d5f 7265  ..r......atom_re
+00002180: 6d6f 7665 6472 8400 0000 7285 0000 0072  movedr....r....r
+00002190: 6e00 0000 7271 0000 0072 8700 0000 7288  n...rq...r....r.
+000021a0: 0000 0072 7300 0000 722d 0000 00da 0570  ...rs...r-.....p
+000021b0: 6172 7473 da04 6d6f 6431 da04 6d6f 6432  arts..mod1..mod2
+000021c0: 721c 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
+000021d0: 4200 0000 1301 0000 736e 0000 0004 0c02  B.......sn......
+000021e0: 0306 0106 0106 0106 fc08 0608 020c 0104  ................
+000021f0: 0112 0112 0108 020c 0102 010a 020e 0108  ................
+00002200: 0208 0108 040c 0112 020a 0106 0112 010a  ................
+00002210: 0104 0102 8008 020e 0108 010e 0102 030e  ................
+00002220: 0204 0102 0110 0208 0112 0110 0102 011a  ................
+00002230: 0602 0108 0210 0210 0104 010a 0102 0102  ................
+00002240: 0106 0106 010a fb02 c804 4072 4200 0000  ..........@rB...
+00002250: 2901 7212 0000 0029 0172 1f00 0000 2901  ).r....).r....).
+00002260: 724b 0000 0029 1f72 3200 0000 da06 7479  rK...).r2.....ty
+00002270: 7069 6e67 da01 74da 0572 646b 6974 7202  ping..t..rdkitr.
+00002280: 0000 00da 0a72 646b 6974 2e43 6865 6d72  .....rdkit.Chemr
+00002290: 0300 0000 7204 0000 00da 0d64 696d 6f72  ....r......dimor
+000022a0: 7068 6974 655f 646c 7205 0000 00da 1976  phite_dlr......v
+000022b0: 6764 5f63 6f75 6e74 6572 6661 6374 7561  gd_counterfactua
+000022c0: 6c73 2e75 7469 6c73 7206 0000 00da 1844  ls.utilsr......D
+000022d0: 4546 4155 4c54 5f41 544f 4d5f 5641 4c45  EFAULT_ATOM_VALE
+000022e0: 4e43 455f 4d41 5072 7b00 0000 da03 7374  NCE_MAPr{.....st
+000022f0: 7272 1e00 0000 7220 0000 00da 044c 6973  rr....r .....Lis
+00002300: 74da 0566 6c6f 6174 7236 0000 00da 0853  t..floatr6.....S
+00002310: 6571 7565 6e63 65da 0843 616c 6c61 626c  equence..Callabl
+00002320: 65da 0462 6f6f 6c72 4a00 0000 da03 696e  e..boolrJ.....in
+00002330: 74da 0464 6963 7472 3f00 0000 da04 4469  t..dictr?.....Di
+00002340: 6374 7240 0000 0072 4100 0000 7242 0000  ctr@...rA...rB..
+00002350: 0072 1c00 0000 721c 0000 0072 1c00 0000  .r....r....r....
+00002360: 721d 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00002370: 0000 0073 7200 0000 0800 0801 0c01 0c01  ...sr...........
+00002380: 0c01 0c02 0c01 0204 0201 0202 0201 0201  ................
+00002390: 0201 06f9 160b 160a 0c06 0201 02ff 0202  ................
+000023a0: 02fe 0803 0afd 0213 0202 0201 02fe 0204  ................
+000023b0: 0201 0201 08f8 1c02 02fe 0206 02fa 0207  ................
+000023c0: 02f9 0208 02f8 0809 0af7 1a53 080c 0c01  ...........S....
+000023d0: 02ff 1202 02fe 0803 0afd 0833 1201 02ff  ...........3....
+000023e0: 0802 0afe 0849 0801 0eff                 .....I....
```

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/molecules.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/generate/molecules.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,68 +1,28 @@
 import itertools
 import typing as t
 from rdkit import Chem
 from rdkit.Chem import rdFMCS
 from rdkit.Chem import AllChem
 
+from dimorphite_dl import DimorphiteDL
 from vgd_counterfactuals.utils import invert_dict
 
 
 DEFAULT_ATOM_VALENCE_MAP = {
     'C': 4,
     'N': 5,
     # 'P': 5,
     'O': 6,
     'F': 1,
     'Cl': 7,
     'S': 6,
 }
 
 
-
-def molecule_differences(mol1: Chem.Mol,
-                         mol2: Chem.Mol,
-                         radius: int = 0,
-                         ) -> t.Tuple[str, str]:
-    """
-    """
-    for mol in [mol1, mol2]:
-        for atom in mol.GetAtoms():
-            value = sum(bond.GetBondType() + bond.GetBondDir() for bond in atom.GetBonds())
-            atom.SetIsotope(value)
-
-    mcs = rdFMCS.FindMCS(
-        [mol1, mol2],
-        atomCompare=rdFMCS.AtomCompare.CompareIsotopes,
-    )
-    common_substructure = Chem.MolFromSmarts(mcs.smartsString)
-
-    results = []
-    for mol in [mol1, mol2]:
-        match = mol.GetSubstructMatch(common_substructure)
-        non_matches = set([index for atom in mol.GetAtoms() if (index := atom.GetIdx()) not in match])
-        for r in range(radius):
-            neighbors = []
-            for atom_index in non_matches:
-                atom = mol.GetAtomWithIdx(atom_index)
-                neighbors += [a.GetIdx() for a in atom.GetNeighbors()]
-
-            non_matches.update(set(neighbors))
-
-        for atom in mol.GetAtoms():
-            atom.SetIsotope(0)
-
-        if len(non_matches) != 0:
-            results.append(Chem.MolFragmentToSmiles(mol, atomsToUse=list(non_matches)))
-        else:
-            results.append('')
-
-    return results
-
-
 def is_bridge_head_carbon(mol: Chem.Mol, pattern: str = '*1=**2=**=*1*2'):
     """
     Checks if the given molecule ``mol`` is a bridge head carbon structure which apparently does not
     appear in chemistry.
     """
     smarts = Chem.MolFromSmarts(pattern)
     is_match = mol.HasSubstructMatch(smarts)
@@ -71,20 +31,41 @@
 
 def is_nitrogen_nitrogen_sulfur(mol: Chem.Mol, pattern: str = 'SNN'):
     smarts = Chem.MolFromSmarts(pattern)
     is_match = mol.HasSubstructMatch(smarts)
     return is_match
 
 
+def fix_protonation_dimorphite(smiles_list: t.List[str],
+                               min_ph: float,
+                               max_ph: float,
+                               ) -> t.List[str]:
+    dmph = DimorphiteDL(
+        min_ph=min_ph,
+        max_ph=max_ph,
+        max_variants=10,
+        label_states=False,
+        pka_precision=1.0,
+    )
+    result = list(itertools.chain.from_iterable(
+        [dmph.protonate(smiles) for smiles in smiles_list]
+    ))
+
+    return result
+
+
 def get_neighborhood(smiles: str,
                      atom_valence_map=DEFAULT_ATOM_VALENCE_MAP,
-                     mol_filters: t.Sequence[t.Callable[[Chem.Mol], bool]] = (
+                     mol_filters: t.Sequence[t.Callable[[Chem.Mol], t.List[str]]] = (
                         is_bridge_head_carbon,
                         is_nitrogen_nitrogen_sulfur,
                      ),
+                     fix_protonation: bool = False,
+                     max_ph: float = 6.4,
+                     min_ph: float = 6.4,
                      ) -> t.List[str]:
     """
     Given a ``smiles`` representation of a molecule, this function will return a list of the SMILES
     representations of all the valid molecules within a 1-edit neighborhood. Optionally, a list of boolean
     functions can be provided for ``mol_filters`` to further limit the kinds of molecules included in the
     result.
 
@@ -94,47 +75,69 @@
         atoms that are listed in this dict will be considered for edit operations such as adding or
         replacing and atom!
     :param mol_filters: A list of functions which each take a Mol object as input and return a boolean value
         to determine whether that atom should be excluded (True) or not (False).
 
     :returns: A list of strings
     """
-    neighbors_set = set()
+    neighbors = []
 
     mol = Chem.MolFromSmiles(smiles)
     free_valence_indices_map = get_free_valence_map(mol)
 
-    neighbors_set.update(get_valid_atom_additions(
+    neighbors += get_valid_atom_additions(
         mol=mol,
         atom_valence_map=atom_valence_map,
         free_valence_indices_map=free_valence_indices_map,
-    ))
+    )
 
-    neighbors_set.update(get_valid_bond_additions(
+    neighbors += get_valid_bond_additions(
         mol=mol,
         free_valence_indices_map=free_valence_indices_map,
-    ))
+    )
 
-    neighbors_set.update(get_valid_bond_removals(
+    neighbors += get_valid_bond_removals(
         mol=mol
-    ))
+    )
 
     # 15.05.23 - All of the above functions will create "valid" molecular SMILES in the sense that RDKit
     # does not tell us that they are completely wrong, but the molecules that are created might still not
     # realistically exist in chemistry, which is why we additionally apply a set of filters that decide
     # for each molecule if it should be included
     neighbors_filtered = []
-    for smiles in neighbors_set:
-        mol = Chem.MolFromSmiles(smiles)
+    for data in neighbors:
+        mol = data['mol']
         if any([func(mol) for func in mol_filters]):
             continue
 
-        neighbors_filtered.append(smiles)
+        neighbors_filtered.append(data)
 
-    return neighbors_filtered
+    neighbors = neighbors_filtered
+
+    # 01.06.2023 - One problem we have encountered when dealing with the counterfactuals for the aggregation
+    # task is that the generated molecules are often times not "realistic" in the sense that they are not
+    # correctly protonated for the target pH range of the task.
+    # This is why we introduce the option to fix the protonation state of these with an external tool here.
+    if fix_protonation:
+        neighbors_protonated = []
+        dmph = DimorphiteDL(
+            min_ph=min_ph,
+            max_ph=max_ph,
+            max_variants=10,
+            label_states=False,
+            pka_precision=1.0,
+        )
+        for data in neighbors:
+            smiles_protonated = dmph.protonate(data['value'])
+            for smiles in smiles_protonated:
+                neighbors_protonated.append({**data, 'value': smiles})
+
+        neighbors = neighbors_protonated
+
+    return neighbors
 
 
 def get_free_valence_map(mol: Chem.Mol, max_valence: int = 8) -> dict:
     result = {}
     for i in range(1, max_valence):
         result[i] = [
             atom.GetIdx()
@@ -144,22 +147,33 @@
 
     return result
 
 
 def get_valid_atom_additions(mol: Chem.Mol,
                              atom_valence_map: t.Dict[str, int],
                              free_valence_indices_map: t.Dict[int, t.List[int]]
-                             ) -> t.Set[str]:
+                             ) -> t.List[dict]:
     """
     Given a molecule ``mol``, this function will return a list of SMILES strings that represent valid
     atom additions to the base molecule.
 
-    :returns: A list of strings.
+    :param mol: The original molecule for which to calculate the modifications
+    :param atom_valence_map: A dict whose keys are string identifiers of atom types (O, N, S...) and the
+        values are the integer valences associated with these atom types.
+    :param free_valence_indices_map: A dict whose keys are integer values for possible atom valences in the
+        molecule and the values are lists containing integer node indices of all the atoms which have that
+        corresponding valence.
+
+    :returns: A list of dictionaries which define the valid modifications. Each dictionary has the keys
+        - mol: The mol object of the NEW molecule
+        - smiles: The SMILES string of the NEW molecule
+        - org: The integer atom index of the ORIGINAL molecule where the modification originates
+        - mod: The integer atom index of the NEW molecule where the modification occurred
     """
-    results = set()
+    results = []
 
     value_bond_type_map = {
         1: Chem.BondType.SINGLE,
         2: Chem.BondType.DOUBLE,
         3: Chem.BondType.TRIPLE,
     }
     for i, bond_type in value_bond_type_map.items():
@@ -169,23 +183,29 @@
                 new_mol = Chem.RWMol(mol)
                 idx = new_mol.AddAtom(Chem.Atom(element))
                 new_mol.AddBond(atom, idx, bond_type)
                 sanitization_result = Chem.SanitizeMol(new_mol, catchErrors=True)
                 if sanitization_result:
                     continue
 
-                smiles = Chem.MolToSmiles(new_mol)
-                results.add(smiles)
+                smiles = Chem.MolToSmiles(new_mol, canonical=False, rootedAtAtom=0)
+                results.append({
+                    'type':     'add_node',
+                    'mol':      new_mol,
+                    'value':    smiles,
+                    'org':      (atom, atom),
+                    'mod':      (atom, idx),
+                })
 
     return results
 
 
 def get_valid_bond_additions(mol: Chem.Mol,
                              free_valence_indices_map: t.Dict[int, t.List[int]]
-                             ) -> t.Set[str]:
+                             ) -> t.List[dict]:
     """
     Given a molecule ``mol``, this function will return a list of SMILES strings which results from valid
     bond additions to that base molecule. Valid bond additions in this case are defined as allowed in
     terms of the atom valences. bond additions may connect two atoms which are not yet directly connected
     or upgrade an existing bond (single to double).
 
     Also disallowed are bonds between two atoms which are themselves already part of a ring.
@@ -193,15 +213,15 @@
     :param mol: The base molecule
     :param free_valence_indices_map: A dict whose keys are integers starting from 0. THe key values
         represent the *free number of valences*. The values are lists of atom indices where each atom in
         the list has to have the corresponding number of free valences given by the dict key.
 
     :returns: A list of strings
     """
-    results = set()
+    results = []
 
     value_bond_type_map = {
         0: None,
         1: Chem.BondType.SINGLE,
         2: Chem.BondType.DOUBLE,
         3: Chem.BondType.TRIPLE,
     }
@@ -236,84 +256,108 @@
                 bond_type = value_bond_type_map[valence]
                 new_mol.AddBond(atom1, atom2, bond_type)
 
             sanitization_result = Chem.SanitizeMol(new_mol, catchErrors=True)
             if sanitization_result:
                 continue
 
-            smiles = Chem.MolToSmiles(new_mol)
-            results.add(smiles)
+            smiles = Chem.MolToSmiles(new_mol, canonical=False, rootedAtAtom=0)
+            results.append({
+                'type':     'modify_edge',
+                'mol':      new_mol,
+                'value':    smiles,
+                'org':      (atom1, atom2),
+                'mod':      (atom1, atom2),
+            })
 
     return results
 
 
 def get_valid_bond_removals(mol: Chem.Mol
-                            ) -> t.Set[str]:
+                            ) -> t.List[dict]:
     """
     Given a molecule ``mol``, this function will return a list of SMILES strings which represent valid
     bond removals. A bond removal is either a downgrade of an existing bond (e.g. double to single) or the
     removal of a single bond which would mean to disconnect at most a single atom from the rest of the
     molecule!
 
     :param mol: The base molecule for the removals.
 
     :returns: A list of strings
     """
-    results = set()
+    results = []
 
     value_bond_type_map = {
         0: None,
         1: Chem.BondType.SINGLE,
         2: Chem.BondType.DOUBLE,
         3: Chem.BondType.TRIPLE,
     }
     bond_type_value_map = invert_dict(value_bond_type_map)
 
     for valence in [1, 2, 3]:
         for bond in mol.GetBonds():
+            atom_removed = None
             atom1, atom2 = bond.GetBeginAtomIdx(), bond.GetEndAtomIdx()
             bond = Chem.Mol(mol).GetBondBetweenAtoms(atom1, atom2)
 
             bond_type = bond.GetBondType()
             if bond_type not in value_bond_type_map.values():
                 continue
 
             new_mol = Chem.RWMol(mol)
             Chem.Kekulize(new_mol, clearAromaticFlags=True)
 
             bond_value = bond_type_value_map[bond_type]
             bond_value -= valence
 
+            # In this case, if the bond value has been evaluated to zero then that means that we want to
+            # completely remove that bond.
             if bond_value == 0:
                 new_mol.RemoveBond(atom1, atom2)
 
+                if new_mol.GetAtomWithIdx(atom1).GetDegree() == 0:
+                    new_mol.RemoveAtom(atom1)
+                    atom_removed = atom1
+                elif new_mol.GetAtomWithIdx(atom2).GetDegree() == 0:
+                    new_mol.RemoveAtom(atom2)
+                    atom_removed = atom2
+
             elif bond_value > 0:
                 bond.SetBondType(value_bond_type_map[bond_value])
                 index = bond.GetIdx()
                 new_mol.ReplaceBond(index, bond)
 
             else:
                 continue
 
             sanitization_result = Chem.SanitizeMol(new_mol, catchErrors=True)
             if sanitization_result:
                 continue
 
-            smiles = Chem.MolToSmiles(new_mol)
+            smiles = Chem.MolToSmiles(new_mol, canonical=False, rootedAtAtom=0)
             if '.' in smiles:
                 parts = sorted(smiles.split('.'), key=len)
                 if len(parts[0]) > 1:
                     continue
 
                 # 10.05.23 - Not filtering this has caused a bug in the down stream machine learning because
                 # we would have essentially allowed "molecules" only consisting of a single atom and those
                 # "graphs" would have no edges at all, which is a case that graph neural networks are not
                 # prepared to handle.
                 if len(Chem.MolFromSmiles(parts[1]).GetAtoms()) < 2:
                     continue
 
                 smiles = parts[1]
 
-            results.add(smiles)
+            mod1 = atom1 if atom1 != atom_removed else atom2
+            mod2 = atom2 if atom2 != atom_removed else atom1
+            results.append({
+                'type':     'remove_edge' if atom_removed else 'modify_edge',
+                'mol':      new_mol,
+                'value':    smiles,
+                'org':      (atom1, atom2),
+                'mod':      (mod1, mod2),
+            })
 
     return results
```

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/generate/smiles_one_step_changes.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/generate/smiles_one_step_changes.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/templates/article.tex.j2` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/templates/article.tex.j2`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/utils.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/utils.py`

 * *Files identical despite different names*

### Comparing `vgd_counterfactuals-0.1.6/vgd_counterfactuals/visualization.py` & `vgd_counterfactuals-0.2.0/vgd_counterfactuals/visualization.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,30 @@
 import typing as t
 
+import numpy as np
 import matplotlib.pyplot as plt
 import visual_graph_datasets.typing as tv
 from matplotlib.backends.backend_pdf import PdfPages
 from imageio.v2 import imread
 
 
+def plot_modification(ax: plt.Axes,
+                      node_positions: np.ndarray,
+                      index1: t.Tuple[float, float],
+                      index2: t.Tuple[float, float],
+                      size: float = 500,
+                      alpha: float = 0.5,
+                      ) -> None:
+    pos1 = node_positions[index1]
+    pos2 = node_positions[index2]
+
+    ax.scatter(*pos1, s=size, color='red', alpha=alpha, zorder=-1, linewidths=0)
+    ax.scatter(*pos2, s=size, color='blue', alpha=alpha, zorder=-1, linewidths=0)
+
+
 def create_counterfactual_pdf(counterfactual_elements: t.List[tv.VgdElementDict],
                               output_path: str,
                               original_element: t.Optional[tv.VgdElementDict] = None,
                               original_label: t.Optional[str] = None,
                               counterfactual_labels: t.Optional[t.List[str]] = None,
                               counterfactual_color: t.Any = '#FFDCDC',
                               base_fig_size: int = 10,
```

### Comparing `vgd_counterfactuals-0.1.6/PKG-INFO` & `vgd_counterfactuals-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgd-counterfactuals
-Version: 0.1.6
+Version: 0.2.0
 Summary: Counterfactual explanations for GNNs based on the visual graph dataset format
 License: MIT
 Keywords: graph neural networks,counterfactuals,explainable AI
 Author: Jonas Teufel
 Author-email: jonseb1998@gmail.com
 Maintainer: Jonas Teufel
 Maintainer-email: jonseb1998@gmail.com
@@ -12,14 +12,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=7.1.2)
+Requires-Dist: dimorphite-dl (>=1.3.2)
 Requires-Dist: jinja2 (>=3.0.3)
 Requires-Dist: matplotlib (>=3.5.3)
 Requires-Dist: numpy (>=1.23.2)
 Requires-Dist: poetry-bumpversion (>=0.3.0)
 Requires-Dist: pycomex (>=0.9.2)
 Requires-Dist: python-decouple (>=3.6)
 Requires-Dist: rdkit (>=2022.9.5)
@@ -32,15 +33,15 @@
    :target: https://www.python.org/
    :alt: made with python
 
 .. |python-version| image:: https://img.shields.io/badge/Python-3.8.0-green.svg
    :target: https://www.python.org/
    :alt: python 3.8
 
-.. |version| image:: https://img.shields.io/badge/version-0.1.6-orange.svg
+.. |version| image:: https://img.shields.io/badge/version-0.2.0-orange.svg
    :target: https://www.python.org/
    :alt: version
 
 .. image:: banner.png
    :alt: banner image
 
 ===================
```

