# Comparing `tmp/thalassa-0.3.0.tar.gz` & `tmp/thalassa-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thalassa-0.3.0.tar", max compression
+gzip compressed data, was "thalassa-0.3.1.tar", max compression
```

## Comparing `thalassa-0.3.0.tar` & `thalassa-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    14138 2023-03-02 09:50:57.249458 thalassa-0.3.0/LICENSE
--rw-r--r--   0        0        0     2392 2023-05-12 15:48:27.668665 thalassa-0.3.0/README.md
--rw-r--r--   0        0        0     3514 2023-05-12 17:03:10.434827 thalassa-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-02 09:50:57.249458 thalassa-0.3.0/thalassa/__init__.py
--rw-r--r--   0        0        0    11314 2023-05-08 05:42:04.878122 thalassa-0.3.0/thalassa/api.py
--rw-r--r--   0        0        0     5510 2023-05-12 14:20:53.774892 thalassa-0.3.0/thalassa/normalization.py
--rw-r--r--   0        0        0     9438 2023-05-12 14:20:53.768225 thalassa-0.3.0/thalassa/utils.py
--rw-r--r--   0        0        0     3849 1970-01-01 00:00:00.000000 thalassa-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    14138 2023-03-02 09:50:57.249458 thalassa-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2828 2023-06-01 07:03:11.100389 thalassa-0.3.1/README.md
+-rw-r--r--   0        0        0     3295 2023-06-01 11:33:12.846650 thalassa-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-02 09:50:57.249458 thalassa-0.3.1/thalassa/__init__.py
+-rw-r--r--   0        0        0    12715 2023-06-01 11:25:39.826012 thalassa-0.3.1/thalassa/api.py
+-rw-r--r--   0        0        0     5510 2023-05-12 14:20:53.774892 thalassa-0.3.1/thalassa/normalization.py
+-rw-r--r--   0        0        0     9438 2023-05-12 14:20:53.768225 thalassa-0.3.1/thalassa/utils.py
+-rw-r--r--   0        0        0     4141 1970-01-01 00:00:00.000000 thalassa-0.3.1/PKG-INFO
```

### Comparing `thalassa-0.3.0/LICENSE` & `thalassa-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `thalassa-0.3.0/README.md` & `thalassa-0.3.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 Thalassa
 ========
 
+[![Documentation Status](https://readthedocs.org/projects/thalassa/badge/?version=latest)](https://thalassa.readthedocs.io/en/latest/?badge=latest) ![GitHub release (latest by date)](https://img.shields.io/github/v/release/ec-jrc/Thalassa) ![CI](https://github.com/ec-jrc/Thalassa/actions/workflows/run_tests.yml/badge.svg)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ec-jrc/Thalassa/master?urlpath=lab)
+
 Thalassa ia a library for visualizing unstructured mesh data.
 
 It builds upon [geoviews](https://geoviews.org/) and [datashader](https://datashader.org/)
 and can easily handle meshes with millions of nodes interactively.
 
 <!-- https://user-images.githubusercontent.com/411196/146007390-88e8cc59-9ae9-4a15-83fd-f7f1f2d724c2.mp4 -->
```

### Comparing `thalassa-0.3.0/pyproject.toml` & `thalassa-0.3.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "thalassa"
-version = "0.3.0"  # overwritten by poetry-dynamic-versioning plugin
+version = "0.3.1"  # overwritten by poetry-dynamic-versioning plugin
 description = "A library for visualizing large scale results of hydrodynamic simulations"
 authors = ["Panos Mavrogiorgos <pmav99@gmail.com>"]
 license = 'EUPL-1.2'
 readme = "README.md"
 repository = "https://github.com/ec-jrc/thalassa.git"
 classifiers = [
     "Operating System :: OS Independent",
@@ -14,44 +14,47 @@
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Scientific/Engineering :: Visualization",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
-    # Datashader 0.14.4 is not compatible with python 3.11
-    # As soon as a new release is made, we should be able to switch back support for 3.11
-    # "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9"
+python = ">=3.9, <4.0"
 Cartopy = "*"
 datashader = "*"
 geopandas = "*"
 geoviews = "*"
+fiona = ">=1.8"
 holoviews = "*"
-# datashader has fixed the incompatibilities with numpy, but they haven't released a new package
-# As soon as datashader 0.14.5 gets released we should be able to remove the pin
-# https://github.com/holoviz/datashader/issues/1158
-numpy = "<1.24"
+numpy = "*"
 pandas = "*"
-panel = "*"
 shapely = "*"
 xarray = {version = "*", extras = ["io", "accel"]}
 
 [tool.poetry.group.dev.dependencies]
 covdefaults = "*"
 mypy = ">=1"
 pytest = "*"
 pytest-cov = ">=3.0"
 ipykernel = "*"
 ipython = "*"
 nbconvert = "*"
 
+[tool.poetry.group.docs.dependencies]
+mkdocs = "*"
+mkdocs-material = "*"
+mkdocstrings = "*"
+mkdocstrings-python = "*"
+pymdown-extensions = "*"
+black = "*"
+
 [tool.poetry-dynamic-versioning]
 enable = false
 dirty = false
 
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
```

### Comparing `thalassa-0.3.0/thalassa/api.py` & `thalassa-0.3.1/thalassa/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import operator
 import os
 import typing
 import warnings
 from functools import reduce
+from typing import Literal
 
 import geoviews as gv
 import holoviews as hv
 import pandas as pd
 import xarray as xr
 from bokeh.models import HoverTool
 from bokeh.models.formatters import DatetimeTickFormatter
@@ -44,20 +45,22 @@
 
 def open_dataset(
     path: str | os.PathLike[str],
     normalize: bool = True,
     **kwargs: dict[str, typing.Any],
 ) -> xr.Dataset:
     """
-    Open the file specified in ``path`` using ``xarray`` and return an `xr.Dataset``
+    Open the file specified in ``path`` using ``xarray`` and return an ``xr.Dataset``
 
-    If ``normalize`` is ``True``, then the file is converted/normalized to the ``Thalassa`` schema.
-    Normalization is currently only supported for ``SCHISM`` and ``ADCIRC`` netcdf files.
+    Parameters:
+        path: The path to the dataset file (netCDF, zarr, grib)
+        normalize: Boolean flag indicating whether the dataset should be converted/normalized to the ``Thalassa`` schema.
+            Normalization is currently only supported for ``SCHISM`` and ``ADCIRC`` netcdf files.
+        kwargs: The ``kwargs`` are being passed through to ``xr.open_dataset``.
 
-    ``kwargs`` are being passed to ``xr.open_dataset``
     """
     default_kwargs: dict[str, typing.Any] = dict(
         mask_and_scale=True,
         cache=False,
         drop_variables=ADCIRC_VARIABLES_TO_BE_DROPPED,
     )
     with warnings.catch_warnings(record=True):
@@ -73,82 +76,116 @@
         days="%m/%d %H",
         months="%Y/%m/%d",
         years="%Y/%m",
     )
     return dtf
 
 
+MAX: typing.Final = "max"
+MIN: typing.Final = "min"
+
+
 def create_trimesh(
     ds: xr.Dataset,
     variable: str | None = None,
-    timestamp: str | pd.Timestamp | None = None,
+    timestamp: Literal["max", "min"] | pd.Timestamp | None = None,
     layer: int | None = None,
 ) -> gv.TriMesh:
+    """
+    Create a ``gv.TriMesh`` object from the provided dataset.
+
+    Parameters:
+        ds: The dataset containing the variable we want to visualize
+        variable: The data variable we want to visualize
+        timestamp: The timestamp which we want to visualize. It can be ``max``, ``min`` or a specific
+            timestamp. If no ``variable`` is given, then ``timestamp`` is ignored.
+        layer: The "layer" of the ``variable``. It only makes sense in 3D models.
+
+    """
     columns = ["lon", "lat"]
     if variable is not None:
         columns.append(variable)
     if layer is not None:
         ds = ds.isel(layer=layer)
-    if timestamp == "max":
-        points_df = ds[columns].max("time").to_dataframe()
-    elif timestamp == "min":
-        points_df = ds[columns].min("time").to_dataframe()
-    elif timestamp:
-        points_df = ds.sel({"time": timestamp})[columns].to_dataframe().drop(columns="time")
+    if variable and timestamp:
+        if timestamp == "max":
+            points_df = ds[columns].max("time").to_dataframe()
+        elif timestamp == "min":
+            points_df = ds[columns].min("time").to_dataframe()
+        else:
+            points_df = ds.sel({"time": timestamp})[columns].to_dataframe().drop(columns="time")
     else:
+        # Maybe throw an warning if user passed a timestamp but no variable?
         points_df = ds[columns].to_dataframe()
     points_df = points_df.reset_index(drop=True)
     if variable:
         points_gv = gv.Points(points_df, kdims=["lon", "lat"], vdims=[variable])
     else:
         points_gv = gv.Points(points_df, kdims=["lon", "lat"])
-    trimesh = gv.TriMesh((ds.triface_nodes.data, points_gv))
+    trimesh = gv.TriMesh((ds.triface_nodes.data, points_gv), name=variable)
     return trimesh
 
 
-def get_tiles() -> gv.Tiles:
-    tiles = gv.WMTS("http://c.tile.openstreetmap.org/{Z}/{X}/{Y}.png")
+def get_tiles(url: str = "http://c.tile.openstreetmap.org/{Z}/{X}/{Y}.png") -> gv.Tiles:
+    """
+    Return a WMTS using the provided `url`.
+
+    Parameters:
+        url: The URL of the Tiling Service. It defaults to Openstreetmap.
+
+    """
+    tiles = gv.WMTS(url)
     return tiles
 
 
 def get_wireframe(
     trimesh: gv.TriMesh,
     x_range: tuple[float, float] | None = None,
     y_range: tuple[float, float] | None = None,
+    dynamic: bool = True,
 ) -> gv.DynamicMap:
+    """Return a ``DynamicMap`` with a wireframe of the mesh."""
     kwargs = dict(element=trimesh.edgepaths, precompute=True)
     if x_range:
         kwargs["x_range"] = x_range
     if y_range:
         kwargs["y_range"] = y_range
-    wireframe = dynspread(rasterize(**kwargs)).opts(tools=[], cmap=["black"])
+    #wireframe = dynspread(rasterize(**kwargs)).opts(tools=[], cmap=["black"])
+    wireframe = rasterize(**kwargs).opts(tools=[], cmap=["black"], title="Mesh")
+    if dynamic:
+        wireframe = dynspread(wireframe)
     return wireframe
 
 
 def get_raster(
     trimesh: gv.TriMesh,
     title: str = "",
     clabel: str = "",
     clim_min: float | None = None,
     clim_max: float | None = None,
     x_range: tuple[float, float] | None = None,
     y_range: tuple[float, float] | None = None,
 ) -> gv.DynamicMap:
+    """
+    Return a ``DynamicMap`` with a rasterized image of the variable.
+
+    Uses ``datashader`` behind the scenes.
+    """
     kwargs = dict(element=trimesh, precompute=True)
     if x_range:
         kwargs["x_range"] = x_range
     if y_range:
         kwargs["y_range"] = y_range
     logger.debug("rasterize kwargs: %s", kwargs)
     raster = rasterize(**kwargs).opts(
         cmap="viridis",
         clabel=clabel,
         colorbar=True,
         clim=(clim_min, clim_max),
-        title=title,
+        title=title or trimesh.name,
         tools=["hover"],
     )
     return raster
 
 
 def _get_stream_timeseries(
     ds: xr.Dataset,
```

### Comparing `thalassa-0.3.0/thalassa/normalization.py` & `thalassa-0.3.1/thalassa/normalization.py`

 * *Files identical despite different names*

### Comparing `thalassa-0.3.0/thalassa/utils.py` & `thalassa-0.3.1/thalassa/utils.py`

 * *Files identical despite different names*

### Comparing `thalassa-0.3.0/PKG-INFO` & `thalassa-0.3.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 Metadata-Version: 2.1
 Name: thalassa
-Version: 0.3.0
+Version: 0.3.1
 Summary: A library for visualizing large scale results of hydrodynamic simulations
 Home-page: https://github.com/ec-jrc/thalassa.git
 License: EUPL-1.2
 Author: Panos Mavrogiorgos
 Author-email: pmav99@gmail.com
-Requires-Python: >=3.9
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: Cartopy
 Requires-Dist: datashader
+Requires-Dist: fiona (>=1.8)
 Requires-Dist: geopandas
 Requires-Dist: geoviews
 Requires-Dist: holoviews
-Requires-Dist: numpy (<1.24)
+Requires-Dist: numpy
 Requires-Dist: pandas
-Requires-Dist: panel
 Requires-Dist: shapely
 Requires-Dist: xarray[accel,io]
 Project-URL: Repository, https://github.com/ec-jrc/thalassa.git
 Description-Content-Type: text/markdown
 
 Thalassa
 ========
 
+[![Documentation Status](https://readthedocs.org/projects/thalassa/badge/?version=latest)](https://thalassa.readthedocs.io/en/latest/?badge=latest) ![GitHub release (latest by date)](https://img.shields.io/github/v/release/ec-jrc/Thalassa) ![CI](https://github.com/ec-jrc/Thalassa/actions/workflows/run_tests.yml/badge.svg)[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ec-jrc/Thalassa/master?urlpath=lab)
+
 Thalassa ia a library for visualizing unstructured mesh data.
 
 It builds upon [geoviews](https://geoviews.org/) and [datashader](https://datashader.org/)
 and can easily handle meshes with millions of nodes interactively.
 
 <!-- https://user-images.githubusercontent.com/411196/146007390-88e8cc59-9ae9-4a15-83fd-f7f1f2d724c2.mp4 -->
```

