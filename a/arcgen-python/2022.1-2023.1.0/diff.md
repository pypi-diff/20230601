# Comparing `tmp/arcgen-python-2022.1.tar.gz` & `tmp/arcgen-python-2023.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arcgen-python-2022.1.tar", last modified: Mon May  2 13:28:21 2022, max compression
+gzip compressed data, was "arcgen-python-2023.1.0.tar", last modified: Thu Jun  1 01:00:51 2023, max compression
```

## Comparing `arcgen-python-2022.1.tar` & `arcgen-python-2023.1.0.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2022-05-02 13:28:21.506706 arcgen-python-2022.1/
--rw-rw-rw-   0        0        0    35149 2022-04-13 13:11:08.000000 arcgen-python-2022.1/LICENSE
--rw-rw-rw-   0        0        0    15250 2022-05-02 13:28:21.502717 arcgen-python-2022.1/PKG-INFO
--rw-rw-rw-   0        0        0    14287 2022-05-02 13:22:16.000000 arcgen-python-2022.1/README.md
-drwxrwxrwx   0        0        0        0 2022-05-02 13:28:21.484766 arcgen-python-2022.1/arcgen/
--rw-rw-rw-   0        0        0       26 2022-04-27 15:20:22.000000 arcgen-python-2022.1/arcgen/__init__.py
--rw-rw-rw-   0        0        0    58185 2022-05-02 13:10:38.000000 arcgen-python-2022.1/arcgen/arcgen.py
-drwxrwxrwx   0        0        0        0 2022-05-02 13:28:21.485763 arcgen-python-2022.1/arcgen/polygonFunctions/
--rw-rw-rw-   0        0        0      107 2022-04-27 15:20:22.000000 arcgen-python-2022.1/arcgen/polygonFunctions/__init__.py
--rw-rw-rw-   0        0        0     9378 2022-05-02 13:07:48.000000 arcgen-python-2022.1/arcgen/polygonFunctions/polygonFunctions.py
-drwxrwxrwx   0        0        0        0 2022-05-02 13:28:21.487757 arcgen-python-2022.1/arcgen/uniquetol/
--rw-rw-rw-   0        0        0       32 2022-04-27 15:20:22.000000 arcgen-python-2022.1/arcgen/uniquetol/__init__.py
--rw-rw-rw-   0        0        0     3249 2022-05-02 13:07:48.000000 arcgen-python-2022.1/arcgen/uniquetol/uniquetol.py
-drwxrwxrwx   0        0        0        0 2022-05-02 13:28:21.502717 arcgen-python-2022.1/arcgen_python.egg-info/
--rw-rw-rw-   0        0        0    15250 2022-05-02 13:28:21.000000 arcgen-python-2022.1/arcgen_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2022-05-02 13:28:21.000000 arcgen-python-2022.1/arcgen_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-02 13:28:21.000000 arcgen-python-2022.1/arcgen_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2022-05-02 13:28:21.000000 arcgen-python-2022.1/arcgen_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-05-02 13:28:21.000000 arcgen-python-2022.1/arcgen_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-02 13:28:21.506706 arcgen-python-2022.1/setup.cfg
--rw-rw-rw-   0        0        0     1311 2022-05-02 13:21:37.000000 arcgen-python-2022.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:00:51.246017 arcgen-python-2023.1.0/
+-rw-rw-rw-   0        0        0    35149 2022-04-12 22:41:44.000000 arcgen-python-2023.1.0/LICENSE
+-rw-rw-rw-   0        0        0    15330 2023-06-01 01:00:51.245016 arcgen-python-2023.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14385 2023-06-01 00:53:11.000000 arcgen-python-2023.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 01:00:51.210518 arcgen-python-2023.1.0/arcgen/
+-rw-rw-rw-   0        0        0       26 2022-04-27 01:03:20.000000 arcgen-python-2023.1.0/arcgen/__init__.py
+-rw-rw-rw-   0        0        0    58185 2023-05-31 18:20:59.000000 arcgen-python-2023.1.0/arcgen/arcgen.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:00:51.213016 arcgen-python-2023.1.0/arcgen/polygonFunctions/
+-rw-rw-rw-   0        0        0      107 2022-04-27 01:03:20.000000 arcgen-python-2023.1.0/arcgen/polygonFunctions/__init__.py
+-rw-rw-rw-   0        0        0     9495 2023-06-01 00:52:25.000000 arcgen-python-2023.1.0/arcgen/polygonFunctions/polygonFunctions.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:00:51.216019 arcgen-python-2023.1.0/arcgen/uniquetol/
+-rw-rw-rw-   0        0        0       32 2022-04-27 01:03:20.000000 arcgen-python-2023.1.0/arcgen/uniquetol/__init__.py
+-rw-rw-rw-   0        0        0     3249 2022-04-30 00:57:21.000000 arcgen-python-2023.1.0/arcgen/uniquetol/uniquetol.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:00:51.241016 arcgen-python-2023.1.0/arcgen_python.egg-info/
+-rw-rw-rw-   0        0        0    15330 2023-06-01 01:00:51.000000 arcgen-python-2023.1.0/arcgen_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2023-06-01 01:00:51.000000 arcgen-python-2023.1.0/arcgen_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 01:00:51.000000 arcgen-python-2023.1.0/arcgen_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-01 01:00:51.000000 arcgen-python-2023.1.0/arcgen_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-01 01:00:51.000000 arcgen-python-2023.1.0/arcgen_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 01:00:51.246017 arcgen-python-2023.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1313 2023-06-01 00:52:53.000000 arcgen-python-2023.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 01:00:51.244017 arcgen-python-2023.1.0/tests/
+-rw-rw-rw-   0        0        0     7719 2023-06-01 00:52:25.000000 arcgen-python-2023.1.0/tests/test_PolygonFunctions.py
+-rw-rw-rw-   0        0        0     2575 2023-06-01 00:52:25.000000 arcgen-python-2023.1.0/tests/test_uniquetol.py
```

### Comparing `arcgen-python-2022.1/LICENSE` & `arcgen-python-2023.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arcgen-python-2022.1/PKG-INFO` & `arcgen-python-2023.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: arcgen-python
-Version: 2022.1
+Version: 2023.1.0
 Summary: Arc-length Response Corridor Generation
 Home-page: https://github.com/IMMC-UWaterloo/ARCGen-Python
 Author: Devon Hartlen
 Author-email: hartlendc@gmail.com
 License: GPL GNU v3
 Project-URL: Documentation, https://github.com/IMMC-UWaterloo/ARCGen-Python
 Project-URL: Source, https://github.com/IMMC-UWaterloo/ARCGen-Python
 Project-URL: tracker, https://github.com/IMMC-UWaterloo/ARCGen-Python/issues
 Keywords: averaging,statistics,corridors,arc-length,response corridors
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ARCGen-Python - Arc-length Response Corridor Generation
 
-ARCGen-Python is a port of the original [ARCGen for MATLAB] (https://github.com/IMMC-UWaterloo/ARCGen). The python version of ACRGen is not updated as regularly as as MATLAB source code. 
+ARCGen-Python is a port of the original [ARCGen for MATLAB](https://github.com/IMMC-UWaterloo/ARCGen). The python version of ACRGen is not updated as regularly as as MATLAB source code. 
 
 Biofidelity response corridors are commonly used to assess the performance of surrogates such as computational models or anthropomorphic test devices while capturing the variability of experimental data. ARCGen represents a generalized method for computing response corridors and the characteristic average of experimental data capable of accommodating most types of input signals, including experimental data that is time-based, cross-variable, non-monotonic, and/or hysteretic. 
 
 This document provides information on how to use ARCGen as well as a high-level overview of the methodologies that ARCGen uses. Exampels can be found in the 'ExampleCasesAndDatasets' folder. While an overview of ARCGen's operation is provided below, please refer to please refer to [Hartlen and Cronin (2022)](https://www.frontiersin.org/article/10.3389/fbioe.2022.843148) for detailed, rigorous coverage. Examples and datasets provided with this code are taken from Hartlen and Cronin (2022). 
 
 ARCGen-Python is available for Python 3.8 can be installed directly from PyPI as follows. 
 
@@ -141,11 +140,12 @@
 ## Statistical Analysis
 Following arc-length reparameterization, all input signals will have the same number of points at the same normalized arc-length. If signal registration has been performed, the registered points will be used for statistical analysis. Statistical analysis is undertaken in a point-wise fashion at each normalized arc-length. This analysis assumes points are uncorrelated and distributed according to a two-dimensional normal distribution. Based on this assumption, an elliptical confidence region can be constructed at each normalized arc-length. The length of the major and minor axes of these ellipses are proportional to the standard deviation at each arc-length. However, unlike a one-dimensional confidence region, where a plus and minus one standard deviation region will account for 68% of variability, the same two-dimensional elliptical region only accounts for 38%. To control the size of the region based on variance, the quantile function of the chi-squared distribution at the desired variance or p-value can be used to scale the size of the ellipse (optional input option `EllipseKFact`).
 
 The characteristic average of the input signals is defined as the mean value at each normalized arc-length. The response corridors are the envelope of all ellipses. As there is no closed-form way of extracting this envelope, a marching-squares algorithm is used to extract this envelope numerically. Because the envelope is extracted numerically, it is important that the number of resampling points (`nResamplePoints`) are large enough to ensure that ellipses are sufficiently overlapped to provide a smooth, realistic envelope. Similarly, the resolution of the marching squares grid (`CorridorRes`) should be fine enough to capture the shape of the ellipses correctly. This last feature is similar to ensuring that the mesh of a finite element or computational fluid dynamics simulation is fine enough to resolve features. 
 
 # Change Log
 
+## Version 2023.1
+Important fix to `polygonFunction.polyxpoly()` as well as fixes to unit tests. 
+
 ## Version 2022.1
 This is the first production release of ARCGen-Python. There will inevitably be bugs. If you discover any throughout the course of your usage of ARCGen-Python, [please open an issue ticket](https://github.com/IMMC-UWaterloo/ARCGen-Python/issues).
-
-
```

### Comparing `arcgen-python-2022.1/README.md` & `arcgen-python-2023.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ARCGen-Python - Arc-length Response Corridor Generation
 
-ARCGen-Python is a port of the original [ARCGen for MATLAB] (https://github.com/IMMC-UWaterloo/ARCGen). The python version of ACRGen is not updated as regularly as as MATLAB source code. 
+ARCGen-Python is a port of the original [ARCGen for MATLAB](https://github.com/IMMC-UWaterloo/ARCGen). The python version of ACRGen is not updated as regularly as as MATLAB source code. 
 
 Biofidelity response corridors are commonly used to assess the performance of surrogates such as computational models or anthropomorphic test devices while capturing the variability of experimental data. ARCGen represents a generalized method for computing response corridors and the characteristic average of experimental data capable of accommodating most types of input signals, including experimental data that is time-based, cross-variable, non-monotonic, and/or hysteretic. 
 
 This document provides information on how to use ARCGen as well as a high-level overview of the methodologies that ARCGen uses. Exampels can be found in the 'ExampleCasesAndDatasets' folder. While an overview of ARCGen's operation is provided below, please refer to please refer to [Hartlen and Cronin (2022)](https://www.frontiersin.org/article/10.3389/fbioe.2022.843148) for detailed, rigorous coverage. Examples and datasets provided with this code are taken from Hartlen and Cronin (2022). 
 
 ARCGen-Python is available for Python 3.8 can be installed directly from PyPI as follows. 
 
@@ -121,9 +121,12 @@
 ## Statistical Analysis
 Following arc-length reparameterization, all input signals will have the same number of points at the same normalized arc-length. If signal registration has been performed, the registered points will be used for statistical analysis. Statistical analysis is undertaken in a point-wise fashion at each normalized arc-length. This analysis assumes points are uncorrelated and distributed according to a two-dimensional normal distribution. Based on this assumption, an elliptical confidence region can be constructed at each normalized arc-length. The length of the major and minor axes of these ellipses are proportional to the standard deviation at each arc-length. However, unlike a one-dimensional confidence region, where a plus and minus one standard deviation region will account for 68% of variability, the same two-dimensional elliptical region only accounts for 38%. To control the size of the region based on variance, the quantile function of the chi-squared distribution at the desired variance or p-value can be used to scale the size of the ellipse (optional input option `EllipseKFact`).
 
 The characteristic average of the input signals is defined as the mean value at each normalized arc-length. The response corridors are the envelope of all ellipses. As there is no closed-form way of extracting this envelope, a marching-squares algorithm is used to extract this envelope numerically. Because the envelope is extracted numerically, it is important that the number of resampling points (`nResamplePoints`) are large enough to ensure that ellipses are sufficiently overlapped to provide a smooth, realistic envelope. Similarly, the resolution of the marching squares grid (`CorridorRes`) should be fine enough to capture the shape of the ellipses correctly. This last feature is similar to ensuring that the mesh of a finite element or computational fluid dynamics simulation is fine enough to resolve features. 
 
 # Change Log
 
+## Version 2023.1
+Important fix to `polygonFunction.polyxpoly()` as well as fixes to unit tests. 
+
 ## Version 2022.1
 This is the first production release of ARCGen-Python. There will inevitably be bugs. If you discover any throughout the course of your usage of ARCGen-Python, [please open an issue ticket](https://github.com/IMMC-UWaterloo/ARCGen-Python/issues).
```

### Comparing `arcgen-python-2022.1/arcgen/arcgen.py` & `arcgen-python-2023.1.0/arcgen/arcgen.py`

 * *Files identical despite different names*

### Comparing `arcgen-python-2022.1/arcgen/polygonFunctions/polygonFunctions.py` & `arcgen-python-2023.1.0/arcgen/polygonFunctions/polygonFunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -243,14 +243,16 @@
             [-poly1[ind[0],0]],
             [-poly2[ind[1],0]],
             [-poly1[ind[0],1]],
             [-poly2[ind[1],1]],
         ])
         # Solve for both reduced indices and actual intercept locations
         X = np.linalg.solve(A,B)
+        # 2023-05-01 (DCH) Bug with X due to array dims. Flatten ensures vector, not array
+        X = X.flatten()
         # break into indices and locations
         interVals[i,:] = [X[2], X[3]]
         interInds[i,:] = [ind[0]+X[0], ind[1]+X[1]]
 
     return interVals, interInds
```

### Comparing `arcgen-python-2022.1/arcgen/uniquetol/uniquetol.py` & `arcgen-python-2023.1.0/arcgen/uniquetol/uniquetol.py`

 * *Files identical despite different names*

### Comparing `arcgen-python-2022.1/arcgen_python.egg-info/PKG-INFO` & `arcgen-python-2023.1.0/arcgen_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: arcgen-python
-Version: 2022.1
+Version: 2023.1.0
 Summary: Arc-length Response Corridor Generation
 Home-page: https://github.com/IMMC-UWaterloo/ARCGen-Python
 Author: Devon Hartlen
 Author-email: hartlendc@gmail.com
 License: GPL GNU v3
 Project-URL: Documentation, https://github.com/IMMC-UWaterloo/ARCGen-Python
 Project-URL: Source, https://github.com/IMMC-UWaterloo/ARCGen-Python
 Project-URL: tracker, https://github.com/IMMC-UWaterloo/ARCGen-Python/issues
 Keywords: averaging,statistics,corridors,arc-length,response corridors
-Platform: UNKNOWN
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ARCGen-Python - Arc-length Response Corridor Generation
 
-ARCGen-Python is a port of the original [ARCGen for MATLAB] (https://github.com/IMMC-UWaterloo/ARCGen). The python version of ACRGen is not updated as regularly as as MATLAB source code. 
+ARCGen-Python is a port of the original [ARCGen for MATLAB](https://github.com/IMMC-UWaterloo/ARCGen). The python version of ACRGen is not updated as regularly as as MATLAB source code. 
 
 Biofidelity response corridors are commonly used to assess the performance of surrogates such as computational models or anthropomorphic test devices while capturing the variability of experimental data. ARCGen represents a generalized method for computing response corridors and the characteristic average of experimental data capable of accommodating most types of input signals, including experimental data that is time-based, cross-variable, non-monotonic, and/or hysteretic. 
 
 This document provides information on how to use ARCGen as well as a high-level overview of the methodologies that ARCGen uses. Exampels can be found in the 'ExampleCasesAndDatasets' folder. While an overview of ARCGen's operation is provided below, please refer to please refer to [Hartlen and Cronin (2022)](https://www.frontiersin.org/article/10.3389/fbioe.2022.843148) for detailed, rigorous coverage. Examples and datasets provided with this code are taken from Hartlen and Cronin (2022). 
 
 ARCGen-Python is available for Python 3.8 can be installed directly from PyPI as follows. 
 
@@ -141,11 +140,12 @@
 ## Statistical Analysis
 Following arc-length reparameterization, all input signals will have the same number of points at the same normalized arc-length. If signal registration has been performed, the registered points will be used for statistical analysis. Statistical analysis is undertaken in a point-wise fashion at each normalized arc-length. This analysis assumes points are uncorrelated and distributed according to a two-dimensional normal distribution. Based on this assumption, an elliptical confidence region can be constructed at each normalized arc-length. The length of the major and minor axes of these ellipses are proportional to the standard deviation at each arc-length. However, unlike a one-dimensional confidence region, where a plus and minus one standard deviation region will account for 68% of variability, the same two-dimensional elliptical region only accounts for 38%. To control the size of the region based on variance, the quantile function of the chi-squared distribution at the desired variance or p-value can be used to scale the size of the ellipse (optional input option `EllipseKFact`).
 
 The characteristic average of the input signals is defined as the mean value at each normalized arc-length. The response corridors are the envelope of all ellipses. As there is no closed-form way of extracting this envelope, a marching-squares algorithm is used to extract this envelope numerically. Because the envelope is extracted numerically, it is important that the number of resampling points (`nResamplePoints`) are large enough to ensure that ellipses are sufficiently overlapped to provide a smooth, realistic envelope. Similarly, the resolution of the marching squares grid (`CorridorRes`) should be fine enough to capture the shape of the ellipses correctly. This last feature is similar to ensuring that the mesh of a finite element or computational fluid dynamics simulation is fine enough to resolve features. 
 
 # Change Log
 
+## Version 2023.1
+Important fix to `polygonFunction.polyxpoly()` as well as fixes to unit tests. 
+
 ## Version 2022.1
 This is the first production release of ARCGen-Python. There will inevitably be bugs. If you discover any throughout the course of your usage of ARCGen-Python, [please open an issue ticket](https://github.com/IMMC-UWaterloo/ARCGen-Python/issues).
-
-
```

### Comparing `arcgen-python-2022.1/setup.py` & `arcgen-python-2023.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md","r", encoding="utf-8") as fh:
       long_description = fh.read()
 
 setup(name='arcgen-python',
-      version='2022.1',
+      version='2023.1.0',
       description='Arc-length Response Corridor Generation',
       long_description= long_description,
       long_description_content_type="text/markdown",
       author='Devon Hartlen',
       author_email='hartlendc@gmail.com',
       url="https://github.com/IMMC-UWaterloo/ARCGen-Python",
       license='GPL GNU v3',
```

