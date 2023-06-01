# Comparing `tmp/simplegeomap-0.0.26.tar.gz` & `tmp/simplegeomap-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simplegeomap-0.0.26.tar", last modified: Wed May 31 06:15:19 2023, max compression
+gzip compressed data, was "dist/simplegeomap-0.0.27.tar", last modified: Thu Jun  1 06:36:19 2023, max compression
```

## Comparing `simplegeomap-0.0.26.tar` & `simplegeomap-0.0.27.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-31 06:15:19.000000 simplegeomap-0.0.26/
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-31 06:15:19.000000 simplegeomap-0.0.26/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.26/README.md
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-31 06:15:19.000000 simplegeomap-0.0.26/simplegeomap.egg-info/
--rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-05-31 06:15:18.000000 simplegeomap-0.0.26/simplegeomap.egg-info/dependency_links.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-05-31 06:15:18.000000 simplegeomap-0.0.26/simplegeomap.egg-info/PKG-INFO
--rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-05-31 06:15:18.000000 simplegeomap-0.0.26/simplegeomap.egg-info/top_level.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)       51 2023-05-31 06:15:18.000000 simplegeomap-0.0.26/simplegeomap.egg-info/requires.txt
--rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-05-31 06:15:18.000000 simplegeomap-0.0.26/simplegeomap.egg-info/SOURCES.txt
-drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-05-31 06:15:19.000000 simplegeomap-0.0.26/simplegeomap/
--rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.26/simplegeomap/__init__.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     6776 2023-05-30 14:07:40.000000 simplegeomap-0.0.26/simplegeomap/simplegeomap.py
--rw-rw-r--   0 burak     (1000) burak     (1000)     5475 2023-05-31 05:56:26.000000 simplegeomap-0.0.26/simplegeomap/util.py
--rw-rw-r--   0 burak     (1000) burak     (1000)      626 2023-05-31 06:14:35.000000 simplegeomap-0.0.26/setup.py
--rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-05-31 06:15:19.000000 simplegeomap-0.0.26/setup.cfg
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-01 06:36:19.000000 simplegeomap-0.0.27/
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-01 06:36:19.000000 simplegeomap-0.0.27/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)     2189 2023-01-06 09:35:10.000000 simplegeomap-0.0.27/README.md
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-01 06:36:19.000000 simplegeomap-0.0.27/simplegeomap.egg-info/
+-rw-rw-r--   0 burak     (1000) burak     (1000)        1 2023-06-01 06:36:18.000000 simplegeomap-0.0.27/simplegeomap.egg-info/dependency_links.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)     3015 2023-06-01 06:36:18.000000 simplegeomap-0.0.27/simplegeomap.egg-info/PKG-INFO
+-rw-rw-r--   0 burak     (1000) burak     (1000)       13 2023-06-01 06:36:18.000000 simplegeomap-0.0.27/simplegeomap.egg-info/top_level.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)       51 2023-06-01 06:36:18.000000 simplegeomap-0.0.27/simplegeomap.egg-info/requires.txt
+-rw-rw-r--   0 burak     (1000) burak     (1000)      272 2023-06-01 06:36:18.000000 simplegeomap-0.0.27/simplegeomap.egg-info/SOURCES.txt
+drwxrwxr-x   0 burak     (1000) burak     (1000)        0 2023-06-01 06:36:19.000000 simplegeomap-0.0.27/simplegeomap/
+-rw-rw-r--   0 burak     (1000) burak     (1000)       28 2023-02-11 07:38:13.000000 simplegeomap-0.0.27/simplegeomap/__init__.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     6876 2023-05-31 12:04:11.000000 simplegeomap-0.0.27/simplegeomap/simplegeomap.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)     6386 2023-05-31 11:57:38.000000 simplegeomap-0.0.27/simplegeomap/util.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)      626 2023-06-01 06:34:42.000000 simplegeomap-0.0.27/setup.py
+-rw-rw-r--   0 burak     (1000) burak     (1000)       38 2023-06-01 06:36:19.000000 simplegeomap-0.0.27/setup.cfg
```

### Comparing `simplegeomap-0.0.26/PKG-INFO` & `simplegeomap-0.0.27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.26
+Version: 0.0.27
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.26/README.md` & `simplegeomap-0.0.27/README.md`

 * *Files identical despite different names*

### Comparing `simplegeomap-0.0.26/simplegeomap.egg-info/PKG-INFO` & `simplegeomap-0.0.27/simplegeomap.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplegeomap
-Version: 0.0.26
+Version: 0.0.27
 Summary: Simple offline map plot utility, for country borders, elevation, water
 Home-page: https://github.com/burakbayramli/simplegeomap
 Author: Burak Bayramli
 License: UNKNOWN
 Description: # SimpleGeoMap
         
         Given a center latitude, longitude and a zoom level simply plot all
```

### Comparing `simplegeomap-0.0.26/simplegeomap/simplegeomap.py` & `simplegeomap-0.0.27/simplegeomap/simplegeomap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+from simplegeomap.util import gltiles, QuadTreeInterpolator, conv2d, initialize_kernel, padding
 from pygeodesy.sphericalNvector import LatLon
 import pandas as pd, zipfile, sys, os, csv, io
 import matplotlib.pyplot as plt
 import numpy as np, json, shapefile
-from simplegeomap.util import gltiles, QuadTreeInterpolator
 
 GWIDTH = 200
 
 def plot_water_df(df,clat,clon,zoom,ax):
     MAX = 60
     CENTER_DIST = (40000. / MAX)*(zoom+1)
     p1 = LatLon(clat,clon) 
@@ -127,15 +127,16 @@
     interpy = interpy[ridx]
     interpz = interpz[ridx]
 
     q = QuadTreeInterpolator(interpx, interpy, interpz)
     interp = np.vectorize(q.interpolate,otypes=[np.float64])
 
     newx,newy = np.meshgrid(glon,glat)
-    newz = interp(newx,newy)
+    newz = interp(newx,newy)    
+    newz = conv2d(padding(newz),initialize_kernel((3,3),1))
     if not levels:
         CS=plt.contour(newx,newy,newz,cmap=plt.cm.binary,levels=[500,1000,1500,2000,3000])
     else:
         CS=plt.contour(newx,newy,newz,cmap=plt.cm.binary,levels=levels)
     plt.clabel(CS, fontsize=10, inline=1)
     
 def plot_line(regarr,ax,color='black',linestyle='solid'):
```

### Comparing `simplegeomap-0.0.26/simplegeomap/util.py` & `simplegeomap-0.0.27/simplegeomap/util.py`

 * *Files 22% similar despite different names*

```diff
@@ -99,14 +99,38 @@
                 mid = meanOf(latlons)
                 res.append([mid.lat,mid.lon,per,type,geo])
 
     df = pd.DataFrame(res)
     df.columns = ['lat','lon','perimeter','type','polygon']
     df.to_csv('/tmp/lake_river.csv',index=None)
 
+def initialize_kernel(size , sigma): 
+    w, h = size                                                  
+    x = np.linspace(-1,1,w)                         
+    y = np.linspace(-1,1, h)                         
+    x_cor, y_cor  = np.meshgrid(x, y) 
+    kernel = 1/(2*np.pi*np.power(sigma,2) )*\
+             np.exp((- (x_cor ** 2 + y_cor ** 2) )/ 
+             (2*np.power(sigma,2)))
+
+    kernel = kernel/np.sum(kernel) # normalization
+    print(kernel)
+    return kernel
+
+def padding(image):
+    padded_image = np.pad(image , ((1,1),(1,1)) , 'constant',
+                   constant_values=(0,0) ) 
+    return padded_image
+
+def conv2d(image, ftr):                           
+    s = ftr.shape + tuple(np.subtract(image.shape, ftr.shape) + 1)
+    sub_image = np.lib.stride_tricks.as_strided(image, shape = s,
+                strides = image.strides * 2)
+    return np.einsum('ij,ijkl->kl', ftr, sub_image)
+    
 def cdist(p1,p2):    
     distances = np.linalg.norm(p1 - p2, axis=1)
     return distances
 
 class QuadTreeInterpolator:
     def __init__(self, x, y, z):
         self.x = x
```

### Comparing `simplegeomap-0.0.26/setup.py` & `simplegeomap-0.0.27/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 
 readme=open("README.md").read()
 
 setuptools.setup(
     name='simplegeomap',    
-    version='0.0.26',
+    version='0.0.27',
     description="Simple offline map plot utility, for country borders, elevation, water",
     long_description=readme,
     long_description_content_type="text/markdown",    
     install_requires=['pandas','pygeodesy','matplotlib','numpy','pyshp','scipy','zarr'],
     include_package_data=True,
     url="https://github.com/burakbayramli/simplegeomap",
     author="Burak Bayramli",
```

