# Comparing `tmp/ncplot-0.3.2.tar.gz` & `tmp/ncplot-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ncplot-0.3.2.tar", last modified: Mon Apr 24 13:23:58 2023, max compression
+gzip compressed data, was "ncplot-0.3.3.tar", last modified: Thu Jun  1 16:22:48 2023, max compression
```

## Comparing `ncplot-0.3.2.tar` & `ncplot-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:23:58.791739 ncplot-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-24 13:23:41.000000 ncplot-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-24 13:23:41.000000 ncplot-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-24 13:23:58.791739 ncplot-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-04-24 13:23:41.000000 ncplot-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:23:58.787739 ncplot-0.3.2/ncplot/
--rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/command_line.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    34266 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-24 13:23:41.000000 ncplot-0.3.2/ncplot/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 13:23:58.791739 ncplot-0.3.2/ncplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 13:23:58.000000 ncplot-0.3.2/ncplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-24 13:23:41.000000 ncplot-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 13:23:58.791739 ncplot-0.3.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-04-24 13:23:41.000000 ncplot-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:22:48.786610 ncplot-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 16:22:33.000000 ncplot-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-01 16:22:33.000000 ncplot-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-06-01 16:22:48.786610 ncplot-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-06-01 16:22:33.000000 ncplot-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:22:48.786610 ncplot-0.3.3/ncplot/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       29 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/command_line.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35379 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-01 16:22:33.000000 ncplot-0.3.3/ncplot/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:22:48.786610 ncplot-0.3.3/ncplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 16:22:48.000000 ncplot-0.3.3/ncplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 16:22:33.000000 ncplot-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:22:48.786610 ncplot-0.3.3/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1952 2023-06-01 16:22:33.000000 ncplot-0.3.3/setup.py
```

### Comparing `ncplot-0.3.2/LICENSE` & `ncplot-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.2/MANIFEST.in` & `ncplot-0.3.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.2/PKG-INFO` & `ncplot-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ncplot
-Version: 0.3.2
+Version: 0.3.3
 Summary: Interactive viewing of NetCDF data
 Home-page: https://github.com/pmlmodelling/ncplot
 Author: Robert Wilson
 Author-email: rwi@pml.ac.uk
 Maintainer: Robert Wilson
 Project-URL: Bug Tracker, https://github.com/pmlmodelling/ncplot/issues
 Project-URL: Documentation, https://ncplot.readthedocs.io/en/stable
```

### Comparing `ncplot-0.3.2/README.md` & `ncplot-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.2/ncplot/command_line.py` & `ncplot-0.3.3/ncplot/command_line.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.2/ncplot/plot.py` & `ncplot-0.3.3/ncplot/plot.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,21 +147,27 @@
 
 
 def in_notebook(out=None):
     """
     Returns ``True`` if the module is running in IPython kernel,
     ``False`` if in IPython shell or other Python shell.
     """
+    import sys
 
     if out is not None:
         return True
+    if "ipykernel" in sys.modules:
+        return True
 
     if "spyder" in sys.modules:
         return False
 
+    if 'debugpy' in sys.modules:
+        return False
+
     return "ipykernel" in sys.modules
 
 
 def view(x, vars=None, autoscale=True, out=None, **kwargs):
     """
     Plot the contents of a NetCDF out
     Parameters
@@ -173,15 +179,22 @@
 
     out : str
         Name of file if you want to store output
 
     """
 
     if "clim" in kwargs:
-        autoscale = False
+        ignore = False
+
+        if kwargs["clim"][0] < 0:
+            if kwargs["clim"][1] > 0:
+                ignore = True
+
+        if not ignore:
+            autoscale = False
 
     coastline = False
 
     if out is not None:
         if out.endswith(".html") is False:
             raise ValueError("out name must end with html")
 
@@ -499,15 +512,16 @@
         selection = [x for x in df.columns if x in vars or x == x_var]
 
         df = df.loc[:, selection].melt(x_var).drop_duplicates().set_index(x_var)
 
         intplot = df.hvplot(
             groupby="variable",
             dynamic=True,
-            responsive=(in_notebook() is False),
+            #responsive=(in_notebook() is False),
+            responsive = False,
             **kwargs,
         )
         if in_notebook(out):
             if out is None:
                 return intplot
             else:
                 hvplot.save(intplot, out)
@@ -579,14 +593,17 @@
             else:
 
                 if autoscale:
 
                     self_max = ds.rename({vars: "x"}).x.max()
                     self_min = ds.rename({vars: "x"}).x.min()
                     v_max = float(max(self_max.values, -self_min.values))
+                    if "clim" in kwargs:
+                        v_max = float(max(-kwargs["clim"][0], kwargs["clim"][1]))
+
                 else:
                     self_max = 1
                     self_min = 1
 
                 # figure out if it needs to be quadmesh
                 if x_var == time_name:
                     quadmesh = True
@@ -614,25 +631,27 @@
                 if self_max > 0 and self_min < 0:
                     if quadmesh:
                         intplot = ds.hvplot.quadmesh(
                             x_var,
                             y_var,
                             vars,
                             cmap="RdBu_r",
-                            responsive=(in_notebook() is False),
+                            #responsive=(in_notebook() is False),
+                            responsive = False,
                             **kwargs,
                         ).redim.range(**{vars: (-v_max, v_max)})
                     else:
                         intplot = ds.hvplot.image(
                             x_var,
                             y_var,
                             vars,
                             cmap="RdBu_r",
                             rasterize=False,
-                            responsive=(in_notebook() is False),
+                            #responsive=(in_notebook() is False),
+                            responsive = False,
                             **kwargs,
                         ).redim.range(**{vars: (-v_max, v_max)})
 
                 else:
                     if quadmesh:
                         intplot = ds.hvplot.quadmesh(
                             x_var, y_var, vars, cmap="viridis", **kwargs
@@ -803,15 +822,16 @@
             .loc[:, vars]
             .reset_index()
             .melt(time_name)
             .set_index(time_name)
             .hvplot(
                 groupby="variable",
                 dynamic=True,
-                responsive=(in_notebook() is False),
+                #responsive=(in_notebook() is False),
+                responsive = False,
                 **kwargs,
             )
         )
         if in_notebook(out):
             if out is None:
                 return intplot
             else:
@@ -846,15 +866,17 @@
                 lat_name,
                 vars,
                 dynamic=True,
                 cmap="viridis",
                 coastline=coastline,
                 projection=projection,
                 rasterize=rasterize,
-                responsive=in_notebook() is False,
+                #responsive=in_notebook() is False,
+                responsive = False,
+
                 **kwargs,
             )
         else:
 
             if coastline:
                 coastline = get_coastline(ds, lon_name, lat_name)
                 try:
@@ -870,15 +892,16 @@
                 lat_name,
                 vars,
                 dynamic=True,
                 cmap="viridis",
                 coastline=coastline,
                 rasterize=False,
                 projection=projection,
-                responsive=in_notebook() is False,
+                #responsive=in_notebook() is False,
+                responsive = False,
                 **kwargs,
             )
 
         if in_notebook(out):
             if out is None:
                 return intplot
             else:
@@ -898,14 +921,16 @@
             warnings.warn(message="Warning: Only the first variable is mapped")
             vars = vars[0]
 
         if autoscale:
             self_max = ds.rename({vars: "x_dim12345"}).x_dim12345.max()
             self_min = ds.rename({vars: "x_dim12345"}).x_dim12345.min()
             v_max = max(self_max.values, -self_min.values)
+            if "clim" in kwargs:
+                v_max = float(max(-kwargs["clim"][0], kwargs["clim"][1]))
         else:
             self_max = 1
             self_min = 1
 
         if (self_max > 0) and (self_min < 0):
             if quadmesh:
                 if coastline:
@@ -924,28 +949,30 @@
                         lat_name,
                         vars,
                         dynamic=True,
                         cmap="RdBu_r",
                         coastline=coastline,
                         projection=projection,
                         rasterize=rasterize,
-                        responsive=(in_notebook() is False),
+                        #responsive=(in_notebook() is False),
+                        responsive = False,
                         **kwargs,
                     ).redim.range(**{vars: (-v_max, v_max)})
                 else:
                     intplot = ds.hvplot.quadmesh(
                         lon_name,
                         lat_name,
                         vars,
                         dynamic=True,
                         cmap="RdBu_r",
                         coastline=coastline,
                         projection=projection,
                         rasterize=rasterize,
-                        responsive=(in_notebook() is False),
+                        #responsive=(in_notebook() is False),
+                        responsive = False,
                         **kwargs,
                     )
             else:
                 if coastline:
                     coastline = get_coastline(ds, lon_name, lat_name)
                     try:
                         projection = ccrs.PlateCarree()
@@ -961,28 +988,30 @@
                         lat_name,
                         vars,
                         dynamic=True,
                         coastline=coastline,
                         projection=projection,
                         rasterize=False,
                         cmap="RdBu_r",
-                        responsive=(in_notebook() is False),
+                        #responsive=(in_notebook() is False),
+                        responsive = False,
                         **kwargs,
                     ).redim.range(**{vars: (-v_max, v_max)})
                 else:
                     intplot = ds.hvplot.image(
                         lon_name,
                         lat_name,
                         vars,
                         dynamic=True,
                         coastline=coastline,
                         projection=projection,
                         rasterize=False,
                         cmap="RdBu_r",
-                        responsive=(in_notebook() is False),
+                        #responsive=(in_notebook() is False),
+                        responsive = False,
                         **kwargs,
                     )
 
             if in_notebook(out):
                 if out is None:
                     return intplot
                 else:
@@ -1014,28 +1043,30 @@
                         lat_name,
                         vars,
                         dynamic=True,
                         cmap="viridis",
                         coastline=coastline,
                         projection=projection,
                         rasterize=rasterize,
-                        responsive=(in_notebook() is False),
+                        #responsive=(in_notebook() is False),
+                        responsive = False,
                         **kwargs,
                     ).redim.range(**{vars: (self_min.values, v_max)})
                 else:
                     intplot = ds.hvplot.quadmesh(
                         lon_name,
                         lat_name,
                         vars,
                         dynamic=True,
                         cmap="viridis",
                         coastline=coastline,
                         projection=projection,
                         rasterize=rasterize,
-                        responsive=(in_notebook() is False),
+                        #responsive=(in_notebook() is False),
+                        responsive = False,
                         **kwargs,
                     )
 
             else:
 
                 if coastline:
                     coastline = get_coastline(ds, lon_name, lat_name)
@@ -1053,28 +1084,30 @@
                         lat_name,
                         vars,
                         dynamic=True,
                         cmap="viridis",
                         coastline=coastline,
                         rasterize=False,
                         projection=projection,
-                        responsive=(in_notebook() is False),
+                        #responsive=(in_notebook() is False),
+                        responsive = False,
                         **kwargs,
                     ).redim.range(**{vars: (self_min.values, v_max)})
                 else:
                     intplot = ds.hvplot.image(
                         lon_name,
                         lat_name,
                         vars,
                         dynamic=True,
                         cmap="viridis",
                         coastline=coastline,
                         rasterize=False,
                         projection=projection,
-                        responsive=(in_notebook() is False),
+                        #responsive=(in_notebook() is False),
+                        responsive = False,
                         **kwargs,
                     )
 
             if in_notebook(out):
                 if out is None:
                     return intplot
                 else:
```

### Comparing `ncplot-0.3.2/ncplot/utils.py` & `ncplot-0.3.3/ncplot/utils.py`

 * *Files identical despite different names*

### Comparing `ncplot-0.3.2/setup.py` & `ncplot-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         ],
 }
 
 
 extras_require["complete"] = ["geoviews"]
 
 setup(name='ncplot',
-      version='0.3.2',
+      version='0.3.3',
       description=DESCRIPTION,
       long_description=long_description,
       long_description_content_type='text/markdown',
 
       python_requires='>=3.6.1',
 
       entry_points={
```

