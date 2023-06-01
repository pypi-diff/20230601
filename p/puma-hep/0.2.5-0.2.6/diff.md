# Comparing `tmp/puma-hep-0.2.5.tar.gz` & `tmp/puma-hep-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "puma-hep-0.2.5.tar", last modified: Fri May 12 15:12:42 2023, max compression
+gzip compressed data, was "puma-hep-0.2.6.tar", last modified: Thu Jun  1 08:56:53 2023, max compression
```

## Comparing `puma-hep-0.2.5.tar` & `puma-hep-0.2.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.061276 puma-hep-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-05-12 15:12:32.000000 puma-hep-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:12:32.000000 puma-hep-0.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-12 15:12:42.061276 puma-hep-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-12 15:12:32.000000 puma-hep-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.053275 puma-hep-0.2.5/puma/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/fraction_scan.py
--rw-r--r--   0 runner    (1001) docker     (123)    22871 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/histogram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.053275 puma-hep-0.2.5/puma/hlplots/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/hlplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16037 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/hlplots/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/hlplots/tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/line_plot_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/pie.py
--rw-r--r--   0 runner    (1001) docker     (123)    28069 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20420 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/roc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.057276 puma-hep-0.2.5/puma/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.057276 puma-hep-0.2.5/puma/tests/hlplots/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/hlplots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/hlplots/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/hlplots/test_tagger.py
--rw-r--r--   0 runner    (1001) docker     (123)    27352 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_line_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_pie_chart.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_plot_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18908 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_roc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_var_vs_eff.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/test_var_vs_var.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.057276 puma-hep-0.2.5/puma/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/test_discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/test_histogram_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/tests/utils/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.057276 puma-hep-0.2.5/puma/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/utils/discriminant.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/utils/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/utils/histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/var_vs_eff.py
--rw-r--r--   0 runner    (1001) docker     (123)    13877 2023-05-12 15:12:32.000000 puma-hep-0.2.5/puma/var_vs_var.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 15:12:42.061276 puma-hep-0.2.5/puma_hep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-05-12 15:12:42.000000 puma-hep-0.2.5/puma_hep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-12 15:12:42.000000 puma-hep-0.2.5/puma_hep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:12:42.000000 puma-hep-0.2.5/puma_hep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 15:12:41.000000 puma-hep-0.2.5/puma_hep.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 15:12:42.000000 puma-hep-0.2.5/puma_hep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-12 15:12:42.000000 puma-hep-0.2.5/puma_hep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-12 15:12:32.000000 puma-hep-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-12 15:12:42.061276 puma-hep-0.2.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-05-12 15:12:32.000000 puma-hep-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.839696 puma-hep-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11345 2023-06-01 08:56:43.000000 puma-hep-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:56:43.000000 puma-hep-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-01 08:56:53.839696 puma-hep-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-01 08:56:43.000000 puma-hep-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.835696 puma-hep-0.2.6/puma/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/fraction_scan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22871 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/histogram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.835696 puma-hep-0.2.6/puma/hlplots/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/hlplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/hlplots/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/hlplots/tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8028 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/line_plot_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27613 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20394 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/roc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.835696 puma-hep-0.2.6/puma/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.835696 puma-hep-0.2.6/puma/tests/hlplots/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/hlplots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/hlplots/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/hlplots/test_tagger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27274 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_line_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7230 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_pie_chart.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_plot_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18908 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_roc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14968 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_var_vs_eff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/test_var_vs_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.835696 puma-hep-0.2.6/puma/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/test_discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11373 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/test_histogram_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/tests/utils/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.839696 puma-hep-0.2.6/puma/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4667 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/utils/discriminant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/utils/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/utils/histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15827 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/var_vs_eff.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13851 2023-06-01 08:56:43.000000 puma-hep-0.2.6/puma/var_vs_var.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:56:53.839696 puma-hep-0.2.6/puma_hep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 08:56:53.000000 puma-hep-0.2.6/puma_hep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-01 08:56:43.000000 puma-hep-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-01 08:56:53.839696 puma-hep-0.2.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      435 2023-06-01 08:56:43.000000 puma-hep-0.2.6/setup.py
```

### Comparing `puma-hep-0.2.5/LICENSE` & `puma-hep-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/PKG-INFO` & `puma-hep-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puma-hep
-Version: 0.2.5
+Version: 0.2.6
 Summary: Plotting API for HEP flavour tagging plots.
 Home-page: https://github.com/umami-hep/puma
 Keywords: machine learning,flavour tagging,plots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `puma-hep-0.2.5/README.md` & `puma-hep-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/histogram.py` & `puma-hep-0.2.6/puma/histogram.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/hlplots/results.py` & `puma-hep-0.2.6/puma/hlplots/results.py`

 * *Files 11% similar despite different names*

```diff
@@ -125,15 +125,15 @@
         if not isinstance(cuts, Cuts):
             cuts = Cuts.empty() if cuts is None else Cuts.from_list(cuts)
         var_list = sum([tagger.variables for tagger in taggers], [label_var])
         var_list += cuts.variables
         var_list = list(set(var_list + [self.perf_var]))
 
         # load data
-        reader = H5Reader(file_path)
+        reader = H5Reader(file_path, precision="full")
         data = reader.load({key: var_list}, num_jets)[key]
 
         # apply cuts
         idx, data = cuts(data)
         if perf_var is not None:
             perf_var = perf_var[idx]
 
@@ -180,74 +180,172 @@
             output name
         """
         base = f"{self.sample}_{self.signal}_{plot_name}"
         if suffix is not None:
             base += f"_{suffix}"
         return Path(self.output_dir / base).with_suffix(f".{self.extension}")
 
+    def plot_probs(
+        self,
+        suffix: str = None,
+        **kwargs,
+    ):
+        """Plot probability distributions.
+
+        Parameters
+        ----------
+        suffix : str, optional
+            Suffix to add to output file name, by default None
+        **kwargs : kwargs
+            key word arguments for `puma.HistogramPlot`
+        """
+        line_styles = get_good_linestyles()
+        flavours = self.backgrounds + [self.signal]
+
+        # group by output probability
+        for flav_prob in flavours:
+            histo = HistogramPlot(
+                n_ratio_panels=1,
+                xlabel=flav_prob.px,
+                ylabel="Normalised number of jets",
+                figsize=(7.0, 4.5),
+                atlas_first_tag=self.atlas_first_tag,
+                atlas_second_tag=self.atlas_second_tag,
+                **kwargs,
+            )
+
+            tagger_labels = []
+            for i, tagger in enumerate(self.taggers.values()):
+                tagger_labels.append(tagger.label if tagger.label else tagger.name)
+                for flav_class in flavours:
+                    histo.add(
+                        Histogram(
+                            tagger.probs(flav_prob, flav_class),
+                            ratio_group=flav_class,
+                            label=flav_class.label if i == 0 else None,
+                            colour=flav_class.colour,
+                            linestyle=line_styles[i],
+                        ),
+                        reference=tagger.reference,
+                    )
+
+            histo.draw()
+            histo.make_linestyle_legend(
+                linestyles=line_styles,
+                labels=tagger_labels,
+                bbox_to_anchor=(0.55, 1),
+            )
+            histo.savefig(self.get_filename(f"probs_{flav_prob.px}", suffix))
+
+        # group by flavour
+        for flav_class in flavours:
+            histo = HistogramPlot(
+                n_ratio_panels=1,
+                xlabel=flav_class.label,
+                ylabel="Normalised number of jets",
+                figsize=(7.0, 4.5),
+                atlas_first_tag=self.atlas_first_tag,
+                atlas_second_tag=self.atlas_second_tag,
+                **kwargs,
+            )
+
+            tagger_labels = []
+            for i, tagger in enumerate(self.taggers.values()):
+                tagger_labels.append(tagger.label if tagger.label else tagger.name)
+                for flav_prob in flavours:
+                    histo.add(
+                        Histogram(
+                            tagger.probs(flav_prob, flav_class),
+                            ratio_group=flav_prob,
+                            label=flav_prob.px if i == 0 else None,
+                            colour=flav_prob.colour,
+                            linestyle=line_styles[i],
+                        ),
+                        reference=tagger.reference,
+                    )
+
+            histo.draw()
+            histo.make_linestyle_legend(
+                linestyles=line_styles,
+                labels=tagger_labels,
+                bbox_to_anchor=(0.55, 1),
+            )
+            histo.savefig(self.get_filename(f"probs_{flav_class}", suffix))
+
     def plot_discs(
         self,
         suffix: str = None,
         exclude_tagger: list = None,
         xlabel: str = None,
+        wp_vlines: list = None,
         **kwargs,
     ):
         """Plot discriminant distributions.
 
         Parameters
         ----------
         suffix : str, optional
             Suffix to add to output file name, by default None
         exclude_tagger : list, optional
             List of taggers to be excluded from this plot, by default None
         xlabel : str, optional
             x-axis label, by default "$D_{b}$"
+        wp_vlines : list, optional
+            List of WPs to draw vertical lines at, by default None
         **kwargs : kwargs
             key word arguments for `puma.HistogramPlot`
         """
         if xlabel is None:
             xlabel = rf"$D_{{{self.signal.name.rstrip('jets')}}}$"
+        if wp_vlines is None:
+            wp_vlines = []
 
         line_styles = get_good_linestyles()
 
-        tagger_output_plot = HistogramPlot(
+        histo = HistogramPlot(
             n_ratio_panels=0,
             xlabel=xlabel,
             ylabel="Normalised number of jets",
             figsize=(7.0, 4.5),
             atlas_first_tag=self.atlas_first_tag,
             atlas_second_tag=self.atlas_second_tag,
             **kwargs,
         )
-        tag_i = 0
-        tag_labels = []
-        for tagger in self.taggers.values():
+
+        tagger_labels = []
+        for i, tagger in enumerate(self.taggers.values()):
             if exclude_tagger is not None and tagger.name in exclude_tagger:
                 continue
             discs = tagger.discriminant(self.signal)
+
+            # get working point
+            for wp in wp_vlines:
+                cut = np.percentile(discs[tagger.is_flav(self.signal)], 100 - wp)
+                label = None if i > 0 else f"{wp}%"
+                histo.draw_vlines([cut], labels=[label], linestyle=line_styles[i])
+
             for flav in self.flavours:
-                tagger_output_plot.add(
+                histo.add(
                     Histogram(
                         discs[tagger.is_flav(flav)],
                         ratio_group=flav,
-                        label=flav.label if tag_i == 0 else None,
+                        label=flav.label if i == 0 else None,
                         colour=flav.colour,
-                        linestyle=line_styles[tag_i],
+                        linestyle=line_styles[i],
                     ),
                     reference=tagger.reference,
                 )
-            tag_i += 1
-            tag_labels.append(tagger.label if tagger.label else tagger.name)
-        tagger_output_plot.draw()
-        tagger_output_plot.make_linestyle_legend(
-            linestyles=line_styles[:tag_i],
-            labels=tag_labels,
+            tagger_labels.append(tagger.label if tagger.label else tagger.name)
+        histo.draw()
+        histo.make_linestyle_legend(
+            linestyles=line_styles,
+            labels=tagger_labels,
             bbox_to_anchor=(0.55, 1),
         )
-        tagger_output_plot.savefig(self.get_filename("disc", suffix))
+        histo.savefig(self.get_filename("disc", suffix))
 
     def plot_rocs(
         self,
         suffix: str = None,
         args_roc_plot: dict = None,
     ):
         """Plots rocs.
```

### Comparing `puma-hep-0.2.5/puma/hlplots/tagger.py` & `puma-hep-0.2.6/puma/hlplots/tagger.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,14 +154,33 @@
         -------
         int
             Number of jets of given flavour
         """
         flavour = Flavours[flavour] if isinstance(flavour, str) else flavour
         return len(flavour.cuts(self.labels).values)
 
+    def probs(self, prob_flavour: Flavour, label_flavour: Flavour = None):
+        """Retrieve probabilities for a given flavour.
+
+        Parameters
+        ----------
+        prob_flavour : Flavour
+            Return probabilities for this flavour class
+        label_flavour : Flavour, optional
+            Only return jets of the given truth flavour, by default None
+
+        Returns
+        -------
+        np.ndarray
+            Probabilities for given flavour
+        """
+        return self.scores[self.is_flav(label_flavour)][
+            f"{self.name}_{prob_flavour.px}"
+        ]
+
     def discriminant(self, signal: Flavour, fx: float = None):
         """Retrieve the discriminant for a given signal class.
 
         Parameters
         ----------
         signal : Flavour
             Signal class for which the discriminant should be retrieved
```

### Comparing `puma-hep-0.2.5/puma/line_plot_2d.py` & `puma-hep-0.2.6/puma/line_plot_2d.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/metrics.py` & `puma-hep-0.2.6/puma/metrics.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/pie.py` & `puma-hep-0.2.6/puma/pie.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/plot_base.py` & `puma-hep-0.2.6/puma/plot_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -341,74 +341,69 @@
         if self.grid:
             self.axis_top.grid(lw=0.3)
             for ratio_axis in self.ratio_axes:
                 ratio_axis.grid(lw=0.3)
 
     def draw_vlines(
         self,
-        vlines_xvalues: list,
-        vlines_label_list: list = None,
-        vlines_line_height_list: list = None,
+        xs: list,
+        labels: list = None,
+        ys: list = None,
         same_height: bool = False,
         colour: str = "#000000",
+        linestyle: str = "dashed",
         fontsize: int = 10,
     ):
         """Drawing working points in plot.
 
         Parameters
         ----------
-        vlines_xvalues : list
+        xs : list
             List of working points x values to draw
-        vlines_label_list : list, optional
+        labels : list, optional
             List with labels for the vertical lines. Must be the same
-            order as the vlines_xvalues. If None, the xvalues * 100 will be
+            order as the xs. If None, the xvalues * 100 will be
             used as labels. By default None
-        vlines_line_height_list : list, optional
+        ys : list, optional
             List with the y height of the vertical lines in percent of the
             upper plot (0 is bottom, 1 is top). Must be the same
-            order as the vlines_xvalues and the labels. By default None
+            order as the xs and the labels. By default None
         same_height : bool, optional
             Working point lines on same height, by default False
         colour : str, optional
             Colour of the vertical line, by default "#000000" (black)
+        linestyle : str, optional
+            Linestyle of the vertical line, by default "dashed"
         fontsize : int, optional
             Fontsize of the vertical line text. By default 10.
         """
-        for vline_counter, vline in enumerate(vlines_xvalues):
+        for i, vline_x in enumerate(xs):
             # Set y-point of the WP lines/text
-            if vlines_line_height_list is None:
-                ytext = 0.65 if same_height else 0.65 - vline_counter * 0.07
-
-            else:
-                ytext = vlines_line_height_list[vline_counter]
+            ytext = (0.65 if same_height else 0.65 - i * 0.07) if ys is None else ys[i]
 
             self.axis_top.axvline(
-                x=vline,
+                x=vline_x,
                 ymax=ytext,
                 color=colour,
-                linestyle="dashed",
+                linestyle=linestyle,
                 linewidth=1.0,
             )
 
             # Set the number above the line
             self.axis_top.text(
-                x=vline - 0.005,
+                x=vline_x - 0.005,
                 y=ytext + 0.005,
-                s=(
-                    f"{int(vline * 100)}%"
-                    if vlines_label_list is None
-                    else f"{vlines_label_list[vline_counter]}"
-                ),
+                s=labels[i] if labels else None,
                 transform=self.axis_top.get_xaxis_text1_transform(0)[0],
                 fontsize=fontsize,
             )
 
             for ratio_axis in self.ratio_axes:
                 ratio_axis.axvline(
-                    x=vline, color=colour, linestyle="dashed", linewidth=1.0
+                    x=vline_x, color=colour, linestyle=linestyle, linewidth=1.0
                 )
 
     def set_title(self, title: str = None, **kwargs):
         """Set title of top panel.
 
         Parameters
         ----------
@@ -583,36 +578,33 @@
         self.fig.savefig(
             plot_name,
             transparent=self.transparent if transparent is None else transparent,
             dpi=self.dpi if dpi is None else dpi,
             **kwargs,
         )
 
-    def atlasify(self, use_tag: bool = True, force: bool = False):
+    def atlasify(self, force: bool = False):
         """Apply ATLAS style to all axes using the atlasify package.
 
         Parameters
         ----------
-        use_tag : bool, optional
-            If False, ATLAS style will be applied but no tag will be put on the plot.
-            If True, the tag will be put on as well, by default True
         force : bool, optional
             Force ATLAS style also if class variable is False, by default False
         """
         if self.plotting_done is False and force is False:
             logger.warning(
                 "`atlasify()` has to be called after plotting --> "
                 "ATLAS style will not be adapted. If you want to do it anyway, "
                 "you can use `force`."
             )
             return
 
         if self.apply_atlas_style or force:
             logger.debug("Initialise ATLAS style using atlasify.")
-            if use_tag is True:
+            if self.use_atlas_tag is True:
                 # TODO: for some reason, pylint complains about the used arguments
                 # when calling atlasify ("unexpected-keyword-arg") error
                 # --> fix this
                 atlasify.atlasify(
                     atlas=self.atlas_first_tag,
                     subtext=self.atlas_second_tag,
                     axes=self.axis_top,
```

### Comparing `puma-hep-0.2.5/puma/roc.py` & `puma-hep-0.2.6/puma/roc.py`

 * *Files 1% similar despite different names*

```diff
@@ -558,15 +558,15 @@
                 for rej_class in self.rej_axes:
                     self.leg_rej_labels[rej_class] = rej_class
 
             self.make_split_legend(handles=plt_handles)
 
         self.plotting_done = True
         if self.apply_atlas_style is True:
-            self.atlasify(use_tag=self.use_atlas_tag)
+            self.atlasify()
             # atlasify can only handle one legend. Therefore, we remove the frame of
             # the second legend by hand
             if self.legend_flavs is not None:
                 self.legend_flavs.set_frame_on(False)
 
     def plot_roc(self, **kwargs) -> mpl.lines.Line2D:
         """Plotting roc curves.
```

### Comparing `puma-hep-0.2.5/puma/tests/hlplots/test_results.py` & `puma-hep-0.2.6/puma/tests/hlplots/test_results.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,14 +87,49 @@
         ------
         AssertionError
             if file does not exist
         """
         if not Path(path).resolve().is_file():
             raise AssertionError(f"File does not exist: {path}")
 
+    def test_plot_probs_bjets(self):
+        """Test that png file is being created."""
+        self.dummy_tagger_1.reference = True
+        self.dummy_tagger_1.f_c = 0.05
+        with tempfile.TemporaryDirectory() as tmp_file:
+            results = Results(signal="bjets", sample="test", output_dir=tmp_file)
+            results.add(self.dummy_tagger_1)
+            results.plot_probs()
+            self.assertIsFile(results.get_filename("probs_bjets"))
+            self.assertIsFile(results.get_filename("probs_cjets"))
+            self.assertIsFile(results.get_filename("probs_ujets"))
+            self.assertIsFile(results.get_filename("probs_pb"))
+            self.assertIsFile(results.get_filename("probs_pc"))
+            self.assertIsFile(results.get_filename("probs_pu"))
+
+    def test_plot_discs_bjets(self):
+        """Test that png file is being created."""
+        self.dummy_tagger_1.reference = True
+        self.dummy_tagger_1.f_c = 0.05
+        with tempfile.TemporaryDirectory() as tmp_file:
+            results = Results(signal="bjets", sample="test", output_dir=tmp_file)
+            results.add(self.dummy_tagger_1)
+            results.plot_discs()
+            self.assertIsFile(results.get_filename("disc"))
+
+    def test_plot_discs_cjets(self):
+        """Test that png file is being created."""
+        self.dummy_tagger_1.reference = True
+        self.dummy_tagger_1.f_b = 0.05
+        with tempfile.TemporaryDirectory() as tmp_file:
+            results = Results(signal="cjets", sample="test", output_dir=tmp_file)
+            results.add(self.dummy_tagger_1)
+            results.plot_discs(wp_vlines=[60])
+            self.assertIsFile(results.get_filename("disc"))
+
     def test_plot_roc_bjets(self):
         """Test that png file is being created."""
         self.dummy_tagger_1.reference = True
         self.dummy_tagger_1.f_c = 0.05
         with tempfile.TemporaryDirectory() as tmp_file:
             results = Results(signal="bjets", sample="test", output_dir=tmp_file)
             results.add(self.dummy_tagger_1)
@@ -149,34 +184,14 @@
                 h_line=self.dummy_tagger_1.working_point,
                 bins=[20, 30, 40, 60, 85, 110, 140, 175, 250],
             )
             self.assertIsFile(Path(tmp_file) / "test_cjets_profile_fixed_cjets_eff.png")
             self.assertIsFile(Path(tmp_file) / "test_cjets_profile_fixed_bjets_rej.png")
             self.assertIsFile(Path(tmp_file) / "test_cjets_profile_fixed_ujets_rej.png")
 
-    def test_plot_discs_bjets(self):
-        """Test that png file is being created."""
-        self.dummy_tagger_1.reference = True
-        self.dummy_tagger_1.f_c = 0.05
-        with tempfile.TemporaryDirectory() as tmp_file:
-            results = Results(signal="bjets", sample="test", output_dir=tmp_file)
-            results.add(self.dummy_tagger_1)
-            results.plot_discs()
-            self.assertIsFile(results.get_filename("disc"))
-
-    def test_plot_discs_cjets(self):
-        """Test that png file is being created."""
-        self.dummy_tagger_1.reference = True
-        self.dummy_tagger_1.f_b = 0.05
-        with tempfile.TemporaryDirectory() as tmp_file:
-            results = Results(signal="cjets", sample="test", output_dir=tmp_file)
-            results.add(self.dummy_tagger_1)
-            results.plot_discs()
-            self.assertIsFile(results.get_filename("disc"))
-
     def test_plot_fraction_scans_hbb_error(self):
         """Test that correct error is raised."""
         self.dummy_tagger_1.reference = True
         self.dummy_tagger_1.f_c = 0.05
         with tempfile.TemporaryDirectory() as tmp_file:
             results = Results(signal="hbb", sample="test", output_dir=tmp_file)
             results.add(self.dummy_tagger_1)
```

### Comparing `puma-hep-0.2.5/puma/tests/hlplots/test_tagger.py` & `puma-hep-0.2.6/puma/tests/hlplots/test_tagger.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/test_histogram.py` & `puma-hep-0.2.6/puma/tests/test_histogram.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,15 +386,15 @@
             atlas_tag_outside=True,
             figsize=(5, 4),
             ylabel="Number of jets",
             n_ratio_panels=1,
         )
         hist_plot.add(self.hist_1, reference=True)
         hist_plot.draw_vlines(
-            vlines_xvalues=[1, 2, 3],
+            xs=[1, 2, 3],
         )
         hist_plot.draw()
 
         plotname = "test_draw_vlines_histogram.png"
         hist_plot.savefig(f"{self.actual_plots_dir}/{plotname}")
         # Uncomment line below to update expected image
         # hist_plot.savefig(f"{self.expected_plots_dir}/{plotname}")
@@ -416,16 +416,16 @@
             atlas_second_tag="",
             figsize=(5, 4),
             ylabel="Number of jets",
             n_ratio_panels=1,
         )
         hist_plot.add(self.hist_1, reference=True)
         hist_plot.draw_vlines(
-            vlines_xvalues=[1, 2, 3],
-            vlines_label_list=["One", "Two", "Three"],
+            xs=[1, 2, 3],
+            labels=["One", "Two", "Three"],
         )
         hist_plot.draw()
 
         plotname = "test_draw_vlines_histogram_custom_labels.png"
         hist_plot.savefig(f"{self.actual_plots_dir}/{plotname}")
         # Uncomment line below to update expected image
         # hist_plot.savefig(f"{self.expected_plots_dir}/{plotname}")
@@ -447,15 +447,15 @@
             atlas_second_tag="",
             figsize=(5, 4),
             ylabel="Number of jets",
             n_ratio_panels=1,
         )
         hist_plot.add(self.hist_1, reference=True)
         hist_plot.draw_vlines(
-            vlines_xvalues=[1, 2, 3],
+            xs=[1, 2, 3],
             same_height=True,
         )
         hist_plot.draw()
 
         plotname = "test_draw_vlines_histogram_same_height.png"
         hist_plot.savefig(f"{self.actual_plots_dir}/{plotname}")
         # Uncomment line below to update expected image
@@ -478,16 +478,16 @@
             atlas_second_tag="",
             figsize=(5, 4),
             ylabel="Number of jets",
             n_ratio_panels=1,
         )
         hist_plot.add(self.hist_1, reference=True)
         hist_plot.draw_vlines(
-            vlines_xvalues=[1, 2, 3],
-            vlines_line_height_list=[0.7, 0.6, 0.5],
+            xs=[1, 2, 3],
+            ys=[0.7, 0.6, 0.5],
         )
         hist_plot.draw()
 
         plotname = "test_draw_vlines_histogram_custom_yheight.png"
         hist_plot.savefig(f"{self.actual_plots_dir}/{plotname}")
         # Uncomment line below to update expected image
         # hist_plot.savefig(f"{self.expected_plots_dir}/{plotname}")
@@ -625,15 +625,15 @@
             )
         )
         hist_plot.draw()
 
         plotname = "test_flavoured_labels.png"
         hist_plot.savefig(f"{self.actual_plots_dir}/{plotname}")
         # Uncomment line below to update expected image
-        hist_plot.savefig(f"{self.expected_plots_dir}/{plotname}")
+        # hist_plot.savefig(f"{self.expected_plots_dir}/{plotname}")
         self.assertIsNone(
             compare_images(
                 f"{self.actual_plots_dir}/{plotname}",
                 f"{self.expected_plots_dir}/{plotname}",
                 tol=1,
             )
         )
```

### Comparing `puma-hep-0.2.5/puma/tests/test_line_2d.py` & `puma-hep-0.2.6/puma/tests/test_line_2d.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/test_metrics.py` & `puma-hep-0.2.6/puma/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/test_pie_chart.py` & `puma-hep-0.2.6/puma/tests/test_pie_chart.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/test_plot_base.py` & `puma-hep-0.2.6/puma/tests/test_plot_base.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/test_roc.py` & `puma-hep-0.2.6/puma/tests/test_roc.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/test_var_vs_eff.py` & `puma-hep-0.2.6/puma/tests/test_var_vs_eff.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/test_var_vs_var.py` & `puma-hep-0.2.6/puma/tests/test_var_vs_var.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/utils/test_discriminant.py` & `puma-hep-0.2.6/puma/tests/utils/test_discriminant.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/utils/test_generate.py` & `puma-hep-0.2.6/puma/tests/utils/test_generate.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/utils/test_histogram_utils.py` & `puma-hep-0.2.6/puma/tests/utils/test_histogram_utils.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/tests/utils/test_utils.py` & `puma-hep-0.2.6/puma/tests/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/utils/__init__.py` & `puma-hep-0.2.6/puma/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/utils/discriminant.py` & `puma-hep-0.2.6/puma/utils/discriminant.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/utils/generate.py` & `puma-hep-0.2.6/puma/utils/generate.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/utils/histogram.py` & `puma-hep-0.2.6/puma/utils/histogram.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/utils/logging.py` & `puma-hep-0.2.6/puma/utils/logging.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/var_vs_eff.py` & `puma-hep-0.2.6/puma/var_vs_eff.py`

 * *Files identical despite different names*

### Comparing `puma-hep-0.2.5/puma/var_vs_var.py` & `puma-hep-0.2.6/puma/var_vs_var.py`

 * *Files 1% similar despite different names*

```diff
@@ -407,8 +407,8 @@
                 self.ylabel_ratio[0],
                 align_right=False,
                 labelpad=labelpad,
             )
         self.make_legend(plt_handles, ax_mpl=self.axis_top)
         self.plotting_done = True
         if self.apply_atlas_style is True:
-            self.atlasify(use_tag=self.use_atlas_tag)
+            self.atlasify()
```

### Comparing `puma-hep-0.2.5/puma_hep.egg-info/PKG-INFO` & `puma-hep-0.2.6/puma_hep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: puma-hep
-Version: 0.2.5
+Version: 0.2.6
 Summary: Plotting API for HEP flavour tagging plots.
 Home-page: https://github.com/umami-hep/puma
 Keywords: machine learning,flavour tagging,plots
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `puma-hep-0.2.5/puma_hep.egg-info/SOURCES.txt` & `puma-hep-0.2.6/puma_hep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

