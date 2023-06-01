# Comparing `tmp/kfactory-0.7.4.tar.gz` & `tmp/kfactory-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.7.4.tar", last modified: Mon May 29 21:48:49 2023, max compression
+gzip compressed data, was "kfactory-0.7.5.tar", last modified: Thu Jun  1 16:20:52 2023, max compression
```

## Comparing `kfactory-0.7.4.tar` & `kfactory-0.7.5.tar`

### file list

```diff
@@ -1,109 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.708952 kfactory-0.7.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-29 21:48:25.000000 kfactory-0.7.4/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-05-29 21:48:25.000000 kfactory-0.7.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-29 21:48:25.000000 kfactory-0.7.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-29 21:48:25.000000 kfactory-0.7.4/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-29 21:48:25.000000 kfactory-0.7.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 21:48:25.000000 kfactory-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-29 21:48:25.000000 kfactory-0.7.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-29 21:48:49.708952 kfactory-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-29 21:48:25.000000 kfactory-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/changelog.d/
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 21:48:25.000000 kfactory-0.7.4/changelog.d/changelog_template.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.692952 kfactory-0.7.4/docs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/overrides/main.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.696952 kfactory-0.7.4/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.696952 kfactory-0.7.4/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/config.md
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/gen_ref_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/intro.md
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.700952 kfactory-0.7.4/docs/source/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/notebooks/02_DRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/notebooks/03_Enclosures.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/pre.md
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-05-29 21:48:25.000000 kfactory-0.7.4/docs/source/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-29 21:48:25.000000 kfactory-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 21:48:49.708952 kfactory-0.7.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.688952 kfactory-0.7.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.700952 kfactory-0.7.4/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.700952 kfactory-0.7.4/src/kfactory/cells/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.704952 kfactory-0.7.4/src/kfactory/cells/dbu/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/dbu/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/cells/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    90744 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/kcell.py
--rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.704952 kfactory-0.7.4/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.704952 kfactory-0.7.4/src/kfactory/technology/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/color_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/klayout_tech.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/layer_map.py
--rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/layer_stack.py
--rw-r--r--   0 runner    (1001) docker     (123)    41776 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/layer_views.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/xml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/technology/yaml_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/typings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.704952 kfactory-0.7.4/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55837 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/utils/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/utils/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/utils/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.708952 kfactory-0.7.4/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-05-29 21:48:25.000000 kfactory-0.7.4/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.700952 kfactory-0.7.4/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-29 21:48:49.000000 kfactory-0.7.4/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-05-29 21:48:49.000000 kfactory-0.7.4/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 21:48:49.000000 kfactory-0.7.4/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-29 21:48:49.000000 kfactory-0.7.4/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 21:48:49.000000 kfactory-0.7.4/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:48:49.708952 kfactory-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_cells.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_cplxcells.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_pdk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-29 21:48:25.000000 kfactory-0.7.4/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.438962 kfactory-0.7.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-06-01 16:20:34.000000 kfactory-0.7.5/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-01 16:20:34.000000 kfactory-0.7.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-06-01 16:20:34.000000 kfactory-0.7.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 16:20:34.000000 kfactory-0.7.5/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-01 16:20:34.000000 kfactory-0.7.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-01 16:20:34.000000 kfactory-0.7.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-06-01 16:20:34.000000 kfactory-0.7.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-01 16:20:52.438962 kfactory-0.7.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-01 16:20:34.000000 kfactory-0.7.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/changelog.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-01 16:20:34.000000 kfactory-0.7.5/changelog.d/changelog_template.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/docs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/overrides/main.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.430962 kfactory-0.7.5/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/config.md
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/gdsfactory.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/intro.md
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/docs/source/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10562 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/notebooks/03_Enclosures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/pre.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-01 16:20:34.000000 kfactory-0.7.5/docs/source/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-06-01 16:20:34.000000 kfactory-0.7.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:20:52.438962 kfactory-0.7.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.426962 kfactory-0.7.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/src/kfactory/cells/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/src/kfactory/cells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/dbu/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/cells/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3432 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94080 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/kcell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8807 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9940 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12507 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20414 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.438962 kfactory-0.7.5/src/kfactory/technology/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/klayout_tech.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/layer_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14087 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/layer_stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41776 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/layer_views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/xml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/technology/yaml_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/typings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.438962 kfactory-0.7.5/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55837 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/utils/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/utils/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/utils/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9316 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.438962 kfactory-0.7.5/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14853 2023-06-01 16:20:34.000000 kfactory-0.7.5/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.434962 kfactory-0.7.5/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-06-01 16:20:52.000000 kfactory-0.7.5/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-01 16:20:52.000000 kfactory-0.7.5/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:20:52.000000 kfactory-0.7.5/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-01 16:20:52.000000 kfactory-0.7.5/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 16:20:52.000000 kfactory-0.7.5/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:20:52.438962 kfactory-0.7.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2775 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3682 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_cells.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_cplxcells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_pdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-06-01 16:20:34.000000 kfactory-0.7.5/tests/test_spiral.py
```

### Comparing `kfactory-0.7.4/.github/ISSUE_TEMPLATE/bug_report.md` & `kfactory-0.7.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/.github/ISSUE_TEMPLATE/feature_request.md` & `kfactory-0.7.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/.github/workflows/pages.yml` & `kfactory-0.7.5/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/.github/workflows/release.yml` & `kfactory-0.7.5/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/.github/workflows/test_code.yml` & `kfactory-0.7.5/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/.pre-commit-config.yaml` & `kfactory-0.7.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/LICENSE` & `kfactory-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/Makefile` & `kfactory-0.7.5/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/PKG-INFO` & `kfactory-0.7.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.7.4
+Version: 0.7.5
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.7.4
+# KFactory 0.7.5
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.4` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.5` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.7.4/README.md` & `kfactory-0.7.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-# KFactory 0.7.4
+# KFactory 0.7.5
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.4` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.5` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.7.4/docs/mkdocs.yml` & `kfactory-0.7.5/docs/mkdocs.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 site_name: KFactory
 repo_url: https://github.com/gdsfactory/kfactory
 site_url: https://gdsfactory.github.io/kfactory
 docs_dir: source
 
 nav:
-  - Home: index.md
+  - Home:
+    - Intro: index.md
+    - gdsfactory.md
   - First Steps:
     - Prerequisites: pre.md
     - 5min Intro to KFactory: intro.md
   - Tutorials:
     - Basice Geometry in KLayout: notebooks/00_geometry.py
     - KCell & Instance: notebooks/01_references.py
     - DRC utils: notebooks/02_DRC.py
     - Enclosures: notebooks/03_Enclosures.py
   - Config Class: config.md
   - API: reference/
+  - Changelog: changelog.md
 theme:
   name: "material"
   features:
     - navigation.tabs
     - navigation.tabs.sticky
   custom_dir: overrides
 
@@ -33,14 +36,15 @@
       toggle:
         icon: material/brightness-7
         name: Switch to dark mode
 watch:
   - ../src/kfactory
 
 markdown_extensions:
+  - admonition
   - pymdownx.superfences
   - pymdownx.tasklist
   - pymdownx.tabbed
   - pymdownx.emoji
   - pymdownx.snippets:
       check_paths: true
```

### Comparing `kfactory-0.7.4/docs/source/_static/complex.png` & `kfactory-0.7.5/docs/source/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/_static/klive.webm` & `kfactory-0.7.5/docs/source/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/_static/waveguide.png` & `kfactory-0.7.5/docs/source/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/complex_cell.py` & `kfactory-0.7.5/docs/source/complex_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/gen_ref_pages.py` & `kfactory-0.7.5/docs/source/gen_ref_pages.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/intro.md` & `kfactory-0.7.5/docs/source/intro.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/notebooks/00_geometry.py` & `kfactory-0.7.5/docs/source/notebooks/00_geometry.py`

 * *Files 9% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # - `DPoint`, `DBox`, `DPolygon`, `DEdge` are in microns
 #
 # Most Shape types are available as microns and dbu parts. They can be converted with `<ShapeTypeDBU>.to_dtype(dbu)` to microns and with `<ShapeTypeMicrons>.to_itype(dbu)` where `dbu` is the the conversion of one database unit to microns
 
 
 # %%
 import kfactory as kf
+import numpy as np
 
 # %%
 # Create a blank cell (essentially an empty GDS cell with some special features)
 c = kf.KCell()
 
 # %%
 # Create and add a polygon from separate lists of x points and y points
@@ -57,14 +58,22 @@
 
 # %% [markdown]
 # **Exercise** :
 #
 # Make a cell similar to the one above that has a second polygon in layer (1, 1)
 
 # %%
+c = kf.KCell()
+points = np.array([(-8, -6), (6, 8), (7, 17), (9, 5)])
+poly = kf.polygon_from_array(points)
+c.shapes(c.kcl.layer(1, 0)).insert(poly1)
+c.shapes(c.kcl.layer(1, 1)).insert(poly1)
+c
+
+# %%
 import kfactory as kf
 
 # %%
 c = kf.KCell()
 
 # %%
 # Create some new geometry from the functions available in the geometry library
@@ -261,17 +270,41 @@
 # %%
 # Like before, let's connect mwg1 and mwg2 together
 mwg1_ref.connect("o2", mwg2_ref.ports["o1"])
 
 # %%
 c2
 
+# %%
+c = kf.KCell()
+bend = kf.cells.euler.bend_euler(radius=10, width=1, layer=0)
+b1 = c << bend
+b2 = c << bend
+b2.mirror_x(x=0)
+c
+
+# %%
+c = kf.KCell()
+bend = kf.cells.euler.bend_euler(radius=10, width=1, layer=0)
+b1 = c << bend
+b2 = c << bend
+b2.mirror_y(y=0)
+c
+
+# %%
+c = kf.KCell()
+bend = kf.cells.euler.bend_euler(radius=10, width=1, layer=0)
+b1 = c << bend
+b2 = c << bend
+b2.mirror_y(y=0)
+b1.ymin = b2.ymax
+c
+
 # %% [markdown]
 #
-#             self.layout_view.active_cellview().layout().cell(event["owner"].name)
 # ## Labels
 #
 # You can add abstract GDS labels (annotate) to your Cells, in order to record information
 # directly into the final GDS file without putting any extra geometry onto any layer
 # This label will display in a GDS viewer, but will not be rendered or printed
 # like the polygons created by gf.cells.text().
```

### Comparing `kfactory-0.7.4/docs/source/notebooks/01_references.py` & `kfactory-0.7.5/docs/source/notebooks/01_references.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/notebooks/02_DRC.py` & `kfactory-0.7.5/docs/source/notebooks/02_DRC.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/notebooks/03_Enclosures.py` & `kfactory-0.7.5/docs/source/notebooks/03_Enclosures.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/pre.md` & `kfactory-0.7.5/docs/source/pre.md`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/star.py` & `kfactory-0.7.5/docs/source/star.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/docs/source/waveguide.py` & `kfactory-0.7.5/docs/source/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/pyproject.toml` & `kfactory-0.7.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 
 
-version = "0.7.4"
+version = "0.7.5"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
 	"klayout >= 0.28.3",
 	"scipy",
 	"ruamel.yaml",
@@ -102,15 +102,15 @@
 strict = true
 exclude = [
 	"tests",
 	"src/kfactory/widgets/interactive.py",
 	"src/kfactory/technology",
 	"src/kfactory/pdk.py",
 ]
-plugins = "pydantic.mypy"
+plugins = "pydantic.mypy, numpy.typing.mypy_plugin"
 
 [tool.pylsp-mypy]
 enabled = true
 live_mode = true
 strict = true
 
 [[tool.mypy.overrides]]
@@ -194,16 +194,16 @@
 
 [tool.towncrier]
 directory = "changelog.d"
 filename = "CHANGELOG.md"
 start_string = "<!-- towncrier release notes start -->\n"
 underlines = ["", "", ""]
 template = "changelog.d/changelog_template.jinja"
-title_format = "## [{version}](https://github.com/gdsfactory/klive/tree/{version}) - {project_date}"
-issue_format = "[#{issue}](https://github.com/gdsfactory/klive/issues/{issue})"
+title_format = "## [{version}](https://github.com/gdsfactory/kfactory/tree/{version}) - {project_date}"
+issue_format = "[#{issue}](https://github.com/gdsfactory/kfactory/issues/{issue})"
 
 [[tool.towncrier.type]]
 directory = "security"
 name = "Security"
 showcontent = true
 
 [[tool.towncrier.type]]
@@ -233,15 +233,15 @@
 
 
 [tool.tbump]
 # Uncomment this if your project is hosted on GitHub:
 # github_url = "https://github.com/<user or organization>/<project>/"
 
 [tool.tbump.version]
-current = "0.7.4"
+current = "0.7.5"
 
 # Example of a semver regexp.
 # Make sure this matches current_version before
 # using tbump
 regex = '''
   (?P<major>\d+)
   \.
```

### Comparing `kfactory-0.7.4/src/kfactory/__init__.py` & `kfactory-0.7.5/src/kfactory/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,20 +16,22 @@
     Ports,
     cell,
     kcl,
     KCLayout,
     default_save,
     LayerEnum,
     show,
+    polygon_from_array,
+    dpolygon_from_array,
 )
 from . import cells, placer, routing, utils, port, pdk
 from .conf import config
 from .pdk import Pdk
 
-__version__ = "0.7.4"
+__version__ = "0.7.5"
 
 logger = config.logger
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
@@ -46,8 +48,10 @@
     "routing",
     "utils",
     "show",
     "config",
     "LayerEnum",
     "logger",
     "pdk",
+    "polygon_from_array",
+    "dpolygon_from_array",
 ]
```

### Comparing `kfactory-0.7.4/src/kfactory/cells/bezier.py` & `kfactory-0.7.5/src/kfactory/cells/bezier.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/cells/circular.py` & `kfactory-0.7.5/src/kfactory/cells/circular.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/cells/dbu/taper.py` & `kfactory-0.7.5/src/kfactory/cells/dbu/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/cells/dbu/waveguide.py` & `kfactory-0.7.5/src/kfactory/cells/dbu/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/cells/euler.py` & `kfactory-0.7.5/src/kfactory/cells/euler.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/cells/taper.py` & `kfactory-0.7.5/src/kfactory/cells/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/cells/waveguide.py` & `kfactory-0.7.5/src/kfactory/cells/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/conf.py` & `kfactory-0.7.5/src/kfactory/conf.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/kcell.py` & `kfactory-0.7.5/src/kfactory/kcell.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,43 +10,30 @@
 
 import functools
 import importlib
 import importlib.util
 import json
 import socket
 from collections.abc import Callable, Hashable, Iterable, Iterator
-
-# from enum import IntEnum
 from enum import Enum, IntEnum
 from hashlib import sha3_512
 from inspect import Parameter, signature
 from pathlib import Path
 from tempfile import gettempdir
-from typing import (  # ParamSpec, # >= python 3.10
-    TYPE_CHECKING,
-    Any,
-    Literal,
-    TypeVar,
-    cast,
-    overload,
-)
+from typing import TYPE_CHECKING, Any, Literal, TypeVar, cast, overload
 
-# from cachetools import Cache, cached
 import cachetools.func
 import numpy as np
 import ruamel.yaml
 from typing_extensions import ParamSpec
 
 from . import kdb
 from .conf import config
 from .port import rename_clockwise
 
-# import struct
-# from abc import abstractmethod
-
 if TYPE_CHECKING:
     from .pdk import Pdk
 
 
 KCellParams = ParamSpec("KCellParams")
 
 AnyTrans = TypeVar(
@@ -189,15 +176,16 @@
     instead of only the `klayout.db.Cell` objects.
     Additionally it allows creation and registration through `create_cell`
 
     All attributes of `klayout.db.Layout` are transparently accessible
 
     Attributes:
         editable: Whether the layout should be opened in editable mode (default: True)
-        rename_function: function that takes an iterable object of ports and renames them
+        rename_function: function that takes an iterable object of ports and renames
+            them
     """
 
     def __init__(self, editable: bool = True, pdk: "Pdk | None" = None) -> None:
         """Create a library of cells.
 
         Args:
             editable: Open the KLayout Layout in editable mode if `True`.
@@ -1006,15 +994,15 @@
             port: The port to add.
             name: Overwrite the name of the port
             keep_mirror: Keep the mirror part of the transformation of a port if
                 `True`, else set the mirror flag to `False`.
         """
         if self._locked:
             raise LockedError(self)
-        self.ports.add_port(port=port, name=name)
+        self.ports.add_port(port=port, name=name, keep_mirror=keep_mirror)
 
     def add_ports(
         self, ports: Iterable[Port], prefix: str = "", keep_mirror: bool = False
     ) -> None:
         """Add a sequence of ports to the cells.
 
         Can be useful to add all ports of a instance for example.
@@ -1629,26 +1617,51 @@
         | kdb.DCplxTrans,
         trans: kdb.Trans | kdb.DTrans | kdb.ICplxTrans | kdb.DCplxTrans | None = None,
         /,
         *,
         no_warn: bool = False,
     ) -> "Instance | None":
         """Transforms the instance or cell with the transformation given."""
+        config.logger.warning(
+            "You are transforming the KCell {}. It is highly discouraged to do this."
+            " You probably want to transform an instance instead.",
+            self.name,
+        )
         if self._locked:
             raise LockedError(self)
         if trans:
             return Instance(
                 self.kcl,
                 self._kdb_cell.transform(
                     inst_or_trans, trans  # type: ignore[arg-type]
                 ),
             )
         else:
             return self._kdb_cell.transform(inst_or_trans)  # type:ignore[arg-type]
 
+    @property
+    def xmin(self) -> int:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self._kdb_cell.bbox().left
+
+    @property
+    def ymin(self) -> int:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self._kdb_cell.bbox().bottom
+
+    @property
+    def xmax(self) -> int:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self._kdb_cell.bbox().right
+
+    @property
+    def ymax(self) -> int:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self._kdb_cell.bbox().top
+
 
 class Instance:
     """An Instance of a KCell.
 
     An Instance is a reference to a KCell with a transformation.
 
     Attributes:
@@ -1992,14 +2005,62 @@
     def __repr__(self) -> str:
         """Return a string representation of the instance."""
         port_names = [p.name for p in self.ports]
         return (
             f"{self.parent_cell.name}: ports {port_names}, {self.kcl[self.cell_index]}"
         )
 
+    def mirror_x(self, x: int = 0) -> None:
+        """Mirror the instance at an x-axis."""
+        self.transform(kdb.Trans(2, True, 2 * x, 0))
+
+    def mirror_y(self, y: int = 0) -> None:
+        """Mirror the instance at an y-axis."""
+        self.transform(kdb.Trans(0, True, 0, 2 * y))
+
+    @property
+    def xmin(self) -> int:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self._instance.bbox().left
+
+    @xmin.setter
+    def xmin(self, __val: int) -> None:
+        """Moves the instance so that the bbox's left x-coordinate."""
+        self.transform(kdb.Trans(__val - self.bbox().left, 0))
+
+    @property
+    def ymin(self) -> int:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self._instance.bbox().bottom
+
+    @ymin.setter
+    def ymin(self, __val: int) -> None:
+        """Moves the instance so that the bbox's left x-coordinate."""
+        self.transform(kdb.Trans(0, __val - self._instance.bbox().bottom))
+
+    @property
+    def xmax(self) -> int:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self._instance.bbox().right
+
+    @xmax.setter
+    def xmax(self, __val: int) -> None:
+        """Moves the instance so that the bbox's left x-coordinate."""
+        self.transform(kdb.Trans(__val - self.bbox().right, 0))
+
+    @property
+    def ymax(self) -> int:
+        """Returns the x-coordinate of the left edge of the bounding box."""
+        return self._instance.bbox().top
+
+    @ymax.setter
+    def ymax(self, __val: int) -> None:
+        """Moves the instance so that the bbox's left x-coordinate."""
+        self.transform(kdb.Trans(0, __val - self._instance.bbox().top))
+
 
 class UMInstance:
     """Make the port able to dynamically give um based info."""
 
     def __init__(self, parent: Instance):
         """Constructor, just needs a pointer to the port.
 
@@ -2078,14 +2139,22 @@
         else:
             self.parent.transform(
                 kdb.DTrans(
                     float(destination[0] - origin[0]), float(destination[1] - origin[1])
                 )
             )
 
+    def mirror_x(self, x: float = 0) -> None:
+        """Mirror the instance at an x-axis."""
+        self.parent.transform(kdb.DTrans(2, True, 2 * x, 0))
+
+    def mirror_y(self, y: float = 0) -> None:
+        """Mirror the instance at an y-axis."""
+        self.parent.transform(kdb.DTrans(0, True, 0, 2 * y))
+
 
 class Instances:
     """Holder for instances.
 
     Allows retrieval by name or index
     """
 
@@ -2170,29 +2239,29 @@
             name: Overwrite the name of the port
             keep_mirror: Keep the mirror flag from the original port if `True`,
                 else set [Port.trans.mirror][kfactory.kcell.Port.trans] (or the complex
                 equivalent) to `False`.
         """
         _port = port.copy()
         if not keep_mirror:
-            if port._trans:
-                port._trans.mirror = False
-            elif port._dcplx_trans:
-                port._dcplx_trans.mirror = False
+            if _port._trans:
+                _port._trans.mirror = False
+            elif _port._dcplx_trans:
+                _port._dcplx_trans.mirror = False
         if name is not None:
             _port.name = name
         self._ports.append(_port)
 
     def add_ports(
         self, ports: Iterable[Port], prefix: str = "", keep_mirror: bool = False
     ) -> None:
         """Append a list of ports."""
         for p in ports:
             name = p.name or ""
-            self.add_port(port=p, name=prefix + name)
+            self.add_port(port=p, name=prefix + name, keep_mirror=keep_mirror)
 
     @overload
     def create_port(
         self,
         *,
         trans: kdb.Trans,
         width: int,
@@ -2780,14 +2849,30 @@
         finally:
             conn.close()
 
     if delete:
         Path(gds_file).unlink()
 
 
+def polygon_from_array(array: Iterable[tuple[int, int]]) -> kdb.Polygon:
+    """Create a DPolygon from a 2D array-like structure. (dbu version).
+
+    Array-like: `[[x1,y1],[x2,y2],...]`
+    """
+    return kdb.Polygon([kdb.Point(int(x), int(y)) for (x, y) in array])
+
+
+def dpolygon_from_array(array: Iterable[tuple[float, float]]) -> kdb.DPolygon:
+    """Create a DPolygon from a 2D array-like structure. (um version).
+
+    Array-like: `[[x1,y1],[x2,y2],...]`
+    """
+    return kdb.DPolygon([kdb.DPoint(int(x), int(y)) for (x, y) in array])
+
+
 __all__ = [
     "KCell",
     "Instance",
     "Port",
     "Ports",
     "autocell",
     "cell",
```

### Comparing `kfactory-0.7.4/src/kfactory/pdk.py` & `kfactory-0.7.5/src/kfactory/pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/placer.py` & `kfactory-0.7.5/src/kfactory/placer.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/port.py` & `kfactory-0.7.5/src/kfactory/port.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/routing/electrical.py` & `kfactory-0.7.5/src/kfactory/routing/electrical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/routing/manhattan.py` & `kfactory-0.7.5/src/kfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/routing/optical.py` & `kfactory-0.7.5/src/kfactory/routing/optical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/technology/klayout_tech.py` & `kfactory-0.7.5/src/kfactory/technology/klayout_tech.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/technology/layer_map.py` & `kfactory-0.7.5/src/kfactory/technology/layer_map.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/technology/layer_stack.py` & `kfactory-0.7.5/src/kfactory/technology/layer_stack.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/technology/layer_views.py` & `kfactory-0.7.5/src/kfactory/technology/layer_views.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/technology/xml_utils.py` & `kfactory-0.7.5/src/kfactory/technology/xml_utils.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/technology/yaml_utils.py` & `kfactory-0.7.5/src/kfactory/technology/yaml_utils.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/typings.py` & `kfactory-0.7.5/src/kfactory/typings.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/utils/__init__.py` & `kfactory-0.7.5/src/kfactory/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/utils/enclosure.py` & `kfactory-0.7.5/src/kfactory/utils/enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/utils/fill.py` & `kfactory-0.7.5/src/kfactory/utils/fill.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/utils/simplify.py` & `kfactory-0.7.5/src/kfactory/utils/simplify.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/utils/violations.py` & `kfactory-0.7.5/src/kfactory/utils/violations.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory/widgets/interactive.py` & `kfactory-0.7.5/src/kfactory/widgets/interactive.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/src/kfactory.egg-info/PKG-INFO` & `kfactory-0.7.5/src/kfactory.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.7.4
+Version: 0.7.5
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: git
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.7.4
+# KFactory 0.7.5
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 | :exclamation:  KFactory is still experimental, expect API changes without notice (even though we try to keep it to a minimum!)   |
 |---------------------------------------------------------------------------------------------------------------------------------|
 
-It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.4` for example.
+It is suggest to pin the version of KFactory in `requirements.txt` or `pyproject.toml` with `kfactory==0.7.5` for example.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
 - [x] Basic cells like euler/circular bends, taper, waveguide
 - [x] Path extrusion (no interface with CrossSections)
```

### Comparing `kfactory-0.7.4/src/kfactory.egg-info/SOURCES.txt` & `kfactory-0.7.5/src/kfactory.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 .github/workflows/test_code.yml
 changelog.d/changelog_template.jinja
 docs/mkdocs.yml
 docs/overrides/main.html
 docs/source/changelog.md
 docs/source/complex_cell.py
 docs/source/config.md
+docs/source/gdsfactory.md
 docs/source/gen_ref_pages.py
 docs/source/index.md
 docs/source/intro.md
 docs/source/layers.py
 docs/source/pre.md
 docs/source/star.py
 docs/source/waveguide.py
```

### Comparing `kfactory-0.7.4/src/kfactory.egg-info/requires.txt` & `kfactory-0.7.5/src/kfactory.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/tests/conftest.py` & `kfactory-0.7.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/tests/test_cells.py` & `kfactory-0.7.5/tests/test_cells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/tests/test_cplxcells.py` & `kfactory-0.7.5/tests/test_cplxcells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/tests/test_enclosure.py` & `kfactory-0.7.5/tests/test_enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/tests/test_extrude.py` & `kfactory-0.7.5/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/tests/test_pdk.py` & `kfactory-0.7.5/tests/test_pdk.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/tests/test_ports.py` & `kfactory-0.7.5/tests/test_ports.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,7 +96,45 @@
     c = kf.KCell()
 
     wg1 = c << wg
     wg2 = c << wg
     wg2.connect("o1", wg1, "o1")
 
     assert wg2.ports["o1"].trans == kf.kdb.Trans(0, False, 0, 0)
+
+
+def test_keep_mirror(LAYER):
+    c = kf.KCell()
+
+    p1 = kf.Port(trans=kf.kdb.Trans.M90, width=1000, layer=LAYER.WG)
+
+    c.add_port(p1, name="o1")
+    c.add_port(p1, name="o2", keep_mirror=True)
+
+    assert c["o1"].trans.is_mirror() is False
+    assert c["o2"].trans.is_mirror() is True
+
+
+def test_addports_keep_mirror(LAYER):
+    c = kf.KCell()
+
+    ports = [
+        kf.Port(
+            name=f"{i}",
+            width=1000,
+            layer=LAYER.WG,
+            trans=kf.kdb.Trans(i, True, 0, 0),
+        )
+        for i in range(4)
+    ]
+
+    c.add_ports(ports, prefix="mirr_", keep_mirror=True)
+    c.add_ports(ports, prefix="nomirr_", keep_mirror=False)
+
+    for i in range(4):
+        t1 = c[f"mirr_{i}"].trans
+        t2 = c[f"nomirr_{i}"].trans
+
+        t2_mirr = t2.dup()
+        t2_mirr.mirror = not t2_mirr.is_mirror()
+
+        assert t1 == t2_mirr
```

### Comparing `kfactory-0.7.4/tests/test_rename.py` & `kfactory-0.7.5/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/tests/test_routing.py` & `kfactory-0.7.5/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.7.4/tests/test_spiral.py` & `kfactory-0.7.5/tests/test_spiral.py`

 * *Files identical despite different names*

