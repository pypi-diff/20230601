# Comparing `tmp/circuitpython-display_ht16k33-0.4.0.tar.gz` & `tmp/circuitpython-display_ht16k33-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitpython-display_ht16k33-0.4.0.tar", last modified: Wed May 31 19:32:33 2023, max compression
+gzip compressed data, was "circuitpython-display_ht16k33-0.4.1.tar", last modified: Wed May 31 23:35:04 2023, max compression
```

## Comparing `circuitpython-display_ht16k33-0.4.0.tar` & `circuitpython-display_ht16k33-0.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.560212 circuitpython-display_ht16k33-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.544212 circuitpython-display_ht16k33-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.552212 circuitpython-display_ht16k33-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-31 19:32:33.560212 circuitpython-display_ht16k33-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.552212 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-31 19:32:33.000000 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-31 19:32:33.000000 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:32:33.000000 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 19:32:33.000000 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 19:32:33.000000 circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.552212 circuitpython-display_ht16k33-0.4.0/display_ht16k33/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/display_ht16k33/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/display_ht16k33/ht16k33.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/display_ht16k33/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)    30175 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/display_ht16k33/segments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.556212 circuitpython-display_ht16k33-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)  1981287 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/7mwahe.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.560212 circuitpython-display_ht16k33-0.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/Logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/Logo.png.license
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/extra_css.css
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/extra_css.css.license
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/font5x8.bin
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)    48491 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/docs/segments.jpg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:32:33.560212 circuitpython-display_ht16k33-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_advanced_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_14x4.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_count_down.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_custom_chars.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_marquee.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-31 19:32:25.000000 circuitpython-display_ht16k33-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 19:32:15.000000 circuitpython-display_ht16k33-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:32:33.560212 circuitpython-display_ht16k33-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.720842 circuitpython-display_ht16k33-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.708842 circuitpython-display_ht16k33-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.712842 circuitpython-display_ht16k33-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13033 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-31 23:35:04.720842 circuitpython-display_ht16k33-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.712842 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-31 23:35:04.000000 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-31 23:35:04.000000 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 23:35:04.000000 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-31 23:35:04.000000 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 23:35:04.000000 circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.716842 circuitpython-display_ht16k33-0.4.1/display_ht16k33/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/display_ht16k33/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7432 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/display_ht16k33/ht16k33.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/display_ht16k33/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30459 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/display_ht16k33/segments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.716842 circuitpython-display_ht16k33-0.4.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)  1981287 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/7mwahe.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.720842 circuitpython-display_ht16k33-0.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/Logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/Logo.png.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/extra_css.css
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/extra_css.css.license
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6962 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/font5x8.bin
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    48491 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/docs/segments.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 23:35:04.720842 circuitpython-display_ht16k33-0.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_advanced_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_14x4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_count_down.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_custom_chars.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_marquee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-31 23:34:56.000000 circuitpython-display_ht16k33-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-31 23:34:45.000000 circuitpython-display_ht16k33-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 23:35:04.720842 circuitpython-display_ht16k33-0.4.1/setup.cfg
```

### Comparing `circuitpython-display_ht16k33-0.4.0/.github/workflows/build.yml` & `circuitpython-display_ht16k33-0.4.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/.github/workflows/release_gh.yml` & `circuitpython-display_ht16k33-0.4.1/.github/workflows/release_gh.yml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/.gitignore` & `circuitpython-display_ht16k33-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/.pre-commit-config.yaml` & `circuitpython-display_ht16k33-0.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/.pylintrc` & `circuitpython-display_ht16k33-0.4.1/.pylintrc`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/LICENSE` & `circuitpython-display_ht16k33-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/PKG-INFO` & `circuitpython-display_ht16k33-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-display_ht16k33
-Version: 0.4.0
+Version: 0.4.1
 Summary: On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 Author-email: JDM <xxxy@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33
 Keywords: sensor,blinka,circuitpython,micropython,display_ht16k33,ht16k33,displayio,matrix,8x8,16x8,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-display_ht16k33-0.4.0/README.rst` & `circuitpython-display_ht16k33-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/PKG-INFO` & `circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitpython-display-ht16k33
-Version: 0.4.0
+Version: 0.4.1
 Summary: On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices.
 Author-email: JDM <xxxy@mozmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33
 Keywords: sensor,blinka,circuitpython,micropython,display_ht16k33,ht16k33,displayio,matrix,8x8,16x8,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `circuitpython-display_ht16k33-0.4.0/circuitpython_display_ht16k33.egg-info/SOURCES.txt` & `circuitpython-display_ht16k33-0.4.1/circuitpython_display_ht16k33.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/display_ht16k33/segments.py` & `circuitpython-display_ht16k33-0.4.1/display_ht16k33/segments.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import displayio
 
 try:
     from typing import Optional, Dict, Tuple, Union
 except ImportError:
     pass
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 __repo__ = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33.git"
 
 
 # fmt: off
 CHARS = (
     0b00000000, 0b00000000,  #
     0b01000000, 0b00000110,  # !
@@ -387,14 +387,18 @@
             self._number(value)
             return
         if isinstance(value, int):
             value = str(value)
         if ":" in value:
             value = value.replace(":", "")
             self._two_points(True)
+        if "." in value:
+
+            self._number(value)
+            return
 
         value_string = str(value)
         for i in range(len(value_string)):
             self.print_digit(i, value_string[len(value_string) - 1 - i])
 
     def print_digit(self, pos: int, char: str) -> None:
         """
@@ -448,14 +452,15 @@
     def clear(self) -> None:
         """
         Clear the digits
         """
         for i in range(4):
             self.print_digit(i, "*")
         self._two_points(False)
+        self.points = False
 
     def __setitem__(self, key: int, value: str) -> None:
         self.print_digit(key, value)
 
     def _two_points(self, show: bool = True):
         if show:
             for i in range(2):
@@ -520,22 +525,24 @@
 
         if loop:
             while True:
                 cycle(text, delay)
         else:
             cycle(text, delay)
 
-    def _number(self, number: float) -> None:
+    def _number(self, number: Union[float, str]) -> None:
         stnum = str(number)
-        dot = stnum.find(".") - 1
-        print(dot)
+        if stnum.count(".") > 1:
+            raise RuntimeError("String with more than two periods are not implemented")
+        dot = stnum.find(".")
         stnum = stnum.replace(".", "")
 
+        for i in range(len(stnum)):
+            self.print_digit(i, stnum[len(stnum) - 1 - i])
         self._period_container[dot].color_index = 2
-        self.print(stnum)
 
 
 class SEG14x4:
     """
     Main class to display the 14x4 segments on the screen
 
     :param int x: x coordinates in pixels for the segment to start. This is the top left
```

### Comparing `circuitpython-display_ht16k33-0.4.0/docs/7mwahe.gif` & `circuitpython-display_ht16k33-0.4.1/docs/7mwahe.gif`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/docs/_static/Logo.png` & `circuitpython-display_ht16k33-0.4.1/docs/_static/Logo.png`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/docs/_static/favicon.ico` & `circuitpython-display_ht16k33-0.4.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/docs/conf.py` & `circuitpython-display_ht16k33-0.4.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/docs/examples.rst` & `circuitpython-display_ht16k33-0.4.1/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/docs/font5x8.bin` & `circuitpython-display_ht16k33-0.4.1/docs/font5x8.bin`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/docs/segments.jpg` & `circuitpython-display_ht16k33-0.4.1/docs/segments.jpg`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_advanced_example.py` & `circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_advanced_example.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_segments_custom_chars.py` & `circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_segments_custom_chars.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_simpletest.py` & `circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_simpletest.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/examples/display_ht16k33_text.py` & `circuitpython-display_ht16k33-0.4.1/examples/display_ht16k33_text.py`

 * *Files identical despite different names*

### Comparing `circuitpython-display_ht16k33-0.4.0/pyproject.toml` & `circuitpython-display_ht16k33-0.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "circuitpython-display_ht16k33"
 description = "On Display Simulation for an HT16K33 driver. Works with 16x8 and 8x8 matrices."
-version = "0.4.0"
+version = "0.4.1"
 readme = "README.rst"
 authors = [
     {name = "JDM", email = "xxxy@mozmail.com"}
 ]
 urls = {Homepage = "https://github.com/jposada202020/CircuitPython_DISPLAY_HT16K33"}
 keywords = [
     "sensor",
```

