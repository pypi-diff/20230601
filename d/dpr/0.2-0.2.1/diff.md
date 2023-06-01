# Comparing `tmp/dpr-0.2.tar.gz` & `tmp/dpr-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dpr-0.2.tar", last modified: Thu Jul 16 15:42:43 2020, max compression
+gzip compressed data, was "dpr-0.2.1.tar", last modified: Thu Jun  1 10:39:59 2023, max compression
```

## Comparing `dpr-0.2.tar` & `dpr-0.2.1.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-16 15:42:43.685962 dpr-0.2/
--rw-r--r--   0 runner    (1001) docker     (116)     1053 2020-07-16 15:42:36.000000 dpr-0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (116)      561 2020-07-16 15:42:36.000000 dpr-0.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (116)     1071 2020-07-16 15:42:36.000000 dpr-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      140 2020-07-16 15:42:36.000000 dpr-0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5730 2020-07-16 15:42:43.685962 dpr-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4613 2020-07-16 15:42:36.000000 dpr-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-16 15:42:43.681962 dpr-0.2/datasets/
--rw-r--r--   0 runner    (1001) docker     (116)      174 2020-07-16 15:42:36.000000 dpr-0.2/datasets/README.md
--rw-r--r--   0 runner    (1001) docker     (116)   349300 2020-07-16 15:42:36.000000 dpr-0.2/datasets/af_left_AFD.txt
--rw-r--r--   0 runner    (1001) docker     (116)    48206 2020-07-16 15:42:36.000000 dpr-0.2/datasets/af_left_AFD_realigned.png
--rw-r--r--   0 runner    (1001) docker     (116)   145053 2020-07-16 15:42:36.000000 dpr-0.2/datasets/af_left_AFD_realigned.txt
--rw-r--r--   0 runner    (1001) docker     (116)     8074 2020-07-16 15:42:36.000000 dpr-0.2/datasets/af_left_average_coordinates.txt
--rw-r--r--   0 runner    (1001) docker     (116)  5820774 2020-07-16 15:42:36.000000 dpr-0.2/datasets/af_left_coordinates.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1875 2020-07-16 15:42:36.000000 dpr-0.2/datasets/af_left_pval_realigned.txt
--rw-r--r--   0 runner    (1001) docker     (116)     6650 2020-07-16 15:42:36.000000 dpr-0.2/datasets/af_left_pval_unaligned.txt
--rw-r--r--   0 runner    (1001) docker     (116)  2541731 2020-07-16 15:42:36.000000 dpr-0.2/datasets/af_left_truncated_coordinates.txt
--rw-r--r--   0 runner    (1001) docker     (116)   185152 2020-07-16 15:42:36.000000 dpr-0.2/datasets/bundles.txt
--rw-r--r--   0 runner    (1001) docker     (116)   178990 2020-07-16 15:42:36.000000 dpr-0.2/datasets/bundles_cut.txt
--rw-r--r--   0 runner    (1001) docker     (116)   370348 2020-07-16 15:42:36.000000 dpr-0.2/datasets/coordinates.pkl
--rw-r--r--   0 runner    (1001) docker     (116)   163425 2020-07-16 15:42:36.000000 dpr-0.2/datasets/pvals_overlay.png
--rw-r--r--   0 runner    (1001) docker     (116)    90452 2020-07-16 15:42:36.000000 dpr-0.2/datasets/pvals_realigned.png
--rw-r--r--   0 runner    (1001) docker     (116)    91613 2020-07-16 15:42:36.000000 dpr-0.2/datasets/pvals_unaligned.png
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-16 15:42:43.681962 dpr-0.2/dpr/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-16 15:42:36.000000 dpr-0.2/dpr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    11146 2020-07-16 15:42:36.000000 dpr-0.2/dpr/register.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-16 15:42:43.685962 dpr-0.2/dpr/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-07-16 15:42:36.000000 dpr-0.2/dpr/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1013 2020-07-16 15:42:36.000000 dpr-0.2/dpr/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (116)     3719 2020-07-16 15:42:36.000000 dpr-0.2/dpr/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-16 15:42:43.681962 dpr-0.2/dpr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5730 2020-07-16 15:42:43.000000 dpr-0.2/dpr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      821 2020-07-16 15:42:43.000000 dpr-0.2/dpr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-16 15:42:43.000000 dpr-0.2/dpr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       40 2020-07-16 15:42:43.000000 dpr-0.2/dpr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2020-07-16 15:42:43.000000 dpr-0.2/dpr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)   818296 2020-07-16 15:42:36.000000 dpr-0.2/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (116)       39 2020-07-16 15:42:36.000000 dpr-0.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-16 15:42:43.685962 dpr-0.2/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (116)     5098 2020-07-16 15:42:36.000000 dpr-0.2/scripts/dpr
--rwxr-xr-x   0 runner    (1001) docker     (116)     4612 2020-07-16 15:42:36.000000 dpr-0.2/scripts/dpr_make_fancy_graph
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-07-16 15:42:43.685962 dpr-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      718 2020-07-16 15:42:36.000000 dpr-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:59.759012 dpr-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-01 10:39:45.000000 dpr-0.2.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-01 10:39:45.000000 dpr-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-01 10:39:45.000000 dpr-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-01 10:39:59.759012 dpr-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3336 2023-06-01 10:39:45.000000 dpr-0.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:59.755012 dpr-0.2.1/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   349300 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/af_left_AFD.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    48206 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/af_left_AFD_realigned.png
+-rw-r--r--   0 runner    (1001) docker     (123)   145053 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/af_left_AFD_realigned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/af_left_average_coordinates.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  5820774 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/af_left_coordinates.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/af_left_pval_realigned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/af_left_pval_unaligned.txt
+-rw-r--r--   0 runner    (1001) docker     (123)  2541731 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/af_left_truncated_coordinates.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   185152 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/bundles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   178990 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/bundles_cut.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   370348 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/coordinates.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)   163425 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/pvals_overlay.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90452 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/pvals_realigned.png
+-rw-r--r--   0 runner    (1001) docker     (123)    91613 2023-06-01 10:39:45.000000 dpr-0.2.1/datasets/pvals_unaligned.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:59.755012 dpr-0.2.1/dpr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:45.000000 dpr-0.2.1/dpr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11097 2023-06-01 10:39:45.000000 dpr-0.2.1/dpr/register.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:59.759012 dpr-0.2.1/dpr/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:45.000000 dpr-0.2.1/dpr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-06-01 10:39:45.000000 dpr-0.2.1/dpr/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3737 2023-06-01 10:39:45.000000 dpr-0.2.1/dpr/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:59.755012 dpr-0.2.1/dpr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-06-01 10:39:59.000000 dpr-0.2.1/dpr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-01 10:39:59.000000 dpr-0.2.1/dpr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 10:39:59.000000 dpr-0.2.1/dpr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 10:39:59.000000 dpr-0.2.1/dpr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 10:39:59.000000 dpr-0.2.1/dpr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   818296 2023-06-01 10:39:45.000000 dpr-0.2.1/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-01 10:39:45.000000 dpr-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 10:39:59.759012 dpr-0.2.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5379 2023-06-01 10:39:45.000000 dpr-0.2.1/scripts/dpr
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4547 2023-06-01 10:39:45.000000 dpr-0.2.1/scripts/dpr_make_fancy_graph
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 10:39:59.759012 dpr-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 10:39:45.000000 dpr-0.2.1/setup.py
```

### Comparing `dpr-0.2/CHANGELOG.md` & `dpr-0.2.1/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # Changelog
 
+## [v0.2.1] - 2023-06-01
+
+- Support for csv files input and output
+- Documentation now available at https://dpr.readthedocs.io
+
 ## [v0.2] - 2020-07-16
 
 - Fix bug due to interpolation in ```dpr.utils.draw_fancy_graph```
 - Add Matlab version and example under the folder ```matlab```
 
 ## [v0.1.2] - 2019-06-18
 - New command line script ```dpr_make_fancy_graph``` to draw p-values over bundles as in the paper
```

### Comparing `dpr-0.2/LICENSE` & `dpr-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dpr-0.2/README.md` & `dpr-0.2.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,31 @@
+Metadata-Version: 2.1
+Name: dpr
+Version: 0.2.1
+Summary: Implementation of "Reducing variability in along-tract analysis with diffusion profile realignment".
+Author-email: Samuel St-Jean <firstname.st_jean@med.lu.se>
+License: MIT License
+Project-URL: Homepage, https://github.com/samuelstjean/dpr
+Project-URL: Documentation, https://dpr.readthedocs.io/en/latest/
+Project-URL: Changelog, https://github.com/samuelstjean/dpr/blob/master/CHANGELOG.md
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Diffusion profile realignment (dpr)
 
 An example and assorted implementation from the manuscript **Reducing variability in along-tract analysis with diffusion profile realignment**.
 Have a look at the [example](example.ipynb) on how to use the package and run it on a small example dataset.
 
 To install the package, just run
 ~~~
 pip install dpr
 ~~~
 
+The documentation is available at https://dpr.readthedocs.io.
 
 ### The matlab version
 
 There is also a shiny new version written in matlab, with an assorted example, available in the [matlab](matlab) folder.
 Feel free to check out and edit the functions as needed for your own usage.
 
 ### A quick example from the command line
@@ -49,41 +63,14 @@
 ~~~
 
 And this is the results
 
 ![](datasets/pvals_unaligned.png)
 ![](datasets/pvals_realigned.png)
 
-### Using docker (instead of installing everything)
-
-Well, you will still need to install docker first, see https://runnable.com/docker/getting-started/.
-After that, you can now pull a version from [Dockerhub](https://hub.docker.com/repository/docker/samuelstjean/dpr).
-
-~~~bash
-docker pull samuelstjean/dpr:v0.2
-~~~
-
-The two diffusion profile realignment scripts can now be run using
-
-~~~bash
-docker run samuelstjean/dpr:v0.2 # the default command is to run dpr --help
-docker run samuelstjean/dpr:v0.2 dpr_make_fancy_graph --help
-~~~
-
-That's it for the basic version, don't hesitate to adapt everything to your needs.
-
-As a more advanced example, to mount your own data folder inside the container (here we re-use the previous example), use
-
-~~~bash
-docker run -it -v /home/samuel/git/dpr/datasets:/mnt samuelstjean/dpr:v0.2 dpr /mnt/af_left_AFD.txt /mnt/af_left_AFD_realigned.txt --exploredti --do_graph -f -v --points 75
-docker run -it -v /home/samuel/git/dpr/datasets:/mnt samuelstjean/dpr:v0.2 dpr_make_fancy_graph /mnt/af_left_pval_unaligned.txt /mnt/af_left_coordinates.txt /mnt/af_left_truncated_coordinates.txt /mnt/af_left_average_coordinates.txt 0,2 /mnt/pvals_unaligned.png --title 'p-values before realignment' -f
-~~~
-
-The result will be located in the folder you specified, here we used ```/home/samuel/git/dpr/datasets```.
-
 ### Datasets and reference
 
 The main reference is
 
 ~~~
 Samuel St-Jean, Maxime Chamberland, Max A. Viergever, Alexander Leemans,
 Reducing variability in along-tract analysis with diffusion profile realignment,
```

### Comparing `dpr-0.2/datasets/af_left_AFD.txt` & `dpr-0.2.1/datasets/af_left_AFD.txt`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/af_left_AFD_realigned.png` & `dpr-0.2.1/datasets/af_left_AFD_realigned.png`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/af_left_AFD_realigned.txt` & `dpr-0.2.1/datasets/af_left_AFD_realigned.txt`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/af_left_average_coordinates.txt` & `dpr-0.2.1/datasets/af_left_average_coordinates.txt`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/af_left_coordinates.txt` & `dpr-0.2.1/datasets/af_left_coordinates.txt`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/af_left_pval_realigned.txt` & `dpr-0.2.1/datasets/af_left_pval_realigned.txt`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/af_left_pval_unaligned.txt` & `dpr-0.2.1/datasets/af_left_pval_unaligned.txt`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/af_left_truncated_coordinates.txt` & `dpr-0.2.1/datasets/af_left_truncated_coordinates.txt`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/bundles.txt` & `dpr-0.2.1/datasets/bundles.txt`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/bundles_cut.txt` & `dpr-0.2.1/datasets/bundles_cut.txt`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/coordinates.pkl` & `dpr-0.2.1/datasets/coordinates.pkl`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/pvals_overlay.png` & `dpr-0.2.1/datasets/pvals_overlay.png`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/pvals_realigned.png` & `dpr-0.2.1/datasets/pvals_realigned.png`

 * *Files identical despite different names*

### Comparing `dpr-0.2/datasets/pvals_unaligned.png` & `dpr-0.2.1/datasets/pvals_unaligned.png`

 * *Files identical despite different names*

### Comparing `dpr-0.2/dpr/register.py` & `dpr-0.2.1/dpr/register.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import division, print_function
-
 import numpy as np
 
 from itertools import product
 from warnings import warn
 
 from scipy import ndimage
```

### Comparing `dpr-0.2/dpr/tests/test_register.py` & `dpr-0.2.1/dpr/tests/test_register.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from __future__ import division, print_function
-
 import numpy as np
 
 from dpr.register import truncate, extrapolate
 
 
 def test_extrapolate():
 
     x = np.arange(-10, 10)
     a, b, c = -1, 0, 4
     y = a * x**2 + b * x + c
     ymax = y.argmax()
 
-    peak, value = extrapolate([x[ymax - 1], x[ymax], x[ymax + 1]],
-                              [y[ymax - 1], y[ymax], y[ymax + 1]],
-                              return_value=True)
+    peak, value = extrapolate(
+        [x[ymax - 1], x[ymax], x[ymax + 1]],
+        [y[ymax - 1], y[ymax], y[ymax + 1]],
+        return_value=True,
+    )
 
     np.testing.assert_array_almost_equal(peak, 0)
     np.testing.assert_array_almost_equal(value, 4)
 
 
 def test_truncate():
     a = np.full((1, 10), np.nan)
     b = np.full((1, 10), np.nan)
     a[:, 2:6] = range(2, 6)
     b[:, 4:7] = range(4, 7)
 
     c = np.concatenate((a, b))
 
     answer = np.array([[4, 5], [4, 5]])
-    np.testing.assert_equal(truncate(c, mode='shortest'), answer)
+    np.testing.assert_equal(truncate(c, mode="shortest"), answer)
 
     answer = np.zeros((2, len(range(2, 7)))) * np.nan
     answer[0, range(4)] = range(2, 6)
     answer[1, range(2, 5)] = range(4, 7)
-    np.testing.assert_equal(truncate(c, mode='longest'), answer)
+    np.testing.assert_equal(truncate(c, mode="longest"), answer)
```

### Comparing `dpr-0.2/dpr/utils.py` & `dpr-0.2.1/dpr/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import division, print_function
-
 import numpy as np
 import matplotlib.pyplot as plt
 
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 
 
 def read_per_line(fname, maxlines=50000):
@@ -39,19 +37,19 @@
         for line in file:
             try:
                 yield line.split(delimiter, 1)[1]
             except IndexError:
                 continue
 
 
-def strip_header(filename, columns=0):
-    header = np.genfromtxt(filename, dtype=str, usecols=columns)
+def strip_header(filename, columns=0, delimiter=None):
+    header = np.genfromtxt(filename, dtype=str, usecols=columns, delimiter=delimiter)
     with open(filename, 'r') as file:
-        ncols = len(file.readline().split())
-    bundles = np.genfromtxt(filename, usecols=range(1, ncols))
+        ncols = len(file.readline().split(delimiter))
+    bundles = np.genfromtxt(filename, usecols=range(1, ncols), delimiter=delimiter)
     return bundles, header
 
 
 # Actual colors I used in the manuscript
 blue = np.array([0.6093924, 0.73212757, 0.82249106])
 green = np.array([0.22953434, 0.57685998, 0.42976558])
```

### Comparing `dpr-0.2/dpr.egg-info/SOURCES.txt` & `dpr-0.2.1/dpr.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 CHANGELOG.md
-Dockerfile
 LICENSE
 MANIFEST.in
 README.md
 example.ipynb
-requirements.txt
+pyproject.toml
 setup.py
 datasets/README.md
 datasets/af_left_AFD.txt
 datasets/af_left_AFD_realigned.png
 datasets/af_left_AFD_realigned.txt
 datasets/af_left_average_coordinates.txt
 datasets/af_left_coordinates.txt
```

### Comparing `dpr-0.2/example.ipynb` & `dpr-0.2.1/example.ipynb`

 * *Files identical despite different names*

### Comparing `dpr-0.2/scripts/dpr` & `dpr-0.2.1/scripts/dpr`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 #!/usr/bin/env python
 
-from __future__ import division, print_function
-
 import numpy as np
 import matplotlib.pyplot as plt
 
 import argparse
 import logging
 import os
 
@@ -38,15 +36,15 @@
     p.add_argument('data', metavar='input',
                    help='Path of the input text file of bundles.')
 
     p.add_argument('output', metavar='output',
                    help='Path of the output text file of realigned bundles.')
 
     p.add_argument('--exploredti', action='store_true',
-                   help='Strip the first column from the input file.')
+                   help='Strip the first column from the input file as used by explore dti to store each subject name.')
 
     p.add_argument('--do_graph', action='store_true',
                    help='Save a small plot of the original and realigned data.')
 
     p.add_argument('--points', metavar='int', type=int,
                    help='Number of points for the final resampling. Default: longest bundle')
 
@@ -84,25 +82,32 @@
 
     if args.verbose:
         logger.setLevel(logging.INFO)
         logger.info('Verbosity is on')
 
     if os.path.isfile(args.output):
         if args.overwrite:
-            logger.warning('Overwriting {}'.format(os.path.realpath(args.output)))
+            logger.warning(f'Overwriting {os.path.realpath(args.output)}')
         else:
-            parser.error('{} already exists! Use -f or --force to overwrite it.'.format(args.output))
+            parser.error(f'{args.output} already exists! Use -f or --force to overwrite it.')
 
     # load the data
+    _, ext = os.path.splitext(args.data)
+
+    if ext == '.csv':
+        delimiter = ','
+    else:
+        delimiter = None
+
     if args.exploredti:
-        data, header = strip_header(args.data)
+        data, header = strip_header(args.data, delimiter=delimiter)
     else:
-        data = np.genfromtxt(args.data)
+        data = np.genfromtxt(args.data, delimiter=delimiter)
 
-    logger.info('Number of bundles is {}, original number of points per tract is {}'.format(*data.shape))
+    logger.info(f'Number of bundles is {data.shape[0]}, original number of points per tract is {data.shape[1]}')
 
     if args.coordinates is not None:
         coordinates = np.genfromtxt(args.coordinates)
         data = flip_fibers(data, coordinates)
 
     aligned, shifts = align_bundles(data)
     truncated = truncate(aligned)
@@ -111,15 +116,15 @@
     if args.points is None:
         num_points = truncated.shape[1]
     else:
         num_points = args.points
 
     resampled = resample_bundles_to_same(truncated, num_points=num_points)
 
-    logger.info('Final number of points per tract is {}'.format(num_points))
+    logger.info(f'Final number of points per tract is {num_points}')
 
     if args.do_graph:
         f, axes = plt.subplots(2, 1, sharex=False, sharey=True)
         labels = 'Before realignment', 'After realignment'
 
         for bund, ax, label in zip([data, resampled], axes, labels):
             mean = np.nanmean(bund, axis=0)
@@ -135,13 +140,20 @@
         f.tight_layout()
         f.savefig(args.output.replace('.txt','.png'), dpi=100, bbox_inches='tight')
 
     # should patch back whatever was removed beforehand here
     if args.exploredti:
         resampled = np.column_stack((header, resampled))
 
+    _, ext = os.path.splitext(args.output)
+
+    if ext == '.csv':
+        delimiter = ','
+    else:
+        delimiter = ' '
+
     with open(args.output, 'w') as file:
-        np.savetxt(file, resampled, delimiter=' ', fmt='%s')
+        np.savetxt(file, resampled, delimiter=delimiter, fmt='%s')
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `dpr-0.2/scripts/dpr_make_fancy_graph` & `dpr-0.2.1/scripts/dpr_make_fancy_graph`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 #!/usr/bin/env python
 
-from __future__ import division, print_function
-
 import numpy as np
 
 import argparse
 import logging
 import os
 
 from dpr.utils import draw_fancy_graph, read_per_line
@@ -94,17 +92,17 @@
 
     if args.verbose:
         logger.setLevel(logging.INFO)
         logger.info('Verbosity is on')
 
     if os.path.isfile(args.output):
         if args.overwrite:
-            logger.warning('Overwriting {}'.format(os.path.realpath(args.output)))
+            logger.warning(f'Overwriting {os.path.realpath(args.output)}')
         else:
-            parser.error('{} already exists! Use -f or --force to overwrite it.'.format(args.output))
+            parser.error(f'{args.output} already exists! Use -f or --force to overwrite it.')
 
     axis1, axis2 = args.columns
 
     # Load up the simple text files
     pvals = np.loadtxt(args.pvals)
 
     representative = np.loadtxt(args.representative)
```

