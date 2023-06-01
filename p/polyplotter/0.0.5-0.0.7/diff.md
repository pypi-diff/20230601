# Comparing `tmp/polyplotter-0.0.5.tar.gz` & `tmp/polyplotter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyplotter-0.0.5.tar", last modified: Sun Oct 23 07:08:26 2022, max compression
+gzip compressed data, was "polyplotter-0.0.7.tar", last modified: Thu Jun  1 02:53:11 2023, max compression
```

## Comparing `polyplotter-0.0.5.tar` & `polyplotter-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-10-23 07:08:26.141051 polyplotter-0.0.5/
--rw-rw-rw-   0        0        0     1094 2022-01-06 01:59:03.000000 polyplotter-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      760 2022-10-23 07:08:26.142052 polyplotter-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      244 2022-08-01 23:36:52.000000 polyplotter-0.0.5/README.md
--rw-rw-rw-   0        0        0      110 2022-01-06 02:08:29.000000 polyplotter-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      655 2022-10-23 07:08:26.146054 polyplotter-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-10-23 07:08:26.121054 polyplotter-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2022-10-23 07:08:26.127054 polyplotter-0.0.5/src/polyplotter/
--rw-rw-rw-   0        0        0       36 2022-01-06 02:00:41.000000 polyplotter-0.0.5/src/polyplotter/__init__.py
--rw-rw-rw-   0        0        0     3087 2022-10-23 07:06:44.000000 polyplotter-0.0.5/src/polyplotter/polyplotter.py
-drwxrwxrwx   0        0        0        0 2022-10-23 07:08:26.140077 polyplotter-0.0.5/src/polyplotter.egg-info/
--rw-rw-rw-   0        0        0      760 2022-10-23 07:08:26.000000 polyplotter-0.0.5/src/polyplotter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2022-10-23 07:08:26.000000 polyplotter-0.0.5/src/polyplotter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-23 07:08:26.000000 polyplotter-0.0.5/src/polyplotter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-10-23 07:08:26.000000 polyplotter-0.0.5/src/polyplotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:11.697207 polyplotter-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 02:52:48.000000 polyplotter-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-01 02:53:11.693207 polyplotter-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 02:52:48.000000 polyplotter-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-01 02:52:48.000000 polyplotter-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 02:53:11.697207 polyplotter-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:11.693207 polyplotter-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:11.693207 polyplotter-0.0.7/src/polyplotter/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-01 02:52:48.000000 polyplotter-0.0.7/src/polyplotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-01 02:52:48.000000 polyplotter-0.0.7/src/polyplotter/polyplotter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:11.693207 polyplotter-0.0.7/src/polyplotter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-01 02:53:11.000000 polyplotter-0.0.7/src/polyplotter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-01 02:53:11.000000 polyplotter-0.0.7/src/polyplotter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:53:11.000000 polyplotter-0.0.7/src/polyplotter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 02:53:11.000000 polyplotter-0.0.7/src/polyplotter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-01 02:53:11.000000 polyplotter-0.0.7/src/polyplotter.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:53:11.693207 polyplotter-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-06-01 02:52:48.000000 polyplotter-0.0.7/tests/test_polyplotter.py
```

### Comparing `polyplotter-0.0.5/LICENSE` & `polyplotter-0.0.7/LICENSE`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Julius Simonelli
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Julius Simonelli
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `polyplotter-0.0.5/src/polyplotter/polyplotter.py` & `polyplotter-0.0.7/src/polyplotter/polyplotter.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,94 +1,98 @@
-import numpy as np
-from matplotlib import pyplot as plt
-from shapely.geometry.multipolygon import MultiPolygon
-from shapely.geometry.polygon import Polygon
-from shapely.geometry.collection import GeometryCollection
-from shapely import wkt
-
-
-def plotpoly(obj, verbose=False):
-    """plotpoly figure outs what the obj is and routes it to the appropriate plotter()
-    How often do I get lists? And what should I do in those cases?
-    TODO: If dictionary, plot every key?
-    If it's a list, should I try to plot it as a whole, and then if that doesn't work, iterate through the list and plot what i can?
-    """
-    if isinstance(obj, np.ndarray):
-        if verbose:
-            print("np.ndarray detected")
-        plot_ndarray_poly(obj)
-    elif isinstance(obj, Polygon):
-        if verbose:
-            print("shapely Polygon detected")
-        plot_shapely_poly(obj)
-    elif isinstance(obj, MultiPolygon):
-        if verbose:
-            print("shapely MultiPolygon detected")
-        plot_shapely_multipoly(obj)
-    elif isinstance(obj, GeometryCollection):
-        if verbose:
-            print("shapely GeometryCollection detected")
-        plot_shapely_geometry_collection(obj)
-    elif isinstance(obj, dict):
-        if verbose:
-            print("dict detected - running recursively on items")
-        for _, v in obj.items():
-            plotpoly(v)
-    elif isinstance(obj, list):
-        if verbose:
-            print("list detected")
-        try:
-            plt.plot(*zip(*obj))
-        except TypeError:
-            if verbose:
-                print("trying recurively on elements of list")
-            for item in obj:
-                plotpoly(item)
-    elif isinstance(obj, str):
-        # for example, wkt
-        if verbose:
-            print("str detected - checking if wkt")
-        try:
-            poly = wkt.loads(obj)
-            plot_shapely_poly(poly)
-        except Exception as e:  # WKTReadingError
-            raise ValueError(f"String not wkt: {obj=}") from e
-    elif isinstance(obj, tuple):
-        """
-        example:
-        x = np.array([1, 3, 5, 7, 9, 6, 4, 1])
-        y = np.array([1, 9, 8, 6, 4, 3, 2, 1])
-        plotpoly(x, y)
-        """
-        plt.plot(*obj)
-    else:
-        print(f"type {type(obj)} not expected")
-        print(f"{obj=}")
-
-
-def plot_ndarray_poly(arr: np.ndarray):
-    """If it's a numpy array, we'll simply wrap in in a shapely geometry first."""
-    poly = Polygon(np.concatenate(arr, axis=0))
-    plot_shapely_poly(poly)
-
-
-def plot_shapely_poly(poly, reverse_y=True):
-    # x, y = poly.exterior.xy
-    if reverse_y:
-        plt.gca().invert_yaxis()
-    plt.plot(*poly.exterior.xy)
-    plt.show()
-
-
-def plot_shapely_multipoly(multipoly, reverse_y=True):
-    if reverse_y:
-        plt.gca().invert_yaxis()
-    for geom in multipoly.geoms:
-        plt.plot(*geom.exterior.xy)
-
-    plt.gca().axis("equal")
-    plt.show()
-
-
-def plot_shapely_geometry_collection(gc):
-    for geom in gc.geoms:
-        print("Need to plot this")
+import numpy as np
+import shapely
+from matplotlib import pyplot as plt
+from shapely.geometry.collection import GeometryCollection
+from shapely.geometry.multipolygon import MultiPolygon
+from shapely.geometry.polygon import Polygon
+
+
+def plotpoly(obj, verbose=False):
+    """plotpoly figure outs what the obj is and routes it to the appropriate plotter()
+    How often do I get lists? And what should I do in those cases?
+    TODO: If dictionary, plot every key?
+    If it's a list, should I try to plot it as a whole, and then if that doesn't work, iterate through the list and plot what i can?
+    """
+    if isinstance(obj, np.ndarray):
+        if verbose:
+            print("np.ndarray detected")
+        plot_ndarray_poly(obj)
+    elif isinstance(obj, Polygon):
+        if verbose:
+            print("shapely Polygon detected")
+        plot_shapely_poly(obj)
+    elif isinstance(obj, MultiPolygon):
+        if verbose:
+            print("shapely MultiPolygon detected")
+        plot_shapely_multipoly(obj)
+    elif isinstance(obj, GeometryCollection):
+        if verbose:
+            print("shapely GeometryCollection detected")
+        plot_shapely_geometry_collection(obj)
+    elif isinstance(obj, dict):
+        if verbose:
+            print("dict detected - running recursively on items")
+        for _, v in obj.items():
+            plotpoly(v)
+    elif isinstance(obj, list):
+        if verbose:
+            print("list detected")
+        try:
+            plt.plot(*zip(*obj))
+        except TypeError:
+            if verbose:
+                print("trying recurively on elements of list")
+            for item in obj:
+                plotpoly(item)
+    elif isinstance(obj, str):
+        # for example, wkt
+        if verbose:
+            print("str detected - checking if wkt")
+        try:
+            poly = shapely.wkt.loads(obj)
+            plot_shapely_poly(poly)
+        except Exception as e:  # WKTReadingError
+            raise ValueError(f"String not wkt: {obj=}") from e
+    elif isinstance(obj, tuple):
+        """
+        example:
+        x = np.array([1, 3, 5, 7, 9, 6, 4, 1])
+        y = np.array([1, 9, 8, 6, 4, 3, 2, 1])
+        plotpoly(x, y)
+        """
+        plt.plot(*obj)
+    else:
+        print(f"type {type(obj)} not expected")
+        print(f"{obj=}")
+
+
+def plot_ndarray_poly(arr: np.ndarray):
+    """If it's a numpy array, we'll wrap it in a shapely geometry first."""
+    try:
+        poly = Polygon(arr)
+    except Exception:
+        # TODO add the test case that requires this
+        poly = Polygon(np.concatenate(arr, axis=0))
+    plot_shapely_poly(poly)
+
+
+def plot_shapely_poly(poly, reverse_y=True):
+    # x, y = poly.exterior.xy
+    if reverse_y:
+        plt.gca().invert_yaxis()
+    plt.plot(*poly.exterior.xy)
+    plt.show()
+
+
+def plot_shapely_multipoly(multipoly, reverse_y=True):
+    if reverse_y:
+        plt.gca().invert_yaxis()
+    for geom in multipoly.geoms:
+        plt.plot(*geom.exterior.xy)
+
+    plt.gca().axis("equal")
+    plt.show()
+
+
+def plot_shapely_geometry_collection(gc):
+    for geom in gc.geoms:
+        print("Need to plot this")
```

