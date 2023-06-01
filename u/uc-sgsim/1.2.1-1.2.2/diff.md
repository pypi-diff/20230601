# Comparing `tmp/uc_sgsim-1.2.1.tar.gz` & `tmp/uc_sgsim-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uc_sgsim-1.2.1.tar", last modified: Thu May 25 16:52:04 2023, max compression
+gzip compressed data, was "uc_sgsim-1.2.2.tar", last modified: Thu Jun  1 11:23:58 2023, max compression
```

## Comparing `uc_sgsim-1.2.1.tar` & `uc_sgsim-1.2.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.911213 uc_sgsim-1.2.1/uc_sgsim/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/uc_sgsim/c_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/c_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    85843 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/c_core/uc_sgsim.dll
--rwxr-xr-x   0 runner    (1001) docker     (123)    37024 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/c_core/uc_sgsim.so
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/uc_sgsim/cov_model/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/cov_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/cov_model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/cov_model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/uc_sgsim/krige/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/krige/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/krige/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/krige/kriging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.915214 uc_sgsim-1.2.1/uc_sgsim/plot/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/plot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/plot/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5031 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/plot/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/random_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/sgsim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-25 16:51:51.000000 uc_sgsim-1.2.1/uc_sgsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 16:52:04.911213 uc_sgsim-1.2.1/uc_sgsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-25 16:52:04.000000 uc_sgsim-1.2.1/uc_sgsim.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8095 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-01 11:23:58.067155 uc_sgsim-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim/c_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/c_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84819 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/c_core/uc_sgsim.dll
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37032 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/c_core/uc_sgsim.so
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim/cov_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/cov_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/cov_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/cov_model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim/krige/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/krige/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/krige/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/krige/kriging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/plot/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/plot/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/random_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/sgsim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-01 11:23:41.000000 uc_sgsim-1.2.2/uc_sgsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:23:58.063155 uc_sgsim-1.2.2/uc_sgsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8665 2023-06-01 11:23:58.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-06-01 11:23:58.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:23:58.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:23:57.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 11:23:58.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 11:23:58.000000 uc_sgsim-1.2.2/uc_sgsim.egg-info/top_level.txt
```

### Comparing `uc_sgsim-1.2.1/LICENSE.md` & `uc_sgsim-1.2.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.1/PKG-INFO` & `uc_sgsim-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uc_sgsim
-Version: 1.2.1
+Version: 1.2.2
 Summary: Random Field Generation
 Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
 Author: Zncl2222
 Author-email: 3002shinning@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -98,80 +98,74 @@
 ## Installation
 ```bash
 pip install uc-sgsim
 ```
 
 ## Features
 * One dimensional unconditional randomfield generation with sequential gaussian simulation algorithm
-* Enable to use muti-cores to run the simulation (mutiprocessing)
+* Muti-cores simulation (mutiprocessing)
 * Run C to generate randomfield in python via ctype interface, or just generate randomfield in python with numpy and scipy library.
 
-
-
 ## Example
 ```py
 import matplotlib.pyplot as plt
 import uc_sgsim as uc
 from uc_sgsim.cov_model import Gaussian
 
 if __name__ == '__main__':
     x = 151  # Model grid, only 1D case is support now
+
     bw_s = 1  # lag step
     bw_l = 35  # lag range
-    randomseed = 12321  # randomseed for simulation
-    a = 17.32  # effective range of covariance model
-    C0 = 1  # sill of covariance model
+    randomseed = 151  # randomseed for simulation
+    k_range = 17.32  # effective range of covariance model
+    sill = 1  # sill of covariance model
 
     nR = 10  # numbers of realizations in each CPU cores,
     # if nR = 1 n_process = 8
     # than you will compute total 8 realizations
 
     # Create Covariance model first
-    Cov_model = Gaussian(bw_l, bw_s, a, C0)
+    cov_model = Gaussian(bw_l, bw_s, k_range, sill)
 
     # Create simulation and input the Cov model
-    sgsim = uc.UCSgsim(X, Cov_model, nR)  # Create class instance that generate field in python
-    sgsim_c = uc.UCSgsimDLL(x, Cov_model, nR) # Create class instance that generate field in c
+    sgsim_py = uc.UCSgsim(x, cov_model, nR) # run sgsim with python
+    sgsim_c = uc.UCSgsimDLL(x, cov_model, nR) # run sgsim with c
 
     # Start compute with n CPUs
-    sgsim.compute_async(n_process=8, randomseed=454) # Generate field (python)
-    sgsim_c.compute(n_process=2, randomseed=151) # Generate field (c)
+    sgsim_c.compute(n_process=2, randomseed=randomseed)
+    sgsim_py.compute(n_process=2, randomseed=987654)
 
-    sgsim.mean_plot('ALL')  # Plot mean
-    sgsim.variance_plot()  # Plot variance
-    sgsim.cdf_plot(x_location=10)  # CDF
-    sgsim.hist_plot(x_location=10)  # Hist
-    sgsim.variogram_compute(n_process=2)  # Compute variogram before plotting
+    sgsim_c.mean_plot('ALL')  # Plot mean
+    sgsim_c.variance_plot()  # Plot variance
+    sgsim_c.cdf_plot(x_location=10)  # CDF
+    sgsim_c.hist_plot(x_location=10)  # Hist
+    sgsim_c.variogram_compute(n_process=2)  # Compute variogram before plotting
     # Plot variogram and mean variogram for validation
-    sgsim.vario_plot()
+    sgsim_c.vario_plot()
     # Save random_field and variogram
-    sgsim.save_random_field('randomfield.csv', save_single=True) # save in single file
-    sgsim.save_variogram('') # save each field individually
+    sgsim_c.save_random_field('randomfields.csv', save_single=True)
+    sgsim_c.save_variogram('variograms.csv', save_single=True)
 
-    # plt.show() to show the matplotlib plot
+    # show figure
     plt.show()
-
-    # Please note that the parameter "n_realizations" means the number of realizations calculate in each process,
-    # so this case will generate total 20 * 4(process) = 80 realizations
-
 ```
 
-
 <p align="center">
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Realizations.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Mean.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variance.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variogram.png"  width="50%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/HIST.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/CDF.png"  width="50%"/>
 </p>
 
 ## Future plans
 * 2D unconditional randomfield generation
-* GUI mode in pyhton
+* GUI (pyhton)
 * More covariance models
 * More kriging methods (etc. Oridinary Kriging)
 * Performance enhancement
 * More completely documents and easy to use designs.
 
 ## Performance
 <p align="center">
```

### Comparing `uc_sgsim-1.2.1/README.md` & `uc_sgsim-1.2.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -81,80 +81,74 @@
 ## Installation
 ```bash
 pip install uc-sgsim
 ```
 
 ## Features
 * One dimensional unconditional randomfield generation with sequential gaussian simulation algorithm
-* Enable to use muti-cores to run the simulation (mutiprocessing)
+* Muti-cores simulation (mutiprocessing)
 * Run C to generate randomfield in python via ctype interface, or just generate randomfield in python with numpy and scipy library.
 
-
-
 ## Example
 ```py
 import matplotlib.pyplot as plt
 import uc_sgsim as uc
 from uc_sgsim.cov_model import Gaussian
 
 if __name__ == '__main__':
     x = 151  # Model grid, only 1D case is support now
+
     bw_s = 1  # lag step
     bw_l = 35  # lag range
-    randomseed = 12321  # randomseed for simulation
-    a = 17.32  # effective range of covariance model
-    C0 = 1  # sill of covariance model
+    randomseed = 151  # randomseed for simulation
+    k_range = 17.32  # effective range of covariance model
+    sill = 1  # sill of covariance model
 
     nR = 10  # numbers of realizations in each CPU cores,
     # if nR = 1 n_process = 8
     # than you will compute total 8 realizations
 
     # Create Covariance model first
-    Cov_model = Gaussian(bw_l, bw_s, a, C0)
+    cov_model = Gaussian(bw_l, bw_s, k_range, sill)
 
     # Create simulation and input the Cov model
-    sgsim = uc.UCSgsim(X, Cov_model, nR)  # Create class instance that generate field in python
-    sgsim_c = uc.UCSgsimDLL(x, Cov_model, nR) # Create class instance that generate field in c
+    sgsim_py = uc.UCSgsim(x, cov_model, nR) # run sgsim with python
+    sgsim_c = uc.UCSgsimDLL(x, cov_model, nR) # run sgsim with c
 
     # Start compute with n CPUs
-    sgsim.compute_async(n_process=8, randomseed=454) # Generate field (python)
-    sgsim_c.compute(n_process=2, randomseed=151) # Generate field (c)
+    sgsim_c.compute(n_process=2, randomseed=randomseed)
+    sgsim_py.compute(n_process=2, randomseed=987654)
 
-    sgsim.mean_plot('ALL')  # Plot mean
-    sgsim.variance_plot()  # Plot variance
-    sgsim.cdf_plot(x_location=10)  # CDF
-    sgsim.hist_plot(x_location=10)  # Hist
-    sgsim.variogram_compute(n_process=2)  # Compute variogram before plotting
+    sgsim_c.mean_plot('ALL')  # Plot mean
+    sgsim_c.variance_plot()  # Plot variance
+    sgsim_c.cdf_plot(x_location=10)  # CDF
+    sgsim_c.hist_plot(x_location=10)  # Hist
+    sgsim_c.variogram_compute(n_process=2)  # Compute variogram before plotting
     # Plot variogram and mean variogram for validation
-    sgsim.vario_plot()
+    sgsim_c.vario_plot()
     # Save random_field and variogram
-    sgsim.save_random_field('randomfield.csv', save_single=True) # save in single file
-    sgsim.save_variogram('') # save each field individually
+    sgsim_c.save_random_field('randomfields.csv', save_single=True)
+    sgsim_c.save_variogram('variograms.csv', save_single=True)
 
-    # plt.show() to show the matplotlib plot
+    # show figure
     plt.show()
-
-    # Please note that the parameter "n_realizations" means the number of realizations calculate in each process,
-    # so this case will generate total 20 * 4(process) = 80 realizations
-
 ```
 
-
 <p align="center">
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Realizations.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Mean.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variance.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variogram.png"  width="50%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/HIST.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/CDF.png"  width="50%"/>
 </p>
 
 ## Future plans
 * 2D unconditional randomfield generation
-* GUI mode in pyhton
+* GUI (pyhton)
 * More covariance models
 * More kriging methods (etc. Oridinary Kriging)
 * Performance enhancement
 * More completely documents and easy to use designs.
 
 ## Performance
 <p align="center">
```

### Comparing `uc_sgsim-1.2.1/setup.cfg` & `uc_sgsim-1.2.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = uc_sgsim
-version = 1.2.1
+version = 1.2.2
 description = Random Field Generation
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/Zncl2222/Stochastic_UC_SGSIM
 author = Zncl2222
 author_email = 3002shinning@gmail.com
 license = MIT
```

### Comparing `uc_sgsim-1.2.1/uc_sgsim/c_core/uc_sgsim.dll` & `uc_sgsim-1.2.2/uc_sgsim/c_core/uc_sgsim.dll`

 * *Files 2% similar despite different names*

#### objdump

```diff
@@ -5,20 +5,20 @@
 
 Characteristics 0x2026
 	executable
 	line numbers stripped
 	large address aware
 	DLL
 
-Time/Date		Wed May 24 15:05:26 2023
+Time/Date		Tue May 30 11:42:46 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	2
 MinorLinkerVersion	30
-SizeOfCode		0000000000007000
-SizeOfInitializedData	0000000000009e00
+SizeOfCode		0000000000006c00
+SizeOfInitializedData	0000000000009a00
 SizeOfUninitializedData	0000000000000c00
 AddressOfEntryPoint	0000000000001330
 BaseOfCode		0000000000001000
 ImageBase		00000000646c0000
 SectionAlignment	00001000
 FileAlignment		00000200
 MajorOSystemVersion	4
@@ -26,35 +26,35 @@
 MajorImageVersion	0
 MinorImageVersion	0
 MajorSubsystemVersion	5
 MinorSubsystemVersion	2
 Win32Version		00000000
 SizeOfImage		00019000
 SizeOfHeaders		00000600
-CheckSum		00019925
+CheckSum		000231ee
 Subsystem		00000003	(Windows CUI)
 DllCharacteristics	00000000
 SizeOfStackReserve	0000000000200000
 SizeOfStackCommit	0000000000001000
 SizeOfHeapReserve	0000000000100000
 SizeOfHeapCommit	0000000000001000
 LoaderFlags		00000000
 NumberOfRvaAndSizes	00000010
 
 The Data Directory
-Entry 0 000000000000d000 00000670 Export Directory [.edata (or where ever we found it)]
+Entry 0 000000000000d000 00000674 Export Directory [.edata (or where ever we found it)]
 Entry 1 000000000000e000 00000720 Import Directory [parts of .idata]
 Entry 2 0000000000000000 00000000 Resource Directory [.rsrc]
 Entry 3 000000000000a000 000005b8 Exception Directory [.pdata]
 Entry 4 0000000000000000 00000000 Security Directory
 Entry 5 0000000000011000 00000064 Base Relocation Directory [.reloc]
 Entry 6 0000000000000000 00000000 Debug Directory
 Entry 7 0000000000000000 00000000 Description Directory
 Entry 8 0000000000000000 00000000 Special Directory
-Entry 9 00000000000091c0 00000028 Thread Storage Directory [.tls]
+Entry 9 00000000000091a0 00000028 Thread Storage Directory [.tls]
 Entry a 0000000000000000 00000000 Load Configuration Directory
 Entry b 0000000000000000 00000000 Bound Import Directory
 Entry c 000000000000e1cc 00000190 Import Address Table Directory
 Entry d 0000000000000000 00000000 Delay Import Directory
 Entry e 0000000000000000 00000000 CLR Runtime Header
 Entry f 0000000000000000 00000000 Reserved
 
@@ -124,149 +124,149 @@
  0000e028	00000000 00000000 00000000 00000000 00000000
 
 There is an export table in .edata at 0x646cd000
 
 The Export Tables (interpreted .edata section contents)
 
 Export Flags 			0
-Time/Date stamp 		646e27b6
+Time/Date stamp 		6475e136
 Major/Minor 			0/0
 Name 				000000000000d28a uc_sgsim.dll
 Ordinal Base 			1
 Number in:
 	Export Address Table 		0000003d
 	[Name Pointer/Ordinal] Table	0000003d
 Table Addresses
 	Export Address Table 		000000000000d028
 	Name Pointer Table 		000000000000d11c
 	Ordinal Table 			000000000000d210
 
 Export Address Table -- Ordinal Base 1
-	[   0] +base[   1] 4eb0 Export RVA
-	[   1] +base[   2] 4329 Export RVA
-	[   2] +base[   3] 18e2 Export RVA
-	[   3] +base[   4] 1704 Export RVA
-	[   4] +base[   5] 13b0 Export RVA
-	[   5] +base[   6] 1543 Export RVA
-	[   6] +base[   7] 278e Export RVA
-	[   7] +base[   8] 2752 Export RVA
-	[   8] +base[   9] 26db Export RVA
-	[   9] +base[  10] 2716 Export RVA
-	[  10] +base[  11] 204c Export RVA
-	[  11] +base[  12] 1e54 Export RVA
-	[  12] +base[  13] 1acf Export RVA
-	[  13] +base[  14] 1c7a Export RVA
-	[  14] +base[  15] 264a Export RVA
-	[  15] +base[  16] 25b5 Export RVA
-	[  16] +base[  17] 248d Export RVA
-	[  17] +base[  18] 2520 Export RVA
-	[  18] +base[  19] 28c6 Export RVA
-	[  19] +base[  20] 2868 Export RVA
-	[  20] +base[  21] 27ca Export RVA
-	[  21] +base[  22] 2817 Export RVA
-	[  22] +base[  23] 2401 Export RVA
-	[  23] +base[  24] 2371 Export RVA
-	[  24] +base[  25] 2253 Export RVA
-	[  25] +base[  26] 22e1 Export RVA
-	[  26] +base[  27] 29c8 Export RVA
-	[  27] +base[  28] 296e Export RVA
-	[  28] +base[  29] 292e Export RVA
-	[  29] +base[  30] 294c Export RVA
-	[  30] +base[  31] 2f24 Export RVA
-	[  31] +base[  32] 302e Export RVA
-	[  32] +base[  33] 2ec0 Export RVA
-	[  33] +base[  34] 4381 Export RVA
-	[  34] +base[  35] 38c7 Export RVA
-	[  35] +base[  36] 3a7b Export RVA
-	[  36] +base[  37] 325d Export RVA
-	[  37] +base[  38] 3f98 Export RVA
-	[  38] +base[  39] 3c1a Export RVA
-	[  39] +base[  40] 4490 Export RVA
-	[  40] +base[  41] 2aae Export RVA
-	[  41] +base[  42] 2d5e Export RVA
-	[  42] +base[  43] 2db2 Export RVA
-	[  43] +base[  44] 2caa Export RVA
-	[  44] +base[  45] 2cf4 Export RVA
-	[  45] +base[  46] 2c6d Export RVA
-	[  46] +base[  47] 2a30 Export RVA
-	[  47] +base[  48] 2e27 Export RVA
+	[   0] +base[   1] 4329 Export RVA
+	[   1] +base[   2] 18e2 Export RVA
+	[   2] +base[   3] 1704 Export RVA
+	[   3] +base[   4] 13b0 Export RVA
+	[   4] +base[   5] 1543 Export RVA
+	[   5] +base[   6] 278e Export RVA
+	[   6] +base[   7] 2752 Export RVA
+	[   7] +base[   8] 26db Export RVA
+	[   8] +base[   9] 2716 Export RVA
+	[   9] +base[  10] 204c Export RVA
+	[  10] +base[  11] 1e54 Export RVA
+	[  11] +base[  12] 1acf Export RVA
+	[  12] +base[  13] 1c7a Export RVA
+	[  13] +base[  14] 264a Export RVA
+	[  14] +base[  15] 25b5 Export RVA
+	[  15] +base[  16] 248d Export RVA
+	[  16] +base[  17] 2520 Export RVA
+	[  17] +base[  18] 28c6 Export RVA
+	[  18] +base[  19] 2868 Export RVA
+	[  19] +base[  20] 27ca Export RVA
+	[  20] +base[  21] 2817 Export RVA
+	[  21] +base[  22] 2401 Export RVA
+	[  22] +base[  23] 2371 Export RVA
+	[  23] +base[  24] 2253 Export RVA
+	[  24] +base[  25] 22e1 Export RVA
+	[  25] +base[  26] 29c8 Export RVA
+	[  26] +base[  27] 296e Export RVA
+	[  27] +base[  28] 292e Export RVA
+	[  28] +base[  29] 294c Export RVA
+	[  29] +base[  30] 2f24 Export RVA
+	[  30] +base[  31] 302e Export RVA
+	[  31] +base[  32] 2ec0 Export RVA
+	[  32] +base[  33] 4381 Export RVA
+	[  33] +base[  34] 38c7 Export RVA
+	[  34] +base[  35] 3a7b Export RVA
+	[  35] +base[  36] 325d Export RVA
+	[  36] +base[  37] 3f98 Export RVA
+	[  37] +base[  38] 3c1a Export RVA
+	[  38] +base[  39] 4490 Export RVA
+	[  39] +base[  40] 2aae Export RVA
+	[  40] +base[  41] 2d5e Export RVA
+	[  41] +base[  42] 2db2 Export RVA
+	[  42] +base[  43] 2caa Export RVA
+	[  43] +base[  44] 2cf4 Export RVA
+	[  44] +base[  45] 2c6d Export RVA
+	[  45] +base[  46] 2a30 Export RVA
+	[  46] +base[  47] 2e27 Export RVA
+	[  47] +base[  48] 4d0e Export RVA
 	[  48] +base[  49] 43dd Export RVA
-	[  49] +base[  50] 50b1 Export RVA
+	[  49] +base[  50] 4dd5 Export RVA
 	[  50] +base[  51] 46d0 Export RVA
 	[  51] +base[  52] 3180 Export RVA
 	[  52] +base[  53] 3231 Export RVA
-	[  53] +base[  54] 451d Export RVA
+	[  53] +base[  54] 451f Export RVA
 	[  54] +base[  55] 4780 Export RVA
-	[  55] +base[  56] 47e5 Export RVA
-	[  56] +base[  57] 4c9b Export RVA
+	[  55] +base[  56] 47e6 Export RVA
+	[  56] +base[  57] 4c0a Export RVA
 	[  57] +base[  58] 34b9 Export RVA
-	[  58] +base[  59] 4d20 Export RVA
-	[  59] +base[  60] 539c Export RVA
-	[  60] +base[  61] 5120 Export RVA
+	[  58] +base[  59] 4c90 Export RVA
+	[  59] +base[  60] 50b6 Export RVA
+	[  60] +base[  61] 4e40 Export RVA
 
 [Ordinal/Name Pointer] Table
-	[   0] Partition2d
-	[   1] arange
-	[   2] c_array_max_double
-	[   3] c_array_max_float
-	[   4] c_array_max_int
-	[   5] c_array_max_long_long
-	[   6] c_array_mean_double
-	[   7] c_array_mean_float
-	[   8] c_array_mean_int
-	[   9] c_array_mean_long_long
-	[  10] c_array_min_double
-	[  11] c_array_min_float
-	[  12] c_array_min_int
-	[  13] c_array_min_long_long
-	[  14] c_array_std_double
-	[  15] c_array_std_float
-	[  16] c_array_std_int
-	[  17] c_array_std_long_long
-	[  18] c_array_sum_double
-	[  19] c_array_sum_float
-	[  20] c_array_sum_int
-	[  21] c_array_sum_long
-	[  22] c_array_var_double
-	[  23] c_array_var_float
-	[  24] c_array_var_int
-	[  25] c_array_var_long_long
-	[  26] cmpfunc_double
-	[  27] cmpfunc_float
-	[  28] cmpfunc_int
-	[  29] cmpfunc_long
-	[  30] cov_model
-	[  31] cov_model2d
-	[  32] cov_model_init
-	[  33] d_arange
-	[  34] find_neighbor
-	[  35] krige_memory_free
-	[  36] krige_param_setting
-	[  37] lu_decomposition
-	[  38] lu_inverse_solver
-	[  39] matrixform
-	[  40] mt19937_generate
-	[  41] mt19937_get_double
-	[  42] mt19937_get_double_range
-	[  43] mt19937_get_float
-	[  44] mt19937_get_float_range
-	[  45] mt19937_get_int32_range
-	[  46] mt19937_init
-	[  47] mt19937_random_normal
+	[   0] arange
+	[   1] c_array_max_double
+	[   2] c_array_max_float
+	[   3] c_array_max_int
+	[   4] c_array_max_long_long
+	[   5] c_array_mean_double
+	[   6] c_array_mean_float
+	[   7] c_array_mean_int
+	[   8] c_array_mean_long_long
+	[   9] c_array_min_double
+	[  10] c_array_min_float
+	[  11] c_array_min_int
+	[  12] c_array_min_long_long
+	[  13] c_array_std_double
+	[  14] c_array_std_float
+	[  15] c_array_std_int
+	[  16] c_array_std_long_long
+	[  17] c_array_sum_double
+	[  18] c_array_sum_float
+	[  19] c_array_sum_int
+	[  20] c_array_sum_long
+	[  21] c_array_var_double
+	[  22] c_array_var_float
+	[  23] c_array_var_int
+	[  24] c_array_var_long_long
+	[  25] cmpfunc_double
+	[  26] cmpfunc_float
+	[  27] cmpfunc_int
+	[  28] cmpfunc_long
+	[  29] cov_model
+	[  30] cov_model2d
+	[  31] cov_model_init
+	[  32] d_arange
+	[  33] find_neighbor
+	[  34] krige_memory_free
+	[  35] krige_param_setting
+	[  36] lu_decomposition
+	[  37] lu_inverse_solver
+	[  38] matrixform
+	[  39] mt19937_generate
+	[  40] mt19937_get_double
+	[  41] mt19937_get_double_range
+	[  42] mt19937_get_float
+	[  43] mt19937_get_float_range
+	[  44] mt19937_get_int32_range
+	[  45] mt19937_init
+	[  46] mt19937_random_normal
+	[  47] partition2d
 	[  48] pdist
 	[  49] quicksort2d
 	[  50] randompath
 	[  51] sampling_state_init
 	[  52] sampling_state_update
 	[  53] save_1darray
 	[  54] sgsim_init
 	[  55] sgsim_run
 	[  56] sgsim_t_free
 	[  57] simple_kriging
-	[  58] swap
+	[  58] swaprows
 	[  59] variance
 	[  60] variogram
 
 The Function Table (interpreted .pdata section contents)
 vma:			BeginAddress	 EndAddress	  UnwindData
  00000000646ca000:	00000000646c1000 00000000646c100c 00000000646cb000
  00000000646ca00c:	00000000646c1010 00000000646c11ff 00000000646cb004
@@ -309,91 +309,91 @@
  00000000646ca1c8:	00000000646c2caa 00000000646c2cf4 00000000646cb1a8
  00000000646ca1d4:	00000000646c2cf4 00000000646c2d5e 00000000646cb1b4
  00000000646ca1e0:	00000000646c2d5e 00000000646c2db2 00000000646cb1c0
  00000000646ca1ec:	00000000646c2db2 00000000646c2e27 00000000646cb1cc
  00000000646ca1f8:	00000000646c2e27 00000000646c2eba 00000000646cb1d8
  00000000646ca204:	00000000646c2ec0 00000000646c2f24 00000000646cb1e8
  00000000646ca210:	00000000646c2f24 00000000646c302e 00000000646cb1f0
- 00000000646ca21c:	00000000646c302e 00000000646c317b 00000000646cb1fc
+ 00000000646ca21c:	00000000646c302e 00000000646c317d 00000000646cb1fc
  00000000646ca228:	00000000646c3180 00000000646c3231 00000000646cb208
  00000000646ca234:	00000000646c3231 00000000646c325d 00000000646cb214
  00000000646ca240:	00000000646c325d 00000000646c34b9 00000000646cb21c
  00000000646ca24c:	00000000646c34b9 00000000646c38c7 00000000646cb228
  00000000646ca258:	00000000646c38c7 00000000646c3a7b 00000000646cb238
  00000000646ca264:	00000000646c3a7b 00000000646c3bc5 00000000646cb244
  00000000646ca270:	00000000646c3bd0 00000000646c3c1a 00000000646cb250
  00000000646ca27c:	00000000646c3c1a 00000000646c3f98 00000000646cb25c
  00000000646ca288:	00000000646c3f98 00000000646c4329 00000000646cb26c
  00000000646ca294:	00000000646c4329 00000000646c4381 00000000646cb278
  00000000646ca2a0:	00000000646c4381 00000000646c43dd 00000000646cb284
  00000000646ca2ac:	00000000646c43dd 00000000646c4490 00000000646cb290
- 00000000646ca2b8:	00000000646c4490 00000000646c451d 00000000646cb29c
- 00000000646ca2c4:	00000000646c451d 00000000646c46cb 00000000646cb2a8
+ 00000000646ca2b8:	00000000646c4490 00000000646c451f 00000000646cb29c
+ 00000000646ca2c4:	00000000646c451f 00000000646c46cd 00000000646cb2a8
  00000000646ca2d0:	00000000646c46d0 00000000646c477f 00000000646cb2b4
- 00000000646ca2dc:	00000000646c4780 00000000646c47e5 00000000646cb2c0
- 00000000646ca2e8:	00000000646c47e5 00000000646c4c9b 00000000646cb2cc
- 00000000646ca2f4:	00000000646c4c9b 00000000646c4cbe 00000000646cb2d8
- 00000000646ca300:	00000000646c4cbe 00000000646c4d18 00000000646cb2e4
- 00000000646ca30c:	00000000646c4d20 00000000646c4eb0 00000000646cb2f0
- 00000000646ca318:	00000000646c4eb0 00000000646c50b1 00000000646cb2fc
- 00000000646ca324:	00000000646c50b1 00000000646c5118 00000000646cb308
- 00000000646ca330:	00000000646c5120 00000000646c539c 00000000646cb314
- 00000000646ca33c:	00000000646c539c 00000000646c5484 00000000646cb324
- 00000000646ca348:	00000000646c54a0 00000000646c54d5 00000000646cb330
- 00000000646ca354:	00000000646c54e0 00000000646c5546 00000000646cb338
- 00000000646ca360:	00000000646c5550 00000000646c556f 00000000646cb344
- 00000000646ca36c:	00000000646c5570 00000000646c5646 00000000646cb348
- 00000000646ca378:	00000000646c5650 00000000646c5748 00000000646cb358
- 00000000646ca384:	00000000646c5750 00000000646c577f 00000000646cb368
- 00000000646ca390:	00000000646c5780 00000000646c57f3 00000000646cb370
- 00000000646ca39c:	00000000646c5800 00000000646c5803 00000000646cb37c
- 00000000646ca3a8:	00000000646c5810 00000000646c5814 00000000646cb380
- 00000000646ca3b4:	00000000646c5820 00000000646c5824 00000000646cb384
- 00000000646ca3c0:	00000000646c5830 00000000646c59fd 00000000646cb394
- 00000000646ca3cc:	00000000646c5a00 00000000646c5cbb 00000000646cb3a4
- 00000000646ca3d8:	00000000646c5cc0 00000000646c5e60 00000000646cb3bc
- 00000000646ca3e4:	00000000646c5e60 00000000646c5f4c 00000000646cb3c4
- 00000000646ca3f0:	00000000646c5f50 00000000646c6137 00000000646cb3d4
- 00000000646ca3fc:	00000000646c6140 00000000646c61aa 00000000646cb3dc
- 00000000646ca408:	00000000646c61b0 00000000646c622f 00000000646cb3ec
- 00000000646ca414:	00000000646c6230 00000000646c62d0 00000000646cb3fc
- 00000000646ca420:	00000000646c62d0 00000000646c63aa 00000000646cb404
- 00000000646ca42c:	00000000646c63b0 00000000646c63ce 00000000646cb40c
- 00000000646ca438:	00000000646c63d0 00000000646c63e2 00000000646cb410
- 00000000646ca444:	00000000646c63f0 00000000646c6434 00000000646cb414
- 00000000646ca450:	00000000646c6440 00000000646c64cd 00000000646cb418
- 00000000646ca45c:	00000000646c64d0 00000000646c6544 00000000646cb424
- 00000000646ca468:	00000000646c6550 00000000646c658e 00000000646cb42c
- 00000000646ca474:	00000000646c6590 00000000646c65ff 00000000646cb434
- 00000000646ca480:	00000000646c6600 00000000646c6637 00000000646cb43c
- 00000000646ca48c:	00000000646c6640 00000000646c66d1 00000000646cb444
- 00000000646ca498:	00000000646c66e0 00000000646c6786 00000000646cb44c
- 00000000646ca4a4:	00000000646c6790 00000000646c6793 00000000646cb454
- 00000000646ca4b0:	00000000646c67e0 00000000646c67e6 00000000646cb458
- 00000000646ca4bc:	00000000646c67f0 00000000646c67f6 00000000646cb45c
- 00000000646ca4c8:	00000000646c6800 00000000646c6854 00000000646cb460
- 00000000646ca4d4:	00000000646c6860 00000000646c6986 00000000646cb464
- 00000000646ca4e0:	00000000646c6990 00000000646c6995 00000000646cb470
- 00000000646ca4ec:	00000000646c69a0 00000000646c6a77 00000000646cb474
- 00000000646ca4f8:	00000000646c6a80 00000000646c6b74 00000000646cb478
- 00000000646ca504:	00000000646c6bb0 00000000646c6d94 00000000646cb484
- 00000000646ca510:	00000000646c6da0 00000000646c6ec0 00000000646cb490
- 00000000646ca51c:	00000000646c6ec0 00000000646c6f56 00000000646cb49c
- 00000000646ca528:	00000000646c6f60 00000000646c74b7 00000000646cb4a4
- 00000000646ca534:	00000000646c74c0 00000000646c773e 00000000646cb4c0
- 00000000646ca540:	00000000646c7810 00000000646c78ce 00000000646cb4cc
- 00000000646ca54c:	00000000646c79f0 00000000646c7a15 00000000646cb4d4
- 00000000646ca558:	00000000646c7a20 00000000646c7ae8 00000000646cb4d8
- 00000000646ca564:	00000000646c7af0 00000000646c7b5f 00000000646cb4e8
- 00000000646ca570:	00000000646c7b60 00000000646c7b7f 00000000646cb4f4
- 00000000646ca57c:	00000000646c7c50 00000000646c7c91 00000000646cb4fc
- 00000000646ca588:	00000000646c7ca0 00000000646c7cac 00000000646cb504
- 00000000646ca594:	00000000646c7cb0 00000000646c7dac 00000000646cb508
- 00000000646ca5a0:	00000000646c7dc0 00000000646c7e29 00000000646cb388
- 00000000646ca5ac:	00000000646c7e30 00000000646c7e35 00000000646cb520
+ 00000000646ca2dc:	00000000646c4780 00000000646c47e6 00000000646cb2c0
+ 00000000646ca2e8:	00000000646c47e6 00000000646c4c0a 00000000646cb2cc
+ 00000000646ca2f4:	00000000646c4c0a 00000000646c4c2d 00000000646cb2d8
+ 00000000646ca300:	00000000646c4c2d 00000000646c4c87 00000000646cb2e4
+ 00000000646ca30c:	00000000646c4c90 00000000646c4d0e 00000000646cb2f0
+ 00000000646ca318:	00000000646c4d0e 00000000646c4dd5 00000000646cb2fc
+ 00000000646ca324:	00000000646c4dd5 00000000646c4e39 00000000646cb308
+ 00000000646ca330:	00000000646c4e40 00000000646c50b6 00000000646cb314
+ 00000000646ca33c:	00000000646c50b6 00000000646c519e 00000000646cb324
+ 00000000646ca348:	00000000646c51b0 00000000646c51e5 00000000646cb330
+ 00000000646ca354:	00000000646c51f0 00000000646c5256 00000000646cb338
+ 00000000646ca360:	00000000646c5260 00000000646c527f 00000000646cb344
+ 00000000646ca36c:	00000000646c5280 00000000646c5356 00000000646cb348
+ 00000000646ca378:	00000000646c5360 00000000646c5458 00000000646cb358
+ 00000000646ca384:	00000000646c5460 00000000646c548f 00000000646cb368
+ 00000000646ca390:	00000000646c5490 00000000646c5503 00000000646cb370
+ 00000000646ca39c:	00000000646c5510 00000000646c5513 00000000646cb37c
+ 00000000646ca3a8:	00000000646c5520 00000000646c5524 00000000646cb380
+ 00000000646ca3b4:	00000000646c5530 00000000646c5534 00000000646cb384
+ 00000000646ca3c0:	00000000646c5540 00000000646c570d 00000000646cb394
+ 00000000646ca3cc:	00000000646c5710 00000000646c59cb 00000000646cb3a4
+ 00000000646ca3d8:	00000000646c59d0 00000000646c5b70 00000000646cb3bc
+ 00000000646ca3e4:	00000000646c5b70 00000000646c5c5c 00000000646cb3c4
+ 00000000646ca3f0:	00000000646c5c60 00000000646c5e47 00000000646cb3d4
+ 00000000646ca3fc:	00000000646c5e50 00000000646c5eba 00000000646cb3dc
+ 00000000646ca408:	00000000646c5ec0 00000000646c5f3f 00000000646cb3ec
+ 00000000646ca414:	00000000646c5f40 00000000646c5fe0 00000000646cb3fc
+ 00000000646ca420:	00000000646c5fe0 00000000646c60ba 00000000646cb404
+ 00000000646ca42c:	00000000646c60c0 00000000646c60de 00000000646cb40c
+ 00000000646ca438:	00000000646c60e0 00000000646c60f2 00000000646cb410
+ 00000000646ca444:	00000000646c6100 00000000646c6144 00000000646cb414
+ 00000000646ca450:	00000000646c6150 00000000646c61dd 00000000646cb418
+ 00000000646ca45c:	00000000646c61e0 00000000646c6254 00000000646cb424
+ 00000000646ca468:	00000000646c6260 00000000646c629e 00000000646cb42c
+ 00000000646ca474:	00000000646c62a0 00000000646c630f 00000000646cb434
+ 00000000646ca480:	00000000646c6310 00000000646c6347 00000000646cb43c
+ 00000000646ca48c:	00000000646c6350 00000000646c63e1 00000000646cb444
+ 00000000646ca498:	00000000646c63f0 00000000646c6496 00000000646cb44c
+ 00000000646ca4a4:	00000000646c64a0 00000000646c64a3 00000000646cb454
+ 00000000646ca4b0:	00000000646c64f0 00000000646c64f6 00000000646cb458
+ 00000000646ca4bc:	00000000646c6500 00000000646c6506 00000000646cb45c
+ 00000000646ca4c8:	00000000646c6510 00000000646c6564 00000000646cb460
+ 00000000646ca4d4:	00000000646c6570 00000000646c6696 00000000646cb464
+ 00000000646ca4e0:	00000000646c66a0 00000000646c66a5 00000000646cb470
+ 00000000646ca4ec:	00000000646c66b0 00000000646c6787 00000000646cb474
+ 00000000646ca4f8:	00000000646c6790 00000000646c6884 00000000646cb478
+ 00000000646ca504:	00000000646c68c0 00000000646c6aa4 00000000646cb484
+ 00000000646ca510:	00000000646c6ab0 00000000646c6bd0 00000000646cb490
+ 00000000646ca51c:	00000000646c6bd0 00000000646c6c66 00000000646cb49c
+ 00000000646ca528:	00000000646c6c70 00000000646c71c7 00000000646cb4a4
+ 00000000646ca534:	00000000646c71d0 00000000646c744e 00000000646cb4c0
+ 00000000646ca540:	00000000646c7520 00000000646c75de 00000000646cb4cc
+ 00000000646ca54c:	00000000646c7700 00000000646c7725 00000000646cb4d4
+ 00000000646ca558:	00000000646c7730 00000000646c77f8 00000000646cb4d8
+ 00000000646ca564:	00000000646c7800 00000000646c786f 00000000646cb4e8
+ 00000000646ca570:	00000000646c7870 00000000646c788f 00000000646cb4f4
+ 00000000646ca57c:	00000000646c7960 00000000646c79a1 00000000646cb4fc
+ 00000000646ca588:	00000000646c79b0 00000000646c79bc 00000000646cb504
+ 00000000646ca594:	00000000646c79c0 00000000646c7abc 00000000646cb508
+ 00000000646ca5a0:	00000000646c7ad0 00000000646c7b39 00000000646cb388
+ 00000000646ca5ac:	00000000646c7b40 00000000646c7b45 00000000646cb520
 
 Dump of .xdata
  00000000646cb000 (rva: 0000b000): 00000000646c1000 - 00000000646c100c
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
  00000000646cb004 (rva: 0000b004): 00000000646c1010 - 00000000646c11ff
 	Version: 1, Flags: none
@@ -649,15 +649,15 @@
 	  pc+0x01: push rbp
  00000000646cb1f0 (rva: 0000b1f0): 00000000646c2f24 - 00000000646c302e
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x40
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb1fc (rva: 0000b1fc): 00000000646c302e - 00000000646c317b
+ 00000000646cb1fc (rva: 0000b1fc): 00000000646c302e - 00000000646c317d
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x40
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
  00000000646cb208 (rva: 0000b208): 00000000646c3180 - 00000000646c3231
 	Version: 1, Flags: none
@@ -729,466 +729,466 @@
 	  pc+0x01: push rbp
  00000000646cb290 (rva: 0000b290): 00000000646c43dd - 00000000646c4490
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x10
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb29c (rva: 0000b29c): 00000000646c4490 - 00000000646c451d
+ 00000000646cb29c (rva: 0000b29c): 00000000646c4490 - 00000000646c451f
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x10
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2a8 (rva: 0000b2a8): 00000000646c451d - 00000000646c46cb
+ 00000000646cb2a8 (rva: 0000b2a8): 00000000646c451f - 00000000646c46cd
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x10, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x10: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x08: alloc large area: rsp = rsp - 0x1e0
 	  pc+0x01: push rbp
  00000000646cb2b4 (rva: 0000b2b4): 00000000646c46d0 - 00000000646c477f
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2c0 (rva: 0000b2c0): 00000000646c4780 - 00000000646c47e5
+ 00000000646cb2c0 (rva: 0000b2c0): 00000000646c4780 - 00000000646c47e6
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2cc (rva: 0000b2cc): 00000000646c47e5 - 00000000646c4c9b
+ 00000000646cb2cc (rva: 0000b2cc): 00000000646c47e6 - 00000000646c4c0a
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x10, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x10: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x08: alloc large area: rsp = rsp - 0xa00
 	  pc+0x01: push rbp
- 00000000646cb2d8 (rva: 0000b2d8): 00000000646c4c9b - 00000000646c4cbe
+ 00000000646cb2d8 (rva: 0000b2d8): 00000000646c4c0a - 00000000646c4c2d
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2e4 (rva: 0000b2e4): 00000000646c4cbe - 00000000646c4d18
+ 00000000646cb2e4 (rva: 0000b2e4): 00000000646c4c2d - 00000000646c4c87
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x20
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2f0 (rva: 0000b2f0): 00000000646c4d20 - 00000000646c4eb0
+ 00000000646cb2f0 (rva: 0000b2f0): 00000000646c4c90 - 00000000646c4d0e
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
-	  pc+0x08: alloc small area: rsp = rsp - 0x20
+	  pc+0x08: alloc small area: rsp = rsp - 0x10
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb2fc (rva: 0000b2fc): 00000000646c4eb0 - 00000000646c50b1
+ 00000000646cb2fc (rva: 0000b2fc): 00000000646c4d0e - 00000000646c4dd5
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb308 (rva: 0000b308): 00000000646c50b1 - 00000000646c5118
+ 00000000646cb308 (rva: 0000b308): 00000000646c4dd5 - 00000000646c4e39
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x30
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb314 (rva: 0000b314): 00000000646c5120 - 00000000646c539c
+ 00000000646cb314 (rva: 0000b314): 00000000646c4e40 - 00000000646c50b6
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x11, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x11: FPReg: rbp = rsp + 0x80 (info = 0x0)
-	  pc+0x09: alloc large area: rsp = rsp - 0x88
+	  pc+0x09: alloc large area: rsp = rsp - 0xb8
 	  pc+0x02: push rbx
 	  pc+0x01: push rbp
- 00000000646cb324 (rva: 0000b324): 00000000646c539c - 00000000646c5484
+ 00000000646cb324 (rva: 0000b324): 00000000646c50b6 - 00000000646c519e
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x08, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x08: alloc small area: rsp = rsp - 0x40
 	  pc+0x04: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x01: push rbp
- 00000000646cb330 (rva: 0000b330): 00000000646c54a0 - 00000000646c54d5
+ 00000000646cb330 (rva: 0000b330): 00000000646c51b0 - 00000000646c51e5
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb338 (rva: 0000b338): 00000000646c54e0 - 00000000646c5546
+ 00000000646cb338 (rva: 0000b338): 00000000646c51f0 - 00000000646c5256
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb344 (rva: 0000b344): 00000000646c5550 - 00000000646c556f
+ 00000000646cb344 (rva: 0000b344): 00000000646c5260 - 00000000646c527f
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb348 (rva: 0000b348): 00000000646c5570 - 00000000646c5646
+ 00000000646cb348 (rva: 0000b348): 00000000646c5280 - 00000000646c5356
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x30
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb358 (rva: 0000b358): 00000000646c5650 - 00000000646c5748
+ 00000000646cb358 (rva: 0000b358): 00000000646c5360 - 00000000646c5458
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: rbp
 	  pc+0x0a: alloc small area: rsp = rsp - 0x70
 	  pc+0x06: FPReg: rbp = rsp + 0x0 (info = 0x0)
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rbp
- 00000000646cb368 (rva: 0000b368): 00000000646c5750 - 00000000646c577f
+ 00000000646cb368 (rva: 0000b368): 00000000646c5460 - 00000000646c548f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb370 (rva: 0000b370): 00000000646c5780 - 00000000646c57f3
+ 00000000646cb370 (rva: 0000b370): 00000000646c5490 - 00000000646c5503
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x28
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb37c (rva: 0000b37c): 00000000646c5800 - 00000000646c5803
+ 00000000646cb37c (rva: 0000b37c): 00000000646c5510 - 00000000646c5513
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb380 (rva: 0000b380): 00000000646c5810 - 00000000646c5814
+ 00000000646cb380 (rva: 0000b380): 00000000646c5520 - 00000000646c5524
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb384 (rva: 0000b384): 00000000646c5820 - 00000000646c5824
+ 00000000646cb384 (rva: 0000b384): 00000000646c5530 - 00000000646c5534
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb394 (rva: 0000b394): 00000000646c5830 - 00000000646c59fd
+ 00000000646cb394 (rva: 0000b394): 00000000646c5540 - 00000000646c570d
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x50
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb3a4 (rva: 0000b3a4): 00000000646c5a00 - 00000000646c5cbb
+ 00000000646cb3a4 (rva: 0000b3a4): 00000000646c5710 - 00000000646c59cb
 	Version: 1, Flags: none
 	Nbr codes: 10, Prologue size: 0x18, Frame offset: 0x8, Frame reg: rbp
 	  pc+0x18: FPReg: rbp = rsp + 0x80 (info = 0x0)
 	  pc+0x10: alloc small area: rsp = rsp - 0x38
 	  pc+0x0c: push rbx
 	  pc+0x0b: push rsi
 	  pc+0x0a: push rdi
 	  pc+0x09: push r12
 	  pc+0x07: push r13
 	  pc+0x05: push r14
 	  pc+0x03: push r15
 	  pc+0x01: push rbp
- 00000000646cb3bc (rva: 0000b3bc): 00000000646c5cc0 - 00000000646c5e60
+ 00000000646cb3bc (rva: 0000b3bc): 00000000646c59d0 - 00000000646c5b70
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb3c4 (rva: 0000b3c4): 00000000646c5e60 - 00000000646c5f4c
+ 00000000646cb3c4 (rva: 0000b3c4): 00000000646c5b70 - 00000000646c5c5c
 	Version: 1, Flags: none
 	Nbr codes: 6, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: alloc small area: rsp = rsp - 0x20
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb3d4 (rva: 0000b3d4): 00000000646c5f50 - 00000000646c6137
+ 00000000646cb3d4 (rva: 0000b3d4): 00000000646c5c60 - 00000000646c5e47
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb3dc (rva: 0000b3dc): 00000000646c6140 - 00000000646c61aa
+ 00000000646cb3dc (rva: 0000b3dc): 00000000646c5e50 - 00000000646c5eba
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb3ec (rva: 0000b3ec): 00000000646c61b0 - 00000000646c622f
+ 00000000646cb3ec (rva: 0000b3ec): 00000000646c5ec0 - 00000000646c5f3f
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb3fc (rva: 0000b3fc): 00000000646c6230 - 00000000646c62d0
+ 00000000646cb3fc (rva: 0000b3fc): 00000000646c5f40 - 00000000646c5fe0
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb404 (rva: 0000b404): 00000000646c62d0 - 00000000646c63aa
+ 00000000646cb404 (rva: 0000b404): 00000000646c5fe0 - 00000000646c60ba
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb40c (rva: 0000b40c): 00000000646c63b0 - 00000000646c63ce
+ 00000000646cb40c (rva: 0000b40c): 00000000646c60c0 - 00000000646c60de
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb410 (rva: 0000b410): 00000000646c63d0 - 00000000646c63e2
+ 00000000646cb410 (rva: 0000b410): 00000000646c60e0 - 00000000646c60f2
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb414 (rva: 0000b414): 00000000646c63f0 - 00000000646c6434
+ 00000000646cb414 (rva: 0000b414): 00000000646c6100 - 00000000646c6144
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb418 (rva: 0000b418): 00000000646c6440 - 00000000646c64cd
+ 00000000646cb418 (rva: 0000b418): 00000000646c6150 - 00000000646c61dd
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000000646cb424 (rva: 0000b424): 00000000646c64d0 - 00000000646c6544
+ 00000000646cb424 (rva: 0000b424): 00000000646c61e0 - 00000000646c6254
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb42c (rva: 0000b42c): 00000000646c6550 - 00000000646c658e
+ 00000000646cb42c (rva: 0000b42c): 00000000646c6260 - 00000000646c629e
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb434 (rva: 0000b434): 00000000646c6590 - 00000000646c65ff
+ 00000000646cb434 (rva: 0000b434): 00000000646c62a0 - 00000000646c630f
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb43c (rva: 0000b43c): 00000000646c6600 - 00000000646c6637
+ 00000000646cb43c (rva: 0000b43c): 00000000646c6310 - 00000000646c6347
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb444 (rva: 0000b444): 00000000646c6640 - 00000000646c66d1
+ 00000000646cb444 (rva: 0000b444): 00000000646c6350 - 00000000646c63e1
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb44c (rva: 0000b44c): 00000000646c66e0 - 00000000646c6786
+ 00000000646cb44c (rva: 0000b44c): 00000000646c63f0 - 00000000646c6496
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x28
- 00000000646cb454 (rva: 0000b454): 00000000646c6790 - 00000000646c6793
+ 00000000646cb454 (rva: 0000b454): 00000000646c64a0 - 00000000646c64a3
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb458 (rva: 0000b458): 00000000646c67e0 - 00000000646c67e6
+ 00000000646cb458 (rva: 0000b458): 00000000646c64f0 - 00000000646c64f6
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb45c (rva: 0000b45c): 00000000646c67f0 - 00000000646c67f6
+ 00000000646cb45c (rva: 0000b45c): 00000000646c6500 - 00000000646c6506
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb460 (rva: 0000b460): 00000000646c6800 - 00000000646c6854
+ 00000000646cb460 (rva: 0000b460): 00000000646c6510 - 00000000646c6564
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb464 (rva: 0000b464): 00000000646c6860 - 00000000646c6986
+ 00000000646cb464 (rva: 0000b464): 00000000646c6570 - 00000000646c6696
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x40
 	  pc+0x05: alloc small area: rsp = rsp - 0x50
 	  pc+0x01: push rbx
- 00000000646cb470 (rva: 0000b470): 00000000646c6990 - 00000000646c6995
+ 00000000646cb470 (rva: 0000b470): 00000000646c66a0 - 00000000646c66a5
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb474 (rva: 0000b474): 00000000646c69a0 - 00000000646c6a77
+ 00000000646cb474 (rva: 0000b474): 00000000646c66b0 - 00000000646c6787
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb478 (rva: 0000b478): 00000000646c6a80 - 00000000646c6b74
+ 00000000646cb478 (rva: 0000b478): 00000000646c6790 - 00000000646c6884
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x60
 	  pc+0x05: alloc small area: rsp = rsp - 0x70
 	  pc+0x01: push rbx
- 00000000646cb484 (rva: 0000b484): 00000000646c6bb0 - 00000000646c6d94
+ 00000000646cb484 (rva: 0000b484): 00000000646c68c0 - 00000000646c6aa4
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x40
 	  pc+0x05: alloc small area: rsp = rsp - 0x50
 	  pc+0x01: push rbx
- 00000000646cb490 (rva: 0000b490): 00000000646c6da0 - 00000000646c6ec0
+ 00000000646cb490 (rva: 0000b490): 00000000646c6ab0 - 00000000646c6bd0
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x0a, Frame offset: 0x0, Frame reg: none
 	  pc+0x0a: save xmm6 at rsp + 0x60
 	  pc+0x05: alloc small area: rsp = rsp - 0x70
 	  pc+0x01: push rbx
- 00000000646cb49c (rva: 0000b49c): 00000000646c6ec0 - 00000000646c6f56
+ 00000000646cb49c (rva: 0000b49c): 00000000646c6bd0 - 00000000646c6c66
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x18
- 00000000646cb4a4 (rva: 0000b4a4): 00000000646c6f60 - 00000000646c74b7
+ 00000000646cb4a4 (rva: 0000b4a4): 00000000646c6c70 - 00000000646c71c7
 	Version: 1, Flags: none
 	Nbr codes: 11, Prologue size: 0x1a, Frame offset: 0x0, Frame reg: none
 	  pc+0x1a: save xmm7 at rsp + 0x80
 	  pc+0x12: save xmm6 at rsp + 0x70
 	  pc+0x0d: alloc large area: rsp = rsp - 0x90
 	  pc+0x06: push rbx
 	  pc+0x05: push rsi
 	  pc+0x04: push rdi
 	  pc+0x03: push rbp
 	  pc+0x02: push r12
- 00000000646cb4c0 (rva: 0000b4c0): 00000000646c74c0 - 00000000646c773e
+ 00000000646cb4c0 (rva: 0000b4c0): 00000000646c71d0 - 00000000646c744e
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x09, Frame offset: 0x0, Frame reg: none
 	  pc+0x09: save xmm6 at rsp + 0x40
 	  pc+0x04: alloc small area: rsp = rsp - 0x58
- 00000000646cb4cc (rva: 0000b4cc): 00000000646c7810 - 00000000646c78ce
+ 00000000646cb4cc (rva: 0000b4cc): 00000000646c7520 - 00000000646c75de
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x30
 	  pc+0x01: push rbx
- 00000000646cb4d4 (rva: 0000b4d4): 00000000646c79f0 - 00000000646c7a15
+ 00000000646cb4d4 (rva: 0000b4d4): 00000000646c7700 - 00000000646c7725
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb4d8 (rva: 0000b4d8): 00000000646c7a20 - 00000000646c7ae8
+ 00000000646cb4d8 (rva: 0000b4d8): 00000000646c7730 - 00000000646c77f8
 	Version: 1, Flags: none
 	Nbr codes: 5, Prologue size: 0x08, Frame offset: 0x0, Frame reg: none
 	  pc+0x08: alloc small area: rsp = rsp - 0x28
 	  pc+0x04: push rbx
 	  pc+0x03: push rsi
 	  pc+0x02: push rdi
 	  pc+0x01: push rbp
- 00000000646cb4e8 (rva: 0000b4e8): 00000000646c7af0 - 00000000646c7b5f
+ 00000000646cb4e8 (rva: 0000b4e8): 00000000646c7800 - 00000000646c786f
 	Version: 1, Flags: none
 	Nbr codes: 4, Prologue size: 0x07, Frame offset: 0x0, Frame reg: none
 	  pc+0x07: alloc small area: rsp = rsp - 0x20
 	  pc+0x03: push rbx
 	  pc+0x02: push rsi
 	  pc+0x01: push rdi
- 00000000646cb4f4 (rva: 0000b4f4): 00000000646c7b60 - 00000000646c7b7f
+ 00000000646cb4f4 (rva: 0000b4f4): 00000000646c7870 - 00000000646c788f
 	Version: 1, Flags: none
 	Nbr codes: 2, Prologue size: 0x05, Frame offset: 0x0, Frame reg: none
 	  pc+0x05: alloc small area: rsp = rsp - 0x20
 	  pc+0x01: push rbx
- 00000000646cb4fc (rva: 0000b4fc): 00000000646c7c50 - 00000000646c7c91
+ 00000000646cb4fc (rva: 0000b4fc): 00000000646c7960 - 00000000646c79a1
 	Version: 1, Flags: none
 	Nbr codes: 1, Prologue size: 0x04, Frame offset: 0x0, Frame reg: none
 	  pc+0x04: alloc small area: rsp = rsp - 0x58
- 00000000646cb504 (rva: 0000b504): 00000000646c7ca0 - 00000000646c7cac
+ 00000000646cb504 (rva: 0000b504): 00000000646c79b0 - 00000000646c79bc
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
- 00000000646cb508 (rva: 0000b508): 00000000646c7cb0 - 00000000646c7dac
+ 00000000646cb508 (rva: 0000b508): 00000000646c79c0 - 00000000646c7abc
 	Version: 1, Flags: none
 	Nbr codes: 9, Prologue size: 0x16, Frame offset: 0x0, Frame reg: none
 	  pc+0x16: save xmm8 at rsp + 0x60
 	  pc+0x10: save xmm7 at rsp + 0x50
 	  pc+0x0b: save xmm6 at rsp + 0x40
 	  pc+0x06: alloc small area: rsp = rsp - 0x78
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb388 (rva: 0000b388): 00000000646c7dc0 - 00000000646c7e29
+ 00000000646cb388 (rva: 0000b388): 00000000646c7ad0 - 00000000646c7b39
 	Version: 1, Flags: none
 	Nbr codes: 3, Prologue size: 0x06, Frame offset: 0x0, Frame reg: none
 	  pc+0x06: alloc small area: rsp = rsp - 0x38
 	  pc+0x02: push rbx
 	  pc+0x01: push rsi
- 00000000646cb520 (rva: 0000b520): 00000000646c7e30 - 00000000646c7e35
+ 00000000646cb520 (rva: 0000b520): 00000000646c7b40 - 00000000646c7b45
 	Version: 1, Flags: none
 	Nbr codes: 0, Prologue size: 0x00, Frame offset: 0x0, Frame reg: none
 
 
 PE File Base Relocations (interpreted .reloc section contents)
 
 Virtual Address: 00007000 Chunk size 12 (0xc) Number of fixups 2
-	reloc    0 offset  e48 [7e48] DIR64
+	reloc    0 offset  b58 [7b58] DIR64
 	reloc    1 offset    0 [7000] ABSOLUTE
 
 Virtual Address: 00008000 Chunk size 20 (0x14) Number of fixups 6
 	reloc    0 offset    0 [8000] DIR64
 	reloc    1 offset   50 [8050] DIR64
 	reloc    2 offset   58 [8058] DIR64
 	reloc    3 offset   60 [8060] DIR64
 	reloc    4 offset   70 [8070] DIR64
 	reloc    5 offset    0 [8000] ABSOLUTE
 
 Virtual Address: 00009000 Chunk size 52 (0x34) Number of fixups 22
-	reloc    0 offset  180 [9180] DIR64
-	reloc    1 offset  188 [9188] DIR64
-	reloc    2 offset  1a0 [91a0] DIR64
-	reloc    3 offset  1c0 [91c0] DIR64
-	reloc    4 offset  1c8 [91c8] DIR64
-	reloc    5 offset  1d0 [91d0] DIR64
-	reloc    6 offset  1d8 [91d8] DIR64
-	reloc    7 offset  5e0 [95e0] DIR64
-	reloc    8 offset  5f0 [95f0] DIR64
-	reloc    9 offset  600 [9600] DIR64
-	reloc   10 offset  610 [9610] DIR64
-	reloc   11 offset  620 [9620] DIR64
-	reloc   12 offset  630 [9630] DIR64
-	reloc   13 offset  640 [9640] DIR64
-	reloc   14 offset  650 [9650] DIR64
-	reloc   15 offset  660 [9660] DIR64
-	reloc   16 offset  670 [9670] DIR64
-	reloc   17 offset  680 [9680] DIR64
-	reloc   18 offset  690 [9690] DIR64
-	reloc   19 offset  6a0 [96a0] DIR64
-	reloc   20 offset  6b0 [96b0] DIR64
+	reloc    0 offset  170 [9170] DIR64
+	reloc    1 offset  178 [9178] DIR64
+	reloc    2 offset  180 [9180] DIR64
+	reloc    3 offset  1a0 [91a0] DIR64
+	reloc    4 offset  1a8 [91a8] DIR64
+	reloc    5 offset  1b0 [91b0] DIR64
+	reloc    6 offset  1b8 [91b8] DIR64
+	reloc    7 offset  5c0 [95c0] DIR64
+	reloc    8 offset  5d0 [95d0] DIR64
+	reloc    9 offset  5e0 [95e0] DIR64
+	reloc   10 offset  5f0 [95f0] DIR64
+	reloc   11 offset  600 [9600] DIR64
+	reloc   12 offset  610 [9610] DIR64
+	reloc   13 offset  620 [9620] DIR64
+	reloc   14 offset  630 [9630] DIR64
+	reloc   15 offset  640 [9640] DIR64
+	reloc   16 offset  650 [9650] DIR64
+	reloc   17 offset  660 [9660] DIR64
+	reloc   18 offset  670 [9670] DIR64
+	reloc   19 offset  680 [9680] DIR64
+	reloc   20 offset  690 [9690] DIR64
 	reloc   21 offset    0 [9000] ABSOLUTE
 
 Virtual Address: 0000f000 Chunk size 16 (0x10) Number of fixups 4
 	reloc    0 offset   18 [f018] DIR64
 	reloc    1 offset   30 [f030] DIR64
 	reloc    2 offset   38 [f038] DIR64
 	reloc    3 offset    0 [f000] ABSOLUTE
 
 Sections:
 Idx Name          Size      VMA               LMA               File off  Algn
-  0 .text         00006e68  00000000646c1000  00000000646c1000  00000600  2**4
+  0 .text         00006b78  00000000646c1000  00000000646c1000  00000600  2**4
                   CONTENTS, ALLOC, LOAD, READONLY, CODE, DATA
-  1 .data         000000a0  00000000646c8000  00000000646c8000  00007600  2**4
+  1 .data         000000a0  00000000646c8000  00000000646c8000  00007200  2**4
                   CONTENTS, ALLOC, LOAD, DATA
-  2 .rdata        00000900  00000000646c9000  00000000646c9000  00007800  2**5
+  2 .rdata        000008e0  00000000646c9000  00000000646c9000  00007400  2**5
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  3 .pdata        000005b8  00000000646ca000  00000000646ca000  00008200  2**2
+  3 .pdata        000005b8  00000000646ca000  00000000646ca000  00007e00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  4 .xdata        00000524  00000000646cb000  00000000646cb000  00008800  2**2
+  4 .xdata        00000524  00000000646cb000  00000000646cb000  00008400  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
   5 .bss          00000b90  00000000646cc000  00000000646cc000  00000000  2**5
                   ALLOC
-  6 .edata        00000670  00000000646cd000  00000000646cd000  00008e00  2**2
+  6 .edata        00000674  00000000646cd000  00000000646cd000  00008a00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
-  7 .idata        00000720  00000000646ce000  00000000646ce000  00009600  2**2
+  7 .idata        00000720  00000000646ce000  00000000646ce000  00009200  2**2
                   CONTENTS, ALLOC, LOAD, DATA
-  8 .CRT          00000058  00000000646cf000  00000000646cf000  00009e00  2**3
+  8 .CRT          00000058  00000000646cf000  00000000646cf000  00009a00  2**3
                   CONTENTS, ALLOC, LOAD, DATA
-  9 .tls          00000010  00000000646d0000  00000000646d0000  0000a000  2**3
+  9 .tls          00000010  00000000646d0000  00000000646d0000  00009c00  2**3
                   CONTENTS, ALLOC, LOAD, DATA
- 10 .reloc        00000064  00000000646d1000  00000000646d1000  0000a200  2**2
+ 10 .reloc        00000064  00000000646d1000  00000000646d1000  00009e00  2**2
                   CONTENTS, ALLOC, LOAD, READONLY, DATA
- 11 .debug_aranges 00000050  00000000646d2000  00000000646d2000  0000a400  2**4
+ 11 .debug_aranges 00000050  00000000646d2000  00000000646d2000  0000a000  2**4
                   CONTENTS, READONLY, DEBUGGING
- 12 .debug_info   00001f08  00000000646d3000  00000000646d3000  0000a600  2**0
+ 12 .debug_info   00001f08  00000000646d3000  00000000646d3000  0000a200  2**0
                   CONTENTS, READONLY, DEBUGGING
- 13 .debug_abbrev 00000149  00000000646d5000  00000000646d5000  0000c600  2**0
+ 13 .debug_abbrev 00000149  00000000646d5000  00000000646d5000  0000c200  2**0
                   CONTENTS, READONLY, DEBUGGING
- 14 .debug_line   00000222  00000000646d6000  00000000646d6000  0000c800  2**0
+ 14 .debug_line   00000222  00000000646d6000  00000000646d6000  0000c400  2**0
                   CONTENTS, READONLY, DEBUGGING
- 15 .debug_frame  00000048  00000000646d7000  00000000646d7000  0000cc00  2**3
+ 15 .debug_frame  00000048  00000000646d7000  00000000646d7000  0000c800  2**3
                   CONTENTS, READONLY, DEBUGGING
- 16 .debug_str    0000009b  00000000646d8000  00000000646d8000  0000ce00  2**0
+ 16 .debug_str    0000009b  00000000646d8000  00000000646d8000  0000ca00  2**0
                   CONTENTS, READONLY, DEBUGGING
 SYMBOL TABLE:
 [  0](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000028 crtdll.c
 File 
 [  2](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000000000 pre_c_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [  4](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 atexit_table
 [  5](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000010 _CRT_INIT
 [  6](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000018 __proc_attached
-[  7](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000650 .rdata$.refptr.__native_startup_lock
+[  7](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000630 .rdata$.refptr.__native_startup_lock
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[  9](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000660 .rdata$.refptr.__native_startup_state
+[  9](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000640 .rdata$.refptr.__native_startup_state
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[ 11](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000620 .rdata$.refptr.__dyn_tls_init_callback
+[ 11](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000600 .rdata$.refptr.__dyn_tls_init_callback
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[ 13](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006a0 .rdata$.refptr.__xi_z
+[ 13](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000680 .rdata$.refptr.__xi_z
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[ 15](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000690 .rdata$.refptr.__xi_a
+[ 15](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000670 .rdata$.refptr.__xi_a
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[ 17](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000680 .rdata$.refptr.__xc_z
+[ 17](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000660 .rdata$.refptr.__xc_z
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[ 19](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000670 .rdata$.refptr.__xc_a
+[ 19](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000650 .rdata$.refptr.__xc_a
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [ 21](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000000200 __DllMainCRTStartup
-[ 22](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000640 .rdata$.refptr.__native_dllmain_reason
+[ 22](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000620 .rdata$.refptr.__native_dllmain_reason
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [ 24](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000330 DllMainCRTStartup
-[ 25](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006b0 .rdata$.refptr.mingw_app_type
+[ 25](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000690 .rdata$.refptr.mingw_app_type
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [ 27](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000000380 atexit
 [ 28](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .text
 AUX scnlen 0x38f nreloc 39 nlnno 0
 [ 30](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [ 32](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .bss
@@ -1253,15 +1253,15 @@
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [ 92](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000003c .xdata
 AUX scnlen 0x148 nreloc 0 nlnno 0
 [ 94](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000054 .pdata
 AUX scnlen 0x150 nreloc 84 nlnno 0
 [ 96](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
-[ 98](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006c0 .rdata$zzz
+[ 98](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006a0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [100](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000007d c_array_mt.c
 File 
 [102](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001a30 mt19937_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [104](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001aae mt19937_generate
 [105](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001c6d mt19937_get_int32_range
@@ -1278,35 +1278,35 @@
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [117](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000184 .xdata
 AUX scnlen 0x64 nreloc 0 nlnno 0
 [119](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001a4 .pdata
 AUX scnlen 0x60 nreloc 24 nlnno 0
 [121](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .rdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
-[123](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000700 .rdata$zzz
+[123](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000006e0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [125](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000091 cov_model.c
 File 
 [127](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000001ec0 cov_model_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [129](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000001f24 cov_model
 [130](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000202e cov_model2d
 [131](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000001ec0 .text
-AUX scnlen 0x2bb nreloc 6 nlnno 0
+AUX scnlen 0x2bd nreloc 6 nlnno 0
 [133](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [135](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [137](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001e8 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [139](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000204 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [141](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .rdata
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[143](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000740 .rdata$zzz
+[143](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000720 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [145](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000b6 krige.c
 File 
 [147](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000020 model
 [148](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000028 k_range
 [149](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000030 estimation
 [150](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000038 krige_var
@@ -1335,40 +1335,40 @@
 AUX scnlen 0x148 nreloc 0 nlnno 0
 [174](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000208 .xdata
 AUX scnlen 0x48 nreloc 0 nlnno 0
 [176](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000228 .pdata
 AUX scnlen 0x48 nreloc 18 nlnno 0
 [178](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000060 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
-[180](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000780 .rdata$zzz
+[180](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000760 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [182](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000cf matrix_tools.c
 File 
 [184](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000002bd0 snprintf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [186](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002c1a lu_inverse_solver
 [187](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000002f98 lu_decomposition
 [188](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003329 arange
 [189](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003381 d_arange
 [190](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000033dd pdist
 [191](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003490 matrixform
-[192](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000351d save_1darray
+[192](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000351f save_1darray
 [193](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000002bd0 .text
-AUX scnlen 0xafb nreloc 28 nlnno 0
+AUX scnlen 0xafd nreloc 28 nlnno 0
 [195](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [197](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000170 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [199](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000250 .xdata
 AUX scnlen 0x64 nreloc 0 nlnno 0
 [201](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000270 .pdata
 AUX scnlen 0x60 nreloc 24 nlnno 0
 [203](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000090 .rdata
 AUX scnlen 0x70 nreloc 0 nlnno 0
-[205](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007c0 .rdata$zzz
+[205](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007a0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [207](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000df random_tools.c
 File 
 [209](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000036d0 randompath
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [211](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000036d0 .text
 AUX scnlen 0xaf nreloc 1 nlnno 0
@@ -1376,194 +1376,194 @@
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [215](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000170 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [217](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002b4 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [219](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002d0 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[221](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000800 .rdata$zzz
+[221](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000007e0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [223](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000000fc sgsim.c
 File 
 [225](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000180 x_grid
 [226](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a0 u_array
 [227](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001c0 sampled
 [228](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e0 variogram_array
 [229](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000200 sgsim_array
 [230](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000220 _sampling
 [231](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000268 flag
 [232](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000026c count
 [233](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003780 sgsim_init
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[235](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000037e5 sgsim_run
-[236](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003c9b sgsim_t_free
-[237](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000003cbe sgsim_memory_free
+[235](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000037e6 sgsim_run
+[236](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003c0a sgsim_t_free
+[237](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000003c2d sgsim_memory_free
 [238](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003780 .text
-AUX scnlen 0x598 nreloc 82 nlnno 0
+AUX scnlen 0x507 nreloc 76 nlnno 0
 [240](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [242](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000180 .bss
 AUX scnlen 0xf0 nreloc 0 nlnno 0
 [244](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002c0 .xdata
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [246](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002dc .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
 [248](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000100 .rdata
-AUX scnlen 0x58 nreloc 0 nlnno 0
-[250](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000840 .rdata$zzz
+AUX scnlen 0x4e nreloc 0 nlnno 0
+[250](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000820 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [252](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000010e sort_tools.c
 File 
-[254](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003d20 swap
+[254](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003c90 swaprows
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[256](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003eb0 Partition2d
-[257](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000040b1 quicksort2d
-[258](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003d20 .text
-AUX scnlen 0x3f8 nreloc 0 nlnno 0
+[256](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003d0e partition2d
+[257](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000003dd5 quicksort2d
+[258](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003c90 .text
+AUX scnlen 0x1a9 nreloc 0 nlnno 0
 [260](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [262](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [264](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002f0 .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
 [266](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000030c .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[268](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000880 .rdata$zzz
+[268](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000860 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
 [270](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000128 variogram.c
 File 
-[272](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004120 variogram
+[272](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000003e40 variogram
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[274](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x000000000000439c variance
-[275](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004120 .text
-AUX scnlen 0x364 nreloc 13 nlnno 0
+[274](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000040b6 variance
+[275](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000003e40 .text
+AUX scnlen 0x35e nreloc 11 nlnno 0
 [277](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [279](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [281](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000314 .xdata
 AUX scnlen 0x1c nreloc 0 nlnno 0
 [283](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000330 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[285](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000160 .rdata
+[285](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000150 .rdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
-[287](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000008c0 .rdata$zzz
+[287](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000008a0 .rdata$zzz
 AUX scnlen 0x3f nreloc 0 nlnno 0
-[289](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000004490 .text
+[289](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000041a0 .text
 [290](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 .data
 [291](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 .bss
 [292](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000684 .idata$7
 [293](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000024c .idata$5
 [294](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000bc .idata$4
 [295](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ca .idata$6
 [296](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000136 fake
 File 
 [298](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c hname
 [299](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc fthunk
-[300](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000044a0 .text
+[300](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000041b0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [302](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [304](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [306](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
 [308](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
 [309](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
 [310](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000144 fake
 File 
-[312](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000044a0 .text
+[312](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000041b0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [314](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [316](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [318](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000000ec .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [320](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000027c .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [322](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000069c .idata$7
 AUX scnlen 0xd nreloc 0 nlnno 0
 [324](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000158 gccmain.c
 File 
-[326](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000044a0 __do_global_dtors
+[326](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000041b0 __do_global_dtors
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [328](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000000 p.93846
-[329](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000044e0 __do_global_ctors
-[330](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005f0 .rdata$.refptr.__CTOR_LIST__
+[329](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000041f0 __do_global_ctors
+[330](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005d0 .rdata$.refptr.__CTOR_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[332](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004550 __main
+[332](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004260 __main
 [333](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000280 initialized
-[334](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000044a0 .text
+[334](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000041b0 .text
 AUX scnlen 0xcf nreloc 7 nlnno 0
 [336](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [338](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000280 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [340](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000330 .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
 [342](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000348 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [344](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000160 natstart.c
 File 
-[346](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004570 .text
+[346](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004280 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [348](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .data
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [350](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000290 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [352](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000178 gs_support.c
 File 
-[354](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004570 __security_init_cookie
+[354](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004280 __security_init_cookie
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [356](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data$__security_cookie
 AUX scnlen 0x8 nreloc 0 nlnno 0 checksum 0x0 assoc 0 comdat 3
 [358](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000090 .data$__security_cookie_complement
 AUX scnlen 0x8 nreloc 0 nlnno 0 checksum 0x0 assoc 0 comdat 3
-[360](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004650 __report_gsfailure
+[360](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004360 __report_gsfailure
 [361](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a0 GS_ContextRecord
 [362](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000780 GS_ExceptionRecord
-[363](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000180 GS_ExceptionPointers
-[364](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004570 .text
+[363](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000170 GS_ExceptionPointers
+[364](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004280 .text
 AUX scnlen 0x1d8 nreloc 29 nlnno 0
 [366](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [368](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002a0 .bss
 AUX scnlen 0x578 nreloc 0 nlnno 0
 [370](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000348 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [372](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000036c .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[374](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000180 .rdata
+[374](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000170 .rdata
 AUX scnlen 0x10 nreloc 2 nlnno 0
 [376](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000019e tlssup.c
 File 
-[378](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000004750 __dyn_tls_dtor
+[378](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000004460 __dyn_tls_dtor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[380](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004780 __dyn_tls_init
-[381](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005e0 .rdata$.refptr._CRT_MT
+[380](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004490 __dyn_tls_init
+[381](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005c0 .rdata$.refptr._CRT_MT
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
 [383](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000048 __xd_a
 [384](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 __xd_z
-[385](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004800 __tlregdtor
-[386](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004750 .text
+[385](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004510 __tlregdtor
+[386](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004460 .text
 AUX scnlen 0xb3 nreloc 5 nlnno 0
 [388](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [390](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000820 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
 [392](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000368 .xdata
 AUX scnlen 0x18 nreloc 0 nlnno 0
 [394](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000384 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [396](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000038 .CRT$XLD
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [398](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .CRT$XLC
 AUX scnlen 0x8 nreloc 1 nlnno 0
-[400](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001a0 .rdata
+[400](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000180 .rdata
 AUX scnlen 0x48 nreloc 5 nlnno 0
 [402](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .CRT$XDZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [404](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000048 .CRT$XDA
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [406](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000040 .CRT$XLZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
@@ -1571,15 +1571,15 @@
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [410](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .tls$ZZZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [412](sec 10)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .tls
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [414](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001ae cinitexe.c
 File 
-[416](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004810 .text
+[416](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004520 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [418](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [420](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000830 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [422](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000008 .CRT$XCZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
@@ -1587,146 +1587,146 @@
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [426](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .CRT$XIZ
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [428](sec  9)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000010 .CRT$XIA
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [430](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001bd mingw_helpers.c
 File 
-[432](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004810 _decode_pointer
+[432](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004520 _decode_pointer
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[434](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004820 _encode_pointer
-[435](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004810 .text
+[434](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004530 _encode_pointer
+[435](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004520 .text
 AUX scnlen 0x14 nreloc 0 nlnno 0
 [437](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [439](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000830 .bss
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [441](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000380 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [443](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a8 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
 [445](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001de pseudo-reloc.c
 File 
-[447](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006dc0 __report_error
+[447](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006ad0 __report_error
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[449](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000004830 __write_memory.part.0
+[449](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 0) 0x0000000000004540 __write_memory.part.0
 [450](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000844 maxSections
 [451](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000848 the_secs
-[452](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004a00 _pei386_runtime_relocator
+[452](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004710 _pei386_runtime_relocator
 [453](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000840 was_init.95174
-[454](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000600 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
+[454](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005e0 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[456](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000610 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST__
+[456](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005f0 .rdata$.refptr.__RUNTIME_PSEUDO_RELOC_LIST__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[458](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000630 .rdata$.refptr.__image_base__
+[458](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000610 .rdata$.refptr.__image_base__
 AUX scnlen 0x8 nreloc 1 nlnno 0 checksum 0x0 assoc 0 comdat 2
-[460](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004830 .text
+[460](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004540 .text
 AUX scnlen 0x48b nreloc 36 nlnno 0
 [462](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [464](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000840 .bss
 AUX scnlen 0x10 nreloc 0 nlnno 0
-[466](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000200 .rdata
+[466](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001e0 .rdata
 AUX scnlen 0x102 nreloc 0 nlnno 0
-[468](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006dc0 .text.unlikely
+[468](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ad0 .text.unlikely
 AUX scnlen 0x69 nreloc 6 nlnno 0
 [470](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000388 .xdata.unlikely
 AUX scnlen 0xc nreloc 0 nlnno 0
 [472](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003c0 .pdata.unlikely
 AUX scnlen 0xc nreloc 3 nlnno 0
 [474](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000394 .xdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
 [476](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003cc .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
 [478](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000001f3 crt_handler.c
 File 
-[480](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000004cc0 __mingw_SEH_error_handler
+[480](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000049d0 __mingw_SEH_error_handler
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[482](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004e60 __mingw_init_ehandler
+[482](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004b70 __mingw_init_ehandler
 [483](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000868 was_here.95013
 [484](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000980 emu_pdata
 [485](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000880 emu_xdata
-[486](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004f50 _gnu_exception_handler
-[487](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004cc0 .text
+[486](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004c60 _gnu_exception_handler
+[487](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000049d0 .text
 AUX scnlen 0x477 nreloc 29 nlnno 0
 [489](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [491](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000860 .bss
 AUX scnlen 0x2a0 nreloc 0 nlnno 0
 [493](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003bc .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [495](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003e4 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[497](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000310 .rdata
+[497](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000002f0 .rdata
 AUX scnlen 0x7 nreloc 0 nlnno 0
 [499](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000207 tlsthrd.c
 File 
-[501](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005140 __mingwthr_run_key_dtors.part.0
+[501](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000004e50 __mingwthr_run_key_dtors.part.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [503](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b20 __mingwthr_cs
 [504](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b00 key_dtor_list
-[505](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000051b0 ___w64_mingwthr_add_key_dtor
+[505](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004ec0 ___w64_mingwthr_add_key_dtor
 [506](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b08 __mingwthr_cs_init
-[507](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005230 ___w64_mingwthr_remove_key_dtor
-[508](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000052d0 __mingw_TLScallback
-[509](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005140 .text
+[507](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004f40 ___w64_mingwthr_remove_key_dtor
+[508](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000004fe0 __mingw_TLScallback
+[509](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000004e50 .text
 AUX scnlen 0x26a nreloc 39 nlnno 0
 [511](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [513](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b00 .bss
 AUX scnlen 0x48 nreloc 0 nlnno 0
 [515](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003dc .xdata
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [517](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000408 .pdata
 AUX scnlen 0x30 nreloc 12 nlnno 0
 [519](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000020f tlsmcrt.c
 File 
-[521](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000053b0 .text
+[521](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000050c0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [523](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000020 .data
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [525](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b60 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [527](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000217 pseudo-reloc-list.c
 File 
-[529](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000053b0 .text
+[529](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000050c0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [531](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [533](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b60 .bss
 AUX scnlen 0x2 nreloc 0 nlnno 0
 [535](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000022e pesect.c
 File 
-[537](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000053b0 _ValidateImageBase.part.0
+[537](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x00000000000050c0 _ValidateImageBase.part.0
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[539](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000053d0 _ValidateImageBase
-[540](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000053f0 _FindPESection
-[541](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005440 _FindPESectionByName
-[542](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000054d0 __mingw_GetSectionForAddress
-[543](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005550 __mingw_GetSectionCount
-[544](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005590 _FindPESectionExec
-[545](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005600 _GetPEImageBase
-[546](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005640 _IsNonwritableInCurrentImage
-[547](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000056e0 __mingw_enum_import_library_names
-[548](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000053b0 .text
+[539](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000050e0 _ValidateImageBase
+[540](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005100 _FindPESection
+[541](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005150 _FindPESectionByName
+[542](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000051e0 __mingw_GetSectionForAddress
+[543](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005260 __mingw_GetSectionCount
+[544](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000052a0 _FindPESectionExec
+[545](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005310 _GetPEImageBase
+[546](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005350 _IsNonwritableInCurrentImage
+[547](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000053f0 __mingw_enum_import_library_names
+[548](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000050c0 .text
 AUX scnlen 0x3d6 nreloc 9 nlnno 0
 [550](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [552](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [554](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000040c .xdata
 AUX scnlen 0x48 nreloc 0 nlnno 0
 [556](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000438 .pdata
 AUX scnlen 0x78 nreloc 30 nlnno 0
 [558](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000023d CRT_fp10.c
 File 
-[560](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005790 _fpreset
+[560](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000054a0 _fpreset
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[562](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005790 fpreset
-[563](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005790 .text
+[562](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000054a0 fpreset
+[563](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054a0 .text
 AUX scnlen 0x3 nreloc 0 nlnno 0
 [565](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [567](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [569](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000454 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
@@ -1736,29 +1736,29 @@
 File 
 [575](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_info
 AUX scnlen 0x2e nreloc 7 nlnno 0
 [577](sec 14)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_abbrev
 AUX scnlen 0x14 nreloc 0 nlnno 0
 [579](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_line
 AUX scnlen 0x7b nreloc 1 nlnno 0
-[581](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000057a0 .text
+[581](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054b0 .text
 AUX scnlen 0x32 nreloc 0 nlnno 0
 [583](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [585](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [587](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_aranges
 AUX scnlen 0x30 nreloc 2 nlnno 0
 [589](sec 17)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_str
 AUX scnlen 0x9b nreloc 0 nlnno 0
 [591](sec 16)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000000 .debug_frame
 AUX scnlen 0x48 nreloc 2 nlnno 0
 [593](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000261 libgcc2.c
 File 
-[595](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000057e0 .text
+[595](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054f0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [597](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [599](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [601](sec 13)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000002e .debug_info
 AUX scnlen 0x1eda nreloc 4 nlnno 0
@@ -1766,874 +1766,874 @@
 AUX scnlen 0x135 nreloc 0 nlnno 0
 [605](sec 12)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .debug_aranges
 AUX scnlen 0x20 nreloc 1 nlnno 0
 [607](sec 15)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000007b .debug_line
 AUX scnlen 0x1a7 nreloc 0 nlnno 0
 [609](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000026f dllentry.c
 File 
-[611](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000057e0 DllEntryPoint
+[611](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000054f0 DllEntryPoint
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[613](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000057e0 .text
+[613](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000054f0 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
 [615](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [617](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [619](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000458 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [621](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004bc .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [623](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000027d dllmain.c
 File 
-[625](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000057f0 DllMain
+[625](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005500 DllMain
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[627](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000057f0 .text
+[627](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005500 .text
 AUX scnlen 0x6 nreloc 0 nlnno 0
 [629](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [631](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [633](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000045c .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [635](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c8 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [637](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000028b fpclassify.c
 File 
-[639](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005800 __fpclassify
+[639](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005510 __fpclassify
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[641](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005800 .text
+[641](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005510 .text
 AUX scnlen 0x54 nreloc 0 nlnno 0
 [643](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [645](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [647](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000460 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [649](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d4 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [651](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000029b sqrt.c
 File 
-[653](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005860 sqrt
+[653](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005570 sqrt
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[655](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005860 .text
+[655](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005570 .text
 AUX scnlen 0x126 nreloc 10 nlnno 0
 [657](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [659](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[661](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000320 .rdata
+[661](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000300 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
 [663](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000464 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [665](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004e0 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [667](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002a9 vsnprintf.c
 File 
-[669](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005990 __ms_vsnprintf
+[669](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000056a0 __ms_vsnprintf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[671](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005990 .text
+[671](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000056a0 .text
 AUX scnlen 0x5 nreloc 1 nlnno 0
 [673](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [675](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [677](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000470 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [679](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004ec .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [681](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002c2 ceil.S
 File 
-[683](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000059a0 ceil
+[683](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000056b0 ceil
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[685](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a60 .is_intnaninf
-[686](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a70 .ret_org
-[687](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a20 .signed_val
-[688](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000350 .huge
-[689](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000358 .zero
-[690](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a11 .doret
-[691](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a0b .l1
-[692](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a50 .doret2
-[693](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005a72 .ret_naninf
-[694](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000059a0 .text
+[685](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005770 .is_intnaninf
+[686](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005780 .ret_org
+[687](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005730 .signed_val
+[688](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000330 .huge
+[689](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000338 .zero
+[690](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005721 .doret
+[691](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x000000000000571b .l1
+[692](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005760 .doret2
+[693](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x0000000000005782 .ret_naninf
+[694](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000056b0 .text
 AUX scnlen 0xd7 nreloc 4 nlnno 0
 [696](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [698](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [700](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000474 .xdata
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [702](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f8 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
-[704](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000350 .rdata
+[704](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000330 .rdata
 AUX scnlen 0x10 nreloc 0 nlnno 0
 [706](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002d2 cos.c
 File 
-[708](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005a80 cos
+[708](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005790 cos
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[710](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005a80 .text
+[710](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005790 .text
 AUX scnlen 0xf4 nreloc 8 nlnno 0
 [712](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [714](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[716](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000360 .rdata
+[716](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000340 .rdata
 AUX scnlen 0x10 nreloc 0 nlnno 0
 [718](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000478 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [720](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000504 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [722](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002dc cosl_internal.S
 File 
-[724](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005b80 __cosl_internal
+[724](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005890 __cosl_internal
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[726](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005b80 .text
+[726](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005890 .text
 AUX scnlen 0x30 nreloc 0 nlnno 0
 [728](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [730](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [732](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002ee exp.c
 File 
-[734](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005bb0 exp
+[734](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000058c0 exp
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [736](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000040 c0
 [737](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000030 c1
-[738](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005bb0 .text
+[738](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000058c0 .text
 AUX scnlen 0x1e4 nreloc 17 nlnno 0
 [740](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000030 .data
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [742](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[744](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000370 .rdata
+[744](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000350 .rdata
 AUX scnlen 0x28 nreloc 0 nlnno 0
 [746](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000484 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [748](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000510 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [750](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000002fe log.c
 File 
-[752](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005da0 log
+[752](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000005ab0 log
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[754](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005da0 .text
+[754](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005ab0 .text
 AUX scnlen 0x120 nreloc 11 nlnno 0
 [756](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [758](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[760](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .rdata
+[760](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000380 .rdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [762](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000490 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [764](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000051c .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [766](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000030f pow.c
 File 
-[768](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005ec0 internal_modf
+[768](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000005bd0 internal_modf
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[770](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005f60 pow
-[771](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005ec0 .text
+[770](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000005c70 pow
+[771](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000005bd0 .text
 AUX scnlen 0x5f7 nreloc 31 nlnno 0
 [773](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [775](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [777](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000049c .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
 [779](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000528 .pdata
 AUX scnlen 0x18 nreloc 6 nlnno 0
-[781](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003c0 .rdata
+[781](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000003a0 .rdata
 AUX scnlen 0x80 nreloc 0 nlnno 0
 [783](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000031f powi.c
 File 
-[785](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000064c0 __powi
+[785](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000061d0 __powi
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[787](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000064c0 .text
+[787](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000061d0 .text
 AUX scnlen 0x27e nreloc 15 nlnno 0
 [789](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [791](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[793](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000440 .rdata
+[793](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000420 .rdata
 AUX scnlen 0x60 nreloc 0 nlnno 0
 [795](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004c0 .xdata
 AUX scnlen 0xc nreloc 0 nlnno 0
 [797](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000540 .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [799](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000329 exp2l.S
 File 
-[801](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006740 exp2l
+[801](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006450 exp2l
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[803](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006740 .text
+[803](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006450 .text
 AUX scnlen 0x68 nreloc 0 nlnno 0
 [805](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [807](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [809](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000335 internal_logl.S
 File 
-[811](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000067b0 one
-[812](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000067b8 limit
-[813](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000067c0 __logl_internal
+[811](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000064c0 one
+[812](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000064c8 limit
+[813](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000064d0 __logl_internal
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[815](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000067b0 .text
+[815](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000064c0 .text
 AUX scnlen 0x51 nreloc 0 nlnno 0
 [817](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [819](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [821](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000343 ldexp.c
 File 
-[823](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006810 ldexp
+[823](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006520 ldexp
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[825](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006810 .text
+[825](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006520 .text
 AUX scnlen 0xbe nreloc 1 nlnno 0
 [827](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [829](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [831](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004cc .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [833](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000054c .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [835](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003e2 log2l.S
 File 
-[837](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000068d0 one
-[838](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000068d8 limit
-[839](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000068e0 log2l
+[837](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000065e0 one
+[838](sec  1)(fl 0x00)(ty    0)(scl   6) (nx 0) 0x00000000000065e8 limit
+[839](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000065f0 log2l
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[841](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000068d0 .text
+[841](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000065e0 .text
 AUX scnlen 0x6c nreloc 0 nlnno 0
 [843](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [845](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[847](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006940 .text
+[847](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006650 .text
 [848](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [849](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [850](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000710 .idata$7
 [851](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000034c .idata$5
 [852](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001bc .idata$4
 [853](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000638 .idata$6
-[854](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006948 .text
+[854](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006658 .text
 [855](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [856](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [857](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000070c .idata$7
 [858](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000344 .idata$5
 [859](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001b4 .idata$4
 [860](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000062e .idata$6
-[861](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006950 .text
+[861](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006660 .text
 [862](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [863](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [864](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000708 .idata$7
 [865](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000033c .idata$5
 [866](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ac .idata$4
 [867](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000624 .idata$6
-[868](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006958 .text
+[868](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006668 .text
 [869](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [870](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [871](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000704 .idata$7
 [872](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000334 .idata$5
 [873](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001a4 .idata$4
 [874](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000061a .idata$6
-[875](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006960 .text
+[875](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006670 .text
 [876](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [877](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [878](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006fc .idata$7
 [879](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000324 .idata$5
 [880](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000194 .idata$4
 [881](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000606 .idata$6
-[882](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006968 .text
+[882](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006678 .text
 [883](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [884](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [885](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f8 .idata$7
 [886](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000031c .idata$5
 [887](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000018c .idata$4
 [888](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005fc .idata$6
-[889](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006970 .text
+[889](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006680 .text
 [890](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [891](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [892](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f4 .idata$7
 [893](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000314 .idata$5
 [894](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000184 .idata$4
 [895](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005f2 .idata$6
-[896](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006978 .text
+[896](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006688 .text
 [897](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [898](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [899](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006f0 .idata$7
 [900](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000030c .idata$5
 [901](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000017c .idata$4
 [902](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ea .idata$6
-[903](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006980 .text
+[903](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006690 .text
 [904](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [905](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [906](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ec .idata$7
 [907](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000304 .idata$5
 [908](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000174 .idata$4
 [909](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005e0 .idata$6
-[910](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006988 .text
+[910](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006698 .text
 [911](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [912](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [913](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e8 .idata$7
 [914](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002fc .idata$5
 [915](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000016c .idata$4
 [916](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005d8 .idata$6
-[917](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006990 .text
+[917](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066a0 .text
 [918](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [919](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [920](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e4 .idata$7
 [921](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002f4 .idata$5
 [922](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000164 .idata$4
 [923](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005ce .idata$6
-[924](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006998 .text
+[924](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066a8 .text
 [925](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [926](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [927](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006e0 .idata$7
 [928](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ec .idata$5
 [929](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000015c .idata$4
 [930](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005c6 .idata$6
-[931](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069a0 .text
+[931](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066b0 .text
 [932](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [933](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [934](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006dc .idata$7
 [935](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002e4 .idata$5
 [936](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000154 .idata$4
 [937](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005bc .idata$6
-[938](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069a8 .text
+[938](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066b8 .text
 [939](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [940](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [941](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d8 .idata$7
 [942](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002dc .idata$5
 [943](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000014c .idata$4
 [944](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005b4 .idata$6
-[945](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069b0 .text
+[945](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066c0 .text
 [946](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [947](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [948](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d4 .idata$7
 [949](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002d4 .idata$5
 [950](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000144 .idata$4
 [951](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005aa .idata$6
-[952](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069b8 .text
+[952](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066c8 .text
 [953](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [954](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [955](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006d0 .idata$7
 [956](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002cc .idata$5
 [957](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000013c .idata$4
 [958](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000005a2 .idata$6
-[959](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069c0 .text
+[959](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066d0 .text
 [960](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [961](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [962](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006cc .idata$7
 [963](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002c4 .idata$5
 [964](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000134 .idata$4
 [965](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000594 .idata$6
-[966](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069c8 .text
+[966](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066d8 .text
 [967](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [968](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [969](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c4 .idata$7
 [970](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002b4 .idata$5
 [971](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000124 .idata$4
 [972](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000580 .idata$6
-[973](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069d0 .text
+[973](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066e0 .text
 [974](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [975](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [976](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006bc .idata$7
 [977](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002a4 .idata$5
 [978](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000114 .idata$4
 [979](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000056c .idata$6
-[980](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069d8 .text
+[980](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066e8 .text
 [981](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [982](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [983](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b8 .idata$7
 [984](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000029c .idata$5
 [985](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000010c .idata$4
 [986](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000562 .idata$6
-[987](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000069e0 .text
+[987](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000066f0 .text
 [988](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000050 .data
 [989](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [990](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b4 .idata$7
 [991](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000294 .idata$5
 [992](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000104 .idata$4
 [993](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000554 .idata$6
 [994](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000003f2 onexit_table.c
 File 
-[996](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x00000000000069f0 _initialize_onexit_table
+[996](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006700 _initialize_onexit_table
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[998](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006a20 _register_onexit_function
-[999](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006af0 _execute_onexit_table
-[1000](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000069f0 .text
+[998](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006730 _register_onexit_function
+[999](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006800 _execute_onexit_table
+[1000](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006700 .text
 AUX scnlen 0x16f nreloc 8 nlnno 0
 [1002](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000050 .data
 AUX scnlen 0x18 nreloc 3 nlnno 0
 [1004](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1006](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004d4 .xdata
 AUX scnlen 0x20 nreloc 0 nlnno 0
 [1008](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000558 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
 [1010](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x0000000000000400 acrt_iob_func.c
 File 
-[1012](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006b60 __acrt_iob_func
+[1012](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006870 __acrt_iob_func
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1014](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b60 .text
+[1014](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006870 .text
 AUX scnlen 0x1f nreloc 1 nlnno 0
 [1016](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000070 .data
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [1018](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1020](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004f4 .xdata
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [1022](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x000000000000057c .pdata
 AUX scnlen 0xc nreloc 3 nlnno 0
 [1024](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x000000000000042a fake
 File 
 [1026](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 hname
 [1027](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 fthunk
-[1028](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b80 .text
+[1028](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006890 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1030](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1032](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1034](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000014 .idata$2
 AUX scnlen 0x14 nreloc 3 nlnno 0
 [1036](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
 [1037](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
-[1038](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b80 .text
+[1038](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006890 .text
 [1039](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1040](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1041](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000700 .idata$7
 [1042](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000032c .idata$5
 [1043](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000019c .idata$4
 [1044](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000610 .idata$6
-[1045](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b88 .text
+[1045](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006898 .text
 [1046](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1047](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1048](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c8 .idata$7
 [1049](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002bc .idata$5
 [1050](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000012c .idata$4
 [1051](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000058a .idata$6
-[1052](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b90 .text
+[1052](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068a0 .text
 [1053](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1054](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1055](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006c0 .idata$7
 [1056](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000002ac .idata$5
 [1057](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000011c .idata$4
 [1058](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000578 .idata$6
-[1059](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006b98 .text
+[1059](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068a8 .text
 [1060](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1061](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1062](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006ac .idata$7
 [1063](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000284 .idata$5
 [1064](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000f4 .idata$4
 [1065](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000532 .idata$6
 [1066](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004cb fake
 File 
-[1068](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ba0 .text
+[1068](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000068b0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1070](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1072](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1074](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000001c4 .idata$4
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [1076](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000354 .idata$5
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [1078](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000714 .idata$7
 AUX scnlen 0xb nreloc 0 nlnno 0
-[1080](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ba0 .text
+[1080](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068b0 .text
 [1081](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1082](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1083](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000698 .idata$7
 [1084](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000274 .idata$5
 [1085](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000e4 .idata$4
 [1086](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000522 .idata$6
-[1087](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ba8 .text
+[1087](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068b8 .text
 [1088](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1089](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1090](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000694 .idata$7
 [1091](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000026c .idata$5
 [1092](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000dc .idata$4
 [1093](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000510 .idata$6
-[1094](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bb0 .text
+[1094](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068c0 .text
 [1095](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1096](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1097](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000690 .idata$7
 [1098](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000264 .idata$5
 [1099](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000d4 .idata$4
 [1100](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004f4 .idata$6
-[1101](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bb8 .text
+[1101](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068c8 .text
 [1102](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1103](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1104](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000068c .idata$7
 [1105](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000025c .idata$5
 [1106](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000cc .idata$4
 [1107](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004e6 .idata$6
-[1108](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bc0 .text
+[1108](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068d0 .text
 [1109](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1110](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1111](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000688 .idata$7
 [1112](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000254 .idata$5
 [1113](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000c4 .idata$4
 [1114](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004d2 .idata$6
-[1115](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bc8 .text
+[1115](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068d8 .text
 [1116](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1117](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1118](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000680 .idata$7
 [1119](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000244 .idata$5
 [1120](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000b4 .idata$4
 [1121](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000004ac .idata$6
-[1122](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bd0 .text
+[1122](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068e0 .text
 [1123](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1124](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1125](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000067c .idata$7
 [1126](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000023c .idata$5
 [1127](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000ac .idata$4
 [1128](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000498 .idata$6
-[1129](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bd8 .text
+[1129](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068e8 .text
 [1130](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1131](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1132](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000678 .idata$7
 [1133](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000234 .idata$5
 [1134](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000a4 .idata$4
 [1135](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000047e .idata$6
-[1136](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006be0 .text
+[1136](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068f0 .text
 [1137](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1138](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1139](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000674 .idata$7
 [1140](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000022c .idata$5
 [1141](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000009c .idata$4
 [1142](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000046a .idata$6
-[1143](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006be8 .text
+[1143](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000068f8 .text
 [1144](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1145](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1146](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000670 .idata$7
 [1147](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000224 .idata$5
 [1148](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000094 .idata$4
 [1149](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000454 .idata$6
-[1150](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bf0 .text
+[1150](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006900 .text
 [1151](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1152](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1153](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000066c .idata$7
 [1154](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000021c .idata$5
 [1155](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000008c .idata$4
 [1156](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000043a .idata$6
-[1157](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006bf8 .text
+[1157](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006908 .text
 [1158](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1159](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1160](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000668 .idata$7
 [1161](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000214 .idata$5
 [1162](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000084 .idata$4
 [1163](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000422 .idata$6
-[1164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c00 .text
+[1164](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006910 .text
 [1165](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1166](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1167](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000664 .idata$7
 [1168](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000020c .idata$5
 [1169](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000007c .idata$4
 [1170](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000406 .idata$6
-[1171](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c08 .text
+[1171](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006918 .text
 [1172](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1173](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1174](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000660 .idata$7
 [1175](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000204 .idata$5
 [1176](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000074 .idata$4
 [1177](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003f6 .idata$6
-[1178](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c10 .text
+[1178](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006920 .text
 [1179](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1180](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1181](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000065c .idata$7
 [1182](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001fc .idata$5
 [1183](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000006c .idata$4
 [1184](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003dc .idata$6
-[1185](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c18 .text
+[1185](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006928 .text
 [1186](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1187](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1188](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000658 .idata$7
 [1189](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001f4 .idata$5
 [1190](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000064 .idata$4
 [1191](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003cc .idata$6
-[1192](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c20 .text
+[1192](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006930 .text
 [1193](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1194](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1195](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000654 .idata$7
 [1196](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001ec .idata$5
 [1197](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000005c .idata$4
 [1198](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003b6 .idata$6
-[1199](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c28 .text
+[1199](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006938 .text
 [1200](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1201](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1202](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000650 .idata$7
 [1203](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001e4 .idata$5
 [1204](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000054 .idata$4
 [1205](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000003a0 .idata$6
-[1206](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c30 .text
+[1206](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006940 .text
 [1207](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1208](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1209](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000064c .idata$7
 [1210](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001dc .idata$5
 [1211](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000004c .idata$4
 [1212](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000038c .idata$6
-[1213](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c38 .text
+[1213](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006948 .text
 [1214](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1215](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1216](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000648 .idata$7
 [1217](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001d4 .idata$5
 [1218](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000044 .idata$4
 [1219](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000374 .idata$6
-[1220](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006c40 .text
+[1220](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006950 .text
 [1221](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1222](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 .bss
 [1223](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000644 .idata$7
 [1224](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000001cc .idata$5
 [1225](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000003c .idata$4
 [1226](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000035c .idata$6
 [1227](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004e5 merr.c
 File 
-[1229](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006c50 __mingw_raise_matherr
+[1229](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 1) 0x0000000000006960 __mingw_raise_matherr
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
 [1231](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b70 stUserMathErr
-[1232](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006ca0 __mingw_setusermatherr
-[1233](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006cb0 _matherr
-[1234](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006c50 .text
+[1232](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069b0 __mingw_setusermatherr
+[1233](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069c0 _matherr
+[1234](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006960 .text
 AUX scnlen 0x15c nreloc 14 nlnno 0
 [1236](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1238](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b70 .bss
 AUX scnlen 0x8 nreloc 0 nlnno 0
 [1240](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004fc .xdata
 AUX scnlen 0x24 nreloc 0 nlnno 0
 [1242](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000588 .pdata
 AUX scnlen 0x24 nreloc 9 nlnno 0
-[1244](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000004a0 .rdata
+[1244](sec  3)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000480 .rdata
 AUX scnlen 0x140 nreloc 7 nlnno 0
-[1246](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006db0 .text
+[1246](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000006ac0 .text
 [1247](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000080 .data
 [1248](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000b80 .bss
 [1249](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000006b0 .idata$7
 [1250](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x000000000000028c .idata$5
 [1251](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x00000000000000fc .idata$4
 [1252](sec  8)(fl 0x00)(ty    0)(scl   3) (nx 0) 0x0000000000000540 .idata$6
 [1253](sec -2)(fl 0x00)(ty    0)(scl 103) (nx 1) 0x00000000000004f7 cygming-crtend.c
 File 
-[1255](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006e30 register_frame_ctor
+[1255](sec  1)(fl 0x00)(ty   20)(scl   3) (nx 1) 0x0000000000006b40 register_frame_ctor
 AUX tagndx 0 ttlsiz 0x0 lnnos 0 next 0
-[1257](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006dc0 .text
+[1257](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006ad0 .text
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1259](sec  2)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000080 .data
 AUX scnlen 0x0 nreloc 0 nlnno 0
 [1261](sec  6)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000b80 .bss
 AUX scnlen 0x0 nreloc 0 nlnno 0
-[1263](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006e30 .text.startup
+[1263](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b40 .text.startup
 AUX scnlen 0x5 nreloc 1 nlnno 0
 [1265](sec  5)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000000520 .xdata.startup
 AUX scnlen 0x4 nreloc 0 nlnno 0
 [1267](sec  4)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x00000000000005ac .pdata.startup
 AUX scnlen 0xc nreloc 3 nlnno 0
-[1269](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006e48 .ctors.65535
+[1269](sec  1)(fl 0x00)(ty    0)(scl   3) (nx 1) 0x0000000000006b58 .ctors.65535
 AUX scnlen 0x8 nreloc 1 nlnno 0
 [1271](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 __xc_z
-[1272](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 ___RUNTIME_PSEUDO_RELOC_LIST__
+[1272](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 ___RUNTIME_PSEUDO_RELOC_LIST__
 [1273](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002c4 __imp__vsnprintf
 [1274](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002cc __imp_abort
 [1275](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000069c __lib64_libkernel32_a_iname
 [1276](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __data_start__
-[1277](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e58 ___DTOR_LIST__
+[1277](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b68 ___DTOR_LIST__
 [1278](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ac __imp__lock
-[1279](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006960 printf
+[1279](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006670 printf
 [1280](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002b4 __imp__mkdir
 [1281](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000023c __imp_RtlVirtualUnwind
-[1282](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bc8 SetUnhandledExceptionFilter
-[1283](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069c0 _vsnprintf
+[1282](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068d8 SetUnhandledExceptionFilter
+[1283](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066d0 _vsnprintf
 [1284](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002d4 __imp_calloc
-[1285](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b90 _lock
-[1286](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069c8 _mkdir
+[1285](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068a0 _lock
+[1286](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066d8 _mkdir
 [1287](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___tls_start__
-[1288](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000660 .refptr.__native_startup_state
+[1288](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000640 .refptr.__native_startup_state
 [1289](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __ImageBase
 [1290](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 __xl_a
-[1291](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c18 GetLastError
-[1292](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c10 GetSystemTimeAsFileTime
+[1291](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006928 GetLastError
+[1292](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006920 GetSystemTimeAsFileTime
 [1293](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000820 mingw_initltssuo_force
-[1294](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 __rt_psrelocs_start
+[1294](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __rt_psrelocs_start
 [1295](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll_characteristics__
 [1296](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_stack_commit__
-[1297](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b98 __iob_func
+[1297](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000068a8 __iob_func
 [1298](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000200000 __size_of_stack_reserve__
 [1299](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000005 __major_subsystem_version__
 [1300](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xl_start__
 [1301](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __imp_DeleteCriticalSection
 [1302](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000038 __xl_d
 [1303](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000008 _tls_end
-[1304](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005f0 .refptr.__CTOR_LIST__
-[1305](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006ba0 VirtualQuery
+[1304](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005d0 .refptr.__CTOR_LIST__
+[1305](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068b0 VirtualQuery
 [1306](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xi_start__
 [1307](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000294 __imp__amsg_exit
 [1308](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000028 ___crt_xi_end__
 [1309](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000029c __imp__errno
 [1310](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _tls_start
-[1311](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006968 perror
-[1312](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000610 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
+[1311](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006678 perror
+[1312](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005f0 .refptr.__RUNTIME_PSEUDO_RELOC_LIST__
 [1313](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000860 __mingw_oldexcpt_handler
 [1314](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001ec __imp_GetCurrentThreadId
-[1315](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006970 malloc
-[1316](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c28 GetCurrentProcessId
+[1315](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006680 malloc
+[1316](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006938 GetCurrentProcessId
 [1317](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 _CRT_MT
-[1318](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bb8 TlsGetValue
-[1319](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bc0 TerminateProcess
+[1318](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068c8 TlsGetValue
+[1319](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068d0 TerminateProcess
 [1320](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __bss_start__
-[1321](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 ___RUNTIME_PSEUDO_RELOC_LIST_END__
-[1322](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bd8 RtlLookupFunctionEntry
+[1321](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 ___RUNTIME_PSEUDO_RELOC_LIST_END__
+[1322](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068e8 RtlLookupFunctionEntry
 [1323](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __size_of_heap_commit__
 [1324](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001f4 __imp_GetLastError
 [1325](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002fc __imp_free
 [1326](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000234 __imp_RtlLookupFunctionEntry
-[1327](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006ba8 VirtualProtect
+[1327](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068b8 VirtualProtect
 [1328](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000830 mingw_app_type
 [1329](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_start__
 [1330](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000214 __imp_LeaveCriticalSection
 [1331](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000204 __imp_GetTickCount
-[1332](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069b8 abort
-[1333](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000600 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
+[1332](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066c8 abort
+[1333](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005e0 .refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__
 [1334](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xp_end__
 [1335](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __dll__
 [1336](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_os_version__
 [1337](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001fc __imp_GetSystemTimeAsFileTime
-[1338](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c38 EnterCriticalSection
-[1339](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000690 .refptr.__xi_a
+[1338](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006948 EnterCriticalSection
+[1339](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000670 .refptr.__xi_a
 [1340](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000646c0000 __image_base__
-[1341](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005e0 .refptr._CRT_MT
-[1342](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006be0 RtlCaptureContext
+[1341](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000005c0 .refptr._CRT_MT
+[1342](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068f0 RtlCaptureContext
 [1343](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000001000 __section_alignment__
 [1344](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 __native_dllmain_reason
-[1345](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069b0 calloc
-[1346](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001c0 _tls_used
-[1347](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bb0 UnhandledExceptionFilter
+[1345](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066c0 calloc
+[1346](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001a0 _tls_used
+[1347](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068c0 UnhandledExceptionFilter
 [1348](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000035c __IAT_end__
-[1349](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 __RUNTIME_PSEUDO_RELOC_LIST__
-[1350](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006990 fprintf
+[1349](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __RUNTIME_PSEUDO_RELOC_LIST__
+[1350](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066a0 fprintf
 [1351](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000224 __imp_RtlAddFunctionTable
-[1352](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000004490 Sleep
+[1352](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000041a0 Sleep
 [1353](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000000a0 __data_end__
 [1354](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000304 __imp_fwrite
-[1355](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e40 __CTOR_LIST__
+[1355](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b50 __CTOR_LIST__
 [1356](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 _head_lib64_libkernel32_a
 [1357](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b90 __bss_end__
 [1358](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000020 __xi_z
-[1359](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c08 GetTickCount
+[1359](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006918 GetTickCount
 [1360](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000018 pcinit
 [1361](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __native_vcclrit_reason
 [1362](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___crt_xc_end__
-[1363](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006be8 RtlAddFunctionTable
-[1364](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000650 .refptr.__native_startup_lock
+[1363](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068f8 RtlAddFunctionTable
+[1364](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000630 .refptr.__native_startup_lock
 [1365](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001d4 __imp_EnterCriticalSection
 [1366](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000082c _tls_index
-[1367](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006958 signal
+[1367](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006668 signal
 [1368](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b80 __native_startup_state
 [1369](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 ___crt_xc_start__
 [1370](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001e4 __imp_GetCurrentProcessId
-[1371](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006948 strncmp
+[1371](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006658 strncmp
 [1372](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000254 __imp_TerminateProcess
 [1373](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000714 __lib64_libmsvcrt_os_a_iname
-[1374](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e40 ___CTOR_LIST__
-[1375](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000620 .refptr.__dyn_tls_init_callback
+[1374](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b50 ___CTOR_LIST__
+[1375](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000600 .refptr.__dyn_tls_init_callback
 [1376](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000334 __imp_signal
-[1377](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006978 log10
+[1377](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006688 log10
 [1378](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000058 __imp__register_onexit_function
-[1379](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b80 realloc
+[1379](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006890 realloc
 [1380](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __rt_psrelocs_size
 [1381](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000021c __imp_QueryPerformanceCounter
 [1382](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000033c __imp_strlen
 [1383](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000314 __imp_malloc
 [1384](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000200 __file_alignment__
 [1385](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000020c __imp_InitializeCriticalSection
 [1386](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000032c __imp_realloc
-[1387](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c00 InitializeCriticalSection
+[1387](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006910 InitializeCriticalSection
 [1388](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002dc __imp_exit
-[1389](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006998 fopen
+[1389](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066a8 fopen
 [1390](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000034c __imp_vfprintf
 [1391](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000004 __major_os_version__
-[1392](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069a0 fclose
+[1392](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066b0 fclose
 [1393](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001cc __IAT_start__
 [1394](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000264 __imp_UnhandledExceptionFilter
 [1395](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000040 __xl_z
 [1396](sec  0)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __end__
 [1397](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000244 __imp_SetUnhandledExceptionFilter
-[1398](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006b0 .refptr.mingw_app_type
+[1398](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000690 .refptr.mingw_app_type
 [1399](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000031c __imp_perror
-[1400](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006e58 __DTOR_LIST__
-[1401](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bd0 RtlVirtualUnwind
+[1400](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006b68 __DTOR_LIST__
+[1401](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000068e0 RtlVirtualUnwind
 [1402](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000060 __imp__initialize_onexit_table
 [1403](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 __xi_a
 [1404](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000024c __imp_Sleep
-[1405](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bf8 LeaveCriticalSection
+[1405](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006908 LeaveCriticalSection
 [1406](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __xc_a
 [1407](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000028c __imp___setusermatherr
 [1408](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000100000 __size_of_heap_reserve__
 [1409](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_start__
 [1410](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000003 __subsystem__
-[1411](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069e0 _amsg_exit
+[1411](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066f0 _amsg_exit
 [1412](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000090 __security_cookie_complement
 [1413](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000025c __imp_TlsGetValue
-[1414](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c30 GetCurrentProcess
+[1414](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006940 GetCurrentProcess
 [1415](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000050 __imp__execute_onexit_table
-[1416](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006db0 __setusermatherr
+[1416](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006ac0 __setusermatherr
 [1417](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002f4 __imp_fprintf
 [1418](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000026c __imp_VirtualProtect
 [1419](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000030 __xl_c
 [1420](sec 10)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000010 ___tls_end__
-[1421](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006bf0 QueryPerformanceCounter
+[1421](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006900 QueryPerformanceCounter
 [1422](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000274 __imp_VirtualQuery
 [1423](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002a4 __imp__initterm
 [1424](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000824 mingw_initltsdyn_force
 [1425](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002e4 __imp_fclose
 [1426](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000284 __imp___iob_func
-[1427](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001a0 __dyn_tls_init_callback
-[1428](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000630 .refptr.__image_base__
-[1429](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069d0 _initterm
-[1430](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006980 fwrite
+[1427](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000180 __dyn_tls_init_callback
+[1428](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000610 .refptr.__image_base__
+[1429](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066e0 _initterm
+[1430](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006690 fwrite
 [1431](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000344 __imp_strncmp
 [1432](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000014 _head_lib64_libmsvcrt_os_a
 [1433](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000070 __imp___acrt_iob_func
 [1434](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __major_image_version__
 [1435](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __loader_flags__
-[1436](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000057a0 ___chkstk_ms
+[1436](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000054b0 ___chkstk_ms
 [1437](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000b88 __native_startup_lock
-[1438](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000640 .refptr.__native_dllmain_reason
+[1438](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000620 .refptr.__native_dllmain_reason
 [1439](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000030c __imp_log10
-[1440](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c20 GetCurrentThreadId
-[1441](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 __rt_psrelocs_end
-[1442](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069a8 exit
+[1440](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006930 GetCurrentThreadId
+[1441](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __rt_psrelocs_end
+[1442](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066b8 exit
 [1443](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000002 __minor_subsystem_version__
 [1444](sec -1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000000 __minor_image_version__
 [1445](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002bc __imp__unlock
-[1446](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000069d8 _errno
+[1446](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x00000000000066e8 _errno
 [1447](sec  6)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000828 mingw_initltsdrot_force
 [1448](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000324 __imp_printf
-[1449](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000670 .refptr.__xc_a
-[1450](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006950 strlen
-[1451](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000006a0 .refptr.__xi_z
-[1452](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006c40 DeleteCriticalSection
+[1449](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000650 .refptr.__xc_a
+[1450](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006660 strlen
+[1451](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000680 .refptr.__xi_z
+[1452](sec  1)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000006950 DeleteCriticalSection
 [1453](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x000000000000022c __imp_RtlCaptureContext
-[1454](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000900 __RUNTIME_PSEUDO_RELOC_LIST_END__
+[1454](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000008e0 __RUNTIME_PSEUDO_RELOC_LIST_END__
 [1455](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000002ec __imp_fopen
-[1456](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006b88 _unlock
+[1456](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006898 _unlock
 [1457](sec  8)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x00000000000001dc __imp_GetCurrentProcess
-[1458](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000680 .refptr.__xc_z
+[1458](sec  3)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000660 .refptr.__xc_z
 [1459](sec  9)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000048 ___crt_xt_end__
-[1460](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006940 vfprintf
-[1461](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006988 free
+[1460](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006650 vfprintf
+[1461](sec  1)(fl 0x00)(ty   20)(scl   2) (nx 0) 0x0000000000006698 free
 [1462](sec  2)(fl 0x00)(ty    0)(scl   2) (nx 0) 0x0000000000000080 __security_cookie
 
 
 
 Disassembly of section .text:
 
 00000000646c1000 <pre_c_init>:
     646c1000:	lea    0xaff9(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c1007:	jmp    646c79f0 <_initialize_onexit_table>
+    646c1007:	jmp    646c7700 <_initialize_onexit_table>
     646c100c:	nopl   0x0(%rax)
 
 00000000646c1010 <_CRT_INIT>:
     646c1010:	push   %r13
     646c1012:	push   %r12
     646c1014:	push   %rbp
     646c1015:	push   %rdi
@@ -2645,74 +2645,74 @@
     646c1021:	mov    %r8,%r13
     646c1024:	jne    646c10a0 <_CRT_INIT+0x90>
     646c1026:	mov    0xafec(%rip),%edx        # 646cc018 <__proc_attached>
     646c102c:	xor    %eax,%eax
     646c102e:	test   %edx,%edx
     646c1030:	jle    646c108b <_CRT_INIT+0x7b>
     646c1032:	sub    $0x1,%edx
-    646c1035:	mov    0x8614(%rip),%rbx        # 646c9650 <.refptr.__native_startup_lock>
+    646c1035:	mov    0x85f4(%rip),%rbx        # 646c9630 <.refptr.__native_startup_lock>
     646c103c:	xor    %ebp,%ebp
     646c103e:	mov    $0x1,%edi
     646c1043:	mov    %edx,0xafcf(%rip)        # 646cc018 <__proc_attached>
     646c1049:	mov    0xd1fc(%rip),%r12        # 646ce24c <__imp_Sleep>
     646c1050:	jmp    646c105a <_CRT_INIT+0x4a>
     646c1052:	mov    $0x3e8,%ecx
     646c1057:	call   *%r12
     646c105a:	mov    %rbp,%rax
     646c105d:	lock cmpxchg %rdi,(%rbx)
     646c1062:	test   %rax,%rax
     646c1065:	mov    %rax,%rsi
     646c1068:	jne    646c1052 <_CRT_INIT+0x42>
-    646c106a:	mov    0x85ef(%rip),%rdi        # 646c9660 <.refptr.__native_startup_state>
+    646c106a:	mov    0x85cf(%rip),%rdi        # 646c9640 <.refptr.__native_startup_state>
     646c1071:	mov    (%rdi),%eax
     646c1073:	cmp    $0x2,%eax
     646c1076:	je     646c1165 <_CRT_INIT+0x155>
     646c107c:	mov    $0x1f,%ecx
-    646c1081:	call   646c79e0 <_amsg_exit>
+    646c1081:	call   646c76f0 <_amsg_exit>
     646c1086:	mov    $0x1,%eax
     646c108b:	add    $0x28,%rsp
     646c108f:	pop    %rbx
     646c1090:	pop    %rsi
     646c1091:	pop    %rdi
     646c1092:	pop    %rbp
     646c1093:	pop    %r12
     646c1095:	pop    %r13
     646c1097:	ret
     646c1098:	nopl   0x0(%rax,%rax,1)
     646c10a0:	cmp    $0x1,%edx
     646c10a3:	jne    646c1153 <_CRT_INIT+0x143>
     646c10a9:	mov    %gs:0x30,%rax
-    646c10b2:	mov    0x8597(%rip),%rbx        # 646c9650 <.refptr.__native_startup_lock>
+    646c10b2:	mov    0x8577(%rip),%rbx        # 646c9630 <.refptr.__native_startup_lock>
     646c10b9:	xor    %edi,%edi
     646c10bb:	mov    0x8(%rax),%rsi
     646c10bf:	mov    0xd186(%rip),%rbp        # 646ce24c <__imp_Sleep>
     646c10c6:	jmp    646c10e0 <_CRT_INIT+0xd0>
     646c10c8:	nopl   0x0(%rax,%rax,1)
     646c10d0:	cmp    %rax,%rsi
     646c10d3:	je     646c1190 <_CRT_INIT+0x180>
     646c10d9:	mov    $0x3e8,%ecx
     646c10de:	call   *%rbp
     646c10e0:	mov    %rdi,%rax
     646c10e3:	lock cmpxchg %rsi,(%rbx)
     646c10e8:	test   %rax,%rax
     646c10eb:	jne    646c10d0 <_CRT_INIT+0xc0>
     646c10ed:	xor    %edi,%edi
-    646c10ef:	mov    0x856a(%rip),%rsi        # 646c9660 <.refptr.__native_startup_state>
+    646c10ef:	mov    0x854a(%rip),%rsi        # 646c9640 <.refptr.__native_startup_state>
     646c10f6:	mov    (%rsi),%eax
     646c10f8:	cmp    $0x1,%eax
     646c10fb:	je     646c11f0 <_CRT_INIT+0x1e0>
     646c1101:	mov    (%rsi),%eax
     646c1103:	test   %eax,%eax
     646c1105:	je     646c11b0 <_CRT_INIT+0x1a0>
     646c110b:	mov    (%rsi),%eax
     646c110d:	cmp    $0x1,%eax
     646c1110:	je     646c11d0 <_CRT_INIT+0x1c0>
     646c1116:	test   %edi,%edi
     646c1118:	je     646c11a0 <_CRT_INIT+0x190>
-    646c111e:	mov    0x84fb(%rip),%rax        # 646c9620 <.refptr.__dyn_tls_init_callback>
+    646c111e:	mov    0x84db(%rip),%rax        # 646c9600 <.refptr.__dyn_tls_init_callback>
     646c1125:	mov    (%rax),%rax
     646c1128:	test   %rax,%rax
     646c112b:	je     646c113a <_CRT_INIT+0x12a>
     646c112d:	mov    %r13,%r8
     646c1130:	mov    $0x2,%edx
     646c1135:	mov    %r12,%rcx
     646c1138:	call   *%rax
@@ -2732,15 +2732,15 @@
     646c115d:	pop    %rsi
     646c115e:	pop    %rdi
     646c115f:	pop    %rbp
     646c1160:	pop    %r12
     646c1162:	pop    %r13
     646c1164:	ret
     646c1165:	lea    0xae94(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c116c:	call   646c7af0 <_execute_onexit_table>
+    646c116c:	call   646c7800 <_execute_onexit_table>
     646c1171:	movl   $0x0,(%rdi)
     646c1177:	xchg   %rsi,(%rbx)
     646c117a:	mov    $0x1,%eax
     646c117f:	add    $0x28,%rsp
     646c1183:	pop    %rbx
     646c1184:	pop    %rsi
     646c1185:	pop    %rdi
@@ -2752,57 +2752,57 @@
     646c1190:	mov    $0x1,%edi
     646c1195:	jmp    646c10ef <_CRT_INIT+0xdf>
     646c119a:	nopw   0x0(%rax,%rax,1)
     646c11a0:	xor    %eax,%eax
     646c11a2:	xchg   %rax,(%rbx)
     646c11a5:	jmp    646c111e <_CRT_INIT+0x10e>
     646c11aa:	nopw   0x0(%rax,%rax,1)
-    646c11b0:	mov    0x84e9(%rip),%rdx        # 646c96a0 <.refptr.__xi_z>
+    646c11b0:	mov    0x84c9(%rip),%rdx        # 646c9680 <.refptr.__xi_z>
     646c11b7:	movl   $0x1,(%rsi)
-    646c11bd:	mov    0x84cc(%rip),%rcx        # 646c9690 <.refptr.__xi_a>
-    646c11c4:	call   646c79d0 <_initterm>
+    646c11bd:	mov    0x84ac(%rip),%rcx        # 646c9670 <.refptr.__xi_a>
+    646c11c4:	call   646c76e0 <_initterm>
     646c11c9:	jmp    646c110b <_CRT_INIT+0xfb>
     646c11ce:	xchg   %ax,%ax
-    646c11d0:	mov    0x84a9(%rip),%rdx        # 646c9680 <.refptr.__xc_z>
-    646c11d7:	mov    0x8492(%rip),%rcx        # 646c9670 <.refptr.__xc_a>
-    646c11de:	call   646c79d0 <_initterm>
+    646c11d0:	mov    0x8489(%rip),%rdx        # 646c9660 <.refptr.__xc_z>
+    646c11d7:	mov    0x8472(%rip),%rcx        # 646c9650 <.refptr.__xc_a>
+    646c11de:	call   646c76e0 <_initterm>
     646c11e3:	movl   $0x2,(%rsi)
     646c11e9:	jmp    646c1116 <_CRT_INIT+0x106>
     646c11ee:	xchg   %ax,%ax
     646c11f0:	mov    $0x1f,%ecx
-    646c11f5:	call   646c79e0 <_amsg_exit>
+    646c11f5:	call   646c76f0 <_amsg_exit>
     646c11fa:	jmp    646c110b <_CRT_INIT+0xfb>
     646c11ff:	nop
 
 00000000646c1200 <__DllMainCRTStartup>:
     646c1200:	push   %r12
     646c1202:	push   %rbp
     646c1203:	push   %rdi
     646c1204:	push   %rsi
     646c1205:	push   %rbx
     646c1206:	sub    $0x20,%rsp
-    646c120a:	mov    0x842f(%rip),%rsi        # 646c9640 <.refptr.__native_dllmain_reason>
+    646c120a:	mov    0x840f(%rip),%rsi        # 646c9620 <.refptr.__native_dllmain_reason>
     646c1211:	test   %edx,%edx
     646c1213:	mov    %rcx,%rdi
     646c1216:	mov    %edx,%ebx
     646c1218:	mov    %edx,(%rsi)
     646c121a:	mov    %r8,%rbp
     646c121d:	jne    646c1273 <__DllMainCRTStartup+0x73>
     646c121f:	mov    0xadf3(%rip),%eax        # 646cc018 <__proc_attached>
     646c1225:	test   %eax,%eax
     646c1227:	je     646c125c <__DllMainCRTStartup+0x5c>
-    646c1229:	call   646c5a00 <_pei386_runtime_relocator>
+    646c1229:	call   646c5710 <_pei386_runtime_relocator>
     646c122e:	mov    %rbp,%r8
     646c1231:	xor    %edx,%edx
     646c1233:	mov    %rdi,%rcx
-    646c1236:	call   646c67f0 <DllMain>
+    646c1236:	call   646c6500 <DllMain>
     646c123b:	mov    %rbp,%r8
     646c123e:	mov    %ebx,%edx
     646c1240:	mov    %rdi,%rcx
-    646c1243:	call   646c67e0 <DllEntryPoint>
+    646c1243:	call   646c64f0 <DllEntryPoint>
     646c1248:	mov    %rbp,%r8
     646c124b:	mov    %ebx,%edx
     646c124d:	mov    %rdi,%rcx
     646c1250:	mov    %eax,%r12d
     646c1253:	call   646c1010 <_CRT_INIT>
     646c1258:	test   %eax,%eax
     646c125a:	jne    646c125f <__DllMainCRTStartup+0x5f>
@@ -2812,94 +2812,94 @@
     646c1268:	add    $0x20,%rsp
     646c126c:	pop    %rbx
     646c126d:	pop    %rsi
     646c126e:	pop    %rdi
     646c126f:	pop    %rbp
     646c1270:	pop    %r12
     646c1272:	ret
-    646c1273:	call   646c5a00 <_pei386_runtime_relocator>
+    646c1273:	call   646c5710 <_pei386_runtime_relocator>
     646c1278:	lea    -0x1(%rbx),%eax
     646c127b:	cmp    $0x1,%eax
     646c127e:	jbe    646c12a0 <__DllMainCRTStartup+0xa0>
     646c1280:	mov    %rbp,%r8
     646c1283:	mov    %ebx,%edx
     646c1285:	mov    %rdi,%rcx
-    646c1288:	call   646c67f0 <DllMain>
+    646c1288:	call   646c6500 <DllMain>
     646c128d:	cmp    $0x3,%ebx
     646c1290:	mov    %eax,%r12d
     646c1293:	jne    646c125f <__DllMainCRTStartup+0x5f>
     646c1295:	jmp    646c123b <__DllMainCRTStartup+0x3b>
     646c1297:	nopw   0x0(%rax,%rax,1)
     646c12a0:	mov    %rbp,%r8
     646c12a3:	mov    %ebx,%edx
     646c12a5:	mov    %rdi,%rcx
     646c12a8:	call   646c1010 <_CRT_INIT>
     646c12ad:	test   %eax,%eax
     646c12af:	je     646c125c <__DllMainCRTStartup+0x5c>
     646c12b1:	mov    %rbp,%r8
     646c12b4:	mov    %ebx,%edx
     646c12b6:	mov    %rdi,%rcx
-    646c12b9:	call   646c67e0 <DllEntryPoint>
+    646c12b9:	call   646c64f0 <DllEntryPoint>
     646c12be:	test   %eax,%eax
     646c12c0:	mov    %eax,%r12d
     646c12c3:	je     646c1320 <__DllMainCRTStartup+0x120>
     646c12c5:	cmp    $0x1,%ebx
     646c12c8:	jne    646c1280 <__DllMainCRTStartup+0x80>
-    646c12ca:	call   646c5550 <__main>
+    646c12ca:	call   646c5260 <__main>
     646c12cf:	mov    %rbp,%r8
     646c12d2:	mov    $0x1,%edx
     646c12d7:	mov    %rdi,%rcx
-    646c12da:	call   646c67f0 <DllMain>
+    646c12da:	call   646c6500 <DllMain>
     646c12df:	test   %eax,%eax
     646c12e1:	mov    %eax,%r12d
     646c12e4:	jne    646c125f <__DllMainCRTStartup+0x5f>
     646c12ea:	mov    %rbp,%r8
     646c12ed:	xor    %edx,%edx
     646c12ef:	mov    %rdi,%rcx
-    646c12f2:	call   646c67f0 <DllMain>
+    646c12f2:	call   646c6500 <DllMain>
     646c12f7:	mov    %rbp,%r8
     646c12fa:	xor    %edx,%edx
     646c12fc:	mov    %rdi,%rcx
-    646c12ff:	call   646c67e0 <DllEntryPoint>
+    646c12ff:	call   646c64f0 <DllEntryPoint>
     646c1304:	mov    %rbp,%r8
     646c1307:	xor    %edx,%edx
     646c1309:	mov    %rdi,%rcx
     646c130c:	call   646c1010 <_CRT_INIT>
     646c1311:	jmp    646c125f <__DllMainCRTStartup+0x5f>
     646c1316:	cs nopw 0x0(%rax,%rax,1)
     646c1320:	cmp    $0x1,%ebx
     646c1323:	jne    646c125c <__DllMainCRTStartup+0x5c>
     646c1329:	jmp    646c1304 <__DllMainCRTStartup+0x104>
     646c132b:	nopl   0x0(%rax,%rax,1)
 
 00000000646c1330 <DllMainCRTStartup>:
     646c1330:	sub    $0x48,%rsp
-    646c1334:	mov    0x8375(%rip),%rax        # 646c96b0 <.refptr.mingw_app_type>
+    646c1334:	mov    0x8355(%rip),%rax        # 646c9690 <.refptr.mingw_app_type>
     646c133b:	movl   $0x0,(%rax)
     646c1341:	cmp    $0x1,%edx
     646c1344:	je     646c1350 <DllMainCRTStartup+0x20>
     646c1346:	add    $0x48,%rsp
     646c134a:	jmp    646c1200 <__DllMainCRTStartup>
     646c134f:	nop
     646c1350:	mov    %r8,0x38(%rsp)
     646c1355:	mov    %edx,0x34(%rsp)
     646c1359:	mov    %rcx,0x28(%rsp)
-    646c135e:	call   646c5570 <__security_init_cookie>
-    646c1363:	call   646c5e60 <__mingw_init_ehandler>
+    646c135e:	call   646c5280 <__security_init_cookie>
+    646c1363:	call   646c5b70 <__mingw_init_ehandler>
     646c1368:	mov    0x38(%rsp),%r8
     646c136d:	mov    0x34(%rsp),%edx
     646c1371:	mov    0x28(%rsp),%rcx
     646c1376:	add    $0x48,%rsp
     646c137a:	jmp    646c1200 <__DllMainCRTStartup>
     646c137f:	nop
 
 00000000646c1380 <atexit>:
     646c1380:	mov    %rcx,%rdx
     646c1383:	lea    0xac76(%rip),%rcx        # 646cc000 <__bss_start__>
-    646c138a:	jmp    646c7a20 <_register_onexit_function>
+    646c138a:	jmp    646c7730 <_register_onexit_function>
     646c138f:	nop
 
 00000000646c1390 <__gcc_register_frame>:
     646c1390:	lea    0x9(%rip),%rcx        # 646c13a0 <__gcc_deregister_frame>
     646c1397:	jmp    646c1380 <atexit>
     646c139c:	nopl   0x0(%rax)
 
@@ -3933,15 +3933,15 @@
     646c227e:	lea    0x0(,%rax,4),%rdx
     646c2286:	mov    0x10(%rbp),%rax
     646c228a:	add    %rdx,%rax
     646c228d:	mov    (%rax),%eax
     646c228f:	cvtsi2sd %eax,%xmm0
     646c2293:	subsd  0x20(%rbp),%xmm0
     646c2298:	movsd  0x6d80(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c22a0:	call   646c6f60 <pow>
+    646c22a0:	call   646c6c70 <pow>
     646c22a5:	movapd %xmm0,%xmm1
     646c22a9:	movsd  -0x8(%rbp),%xmm0
     646c22ae:	addsd  %xmm1,%xmm0
     646c22b2:	movsd  %xmm0,-0x8(%rbp)
     646c22b7:	addl   $0x1,-0xc(%rbp)
     646c22bb:	mov    -0xc(%rbp),%eax
     646c22be:	cmp    0x18(%rbp),%eax
@@ -3971,15 +3971,15 @@
     646c230c:	lea    0x0(,%rax,8),%rdx
     646c2314:	mov    0x10(%rbp),%rax
     646c2318:	add    %rdx,%rax
     646c231b:	mov    (%rax),%rax
     646c231e:	cvtsi2sd %rax,%xmm0
     646c2323:	subsd  0x20(%rbp),%xmm0
     646c2328:	movsd  0x6cf0(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c2330:	call   646c6f60 <pow>
+    646c2330:	call   646c6c70 <pow>
     646c2335:	movapd %xmm0,%xmm1
     646c2339:	movsd  -0x8(%rbp),%xmm0
     646c233e:	addsd  %xmm1,%xmm0
     646c2342:	movsd  %xmm0,-0x8(%rbp)
     646c2347:	addl   $0x1,-0xc(%rbp)
     646c234b:	mov    -0xc(%rbp),%eax
     646c234e:	cmp    0x18(%rbp),%eax
@@ -4009,15 +4009,15 @@
     646c239c:	lea    0x0(,%rax,4),%rdx
     646c23a4:	mov    0x10(%rbp),%rax
     646c23a8:	add    %rdx,%rax
     646c23ab:	movss  (%rax),%xmm0
     646c23af:	cvtss2sd %xmm0,%xmm0
     646c23b3:	subsd  0x20(%rbp),%xmm0
     646c23b8:	movsd  0x6c60(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c23c0:	call   646c6f60 <pow>
+    646c23c0:	call   646c6c70 <pow>
     646c23c5:	movapd %xmm0,%xmm1
     646c23c9:	movsd  -0x8(%rbp),%xmm0
     646c23ce:	addsd  %xmm1,%xmm0
     646c23d2:	movsd  %xmm0,-0x8(%rbp)
     646c23d7:	addl   $0x1,-0xc(%rbp)
     646c23db:	mov    -0xc(%rbp),%eax
     646c23de:	cmp    0x18(%rbp),%eax
@@ -4046,15 +4046,15 @@
     646c242a:	cltq
     646c242c:	lea    0x0(,%rax,8),%rdx
     646c2434:	mov    0x10(%rbp),%rax
     646c2438:	add    %rdx,%rax
     646c243b:	movsd  (%rax),%xmm0
     646c243f:	subsd  0x20(%rbp),%xmm0
     646c2444:	movsd  0x6bd4(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c244c:	call   646c6f60 <pow>
+    646c244c:	call   646c6c70 <pow>
     646c2451:	movapd %xmm0,%xmm1
     646c2455:	movsd  -0x8(%rbp),%xmm0
     646c245a:	addsd  %xmm1,%xmm0
     646c245e:	movsd  %xmm0,-0x8(%rbp)
     646c2463:	addl   $0x1,-0xc(%rbp)
     646c2467:	mov    -0xc(%rbp),%eax
     646c246a:	cmp    0x18(%rbp),%eax
@@ -4084,27 +4084,27 @@
     646c24b8:	lea    0x0(,%rax,4),%rdx
     646c24c0:	mov    0x10(%rbp),%rax
     646c24c4:	add    %rdx,%rax
     646c24c7:	mov    (%rax),%eax
     646c24c9:	cvtsi2sd %eax,%xmm0
     646c24cd:	subsd  0x20(%rbp),%xmm0
     646c24d2:	movsd  0x6b46(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c24da:	call   646c6f60 <pow>
+    646c24da:	call   646c6c70 <pow>
     646c24df:	movapd %xmm0,%xmm1
     646c24e3:	movsd  -0x8(%rbp),%xmm0
     646c24e8:	addsd  %xmm1,%xmm0
     646c24ec:	movsd  %xmm0,-0x8(%rbp)
     646c24f1:	addl   $0x1,-0xc(%rbp)
     646c24f5:	mov    -0xc(%rbp),%eax
     646c24f8:	cmp    0x18(%rbp),%eax
     646c24fb:	jl     646c24b3 <c_array_std_int+0x26>
     646c24fd:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c2502:	movsd  -0x8(%rbp),%xmm0
     646c2507:	divsd  %xmm1,%xmm0
-    646c250b:	call   646c6860 <sqrt>
+    646c250b:	call   646c6570 <sqrt>
     646c2510:	movq   %xmm0,%rax
     646c2515:	movq   %rax,%xmm0
     646c251a:	add    $0x30,%rsp
     646c251e:	pop    %rbp
     646c251f:	ret
 
 00000000646c2520 <c_array_std_long_long>:
@@ -4123,27 +4123,27 @@
     646c254b:	lea    0x0(,%rax,8),%rdx
     646c2553:	mov    0x10(%rbp),%rax
     646c2557:	add    %rdx,%rax
     646c255a:	mov    (%rax),%rax
     646c255d:	cvtsi2sd %rax,%xmm0
     646c2562:	subsd  0x20(%rbp),%xmm0
     646c2567:	movsd  0x6ab1(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c256f:	call   646c6f60 <pow>
+    646c256f:	call   646c6c70 <pow>
     646c2574:	movapd %xmm0,%xmm1
     646c2578:	movsd  -0x8(%rbp),%xmm0
     646c257d:	addsd  %xmm1,%xmm0
     646c2581:	movsd  %xmm0,-0x8(%rbp)
     646c2586:	addl   $0x1,-0xc(%rbp)
     646c258a:	mov    -0xc(%rbp),%eax
     646c258d:	cmp    0x18(%rbp),%eax
     646c2590:	jl     646c2546 <c_array_std_long_long+0x26>
     646c2592:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c2597:	movsd  -0x8(%rbp),%xmm0
     646c259c:	divsd  %xmm1,%xmm0
-    646c25a0:	call   646c6860 <sqrt>
+    646c25a0:	call   646c6570 <sqrt>
     646c25a5:	movq   %xmm0,%rax
     646c25aa:	movq   %rax,%xmm0
     646c25af:	add    $0x30,%rsp
     646c25b3:	pop    %rbp
     646c25b4:	ret
 
 00000000646c25b5 <c_array_std_float>:
@@ -4162,27 +4162,27 @@
     646c25e0:	lea    0x0(,%rax,4),%rdx
     646c25e8:	mov    0x10(%rbp),%rax
     646c25ec:	add    %rdx,%rax
     646c25ef:	movss  (%rax),%xmm0
     646c25f3:	cvtss2sd %xmm0,%xmm0
     646c25f7:	subsd  0x20(%rbp),%xmm0
     646c25fc:	movsd  0x6a1c(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c2604:	call   646c6f60 <pow>
+    646c2604:	call   646c6c70 <pow>
     646c2609:	movapd %xmm0,%xmm1
     646c260d:	movsd  -0x8(%rbp),%xmm0
     646c2612:	addsd  %xmm1,%xmm0
     646c2616:	movsd  %xmm0,-0x8(%rbp)
     646c261b:	addl   $0x1,-0xc(%rbp)
     646c261f:	mov    -0xc(%rbp),%eax
     646c2622:	cmp    0x18(%rbp),%eax
     646c2625:	jl     646c25db <c_array_std_float+0x26>
     646c2627:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c262c:	movsd  -0x8(%rbp),%xmm0
     646c2631:	divsd  %xmm1,%xmm0
-    646c2635:	call   646c6860 <sqrt>
+    646c2635:	call   646c6570 <sqrt>
     646c263a:	movq   %xmm0,%rax
     646c263f:	movq   %rax,%xmm0
     646c2644:	add    $0x30,%rsp
     646c2648:	pop    %rbp
     646c2649:	ret
 
 00000000646c264a <c_array_std_double>:
@@ -4200,27 +4200,27 @@
     646c2673:	cltq
     646c2675:	lea    0x0(,%rax,8),%rdx
     646c267d:	mov    0x10(%rbp),%rax
     646c2681:	add    %rdx,%rax
     646c2684:	movsd  (%rax),%xmm0
     646c2688:	subsd  0x20(%rbp),%xmm0
     646c268d:	movsd  0x698b(%rip),%xmm1        # 646c9020 <.rdata+0x20>
-    646c2695:	call   646c6f60 <pow>
+    646c2695:	call   646c6c70 <pow>
     646c269a:	movapd %xmm0,%xmm1
     646c269e:	movsd  -0x8(%rbp),%xmm0
     646c26a3:	addsd  %xmm1,%xmm0
     646c26a7:	movsd  %xmm0,-0x8(%rbp)
     646c26ac:	addl   $0x1,-0xc(%rbp)
     646c26b0:	mov    -0xc(%rbp),%eax
     646c26b3:	cmp    0x18(%rbp),%eax
     646c26b6:	jl     646c2670 <c_array_std_double+0x26>
     646c26b8:	cvtsi2sdl 0x18(%rbp),%xmm1
     646c26bd:	movsd  -0x8(%rbp),%xmm0
     646c26c2:	divsd  %xmm1,%xmm0
-    646c26c6:	call   646c6860 <sqrt>
+    646c26c6:	call   646c6570 <sqrt>
     646c26cb:	movq   %xmm0,%rax
     646c26d0:	movq   %rax,%xmm0
     646c26d5:	add    $0x30,%rsp
     646c26d9:	pop    %rbp
     646c26da:	ret
 
 00000000646c26db <c_array_mean_int>:
@@ -4820,24 +4820,24 @@
     646c2e45:	mov    %rax,-0x18(%rbp)
     646c2e49:	mov    0x10(%rbp),%rcx
     646c2e4d:	call   646c2d5e <mt19937_get_double>
     646c2e52:	movq   %xmm0,%rax
     646c2e57:	mov    %rax,-0x20(%rbp)
     646c2e5b:	mov    -0x18(%rbp),%rax
     646c2e5f:	movq   %rax,%xmm0
-    646c2e64:	call   646c6da0 <log>
+    646c2e64:	call   646c6ab0 <log>
     646c2e69:	movapd %xmm0,%xmm1
     646c2e6d:	movsd  0x61cb(%rip),%xmm0        # 646c9040 <.rdata+0x10>
     646c2e75:	mulsd  %xmm1,%xmm0
-    646c2e79:	call   646c6860 <sqrt>
+    646c2e79:	call   646c6570 <sqrt>
     646c2e7e:	movapd %xmm0,%xmm6
     646c2e82:	movsd  -0x20(%rbp),%xmm1
     646c2e87:	movsd  0x61b9(%rip),%xmm0        # 646c9048 <.rdata+0x18>
     646c2e8f:	mulsd  %xmm1,%xmm0
-    646c2e93:	call   646c6a80 <cos>
+    646c2e93:	call   646c6790 <cos>
     646c2e98:	mulsd  %xmm6,%xmm0
     646c2e9c:	movsd  %xmm0,-0x28(%rbp)
     646c2ea1:	movsd  -0x28(%rbp),%xmm0
     646c2ea6:	movq   %xmm0,%rax
     646c2eab:	movq   %rax,%xmm0
     646c2eb0:	movaps -0x10(%rbp),%xmm6
     646c2eb4:	add    $0x50,%rsp
@@ -4915,15 +4915,15 @@
     646c2f9f:	mulsd  %xmm1,%xmm0
     646c2fa3:	mov    0x28(%rbp),%rax
     646c2fa7:	movsd  0x10(%rax),%xmm2
     646c2fac:	mov    0x28(%rbp),%rax
     646c2fb0:	movsd  0x10(%rax),%xmm1
     646c2fb5:	mulsd  %xmm2,%xmm1
     646c2fb9:	divsd  %xmm1,%xmm0
-    646c2fbd:	call   646c6bb0 <exp>
+    646c2fbd:	call   646c68c0 <exp>
     646c2fc2:	movapd %xmm0,%xmm1
     646c2fc6:	movsd  0x608a(%rip),%xmm0        # 646c9058 <.rdata+0x8>
     646c2fce:	subsd  %xmm1,%xmm0
     646c2fd2:	movsd  %xmm0,-0x18(%rbp)
     646c2fd7:	mov    0x28(%rbp),%rax
     646c2fdb:	movsd  0x18(%rax),%xmm0
     646c2fe0:	movsd  -0x10(%rbp),%xmm1
@@ -4957,87 +4957,84 @@
     646c303e:	mov    %r8d,0x20(%rbp)
     646c3042:	mov    %r9,0x28(%rbp)
     646c3046:	mov    0x28(%rbp),%rax
     646c304a:	movsd  0x18(%rax),%xmm0
     646c304f:	mov    0x28(%rbp),%rax
     646c3053:	movsd  0x20(%rax),%xmm1
     646c3058:	subsd  %xmm1,%xmm0
-    646c305c:	movsd  %xmm0,-0x10(%rbp)
+    646c305c:	movsd  %xmm0,-0x18(%rbp)
     646c3061:	movl   $0x0,-0x4(%rbp)
-    646c3068:	jmp    646c3168 <cov_model2d+0x13a>
-    646c306d:	movl   $0x0,-0x8(%rbp)
-    646c3074:	jmp    646c3158 <cov_model2d+0x12a>
-    646c3079:	mov    -0x4(%rbp),%eax
-    646c307c:	cltq
-    646c307e:	lea    0x0(,%rax,8),%rdx
-    646c3086:	mov    0x10(%rbp),%rax
-    646c308a:	add    %rdx,%rax
-    646c308d:	mov    (%rax),%rdx
-    646c3090:	mov    -0x8(%rbp),%eax
-    646c3093:	cltq
-    646c3095:	shl    $0x3,%rax
-    646c3099:	add    %rdx,%rax
-    646c309c:	movsd  (%rax),%xmm1
-    646c30a0:	mov    -0x4(%rbp),%eax
-    646c30a3:	cltq
-    646c30a5:	lea    0x0(,%rax,8),%rdx
-    646c30ad:	mov    0x10(%rbp),%rax
-    646c30b1:	add    %rdx,%rax
-    646c30b4:	mov    (%rax),%rdx
-    646c30b7:	mov    -0x8(%rbp),%eax
-    646c30ba:	cltq
-    646c30bc:	shl    $0x3,%rax
-    646c30c0:	add    %rdx,%rax
-    646c30c3:	movsd  (%rax),%xmm0
-    646c30c7:	mulsd  %xmm0,%xmm1
-    646c30cb:	movsd  0x5f7d(%rip),%xmm0        # 646c9050 <.rdata>
-    646c30d3:	mulsd  %xmm1,%xmm0
-    646c30d7:	mov    0x28(%rbp),%rax
-    646c30db:	movsd  0x10(%rax),%xmm2
-    646c30e0:	mov    0x28(%rbp),%rax
-    646c30e4:	movsd  0x10(%rax),%xmm1
-    646c30e9:	mulsd  %xmm2,%xmm1
-    646c30ed:	divsd  %xmm1,%xmm0
-    646c30f1:	call   646c6bb0 <exp>
-    646c30f6:	movapd %xmm0,%xmm1
-    646c30fa:	movsd  0x5f56(%rip),%xmm0        # 646c9058 <.rdata+0x8>
-    646c3102:	subsd  %xmm1,%xmm0
-    646c3106:	movsd  %xmm0,-0x18(%rbp)
-    646c310b:	mov    0x28(%rbp),%rax
-    646c310f:	movsd  0x18(%rax),%xmm0
-    646c3114:	movsd  -0x10(%rbp),%xmm1
-    646c3119:	mulsd  -0x18(%rbp),%xmm1
-    646c311e:	subsd  %xmm1,%xmm0
-    646c3122:	movapd %xmm0,%xmm1
-    646c3126:	mov    0x28(%rbp),%rax
-    646c312a:	movsd  0x20(%rax),%xmm0
-    646c312f:	mov    0x20(%rbp),%eax
-    646c3132:	imul   -0x4(%rbp),%eax
-    646c3136:	mov    -0x8(%rbp),%edx
-    646c3139:	add    %edx,%eax
-    646c313b:	cltq
-    646c313d:	lea    0x0(,%rax,8),%rdx
-    646c3145:	mov    0x18(%rbp),%rax
-    646c3149:	add    %rdx,%rax
-    646c314c:	addsd  %xmm1,%xmm0
-    646c3150:	movsd  %xmm0,(%rax)
-    646c3154:	addl   $0x1,-0x8(%rbp)
-    646c3158:	mov    -0x8(%rbp),%eax
-    646c315b:	cmp    0x20(%rbp),%eax
-    646c315e:	jl     646c3079 <cov_model2d+0x4b>
-    646c3164:	addl   $0x1,-0x4(%rbp)
-    646c3168:	mov    -0x4(%rbp),%eax
-    646c316b:	cmp    0x20(%rbp),%eax
-    646c316e:	jl     646c306d <cov_model2d+0x3f>
-    646c3174:	nop
-    646c3175:	add    $0x40,%rsp
-    646c3179:	pop    %rbp
-    646c317a:	ret
-    646c317b:	nop
-    646c317c:	nop
+    646c3068:	movl   $0x0,-0x8(%rbp)
+    646c306f:	jmp    646c316a <cov_model2d+0x13c>
+    646c3074:	movl   $0x0,-0xc(%rbp)
+    646c307b:	jmp    646c315a <cov_model2d+0x12c>
+    646c3080:	mov    -0x8(%rbp),%eax
+    646c3083:	cltq
+    646c3085:	lea    0x0(,%rax,8),%rdx
+    646c308d:	mov    0x10(%rbp),%rax
+    646c3091:	add    %rdx,%rax
+    646c3094:	mov    (%rax),%rdx
+    646c3097:	mov    -0xc(%rbp),%eax
+    646c309a:	cltq
+    646c309c:	shl    $0x3,%rax
+    646c30a0:	add    %rdx,%rax
+    646c30a3:	movsd  (%rax),%xmm1
+    646c30a7:	mov    -0x8(%rbp),%eax
+    646c30aa:	cltq
+    646c30ac:	lea    0x0(,%rax,8),%rdx
+    646c30b4:	mov    0x10(%rbp),%rax
+    646c30b8:	add    %rdx,%rax
+    646c30bb:	mov    (%rax),%rdx
+    646c30be:	mov    -0xc(%rbp),%eax
+    646c30c1:	cltq
+    646c30c3:	shl    $0x3,%rax
+    646c30c7:	add    %rdx,%rax
+    646c30ca:	movsd  (%rax),%xmm0
+    646c30ce:	mulsd  %xmm0,%xmm1
+    646c30d2:	movsd  0x5f76(%rip),%xmm0        # 646c9050 <.rdata>
+    646c30da:	mulsd  %xmm1,%xmm0
+    646c30de:	mov    0x28(%rbp),%rax
+    646c30e2:	movsd  0x10(%rax),%xmm2
+    646c30e7:	mov    0x28(%rbp),%rax
+    646c30eb:	movsd  0x10(%rax),%xmm1
+    646c30f0:	mulsd  %xmm2,%xmm1
+    646c30f4:	divsd  %xmm1,%xmm0
+    646c30f8:	call   646c68c0 <exp>
+    646c30fd:	movapd %xmm0,%xmm1
+    646c3101:	movsd  0x5f4f(%rip),%xmm0        # 646c9058 <.rdata+0x8>
+    646c3109:	subsd  %xmm1,%xmm0
+    646c310d:	movsd  %xmm0,-0x20(%rbp)
+    646c3112:	mov    0x28(%rbp),%rax
+    646c3116:	movsd  0x18(%rax),%xmm0
+    646c311b:	movsd  -0x18(%rbp),%xmm1
+    646c3120:	mulsd  -0x20(%rbp),%xmm1
+    646c3125:	subsd  %xmm1,%xmm0
+    646c3129:	movapd %xmm0,%xmm1
+    646c312d:	mov    0x28(%rbp),%rax
+    646c3131:	movsd  0x20(%rax),%xmm0
+    646c3136:	mov    -0x4(%rbp),%eax
+    646c3139:	cltq
+    646c313b:	lea    0x0(,%rax,8),%rdx
+    646c3143:	mov    0x18(%rbp),%rax
+    646c3147:	add    %rdx,%rax
+    646c314a:	addsd  %xmm1,%xmm0
+    646c314e:	movsd  %xmm0,(%rax)
+    646c3152:	addl   $0x1,-0x4(%rbp)
+    646c3156:	addl   $0x1,-0xc(%rbp)
+    646c315a:	mov    -0xc(%rbp),%eax
+    646c315d:	cmp    0x20(%rbp),%eax
+    646c3160:	jl     646c3080 <cov_model2d+0x52>
+    646c3166:	addl   $0x1,-0x8(%rbp)
+    646c316a:	mov    -0x8(%rbp),%eax
+    646c316d:	cmp    0x20(%rbp),%eax
+    646c3170:	jl     646c3074 <cov_model2d+0x46>
+    646c3176:	nop
+    646c3177:	add    $0x40,%rsp
+    646c317b:	pop    %rbp
+    646c317c:	ret
     646c317d:	nop
     646c317e:	nop
     646c317f:	nop
 
 00000000646c3180 <sampling_state_init>:
     646c3180:	push   %rbp
     646c3181:	mov    %rsp,%rbp
@@ -5061,15 +5058,15 @@
     646c31cc:	cltq
     646c31ce:	mov    0x10(%rbp),%rdx
     646c31d2:	mov    %rax,0x28(%rdx)
     646c31d6:	mov    0x18(%rbp),%eax
     646c31d9:	cltq
     646c31db:	mov    $0x8,%edx
     646c31e0:	mov    %rax,%rcx
-    646c31e3:	call   646c79b0 <calloc>
+    646c31e3:	call   646c76c0 <calloc>
     646c31e8:	mov    %rax,%rdx
     646c31eb:	mov    0x10(%rbp),%rax
     646c31ef:	mov    %rdx,0x18(%rax)
     646c31f3:	mov    0x18(%rbp),%eax
     646c31f6:	cltq
     646c31f8:	mov    0x10(%rbp),%rdx
     646c31fc:	mov    %rax,0x38(%rdx)
@@ -5077,15 +5074,15 @@
     646c3203:	cltq
     646c3205:	mov    0x10(%rbp),%rdx
     646c3209:	mov    %rax,0x40(%rdx)
     646c320d:	mov    0x18(%rbp),%eax
     646c3210:	cltq
     646c3212:	mov    $0x8,%edx
     646c3217:	mov    %rax,%rcx
-    646c321a:	call   646c79b0 <calloc>
+    646c321a:	call   646c76c0 <calloc>
     646c321f:	mov    %rax,%rdx
     646c3222:	mov    0x10(%rbp),%rax
     646c3226:	mov    %rdx,0x30(%rax)
     646c322a:	nop
     646c322b:	add    $0x20,%rsp
     646c322f:	pop    %rbp
     646c3230:	ret
@@ -5118,101 +5115,101 @@
     646c327d:	mov    -0x28(%rbp),%rax
     646c3281:	movsd  0x10(%rax),%xmm0
     646c3286:	movsd  %xmm0,0x8d9a(%rip)        # 646cc028 <k_range>
     646c328e:	movq   $0xa,0x8dbf(%rip)        # 646cc058 <location+0x8>
     646c3299:	movq   $0xa,0x8dbc(%rip)        # 646cc060 <location+0x10>
     646c32a4:	mov    $0x8,%edx
     646c32a9:	mov    $0xa,%ecx
-    646c32ae:	call   646c79b0 <calloc>
+    646c32ae:	call   646c76c0 <calloc>
     646c32b3:	mov    %rax,0x8d96(%rip)        # 646cc050 <location>
     646c32ba:	movq   $0xa,0x8db3(%rip)        # 646cc078 <loc_cov+0x8>
     646c32c5:	movq   $0xa,0x8db0(%rip)        # 646cc080 <loc_cov+0x10>
     646c32d0:	mov    $0x8,%edx
     646c32d5:	mov    $0xa,%ecx
-    646c32da:	call   646c79b0 <calloc>
+    646c32da:	call   646c76c0 <calloc>
     646c32df:	mov    %rax,0x8d8a(%rip)        # 646cc070 <loc_cov>
     646c32e6:	movq   $0xa,0x8dc7(%rip)        # 646cc0b8 <loc_cov2+0x8>
     646c32f1:	movq   $0xa,0x8dc4(%rip)        # 646cc0c0 <loc_cov2+0x10>
     646c32fc:	mov    $0x8,%edx
     646c3301:	mov    $0xa,%ecx
-    646c3306:	call   646c79b0 <calloc>
+    646c3306:	call   646c76c0 <calloc>
     646c330b:	mov    %rax,0x8d9e(%rip)        # 646cc0b0 <loc_cov2>
     646c3312:	movq   $0xa,0x8ddb(%rip)        # 646cc0f8 <weights+0x8>
     646c331d:	movq   $0xa,0x8dd8(%rip)        # 646cc100 <weights+0x10>
     646c3328:	mov    $0x8,%edx
     646c332d:	mov    $0xa,%ecx
-    646c3332:	call   646c79b0 <calloc>
+    646c3332:	call   646c76c0 <calloc>
     646c3337:	mov    %rax,0x8db2(%rip)        # 646cc0f0 <weights>
     646c333e:	movq   $0x64,0x8d8f(%rip)        # 646cc0d8 <flatten_temp+0x8>
     646c3349:	movq   $0x64,0x8d8c(%rip)        # 646cc0e0 <flatten_temp+0x10>
     646c3354:	mov    $0x8,%edx
     646c3359:	mov    $0x64,%ecx
-    646c335e:	call   646c79b0 <calloc>
+    646c335e:	call   646c76c0 <calloc>
     646c3363:	mov    %rax,0x8d66(%rip)        # 646cc0d0 <flatten_temp>
     646c336a:	movq   $0xa,0x8d23(%rip)        # 646cc098 <data_temp+0x8>
     646c3375:	movq   $0xa,0x8d20(%rip)        # 646cc0a0 <data_temp+0x10>
     646c3380:	mov    $0x8,%edx
     646c3385:	mov    $0xa,%ecx
-    646c338a:	call   646c79b0 <calloc>
+    646c338a:	call   646c76c0 <calloc>
     646c338f:	mov    %rax,0x8cfa(%rip)        # 646cc090 <data_temp>
     646c3396:	movq   $0xa,0x8d97(%rip)        # 646cc138 <pdist_temp+0x8>
     646c33a1:	movq   $0xa,0x8d94(%rip)        # 646cc140 <pdist_temp+0x10>
     646c33ac:	mov    $0x50,%ecx
-    646c33b1:	call   646c7970 <malloc>
+    646c33b1:	call   646c7680 <malloc>
     646c33b6:	mov    %rax,0x8d73(%rip)        # 646cc130 <pdist_temp>
     646c33bd:	movl   $0x0,-0x54(%rbp)
     646c33c4:	jmp    646c33eb <krige_param_setting+0x18e>
     646c33c6:	mov    0x8d63(%rip),%rdx        # 646cc130 <pdist_temp>
     646c33cd:	mov    -0x54(%rbp),%eax
     646c33d0:	cltq
     646c33d2:	shl    $0x3,%rax
     646c33d6:	lea    (%rdx,%rax,1),%rbx
     646c33da:	mov    $0x50,%ecx
-    646c33df:	call   646c7970 <malloc>
+    646c33df:	call   646c7680 <malloc>
     646c33e4:	mov    %rax,(%rbx)
     646c33e7:	addl   $0x1,-0x54(%rbp)
     646c33eb:	cmpl   $0x9,-0x54(%rbp)
     646c33ef:	jle    646c33c6 <krige_param_setting+0x169>
     646c33f1:	movq   $0xa,0x8d5c(%rip)        # 646cc158 <datacov+0x8>
     646c33fc:	movq   $0xa,0x8d59(%rip)        # 646cc160 <datacov+0x10>
     646c3407:	mov    $0x50,%ecx
-    646c340c:	call   646c7970 <malloc>
+    646c340c:	call   646c7680 <malloc>
     646c3411:	mov    %rax,0x8d38(%rip)        # 646cc150 <datacov>
     646c3418:	movl   $0x0,-0x58(%rbp)
     646c341f:	jmp    646c3446 <krige_param_setting+0x1e9>
     646c3421:	mov    0x8d28(%rip),%rdx        # 646cc150 <datacov>
     646c3428:	mov    -0x58(%rbp),%eax
     646c342b:	cltq
     646c342d:	shl    $0x3,%rax
     646c3431:	lea    (%rdx,%rax,1),%rbx
     646c3435:	mov    $0x50,%ecx
-    646c343a:	call   646c7970 <malloc>
+    646c343a:	call   646c7680 <malloc>
     646c343f:	mov    %rax,(%rbx)
     646c3442:	addl   $0x1,-0x58(%rbp)
     646c3446:	cmpl   $0x9,-0x58(%rbp)
     646c344a:	jle    646c3421 <krige_param_setting+0x1c4>
     646c344c:	mov    -0x30(%rbp),%eax
     646c344f:	cltq
     646c3451:	mov    %rax,0x8cc0(%rip)        # 646cc118 <array2d_temp+0x8>
     646c3458:	movq   $0x3,0x8cbd(%rip)        # 646cc120 <array2d_temp+0x10>
     646c3463:	mov    -0x30(%rbp),%eax
     646c3466:	cltq
     646c3468:	shl    $0x3,%rax
     646c346c:	mov    %rax,%rcx
-    646c346f:	call   646c7970 <malloc>
+    646c346f:	call   646c7680 <malloc>
     646c3474:	mov    %rax,0x8c95(%rip)        # 646cc110 <array2d_temp>
     646c347b:	movl   $0x0,-0x5c(%rbp)
     646c3482:	jmp    646c34a9 <krige_param_setting+0x24c>
     646c3484:	mov    0x8c85(%rip),%rdx        # 646cc110 <array2d_temp>
     646c348b:	mov    -0x5c(%rbp),%eax
     646c348e:	cltq
     646c3490:	shl    $0x3,%rax
     646c3494:	lea    (%rdx,%rax,1),%rbx
     646c3498:	mov    $0x18,%ecx
-    646c349d:	call   646c7970 <malloc>
+    646c349d:	call   646c7680 <malloc>
     646c34a2:	mov    %rax,(%rbx)
     646c34a5:	addl   $0x1,-0x5c(%rbp)
     646c34a9:	mov    -0x5c(%rbp),%eax
     646c34ac:	cmp    -0x30(%rbp),%eax
     646c34af:	jl     646c3484 <krige_param_setting+0x227>
     646c34b1:	nop
     646c34b2:	add    $0x38,%rsp
@@ -5301,15 +5298,15 @@
     646c35d7:	mov    0x18(%rbp),%rax
     646c35db:	mov    0x4(%rax),%eax
     646c35de:	lea    -0x1(%rax),%edx
     646c35e1:	mov    0x8b28(%rip),%rax        # 646cc110 <array2d_temp>
     646c35e8:	mov    %edx,%r8d
     646c35eb:	mov    $0x0,%edx
     646c35f0:	mov    %rax,%rcx
-    646c35f3:	call   646c50b1 <quicksort2d>
+    646c35f3:	call   646c4dd5 <quicksort2d>
     646c35f8:	movl   $0x0,-0x18(%rbp)
     646c35ff:	jmp    646c3668 <simple_kriging+0x1af>
     646c3601:	mov    0x8b08(%rip),%rdx        # 646cc110 <array2d_temp>
     646c3608:	mov    -0x18(%rbp),%eax
     646c360b:	cltq
     646c360d:	shl    $0x3,%rax
     646c3611:	add    %rdx,%rax
@@ -5446,15 +5443,15 @@
     646c384f:	mov    %rax,%rcx
     646c3852:	call   646c2e27 <mt19937_random_normal>
     646c3857:	movapd %xmm0,%xmm6
     646c385b:	mov    0x87d6(%rip),%rax        # 646cc038 <krige_var>
     646c3862:	movsd  0x57f6(%rip),%xmm0        # 646c9060 <.rdata>
     646c386a:	movapd %xmm0,%xmm1
     646c386e:	movq   %rax,%xmm0
-    646c3873:	call   646c6f60 <pow>
+    646c3873:	call   646c6c70 <pow>
     646c3878:	mulsd  %xmm6,%xmm0
     646c387c:	movsd  %xmm0,0x87bc(%rip)        # 646cc040 <fix>
     646c3884:	movsd  0x87a4(%rip),%xmm1        # 646cc030 <estimation>
     646c388c:	movsd  0x87ac(%rip),%xmm0        # 646cc040 <fix>
     646c3894:	mov    0x18(%rbp),%rax
     646c3898:	movsd  0x10(%rax),%xmm2
     646c389d:	cvttsd2si %xmm2,%eax
@@ -5585,87 +5582,87 @@
 
 00000000646c3a7b <krige_memory_free>:
     646c3a7b:	push   %rbp
     646c3a7c:	mov    %rsp,%rbp
     646c3a7f:	sub    $0x30,%rsp
     646c3a83:	mov    0x85c6(%rip),%rax        # 646cc050 <location>
     646c3a8a:	mov    %rax,%rcx
-    646c3a8d:	call   646c7988 <free>
+    646c3a8d:	call   646c7698 <free>
     646c3a92:	mov    0x85d7(%rip),%rax        # 646cc070 <loc_cov>
     646c3a99:	mov    %rax,%rcx
-    646c3a9c:	call   646c7988 <free>
+    646c3a9c:	call   646c7698 <free>
     646c3aa1:	mov    0x85e8(%rip),%rax        # 646cc090 <data_temp>
     646c3aa8:	mov    %rax,%rcx
-    646c3aab:	call   646c7988 <free>
+    646c3aab:	call   646c7698 <free>
     646c3ab0:	mov    0x85f9(%rip),%rax        # 646cc0b0 <loc_cov2>
     646c3ab7:	mov    %rax,%rcx
-    646c3aba:	call   646c7988 <free>
+    646c3aba:	call   646c7698 <free>
     646c3abf:	mov    0x860a(%rip),%rax        # 646cc0d0 <flatten_temp>
     646c3ac6:	mov    %rax,%rcx
-    646c3ac9:	call   646c7988 <free>
+    646c3ac9:	call   646c7698 <free>
     646c3ace:	mov    0x861b(%rip),%rax        # 646cc0f0 <weights>
     646c3ad5:	mov    %rax,%rcx
-    646c3ad8:	call   646c7988 <free>
+    646c3ad8:	call   646c7698 <free>
     646c3add:	movl   $0x0,-0x4(%rbp)
     646c3ae4:	jmp    646c3b08 <krige_memory_free+0x8d>
     646c3ae6:	mov    0x8623(%rip),%rdx        # 646cc110 <array2d_temp>
     646c3aed:	mov    -0x4(%rbp),%eax
     646c3af0:	cltq
     646c3af2:	shl    $0x3,%rax
     646c3af6:	add    %rdx,%rax
     646c3af9:	mov    (%rax),%rax
     646c3afc:	mov    %rax,%rcx
-    646c3aff:	call   646c7988 <free>
+    646c3aff:	call   646c7698 <free>
     646c3b04:	addl   $0x1,-0x4(%rbp)
     646c3b08:	mov    -0x4(%rbp),%eax
     646c3b0b:	cltq
     646c3b0d:	mov    0x8604(%rip),%rdx        # 646cc118 <array2d_temp+0x8>
     646c3b14:	cmp    %rdx,%rax
     646c3b17:	jb     646c3ae6 <krige_memory_free+0x6b>
     646c3b19:	mov    0x85f0(%rip),%rax        # 646cc110 <array2d_temp>
     646c3b20:	mov    %rax,%rcx
-    646c3b23:	call   646c7988 <free>
+    646c3b23:	call   646c7698 <free>
     646c3b28:	movl   $0x0,-0x8(%rbp)
     646c3b2f:	jmp    646c3b53 <krige_memory_free+0xd8>
     646c3b31:	mov    0x85f8(%rip),%rdx        # 646cc130 <pdist_temp>
     646c3b38:	mov    -0x8(%rbp),%eax
     646c3b3b:	cltq
     646c3b3d:	shl    $0x3,%rax
     646c3b41:	add    %rdx,%rax
     646c3b44:	mov    (%rax),%rax
     646c3b47:	mov    %rax,%rcx
-    646c3b4a:	call   646c7988 <free>
+    646c3b4a:	call   646c7698 <free>
     646c3b4f:	addl   $0x1,-0x8(%rbp)
     646c3b53:	mov    -0x8(%rbp),%eax
     646c3b56:	cltq
     646c3b58:	mov    0x85d9(%rip),%rdx        # 646cc138 <pdist_temp+0x8>
     646c3b5f:	cmp    %rdx,%rax
     646c3b62:	jb     646c3b31 <krige_memory_free+0xb6>
     646c3b64:	mov    0x85c5(%rip),%rax        # 646cc130 <pdist_temp>
     646c3b6b:	mov    %rax,%rcx
-    646c3b6e:	call   646c7988 <free>
+    646c3b6e:	call   646c7698 <free>
     646c3b73:	movl   $0x0,-0xc(%rbp)
     646c3b7a:	jmp    646c3b9e <krige_memory_free+0x123>
     646c3b7c:	mov    0x85cd(%rip),%rdx        # 646cc150 <datacov>
     646c3b83:	mov    -0xc(%rbp),%eax
     646c3b86:	cltq
     646c3b88:	shl    $0x3,%rax
     646c3b8c:	add    %rdx,%rax
     646c3b8f:	mov    (%rax),%rax
     646c3b92:	mov    %rax,%rcx
-    646c3b95:	call   646c7988 <free>
+    646c3b95:	call   646c7698 <free>
     646c3b9a:	addl   $0x1,-0xc(%rbp)
     646c3b9e:	mov    -0xc(%rbp),%eax
     646c3ba1:	cltq
     646c3ba3:	mov    0x85ae(%rip),%rdx        # 646cc158 <datacov+0x8>
     646c3baa:	cmp    %rdx,%rax
     646c3bad:	jb     646c3b7c <krige_memory_free+0x101>
     646c3baf:	mov    0x859a(%rip),%rax        # 646cc150 <datacov>
     646c3bb6:	mov    %rax,%rcx
-    646c3bb9:	call   646c7988 <free>
+    646c3bb9:	call   646c7698 <free>
     646c3bbe:	nop
     646c3bbf:	add    $0x30,%rsp
     646c3bc3:	pop    %rbp
     646c3bc4:	ret
     646c3bc5:	nop
     646c3bc6:	nop
     646c3bc7:	nop
@@ -5691,15 +5688,15 @@
     646c3bf0:	mov    -0x10(%rbp),%rcx
     646c3bf4:	mov    0x20(%rbp),%rdx
     646c3bf8:	mov    0x18(%rbp),%rax
     646c3bfc:	mov    %rcx,%r9
     646c3bff:	mov    %rdx,%r8
     646c3c02:	mov    %rax,%rdx
     646c3c05:	mov    0x10(%rbp),%rcx
-    646c3c09:	call   646c6990 <__ms_vsnprintf>
+    646c3c09:	call   646c66a0 <__ms_vsnprintf>
     646c3c0e:	mov    %eax,-0x4(%rbp)
     646c3c11:	mov    -0x4(%rbp),%eax
     646c3c14:	add    $0x30,%rsp
     646c3c18:	pop    %rbp
     646c3c19:	ret
 
 00000000646c3c1a <lu_inverse_solver>:
@@ -5710,43 +5707,43 @@
     646c3c2b:	mov    %rcx,0x70(%rbp)
     646c3c2f:	mov    %rdx,0x78(%rbp)
     646c3c33:	mov    %r8,0x80(%rbp)
     646c3c3a:	mov    %r9d,0x88(%rbp)
     646c3c41:	movq   $0xa,0x18(%rbp)
     646c3c49:	movq   $0xa,0x20(%rbp)
     646c3c51:	mov    $0x50,%ecx
-    646c3c56:	call   646c7970 <malloc>
+    646c3c56:	call   646c7680 <malloc>
     646c3c5b:	mov    %rax,0x10(%rbp)
     646c3c5f:	movl   $0x0,0x4c(%rbp)
     646c3c66:	jmp    646c3c8a <lu_inverse_solver+0x70>
     646c3c68:	mov    0x10(%rbp),%rdx
     646c3c6c:	mov    0x4c(%rbp),%eax
     646c3c6f:	cltq
     646c3c71:	shl    $0x3,%rax
     646c3c75:	lea    (%rdx,%rax,1),%rbx
     646c3c79:	mov    $0x50,%ecx
-    646c3c7e:	call   646c7970 <malloc>
+    646c3c7e:	call   646c7680 <malloc>
     646c3c83:	mov    %rax,(%rbx)
     646c3c86:	addl   $0x1,0x4c(%rbp)
     646c3c8a:	cmpl   $0x9,0x4c(%rbp)
     646c3c8e:	jle    646c3c68 <lu_inverse_solver+0x4e>
     646c3c90:	movq   $0xa,-0x8(%rbp)
     646c3c98:	movq   $0xa,0x0(%rbp)
     646c3ca0:	mov    $0x50,%ecx
-    646c3ca5:	call   646c7970 <malloc>
+    646c3ca5:	call   646c7680 <malloc>
     646c3caa:	mov    %rax,-0x10(%rbp)
     646c3cae:	movl   $0x0,0x48(%rbp)
     646c3cb5:	jmp    646c3cd9 <lu_inverse_solver+0xbf>
     646c3cb7:	mov    -0x10(%rbp),%rdx
     646c3cbb:	mov    0x48(%rbp),%eax
     646c3cbe:	cltq
     646c3cc0:	shl    $0x3,%rax
     646c3cc4:	lea    (%rdx,%rax,1),%rbx
     646c3cc8:	mov    $0x50,%ecx
-    646c3ccd:	call   646c7970 <malloc>
+    646c3ccd:	call   646c7680 <malloc>
     646c3cd2:	mov    %rax,(%rbx)
     646c3cd5:	addl   $0x1,0x48(%rbp)
     646c3cd9:	cmpl   $0x9,0x48(%rbp)
     646c3cdd:	jle    646c3cb7 <lu_inverse_solver+0x9d>
     646c3cdf:	mov    -0x10(%rbp),%rdx
     646c3ce3:	mov    0x10(%rbp),%rax
     646c3ce7:	mov    0x88(%rbp),%ecx
@@ -5892,43 +5889,43 @@
     646c3f12:	mov    0x10(%rbp),%rdx
     646c3f16:	mov    0x34(%rbp),%eax
     646c3f19:	cltq
     646c3f1b:	shl    $0x3,%rax
     646c3f1f:	add    %rdx,%rax
     646c3f22:	mov    (%rax),%rax
     646c3f25:	mov    %rax,%rcx
-    646c3f28:	call   646c7988 <free>
+    646c3f28:	call   646c7698 <free>
     646c3f2d:	addl   $0x1,0x34(%rbp)
     646c3f31:	mov    0x34(%rbp),%eax
     646c3f34:	cltq
     646c3f36:	mov    0x18(%rbp),%rdx
     646c3f3a:	cmp    %rdx,%rax
     646c3f3d:	jb     646c3f12 <lu_inverse_solver+0x2f8>
     646c3f3f:	mov    0x10(%rbp),%rax
     646c3f43:	mov    %rax,%rcx
-    646c3f46:	call   646c7988 <free>
+    646c3f46:	call   646c7698 <free>
     646c3f4b:	movl   $0x0,0x30(%rbp)
     646c3f52:	jmp    646c3f73 <lu_inverse_solver+0x359>
     646c3f54:	mov    -0x10(%rbp),%rdx
     646c3f58:	mov    0x30(%rbp),%eax
     646c3f5b:	cltq
     646c3f5d:	shl    $0x3,%rax
     646c3f61:	add    %rdx,%rax
     646c3f64:	mov    (%rax),%rax
     646c3f67:	mov    %rax,%rcx
-    646c3f6a:	call   646c7988 <free>
+    646c3f6a:	call   646c7698 <free>
     646c3f6f:	addl   $0x1,0x30(%rbp)
     646c3f73:	mov    0x30(%rbp),%eax
     646c3f76:	cltq
     646c3f78:	mov    -0x8(%rbp),%rdx
     646c3f7c:	cmp    %rdx,%rax
     646c3f7f:	jb     646c3f54 <lu_inverse_solver+0x33a>
     646c3f81:	mov    -0x10(%rbp),%rax
     646c3f85:	mov    %rax,%rcx
-    646c3f88:	call   646c7988 <free>
+    646c3f88:	call   646c7698 <free>
     646c3f8d:	nop
     646c3f8e:	add    $0xd8,%rsp
     646c3f95:	pop    %rbx
     646c3f96:	pop    %rbp
     646c3f97:	ret
 
 00000000646c3f98 <lu_decomposition>:
@@ -6187,15 +6184,15 @@
     646c432a:	mov    %rsp,%rbp
     646c432d:	sub    $0x30,%rsp
     646c4331:	mov    %ecx,0x10(%rbp)
     646c4334:	mov    0x10(%rbp),%eax
     646c4337:	cltq
     646c4339:	shl    $0x2,%rax
     646c433d:	mov    %rax,%rcx
-    646c4340:	call   646c7970 <malloc>
+    646c4340:	call   646c7680 <malloc>
     646c4345:	mov    %rax,-0x10(%rbp)
     646c4349:	movl   $0x0,-0x4(%rbp)
     646c4350:	jmp    646c436f <arange+0x46>
     646c4352:	mov    -0x4(%rbp),%eax
     646c4355:	cltq
     646c4357:	lea    0x0(,%rax,4),%rdx
     646c435f:	mov    -0x10(%rbp),%rax
@@ -6216,15 +6213,15 @@
     646c4382:	mov    %rsp,%rbp
     646c4385:	sub    $0x30,%rsp
     646c4389:	mov    %ecx,0x10(%rbp)
     646c438c:	mov    0x10(%rbp),%eax
     646c438f:	cltq
     646c4391:	shl    $0x3,%rax
     646c4395:	mov    %rax,%rcx
-    646c4398:	call   646c7970 <malloc>
+    646c4398:	call   646c7680 <malloc>
     646c439d:	mov    %rax,-0x10(%rbp)
     646c43a1:	movl   $0x0,-0x4(%rbp)
     646c43a8:	jmp    646c43cb <d_arange+0x4a>
     646c43aa:	mov    -0x4(%rbp),%eax
     646c43ad:	cltq
     646c43af:	lea    0x0(,%rax,8),%rdx
     646c43b7:	mov    -0x10(%rbp),%rax
@@ -6294,141 +6291,138 @@
     646c4490:	push   %rbp
     646c4491:	mov    %rsp,%rbp
     646c4494:	sub    $0x10,%rsp
     646c4498:	mov    %rcx,0x10(%rbp)
     646c449c:	mov    %rdx,0x18(%rbp)
     646c44a0:	mov    %r8d,0x20(%rbp)
     646c44a4:	movl   $0x0,-0x4(%rbp)
-    646c44ab:	jmp    646c450e <matrixform+0x7e>
-    646c44ad:	movl   $0x0,-0x8(%rbp)
-    646c44b4:	jmp    646c4502 <matrixform+0x72>
-    646c44b6:	mov    0x20(%rbp),%eax
-    646c44b9:	imul   -0x4(%rbp),%eax
-    646c44bd:	mov    -0x8(%rbp),%edx
-    646c44c0:	add    %edx,%eax
-    646c44c2:	cltq
-    646c44c4:	lea    0x0(,%rax,8),%rdx
-    646c44cc:	mov    0x10(%rbp),%rax
-    646c44d0:	add    %rax,%rdx
-    646c44d3:	mov    -0x4(%rbp),%eax
-    646c44d6:	cltq
-    646c44d8:	lea    0x0(,%rax,8),%rcx
-    646c44e0:	mov    0x18(%rbp),%rax
-    646c44e4:	add    %rcx,%rax
-    646c44e7:	mov    (%rax),%rcx
-    646c44ea:	mov    -0x8(%rbp),%eax
-    646c44ed:	cltq
-    646c44ef:	shl    $0x3,%rax
-    646c44f3:	add    %rcx,%rax
-    646c44f6:	movsd  (%rdx),%xmm0
-    646c44fa:	movsd  %xmm0,(%rax)
-    646c44fe:	addl   $0x1,-0x8(%rbp)
-    646c4502:	mov    -0x8(%rbp),%eax
-    646c4505:	cmp    0x20(%rbp),%eax
-    646c4508:	jl     646c44b6 <matrixform+0x26>
-    646c450a:	addl   $0x1,-0x4(%rbp)
-    646c450e:	mov    -0x4(%rbp),%eax
-    646c4511:	cmp    0x20(%rbp),%eax
-    646c4514:	jl     646c44ad <matrixform+0x1d>
-    646c4516:	nop
-    646c4517:	add    $0x10,%rsp
-    646c451b:	pop    %rbp
-    646c451c:	ret
-
-00000000646c451d <save_1darray>:
-    646c451d:	push   %rbp
-    646c451e:	sub    $0x1e0,%rsp
-    646c4525:	lea    0x80(%rsp),%rbp
-    646c452d:	mov    %rcx,0x170(%rbp)
-    646c4534:	mov    %edx,0x178(%rbp)
-    646c453a:	mov    %r8,0x180(%rbp)
-    646c4541:	mov    %r9,0x188(%rbp)
-    646c4548:	cvtsi2sdl 0x190(%rbp),%xmm0
-    646c4550:	call   646c7978 <log10>
-    646c4555:	movq   %xmm0,%rax
-    646c455a:	movq   %rax,%xmm0
-    646c455f:	call   646c69a0 <ceil>
-    646c4564:	cvttsd2si %xmm0,%eax
-    646c4568:	add    $0x1,%eax
-    646c456b:	mov    %eax,0x158(%rbp)
-    646c4571:	mov    0x188(%rbp),%rcx
-    646c4578:	lea    0x80(%rbp),%rax
-    646c457f:	mov    0x158(%rbp),%edx
-    646c4585:	mov    %edx,0x28(%rsp)
-    646c4589:	mov    0x180(%rbp),%rdx
-    646c4590:	mov    %rdx,0x20(%rsp)
-    646c4595:	mov    %rcx,%r9
-    646c4598:	lea    0x4af1(%rip),%r8        # 646c9090 <.rdata>
-    646c459f:	mov    $0xc8,%edx
-    646c45a4:	mov    %rax,%rcx
-    646c45a7:	call   646c3bd0 <snprintf>
-    646c45ac:	mov    0x188(%rbp),%rax
-    646c45b3:	mov    %rax,%rcx
-    646c45b6:	call   646c79c8 <_mkdir>
-    646c45bb:	cmp    $0xffffffff,%eax
-    646c45be:	jne    646c45dc <save_1darray+0xbf>
-    646c45c0:	mov    0x9cd5(%rip),%rax        # 646ce29c <__imp__errno>
-    646c45c7:	call   *%rax
-    646c45c9:	mov    (%rax),%eax
-    646c45cb:	cmp    $0x11,%eax
-    646c45ce:	je     646c45dc <save_1darray+0xbf>
-    646c45d0:	lea    0x4ac8(%rip),%rcx        # 646c909f <.rdata+0xf>
-    646c45d7:	call   646c7960 <printf>
-    646c45dc:	mov    0x198(%rbp),%ecx
-    646c45e2:	lea    0x80(%rbp),%rdx
-    646c45e9:	lea    -0x50(%rbp),%rax
-    646c45ed:	mov    %ecx,%r9d
-    646c45f0:	mov    %rdx,%r8
-    646c45f3:	mov    $0xc8,%edx
-    646c45f8:	mov    %rax,%rcx
-    646c45fb:	call   646c3bd0 <snprintf>
-    646c4600:	lea    -0x50(%rbp),%rax
-    646c4604:	lea    0x4aaa(%rip),%rdx        # 646c90b5 <.rdata+0x25>
-    646c460b:	mov    %rax,%rcx
-    646c460e:	call   646c7998 <fopen>
-    646c4613:	mov    %rax,0x150(%rbp)
-    646c461a:	cmpq   $0x0,0x150(%rbp)
-    646c4622:	jne    646c463a <save_1darray+0x11d>
-    646c4624:	lea    0x4a8c(%rip),%rcx        # 646c90b7 <.rdata+0x27>
-    646c462b:	call   646c7968 <perror>
-    646c4630:	mov    $0x1,%ecx
-    646c4635:	call   646c79a8 <exit>
-    646c463a:	movl   $0x0,0x15c(%rbp)
-    646c4644:	jmp    646c46a4 <save_1darray+0x187>
-    646c4646:	mov    0x15c(%rbp),%eax
-    646c464c:	cltq
-    646c464e:	lea    0x0(,%rax,8),%rdx
-    646c4656:	mov    0x170(%rbp),%rax
-    646c465d:	add    %rdx,%rax
-    646c4660:	movsd  (%rax),%xmm0
-    646c4664:	movq   %xmm0,%rax
-    646c4669:	mov    %rax,%rdx
-    646c466c:	mov    %rdx,%rcx
-    646c466f:	movq   %rax,%xmm0
-    646c4674:	mov    0x15c(%rbp),%edx
-    646c467a:	mov    0x150(%rbp),%rax
-    646c4681:	movq   %rcx,%xmm3
-    646c4686:	movq   %xmm0,%r9
-    646c468b:	mov    %edx,%r8d
-    646c468e:	lea    0x4a3a(%rip),%rdx        # 646c90cf <.rdata+0x3f>
-    646c4695:	mov    %rax,%rcx
-    646c4698:	call   646c7990 <fprintf>
-    646c469d:	addl   $0x1,0x15c(%rbp)
-    646c46a4:	mov    0x15c(%rbp),%eax
-    646c46aa:	cmp    0x178(%rbp),%eax
-    646c46b0:	jl     646c4646 <save_1darray+0x129>
-    646c46b2:	mov    0x150(%rbp),%rax
-    646c46b9:	mov    %rax,%rcx
-    646c46bc:	call   646c79a0 <fclose>
-    646c46c1:	nop
-    646c46c2:	add    $0x1e0,%rsp
-    646c46c9:	pop    %rbp
-    646c46ca:	ret
-    646c46cb:	nop
-    646c46cc:	nop
+    646c44ab:	movl   $0x0,-0x8(%rbp)
+    646c44b2:	jmp    646c4510 <matrixform+0x80>
+    646c44b4:	movl   $0x0,-0xc(%rbp)
+    646c44bb:	jmp    646c4504 <matrixform+0x74>
+    646c44bd:	mov    -0x4(%rbp),%eax
+    646c44c0:	cltq
+    646c44c2:	lea    0x0(,%rax,8),%rdx
+    646c44ca:	mov    0x10(%rbp),%rax
+    646c44ce:	add    %rax,%rdx
+    646c44d1:	mov    -0x8(%rbp),%eax
+    646c44d4:	cltq
+    646c44d6:	lea    0x0(,%rax,8),%rcx
+    646c44de:	mov    0x18(%rbp),%rax
+    646c44e2:	add    %rcx,%rax
+    646c44e5:	mov    (%rax),%rcx
+    646c44e8:	mov    -0xc(%rbp),%eax
+    646c44eb:	cltq
+    646c44ed:	shl    $0x3,%rax
+    646c44f1:	add    %rcx,%rax
+    646c44f4:	movsd  (%rdx),%xmm0
+    646c44f8:	movsd  %xmm0,(%rax)
+    646c44fc:	addl   $0x1,-0x4(%rbp)
+    646c4500:	addl   $0x1,-0xc(%rbp)
+    646c4504:	mov    -0xc(%rbp),%eax
+    646c4507:	cmp    0x20(%rbp),%eax
+    646c450a:	jl     646c44bd <matrixform+0x2d>
+    646c450c:	addl   $0x1,-0x8(%rbp)
+    646c4510:	mov    -0x8(%rbp),%eax
+    646c4513:	cmp    0x20(%rbp),%eax
+    646c4516:	jl     646c44b4 <matrixform+0x24>
+    646c4518:	nop
+    646c4519:	add    $0x10,%rsp
+    646c451d:	pop    %rbp
+    646c451e:	ret
+
+00000000646c451f <save_1darray>:
+    646c451f:	push   %rbp
+    646c4520:	sub    $0x1e0,%rsp
+    646c4527:	lea    0x80(%rsp),%rbp
+    646c452f:	mov    %rcx,0x170(%rbp)
+    646c4536:	mov    %edx,0x178(%rbp)
+    646c453c:	mov    %r8,0x180(%rbp)
+    646c4543:	mov    %r9,0x188(%rbp)
+    646c454a:	cvtsi2sdl 0x190(%rbp),%xmm0
+    646c4552:	call   646c7688 <log10>
+    646c4557:	movq   %xmm0,%rax
+    646c455c:	movq   %rax,%xmm0
+    646c4561:	call   646c66b0 <ceil>
+    646c4566:	cvttsd2si %xmm0,%eax
+    646c456a:	add    $0x1,%eax
+    646c456d:	mov    %eax,0x158(%rbp)
+    646c4573:	mov    0x188(%rbp),%rcx
+    646c457a:	lea    0x80(%rbp),%rax
+    646c4581:	mov    0x158(%rbp),%edx
+    646c4587:	mov    %edx,0x28(%rsp)
+    646c458b:	mov    0x180(%rbp),%rdx
+    646c4592:	mov    %rdx,0x20(%rsp)
+    646c4597:	mov    %rcx,%r9
+    646c459a:	lea    0x4aef(%rip),%r8        # 646c9090 <.rdata>
+    646c45a1:	mov    $0xc8,%edx
+    646c45a6:	mov    %rax,%rcx
+    646c45a9:	call   646c3bd0 <snprintf>
+    646c45ae:	mov    0x188(%rbp),%rax
+    646c45b5:	mov    %rax,%rcx
+    646c45b8:	call   646c76d8 <_mkdir>
+    646c45bd:	cmp    $0xffffffff,%eax
+    646c45c0:	jne    646c45de <save_1darray+0xbf>
+    646c45c2:	mov    0x9cd3(%rip),%rax        # 646ce29c <__imp__errno>
+    646c45c9:	call   *%rax
+    646c45cb:	mov    (%rax),%eax
+    646c45cd:	cmp    $0x11,%eax
+    646c45d0:	je     646c45de <save_1darray+0xbf>
+    646c45d2:	lea    0x4ac6(%rip),%rcx        # 646c909f <.rdata+0xf>
+    646c45d9:	call   646c7670 <printf>
+    646c45de:	mov    0x198(%rbp),%ecx
+    646c45e4:	lea    0x80(%rbp),%rdx
+    646c45eb:	lea    -0x50(%rbp),%rax
+    646c45ef:	mov    %ecx,%r9d
+    646c45f2:	mov    %rdx,%r8
+    646c45f5:	mov    $0xc8,%edx
+    646c45fa:	mov    %rax,%rcx
+    646c45fd:	call   646c3bd0 <snprintf>
+    646c4602:	lea    -0x50(%rbp),%rax
+    646c4606:	lea    0x4aa8(%rip),%rdx        # 646c90b5 <.rdata+0x25>
+    646c460d:	mov    %rax,%rcx
+    646c4610:	call   646c76a8 <fopen>
+    646c4615:	mov    %rax,0x150(%rbp)
+    646c461c:	cmpq   $0x0,0x150(%rbp)
+    646c4624:	jne    646c463c <save_1darray+0x11d>
+    646c4626:	lea    0x4a8a(%rip),%rcx        # 646c90b7 <.rdata+0x27>
+    646c462d:	call   646c7678 <perror>
+    646c4632:	mov    $0x1,%ecx
+    646c4637:	call   646c76b8 <exit>
+    646c463c:	movl   $0x0,0x15c(%rbp)
+    646c4646:	jmp    646c46a6 <save_1darray+0x187>
+    646c4648:	mov    0x15c(%rbp),%eax
+    646c464e:	cltq
+    646c4650:	lea    0x0(,%rax,8),%rdx
+    646c4658:	mov    0x170(%rbp),%rax
+    646c465f:	add    %rdx,%rax
+    646c4662:	movsd  (%rax),%xmm0
+    646c4666:	movq   %xmm0,%rax
+    646c466b:	mov    %rax,%rdx
+    646c466e:	mov    %rdx,%rcx
+    646c4671:	movq   %rax,%xmm0
+    646c4676:	mov    0x15c(%rbp),%edx
+    646c467c:	mov    0x150(%rbp),%rax
+    646c4683:	movq   %rcx,%xmm3
+    646c4688:	movq   %xmm0,%r9
+    646c468d:	mov    %edx,%r8d
+    646c4690:	lea    0x4a38(%rip),%rdx        # 646c90cf <.rdata+0x3f>
+    646c4697:	mov    %rax,%rcx
+    646c469a:	call   646c76a0 <fprintf>
+    646c469f:	addl   $0x1,0x15c(%rbp)
+    646c46a6:	mov    0x15c(%rbp),%eax
+    646c46ac:	cmp    0x178(%rbp),%eax
+    646c46b2:	jl     646c4648 <save_1darray+0x129>
+    646c46b4:	mov    0x150(%rbp),%rax
+    646c46bb:	mov    %rax,%rcx
+    646c46be:	call   646c76b0 <fclose>
+    646c46c3:	nop
+    646c46c4:	add    $0x1e0,%rsp
+    646c46cb:	pop    %rbp
+    646c46cc:	ret
     646c46cd:	nop
     646c46ce:	nop
     646c46cf:	nop
 
 00000000646c46d0 <randompath>:
     646c46d0:	push   %rbp
     646c46d1:	mov    %rsp,%rbp
@@ -6497,4175 +6491,3970 @@
     646c47a0:	mov    0x10(%rbp),%rax
     646c47a4:	mov    0x20(%rbp),%edx
     646c47a7:	mov    %edx,0x4(%rax)
     646c47aa:	mov    0x10(%rbp),%rax
     646c47ae:	mov    0x28(%rbp),%edx
     646c47b1:	mov    %edx,0x8(%rax)
     646c47b4:	cmpl   $0x1,0x30(%rbp)
-    646c47b8:	jne    646c47de <sgsim_init+0x5e>
+    646c47b8:	jne    646c47df <sgsim_init+0x5f>
     646c47ba:	mov    0x18(%rbp),%eax
     646c47bd:	imul   0x20(%rbp),%eax
     646c47c1:	mov    %eax,-0x4(%rbp)
     646c47c4:	mov    -0x4(%rbp),%eax
-    646c47c7:	shl    $0x3,%rax
-    646c47cb:	mov    %rax,%rcx
-    646c47ce:	call   646c7970 <malloc>
-    646c47d3:	mov    %rax,%rdx
-    646c47d6:	mov    0x10(%rbp),%rax
-    646c47da:	mov    %rdx,0x10(%rax)
-    646c47de:	nop
-    646c47df:	add    $0x30,%rsp
-    646c47e3:	pop    %rbp
-    646c47e4:	ret
-
-00000000646c47e5 <sgsim_run>:
-    646c47e5:	push   %rbp
-    646c47e6:	sub    $0xa00,%rsp
-    646c47ed:	lea    0x80(%rsp),%rbp
-    646c47f5:	mov    %rcx,0x990(%rbp)
-    646c47fc:	mov    %rdx,0x998(%rbp)
-    646c4803:	mov    %r8d,0x9a0(%rbp)
-    646c480a:	mov    0x990(%rbp),%rax
-    646c4811:	mov    0x8(%rax),%eax
-    646c4814:	mov    %eax,%edx
-    646c4816:	lea    -0x50(%rbp),%rax
-    646c481a:	mov    %rax,%rcx
-    646c481d:	call   646c2a30 <mt19937_init>
-    646c4822:	mov    0x990(%rbp),%rax
-    646c4829:	mov    (%rax),%eax
-    646c482b:	mov    %eax,%edx
-    646c482d:	lea    0x79ec(%rip),%rcx        # 646cc220 <_sampling>
-    646c4834:	call   646c3180 <sampling_state_init>
-    646c4839:	mov    0x998(%rbp),%rax
-    646c4840:	mov    0x8(%rax),%eax
-    646c4843:	cltq
-    646c4845:	mov    %rax,0x799c(%rip)        # 646cc1e8 <variogram_array+0x8>
-    646c484c:	mov    0x998(%rbp),%rax
-    646c4853:	mov    0x8(%rax),%eax
-    646c4856:	cltq
-    646c4858:	mov    %rax,0x7991(%rip)        # 646cc1f0 <variogram_array+0x10>
-    646c485f:	mov    0x998(%rbp),%rax
-    646c4866:	mov    0x8(%rax),%eax
-    646c4869:	cltq
-    646c486b:	mov    $0x8,%edx
-    646c4870:	mov    %rax,%rcx
-    646c4873:	call   646c79b0 <calloc>
-    646c4878:	mov    %rax,0x7961(%rip)        # 646cc1e0 <variogram_array>
-    646c487f:	mov    0x990(%rbp),%rax
-    646c4886:	mov    (%rax),%eax
-    646c4888:	cltq
-    646c488a:	mov    %rax,0x7977(%rip)        # 646cc208 <sgsim_array+0x8>
-    646c4891:	mov    0x990(%rbp),%rax
-    646c4898:	mov    (%rax),%eax
-    646c489a:	cltq
-    646c489c:	mov    %rax,0x796d(%rip)        # 646cc210 <sgsim_array+0x10>
-    646c48a3:	mov    0x990(%rbp),%rax
-    646c48aa:	mov    (%rax),%eax
-    646c48ac:	cltq
-    646c48ae:	mov    $0x8,%edx
-    646c48b3:	mov    %rax,%rcx
-    646c48b6:	call   646c79b0 <calloc>
-    646c48bb:	mov    %rax,0x793e(%rip)        # 646cc200 <sgsim_array>
-    646c48c2:	mov    0x990(%rbp),%rax
-    646c48c9:	mov    (%rax),%eax
-    646c48cb:	mov    0x998(%rbp),%rdx
-    646c48d2:	mov    %eax,%ecx
-    646c48d4:	call   646c325d <krige_param_setting>
-    646c48d9:	mov    0x990(%rbp),%rax
-    646c48e0:	mov    (%rax),%eax
-    646c48e2:	mov    %eax,%ecx
-    646c48e4:	call   646c4329 <arange>
-    646c48e9:	mov    %rax,0x7890(%rip)        # 646cc180 <x_grid>
-    646c48f0:	movl   $0x0,0x7972(%rip)        # 646cc26c <count>
-    646c48fa:	jmp    646c4c6f <sgsim_run+0x48a>
-    646c48ff:	mov    0x7967(%rip),%eax        # 646cc26c <count>
-    646c4905:	mov    %eax,%edx
-    646c4907:	lea    0x47f2(%rip),%rcx        # 646c9100 <.rdata>
-    646c490e:	call   646c7960 <printf>
-    646c4913:	movl   $0x0,0x7907(%rip)        # 646cc224 <_sampling+0x4>
-    646c491d:	movl   $0x0,0x78f9(%rip)        # 646cc220 <_sampling>
-    646c4927:	movl   $0x0,0x7937(%rip)        # 646cc268 <flag>
-    646c4931:	mov    0x990(%rbp),%rax
-    646c4938:	mov    (%rax),%edx
-    646c493a:	mov    0x783f(%rip),%rax        # 646cc180 <x_grid>
-    646c4941:	lea    -0x50(%rbp),%rcx
-    646c4945:	mov    %rcx,%r8
-    646c4948:	mov    %rax,%rcx
-    646c494b:	call   646c46d0 <randompath>
-    646c4950:	mov    %rax,0x7829(%rip)        # 646cc180 <x_grid>
-    646c4957:	movl   $0x0,0x97c(%rbp)
-    646c4961:	jmp    646c49c8 <sgsim_run+0x1e3>
-    646c4963:	mov    0x7896(%rip),%rdx        # 646cc200 <sgsim_array>
-    646c496a:	mov    0x97c(%rbp),%eax
-    646c4970:	cltq
-    646c4972:	shl    $0x3,%rax
-    646c4976:	add    %rdx,%rax
-    646c4979:	pxor   %xmm0,%xmm0
-    646c497d:	movsd  %xmm0,(%rax)
-    646c4981:	mov    0x78b0(%rip),%rdx        # 646cc238 <_sampling+0x18>
-    646c4988:	mov    0x97c(%rbp),%eax
-    646c498e:	cltq
-    646c4990:	shl    $0x3,%rax
-    646c4994:	add    %rdx,%rax
-    646c4997:	pxor   %xmm0,%xmm0
-    646c499b:	movsd  %xmm0,(%rax)
-    646c499f:	mov    0x78aa(%rip),%rdx        # 646cc250 <_sampling+0x30>
-    646c49a6:	mov    0x97c(%rbp),%eax
-    646c49ac:	cltq
-    646c49ae:	shl    $0x3,%rax
-    646c49b2:	add    %rdx,%rax
-    646c49b5:	movsd  0x4793(%rip),%xmm0        # 646c9150 <.rdata+0x50>
-    646c49bd:	movsd  %xmm0,(%rax)
-    646c49c1:	addl   $0x1,0x97c(%rbp)
-    646c49c8:	mov    0x990(%rbp),%rax
-    646c49cf:	mov    (%rax),%eax
-    646c49d1:	cmp    %eax,0x97c(%rbp)
-    646c49d7:	jl     646c4963 <sgsim_run+0x17e>
-    646c49d9:	movl   $0x0,0x978(%rbp)
-    646c49e3:	jmp    646c4b61 <sgsim_run+0x37c>
-    646c49e8:	mov    0x7791(%rip),%rdx        # 646cc180 <x_grid>
-    646c49ef:	mov    0x978(%rbp),%eax
-    646c49f5:	cltq
-    646c49f7:	shl    $0x2,%rax
-    646c49fb:	add    %rdx,%rax
-    646c49fe:	mov    (%rax),%eax
-    646c4a00:	cvtsi2sd %eax,%xmm0
-    646c4a04:	mov    0x978(%rbp),%eax
-    646c4a0a:	mov    %eax,%r8d
-    646c4a0d:	movapd %xmm0,%xmm1
-    646c4a11:	lea    0x7808(%rip),%rcx        # 646cc220 <_sampling>
-    646c4a18:	call   646c3231 <sampling_state_update>
-    646c4a1d:	mov    0x77dc(%rip),%rax        # 646cc200 <sgsim_array>
-    646c4a24:	lea    -0x50(%rbp),%rdx
-    646c4a28:	mov    %rdx,%r8
-    646c4a2b:	lea    0x77ee(%rip),%rdx        # 646cc220 <_sampling>
-    646c4a32:	mov    %rax,%rcx
-    646c4a35:	call   646c34b9 <simple_kriging>
-    646c4a3a:	mov    0x77bf(%rip),%rdx        # 646cc200 <sgsim_array>
-    646c4a41:	mov    0x7738(%rip),%rcx        # 646cc180 <x_grid>
-    646c4a48:	mov    0x978(%rbp),%eax
-    646c4a4e:	cltq
-    646c4a50:	shl    $0x2,%rax
-    646c4a54:	add    %rcx,%rax
-    646c4a57:	mov    (%rax),%eax
-    646c4a59:	cltq
-    646c4a5b:	shl    $0x3,%rax
-    646c4a5f:	add    %rax,%rdx
-    646c4a62:	mov    0x990(%rbp),%rax
-    646c4a69:	mov    0x10(%rax),%rcx
-    646c4a6d:	mov    0x770c(%rip),%r8        # 646cc180 <x_grid>
-    646c4a74:	mov    0x978(%rbp),%eax
-    646c4a7a:	cltq
-    646c4a7c:	shl    $0x2,%rax
-    646c4a80:	add    %r8,%rax
-    646c4a83:	mov    (%rax),%r8d
-    646c4a86:	mov    0x990(%rbp),%rax
-    646c4a8d:	mov    (%rax),%r9d
-    646c4a90:	mov    0x77d6(%rip),%eax        # 646cc26c <count>
-    646c4a96:	imul   %r9d,%eax
-    646c4a9a:	add    %r8d,%eax
-    646c4a9d:	cltq
-    646c4a9f:	shl    $0x3,%rax
-    646c4aa3:	add    %rcx,%rax
-    646c4aa6:	movsd  (%rdx),%xmm0
-    646c4aaa:	movsd  %xmm0,(%rax)
-    646c4aae:	mov    0x776c(%rip),%eax        # 646cc220 <_sampling>
-    646c4ab4:	cmp    $0x7,%eax
-    646c4ab7:	jg     646c4ac8 <sgsim_run+0x2e3>
-    646c4ab9:	mov    0x7761(%rip),%eax        # 646cc220 <_sampling>
-    646c4abf:	add    $0x1,%eax
-    646c4ac2:	mov    %eax,0x7758(%rip)        # 646cc220 <_sampling>
-    646c4ac8:	mov    0x76b1(%rip),%rdx        # 646cc180 <x_grid>
-    646c4acf:	mov    0x978(%rbp),%eax
-    646c4ad5:	cltq
-    646c4ad7:	shl    $0x2,%rax
-    646c4adb:	add    %rdx,%rax
-    646c4ade:	mov    (%rax),%ecx
-    646c4ae0:	mov    0x7751(%rip),%rdx        # 646cc238 <_sampling+0x18>
-    646c4ae7:	mov    0x978(%rbp),%eax
-    646c4aed:	cltq
-    646c4aef:	shl    $0x3,%rax
-    646c4af3:	add    %rdx,%rax
-    646c4af6:	cvtsi2sd %ecx,%xmm0
-    646c4afa:	movsd  %xmm0,(%rax)
-    646c4afe:	mov    0x7720(%rip),%eax        # 646cc224 <_sampling+0x4>
-    646c4b04:	add    $0x1,%eax
-    646c4b07:	mov    %eax,0x7717(%rip)        # 646cc224 <_sampling+0x4>
-    646c4b0d:	mov    0x76ec(%rip),%rdx        # 646cc200 <sgsim_array>
-    646c4b14:	mov    0x7665(%rip),%rcx        # 646cc180 <x_grid>
-    646c4b1b:	mov    0x978(%rbp),%eax
-    646c4b21:	cltq
-    646c4b23:	shl    $0x2,%rax
-    646c4b27:	add    %rcx,%rax
-    646c4b2a:	mov    (%rax),%eax
-    646c4b2c:	cltq
-    646c4b2e:	shl    $0x3,%rax
-    646c4b32:	add    %rdx,%rax
-    646c4b35:	mov    (%rax),%rax
-    646c4b38:	movq   %rax,%xmm0
-    646c4b3d:	call   646c6800 <__fpclassify>
-    646c4b42:	and    $0x100,%eax
-    646c4b47:	test   %eax,%eax
-    646c4b49:	je     646c4b5a <sgsim_run+0x375>
-    646c4b4b:	mov    0x7717(%rip),%eax        # 646cc268 <flag>
-    646c4b51:	add    $0x1,%eax
-    646c4b54:	mov    %eax,0x770e(%rip)        # 646cc268 <flag>
-    646c4b5a:	addl   $0x1,0x978(%rbp)
-    646c4b61:	mov    0x990(%rbp),%rax
-    646c4b68:	mov    (%rax),%eax
-    646c4b6a:	cmp    %eax,0x978(%rbp)
-    646c4b70:	jl     646c49e8 <sgsim_run+0x203>
-    646c4b76:	mov    0x76f0(%rip),%eax        # 646cc26c <count>
-    646c4b7c:	add    $0x1,%eax
-    646c4b7f:	mov    %eax,0x76e7(%rip)        # 646cc26c <count>
+    646c47c7:	mov    $0x8,%edx
+    646c47cc:	mov    %rax,%rcx
+    646c47cf:	call   646c76c0 <calloc>
+    646c47d4:	mov    %rax,%rdx
+    646c47d7:	mov    0x10(%rbp),%rax
+    646c47db:	mov    %rdx,0x10(%rax)
+    646c47df:	nop
+    646c47e0:	add    $0x30,%rsp
+    646c47e4:	pop    %rbp
+    646c47e5:	ret
+
+00000000646c47e6 <sgsim_run>:
+    646c47e6:	push   %rbp
+    646c47e7:	sub    $0xa00,%rsp
+    646c47ee:	lea    0x80(%rsp),%rbp
+    646c47f6:	mov    %rcx,0x990(%rbp)
+    646c47fd:	mov    %rdx,0x998(%rbp)
+    646c4804:	mov    %r8d,0x9a0(%rbp)
+    646c480b:	mov    0x990(%rbp),%rax
+    646c4812:	mov    0x8(%rax),%eax
+    646c4815:	mov    %eax,%edx
+    646c4817:	lea    -0x50(%rbp),%rax
+    646c481b:	mov    %rax,%rcx
+    646c481e:	call   646c2a30 <mt19937_init>
+    646c4823:	mov    0x990(%rbp),%rax
+    646c482a:	mov    (%rax),%eax
+    646c482c:	mov    %eax,%edx
+    646c482e:	lea    0x79eb(%rip),%rcx        # 646cc220 <_sampling>
+    646c4835:	call   646c3180 <sampling_state_init>
+    646c483a:	mov    0x998(%rbp),%rax
+    646c4841:	mov    0x8(%rax),%eax
+    646c4844:	cltq
+    646c4846:	mov    %rax,0x799b(%rip)        # 646cc1e8 <variogram_array+0x8>
+    646c484d:	mov    0x998(%rbp),%rax
+    646c4854:	mov    0x8(%rax),%eax
+    646c4857:	cltq
+    646c4859:	mov    %rax,0x7990(%rip)        # 646cc1f0 <variogram_array+0x10>
+    646c4860:	mov    0x998(%rbp),%rax
+    646c4867:	mov    0x8(%rax),%eax
+    646c486a:	cltq
+    646c486c:	mov    $0x8,%edx
+    646c4871:	mov    %rax,%rcx
+    646c4874:	call   646c76c0 <calloc>
+    646c4879:	mov    %rax,0x7960(%rip)        # 646cc1e0 <variogram_array>
+    646c4880:	mov    0x990(%rbp),%rax
+    646c4887:	mov    (%rax),%eax
+    646c4889:	cltq
+    646c488b:	mov    %rax,0x7976(%rip)        # 646cc208 <sgsim_array+0x8>
+    646c4892:	mov    0x990(%rbp),%rax
+    646c4899:	mov    (%rax),%eax
+    646c489b:	cltq
+    646c489d:	mov    %rax,0x796c(%rip)        # 646cc210 <sgsim_array+0x10>
+    646c48a4:	mov    0x990(%rbp),%rax
+    646c48ab:	mov    (%rax),%eax
+    646c48ad:	cltq
+    646c48af:	mov    $0x8,%edx
+    646c48b4:	mov    %rax,%rcx
+    646c48b7:	call   646c76c0 <calloc>
+    646c48bc:	mov    %rax,0x793d(%rip)        # 646cc200 <sgsim_array>
+    646c48c3:	mov    0x990(%rbp),%rax
+    646c48ca:	mov    (%rax),%eax
+    646c48cc:	mov    0x998(%rbp),%rdx
+    646c48d3:	mov    %eax,%ecx
+    646c48d5:	call   646c325d <krige_param_setting>
+    646c48da:	mov    0x990(%rbp),%rax
+    646c48e1:	mov    (%rax),%eax
+    646c48e3:	mov    %eax,%ecx
+    646c48e5:	call   646c4329 <arange>
+    646c48ea:	mov    %rax,0x788f(%rip)        # 646cc180 <x_grid>
+    646c48f1:	movl   $0x0,0x7971(%rip)        # 646cc26c <count>
+    646c48fb:	jmp    646c4bde <sgsim_run+0x3f8>
+    646c4900:	mov    0x7966(%rip),%eax        # 646cc26c <count>
+    646c4906:	mov    %eax,%edx
+    646c4908:	lea    0x47f1(%rip),%rcx        # 646c9100 <.rdata>
+    646c490f:	call   646c7670 <printf>
+    646c4914:	movl   $0x0,0x7906(%rip)        # 646cc224 <_sampling+0x4>
+    646c491e:	movl   $0x0,0x78f8(%rip)        # 646cc220 <_sampling>
+    646c4928:	movl   $0x0,0x7936(%rip)        # 646cc268 <flag>
+    646c4932:	mov    0x990(%rbp),%rax
+    646c4939:	mov    (%rax),%edx
+    646c493b:	mov    0x783e(%rip),%rax        # 646cc180 <x_grid>
+    646c4942:	lea    -0x50(%rbp),%rcx
+    646c4946:	mov    %rcx,%r8
+    646c4949:	mov    %rax,%rcx
+    646c494c:	call   646c46d0 <randompath>
+    646c4951:	mov    %rax,0x7828(%rip)        # 646cc180 <x_grid>
+    646c4958:	movl   $0x0,0x97c(%rbp)
+    646c4962:	jmp    646c4ae0 <sgsim_run+0x2fa>
+    646c4967:	mov    0x7812(%rip),%rdx        # 646cc180 <x_grid>
+    646c496e:	mov    0x97c(%rbp),%eax
+    646c4974:	cltq
+    646c4976:	shl    $0x2,%rax
+    646c497a:	add    %rdx,%rax
+    646c497d:	mov    (%rax),%eax
+    646c497f:	cvtsi2sd %eax,%xmm0
+    646c4983:	mov    0x97c(%rbp),%eax
+    646c4989:	mov    %eax,%r8d
+    646c498c:	movapd %xmm0,%xmm1
+    646c4990:	lea    0x7889(%rip),%rcx        # 646cc220 <_sampling>
+    646c4997:	call   646c3231 <sampling_state_update>
+    646c499c:	mov    0x785d(%rip),%rax        # 646cc200 <sgsim_array>
+    646c49a3:	lea    -0x50(%rbp),%rdx
+    646c49a7:	mov    %rdx,%r8
+    646c49aa:	lea    0x786f(%rip),%rdx        # 646cc220 <_sampling>
+    646c49b1:	mov    %rax,%rcx
+    646c49b4:	call   646c34b9 <simple_kriging>
+    646c49b9:	mov    0x7840(%rip),%rdx        # 646cc200 <sgsim_array>
+    646c49c0:	mov    0x77b9(%rip),%rcx        # 646cc180 <x_grid>
+    646c49c7:	mov    0x97c(%rbp),%eax
+    646c49cd:	cltq
+    646c49cf:	shl    $0x2,%rax
+    646c49d3:	add    %rcx,%rax
+    646c49d6:	mov    (%rax),%eax
+    646c49d8:	cltq
+    646c49da:	shl    $0x3,%rax
+    646c49de:	add    %rax,%rdx
+    646c49e1:	mov    0x990(%rbp),%rax
+    646c49e8:	mov    0x10(%rax),%rcx
+    646c49ec:	mov    0x778d(%rip),%r8        # 646cc180 <x_grid>
+    646c49f3:	mov    0x97c(%rbp),%eax
+    646c49f9:	cltq
+    646c49fb:	shl    $0x2,%rax
+    646c49ff:	add    %r8,%rax
+    646c4a02:	mov    (%rax),%r8d
+    646c4a05:	mov    0x990(%rbp),%rax
+    646c4a0c:	mov    (%rax),%r9d
+    646c4a0f:	mov    0x7857(%rip),%eax        # 646cc26c <count>
+    646c4a15:	imul   %r9d,%eax
+    646c4a19:	add    %r8d,%eax
+    646c4a1c:	cltq
+    646c4a1e:	shl    $0x3,%rax
+    646c4a22:	add    %rcx,%rax
+    646c4a25:	movsd  (%rdx),%xmm0
+    646c4a29:	movsd  %xmm0,(%rax)
+    646c4a2d:	mov    0x77ed(%rip),%eax        # 646cc220 <_sampling>
+    646c4a33:	cmp    $0x7,%eax
+    646c4a36:	jg     646c4a47 <sgsim_run+0x261>
+    646c4a38:	mov    0x77e2(%rip),%eax        # 646cc220 <_sampling>
+    646c4a3e:	add    $0x1,%eax
+    646c4a41:	mov    %eax,0x77d9(%rip)        # 646cc220 <_sampling>
+    646c4a47:	mov    0x7732(%rip),%rdx        # 646cc180 <x_grid>
+    646c4a4e:	mov    0x97c(%rbp),%eax
+    646c4a54:	cltq
+    646c4a56:	shl    $0x2,%rax
+    646c4a5a:	add    %rdx,%rax
+    646c4a5d:	mov    (%rax),%ecx
+    646c4a5f:	mov    0x77d2(%rip),%rdx        # 646cc238 <_sampling+0x18>
+    646c4a66:	mov    0x97c(%rbp),%eax
+    646c4a6c:	cltq
+    646c4a6e:	shl    $0x3,%rax
+    646c4a72:	add    %rdx,%rax
+    646c4a75:	cvtsi2sd %ecx,%xmm0
+    646c4a79:	movsd  %xmm0,(%rax)
+    646c4a7d:	mov    0x77a1(%rip),%eax        # 646cc224 <_sampling+0x4>
+    646c4a83:	add    $0x1,%eax
+    646c4a86:	mov    %eax,0x7798(%rip)        # 646cc224 <_sampling+0x4>
+    646c4a8c:	mov    0x776d(%rip),%rdx        # 646cc200 <sgsim_array>
+    646c4a93:	mov    0x76e6(%rip),%rcx        # 646cc180 <x_grid>
+    646c4a9a:	mov    0x97c(%rbp),%eax
+    646c4aa0:	cltq
+    646c4aa2:	shl    $0x2,%rax
+    646c4aa6:	add    %rcx,%rax
+    646c4aa9:	mov    (%rax),%eax
+    646c4aab:	cltq
+    646c4aad:	shl    $0x3,%rax
+    646c4ab1:	add    %rdx,%rax
+    646c4ab4:	mov    (%rax),%rax
+    646c4ab7:	movq   %rax,%xmm0
+    646c4abc:	call   646c6510 <__fpclassify>
+    646c4ac1:	and    $0x100,%eax
+    646c4ac6:	test   %eax,%eax
+    646c4ac8:	je     646c4ad9 <sgsim_run+0x2f3>
+    646c4aca:	mov    0x7798(%rip),%eax        # 646cc268 <flag>
+    646c4ad0:	add    $0x1,%eax
+    646c4ad3:	mov    %eax,0x778f(%rip)        # 646cc268 <flag>
+    646c4ad9:	addl   $0x1,0x97c(%rbp)
+    646c4ae0:	mov    0x990(%rbp),%rax
+    646c4ae7:	mov    (%rax),%eax
+    646c4ae9:	cmp    %eax,0x97c(%rbp)
+    646c4aef:	jl     646c4967 <sgsim_run+0x181>
+    646c4af5:	cmpl   $0x1,0x9a0(%rbp)
+    646c4afc:	jne    646c4b37 <sgsim_run+0x351>
+    646c4afe:	mov    0x998(%rbp),%rax
+    646c4b05:	mov    0x4(%rax),%ecx
+    646c4b08:	mov    0x998(%rbp),%rax
+    646c4b0f:	mov    0x8(%rax),%r9d
+    646c4b13:	mov    0x990(%rbp),%rax
+    646c4b1a:	mov    (%rax),%r8d
+    646c4b1d:	mov    0x76bc(%rip),%rdx        # 646cc1e0 <variogram_array>
+    646c4b24:	mov    0x76d5(%rip),%rax        # 646cc200 <sgsim_array>
+    646c4b2b:	mov    %ecx,0x20(%rsp)
+    646c4b2f:	mov    %rax,%rcx
+    646c4b32:	call   646c4e40 <variogram>
+    646c4b37:	mov    0x772b(%rip),%eax        # 646cc268 <flag>
+    646c4b3d:	test   %eax,%eax
+    646c4b3f:	jne    646c4bde <sgsim_run+0x3f8>
+    646c4b45:	mov    0x7720(%rip),%r8d        # 646cc26c <count>
+    646c4b4c:	mov    0x990(%rbp),%rax
+    646c4b53:	mov    0x4(%rax),%ecx
+    646c4b56:	mov    0x990(%rbp),%rax
+    646c4b5d:	mov    (%rax),%edx
+    646c4b5f:	mov    0x769a(%rip),%rax        # 646cc200 <sgsim_array>
+    646c4b66:	mov    %r8d,0x28(%rsp)
+    646c4b6b:	mov    %ecx,0x20(%rsp)
+    646c4b6f:	lea    0x4597(%rip),%r9        # 646c910d <.rdata+0xd>
+    646c4b76:	lea    0x45a0(%rip),%r8        # 646c911d <.rdata+0x1d>
+    646c4b7d:	mov    %rax,%rcx
+    646c4b80:	call   646c451f <save_1darray>
     646c4b85:	cmpl   $0x1,0x9a0(%rbp)
-    646c4b8c:	jne    646c4bc7 <sgsim_run+0x3e2>
-    646c4b8e:	mov    0x998(%rbp),%rax
-    646c4b95:	mov    0x4(%rax),%ecx
-    646c4b98:	mov    0x998(%rbp),%rax
-    646c4b9f:	mov    0x8(%rax),%r9d
-    646c4ba3:	mov    0x990(%rbp),%rax
-    646c4baa:	mov    (%rax),%r8d
-    646c4bad:	mov    0x762c(%rip),%rdx        # 646cc1e0 <variogram_array>
-    646c4bb4:	mov    0x7645(%rip),%rax        # 646cc200 <sgsim_array>
-    646c4bbb:	mov    %ecx,0x20(%rsp)
-    646c4bbf:	mov    %rax,%rcx
-    646c4bc2:	call   646c5120 <variogram>
-    646c4bc7:	mov    0x769b(%rip),%eax        # 646cc268 <flag>
-    646c4bcd:	test   %eax,%eax
-    646c4bcf:	jle    646c4be5 <sgsim_run+0x400>
-    646c4bd1:	mov    0x7695(%rip),%eax        # 646cc26c <count>
-    646c4bd7:	sub    $0x1,%eax
-    646c4bda:	mov    %eax,0x768c(%rip)        # 646cc26c <count>
-    646c4be0:	jmp    646c4c6f <sgsim_run+0x48a>
-    646c4be5:	mov    0x7680(%rip),%r8d        # 646cc26c <count>
-    646c4bec:	mov    0x990(%rbp),%rax
-    646c4bf3:	mov    0x4(%rax),%ecx
-    646c4bf6:	mov    0x990(%rbp),%rax
-    646c4bfd:	mov    (%rax),%edx
-    646c4bff:	mov    0x75fa(%rip),%rax        # 646cc200 <sgsim_array>
-    646c4c06:	mov    %r8d,0x28(%rsp)
-    646c4c0b:	mov    %ecx,0x20(%rsp)
-    646c4c0f:	lea    0x44f7(%rip),%r9        # 646c910d <.rdata+0xd>
-    646c4c16:	lea    0x4500(%rip),%r8        # 646c911d <.rdata+0x1d>
-    646c4c1d:	mov    %rax,%rcx
-    646c4c20:	call   646c451d <save_1darray>
-    646c4c25:	cmpl   $0x1,0x9a0(%rbp)
-    646c4c2c:	jne    646c4c6f <sgsim_run+0x48a>
-    646c4c2e:	mov    0x7637(%rip),%r8d        # 646cc26c <count>
-    646c4c35:	mov    0x990(%rbp),%rax
-    646c4c3c:	mov    0x4(%rax),%ecx
-    646c4c3f:	mov    0x998(%rbp),%rax
-    646c4c46:	mov    0x8(%rax),%edx
-    646c4c49:	mov    0x7590(%rip),%rax        # 646cc1e0 <variogram_array>
-    646c4c50:	mov    %r8d,0x28(%rsp)
-    646c4c55:	mov    %ecx,0x20(%rsp)
-    646c4c59:	lea    0x44ca(%rip),%r9        # 646c912a <.rdata+0x2a>
-    646c4c60:	lea    0x44dd(%rip),%r8        # 646c9144 <.rdata+0x44>
-    646c4c67:	mov    %rax,%rcx
-    646c4c6a:	call   646c451d <save_1darray>
-    646c4c6f:	mov    0x990(%rbp),%rax
-    646c4c76:	mov    0x4(%rax),%edx
-    646c4c79:	mov    0x75ed(%rip),%eax        # 646cc26c <count>
-    646c4c7f:	cmp    %eax,%edx
-    646c4c81:	jg     646c48ff <sgsim_run+0x11a>
-    646c4c87:	call   646c3a7b <krige_memory_free>
-    646c4c8c:	call   646c4cbe <sgsim_memory_free>
-    646c4c91:	nop
-    646c4c92:	add    $0xa00,%rsp
-    646c4c99:	pop    %rbp
-    646c4c9a:	ret
-
-00000000646c4c9b <sgsim_t_free>:
-    646c4c9b:	push   %rbp
-    646c4c9c:	mov    %rsp,%rbp
-    646c4c9f:	sub    $0x20,%rsp
-    646c4ca3:	mov    %rcx,0x10(%rbp)
-    646c4ca7:	mov    0x10(%rbp),%rax
-    646c4cab:	mov    0x10(%rax),%rax
-    646c4caf:	mov    %rax,%rcx
-    646c4cb2:	call   646c7988 <free>
-    646c4cb7:	nop
-    646c4cb8:	add    $0x20,%rsp
-    646c4cbc:	pop    %rbp
-    646c4cbd:	ret
-
-00000000646c4cbe <sgsim_memory_free>:
-    646c4cbe:	push   %rbp
-    646c4cbf:	mov    %rsp,%rbp
-    646c4cc2:	sub    $0x20,%rsp
-    646c4cc6:	mov    0x756b(%rip),%rax        # 646cc238 <_sampling+0x18>
-    646c4ccd:	mov    %rax,%rcx
-    646c4cd0:	call   646c7988 <free>
-    646c4cd5:	mov    0x7574(%rip),%rax        # 646cc250 <_sampling+0x30>
-    646c4cdc:	mov    %rax,%rcx
-    646c4cdf:	call   646c7988 <free>
-    646c4ce4:	mov    0x7515(%rip),%rax        # 646cc200 <sgsim_array>
-    646c4ceb:	mov    %rax,%rcx
-    646c4cee:	call   646c7988 <free>
-    646c4cf3:	mov    0x7486(%rip),%rax        # 646cc180 <x_grid>
-    646c4cfa:	mov    %rax,%rcx
-    646c4cfd:	call   646c7988 <free>
-    646c4d02:	mov    0x74d7(%rip),%rax        # 646cc1e0 <variogram_array>
-    646c4d09:	mov    %rax,%rcx
-    646c4d0c:	call   646c7988 <free>
-    646c4d11:	nop
-    646c4d12:	add    $0x20,%rsp
-    646c4d16:	pop    %rbp
-    646c4d17:	ret
-    646c4d18:	nop
-    646c4d19:	nop
-    646c4d1a:	nop
-    646c4d1b:	nop
-    646c4d1c:	nop
-    646c4d1d:	nop
-    646c4d1e:	nop
-    646c4d1f:	nop
-
-00000000646c4d20 <swap>:
-    646c4d20:	push   %rbp
-    646c4d21:	mov    %rsp,%rbp
-    646c4d24:	sub    $0x20,%rsp
-    646c4d28:	mov    %rcx,0x10(%rbp)
-    646c4d2c:	mov    %edx,0x18(%rbp)
-    646c4d2f:	mov    %r8d,0x20(%rbp)
-    646c4d33:	mov    0x20(%rbp),%eax
-    646c4d36:	cltq
-    646c4d38:	lea    0x0(,%rax,8),%rdx
-    646c4d40:	mov    0x10(%rbp),%rax
-    646c4d44:	add    %rdx,%rax
-    646c4d47:	mov    (%rax),%rax
-    646c4d4a:	movsd  (%rax),%xmm0
-    646c4d4e:	movsd  %xmm0,-0x8(%rbp)
-    646c4d53:	mov    0x20(%rbp),%eax
-    646c4d56:	cltq
-    646c4d58:	lea    0x0(,%rax,8),%rdx
-    646c4d60:	mov    0x10(%rbp),%rax
-    646c4d64:	add    %rdx,%rax
-    646c4d67:	mov    (%rax),%rax
-    646c4d6a:	movsd  0x8(%rax),%xmm0
-    646c4d6f:	movsd  %xmm0,-0x10(%rbp)
-    646c4d74:	mov    0x20(%rbp),%eax
-    646c4d77:	cltq
-    646c4d79:	lea    0x0(,%rax,8),%rdx
-    646c4d81:	mov    0x10(%rbp),%rax
-    646c4d85:	add    %rdx,%rax
-    646c4d88:	mov    (%rax),%rax
-    646c4d8b:	movsd  0x10(%rax),%xmm0
-    646c4d90:	movsd  %xmm0,-0x18(%rbp)
-    646c4d95:	mov    0x18(%rbp),%eax
-    646c4d98:	cltq
-    646c4d9a:	lea    0x0(,%rax,8),%rdx
-    646c4da2:	mov    0x10(%rbp),%rax
-    646c4da6:	add    %rdx,%rax
-    646c4da9:	mov    (%rax),%rdx
-    646c4dac:	mov    0x20(%rbp),%eax
-    646c4daf:	cltq
-    646c4db1:	lea    0x0(,%rax,8),%rcx
-    646c4db9:	mov    0x10(%rbp),%rax
-    646c4dbd:	add    %rcx,%rax
-    646c4dc0:	mov    (%rax),%rax
-    646c4dc3:	movsd  (%rdx),%xmm0
-    646c4dc7:	movsd  %xmm0,(%rax)
-    646c4dcb:	mov    0x18(%rbp),%eax
-    646c4dce:	cltq
-    646c4dd0:	lea    0x0(,%rax,8),%rdx
-    646c4dd8:	mov    0x10(%rbp),%rax
-    646c4ddc:	add    %rdx,%rax
-    646c4ddf:	mov    (%rax),%rdx
-    646c4de2:	mov    0x20(%rbp),%eax
-    646c4de5:	cltq
-    646c4de7:	lea    0x0(,%rax,8),%rcx
-    646c4def:	mov    0x10(%rbp),%rax
-    646c4df3:	add    %rcx,%rax
-    646c4df6:	mov    (%rax),%rax
-    646c4df9:	add    $0x8,%rax
-    646c4dfd:	movsd  0x8(%rdx),%xmm0
-    646c4e02:	movsd  %xmm0,(%rax)
-    646c4e06:	mov    0x18(%rbp),%eax
-    646c4e09:	cltq
-    646c4e0b:	lea    0x0(,%rax,8),%rdx
-    646c4e13:	mov    0x10(%rbp),%rax
-    646c4e17:	add    %rdx,%rax
-    646c4e1a:	mov    (%rax),%rdx
-    646c4e1d:	mov    0x20(%rbp),%eax
-    646c4e20:	cltq
-    646c4e22:	lea    0x0(,%rax,8),%rcx
-    646c4e2a:	mov    0x10(%rbp),%rax
-    646c4e2e:	add    %rcx,%rax
-    646c4e31:	mov    (%rax),%rax
-    646c4e34:	add    $0x10,%rax
-    646c4e38:	movsd  0x10(%rdx),%xmm0
-    646c4e3d:	movsd  %xmm0,(%rax)
-    646c4e41:	mov    0x18(%rbp),%eax
-    646c4e44:	cltq
-    646c4e46:	lea    0x0(,%rax,8),%rdx
-    646c4e4e:	mov    0x10(%rbp),%rax
-    646c4e52:	add    %rdx,%rax
-    646c4e55:	mov    (%rax),%rax
-    646c4e58:	movsd  -0x8(%rbp),%xmm0
-    646c4e5d:	movsd  %xmm0,(%rax)
-    646c4e61:	mov    0x18(%rbp),%eax
+    646c4b8c:	jne    646c4bcf <sgsim_run+0x3e9>
+    646c4b8e:	mov    0x76d7(%rip),%r8d        # 646cc26c <count>
+    646c4b95:	mov    0x990(%rbp),%rax
+    646c4b9c:	mov    0x4(%rax),%ecx
+    646c4b9f:	mov    0x998(%rbp),%rax
+    646c4ba6:	mov    0x8(%rax),%edx
+    646c4ba9:	mov    0x7630(%rip),%rax        # 646cc1e0 <variogram_array>
+    646c4bb0:	mov    %r8d,0x28(%rsp)
+    646c4bb5:	mov    %ecx,0x20(%rsp)
+    646c4bb9:	lea    0x456a(%rip),%r9        # 646c912a <.rdata+0x2a>
+    646c4bc0:	lea    0x457d(%rip),%r8        # 646c9144 <.rdata+0x44>
+    646c4bc7:	mov    %rax,%rcx
+    646c4bca:	call   646c451f <save_1darray>
+    646c4bcf:	mov    0x7697(%rip),%eax        # 646cc26c <count>
+    646c4bd5:	add    $0x1,%eax
+    646c4bd8:	mov    %eax,0x768e(%rip)        # 646cc26c <count>
+    646c4bde:	mov    0x990(%rbp),%rax
+    646c4be5:	mov    0x4(%rax),%edx
+    646c4be8:	mov    0x767e(%rip),%eax        # 646cc26c <count>
+    646c4bee:	cmp    %eax,%edx
+    646c4bf0:	jg     646c4900 <sgsim_run+0x11a>
+    646c4bf6:	call   646c3a7b <krige_memory_free>
+    646c4bfb:	call   646c4c2d <sgsim_memory_free>
+    646c4c00:	nop
+    646c4c01:	add    $0xa00,%rsp
+    646c4c08:	pop    %rbp
+    646c4c09:	ret
+
+00000000646c4c0a <sgsim_t_free>:
+    646c4c0a:	push   %rbp
+    646c4c0b:	mov    %rsp,%rbp
+    646c4c0e:	sub    $0x20,%rsp
+    646c4c12:	mov    %rcx,0x10(%rbp)
+    646c4c16:	mov    0x10(%rbp),%rax
+    646c4c1a:	mov    0x10(%rax),%rax
+    646c4c1e:	mov    %rax,%rcx
+    646c4c21:	call   646c7698 <free>
+    646c4c26:	nop
+    646c4c27:	add    $0x20,%rsp
+    646c4c2b:	pop    %rbp
+    646c4c2c:	ret
+
+00000000646c4c2d <sgsim_memory_free>:
+    646c4c2d:	push   %rbp
+    646c4c2e:	mov    %rsp,%rbp
+    646c4c31:	sub    $0x20,%rsp
+    646c4c35:	mov    0x75fc(%rip),%rax        # 646cc238 <_sampling+0x18>
+    646c4c3c:	mov    %rax,%rcx
+    646c4c3f:	call   646c7698 <free>
+    646c4c44:	mov    0x7605(%rip),%rax        # 646cc250 <_sampling+0x30>
+    646c4c4b:	mov    %rax,%rcx
+    646c4c4e:	call   646c7698 <free>
+    646c4c53:	mov    0x75a6(%rip),%rax        # 646cc200 <sgsim_array>
+    646c4c5a:	mov    %rax,%rcx
+    646c4c5d:	call   646c7698 <free>
+    646c4c62:	mov    0x7517(%rip),%rax        # 646cc180 <x_grid>
+    646c4c69:	mov    %rax,%rcx
+    646c4c6c:	call   646c7698 <free>
+    646c4c71:	mov    0x7568(%rip),%rax        # 646cc1e0 <variogram_array>
+    646c4c78:	mov    %rax,%rcx
+    646c4c7b:	call   646c7698 <free>
+    646c4c80:	nop
+    646c4c81:	add    $0x20,%rsp
+    646c4c85:	pop    %rbp
+    646c4c86:	ret
+    646c4c87:	nop
+    646c4c88:	nop
+    646c4c89:	nop
+    646c4c8a:	nop
+    646c4c8b:	nop
+    646c4c8c:	nop
+    646c4c8d:	nop
+    646c4c8e:	nop
+    646c4c8f:	nop
+
+00000000646c4c90 <swaprows>:
+    646c4c90:	push   %rbp
+    646c4c91:	mov    %rsp,%rbp
+    646c4c94:	sub    $0x10,%rsp
+    646c4c98:	mov    %rcx,0x10(%rbp)
+    646c4c9c:	mov    %edx,0x18(%rbp)
+    646c4c9f:	mov    %r8d,0x20(%rbp)
+    646c4ca3:	mov    0x20(%rbp),%eax
+    646c4ca6:	cltq
+    646c4ca8:	lea    0x0(,%rax,8),%rdx
+    646c4cb0:	mov    0x10(%rbp),%rax
+    646c4cb4:	add    %rdx,%rax
+    646c4cb7:	mov    (%rax),%rax
+    646c4cba:	mov    %rax,-0x8(%rbp)
+    646c4cbe:	mov    0x18(%rbp),%eax
+    646c4cc1:	cltq
+    646c4cc3:	lea    0x0(,%rax,8),%rdx
+    646c4ccb:	mov    0x10(%rbp),%rax
+    646c4ccf:	add    %rax,%rdx
+    646c4cd2:	mov    0x20(%rbp),%eax
+    646c4cd5:	cltq
+    646c4cd7:	lea    0x0(,%rax,8),%rcx
+    646c4cdf:	mov    0x10(%rbp),%rax
+    646c4ce3:	add    %rcx,%rax
+    646c4ce6:	mov    (%rdx),%rdx
+    646c4ce9:	mov    %rdx,(%rax)
+    646c4cec:	mov    0x18(%rbp),%eax
+    646c4cef:	cltq
+    646c4cf1:	lea    0x0(,%rax,8),%rdx
+    646c4cf9:	mov    0x10(%rbp),%rax
+    646c4cfd:	add    %rdx,%rax
+    646c4d00:	mov    -0x8(%rbp),%rdx
+    646c4d04:	mov    %rdx,(%rax)
+    646c4d07:	nop
+    646c4d08:	add    $0x10,%rsp
+    646c4d0c:	pop    %rbp
+    646c4d0d:	ret
+
+00000000646c4d0e <partition2d>:
+    646c4d0e:	push   %rbp
+    646c4d0f:	mov    %rsp,%rbp
+    646c4d12:	sub    $0x30,%rsp
+    646c4d16:	mov    %rcx,0x10(%rbp)
+    646c4d1a:	mov    %edx,0x18(%rbp)
+    646c4d1d:	mov    %r8d,0x20(%rbp)
+    646c4d21:	mov    0x18(%rbp),%eax
+    646c4d24:	cltq
+    646c4d26:	lea    0x0(,%rax,8),%rdx
+    646c4d2e:	mov    0x10(%rbp),%rax
+    646c4d32:	add    %rdx,%rax
+    646c4d35:	mov    (%rax),%rax
+    646c4d38:	movsd  0x10(%rax),%xmm0
+    646c4d3d:	movsd  %xmm0,-0x10(%rbp)
+    646c4d42:	mov    0x18(%rbp),%eax
+    646c4d45:	sub    $0x1,%eax
+    646c4d48:	mov    %eax,-0x4(%rbp)
+    646c4d4b:	mov    0x20(%rbp),%eax
+    646c4d4e:	add    $0x1,%eax
+    646c4d51:	mov    %eax,-0x8(%rbp)
+    646c4d54:	addl   $0x1,-0x4(%rbp)
+    646c4d58:	mov    -0x4(%rbp),%eax
+    646c4d5b:	cltq
+    646c4d5d:	lea    0x0(,%rax,8),%rdx
+    646c4d65:	mov    0x10(%rbp),%rax
+    646c4d69:	add    %rdx,%rax
+    646c4d6c:	mov    (%rax),%rax
+    646c4d6f:	add    $0x10,%rax
+    646c4d73:	movsd  (%rax),%xmm1
+    646c4d77:	movsd  -0x10(%rbp),%xmm0
+    646c4d7c:	comisd %xmm1,%xmm0
+    646c4d80:	ja     646c4d54 <partition2d+0x46>
+    646c4d82:	subl   $0x1,-0x8(%rbp)
+    646c4d86:	mov    -0x8(%rbp),%eax
+    646c4d89:	cltq
+    646c4d8b:	lea    0x0(,%rax,8),%rdx
+    646c4d93:	mov    0x10(%rbp),%rax
+    646c4d97:	add    %rdx,%rax
+    646c4d9a:	mov    (%rax),%rax
+    646c4d9d:	add    $0x10,%rax
+    646c4da1:	movsd  (%rax),%xmm0
+    646c4da5:	comisd -0x10(%rbp),%xmm0
+    646c4daa:	ja     646c4d82 <partition2d+0x74>
+    646c4dac:	mov    -0x4(%rbp),%eax
+    646c4daf:	cmp    -0x8(%rbp),%eax
+    646c4db2:	jl     646c4db9 <partition2d+0xab>
+    646c4db4:	mov    -0x8(%rbp),%eax
+    646c4db7:	jmp    646c4dcf <partition2d+0xc1>
+    646c4db9:	mov    -0x8(%rbp),%edx
+    646c4dbc:	mov    -0x4(%rbp),%eax
+    646c4dbf:	mov    %edx,%r8d
+    646c4dc2:	mov    %eax,%edx
+    646c4dc4:	mov    0x10(%rbp),%rcx
+    646c4dc8:	call   646c4c90 <swaprows>
+    646c4dcd:	jmp    646c4d54 <partition2d+0x46>
+    646c4dcf:	add    $0x30,%rsp
+    646c4dd3:	pop    %rbp
+    646c4dd4:	ret
+
+00000000646c4dd5 <quicksort2d>:
+    646c4dd5:	push   %rbp
+    646c4dd6:	mov    %rsp,%rbp
+    646c4dd9:	sub    $0x30,%rsp
+    646c4ddd:	mov    %rcx,0x10(%rbp)
+    646c4de1:	mov    %edx,0x18(%rbp)
+    646c4de4:	mov    %r8d,0x20(%rbp)
+    646c4de8:	mov    0x18(%rbp),%eax
+    646c4deb:	cmp    0x20(%rbp),%eax
+    646c4dee:	jge    646c4e32 <quicksort2d+0x5d>
+    646c4df0:	mov    0x20(%rbp),%edx
+    646c4df3:	mov    0x18(%rbp),%eax
+    646c4df6:	mov    %edx,%r8d
+    646c4df9:	mov    %eax,%edx
+    646c4dfb:	mov    0x10(%rbp),%rcx
+    646c4dff:	call   646c4d0e <partition2d>
+    646c4e04:	mov    %eax,-0x4(%rbp)
+    646c4e07:	mov    -0x4(%rbp),%edx
+    646c4e0a:	mov    0x18(%rbp),%eax
+    646c4e0d:	mov    %edx,%r8d
+    646c4e10:	mov    %eax,%edx
+    646c4e12:	mov    0x10(%rbp),%rcx
+    646c4e16:	call   646c4dd5 <quicksort2d>
+    646c4e1b:	mov    -0x4(%rbp),%eax
+    646c4e1e:	add    $0x1,%eax
+    646c4e21:	mov    0x20(%rbp),%edx
+    646c4e24:	mov    %edx,%r8d
+    646c4e27:	mov    %eax,%edx
+    646c4e29:	mov    0x10(%rbp),%rcx
+    646c4e2d:	call   646c4dd5 <quicksort2d>
+    646c4e32:	nop
+    646c4e33:	add    $0x30,%rsp
+    646c4e37:	pop    %rbp
+    646c4e38:	ret
+    646c4e39:	nop
+    646c4e3a:	nop
+    646c4e3b:	nop
+    646c4e3c:	nop
+    646c4e3d:	nop
+    646c4e3e:	nop
+    646c4e3f:	nop
+
+00000000646c4e40 <variogram>:
+    646c4e40:	push   %rbp
+    646c4e41:	push   %rbx
+    646c4e42:	sub    $0xb8,%rsp
+    646c4e49:	lea    0x80(%rsp),%rbp
+    646c4e51:	mov    %rcx,0x50(%rbp)
+    646c4e55:	mov    %rdx,0x58(%rbp)
+    646c4e59:	mov    %r8d,0x60(%rbp)
+    646c4e5d:	mov    %r9d,0x68(%rbp)
+    646c4e61:	mov    0x60(%rbp),%eax
     646c4e64:	cltq
-    646c4e66:	lea    0x0(,%rax,8),%rdx
-    646c4e6e:	mov    0x10(%rbp),%rax
-    646c4e72:	add    %rdx,%rax
-    646c4e75:	mov    (%rax),%rax
-    646c4e78:	add    $0x8,%rax
-    646c4e7c:	movsd  -0x10(%rbp),%xmm0
-    646c4e81:	movsd  %xmm0,(%rax)
-    646c4e85:	mov    0x18(%rbp),%eax
-    646c4e88:	cltq
-    646c4e8a:	lea    0x0(,%rax,8),%rdx
-    646c4e92:	mov    0x10(%rbp),%rax
-    646c4e96:	add    %rdx,%rax
-    646c4e99:	mov    (%rax),%rax
-    646c4e9c:	add    $0x10,%rax
-    646c4ea0:	movsd  -0x18(%rbp),%xmm0
-    646c4ea5:	movsd  %xmm0,(%rax)
-    646c4ea9:	nop
-    646c4eaa:	add    $0x20,%rsp
-    646c4eae:	pop    %rbp
-    646c4eaf:	ret
-
-00000000646c4eb0 <Partition2d>:
-    646c4eb0:	push   %rbp
-    646c4eb1:	mov    %rsp,%rbp
-    646c4eb4:	sub    $0x30,%rsp
-    646c4eb8:	mov    %rcx,0x10(%rbp)
-    646c4ebc:	mov    %edx,0x18(%rbp)
-    646c4ebf:	mov    %r8d,0x20(%rbp)
-    646c4ec3:	mov    0x20(%rbp),%eax
-    646c4ec6:	sub    0x18(%rbp),%eax
-    646c4ec9:	mov    %eax,%edx
-    646c4ecb:	shr    $0x1f,%edx
-    646c4ece:	add    %edx,%eax
-    646c4ed0:	sar    %eax
-    646c4ed2:	mov    %eax,%edx
-    646c4ed4:	mov    0x18(%rbp),%eax
-    646c4ed7:	add    %edx,%eax
-    646c4ed9:	mov    %eax,-0x4(%rbp)
-    646c4edc:	mov    0x18(%rbp),%eax
-    646c4edf:	cltq
-    646c4ee1:	lea    0x0(,%rax,8),%rdx
-    646c4ee9:	mov    0x10(%rbp),%rax
-    646c4eed:	add    %rdx,%rax
-    646c4ef0:	mov    (%rax),%rax
-    646c4ef3:	add    $0x10,%rax
-    646c4ef7:	movsd  (%rax),%xmm0
-    646c4efb:	mov    0x20(%rbp),%eax
-    646c4efe:	cltq
-    646c4f00:	lea    0x0(,%rax,8),%rdx
-    646c4f08:	mov    0x10(%rbp),%rax
-    646c4f0c:	add    %rdx,%rax
-    646c4f0f:	mov    (%rax),%rax
-    646c4f12:	add    $0x10,%rax
-    646c4f16:	movsd  (%rax),%xmm1
-    646c4f1a:	comisd %xmm1,%xmm0
-    646c4f1e:	jbe    646c4f34 <Partition2d+0x84>
-    646c4f20:	mov    0x20(%rbp),%edx
-    646c4f23:	mov    0x18(%rbp),%eax
-    646c4f26:	mov    %edx,%r8d
-    646c4f29:	mov    %eax,%edx
-    646c4f2b:	mov    0x10(%rbp),%rcx
-    646c4f2f:	call   646c4d20 <swap>
-    646c4f34:	mov    -0x4(%rbp),%eax
-    646c4f37:	cltq
-    646c4f39:	lea    0x0(,%rax,8),%rdx
-    646c4f41:	mov    0x10(%rbp),%rax
-    646c4f45:	add    %rdx,%rax
-    646c4f48:	mov    (%rax),%rax
-    646c4f4b:	add    $0x10,%rax
-    646c4f4f:	movsd  (%rax),%xmm0
-    646c4f53:	mov    0x20(%rbp),%eax
-    646c4f56:	cltq
-    646c4f58:	lea    0x0(,%rax,8),%rdx
-    646c4f60:	mov    0x10(%rbp),%rax
-    646c4f64:	add    %rdx,%rax
-    646c4f67:	mov    (%rax),%rax
-    646c4f6a:	add    $0x10,%rax
-    646c4f6e:	movsd  (%rax),%xmm1
-    646c4f72:	comisd %xmm1,%xmm0
-    646c4f76:	jbe    646c4f8c <Partition2d+0xdc>
-    646c4f78:	mov    0x20(%rbp),%edx
-    646c4f7b:	mov    -0x4(%rbp),%eax
-    646c4f7e:	mov    %edx,%r8d
-    646c4f81:	mov    %eax,%edx
-    646c4f83:	mov    0x10(%rbp),%rcx
-    646c4f87:	call   646c4d20 <swap>
-    646c4f8c:	mov    -0x4(%rbp),%eax
-    646c4f8f:	cltq
-    646c4f91:	lea    0x0(,%rax,8),%rdx
-    646c4f99:	mov    0x10(%rbp),%rax
-    646c4f9d:	add    %rdx,%rax
-    646c4fa0:	mov    (%rax),%rax
-    646c4fa3:	add    $0x10,%rax
-    646c4fa7:	movsd  (%rax),%xmm0
-    646c4fab:	mov    0x18(%rbp),%eax
-    646c4fae:	cltq
-    646c4fb0:	lea    0x0(,%rax,8),%rdx
-    646c4fb8:	mov    0x10(%rbp),%rax
-    646c4fbc:	add    %rdx,%rax
-    646c4fbf:	mov    (%rax),%rax
-    646c4fc2:	add    $0x10,%rax
-    646c4fc6:	movsd  (%rax),%xmm1
-    646c4fca:	comisd %xmm1,%xmm0
-    646c4fce:	jbe    646c4fe4 <Partition2d+0x134>
-    646c4fd0:	mov    0x18(%rbp),%edx
-    646c4fd3:	mov    -0x4(%rbp),%eax
-    646c4fd6:	mov    %edx,%r8d
-    646c4fd9:	mov    %eax,%edx
-    646c4fdb:	mov    0x10(%rbp),%rcx
-    646c4fdf:	call   646c4d20 <swap>
-    646c4fe4:	mov    0x18(%rbp),%eax
-    646c4fe7:	cltq
-    646c4fe9:	lea    0x0(,%rax,8),%rdx
-    646c4ff1:	mov    0x10(%rbp),%rax
-    646c4ff5:	add    %rdx,%rax
-    646c4ff8:	mov    (%rax),%rax
-    646c4ffb:	movsd  0x10(%rax),%xmm0
-    646c5000:	movsd  %xmm0,-0x10(%rbp)
-    646c5005:	jmp    646c509c <Partition2d+0x1ec>
-    646c500a:	subl   $0x1,0x20(%rbp)
-    646c500e:	mov    0x18(%rbp),%eax
-    646c5011:	cmp    0x20(%rbp),%eax
-    646c5014:	jge    646c503c <Partition2d+0x18c>
-    646c5016:	mov    0x20(%rbp),%eax
-    646c5019:	cltq
-    646c501b:	lea    0x0(,%rax,8),%rdx
-    646c5023:	mov    0x10(%rbp),%rax
-    646c5027:	add    %rdx,%rax
-    646c502a:	mov    (%rax),%rax
-    646c502d:	add    $0x10,%rax
-    646c5031:	movsd  (%rax),%xmm0
-    646c5035:	comisd -0x10(%rbp),%xmm0
-    646c503a:	jae    646c500a <Partition2d+0x15a>
-    646c503c:	mov    0x20(%rbp),%edx
-    646c503f:	mov    0x18(%rbp),%eax
-    646c5042:	mov    %edx,%r8d
-    646c5045:	mov    %eax,%edx
-    646c5047:	mov    0x10(%rbp),%rcx
-    646c504b:	call   646c4d20 <swap>
-    646c5050:	jmp    646c5056 <Partition2d+0x1a6>
-    646c5052:	addl   $0x1,0x18(%rbp)
-    646c5056:	mov    0x18(%rbp),%eax
-    646c5059:	cmp    0x20(%rbp),%eax
-    646c505c:	jge    646c5088 <Partition2d+0x1d8>
-    646c505e:	mov    0x18(%rbp),%eax
-    646c5061:	cltq
-    646c5063:	lea    0x0(,%rax,8),%rdx
-    646c506b:	mov    0x10(%rbp),%rax
-    646c506f:	add    %rdx,%rax
-    646c5072:	mov    (%rax),%rax
-    646c5075:	add    $0x10,%rax
-    646c5079:	movsd  (%rax),%xmm1
-    646c507d:	movsd  -0x10(%rbp),%xmm0
-    646c5082:	comisd %xmm1,%xmm0
-    646c5086:	jae    646c5052 <Partition2d+0x1a2>
-    646c5088:	mov    0x20(%rbp),%edx
-    646c508b:	mov    0x18(%rbp),%eax
-    646c508e:	mov    %edx,%r8d
-    646c5091:	mov    %eax,%edx
-    646c5093:	mov    0x10(%rbp),%rcx
-    646c5097:	call   646c4d20 <swap>
-    646c509c:	mov    0x18(%rbp),%eax
-    646c509f:	cmp    0x20(%rbp),%eax
-    646c50a2:	jl     646c500e <Partition2d+0x15e>
-    646c50a8:	mov    0x18(%rbp),%eax
-    646c50ab:	add    $0x30,%rsp
-    646c50af:	pop    %rbp
-    646c50b0:	ret
-
-00000000646c50b1 <quicksort2d>:
-    646c50b1:	push   %rbp
-    646c50b2:	mov    %rsp,%rbp
-    646c50b5:	sub    $0x30,%rsp
-    646c50b9:	mov    %rcx,0x10(%rbp)
-    646c50bd:	mov    %edx,0x18(%rbp)
-    646c50c0:	mov    %r8d,0x20(%rbp)
-    646c50c4:	mov    0x18(%rbp),%eax
-    646c50c7:	cmp    0x20(%rbp),%eax
-    646c50ca:	jge    646c5111 <quicksort2d+0x60>
-    646c50cc:	mov    0x20(%rbp),%edx
-    646c50cf:	mov    0x18(%rbp),%eax
-    646c50d2:	mov    %edx,%r8d
-    646c50d5:	mov    %eax,%edx
-    646c50d7:	mov    0x10(%rbp),%rcx
-    646c50db:	call   646c4eb0 <Partition2d>
-    646c50e0:	mov    %eax,-0x4(%rbp)
-    646c50e3:	mov    -0x4(%rbp),%eax
-    646c50e6:	lea    -0x1(%rax),%edx
-    646c50e9:	mov    0x18(%rbp),%eax
-    646c50ec:	mov    %edx,%r8d
-    646c50ef:	mov    %eax,%edx
-    646c50f1:	mov    0x10(%rbp),%rcx
-    646c50f5:	call   646c50b1 <quicksort2d>
-    646c50fa:	mov    -0x4(%rbp),%eax
-    646c50fd:	add    $0x1,%eax
-    646c5100:	mov    0x20(%rbp),%edx
-    646c5103:	mov    %edx,%r8d
-    646c5106:	mov    %eax,%edx
-    646c5108:	mov    0x10(%rbp),%rcx
-    646c510c:	call   646c50b1 <quicksort2d>
-    646c5111:	nop
-    646c5112:	add    $0x30,%rsp
-    646c5116:	pop    %rbp
-    646c5117:	ret
-    646c5118:	nop
-    646c5119:	nop
-    646c511a:	nop
-    646c511b:	nop
-    646c511c:	nop
-    646c511d:	nop
-    646c511e:	nop
-    646c511f:	nop
-
-00000000646c5120 <variogram>:
-    646c5120:	push   %rbp
-    646c5121:	push   %rbx
-    646c5122:	sub    $0x88,%rsp
-    646c5129:	lea    0x80(%rsp),%rbp
-    646c5131:	mov    %rcx,0x20(%rbp)
-    646c5135:	mov    %rdx,0x28(%rbp)
-    646c5139:	mov    %r8d,0x30(%rbp)
-    646c513d:	mov    %r9d,0x38(%rbp)
-    646c5141:	mov    0x30(%rbp),%eax
-    646c5144:	cltq
-    646c5146:	mov    %rax,-0x58(%rbp)
-    646c514a:	mov    0x30(%rbp),%eax
-    646c514d:	cltq
-    646c514f:	mov    %rax,-0x50(%rbp)
-    646c5153:	mov    0x30(%rbp),%eax
-    646c5156:	cltq
-    646c5158:	shl    $0x3,%rax
-    646c515c:	mov    %rax,%rcx
-    646c515f:	call   646c7970 <malloc>
-    646c5164:	mov    %rax,-0x60(%rbp)
-    646c5168:	movl   $0x0,-0x14(%rbp)
-    646c516f:	jmp    646c519b <variogram+0x7b>
-    646c5171:	mov    0x30(%rbp),%eax
-    646c5174:	cltq
-    646c5176:	shl    $0x3,%rax
-    646c517a:	mov    -0x60(%rbp),%rcx
-    646c517e:	mov    -0x14(%rbp),%edx
-    646c5181:	movslq %edx,%rdx
-    646c5184:	shl    $0x3,%rdx
-    646c5188:	lea    (%rcx,%rdx,1),%rbx
-    646c518c:	mov    %rax,%rcx
-    646c518f:	call   646c7970 <malloc>
-    646c5194:	mov    %rax,(%rbx)
-    646c5197:	addl   $0x1,-0x14(%rbp)
-    646c519b:	mov    -0x14(%rbp),%eax
-    646c519e:	cmp    0x30(%rbp),%eax
-    646c51a1:	jl     646c5171 <variogram+0x51>
-    646c51a3:	mov    0x30(%rbp),%eax
-    646c51a6:	mov    %eax,%ecx
-    646c51a8:	call   646c4381 <d_arange>
-    646c51ad:	mov    %rax,-0x40(%rbp)
-    646c51b1:	mov    -0x60(%rbp),%rdx
-    646c51b5:	mov    -0x40(%rbp),%rax
-    646c51b9:	mov    0x30(%rbp),%ecx
-    646c51bc:	mov    %ecx,%r8d
-    646c51bf:	mov    %rax,%rcx
-    646c51c2:	call   646c43dd <pdist>
-    646c51c7:	movl   $0x0,-0x18(%rbp)
-    646c51ce:	jmp    646c5337 <variogram+0x217>
-    646c51d3:	pxor   %xmm0,%xmm0
-    646c51d7:	movsd  %xmm0,-0x8(%rbp)
-    646c51dc:	pxor   %xmm0,%xmm0
-    646c51e0:	movsd  %xmm0,-0x10(%rbp)
-    646c51e5:	movl   $0x0,-0x1c(%rbp)
-    646c51ec:	jmp    646c52e8 <variogram+0x1c8>
-    646c51f1:	mov    -0x1c(%rbp),%eax
-    646c51f4:	add    $0x1,%eax
-    646c51f7:	mov    %eax,-0x20(%rbp)
-    646c51fa:	jmp    646c52d8 <variogram+0x1b8>
-    646c51ff:	mov    -0x60(%rbp),%rdx
-    646c5203:	mov    -0x1c(%rbp),%eax
-    646c5206:	cltq
-    646c5208:	shl    $0x3,%rax
-    646c520c:	add    %rdx,%rax
-    646c520f:	mov    (%rax),%rdx
-    646c5212:	mov    -0x20(%rbp),%eax
-    646c5215:	cltq
-    646c5217:	shl    $0x3,%rax
-    646c521b:	add    %rdx,%rax
-    646c521e:	movsd  (%rax),%xmm0
-    646c5222:	mov    -0x18(%rbp),%eax
-    646c5225:	sub    0x40(%rbp),%eax
-    646c5228:	cvtsi2sd %eax,%xmm1
-    646c522c:	comisd %xmm1,%xmm0
-    646c5230:	jb     646c52d4 <variogram+0x1b4>
-    646c5236:	mov    -0x60(%rbp),%rdx
-    646c523a:	mov    -0x1c(%rbp),%eax
-    646c523d:	cltq
-    646c523f:	shl    $0x3,%rax
-    646c5243:	add    %rdx,%rax
-    646c5246:	mov    (%rax),%rdx
-    646c5249:	mov    -0x20(%rbp),%eax
-    646c524c:	cltq
-    646c524e:	shl    $0x3,%rax
-    646c5252:	add    %rdx,%rax
-    646c5255:	movsd  (%rax),%xmm1
-    646c5259:	mov    -0x18(%rbp),%edx
-    646c525c:	mov    0x40(%rbp),%eax
-    646c525f:	add    %edx,%eax
-    646c5261:	cvtsi2sd %eax,%xmm0
-    646c5265:	comisd %xmm1,%xmm0
-    646c5269:	jb     646c52d4 <variogram+0x1b4>
-    646c526b:	mov    -0x1c(%rbp),%eax
-    646c526e:	cltq
-    646c5270:	lea    0x0(,%rax,8),%rdx
-    646c5278:	mov    0x20(%rbp),%rax
-    646c527c:	add    %rdx,%rax
-    646c527f:	movsd  (%rax),%xmm0
-    646c5283:	mov    -0x20(%rbp),%eax
-    646c5286:	cltq
-    646c5288:	lea    0x0(,%rax,8),%rdx
-    646c5290:	mov    0x20(%rbp),%rax
-    646c5294:	add    %rdx,%rax
-    646c5297:	movsd  (%rax),%xmm1
-    646c529b:	subsd  %xmm1,%xmm0
-    646c529f:	movsd  0x3eb9(%rip),%xmm1        # 646c9160 <.rdata>
-    646c52a7:	call   646c6f60 <pow>
-    646c52ac:	movapd %xmm0,%xmm1
-    646c52b0:	movsd  -0x8(%rbp),%xmm0
-    646c52b5:	addsd  %xmm1,%xmm0
-    646c52b9:	movsd  %xmm0,-0x8(%rbp)
-    646c52be:	movsd  -0x10(%rbp),%xmm1
-    646c52c3:	movsd  0x3e9d(%rip),%xmm0        # 646c9168 <.rdata+0x8>
-    646c52cb:	addsd  %xmm1,%xmm0
-    646c52cf:	movsd  %xmm0,-0x10(%rbp)
-    646c52d4:	addl   $0x1,-0x20(%rbp)
-    646c52d8:	mov    -0x20(%rbp),%eax
-    646c52db:	cmp    0x30(%rbp),%eax
-    646c52de:	jl     646c51ff <variogram+0xdf>
-    646c52e4:	addl   $0x1,-0x1c(%rbp)
-    646c52e8:	mov    -0x1c(%rbp),%eax
-    646c52eb:	cmp    0x30(%rbp),%eax
-    646c52ee:	jl     646c51f1 <variogram+0xd1>
-    646c52f4:	movsd  -0x8(%rbp),%xmm0
-    646c52f9:	comisd 0x3e6f(%rip),%xmm0        # 646c9170 <.rdata+0x10>
-    646c5301:	jb     646c5331 <variogram+0x211>
-    646c5303:	movsd  -0x10(%rbp),%xmm0
-    646c5308:	movapd %xmm0,%xmm1
-    646c530c:	addsd  %xmm0,%xmm1
-    646c5310:	mov    -0x18(%rbp),%eax
-    646c5313:	cltq
-    646c5315:	lea    0x0(,%rax,8),%rdx
-    646c531d:	mov    0x28(%rbp),%rax
-    646c5321:	add    %rdx,%rax
-    646c5324:	movsd  -0x8(%rbp),%xmm0
-    646c5329:	divsd  %xmm1,%xmm0
-    646c532d:	movsd  %xmm0,(%rax)
-    646c5331:	mov    0x40(%rbp),%eax
-    646c5334:	add    %eax,-0x18(%rbp)
-    646c5337:	mov    -0x18(%rbp),%eax
-    646c533a:	cmp    0x38(%rbp),%eax
-    646c533d:	jl     646c51d3 <variogram+0xb3>
-    646c5343:	mov    -0x40(%rbp),%rax
-    646c5347:	mov    %rax,%rcx
-    646c534a:	call   646c7988 <free>
-    646c534f:	movl   $0x0,-0x24(%rbp)
-    646c5356:	jmp    646c5377 <variogram+0x257>
-    646c5358:	mov    -0x60(%rbp),%rdx
-    646c535c:	mov    -0x24(%rbp),%eax
-    646c535f:	cltq
-    646c5361:	shl    $0x3,%rax
-    646c5365:	add    %rdx,%rax
-    646c5368:	mov    (%rax),%rax
-    646c536b:	mov    %rax,%rcx
-    646c536e:	call   646c7988 <free>
-    646c5373:	addl   $0x1,-0x24(%rbp)
-    646c5377:	mov    -0x24(%rbp),%eax
-    646c537a:	cltq
-    646c537c:	mov    -0x58(%rbp),%rdx
-    646c5380:	cmp    %rdx,%rax
-    646c5383:	jb     646c5358 <variogram+0x238>
-    646c5385:	mov    -0x60(%rbp),%rax
-    646c5389:	mov    %rax,%rcx
-    646c538c:	call   646c7988 <free>
-    646c5391:	nop
-    646c5392:	add    $0x88,%rsp
-    646c5399:	pop    %rbx
-    646c539a:	pop    %rbp
-    646c539b:	ret
-
-00000000646c539c <variance>:
-    646c539c:	push   %rbp
-    646c539d:	mov    %rsp,%rbp
-    646c53a0:	sub    $0x40,%rsp
-    646c53a4:	mov    %rcx,0x10(%rbp)
-    646c53a8:	mov    %edx,0x18(%rbp)
-    646c53ab:	pxor   %xmm0,%xmm0
-    646c53af:	movsd  %xmm0,-0x8(%rbp)
-    646c53b4:	pxor   %xmm0,%xmm0
-    646c53b8:	movsd  %xmm0,-0x10(%rbp)
-    646c53bd:	movl   $0x0,-0x14(%rbp)
-    646c53c4:	jmp    646c53f0 <variance+0x54>
-    646c53c6:	mov    -0x14(%rbp),%eax
-    646c53c9:	cltq
-    646c53cb:	lea    0x0(,%rax,8),%rdx
-    646c53d3:	mov    0x10(%rbp),%rax
-    646c53d7:	add    %rdx,%rax
-    646c53da:	movsd  (%rax),%xmm0
-    646c53de:	movsd  -0x8(%rbp),%xmm1
-    646c53e3:	addsd  %xmm1,%xmm0
-    646c53e7:	movsd  %xmm0,-0x8(%rbp)
-    646c53ec:	addl   $0x1,-0x14(%rbp)
-    646c53f0:	mov    -0x14(%rbp),%eax
-    646c53f3:	cmp    0x18(%rbp),%eax
-    646c53f6:	jl     646c53c6 <variance+0x2a>
-    646c53f8:	cvtsi2sdl 0x18(%rbp),%xmm1
-    646c53fd:	movsd  -0x8(%rbp),%xmm0
-    646c5402:	divsd  %xmm1,%xmm0
-    646c5406:	movsd  %xmm0,-0x8(%rbp)
-    646c540b:	movl   $0x0,-0x18(%rbp)
-    646c5412:	jmp    646c5454 <variance+0xb8>
-    646c5414:	mov    -0x18(%rbp),%eax
-    646c5417:	cltq
-    646c5419:	lea    0x0(,%rax,8),%rdx
-    646c5421:	mov    0x10(%rbp),%rax
-    646c5425:	add    %rdx,%rax
-    646c5428:	movsd  (%rax),%xmm0
-    646c542c:	subsd  -0x8(%rbp),%xmm0
-    646c5431:	movsd  0x3d27(%rip),%xmm1        # 646c9160 <.rdata>
-    646c5439:	call   646c6f60 <pow>
-    646c543e:	movapd %xmm0,%xmm1
-    646c5442:	movsd  -0x10(%rbp),%xmm0
-    646c5447:	addsd  %xmm1,%xmm0
-    646c544b:	movsd  %xmm0,-0x10(%rbp)
-    646c5450:	addl   $0x1,-0x18(%rbp)
-    646c5454:	mov    -0x18(%rbp),%eax
-    646c5457:	cmp    0x18(%rbp),%eax
-    646c545a:	jl     646c5414 <variance+0x78>
-    646c545c:	cvtsi2sdl 0x18(%rbp),%xmm1
-    646c5461:	movsd  -0x10(%rbp),%xmm0
-    646c5466:	divsd  %xmm1,%xmm0
-    646c546a:	movsd  %xmm0,-0x10(%rbp)
-    646c546f:	movsd  -0x10(%rbp),%xmm0
-    646c5474:	movq   %xmm0,%rax
-    646c5479:	movq   %rax,%xmm0
-    646c547e:	add    $0x40,%rsp
-    646c5482:	pop    %rbp
-    646c5483:	ret
-    646c5484:	nop
-    646c5485:	nop
-    646c5486:	nop
-    646c5487:	nop
-    646c5488:	nop
-    646c5489:	nop
-    646c548a:	nop
-    646c548b:	nop
-    646c548c:	nop
-    646c548d:	nop
-    646c548e:	nop
+    646c4e66:	mov    %rax,-0x58(%rbp)
+    646c4e6a:	mov    0x60(%rbp),%eax
+    646c4e6d:	cltq
+    646c4e6f:	mov    %rax,-0x50(%rbp)
+    646c4e73:	mov    0x60(%rbp),%eax
+    646c4e76:	cltq
+    646c4e78:	shl    $0x3,%rax
+    646c4e7c:	mov    %rax,%rcx
+    646c4e7f:	call   646c7680 <malloc>
+    646c4e84:	mov    %rax,-0x60(%rbp)
+    646c4e88:	movl   $0x0,0x1c(%rbp)
+    646c4e8f:	jmp    646c4ebb <variogram+0x7b>
+    646c4e91:	mov    0x60(%rbp),%eax
+    646c4e94:	cltq
+    646c4e96:	shl    $0x3,%rax
+    646c4e9a:	mov    -0x60(%rbp),%rcx
+    646c4e9e:	mov    0x1c(%rbp),%edx
+    646c4ea1:	movslq %edx,%rdx
+    646c4ea4:	shl    $0x3,%rdx
+    646c4ea8:	lea    (%rcx,%rdx,1),%rbx
+    646c4eac:	mov    %rax,%rcx
+    646c4eaf:	call   646c7680 <malloc>
+    646c4eb4:	mov    %rax,(%rbx)
+    646c4eb7:	addl   $0x1,0x1c(%rbp)
+    646c4ebb:	mov    0x1c(%rbp),%eax
+    646c4ebe:	cmp    0x60(%rbp),%eax
+    646c4ec1:	jl     646c4e91 <variogram+0x51>
+    646c4ec3:	mov    0x60(%rbp),%eax
+    646c4ec6:	mov    %eax,%ecx
+    646c4ec8:	call   646c4381 <d_arange>
+    646c4ecd:	mov    %rax,-0x40(%rbp)
+    646c4ed1:	mov    -0x60(%rbp),%rdx
+    646c4ed5:	mov    -0x40(%rbp),%rax
+    646c4ed9:	mov    0x60(%rbp),%ecx
+    646c4edc:	mov    %ecx,%r8d
+    646c4edf:	mov    %rax,%rcx
+    646c4ee2:	call   646c43dd <pdist>
+    646c4ee7:	movl   $0x0,0x18(%rbp)
+    646c4eee:	jmp    646c5051 <variogram+0x211>
+    646c4ef3:	pxor   %xmm0,%xmm0
+    646c4ef7:	movsd  %xmm0,0x28(%rbp)
+    646c4efc:	pxor   %xmm0,%xmm0
+    646c4f00:	movsd  %xmm0,0x20(%rbp)
+    646c4f05:	mov    0x18(%rbp),%eax
+    646c4f08:	sub    0x70(%rbp),%eax
+    646c4f0b:	cvtsi2sd %eax,%xmm0
+    646c4f0f:	movsd  %xmm0,0x0(%rbp)
+    646c4f14:	mov    0x18(%rbp),%edx
+    646c4f17:	mov    0x70(%rbp),%eax
+    646c4f1a:	add    %edx,%eax
+    646c4f1c:	cvtsi2sd %eax,%xmm0
+    646c4f20:	movsd  %xmm0,-0x8(%rbp)
+    646c4f25:	movl   $0x0,0x14(%rbp)
+    646c4f2c:	jmp    646c5002 <variogram+0x1c2>
+    646c4f31:	mov    0x14(%rbp),%eax
+    646c4f34:	cltq
+    646c4f36:	lea    0x0(,%rax,8),%rdx
+    646c4f3e:	mov    0x50(%rbp),%rax
+    646c4f42:	add    %rdx,%rax
+    646c4f45:	movsd  (%rax),%xmm0
+    646c4f49:	movsd  %xmm0,-0x10(%rbp)
+    646c4f4e:	movl   $0x0,0x10(%rbp)
+    646c4f55:	jmp    646c4ff2 <variogram+0x1b2>
+    646c4f5a:	mov    -0x60(%rbp),%rdx
+    646c4f5e:	mov    0x14(%rbp),%eax
+    646c4f61:	cltq
+    646c4f63:	shl    $0x3,%rax
+    646c4f67:	add    %rdx,%rax
+    646c4f6a:	mov    (%rax),%rdx
+    646c4f6d:	mov    0x10(%rbp),%eax
+    646c4f70:	cltq
+    646c4f72:	shl    $0x3,%rax
+    646c4f76:	add    %rdx,%rax
+    646c4f79:	movsd  (%rax),%xmm0
+    646c4f7d:	movsd  %xmm0,-0x18(%rbp)
+    646c4f82:	movsd  -0x18(%rbp),%xmm0
+    646c4f87:	comisd 0x0(%rbp),%xmm0
+    646c4f8c:	jb     646c4fee <variogram+0x1ae>
+    646c4f8e:	movsd  -0x8(%rbp),%xmm0
+    646c4f93:	comisd -0x18(%rbp),%xmm0
+    646c4f98:	jb     646c4fee <variogram+0x1ae>
+    646c4f9a:	mov    0x10(%rbp),%eax
+    646c4f9d:	cltq
+    646c4f9f:	lea    0x0(,%rax,8),%rdx
+    646c4fa7:	mov    0x50(%rbp),%rax
+    646c4fab:	add    %rdx,%rax
+    646c4fae:	movsd  (%rax),%xmm1
+    646c4fb2:	movsd  -0x10(%rbp),%xmm0
+    646c4fb7:	subsd  %xmm1,%xmm0
+    646c4fbb:	movsd  %xmm0,-0x20(%rbp)
+    646c4fc0:	movsd  -0x20(%rbp),%xmm0
+    646c4fc5:	mulsd  -0x20(%rbp),%xmm0
+    646c4fca:	movsd  0x28(%rbp),%xmm1
+    646c4fcf:	addsd  %xmm1,%xmm0
+    646c4fd3:	movsd  %xmm0,0x28(%rbp)
+    646c4fd8:	movsd  0x20(%rbp),%xmm1
+    646c4fdd:	movsd  0x416b(%rip),%xmm0        # 646c9150 <.rdata>
+    646c4fe5:	addsd  %xmm1,%xmm0
+    646c4fe9:	movsd  %xmm0,0x20(%rbp)
+    646c4fee:	addl   $0x1,0x10(%rbp)
+    646c4ff2:	mov    0x10(%rbp),%eax
+    646c4ff5:	cmp    0x14(%rbp),%eax
+    646c4ff8:	jl     646c4f5a <variogram+0x11a>
+    646c4ffe:	addl   $0x1,0x14(%rbp)
+    646c5002:	mov    0x14(%rbp),%eax
+    646c5005:	cmp    0x60(%rbp),%eax
+    646c5008:	jl     646c4f31 <variogram+0xf1>
+    646c500e:	movsd  0x28(%rbp),%xmm0
+    646c5013:	comisd 0x413d(%rip),%xmm0        # 646c9158 <.rdata+0x8>
+    646c501b:	jb     646c504b <variogram+0x20b>
+    646c501d:	movsd  0x20(%rbp),%xmm0
+    646c5022:	movapd %xmm0,%xmm1
+    646c5026:	addsd  %xmm0,%xmm1
+    646c502a:	mov    0x18(%rbp),%eax
+    646c502d:	cltq
+    646c502f:	lea    0x0(,%rax,8),%rdx
+    646c5037:	mov    0x58(%rbp),%rax
+    646c503b:	add    %rdx,%rax
+    646c503e:	movsd  0x28(%rbp),%xmm0
+    646c5043:	divsd  %xmm1,%xmm0
+    646c5047:	movsd  %xmm0,(%rax)
+    646c504b:	mov    0x70(%rbp),%eax
+    646c504e:	add    %eax,0x18(%rbp)
+    646c5051:	mov    0x18(%rbp),%eax
+    646c5054:	cmp    0x68(%rbp),%eax
+    646c5057:	jl     646c4ef3 <variogram+0xb3>
+    646c505d:	mov    -0x40(%rbp),%rax
+    646c5061:	mov    %rax,%rcx
+    646c5064:	call   646c7698 <free>
+    646c5069:	movl   $0x0,0xc(%rbp)
+    646c5070:	jmp    646c5091 <variogram+0x251>
+    646c5072:	mov    -0x60(%rbp),%rdx
+    646c5076:	mov    0xc(%rbp),%eax
+    646c5079:	cltq
+    646c507b:	shl    $0x3,%rax
+    646c507f:	add    %rdx,%rax
+    646c5082:	mov    (%rax),%rax
+    646c5085:	mov    %rax,%rcx
+    646c5088:	call   646c7698 <free>
+    646c508d:	addl   $0x1,0xc(%rbp)
+    646c5091:	mov    0xc(%rbp),%eax
+    646c5094:	cltq
+    646c5096:	mov    -0x58(%rbp),%rdx
+    646c509a:	cmp    %rdx,%rax
+    646c509d:	jb     646c5072 <variogram+0x232>
+    646c509f:	mov    -0x60(%rbp),%rax
+    646c50a3:	mov    %rax,%rcx
+    646c50a6:	call   646c7698 <free>
+    646c50ab:	nop
+    646c50ac:	add    $0xb8,%rsp
+    646c50b3:	pop    %rbx
+    646c50b4:	pop    %rbp
+    646c50b5:	ret
+
+00000000646c50b6 <variance>:
+    646c50b6:	push   %rbp
+    646c50b7:	mov    %rsp,%rbp
+    646c50ba:	sub    $0x40,%rsp
+    646c50be:	mov    %rcx,0x10(%rbp)
+    646c50c2:	mov    %edx,0x18(%rbp)
+    646c50c5:	pxor   %xmm0,%xmm0
+    646c50c9:	movsd  %xmm0,-0x8(%rbp)
+    646c50ce:	pxor   %xmm0,%xmm0
+    646c50d2:	movsd  %xmm0,-0x10(%rbp)
+    646c50d7:	movl   $0x0,-0x14(%rbp)
+    646c50de:	jmp    646c510a <variance+0x54>
+    646c50e0:	mov    -0x14(%rbp),%eax
+    646c50e3:	cltq
+    646c50e5:	lea    0x0(,%rax,8),%rdx
+    646c50ed:	mov    0x10(%rbp),%rax
+    646c50f1:	add    %rdx,%rax
+    646c50f4:	movsd  (%rax),%xmm0
+    646c50f8:	movsd  -0x8(%rbp),%xmm1
+    646c50fd:	addsd  %xmm1,%xmm0
+    646c5101:	movsd  %xmm0,-0x8(%rbp)
+    646c5106:	addl   $0x1,-0x14(%rbp)
+    646c510a:	mov    -0x14(%rbp),%eax
+    646c510d:	cmp    0x18(%rbp),%eax
+    646c5110:	jl     646c50e0 <variance+0x2a>
+    646c5112:	cvtsi2sdl 0x18(%rbp),%xmm1
+    646c5117:	movsd  -0x8(%rbp),%xmm0
+    646c511c:	divsd  %xmm1,%xmm0
+    646c5120:	movsd  %xmm0,-0x8(%rbp)
+    646c5125:	movl   $0x0,-0x18(%rbp)
+    646c512c:	jmp    646c516e <variance+0xb8>
+    646c512e:	mov    -0x18(%rbp),%eax
+    646c5131:	cltq
+    646c5133:	lea    0x0(,%rax,8),%rdx
+    646c513b:	mov    0x10(%rbp),%rax
+    646c513f:	add    %rdx,%rax
+    646c5142:	movsd  (%rax),%xmm0
+    646c5146:	subsd  -0x8(%rbp),%xmm0
+    646c514b:	movsd  0x400d(%rip),%xmm1        # 646c9160 <.rdata+0x10>
+    646c5153:	call   646c6c70 <pow>
+    646c5158:	movapd %xmm0,%xmm1
+    646c515c:	movsd  -0x10(%rbp),%xmm0
+    646c5161:	addsd  %xmm1,%xmm0
+    646c5165:	movsd  %xmm0,-0x10(%rbp)
+    646c516a:	addl   $0x1,-0x18(%rbp)
+    646c516e:	mov    -0x18(%rbp),%eax
+    646c5171:	cmp    0x18(%rbp),%eax
+    646c5174:	jl     646c512e <variance+0x78>
+    646c5176:	cvtsi2sdl 0x18(%rbp),%xmm1
+    646c517b:	movsd  -0x10(%rbp),%xmm0
+    646c5180:	divsd  %xmm1,%xmm0
+    646c5184:	movsd  %xmm0,-0x10(%rbp)
+    646c5189:	movsd  -0x10(%rbp),%xmm0
+    646c518e:	movq   %xmm0,%rax
+    646c5193:	movq   %rax,%xmm0
+    646c5198:	add    $0x40,%rsp
+    646c519c:	pop    %rbp
+    646c519d:	ret
+    646c519e:	nop
+    646c519f:	nop
+
+00000000646c51a0 <Sleep>:
+    646c51a0:	jmp    *0x90a6(%rip)        # 646ce24c <__imp_Sleep>
+    646c51a6:	nop
+    646c51a7:	nop
+    646c51a8:	nopl   0x0(%rax,%rax,1)
+
+00000000646c51b0 <__do_global_dtors>:
+    646c51b0:	sub    $0x28,%rsp
+    646c51b4:	mov    0x2e45(%rip),%rax        # 646c8000 <__data_start__>
+    646c51bb:	mov    (%rax),%rax
+    646c51be:	test   %rax,%rax
+    646c51c1:	je     646c51e0 <__do_global_dtors+0x30>
+    646c51c3:	call   *%rax
+    646c51c5:	mov    0x2e34(%rip),%rax        # 646c8000 <__data_start__>
+    646c51cc:	lea    0x8(%rax),%rdx
+    646c51d0:	mov    0x8(%rax),%rax
+    646c51d4:	mov    %rdx,0x2e25(%rip)        # 646c8000 <__data_start__>
+    646c51db:	test   %rax,%rax
+    646c51de:	jne    646c51c3 <__do_global_dtors+0x13>
+    646c51e0:	add    $0x28,%rsp
+    646c51e4:	ret
+    646c51e5:	nop
+    646c51e6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c51f0 <__do_global_ctors>:
+    646c51f0:	push   %rsi
+    646c51f1:	push   %rbx
+    646c51f2:	sub    $0x28,%rsp
+    646c51f6:	mov    0x43d3(%rip),%rcx        # 646c95d0 <.refptr.__CTOR_LIST__>
+    646c51fd:	mov    (%rcx),%rdx
+    646c5200:	cmp    $0xffffffff,%edx
+    646c5203:	mov    %edx,%eax
+    646c5205:	je     646c5240 <__do_global_ctors+0x50>
+    646c5207:	test   %eax,%eax
+    646c5209:	je     646c522b <__do_global_ctors+0x3b>
+    646c520b:	mov    %eax,%edx
+    646c520d:	sub    $0x1,%eax
+    646c5210:	lea    (%rcx,%rdx,8),%rbx
+    646c5214:	sub    %rax,%rdx
+    646c5217:	lea    -0x8(%rcx,%rdx,8),%rsi
+    646c521c:	nopl   0x0(%rax)
+    646c5220:	call   *(%rbx)
+    646c5222:	sub    $0x8,%rbx
+    646c5226:	cmp    %rsi,%rbx
+    646c5229:	jne    646c5220 <__do_global_ctors+0x30>
+    646c522b:	lea    -0x82(%rip),%rcx        # 646c51b0 <__do_global_dtors>
+    646c5232:	add    $0x28,%rsp
+    646c5236:	pop    %rbx
+    646c5237:	pop    %rsi
+    646c5238:	jmp    646c1380 <atexit>
+    646c523d:	nopl   (%rax)
+    646c5240:	xor    %eax,%eax
+    646c5242:	jmp    646c5246 <__do_global_ctors+0x56>
+    646c5244:	mov    %edx,%eax
+    646c5246:	lea    0x1(%rax),%r8d
+    646c524a:	cmpq   $0x0,(%rcx,%r8,8)
+    646c524f:	mov    %r8,%rdx
+    646c5252:	jne    646c5244 <__do_global_ctors+0x54>
+    646c5254:	jmp    646c5207 <__do_global_ctors+0x17>
+    646c5256:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5260 <__main>:
+    646c5260:	mov    0x701a(%rip),%eax        # 646cc280 <initialized>
+    646c5266:	test   %eax,%eax
+    646c5268:	je     646c5270 <__main+0x10>
+    646c526a:	ret
+    646c526b:	nopl   0x0(%rax,%rax,1)
+    646c5270:	movl   $0x1,0x7006(%rip)        # 646cc280 <initialized>
+    646c527a:	jmp    646c51f0 <__do_global_ctors>
+    646c527f:	nop
+
+00000000646c5280 <__security_init_cookie>:
+    646c5280:	push   %r12
+    646c5282:	push   %rbp
+    646c5283:	push   %rdi
+    646c5284:	push   %rsi
+    646c5285:	push   %rbx
+    646c5286:	sub    $0x30,%rsp
+    646c528a:	mov    0x2def(%rip),%rbx        # 646c8080 <__security_cookie>
+    646c5291:	movabs $0x2b992ddfa232,%rax
+    646c529b:	cmp    %rax,%rbx
+    646c529e:	movq   $0x0,0x20(%rsp)
+    646c52a7:	je     646c52c0 <__security_init_cookie+0x40>
+    646c52a9:	not    %rbx
+    646c52ac:	mov    %rbx,0x2ddd(%rip)        # 646c8090 <__security_cookie_complement>
+    646c52b3:	add    $0x30,%rsp
+    646c52b7:	pop    %rbx
+    646c52b8:	pop    %rsi
+    646c52b9:	pop    %rdi
+    646c52ba:	pop    %rbp
+    646c52bb:	pop    %r12
+    646c52bd:	ret
+    646c52be:	xchg   %ax,%ax
+    646c52c0:	lea    0x20(%rsp),%rcx
+    646c52c5:	call   *0x8f31(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
+    646c52cb:	mov    0x20(%rsp),%rsi
+    646c52d0:	call   *0x8f0e(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
+    646c52d6:	mov    %eax,%r12d
+    646c52d9:	call   *0x8f0d(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
+    646c52df:	mov    %eax,%ebp
+    646c52e1:	call   *0x8f1d(%rip)        # 646ce204 <__imp_GetTickCount>
+    646c52e7:	lea    0x28(%rsp),%rcx
+    646c52ec:	mov    %eax,%edi
+    646c52ee:	call   *0x8f28(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
+    646c52f4:	xor    0x28(%rsp),%rsi
+    646c52f9:	mov    %r12d,%eax
+    646c52fc:	movabs $0xffffffffffff,%rdx
+    646c5306:	xor    %rsi,%rax
+    646c5309:	mov    %ebp,%esi
+    646c530b:	xor    %rax,%rsi
+    646c530e:	mov    %edi,%eax
+    646c5310:	xor    %rsi,%rax
+    646c5313:	and    %rdx,%rax
+    646c5316:	cmp    %rbx,%rax
+    646c5319:	je     646c5340 <__security_init_cookie+0xc0>
+    646c531b:	mov    %rax,%rdx
+    646c531e:	not    %rdx
+    646c5321:	mov    %rax,0x2d58(%rip)        # 646c8080 <__security_cookie>
+    646c5328:	mov    %rdx,0x2d61(%rip)        # 646c8090 <__security_cookie_complement>
+    646c532f:	add    $0x30,%rsp
+    646c5333:	pop    %rbx
+    646c5334:	pop    %rsi
+    646c5335:	pop    %rdi
+    646c5336:	pop    %rbp
+    646c5337:	pop    %r12
+    646c5339:	ret
+    646c533a:	nopw   0x0(%rax,%rax,1)
+    646c5340:	movabs $0xffffd466d2205dcc,%rdx
+    646c534a:	movabs $0x2b992ddfa233,%rax
+    646c5354:	jmp    646c5321 <__security_init_cookie+0xa1>
+    646c5356:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5360 <__report_gsfailure>:
+    646c5360:	push   %rbp
+    646c5361:	push   %rsi
+    646c5362:	push   %rbx
+    646c5363:	mov    %rsp,%rbp
+    646c5366:	sub    $0x70,%rsp
+    646c536a:	mov    %rcx,%rsi
+    646c536d:	lea    0x6f2c(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
+    646c5374:	call   *0x8eb2(%rip)        # 646ce22c <__imp_RtlCaptureContext>
+    646c537a:	mov    0x7017(%rip),%rbx        # 646cc398 <GS_ContextRecord+0xf8>
+    646c5381:	lea    -0x28(%rbp),%rdx
+    646c5385:	xor    %r8d,%r8d
+    646c5388:	mov    %rbx,%rcx
+    646c538b:	call   *0x8ea3(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
+    646c5391:	test   %rax,%rax
+    646c5394:	je     646c543d <__report_gsfailure+0xdd>
+    646c539a:	lea    -0x20(%rbp),%rdx
+    646c539e:	mov    %rax,%r9
+    646c53a1:	mov    %rbx,%r8
+    646c53a4:	movq   $0x0,0x38(%rsp)
+    646c53ad:	lea    0x6eec(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
+    646c53b4:	mov    %rdx,0x30(%rsp)
+    646c53b9:	lea    -0x18(%rbp),%rdx
+    646c53bd:	mov    %rcx,0x20(%rsp)
+    646c53c2:	xor    %ecx,%ecx
+    646c53c4:	mov    %rdx,0x28(%rsp)
+    646c53c9:	mov    -0x28(%rbp),%rdx
+    646c53cd:	call   *0x8e69(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
+    646c53d3:	mov    0x6fbe(%rip),%rax        # 646cc398 <GS_ContextRecord+0xf8>
+    646c53da:	xor    %ecx,%ecx
+    646c53dc:	mov    %rsi,0x6f3d(%rip)        # 646cc320 <GS_ContextRecord+0x80>
+    646c53e3:	mov    %rax,0x73a6(%rip)        # 646cc790 <GS_ExceptionRecord+0x10>
+    646c53ea:	movabs $0x1c0000409,%rax
+    646c53f4:	mov    %rax,0x7385(%rip)        # 646cc780 <GS_ExceptionRecord>
+    646c53fb:	mov    0x2c7e(%rip),%rax        # 646c8080 <__security_cookie>
+    646c5402:	mov    %rax,-0x10(%rbp)
+    646c5406:	mov    0x2c83(%rip),%rax        # 646c8090 <__security_cookie_complement>
+    646c540d:	mov    %rax,-0x8(%rbp)
+    646c5411:	call   *0x8e2d(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
+    646c5417:	lea    0x3d52(%rip),%rcx        # 646c9170 <GS_ExceptionPointers>
+    646c541e:	call   *0x8e40(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
+    646c5424:	call   *0x8db2(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
+    646c542a:	mov    $0xc0000409,%edx
+    646c542f:	mov    %rax,%rcx
+    646c5432:	call   *0x8e1c(%rip)        # 646ce254 <__imp_TerminateProcess>
+    646c5438:	call   646c76c8 <abort>
+    646c543d:	mov    0x18(%rbp),%rax
+    646c5441:	mov    %rax,0x6f50(%rip)        # 646cc398 <GS_ContextRecord+0xf8>
+    646c5448:	lea    0x8(%rbp),%rax
+    646c544c:	mov    %rax,0x6ee5(%rip)        # 646cc338 <GS_ContextRecord+0x98>
+    646c5453:	jmp    646c53d3 <__report_gsfailure+0x73>
+    646c5458:	nop
+    646c5459:	nop
+    646c545a:	nop
+    646c545b:	nop
+    646c545c:	nop
+    646c545d:	nop
+    646c545e:	nop
+    646c545f:	nop
+
+00000000646c5460 <__dyn_tls_dtor>:
+    646c5460:	sub    $0x28,%rsp
+    646c5464:	cmp    $0x3,%edx
+    646c5467:	je     646c5480 <__dyn_tls_dtor+0x20>
+    646c5469:	test   %edx,%edx
+    646c546b:	je     646c5480 <__dyn_tls_dtor+0x20>
+    646c546d:	mov    $0x1,%eax
+    646c5472:	add    $0x28,%rsp
+    646c5476:	ret
+    646c5477:	nopw   0x0(%rax,%rax,1)
+    646c5480:	call   646c5fe0 <__mingw_TLScallback>
+    646c5485:	mov    $0x1,%eax
+    646c548a:	add    $0x28,%rsp
+    646c548e:	ret
     646c548f:	nop
 
-00000000646c5490 <Sleep>:
-    646c5490:	jmp    *0x8db6(%rip)        # 646ce24c <__imp_Sleep>
-    646c5496:	nop
-    646c5497:	nop
-    646c5498:	nopl   0x0(%rax,%rax,1)
-
-00000000646c54a0 <__do_global_dtors>:
-    646c54a0:	sub    $0x28,%rsp
-    646c54a4:	mov    0x2b55(%rip),%rax        # 646c8000 <__data_start__>
-    646c54ab:	mov    (%rax),%rax
-    646c54ae:	test   %rax,%rax
-    646c54b1:	je     646c54d0 <__do_global_dtors+0x30>
-    646c54b3:	call   *%rax
-    646c54b5:	mov    0x2b44(%rip),%rax        # 646c8000 <__data_start__>
-    646c54bc:	lea    0x8(%rax),%rdx
-    646c54c0:	mov    0x8(%rax),%rax
-    646c54c4:	mov    %rdx,0x2b35(%rip)        # 646c8000 <__data_start__>
-    646c54cb:	test   %rax,%rax
-    646c54ce:	jne    646c54b3 <__do_global_dtors+0x13>
-    646c54d0:	add    $0x28,%rsp
-    646c54d4:	ret
-    646c54d5:	nop
-    646c54d6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c54e0 <__do_global_ctors>:
-    646c54e0:	push   %rsi
-    646c54e1:	push   %rbx
-    646c54e2:	sub    $0x28,%rsp
-    646c54e6:	mov    0x4103(%rip),%rcx        # 646c95f0 <.refptr.__CTOR_LIST__>
-    646c54ed:	mov    (%rcx),%rdx
-    646c54f0:	cmp    $0xffffffff,%edx
-    646c54f3:	mov    %edx,%eax
-    646c54f5:	je     646c5530 <__do_global_ctors+0x50>
-    646c54f7:	test   %eax,%eax
-    646c54f9:	je     646c551b <__do_global_ctors+0x3b>
-    646c54fb:	mov    %eax,%edx
-    646c54fd:	sub    $0x1,%eax
-    646c5500:	lea    (%rcx,%rdx,8),%rbx
-    646c5504:	sub    %rax,%rdx
-    646c5507:	lea    -0x8(%rcx,%rdx,8),%rsi
-    646c550c:	nopl   0x0(%rax)
-    646c5510:	call   *(%rbx)
-    646c5512:	sub    $0x8,%rbx
-    646c5516:	cmp    %rsi,%rbx
-    646c5519:	jne    646c5510 <__do_global_ctors+0x30>
-    646c551b:	lea    -0x82(%rip),%rcx        # 646c54a0 <__do_global_dtors>
-    646c5522:	add    $0x28,%rsp
-    646c5526:	pop    %rbx
-    646c5527:	pop    %rsi
-    646c5528:	jmp    646c1380 <atexit>
-    646c552d:	nopl   (%rax)
-    646c5530:	xor    %eax,%eax
-    646c5532:	jmp    646c5536 <__do_global_ctors+0x56>
-    646c5534:	mov    %edx,%eax
-    646c5536:	lea    0x1(%rax),%r8d
-    646c553a:	cmpq   $0x0,(%rcx,%r8,8)
-    646c553f:	mov    %r8,%rdx
-    646c5542:	jne    646c5534 <__do_global_ctors+0x54>
-    646c5544:	jmp    646c54f7 <__do_global_ctors+0x17>
-    646c5546:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5550 <__main>:
-    646c5550:	mov    0x6d2a(%rip),%eax        # 646cc280 <initialized>
-    646c5556:	test   %eax,%eax
-    646c5558:	je     646c5560 <__main+0x10>
-    646c555a:	ret
-    646c555b:	nopl   0x0(%rax,%rax,1)
-    646c5560:	movl   $0x1,0x6d16(%rip)        # 646cc280 <initialized>
-    646c556a:	jmp    646c54e0 <__do_global_ctors>
+00000000646c5490 <__dyn_tls_init>:
+    646c5490:	push   %rsi
+    646c5491:	push   %rbx
+    646c5492:	sub    $0x28,%rsp
+    646c5496:	mov    0x4123(%rip),%rax        # 646c95c0 <.refptr._CRT_MT>
+    646c549d:	cmpl   $0x2,(%rax)
+    646c54a0:	je     646c54a8 <__dyn_tls_init+0x18>
+    646c54a2:	movl   $0x2,(%rax)
+    646c54a8:	cmp    $0x2,%edx
+    646c54ab:	je     646c54c0 <__dyn_tls_init+0x30>
+    646c54ad:	cmp    $0x1,%edx
+    646c54b0:	je     646c54f2 <__dyn_tls_init+0x62>
+    646c54b2:	mov    $0x1,%eax
+    646c54b7:	add    $0x28,%rsp
+    646c54bb:	pop    %rbx
+    646c54bc:	pop    %rsi
+    646c54bd:	ret
+    646c54be:	xchg   %ax,%ax
+    646c54c0:	lea    0x9b89(%rip),%rbx        # 646cf050 <__xd_z>
+    646c54c7:	lea    0x9b82(%rip),%rsi        # 646cf050 <__xd_z>
+    646c54ce:	cmp    %rbx,%rsi
+    646c54d1:	je     646c54b2 <__dyn_tls_init+0x22>
+    646c54d3:	mov    (%rbx),%rax
+    646c54d6:	test   %rax,%rax
+    646c54d9:	je     646c54dd <__dyn_tls_init+0x4d>
+    646c54db:	call   *%rax
+    646c54dd:	add    $0x8,%rbx
+    646c54e1:	cmp    %rbx,%rsi
+    646c54e4:	jne    646c54d3 <__dyn_tls_init+0x43>
+    646c54e6:	mov    $0x1,%eax
+    646c54eb:	add    $0x28,%rsp
+    646c54ef:	pop    %rbx
+    646c54f0:	pop    %rsi
+    646c54f1:	ret
+    646c54f2:	call   646c5fe0 <__mingw_TLScallback>
+    646c54f7:	mov    $0x1,%eax
+    646c54fc:	add    $0x28,%rsp
+    646c5500:	pop    %rbx
+    646c5501:	pop    %rsi
+    646c5502:	ret
+    646c5503:	nopl   (%rax)
+    646c5506:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5510 <__tlregdtor>:
+    646c5510:	xor    %eax,%eax
+    646c5512:	ret
+    646c5513:	nop
+    646c5514:	nop
+    646c5515:	nop
+    646c5516:	nop
+    646c5517:	nop
+    646c5518:	nop
+    646c5519:	nop
+    646c551a:	nop
+    646c551b:	nop
+    646c551c:	nop
+    646c551d:	nop
+    646c551e:	nop
+    646c551f:	nop
+
+00000000646c5520 <_decode_pointer>:
+    646c5520:	mov    %rcx,%rax
+    646c5523:	ret
+    646c5524:	xchg   %ax,%ax
+    646c5526:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c5530 <_encode_pointer>:
+    646c5530:	mov    %rcx,%rax
+    646c5533:	ret
+    646c5534:	nop
+    646c5535:	nop
+    646c5536:	nop
+    646c5537:	nop
+    646c5538:	nop
+    646c5539:	nop
+    646c553a:	nop
+    646c553b:	nop
+    646c553c:	nop
+    646c553d:	nop
+    646c553e:	nop
+    646c553f:	nop
+
+00000000646c5540 <__write_memory.part.0>:
+    646c5540:	push   %r12
+    646c5542:	push   %rbp
+    646c5543:	push   %rdi
+    646c5544:	push   %rsi
+    646c5545:	push   %rbx
+    646c5546:	sub    $0x50,%rsp
+    646c554a:	movslq 0x72f3(%rip),%rsi        # 646cc844 <maxSections>
+    646c5551:	test   %esi,%esi
+    646c5553:	mov    %rcx,%rbx
+    646c5556:	mov    %rdx,%rbp
+    646c5559:	mov    %r8,%rdi
+    646c555c:	jle    646c56c8 <__write_memory.part.0+0x188>
+    646c5562:	mov    0x72df(%rip),%rax        # 646cc848 <the_secs>
+    646c5569:	xor    %ecx,%ecx
+    646c556b:	add    $0x18,%rax
     646c556f:	nop
-
-00000000646c5570 <__security_init_cookie>:
-    646c5570:	push   %r12
-    646c5572:	push   %rbp
-    646c5573:	push   %rdi
-    646c5574:	push   %rsi
-    646c5575:	push   %rbx
-    646c5576:	sub    $0x30,%rsp
-    646c557a:	mov    0x2aff(%rip),%rbx        # 646c8080 <__security_cookie>
-    646c5581:	movabs $0x2b992ddfa232,%rax
-    646c558b:	cmp    %rax,%rbx
-    646c558e:	movq   $0x0,0x20(%rsp)
-    646c5597:	je     646c55b0 <__security_init_cookie+0x40>
-    646c5599:	not    %rbx
-    646c559c:	mov    %rbx,0x2aed(%rip)        # 646c8090 <__security_cookie_complement>
-    646c55a3:	add    $0x30,%rsp
-    646c55a7:	pop    %rbx
-    646c55a8:	pop    %rsi
-    646c55a9:	pop    %rdi
-    646c55aa:	pop    %rbp
-    646c55ab:	pop    %r12
-    646c55ad:	ret
-    646c55ae:	xchg   %ax,%ax
-    646c55b0:	lea    0x20(%rsp),%rcx
-    646c55b5:	call   *0x8c41(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
-    646c55bb:	mov    0x20(%rsp),%rsi
-    646c55c0:	call   *0x8c1e(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
-    646c55c6:	mov    %eax,%r12d
-    646c55c9:	call   *0x8c1d(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
-    646c55cf:	mov    %eax,%ebp
-    646c55d1:	call   *0x8c2d(%rip)        # 646ce204 <__imp_GetTickCount>
-    646c55d7:	lea    0x28(%rsp),%rcx
-    646c55dc:	mov    %eax,%edi
-    646c55de:	call   *0x8c38(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
-    646c55e4:	xor    0x28(%rsp),%rsi
-    646c55e9:	mov    %r12d,%eax
-    646c55ec:	movabs $0xffffffffffff,%rdx
-    646c55f6:	xor    %rsi,%rax
-    646c55f9:	mov    %ebp,%esi
-    646c55fb:	xor    %rax,%rsi
-    646c55fe:	mov    %edi,%eax
-    646c5600:	xor    %rsi,%rax
-    646c5603:	and    %rdx,%rax
-    646c5606:	cmp    %rbx,%rax
-    646c5609:	je     646c5630 <__security_init_cookie+0xc0>
-    646c560b:	mov    %rax,%rdx
-    646c560e:	not    %rdx
-    646c5611:	mov    %rax,0x2a68(%rip)        # 646c8080 <__security_cookie>
-    646c5618:	mov    %rdx,0x2a71(%rip)        # 646c8090 <__security_cookie_complement>
-    646c561f:	add    $0x30,%rsp
-    646c5623:	pop    %rbx
-    646c5624:	pop    %rsi
-    646c5625:	pop    %rdi
-    646c5626:	pop    %rbp
-    646c5627:	pop    %r12
-    646c5629:	ret
-    646c562a:	nopw   0x0(%rax,%rax,1)
-    646c5630:	movabs $0xffffd466d2205dcc,%rdx
-    646c563a:	movabs $0x2b992ddfa233,%rax
-    646c5644:	jmp    646c5611 <__security_init_cookie+0xa1>
-    646c5646:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5650 <__report_gsfailure>:
-    646c5650:	push   %rbp
-    646c5651:	push   %rsi
-    646c5652:	push   %rbx
-    646c5653:	mov    %rsp,%rbp
-    646c5656:	sub    $0x70,%rsp
-    646c565a:	mov    %rcx,%rsi
-    646c565d:	lea    0x6c3c(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
-    646c5664:	call   *0x8bc2(%rip)        # 646ce22c <__imp_RtlCaptureContext>
-    646c566a:	mov    0x6d27(%rip),%rbx        # 646cc398 <GS_ContextRecord+0xf8>
-    646c5671:	lea    -0x28(%rbp),%rdx
-    646c5675:	xor    %r8d,%r8d
-    646c5678:	mov    %rbx,%rcx
-    646c567b:	call   *0x8bb3(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
-    646c5681:	test   %rax,%rax
-    646c5684:	je     646c572d <__report_gsfailure+0xdd>
-    646c568a:	lea    -0x20(%rbp),%rdx
-    646c568e:	mov    %rax,%r9
-    646c5691:	mov    %rbx,%r8
-    646c5694:	movq   $0x0,0x38(%rsp)
-    646c569d:	lea    0x6bfc(%rip),%rcx        # 646cc2a0 <GS_ContextRecord>
-    646c56a4:	mov    %rdx,0x30(%rsp)
-    646c56a9:	lea    -0x18(%rbp),%rdx
-    646c56ad:	mov    %rcx,0x20(%rsp)
-    646c56b2:	xor    %ecx,%ecx
-    646c56b4:	mov    %rdx,0x28(%rsp)
-    646c56b9:	mov    -0x28(%rbp),%rdx
-    646c56bd:	call   *0x8b79(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
-    646c56c3:	mov    0x6cce(%rip),%rax        # 646cc398 <GS_ContextRecord+0xf8>
-    646c56ca:	xor    %ecx,%ecx
-    646c56cc:	mov    %rsi,0x6c4d(%rip)        # 646cc320 <GS_ContextRecord+0x80>
-    646c56d3:	mov    %rax,0x70b6(%rip)        # 646cc790 <GS_ExceptionRecord+0x10>
-    646c56da:	movabs $0x1c0000409,%rax
-    646c56e4:	mov    %rax,0x7095(%rip)        # 646cc780 <GS_ExceptionRecord>
-    646c56eb:	mov    0x298e(%rip),%rax        # 646c8080 <__security_cookie>
-    646c56f2:	mov    %rax,-0x10(%rbp)
-    646c56f6:	mov    0x2993(%rip),%rax        # 646c8090 <__security_cookie_complement>
-    646c56fd:	mov    %rax,-0x8(%rbp)
-    646c5701:	call   *0x8b3d(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
-    646c5707:	lea    0x3a72(%rip),%rcx        # 646c9180 <GS_ExceptionPointers>
-    646c570e:	call   *0x8b50(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
-    646c5714:	call   *0x8ac2(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
-    646c571a:	mov    $0xc0000409,%edx
-    646c571f:	mov    %rax,%rcx
-    646c5722:	call   *0x8b2c(%rip)        # 646ce254 <__imp_TerminateProcess>
-    646c5728:	call   646c79b8 <abort>
-    646c572d:	mov    0x18(%rbp),%rax
-    646c5731:	mov    %rax,0x6c60(%rip)        # 646cc398 <GS_ContextRecord+0xf8>
-    646c5738:	lea    0x8(%rbp),%rax
-    646c573c:	mov    %rax,0x6bf5(%rip)        # 646cc338 <GS_ContextRecord+0x98>
-    646c5743:	jmp    646c56c3 <__report_gsfailure+0x73>
-    646c5748:	nop
-    646c5749:	nop
-    646c574a:	nop
-    646c574b:	nop
-    646c574c:	nop
-    646c574d:	nop
-    646c574e:	nop
-    646c574f:	nop
-
-00000000646c5750 <__dyn_tls_dtor>:
-    646c5750:	sub    $0x28,%rsp
-    646c5754:	cmp    $0x3,%edx
-    646c5757:	je     646c5770 <__dyn_tls_dtor+0x20>
-    646c5759:	test   %edx,%edx
-    646c575b:	je     646c5770 <__dyn_tls_dtor+0x20>
-    646c575d:	mov    $0x1,%eax
-    646c5762:	add    $0x28,%rsp
-    646c5766:	ret
-    646c5767:	nopw   0x0(%rax,%rax,1)
-    646c5770:	call   646c62d0 <__mingw_TLScallback>
-    646c5775:	mov    $0x1,%eax
-    646c577a:	add    $0x28,%rsp
-    646c577e:	ret
-    646c577f:	nop
-
-00000000646c5780 <__dyn_tls_init>:
-    646c5780:	push   %rsi
-    646c5781:	push   %rbx
-    646c5782:	sub    $0x28,%rsp
-    646c5786:	mov    0x3e53(%rip),%rax        # 646c95e0 <.refptr._CRT_MT>
-    646c578d:	cmpl   $0x2,(%rax)
-    646c5790:	je     646c5798 <__dyn_tls_init+0x18>
-    646c5792:	movl   $0x2,(%rax)
-    646c5798:	cmp    $0x2,%edx
-    646c579b:	je     646c57b0 <__dyn_tls_init+0x30>
-    646c579d:	cmp    $0x1,%edx
-    646c57a0:	je     646c57e2 <__dyn_tls_init+0x62>
-    646c57a2:	mov    $0x1,%eax
-    646c57a7:	add    $0x28,%rsp
-    646c57ab:	pop    %rbx
-    646c57ac:	pop    %rsi
-    646c57ad:	ret
-    646c57ae:	xchg   %ax,%ax
-    646c57b0:	lea    0x9899(%rip),%rbx        # 646cf050 <__xd_z>
-    646c57b7:	lea    0x9892(%rip),%rsi        # 646cf050 <__xd_z>
-    646c57be:	cmp    %rbx,%rsi
-    646c57c1:	je     646c57a2 <__dyn_tls_init+0x22>
-    646c57c3:	mov    (%rbx),%rax
-    646c57c6:	test   %rax,%rax
-    646c57c9:	je     646c57cd <__dyn_tls_init+0x4d>
-    646c57cb:	call   *%rax
-    646c57cd:	add    $0x8,%rbx
-    646c57d1:	cmp    %rbx,%rsi
-    646c57d4:	jne    646c57c3 <__dyn_tls_init+0x43>
-    646c57d6:	mov    $0x1,%eax
-    646c57db:	add    $0x28,%rsp
-    646c57df:	pop    %rbx
-    646c57e0:	pop    %rsi
-    646c57e1:	ret
-    646c57e2:	call   646c62d0 <__mingw_TLScallback>
-    646c57e7:	mov    $0x1,%eax
-    646c57ec:	add    $0x28,%rsp
-    646c57f0:	pop    %rbx
-    646c57f1:	pop    %rsi
-    646c57f2:	ret
-    646c57f3:	nopl   (%rax)
-    646c57f6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5800 <__tlregdtor>:
-    646c5800:	xor    %eax,%eax
-    646c5802:	ret
-    646c5803:	nop
-    646c5804:	nop
-    646c5805:	nop
-    646c5806:	nop
-    646c5807:	nop
-    646c5808:	nop
-    646c5809:	nop
-    646c580a:	nop
-    646c580b:	nop
-    646c580c:	nop
-    646c580d:	nop
-    646c580e:	nop
-    646c580f:	nop
-
-00000000646c5810 <_decode_pointer>:
-    646c5810:	mov    %rcx,%rax
-    646c5813:	ret
-    646c5814:	xchg   %ax,%ax
-    646c5816:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c5820 <_encode_pointer>:
-    646c5820:	mov    %rcx,%rax
-    646c5823:	ret
-    646c5824:	nop
-    646c5825:	nop
-    646c5826:	nop
-    646c5827:	nop
-    646c5828:	nop
-    646c5829:	nop
-    646c582a:	nop
-    646c582b:	nop
-    646c582c:	nop
-    646c582d:	nop
-    646c582e:	nop
-    646c582f:	nop
-
-00000000646c5830 <__write_memory.part.0>:
-    646c5830:	push   %r12
-    646c5832:	push   %rbp
-    646c5833:	push   %rdi
-    646c5834:	push   %rsi
-    646c5835:	push   %rbx
-    646c5836:	sub    $0x50,%rsp
-    646c583a:	movslq 0x7003(%rip),%rsi        # 646cc844 <maxSections>
-    646c5841:	test   %esi,%esi
-    646c5843:	mov    %rcx,%rbx
-    646c5846:	mov    %rdx,%rbp
-    646c5849:	mov    %r8,%rdi
-    646c584c:	jle    646c59b8 <__write_memory.part.0+0x188>
-    646c5852:	mov    0x6fef(%rip),%rax        # 646cc848 <the_secs>
-    646c5859:	xor    %ecx,%ecx
-    646c585b:	add    $0x18,%rax
-    646c585f:	nop
-    646c5860:	mov    (%rax),%rdx
-    646c5863:	cmp    %rdx,%rbx
-    646c5866:	jb     646c587c <__write_memory.part.0+0x4c>
-    646c5868:	mov    0x8(%rax),%r8
-    646c586c:	mov    0x8(%r8),%r8d
-    646c5870:	add    %r8,%rdx
-    646c5873:	cmp    %rdx,%rbx
-    646c5876:	jb     646c5905 <__write_memory.part.0+0xd5>
-    646c587c:	add    $0x1,%ecx
-    646c587f:	add    $0x28,%rax
-    646c5883:	cmp    %esi,%ecx
-    646c5885:	jne    646c5860 <__write_memory.part.0+0x30>
-    646c5887:	mov    %rbx,%rcx
-    646c588a:	call   646c64d0 <__mingw_GetSectionForAddress>
-    646c588f:	test   %rax,%rax
-    646c5892:	mov    %rax,%r12
-    646c5895:	je     646c59ed <__write_memory.part.0+0x1bd>
-    646c589b:	mov    0x6fa6(%rip),%rax        # 646cc848 <the_secs>
-    646c58a2:	lea    (%rsi,%rsi,4),%rsi
-    646c58a6:	shl    $0x3,%rsi
-    646c58aa:	add    %rsi,%rax
-    646c58ad:	mov    %r12,0x20(%rax)
-    646c58b1:	movl   $0x0,(%rax)
-    646c58b7:	call   646c6600 <_GetPEImageBase>
-    646c58bc:	mov    0xc(%r12),%ecx
-    646c58c1:	lea    0x20(%rsp),%rdx
-    646c58c6:	mov    $0x30,%r8d
-    646c58cc:	add    %rax,%rcx
-    646c58cf:	mov    0x6f72(%rip),%rax        # 646cc848 <the_secs>
-    646c58d6:	mov    %rcx,0x18(%rax,%rsi,1)
-    646c58db:	call   *0x8993(%rip)        # 646ce274 <__imp_VirtualQuery>
-    646c58e1:	test   %rax,%rax
-    646c58e4:	je     646c59d0 <__write_memory.part.0+0x1a0>
-    646c58ea:	mov    0x44(%rsp),%eax
-    646c58ee:	lea    -0x4(%rax),%edx
-    646c58f1:	and    $0xfffffffb,%edx
-    646c58f4:	je     646c58fe <__write_memory.part.0+0xce>
-    646c58f6:	sub    $0x40,%eax
-    646c58f9:	and    $0xffffffbf,%eax
-    646c58fc:	jne    646c5960 <__write_memory.part.0+0x130>
-    646c58fe:	addl   $0x1,0x6f3f(%rip)        # 646cc844 <maxSections>
-    646c5905:	cmp    $0x8,%edi
-    646c5908:	jae    646c5933 <__write_memory.part.0+0x103>
-    646c590a:	test   $0x4,%dil
-    646c590e:	jne    646c59a4 <__write_memory.part.0+0x174>
-    646c5914:	test   %edi,%edi
-    646c5916:	je     646c5928 <__write_memory.part.0+0xf8>
-    646c5918:	movzbl 0x0(%rbp),%eax
-    646c591c:	test   $0x2,%dil
-    646c5920:	mov    %al,(%rbx)
-    646c5922:	jne    646c59bf <__write_memory.part.0+0x18f>
-    646c5928:	add    $0x50,%rsp
-    646c592c:	pop    %rbx
-    646c592d:	pop    %rsi
-    646c592e:	pop    %rdi
-    646c592f:	pop    %rbp
-    646c5930:	pop    %r12
-    646c5932:	ret
-    646c5933:	mov    %edi,%eax
-    646c5935:	sub    $0x1,%edi
-    646c5938:	mov    -0x8(%rbp,%rax,1),%rdx
-    646c593d:	cmp    $0x8,%edi
-    646c5940:	mov    %rdx,-0x8(%rbx,%rax,1)
-    646c5945:	jb     646c5928 <__write_memory.part.0+0xf8>
-    646c5947:	and    $0xfffffff8,%edi
-    646c594a:	xor    %eax,%eax
-    646c594c:	mov    %eax,%edx
-    646c594e:	add    $0x8,%eax
-    646c5951:	mov    0x0(%rbp,%rdx,1),%rcx
-    646c5956:	cmp    %edi,%eax
-    646c5958:	mov    %rcx,(%rbx,%rdx,1)
-    646c595c:	jb     646c594c <__write_memory.part.0+0x11c>
-    646c595e:	jmp    646c5928 <__write_memory.part.0+0xf8>
-    646c5960:	add    0x6ee1(%rip),%rsi        # 646cc848 <the_secs>
-    646c5967:	mov    $0x40,%r8d
-    646c596d:	mov    0x20(%rsp),%rcx
-    646c5972:	mov    0x38(%rsp),%rdx
-    646c5977:	mov    %rsi,%r9
-    646c597a:	mov    %rcx,0x8(%rsi)
-    646c597e:	mov    %rdx,0x10(%rsi)
-    646c5982:	call   *0x88e4(%rip)        # 646ce26c <__imp_VirtualProtect>
-    646c5988:	test   %eax,%eax
-    646c598a:	jne    646c58fe <__write_memory.part.0+0xce>
-    646c5990:	call   *0x885e(%rip)        # 646ce1f4 <__imp_GetLastError>
-    646c5996:	lea    0x38db(%rip),%rcx        # 646c9278 <.rdata+0x78>
-    646c599d:	mov    %eax,%edx
-    646c599f:	call   646c7dc0 <__report_error>
-    646c59a4:	mov    0x0(%rbp),%eax
-    646c59a7:	mov    %edi,%edi
-    646c59a9:	mov    %eax,(%rbx)
-    646c59ab:	mov    -0x4(%rbp,%rdi,1),%eax
-    646c59af:	mov    %eax,-0x4(%rbx,%rdi,1)
-    646c59b3:	jmp    646c5928 <__write_memory.part.0+0xf8>
-    646c59b8:	xor    %esi,%esi
-    646c59ba:	jmp    646c5887 <__write_memory.part.0+0x57>
-    646c59bf:	mov    %edi,%edi
-    646c59c1:	movzwl -0x2(%rbp,%rdi,1),%eax
-    646c59c6:	mov    %ax,-0x2(%rbx,%rdi,1)
-    646c59cb:	jmp    646c5928 <__write_memory.part.0+0xf8>
-    646c59d0:	mov    0x6e71(%rip),%rax        # 646cc848 <the_secs>
-    646c59d7:	lea    0x3862(%rip),%rcx        # 646c9240 <.rdata+0x40>
-    646c59de:	mov    0x8(%r12),%edx
-    646c59e3:	mov    0x18(%rax,%rsi,1),%r8
-    646c59e8:	call   646c7dc0 <__report_error>
-    646c59ed:	lea    0x382c(%rip),%rcx        # 646c9220 <.rdata+0x20>
-    646c59f4:	mov    %rbx,%rdx
-    646c59f7:	call   646c7dc0 <__report_error>
-    646c59fc:	nop
-    646c59fd:	nopl   (%rax)
-
-00000000646c5a00 <_pei386_runtime_relocator>:
-    646c5a00:	push   %rbp
-    646c5a01:	push   %r15
-    646c5a03:	push   %r14
-    646c5a05:	push   %r13
-    646c5a07:	push   %r12
-    646c5a09:	push   %rdi
-    646c5a0a:	push   %rsi
-    646c5a0b:	push   %rbx
-    646c5a0c:	sub    $0x38,%rsp
-    646c5a10:	lea    0x80(%rsp),%rbp
-    646c5a18:	mov    0x6e22(%rip),%ebx        # 646cc840 <was_init.95174>
-    646c5a1e:	test   %ebx,%ebx
-    646c5a20:	je     646c5a33 <_pei386_runtime_relocator+0x33>
-    646c5a22:	lea    -0x48(%rbp),%rsp
-    646c5a26:	pop    %rbx
-    646c5a27:	pop    %rsi
-    646c5a28:	pop    %rdi
-    646c5a29:	pop    %r12
-    646c5a2b:	pop    %r13
-    646c5a2d:	pop    %r14
-    646c5a2f:	pop    %r15
-    646c5a31:	pop    %rbp
-    646c5a32:	ret
-    646c5a33:	movl   $0x1,0x6e03(%rip)        # 646cc840 <was_init.95174>
-    646c5a3d:	call   646c6550 <__mingw_GetSectionCount>
-    646c5a42:	cltq
-    646c5a44:	lea    (%rax,%rax,4),%rax
-    646c5a48:	lea    0x1e(,%rax,8),%rax
-    646c5a50:	and    $0xfffffffffffffff0,%rax
-    646c5a54:	call   646c67a0 <___chkstk_ms>
-    646c5a59:	mov    0x3ba0(%rip),%r12        # 646c9600 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
-    646c5a60:	movl   $0x0,0x6dda(%rip)        # 646cc844 <maxSections>
-    646c5a6a:	mov    0x3b9f(%rip),%rsi        # 646c9610 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
-    646c5a71:	sub    %rax,%rsp
-    646c5a74:	lea    0x20(%rsp),%rax
-    646c5a79:	mov    %rax,0x6dc8(%rip)        # 646cc848 <the_secs>
-    646c5a80:	mov    %r12,%rax
-    646c5a83:	sub    %rsi,%rax
-    646c5a86:	cmp    $0x7,%rax
-    646c5a8a:	jle    646c5a22 <_pei386_runtime_relocator+0x22>
-    646c5a8c:	cmp    $0xb,%rax
-    646c5a90:	mov    (%rsi),%edx
-    646c5a92:	jle    646c5b60 <_pei386_runtime_relocator+0x160>
-    646c5a98:	test   %edx,%edx
-    646c5a9a:	je     646c5b44 <_pei386_runtime_relocator+0x144>
-    646c5aa0:	cmp    %r12,%rsi
-    646c5aa3:	jae    646c5a22 <_pei386_runtime_relocator+0x22>
-    646c5aa9:	lea    0x8(%rsi),%r14
-    646c5aad:	add    $0x7,%r12
-    646c5ab1:	mov    0x3b78(%rip),%r13        # 646c9630 <.refptr.__image_base__>
-    646c5ab8:	lea    -0x58(%rbp),%rdi
-    646c5abc:	sub    %r14,%r12
-    646c5abf:	shr    $0x3,%r12
-    646c5ac3:	lea    0x8(%rsi,%r12,8),%r12
-    646c5ac8:	jmp    646c5ad4 <_pei386_runtime_relocator+0xd4>
-    646c5aca:	nopw   0x0(%rax,%rax,1)
-    646c5ad0:	add    $0x8,%r14
-    646c5ad4:	mov    0x4(%rsi),%ecx
-    646c5ad7:	mov    $0x4,%r8d
-    646c5add:	mov    %rdi,%rdx
-    646c5ae0:	mov    (%rsi),%eax
-    646c5ae2:	mov    %r14,%rsi
-    646c5ae5:	add    %r13,%rcx
-    646c5ae8:	add    (%rcx),%eax
-    646c5aea:	mov    %eax,-0x58(%rbp)
-    646c5aed:	call   646c5830 <__write_memory.part.0>
-    646c5af2:	cmp    %r12,%r14
-    646c5af5:	jne    646c5ad0 <_pei386_runtime_relocator+0xd0>
-    646c5af7:	mov    0x6d47(%rip),%eax        # 646cc844 <maxSections>
-    646c5afd:	xor    %esi,%esi
-    646c5aff:	mov    0x8766(%rip),%r12        # 646ce26c <__imp_VirtualProtect>
-    646c5b06:	test   %eax,%eax
-    646c5b08:	jle    646c5a22 <_pei386_runtime_relocator+0x22>
-    646c5b0e:	xchg   %ax,%ax
-    646c5b10:	mov    0x6d31(%rip),%rax        # 646cc848 <the_secs>
-    646c5b17:	add    %rsi,%rax
-    646c5b1a:	mov    (%rax),%r8d
-    646c5b1d:	test   %r8d,%r8d
-    646c5b20:	je     646c5b30 <_pei386_runtime_relocator+0x130>
-    646c5b22:	mov    0x10(%rax),%rdx
-    646c5b26:	mov    %rdi,%r9
-    646c5b29:	mov    0x8(%rax),%rcx
-    646c5b2d:	call   *%r12
-    646c5b30:	add    $0x1,%ebx
-    646c5b33:	add    $0x28,%rsi
-    646c5b37:	cmp    0x6d07(%rip),%ebx        # 646cc844 <maxSections>
-    646c5b3d:	jl     646c5b10 <_pei386_runtime_relocator+0x110>
-    646c5b3f:	jmp    646c5a22 <_pei386_runtime_relocator+0x22>
-    646c5b44:	mov    0x4(%rsi),%ecx
-    646c5b47:	test   %ecx,%ecx
-    646c5b49:	jne    646c5aa0 <_pei386_runtime_relocator+0xa0>
-    646c5b4f:	mov    0x8(%rsi),%edx
-    646c5b52:	test   %edx,%edx
-    646c5b54:	jne    646c5b73 <_pei386_runtime_relocator+0x173>
-    646c5b56:	mov    0xc(%rsi),%edx
-    646c5b59:	add    $0xc,%rsi
-    646c5b5d:	nopl   (%rax)
-    646c5b60:	test   %edx,%edx
-    646c5b62:	jne    646c5aa0 <_pei386_runtime_relocator+0xa0>
-    646c5b68:	mov    0x4(%rsi),%eax
-    646c5b6b:	test   %eax,%eax
-    646c5b6d:	jne    646c5aa0 <_pei386_runtime_relocator+0xa0>
-    646c5b73:	mov    0x8(%rsi),%edx
-    646c5b76:	cmp    $0x1,%edx
-    646c5b79:	jne    646c5cae <_pei386_runtime_relocator+0x2ae>
-    646c5b7f:	mov    0x3aaa(%rip),%r13        # 646c9630 <.refptr.__image_base__>
-    646c5b86:	add    $0xc,%rsi
-    646c5b8a:	movabs $0xffffffff00000000,%r15
-    646c5b94:	lea    -0x58(%rbp),%r14
-    646c5b98:	cmp    %r12,%rsi
-    646c5b9b:	jb     646c5be5 <_pei386_runtime_relocator+0x1e5>
-    646c5b9d:	jmp    646c5a22 <_pei386_runtime_relocator+0x22>
-    646c5ba2:	jbe    646c5c60 <_pei386_runtime_relocator+0x260>
-    646c5ba8:	cmp    $0x20,%edx
-    646c5bab:	je     646c5c30 <_pei386_runtime_relocator+0x230>
-    646c5bb1:	cmp    $0x40,%edx
-    646c5bb4:	jne    646c5c9a <_pei386_runtime_relocator+0x29a>
-    646c5bba:	mov    (%rcx),%rdx
-    646c5bbd:	mov    $0x8,%r8d
-    646c5bc3:	mov    %r14,%rdi
-    646c5bc6:	sub    %rax,%rdx
-    646c5bc9:	add    %r9,%rdx
-    646c5bcc:	mov    %rdx,-0x58(%rbp)
-    646c5bd0:	mov    %r14,%rdx
-    646c5bd3:	call   646c5830 <__write_memory.part.0>
-    646c5bd8:	add    $0xc,%rsi
-    646c5bdc:	cmp    %r12,%rsi
-    646c5bdf:	jae    646c5af7 <_pei386_runtime_relocator+0xf7>
-    646c5be5:	mov    0x4(%rsi),%ecx
-    646c5be8:	mov    (%rsi),%eax
-    646c5bea:	movzbl 0x8(%rsi),%edx
-    646c5bee:	add    %r13,%rcx
-    646c5bf1:	add    %r13,%rax
-    646c5bf4:	cmp    $0x10,%edx
-    646c5bf7:	mov    (%rax),%r9
-    646c5bfa:	jne    646c5ba2 <_pei386_runtime_relocator+0x1a2>
-    646c5bfc:	movzwl (%rcx),%r8d
-    646c5c00:	mov    %r14,%rdx
-    646c5c03:	mov    %r14,%rdi
-    646c5c06:	mov    %r8,%r10
-    646c5c09:	or     $0xffffffffffff0000,%r10
-    646c5c10:	test   %r8w,%r8w
-    646c5c14:	cmovs  %r10,%r8
-    646c5c18:	sub    %rax,%r8
-    646c5c1b:	add    %r9,%r8
-    646c5c1e:	mov    %r8,-0x58(%rbp)
-    646c5c22:	mov    $0x2,%r8d
-    646c5c28:	call   646c5830 <__write_memory.part.0>
-    646c5c2d:	jmp    646c5bd8 <_pei386_runtime_relocator+0x1d8>
-    646c5c2f:	nop
-    646c5c30:	mov    (%rcx),%edx
-    646c5c32:	mov    %r14,%rdi
-    646c5c35:	mov    %rdx,%r8
-    646c5c38:	or     %r15,%rdx
-    646c5c3b:	test   %r8d,%r8d
-    646c5c3e:	cmovns %r8,%rdx
-    646c5c42:	mov    $0x4,%r8d
-    646c5c48:	sub    %rax,%rdx
-    646c5c4b:	add    %r9,%rdx
-    646c5c4e:	mov    %rdx,-0x58(%rbp)
-    646c5c52:	mov    %r14,%rdx
-    646c5c55:	call   646c5830 <__write_memory.part.0>
-    646c5c5a:	jmp    646c5bd8 <_pei386_runtime_relocator+0x1d8>
-    646c5c5f:	nop
-    646c5c60:	cmp    $0x8,%edx
-    646c5c63:	jne    646c5c9a <_pei386_runtime_relocator+0x29a>
-    646c5c65:	movzbl (%rcx),%r8d
-    646c5c69:	mov    %r14,%rdx
-    646c5c6c:	mov    %r14,%rdi
-    646c5c6f:	mov    %r8,%r10
-    646c5c72:	or     $0xffffffffffffff00,%r10
-    646c5c79:	test   %r8b,%r8b
-    646c5c7c:	cmovs  %r10,%r8
-    646c5c80:	sub    %rax,%r8
-    646c5c83:	add    %r9,%r8
-    646c5c86:	mov    %r8,-0x58(%rbp)
-    646c5c8a:	mov    $0x1,%r8d
-    646c5c90:	call   646c5830 <__write_memory.part.0>
-    646c5c95:	jmp    646c5bd8 <_pei386_runtime_relocator+0x1d8>
-    646c5c9a:	lea    0x3637(%rip),%rcx        # 646c92d8 <.rdata+0xd8>
-    646c5ca1:	movq   $0x0,-0x58(%rbp)
-    646c5ca9:	call   646c7dc0 <__report_error>
-    646c5cae:	lea    0x35eb(%rip),%rcx        # 646c92a0 <.rdata+0xa0>
-    646c5cb5:	call   646c7dc0 <__report_error>
-    646c5cba:	nop
-    646c5cbb:	nop
-    646c5cbc:	nop
-    646c5cbd:	nop
-    646c5cbe:	nop
-    646c5cbf:	nop
-
-00000000646c5cc0 <__mingw_SEH_error_handler>:
-    646c5cc0:	sub    $0x28,%rsp
-    646c5cc4:	mov    (%rcx),%eax
-    646c5cc6:	cmp    $0xc0000091,%eax
-    646c5ccb:	ja     646c5d30 <__mingw_SEH_error_handler+0x70>
-    646c5ccd:	cmp    $0xc000008d,%eax
-    646c5cd2:	jae    646c5d4f <__mingw_SEH_error_handler+0x8f>
-    646c5cd4:	cmp    $0xc0000008,%eax
-    646c5cd9:	je     646c5de4 <__mingw_SEH_error_handler+0x124>
-    646c5cdf:	ja     646c5db0 <__mingw_SEH_error_handler+0xf0>
-    646c5ce5:	cmp    $0x80000002,%eax
-    646c5cea:	je     646c5de4 <__mingw_SEH_error_handler+0x124>
-    646c5cf0:	cmp    $0xc0000005,%eax
-    646c5cf5:	jne    646c5dbe <__mingw_SEH_error_handler+0xfe>
-    646c5cfb:	xor    %edx,%edx
-    646c5cfd:	mov    $0xb,%ecx
-    646c5d02:	call   646c7958 <signal>
-    646c5d07:	cmp    $0x1,%rax
-    646c5d0b:	je     646c5e40 <__mingw_SEH_error_handler+0x180>
-    646c5d11:	test   %rax,%rax
-    646c5d14:	je     646c5e56 <__mingw_SEH_error_handler+0x196>
-    646c5d1a:	mov    $0xb,%ecx
-    646c5d1f:	call   *%rax
-    646c5d21:	xor    %eax,%eax
-    646c5d23:	add    $0x28,%rsp
-    646c5d27:	ret
-    646c5d28:	nopl   0x0(%rax,%rax,1)
-    646c5d30:	cmp    $0xc0000094,%eax
-    646c5d35:	je     646c5df0 <__mingw_SEH_error_handler+0x130>
-    646c5d3b:	ja     646c5d74 <__mingw_SEH_error_handler+0xb4>
-    646c5d3d:	cmp    $0xc0000092,%eax
-    646c5d42:	je     646c5de4 <__mingw_SEH_error_handler+0x124>
-    646c5d48:	cmp    $0xc0000093,%eax
-    646c5d4d:	jne    646c5dbe <__mingw_SEH_error_handler+0xfe>
-    646c5d4f:	xor    %edx,%edx
-    646c5d51:	mov    $0x8,%ecx
-    646c5d56:	call   646c7958 <signal>
-    646c5d5b:	cmp    $0x1,%rax
-    646c5d5f:	je     646c5dd0 <__mingw_SEH_error_handler+0x110>
-    646c5d61:	test   %rax,%rax
-    646c5d64:	je     646c5dbe <__mingw_SEH_error_handler+0xfe>
-    646c5d66:	mov    $0x8,%ecx
-    646c5d6b:	call   *%rax
-    646c5d6d:	xor    %eax,%eax
-    646c5d6f:	add    $0x28,%rsp
-    646c5d73:	ret
-    646c5d74:	cmp    $0xc0000095,%eax
-    646c5d79:	je     646c5de4 <__mingw_SEH_error_handler+0x124>
-    646c5d7b:	cmp    $0xc0000096,%eax
-    646c5d80:	jne    646c5dbe <__mingw_SEH_error_handler+0xfe>
-    646c5d82:	xor    %edx,%edx
-    646c5d84:	mov    $0x4,%ecx
-    646c5d89:	call   646c7958 <signal>
-    646c5d8e:	cmp    $0x1,%rax
-    646c5d92:	je     646c5e20 <__mingw_SEH_error_handler+0x160>
-    646c5d98:	test   %rax,%rax
-    646c5d9b:	je     646c5e56 <__mingw_SEH_error_handler+0x196>
-    646c5da1:	mov    $0x4,%ecx
-    646c5da6:	call   *%rax
-    646c5da8:	xor    %eax,%eax
-    646c5daa:	add    $0x28,%rsp
-    646c5dae:	ret
-    646c5daf:	nop
-    646c5db0:	cmp    $0xc000001d,%eax
-    646c5db5:	je     646c5d82 <__mingw_SEH_error_handler+0xc2>
-    646c5db7:	cmp    $0xc000008c,%eax
-    646c5dbc:	je     646c5de4 <__mingw_SEH_error_handler+0x124>
-    646c5dbe:	mov    $0x1,%eax
-    646c5dc3:	add    $0x28,%rsp
-    646c5dc7:	ret
-    646c5dc8:	nopl   0x0(%rax,%rax,1)
-    646c5dd0:	mov    $0x1,%edx
-    646c5dd5:	mov    $0x8,%ecx
-    646c5dda:	call   646c7958 <signal>
-    646c5ddf:	call   646c6790 <_fpreset>
-    646c5de4:	xor    %eax,%eax
-    646c5de6:	add    $0x28,%rsp
-    646c5dea:	ret
-    646c5deb:	nopl   0x0(%rax,%rax,1)
-    646c5df0:	xor    %edx,%edx
-    646c5df2:	mov    $0x8,%ecx
-    646c5df7:	call   646c7958 <signal>
-    646c5dfc:	cmp    $0x1,%rax
-    646c5e00:	jne    646c5d61 <__mingw_SEH_error_handler+0xa1>
-    646c5e06:	mov    $0x1,%edx
-    646c5e0b:	mov    $0x8,%ecx
-    646c5e10:	call   646c7958 <signal>
-    646c5e15:	xor    %eax,%eax
-    646c5e17:	jmp    646c5d23 <__mingw_SEH_error_handler+0x63>
-    646c5e1c:	nopl   0x0(%rax)
-    646c5e20:	mov    $0x1,%edx
-    646c5e25:	mov    $0x4,%ecx
-    646c5e2a:	call   646c7958 <signal>
-    646c5e2f:	xor    %eax,%eax
-    646c5e31:	jmp    646c5d23 <__mingw_SEH_error_handler+0x63>
-    646c5e36:	cs nopw 0x0(%rax,%rax,1)
-    646c5e40:	mov    $0x1,%edx
-    646c5e45:	mov    $0xb,%ecx
-    646c5e4a:	call   646c7958 <signal>
-    646c5e4f:	xor    %eax,%eax
-    646c5e51:	jmp    646c5d23 <__mingw_SEH_error_handler+0x63>
-    646c5e56:	mov    $0x4,%eax
-    646c5e5b:	jmp    646c5d23 <__mingw_SEH_error_handler+0x63>
-
-00000000646c5e60 <__mingw_init_ehandler>:
-    646c5e60:	push   %r12
-    646c5e62:	push   %rbp
-    646c5e63:	push   %rdi
-    646c5e64:	push   %rsi
-    646c5e65:	push   %rbx
-    646c5e66:	sub    $0x20,%rsp
-    646c5e6a:	call   646c6600 <_GetPEImageBase>
-    646c5e6f:	mov    %rax,%rbp
-    646c5e72:	mov    0x69f0(%rip),%eax        # 646cc868 <was_here.95013>
-    646c5e78:	test   %eax,%eax
-    646c5e7a:	jne    646c5ea1 <__mingw_init_ehandler+0x41>
-    646c5e7c:	test   %rbp,%rbp
-    646c5e7f:	je     646c5ea1 <__mingw_init_ehandler+0x41>
-    646c5e81:	lea    0x3488(%rip),%rcx        # 646c9310 <.rdata>
-    646c5e88:	movl   $0x1,0x69d6(%rip)        # 646cc868 <was_here.95013>
-    646c5e92:	call   646c6440 <_FindPESectionByName>
-    646c5e97:	test   %rax,%rax
-    646c5e9a:	je     646c5eb0 <__mingw_init_ehandler+0x50>
-    646c5e9c:	mov    $0x1,%eax
-    646c5ea1:	add    $0x20,%rsp
-    646c5ea5:	pop    %rbx
-    646c5ea6:	pop    %rsi
-    646c5ea7:	pop    %rdi
-    646c5ea8:	pop    %rbp
-    646c5ea9:	pop    %r12
-    646c5eab:	ret
-    646c5eac:	nopl   0x0(%rax)
-    646c5eb0:	lea    0x6ac9(%rip),%rbx        # 646cc980 <emu_pdata>
-    646c5eb7:	mov    $0x30,%ecx
-    646c5ebc:	xor    %esi,%esi
-    646c5ebe:	lea    0x69bb(%rip),%rdx        # 646cc880 <emu_xdata>
-    646c5ec5:	mov    %rbx,%rdi
-    646c5ec8:	rep stos %rax,%es:(%rdi)
-    646c5ecb:	lea    -0x212(%rip),%r12        # 646c5cc0 <__mingw_SEH_error_handler>
-    646c5ed2:	mov    $0x20,%ecx
-    646c5ed7:	mov    %rdx,%rdi
-    646c5eda:	rep stos %rax,%es:(%rdi)
-    646c5edd:	sub    %rbp,%r12
-    646c5ee0:	mov    %rdx,%rdi
-    646c5ee3:	jmp    646c5f13 <__mingw_init_ehandler+0xb3>
-    646c5ee5:	movb   $0x9,(%rdi)
-    646c5ee8:	add    $0x1,%rsi
-    646c5eec:	add    $0xc,%rbx
-    646c5ef0:	mov    %r12d,0x4(%rdi)
-    646c5ef4:	mov    0xc(%rax),%ecx
-    646c5ef7:	mov    %ecx,-0xc(%rbx)
-    646c5efa:	add    0x8(%rax),%ecx
-    646c5efd:	mov    %rdi,%rax
-    646c5f00:	add    $0x8,%rdi
-    646c5f04:	sub    %rbp,%rax
-    646c5f07:	mov    %eax,-0x4(%rbx)
-    646c5f0a:	mov    %ecx,-0x8(%rbx)
-    646c5f0d:	cmp    $0x20,%rsi
-    646c5f11:	je     646c5f45 <__mingw_init_ehandler+0xe5>
-    646c5f13:	mov    %rsi,%rcx
-    646c5f16:	call   646c6590 <_FindPESectionExec>
-    646c5f1b:	test   %rax,%rax
-    646c5f1e:	jne    646c5ee5 <__mingw_init_ehandler+0x85>
-    646c5f20:	test   %rsi,%rsi
-    646c5f23:	mov    %esi,%edx
-    646c5f25:	je     646c5e9c <__mingw_init_ehandler+0x3c>
-    646c5f2b:	nopl   0x0(%rax,%rax,1)
-    646c5f30:	lea    0x6a49(%rip),%rcx        # 646cc980 <emu_pdata>
-    646c5f37:	mov    %rbp,%r8
-    646c5f3a:	call   *0x82e4(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
-    646c5f40:	jmp    646c5e9c <__mingw_init_ehandler+0x3c>
-    646c5f45:	mov    $0x20,%edx
-    646c5f4a:	jmp    646c5f30 <__mingw_init_ehandler+0xd0>
-    646c5f4c:	nopl   0x0(%rax)
-
-00000000646c5f50 <_gnu_exception_handler>:
-    646c5f50:	push   %rbx
-    646c5f51:	sub    $0x20,%rsp
-    646c5f55:	mov    (%rcx),%rdx
-    646c5f58:	mov    (%rdx),%eax
-    646c5f5a:	mov    %rcx,%rbx
-    646c5f5d:	mov    %eax,%ecx
-    646c5f5f:	and    $0x20ffffff,%ecx
-    646c5f65:	cmp    $0x20474343,%ecx
-    646c5f6b:	je     646c6030 <_gnu_exception_handler+0xe0>
-    646c5f71:	cmp    $0xc0000091,%eax
-    646c5f76:	ja     646c5fe0 <_gnu_exception_handler+0x90>
-    646c5f78:	cmp    $0xc000008d,%eax
-    646c5f7d:	jae    646c5ffb <_gnu_exception_handler+0xab>
-    646c5f7f:	cmp    $0xc0000008,%eax
-    646c5f84:	je     646c603a <_gnu_exception_handler+0xea>
-    646c5f8a:	ja     646c6084 <_gnu_exception_handler+0x134>
-    646c5f90:	cmp    $0x80000002,%eax
-    646c5f95:	je     646c603a <_gnu_exception_handler+0xea>
-    646c5f9b:	cmp    $0xc0000005,%eax
-    646c5fa0:	jne    646c5fc1 <_gnu_exception_handler+0x71>
-    646c5fa2:	xor    %edx,%edx
-    646c5fa4:	mov    $0xb,%ecx
-    646c5fa9:	call   646c7958 <signal>
-    646c5fae:	cmp    $0x1,%rax
-    646c5fb2:	je     646c6109 <_gnu_exception_handler+0x1b9>
-    646c5fb8:	test   %rax,%rax
-    646c5fbb:	jne    646c60d0 <_gnu_exception_handler+0x180>
-    646c5fc1:	mov    0x6898(%rip),%rax        # 646cc860 <__mingw_oldexcpt_handler>
-    646c5fc8:	test   %rax,%rax
-    646c5fcb:	je     646c60e1 <_gnu_exception_handler+0x191>
-    646c5fd1:	mov    %rbx,%rcx
-    646c5fd4:	add    $0x20,%rsp
-    646c5fd8:	pop    %rbx
-    646c5fd9:	rex.W jmp *%rax
-    646c5fdc:	nopl   0x0(%rax)
-    646c5fe0:	cmp    $0xc0000094,%eax
-    646c5fe5:	je     646c60a0 <_gnu_exception_handler+0x150>
-    646c5feb:	ja     646c6045 <_gnu_exception_handler+0xf5>
-    646c5fed:	cmp    $0xc0000092,%eax
-    646c5ff2:	je     646c603a <_gnu_exception_handler+0xea>
-    646c5ff4:	cmp    $0xc0000093,%eax
-    646c5ff9:	jne    646c5fc1 <_gnu_exception_handler+0x71>
-    646c5ffb:	xor    %edx,%edx
-    646c5ffd:	mov    $0x8,%ecx
-    646c6002:	call   646c7958 <signal>
-    646c6007:	cmp    $0x1,%rax
-    646c600b:	je     646c60f0 <_gnu_exception_handler+0x1a0>
-    646c6011:	test   %rax,%rax
-    646c6014:	je     646c5fc1 <_gnu_exception_handler+0x71>
-    646c6016:	mov    $0x8,%ecx
-    646c601b:	call   *%rax
-    646c601d:	mov    $0xffffffff,%eax
-    646c6022:	add    $0x20,%rsp
-    646c6026:	pop    %rbx
-    646c6027:	ret
-    646c6028:	nopl   0x0(%rax,%rax,1)
-    646c6030:	testb  $0x1,0x4(%rdx)
-    646c6034:	jne    646c5f71 <_gnu_exception_handler+0x21>
-    646c603a:	mov    $0xffffffff,%eax
-    646c603f:	add    $0x20,%rsp
-    646c6043:	pop    %rbx
-    646c6044:	ret
-    646c6045:	cmp    $0xc0000095,%eax
-    646c604a:	je     646c603a <_gnu_exception_handler+0xea>
-    646c604c:	cmp    $0xc0000096,%eax
-    646c6051:	jne    646c5fc1 <_gnu_exception_handler+0x71>
-    646c6057:	xor    %edx,%edx
-    646c6059:	mov    $0x4,%ecx
-    646c605e:	call   646c7958 <signal>
-    646c6063:	cmp    $0x1,%rax
-    646c6067:	je     646c6120 <_gnu_exception_handler+0x1d0>
-    646c606d:	test   %rax,%rax
-    646c6070:	je     646c5fc1 <_gnu_exception_handler+0x71>
-    646c6076:	mov    $0x4,%ecx
-    646c607b:	call   *%rax
-    646c607d:	mov    $0xffffffff,%eax
-    646c6082:	jmp    646c6022 <_gnu_exception_handler+0xd2>
-    646c6084:	cmp    $0xc000001d,%eax
-    646c6089:	je     646c6057 <_gnu_exception_handler+0x107>
-    646c608b:	cmp    $0xc000008c,%eax
-    646c6090:	jne    646c5fc1 <_gnu_exception_handler+0x71>
-    646c6096:	jmp    646c603a <_gnu_exception_handler+0xea>
-    646c6098:	nopl   0x0(%rax,%rax,1)
-    646c60a0:	xor    %edx,%edx
-    646c60a2:	mov    $0x8,%ecx
-    646c60a7:	call   646c7958 <signal>
-    646c60ac:	cmp    $0x1,%rax
-    646c60b0:	jne    646c6011 <_gnu_exception_handler+0xc1>
-    646c60b6:	mov    $0x1,%edx
-    646c60bb:	mov    $0x8,%ecx
-    646c60c0:	call   646c7958 <signal>
-    646c60c5:	mov    $0xffffffff,%eax
-    646c60ca:	jmp    646c6022 <_gnu_exception_handler+0xd2>
-    646c60cf:	nop
-    646c60d0:	mov    $0xb,%ecx
-    646c60d5:	call   *%rax
-    646c60d7:	mov    $0xffffffff,%eax
-    646c60dc:	jmp    646c6022 <_gnu_exception_handler+0xd2>
-    646c60e1:	xor    %eax,%eax
-    646c60e3:	jmp    646c6022 <_gnu_exception_handler+0xd2>
-    646c60e8:	nopl   0x0(%rax,%rax,1)
-    646c60f0:	mov    $0x1,%edx
-    646c60f5:	mov    $0x8,%ecx
-    646c60fa:	call   646c7958 <signal>
-    646c60ff:	call   646c6790 <_fpreset>
-    646c6104:	jmp    646c603a <_gnu_exception_handler+0xea>
-    646c6109:	mov    $0x1,%edx
-    646c610e:	mov    $0xb,%ecx
-    646c6113:	call   646c7958 <signal>
-    646c6118:	or     $0xffffffff,%eax
-    646c611b:	jmp    646c6022 <_gnu_exception_handler+0xd2>
-    646c6120:	mov    $0x1,%edx
-    646c6125:	mov    $0x4,%ecx
-    646c612a:	call   646c7958 <signal>
-    646c612f:	or     $0xffffffff,%eax
-    646c6132:	jmp    646c6022 <_gnu_exception_handler+0xd2>
-    646c6137:	nop
-    646c6138:	nop
-    646c6139:	nop
-    646c613a:	nop
-    646c613b:	nop
-    646c613c:	nop
-    646c613d:	nop
-    646c613e:	nop
-    646c613f:	nop
-
-00000000646c6140 <__mingwthr_run_key_dtors.part.0>:
-    646c6140:	push   %rbp
-    646c6141:	push   %rdi
-    646c6142:	push   %rsi
-    646c6143:	push   %rbx
-    646c6144:	sub    $0x28,%rsp
-    646c6148:	lea    0x69d1(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c614f:	call   *0x807f(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c6155:	mov    0x69a4(%rip),%rbx        # 646ccb00 <key_dtor_list>
-    646c615c:	test   %rbx,%rbx
-    646c615f:	je     646c6194 <__mingwthr_run_key_dtors.part.0+0x54>
-    646c6161:	mov    0x80f4(%rip),%rbp        # 646ce25c <__imp_TlsGetValue>
-    646c6168:	mov    0x8085(%rip),%rdi        # 646ce1f4 <__imp_GetLastError>
-    646c616f:	nop
-    646c6170:	mov    (%rbx),%ecx
-    646c6172:	call   *%rbp
-    646c6174:	mov    %rax,%rsi
-    646c6177:	call   *%rdi
-    646c6179:	test   %eax,%eax
-    646c617b:	jne    646c618b <__mingwthr_run_key_dtors.part.0+0x4b>
-    646c617d:	test   %rsi,%rsi
-    646c6180:	je     646c618b <__mingwthr_run_key_dtors.part.0+0x4b>
-    646c6182:	mov    0x8(%rbx),%rax
-    646c6186:	mov    %rsi,%rcx
-    646c6189:	call   *%rax
-    646c618b:	mov    0x10(%rbx),%rbx
-    646c618f:	test   %rbx,%rbx
-    646c6192:	jne    646c6170 <__mingwthr_run_key_dtors.part.0+0x30>
-    646c6194:	lea    0x6985(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c619b:	add    $0x28,%rsp
-    646c619f:	pop    %rbx
-    646c61a0:	pop    %rsi
-    646c61a1:	pop    %rdi
-    646c61a2:	pop    %rbp
-    646c61a3:	rex.W jmp *0x806a(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c61aa:	nopw   0x0(%rax,%rax,1)
-
-00000000646c61b0 <___w64_mingwthr_add_key_dtor>:
-    646c61b0:	push   %rbp
-    646c61b1:	push   %rdi
-    646c61b2:	push   %rsi
-    646c61b3:	push   %rbx
-    646c61b4:	sub    $0x28,%rsp
-    646c61b8:	mov    0x694a(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c61be:	xor    %esi,%esi
-    646c61c0:	test   %eax,%eax
-    646c61c2:	mov    %ecx,%ebp
-    646c61c4:	mov    %rdx,%rdi
-    646c61c7:	jne    646c61d4 <___w64_mingwthr_add_key_dtor+0x24>
-    646c61c9:	mov    %esi,%eax
-    646c61cb:	add    $0x28,%rsp
-    646c61cf:	pop    %rbx
-    646c61d0:	pop    %rsi
-    646c61d1:	pop    %rdi
-    646c61d2:	pop    %rbp
-    646c61d3:	ret
-    646c61d4:	mov    $0x18,%edx
-    646c61d9:	mov    $0x1,%ecx
-    646c61de:	call   646c79b0 <calloc>
-    646c61e3:	test   %rax,%rax
-    646c61e6:	mov    %rax,%rbx
-    646c61e9:	je     646c6228 <___w64_mingwthr_add_key_dtor+0x78>
-    646c61eb:	mov    %ebp,(%rax)
-    646c61ed:	lea    0x692c(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c61f4:	mov    %rdi,0x8(%rax)
-    646c61f8:	call   *0x7fd6(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c61fe:	mov    0x68fb(%rip),%rax        # 646ccb00 <key_dtor_list>
-    646c6205:	lea    0x6914(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c620c:	mov    %rbx,0x68ed(%rip)        # 646ccb00 <key_dtor_list>
-    646c6213:	mov    %rax,0x10(%rbx)
-    646c6217:	call   *0x7ff7(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c621d:	mov    %esi,%eax
-    646c621f:	add    $0x28,%rsp
-    646c6223:	pop    %rbx
-    646c6224:	pop    %rsi
-    646c6225:	pop    %rdi
-    646c6226:	pop    %rbp
-    646c6227:	ret
-    646c6228:	mov    $0xffffffff,%esi
-    646c622d:	jmp    646c61c9 <___w64_mingwthr_add_key_dtor+0x19>
-    646c622f:	nop
-
-00000000646c6230 <___w64_mingwthr_remove_key_dtor>:
-    646c6230:	push   %rbx
-    646c6231:	sub    $0x20,%rsp
-    646c6235:	mov    0x68cd(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c623b:	test   %eax,%eax
-    646c623d:	mov    %ecx,%ebx
-    646c623f:	jne    646c6250 <___w64_mingwthr_remove_key_dtor+0x20>
-    646c6241:	xor    %eax,%eax
-    646c6243:	add    $0x20,%rsp
-    646c6247:	pop    %rbx
-    646c6248:	ret
-    646c6249:	nopl   0x0(%rax)
-    646c6250:	lea    0x68c9(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c6257:	call   *0x7f77(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c625d:	mov    0x689c(%rip),%rax        # 646ccb00 <key_dtor_list>
-    646c6264:	test   %rax,%rax
-    646c6267:	je     646c6283 <___w64_mingwthr_remove_key_dtor+0x53>
-    646c6269:	mov    (%rax),%edx
-    646c626b:	cmp    %edx,%ebx
-    646c626d:	jne    646c627a <___w64_mingwthr_remove_key_dtor+0x4a>
-    646c626f:	jmp    646c62c0 <___w64_mingwthr_remove_key_dtor+0x90>
-    646c6271:	mov    (%rcx),%edx
-    646c6273:	cmp    %ebx,%edx
-    646c6275:	je     646c62a0 <___w64_mingwthr_remove_key_dtor+0x70>
-    646c6277:	mov    %rcx,%rax
-    646c627a:	mov    0x10(%rax),%rcx
-    646c627e:	test   %rcx,%rcx
-    646c6281:	jne    646c6271 <___w64_mingwthr_remove_key_dtor+0x41>
-    646c6283:	lea    0x6896(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c628a:	call   *0x7f84(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c6290:	xor    %eax,%eax
-    646c6292:	add    $0x20,%rsp
-    646c6296:	pop    %rbx
-    646c6297:	ret
-    646c6298:	nopl   0x0(%rax,%rax,1)
-    646c62a0:	mov    0x10(%rcx),%rdx
-    646c62a4:	mov    %rdx,0x10(%rax)
-    646c62a8:	call   646c7988 <free>
-    646c62ad:	lea    0x686c(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c62b4:	call   *0x7f5a(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c62ba:	jmp    646c6290 <___w64_mingwthr_remove_key_dtor+0x60>
-    646c62bc:	nopl   0x0(%rax)
-    646c62c0:	mov    0x10(%rax),%rdx
-    646c62c4:	mov    %rax,%rcx
-    646c62c7:	mov    %rdx,0x6832(%rip)        # 646ccb00 <key_dtor_list>
-    646c62ce:	jmp    646c62a8 <___w64_mingwthr_remove_key_dtor+0x78>
-
-00000000646c62d0 <__mingw_TLScallback>:
-    646c62d0:	push   %rbx
-    646c62d1:	sub    $0x20,%rsp
-    646c62d5:	cmp    $0x1,%edx
-    646c62d8:	je     646c6370 <__mingw_TLScallback+0xa0>
-    646c62de:	jb     646c6310 <__mingw_TLScallback+0x40>
-    646c62e0:	cmp    $0x2,%edx
-    646c62e3:	je     646c6300 <__mingw_TLScallback+0x30>
-    646c62e5:	cmp    $0x3,%edx
-    646c62e8:	jne    646c6305 <__mingw_TLScallback+0x35>
-    646c62ea:	mov    0x6818(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c62f0:	test   %eax,%eax
-    646c62f2:	je     646c6305 <__mingw_TLScallback+0x35>
-    646c62f4:	call   646c6140 <__mingwthr_run_key_dtors.part.0>
-    646c62f9:	jmp    646c6305 <__mingw_TLScallback+0x35>
-    646c62fb:	nopl   0x0(%rax,%rax,1)
-    646c6300:	call   646c6790 <_fpreset>
-    646c6305:	mov    $0x1,%eax
-    646c630a:	add    $0x20,%rsp
-    646c630e:	pop    %rbx
-    646c630f:	ret
-    646c6310:	mov    0x67f2(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c6316:	test   %eax,%eax
-    646c6318:	jne    646c63a0 <__mingw_TLScallback+0xd0>
-    646c631e:	mov    0x67e4(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c6324:	cmp    $0x1,%eax
-    646c6327:	jne    646c6305 <__mingw_TLScallback+0x35>
-    646c6329:	mov    0x67d0(%rip),%rcx        # 646ccb00 <key_dtor_list>
-    646c6330:	test   %rcx,%rcx
-    646c6333:	je     646c6346 <__mingw_TLScallback+0x76>
-    646c6335:	mov    0x10(%rcx),%rbx
-    646c6339:	call   646c7988 <free>
-    646c633e:	test   %rbx,%rbx
-    646c6341:	mov    %rbx,%rcx
-    646c6344:	jne    646c6335 <__mingw_TLScallback+0x65>
-    646c6346:	lea    0x67d3(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c634d:	movq   $0x0,0x67a8(%rip)        # 646ccb00 <key_dtor_list>
-    646c6358:	movl   $0x0,0x67a6(%rip)        # 646ccb08 <__mingwthr_cs_init>
-    646c6362:	call   *0x7e64(%rip)        # 646ce1cc <__IAT_start__>
-    646c6368:	jmp    646c6305 <__mingw_TLScallback+0x35>
-    646c636a:	nopw   0x0(%rax,%rax,1)
-    646c6370:	mov    0x6792(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
-    646c6376:	test   %eax,%eax
-    646c6378:	je     646c6390 <__mingw_TLScallback+0xc0>
-    646c637a:	movl   $0x1,0x6784(%rip)        # 646ccb08 <__mingwthr_cs_init>
-    646c6384:	mov    $0x1,%eax
-    646c6389:	add    $0x20,%rsp
-    646c638d:	pop    %rbx
-    646c638e:	ret
-    646c638f:	nop
-    646c6390:	lea    0x6789(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
-    646c6397:	call   *0x7e6f(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
-    646c639d:	jmp    646c637a <__mingw_TLScallback+0xaa>
-    646c639f:	nop
-    646c63a0:	call   646c6140 <__mingwthr_run_key_dtors.part.0>
-    646c63a5:	jmp    646c631e <__mingw_TLScallback+0x4e>
-    646c63aa:	nop
-    646c63ab:	nop
-    646c63ac:	nop
-    646c63ad:	nop
-    646c63ae:	nop
-    646c63af:	nop
-
-00000000646c63b0 <_ValidateImageBase.part.0>:
-    646c63b0:	movslq 0x3c(%rcx),%rax
-    646c63b4:	add    %rax,%rcx
-    646c63b7:	xor    %eax,%eax
-    646c63b9:	cmpl   $0x4550,(%rcx)
-    646c63bf:	je     646c63c2 <_ValidateImageBase.part.0+0x12>
-    646c63c1:	ret
-    646c63c2:	xor    %eax,%eax
-    646c63c4:	cmpw   $0x20b,0x18(%rcx)
-    646c63ca:	sete   %al
-    646c63cd:	ret
-    646c63ce:	xchg   %ax,%ax
-
-00000000646c63d0 <_ValidateImageBase>:
-    646c63d0:	cmpw   $0x5a4d,(%rcx)
-    646c63d5:	je     646c63e0 <_ValidateImageBase+0x10>
-    646c63d7:	xor    %eax,%eax
-    646c63d9:	ret
-    646c63da:	nopw   0x0(%rax,%rax,1)
-    646c63e0:	jmp    646c63b0 <_ValidateImageBase.part.0>
-    646c63e2:	nopl   0x0(%rax)
+    646c5570:	mov    (%rax),%rdx
+    646c5573:	cmp    %rdx,%rbx
+    646c5576:	jb     646c558c <__write_memory.part.0+0x4c>
+    646c5578:	mov    0x8(%rax),%r8
+    646c557c:	mov    0x8(%r8),%r8d
+    646c5580:	add    %r8,%rdx
+    646c5583:	cmp    %rdx,%rbx
+    646c5586:	jb     646c5615 <__write_memory.part.0+0xd5>
+    646c558c:	add    $0x1,%ecx
+    646c558f:	add    $0x28,%rax
+    646c5593:	cmp    %esi,%ecx
+    646c5595:	jne    646c5570 <__write_memory.part.0+0x30>
+    646c5597:	mov    %rbx,%rcx
+    646c559a:	call   646c61e0 <__mingw_GetSectionForAddress>
+    646c559f:	test   %rax,%rax
+    646c55a2:	mov    %rax,%r12
+    646c55a5:	je     646c56fd <__write_memory.part.0+0x1bd>
+    646c55ab:	mov    0x7296(%rip),%rax        # 646cc848 <the_secs>
+    646c55b2:	lea    (%rsi,%rsi,4),%rsi
+    646c55b6:	shl    $0x3,%rsi
+    646c55ba:	add    %rsi,%rax
+    646c55bd:	mov    %r12,0x20(%rax)
+    646c55c1:	movl   $0x0,(%rax)
+    646c55c7:	call   646c6310 <_GetPEImageBase>
+    646c55cc:	mov    0xc(%r12),%ecx
+    646c55d1:	lea    0x20(%rsp),%rdx
+    646c55d6:	mov    $0x30,%r8d
+    646c55dc:	add    %rax,%rcx
+    646c55df:	mov    0x7262(%rip),%rax        # 646cc848 <the_secs>
+    646c55e6:	mov    %rcx,0x18(%rax,%rsi,1)
+    646c55eb:	call   *0x8c83(%rip)        # 646ce274 <__imp_VirtualQuery>
+    646c55f1:	test   %rax,%rax
+    646c55f4:	je     646c56e0 <__write_memory.part.0+0x1a0>
+    646c55fa:	mov    0x44(%rsp),%eax
+    646c55fe:	lea    -0x4(%rax),%edx
+    646c5601:	and    $0xfffffffb,%edx
+    646c5604:	je     646c560e <__write_memory.part.0+0xce>
+    646c5606:	sub    $0x40,%eax
+    646c5609:	and    $0xffffffbf,%eax
+    646c560c:	jne    646c5670 <__write_memory.part.0+0x130>
+    646c560e:	addl   $0x1,0x722f(%rip)        # 646cc844 <maxSections>
+    646c5615:	cmp    $0x8,%edi
+    646c5618:	jae    646c5643 <__write_memory.part.0+0x103>
+    646c561a:	test   $0x4,%dil
+    646c561e:	jne    646c56b4 <__write_memory.part.0+0x174>
+    646c5624:	test   %edi,%edi
+    646c5626:	je     646c5638 <__write_memory.part.0+0xf8>
+    646c5628:	movzbl 0x0(%rbp),%eax
+    646c562c:	test   $0x2,%dil
+    646c5630:	mov    %al,(%rbx)
+    646c5632:	jne    646c56cf <__write_memory.part.0+0x18f>
+    646c5638:	add    $0x50,%rsp
+    646c563c:	pop    %rbx
+    646c563d:	pop    %rsi
+    646c563e:	pop    %rdi
+    646c563f:	pop    %rbp
+    646c5640:	pop    %r12
+    646c5642:	ret
+    646c5643:	mov    %edi,%eax
+    646c5645:	sub    $0x1,%edi
+    646c5648:	mov    -0x8(%rbp,%rax,1),%rdx
+    646c564d:	cmp    $0x8,%edi
+    646c5650:	mov    %rdx,-0x8(%rbx,%rax,1)
+    646c5655:	jb     646c5638 <__write_memory.part.0+0xf8>
+    646c5657:	and    $0xfffffff8,%edi
+    646c565a:	xor    %eax,%eax
+    646c565c:	mov    %eax,%edx
+    646c565e:	add    $0x8,%eax
+    646c5661:	mov    0x0(%rbp,%rdx,1),%rcx
+    646c5666:	cmp    %edi,%eax
+    646c5668:	mov    %rcx,(%rbx,%rdx,1)
+    646c566c:	jb     646c565c <__write_memory.part.0+0x11c>
+    646c566e:	jmp    646c5638 <__write_memory.part.0+0xf8>
+    646c5670:	add    0x71d1(%rip),%rsi        # 646cc848 <the_secs>
+    646c5677:	mov    $0x40,%r8d
+    646c567d:	mov    0x20(%rsp),%rcx
+    646c5682:	mov    0x38(%rsp),%rdx
+    646c5687:	mov    %rsi,%r9
+    646c568a:	mov    %rcx,0x8(%rsi)
+    646c568e:	mov    %rdx,0x10(%rsi)
+    646c5692:	call   *0x8bd4(%rip)        # 646ce26c <__imp_VirtualProtect>
+    646c5698:	test   %eax,%eax
+    646c569a:	jne    646c560e <__write_memory.part.0+0xce>
+    646c56a0:	call   *0x8b4e(%rip)        # 646ce1f4 <__imp_GetLastError>
+    646c56a6:	lea    0x3bab(%rip),%rcx        # 646c9258 <.rdata+0x78>
+    646c56ad:	mov    %eax,%edx
+    646c56af:	call   646c7ad0 <__report_error>
+    646c56b4:	mov    0x0(%rbp),%eax
+    646c56b7:	mov    %edi,%edi
+    646c56b9:	mov    %eax,(%rbx)
+    646c56bb:	mov    -0x4(%rbp,%rdi,1),%eax
+    646c56bf:	mov    %eax,-0x4(%rbx,%rdi,1)
+    646c56c3:	jmp    646c5638 <__write_memory.part.0+0xf8>
+    646c56c8:	xor    %esi,%esi
+    646c56ca:	jmp    646c5597 <__write_memory.part.0+0x57>
+    646c56cf:	mov    %edi,%edi
+    646c56d1:	movzwl -0x2(%rbp,%rdi,1),%eax
+    646c56d6:	mov    %ax,-0x2(%rbx,%rdi,1)
+    646c56db:	jmp    646c5638 <__write_memory.part.0+0xf8>
+    646c56e0:	mov    0x7161(%rip),%rax        # 646cc848 <the_secs>
+    646c56e7:	lea    0x3b32(%rip),%rcx        # 646c9220 <.rdata+0x40>
+    646c56ee:	mov    0x8(%r12),%edx
+    646c56f3:	mov    0x18(%rax,%rsi,1),%r8
+    646c56f8:	call   646c7ad0 <__report_error>
+    646c56fd:	lea    0x3afc(%rip),%rcx        # 646c9200 <.rdata+0x20>
+    646c5704:	mov    %rbx,%rdx
+    646c5707:	call   646c7ad0 <__report_error>
+    646c570c:	nop
+    646c570d:	nopl   (%rax)
+
+00000000646c5710 <_pei386_runtime_relocator>:
+    646c5710:	push   %rbp
+    646c5711:	push   %r15
+    646c5713:	push   %r14
+    646c5715:	push   %r13
+    646c5717:	push   %r12
+    646c5719:	push   %rdi
+    646c571a:	push   %rsi
+    646c571b:	push   %rbx
+    646c571c:	sub    $0x38,%rsp
+    646c5720:	lea    0x80(%rsp),%rbp
+    646c5728:	mov    0x7112(%rip),%ebx        # 646cc840 <was_init.95174>
+    646c572e:	test   %ebx,%ebx
+    646c5730:	je     646c5743 <_pei386_runtime_relocator+0x33>
+    646c5732:	lea    -0x48(%rbp),%rsp
+    646c5736:	pop    %rbx
+    646c5737:	pop    %rsi
+    646c5738:	pop    %rdi
+    646c5739:	pop    %r12
+    646c573b:	pop    %r13
+    646c573d:	pop    %r14
+    646c573f:	pop    %r15
+    646c5741:	pop    %rbp
+    646c5742:	ret
+    646c5743:	movl   $0x1,0x70f3(%rip)        # 646cc840 <was_init.95174>
+    646c574d:	call   646c6260 <__mingw_GetSectionCount>
+    646c5752:	cltq
+    646c5754:	lea    (%rax,%rax,4),%rax
+    646c5758:	lea    0x1e(,%rax,8),%rax
+    646c5760:	and    $0xfffffffffffffff0,%rax
+    646c5764:	call   646c64b0 <___chkstk_ms>
+    646c5769:	mov    0x3e70(%rip),%r12        # 646c95e0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>
+    646c5770:	movl   $0x0,0x70ca(%rip)        # 646cc844 <maxSections>
+    646c577a:	mov    0x3e6f(%rip),%rsi        # 646c95f0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>
+    646c5781:	sub    %rax,%rsp
+    646c5784:	lea    0x20(%rsp),%rax
+    646c5789:	mov    %rax,0x70b8(%rip)        # 646cc848 <the_secs>
+    646c5790:	mov    %r12,%rax
+    646c5793:	sub    %rsi,%rax
+    646c5796:	cmp    $0x7,%rax
+    646c579a:	jle    646c5732 <_pei386_runtime_relocator+0x22>
+    646c579c:	cmp    $0xb,%rax
+    646c57a0:	mov    (%rsi),%edx
+    646c57a2:	jle    646c5870 <_pei386_runtime_relocator+0x160>
+    646c57a8:	test   %edx,%edx
+    646c57aa:	je     646c5854 <_pei386_runtime_relocator+0x144>
+    646c57b0:	cmp    %r12,%rsi
+    646c57b3:	jae    646c5732 <_pei386_runtime_relocator+0x22>
+    646c57b9:	lea    0x8(%rsi),%r14
+    646c57bd:	add    $0x7,%r12
+    646c57c1:	mov    0x3e48(%rip),%r13        # 646c9610 <.refptr.__image_base__>
+    646c57c8:	lea    -0x58(%rbp),%rdi
+    646c57cc:	sub    %r14,%r12
+    646c57cf:	shr    $0x3,%r12
+    646c57d3:	lea    0x8(%rsi,%r12,8),%r12
+    646c57d8:	jmp    646c57e4 <_pei386_runtime_relocator+0xd4>
+    646c57da:	nopw   0x0(%rax,%rax,1)
+    646c57e0:	add    $0x8,%r14
+    646c57e4:	mov    0x4(%rsi),%ecx
+    646c57e7:	mov    $0x4,%r8d
+    646c57ed:	mov    %rdi,%rdx
+    646c57f0:	mov    (%rsi),%eax
+    646c57f2:	mov    %r14,%rsi
+    646c57f5:	add    %r13,%rcx
+    646c57f8:	add    (%rcx),%eax
+    646c57fa:	mov    %eax,-0x58(%rbp)
+    646c57fd:	call   646c5540 <__write_memory.part.0>
+    646c5802:	cmp    %r12,%r14
+    646c5805:	jne    646c57e0 <_pei386_runtime_relocator+0xd0>
+    646c5807:	mov    0x7037(%rip),%eax        # 646cc844 <maxSections>
+    646c580d:	xor    %esi,%esi
+    646c580f:	mov    0x8a56(%rip),%r12        # 646ce26c <__imp_VirtualProtect>
+    646c5816:	test   %eax,%eax
+    646c5818:	jle    646c5732 <_pei386_runtime_relocator+0x22>
+    646c581e:	xchg   %ax,%ax
+    646c5820:	mov    0x7021(%rip),%rax        # 646cc848 <the_secs>
+    646c5827:	add    %rsi,%rax
+    646c582a:	mov    (%rax),%r8d
+    646c582d:	test   %r8d,%r8d
+    646c5830:	je     646c5840 <_pei386_runtime_relocator+0x130>
+    646c5832:	mov    0x10(%rax),%rdx
+    646c5836:	mov    %rdi,%r9
+    646c5839:	mov    0x8(%rax),%rcx
+    646c583d:	call   *%r12
+    646c5840:	add    $0x1,%ebx
+    646c5843:	add    $0x28,%rsi
+    646c5847:	cmp    0x6ff7(%rip),%ebx        # 646cc844 <maxSections>
+    646c584d:	jl     646c5820 <_pei386_runtime_relocator+0x110>
+    646c584f:	jmp    646c5732 <_pei386_runtime_relocator+0x22>
+    646c5854:	mov    0x4(%rsi),%ecx
+    646c5857:	test   %ecx,%ecx
+    646c5859:	jne    646c57b0 <_pei386_runtime_relocator+0xa0>
+    646c585f:	mov    0x8(%rsi),%edx
+    646c5862:	test   %edx,%edx
+    646c5864:	jne    646c5883 <_pei386_runtime_relocator+0x173>
+    646c5866:	mov    0xc(%rsi),%edx
+    646c5869:	add    $0xc,%rsi
+    646c586d:	nopl   (%rax)
+    646c5870:	test   %edx,%edx
+    646c5872:	jne    646c57b0 <_pei386_runtime_relocator+0xa0>
+    646c5878:	mov    0x4(%rsi),%eax
+    646c587b:	test   %eax,%eax
+    646c587d:	jne    646c57b0 <_pei386_runtime_relocator+0xa0>
+    646c5883:	mov    0x8(%rsi),%edx
+    646c5886:	cmp    $0x1,%edx
+    646c5889:	jne    646c59be <_pei386_runtime_relocator+0x2ae>
+    646c588f:	mov    0x3d7a(%rip),%r13        # 646c9610 <.refptr.__image_base__>
+    646c5896:	add    $0xc,%rsi
+    646c589a:	movabs $0xffffffff00000000,%r15
+    646c58a4:	lea    -0x58(%rbp),%r14
+    646c58a8:	cmp    %r12,%rsi
+    646c58ab:	jb     646c58f5 <_pei386_runtime_relocator+0x1e5>
+    646c58ad:	jmp    646c5732 <_pei386_runtime_relocator+0x22>
+    646c58b2:	jbe    646c5970 <_pei386_runtime_relocator+0x260>
+    646c58b8:	cmp    $0x20,%edx
+    646c58bb:	je     646c5940 <_pei386_runtime_relocator+0x230>
+    646c58c1:	cmp    $0x40,%edx
+    646c58c4:	jne    646c59aa <_pei386_runtime_relocator+0x29a>
+    646c58ca:	mov    (%rcx),%rdx
+    646c58cd:	mov    $0x8,%r8d
+    646c58d3:	mov    %r14,%rdi
+    646c58d6:	sub    %rax,%rdx
+    646c58d9:	add    %r9,%rdx
+    646c58dc:	mov    %rdx,-0x58(%rbp)
+    646c58e0:	mov    %r14,%rdx
+    646c58e3:	call   646c5540 <__write_memory.part.0>
+    646c58e8:	add    $0xc,%rsi
+    646c58ec:	cmp    %r12,%rsi
+    646c58ef:	jae    646c5807 <_pei386_runtime_relocator+0xf7>
+    646c58f5:	mov    0x4(%rsi),%ecx
+    646c58f8:	mov    (%rsi),%eax
+    646c58fa:	movzbl 0x8(%rsi),%edx
+    646c58fe:	add    %r13,%rcx
+    646c5901:	add    %r13,%rax
+    646c5904:	cmp    $0x10,%edx
+    646c5907:	mov    (%rax),%r9
+    646c590a:	jne    646c58b2 <_pei386_runtime_relocator+0x1a2>
+    646c590c:	movzwl (%rcx),%r8d
+    646c5910:	mov    %r14,%rdx
+    646c5913:	mov    %r14,%rdi
+    646c5916:	mov    %r8,%r10
+    646c5919:	or     $0xffffffffffff0000,%r10
+    646c5920:	test   %r8w,%r8w
+    646c5924:	cmovs  %r10,%r8
+    646c5928:	sub    %rax,%r8
+    646c592b:	add    %r9,%r8
+    646c592e:	mov    %r8,-0x58(%rbp)
+    646c5932:	mov    $0x2,%r8d
+    646c5938:	call   646c5540 <__write_memory.part.0>
+    646c593d:	jmp    646c58e8 <_pei386_runtime_relocator+0x1d8>
+    646c593f:	nop
+    646c5940:	mov    (%rcx),%edx
+    646c5942:	mov    %r14,%rdi
+    646c5945:	mov    %rdx,%r8
+    646c5948:	or     %r15,%rdx
+    646c594b:	test   %r8d,%r8d
+    646c594e:	cmovns %r8,%rdx
+    646c5952:	mov    $0x4,%r8d
+    646c5958:	sub    %rax,%rdx
+    646c595b:	add    %r9,%rdx
+    646c595e:	mov    %rdx,-0x58(%rbp)
+    646c5962:	mov    %r14,%rdx
+    646c5965:	call   646c5540 <__write_memory.part.0>
+    646c596a:	jmp    646c58e8 <_pei386_runtime_relocator+0x1d8>
+    646c596f:	nop
+    646c5970:	cmp    $0x8,%edx
+    646c5973:	jne    646c59aa <_pei386_runtime_relocator+0x29a>
+    646c5975:	movzbl (%rcx),%r8d
+    646c5979:	mov    %r14,%rdx
+    646c597c:	mov    %r14,%rdi
+    646c597f:	mov    %r8,%r10
+    646c5982:	or     $0xffffffffffffff00,%r10
+    646c5989:	test   %r8b,%r8b
+    646c598c:	cmovs  %r10,%r8
+    646c5990:	sub    %rax,%r8
+    646c5993:	add    %r9,%r8
+    646c5996:	mov    %r8,-0x58(%rbp)
+    646c599a:	mov    $0x1,%r8d
+    646c59a0:	call   646c5540 <__write_memory.part.0>
+    646c59a5:	jmp    646c58e8 <_pei386_runtime_relocator+0x1d8>
+    646c59aa:	lea    0x3907(%rip),%rcx        # 646c92b8 <.rdata+0xd8>
+    646c59b1:	movq   $0x0,-0x58(%rbp)
+    646c59b9:	call   646c7ad0 <__report_error>
+    646c59be:	lea    0x38bb(%rip),%rcx        # 646c9280 <.rdata+0xa0>
+    646c59c5:	call   646c7ad0 <__report_error>
+    646c59ca:	nop
+    646c59cb:	nop
+    646c59cc:	nop
+    646c59cd:	nop
+    646c59ce:	nop
+    646c59cf:	nop
+
+00000000646c59d0 <__mingw_SEH_error_handler>:
+    646c59d0:	sub    $0x28,%rsp
+    646c59d4:	mov    (%rcx),%eax
+    646c59d6:	cmp    $0xc0000091,%eax
+    646c59db:	ja     646c5a40 <__mingw_SEH_error_handler+0x70>
+    646c59dd:	cmp    $0xc000008d,%eax
+    646c59e2:	jae    646c5a5f <__mingw_SEH_error_handler+0x8f>
+    646c59e4:	cmp    $0xc0000008,%eax
+    646c59e9:	je     646c5af4 <__mingw_SEH_error_handler+0x124>
+    646c59ef:	ja     646c5ac0 <__mingw_SEH_error_handler+0xf0>
+    646c59f5:	cmp    $0x80000002,%eax
+    646c59fa:	je     646c5af4 <__mingw_SEH_error_handler+0x124>
+    646c5a00:	cmp    $0xc0000005,%eax
+    646c5a05:	jne    646c5ace <__mingw_SEH_error_handler+0xfe>
+    646c5a0b:	xor    %edx,%edx
+    646c5a0d:	mov    $0xb,%ecx
+    646c5a12:	call   646c7668 <signal>
+    646c5a17:	cmp    $0x1,%rax
+    646c5a1b:	je     646c5b50 <__mingw_SEH_error_handler+0x180>
+    646c5a21:	test   %rax,%rax
+    646c5a24:	je     646c5b66 <__mingw_SEH_error_handler+0x196>
+    646c5a2a:	mov    $0xb,%ecx
+    646c5a2f:	call   *%rax
+    646c5a31:	xor    %eax,%eax
+    646c5a33:	add    $0x28,%rsp
+    646c5a37:	ret
+    646c5a38:	nopl   0x0(%rax,%rax,1)
+    646c5a40:	cmp    $0xc0000094,%eax
+    646c5a45:	je     646c5b00 <__mingw_SEH_error_handler+0x130>
+    646c5a4b:	ja     646c5a84 <__mingw_SEH_error_handler+0xb4>
+    646c5a4d:	cmp    $0xc0000092,%eax
+    646c5a52:	je     646c5af4 <__mingw_SEH_error_handler+0x124>
+    646c5a58:	cmp    $0xc0000093,%eax
+    646c5a5d:	jne    646c5ace <__mingw_SEH_error_handler+0xfe>
+    646c5a5f:	xor    %edx,%edx
+    646c5a61:	mov    $0x8,%ecx
+    646c5a66:	call   646c7668 <signal>
+    646c5a6b:	cmp    $0x1,%rax
+    646c5a6f:	je     646c5ae0 <__mingw_SEH_error_handler+0x110>
+    646c5a71:	test   %rax,%rax
+    646c5a74:	je     646c5ace <__mingw_SEH_error_handler+0xfe>
+    646c5a76:	mov    $0x8,%ecx
+    646c5a7b:	call   *%rax
+    646c5a7d:	xor    %eax,%eax
+    646c5a7f:	add    $0x28,%rsp
+    646c5a83:	ret
+    646c5a84:	cmp    $0xc0000095,%eax
+    646c5a89:	je     646c5af4 <__mingw_SEH_error_handler+0x124>
+    646c5a8b:	cmp    $0xc0000096,%eax
+    646c5a90:	jne    646c5ace <__mingw_SEH_error_handler+0xfe>
+    646c5a92:	xor    %edx,%edx
+    646c5a94:	mov    $0x4,%ecx
+    646c5a99:	call   646c7668 <signal>
+    646c5a9e:	cmp    $0x1,%rax
+    646c5aa2:	je     646c5b30 <__mingw_SEH_error_handler+0x160>
+    646c5aa8:	test   %rax,%rax
+    646c5aab:	je     646c5b66 <__mingw_SEH_error_handler+0x196>
+    646c5ab1:	mov    $0x4,%ecx
+    646c5ab6:	call   *%rax
+    646c5ab8:	xor    %eax,%eax
+    646c5aba:	add    $0x28,%rsp
+    646c5abe:	ret
+    646c5abf:	nop
+    646c5ac0:	cmp    $0xc000001d,%eax
+    646c5ac5:	je     646c5a92 <__mingw_SEH_error_handler+0xc2>
+    646c5ac7:	cmp    $0xc000008c,%eax
+    646c5acc:	je     646c5af4 <__mingw_SEH_error_handler+0x124>
+    646c5ace:	mov    $0x1,%eax
+    646c5ad3:	add    $0x28,%rsp
+    646c5ad7:	ret
+    646c5ad8:	nopl   0x0(%rax,%rax,1)
+    646c5ae0:	mov    $0x1,%edx
+    646c5ae5:	mov    $0x8,%ecx
+    646c5aea:	call   646c7668 <signal>
+    646c5aef:	call   646c64a0 <_fpreset>
+    646c5af4:	xor    %eax,%eax
+    646c5af6:	add    $0x28,%rsp
+    646c5afa:	ret
+    646c5afb:	nopl   0x0(%rax,%rax,1)
+    646c5b00:	xor    %edx,%edx
+    646c5b02:	mov    $0x8,%ecx
+    646c5b07:	call   646c7668 <signal>
+    646c5b0c:	cmp    $0x1,%rax
+    646c5b10:	jne    646c5a71 <__mingw_SEH_error_handler+0xa1>
+    646c5b16:	mov    $0x1,%edx
+    646c5b1b:	mov    $0x8,%ecx
+    646c5b20:	call   646c7668 <signal>
+    646c5b25:	xor    %eax,%eax
+    646c5b27:	jmp    646c5a33 <__mingw_SEH_error_handler+0x63>
+    646c5b2c:	nopl   0x0(%rax)
+    646c5b30:	mov    $0x1,%edx
+    646c5b35:	mov    $0x4,%ecx
+    646c5b3a:	call   646c7668 <signal>
+    646c5b3f:	xor    %eax,%eax
+    646c5b41:	jmp    646c5a33 <__mingw_SEH_error_handler+0x63>
+    646c5b46:	cs nopw 0x0(%rax,%rax,1)
+    646c5b50:	mov    $0x1,%edx
+    646c5b55:	mov    $0xb,%ecx
+    646c5b5a:	call   646c7668 <signal>
+    646c5b5f:	xor    %eax,%eax
+    646c5b61:	jmp    646c5a33 <__mingw_SEH_error_handler+0x63>
+    646c5b66:	mov    $0x4,%eax
+    646c5b6b:	jmp    646c5a33 <__mingw_SEH_error_handler+0x63>
+
+00000000646c5b70 <__mingw_init_ehandler>:
+    646c5b70:	push   %r12
+    646c5b72:	push   %rbp
+    646c5b73:	push   %rdi
+    646c5b74:	push   %rsi
+    646c5b75:	push   %rbx
+    646c5b76:	sub    $0x20,%rsp
+    646c5b7a:	call   646c6310 <_GetPEImageBase>
+    646c5b7f:	mov    %rax,%rbp
+    646c5b82:	mov    0x6ce0(%rip),%eax        # 646cc868 <was_here.95013>
+    646c5b88:	test   %eax,%eax
+    646c5b8a:	jne    646c5bb1 <__mingw_init_ehandler+0x41>
+    646c5b8c:	test   %rbp,%rbp
+    646c5b8f:	je     646c5bb1 <__mingw_init_ehandler+0x41>
+    646c5b91:	lea    0x3758(%rip),%rcx        # 646c92f0 <.rdata>
+    646c5b98:	movl   $0x1,0x6cc6(%rip)        # 646cc868 <was_here.95013>
+    646c5ba2:	call   646c6150 <_FindPESectionByName>
+    646c5ba7:	test   %rax,%rax
+    646c5baa:	je     646c5bc0 <__mingw_init_ehandler+0x50>
+    646c5bac:	mov    $0x1,%eax
+    646c5bb1:	add    $0x20,%rsp
+    646c5bb5:	pop    %rbx
+    646c5bb6:	pop    %rsi
+    646c5bb7:	pop    %rdi
+    646c5bb8:	pop    %rbp
+    646c5bb9:	pop    %r12
+    646c5bbb:	ret
+    646c5bbc:	nopl   0x0(%rax)
+    646c5bc0:	lea    0x6db9(%rip),%rbx        # 646cc980 <emu_pdata>
+    646c5bc7:	mov    $0x30,%ecx
+    646c5bcc:	xor    %esi,%esi
+    646c5bce:	lea    0x6cab(%rip),%rdx        # 646cc880 <emu_xdata>
+    646c5bd5:	mov    %rbx,%rdi
+    646c5bd8:	rep stos %rax,%es:(%rdi)
+    646c5bdb:	lea    -0x212(%rip),%r12        # 646c59d0 <__mingw_SEH_error_handler>
+    646c5be2:	mov    $0x20,%ecx
+    646c5be7:	mov    %rdx,%rdi
+    646c5bea:	rep stos %rax,%es:(%rdi)
+    646c5bed:	sub    %rbp,%r12
+    646c5bf0:	mov    %rdx,%rdi
+    646c5bf3:	jmp    646c5c23 <__mingw_init_ehandler+0xb3>
+    646c5bf5:	movb   $0x9,(%rdi)
+    646c5bf8:	add    $0x1,%rsi
+    646c5bfc:	add    $0xc,%rbx
+    646c5c00:	mov    %r12d,0x4(%rdi)
+    646c5c04:	mov    0xc(%rax),%ecx
+    646c5c07:	mov    %ecx,-0xc(%rbx)
+    646c5c0a:	add    0x8(%rax),%ecx
+    646c5c0d:	mov    %rdi,%rax
+    646c5c10:	add    $0x8,%rdi
+    646c5c14:	sub    %rbp,%rax
+    646c5c17:	mov    %eax,-0x4(%rbx)
+    646c5c1a:	mov    %ecx,-0x8(%rbx)
+    646c5c1d:	cmp    $0x20,%rsi
+    646c5c21:	je     646c5c55 <__mingw_init_ehandler+0xe5>
+    646c5c23:	mov    %rsi,%rcx
+    646c5c26:	call   646c62a0 <_FindPESectionExec>
+    646c5c2b:	test   %rax,%rax
+    646c5c2e:	jne    646c5bf5 <__mingw_init_ehandler+0x85>
+    646c5c30:	test   %rsi,%rsi
+    646c5c33:	mov    %esi,%edx
+    646c5c35:	je     646c5bac <__mingw_init_ehandler+0x3c>
+    646c5c3b:	nopl   0x0(%rax,%rax,1)
+    646c5c40:	lea    0x6d39(%rip),%rcx        # 646cc980 <emu_pdata>
+    646c5c47:	mov    %rbp,%r8
+    646c5c4a:	call   *0x85d4(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
+    646c5c50:	jmp    646c5bac <__mingw_init_ehandler+0x3c>
+    646c5c55:	mov    $0x20,%edx
+    646c5c5a:	jmp    646c5c40 <__mingw_init_ehandler+0xd0>
+    646c5c5c:	nopl   0x0(%rax)
+
+00000000646c5c60 <_gnu_exception_handler>:
+    646c5c60:	push   %rbx
+    646c5c61:	sub    $0x20,%rsp
+    646c5c65:	mov    (%rcx),%rdx
+    646c5c68:	mov    (%rdx),%eax
+    646c5c6a:	mov    %rcx,%rbx
+    646c5c6d:	mov    %eax,%ecx
+    646c5c6f:	and    $0x20ffffff,%ecx
+    646c5c75:	cmp    $0x20474343,%ecx
+    646c5c7b:	je     646c5d40 <_gnu_exception_handler+0xe0>
+    646c5c81:	cmp    $0xc0000091,%eax
+    646c5c86:	ja     646c5cf0 <_gnu_exception_handler+0x90>
+    646c5c88:	cmp    $0xc000008d,%eax
+    646c5c8d:	jae    646c5d0b <_gnu_exception_handler+0xab>
+    646c5c8f:	cmp    $0xc0000008,%eax
+    646c5c94:	je     646c5d4a <_gnu_exception_handler+0xea>
+    646c5c9a:	ja     646c5d94 <_gnu_exception_handler+0x134>
+    646c5ca0:	cmp    $0x80000002,%eax
+    646c5ca5:	je     646c5d4a <_gnu_exception_handler+0xea>
+    646c5cab:	cmp    $0xc0000005,%eax
+    646c5cb0:	jne    646c5cd1 <_gnu_exception_handler+0x71>
+    646c5cb2:	xor    %edx,%edx
+    646c5cb4:	mov    $0xb,%ecx
+    646c5cb9:	call   646c7668 <signal>
+    646c5cbe:	cmp    $0x1,%rax
+    646c5cc2:	je     646c5e19 <_gnu_exception_handler+0x1b9>
+    646c5cc8:	test   %rax,%rax
+    646c5ccb:	jne    646c5de0 <_gnu_exception_handler+0x180>
+    646c5cd1:	mov    0x6b88(%rip),%rax        # 646cc860 <__mingw_oldexcpt_handler>
+    646c5cd8:	test   %rax,%rax
+    646c5cdb:	je     646c5df1 <_gnu_exception_handler+0x191>
+    646c5ce1:	mov    %rbx,%rcx
+    646c5ce4:	add    $0x20,%rsp
+    646c5ce8:	pop    %rbx
+    646c5ce9:	rex.W jmp *%rax
+    646c5cec:	nopl   0x0(%rax)
+    646c5cf0:	cmp    $0xc0000094,%eax
+    646c5cf5:	je     646c5db0 <_gnu_exception_handler+0x150>
+    646c5cfb:	ja     646c5d55 <_gnu_exception_handler+0xf5>
+    646c5cfd:	cmp    $0xc0000092,%eax
+    646c5d02:	je     646c5d4a <_gnu_exception_handler+0xea>
+    646c5d04:	cmp    $0xc0000093,%eax
+    646c5d09:	jne    646c5cd1 <_gnu_exception_handler+0x71>
+    646c5d0b:	xor    %edx,%edx
+    646c5d0d:	mov    $0x8,%ecx
+    646c5d12:	call   646c7668 <signal>
+    646c5d17:	cmp    $0x1,%rax
+    646c5d1b:	je     646c5e00 <_gnu_exception_handler+0x1a0>
+    646c5d21:	test   %rax,%rax
+    646c5d24:	je     646c5cd1 <_gnu_exception_handler+0x71>
+    646c5d26:	mov    $0x8,%ecx
+    646c5d2b:	call   *%rax
+    646c5d2d:	mov    $0xffffffff,%eax
+    646c5d32:	add    $0x20,%rsp
+    646c5d36:	pop    %rbx
+    646c5d37:	ret
+    646c5d38:	nopl   0x0(%rax,%rax,1)
+    646c5d40:	testb  $0x1,0x4(%rdx)
+    646c5d44:	jne    646c5c81 <_gnu_exception_handler+0x21>
+    646c5d4a:	mov    $0xffffffff,%eax
+    646c5d4f:	add    $0x20,%rsp
+    646c5d53:	pop    %rbx
+    646c5d54:	ret
+    646c5d55:	cmp    $0xc0000095,%eax
+    646c5d5a:	je     646c5d4a <_gnu_exception_handler+0xea>
+    646c5d5c:	cmp    $0xc0000096,%eax
+    646c5d61:	jne    646c5cd1 <_gnu_exception_handler+0x71>
+    646c5d67:	xor    %edx,%edx
+    646c5d69:	mov    $0x4,%ecx
+    646c5d6e:	call   646c7668 <signal>
+    646c5d73:	cmp    $0x1,%rax
+    646c5d77:	je     646c5e30 <_gnu_exception_handler+0x1d0>
+    646c5d7d:	test   %rax,%rax
+    646c5d80:	je     646c5cd1 <_gnu_exception_handler+0x71>
+    646c5d86:	mov    $0x4,%ecx
+    646c5d8b:	call   *%rax
+    646c5d8d:	mov    $0xffffffff,%eax
+    646c5d92:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
+    646c5d94:	cmp    $0xc000001d,%eax
+    646c5d99:	je     646c5d67 <_gnu_exception_handler+0x107>
+    646c5d9b:	cmp    $0xc000008c,%eax
+    646c5da0:	jne    646c5cd1 <_gnu_exception_handler+0x71>
+    646c5da6:	jmp    646c5d4a <_gnu_exception_handler+0xea>
+    646c5da8:	nopl   0x0(%rax,%rax,1)
+    646c5db0:	xor    %edx,%edx
+    646c5db2:	mov    $0x8,%ecx
+    646c5db7:	call   646c7668 <signal>
+    646c5dbc:	cmp    $0x1,%rax
+    646c5dc0:	jne    646c5d21 <_gnu_exception_handler+0xc1>
+    646c5dc6:	mov    $0x1,%edx
+    646c5dcb:	mov    $0x8,%ecx
+    646c5dd0:	call   646c7668 <signal>
+    646c5dd5:	mov    $0xffffffff,%eax
+    646c5dda:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
+    646c5ddf:	nop
+    646c5de0:	mov    $0xb,%ecx
+    646c5de5:	call   *%rax
+    646c5de7:	mov    $0xffffffff,%eax
+    646c5dec:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
+    646c5df1:	xor    %eax,%eax
+    646c5df3:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
+    646c5df8:	nopl   0x0(%rax,%rax,1)
+    646c5e00:	mov    $0x1,%edx
+    646c5e05:	mov    $0x8,%ecx
+    646c5e0a:	call   646c7668 <signal>
+    646c5e0f:	call   646c64a0 <_fpreset>
+    646c5e14:	jmp    646c5d4a <_gnu_exception_handler+0xea>
+    646c5e19:	mov    $0x1,%edx
+    646c5e1e:	mov    $0xb,%ecx
+    646c5e23:	call   646c7668 <signal>
+    646c5e28:	or     $0xffffffff,%eax
+    646c5e2b:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
+    646c5e30:	mov    $0x1,%edx
+    646c5e35:	mov    $0x4,%ecx
+    646c5e3a:	call   646c7668 <signal>
+    646c5e3f:	or     $0xffffffff,%eax
+    646c5e42:	jmp    646c5d32 <_gnu_exception_handler+0xd2>
+    646c5e47:	nop
+    646c5e48:	nop
+    646c5e49:	nop
+    646c5e4a:	nop
+    646c5e4b:	nop
+    646c5e4c:	nop
+    646c5e4d:	nop
+    646c5e4e:	nop
+    646c5e4f:	nop
+
+00000000646c5e50 <__mingwthr_run_key_dtors.part.0>:
+    646c5e50:	push   %rbp
+    646c5e51:	push   %rdi
+    646c5e52:	push   %rsi
+    646c5e53:	push   %rbx
+    646c5e54:	sub    $0x28,%rsp
+    646c5e58:	lea    0x6cc1(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5e5f:	call   *0x836f(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c5e65:	mov    0x6c94(%rip),%rbx        # 646ccb00 <key_dtor_list>
+    646c5e6c:	test   %rbx,%rbx
+    646c5e6f:	je     646c5ea4 <__mingwthr_run_key_dtors.part.0+0x54>
+    646c5e71:	mov    0x83e4(%rip),%rbp        # 646ce25c <__imp_TlsGetValue>
+    646c5e78:	mov    0x8375(%rip),%rdi        # 646ce1f4 <__imp_GetLastError>
+    646c5e7f:	nop
+    646c5e80:	mov    (%rbx),%ecx
+    646c5e82:	call   *%rbp
+    646c5e84:	mov    %rax,%rsi
+    646c5e87:	call   *%rdi
+    646c5e89:	test   %eax,%eax
+    646c5e8b:	jne    646c5e9b <__mingwthr_run_key_dtors.part.0+0x4b>
+    646c5e8d:	test   %rsi,%rsi
+    646c5e90:	je     646c5e9b <__mingwthr_run_key_dtors.part.0+0x4b>
+    646c5e92:	mov    0x8(%rbx),%rax
+    646c5e96:	mov    %rsi,%rcx
+    646c5e99:	call   *%rax
+    646c5e9b:	mov    0x10(%rbx),%rbx
+    646c5e9f:	test   %rbx,%rbx
+    646c5ea2:	jne    646c5e80 <__mingwthr_run_key_dtors.part.0+0x30>
+    646c5ea4:	lea    0x6c75(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5eab:	add    $0x28,%rsp
+    646c5eaf:	pop    %rbx
+    646c5eb0:	pop    %rsi
+    646c5eb1:	pop    %rdi
+    646c5eb2:	pop    %rbp
+    646c5eb3:	rex.W jmp *0x835a(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c5eba:	nopw   0x0(%rax,%rax,1)
+
+00000000646c5ec0 <___w64_mingwthr_add_key_dtor>:
+    646c5ec0:	push   %rbp
+    646c5ec1:	push   %rdi
+    646c5ec2:	push   %rsi
+    646c5ec3:	push   %rbx
+    646c5ec4:	sub    $0x28,%rsp
+    646c5ec8:	mov    0x6c3a(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c5ece:	xor    %esi,%esi
+    646c5ed0:	test   %eax,%eax
+    646c5ed2:	mov    %ecx,%ebp
+    646c5ed4:	mov    %rdx,%rdi
+    646c5ed7:	jne    646c5ee4 <___w64_mingwthr_add_key_dtor+0x24>
+    646c5ed9:	mov    %esi,%eax
+    646c5edb:	add    $0x28,%rsp
+    646c5edf:	pop    %rbx
+    646c5ee0:	pop    %rsi
+    646c5ee1:	pop    %rdi
+    646c5ee2:	pop    %rbp
+    646c5ee3:	ret
+    646c5ee4:	mov    $0x18,%edx
+    646c5ee9:	mov    $0x1,%ecx
+    646c5eee:	call   646c76c0 <calloc>
+    646c5ef3:	test   %rax,%rax
+    646c5ef6:	mov    %rax,%rbx
+    646c5ef9:	je     646c5f38 <___w64_mingwthr_add_key_dtor+0x78>
+    646c5efb:	mov    %ebp,(%rax)
+    646c5efd:	lea    0x6c1c(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5f04:	mov    %rdi,0x8(%rax)
+    646c5f08:	call   *0x82c6(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c5f0e:	mov    0x6beb(%rip),%rax        # 646ccb00 <key_dtor_list>
+    646c5f15:	lea    0x6c04(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5f1c:	mov    %rbx,0x6bdd(%rip)        # 646ccb00 <key_dtor_list>
+    646c5f23:	mov    %rax,0x10(%rbx)
+    646c5f27:	call   *0x82e7(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c5f2d:	mov    %esi,%eax
+    646c5f2f:	add    $0x28,%rsp
+    646c5f33:	pop    %rbx
+    646c5f34:	pop    %rsi
+    646c5f35:	pop    %rdi
+    646c5f36:	pop    %rbp
+    646c5f37:	ret
+    646c5f38:	mov    $0xffffffff,%esi
+    646c5f3d:	jmp    646c5ed9 <___w64_mingwthr_add_key_dtor+0x19>
+    646c5f3f:	nop
+
+00000000646c5f40 <___w64_mingwthr_remove_key_dtor>:
+    646c5f40:	push   %rbx
+    646c5f41:	sub    $0x20,%rsp
+    646c5f45:	mov    0x6bbd(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c5f4b:	test   %eax,%eax
+    646c5f4d:	mov    %ecx,%ebx
+    646c5f4f:	jne    646c5f60 <___w64_mingwthr_remove_key_dtor+0x20>
+    646c5f51:	xor    %eax,%eax
+    646c5f53:	add    $0x20,%rsp
+    646c5f57:	pop    %rbx
+    646c5f58:	ret
+    646c5f59:	nopl   0x0(%rax)
+    646c5f60:	lea    0x6bb9(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5f67:	call   *0x8267(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
+    646c5f6d:	mov    0x6b8c(%rip),%rax        # 646ccb00 <key_dtor_list>
+    646c5f74:	test   %rax,%rax
+    646c5f77:	je     646c5f93 <___w64_mingwthr_remove_key_dtor+0x53>
+    646c5f79:	mov    (%rax),%edx
+    646c5f7b:	cmp    %edx,%ebx
+    646c5f7d:	jne    646c5f8a <___w64_mingwthr_remove_key_dtor+0x4a>
+    646c5f7f:	jmp    646c5fd0 <___w64_mingwthr_remove_key_dtor+0x90>
+    646c5f81:	mov    (%rcx),%edx
+    646c5f83:	cmp    %ebx,%edx
+    646c5f85:	je     646c5fb0 <___w64_mingwthr_remove_key_dtor+0x70>
+    646c5f87:	mov    %rcx,%rax
+    646c5f8a:	mov    0x10(%rax),%rcx
+    646c5f8e:	test   %rcx,%rcx
+    646c5f91:	jne    646c5f81 <___w64_mingwthr_remove_key_dtor+0x41>
+    646c5f93:	lea    0x6b86(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5f9a:	call   *0x8274(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c5fa0:	xor    %eax,%eax
+    646c5fa2:	add    $0x20,%rsp
+    646c5fa6:	pop    %rbx
+    646c5fa7:	ret
+    646c5fa8:	nopl   0x0(%rax,%rax,1)
+    646c5fb0:	mov    0x10(%rcx),%rdx
+    646c5fb4:	mov    %rdx,0x10(%rax)
+    646c5fb8:	call   646c7698 <free>
+    646c5fbd:	lea    0x6b5c(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c5fc4:	call   *0x824a(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c5fca:	jmp    646c5fa0 <___w64_mingwthr_remove_key_dtor+0x60>
+    646c5fcc:	nopl   0x0(%rax)
+    646c5fd0:	mov    0x10(%rax),%rdx
+    646c5fd4:	mov    %rax,%rcx
+    646c5fd7:	mov    %rdx,0x6b22(%rip)        # 646ccb00 <key_dtor_list>
+    646c5fde:	jmp    646c5fb8 <___w64_mingwthr_remove_key_dtor+0x78>
+
+00000000646c5fe0 <__mingw_TLScallback>:
+    646c5fe0:	push   %rbx
+    646c5fe1:	sub    $0x20,%rsp
+    646c5fe5:	cmp    $0x1,%edx
+    646c5fe8:	je     646c6080 <__mingw_TLScallback+0xa0>
+    646c5fee:	jb     646c6020 <__mingw_TLScallback+0x40>
+    646c5ff0:	cmp    $0x2,%edx
+    646c5ff3:	je     646c6010 <__mingw_TLScallback+0x30>
+    646c5ff5:	cmp    $0x3,%edx
+    646c5ff8:	jne    646c6015 <__mingw_TLScallback+0x35>
+    646c5ffa:	mov    0x6b08(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c6000:	test   %eax,%eax
+    646c6002:	je     646c6015 <__mingw_TLScallback+0x35>
+    646c6004:	call   646c5e50 <__mingwthr_run_key_dtors.part.0>
+    646c6009:	jmp    646c6015 <__mingw_TLScallback+0x35>
+    646c600b:	nopl   0x0(%rax,%rax,1)
+    646c6010:	call   646c64a0 <_fpreset>
+    646c6015:	mov    $0x1,%eax
+    646c601a:	add    $0x20,%rsp
+    646c601e:	pop    %rbx
+    646c601f:	ret
+    646c6020:	mov    0x6ae2(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c6026:	test   %eax,%eax
+    646c6028:	jne    646c60b0 <__mingw_TLScallback+0xd0>
+    646c602e:	mov    0x6ad4(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c6034:	cmp    $0x1,%eax
+    646c6037:	jne    646c6015 <__mingw_TLScallback+0x35>
+    646c6039:	mov    0x6ac0(%rip),%rcx        # 646ccb00 <key_dtor_list>
+    646c6040:	test   %rcx,%rcx
+    646c6043:	je     646c6056 <__mingw_TLScallback+0x76>
+    646c6045:	mov    0x10(%rcx),%rbx
+    646c6049:	call   646c7698 <free>
+    646c604e:	test   %rbx,%rbx
+    646c6051:	mov    %rbx,%rcx
+    646c6054:	jne    646c6045 <__mingw_TLScallback+0x65>
+    646c6056:	lea    0x6ac3(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c605d:	movq   $0x0,0x6a98(%rip)        # 646ccb00 <key_dtor_list>
+    646c6068:	movl   $0x0,0x6a96(%rip)        # 646ccb08 <__mingwthr_cs_init>
+    646c6072:	call   *0x8154(%rip)        # 646ce1cc <__IAT_start__>
+    646c6078:	jmp    646c6015 <__mingw_TLScallback+0x35>
+    646c607a:	nopw   0x0(%rax,%rax,1)
+    646c6080:	mov    0x6a82(%rip),%eax        # 646ccb08 <__mingwthr_cs_init>
+    646c6086:	test   %eax,%eax
+    646c6088:	je     646c60a0 <__mingw_TLScallback+0xc0>
+    646c608a:	movl   $0x1,0x6a74(%rip)        # 646ccb08 <__mingwthr_cs_init>
+    646c6094:	mov    $0x1,%eax
+    646c6099:	add    $0x20,%rsp
+    646c609d:	pop    %rbx
+    646c609e:	ret
+    646c609f:	nop
+    646c60a0:	lea    0x6a79(%rip),%rcx        # 646ccb20 <__mingwthr_cs>
+    646c60a7:	call   *0x815f(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
+    646c60ad:	jmp    646c608a <__mingw_TLScallback+0xaa>
+    646c60af:	nop
+    646c60b0:	call   646c5e50 <__mingwthr_run_key_dtors.part.0>
+    646c60b5:	jmp    646c602e <__mingw_TLScallback+0x4e>
+    646c60ba:	nop
+    646c60bb:	nop
+    646c60bc:	nop
+    646c60bd:	nop
+    646c60be:	nop
+    646c60bf:	nop
+
+00000000646c60c0 <_ValidateImageBase.part.0>:
+    646c60c0:	movslq 0x3c(%rcx),%rax
+    646c60c4:	add    %rax,%rcx
+    646c60c7:	xor    %eax,%eax
+    646c60c9:	cmpl   $0x4550,(%rcx)
+    646c60cf:	je     646c60d2 <_ValidateImageBase.part.0+0x12>
+    646c60d1:	ret
+    646c60d2:	xor    %eax,%eax
+    646c60d4:	cmpw   $0x20b,0x18(%rcx)
+    646c60da:	sete   %al
+    646c60dd:	ret
+    646c60de:	xchg   %ax,%ax
+
+00000000646c60e0 <_ValidateImageBase>:
+    646c60e0:	cmpw   $0x5a4d,(%rcx)
+    646c60e5:	je     646c60f0 <_ValidateImageBase+0x10>
+    646c60e7:	xor    %eax,%eax
+    646c60e9:	ret
+    646c60ea:	nopw   0x0(%rax,%rax,1)
+    646c60f0:	jmp    646c60c0 <_ValidateImageBase.part.0>
+    646c60f2:	nopl   0x0(%rax)
+    646c60f6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6100 <_FindPESection>:
+    646c6100:	movslq 0x3c(%rcx),%rax
+    646c6104:	add    %rax,%rcx
+    646c6107:	movzwl 0x14(%rcx),%eax
+    646c610b:	lea    0x18(%rcx,%rax,1),%rax
+    646c6110:	movzwl 0x6(%rcx),%ecx
+    646c6114:	test   %ecx,%ecx
+    646c6116:	je     646c6141 <_FindPESection+0x41>
+    646c6118:	sub    $0x1,%ecx
+    646c611b:	lea    (%rcx,%rcx,4),%rcx
+    646c611f:	lea    0x28(%rax,%rcx,8),%r9
+    646c6124:	mov    0xc(%rax),%r8d
+    646c6128:	cmp    %rdx,%r8
+    646c612b:	mov    %r8,%rcx
+    646c612e:	ja     646c6138 <_FindPESection+0x38>
+    646c6130:	add    0x8(%rax),%ecx
+    646c6133:	cmp    %rdx,%rcx
+    646c6136:	ja     646c6143 <_FindPESection+0x43>
+    646c6138:	add    $0x28,%rax
+    646c613c:	cmp    %r9,%rax
+    646c613f:	jne    646c6124 <_FindPESection+0x24>
+    646c6141:	xor    %eax,%eax
+    646c6143:	ret
+    646c6144:	xchg   %ax,%ax
+    646c6146:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6150 <_FindPESectionByName>:
+    646c6150:	push   %rdi
+    646c6151:	push   %rsi
+    646c6152:	push   %rbx
+    646c6153:	sub    $0x20,%rsp
+    646c6157:	mov    %rcx,%rsi
+    646c615a:	call   646c7660 <strlen>
+    646c615f:	cmp    $0x8,%rax
+    646c6163:	ja     646c61d0 <_FindPESectionByName+0x80>
+    646c6165:	mov    0x34a4(%rip),%rdx        # 646c9610 <.refptr.__image_base__>
+    646c616c:	cmpw   $0x5a4d,(%rdx)
+    646c6171:	jne    646c61d0 <_FindPESectionByName+0x80>
+    646c6173:	mov    %rdx,%rcx
+    646c6176:	call   646c60c0 <_ValidateImageBase.part.0>
+    646c617b:	test   %eax,%eax
+    646c617d:	je     646c61d0 <_FindPESectionByName+0x80>
+    646c617f:	movslq 0x3c(%rdx),%rcx
+    646c6183:	add    %rdx,%rcx
+    646c6186:	movzwl 0x14(%rcx),%eax
+    646c618a:	lea    0x18(%rcx,%rax,1),%rbx
+    646c618f:	movzwl 0x6(%rcx),%eax
+    646c6193:	test   %eax,%eax
+    646c6195:	je     646c61d0 <_FindPESectionByName+0x80>
+    646c6197:	sub    $0x1,%eax
+    646c619a:	lea    (%rax,%rax,4),%rax
+    646c619e:	lea    0x28(%rbx,%rax,8),%rdi
+    646c61a3:	jmp    646c61ae <_FindPESectionByName+0x5e>
+    646c61a5:	add    $0x28,%rbx
+    646c61a9:	cmp    %rdi,%rbx
+    646c61ac:	je     646c61d0 <_FindPESectionByName+0x80>
+    646c61ae:	mov    $0x8,%r8d
+    646c61b4:	mov    %rsi,%rdx
+    646c61b7:	mov    %rbx,%rcx
+    646c61ba:	call   646c7658 <strncmp>
+    646c61bf:	test   %eax,%eax
+    646c61c1:	jne    646c61a5 <_FindPESectionByName+0x55>
+    646c61c3:	mov    %rbx,%rax
+    646c61c6:	add    $0x20,%rsp
+    646c61ca:	pop    %rbx
+    646c61cb:	pop    %rsi
+    646c61cc:	pop    %rdi
+    646c61cd:	ret
+    646c61ce:	xchg   %ax,%ax
+    646c61d0:	xor    %ebx,%ebx
+    646c61d2:	mov    %rbx,%rax
+    646c61d5:	add    $0x20,%rsp
+    646c61d9:	pop    %rbx
+    646c61da:	pop    %rsi
+    646c61db:	pop    %rdi
+    646c61dc:	ret
+    646c61dd:	nopl   (%rax)
+
+00000000646c61e0 <__mingw_GetSectionForAddress>:
+    646c61e0:	sub    $0x28,%rsp
+    646c61e4:	mov    0x3425(%rip),%r8        # 646c9610 <.refptr.__image_base__>
+    646c61eb:	cmpw   $0x5a4d,(%r8)
+    646c61f1:	mov    %rcx,%rdx
+    646c61f4:	jne    646c624d <__mingw_GetSectionForAddress+0x6d>
+    646c61f6:	mov    %r8,%rcx
+    646c61f9:	call   646c60c0 <_ValidateImageBase.part.0>
+    646c61fe:	test   %eax,%eax
+    646c6200:	je     646c624d <__mingw_GetSectionForAddress+0x6d>
+    646c6202:	movslq 0x3c(%r8),%rax
+    646c6206:	mov    %rdx,%rcx
+    646c6209:	sub    %r8,%rcx
+    646c620c:	add    %rax,%r8
+    646c620f:	movzwl 0x6(%r8),%edx
+    646c6214:	movzwl 0x14(%r8),%eax
+    646c6219:	test   %edx,%edx
+    646c621b:	lea    0x18(%r8,%rax,1),%rax
+    646c6220:	je     646c624d <__mingw_GetSectionForAddress+0x6d>
+    646c6222:	sub    $0x1,%edx
+    646c6225:	lea    (%rdx,%rdx,4),%rdx
+    646c6229:	lea    0x28(%rax,%rdx,8),%r9
+    646c622e:	xchg   %ax,%ax
+    646c6230:	mov    0xc(%rax),%r8d
+    646c6234:	cmp    %r8,%rcx
+    646c6237:	mov    %r8,%rdx
+    646c623a:	jb     646c6244 <__mingw_GetSectionForAddress+0x64>
+    646c623c:	add    0x8(%rax),%edx
+    646c623f:	cmp    %rdx,%rcx
+    646c6242:	jb     646c624f <__mingw_GetSectionForAddress+0x6f>
+    646c6244:	add    $0x28,%rax
+    646c6248:	cmp    %r9,%rax
+    646c624b:	jne    646c6230 <__mingw_GetSectionForAddress+0x50>
+    646c624d:	xor    %eax,%eax
+    646c624f:	add    $0x28,%rsp
+    646c6253:	ret
+    646c6254:	xchg   %ax,%ax
+    646c6256:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6260 <__mingw_GetSectionCount>:
+    646c6260:	sub    $0x28,%rsp
+    646c6264:	mov    0x33a5(%rip),%rdx        # 646c9610 <.refptr.__image_base__>
+    646c626b:	xor    %r8d,%r8d
+    646c626e:	cmpw   $0x5a4d,(%rdx)
+    646c6273:	je     646c6280 <__mingw_GetSectionCount+0x20>
+    646c6275:	mov    %r8d,%eax
+    646c6278:	add    $0x28,%rsp
+    646c627c:	ret
+    646c627d:	nopl   (%rax)
+    646c6280:	mov    %rdx,%rcx
+    646c6283:	call   646c60c0 <_ValidateImageBase.part.0>
+    646c6288:	test   %eax,%eax
+    646c628a:	je     646c6275 <__mingw_GetSectionCount+0x15>
+    646c628c:	movslq 0x3c(%rdx),%rax
+    646c6290:	movzwl 0x6(%rax,%rdx,1),%r8d
+    646c6296:	mov    %r8d,%eax
+    646c6299:	add    $0x28,%rsp
+    646c629d:	ret
+    646c629e:	xchg   %ax,%ax
+
+00000000646c62a0 <_FindPESectionExec>:
+    646c62a0:	sub    $0x28,%rsp
+    646c62a4:	mov    0x3365(%rip),%r8        # 646c9610 <.refptr.__image_base__>
+    646c62ab:	cmpw   $0x5a4d,(%r8)
+    646c62b1:	mov    %rcx,%rdx
+    646c62b4:	jne    646c6308 <_FindPESectionExec+0x68>
+    646c62b6:	mov    %r8,%rcx
+    646c62b9:	call   646c60c0 <_ValidateImageBase.part.0>
+    646c62be:	test   %eax,%eax
+    646c62c0:	je     646c6308 <_FindPESectionExec+0x68>
+    646c62c2:	movslq 0x3c(%r8),%rcx
+    646c62c6:	add    %r8,%rcx
+    646c62c9:	movzwl 0x14(%rcx),%eax
+    646c62cd:	lea    0x18(%rcx,%rax,1),%rax
+    646c62d2:	movzwl 0x6(%rcx),%ecx
+    646c62d6:	test   %ecx,%ecx
+    646c62d8:	je     646c6308 <_FindPESectionExec+0x68>
+    646c62da:	sub    $0x1,%ecx
+    646c62dd:	lea    (%rcx,%rcx,4),%rcx
+    646c62e1:	lea    0x28(%rax,%rcx,8),%rcx
+    646c62e6:	cs nopw 0x0(%rax,%rax,1)
+    646c62f0:	testb  $0x20,0x27(%rax)
+    646c62f4:	je     646c62ff <_FindPESectionExec+0x5f>
+    646c62f6:	test   %rdx,%rdx
+    646c62f9:	je     646c630a <_FindPESectionExec+0x6a>
+    646c62fb:	sub    $0x1,%rdx
+    646c62ff:	add    $0x28,%rax
+    646c6303:	cmp    %rcx,%rax
+    646c6306:	jne    646c62f0 <_FindPESectionExec+0x50>
+    646c6308:	xor    %eax,%eax
+    646c630a:	add    $0x28,%rsp
+    646c630e:	ret
+    646c630f:	nop
+
+00000000646c6310 <_GetPEImageBase>:
+    646c6310:	sub    $0x28,%rsp
+    646c6314:	mov    0x32f5(%rip),%rdx        # 646c9610 <.refptr.__image_base__>
+    646c631b:	cmpw   $0x5a4d,(%rdx)
+    646c6320:	jne    646c6340 <_GetPEImageBase+0x30>
+    646c6322:	mov    %rdx,%rcx
+    646c6325:	call   646c60c0 <_ValidateImageBase.part.0>
+    646c632a:	test   %eax,%eax
+    646c632c:	mov    $0x0,%eax
+    646c6331:	cmovne %rdx,%rax
+    646c6335:	add    $0x28,%rsp
+    646c6339:	ret
+    646c633a:	nopw   0x0(%rax,%rax,1)
+    646c6340:	xor    %eax,%eax
+    646c6342:	add    $0x28,%rsp
+    646c6346:	ret
+    646c6347:	nopw   0x0(%rax,%rax,1)
+
+00000000646c6350 <_IsNonwritableInCurrentImage>:
+    646c6350:	sub    $0x28,%rsp
+    646c6354:	mov    0x32b5(%rip),%r8        # 646c9610 <.refptr.__image_base__>
+    646c635b:	xor    %eax,%eax
+    646c635d:	cmpw   $0x5a4d,(%r8)
+    646c6363:	mov    %rcx,%rdx
+    646c6366:	je     646c6370 <_IsNonwritableInCurrentImage+0x20>
+    646c6368:	add    $0x28,%rsp
+    646c636c:	ret
+    646c636d:	nopl   (%rax)
+    646c6370:	mov    %r8,%rcx
+    646c6373:	call   646c60c0 <_ValidateImageBase.part.0>
+    646c6378:	test   %eax,%eax
+    646c637a:	je     646c6368 <_IsNonwritableInCurrentImage+0x18>
+    646c637c:	movslq 0x3c(%r8),%rax
+    646c6380:	mov    %rdx,%rcx
+    646c6383:	sub    %r8,%rcx
+    646c6386:	add    %rax,%r8
+    646c6389:	movzwl 0x6(%r8),%edx
+    646c638e:	movzwl 0x14(%r8),%eax
+    646c6393:	test   %edx,%edx
+    646c6395:	lea    0x18(%r8,%rax,1),%rax
+    646c639a:	je     646c63cd <_IsNonwritableInCurrentImage+0x7d>
+    646c639c:	sub    $0x1,%edx
+    646c639f:	lea    (%rdx,%rdx,4),%rdx
+    646c63a3:	lea    0x28(%rax,%rdx,8),%r9
+    646c63a8:	nopl   0x0(%rax,%rax,1)
+    646c63b0:	mov    0xc(%rax),%r8d
+    646c63b4:	cmp    %r8,%rcx
+    646c63b7:	mov    %r8,%rdx
+    646c63ba:	jb     646c63c4 <_IsNonwritableInCurrentImage+0x74>
+    646c63bc:	add    0x8(%rax),%edx
+    646c63bf:	cmp    %rdx,%rcx
+    646c63c2:	jb     646c63d4 <_IsNonwritableInCurrentImage+0x84>
+    646c63c4:	add    $0x28,%rax
+    646c63c8:	cmp    %r9,%rax
+    646c63cb:	jne    646c63b0 <_IsNonwritableInCurrentImage+0x60>
+    646c63cd:	xor    %eax,%eax
+    646c63cf:	add    $0x28,%rsp
+    646c63d3:	ret
+    646c63d4:	mov    0x24(%rax),%eax
+    646c63d7:	not    %eax
+    646c63d9:	shr    $0x1f,%eax
+    646c63dc:	add    $0x28,%rsp
+    646c63e0:	ret
+    646c63e1:	nopl   0x0(%rax,%rax,1)
     646c63e6:	cs nopw 0x0(%rax,%rax,1)
 
-00000000646c63f0 <_FindPESection>:
-    646c63f0:	movslq 0x3c(%rcx),%rax
-    646c63f4:	add    %rax,%rcx
-    646c63f7:	movzwl 0x14(%rcx),%eax
-    646c63fb:	lea    0x18(%rcx,%rax,1),%rax
-    646c6400:	movzwl 0x6(%rcx),%ecx
-    646c6404:	test   %ecx,%ecx
-    646c6406:	je     646c6431 <_FindPESection+0x41>
-    646c6408:	sub    $0x1,%ecx
-    646c640b:	lea    (%rcx,%rcx,4),%rcx
-    646c640f:	lea    0x28(%rax,%rcx,8),%r9
-    646c6414:	mov    0xc(%rax),%r8d
-    646c6418:	cmp    %rdx,%r8
-    646c641b:	mov    %r8,%rcx
-    646c641e:	ja     646c6428 <_FindPESection+0x38>
-    646c6420:	add    0x8(%rax),%ecx
-    646c6423:	cmp    %rdx,%rcx
-    646c6426:	ja     646c6433 <_FindPESection+0x43>
-    646c6428:	add    $0x28,%rax
-    646c642c:	cmp    %r9,%rax
-    646c642f:	jne    646c6414 <_FindPESection+0x24>
-    646c6431:	xor    %eax,%eax
-    646c6433:	ret
-    646c6434:	xchg   %ax,%ax
-    646c6436:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6440 <_FindPESectionByName>:
-    646c6440:	push   %rdi
-    646c6441:	push   %rsi
-    646c6442:	push   %rbx
-    646c6443:	sub    $0x20,%rsp
-    646c6447:	mov    %rcx,%rsi
-    646c644a:	call   646c7950 <strlen>
-    646c644f:	cmp    $0x8,%rax
-    646c6453:	ja     646c64c0 <_FindPESectionByName+0x80>
-    646c6455:	mov    0x31d4(%rip),%rdx        # 646c9630 <.refptr.__image_base__>
-    646c645c:	cmpw   $0x5a4d,(%rdx)
-    646c6461:	jne    646c64c0 <_FindPESectionByName+0x80>
-    646c6463:	mov    %rdx,%rcx
-    646c6466:	call   646c63b0 <_ValidateImageBase.part.0>
-    646c646b:	test   %eax,%eax
-    646c646d:	je     646c64c0 <_FindPESectionByName+0x80>
-    646c646f:	movslq 0x3c(%rdx),%rcx
-    646c6473:	add    %rdx,%rcx
-    646c6476:	movzwl 0x14(%rcx),%eax
-    646c647a:	lea    0x18(%rcx,%rax,1),%rbx
-    646c647f:	movzwl 0x6(%rcx),%eax
-    646c6483:	test   %eax,%eax
-    646c6485:	je     646c64c0 <_FindPESectionByName+0x80>
-    646c6487:	sub    $0x1,%eax
-    646c648a:	lea    (%rax,%rax,4),%rax
-    646c648e:	lea    0x28(%rbx,%rax,8),%rdi
-    646c6493:	jmp    646c649e <_FindPESectionByName+0x5e>
-    646c6495:	add    $0x28,%rbx
-    646c6499:	cmp    %rdi,%rbx
-    646c649c:	je     646c64c0 <_FindPESectionByName+0x80>
-    646c649e:	mov    $0x8,%r8d
-    646c64a4:	mov    %rsi,%rdx
-    646c64a7:	mov    %rbx,%rcx
-    646c64aa:	call   646c7948 <strncmp>
-    646c64af:	test   %eax,%eax
-    646c64b1:	jne    646c6495 <_FindPESectionByName+0x55>
-    646c64b3:	mov    %rbx,%rax
-    646c64b6:	add    $0x20,%rsp
-    646c64ba:	pop    %rbx
-    646c64bb:	pop    %rsi
-    646c64bc:	pop    %rdi
-    646c64bd:	ret
-    646c64be:	xchg   %ax,%ax
-    646c64c0:	xor    %ebx,%ebx
-    646c64c2:	mov    %rbx,%rax
-    646c64c5:	add    $0x20,%rsp
-    646c64c9:	pop    %rbx
-    646c64ca:	pop    %rsi
-    646c64cb:	pop    %rdi
-    646c64cc:	ret
-    646c64cd:	nopl   (%rax)
-
-00000000646c64d0 <__mingw_GetSectionForAddress>:
-    646c64d0:	sub    $0x28,%rsp
-    646c64d4:	mov    0x3155(%rip),%r8        # 646c9630 <.refptr.__image_base__>
-    646c64db:	cmpw   $0x5a4d,(%r8)
-    646c64e1:	mov    %rcx,%rdx
-    646c64e4:	jne    646c653d <__mingw_GetSectionForAddress+0x6d>
-    646c64e6:	mov    %r8,%rcx
-    646c64e9:	call   646c63b0 <_ValidateImageBase.part.0>
-    646c64ee:	test   %eax,%eax
-    646c64f0:	je     646c653d <__mingw_GetSectionForAddress+0x6d>
-    646c64f2:	movslq 0x3c(%r8),%rax
-    646c64f6:	mov    %rdx,%rcx
-    646c64f9:	sub    %r8,%rcx
-    646c64fc:	add    %rax,%r8
-    646c64ff:	movzwl 0x6(%r8),%edx
-    646c6504:	movzwl 0x14(%r8),%eax
-    646c6509:	test   %edx,%edx
-    646c650b:	lea    0x18(%r8,%rax,1),%rax
-    646c6510:	je     646c653d <__mingw_GetSectionForAddress+0x6d>
-    646c6512:	sub    $0x1,%edx
-    646c6515:	lea    (%rdx,%rdx,4),%rdx
-    646c6519:	lea    0x28(%rax,%rdx,8),%r9
-    646c651e:	xchg   %ax,%ax
-    646c6520:	mov    0xc(%rax),%r8d
-    646c6524:	cmp    %r8,%rcx
-    646c6527:	mov    %r8,%rdx
-    646c652a:	jb     646c6534 <__mingw_GetSectionForAddress+0x64>
-    646c652c:	add    0x8(%rax),%edx
-    646c652f:	cmp    %rdx,%rcx
-    646c6532:	jb     646c653f <__mingw_GetSectionForAddress+0x6f>
-    646c6534:	add    $0x28,%rax
-    646c6538:	cmp    %r9,%rax
-    646c653b:	jne    646c6520 <__mingw_GetSectionForAddress+0x50>
-    646c653d:	xor    %eax,%eax
-    646c653f:	add    $0x28,%rsp
-    646c6543:	ret
-    646c6544:	xchg   %ax,%ax
-    646c6546:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6550 <__mingw_GetSectionCount>:
-    646c6550:	sub    $0x28,%rsp
-    646c6554:	mov    0x30d5(%rip),%rdx        # 646c9630 <.refptr.__image_base__>
-    646c655b:	xor    %r8d,%r8d
-    646c655e:	cmpw   $0x5a4d,(%rdx)
-    646c6563:	je     646c6570 <__mingw_GetSectionCount+0x20>
-    646c6565:	mov    %r8d,%eax
-    646c6568:	add    $0x28,%rsp
-    646c656c:	ret
-    646c656d:	nopl   (%rax)
-    646c6570:	mov    %rdx,%rcx
-    646c6573:	call   646c63b0 <_ValidateImageBase.part.0>
-    646c6578:	test   %eax,%eax
-    646c657a:	je     646c6565 <__mingw_GetSectionCount+0x15>
-    646c657c:	movslq 0x3c(%rdx),%rax
-    646c6580:	movzwl 0x6(%rax,%rdx,1),%r8d
-    646c6586:	mov    %r8d,%eax
-    646c6589:	add    $0x28,%rsp
-    646c658d:	ret
-    646c658e:	xchg   %ax,%ax
-
-00000000646c6590 <_FindPESectionExec>:
-    646c6590:	sub    $0x28,%rsp
-    646c6594:	mov    0x3095(%rip),%r8        # 646c9630 <.refptr.__image_base__>
-    646c659b:	cmpw   $0x5a4d,(%r8)
-    646c65a1:	mov    %rcx,%rdx
-    646c65a4:	jne    646c65f8 <_FindPESectionExec+0x68>
-    646c65a6:	mov    %r8,%rcx
-    646c65a9:	call   646c63b0 <_ValidateImageBase.part.0>
-    646c65ae:	test   %eax,%eax
-    646c65b0:	je     646c65f8 <_FindPESectionExec+0x68>
-    646c65b2:	movslq 0x3c(%r8),%rcx
-    646c65b6:	add    %r8,%rcx
-    646c65b9:	movzwl 0x14(%rcx),%eax
-    646c65bd:	lea    0x18(%rcx,%rax,1),%rax
-    646c65c2:	movzwl 0x6(%rcx),%ecx
-    646c65c6:	test   %ecx,%ecx
-    646c65c8:	je     646c65f8 <_FindPESectionExec+0x68>
-    646c65ca:	sub    $0x1,%ecx
-    646c65cd:	lea    (%rcx,%rcx,4),%rcx
-    646c65d1:	lea    0x28(%rax,%rcx,8),%rcx
-    646c65d6:	cs nopw 0x0(%rax,%rax,1)
-    646c65e0:	testb  $0x20,0x27(%rax)
-    646c65e4:	je     646c65ef <_FindPESectionExec+0x5f>
-    646c65e6:	test   %rdx,%rdx
-    646c65e9:	je     646c65fa <_FindPESectionExec+0x6a>
-    646c65eb:	sub    $0x1,%rdx
-    646c65ef:	add    $0x28,%rax
-    646c65f3:	cmp    %rcx,%rax
-    646c65f6:	jne    646c65e0 <_FindPESectionExec+0x50>
-    646c65f8:	xor    %eax,%eax
-    646c65fa:	add    $0x28,%rsp
-    646c65fe:	ret
-    646c65ff:	nop
-
-00000000646c6600 <_GetPEImageBase>:
-    646c6600:	sub    $0x28,%rsp
-    646c6604:	mov    0x3025(%rip),%rdx        # 646c9630 <.refptr.__image_base__>
-    646c660b:	cmpw   $0x5a4d,(%rdx)
-    646c6610:	jne    646c6630 <_GetPEImageBase+0x30>
-    646c6612:	mov    %rdx,%rcx
-    646c6615:	call   646c63b0 <_ValidateImageBase.part.0>
-    646c661a:	test   %eax,%eax
-    646c661c:	mov    $0x0,%eax
-    646c6621:	cmovne %rdx,%rax
-    646c6625:	add    $0x28,%rsp
-    646c6629:	ret
-    646c662a:	nopw   0x0(%rax,%rax,1)
-    646c6630:	xor    %eax,%eax
-    646c6632:	add    $0x28,%rsp
-    646c6636:	ret
-    646c6637:	nopw   0x0(%rax,%rax,1)
-
-00000000646c6640 <_IsNonwritableInCurrentImage>:
-    646c6640:	sub    $0x28,%rsp
-    646c6644:	mov    0x2fe5(%rip),%r8        # 646c9630 <.refptr.__image_base__>
-    646c664b:	xor    %eax,%eax
-    646c664d:	cmpw   $0x5a4d,(%r8)
-    646c6653:	mov    %rcx,%rdx
-    646c6656:	je     646c6660 <_IsNonwritableInCurrentImage+0x20>
-    646c6658:	add    $0x28,%rsp
-    646c665c:	ret
-    646c665d:	nopl   (%rax)
-    646c6660:	mov    %r8,%rcx
-    646c6663:	call   646c63b0 <_ValidateImageBase.part.0>
-    646c6668:	test   %eax,%eax
-    646c666a:	je     646c6658 <_IsNonwritableInCurrentImage+0x18>
-    646c666c:	movslq 0x3c(%r8),%rax
-    646c6670:	mov    %rdx,%rcx
-    646c6673:	sub    %r8,%rcx
-    646c6676:	add    %rax,%r8
-    646c6679:	movzwl 0x6(%r8),%edx
-    646c667e:	movzwl 0x14(%r8),%eax
-    646c6683:	test   %edx,%edx
-    646c6685:	lea    0x18(%r8,%rax,1),%rax
-    646c668a:	je     646c66bd <_IsNonwritableInCurrentImage+0x7d>
-    646c668c:	sub    $0x1,%edx
-    646c668f:	lea    (%rdx,%rdx,4),%rdx
-    646c6693:	lea    0x28(%rax,%rdx,8),%r9
-    646c6698:	nopl   0x0(%rax,%rax,1)
-    646c66a0:	mov    0xc(%rax),%r8d
-    646c66a4:	cmp    %r8,%rcx
-    646c66a7:	mov    %r8,%rdx
-    646c66aa:	jb     646c66b4 <_IsNonwritableInCurrentImage+0x74>
-    646c66ac:	add    0x8(%rax),%edx
-    646c66af:	cmp    %rdx,%rcx
-    646c66b2:	jb     646c66c4 <_IsNonwritableInCurrentImage+0x84>
-    646c66b4:	add    $0x28,%rax
-    646c66b8:	cmp    %r9,%rax
-    646c66bb:	jne    646c66a0 <_IsNonwritableInCurrentImage+0x60>
-    646c66bd:	xor    %eax,%eax
-    646c66bf:	add    $0x28,%rsp
-    646c66c3:	ret
-    646c66c4:	mov    0x24(%rax),%eax
-    646c66c7:	not    %eax
-    646c66c9:	shr    $0x1f,%eax
-    646c66cc:	add    $0x28,%rsp
-    646c66d0:	ret
-    646c66d1:	nopl   0x0(%rax,%rax,1)
-    646c66d6:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c66e0 <__mingw_enum_import_library_names>:
-    646c66e0:	sub    $0x28,%rsp
-    646c66e4:	mov    0x2f45(%rip),%r11        # 646c9630 <.refptr.__image_base__>
-    646c66eb:	cmpw   $0x5a4d,(%r11)
-    646c66f1:	mov    %ecx,%r9d
-    646c66f4:	jne    646c674e <__mingw_enum_import_library_names+0x6e>
-    646c66f6:	mov    %r11,%rcx
-    646c66f9:	call   646c63b0 <_ValidateImageBase.part.0>
-    646c66fe:	test   %eax,%eax
-    646c6700:	je     646c674e <__mingw_enum_import_library_names+0x6e>
-    646c6702:	movslq 0x3c(%r11),%rax
-    646c6706:	add    %r11,%rax
-    646c6709:	mov    0x90(%rax),%edx
-    646c670f:	test   %edx,%edx
-    646c6711:	je     646c674e <__mingw_enum_import_library_names+0x6e>
-    646c6713:	movzwl 0x14(%rax),%ecx
-    646c6717:	lea    0x18(%rax,%rcx,1),%rcx
-    646c671c:	movzwl 0x6(%rax),%eax
-    646c6720:	test   %eax,%eax
-    646c6722:	je     646c674e <__mingw_enum_import_library_names+0x6e>
-    646c6724:	sub    $0x1,%eax
-    646c6727:	lea    (%rax,%rax,4),%rax
-    646c672b:	lea    0x28(%rcx,%rax,8),%rax
-    646c6730:	mov    0xc(%rcx),%r10d
-    646c6734:	cmp    %r10,%rdx
-    646c6737:	mov    %r10,%r8
-    646c673a:	jb     646c6745 <__mingw_enum_import_library_names+0x65>
-    646c673c:	add    0x8(%rcx),%r8d
-    646c6740:	cmp    %r8,%rdx
-    646c6743:	jb     646c6755 <__mingw_enum_import_library_names+0x75>
-    646c6745:	add    $0x28,%rcx
-    646c6749:	cmp    %rax,%rcx
-    646c674c:	jne    646c6730 <__mingw_enum_import_library_names+0x50>
-    646c674e:	xor    %eax,%eax
-    646c6750:	add    $0x28,%rsp
-    646c6754:	ret
-    646c6755:	add    %r11,%rdx
-    646c6758:	jne    646c6768 <__mingw_enum_import_library_names+0x88>
-    646c675a:	jmp    646c674e <__mingw_enum_import_library_names+0x6e>
-    646c675c:	nopl   0x0(%rax)
-    646c6760:	sub    $0x1,%r9d
-    646c6764:	add    $0x14,%rdx
-    646c6768:	mov    0x4(%rdx),%ecx
-    646c676b:	test   %ecx,%ecx
-    646c676d:	jne    646c6776 <__mingw_enum_import_library_names+0x96>
-    646c676f:	mov    0xc(%rdx),%eax
-    646c6772:	test   %eax,%eax
-    646c6774:	je     646c674e <__mingw_enum_import_library_names+0x6e>
-    646c6776:	test   %r9d,%r9d
-    646c6779:	jg     646c6760 <__mingw_enum_import_library_names+0x80>
-    646c677b:	mov    0xc(%rdx),%eax
-    646c677e:	add    %r11,%rax
-    646c6781:	add    $0x28,%rsp
-    646c6785:	ret
-    646c6786:	nop
-    646c6787:	nop
-    646c6788:	nop
-    646c6789:	nop
-    646c678a:	nop
-    646c678b:	nop
-    646c678c:	nop
-    646c678d:	nop
-    646c678e:	nop
-    646c678f:	nop
-
-00000000646c6790 <_fpreset>:
-    646c6790:	fninit
-    646c6792:	ret
-    646c6793:	nop
-    646c6794:	nop
-    646c6795:	nop
-    646c6796:	nop
-    646c6797:	nop
-    646c6798:	nop
-    646c6799:	nop
-    646c679a:	nop
-    646c679b:	nop
-    646c679c:	nop
-    646c679d:	nop
-    646c679e:	nop
-    646c679f:	nop
+00000000646c63f0 <__mingw_enum_import_library_names>:
+    646c63f0:	sub    $0x28,%rsp
+    646c63f4:	mov    0x3215(%rip),%r11        # 646c9610 <.refptr.__image_base__>
+    646c63fb:	cmpw   $0x5a4d,(%r11)
+    646c6401:	mov    %ecx,%r9d
+    646c6404:	jne    646c645e <__mingw_enum_import_library_names+0x6e>
+    646c6406:	mov    %r11,%rcx
+    646c6409:	call   646c60c0 <_ValidateImageBase.part.0>
+    646c640e:	test   %eax,%eax
+    646c6410:	je     646c645e <__mingw_enum_import_library_names+0x6e>
+    646c6412:	movslq 0x3c(%r11),%rax
+    646c6416:	add    %r11,%rax
+    646c6419:	mov    0x90(%rax),%edx
+    646c641f:	test   %edx,%edx
+    646c6421:	je     646c645e <__mingw_enum_import_library_names+0x6e>
+    646c6423:	movzwl 0x14(%rax),%ecx
+    646c6427:	lea    0x18(%rax,%rcx,1),%rcx
+    646c642c:	movzwl 0x6(%rax),%eax
+    646c6430:	test   %eax,%eax
+    646c6432:	je     646c645e <__mingw_enum_import_library_names+0x6e>
+    646c6434:	sub    $0x1,%eax
+    646c6437:	lea    (%rax,%rax,4),%rax
+    646c643b:	lea    0x28(%rcx,%rax,8),%rax
+    646c6440:	mov    0xc(%rcx),%r10d
+    646c6444:	cmp    %r10,%rdx
+    646c6447:	mov    %r10,%r8
+    646c644a:	jb     646c6455 <__mingw_enum_import_library_names+0x65>
+    646c644c:	add    0x8(%rcx),%r8d
+    646c6450:	cmp    %r8,%rdx
+    646c6453:	jb     646c6465 <__mingw_enum_import_library_names+0x75>
+    646c6455:	add    $0x28,%rcx
+    646c6459:	cmp    %rax,%rcx
+    646c645c:	jne    646c6440 <__mingw_enum_import_library_names+0x50>
+    646c645e:	xor    %eax,%eax
+    646c6460:	add    $0x28,%rsp
+    646c6464:	ret
+    646c6465:	add    %r11,%rdx
+    646c6468:	jne    646c6478 <__mingw_enum_import_library_names+0x88>
+    646c646a:	jmp    646c645e <__mingw_enum_import_library_names+0x6e>
+    646c646c:	nopl   0x0(%rax)
+    646c6470:	sub    $0x1,%r9d
+    646c6474:	add    $0x14,%rdx
+    646c6478:	mov    0x4(%rdx),%ecx
+    646c647b:	test   %ecx,%ecx
+    646c647d:	jne    646c6486 <__mingw_enum_import_library_names+0x96>
+    646c647f:	mov    0xc(%rdx),%eax
+    646c6482:	test   %eax,%eax
+    646c6484:	je     646c645e <__mingw_enum_import_library_names+0x6e>
+    646c6486:	test   %r9d,%r9d
+    646c6489:	jg     646c6470 <__mingw_enum_import_library_names+0x80>
+    646c648b:	mov    0xc(%rdx),%eax
+    646c648e:	add    %r11,%rax
+    646c6491:	add    $0x28,%rsp
+    646c6495:	ret
+    646c6496:	nop
+    646c6497:	nop
+    646c6498:	nop
+    646c6499:	nop
+    646c649a:	nop
+    646c649b:	nop
+    646c649c:	nop
+    646c649d:	nop
+    646c649e:	nop
+    646c649f:	nop
+
+00000000646c64a0 <_fpreset>:
+    646c64a0:	fninit
+    646c64a2:	ret
+    646c64a3:	nop
+    646c64a4:	nop
+    646c64a5:	nop
+    646c64a6:	nop
+    646c64a7:	nop
+    646c64a8:	nop
+    646c64a9:	nop
+    646c64aa:	nop
+    646c64ab:	nop
+    646c64ac:	nop
+    646c64ad:	nop
+    646c64ae:	nop
+    646c64af:	nop
 
-00000000646c67a0 <___chkstk_ms>:
+00000000646c64b0 <___chkstk_ms>:
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:117
-    646c67a0:	push   %rcx
+    646c64b0:	push   %rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:119
-    646c67a1:	push   %rax
+    646c64b1:	push   %rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:121
-    646c67a2:	cmp    $0x1000,%rax
+    646c64b2:	cmp    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:122
-    646c67a8:	lea    0x18(%rsp),%rcx
+    646c64b8:	lea    0x18(%rsp),%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:123
-    646c67ad:	jb     646c67c8 <___chkstk_ms+0x28>
+    646c64bd:	jb     646c64d8 <___chkstk_ms+0x28>
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:125
-    646c67af:	sub    $0x1000,%rcx
+    646c64bf:	sub    $0x1000,%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:126
-    646c67b6:	orq    $0x0,(%rcx)
+    646c64c6:	orq    $0x0,(%rcx)
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:127
-    646c67ba:	sub    $0x1000,%rax
+    646c64ca:	sub    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:128
-    646c67c0:	cmp    $0x1000,%rax
+    646c64d0:	cmp    $0x1000,%rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:129
-    646c67c6:	ja     646c67af <___chkstk_ms+0xf>
+    646c64d6:	ja     646c64bf <___chkstk_ms+0xf>
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:131
-    646c67c8:	sub    %rax,%rcx
+    646c64d8:	sub    %rax,%rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:132
-    646c67cb:	orq    $0x0,(%rcx)
+    646c64db:	orq    $0x0,(%rcx)
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:134
-    646c67cf:	pop    %rax
+    646c64df:	pop    %rax
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:136
-    646c67d0:	pop    %rcx
+    646c64e0:	pop    %rcx
 C:\mingw810\x86_64-810-win32-seh-rt_v6-rev0\build\gcc-8.1.0\x86_64-w64-mingw32\libgcc/../../../../../src/gcc-8.1.0/libgcc/config/i386/cygwin.S:138
-    646c67d1:	ret
-    646c67d2:	nop
-    646c67d3:	nop
-    646c67d4:	nop
-    646c67d5:	nop
-    646c67d6:	nop
-    646c67d7:	nop
-    646c67d8:	nop
-    646c67d9:	nop
-    646c67da:	nop
-    646c67db:	nop
-    646c67dc:	nop
-    646c67dd:	nop
-    646c67de:	nop
-    646c67df:	nop
-
-00000000646c67e0 <DllEntryPoint>:
-    646c67e0:	mov    $0x1,%eax
-    646c67e5:	ret
-    646c67e6:	nop
-    646c67e7:	nop
-    646c67e8:	nop
-    646c67e9:	nop
-    646c67ea:	nop
-    646c67eb:	nop
-    646c67ec:	nop
-    646c67ed:	nop
-    646c67ee:	nop
-    646c67ef:	nop
-
-00000000646c67f0 <DllMain>:
-    646c67f0:	mov    $0x1,%eax
-    646c67f5:	ret
-    646c67f6:	nop
-    646c67f7:	nop
-    646c67f8:	nop
-    646c67f9:	nop
-    646c67fa:	nop
-    646c67fb:	nop
-    646c67fc:	nop
-    646c67fd:	nop
-    646c67fe:	nop
-    646c67ff:	nop
-
-00000000646c6800 <__fpclassify>:
-    646c6800:	movq   %xmm0,%rax
-    646c6805:	movq   %xmm0,%rdx
-    646c680a:	shr    $0x20,%rax
-    646c680e:	mov    %eax,%ecx
-    646c6810:	and    $0xfffff,%ecx
-    646c6816:	or     %edx,%ecx
-    646c6818:	mov    %eax,%edx
-    646c681a:	mov    $0x4000,%eax
-    646c681f:	and    $0x7ff00000,%edx
-    646c6825:	mov    %ecx,%r8d
-    646c6828:	or     %edx,%r8d
-    646c682b:	je     646c6843 <__fpclassify+0x43>
-    646c682d:	test   %edx,%edx
-    646c682f:	mov    $0x4400,%eax
-    646c6834:	je     646c6843 <__fpclassify+0x43>
-    646c6836:	cmp    $0x7ff00000,%edx
-    646c683c:	mov    $0x400,%eax
-    646c6841:	je     646c6844 <__fpclassify+0x44>
-    646c6843:	ret
-    646c6844:	cmp    $0x1,%ecx
-    646c6847:	sbb    %eax,%eax
-    646c6849:	and    $0x400,%eax
-    646c684e:	add    $0x100,%eax
-    646c6853:	ret
-    646c6854:	nop
-    646c6855:	nop
-    646c6856:	nop
-    646c6857:	nop
-    646c6858:	nop
-    646c6859:	nop
-    646c685a:	nop
-    646c685b:	nop
-    646c685c:	nop
-    646c685d:	nop
-    646c685e:	nop
-    646c685f:	nop
-
-00000000646c6860 <sqrt>:
-    646c6860:	push   %rbx
-    646c6861:	sub    $0x50,%rsp
-    646c6865:	movaps %xmm6,0x40(%rsp)
-    646c686a:	movq   %xmm0,%rdx
-    646c686f:	movq   %xmm0,%rbx
-    646c6874:	shr    $0x20,%rdx
-    646c6878:	mov    %edx,%eax
-    646c687a:	mov    %edx,%ecx
-    646c687c:	and    $0xfffff,%eax
-    646c6881:	and    $0x7ff00000,%ecx
-    646c6887:	or     %ebx,%eax
-    646c6889:	mov    %eax,%r8d
-    646c688c:	or     %ecx,%r8d
-    646c688f:	je     646c68d0 <sqrt+0x70>
-    646c6891:	test   %ecx,%ecx
-    646c6893:	jne    646c68f0 <sqrt+0x90>
-    646c6895:	test   %edx,%edx
-    646c6897:	js     646c6910 <sqrt+0xb0>
-    646c6899:	movsd  0x2a9f(%rip),%xmm0        # 646c9340 <.rdata+0x20>
-    646c68a1:	movq   %rbx,%xmm1
-    646c68a6:	ucomisd %xmm0,%xmm1
-    646c68aa:	jp     646c68ae <sqrt+0x4e>
-    646c68ac:	je     646c68c3 <sqrt+0x63>
-    646c68ae:	mov    %rbx,0x38(%rsp)
-    646c68b3:	fldl   0x38(%rsp)
-    646c68b7:	fsqrt
-    646c68b9:	fstpl  0x38(%rsp)
-    646c68bd:	movsd  0x38(%rsp),%xmm0
-    646c68c3:	movaps 0x40(%rsp),%xmm6
-    646c68c8:	add    $0x50,%rsp
-    646c68cc:	pop    %rbx
-    646c68cd:	ret
-    646c68ce:	xchg   %ax,%ax
-    646c68d0:	test   %edx,%edx
-    646c68d2:	pxor   %xmm0,%xmm0
-    646c68d6:	jns    646c68c3 <sqrt+0x63>
-    646c68d8:	movsd  0x2a48(%rip),%xmm0        # 646c9328 <.rdata+0x8>
-    646c68e0:	movaps 0x40(%rsp),%xmm6
-    646c68e5:	add    $0x50,%rsp
-    646c68e9:	pop    %rbx
-    646c68ea:	ret
-    646c68eb:	nopl   0x0(%rax,%rax,1)
-    646c68f0:	cmp    $0x7ff00000,%ecx
-    646c68f6:	jne    646c6895 <sqrt+0x35>
-    646c68f8:	test   %eax,%eax
-    646c68fa:	jne    646c6952 <sqrt+0xf2>
-    646c68fc:	test   %edx,%edx
-    646c68fe:	js     646c6910 <sqrt+0xb0>
-    646c6900:	movsd  0x2a30(%rip),%xmm0        # 646c9338 <.rdata+0x18>
-    646c6908:	jmp    646c68c3 <sqrt+0x63>
-    646c690a:	nopw   0x0(%rax,%rax,1)
-    646c6910:	call   646c79d8 <_errno>
-    646c6915:	movq   %rbx,%xmm2
-    646c691a:	mov    $0x1,%ecx
-    646c691f:	movsd  0x2a09(%rip),%xmm6        # 646c9330 <.rdata+0x10>
-    646c6927:	movl   $0x21,(%rax)
-    646c692d:	lea    0x29ec(%rip),%rdx        # 646c9320 <.rdata>
-    646c6934:	pxor   %xmm3,%xmm3
-    646c6938:	movsd  %xmm6,0x20(%rsp)
-    646c693e:	call   646c7c50 <__mingw_raise_matherr>
-    646c6943:	movapd %xmm6,%xmm0
-    646c6947:	movaps 0x40(%rsp),%xmm6
-    646c694c:	add    $0x50,%rsp
-    646c6950:	pop    %rbx
-    646c6951:	ret
-    646c6952:	call   646c79d8 <_errno>
-    646c6957:	movq   %rbx,%xmm2
-    646c695c:	mov    $0x1,%ecx
-    646c6961:	pxor   %xmm3,%xmm3
-    646c6965:	movl   $0x21,(%rax)
-    646c696b:	lea    0x29ae(%rip),%rdx        # 646c9320 <.rdata>
-    646c6972:	mov    %rbx,0x20(%rsp)
-    646c6977:	call   646c7c50 <__mingw_raise_matherr>
-    646c697c:	movq   %rbx,%xmm0
-    646c6981:	jmp    646c68c3 <sqrt+0x63>
-    646c6986:	nop
-    646c6987:	nop
-    646c6988:	nop
-    646c6989:	nop
-    646c698a:	nop
-    646c698b:	nop
-    646c698c:	nop
-    646c698d:	nop
-    646c698e:	nop
-    646c698f:	nop
-
-00000000646c6990 <__ms_vsnprintf>:
-    646c6990:	jmp    646c79c0 <_vsnprintf>
-    646c6995:	nop
-    646c6996:	nop
-    646c6997:	nop
-    646c6998:	nop
-    646c6999:	nop
-    646c699a:	nop
-    646c699b:	nop
-    646c699c:	nop
-    646c699d:	nop
-    646c699e:	nop
-    646c699f:	nop
-
-00000000646c69a0 <ceil>:
-    646c69a0:	movq   %xmm0,%rax
-    646c69a5:	mov    %rax,%rcx
-    646c69a8:	sar    $0x34,%rcx
-    646c69ac:	and    $0x7ff,%ecx
-    646c69b2:	sub    $0x3ff,%ecx
-    646c69b8:	cmp    $0x33,%ecx
-    646c69bb:	jg     646c6a60 <.is_intnaninf>
-    646c69c1:	test   %rax,%rax
-    646c69c4:	je     646c6a70 <.ret_org>
-    646c69ca:	test   %ecx,%ecx
-    646c69cc:	js     646c6a20 <.signed_val>
-    646c69ce:	movabs $0xfffffffffffff,%rdx
-    646c69d8:	sar    %cl,%rdx
-    646c69db:	test   %rax,%rdx
-    646c69de:	je     646c6a70 <.ret_org>
-    646c69e4:	addsd  0x2964(%rip),%xmm0        # 646c9350 <.huge>
-    646c69ec:	ucomisd 0x2964(%rip),%xmm0        # 646c9358 <.zero>
-    646c69f4:	jbe    646c6a11 <.doret>
-    646c69f6:	test   %rax,%rax
-    646c69f9:	jle    646c6a0b <.l1>
-    646c69fb:	movabs $0x10000000000000,%r8
-    646c6a05:	shr    %cl,%r8
-    646c6a08:	add    %r8,%rax
-
-00000000646c6a0b <.l1>:
-    646c6a0b:	not    %rdx
-    646c6a0e:	and    %rdx,%rax
-
-00000000646c6a11 <.doret>:
-    646c6a11:	movq   %rax,%xmm0
-    646c6a16:	ret
-    646c6a17:	nopw   0x0(%rax,%rax,1)
-
-00000000646c6a20 <.signed_val>:
-    646c6a20:	addsd  0x2928(%rip),%xmm0        # 646c9350 <.huge>
-    646c6a28:	ucomisd 0x2928(%rip),%xmm0        # 646c9358 <.zero>
-    646c6a30:	jbe    646c6a50 <.doret2>
-    646c6a32:	test   %rax,%rax
-    646c6a35:	movabs $0x3ff0000000000000,%rdx
-    646c6a3f:	movabs $0x8000000000000000,%rax
-    646c6a49:	cmovns %rdx,%rax
-    646c6a4d:	nopl   (%rax)
-
-00000000646c6a50 <.doret2>:
-    646c6a50:	movq   %rax,%xmm0
-    646c6a55:	ret
-    646c6a56:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6a60 <.is_intnaninf>:
-    646c6a60:	cmp    $0x400,%ecx
-    646c6a66:	je     646c6a72 <.ret_naninf>
-    646c6a68:	nopl   0x0(%rax,%rax,1)
-
-00000000646c6a70 <.ret_org>:
-    646c6a70:	repz ret
-
-00000000646c6a72 <.ret_naninf>:
-    646c6a72:	addsd  %xmm0,%xmm0
-    646c6a76:	ret
-    646c6a77:	nop
-    646c6a78:	nop
-    646c6a79:	nop
-    646c6a7a:	nop
-    646c6a7b:	nop
-    646c6a7c:	nop
-    646c6a7d:	nop
-    646c6a7e:	nop
-    646c6a7f:	nop
-
-00000000646c6a80 <cos>:
-    646c6a80:	push   %rbx
-    646c6a81:	sub    $0x70,%rsp
-    646c6a85:	movaps %xmm6,0x60(%rsp)
-    646c6a8a:	movq   %xmm0,%rax
-    646c6a8f:	movq   %xmm0,%rbx
-    646c6a94:	shr    $0x20,%rax
-    646c6a98:	mov    %eax,%edx
-    646c6a9a:	and    $0x7ff00000,%eax
-    646c6a9f:	and    $0xfffff,%edx
-    646c6aa5:	or     %ebx,%edx
-    646c6aa7:	mov    %edx,%ecx
-    646c6aa9:	or     %eax,%ecx
-    646c6aab:	sete   %r8b
-    646c6aaf:	test   %eax,%eax
-    646c6ab1:	sete   %cl
-    646c6ab4:	or     %cl,%r8b
-    646c6ab7:	jne    646c6ac0 <cos+0x40>
-    646c6ab9:	cmp    $0x7ff00000,%eax
-    646c6abe:	je     646c6af5 <cos+0x75>
-    646c6ac0:	mov    %rbx,0x30(%rsp)
-    646c6ac5:	lea    0x50(%rsp),%rcx
-    646c6aca:	fldl   0x30(%rsp)
-    646c6ace:	fstpt  0x40(%rsp)
-    646c6ad2:	lea    0x40(%rsp),%rdx
-    646c6ad7:	call   646c6b80 <__cosl_internal>
-    646c6adc:	fldt   0x50(%rsp)
-    646c6ae0:	fstpl  0x38(%rsp)
-    646c6ae4:	movsd  0x38(%rsp),%xmm0
-    646c6aea:	movaps 0x60(%rsp),%xmm6
-    646c6aef:	add    $0x70,%rsp
-    646c6af3:	pop    %rbx
-    646c6af4:	ret
-    646c6af5:	test   %edx,%edx
-    646c6af7:	jne    646c6b40 <cos+0xc0>
-    646c6af9:	call   646c79d8 <_errno>
-    646c6afe:	movq   %rbx,%xmm2
-    646c6b03:	mov    $0x1,%ecx
-    646c6b08:	movsd  0x2858(%rip),%xmm6        # 646c9368 <.rdata+0x8>
-    646c6b10:	movl   $0x21,(%rax)
-    646c6b16:	lea    0x2843(%rip),%rdx        # 646c9360 <.rdata>
-    646c6b1d:	pxor   %xmm3,%xmm3
-    646c6b21:	movsd  %xmm6,0x20(%rsp)
-    646c6b27:	call   646c7c50 <__mingw_raise_matherr>
-    646c6b2c:	movapd %xmm6,%xmm0
-    646c6b30:	movaps 0x60(%rsp),%xmm6
-    646c6b35:	add    $0x70,%rsp
-    646c6b39:	pop    %rbx
-    646c6b3a:	ret
-    646c6b3b:	nopl   0x0(%rax,%rax,1)
-    646c6b40:	call   646c79d8 <_errno>
+    646c64e1:	ret
+    646c64e2:	nop
+    646c64e3:	nop
+    646c64e4:	nop
+    646c64e5:	nop
+    646c64e6:	nop
+    646c64e7:	nop
+    646c64e8:	nop
+    646c64e9:	nop
+    646c64ea:	nop
+    646c64eb:	nop
+    646c64ec:	nop
+    646c64ed:	nop
+    646c64ee:	nop
+    646c64ef:	nop
+
+00000000646c64f0 <DllEntryPoint>:
+    646c64f0:	mov    $0x1,%eax
+    646c64f5:	ret
+    646c64f6:	nop
+    646c64f7:	nop
+    646c64f8:	nop
+    646c64f9:	nop
+    646c64fa:	nop
+    646c64fb:	nop
+    646c64fc:	nop
+    646c64fd:	nop
+    646c64fe:	nop
+    646c64ff:	nop
+
+00000000646c6500 <DllMain>:
+    646c6500:	mov    $0x1,%eax
+    646c6505:	ret
+    646c6506:	nop
+    646c6507:	nop
+    646c6508:	nop
+    646c6509:	nop
+    646c650a:	nop
+    646c650b:	nop
+    646c650c:	nop
+    646c650d:	nop
+    646c650e:	nop
+    646c650f:	nop
+
+00000000646c6510 <__fpclassify>:
+    646c6510:	movq   %xmm0,%rax
+    646c6515:	movq   %xmm0,%rdx
+    646c651a:	shr    $0x20,%rax
+    646c651e:	mov    %eax,%ecx
+    646c6520:	and    $0xfffff,%ecx
+    646c6526:	or     %edx,%ecx
+    646c6528:	mov    %eax,%edx
+    646c652a:	mov    $0x4000,%eax
+    646c652f:	and    $0x7ff00000,%edx
+    646c6535:	mov    %ecx,%r8d
+    646c6538:	or     %edx,%r8d
+    646c653b:	je     646c6553 <__fpclassify+0x43>
+    646c653d:	test   %edx,%edx
+    646c653f:	mov    $0x4400,%eax
+    646c6544:	je     646c6553 <__fpclassify+0x43>
+    646c6546:	cmp    $0x7ff00000,%edx
+    646c654c:	mov    $0x400,%eax
+    646c6551:	je     646c6554 <__fpclassify+0x44>
+    646c6553:	ret
+    646c6554:	cmp    $0x1,%ecx
+    646c6557:	sbb    %eax,%eax
+    646c6559:	and    $0x400,%eax
+    646c655e:	add    $0x100,%eax
+    646c6563:	ret
+    646c6564:	nop
+    646c6565:	nop
+    646c6566:	nop
+    646c6567:	nop
+    646c6568:	nop
+    646c6569:	nop
+    646c656a:	nop
+    646c656b:	nop
+    646c656c:	nop
+    646c656d:	nop
+    646c656e:	nop
+    646c656f:	nop
+
+00000000646c6570 <sqrt>:
+    646c6570:	push   %rbx
+    646c6571:	sub    $0x50,%rsp
+    646c6575:	movaps %xmm6,0x40(%rsp)
+    646c657a:	movq   %xmm0,%rdx
+    646c657f:	movq   %xmm0,%rbx
+    646c6584:	shr    $0x20,%rdx
+    646c6588:	mov    %edx,%eax
+    646c658a:	mov    %edx,%ecx
+    646c658c:	and    $0xfffff,%eax
+    646c6591:	and    $0x7ff00000,%ecx
+    646c6597:	or     %ebx,%eax
+    646c6599:	mov    %eax,%r8d
+    646c659c:	or     %ecx,%r8d
+    646c659f:	je     646c65e0 <sqrt+0x70>
+    646c65a1:	test   %ecx,%ecx
+    646c65a3:	jne    646c6600 <sqrt+0x90>
+    646c65a5:	test   %edx,%edx
+    646c65a7:	js     646c6620 <sqrt+0xb0>
+    646c65a9:	movsd  0x2d6f(%rip),%xmm0        # 646c9320 <.rdata+0x20>
+    646c65b1:	movq   %rbx,%xmm1
+    646c65b6:	ucomisd %xmm0,%xmm1
+    646c65ba:	jp     646c65be <sqrt+0x4e>
+    646c65bc:	je     646c65d3 <sqrt+0x63>
+    646c65be:	mov    %rbx,0x38(%rsp)
+    646c65c3:	fldl   0x38(%rsp)
+    646c65c7:	fsqrt
+    646c65c9:	fstpl  0x38(%rsp)
+    646c65cd:	movsd  0x38(%rsp),%xmm0
+    646c65d3:	movaps 0x40(%rsp),%xmm6
+    646c65d8:	add    $0x50,%rsp
+    646c65dc:	pop    %rbx
+    646c65dd:	ret
+    646c65de:	xchg   %ax,%ax
+    646c65e0:	test   %edx,%edx
+    646c65e2:	pxor   %xmm0,%xmm0
+    646c65e6:	jns    646c65d3 <sqrt+0x63>
+    646c65e8:	movsd  0x2d18(%rip),%xmm0        # 646c9308 <.rdata+0x8>
+    646c65f0:	movaps 0x40(%rsp),%xmm6
+    646c65f5:	add    $0x50,%rsp
+    646c65f9:	pop    %rbx
+    646c65fa:	ret
+    646c65fb:	nopl   0x0(%rax,%rax,1)
+    646c6600:	cmp    $0x7ff00000,%ecx
+    646c6606:	jne    646c65a5 <sqrt+0x35>
+    646c6608:	test   %eax,%eax
+    646c660a:	jne    646c6662 <sqrt+0xf2>
+    646c660c:	test   %edx,%edx
+    646c660e:	js     646c6620 <sqrt+0xb0>
+    646c6610:	movsd  0x2d00(%rip),%xmm0        # 646c9318 <.rdata+0x18>
+    646c6618:	jmp    646c65d3 <sqrt+0x63>
+    646c661a:	nopw   0x0(%rax,%rax,1)
+    646c6620:	call   646c76e8 <_errno>
+    646c6625:	movq   %rbx,%xmm2
+    646c662a:	mov    $0x1,%ecx
+    646c662f:	movsd  0x2cd9(%rip),%xmm6        # 646c9310 <.rdata+0x10>
+    646c6637:	movl   $0x21,(%rax)
+    646c663d:	lea    0x2cbc(%rip),%rdx        # 646c9300 <.rdata>
+    646c6644:	pxor   %xmm3,%xmm3
+    646c6648:	movsd  %xmm6,0x20(%rsp)
+    646c664e:	call   646c7960 <__mingw_raise_matherr>
+    646c6653:	movapd %xmm6,%xmm0
+    646c6657:	movaps 0x40(%rsp),%xmm6
+    646c665c:	add    $0x50,%rsp
+    646c6660:	pop    %rbx
+    646c6661:	ret
+    646c6662:	call   646c76e8 <_errno>
+    646c6667:	movq   %rbx,%xmm2
+    646c666c:	mov    $0x1,%ecx
+    646c6671:	pxor   %xmm3,%xmm3
+    646c6675:	movl   $0x21,(%rax)
+    646c667b:	lea    0x2c7e(%rip),%rdx        # 646c9300 <.rdata>
+    646c6682:	mov    %rbx,0x20(%rsp)
+    646c6687:	call   646c7960 <__mingw_raise_matherr>
+    646c668c:	movq   %rbx,%xmm0
+    646c6691:	jmp    646c65d3 <sqrt+0x63>
+    646c6696:	nop
+    646c6697:	nop
+    646c6698:	nop
+    646c6699:	nop
+    646c669a:	nop
+    646c669b:	nop
+    646c669c:	nop
+    646c669d:	nop
+    646c669e:	nop
+    646c669f:	nop
+
+00000000646c66a0 <__ms_vsnprintf>:
+    646c66a0:	jmp    646c76d0 <_vsnprintf>
+    646c66a5:	nop
+    646c66a6:	nop
+    646c66a7:	nop
+    646c66a8:	nop
+    646c66a9:	nop
+    646c66aa:	nop
+    646c66ab:	nop
+    646c66ac:	nop
+    646c66ad:	nop
+    646c66ae:	nop
+    646c66af:	nop
+
+00000000646c66b0 <ceil>:
+    646c66b0:	movq   %xmm0,%rax
+    646c66b5:	mov    %rax,%rcx
+    646c66b8:	sar    $0x34,%rcx
+    646c66bc:	and    $0x7ff,%ecx
+    646c66c2:	sub    $0x3ff,%ecx
+    646c66c8:	cmp    $0x33,%ecx
+    646c66cb:	jg     646c6770 <.is_intnaninf>
+    646c66d1:	test   %rax,%rax
+    646c66d4:	je     646c6780 <.ret_org>
+    646c66da:	test   %ecx,%ecx
+    646c66dc:	js     646c6730 <.signed_val>
+    646c66de:	movabs $0xfffffffffffff,%rdx
+    646c66e8:	sar    %cl,%rdx
+    646c66eb:	test   %rax,%rdx
+    646c66ee:	je     646c6780 <.ret_org>
+    646c66f4:	addsd  0x2c34(%rip),%xmm0        # 646c9330 <.huge>
+    646c66fc:	ucomisd 0x2c34(%rip),%xmm0        # 646c9338 <.zero>
+    646c6704:	jbe    646c6721 <.doret>
+    646c6706:	test   %rax,%rax
+    646c6709:	jle    646c671b <.l1>
+    646c670b:	movabs $0x10000000000000,%r8
+    646c6715:	shr    %cl,%r8
+    646c6718:	add    %r8,%rax
+
+00000000646c671b <.l1>:
+    646c671b:	not    %rdx
+    646c671e:	and    %rdx,%rax
+
+00000000646c6721 <.doret>:
+    646c6721:	movq   %rax,%xmm0
+    646c6726:	ret
+    646c6727:	nopw   0x0(%rax,%rax,1)
+
+00000000646c6730 <.signed_val>:
+    646c6730:	addsd  0x2bf8(%rip),%xmm0        # 646c9330 <.huge>
+    646c6738:	ucomisd 0x2bf8(%rip),%xmm0        # 646c9338 <.zero>
+    646c6740:	jbe    646c6760 <.doret2>
+    646c6742:	test   %rax,%rax
+    646c6745:	movabs $0x3ff0000000000000,%rdx
+    646c674f:	movabs $0x8000000000000000,%rax
+    646c6759:	cmovns %rdx,%rax
+    646c675d:	nopl   (%rax)
+
+00000000646c6760 <.doret2>:
+    646c6760:	movq   %rax,%xmm0
+    646c6765:	ret
+    646c6766:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6770 <.is_intnaninf>:
+    646c6770:	cmp    $0x400,%ecx
+    646c6776:	je     646c6782 <.ret_naninf>
+    646c6778:	nopl   0x0(%rax,%rax,1)
+
+00000000646c6780 <.ret_org>:
+    646c6780:	repz ret
+
+00000000646c6782 <.ret_naninf>:
+    646c6782:	addsd  %xmm0,%xmm0
+    646c6786:	ret
+    646c6787:	nop
+    646c6788:	nop
+    646c6789:	nop
+    646c678a:	nop
+    646c678b:	nop
+    646c678c:	nop
+    646c678d:	nop
+    646c678e:	nop
+    646c678f:	nop
+
+00000000646c6790 <cos>:
+    646c6790:	push   %rbx
+    646c6791:	sub    $0x70,%rsp
+    646c6795:	movaps %xmm6,0x60(%rsp)
+    646c679a:	movq   %xmm0,%rax
+    646c679f:	movq   %xmm0,%rbx
+    646c67a4:	shr    $0x20,%rax
+    646c67a8:	mov    %eax,%edx
+    646c67aa:	and    $0x7ff00000,%eax
+    646c67af:	and    $0xfffff,%edx
+    646c67b5:	or     %ebx,%edx
+    646c67b7:	mov    %edx,%ecx
+    646c67b9:	or     %eax,%ecx
+    646c67bb:	sete   %r8b
+    646c67bf:	test   %eax,%eax
+    646c67c1:	sete   %cl
+    646c67c4:	or     %cl,%r8b
+    646c67c7:	jne    646c67d0 <cos+0x40>
+    646c67c9:	cmp    $0x7ff00000,%eax
+    646c67ce:	je     646c6805 <cos+0x75>
+    646c67d0:	mov    %rbx,0x30(%rsp)
+    646c67d5:	lea    0x50(%rsp),%rcx
+    646c67da:	fldl   0x30(%rsp)
+    646c67de:	fstpt  0x40(%rsp)
+    646c67e2:	lea    0x40(%rsp),%rdx
+    646c67e7:	call   646c6890 <__cosl_internal>
+    646c67ec:	fldt   0x50(%rsp)
+    646c67f0:	fstpl  0x38(%rsp)
+    646c67f4:	movsd  0x38(%rsp),%xmm0
+    646c67fa:	movaps 0x60(%rsp),%xmm6
+    646c67ff:	add    $0x70,%rsp
+    646c6803:	pop    %rbx
+    646c6804:	ret
+    646c6805:	test   %edx,%edx
+    646c6807:	jne    646c6850 <cos+0xc0>
+    646c6809:	call   646c76e8 <_errno>
+    646c680e:	movq   %rbx,%xmm2
+    646c6813:	mov    $0x1,%ecx
+    646c6818:	movsd  0x2b28(%rip),%xmm6        # 646c9348 <.rdata+0x8>
+    646c6820:	movl   $0x21,(%rax)
+    646c6826:	lea    0x2b13(%rip),%rdx        # 646c9340 <.rdata>
+    646c682d:	pxor   %xmm3,%xmm3
+    646c6831:	movsd  %xmm6,0x20(%rsp)
+    646c6837:	call   646c7960 <__mingw_raise_matherr>
+    646c683c:	movapd %xmm6,%xmm0
+    646c6840:	movaps 0x60(%rsp),%xmm6
+    646c6845:	add    $0x70,%rsp
+    646c6849:	pop    %rbx
+    646c684a:	ret
+    646c684b:	nopl   0x0(%rax,%rax,1)
+    646c6850:	call   646c76e8 <_errno>
+    646c6855:	movq   %rbx,%xmm2
+    646c685a:	mov    $0x1,%ecx
+    646c685f:	pxor   %xmm3,%xmm3
+    646c6863:	movl   $0x21,(%rax)
+    646c6869:	lea    0x2ad0(%rip),%rdx        # 646c9340 <.rdata>
+    646c6870:	mov    %rbx,0x20(%rsp)
+    646c6875:	call   646c7960 <__mingw_raise_matherr>
+    646c687a:	movq   %rbx,%xmm0
+    646c687f:	jmp    646c67fa <cos+0x6a>
+    646c6884:	nop
+    646c6885:	nop
+    646c6886:	nop
+    646c6887:	nop
+    646c6888:	nop
+    646c6889:	nop
+    646c688a:	nop
+    646c688b:	nop
+    646c688c:	nop
+    646c688d:	nop
+    646c688e:	nop
+    646c688f:	nop
+
+00000000646c6890 <__cosl_internal>:
+    646c6890:	fldt   (%rdx)
+    646c6892:	fcos
+    646c6894:	fnstsw %ax
+    646c6896:	test   $0x400,%eax
+    646c689b:	je     646c68b2 <__cosl_internal+0x22>
+    646c689d:	fldpi
+    646c689f:	fadd   %st(0),%st
+    646c68a1:	fxch   %st(1)
+    646c68a3:	fprem1
+    646c68a5:	fnstsw %ax
+    646c68a7:	test   $0x400,%eax
+    646c68ac:	jne    646c68a3 <__cosl_internal+0x13>
+    646c68ae:	fstp   %st(1)
+    646c68b0:	fcos
+    646c68b2:	mov    %rcx,%rax
+    646c68b5:	movq   $0x0,0x8(%rcx)
+    646c68bd:	fstpt  (%rcx)
+    646c68bf:	ret
+
+00000000646c68c0 <exp>:
+    646c68c0:	push   %rbx
+    646c68c1:	sub    $0x50,%rsp
+    646c68c5:	movaps %xmm6,0x40(%rsp)
+    646c68ca:	movsd  0x2a8e(%rip),%xmm6        # 646c9360 <.rdata+0x10>
+    646c68d2:	movq   %xmm0,%rdx
+    646c68d7:	movq   %xmm0,%rbx
+    646c68dc:	shr    $0x20,%rdx
+    646c68e0:	mov    %edx,%eax
+    646c68e2:	mov    %edx,%ecx
+    646c68e4:	and    $0xfffff,%eax
+    646c68e9:	and    $0x7ff00000,%ecx
+    646c68ef:	or     %ebx,%eax
+    646c68f1:	mov    %eax,%r8d
+    646c68f4:	or     %ecx,%r8d
+    646c68f7:	je     646c6929 <exp+0x69>
+    646c68f9:	cmp    $0x7ff00000,%ecx
+    646c68ff:	je     646c69c0 <exp+0x100>
+    646c6905:	ucomisd 0x2a5b(%rip),%xmm0        # 646c9368 <.rdata+0x18>
+    646c690d:	movapd %xmm0,%xmm1
+    646c6911:	ja     646c6a12 <exp+0x152>
+    646c6917:	movsd  0x2a51(%rip),%xmm0        # 646c9370 <.rdata+0x20>
+    646c691f:	pxor   %xmm6,%xmm6
+    646c6923:	ucomisd %xmm1,%xmm0
+    646c6927:	jbe    646c6940 <exp+0x80>
+    646c6929:	movapd %xmm6,%xmm0
+    646c692d:	movaps 0x40(%rsp),%xmm6
+    646c6932:	add    $0x50,%rsp
+    646c6936:	pop    %rbx
+    646c6937:	ret
+    646c6938:	nopl   0x0(%rax,%rax,1)
+    646c6940:	mov    %rbx,0x30(%rsp)
+    646c6945:	fldl   0x30(%rsp)
+    646c6949:	fldl2e
+    646c694b:	fmul   %st(1),%st
+    646c694d:	sub    $0x8,%rsp
+    646c6951:	fnstcw 0x4(%rsp)
+    646c6955:	movzwl 0x4(%rsp),%eax
+    646c695a:	or     $0xc,%ah
+    646c695d:	mov    %ax,(%rsp)
+    646c6961:	fldcw  (%rsp)
+    646c6964:	frndint
+    646c6966:	fld    %st(1)
+    646c6968:	frndint
+    646c696a:	fldcw  0x4(%rsp)
+    646c696e:	add    $0x8,%rsp
+    646c6972:	fld    %st(1)
+    646c6974:	fldt   0x16c6(%rip)        # 646c8040 <c0>
+    646c697a:	fld    %st(2)
+    646c697c:	fmul   %st(1),%st
+    646c697e:	fsubp  %st,%st(2)
+    646c6980:	fld    %st(4)
+    646c6982:	fsub   %st(3),%st
+    646c6984:	fmulp  %st,%st(1)
+    646c6986:	faddp  %st,%st(1)
+    646c6988:	fldt   0x16a2(%rip)        # 646c8030 <c1>
+    646c698e:	fmul   %st(4),%st
+    646c6990:	faddp  %st,%st(1)
+    646c6992:	f2xm1
+    646c6994:	fld1
+    646c6996:	faddp  %st,%st(1)
+    646c6998:	fstp   %st(1)
+    646c699a:	fscale
+    646c699c:	fstp   %st(1)
+    646c699e:	fstp   %st(1)
+    646c69a0:	fstpl  0x38(%rsp)
+    646c69a4:	movsd  0x38(%rsp),%xmm6
+    646c69aa:	movapd %xmm6,%xmm0
+    646c69ae:	movaps 0x40(%rsp),%xmm6
+    646c69b3:	add    $0x50,%rsp
+    646c69b7:	pop    %rbx
+    646c69b8:	ret
+    646c69b9:	nopl   0x0(%rax)
+    646c69c0:	test   %eax,%eax
+    646c69c2:	jne    646c6a70 <exp+0x1b0>
+    646c69c8:	test   %edx,%edx
+    646c69ca:	js     646c6a54 <exp+0x194>
+    646c69d0:	call   646c76e8 <_errno>
+    646c69d5:	movsd  0x297b(%rip),%xmm6        # 646c9358 <.rdata+0x8>
+    646c69dd:	mov    $0x4,%ecx
+    646c69e2:	movl   $0x22,(%rax)
+    646c69e8:	movsd  %xmm6,0x20(%rsp)
+    646c69ee:	movq   %rbx,%xmm2
+    646c69f3:	pxor   %xmm3,%xmm3
+    646c69f7:	lea    0x2952(%rip),%rdx        # 646c9350 <.rdata>
+    646c69fe:	call   646c7960 <__mingw_raise_matherr>
+    646c6a03:	movapd %xmm6,%xmm0
+    646c6a07:	movaps 0x40(%rsp),%xmm6
+    646c6a0c:	add    $0x50,%rsp
+    646c6a10:	pop    %rbx
+    646c6a11:	ret
+    646c6a12:	call   646c76e8 <_errno>
+    646c6a17:	movq   %rbx,%xmm2
+    646c6a1c:	mov    $0x3,%ecx
+    646c6a21:	movsd  0x292f(%rip),%xmm6        # 646c9358 <.rdata+0x8>
+    646c6a29:	movl   $0x22,(%rax)
+    646c6a2f:	lea    0x291a(%rip),%rdx        # 646c9350 <.rdata>
+    646c6a36:	pxor   %xmm3,%xmm3
+    646c6a3a:	movsd  %xmm6,0x20(%rsp)
+    646c6a40:	call   646c7960 <__mingw_raise_matherr>
+    646c6a45:	movapd %xmm6,%xmm0
+    646c6a49:	movaps 0x40(%rsp),%xmm6
+    646c6a4e:	add    $0x50,%rsp
+    646c6a52:	pop    %rbx
+    646c6a53:	ret
+    646c6a54:	call   646c76e8 <_errno>
+    646c6a59:	pxor   %xmm6,%xmm6
+    646c6a5d:	mov    $0x3,%ecx
+    646c6a62:	movl   $0x22,(%rax)
+    646c6a68:	jmp    646c69e8 <exp+0x128>
+    646c6a6d:	nopl   (%rax)
+    646c6a70:	call   646c76e8 <_errno>
+    646c6a75:	movq   %rbx,%xmm2
+    646c6a7a:	mov    $0x1,%ecx
+    646c6a7f:	pxor   %xmm3,%xmm3
+    646c6a83:	movl   $0x21,(%rax)
+    646c6a89:	lea    0x28c0(%rip),%rdx        # 646c9350 <.rdata>
+    646c6a90:	movq   %rbx,%xmm6
+    646c6a95:	mov    %rbx,0x20(%rsp)
+    646c6a9a:	call   646c7960 <__mingw_raise_matherr>
+    646c6a9f:	jmp    646c6929 <exp+0x69>
+    646c6aa4:	nop
+    646c6aa5:	nop
+    646c6aa6:	nop
+    646c6aa7:	nop
+    646c6aa8:	nop
+    646c6aa9:	nop
+    646c6aaa:	nop
+    646c6aab:	nop
+    646c6aac:	nop
+    646c6aad:	nop
+    646c6aae:	nop
+    646c6aaf:	nop
+
+00000000646c6ab0 <log>:
+    646c6ab0:	push   %rbx
+    646c6ab1:	sub    $0x70,%rsp
+    646c6ab5:	movaps %xmm6,0x60(%rsp)
+    646c6aba:	movq   %xmm0,%rdx
+    646c6abf:	movq   %xmm0,%rbx
+    646c6ac4:	shr    $0x20,%rdx
+    646c6ac8:	mov    %edx,%eax
+    646c6aca:	mov    %edx,%ecx
+    646c6acc:	and    $0xfffff,%eax
+    646c6ad1:	and    $0x7ff00000,%ecx
+    646c6ad7:	or     %ebx,%eax
+    646c6ad9:	mov    %eax,%r8d
+    646c6adc:	or     %ecx,%r8d
+    646c6adf:	je     646c6b40 <log+0x90>
+    646c6ae1:	test   %ecx,%ecx
+    646c6ae3:	jne    646c6b22 <log+0x72>
+    646c6ae5:	test   %edx,%edx
+    646c6ae7:	js     646c6b8e <log+0xde>
+    646c6aed:	mov    %rbx,0x30(%rsp)
+    646c6af2:	lea    0x50(%rsp),%rcx
+    646c6af7:	fldl   0x30(%rsp)
+    646c6afb:	fstpt  0x40(%rsp)
+    646c6aff:	lea    0x40(%rsp),%rdx
+    646c6b04:	call   646c74d0 <__logl_internal>
+    646c6b09:	fldt   0x50(%rsp)
+    646c6b0d:	fstpl  0x38(%rsp)
+    646c6b11:	movsd  0x38(%rsp),%xmm0
+    646c6b17:	movaps 0x60(%rsp),%xmm6
+    646c6b1c:	add    $0x70,%rsp
+    646c6b20:	pop    %rbx
+    646c6b21:	ret
+    646c6b22:	cmp    $0x7ff00000,%ecx
+    646c6b28:	jne    646c6ae5 <log+0x35>
+    646c6b2a:	test   %eax,%eax
+    646c6b2c:	je     646c6b82 <log+0xd2>
+    646c6b2e:	test   %edx,%edx
+    646c6b30:	js     646c6b8e <log+0xde>
+    646c6b32:	movsd  0x2856(%rip),%xmm0        # 646c9390 <.rdata+0x10>
+    646c6b3a:	jmp    646c6b17 <log+0x67>
+    646c6b3c:	nopl   0x0(%rax)
+    646c6b40:	call   646c76e8 <_errno>
     646c6b45:	movq   %rbx,%xmm2
-    646c6b4a:	mov    $0x1,%ecx
-    646c6b4f:	pxor   %xmm3,%xmm3
-    646c6b53:	movl   $0x21,(%rax)
-    646c6b59:	lea    0x2800(%rip),%rdx        # 646c9360 <.rdata>
-    646c6b60:	mov    %rbx,0x20(%rsp)
-    646c6b65:	call   646c7c50 <__mingw_raise_matherr>
-    646c6b6a:	movq   %rbx,%xmm0
-    646c6b6f:	jmp    646c6aea <cos+0x6a>
-    646c6b74:	nop
-    646c6b75:	nop
-    646c6b76:	nop
-    646c6b77:	nop
-    646c6b78:	nop
-    646c6b79:	nop
-    646c6b7a:	nop
-    646c6b7b:	nop
-    646c6b7c:	nop
-    646c6b7d:	nop
-    646c6b7e:	nop
-    646c6b7f:	nop
-
-00000000646c6b80 <__cosl_internal>:
-    646c6b80:	fldt   (%rdx)
-    646c6b82:	fcos
-    646c6b84:	fnstsw %ax
-    646c6b86:	test   $0x400,%eax
-    646c6b8b:	je     646c6ba2 <__cosl_internal+0x22>
-    646c6b8d:	fldpi
-    646c6b8f:	fadd   %st(0),%st
-    646c6b91:	fxch   %st(1)
-    646c6b93:	fprem1
-    646c6b95:	fnstsw %ax
-    646c6b97:	test   $0x400,%eax
-    646c6b9c:	jne    646c6b93 <__cosl_internal+0x13>
-    646c6b9e:	fstp   %st(1)
-    646c6ba0:	fcos
-    646c6ba2:	mov    %rcx,%rax
-    646c6ba5:	movq   $0x0,0x8(%rcx)
-    646c6bad:	fstpt  (%rcx)
-    646c6baf:	ret
-
-00000000646c6bb0 <exp>:
-    646c6bb0:	push   %rbx
-    646c6bb1:	sub    $0x50,%rsp
-    646c6bb5:	movaps %xmm6,0x40(%rsp)
-    646c6bba:	movsd  0x27be(%rip),%xmm6        # 646c9380 <.rdata+0x10>
-    646c6bc2:	movq   %xmm0,%rdx
-    646c6bc7:	movq   %xmm0,%rbx
-    646c6bcc:	shr    $0x20,%rdx
-    646c6bd0:	mov    %edx,%eax
-    646c6bd2:	mov    %edx,%ecx
-    646c6bd4:	and    $0xfffff,%eax
-    646c6bd9:	and    $0x7ff00000,%ecx
-    646c6bdf:	or     %ebx,%eax
-    646c6be1:	mov    %eax,%r8d
-    646c6be4:	or     %ecx,%r8d
-    646c6be7:	je     646c6c19 <exp+0x69>
-    646c6be9:	cmp    $0x7ff00000,%ecx
-    646c6bef:	je     646c6cb0 <exp+0x100>
-    646c6bf5:	ucomisd 0x278b(%rip),%xmm0        # 646c9388 <.rdata+0x18>
-    646c6bfd:	movapd %xmm0,%xmm1
-    646c6c01:	ja     646c6d02 <exp+0x152>
-    646c6c07:	movsd  0x2781(%rip),%xmm0        # 646c9390 <.rdata+0x20>
-    646c6c0f:	pxor   %xmm6,%xmm6
-    646c6c13:	ucomisd %xmm1,%xmm0
-    646c6c17:	jbe    646c6c30 <exp+0x80>
-    646c6c19:	movapd %xmm6,%xmm0
-    646c6c1d:	movaps 0x40(%rsp),%xmm6
-    646c6c22:	add    $0x50,%rsp
-    646c6c26:	pop    %rbx
-    646c6c27:	ret
-    646c6c28:	nopl   0x0(%rax,%rax,1)
-    646c6c30:	mov    %rbx,0x30(%rsp)
-    646c6c35:	fldl   0x30(%rsp)
-    646c6c39:	fldl2e
-    646c6c3b:	fmul   %st(1),%st
-    646c6c3d:	sub    $0x8,%rsp
-    646c6c41:	fnstcw 0x4(%rsp)
-    646c6c45:	movzwl 0x4(%rsp),%eax
-    646c6c4a:	or     $0xc,%ah
-    646c6c4d:	mov    %ax,(%rsp)
-    646c6c51:	fldcw  (%rsp)
-    646c6c54:	frndint
-    646c6c56:	fld    %st(1)
-    646c6c58:	frndint
-    646c6c5a:	fldcw  0x4(%rsp)
-    646c6c5e:	add    $0x8,%rsp
-    646c6c62:	fld    %st(1)
-    646c6c64:	fldt   0x13d6(%rip)        # 646c8040 <c0>
-    646c6c6a:	fld    %st(2)
-    646c6c6c:	fmul   %st(1),%st
-    646c6c6e:	fsubp  %st,%st(2)
-    646c6c70:	fld    %st(4)
-    646c6c72:	fsub   %st(3),%st
-    646c6c74:	fmulp  %st,%st(1)
-    646c6c76:	faddp  %st,%st(1)
-    646c6c78:	fldt   0x13b2(%rip)        # 646c8030 <c1>
-    646c6c7e:	fmul   %st(4),%st
-    646c6c80:	faddp  %st,%st(1)
-    646c6c82:	f2xm1
-    646c6c84:	fld1
-    646c6c86:	faddp  %st,%st(1)
-    646c6c88:	fstp   %st(1)
-    646c6c8a:	fscale
-    646c6c8c:	fstp   %st(1)
-    646c6c8e:	fstp   %st(1)
-    646c6c90:	fstpl  0x38(%rsp)
-    646c6c94:	movsd  0x38(%rsp),%xmm6
-    646c6c9a:	movapd %xmm6,%xmm0
-    646c6c9e:	movaps 0x40(%rsp),%xmm6
-    646c6ca3:	add    $0x50,%rsp
-    646c6ca7:	pop    %rbx
-    646c6ca8:	ret
-    646c6ca9:	nopl   0x0(%rax)
-    646c6cb0:	test   %eax,%eax
-    646c6cb2:	jne    646c6d60 <exp+0x1b0>
-    646c6cb8:	test   %edx,%edx
-    646c6cba:	js     646c6d44 <exp+0x194>
-    646c6cc0:	call   646c79d8 <_errno>
-    646c6cc5:	movsd  0x26ab(%rip),%xmm6        # 646c9378 <.rdata+0x8>
-    646c6ccd:	mov    $0x4,%ecx
-    646c6cd2:	movl   $0x22,(%rax)
-    646c6cd8:	movsd  %xmm6,0x20(%rsp)
-    646c6cde:	movq   %rbx,%xmm2
-    646c6ce3:	pxor   %xmm3,%xmm3
-    646c6ce7:	lea    0x2682(%rip),%rdx        # 646c9370 <.rdata>
-    646c6cee:	call   646c7c50 <__mingw_raise_matherr>
-    646c6cf3:	movapd %xmm6,%xmm0
-    646c6cf7:	movaps 0x40(%rsp),%xmm6
-    646c6cfc:	add    $0x50,%rsp
-    646c6d00:	pop    %rbx
-    646c6d01:	ret
-    646c6d02:	call   646c79d8 <_errno>
-    646c6d07:	movq   %rbx,%xmm2
-    646c6d0c:	mov    $0x3,%ecx
-    646c6d11:	movsd  0x265f(%rip),%xmm6        # 646c9378 <.rdata+0x8>
-    646c6d19:	movl   $0x22,(%rax)
-    646c6d1f:	lea    0x264a(%rip),%rdx        # 646c9370 <.rdata>
-    646c6d26:	pxor   %xmm3,%xmm3
-    646c6d2a:	movsd  %xmm6,0x20(%rsp)
-    646c6d30:	call   646c7c50 <__mingw_raise_matherr>
-    646c6d35:	movapd %xmm6,%xmm0
-    646c6d39:	movaps 0x40(%rsp),%xmm6
-    646c6d3e:	add    $0x50,%rsp
-    646c6d42:	pop    %rbx
-    646c6d43:	ret
-    646c6d44:	call   646c79d8 <_errno>
-    646c6d49:	pxor   %xmm6,%xmm6
-    646c6d4d:	mov    $0x3,%ecx
-    646c6d52:	movl   $0x22,(%rax)
-    646c6d58:	jmp    646c6cd8 <exp+0x128>
-    646c6d5d:	nopl   (%rax)
-    646c6d60:	call   646c79d8 <_errno>
-    646c6d65:	movq   %rbx,%xmm2
-    646c6d6a:	mov    $0x1,%ecx
-    646c6d6f:	pxor   %xmm3,%xmm3
-    646c6d73:	movl   $0x21,(%rax)
-    646c6d79:	lea    0x25f0(%rip),%rdx        # 646c9370 <.rdata>
-    646c6d80:	movq   %rbx,%xmm6
-    646c6d85:	mov    %rbx,0x20(%rsp)
-    646c6d8a:	call   646c7c50 <__mingw_raise_matherr>
-    646c6d8f:	jmp    646c6c19 <exp+0x69>
-    646c6d94:	nop
-    646c6d95:	nop
-    646c6d96:	nop
-    646c6d97:	nop
-    646c6d98:	nop
-    646c6d99:	nop
-    646c6d9a:	nop
-    646c6d9b:	nop
-    646c6d9c:	nop
-    646c6d9d:	nop
-    646c6d9e:	nop
-    646c6d9f:	nop
-
-00000000646c6da0 <log>:
-    646c6da0:	push   %rbx
-    646c6da1:	sub    $0x70,%rsp
-    646c6da5:	movaps %xmm6,0x60(%rsp)
-    646c6daa:	movq   %xmm0,%rdx
-    646c6daf:	movq   %xmm0,%rbx
-    646c6db4:	shr    $0x20,%rdx
-    646c6db8:	mov    %edx,%eax
-    646c6dba:	mov    %edx,%ecx
-    646c6dbc:	and    $0xfffff,%eax
-    646c6dc1:	and    $0x7ff00000,%ecx
-    646c6dc7:	or     %ebx,%eax
-    646c6dc9:	mov    %eax,%r8d
-    646c6dcc:	or     %ecx,%r8d
-    646c6dcf:	je     646c6e30 <log+0x90>
-    646c6dd1:	test   %ecx,%ecx
-    646c6dd3:	jne    646c6e12 <log+0x72>
-    646c6dd5:	test   %edx,%edx
-    646c6dd7:	js     646c6e7e <log+0xde>
-    646c6ddd:	mov    %rbx,0x30(%rsp)
-    646c6de2:	lea    0x50(%rsp),%rcx
-    646c6de7:	fldl   0x30(%rsp)
-    646c6deb:	fstpt  0x40(%rsp)
-    646c6def:	lea    0x40(%rsp),%rdx
-    646c6df4:	call   646c77c0 <__logl_internal>
-    646c6df9:	fldt   0x50(%rsp)
-    646c6dfd:	fstpl  0x38(%rsp)
-    646c6e01:	movsd  0x38(%rsp),%xmm0
-    646c6e07:	movaps 0x60(%rsp),%xmm6
-    646c6e0c:	add    $0x70,%rsp
-    646c6e10:	pop    %rbx
-    646c6e11:	ret
-    646c6e12:	cmp    $0x7ff00000,%ecx
-    646c6e18:	jne    646c6dd5 <log+0x35>
-    646c6e1a:	test   %eax,%eax
-    646c6e1c:	je     646c6e72 <log+0xd2>
-    646c6e1e:	test   %edx,%edx
-    646c6e20:	js     646c6e7e <log+0xde>
-    646c6e22:	movsd  0x2586(%rip),%xmm0        # 646c93b0 <.rdata+0x10>
-    646c6e2a:	jmp    646c6e07 <log+0x67>
-    646c6e2c:	nopl   0x0(%rax)
-    646c6e30:	call   646c79d8 <_errno>
-    646c6e35:	movq   %rbx,%xmm2
-    646c6e3a:	mov    $0x3,%ecx
-    646c6e3f:	movsd  0x2561(%rip),%xmm6        # 646c93a8 <.rdata+0x8>
-    646c6e47:	movl   $0x22,(%rax)
-    646c6e4d:	lea    0x254c(%rip),%rdx        # 646c93a0 <.rdata>
-    646c6e54:	pxor   %xmm3,%xmm3
-    646c6e58:	movsd  %xmm6,0x20(%rsp)
-    646c6e5e:	call   646c7c50 <__mingw_raise_matherr>
-    646c6e63:	movapd %xmm6,%xmm0
-    646c6e67:	movaps 0x60(%rsp),%xmm6
-    646c6e6c:	add    $0x70,%rsp
-    646c6e70:	pop    %rbx
-    646c6e71:	ret
-    646c6e72:	test   %edx,%edx
-    646c6e74:	movsd  0x253c(%rip),%xmm0        # 646c93b8 <.rdata+0x18>
-    646c6e7c:	jns    646c6e07 <log+0x67>
-    646c6e7e:	call   646c79d8 <_errno>
-    646c6e83:	movq   %rbx,%xmm2
-    646c6e88:	mov    $0x1,%ecx
-    646c6e8d:	movsd  0x251b(%rip),%xmm6        # 646c93b0 <.rdata+0x10>
-    646c6e95:	movl   $0x21,(%rax)
-    646c6e9b:	lea    0x24fe(%rip),%rdx        # 646c93a0 <.rdata>
-    646c6ea2:	pxor   %xmm3,%xmm3
-    646c6ea6:	movsd  %xmm6,0x20(%rsp)
-    646c6eac:	call   646c7c50 <__mingw_raise_matherr>
-    646c6eb1:	movapd %xmm6,%xmm0
-    646c6eb5:	movaps 0x60(%rsp),%xmm6
-    646c6eba:	add    $0x70,%rsp
-    646c6ebe:	pop    %rbx
-    646c6ebf:	ret
-
-00000000646c6ec0 <internal_modf>:
-    646c6ec0:	sub    $0x18,%rsp
-    646c6ec4:	movsd  %xmm0,0x8(%rsp)
-    646c6eca:	fldl   0x8(%rsp)
-    646c6ece:	push   %rax
-    646c6ecf:	sub    $0x8,%rsp
-    646c6ed3:	fnstcw 0x4(%rsp)
-    646c6ed7:	movzwl 0x4(%rsp),%eax
-    646c6edc:	or     $0xc,%ah
-    646c6edf:	mov    %ax,(%rsp)
-    646c6ee3:	fldcw  (%rsp)
-    646c6ee6:	frndint
-    646c6ee8:	fldcw  0x4(%rsp)
-    646c6eec:	add    $0x8,%rsp
-    646c6ef0:	pop    %rax
-    646c6ef1:	movq   %xmm0,%rax
-    646c6ef6:	fstpl  0x8(%rsp)
-    646c6efa:	movsd  0x8(%rsp),%xmm1
-    646c6f00:	shr    $0x20,%rax
-    646c6f04:	mov    %eax,%ecx
-    646c6f06:	movsd  %xmm1,(%rdx)
-    646c6f0a:	movq   %xmm0,%rdx
-    646c6f0f:	and    $0x7ff00000,%eax
-    646c6f14:	and    $0xfffff,%ecx
-    646c6f1a:	or     %edx,%ecx
-    646c6f1c:	mov    %ecx,%edx
-    646c6f1e:	or     %eax,%edx
-    646c6f20:	sete   %dl
-    646c6f23:	test   %eax,%eax
-    646c6f25:	sete   %r8b
-    646c6f29:	or     %r8d,%edx
-    646c6f2c:	xor    $0x1,%edx
-    646c6f2f:	cmp    $0x7ff00000,%eax
-    646c6f34:	sete   %al
-    646c6f37:	test   %al,%dl
-    646c6f39:	je     646c6f3f <internal_modf+0x7f>
-    646c6f3b:	test   %ecx,%ecx
-    646c6f3d:	je     646c6f50 <internal_modf+0x90>
-    646c6f3f:	subsd  0x8(%rsp),%xmm0
-    646c6f45:	add    $0x18,%rsp
-    646c6f49:	ret
-    646c6f4a:	nopw   0x0(%rax,%rax,1)
-    646c6f50:	pxor   %xmm0,%xmm0
-    646c6f54:	jmp    646c6f45 <internal_modf+0x85>
-    646c6f56:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c6f60 <pow>:
-    646c6f60:	push   %r12
-    646c6f62:	push   %rbp
-    646c6f63:	push   %rdi
-    646c6f64:	push   %rsi
-    646c6f65:	push   %rbx
-    646c6f66:	sub    $0x90,%rsp
-    646c6f6d:	movaps %xmm6,0x70(%rsp)
-    646c6f72:	movaps %xmm7,0x80(%rsp)
-    646c6f7a:	mov    $0x4000,%edx
-    646c6f7f:	movq   %xmm0,%rbx
-    646c6f84:	movq   %xmm0,%rdi
-    646c6f89:	movq   %xmm1,%rbp
-    646c6f8e:	shr    $0x20,%rbx
-    646c6f92:	mov    %ebx,%eax
-    646c6f94:	mov    %ebx,%ecx
-    646c6f96:	and    $0xfffff,%eax
-    646c6f9b:	and    $0x7ff00000,%ecx
-    646c6fa1:	or     %edi,%eax
-    646c6fa3:	mov    %ecx,%esi
-    646c6fa5:	or     %eax,%esi
-    646c6fa7:	je     646c6fb6 <pow+0x56>
-    646c6fa9:	test   %ecx,%ecx
-    646c6fab:	mov    $0x4400,%edx
-    646c6fb0:	jne    646c7101 <pow+0x1a1>
-    646c6fb6:	mov    %rbp,%rsi
-    646c6fb9:	movsd  0x242f(%rip),%xmm6        # 646c93f0 <.rdata+0x30>
-    646c6fc1:	shr    $0x20,%rsi
-    646c6fc5:	mov    %esi,%eax
-    646c6fc7:	mov    %esi,%ecx
-    646c6fc9:	and    $0xfffff,%eax
-    646c6fce:	and    $0x7ff00000,%ecx
-    646c6fd4:	or     %ebp,%eax
-    646c6fd6:	mov    %ecx,%r9d
-    646c6fd9:	or     %eax,%r9d
-    646c6fdc:	je     646c706b <pow+0x10b>
-    646c6fe2:	test   %ecx,%ecx
-    646c6fe4:	jne    646c7090 <pow+0x130>
-    646c6fea:	mov    $0x4400,%r8d
-    646c6ff0:	movsd  0x23f8(%rip),%xmm2        # 646c93f0 <.rdata+0x30>
-    646c6ff8:	movq   %rdi,%xmm4
-    646c6ffd:	ucomisd %xmm2,%xmm4
-    646c7001:	jp     646c7009 <pow+0xa9>
-    646c7003:	je     646c7458 <pow+0x4f8>
-    646c7009:	cmp    $0x100,%edx
-    646c700f:	je     646c70c0 <pow+0x160>
-    646c7015:	cmp    $0x4000,%edx
-    646c701b:	je     646c7130 <pow+0x1d0>
-    646c7021:	cmp    $0x500,%r8d
-    646c7028:	je     646c7180 <pow+0x220>
-    646c702e:	cmp    $0x500,%edx
-    646c7034:	jne    646c71a5 <pow+0x245>
-    646c703a:	test   %ebx,%ebx
-    646c703c:	js     646c7341 <pow+0x3e1>
-    646c7042:	mov    $0xffffffff,%edx
-    646c7047:	movq   %rbp,%xmm0
-    646c704c:	call   646c7810 <ldexp>
-    646c7051:	lea    0x68(%rsp),%rdx
-    646c7056:	call   646c6ec0 <internal_modf>
-    646c705b:	test   %esi,%esi
-    646c705d:	js     646c7162 <pow+0x202>
-    646c7063:	movsd  0x237d(%rip),%xmm6        # 646c93e8 <.rdata+0x28>
-    646c706b:	movapd %xmm6,%xmm0
-    646c706f:	movaps 0x80(%rsp),%xmm7
-    646c7077:	movaps 0x70(%rsp),%xmm6
-    646c707c:	add    $0x90,%rsp
-    646c7083:	pop    %rbx
-    646c7084:	pop    %rsi
-    646c7085:	pop    %rdi
-    646c7086:	pop    %rbp
-    646c7087:	pop    %r12
-    646c7089:	ret
-    646c708a:	nopw   0x0(%rax,%rax,1)
-    646c7090:	cmp    $0x7ff00000,%ecx
-    646c7096:	mov    $0x400,%r8d
-    646c709c:	jne    646c6ff0 <pow+0x90>
-    646c70a2:	test   %eax,%eax
-    646c70a4:	mov    $0x500,%r8d
-    646c70aa:	je     646c6ff0 <pow+0x90>
-    646c70b0:	movq   %rdi,%xmm5
-    646c70b5:	ucomisd %xmm6,%xmm5
-    646c70b9:	jp     646c70c0 <pow+0x160>
-    646c70bb:	je     646c706b <pow+0x10b>
-    646c70bd:	nopl   (%rax)
-    646c70c0:	test   %ebx,%ebx
-    646c70c2:	movsd  0x2306(%rip),%xmm6        # 646c93d0 <.rdata+0x10>
-    646c70ca:	js     646c7170 <pow+0x210>
-    646c70d0:	call   646c79d8 <_errno>
-    646c70d5:	movl   $0x21,(%rax)
-    646c70db:	movsd  %xmm6,0x20(%rsp)
-    646c70e1:	movq   %rbp,%xmm3
-    646c70e6:	movq   %rdi,%xmm2
-    646c70eb:	mov    $0x1,%ecx
-    646c70f0:	lea    0x22c9(%rip),%rdx        # 646c93c0 <.rdata>
-    646c70f7:	call   646c7c50 <__mingw_raise_matherr>
-    646c70fc:	jmp    646c706b <pow+0x10b>
-    646c7101:	cmp    $0x7ff00000,%ecx
-    646c7107:	mov    $0x400,%edx
-    646c710c:	jne    646c6fb6 <pow+0x56>
-    646c7112:	cmp    $0x1,%eax
-    646c7115:	sbb    %edx,%edx
-    646c7117:	and    $0x400,%edx
-    646c711d:	add    $0x100,%edx
-    646c7123:	jmp    646c6fb6 <pow+0x56>
-    646c7128:	nopl   0x0(%rax,%rax,1)
-    646c7130:	cmp    $0x500,%r8d
-    646c7137:	je     646c715a <pow+0x1fa>
-    646c7139:	test   %ebx,%ebx
-    646c713b:	js     646c7300 <pow+0x3a0>
-    646c7141:	mov    $0xffffffff,%edx
-    646c7146:	movq   %rbp,%xmm0
-    646c714b:	call   646c7810 <ldexp>
-    646c7150:	lea    0x68(%rsp),%rdx
-    646c7155:	call   646c6ec0 <internal_modf>
-    646c715a:	test   %esi,%esi
-    646c715c:	js     646c7063 <pow+0x103>
-    646c7162:	pxor   %xmm6,%xmm6
-    646c7166:	jmp    646c706b <pow+0x10b>
-    646c716b:	nopl   0x0(%rax,%rax,1)
-    646c7170:	movsd  0x2250(%rip),%xmm6        # 646c93c8 <.rdata+0x8>
-    646c7178:	jmp    646c70d0 <pow+0x170>
-    646c717d:	nopl   (%rax)
-    646c7180:	cmp    $0x500,%edx
-    646c7186:	je     646c705b <pow+0xfb>
-    646c718c:	test   %ebx,%ebx
-    646c718e:	js     646c7435 <pow+0x4d5>
-    646c7194:	movq   %rdi,%xmm5
-    646c7199:	ucomisd %xmm2,%xmm5
-    646c719d:	ja     646c705b <pow+0xfb>
-    646c71a3:	jmp    646c715a <pow+0x1fa>
-    646c71a5:	lea    0x68(%rsp),%rsi
-    646c71aa:	movq   %rbp,%xmm0
-    646c71af:	pxor   %xmm7,%xmm7
-    646c71b3:	mov    %rsi,%rdx
-    646c71b6:	call   646c6ec0 <internal_modf>
-    646c71bb:	ucomisd %xmm7,%xmm0
-    646c71bf:	jp     646c7281 <pow+0x321>
-    646c71c5:	jne    646c7281 <pow+0x321>
-    646c71cb:	movsd  0x68(%rsp),%xmm0
-    646c71d1:	movsd  0x2247(%rip),%xmm1        # 646c9420 <.rdata+0x60>
-    646c71d9:	ucomisd %xmm0,%xmm1
-    646c71dd:	jb     646c71ed <pow+0x28d>
-    646c71df:	ucomisd 0x2241(%rip),%xmm0        # 646c9428 <.rdata+0x68>
-    646c71e7:	jae    646c7493 <pow+0x533>
-    646c71ed:	lea    0x50(%rsp),%r12
-    646c71f2:	movq   %rdi,%xmm5
-    646c71f7:	andpd  0x2231(%rip),%xmm5        # 646c9430 <.rdata+0x70>
-    646c71ff:	movsd  %xmm5,0x30(%rsp)
-    646c7205:	lea    0x40(%rsp),%rdi
-    646c720a:	fldl   0x30(%rsp)
-    646c720e:	mov    %r12,%rcx
-    646c7211:	fstpt  0x40(%rsp)
-    646c7215:	mov    %rdi,%rdx
-    646c7218:	call   646c78e0 <log2l>
-    646c721d:	mov    %rdi,%rdx
-    646c7220:	mov    %r12,%rcx
-    646c7223:	fldt   0x50(%rsp)
-    646c7227:	mov    %rbp,0x30(%rsp)
-    646c722c:	fldl   0x30(%rsp)
-    646c7230:	fmulp  %st,%st(1)
-    646c7232:	fstpt  0x40(%rsp)
-    646c7236:	call   646c7740 <exp2l>
-    646c723b:	test   %ebx,%ebx
-    646c723d:	fldt   0x50(%rsp)
-    646c7241:	fstpl  0x38(%rsp)
-    646c7245:	movsd  0x38(%rsp),%xmm6
-    646c724b:	jns    646c706b <pow+0x10b>
-    646c7251:	mov    $0xffffffff,%edx
-    646c7256:	movq   %rbp,%xmm0
-    646c725b:	call   646c7810 <ldexp>
-    646c7260:	mov    %rsi,%rdx
-    646c7263:	call   646c6ec0 <internal_modf>
-    646c7268:	ucomisd %xmm7,%xmm0
-    646c726c:	jp     646c7274 <pow+0x314>
-    646c726e:	je     646c706b <pow+0x10b>
-    646c7274:	xorpd  0x2184(%rip),%xmm6        # 646c9400 <.rdata+0x40>
-    646c727c:	jmp    646c706b <pow+0x10b>
-    646c7281:	test   %ebx,%ebx
-    646c7283:	js     646c747b <pow+0x51b>
-    646c7289:	movq   %rbp,%xmm5
-    646c728e:	ucomisd 0x2182(%rip),%xmm5        # 646c9418 <.rdata+0x58>
-    646c7296:	jp     646c729e <pow+0x33e>
-    646c7298:	je     646c7461 <pow+0x501>
-    646c729e:	lea    0x50(%rsp),%rbx
-    646c72a3:	movq   %rdi,%xmm3
-    646c72a8:	andpd  0x2180(%rip),%xmm3        # 646c9430 <.rdata+0x70>
-    646c72b0:	movsd  %xmm3,0x30(%rsp)
-    646c72b6:	lea    0x40(%rsp),%rsi
-    646c72bb:	fldl   0x30(%rsp)
-    646c72bf:	mov    %rbx,%rcx
-    646c72c2:	fstpt  0x40(%rsp)
-    646c72c6:	mov    %rsi,%rdx
-    646c72c9:	call   646c78e0 <log2l>
-    646c72ce:	mov    %rsi,%rdx
-    646c72d1:	mov    %rbx,%rcx
-    646c72d4:	fldt   0x50(%rsp)
-    646c72d8:	mov    %rbp,0x30(%rsp)
-    646c72dd:	fldl   0x30(%rsp)
-    646c72e1:	fmulp  %st,%st(1)
-    646c72e3:	fstpt  0x40(%rsp)
-    646c72e7:	call   646c7740 <exp2l>
-    646c72ec:	fldt   0x50(%rsp)
-    646c72f0:	fstpl  0x38(%rsp)
-    646c72f4:	movsd  0x38(%rsp),%xmm6
-    646c72fa:	jmp    646c706b <pow+0x10b>
-    646c72ff:	nop
-    646c7300:	lea    0x68(%rsp),%rbx
-    646c7305:	movq   %rbp,%xmm0
-    646c730a:	pxor   %xmm7,%xmm7
-    646c730e:	mov    %rbx,%rdx
-    646c7311:	call   646c6ec0 <internal_modf>
-    646c7316:	ucomisd %xmm7,%xmm0
-    646c731a:	jp     646c7322 <pow+0x3c2>
-    646c731c:	je     646c7401 <pow+0x4a1>
-    646c7322:	test   %esi,%esi
-    646c7324:	jns    646c7162 <pow+0x202>
-    646c732a:	btc    $0x3f,%rdi
-    646c732f:	movq   %rdi,%xmm5
-    646c7334:	divsd  %xmm5,%xmm2
-    646c7338:	movapd %xmm2,%xmm6
-    646c733c:	jmp    646c706b <pow+0x10b>
-    646c7341:	lea    0x68(%rsp),%rbx
-    646c7346:	movq   %rbp,%xmm0
-    646c734b:	pxor   %xmm7,%xmm7
-    646c734f:	mov    %rbx,%rdx
-    646c7352:	call   646c6ec0 <internal_modf>
-    646c7357:	ucomisd %xmm7,%xmm0
-    646c735b:	jp     646c735f <pow+0x3ff>
-    646c735d:	je     646c7381 <pow+0x421>
-    646c735f:	test   %esi,%esi
-    646c7361:	movq   %rdi,%xmm6
-    646c7366:	xorpd  0x2092(%rip),%xmm6        # 646c9400 <.rdata+0x40>
-    646c736e:	jns    646c706b <pow+0x10b>
-    646c7374:	divsd  %xmm6,%xmm2
-    646c7378:	movapd %xmm2,%xmm6
-    646c737c:	jmp    646c706b <pow+0x10b>
-    646c7381:	mov    $0xffffffff,%edx
-    646c7386:	movq   %rbp,%xmm0
-    646c738b:	call   646c7810 <ldexp>
-    646c7390:	mov    %rbx,%rdx
-    646c7393:	call   646c6ec0 <internal_modf>
-    646c7398:	mov    $0x0,%edx
-    646c739d:	ucomisd %xmm7,%xmm0
-    646c73a1:	setnp  %al
-    646c73a4:	cmovne %edx,%eax
-    646c73a7:	mov    %esi,%edx
-    646c73a9:	shr    $0x1f,%edx
-    646c73ac:	test   %dl,%dl
-    646c73ae:	je     646c73b8 <pow+0x458>
-    646c73b0:	test   %al,%al
-    646c73b2:	jne    646c7162 <pow+0x202>
-    646c73b8:	mov    %esi,%edx
-    646c73ba:	mov    $0x1,%r8d
-    646c73c0:	not    %edx
-    646c73c2:	shr    $0x1f,%edx
-    646c73c5:	ucomisd %xmm7,%xmm0
-    646c73c9:	setp   %cl
-    646c73cc:	cmovne %r8d,%ecx
-    646c73d0:	test   %cl,%cl
-    646c73d2:	je     646c73d8 <pow+0x478>
-    646c73d4:	test   %dl,%dl
-    646c73d6:	jne    646c73f4 <pow+0x494>
-    646c73d8:	test   %al,%al
-    646c73da:	je     646c73e4 <pow+0x484>
-    646c73dc:	test   %dl,%dl
-    646c73de:	jne    646c7063 <pow+0x103>
-    646c73e4:	test   %esi,%esi
-    646c73e6:	js     646c741c <pow+0x4bc>
-    646c73e8:	ucomisd %xmm7,%xmm0
-    646c73ec:	jp     646c73f4 <pow+0x494>
-    646c73ee:	je     646c7063 <pow+0x103>
-    646c73f4:	movsd  0x1fe4(%rip),%xmm6        # 646c93e0 <.rdata+0x20>
-    646c73fc:	jmp    646c706b <pow+0x10b>
-    646c7401:	mov    $0xffffffff,%edx
-    646c7406:	movq   %rbp,%xmm0
-    646c740b:	call   646c7810 <ldexp>
-    646c7410:	mov    %rbx,%rdx
-    646c7413:	call   646c6ec0 <internal_modf>
-    646c7418:	test   %esi,%esi
-    646c741a:	js     646c73e8 <pow+0x488>
-    646c741c:	ucomisd %xmm7,%xmm0
-    646c7420:	jp     646c7428 <pow+0x4c8>
-    646c7422:	je     646c7162 <pow+0x202>
-    646c7428:	movsd  0x1fa8(%rip),%xmm6        # 646c93d8 <.rdata+0x18>
-    646c7430:	jmp    646c706b <pow+0x10b>
-    646c7435:	movq   %rdi,%xmm5
-    646c743a:	xorpd  0x1fbe(%rip),%xmm5        # 646c9400 <.rdata+0x40>
-    646c7442:	movq   %xmm5,%rax
-    646c7447:	movq   %rdi,%xmm5
-    646c744c:	ucomisd 0x1fbc(%rip),%xmm5        # 646c9410 <.rdata+0x50>
-    646c7454:	jp     646c74af <pow+0x54f>
-    646c7456:	jne    646c74af <pow+0x54f>
-    646c7458:	movapd %xmm2,%xmm6
-    646c745c:	jmp    646c706b <pow+0x10b>
-    646c7461:	mov    %rdi,0x30(%rsp)
-    646c7466:	fldl   0x30(%rsp)
-    646c746a:	fsqrt
-    646c746c:	fstpl  0x30(%rsp)
-    646c7470:	movsd  0x30(%rsp),%xmm6
-    646c7476:	jmp    646c706b <pow+0x10b>
-    646c747b:	call   646c79d8 <_errno>
-    646c7480:	movsd  0x1f40(%rip),%xmm6        # 646c93c8 <.rdata+0x8>
-    646c7488:	movl   $0x21,(%rax)
-    646c748e:	jmp    646c70db <pow+0x17b>
-    646c7493:	movq   %rbp,%xmm3
-    646c7498:	movq   %rdi,%xmm0
-    646c749d:	cvttsd2si %xmm3,%edx
-    646c74a1:	call   646c74c0 <__powi>
-    646c74a6:	movapd %xmm0,%xmm6
-    646c74aa:	jmp    646c706b <pow+0x10b>
-    646c74af:	mov    %rax,%rdi
-    646c74b2:	jmp    646c7194 <pow+0x234>
-    646c74b7:	nop
+    646c6b4a:	mov    $0x3,%ecx
+    646c6b4f:	movsd  0x2831(%rip),%xmm6        # 646c9388 <.rdata+0x8>
+    646c6b57:	movl   $0x22,(%rax)
+    646c6b5d:	lea    0x281c(%rip),%rdx        # 646c9380 <.rdata>
+    646c6b64:	pxor   %xmm3,%xmm3
+    646c6b68:	movsd  %xmm6,0x20(%rsp)
+    646c6b6e:	call   646c7960 <__mingw_raise_matherr>
+    646c6b73:	movapd %xmm6,%xmm0
+    646c6b77:	movaps 0x60(%rsp),%xmm6
+    646c6b7c:	add    $0x70,%rsp
+    646c6b80:	pop    %rbx
+    646c6b81:	ret
+    646c6b82:	test   %edx,%edx
+    646c6b84:	movsd  0x280c(%rip),%xmm0        # 646c9398 <.rdata+0x18>
+    646c6b8c:	jns    646c6b17 <log+0x67>
+    646c6b8e:	call   646c76e8 <_errno>
+    646c6b93:	movq   %rbx,%xmm2
+    646c6b98:	mov    $0x1,%ecx
+    646c6b9d:	movsd  0x27eb(%rip),%xmm6        # 646c9390 <.rdata+0x10>
+    646c6ba5:	movl   $0x21,(%rax)
+    646c6bab:	lea    0x27ce(%rip),%rdx        # 646c9380 <.rdata>
+    646c6bb2:	pxor   %xmm3,%xmm3
+    646c6bb6:	movsd  %xmm6,0x20(%rsp)
+    646c6bbc:	call   646c7960 <__mingw_raise_matherr>
+    646c6bc1:	movapd %xmm6,%xmm0
+    646c6bc5:	movaps 0x60(%rsp),%xmm6
+    646c6bca:	add    $0x70,%rsp
+    646c6bce:	pop    %rbx
+    646c6bcf:	ret
+
+00000000646c6bd0 <internal_modf>:
+    646c6bd0:	sub    $0x18,%rsp
+    646c6bd4:	movsd  %xmm0,0x8(%rsp)
+    646c6bda:	fldl   0x8(%rsp)
+    646c6bde:	push   %rax
+    646c6bdf:	sub    $0x8,%rsp
+    646c6be3:	fnstcw 0x4(%rsp)
+    646c6be7:	movzwl 0x4(%rsp),%eax
+    646c6bec:	or     $0xc,%ah
+    646c6bef:	mov    %ax,(%rsp)
+    646c6bf3:	fldcw  (%rsp)
+    646c6bf6:	frndint
+    646c6bf8:	fldcw  0x4(%rsp)
+    646c6bfc:	add    $0x8,%rsp
+    646c6c00:	pop    %rax
+    646c6c01:	movq   %xmm0,%rax
+    646c6c06:	fstpl  0x8(%rsp)
+    646c6c0a:	movsd  0x8(%rsp),%xmm1
+    646c6c10:	shr    $0x20,%rax
+    646c6c14:	mov    %eax,%ecx
+    646c6c16:	movsd  %xmm1,(%rdx)
+    646c6c1a:	movq   %xmm0,%rdx
+    646c6c1f:	and    $0x7ff00000,%eax
+    646c6c24:	and    $0xfffff,%ecx
+    646c6c2a:	or     %edx,%ecx
+    646c6c2c:	mov    %ecx,%edx
+    646c6c2e:	or     %eax,%edx
+    646c6c30:	sete   %dl
+    646c6c33:	test   %eax,%eax
+    646c6c35:	sete   %r8b
+    646c6c39:	or     %r8d,%edx
+    646c6c3c:	xor    $0x1,%edx
+    646c6c3f:	cmp    $0x7ff00000,%eax
+    646c6c44:	sete   %al
+    646c6c47:	test   %al,%dl
+    646c6c49:	je     646c6c4f <internal_modf+0x7f>
+    646c6c4b:	test   %ecx,%ecx
+    646c6c4d:	je     646c6c60 <internal_modf+0x90>
+    646c6c4f:	subsd  0x8(%rsp),%xmm0
+    646c6c55:	add    $0x18,%rsp
+    646c6c59:	ret
+    646c6c5a:	nopw   0x0(%rax,%rax,1)
+    646c6c60:	pxor   %xmm0,%xmm0
+    646c6c64:	jmp    646c6c55 <internal_modf+0x85>
+    646c6c66:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c6c70 <pow>:
+    646c6c70:	push   %r12
+    646c6c72:	push   %rbp
+    646c6c73:	push   %rdi
+    646c6c74:	push   %rsi
+    646c6c75:	push   %rbx
+    646c6c76:	sub    $0x90,%rsp
+    646c6c7d:	movaps %xmm6,0x70(%rsp)
+    646c6c82:	movaps %xmm7,0x80(%rsp)
+    646c6c8a:	mov    $0x4000,%edx
+    646c6c8f:	movq   %xmm0,%rbx
+    646c6c94:	movq   %xmm0,%rdi
+    646c6c99:	movq   %xmm1,%rbp
+    646c6c9e:	shr    $0x20,%rbx
+    646c6ca2:	mov    %ebx,%eax
+    646c6ca4:	mov    %ebx,%ecx
+    646c6ca6:	and    $0xfffff,%eax
+    646c6cab:	and    $0x7ff00000,%ecx
+    646c6cb1:	or     %edi,%eax
+    646c6cb3:	mov    %ecx,%esi
+    646c6cb5:	or     %eax,%esi
+    646c6cb7:	je     646c6cc6 <pow+0x56>
+    646c6cb9:	test   %ecx,%ecx
+    646c6cbb:	mov    $0x4400,%edx
+    646c6cc0:	jne    646c6e11 <pow+0x1a1>
+    646c6cc6:	mov    %rbp,%rsi
+    646c6cc9:	movsd  0x26ff(%rip),%xmm6        # 646c93d0 <.rdata+0x30>
+    646c6cd1:	shr    $0x20,%rsi
+    646c6cd5:	mov    %esi,%eax
+    646c6cd7:	mov    %esi,%ecx
+    646c6cd9:	and    $0xfffff,%eax
+    646c6cde:	and    $0x7ff00000,%ecx
+    646c6ce4:	or     %ebp,%eax
+    646c6ce6:	mov    %ecx,%r9d
+    646c6ce9:	or     %eax,%r9d
+    646c6cec:	je     646c6d7b <pow+0x10b>
+    646c6cf2:	test   %ecx,%ecx
+    646c6cf4:	jne    646c6da0 <pow+0x130>
+    646c6cfa:	mov    $0x4400,%r8d
+    646c6d00:	movsd  0x26c8(%rip),%xmm2        # 646c93d0 <.rdata+0x30>
+    646c6d08:	movq   %rdi,%xmm4
+    646c6d0d:	ucomisd %xmm2,%xmm4
+    646c6d11:	jp     646c6d19 <pow+0xa9>
+    646c6d13:	je     646c7168 <pow+0x4f8>
+    646c6d19:	cmp    $0x100,%edx
+    646c6d1f:	je     646c6dd0 <pow+0x160>
+    646c6d25:	cmp    $0x4000,%edx
+    646c6d2b:	je     646c6e40 <pow+0x1d0>
+    646c6d31:	cmp    $0x500,%r8d
+    646c6d38:	je     646c6e90 <pow+0x220>
+    646c6d3e:	cmp    $0x500,%edx
+    646c6d44:	jne    646c6eb5 <pow+0x245>
+    646c6d4a:	test   %ebx,%ebx
+    646c6d4c:	js     646c7051 <pow+0x3e1>
+    646c6d52:	mov    $0xffffffff,%edx
+    646c6d57:	movq   %rbp,%xmm0
+    646c6d5c:	call   646c7520 <ldexp>
+    646c6d61:	lea    0x68(%rsp),%rdx
+    646c6d66:	call   646c6bd0 <internal_modf>
+    646c6d6b:	test   %esi,%esi
+    646c6d6d:	js     646c6e72 <pow+0x202>
+    646c6d73:	movsd  0x264d(%rip),%xmm6        # 646c93c8 <.rdata+0x28>
+    646c6d7b:	movapd %xmm6,%xmm0
+    646c6d7f:	movaps 0x80(%rsp),%xmm7
+    646c6d87:	movaps 0x70(%rsp),%xmm6
+    646c6d8c:	add    $0x90,%rsp
+    646c6d93:	pop    %rbx
+    646c6d94:	pop    %rsi
+    646c6d95:	pop    %rdi
+    646c6d96:	pop    %rbp
+    646c6d97:	pop    %r12
+    646c6d99:	ret
+    646c6d9a:	nopw   0x0(%rax,%rax,1)
+    646c6da0:	cmp    $0x7ff00000,%ecx
+    646c6da6:	mov    $0x400,%r8d
+    646c6dac:	jne    646c6d00 <pow+0x90>
+    646c6db2:	test   %eax,%eax
+    646c6db4:	mov    $0x500,%r8d
+    646c6dba:	je     646c6d00 <pow+0x90>
+    646c6dc0:	movq   %rdi,%xmm5
+    646c6dc5:	ucomisd %xmm6,%xmm5
+    646c6dc9:	jp     646c6dd0 <pow+0x160>
+    646c6dcb:	je     646c6d7b <pow+0x10b>
+    646c6dcd:	nopl   (%rax)
+    646c6dd0:	test   %ebx,%ebx
+    646c6dd2:	movsd  0x25d6(%rip),%xmm6        # 646c93b0 <.rdata+0x10>
+    646c6dda:	js     646c6e80 <pow+0x210>
+    646c6de0:	call   646c76e8 <_errno>
+    646c6de5:	movl   $0x21,(%rax)
+    646c6deb:	movsd  %xmm6,0x20(%rsp)
+    646c6df1:	movq   %rbp,%xmm3
+    646c6df6:	movq   %rdi,%xmm2
+    646c6dfb:	mov    $0x1,%ecx
+    646c6e00:	lea    0x2599(%rip),%rdx        # 646c93a0 <.rdata>
+    646c6e07:	call   646c7960 <__mingw_raise_matherr>
+    646c6e0c:	jmp    646c6d7b <pow+0x10b>
+    646c6e11:	cmp    $0x7ff00000,%ecx
+    646c6e17:	mov    $0x400,%edx
+    646c6e1c:	jne    646c6cc6 <pow+0x56>
+    646c6e22:	cmp    $0x1,%eax
+    646c6e25:	sbb    %edx,%edx
+    646c6e27:	and    $0x400,%edx
+    646c6e2d:	add    $0x100,%edx
+    646c6e33:	jmp    646c6cc6 <pow+0x56>
+    646c6e38:	nopl   0x0(%rax,%rax,1)
+    646c6e40:	cmp    $0x500,%r8d
+    646c6e47:	je     646c6e6a <pow+0x1fa>
+    646c6e49:	test   %ebx,%ebx
+    646c6e4b:	js     646c7010 <pow+0x3a0>
+    646c6e51:	mov    $0xffffffff,%edx
+    646c6e56:	movq   %rbp,%xmm0
+    646c6e5b:	call   646c7520 <ldexp>
+    646c6e60:	lea    0x68(%rsp),%rdx
+    646c6e65:	call   646c6bd0 <internal_modf>
+    646c6e6a:	test   %esi,%esi
+    646c6e6c:	js     646c6d73 <pow+0x103>
+    646c6e72:	pxor   %xmm6,%xmm6
+    646c6e76:	jmp    646c6d7b <pow+0x10b>
+    646c6e7b:	nopl   0x0(%rax,%rax,1)
+    646c6e80:	movsd  0x2520(%rip),%xmm6        # 646c93a8 <.rdata+0x8>
+    646c6e88:	jmp    646c6de0 <pow+0x170>
+    646c6e8d:	nopl   (%rax)
+    646c6e90:	cmp    $0x500,%edx
+    646c6e96:	je     646c6d6b <pow+0xfb>
+    646c6e9c:	test   %ebx,%ebx
+    646c6e9e:	js     646c7145 <pow+0x4d5>
+    646c6ea4:	movq   %rdi,%xmm5
+    646c6ea9:	ucomisd %xmm2,%xmm5
+    646c6ead:	ja     646c6d6b <pow+0xfb>
+    646c6eb3:	jmp    646c6e6a <pow+0x1fa>
+    646c6eb5:	lea    0x68(%rsp),%rsi
+    646c6eba:	movq   %rbp,%xmm0
+    646c6ebf:	pxor   %xmm7,%xmm7
+    646c6ec3:	mov    %rsi,%rdx
+    646c6ec6:	call   646c6bd0 <internal_modf>
+    646c6ecb:	ucomisd %xmm7,%xmm0
+    646c6ecf:	jp     646c6f91 <pow+0x321>
+    646c6ed5:	jne    646c6f91 <pow+0x321>
+    646c6edb:	movsd  0x68(%rsp),%xmm0
+    646c6ee1:	movsd  0x2517(%rip),%xmm1        # 646c9400 <.rdata+0x60>
+    646c6ee9:	ucomisd %xmm0,%xmm1
+    646c6eed:	jb     646c6efd <pow+0x28d>
+    646c6eef:	ucomisd 0x2511(%rip),%xmm0        # 646c9408 <.rdata+0x68>
+    646c6ef7:	jae    646c71a3 <pow+0x533>
+    646c6efd:	lea    0x50(%rsp),%r12
+    646c6f02:	movq   %rdi,%xmm5
+    646c6f07:	andpd  0x2501(%rip),%xmm5        # 646c9410 <.rdata+0x70>
+    646c6f0f:	movsd  %xmm5,0x30(%rsp)
+    646c6f15:	lea    0x40(%rsp),%rdi
+    646c6f1a:	fldl   0x30(%rsp)
+    646c6f1e:	mov    %r12,%rcx
+    646c6f21:	fstpt  0x40(%rsp)
+    646c6f25:	mov    %rdi,%rdx
+    646c6f28:	call   646c75f0 <log2l>
+    646c6f2d:	mov    %rdi,%rdx
+    646c6f30:	mov    %r12,%rcx
+    646c6f33:	fldt   0x50(%rsp)
+    646c6f37:	mov    %rbp,0x30(%rsp)
+    646c6f3c:	fldl   0x30(%rsp)
+    646c6f40:	fmulp  %st,%st(1)
+    646c6f42:	fstpt  0x40(%rsp)
+    646c6f46:	call   646c7450 <exp2l>
+    646c6f4b:	test   %ebx,%ebx
+    646c6f4d:	fldt   0x50(%rsp)
+    646c6f51:	fstpl  0x38(%rsp)
+    646c6f55:	movsd  0x38(%rsp),%xmm6
+    646c6f5b:	jns    646c6d7b <pow+0x10b>
+    646c6f61:	mov    $0xffffffff,%edx
+    646c6f66:	movq   %rbp,%xmm0
+    646c6f6b:	call   646c7520 <ldexp>
+    646c6f70:	mov    %rsi,%rdx
+    646c6f73:	call   646c6bd0 <internal_modf>
+    646c6f78:	ucomisd %xmm7,%xmm0
+    646c6f7c:	jp     646c6f84 <pow+0x314>
+    646c6f7e:	je     646c6d7b <pow+0x10b>
+    646c6f84:	xorpd  0x2454(%rip),%xmm6        # 646c93e0 <.rdata+0x40>
+    646c6f8c:	jmp    646c6d7b <pow+0x10b>
+    646c6f91:	test   %ebx,%ebx
+    646c6f93:	js     646c718b <pow+0x51b>
+    646c6f99:	movq   %rbp,%xmm5
+    646c6f9e:	ucomisd 0x2452(%rip),%xmm5        # 646c93f8 <.rdata+0x58>
+    646c6fa6:	jp     646c6fae <pow+0x33e>
+    646c6fa8:	je     646c7171 <pow+0x501>
+    646c6fae:	lea    0x50(%rsp),%rbx
+    646c6fb3:	movq   %rdi,%xmm3
+    646c6fb8:	andpd  0x2450(%rip),%xmm3        # 646c9410 <.rdata+0x70>
+    646c6fc0:	movsd  %xmm3,0x30(%rsp)
+    646c6fc6:	lea    0x40(%rsp),%rsi
+    646c6fcb:	fldl   0x30(%rsp)
+    646c6fcf:	mov    %rbx,%rcx
+    646c6fd2:	fstpt  0x40(%rsp)
+    646c6fd6:	mov    %rsi,%rdx
+    646c6fd9:	call   646c75f0 <log2l>
+    646c6fde:	mov    %rsi,%rdx
+    646c6fe1:	mov    %rbx,%rcx
+    646c6fe4:	fldt   0x50(%rsp)
+    646c6fe8:	mov    %rbp,0x30(%rsp)
+    646c6fed:	fldl   0x30(%rsp)
+    646c6ff1:	fmulp  %st,%st(1)
+    646c6ff3:	fstpt  0x40(%rsp)
+    646c6ff7:	call   646c7450 <exp2l>
+    646c6ffc:	fldt   0x50(%rsp)
+    646c7000:	fstpl  0x38(%rsp)
+    646c7004:	movsd  0x38(%rsp),%xmm6
+    646c700a:	jmp    646c6d7b <pow+0x10b>
+    646c700f:	nop
+    646c7010:	lea    0x68(%rsp),%rbx
+    646c7015:	movq   %rbp,%xmm0
+    646c701a:	pxor   %xmm7,%xmm7
+    646c701e:	mov    %rbx,%rdx
+    646c7021:	call   646c6bd0 <internal_modf>
+    646c7026:	ucomisd %xmm7,%xmm0
+    646c702a:	jp     646c7032 <pow+0x3c2>
+    646c702c:	je     646c7111 <pow+0x4a1>
+    646c7032:	test   %esi,%esi
+    646c7034:	jns    646c6e72 <pow+0x202>
+    646c703a:	btc    $0x3f,%rdi
+    646c703f:	movq   %rdi,%xmm5
+    646c7044:	divsd  %xmm5,%xmm2
+    646c7048:	movapd %xmm2,%xmm6
+    646c704c:	jmp    646c6d7b <pow+0x10b>
+    646c7051:	lea    0x68(%rsp),%rbx
+    646c7056:	movq   %rbp,%xmm0
+    646c705b:	pxor   %xmm7,%xmm7
+    646c705f:	mov    %rbx,%rdx
+    646c7062:	call   646c6bd0 <internal_modf>
+    646c7067:	ucomisd %xmm7,%xmm0
+    646c706b:	jp     646c706f <pow+0x3ff>
+    646c706d:	je     646c7091 <pow+0x421>
+    646c706f:	test   %esi,%esi
+    646c7071:	movq   %rdi,%xmm6
+    646c7076:	xorpd  0x2362(%rip),%xmm6        # 646c93e0 <.rdata+0x40>
+    646c707e:	jns    646c6d7b <pow+0x10b>
+    646c7084:	divsd  %xmm6,%xmm2
+    646c7088:	movapd %xmm2,%xmm6
+    646c708c:	jmp    646c6d7b <pow+0x10b>
+    646c7091:	mov    $0xffffffff,%edx
+    646c7096:	movq   %rbp,%xmm0
+    646c709b:	call   646c7520 <ldexp>
+    646c70a0:	mov    %rbx,%rdx
+    646c70a3:	call   646c6bd0 <internal_modf>
+    646c70a8:	mov    $0x0,%edx
+    646c70ad:	ucomisd %xmm7,%xmm0
+    646c70b1:	setnp  %al
+    646c70b4:	cmovne %edx,%eax
+    646c70b7:	mov    %esi,%edx
+    646c70b9:	shr    $0x1f,%edx
+    646c70bc:	test   %dl,%dl
+    646c70be:	je     646c70c8 <pow+0x458>
+    646c70c0:	test   %al,%al
+    646c70c2:	jne    646c6e72 <pow+0x202>
+    646c70c8:	mov    %esi,%edx
+    646c70ca:	mov    $0x1,%r8d
+    646c70d0:	not    %edx
+    646c70d2:	shr    $0x1f,%edx
+    646c70d5:	ucomisd %xmm7,%xmm0
+    646c70d9:	setp   %cl
+    646c70dc:	cmovne %r8d,%ecx
+    646c70e0:	test   %cl,%cl
+    646c70e2:	je     646c70e8 <pow+0x478>
+    646c70e4:	test   %dl,%dl
+    646c70e6:	jne    646c7104 <pow+0x494>
+    646c70e8:	test   %al,%al
+    646c70ea:	je     646c70f4 <pow+0x484>
+    646c70ec:	test   %dl,%dl
+    646c70ee:	jne    646c6d73 <pow+0x103>
+    646c70f4:	test   %esi,%esi
+    646c70f6:	js     646c712c <pow+0x4bc>
+    646c70f8:	ucomisd %xmm7,%xmm0
+    646c70fc:	jp     646c7104 <pow+0x494>
+    646c70fe:	je     646c6d73 <pow+0x103>
+    646c7104:	movsd  0x22b4(%rip),%xmm6        # 646c93c0 <.rdata+0x20>
+    646c710c:	jmp    646c6d7b <pow+0x10b>
+    646c7111:	mov    $0xffffffff,%edx
+    646c7116:	movq   %rbp,%xmm0
+    646c711b:	call   646c7520 <ldexp>
+    646c7120:	mov    %rbx,%rdx
+    646c7123:	call   646c6bd0 <internal_modf>
+    646c7128:	test   %esi,%esi
+    646c712a:	js     646c70f8 <pow+0x488>
+    646c712c:	ucomisd %xmm7,%xmm0
+    646c7130:	jp     646c7138 <pow+0x4c8>
+    646c7132:	je     646c6e72 <pow+0x202>
+    646c7138:	movsd  0x2278(%rip),%xmm6        # 646c93b8 <.rdata+0x18>
+    646c7140:	jmp    646c6d7b <pow+0x10b>
+    646c7145:	movq   %rdi,%xmm5
+    646c714a:	xorpd  0x228e(%rip),%xmm5        # 646c93e0 <.rdata+0x40>
+    646c7152:	movq   %xmm5,%rax
+    646c7157:	movq   %rdi,%xmm5
+    646c715c:	ucomisd 0x228c(%rip),%xmm5        # 646c93f0 <.rdata+0x50>
+    646c7164:	jp     646c71bf <pow+0x54f>
+    646c7166:	jne    646c71bf <pow+0x54f>
+    646c7168:	movapd %xmm2,%xmm6
+    646c716c:	jmp    646c6d7b <pow+0x10b>
+    646c7171:	mov    %rdi,0x30(%rsp)
+    646c7176:	fldl   0x30(%rsp)
+    646c717a:	fsqrt
+    646c717c:	fstpl  0x30(%rsp)
+    646c7180:	movsd  0x30(%rsp),%xmm6
+    646c7186:	jmp    646c6d7b <pow+0x10b>
+    646c718b:	call   646c76e8 <_errno>
+    646c7190:	movsd  0x2210(%rip),%xmm6        # 646c93a8 <.rdata+0x8>
+    646c7198:	movl   $0x21,(%rax)
+    646c719e:	jmp    646c6deb <pow+0x17b>
+    646c71a3:	movq   %rbp,%xmm3
+    646c71a8:	movq   %rdi,%xmm0
+    646c71ad:	cvttsd2si %xmm3,%edx
+    646c71b1:	call   646c71d0 <__powi>
+    646c71b6:	movapd %xmm0,%xmm6
+    646c71ba:	jmp    646c6d7b <pow+0x10b>
+    646c71bf:	mov    %rax,%rdi
+    646c71c2:	jmp    646c6ea4 <pow+0x234>
+    646c71c7:	nop
+    646c71c8:	nop
+    646c71c9:	nop
+    646c71ca:	nop
+    646c71cb:	nop
+    646c71cc:	nop
+    646c71cd:	nop
+    646c71ce:	nop
+    646c71cf:	nop
+
+00000000646c71d0 <__powi>:
+    646c71d0:	sub    $0x58,%rsp
+    646c71d4:	movaps %xmm6,0x40(%rsp)
+    646c71d9:	movsd  0x2257(%rip),%xmm1        # 646c9438 <.rdata+0x18>
+    646c71e1:	mov    $0x0,%r10d
+    646c71e7:	movq   %xmm0,%r8
+    646c71ec:	movq   %xmm0,%rax
+    646c71f1:	shr    $0x20,%r8
+    646c71f5:	mov    %r8d,%ecx
+    646c71f8:	mov    %r8d,%r9d
+    646c71fb:	and    $0xfffff,%ecx
+    646c7201:	and    $0x7ff00000,%r9d
+    646c7208:	or     %eax,%ecx
+    646c720a:	ucomisd %xmm1,%xmm0
+    646c720e:	mov    %r9d,%r11d
+    646c7211:	setnp  %al
+    646c7214:	cmovne %r10d,%eax
+    646c7218:	test   %edx,%edx
+    646c721a:	sete   %r10b
+    646c721e:	or     %r10d,%eax
+    646c7221:	or     %ecx,%r11d
+    646c7224:	jne    646c7260 <__powi+0x90>
+    646c7226:	test   %al,%al
+    646c7228:	movapd %xmm1,%xmm6
+    646c722c:	jne    646c7250 <__powi+0x80>
+    646c722e:	mov    %edx,%eax
+    646c7230:	and    $0x1,%eax
+    646c7233:	test   %edx,%edx
+    646c7235:	js     646c7325 <__powi+0x155>
+    646c723b:	test   %eax,%eax
+    646c723d:	pxor   %xmm6,%xmm6
+    646c7241:	je     646c7250 <__powi+0x80>
+    646c7243:	test   %r8d,%r8d
+    646c7246:	jns    646c7250 <__powi+0x80>
+    646c7248:	movsd  0x21f0(%rip),%xmm6        # 646c9440 <.rdata+0x20>
+    646c7250:	movapd %xmm6,%xmm0
+    646c7254:	movaps 0x40(%rsp),%xmm6
+    646c7259:	add    $0x58,%rsp
+    646c725d:	ret
+    646c725e:	xchg   %ax,%ax
+    646c7260:	test   %r9d,%r9d
+    646c7263:	jne    646c72d0 <__powi+0x100>
+    646c7265:	test   %al,%al
+    646c7267:	movapd %xmm1,%xmm6
+    646c726b:	jne    646c7250 <__powi+0x80>
+    646c726d:	mov    %edx,%eax
+    646c726f:	movapd %xmm0,%xmm6
+    646c7273:	andpd  0x21e5(%rip),%xmm6        # 646c9460 <.rdata+0x40>
+    646c727b:	and    $0x1,%eax
+    646c727e:	test   %edx,%edx
+    646c7280:	js     646c7312 <__powi+0x142>
+    646c7286:	cmp    $0x1,%edx
+    646c7289:	je     646c72b1 <__powi+0xe1>
+    646c728b:	test   $0x1,%dl
+    646c728e:	jne    646c73c0 <__powi+0x1f0>
+    646c7294:	movapd %xmm6,%xmm0
+    646c7298:	shr    %edx
+    646c729a:	movapd %xmm1,%xmm6
+    646c729e:	xchg   %ax,%ax
+    646c72a0:	mulsd  %xmm0,%xmm0
+    646c72a4:	test   $0x1,%dl
+    646c72a7:	je     646c72ad <__powi+0xdd>
+    646c72a9:	mulsd  %xmm0,%xmm6
+    646c72ad:	shr    %edx
+    646c72af:	jne    646c72a0 <__powi+0xd0>
+    646c72b1:	shr    $0x1f,%r8d
+    646c72b5:	test   %r8b,%r8b
+    646c72b8:	je     646c7250 <__powi+0x80>
+    646c72ba:	test   %eax,%eax
+    646c72bc:	je     646c7250 <__powi+0x80>
+    646c72be:	xorpd  0x21aa(%rip),%xmm6        # 646c9470 <.rdata+0x50>
+    646c72c6:	jmp    646c7250 <__powi+0x80>
+    646c72c8:	nopl   0x0(%rax,%rax,1)
+    646c72d0:	cmp    $0x7ff00000,%r9d
+    646c72d7:	jne    646c7265 <__powi+0x95>
+    646c72d9:	test   %ecx,%ecx
+    646c72db:	jne    646c7350 <__powi+0x180>
+    646c72dd:	mov    %edx,%r9d
+    646c72e0:	movapd %xmm1,%xmm6
+    646c72e4:	and    $0x1,%r9d
+    646c72e8:	test   %al,%al
+    646c72ea:	jne    646c7250 <__powi+0x80>
+    646c72f0:	test   %r8d,%r8d
+    646c72f3:	js     646c73e0 <__powi+0x210>
+    646c72f9:	test   %edx,%edx
+    646c72fb:	movsd  0x2145(%rip),%xmm6        # 646c9448 <.rdata+0x28>
+    646c7303:	jns    646c7250 <__powi+0x80>
+    646c7309:	pxor   %xmm6,%xmm6
+    646c730d:	jmp    646c7250 <__powi+0x80>
+    646c7312:	movapd %xmm1,%xmm4
+    646c7316:	neg    %edx
+    646c7318:	divsd  %xmm6,%xmm4
+    646c731c:	movapd %xmm4,%xmm6
+    646c7320:	jmp    646c7286 <__powi+0xb6>
+    646c7325:	test   %eax,%eax
+    646c7327:	movsd  0x2119(%rip),%xmm6        # 646c9448 <.rdata+0x28>
+    646c732f:	je     646c7250 <__powi+0x80>
+    646c7335:	test   %r8d,%r8d
+    646c7338:	jns    646c7250 <__powi+0x80>
+    646c733e:	movsd  0x210a(%rip),%xmm6        # 646c9450 <.rdata+0x30>
+    646c7346:	jmp    646c7250 <__powi+0x80>
+    646c734b:	nopl   0x0(%rax,%rax,1)
+    646c7350:	test   %al,%al
+    646c7352:	movapd %xmm1,%xmm6
+    646c7356:	jne    646c7250 <__powi+0x80>
+    646c735c:	test   %r8d,%r8d
+    646c735f:	movsd  0x20c9(%rip),%xmm6        # 646c9430 <.rdata+0x10>
+    646c7367:	js     646c73d0 <__powi+0x200>
+    646c7369:	mov    %edx,0x3c(%rsp)
+    646c736d:	movsd  %xmm0,0x30(%rsp)
+    646c7373:	call   646c76e8 <_errno>
+    646c7378:	mov    0x3c(%rsp),%edx
+    646c737c:	pxor   %xmm3,%xmm3
+    646c7380:	mov    $0x1,%ecx
+    646c7385:	movsd  0x30(%rsp),%xmm0
+    646c738b:	movl   $0x21,(%rax)
+    646c7391:	movsd  %xmm6,0x20(%rsp)
+    646c7397:	movapd %xmm0,%xmm2
+    646c739b:	cvtsi2sd %edx,%xmm3
+    646c739f:	lea    0x207a(%rip),%rdx        # 646c9420 <.rdata>
+    646c73a6:	call   646c7960 <__mingw_raise_matherr>
+    646c73ab:	movapd %xmm6,%xmm0
+    646c73af:	movaps 0x40(%rsp),%xmm6
+    646c73b4:	add    $0x58,%rsp
+    646c73b8:	ret
+    646c73b9:	nopl   0x0(%rax)
+    646c73c0:	movapd %xmm6,%xmm1
+    646c73c4:	jmp    646c7294 <__powi+0xc4>
+    646c73c9:	nopl   0x0(%rax)
+    646c73d0:	movsd  0x2050(%rip),%xmm6        # 646c9428 <.rdata+0x8>
+    646c73d8:	jmp    646c7369 <__powi+0x199>
+    646c73da:	nopw   0x0(%rax,%rax,1)
+    646c73e0:	mov    %edx,%eax
+    646c73e2:	not    %eax
+    646c73e4:	mov    %eax,%ecx
+    646c73e6:	and    $0x1,%ecx
+    646c73e9:	test   %edx,%edx
+    646c73eb:	jns    646c73f9 <__powi+0x229>
+    646c73ed:	test   %cl,%cl
+    646c73ef:	pxor   %xmm6,%xmm6
+    646c73f3:	jne    646c7250 <__powi+0x80>
+    646c73f9:	shr    $0x1f,%eax
+    646c73fc:	test   $0x1,%dl
+    646c73ff:	je     646c7411 <__powi+0x241>
+    646c7401:	test   %al,%al
+    646c7403:	movsd  0x2045(%rip),%xmm6        # 646c9450 <.rdata+0x30>
+    646c740b:	jne    646c7250 <__powi+0x80>
+    646c7411:	test   %cl,%cl
+    646c7413:	je     646c7425 <__powi+0x255>
+    646c7415:	test   %al,%al
+    646c7417:	movsd  0x2029(%rip),%xmm6        # 646c9448 <.rdata+0x28>
+    646c741f:	jne    646c7250 <__powi+0x80>
+    646c7425:	test   %edx,%edx
+    646c7427:	js     646c7440 <__powi+0x270>
+    646c7429:	and    $0x1,%dl
+    646c742c:	jne    646c733e <__powi+0x16e>
+    646c7432:	movsd  0x200e(%rip),%xmm6        # 646c9448 <.rdata+0x28>
+    646c743a:	jmp    646c7250 <__powi+0x80>
+    646c743f:	nop
+    646c7440:	test   %r9d,%r9d
+    646c7443:	jne    646c7248 <__powi+0x78>
+    646c7449:	jmp    646c7309 <__powi+0x139>
+    646c744e:	nop
+    646c744f:	nop
+
+00000000646c7450 <exp2l>:
+    646c7450:	fldt   (%rdx)
+    646c7452:	fxam
+    646c7454:	fstsw  %ax
+    646c7457:	mov    $0x45,%dh
+    646c7459:	and    %ah,%dh
+    646c745b:	cmp    $0x5,%dh
+    646c745e:	je     646c749f <exp2l+0x4f>
+    646c7460:	fld    %st(0)
+    646c7462:	sub    $0x8,%rsp
+    646c7466:	fnstcw 0x4(%rsp)
+    646c746a:	movzwl 0x4(%rsp),%eax
+    646c746f:	or     $0xc,%ah
+    646c7472:	mov    %ax,(%rsp)
+    646c7476:	fldcw  (%rsp)
+    646c7479:	frndint
+    646c747b:	fldcw  0x4(%rsp)
+    646c747f:	add    $0x8,%rsp
+    646c7483:	fsubr  %st,%st(1)
+    646c7485:	fxch   %st(1)
+    646c7487:	f2xm1
+    646c7489:	fld1
+    646c748b:	faddp  %st,%st(1)
+    646c748d:	fscale
+    646c748f:	fstp   %st(1)
+    646c7491:	mov    %rcx,%rax
+    646c7494:	movq   $0x0,0x8(%rcx)
+    646c749c:	fstpt  (%rcx)
+    646c749e:	ret
+    646c749f:	test   $0x200,%eax
+    646c74a4:	je     646c74aa <exp2l+0x5a>
+    646c74a6:	fstp   %st(0)
+    646c74a8:	fldz
+    646c74aa:	mov    %rcx,%rax
+    646c74ad:	movq   $0x0,0x8(%rcx)
+    646c74b5:	fstpt  (%rcx)
+    646c74b7:	ret
     646c74b8:	nop
     646c74b9:	nop
     646c74ba:	nop
     646c74bb:	nop
     646c74bc:	nop
     646c74bd:	nop
     646c74be:	nop
     646c74bf:	nop
 
-00000000646c74c0 <__powi>:
-    646c74c0:	sub    $0x58,%rsp
-    646c74c4:	movaps %xmm6,0x40(%rsp)
-    646c74c9:	movsd  0x1f87(%rip),%xmm1        # 646c9458 <.rdata+0x18>
-    646c74d1:	mov    $0x0,%r10d
-    646c74d7:	movq   %xmm0,%r8
-    646c74dc:	movq   %xmm0,%rax
-    646c74e1:	shr    $0x20,%r8
-    646c74e5:	mov    %r8d,%ecx
-    646c74e8:	mov    %r8d,%r9d
-    646c74eb:	and    $0xfffff,%ecx
-    646c74f1:	and    $0x7ff00000,%r9d
-    646c74f8:	or     %eax,%ecx
-    646c74fa:	ucomisd %xmm1,%xmm0
-    646c74fe:	mov    %r9d,%r11d
-    646c7501:	setnp  %al
-    646c7504:	cmovne %r10d,%eax
-    646c7508:	test   %edx,%edx
-    646c750a:	sete   %r10b
-    646c750e:	or     %r10d,%eax
-    646c7511:	or     %ecx,%r11d
-    646c7514:	jne    646c7550 <__powi+0x90>
-    646c7516:	test   %al,%al
-    646c7518:	movapd %xmm1,%xmm6
-    646c751c:	jne    646c7540 <__powi+0x80>
-    646c751e:	mov    %edx,%eax
-    646c7520:	and    $0x1,%eax
-    646c7523:	test   %edx,%edx
-    646c7525:	js     646c7615 <__powi+0x155>
-    646c752b:	test   %eax,%eax
-    646c752d:	pxor   %xmm6,%xmm6
-    646c7531:	je     646c7540 <__powi+0x80>
-    646c7533:	test   %r8d,%r8d
-    646c7536:	jns    646c7540 <__powi+0x80>
-    646c7538:	movsd  0x1f20(%rip),%xmm6        # 646c9460 <.rdata+0x20>
-    646c7540:	movapd %xmm6,%xmm0
-    646c7544:	movaps 0x40(%rsp),%xmm6
-    646c7549:	add    $0x58,%rsp
-    646c754d:	ret
-    646c754e:	xchg   %ax,%ax
-    646c7550:	test   %r9d,%r9d
-    646c7553:	jne    646c75c0 <__powi+0x100>
-    646c7555:	test   %al,%al
-    646c7557:	movapd %xmm1,%xmm6
-    646c755b:	jne    646c7540 <__powi+0x80>
-    646c755d:	mov    %edx,%eax
-    646c755f:	movapd %xmm0,%xmm6
-    646c7563:	andpd  0x1f15(%rip),%xmm6        # 646c9480 <.rdata+0x40>
-    646c756b:	and    $0x1,%eax
-    646c756e:	test   %edx,%edx
-    646c7570:	js     646c7602 <__powi+0x142>
-    646c7576:	cmp    $0x1,%edx
-    646c7579:	je     646c75a1 <__powi+0xe1>
-    646c757b:	test   $0x1,%dl
-    646c757e:	jne    646c76b0 <__powi+0x1f0>
-    646c7584:	movapd %xmm6,%xmm0
-    646c7588:	shr    %edx
-    646c758a:	movapd %xmm1,%xmm6
-    646c758e:	xchg   %ax,%ax
-    646c7590:	mulsd  %xmm0,%xmm0
-    646c7594:	test   $0x1,%dl
-    646c7597:	je     646c759d <__powi+0xdd>
-    646c7599:	mulsd  %xmm0,%xmm6
-    646c759d:	shr    %edx
-    646c759f:	jne    646c7590 <__powi+0xd0>
-    646c75a1:	shr    $0x1f,%r8d
-    646c75a5:	test   %r8b,%r8b
-    646c75a8:	je     646c7540 <__powi+0x80>
-    646c75aa:	test   %eax,%eax
-    646c75ac:	je     646c7540 <__powi+0x80>
-    646c75ae:	xorpd  0x1eda(%rip),%xmm6        # 646c9490 <.rdata+0x50>
-    646c75b6:	jmp    646c7540 <__powi+0x80>
-    646c75b8:	nopl   0x0(%rax,%rax,1)
-    646c75c0:	cmp    $0x7ff00000,%r9d
-    646c75c7:	jne    646c7555 <__powi+0x95>
-    646c75c9:	test   %ecx,%ecx
-    646c75cb:	jne    646c7640 <__powi+0x180>
-    646c75cd:	mov    %edx,%r9d
-    646c75d0:	movapd %xmm1,%xmm6
-    646c75d4:	and    $0x1,%r9d
-    646c75d8:	test   %al,%al
-    646c75da:	jne    646c7540 <__powi+0x80>
-    646c75e0:	test   %r8d,%r8d
-    646c75e3:	js     646c76d0 <__powi+0x210>
-    646c75e9:	test   %edx,%edx
-    646c75eb:	movsd  0x1e75(%rip),%xmm6        # 646c9468 <.rdata+0x28>
-    646c75f3:	jns    646c7540 <__powi+0x80>
-    646c75f9:	pxor   %xmm6,%xmm6
-    646c75fd:	jmp    646c7540 <__powi+0x80>
-    646c7602:	movapd %xmm1,%xmm4
-    646c7606:	neg    %edx
-    646c7608:	divsd  %xmm6,%xmm4
-    646c760c:	movapd %xmm4,%xmm6
-    646c7610:	jmp    646c7576 <__powi+0xb6>
-    646c7615:	test   %eax,%eax
-    646c7617:	movsd  0x1e49(%rip),%xmm6        # 646c9468 <.rdata+0x28>
-    646c761f:	je     646c7540 <__powi+0x80>
-    646c7625:	test   %r8d,%r8d
-    646c7628:	jns    646c7540 <__powi+0x80>
-    646c762e:	movsd  0x1e3a(%rip),%xmm6        # 646c9470 <.rdata+0x30>
-    646c7636:	jmp    646c7540 <__powi+0x80>
-    646c763b:	nopl   0x0(%rax,%rax,1)
-    646c7640:	test   %al,%al
-    646c7642:	movapd %xmm1,%xmm6
-    646c7646:	jne    646c7540 <__powi+0x80>
-    646c764c:	test   %r8d,%r8d
-    646c764f:	movsd  0x1df9(%rip),%xmm6        # 646c9450 <.rdata+0x10>
-    646c7657:	js     646c76c0 <__powi+0x200>
-    646c7659:	mov    %edx,0x3c(%rsp)
-    646c765d:	movsd  %xmm0,0x30(%rsp)
-    646c7663:	call   646c79d8 <_errno>
-    646c7668:	mov    0x3c(%rsp),%edx
-    646c766c:	pxor   %xmm3,%xmm3
-    646c7670:	mov    $0x1,%ecx
-    646c7675:	movsd  0x30(%rsp),%xmm0
-    646c767b:	movl   $0x21,(%rax)
-    646c7681:	movsd  %xmm6,0x20(%rsp)
-    646c7687:	movapd %xmm0,%xmm2
-    646c768b:	cvtsi2sd %edx,%xmm3
-    646c768f:	lea    0x1daa(%rip),%rdx        # 646c9440 <.rdata>
-    646c7696:	call   646c7c50 <__mingw_raise_matherr>
-    646c769b:	movapd %xmm6,%xmm0
-    646c769f:	movaps 0x40(%rsp),%xmm6
-    646c76a4:	add    $0x58,%rsp
-    646c76a8:	ret
-    646c76a9:	nopl   0x0(%rax)
-    646c76b0:	movapd %xmm6,%xmm1
-    646c76b4:	jmp    646c7584 <__powi+0xc4>
-    646c76b9:	nopl   0x0(%rax)
-    646c76c0:	movsd  0x1d80(%rip),%xmm6        # 646c9448 <.rdata+0x8>
-    646c76c8:	jmp    646c7659 <__powi+0x199>
-    646c76ca:	nopw   0x0(%rax,%rax,1)
-    646c76d0:	mov    %edx,%eax
-    646c76d2:	not    %eax
-    646c76d4:	mov    %eax,%ecx
-    646c76d6:	and    $0x1,%ecx
-    646c76d9:	test   %edx,%edx
-    646c76db:	jns    646c76e9 <__powi+0x229>
-    646c76dd:	test   %cl,%cl
-    646c76df:	pxor   %xmm6,%xmm6
-    646c76e3:	jne    646c7540 <__powi+0x80>
-    646c76e9:	shr    $0x1f,%eax
-    646c76ec:	test   $0x1,%dl
-    646c76ef:	je     646c7701 <__powi+0x241>
-    646c76f1:	test   %al,%al
-    646c76f3:	movsd  0x1d75(%rip),%xmm6        # 646c9470 <.rdata+0x30>
-    646c76fb:	jne    646c7540 <__powi+0x80>
-    646c7701:	test   %cl,%cl
-    646c7703:	je     646c7715 <__powi+0x255>
-    646c7705:	test   %al,%al
-    646c7707:	movsd  0x1d59(%rip),%xmm6        # 646c9468 <.rdata+0x28>
-    646c770f:	jne    646c7540 <__powi+0x80>
-    646c7715:	test   %edx,%edx
-    646c7717:	js     646c7730 <__powi+0x270>
-    646c7719:	and    $0x1,%dl
-    646c771c:	jne    646c762e <__powi+0x16e>
-    646c7722:	movsd  0x1d3e(%rip),%xmm6        # 646c9468 <.rdata+0x28>
-    646c772a:	jmp    646c7540 <__powi+0x80>
-    646c772f:	nop
-    646c7730:	test   %r9d,%r9d
-    646c7733:	jne    646c7538 <__powi+0x78>
-    646c7739:	jmp    646c75f9 <__powi+0x139>
-    646c773e:	nop
-    646c773f:	nop
-
-00000000646c7740 <exp2l>:
-    646c7740:	fldt   (%rdx)
-    646c7742:	fxam
-    646c7744:	fstsw  %ax
-    646c7747:	mov    $0x45,%dh
-    646c7749:	and    %ah,%dh
-    646c774b:	cmp    $0x5,%dh
-    646c774e:	je     646c778f <exp2l+0x4f>
-    646c7750:	fld    %st(0)
-    646c7752:	sub    $0x8,%rsp
-    646c7756:	fnstcw 0x4(%rsp)
-    646c775a:	movzwl 0x4(%rsp),%eax
-    646c775f:	or     $0xc,%ah
-    646c7762:	mov    %ax,(%rsp)
-    646c7766:	fldcw  (%rsp)
-    646c7769:	frndint
-    646c776b:	fldcw  0x4(%rsp)
-    646c776f:	add    $0x8,%rsp
-    646c7773:	fsubr  %st,%st(1)
-    646c7775:	fxch   %st(1)
-    646c7777:	f2xm1
-    646c7779:	fld1
-    646c777b:	faddp  %st,%st(1)
-    646c777d:	fscale
-    646c777f:	fstp   %st(1)
-    646c7781:	mov    %rcx,%rax
-    646c7784:	movq   $0x0,0x8(%rcx)
-    646c778c:	fstpt  (%rcx)
-    646c778e:	ret
-    646c778f:	test   $0x200,%eax
-    646c7794:	je     646c779a <exp2l+0x5a>
-    646c7796:	fstp   %st(0)
-    646c7798:	fldz
-    646c779a:	mov    %rcx,%rax
-    646c779d:	movq   $0x0,0x8(%rcx)
-    646c77a5:	fstpt  (%rcx)
-    646c77a7:	ret
-    646c77a8:	nop
-    646c77a9:	nop
-    646c77aa:	nop
-    646c77ab:	nop
-    646c77ac:	nop
-    646c77ad:	nop
-    646c77ae:	nop
-    646c77af:	nop
-
-00000000646c77b0 <one>:
-    646c77b0:	add    %al,(%rax)
-    646c77b2:	add    %al,(%rax)
-    646c77b4:	add    %al,(%rax)
-    646c77b6:	lock (bad)
-
-00000000646c77b8 <limit>:
-    646c77b8:	pop    %rdx
-    646c77ba:	cmc
-    646c77bb:	sub    %bl,-0x2e(%rdi,%rcx,4)
-    646c77bf:	(bad)
-
-00000000646c77c0 <__logl_internal>:
-    646c77c0:	fldln2
-    646c77c2:	fldt   (%rdx)
-    646c77c4:	fld    %st(0)
-    646c77c6:	fsubl  -0x1c(%rip)        # 646c77b0 <one>
-    646c77cc:	fld    %st(0)
-    646c77ce:	fabs
-    646c77d0:	fcompl -0x1e(%rip)        # 646c77b8 <limit>
-    646c77d6:	fnstsw %ax
-    646c77d8:	and    $0x45,%ah
-    646c77db:	je     646c77ef <__logl_internal+0x2f>
-    646c77dd:	fstp   %st(1)
-    646c77df:	fyl2xp1
-    646c77e1:	mov    %rcx,%rax
-    646c77e4:	movq   $0x0,0x8(%rcx)
-    646c77ec:	fstpt  (%rcx)
-    646c77ee:	ret
-    646c77ef:	fstp   %st(0)
-    646c77f1:	fyl2x
-    646c77f3:	mov    %rcx,%rax
-    646c77f6:	movq   $0x0,0x8(%rcx)
-    646c77fe:	fstpt  (%rcx)
-    646c7800:	ret
-    646c7801:	nop
-    646c7802:	nop
-    646c7803:	nop
-    646c7804:	nop
-    646c7805:	nop
-    646c7806:	nop
-    646c7807:	nop
-    646c7808:	nop
-    646c7809:	nop
-    646c780a:	nop
-    646c780b:	nop
-    646c780c:	nop
-    646c780d:	nop
-    646c780e:	nop
-    646c780f:	nop
-
-00000000646c7810 <ldexp>:
-    646c7810:	push   %rbx
-    646c7811:	sub    $0x30,%rsp
-    646c7815:	movq   %xmm0,%rax
-    646c781a:	movq   %xmm0,%rbx
-    646c781f:	shr    $0x20,%rax
-    646c7823:	mov    %eax,%r8d
-    646c7826:	and    $0x7fffffff,%r8d
-    646c782d:	or     %ebx,%r8d
-    646c7830:	sete   %r8b
-    646c7834:	and    $0x7ff00000,%eax
-    646c7839:	sete   %cl
-    646c783c:	or     %cl,%r8b
-    646c783f:	jne    646c7848 <ldexp+0x38>
-    646c7841:	cmp    $0x7ff00000,%eax
-    646c7846:	je     646c78c3 <ldexp+0xb3>
-    646c7848:	movq   %rbx,%xmm1
-    646c784d:	pxor   %xmm0,%xmm0
-    646c7851:	ucomisd %xmm0,%xmm1
-    646c7855:	jp     646c7859 <ldexp+0x49>
-    646c7857:	je     646c78c3 <ldexp+0xb3>
-    646c7859:	pxor   %xmm2,%xmm2
-    646c785d:	cvtsi2sd %edx,%xmm2
-    646c7861:	mov    %rbx,0x20(%rsp)
-    646c7866:	fldl   0x20(%rsp)
-    646c786a:	movsd  %xmm2,0x28(%rsp)
-    646c7870:	fldl   0x28(%rsp)
-    646c7874:	fxch   %st(1)
-    646c7876:	fscale
-    646c7878:	fstp   %st(1)
-    646c787a:	fstpl  0x20(%rsp)
-    646c787e:	mov    0x20(%rsp),%rbx
-    646c7883:	mov    %rbx,%rax
-    646c7886:	shr    $0x20,%rax
-    646c788a:	mov    %eax,%ecx
-    646c788c:	and    $0x7fffffff,%ecx
-    646c7892:	or     %ebx,%ecx
-    646c7894:	sete   %cl
-    646c7897:	and    $0x7ff00000,%eax
-    646c789c:	sete   %dl
-    646c789f:	or     %dl,%cl
-    646c78a1:	jne    646c78aa <ldexp+0x9a>
-    646c78a3:	cmp    $0x7ff00000,%eax
-    646c78a8:	je     646c78b8 <ldexp+0xa8>
-    646c78aa:	movsd  0x20(%rsp),%xmm3
-    646c78b0:	ucomisd %xmm0,%xmm3
-    646c78b4:	jp     646c78c3 <ldexp+0xb3>
-    646c78b6:	jne    646c78c3 <ldexp+0xb3>
-    646c78b8:	call   646c79d8 <_errno>
-    646c78bd:	movl   $0x22,(%rax)
-    646c78c3:	movq   %rbx,%xmm0
-    646c78c8:	add    $0x30,%rsp
-    646c78cc:	pop    %rbx
-    646c78cd:	ret
+00000000646c74c0 <one>:
+    646c74c0:	add    %al,(%rax)
+    646c74c2:	add    %al,(%rax)
+    646c74c4:	add    %al,(%rax)
+    646c74c6:	lock (bad)
+
+00000000646c74c8 <limit>:
+    646c74c8:	pop    %rdx
+    646c74ca:	cmc
+    646c74cb:	sub    %bl,-0x2e(%rdi,%rcx,4)
+    646c74cf:	(bad)
+
+00000000646c74d0 <__logl_internal>:
+    646c74d0:	fldln2
+    646c74d2:	fldt   (%rdx)
+    646c74d4:	fld    %st(0)
+    646c74d6:	fsubl  -0x1c(%rip)        # 646c74c0 <one>
+    646c74dc:	fld    %st(0)
+    646c74de:	fabs
+    646c74e0:	fcompl -0x1e(%rip)        # 646c74c8 <limit>
+    646c74e6:	fnstsw %ax
+    646c74e8:	and    $0x45,%ah
+    646c74eb:	je     646c74ff <__logl_internal+0x2f>
+    646c74ed:	fstp   %st(1)
+    646c74ef:	fyl2xp1
+    646c74f1:	mov    %rcx,%rax
+    646c74f4:	movq   $0x0,0x8(%rcx)
+    646c74fc:	fstpt  (%rcx)
+    646c74fe:	ret
+    646c74ff:	fstp   %st(0)
+    646c7501:	fyl2x
+    646c7503:	mov    %rcx,%rax
+    646c7506:	movq   $0x0,0x8(%rcx)
+    646c750e:	fstpt  (%rcx)
+    646c7510:	ret
+    646c7511:	nop
+    646c7512:	nop
+    646c7513:	nop
+    646c7514:	nop
+    646c7515:	nop
+    646c7516:	nop
+    646c7517:	nop
+    646c7518:	nop
+    646c7519:	nop
+    646c751a:	nop
+    646c751b:	nop
+    646c751c:	nop
+    646c751d:	nop
+    646c751e:	nop
+    646c751f:	nop
+
+00000000646c7520 <ldexp>:
+    646c7520:	push   %rbx
+    646c7521:	sub    $0x30,%rsp
+    646c7525:	movq   %xmm0,%rax
+    646c752a:	movq   %xmm0,%rbx
+    646c752f:	shr    $0x20,%rax
+    646c7533:	mov    %eax,%r8d
+    646c7536:	and    $0x7fffffff,%r8d
+    646c753d:	or     %ebx,%r8d
+    646c7540:	sete   %r8b
+    646c7544:	and    $0x7ff00000,%eax
+    646c7549:	sete   %cl
+    646c754c:	or     %cl,%r8b
+    646c754f:	jne    646c7558 <ldexp+0x38>
+    646c7551:	cmp    $0x7ff00000,%eax
+    646c7556:	je     646c75d3 <ldexp+0xb3>
+    646c7558:	movq   %rbx,%xmm1
+    646c755d:	pxor   %xmm0,%xmm0
+    646c7561:	ucomisd %xmm0,%xmm1
+    646c7565:	jp     646c7569 <ldexp+0x49>
+    646c7567:	je     646c75d3 <ldexp+0xb3>
+    646c7569:	pxor   %xmm2,%xmm2
+    646c756d:	cvtsi2sd %edx,%xmm2
+    646c7571:	mov    %rbx,0x20(%rsp)
+    646c7576:	fldl   0x20(%rsp)
+    646c757a:	movsd  %xmm2,0x28(%rsp)
+    646c7580:	fldl   0x28(%rsp)
+    646c7584:	fxch   %st(1)
+    646c7586:	fscale
+    646c7588:	fstp   %st(1)
+    646c758a:	fstpl  0x20(%rsp)
+    646c758e:	mov    0x20(%rsp),%rbx
+    646c7593:	mov    %rbx,%rax
+    646c7596:	shr    $0x20,%rax
+    646c759a:	mov    %eax,%ecx
+    646c759c:	and    $0x7fffffff,%ecx
+    646c75a2:	or     %ebx,%ecx
+    646c75a4:	sete   %cl
+    646c75a7:	and    $0x7ff00000,%eax
+    646c75ac:	sete   %dl
+    646c75af:	or     %dl,%cl
+    646c75b1:	jne    646c75ba <ldexp+0x9a>
+    646c75b3:	cmp    $0x7ff00000,%eax
+    646c75b8:	je     646c75c8 <ldexp+0xa8>
+    646c75ba:	movsd  0x20(%rsp),%xmm3
+    646c75c0:	ucomisd %xmm0,%xmm3
+    646c75c4:	jp     646c75d3 <ldexp+0xb3>
+    646c75c6:	jne    646c75d3 <ldexp+0xb3>
+    646c75c8:	call   646c76e8 <_errno>
+    646c75cd:	movl   $0x22,(%rax)
+    646c75d3:	movq   %rbx,%xmm0
+    646c75d8:	add    $0x30,%rsp
+    646c75dc:	pop    %rbx
+    646c75dd:	ret
+    646c75de:	nop
+    646c75df:	nop
+
+00000000646c75e0 <one>:
+    646c75e0:	add    %al,(%rax)
+    646c75e2:	add    %al,(%rax)
+    646c75e4:	add    %al,(%rax)
+    646c75e6:	lock (bad)
+
+00000000646c75e8 <limit>:
+    646c75e8:	pop    %rdx
+    646c75ea:	cmc
+    646c75eb:	sub    %bl,-0x2e(%rdi,%rcx,4)
+    646c75ef:	(bad)
+
+00000000646c75f0 <log2l>:
+    646c75f0:	fldl   -0x16(%rip)        # 646c75e0 <one>
+    646c75f6:	fldt   (%rdx)
+    646c75f8:	fxam
+    646c75fa:	fnstsw %ax
+    646c75fc:	fld    %st(0)
+    646c75fe:	sahf
+    646c75ff:	jb     646c7638 <log2l+0x48>
+    646c7601:	fsub   %st(2),%st
+    646c7603:	fld    %st(0)
+    646c7605:	fabs
+    646c7607:	fcompl -0x25(%rip)        # 646c75e8 <limit>
+    646c760d:	fnstsw %ax
+    646c760f:	and    $0x45,%ah
+    646c7612:	je     646c7626 <log2l+0x36>
+    646c7614:	fstp   %st(1)
+    646c7616:	fyl2xp1
+    646c7618:	mov    %rcx,%rax
+    646c761b:	movq   $0x0,0x8(%rcx)
+    646c7623:	fstpt  (%rcx)
+    646c7625:	ret
+    646c7626:	fstp   %st(0)
+    646c7628:	fyl2x
+    646c762a:	mov    %rcx,%rax
+    646c762d:	movq   $0x0,0x8(%rcx)
+    646c7635:	fstpt  (%rcx)
+    646c7637:	ret
+    646c7638:	jp     646c7601 <log2l+0x11>
+    646c763a:	fstp   %st(1)
+    646c763c:	fstp   %st(1)
+    646c763e:	mov    %rcx,%rax
+    646c7641:	movq   $0x0,0x8(%rcx)
+    646c7649:	fstpt  (%rcx)
+    646c764b:	ret
+    646c764c:	nop
+    646c764d:	nop
+    646c764e:	nop
+    646c764f:	nop
+
+00000000646c7650 <vfprintf>:
+    646c7650:	jmp    *0x6cf6(%rip)        # 646ce34c <__imp_vfprintf>
+    646c7656:	nop
+    646c7657:	nop
+
+00000000646c7658 <strncmp>:
+    646c7658:	jmp    *0x6ce6(%rip)        # 646ce344 <__imp_strncmp>
+    646c765e:	nop
+    646c765f:	nop
+
+00000000646c7660 <strlen>:
+    646c7660:	jmp    *0x6cd6(%rip)        # 646ce33c <__imp_strlen>
+    646c7666:	nop
+    646c7667:	nop
+
+00000000646c7668 <signal>:
+    646c7668:	jmp    *0x6cc6(%rip)        # 646ce334 <__imp_signal>
+    646c766e:	nop
+    646c766f:	nop
+
+00000000646c7670 <printf>:
+    646c7670:	jmp    *0x6cae(%rip)        # 646ce324 <__imp_printf>
+    646c7676:	nop
+    646c7677:	nop
+
+00000000646c7678 <perror>:
+    646c7678:	jmp    *0x6c9e(%rip)        # 646ce31c <__imp_perror>
+    646c767e:	nop
+    646c767f:	nop
+
+00000000646c7680 <malloc>:
+    646c7680:	jmp    *0x6c8e(%rip)        # 646ce314 <__imp_malloc>
+    646c7686:	nop
+    646c7687:	nop
+
+00000000646c7688 <log10>:
+    646c7688:	jmp    *0x6c7e(%rip)        # 646ce30c <__imp_log10>
+    646c768e:	nop
+    646c768f:	nop
+
+00000000646c7690 <fwrite>:
+    646c7690:	jmp    *0x6c6e(%rip)        # 646ce304 <__imp_fwrite>
+    646c7696:	nop
+    646c7697:	nop
+
+00000000646c7698 <free>:
+    646c7698:	jmp    *0x6c5e(%rip)        # 646ce2fc <__imp_free>
+    646c769e:	nop
+    646c769f:	nop
+
+00000000646c76a0 <fprintf>:
+    646c76a0:	jmp    *0x6c4e(%rip)        # 646ce2f4 <__imp_fprintf>
+    646c76a6:	nop
+    646c76a7:	nop
+
+00000000646c76a8 <fopen>:
+    646c76a8:	jmp    *0x6c3e(%rip)        # 646ce2ec <__imp_fopen>
+    646c76ae:	nop
+    646c76af:	nop
+
+00000000646c76b0 <fclose>:
+    646c76b0:	jmp    *0x6c2e(%rip)        # 646ce2e4 <__imp_fclose>
+    646c76b6:	nop
+    646c76b7:	nop
+
+00000000646c76b8 <exit>:
+    646c76b8:	jmp    *0x6c1e(%rip)        # 646ce2dc <__imp_exit>
+    646c76be:	nop
+    646c76bf:	nop
+
+00000000646c76c0 <calloc>:
+    646c76c0:	jmp    *0x6c0e(%rip)        # 646ce2d4 <__imp_calloc>
+    646c76c6:	nop
+    646c76c7:	nop
+
+00000000646c76c8 <abort>:
+    646c76c8:	jmp    *0x6bfe(%rip)        # 646ce2cc <__imp_abort>
+    646c76ce:	nop
+    646c76cf:	nop
+
+00000000646c76d0 <_vsnprintf>:
+    646c76d0:	jmp    *0x6bee(%rip)        # 646ce2c4 <__imp__vsnprintf>
+    646c76d6:	nop
+    646c76d7:	nop
+
+00000000646c76d8 <_mkdir>:
+    646c76d8:	jmp    *0x6bd6(%rip)        # 646ce2b4 <__imp__mkdir>
+    646c76de:	nop
+    646c76df:	nop
+
+00000000646c76e0 <_initterm>:
+    646c76e0:	jmp    *0x6bbe(%rip)        # 646ce2a4 <__imp__initterm>
+    646c76e6:	nop
+    646c76e7:	nop
+
+00000000646c76e8 <_errno>:
+    646c76e8:	jmp    *0x6bae(%rip)        # 646ce29c <__imp__errno>
+    646c76ee:	nop
+    646c76ef:	nop
+
+00000000646c76f0 <_amsg_exit>:
+    646c76f0:	jmp    *0x6b9e(%rip)        # 646ce294 <__imp__amsg_exit>
+    646c76f6:	nop
+    646c76f7:	nop
+    646c76f8:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7700 <_initialize_onexit_table>:
+    646c7700:	test   %rcx,%rcx
+    646c7703:	je     646c771f <_initialize_onexit_table+0x1f>
+    646c7705:	xor    %eax,%eax
+    646c7707:	movq   $0x0,0x10(%rcx)
+    646c770f:	movq   $0x0,0x8(%rcx)
+    646c7717:	movq   $0x0,(%rcx)
+    646c771e:	ret
+    646c771f:	mov    $0xffffffff,%eax
+    646c7724:	ret
+    646c7725:	nop
+    646c7726:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c7730 <_register_onexit_function>:
+    646c7730:	push   %rbp
+    646c7731:	push   %rdi
+    646c7732:	push   %rsi
+    646c7733:	push   %rbx
+    646c7734:	sub    $0x28,%rsp
+    646c7738:	test   %rcx,%rcx
+    646c773b:	mov    %rcx,%rbx
+    646c773e:	mov    %rdx,%rdi
+    646c7741:	je     646c77e0 <_register_onexit_function+0xb0>
+    646c7747:	mov    $0x8,%ecx
+    646c774c:	call   646c78a0 <_lock>
+    646c7751:	cmpq   $0x0,(%rbx)
+    646c7755:	je     646c77b4 <_register_onexit_function+0x84>
+    646c7757:	mov    0x8(%rbx),%rsi
+    646c775b:	mov    0x10(%rbx),%rax
+    646c775f:	cmp    %rsi,%rax
+    646c7762:	je     646c7784 <_register_onexit_function+0x54>
+    646c7764:	lea    0x8(%rsi),%rax
+    646c7768:	mov    $0x8,%ecx
+    646c776d:	mov    %rax,0x8(%rbx)
+    646c7771:	mov    %rdi,(%rsi)
+    646c7774:	call   646c7898 <_unlock>
+    646c7779:	xor    %eax,%eax
+    646c777b:	add    $0x28,%rsp
+    646c777f:	pop    %rbx
+    646c7780:	pop    %rsi
+    646c7781:	pop    %rdi
+    646c7782:	pop    %rbp
+    646c7783:	ret
+    646c7784:	mov    (%rbx),%rcx
+    646c7787:	sub    %rcx,%rsi
+    646c778a:	mov    %rsi,%rax
+    646c778d:	sar    $0x3,%rax
+    646c7791:	shl    $0x4,%rax
+    646c7795:	mov    %rax,%rdx
+    646c7798:	mov    %rax,%rbp
+    646c779b:	call   646c7890 <realloc>
+    646c77a0:	test   %rax,%rax
+    646c77a3:	je     646c77e7 <_register_onexit_function+0xb7>
+    646c77a5:	mov    %rax,(%rbx)
+    646c77a8:	add    %rax,%rsi
+    646c77ab:	add    %rbp,%rax
+    646c77ae:	mov    %rax,0x10(%rbx)
+    646c77b2:	jmp    646c7764 <_register_onexit_function+0x34>
+    646c77b4:	mov    $0x8,%edx
+    646c77b9:	mov    $0x20,%ecx
+    646c77be:	call   646c76c0 <calloc>
+    646c77c3:	test   %rax,%rax
+    646c77c6:	mov    %rax,%rsi
+    646c77c9:	mov    %rax,(%rbx)
+    646c77cc:	je     646c77e7 <_register_onexit_function+0xb7>
+    646c77ce:	mov    %rax,0x8(%rbx)
+    646c77d2:	lea    0x100(%rax),%rax
+    646c77d9:	mov    %rax,0x10(%rbx)
+    646c77dd:	jmp    646c775f <_register_onexit_function+0x2f>
+    646c77df:	nop
+    646c77e0:	mov    $0xffffffff,%eax
+    646c77e5:	jmp    646c777b <_register_onexit_function+0x4b>
+    646c77e7:	mov    $0x8,%ecx
+    646c77ec:	call   646c7898 <_unlock>
+    646c77f1:	mov    $0xffffffff,%eax
+    646c77f6:	jmp    646c777b <_register_onexit_function+0x4b>
+    646c77f8:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7800 <_execute_onexit_table>:
+    646c7800:	push   %rdi
+    646c7801:	push   %rsi
+    646c7802:	push   %rbx
+    646c7803:	sub    $0x20,%rsp
+    646c7807:	mov    %rcx,%rdi
+    646c780a:	mov    $0x8,%ecx
+    646c780f:	call   646c78a0 <_lock>
+    646c7814:	mov    (%rdi),%rsi
+    646c7817:	mov    $0x8,%ecx
+    646c781c:	movq   $0x0,0x10(%rdi)
+    646c7824:	mov    0x8(%rdi),%rbx
+    646c7828:	movq   $0x0,(%rdi)
+    646c782f:	movq   $0x0,0x8(%rdi)
+    646c7837:	call   646c7898 <_unlock>
+    646c783c:	test   %rsi,%rsi
+    646c783f:	je     646c7865 <_execute_onexit_table+0x65>
+    646c7841:	sub    $0x8,%rbx
+    646c7845:	cmp    %rbx,%rsi
+    646c7848:	ja     646c785d <_execute_onexit_table+0x5d>
+    646c784a:	mov    (%rbx),%rax
+    646c784d:	test   %rax,%rax
+    646c7850:	je     646c7841 <_execute_onexit_table+0x41>
+    646c7852:	call   *%rax
+    646c7854:	sub    $0x8,%rbx
+    646c7858:	cmp    %rbx,%rsi
+    646c785b:	jbe    646c784a <_execute_onexit_table+0x4a>
+    646c785d:	mov    %rsi,%rcx
+    646c7860:	call   646c7698 <free>
+    646c7865:	xor    %eax,%eax
+    646c7867:	add    $0x20,%rsp
+    646c786b:	pop    %rbx
+    646c786c:	pop    %rsi
+    646c786d:	pop    %rdi
+    646c786e:	ret
+    646c786f:	nop
+
+00000000646c7870 <__acrt_iob_func>:
+    646c7870:	push   %rbx
+    646c7871:	sub    $0x20,%rsp
+    646c7875:	mov    %ecx,%ebx
+    646c7877:	call   646c78a8 <__iob_func>
+    646c787c:	mov    %ebx,%ecx
+    646c787e:	lea    (%rcx,%rcx,2),%rdx
+    646c7882:	shl    $0x4,%rdx
+    646c7886:	add    %rdx,%rax
+    646c7889:	add    $0x20,%rsp
+    646c788d:	pop    %rbx
+    646c788e:	ret
+    646c788f:	nop
+
+00000000646c7890 <realloc>:
+    646c7890:	jmp    *0x6a96(%rip)        # 646ce32c <__imp_realloc>
+    646c7896:	nop
+    646c7897:	nop
+
+00000000646c7898 <_unlock>:
+    646c7898:	jmp    *0x6a1e(%rip)        # 646ce2bc <__imp__unlock>
+    646c789e:	nop
+    646c789f:	nop
+
+00000000646c78a0 <_lock>:
+    646c78a0:	jmp    *0x6a06(%rip)        # 646ce2ac <__imp__lock>
+    646c78a6:	nop
+    646c78a7:	nop
+
+00000000646c78a8 <__iob_func>:
+    646c78a8:	jmp    *0x69d6(%rip)        # 646ce284 <__imp___iob_func>
+    646c78ae:	nop
+    646c78af:	nop
+
+00000000646c78b0 <VirtualQuery>:
+    646c78b0:	jmp    *0x69be(%rip)        # 646ce274 <__imp_VirtualQuery>
+    646c78b6:	nop
+    646c78b7:	nop
+
+00000000646c78b8 <VirtualProtect>:
+    646c78b8:	jmp    *0x69ae(%rip)        # 646ce26c <__imp_VirtualProtect>
+    646c78be:	nop
+    646c78bf:	nop
+
+00000000646c78c0 <UnhandledExceptionFilter>:
+    646c78c0:	jmp    *0x699e(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
+    646c78c6:	nop
+    646c78c7:	nop
+
+00000000646c78c8 <TlsGetValue>:
+    646c78c8:	jmp    *0x698e(%rip)        # 646ce25c <__imp_TlsGetValue>
     646c78ce:	nop
     646c78cf:	nop
 
-00000000646c78d0 <one>:
-    646c78d0:	add    %al,(%rax)
-    646c78d2:	add    %al,(%rax)
-    646c78d4:	add    %al,(%rax)
-    646c78d6:	lock (bad)
-
-00000000646c78d8 <limit>:
-    646c78d8:	pop    %rdx
-    646c78da:	cmc
-    646c78db:	sub    %bl,-0x2e(%rdi,%rcx,4)
-    646c78df:	(bad)
-
-00000000646c78e0 <log2l>:
-    646c78e0:	fldl   -0x16(%rip)        # 646c78d0 <one>
-    646c78e6:	fldt   (%rdx)
-    646c78e8:	fxam
-    646c78ea:	fnstsw %ax
-    646c78ec:	fld    %st(0)
-    646c78ee:	sahf
-    646c78ef:	jb     646c7928 <log2l+0x48>
-    646c78f1:	fsub   %st(2),%st
-    646c78f3:	fld    %st(0)
-    646c78f5:	fabs
-    646c78f7:	fcompl -0x25(%rip)        # 646c78d8 <limit>
-    646c78fd:	fnstsw %ax
-    646c78ff:	and    $0x45,%ah
-    646c7902:	je     646c7916 <log2l+0x36>
-    646c7904:	fstp   %st(1)
-    646c7906:	fyl2xp1
-    646c7908:	mov    %rcx,%rax
-    646c790b:	movq   $0x0,0x8(%rcx)
-    646c7913:	fstpt  (%rcx)
-    646c7915:	ret
-    646c7916:	fstp   %st(0)
-    646c7918:	fyl2x
-    646c791a:	mov    %rcx,%rax
-    646c791d:	movq   $0x0,0x8(%rcx)
-    646c7925:	fstpt  (%rcx)
-    646c7927:	ret
-    646c7928:	jp     646c78f1 <log2l+0x11>
-    646c792a:	fstp   %st(1)
-    646c792c:	fstp   %st(1)
-    646c792e:	mov    %rcx,%rax
-    646c7931:	movq   $0x0,0x8(%rcx)
-    646c7939:	fstpt  (%rcx)
-    646c793b:	ret
-    646c793c:	nop
-    646c793d:	nop
+00000000646c78d0 <TerminateProcess>:
+    646c78d0:	jmp    *0x697e(%rip)        # 646ce254 <__imp_TerminateProcess>
+    646c78d6:	nop
+    646c78d7:	nop
+
+00000000646c78d8 <SetUnhandledExceptionFilter>:
+    646c78d8:	jmp    *0x6966(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
+    646c78de:	nop
+    646c78df:	nop
+
+00000000646c78e0 <RtlVirtualUnwind>:
+    646c78e0:	jmp    *0x6956(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
+    646c78e6:	nop
+    646c78e7:	nop
+
+00000000646c78e8 <RtlLookupFunctionEntry>:
+    646c78e8:	jmp    *0x6946(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
+    646c78ee:	nop
+    646c78ef:	nop
+
+00000000646c78f0 <RtlCaptureContext>:
+    646c78f0:	jmp    *0x6936(%rip)        # 646ce22c <__imp_RtlCaptureContext>
+    646c78f6:	nop
+    646c78f7:	nop
+
+00000000646c78f8 <RtlAddFunctionTable>:
+    646c78f8:	jmp    *0x6926(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
+    646c78fe:	nop
+    646c78ff:	nop
+
+00000000646c7900 <QueryPerformanceCounter>:
+    646c7900:	jmp    *0x6916(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
+    646c7906:	nop
+    646c7907:	nop
+
+00000000646c7908 <LeaveCriticalSection>:
+    646c7908:	jmp    *0x6906(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
+    646c790e:	nop
+    646c790f:	nop
+
+00000000646c7910 <InitializeCriticalSection>:
+    646c7910:	jmp    *0x68f6(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
+    646c7916:	nop
+    646c7917:	nop
+
+00000000646c7918 <GetTickCount>:
+    646c7918:	jmp    *0x68e6(%rip)        # 646ce204 <__imp_GetTickCount>
+    646c791e:	nop
+    646c791f:	nop
+
+00000000646c7920 <GetSystemTimeAsFileTime>:
+    646c7920:	jmp    *0x68d6(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
+    646c7926:	nop
+    646c7927:	nop
+
+00000000646c7928 <GetLastError>:
+    646c7928:	jmp    *0x68c6(%rip)        # 646ce1f4 <__imp_GetLastError>
+    646c792e:	nop
+    646c792f:	nop
+
+00000000646c7930 <GetCurrentThreadId>:
+    646c7930:	jmp    *0x68b6(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
+    646c7936:	nop
+    646c7937:	nop
+
+00000000646c7938 <GetCurrentProcessId>:
+    646c7938:	jmp    *0x68a6(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
     646c793e:	nop
     646c793f:	nop
 
-00000000646c7940 <vfprintf>:
-    646c7940:	jmp    *0x6a06(%rip)        # 646ce34c <__imp_vfprintf>
+00000000646c7940 <GetCurrentProcess>:
+    646c7940:	jmp    *0x6896(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
     646c7946:	nop
     646c7947:	nop
 
-00000000646c7948 <strncmp>:
-    646c7948:	jmp    *0x69f6(%rip)        # 646ce344 <__imp_strncmp>
+00000000646c7948 <EnterCriticalSection>:
+    646c7948:	jmp    *0x6886(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
     646c794e:	nop
     646c794f:	nop
 
-00000000646c7950 <strlen>:
-    646c7950:	jmp    *0x69e6(%rip)        # 646ce33c <__imp_strlen>
+00000000646c7950 <DeleteCriticalSection>:
+    646c7950:	jmp    *0x6876(%rip)        # 646ce1cc <__IAT_start__>
     646c7956:	nop
     646c7957:	nop
+    646c7958:	nopl   0x0(%rax,%rax,1)
 
-00000000646c7958 <signal>:
-    646c7958:	jmp    *0x69d6(%rip)        # 646ce334 <__imp_signal>
-    646c795e:	nop
-    646c795f:	nop
-
-00000000646c7960 <printf>:
-    646c7960:	jmp    *0x69be(%rip)        # 646ce324 <__imp_printf>
-    646c7966:	nop
-    646c7967:	nop
-
-00000000646c7968 <perror>:
-    646c7968:	jmp    *0x69ae(%rip)        # 646ce31c <__imp_perror>
-    646c796e:	nop
-    646c796f:	nop
-
-00000000646c7970 <malloc>:
-    646c7970:	jmp    *0x699e(%rip)        # 646ce314 <__imp_malloc>
-    646c7976:	nop
-    646c7977:	nop
-
-00000000646c7978 <log10>:
-    646c7978:	jmp    *0x698e(%rip)        # 646ce30c <__imp_log10>
-    646c797e:	nop
-    646c797f:	nop
-
-00000000646c7980 <fwrite>:
-    646c7980:	jmp    *0x697e(%rip)        # 646ce304 <__imp_fwrite>
-    646c7986:	nop
-    646c7987:	nop
-
-00000000646c7988 <free>:
-    646c7988:	jmp    *0x696e(%rip)        # 646ce2fc <__imp_free>
-    646c798e:	nop
-    646c798f:	nop
-
-00000000646c7990 <fprintf>:
-    646c7990:	jmp    *0x695e(%rip)        # 646ce2f4 <__imp_fprintf>
-    646c7996:	nop
-    646c7997:	nop
-
-00000000646c7998 <fopen>:
-    646c7998:	jmp    *0x694e(%rip)        # 646ce2ec <__imp_fopen>
-    646c799e:	nop
-    646c799f:	nop
-
-00000000646c79a0 <fclose>:
-    646c79a0:	jmp    *0x693e(%rip)        # 646ce2e4 <__imp_fclose>
-    646c79a6:	nop
-    646c79a7:	nop
-
-00000000646c79a8 <exit>:
-    646c79a8:	jmp    *0x692e(%rip)        # 646ce2dc <__imp_exit>
-    646c79ae:	nop
-    646c79af:	nop
-
-00000000646c79b0 <calloc>:
-    646c79b0:	jmp    *0x691e(%rip)        # 646ce2d4 <__imp_calloc>
-    646c79b6:	nop
-    646c79b7:	nop
-
-00000000646c79b8 <abort>:
-    646c79b8:	jmp    *0x690e(%rip)        # 646ce2cc <__imp_abort>
-    646c79be:	nop
-    646c79bf:	nop
-
-00000000646c79c0 <_vsnprintf>:
-    646c79c0:	jmp    *0x68fe(%rip)        # 646ce2c4 <__imp__vsnprintf>
-    646c79c6:	nop
-    646c79c7:	nop
-
-00000000646c79c8 <_mkdir>:
-    646c79c8:	jmp    *0x68e6(%rip)        # 646ce2b4 <__imp__mkdir>
-    646c79ce:	nop
-    646c79cf:	nop
-
-00000000646c79d0 <_initterm>:
-    646c79d0:	jmp    *0x68ce(%rip)        # 646ce2a4 <__imp__initterm>
-    646c79d6:	nop
-    646c79d7:	nop
-
-00000000646c79d8 <_errno>:
-    646c79d8:	jmp    *0x68be(%rip)        # 646ce29c <__imp__errno>
-    646c79de:	nop
-    646c79df:	nop
-
-00000000646c79e0 <_amsg_exit>:
-    646c79e0:	jmp    *0x68ae(%rip)        # 646ce294 <__imp__amsg_exit>
-    646c79e6:	nop
-    646c79e7:	nop
-    646c79e8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c79f0 <_initialize_onexit_table>:
-    646c79f0:	test   %rcx,%rcx
-    646c79f3:	je     646c7a0f <_initialize_onexit_table+0x1f>
-    646c79f5:	xor    %eax,%eax
-    646c79f7:	movq   $0x0,0x10(%rcx)
-    646c79ff:	movq   $0x0,0x8(%rcx)
-    646c7a07:	movq   $0x0,(%rcx)
-    646c7a0e:	ret
-    646c7a0f:	mov    $0xffffffff,%eax
-    646c7a14:	ret
-    646c7a15:	nop
-    646c7a16:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c7a20 <_register_onexit_function>:
-    646c7a20:	push   %rbp
-    646c7a21:	push   %rdi
-    646c7a22:	push   %rsi
-    646c7a23:	push   %rbx
-    646c7a24:	sub    $0x28,%rsp
-    646c7a28:	test   %rcx,%rcx
-    646c7a2b:	mov    %rcx,%rbx
-    646c7a2e:	mov    %rdx,%rdi
-    646c7a31:	je     646c7ad0 <_register_onexit_function+0xb0>
-    646c7a37:	mov    $0x8,%ecx
-    646c7a3c:	call   646c7b90 <_lock>
-    646c7a41:	cmpq   $0x0,(%rbx)
-    646c7a45:	je     646c7aa4 <_register_onexit_function+0x84>
-    646c7a47:	mov    0x8(%rbx),%rsi
-    646c7a4b:	mov    0x10(%rbx),%rax
-    646c7a4f:	cmp    %rsi,%rax
-    646c7a52:	je     646c7a74 <_register_onexit_function+0x54>
-    646c7a54:	lea    0x8(%rsi),%rax
-    646c7a58:	mov    $0x8,%ecx
-    646c7a5d:	mov    %rax,0x8(%rbx)
-    646c7a61:	mov    %rdi,(%rsi)
-    646c7a64:	call   646c7b88 <_unlock>
-    646c7a69:	xor    %eax,%eax
-    646c7a6b:	add    $0x28,%rsp
-    646c7a6f:	pop    %rbx
-    646c7a70:	pop    %rsi
-    646c7a71:	pop    %rdi
-    646c7a72:	pop    %rbp
-    646c7a73:	ret
-    646c7a74:	mov    (%rbx),%rcx
-    646c7a77:	sub    %rcx,%rsi
-    646c7a7a:	mov    %rsi,%rax
-    646c7a7d:	sar    $0x3,%rax
-    646c7a81:	shl    $0x4,%rax
-    646c7a85:	mov    %rax,%rdx
-    646c7a88:	mov    %rax,%rbp
-    646c7a8b:	call   646c7b80 <realloc>
-    646c7a90:	test   %rax,%rax
-    646c7a93:	je     646c7ad7 <_register_onexit_function+0xb7>
-    646c7a95:	mov    %rax,(%rbx)
-    646c7a98:	add    %rax,%rsi
-    646c7a9b:	add    %rbp,%rax
-    646c7a9e:	mov    %rax,0x10(%rbx)
-    646c7aa2:	jmp    646c7a54 <_register_onexit_function+0x34>
-    646c7aa4:	mov    $0x8,%edx
-    646c7aa9:	mov    $0x20,%ecx
-    646c7aae:	call   646c79b0 <calloc>
-    646c7ab3:	test   %rax,%rax
-    646c7ab6:	mov    %rax,%rsi
-    646c7ab9:	mov    %rax,(%rbx)
-    646c7abc:	je     646c7ad7 <_register_onexit_function+0xb7>
-    646c7abe:	mov    %rax,0x8(%rbx)
-    646c7ac2:	lea    0x100(%rax),%rax
-    646c7ac9:	mov    %rax,0x10(%rbx)
-    646c7acd:	jmp    646c7a4f <_register_onexit_function+0x2f>
-    646c7acf:	nop
-    646c7ad0:	mov    $0xffffffff,%eax
-    646c7ad5:	jmp    646c7a6b <_register_onexit_function+0x4b>
-    646c7ad7:	mov    $0x8,%ecx
-    646c7adc:	call   646c7b88 <_unlock>
-    646c7ae1:	mov    $0xffffffff,%eax
-    646c7ae6:	jmp    646c7a6b <_register_onexit_function+0x4b>
-    646c7ae8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c7af0 <_execute_onexit_table>:
-    646c7af0:	push   %rdi
-    646c7af1:	push   %rsi
-    646c7af2:	push   %rbx
-    646c7af3:	sub    $0x20,%rsp
-    646c7af7:	mov    %rcx,%rdi
-    646c7afa:	mov    $0x8,%ecx
-    646c7aff:	call   646c7b90 <_lock>
-    646c7b04:	mov    (%rdi),%rsi
-    646c7b07:	mov    $0x8,%ecx
-    646c7b0c:	movq   $0x0,0x10(%rdi)
-    646c7b14:	mov    0x8(%rdi),%rbx
-    646c7b18:	movq   $0x0,(%rdi)
-    646c7b1f:	movq   $0x0,0x8(%rdi)
-    646c7b27:	call   646c7b88 <_unlock>
-    646c7b2c:	test   %rsi,%rsi
-    646c7b2f:	je     646c7b55 <_execute_onexit_table+0x65>
-    646c7b31:	sub    $0x8,%rbx
-    646c7b35:	cmp    %rbx,%rsi
-    646c7b38:	ja     646c7b4d <_execute_onexit_table+0x5d>
-    646c7b3a:	mov    (%rbx),%rax
-    646c7b3d:	test   %rax,%rax
-    646c7b40:	je     646c7b31 <_execute_onexit_table+0x41>
-    646c7b42:	call   *%rax
-    646c7b44:	sub    $0x8,%rbx
-    646c7b48:	cmp    %rbx,%rsi
-    646c7b4b:	jbe    646c7b3a <_execute_onexit_table+0x4a>
-    646c7b4d:	mov    %rsi,%rcx
-    646c7b50:	call   646c7988 <free>
-    646c7b55:	xor    %eax,%eax
-    646c7b57:	add    $0x20,%rsp
-    646c7b5b:	pop    %rbx
-    646c7b5c:	pop    %rsi
-    646c7b5d:	pop    %rdi
-    646c7b5e:	ret
-    646c7b5f:	nop
-
-00000000646c7b60 <__acrt_iob_func>:
-    646c7b60:	push   %rbx
-    646c7b61:	sub    $0x20,%rsp
-    646c7b65:	mov    %ecx,%ebx
-    646c7b67:	call   646c7b98 <__iob_func>
-    646c7b6c:	mov    %ebx,%ecx
-    646c7b6e:	lea    (%rcx,%rcx,2),%rdx
-    646c7b72:	shl    $0x4,%rdx
-    646c7b76:	add    %rdx,%rax
-    646c7b79:	add    $0x20,%rsp
-    646c7b7d:	pop    %rbx
-    646c7b7e:	ret
-    646c7b7f:	nop
-
-00000000646c7b80 <realloc>:
-    646c7b80:	jmp    *0x67a6(%rip)        # 646ce32c <__imp_realloc>
-    646c7b86:	nop
-    646c7b87:	nop
-
-00000000646c7b88 <_unlock>:
-    646c7b88:	jmp    *0x672e(%rip)        # 646ce2bc <__imp__unlock>
-    646c7b8e:	nop
-    646c7b8f:	nop
-
-00000000646c7b90 <_lock>:
-    646c7b90:	jmp    *0x6716(%rip)        # 646ce2ac <__imp__lock>
-    646c7b96:	nop
-    646c7b97:	nop
-
-00000000646c7b98 <__iob_func>:
-    646c7b98:	jmp    *0x66e6(%rip)        # 646ce284 <__imp___iob_func>
-    646c7b9e:	nop
-    646c7b9f:	nop
-
-00000000646c7ba0 <VirtualQuery>:
-    646c7ba0:	jmp    *0x66ce(%rip)        # 646ce274 <__imp_VirtualQuery>
-    646c7ba6:	nop
-    646c7ba7:	nop
-
-00000000646c7ba8 <VirtualProtect>:
-    646c7ba8:	jmp    *0x66be(%rip)        # 646ce26c <__imp_VirtualProtect>
-    646c7bae:	nop
-    646c7baf:	nop
-
-00000000646c7bb0 <UnhandledExceptionFilter>:
-    646c7bb0:	jmp    *0x66ae(%rip)        # 646ce264 <__imp_UnhandledExceptionFilter>
-    646c7bb6:	nop
-    646c7bb7:	nop
-
-00000000646c7bb8 <TlsGetValue>:
-    646c7bb8:	jmp    *0x669e(%rip)        # 646ce25c <__imp_TlsGetValue>
-    646c7bbe:	nop
-    646c7bbf:	nop
-
-00000000646c7bc0 <TerminateProcess>:
-    646c7bc0:	jmp    *0x668e(%rip)        # 646ce254 <__imp_TerminateProcess>
-    646c7bc6:	nop
-    646c7bc7:	nop
-
-00000000646c7bc8 <SetUnhandledExceptionFilter>:
-    646c7bc8:	jmp    *0x6676(%rip)        # 646ce244 <__imp_SetUnhandledExceptionFilter>
-    646c7bce:	nop
-    646c7bcf:	nop
-
-00000000646c7bd0 <RtlVirtualUnwind>:
-    646c7bd0:	jmp    *0x6666(%rip)        # 646ce23c <__imp_RtlVirtualUnwind>
-    646c7bd6:	nop
-    646c7bd7:	nop
-
-00000000646c7bd8 <RtlLookupFunctionEntry>:
-    646c7bd8:	jmp    *0x6656(%rip)        # 646ce234 <__imp_RtlLookupFunctionEntry>
-    646c7bde:	nop
-    646c7bdf:	nop
-
-00000000646c7be0 <RtlCaptureContext>:
-    646c7be0:	jmp    *0x6646(%rip)        # 646ce22c <__imp_RtlCaptureContext>
-    646c7be6:	nop
-    646c7be7:	nop
-
-00000000646c7be8 <RtlAddFunctionTable>:
-    646c7be8:	jmp    *0x6636(%rip)        # 646ce224 <__imp_RtlAddFunctionTable>
-    646c7bee:	nop
-    646c7bef:	nop
-
-00000000646c7bf0 <QueryPerformanceCounter>:
-    646c7bf0:	jmp    *0x6626(%rip)        # 646ce21c <__imp_QueryPerformanceCounter>
-    646c7bf6:	nop
-    646c7bf7:	nop
-
-00000000646c7bf8 <LeaveCriticalSection>:
-    646c7bf8:	jmp    *0x6616(%rip)        # 646ce214 <__imp_LeaveCriticalSection>
-    646c7bfe:	nop
-    646c7bff:	nop
-
-00000000646c7c00 <InitializeCriticalSection>:
-    646c7c00:	jmp    *0x6606(%rip)        # 646ce20c <__imp_InitializeCriticalSection>
-    646c7c06:	nop
-    646c7c07:	nop
-
-00000000646c7c08 <GetTickCount>:
-    646c7c08:	jmp    *0x65f6(%rip)        # 646ce204 <__imp_GetTickCount>
-    646c7c0e:	nop
-    646c7c0f:	nop
-
-00000000646c7c10 <GetSystemTimeAsFileTime>:
-    646c7c10:	jmp    *0x65e6(%rip)        # 646ce1fc <__imp_GetSystemTimeAsFileTime>
-    646c7c16:	nop
-    646c7c17:	nop
-
-00000000646c7c18 <GetLastError>:
-    646c7c18:	jmp    *0x65d6(%rip)        # 646ce1f4 <__imp_GetLastError>
-    646c7c1e:	nop
-    646c7c1f:	nop
-
-00000000646c7c20 <GetCurrentThreadId>:
-    646c7c20:	jmp    *0x65c6(%rip)        # 646ce1ec <__imp_GetCurrentThreadId>
-    646c7c26:	nop
-    646c7c27:	nop
-
-00000000646c7c28 <GetCurrentProcessId>:
-    646c7c28:	jmp    *0x65b6(%rip)        # 646ce1e4 <__imp_GetCurrentProcessId>
-    646c7c2e:	nop
-    646c7c2f:	nop
-
-00000000646c7c30 <GetCurrentProcess>:
-    646c7c30:	jmp    *0x65a6(%rip)        # 646ce1dc <__imp_GetCurrentProcess>
-    646c7c36:	nop
-    646c7c37:	nop
-
-00000000646c7c38 <EnterCriticalSection>:
-    646c7c38:	jmp    *0x6596(%rip)        # 646ce1d4 <__imp_EnterCriticalSection>
-    646c7c3e:	nop
-    646c7c3f:	nop
-
-00000000646c7c40 <DeleteCriticalSection>:
-    646c7c40:	jmp    *0x6586(%rip)        # 646ce1cc <__IAT_start__>
-    646c7c46:	nop
-    646c7c47:	nop
-    646c7c48:	nopl   0x0(%rax,%rax,1)
-
-00000000646c7c50 <__mingw_raise_matherr>:
-    646c7c50:	sub    $0x58,%rsp
-    646c7c54:	mov    0x4f15(%rip),%rax        # 646ccb70 <stUserMathErr>
-    646c7c5b:	test   %rax,%rax
-    646c7c5e:	je     646c7c8c <__mingw_raise_matherr+0x3c>
-    646c7c60:	movsd  0x80(%rsp),%xmm0
-    646c7c69:	mov    %ecx,0x20(%rsp)
-    646c7c6d:	lea    0x20(%rsp),%rcx
-    646c7c72:	mov    %rdx,0x28(%rsp)
-    646c7c77:	movsd  %xmm2,0x30(%rsp)
-    646c7c7d:	movsd  %xmm3,0x38(%rsp)
-    646c7c83:	movsd  %xmm0,0x40(%rsp)
-    646c7c89:	call   *%rax
-    646c7c8b:	nop
-    646c7c8c:	add    $0x58,%rsp
-    646c7c90:	ret
-    646c7c91:	nopl   0x0(%rax,%rax,1)
-    646c7c96:	cs nopw 0x0(%rax,%rax,1)
-
-00000000646c7ca0 <__mingw_setusermatherr>:
-    646c7ca0:	mov    %rcx,0x4ec9(%rip)        # 646ccb70 <stUserMathErr>
-    646c7ca7:	jmp    646c7db0 <__setusermatherr>
-    646c7cac:	nopl   0x0(%rax)
-
-00000000646c7cb0 <_matherr>:
-    646c7cb0:	push   %rsi
-    646c7cb1:	push   %rbx
-    646c7cb2:	sub    $0x78,%rsp
-    646c7cb6:	movaps %xmm6,0x40(%rsp)
-    646c7cbb:	movaps %xmm7,0x50(%rsp)
-    646c7cc0:	movaps %xmm8,0x60(%rsp)
-    646c7cc6:	cmpl   $0x6,(%rcx)
-    646c7cc9:	ja     646c7da0 <_matherr+0xf0>
-    646c7ccf:	mov    (%rcx),%eax
-    646c7cd1:	lea    0x18ec(%rip),%rdx        # 646c95c4 <.rdata+0x124>
-    646c7cd8:	movslq (%rdx,%rax,4),%rax
-    646c7cdc:	add    %rdx,%rax
-    646c7cdf:	jmp    *%rax
-    646c7ce1:	lea    0x17b8(%rip),%rbx        # 646c94a0 <.rdata>
-    646c7ce8:	mov    0x8(%rcx),%rsi
-    646c7cec:	movsd  0x20(%rcx),%xmm8
-    646c7cf2:	movsd  0x18(%rcx),%xmm7
-    646c7cf7:	movsd  0x10(%rcx),%xmm6
-    646c7cfc:	mov    $0x2,%ecx
-    646c7d01:	call   646c7b60 <__acrt_iob_func>
-    646c7d06:	movsd  %xmm8,0x30(%rsp)
-    646c7d0d:	mov    %rsi,%r9
-    646c7d10:	mov    %rbx,%r8
-    646c7d13:	movsd  %xmm7,0x28(%rsp)
-    646c7d19:	lea    0x1878(%rip),%rdx        # 646c9598 <.rdata+0xf8>
-    646c7d20:	mov    %rax,%rcx
-    646c7d23:	movsd  %xmm6,0x20(%rsp)
-    646c7d29:	call   646c7990 <fprintf>
-    646c7d2e:	nop
-    646c7d2f:	movaps 0x40(%rsp),%xmm6
-    646c7d34:	xor    %eax,%eax
-    646c7d36:	movaps 0x50(%rsp),%xmm7
-    646c7d3b:	movaps 0x60(%rsp),%xmm8
-    646c7d41:	add    $0x78,%rsp
-    646c7d45:	pop    %rbx
-    646c7d46:	pop    %rsi
-    646c7d47:	ret
-    646c7d48:	nopl   0x0(%rax,%rax,1)
-    646c7d50:	lea    0x1768(%rip),%rbx        # 646c94bf <.rdata+0x1f>
-    646c7d57:	jmp    646c7ce8 <_matherr+0x38>
-    646c7d59:	nopl   0x0(%rax)
-    646c7d60:	lea    0x1779(%rip),%rbx        # 646c94e0 <.rdata+0x40>
-    646c7d67:	jmp    646c7ce8 <_matherr+0x38>
-    646c7d6c:	nopl   0x0(%rax)
-    646c7d70:	lea    0x17d9(%rip),%rbx        # 646c9550 <.rdata+0xb0>
-    646c7d77:	jmp    646c7ce8 <_matherr+0x38>
-    646c7d7c:	nopl   0x0(%rax)
-    646c7d80:	lea    0x17a1(%rip),%rbx        # 646c9528 <.rdata+0x88>
-    646c7d87:	jmp    646c7ce8 <_matherr+0x38>
-    646c7d8c:	nopl   0x0(%rax)
-    646c7d90:	lea    0x1769(%rip),%rbx        # 646c9500 <.rdata+0x60>
-    646c7d97:	jmp    646c7ce8 <_matherr+0x38>
-    646c7d9c:	nopl   0x0(%rax)
-    646c7da0:	lea    0x17df(%rip),%rbx        # 646c9586 <.rdata+0xe6>
-    646c7da7:	jmp    646c7ce8 <_matherr+0x38>
-    646c7dac:	nop
-    646c7dad:	nop
-    646c7dae:	nop
-    646c7daf:	nop
-
-00000000646c7db0 <__setusermatherr>:
-    646c7db0:	jmp    *0x64d6(%rip)        # 646ce28c <__imp___setusermatherr>
-    646c7db6:	nop
-    646c7db7:	nop
-    646c7db8:	nopl   0x0(%rax,%rax,1)
-
-00000000646c7dc0 <__report_error>:
-    646c7dc0:	push   %rsi
-    646c7dc1:	push   %rbx
-    646c7dc2:	sub    $0x38,%rsp
-    646c7dc6:	lea    0x58(%rsp),%rax
-    646c7dcb:	mov    %rcx,%rbx
-    646c7dce:	mov    $0x2,%ecx
-    646c7dd3:	mov    %rdx,0x58(%rsp)
-    646c7dd8:	mov    %r8,0x60(%rsp)
-    646c7ddd:	mov    %r9,0x68(%rsp)
-    646c7de2:	mov    %rax,0x28(%rsp)
-    646c7de7:	call   646c7b60 <__acrt_iob_func>
-    646c7dec:	mov    $0x1b,%r8d
-    646c7df2:	mov    $0x1,%edx
-    646c7df7:	lea    0x1402(%rip),%rcx        # 646c9200 <.rdata>
-    646c7dfe:	mov    %rax,%r9
-    646c7e01:	call   646c7980 <fwrite>
-    646c7e06:	mov    0x28(%rsp),%rsi
-    646c7e0b:	mov    $0x2,%ecx
-    646c7e10:	call   646c7b60 <__acrt_iob_func>
-    646c7e15:	mov    %rbx,%rdx
-    646c7e18:	mov    %rax,%rcx
-    646c7e1b:	mov    %rsi,%r8
-    646c7e1e:	call   646c7940 <vfprintf>
-    646c7e23:	call   646c79b8 <abort>
-    646c7e28:	nop
-    646c7e29:	nop
-    646c7e2a:	nop
-    646c7e2b:	nop
-    646c7e2c:	nop
-    646c7e2d:	nop
-    646c7e2e:	nop
-    646c7e2f:	nop
-
-00000000646c7e30 <register_frame_ctor>:
-    646c7e30:	jmp    646c1390 <__gcc_register_frame>
-    646c7e35:	nop
-    646c7e36:	nop
-    646c7e37:	nop
-    646c7e38:	nop
-    646c7e39:	nop
-    646c7e3a:	nop
-    646c7e3b:	nop
-    646c7e3c:	nop
-    646c7e3d:	nop
-    646c7e3e:	nop
-    646c7e3f:	nop
-
-00000000646c7e40 <__CTOR_LIST__>:
-    646c7e40:	(bad)
-    646c7e41:	(bad)
-    646c7e42:	(bad)
-    646c7e43:	(bad)
-    646c7e44:	(bad)
-    646c7e45:	(bad)
-    646c7e46:	(bad)
-    646c7e47:	push   (%rax)
-
-00000000646c7e48 <.ctors.65535>:
-    646c7e48:	xor    %bh,0x6c(%rsi)
-    646c7e4b:	add    %al,%fs:(%rax)
-	...
-
-00000000646c7e58 <__DTOR_LIST__>:
-    646c7e58:	(bad)
-    646c7e59:	(bad)
-    646c7e5a:	(bad)
-    646c7e5b:	(bad)
-    646c7e5c:	(bad)
-    646c7e5d:	(bad)
-    646c7e5e:	(bad)
-    646c7e5f:	incl   (%rax)
-    646c7e61:	add    %al,(%rax)
-    646c7e63:	add    %al,(%rax)
-    646c7e65:	add    %al,(%rax)
+00000000646c7960 <__mingw_raise_matherr>:
+    646c7960:	sub    $0x58,%rsp
+    646c7964:	mov    0x5205(%rip),%rax        # 646ccb70 <stUserMathErr>
+    646c796b:	test   %rax,%rax
+    646c796e:	je     646c799c <__mingw_raise_matherr+0x3c>
+    646c7970:	movsd  0x80(%rsp),%xmm0
+    646c7979:	mov    %ecx,0x20(%rsp)
+    646c797d:	lea    0x20(%rsp),%rcx
+    646c7982:	mov    %rdx,0x28(%rsp)
+    646c7987:	movsd  %xmm2,0x30(%rsp)
+    646c798d:	movsd  %xmm3,0x38(%rsp)
+    646c7993:	movsd  %xmm0,0x40(%rsp)
+    646c7999:	call   *%rax
+    646c799b:	nop
+    646c799c:	add    $0x58,%rsp
+    646c79a0:	ret
+    646c79a1:	nopl   0x0(%rax,%rax,1)
+    646c79a6:	cs nopw 0x0(%rax,%rax,1)
+
+00000000646c79b0 <__mingw_setusermatherr>:
+    646c79b0:	mov    %rcx,0x51b9(%rip)        # 646ccb70 <stUserMathErr>
+    646c79b7:	jmp    646c7ac0 <__setusermatherr>
+    646c79bc:	nopl   0x0(%rax)
+
+00000000646c79c0 <_matherr>:
+    646c79c0:	push   %rsi
+    646c79c1:	push   %rbx
+    646c79c2:	sub    $0x78,%rsp
+    646c79c6:	movaps %xmm6,0x40(%rsp)
+    646c79cb:	movaps %xmm7,0x50(%rsp)
+    646c79d0:	movaps %xmm8,0x60(%rsp)
+    646c79d6:	cmpl   $0x6,(%rcx)
+    646c79d9:	ja     646c7ab0 <_matherr+0xf0>
+    646c79df:	mov    (%rcx),%eax
+    646c79e1:	lea    0x1bbc(%rip),%rdx        # 646c95a4 <.rdata+0x124>
+    646c79e8:	movslq (%rdx,%rax,4),%rax
+    646c79ec:	add    %rdx,%rax
+    646c79ef:	jmp    *%rax
+    646c79f1:	lea    0x1a88(%rip),%rbx        # 646c9480 <.rdata>
+    646c79f8:	mov    0x8(%rcx),%rsi
+    646c79fc:	movsd  0x20(%rcx),%xmm8
+    646c7a02:	movsd  0x18(%rcx),%xmm7
+    646c7a07:	movsd  0x10(%rcx),%xmm6
+    646c7a0c:	mov    $0x2,%ecx
+    646c7a11:	call   646c7870 <__acrt_iob_func>
+    646c7a16:	movsd  %xmm8,0x30(%rsp)
+    646c7a1d:	mov    %rsi,%r9
+    646c7a20:	mov    %rbx,%r8
+    646c7a23:	movsd  %xmm7,0x28(%rsp)
+    646c7a29:	lea    0x1b48(%rip),%rdx        # 646c9578 <.rdata+0xf8>
+    646c7a30:	mov    %rax,%rcx
+    646c7a33:	movsd  %xmm6,0x20(%rsp)
+    646c7a39:	call   646c76a0 <fprintf>
+    646c7a3e:	nop
+    646c7a3f:	movaps 0x40(%rsp),%xmm6
+    646c7a44:	xor    %eax,%eax
+    646c7a46:	movaps 0x50(%rsp),%xmm7
+    646c7a4b:	movaps 0x60(%rsp),%xmm8
+    646c7a51:	add    $0x78,%rsp
+    646c7a55:	pop    %rbx
+    646c7a56:	pop    %rsi
+    646c7a57:	ret
+    646c7a58:	nopl   0x0(%rax,%rax,1)
+    646c7a60:	lea    0x1a38(%rip),%rbx        # 646c949f <.rdata+0x1f>
+    646c7a67:	jmp    646c79f8 <_matherr+0x38>
+    646c7a69:	nopl   0x0(%rax)
+    646c7a70:	lea    0x1a49(%rip),%rbx        # 646c94c0 <.rdata+0x40>
+    646c7a77:	jmp    646c79f8 <_matherr+0x38>
+    646c7a7c:	nopl   0x0(%rax)
+    646c7a80:	lea    0x1aa9(%rip),%rbx        # 646c9530 <.rdata+0xb0>
+    646c7a87:	jmp    646c79f8 <_matherr+0x38>
+    646c7a8c:	nopl   0x0(%rax)
+    646c7a90:	lea    0x1a71(%rip),%rbx        # 646c9508 <.rdata+0x88>
+    646c7a97:	jmp    646c79f8 <_matherr+0x38>
+    646c7a9c:	nopl   0x0(%rax)
+    646c7aa0:	lea    0x1a39(%rip),%rbx        # 646c94e0 <.rdata+0x60>
+    646c7aa7:	jmp    646c79f8 <_matherr+0x38>
+    646c7aac:	nopl   0x0(%rax)
+    646c7ab0:	lea    0x1aaf(%rip),%rbx        # 646c9566 <.rdata+0xe6>
+    646c7ab7:	jmp    646c79f8 <_matherr+0x38>
+    646c7abc:	nop
+    646c7abd:	nop
+    646c7abe:	nop
+    646c7abf:	nop
+
+00000000646c7ac0 <__setusermatherr>:
+    646c7ac0:	jmp    *0x67c6(%rip)        # 646ce28c <__imp___setusermatherr>
+    646c7ac6:	nop
+    646c7ac7:	nop
+    646c7ac8:	nopl   0x0(%rax,%rax,1)
+
+00000000646c7ad0 <__report_error>:
+    646c7ad0:	push   %rsi
+    646c7ad1:	push   %rbx
+    646c7ad2:	sub    $0x38,%rsp
+    646c7ad6:	lea    0x58(%rsp),%rax
+    646c7adb:	mov    %rcx,%rbx
+    646c7ade:	mov    $0x2,%ecx
+    646c7ae3:	mov    %rdx,0x58(%rsp)
+    646c7ae8:	mov    %r8,0x60(%rsp)
+    646c7aed:	mov    %r9,0x68(%rsp)
+    646c7af2:	mov    %rax,0x28(%rsp)
+    646c7af7:	call   646c7870 <__acrt_iob_func>
+    646c7afc:	mov    $0x1b,%r8d
+    646c7b02:	mov    $0x1,%edx
+    646c7b07:	lea    0x16d2(%rip),%rcx        # 646c91e0 <.rdata>
+    646c7b0e:	mov    %rax,%r9
+    646c7b11:	call   646c7690 <fwrite>
+    646c7b16:	mov    0x28(%rsp),%rsi
+    646c7b1b:	mov    $0x2,%ecx
+    646c7b20:	call   646c7870 <__acrt_iob_func>
+    646c7b25:	mov    %rbx,%rdx
+    646c7b28:	mov    %rax,%rcx
+    646c7b2b:	mov    %rsi,%r8
+    646c7b2e:	call   646c7650 <vfprintf>
+    646c7b33:	call   646c76c8 <abort>
+    646c7b38:	nop
+    646c7b39:	nop
+    646c7b3a:	nop
+    646c7b3b:	nop
+    646c7b3c:	nop
+    646c7b3d:	nop
+    646c7b3e:	nop
+    646c7b3f:	nop
+
+00000000646c7b40 <register_frame_ctor>:
+    646c7b40:	jmp    646c1390 <__gcc_register_frame>
+    646c7b45:	nop
+    646c7b46:	nop
+    646c7b47:	nop
+    646c7b48:	nop
+    646c7b49:	nop
+    646c7b4a:	nop
+    646c7b4b:	nop
+    646c7b4c:	nop
+    646c7b4d:	nop
+    646c7b4e:	nop
+    646c7b4f:	nop
+
+00000000646c7b50 <__CTOR_LIST__>:
+    646c7b50:	(bad)
+    646c7b51:	(bad)
+    646c7b52:	(bad)
+    646c7b53:	(bad)
+    646c7b54:	(bad)
+    646c7b55:	(bad)
+    646c7b56:	(bad)
+    646c7b57:	incl   0x7b(%rax)
+
+00000000646c7b58 <.ctors.65535>:
+    646c7b58:	rex jnp 646c7bc7 <__DTOR_LIST__+0x5f>
+    646c7b5b:	add    %al,%fs:(%rax)
+	...
+
+00000000646c7b68 <__DTOR_LIST__>:
+    646c7b68:	(bad)
+    646c7b69:	(bad)
+    646c7b6a:	(bad)
+    646c7b6b:	(bad)
+    646c7b6c:	(bad)
+    646c7b6d:	(bad)
+    646c7b6e:	(bad)
+    646c7b6f:	incl   (%rax)
+    646c7b71:	add    %al,(%rax)
+    646c7b73:	add    %al,(%rax)
+    646c7b75:	add    %al,(%rax)
 	...
 
 Disassembly of section .data:
 
 00000000646c8000 <__data_start__>:
-    646c8000:	(bad)
-    646c8001:	jle    646c806f <__imp__initialize_onexit_table+0xf>
+    646c8000:	jo     646c807d <__imp___acrt_iob_func+0xd>
+    646c8002:	insb   (%dx),%es:(%rdi)
     646c8003:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8010 <__native_vcclrit_reason>:
     646c8010:	(bad)
     646c8011:	(bad)
     646c8012:	(bad)
@@ -10703,31 +10492,31 @@
     646c8044:	add    %al,(%rax)
     646c8046:	stos   %al,%es:(%rdi)
     646c8047:	mov    $0x3fff,%eax
     646c804c:	add    %al,(%rax)
 	...
 
 00000000646c8050 <__imp__execute_onexit_table>:
-    646c8050:	lock jp 646c80bf <__data_end__+0x1f>
+    646c8050:	add    %bh,0x6c(%rax)
     646c8053:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8058 <__imp__register_onexit_function>:
-    646c8058:	and    %bh,0x6c(%rdx)
+    646c8058:	xor    %dh,0x6c(%rdi)
     646c805b:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8060 <__imp__initialize_onexit_table>:
-    646c8060:	lock jns 646c80cf <__data_end__+0x2f>
+    646c8060:	add    %dh,0x6c(%rdi)
     646c8063:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8070 <__imp___acrt_iob_func>:
-    646c8070:	(bad)
-    646c8071:	jnp    646c80df <__data_end__+0x3f>
+    646c8070:	jo     646c80ea <__data_end__+0x4a>
+    646c8072:	insb   (%dx),%es:(%rdi)
     646c8073:	add    %al,%fs:(%rax)
 	...
 
 00000000646c8080 <__security_cookie>:
     646c8080:	xor    0x2b992ddf(%rdx),%ah
 	...
 
@@ -10853,15 +10642,15 @@
     646c90f7:	jg     646c90f9 <.rdata+0x69>
     646c90f9:	add    %al,(%rax)
     646c90fb:	add    %al,(%rax)
     646c90fd:	add    %al,(%rax)
 	...
 
 00000000646c9100 <.rdata>:
-    646c9100:	rex.WRX jne 646c9170 <.rdata+0x10>
+    646c9100:	rex.WRX jne 646c9170 <GS_ExceptionPointers>
     646c9103:	(bad)
     646c9105:	jb     646c9127 <.rdata+0x27>
     646c9107:	cmp    $0xa642520,%eax
     646c910c:	add    %ch,(%rsi)
     646c910e:	(bad)
     646c910f:	push   %rdx
     646c9110:	gs (bad)
@@ -10874,834 +10663,842 @@
     646c9121:	imul   $0x6e6f6974,0x61(%rdx),%edi
     646c9128:	jae    646c912a <.rdata+0x2a>
     646c912a:	cs (bad)
     646c912c:	push   %rdx
     646c912d:	gs (bad)
     646c912f:	insb   (%dx),%es:(%rdi)
     646c9130:	imul   $0x6e6f6974,0x61(%rdx),%edi
-    646c9137:	jae    646c9168 <.rdata+0x8>
+    646c9137:	jae    646c9168 <.rdata+0x18>
     646c9139:	push   %rsi
     646c913a:	(bad)
-    646c913b:	jb     646c91a6 <__dyn_tls_init_callback+0x6>
+    646c913b:	jb     646c91a6 <_tls_used+0x6>
     646c913d:	outsl  %ds:(%rsi),(%dx)
-    646c913e:	addr32 jb 646c91a2 <__dyn_tls_init_callback+0x2>
+    646c913e:	addr32 jb 646c91a2 <_tls_used+0x2>
     646c9141:	insl   (%dx),%es:(%rdi)
     646c9142:	(bad)
     646c9143:	add    %dl,0x61(%rsi)
-    646c9146:	jb     646c91b1 <__dyn_tls_init_callback+0x11>
+    646c9146:	jb     646c91b1 <_tls_used+0x11>
     646c9148:	outsl  %ds:(%rsi),(%dx)
-    646c9149:	addr32 jb 646c91ad <__dyn_tls_init_callback+0xd>
+    646c9149:	addr32 jb 646c91ad <_tls_used+0xd>
     646c914c:	insl   (%dx),%es:(%rdi)
-	...
-    646c9155:	add    %dh,%al
-    646c9157:	mov    $0x0,%edi
-    646c915c:	add    %al,(%rax)
+    646c914d:	add    %al,(%rax)
 	...
 
-00000000646c9160 <.rdata>:
-    646c9160:	add    %al,(%rax)
+00000000646c9150 <.rdata>:
+    646c9150:	add    %al,(%rax)
+    646c9152:	add    %al,(%rax)
+    646c9154:	add    %al,(%rax)
+    646c9156:	lock (bad)
+    646c9158:	(bad)
+    646c9159:	in     (%dx),%eax
+    646c915a:	mov    $0xa0,%ch
+    646c915c:	test   $0x3eb0,%esi
     646c9162:	add    %al,(%rax)
     646c9164:	add    %al,(%rax)
     646c9166:	add    %al,0x0(%rax)
     646c9169:	add    %al,(%rax)
     646c916b:	add    %al,(%rax)
-    646c916d:	add    %dh,%al
-    646c916f:	(bad)
-    646c9170:	(bad)
-    646c9171:	in     (%dx),%eax
-    646c9172:	mov    $0xa0,%ch
-    646c9174:	test   $0x3eb0,%esi
-    646c917a:	add    %al,(%rax)
-    646c917c:	add    %al,(%rax)
+    646c916d:	add    %al,(%rax)
 	...
 
-00000000646c9180 <GS_ExceptionPointers>:
-    646c9180:	add    $0x6c,%bh
+00000000646c9170 <GS_ExceptionPointers>:
+    646c9170:	add    $0x6c,%bh
+    646c9173:	add    %al,%fs:(%rax)
+    646c9176:	add    %al,(%rax)
+    646c9178:	movabs 0x9000000000646cc2,%al
+
+00000000646c9180 <__dyn_tls_init_callback>:
+    646c9180:	nop
+    646c9181:	push   %rsp
+    646c9182:	insb   (%dx),%es:(%rdi)
     646c9183:	add    %al,%fs:(%rax)
-    646c9186:	add    %al,(%rax)
-    646c9188:	movabs 0x646cc2,%al
 	...
 
-00000000646c91a0 <__dyn_tls_init_callback>:
-    646c91a0:	adcb   $0x64,0x6c(%rdi)
-	...
-
-00000000646c91c0 <_tls_used>:
-    646c91c0:	add    %al,(%rax)
-    646c91c2:	insl   (%dx),%es:(%rdi)
-    646c91c3:	add    %al,%fs:(%rax)
-    646c91c6:	add    %al,(%rax)
-    646c91c8:	or     %al,(%rax)
-    646c91ca:	insl   (%dx),%es:(%rdi)
-    646c91cb:	add    %al,%fs:(%rax)
-    646c91ce:	add    %al,(%rax)
-    646c91d0:	sub    $0xc8,%al
-    646c91d2:	insb   (%dx),%es:(%rdi)
-    646c91d3:	add    %al,%fs:(%rax)
-    646c91d6:	add    %al,(%rax)
-    646c91d8:	xor    %dh,%al
-    646c91da:	insb   (%dx),%es:(%rdi)
-    646c91db:	add    %al,%fs:(%rax)
-	...
-
-00000000646c9200 <.rdata>:
-    646c9200:	imul   $0x36772d77,0x67(%r14),%r13
-    646c9208:	xor    $0x20,%al
-    646c920a:	jb     646c9281 <.rdata+0x81>
-    646c920c:	outsb  %ds:(%rsi),(%dx)
-    646c920d:	je     646c9278 <.rdata+0x78>
-    646c920f:	insl   (%dx),%es:(%rdi)
-    646c9210:	and    %ah,%gs:0x61(%rsi)
-    646c9214:	imul   $0xa3a65,0x72(%rbp,%rsi,2),%ebp
-    646c921c:	add    %al,(%rax)
-    646c921e:	add    %al,(%rax)
-    646c9220:	rex.B
-    646c9221:	fs fs jb 646c928a <.rdata+0x8a>
-    646c9225:	jae    646c929a <.rdata+0x9a>
-    646c9227:	and    %ah,0x61682070(%rip)        # c5d4b29d <.debug_str+0x6167329d>
-    646c922d:	jae    646c924f <.rdata+0x4f>
-    646c922f:	outsb  %ds:(%rsi),(%dx)
-    646c9230:	outsl  %ds:(%rsi),(%dx)
-    646c9231:	and    %ch,0x6d(%rcx)
-    646c9234:	(bad)
-    646c9235:	addr32 gs sub $0x74636573,%eax
-    646c923c:	imul   $0x56202000,0x6e(%rdi),%ebp
-    646c9243:	imul   $0x516c6175,0x74(%rdx),%esi
-    646c924a:	jne    646c92b1 <.rdata+0xb1>
-    646c924c:	jb     646c92c7 <.rdata+0xc7>
-    646c924e:	and    %ah,0x61(%rsi)
-    646c9251:	imul   $0x726f6620,0x64(%rbp,%riz,2),%ebp
-    646c9259:	and    %ah,0x79622064(%rip)        # ddceb2c3 <.debug_str+0x796132c3>
-    646c925f:	je     646c92c6 <.rdata+0xc6>
-    646c9261:	jae    646c9283 <.rdata+0x83>
-    646c9263:	(bad)
-    646c9264:	je     646c9286 <.rdata+0x86>
-    646c9266:	(bad)
-    646c9267:	fs fs jb 646c92d0 <.rdata+0xd0>
-    646c926b:	jae    646c92e0 <.rdata+0xe0>
-    646c926d:	and    %ah,0x70(%rip)        # 646c92e3 <.rdata+0xe3>
-    646c9273:	add    %al,(%rax)
-    646c9275:	add    %al,(%rax)
-    646c9277:	add    %ah,(%rax)
-    646c9279:	and    %dl,0x69(%rsi)
-    646c927c:	jb     646c92f2 <.rdata+0xf2>
-    646c927e:	jne    646c92e1 <.rdata+0xe1>
-    646c9280:	insb   (%dx),%es:(%rdi)
-    646c9281:	push   %rax
-    646c9282:	jb     646c92f3 <.rdata+0xf3>
-    646c9284:	je     646c92eb <.rdata+0xeb>
-    646c9286:	movsxd 0x66(%rax,%riz,1),%esi
-    646c928a:	(bad)
-    646c928b:	imul   $0x74697720,0x64(%rbp,%riz,2),%ebp
-    646c9293:	push   $0x646f6320
-    646c9298:	and    %dh,%gs:(%rax)
-    646c929b:	js     646c92c2 <.rdata+0xc2>
-    646c929d:	js     646c929f <.rdata+0x9f>
-    646c929f:	add    %ah,(%rax)
-    646c92a1:	and    %dl,0x6e(%rbp)
-    646c92a4:	imul   $0x77,0x6f(%rsi),%ebp
-    646c92a8:	outsb  %ds:(%rsi),(%dx)
-    646c92a9:	and    %dh,0x73(%rax)
-    646c92ac:	gs jne 646c9313 <.rdata+0x3>
-    646c92af:	outsl  %ds:(%rsi),(%dx)
-    646c92b0:	and    %dh,0x65(%rdx)
-    646c92b3:	insb   (%dx),%es:(%rdi)
-    646c92b4:	outsl  %ds:(%rsi),(%dx)
-    646c92b5:	movsxd 0x74(%rcx),%esp
-    646c92b8:	imul   $0x6f727020,0x6e(%rdi),%ebp
-    646c92bf:	je     646c9330 <.rdata+0x10>
-    646c92c1:	movsxd 0x6c(%rdi),%ebp
-    646c92c4:	and    %dh,0x65(%rsi)
-    646c92c7:	jb     646c933c <.rdata+0x1c>
-    646c92c9:	imul   $0x2e642520,0x6e(%rdi),%ebp
-    646c92d0:	or     (%rax),%al
-    646c92d2:	add    %al,(%rax)
-    646c92d4:	add    %al,(%rax)
-    646c92d6:	add    %al,(%rax)
-    646c92d8:	and    %ah,(%rax)
-    646c92da:	push   %rbp
-    646c92db:	outsb  %ds:(%rsi),(%dx)
-    646c92dc:	imul   $0x77,0x6f(%rsi),%ebp
-    646c92e0:	outsb  %ds:(%rsi),(%dx)
-    646c92e1:	and    %dh,0x73(%rax)
-    646c92e4:	gs jne 646c934b <.rdata+0x2b>
-    646c92e7:	outsl  %ds:(%rsi),(%dx)
-    646c92e8:	and    %dh,0x65(%rdx)
-    646c92eb:	insb   (%dx),%es:(%rdi)
-    646c92ec:	outsl  %ds:(%rsi),(%dx)
-    646c92ed:	movsxd 0x74(%rcx),%esp
-    646c92f0:	imul   $0x74696220,0x6e(%rdi),%ebp
-    646c92f7:	and    %dh,0x69(%rbx)
-    646c92fa:	jp     646c9361 <.rdata+0x1>
-    646c92fc:	and    %ah,0xa2e64(%rip)        # 6476c166 <.debug_str+0x94166>
-	...
-
-00000000646c9310 <.rdata>:
-    646c9310:	jo,pn  646c9377 <.rdata+0x7>
-    646c9313:	(bad)
-    646c9314:	je     646c9377 <.rdata+0x7>
-	...
-
-00000000646c9320 <.rdata>:
-    646c9320:	jae    646c9393 <.rdata+0x23>
-    646c9322:	jb     646c9398 <.rdata+0x28>
-	...
-    646c932c:	add    %al,(%rax)
-    646c932e:	add    %al,0x0(%rax)
-    646c9334:	add    %al,(%rax)
-    646c9336:	clc
-    646c9337:	incl   (%rax)
-    646c9339:	add    %al,(%rax)
-    646c933b:	add    %al,(%rax)
-    646c933d:	add    %dh,%al
-    646c933f:	jg     646c9341 <.rdata+0x21>
-    646c9341:	add    %al,(%rax)
-    646c9343:	add    %al,(%rax)
-    646c9345:	add    %dh,%al
-    646c9347:	(bad)
-	...
-
-00000000646c9350 <.huge>:
-    646c9350:	pushf
-    646c9351:	jne    646c9353 <.huge+0x3>
-    646c9353:	mov    %bh,(%rsp,%riz,8)
-    646c9356:	(bad)
-    646c9357:	jle    646c9359 <.zero+0x1>
-
-00000000646c9358 <.zero>:
-	...
-
-00000000646c9360 <.rdata>:
-    646c9360:	movsxd 0x73(%rdi),%ebp
-	...
-    646c936b:	add    %al,(%rax)
-    646c936d:	add    %bh,%al
-    646c936f:	jg     646c93d6 <.rdata+0x16>
-
-00000000646c9370 <.rdata>:
-    646c9370:	gs js  646c93e3 <.rdata+0x23>
-	...
-    646c937b:	add    %al,(%rax)
-    646c937d:	add    %dh,%al
-    646c937f:	jg     646c9381 <.rdata+0x11>
-    646c9381:	add    %al,(%rax)
-    646c9383:	add    %al,(%rax)
-    646c9385:	add    %dh,%al
-    646c9387:	(bad)
-    646c9388:	out    %eax,(%dx)
-    646c9389:	cmp    %edi,%edx
-    646c938b:	incb   0x2e(%rdx)
-    646c938e:	xchg   %al,0x51(%rax)
-    646c9391:	xor    %ch,-0x78b6ef2b(%rip)        # ffffffffebb5a46c <.debug_str+0xffffffff8748246c>
-    646c9397:	rolb   $0x0,(%rax)
-    646c939a:	add    %al,(%rax)
-    646c939c:	add    %al,(%rax)
-	...
+00000000646c91a0 <_tls_used>:
+    646c91a0:	add    %al,(%rax)
+    646c91a2:	insl   (%dx),%es:(%rdi)
+    646c91a3:	add    %al,%fs:(%rax)
+    646c91a6:	add    %al,(%rax)
+    646c91a8:	or     %al,(%rax)
+    646c91aa:	insl   (%dx),%es:(%rdi)
+    646c91ab:	add    %al,%fs:(%rax)
+    646c91ae:	add    %al,(%rax)
+    646c91b0:	sub    $0xc8,%al
+    646c91b2:	insb   (%dx),%es:(%rdi)
+    646c91b3:	add    %al,%fs:(%rax)
+    646c91b6:	add    %al,(%rax)
+    646c91b8:	xor    %dh,%al
+    646c91ba:	insb   (%dx),%es:(%rdi)
+    646c91bb:	add    %al,%fs:(%rax)
+	...
+
+00000000646c91e0 <.rdata>:
+    646c91e0:	imul   $0x36772d77,0x67(%r14),%r13
+    646c91e8:	xor    $0x20,%al
+    646c91ea:	jb     646c9261 <.rdata+0x81>
+    646c91ec:	outsb  %ds:(%rsi),(%dx)
+    646c91ed:	je     646c9258 <.rdata+0x78>
+    646c91ef:	insl   (%dx),%es:(%rdi)
+    646c91f0:	and    %ah,%gs:0x61(%rsi)
+    646c91f4:	imul   $0xa3a65,0x72(%rbp,%rsi,2),%ebp
+    646c91fc:	add    %al,(%rax)
+    646c91fe:	add    %al,(%rax)
+    646c9200:	rex.B
+    646c9201:	fs fs jb 646c926a <.rdata+0x8a>
+    646c9205:	jae    646c927a <.rdata+0x9a>
+    646c9207:	and    %ah,0x61682070(%rip)        # c5d4b27d <.debug_str+0x6167327d>
+    646c920d:	jae    646c922f <.rdata+0x4f>
+    646c920f:	outsb  %ds:(%rsi),(%dx)
+    646c9210:	outsl  %ds:(%rsi),(%dx)
+    646c9211:	and    %ch,0x6d(%rcx)
+    646c9214:	(bad)
+    646c9215:	addr32 gs sub $0x74636573,%eax
+    646c921c:	imul   $0x56202000,0x6e(%rdi),%ebp
+    646c9223:	imul   $0x516c6175,0x74(%rdx),%esi
+    646c922a:	jne    646c9291 <.rdata+0xb1>
+    646c922c:	jb     646c92a7 <.rdata+0xc7>
+    646c922e:	and    %ah,0x61(%rsi)
+    646c9231:	imul   $0x726f6620,0x64(%rbp,%riz,2),%ebp
+    646c9239:	and    %ah,0x79622064(%rip)        # ddceb2a3 <.debug_str+0x796132a3>
+    646c923f:	je     646c92a6 <.rdata+0xc6>
+    646c9241:	jae    646c9263 <.rdata+0x83>
+    646c9243:	(bad)
+    646c9244:	je     646c9266 <.rdata+0x86>
+    646c9246:	(bad)
+    646c9247:	fs fs jb 646c92b0 <.rdata+0xd0>
+    646c924b:	jae    646c92c0 <.rdata+0xe0>
+    646c924d:	and    %ah,0x70(%rip)        # 646c92c3 <.rdata+0xe3>
+    646c9253:	add    %al,(%rax)
+    646c9255:	add    %al,(%rax)
+    646c9257:	add    %ah,(%rax)
+    646c9259:	and    %dl,0x69(%rsi)
+    646c925c:	jb     646c92d2 <.rdata+0xf2>
+    646c925e:	jne    646c92c1 <.rdata+0xe1>
+    646c9260:	insb   (%dx),%es:(%rdi)
+    646c9261:	push   %rax
+    646c9262:	jb     646c92d3 <.rdata+0xf3>
+    646c9264:	je     646c92cb <.rdata+0xeb>
+    646c9266:	movsxd 0x66(%rax,%riz,1),%esi
+    646c926a:	(bad)
+    646c926b:	imul   $0x74697720,0x64(%rbp,%riz,2),%ebp
+    646c9273:	push   $0x646f6320
+    646c9278:	and    %dh,%gs:(%rax)
+    646c927b:	js     646c92a2 <.rdata+0xc2>
+    646c927d:	js     646c927f <.rdata+0x9f>
+    646c927f:	add    %ah,(%rax)
+    646c9281:	and    %dl,0x6e(%rbp)
+    646c9284:	imul   $0x77,0x6f(%rsi),%ebp
+    646c9288:	outsb  %ds:(%rsi),(%dx)
+    646c9289:	and    %dh,0x73(%rax)
+    646c928c:	gs jne 646c92f3 <.rdata+0x3>
+    646c928f:	outsl  %ds:(%rsi),(%dx)
+    646c9290:	and    %dh,0x65(%rdx)
+    646c9293:	insb   (%dx),%es:(%rdi)
+    646c9294:	outsl  %ds:(%rsi),(%dx)
+    646c9295:	movsxd 0x74(%rcx),%esp
+    646c9298:	imul   $0x6f727020,0x6e(%rdi),%ebp
+    646c929f:	je     646c9310 <.rdata+0x10>
+    646c92a1:	movsxd 0x6c(%rdi),%ebp
+    646c92a4:	and    %dh,0x65(%rsi)
+    646c92a7:	jb     646c931c <.rdata+0x1c>
+    646c92a9:	imul   $0x2e642520,0x6e(%rdi),%ebp
+    646c92b0:	or     (%rax),%al
+    646c92b2:	add    %al,(%rax)
+    646c92b4:	add    %al,(%rax)
+    646c92b6:	add    %al,(%rax)
+    646c92b8:	and    %ah,(%rax)
+    646c92ba:	push   %rbp
+    646c92bb:	outsb  %ds:(%rsi),(%dx)
+    646c92bc:	imul   $0x77,0x6f(%rsi),%ebp
+    646c92c0:	outsb  %ds:(%rsi),(%dx)
+    646c92c1:	and    %dh,0x73(%rax)
+    646c92c4:	gs jne 646c932b <.rdata+0x2b>
+    646c92c7:	outsl  %ds:(%rsi),(%dx)
+    646c92c8:	and    %dh,0x65(%rdx)
+    646c92cb:	insb   (%dx),%es:(%rdi)
+    646c92cc:	outsl  %ds:(%rsi),(%dx)
+    646c92cd:	movsxd 0x74(%rcx),%esp
+    646c92d0:	imul   $0x74696220,0x6e(%rdi),%ebp
+    646c92d7:	and    %dh,0x69(%rbx)
+    646c92da:	jp     646c9341 <.rdata+0x1>
+    646c92dc:	and    %ah,0xa2e64(%rip)        # 6476c146 <.debug_str+0x94146>
+	...
+
+00000000646c92f0 <.rdata>:
+    646c92f0:	jo,pn  646c9357 <.rdata+0x7>
+    646c92f3:	(bad)
+    646c92f4:	je     646c9357 <.rdata+0x7>
+	...
+
+00000000646c9300 <.rdata>:
+    646c9300:	jae    646c9373 <.rdata+0x23>
+    646c9302:	jb     646c9378 <.rdata+0x28>
+	...
+    646c930c:	add    %al,(%rax)
+    646c930e:	add    %al,0x0(%rax)
+    646c9314:	add    %al,(%rax)
+    646c9316:	clc
+    646c9317:	incl   (%rax)
+    646c9319:	add    %al,(%rax)
+    646c931b:	add    %al,(%rax)
+    646c931d:	add    %dh,%al
+    646c931f:	jg     646c9321 <.rdata+0x21>
+    646c9321:	add    %al,(%rax)
+    646c9323:	add    %al,(%rax)
+    646c9325:	add    %dh,%al
+    646c9327:	(bad)
+	...
+
+00000000646c9330 <.huge>:
+    646c9330:	pushf
+    646c9331:	jne    646c9333 <.huge+0x3>
+    646c9333:	mov    %bh,(%rsp,%riz,8)
+    646c9336:	(bad)
+    646c9337:	jle    646c9339 <.zero+0x1>
+
+00000000646c9338 <.zero>:
+	...
+
+00000000646c9340 <.rdata>:
+    646c9340:	movsxd 0x73(%rdi),%ebp
+	...
+    646c934b:	add    %al,(%rax)
+    646c934d:	add    %bh,%al
+    646c934f:	jg     646c93b6 <.rdata+0x16>
+
+00000000646c9350 <.rdata>:
+    646c9350:	gs js  646c93c3 <.rdata+0x23>
+	...
+    646c935b:	add    %al,(%rax)
+    646c935d:	add    %dh,%al
+    646c935f:	jg     646c9361 <.rdata+0x11>
+    646c9361:	add    %al,(%rax)
+    646c9363:	add    %al,(%rax)
+    646c9365:	add    %dh,%al
+    646c9367:	(bad)
+    646c9368:	out    %eax,(%dx)
+    646c9369:	cmp    %edi,%edx
+    646c936b:	incb   0x2e(%rdx)
+    646c936e:	xchg   %al,0x51(%rax)
+    646c9371:	xor    %ch,-0x78b6ef2b(%rip)        # ffffffffebb5a44c <.debug_str+0xffffffff8748244c>
+    646c9377:	rolb   $0x0,(%rax)
+    646c937a:	add    %al,(%rax)
+    646c937c:	add    %al,(%rax)
+	...
+
+00000000646c9380 <.rdata>:
+    646c9380:	insb   (%dx),%es:(%rdi)
+    646c9381:	outsl  %ds:(%rsi),(%dx)
+    646c9382:	add    %al,(%eax)
+	...
+    646c938d:	add    %dh,%al
+    646c938f:	incl   (%rax)
+    646c9391:	add    %al,(%rax)
+    646c9393:	add    %al,(%rax)
+    646c9395:	add    %bh,%al
+    646c9397:	jg     646c9399 <.rdata+0x19>
+    646c9399:	add    %al,(%rax)
+    646c939b:	add    %al,(%rax)
+    646c939d:	add    %dh,%al
+    646c939f:	jg     646c9411 <.rdata+0x71>
 
 00000000646c93a0 <.rdata>:
-    646c93a0:	insb   (%dx),%es:(%rdi)
-    646c93a1:	outsl  %ds:(%rsi),(%dx)
-    646c93a2:	add    %al,(%eax)
+    646c93a0:	jo     646c9411 <.rdata+0x71>
+    646c93a2:	ja     646c93a4 <.rdata+0x4>
 	...
-    646c93ad:	add    %dh,%al
+    646c93ac:	add    %al,(%rax)
+    646c93ae:	clc
     646c93af:	incl   (%rax)
     646c93b1:	add    %al,(%rax)
     646c93b3:	add    %al,(%rax)
     646c93b5:	add    %bh,%al
     646c93b7:	jg     646c93b9 <.rdata+0x19>
     646c93b9:	add    %al,(%rax)
     646c93bb:	add    %al,(%rax)
-    646c93bd:	add    %dh,%al
-    646c93bf:	jg     646c9431 <.rdata+0x71>
-
-00000000646c93c0 <.rdata>:
-    646c93c0:	jo     646c9431 <.rdata+0x71>
-    646c93c2:	ja     646c93c4 <.rdata+0x4>
-	...
-    646c93cc:	add    %al,(%rax)
-    646c93ce:	clc
-    646c93cf:	incl   (%rax)
+    646c93bd:	add    %al,(%rax)
+    646c93bf:	addb   $0x0,(%rax)
+    646c93c2:	add    %al,(%rax)
+    646c93c4:	add    %al,(%rax)
+    646c93c6:	lock incl (%rax)
+    646c93c9:	add    %al,(%rax)
+    646c93cb:	add    %al,(%rax)
+    646c93cd:	add    %dh,%al
+    646c93cf:	jg     646c93d1 <.rdata+0x31>
     646c93d1:	add    %al,(%rax)
     646c93d3:	add    %al,(%rax)
-    646c93d5:	add    %bh,%al
-    646c93d7:	jg     646c93d9 <.rdata+0x19>
-    646c93d9:	add    %al,(%rax)
-    646c93db:	add    %al,(%rax)
-    646c93dd:	add    %al,(%rax)
-    646c93df:	addb   $0x0,(%rax)
-    646c93e2:	add    %al,(%rax)
+    646c93d5:	add    %dh,%al
+    646c93d7:	(bad)
+	...
     646c93e4:	add    %al,(%rax)
-    646c93e6:	lock incl (%rax)
-    646c93e9:	add    %al,(%rax)
-    646c93eb:	add    %al,(%rax)
-    646c93ed:	add    %dh,%al
-    646c93ef:	jg     646c93f1 <.rdata+0x31>
-    646c93f1:	add    %al,(%rax)
-    646c93f3:	add    %al,(%rax)
-    646c93f5:	add    %dh,%al
-    646c93f7:	(bad)
-	...
-    646c9404:	add    %al,(%rax)
-    646c9406:	add    %al,0x0(%rax)
-	...
-    646c9414:	add    %al,(%rax)
-    646c9416:	lock mov $0x0,%edi
-    646c941c:	add    %al,(%rax)
-    646c941e:	loopne 646c945f <.rdata+0x1f>
-    646c9420:	add    %al,(%rax)
-    646c9422:	sar    $0xff,%bh
-    646c9425:	(bad)
-    646c9426:	filds  0x0(%rcx)
-    646c9429:	add    %al,(%rax)
-    646c942b:	add    %al,(%rax)
-    646c942d:	add    %ah,%al
-    646c942f:	sar    $0xff,%edi
-    646c9432:	(bad)
-    646c9433:	(bad)
-    646c9434:	(bad)
-    646c9435:	(bad)
-    646c9436:	(bad)
-    646c9437:	jg     646c9439 <.rdata+0x79>
+    646c93e6:	add    %al,0x0(%rax)
+	...
+    646c93f4:	add    %al,(%rax)
+    646c93f6:	lock mov $0x0,%edi
+    646c93fc:	add    %al,(%rax)
+    646c93fe:	loopne 646c943f <.rdata+0x1f>
+    646c9400:	add    %al,(%rax)
+    646c9402:	sar    $0xff,%bh
+    646c9405:	(bad)
+    646c9406:	filds  0x0(%rcx)
+    646c9409:	add    %al,(%rax)
+    646c940b:	add    %al,(%rax)
+    646c940d:	add    %ah,%al
+    646c940f:	sar    $0xff,%edi
+    646c9412:	(bad)
+    646c9413:	(bad)
+    646c9414:	(bad)
+    646c9415:	(bad)
+    646c9416:	(bad)
+    646c9417:	jg     646c9419 <.rdata+0x79>
+    646c9419:	add    %al,(%rax)
+    646c941b:	add    %al,(%rax)
+    646c941d:	add    %al,(%rax)
+	...
+
+00000000646c9420 <.rdata>:
+    646c9420:	pop    %rdi
+    646c9421:	pop    %rdi
+    646c9422:	jo     646c9493 <.rdata+0x13>
+    646c9424:	ja     646c948f <.rdata+0xf>
+	...
+    646c942e:	clc
+    646c942f:	incl   (%rax)
+    646c9431:	add    %al,(%rax)
+    646c9433:	add    %al,(%rax)
+    646c9435:	add    %bh,%al
+    646c9437:	jg     646c9439 <.rdata+0x19>
     646c9439:	add    %al,(%rax)
     646c943b:	add    %al,(%rax)
-    646c943d:	add    %al,(%rax)
-	...
-
-00000000646c9440 <.rdata>:
-    646c9440:	pop    %rdi
-    646c9441:	pop    %rdi
-    646c9442:	jo     646c94b3 <.rdata+0x13>
-    646c9444:	ja     646c94af <.rdata+0xf>
-	...
-    646c944e:	clc
-    646c944f:	incl   (%rax)
+    646c943d:	add    %dh,%al
+    646c943f:	(bad)
+    646c9440:	add    %al,(%rax)
+    646c9442:	add    %al,(%rax)
+    646c9444:	add    %al,(%rax)
+    646c9446:	add    %al,0x0(%rax)
+    646c944c:	add    %al,(%rax)
+    646c944e:	lock jg 646c9451 <.rdata+0x31>
     646c9451:	add    %al,(%rax)
     646c9453:	add    %al,(%rax)
-    646c9455:	add    %bh,%al
-    646c9457:	jg     646c9459 <.rdata+0x19>
+    646c9455:	add    %dh,%al
+    646c9457:	incl   (%rax)
     646c9459:	add    %al,(%rax)
     646c945b:	add    %al,(%rax)
-    646c945d:	add    %dh,%al
-    646c945f:	(bad)
-    646c9460:	add    %al,(%rax)
-    646c9462:	add    %al,(%rax)
-    646c9464:	add    %al,(%rax)
-    646c9466:	add    %al,0x0(%rax)
-    646c946c:	add    %al,(%rax)
-    646c946e:	lock jg 646c9471 <.rdata+0x31>
-    646c9471:	add    %al,(%rax)
-    646c9473:	add    %al,(%rax)
-    646c9475:	add    %dh,%al
-    646c9477:	incl   (%rax)
-    646c9479:	add    %al,(%rax)
-    646c947b:	add    %al,(%rax)
-    646c947d:	add    %al,(%rax)
-    646c947f:	add    %bh,%bh
-    646c9481:	(bad)
-    646c9482:	(bad)
-    646c9483:	(bad)
-    646c9484:	(bad)
-    646c9485:	(bad)
-    646c9486:	(bad)
-    646c9487:	jg     646c9489 <.rdata+0x49>
-	...
-    646c9495:	add    %al,(%rax)
-    646c9497:	addb   $0x0,(%rax)
-    646c949a:	add    %al,(%rax)
-    646c949c:	add    %al,(%rax)
-	...
-
-00000000646c94a0 <.rdata>:
-    646c94a0:	rex.B jb 646c950a <.rdata+0x6a>
-    646c94a3:	jne    646c9512 <.rdata+0x72>
-    646c94a5:	outsb  %gs:(%rsi),(%dx)
-    646c94a7:	je     646c94c9 <.rdata+0x29>
-    646c94a9:	outsl  %fs:(%rsi),(%dx)
-    646c94ab:	insl   (%dx),%es:(%rdi)
-    646c94ac:	(bad)
-    646c94ad:	imul   $0x6f727265,0x20(%rsi),%ebp
-    646c94b4:	jb     646c94d6 <.rdata+0x36>
-    646c94b6:	sub    %al,0x4d(%rdi,%rcx,2)
-    646c94ba:	rex.B
-    646c94bb:	rex.WB
-    646c94bc:	rex.WRX sub %r8,(%rax)
-    646c94bf:	rex.B jb 646c9529 <.rdata+0x89>
-    646c94c2:	jne    646c9531 <.rdata+0x91>
-    646c94c4:	outsb  %gs:(%rsi),(%dx)
-    646c94c6:	je     646c94e8 <.rdata+0x48>
-    646c94c8:	jae    646c9533 <.rdata+0x93>
-    646c94ca:	outsb  %ds:(%rsi),(%dx)
-    646c94cb:	addr32 jne 646c953a <.rdata+0x9a>
-    646c94ce:	(bad)
-    646c94cf:	jb     646c953a <.rdata+0x9a>
-    646c94d1:	je     646c954c <.rdata+0xac>
-    646c94d3:	and    %ch,(%rax)
-    646c94d5:	push   %rbx
-    646c94d6:	rex.WB
-    646c94d7:	rex.RXB
-    646c94d8:	rex.WRX sub %r8,(%rax)
-    646c94db:	add    %al,(%rax)
-    646c94dd:	add    %al,(%rax)
-    646c94df:	add    %cl,0x76(%rdi)
-    646c94e2:	gs jb  646c954b <.rdata+0xab>
-    646c94e5:	insb   (%dx),%es:(%rdi)
-    646c94e6:	outsl  %ds:(%rsi),(%dx)
-    646c94e7:	ja     646c9509 <.rdata+0x69>
-    646c94e9:	jb     646c954c <.rdata+0xac>
-    646c94eb:	outsb  %ds:(%rsi),(%dx)
-    646c94ec:	and    %ah,%gs:0x72(%ebp)
-    646c94f1:	jb     646c9562 <.rdata+0xc2>
-    646c94f3:	jb     646c9515 <.rdata+0x75>
-    646c94f5:	sub    %cl,0x56(%rdi)
-    646c94f8:	rex.RB push %r10
-    646c94fa:	rex.RX
-    646c94fb:	rex.WR
-    646c94fc:	rex.WRXB push %r15
-    646c94fe:	sub    %eax,(%rax)
-    646c9500:	push   %rax
-    646c9501:	(bad)
-    646c9502:	jb     646c9578 <.rdata+0xd8>
-    646c9504:	imul   $0x736f6c20,0x6c(%rcx),%esp
-    646c950b:	jae    646c952d <.rdata+0x8d>
-    646c950d:	outsl  %ds:(%rsi),(%dx)
-    646c950e:	data16 and %dh,0x69(%rbx)
-    646c9512:	outsb  %ds:(%esi),(%dx)
-    646c9514:	imul   $0x636e6163,0x69(%rsi),%esp
-    646c951b:	and    %ch,%gs:(%rax)
-    646c951e:	push   %rax
-    646c951f:	rex.WR
-    646c9520:	rex.WRXB push %r11
-    646c9522:	push   %rbx
-    646c9523:	sub    %eax,(%rax)
-    646c9525:	add    %al,(%rax)
-    646c9527:	add    %dl,0x74(%rdi,%rbp,2)
-    646c952b:	(bad)
-    646c952c:	insb   (%dx),%es:(%rdi)
-    646c952d:	and    %ch,0x73(%rdi,%rbp,2)
-    646c9531:	jae    646c9553 <.rdata+0xb3>
-    646c9533:	outsl  %ds:(%rsi),(%dx)
-    646c9534:	data16 and %dh,0x69(%rbx)
-    646c9538:	outsb  %ds:(%esi),(%dx)
-    646c953a:	imul   $0x636e6163,0x69(%rsi),%esp
-    646c9541:	and    %ch,%gs:(%rax)
-    646c9544:	push   %rsp
-    646c9545:	rex.WR
-    646c9546:	rex.WRXB push %r11
-    646c9548:	push   %rbx
-    646c9549:	sub    %eax,(%rax)
-    646c954b:	add    %al,(%rax)
-    646c954d:	add    %al,(%rax)
-    646c954f:	add    %dl,0x65(%rax,%rbp,2)
-    646c9553:	and    %dh,0x65(%rdx)
-    646c9556:	jae    646c95cd <.rdata+0x12d>
-    646c9558:	insb   (%dx),%es:(%rdi)
-    646c9559:	je     646c957b <.rdata+0xdb>
-    646c955b:	imul   $0x206f6f74,0x20(%rbx),%esi
-    646c9562:	jae    646c95d1 <.rdata+0x131>
-    646c9564:	(bad)
-    646c9565:	insb   (%dx),%es:(%rdi)
-    646c9566:	insb   (%dx),%es:(%rdi)
-    646c9567:	and    %dh,0x20(%rdi,%rbp,2)
-    646c956b:	(bad)
-    646c956d:	and    %dh,0x65(%rdx)
-    646c9570:	jo     646c95e4 <.refptr._CRT_MT+0x4>
-    646c9572:	gs jae 646c95da <.rdata+0x13a>
-    646c9575:	outsb  %ds:(%rsi),(%dx)
-    646c9576:	je     646c95dd <.rdata+0x13d>
-    646c9578:	and    %ch,%fs:(%rax)
-    646c957b:	push   %rbp
-    646c957c:	rex.WRX
-    646c957d:	rex.R
-    646c957e:	rex.RB push %r10
-    646c9580:	rex.RX
-    646c9581:	rex.WR
-    646c9582:	rex.WRXB push %r15
-    646c9584:	sub    %eax,(%rax)
-    646c9586:	push   %rbp
-    646c9587:	outsb  %ds:(%rsi),(%dx)
-    646c9588:	imul   $0x77,0x6f(%rsi),%ebp
-    646c958c:	outsb  %ds:(%rsi),(%dx)
-    646c958d:	and    %ah,0x72(%rbp)
-    646c9590:	jb     646c9601 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__+0x1>
-    646c9592:	jb     646c9594 <.rdata+0xf4>
-    646c9594:	add    %al,(%rax)
-    646c9596:	add    %al,(%rax)
-    646c9598:	pop    %rdi
-    646c9599:	insl   (%dx),%es:(%rdi)
-    646c959a:	(bad)
-    646c959b:	je     646c9605 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__+0x5>
-    646c959d:	gs jb  646c9612 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__+0x2>
-    646c95a0:	sub    %ch,(%rcx)
-    646c95a2:	cmp    (%rax),%ah
-    646c95a4:	and    $0x6e692073,%eax
-    646c95a9:	and    %ah,0x67252873(%rip)        # cb91be22 <.debug_str+0x67243e22>
-    646c95af:	sub    $0x20,%al
-    646c95b1:	and    $0x20202967,%eax
-    646c95b6:	sub    %dh,0x65(%rdx)
-    646c95b9:	je     646c9631 <.refptr.__image_base__+0x1>
+    646c945d:	add    %al,(%rax)
+    646c945f:	add    %bh,%bh
+    646c9461:	(bad)
+    646c9462:	(bad)
+    646c9463:	(bad)
+    646c9464:	(bad)
+    646c9465:	(bad)
+    646c9466:	(bad)
+    646c9467:	jg     646c9469 <.rdata+0x49>
+	...
+    646c9475:	add    %al,(%rax)
+    646c9477:	addb   $0x0,(%rax)
+    646c947a:	add    %al,(%rax)
+    646c947c:	add    %al,(%rax)
+	...
+
+00000000646c9480 <.rdata>:
+    646c9480:	rex.B jb 646c94ea <.rdata+0x6a>
+    646c9483:	jne    646c94f2 <.rdata+0x72>
+    646c9485:	outsb  %gs:(%rsi),(%dx)
+    646c9487:	je     646c94a9 <.rdata+0x29>
+    646c9489:	outsl  %fs:(%rsi),(%dx)
+    646c948b:	insl   (%dx),%es:(%rdi)
+    646c948c:	(bad)
+    646c948d:	imul   $0x6f727265,0x20(%rsi),%ebp
+    646c9494:	jb     646c94b6 <.rdata+0x36>
+    646c9496:	sub    %al,0x4d(%rdi,%rcx,2)
+    646c949a:	rex.B
+    646c949b:	rex.WB
+    646c949c:	rex.WRX sub %r8,(%rax)
+    646c949f:	rex.B jb 646c9509 <.rdata+0x89>
+    646c94a2:	jne    646c9511 <.rdata+0x91>
+    646c94a4:	outsb  %gs:(%rsi),(%dx)
+    646c94a6:	je     646c94c8 <.rdata+0x48>
+    646c94a8:	jae    646c9513 <.rdata+0x93>
+    646c94aa:	outsb  %ds:(%rsi),(%dx)
+    646c94ab:	addr32 jne 646c951a <.rdata+0x9a>
+    646c94ae:	(bad)
+    646c94af:	jb     646c951a <.rdata+0x9a>
+    646c94b1:	je     646c952c <.rdata+0xac>
+    646c94b3:	and    %ch,(%rax)
+    646c94b5:	push   %rbx
+    646c94b6:	rex.WB
+    646c94b7:	rex.RXB
+    646c94b8:	rex.WRX sub %r8,(%rax)
+    646c94bb:	add    %al,(%rax)
+    646c94bd:	add    %al,(%rax)
+    646c94bf:	add    %cl,0x76(%rdi)
+    646c94c2:	gs jb  646c952b <.rdata+0xab>
+    646c94c5:	insb   (%dx),%es:(%rdi)
+    646c94c6:	outsl  %ds:(%rsi),(%dx)
+    646c94c7:	ja     646c94e9 <.rdata+0x69>
+    646c94c9:	jb     646c952c <.rdata+0xac>
+    646c94cb:	outsb  %ds:(%rsi),(%dx)
+    646c94cc:	and    %ah,%gs:0x72(%ebp)
+    646c94d1:	jb     646c9542 <.rdata+0xc2>
+    646c94d3:	jb     646c94f5 <.rdata+0x75>
+    646c94d5:	sub    %cl,0x56(%rdi)
+    646c94d8:	rex.RB push %r10
+    646c94da:	rex.RX
+    646c94db:	rex.WR
+    646c94dc:	rex.WRXB push %r15
+    646c94de:	sub    %eax,(%rax)
+    646c94e0:	push   %rax
+    646c94e1:	(bad)
+    646c94e2:	jb     646c9558 <.rdata+0xd8>
+    646c94e4:	imul   $0x736f6c20,0x6c(%rcx),%esp
+    646c94eb:	jae    646c950d <.rdata+0x8d>
+    646c94ed:	outsl  %ds:(%rsi),(%dx)
+    646c94ee:	data16 and %dh,0x69(%rbx)
+    646c94f2:	outsb  %ds:(%esi),(%dx)
+    646c94f4:	imul   $0x636e6163,0x69(%rsi),%esp
+    646c94fb:	and    %ch,%gs:(%rax)
+    646c94fe:	push   %rax
+    646c94ff:	rex.WR
+    646c9500:	rex.WRXB push %r11
+    646c9502:	push   %rbx
+    646c9503:	sub    %eax,(%rax)
+    646c9505:	add    %al,(%rax)
+    646c9507:	add    %dl,0x74(%rdi,%rbp,2)
+    646c950b:	(bad)
+    646c950c:	insb   (%dx),%es:(%rdi)
+    646c950d:	and    %ch,0x73(%rdi,%rbp,2)
+    646c9511:	jae    646c9533 <.rdata+0xb3>
+    646c9513:	outsl  %ds:(%rsi),(%dx)
+    646c9514:	data16 and %dh,0x69(%rbx)
+    646c9518:	outsb  %ds:(%esi),(%dx)
+    646c951a:	imul   $0x636e6163,0x69(%rsi),%esp
+    646c9521:	and    %ch,%gs:(%rax)
+    646c9524:	push   %rsp
+    646c9525:	rex.WR
+    646c9526:	rex.WRXB push %r11
+    646c9528:	push   %rbx
+    646c9529:	sub    %eax,(%rax)
+    646c952b:	add    %al,(%rax)
+    646c952d:	add    %al,(%rax)
+    646c952f:	add    %dl,0x65(%rax,%rbp,2)
+    646c9533:	and    %dh,0x65(%rdx)
+    646c9536:	jae    646c95ad <.rdata+0x12d>
+    646c9538:	insb   (%dx),%es:(%rdi)
+    646c9539:	je     646c955b <.rdata+0xdb>
+    646c953b:	imul   $0x206f6f74,0x20(%rbx),%esi
+    646c9542:	jae    646c95b1 <.rdata+0x131>
+    646c9544:	(bad)
+    646c9545:	insb   (%dx),%es:(%rdi)
+    646c9546:	insb   (%dx),%es:(%rdi)
+    646c9547:	and    %dh,0x20(%rdi,%rbp,2)
+    646c954b:	(bad)
+    646c954d:	and    %dh,0x65(%rdx)
+    646c9550:	jo     646c95c4 <.refptr._CRT_MT+0x4>
+    646c9552:	gs jae 646c95ba <.rdata+0x13a>
+    646c9555:	outsb  %ds:(%rsi),(%dx)
+    646c9556:	je     646c95bd <.rdata+0x13d>
+    646c9558:	and    %ch,%fs:(%rax)
+    646c955b:	push   %rbp
+    646c955c:	rex.WRX
+    646c955d:	rex.R
+    646c955e:	rex.RB push %r10
+    646c9560:	rex.RX
+    646c9561:	rex.WR
+    646c9562:	rex.WRXB push %r15
+    646c9564:	sub    %eax,(%rax)
+    646c9566:	push   %rbp
+    646c9567:	outsb  %ds:(%rsi),(%dx)
+    646c9568:	imul   $0x77,0x6f(%rsi),%ebp
+    646c956c:	outsb  %ds:(%rsi),(%dx)
+    646c956d:	and    %ah,0x72(%rbp)
+    646c9570:	jb     646c95e1 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__+0x1>
+    646c9572:	jb     646c9574 <.rdata+0xf4>
+    646c9574:	add    %al,(%rax)
+    646c9576:	add    %al,(%rax)
+    646c9578:	pop    %rdi
+    646c9579:	insl   (%dx),%es:(%rdi)
+    646c957a:	(bad)
+    646c957b:	je     646c95e5 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__+0x5>
+    646c957d:	gs jb  646c95f2 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__+0x2>
+    646c9580:	sub    %ch,(%rcx)
+    646c9582:	cmp    (%rax),%ah
+    646c9584:	and    $0x6e692073,%eax
+    646c9589:	and    %ah,0x67252873(%rip)        # cb91be02 <.debug_str+0x67243e02>
+    646c958f:	sub    $0x20,%al
+    646c9591:	and    $0x20202967,%eax
+    646c9596:	sub    %dh,0x65(%rdx)
+    646c9599:	je     646c9611 <.refptr.__image_base__+0x1>
+    646c959b:	(bad)
+    646c959c:	insb   (%dx),%es:(%rdi)
+    646c959d:	cmp    $0xa296725,%eax
+    646c95a2:	add    %al,(%rax)
+    646c95a4:	or     $0xe5,%al
+    646c95a6:	(bad)
+    646c95a7:	decl   -0x1c(%rbp)
+    646c95aa:	(bad)
+    646c95ab:	(bad)
+    646c95ac:	mov    $0xccffffe4,%esp
+    646c95b1:	in     $0xff,%al
+    646c95b3:	(bad)
+    646c95b4:	fsub   %st,%st(4)
+    646c95b6:	(bad)
+    646c95b7:	(bad)
+    646c95b8:	in     (%dx),%al
+    646c95b9:	in     $0xff,%al
     646c95bb:	(bad)
-    646c95bc:	insb   (%dx),%es:(%rdi)
-    646c95bd:	cmp    $0xa296725,%eax
-    646c95c2:	add    %al,(%rax)
-    646c95c4:	fsub   %st,%st(7)
-    646c95c6:	(bad)
-    646c95c7:	lcall  *-0x73000019(%rip)        # fffffffff16c95b4 <.debug_str+0xffffffff8cff15b4>
-    646c95cd:	out    %eax,$0xff
-    646c95cf:	lcall  *-0x18530001(%rdi,%riz,8)
-    646c95d6:	(bad)
-    646c95d7:	(bad)
-    646c95d8:	mov    $0xccffffe7,%esp
-    646c95dd:	out    %eax,$0xff
-    646c95df:	jmp    *(%rax)
+    646c95bc:	cld
+    646c95bd:	in     $0xff,%al
+    646c95bf:	jmp    *(%rax)
+
+00000000646c95c0 <.refptr._CRT_MT>:
+    646c95c0:	and    %al,0x646c(%rax)
+	...
+
+00000000646c95d0 <.refptr.__CTOR_LIST__>:
+    646c95d0:	push   %rax
+    646c95d1:	jnp    646c963f <.refptr.__native_startup_lock+0xf>
+    646c95d3:	add    %al,%fs:(%rax)
+	...
 
-00000000646c95e0 <.refptr._CRT_MT>:
-    646c95e0:	and    %al,0x646c(%rax)
+00000000646c95e0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>:
+    646c95e0:	loopne 646c957a <.rdata+0xfa>
+    646c95e2:	insb   (%dx),%es:(%rdi)
+    646c95e3:	add    %al,%fs:(%rax)
 	...
 
-00000000646c95f0 <.refptr.__CTOR_LIST__>:
-    646c95f0:	rex jle 646c965f <.refptr.__native_startup_lock+0xf>
+00000000646c95f0 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>:
+    646c95f0:	loopne 646c958a <.rdata+0x10a>
+    646c95f2:	insb   (%dx),%es:(%rdi)
     646c95f3:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9600 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST_END__>:
-    646c9600:	add    %bl,0x646c(%rcx)
+00000000646c9600 <.refptr.__dyn_tls_init_callback>:
+    646c9600:	adcb   $0x0,0x646c(%rcx)
 	...
 
-00000000646c9610 <.refptr.__RUNTIME_PSEUDO_RELOC_LIST__>:
-    646c9610:	add    %bl,0x646c(%rcx)
+00000000646c9610 <.refptr.__image_base__>:
+    646c9610:	add    %al,(%rax)
+    646c9612:	insb   (%dx),%es:(%rdi)
+    646c9613:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9620 <.refptr.__dyn_tls_init_callback>:
-    646c9620:	movabs 0x646c91,%al
-    646c9629:	add    %al,(%rax)
-    646c962b:	add    %al,(%rax)
-    646c962d:	add    %al,(%rax)
+00000000646c9620 <.refptr.__native_dllmain_reason>:
+    646c9620:	adc    $0x80,%al
+    646c9622:	insb   (%dx),%es:(%rdi)
+    646c9623:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9630 <.refptr.__image_base__>:
-    646c9630:	add    %al,(%rax)
+00000000646c9630 <.refptr.__native_startup_lock>:
+    646c9630:	mov    %cl,%bl
     646c9632:	insb   (%dx),%es:(%rdi)
     646c9633:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9640 <.refptr.__native_dllmain_reason>:
-    646c9640:	adc    $0x80,%al
-    646c9642:	insb   (%dx),%es:(%rdi)
+00000000646c9640 <.refptr.__native_startup_state>:
+    646c9640:	or     $0x6c,%bl
     646c9643:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9650 <.refptr.__native_startup_lock>:
-    646c9650:	mov    %cl,%bl
+00000000646c9650 <.refptr.__xc_a>:
+    646c9650:	add    %dh,%al
     646c9652:	insb   (%dx),%es:(%rdi)
     646c9653:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9660 <.refptr.__native_startup_state>:
-    646c9660:	or     $0x6c,%bl
+00000000646c9660 <.refptr.__xc_z>:
+    646c9660:	or     %dh,%al
+    646c9662:	insb   (%dx),%es:(%rdi)
     646c9663:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9670 <.refptr.__xc_a>:
-    646c9670:	add    %dh,%al
+00000000646c9670 <.refptr.__xi_a>:
+    646c9670:	adc    %dh,%al
     646c9672:	insb   (%dx),%es:(%rdi)
     646c9673:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9680 <.refptr.__xc_z>:
-    646c9680:	or     %dh,%al
+00000000646c9680 <.refptr.__xi_z>:
+    646c9680:	and    %dh,%al
     646c9682:	insb   (%dx),%es:(%rdi)
     646c9683:	add    %al,%fs:(%rax)
 	...
 
-00000000646c9690 <.refptr.__xi_a>:
-    646c9690:	adc    %dh,%al
+00000000646c9690 <.refptr.mingw_app_type>:
+    646c9690:	xor    %cl,%al
     646c9692:	insb   (%dx),%es:(%rdi)
     646c9693:	add    %al,%fs:(%rax)
 	...
 
-00000000646c96a0 <.refptr.__xi_z>:
-    646c96a0:	and    %dh,%al
-    646c96a2:	insb   (%dx),%es:(%rdi)
-    646c96a3:	add    %al,%fs:(%rax)
-	...
-
-00000000646c96b0 <.refptr.mingw_app_type>:
-    646c96b0:	xor    %cl,%al
-    646c96b2:	insb   (%dx),%es:(%rdi)
-    646c96b3:	add    %al,%fs:(%rax)
-	...
-
-00000000646c96c0 <.rdata$zzz>:
-    646c96c0:	rex.RXB
-    646c96c1:	rex.XB
-    646c96c2:	rex.XB cmp (%r8),%spl
-    646c96c5:	sub    %bh,0x38(%rax)
-    646c96c8:	ss pop %rdi
-    646c96ca:	ss xor $0x2d,%al
-    646c96cd:	ja     646c9738 <.rdata$zzz+0x38>
-    646c96cf:	outsb  %ds:(%rsi),(%dx)
-    646c96d0:	xor    (%rdx),%esi
-    646c96d2:	sub    $0x2d686573,%eax
-    646c96d7:	jb     646c973e <.rdata$zzz+0x3e>
-    646c96d9:	jbe    646c970b <.rdata$zzz+0xb>
-    646c96db:	sub    $0x20,%al
-    646c96dd:	rex.X jne 646c9749 <.rdata$zzz+0x9>
-    646c96e0:	insb   (%dx),%es:(%rdi)
-    646c96e1:	je     646c9703 <.rdata$zzz+0x3>
-    646c96e3:	(bad)
-    646c96e4:	jns    646c9706 <.rdata$zzz+0x6>
-    646c96e6:	imul   $0x36572d57,0x47(%r14),%r13
-    646c96ee:	xor    $0x20,%al
-    646c96f0:	jo     646c9764 <.rdata$zzz+0x24>
-    646c96f2:	outsl  %ds:(%rsi),(%dx)
-    646c96f3:	push   $0x65
-    646c96f5:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c96f9:	cmp    %ch,(%rsi)
-    646c96fb:	xor    %ebp,(%rsi)
-    646c96fd:	xor    %al,(%rax)
-	...
-
-00000000646c9700 <.rdata$zzz>:
-    646c9700:	rex.RXB
-    646c9701:	rex.XB
-    646c9702:	rex.XB cmp (%r8),%spl
-    646c9705:	sub    %bh,0x38(%rax)
-    646c9708:	ss pop %rdi
-    646c970a:	ss xor $0x2d,%al
-    646c970d:	ja     646c9778 <.rdata$zzz+0x38>
-    646c970f:	outsb  %ds:(%rsi),(%dx)
-    646c9710:	xor    (%rdx),%esi
-    646c9712:	sub    $0x2d686573,%eax
-    646c9717:	jb     646c977e <.rdata$zzz+0x3e>
-    646c9719:	jbe    646c974b <.rdata$zzz+0xb>
-    646c971b:	sub    $0x20,%al
-    646c971d:	rex.X jne 646c9789 <.rdata$zzz+0x9>
-    646c9720:	insb   (%dx),%es:(%rdi)
-    646c9721:	je     646c9743 <.rdata$zzz+0x3>
-    646c9723:	(bad)
-    646c9724:	jns    646c9746 <.rdata$zzz+0x6>
-    646c9726:	imul   $0x36572d57,0x47(%r14),%r13
-    646c972e:	xor    $0x20,%al
-    646c9730:	jo     646c97a4 <.rdata$zzz+0x24>
-    646c9732:	outsl  %ds:(%rsi),(%dx)
-    646c9733:	push   $0x65
-    646c9735:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c9739:	cmp    %ch,(%rsi)
-    646c973b:	xor    %ebp,(%rsi)
-    646c973d:	xor    %al,(%rax)
-	...
-
-00000000646c9740 <.rdata$zzz>:
-    646c9740:	rex.RXB
-    646c9741:	rex.XB
-    646c9742:	rex.XB cmp (%r8),%spl
-    646c9745:	sub    %bh,0x38(%rax)
-    646c9748:	ss pop %rdi
-    646c974a:	ss xor $0x2d,%al
-    646c974d:	ja     646c97b8 <.rdata$zzz+0x38>
-    646c974f:	outsb  %ds:(%rsi),(%dx)
-    646c9750:	xor    (%rdx),%esi
-    646c9752:	sub    $0x2d686573,%eax
-    646c9757:	jb     646c97be <.rdata$zzz+0x3e>
-    646c9759:	jbe    646c978b <.rdata$zzz+0xb>
-    646c975b:	sub    $0x20,%al
-    646c975d:	rex.X jne 646c97c9 <.rdata$zzz+0x9>
-    646c9760:	insb   (%dx),%es:(%rdi)
-    646c9761:	je     646c9783 <.rdata$zzz+0x3>
-    646c9763:	(bad)
-    646c9764:	jns    646c9786 <.rdata$zzz+0x6>
-    646c9766:	imul   $0x36572d57,0x47(%r14),%r13
-    646c976e:	xor    $0x20,%al
-    646c9770:	jo     646c97e4 <.rdata$zzz+0x24>
-    646c9772:	outsl  %ds:(%rsi),(%dx)
-    646c9773:	push   $0x65
-    646c9775:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c9779:	cmp    %ch,(%rsi)
-    646c977b:	xor    %ebp,(%rsi)
-    646c977d:	xor    %al,(%rax)
-	...
-
-00000000646c9780 <.rdata$zzz>:
-    646c9780:	rex.RXB
-    646c9781:	rex.XB
-    646c9782:	rex.XB cmp (%r8),%spl
-    646c9785:	sub    %bh,0x38(%rax)
-    646c9788:	ss pop %rdi
-    646c978a:	ss xor $0x2d,%al
-    646c978d:	ja     646c97f8 <.rdata$zzz+0x38>
-    646c978f:	outsb  %ds:(%rsi),(%dx)
-    646c9790:	xor    (%rdx),%esi
-    646c9792:	sub    $0x2d686573,%eax
-    646c9797:	jb     646c97fe <.rdata$zzz+0x3e>
-    646c9799:	jbe    646c97cb <.rdata$zzz+0xb>
-    646c979b:	sub    $0x20,%al
-    646c979d:	rex.X jne 646c9809 <.rdata$zzz+0x9>
-    646c97a0:	insb   (%dx),%es:(%rdi)
-    646c97a1:	je     646c97c3 <.rdata$zzz+0x3>
-    646c97a3:	(bad)
-    646c97a4:	jns    646c97c6 <.rdata$zzz+0x6>
-    646c97a6:	imul   $0x36572d57,0x47(%r14),%r13
-    646c97ae:	xor    $0x20,%al
-    646c97b0:	jo     646c9824 <.rdata$zzz+0x24>
-    646c97b2:	outsl  %ds:(%rsi),(%dx)
-    646c97b3:	push   $0x65
-    646c97b5:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c97b9:	cmp    %ch,(%rsi)
-    646c97bb:	xor    %ebp,(%rsi)
-    646c97bd:	xor    %al,(%rax)
-	...
-
-00000000646c97c0 <.rdata$zzz>:
-    646c97c0:	rex.RXB
-    646c97c1:	rex.XB
-    646c97c2:	rex.XB cmp (%r8),%spl
-    646c97c5:	sub    %bh,0x38(%rax)
-    646c97c8:	ss pop %rdi
-    646c97ca:	ss xor $0x2d,%al
-    646c97cd:	ja     646c9838 <.rdata$zzz+0x38>
-    646c97cf:	outsb  %ds:(%rsi),(%dx)
-    646c97d0:	xor    (%rdx),%esi
-    646c97d2:	sub    $0x2d686573,%eax
-    646c97d7:	jb     646c983e <.rdata$zzz+0x3e>
-    646c97d9:	jbe    646c980b <.rdata$zzz+0xb>
-    646c97db:	sub    $0x20,%al
-    646c97dd:	rex.X jne 646c9849 <.rdata$zzz+0x9>
-    646c97e0:	insb   (%dx),%es:(%rdi)
-    646c97e1:	je     646c9803 <.rdata$zzz+0x3>
-    646c97e3:	(bad)
-    646c97e4:	jns    646c9806 <.rdata$zzz+0x6>
-    646c97e6:	imul   $0x36572d57,0x47(%r14),%r13
-    646c97ee:	xor    $0x20,%al
-    646c97f0:	jo     646c9864 <.rdata$zzz+0x24>
-    646c97f2:	outsl  %ds:(%rsi),(%dx)
-    646c97f3:	push   $0x65
-    646c97f5:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c97f9:	cmp    %ch,(%rsi)
-    646c97fb:	xor    %ebp,(%rsi)
-    646c97fd:	xor    %al,(%rax)
-	...
-
-00000000646c9800 <.rdata$zzz>:
-    646c9800:	rex.RXB
-    646c9801:	rex.XB
-    646c9802:	rex.XB cmp (%r8),%spl
-    646c9805:	sub    %bh,0x38(%rax)
-    646c9808:	ss pop %rdi
-    646c980a:	ss xor $0x2d,%al
-    646c980d:	ja     646c9878 <.rdata$zzz+0x38>
-    646c980f:	outsb  %ds:(%rsi),(%dx)
-    646c9810:	xor    (%rdx),%esi
-    646c9812:	sub    $0x2d686573,%eax
-    646c9817:	jb     646c987e <.rdata$zzz+0x3e>
-    646c9819:	jbe    646c984b <.rdata$zzz+0xb>
-    646c981b:	sub    $0x20,%al
-    646c981d:	rex.X jne 646c9889 <.rdata$zzz+0x9>
-    646c9820:	insb   (%dx),%es:(%rdi)
-    646c9821:	je     646c9843 <.rdata$zzz+0x3>
-    646c9823:	(bad)
-    646c9824:	jns    646c9846 <.rdata$zzz+0x6>
-    646c9826:	imul   $0x36572d57,0x47(%r14),%r13
-    646c982e:	xor    $0x20,%al
-    646c9830:	jo     646c98a4 <.rdata$zzz+0x24>
-    646c9832:	outsl  %ds:(%rsi),(%dx)
-    646c9833:	push   $0x65
-    646c9835:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c9839:	cmp    %ch,(%rsi)
-    646c983b:	xor    %ebp,(%rsi)
-    646c983d:	xor    %al,(%rax)
-	...
-
-00000000646c9840 <.rdata$zzz>:
-    646c9840:	rex.RXB
-    646c9841:	rex.XB
-    646c9842:	rex.XB cmp (%r8),%spl
-    646c9845:	sub    %bh,0x38(%rax)
-    646c9848:	ss pop %rdi
-    646c984a:	ss xor $0x2d,%al
-    646c984d:	ja     646c98b8 <.rdata$zzz+0x38>
-    646c984f:	outsb  %ds:(%rsi),(%dx)
-    646c9850:	xor    (%rdx),%esi
-    646c9852:	sub    $0x2d686573,%eax
-    646c9857:	jb     646c98be <.rdata$zzz+0x3e>
-    646c9859:	jbe    646c988b <.rdata$zzz+0xb>
-    646c985b:	sub    $0x20,%al
-    646c985d:	rex.X jne 646c98c9 <.rdata$zzz+0x9>
-    646c9860:	insb   (%dx),%es:(%rdi)
-    646c9861:	je     646c9883 <.rdata$zzz+0x3>
-    646c9863:	(bad)
-    646c9864:	jns    646c9886 <.rdata$zzz+0x6>
-    646c9866:	imul   $0x36572d57,0x47(%r14),%r13
-    646c986e:	xor    $0x20,%al
-    646c9870:	jo     646c98e4 <.rdata$zzz+0x24>
-    646c9872:	outsl  %ds:(%rsi),(%dx)
-    646c9873:	push   $0x65
-    646c9875:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c9879:	cmp    %ch,(%rsi)
-    646c987b:	xor    %ebp,(%rsi)
-    646c987d:	xor    %al,(%rax)
-	...
-
-00000000646c9880 <.rdata$zzz>:
-    646c9880:	rex.RXB
-    646c9881:	rex.XB
-    646c9882:	rex.XB cmp (%r8),%spl
-    646c9885:	sub    %bh,0x38(%rax)
-    646c9888:	ss pop %rdi
-    646c988a:	ss xor $0x2d,%al
-    646c988d:	ja     646c98f8 <.rdata$zzz+0x38>
-    646c988f:	outsb  %ds:(%rsi),(%dx)
-    646c9890:	xor    (%rdx),%esi
-    646c9892:	sub    $0x2d686573,%eax
-    646c9897:	jb     646c98fe <.rdata$zzz+0x3e>
-    646c9899:	jbe    646c98cb <.rdata$zzz+0xb>
-    646c989b:	sub    $0x20,%al
-    646c989d:	rex.X jne 646c9909 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x9>
-    646c98a0:	insb   (%dx),%es:(%rdi)
-    646c98a1:	je     646c98c3 <.rdata$zzz+0x3>
-    646c98a3:	(bad)
-    646c98a4:	jns    646c98c6 <.rdata$zzz+0x6>
-    646c98a6:	imul   $0x36572d57,0x47(%r14),%r13
-    646c98ae:	xor    $0x20,%al
-    646c98b0:	jo     646c9924 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x24>
-    646c98b2:	outsl  %ds:(%rsi),(%dx)
-    646c98b3:	push   $0x65
-    646c98b5:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c98b9:	cmp    %ch,(%rsi)
-    646c98bb:	xor    %ebp,(%rsi)
-    646c98bd:	xor    %al,(%rax)
-	...
-
-00000000646c98c0 <.rdata$zzz>:
-    646c98c0:	rex.RXB
-    646c98c1:	rex.XB
-    646c98c2:	rex.XB cmp (%r8),%spl
-    646c98c5:	sub    %bh,0x38(%rax)
-    646c98c8:	ss pop %rdi
-    646c98ca:	ss xor $0x2d,%al
-    646c98cd:	ja     646c9938 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x38>
-    646c98cf:	outsb  %ds:(%rsi),(%dx)
-    646c98d0:	xor    (%rdx),%esi
-    646c98d2:	sub    $0x2d686573,%eax
-    646c98d7:	jb     646c993e <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x3e>
-    646c98d9:	jbe    646c990b <__RUNTIME_PSEUDO_RELOC_LIST_END__+0xb>
-    646c98db:	sub    $0x20,%al
-    646c98dd:	rex.X jne 646c9949 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x49>
-    646c98e0:	insb   (%dx),%es:(%rdi)
-    646c98e1:	je     646c9903 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x3>
-    646c98e3:	(bad)
-    646c98e4:	jns    646c9906 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x6>
-    646c98e6:	imul   $0x36572d57,0x47(%r14),%r13
-    646c98ee:	xor    $0x20,%al
-    646c98f0:	jo     646c9964 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x64>
-    646c98f2:	outsl  %ds:(%rsi),(%dx)
-    646c98f3:	push   $0x65
-    646c98f5:	movsxd 0x20(%rcx,%rbp,1),%esi
-    646c98f9:	cmp    %ch,(%rsi)
-    646c98fb:	xor    %ebp,(%rsi)
-    646c98fd:	xor    %al,(%rax)
+00000000646c96a0 <.rdata$zzz>:
+    646c96a0:	rex.RXB
+    646c96a1:	rex.XB
+    646c96a2:	rex.XB cmp (%r8),%spl
+    646c96a5:	sub    %bh,0x38(%rax)
+    646c96a8:	ss pop %rdi
+    646c96aa:	ss xor $0x2d,%al
+    646c96ad:	ja     646c9718 <.rdata$zzz+0x38>
+    646c96af:	outsb  %ds:(%rsi),(%dx)
+    646c96b0:	xor    (%rdx),%esi
+    646c96b2:	sub    $0x2d686573,%eax
+    646c96b7:	jb     646c971e <.rdata$zzz+0x3e>
+    646c96b9:	jbe    646c96eb <.rdata$zzz+0xb>
+    646c96bb:	sub    $0x20,%al
+    646c96bd:	rex.X jne 646c9729 <.rdata$zzz+0x9>
+    646c96c0:	insb   (%dx),%es:(%rdi)
+    646c96c1:	je     646c96e3 <.rdata$zzz+0x3>
+    646c96c3:	(bad)
+    646c96c4:	jns    646c96e6 <.rdata$zzz+0x6>
+    646c96c6:	imul   $0x36572d57,0x47(%r14),%r13
+    646c96ce:	xor    $0x20,%al
+    646c96d0:	jo     646c9744 <.rdata$zzz+0x24>
+    646c96d2:	outsl  %ds:(%rsi),(%dx)
+    646c96d3:	push   $0x65
+    646c96d5:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c96d9:	cmp    %ch,(%rsi)
+    646c96db:	xor    %ebp,(%rsi)
+    646c96dd:	xor    %al,(%rax)
+	...
+
+00000000646c96e0 <.rdata$zzz>:
+    646c96e0:	rex.RXB
+    646c96e1:	rex.XB
+    646c96e2:	rex.XB cmp (%r8),%spl
+    646c96e5:	sub    %bh,0x38(%rax)
+    646c96e8:	ss pop %rdi
+    646c96ea:	ss xor $0x2d,%al
+    646c96ed:	ja     646c9758 <.rdata$zzz+0x38>
+    646c96ef:	outsb  %ds:(%rsi),(%dx)
+    646c96f0:	xor    (%rdx),%esi
+    646c96f2:	sub    $0x2d686573,%eax
+    646c96f7:	jb     646c975e <.rdata$zzz+0x3e>
+    646c96f9:	jbe    646c972b <.rdata$zzz+0xb>
+    646c96fb:	sub    $0x20,%al
+    646c96fd:	rex.X jne 646c9769 <.rdata$zzz+0x9>
+    646c9700:	insb   (%dx),%es:(%rdi)
+    646c9701:	je     646c9723 <.rdata$zzz+0x3>
+    646c9703:	(bad)
+    646c9704:	jns    646c9726 <.rdata$zzz+0x6>
+    646c9706:	imul   $0x36572d57,0x47(%r14),%r13
+    646c970e:	xor    $0x20,%al
+    646c9710:	jo     646c9784 <.rdata$zzz+0x24>
+    646c9712:	outsl  %ds:(%rsi),(%dx)
+    646c9713:	push   $0x65
+    646c9715:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c9719:	cmp    %ch,(%rsi)
+    646c971b:	xor    %ebp,(%rsi)
+    646c971d:	xor    %al,(%rax)
+	...
+
+00000000646c9720 <.rdata$zzz>:
+    646c9720:	rex.RXB
+    646c9721:	rex.XB
+    646c9722:	rex.XB cmp (%r8),%spl
+    646c9725:	sub    %bh,0x38(%rax)
+    646c9728:	ss pop %rdi
+    646c972a:	ss xor $0x2d,%al
+    646c972d:	ja     646c9798 <.rdata$zzz+0x38>
+    646c972f:	outsb  %ds:(%rsi),(%dx)
+    646c9730:	xor    (%rdx),%esi
+    646c9732:	sub    $0x2d686573,%eax
+    646c9737:	jb     646c979e <.rdata$zzz+0x3e>
+    646c9739:	jbe    646c976b <.rdata$zzz+0xb>
+    646c973b:	sub    $0x20,%al
+    646c973d:	rex.X jne 646c97a9 <.rdata$zzz+0x9>
+    646c9740:	insb   (%dx),%es:(%rdi)
+    646c9741:	je     646c9763 <.rdata$zzz+0x3>
+    646c9743:	(bad)
+    646c9744:	jns    646c9766 <.rdata$zzz+0x6>
+    646c9746:	imul   $0x36572d57,0x47(%r14),%r13
+    646c974e:	xor    $0x20,%al
+    646c9750:	jo     646c97c4 <.rdata$zzz+0x24>
+    646c9752:	outsl  %ds:(%rsi),(%dx)
+    646c9753:	push   $0x65
+    646c9755:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c9759:	cmp    %ch,(%rsi)
+    646c975b:	xor    %ebp,(%rsi)
+    646c975d:	xor    %al,(%rax)
+	...
+
+00000000646c9760 <.rdata$zzz>:
+    646c9760:	rex.RXB
+    646c9761:	rex.XB
+    646c9762:	rex.XB cmp (%r8),%spl
+    646c9765:	sub    %bh,0x38(%rax)
+    646c9768:	ss pop %rdi
+    646c976a:	ss xor $0x2d,%al
+    646c976d:	ja     646c97d8 <.rdata$zzz+0x38>
+    646c976f:	outsb  %ds:(%rsi),(%dx)
+    646c9770:	xor    (%rdx),%esi
+    646c9772:	sub    $0x2d686573,%eax
+    646c9777:	jb     646c97de <.rdata$zzz+0x3e>
+    646c9779:	jbe    646c97ab <.rdata$zzz+0xb>
+    646c977b:	sub    $0x20,%al
+    646c977d:	rex.X jne 646c97e9 <.rdata$zzz+0x9>
+    646c9780:	insb   (%dx),%es:(%rdi)
+    646c9781:	je     646c97a3 <.rdata$zzz+0x3>
+    646c9783:	(bad)
+    646c9784:	jns    646c97a6 <.rdata$zzz+0x6>
+    646c9786:	imul   $0x36572d57,0x47(%r14),%r13
+    646c978e:	xor    $0x20,%al
+    646c9790:	jo     646c9804 <.rdata$zzz+0x24>
+    646c9792:	outsl  %ds:(%rsi),(%dx)
+    646c9793:	push   $0x65
+    646c9795:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c9799:	cmp    %ch,(%rsi)
+    646c979b:	xor    %ebp,(%rsi)
+    646c979d:	xor    %al,(%rax)
+	...
+
+00000000646c97a0 <.rdata$zzz>:
+    646c97a0:	rex.RXB
+    646c97a1:	rex.XB
+    646c97a2:	rex.XB cmp (%r8),%spl
+    646c97a5:	sub    %bh,0x38(%rax)
+    646c97a8:	ss pop %rdi
+    646c97aa:	ss xor $0x2d,%al
+    646c97ad:	ja     646c9818 <.rdata$zzz+0x38>
+    646c97af:	outsb  %ds:(%rsi),(%dx)
+    646c97b0:	xor    (%rdx),%esi
+    646c97b2:	sub    $0x2d686573,%eax
+    646c97b7:	jb     646c981e <.rdata$zzz+0x3e>
+    646c97b9:	jbe    646c97eb <.rdata$zzz+0xb>
+    646c97bb:	sub    $0x20,%al
+    646c97bd:	rex.X jne 646c9829 <.rdata$zzz+0x9>
+    646c97c0:	insb   (%dx),%es:(%rdi)
+    646c97c1:	je     646c97e3 <.rdata$zzz+0x3>
+    646c97c3:	(bad)
+    646c97c4:	jns    646c97e6 <.rdata$zzz+0x6>
+    646c97c6:	imul   $0x36572d57,0x47(%r14),%r13
+    646c97ce:	xor    $0x20,%al
+    646c97d0:	jo     646c9844 <.rdata$zzz+0x24>
+    646c97d2:	outsl  %ds:(%rsi),(%dx)
+    646c97d3:	push   $0x65
+    646c97d5:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c97d9:	cmp    %ch,(%rsi)
+    646c97db:	xor    %ebp,(%rsi)
+    646c97dd:	xor    %al,(%rax)
+	...
+
+00000000646c97e0 <.rdata$zzz>:
+    646c97e0:	rex.RXB
+    646c97e1:	rex.XB
+    646c97e2:	rex.XB cmp (%r8),%spl
+    646c97e5:	sub    %bh,0x38(%rax)
+    646c97e8:	ss pop %rdi
+    646c97ea:	ss xor $0x2d,%al
+    646c97ed:	ja     646c9858 <.rdata$zzz+0x38>
+    646c97ef:	outsb  %ds:(%rsi),(%dx)
+    646c97f0:	xor    (%rdx),%esi
+    646c97f2:	sub    $0x2d686573,%eax
+    646c97f7:	jb     646c985e <.rdata$zzz+0x3e>
+    646c97f9:	jbe    646c982b <.rdata$zzz+0xb>
+    646c97fb:	sub    $0x20,%al
+    646c97fd:	rex.X jne 646c9869 <.rdata$zzz+0x9>
+    646c9800:	insb   (%dx),%es:(%rdi)
+    646c9801:	je     646c9823 <.rdata$zzz+0x3>
+    646c9803:	(bad)
+    646c9804:	jns    646c9826 <.rdata$zzz+0x6>
+    646c9806:	imul   $0x36572d57,0x47(%r14),%r13
+    646c980e:	xor    $0x20,%al
+    646c9810:	jo     646c9884 <.rdata$zzz+0x24>
+    646c9812:	outsl  %ds:(%rsi),(%dx)
+    646c9813:	push   $0x65
+    646c9815:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c9819:	cmp    %ch,(%rsi)
+    646c981b:	xor    %ebp,(%rsi)
+    646c981d:	xor    %al,(%rax)
+	...
+
+00000000646c9820 <.rdata$zzz>:
+    646c9820:	rex.RXB
+    646c9821:	rex.XB
+    646c9822:	rex.XB cmp (%r8),%spl
+    646c9825:	sub    %bh,0x38(%rax)
+    646c9828:	ss pop %rdi
+    646c982a:	ss xor $0x2d,%al
+    646c982d:	ja     646c9898 <.rdata$zzz+0x38>
+    646c982f:	outsb  %ds:(%rsi),(%dx)
+    646c9830:	xor    (%rdx),%esi
+    646c9832:	sub    $0x2d686573,%eax
+    646c9837:	jb     646c989e <.rdata$zzz+0x3e>
+    646c9839:	jbe    646c986b <.rdata$zzz+0xb>
+    646c983b:	sub    $0x20,%al
+    646c983d:	rex.X jne 646c98a9 <.rdata$zzz+0x9>
+    646c9840:	insb   (%dx),%es:(%rdi)
+    646c9841:	je     646c9863 <.rdata$zzz+0x3>
+    646c9843:	(bad)
+    646c9844:	jns    646c9866 <.rdata$zzz+0x6>
+    646c9846:	imul   $0x36572d57,0x47(%r14),%r13
+    646c984e:	xor    $0x20,%al
+    646c9850:	jo     646c98c4 <.rdata$zzz+0x24>
+    646c9852:	outsl  %ds:(%rsi),(%dx)
+    646c9853:	push   $0x65
+    646c9855:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c9859:	cmp    %ch,(%rsi)
+    646c985b:	xor    %ebp,(%rsi)
+    646c985d:	xor    %al,(%rax)
+	...
+
+00000000646c9860 <.rdata$zzz>:
+    646c9860:	rex.RXB
+    646c9861:	rex.XB
+    646c9862:	rex.XB cmp (%r8),%spl
+    646c9865:	sub    %bh,0x38(%rax)
+    646c9868:	ss pop %rdi
+    646c986a:	ss xor $0x2d,%al
+    646c986d:	ja     646c98d8 <.rdata$zzz+0x38>
+    646c986f:	outsb  %ds:(%rsi),(%dx)
+    646c9870:	xor    (%rdx),%esi
+    646c9872:	sub    $0x2d686573,%eax
+    646c9877:	jb     646c98de <.rdata$zzz+0x3e>
+    646c9879:	jbe    646c98ab <.rdata$zzz+0xb>
+    646c987b:	sub    $0x20,%al
+    646c987d:	rex.X jne 646c98e9 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x9>
+    646c9880:	insb   (%dx),%es:(%rdi)
+    646c9881:	je     646c98a3 <.rdata$zzz+0x3>
+    646c9883:	(bad)
+    646c9884:	jns    646c98a6 <.rdata$zzz+0x6>
+    646c9886:	imul   $0x36572d57,0x47(%r14),%r13
+    646c988e:	xor    $0x20,%al
+    646c9890:	jo     646c9904 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x24>
+    646c9892:	outsl  %ds:(%rsi),(%dx)
+    646c9893:	push   $0x65
+    646c9895:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c9899:	cmp    %ch,(%rsi)
+    646c989b:	xor    %ebp,(%rsi)
+    646c989d:	xor    %al,(%rax)
+	...
+
+00000000646c98a0 <.rdata$zzz>:
+    646c98a0:	rex.RXB
+    646c98a1:	rex.XB
+    646c98a2:	rex.XB cmp (%r8),%spl
+    646c98a5:	sub    %bh,0x38(%rax)
+    646c98a8:	ss pop %rdi
+    646c98aa:	ss xor $0x2d,%al
+    646c98ad:	ja     646c9918 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x38>
+    646c98af:	outsb  %ds:(%rsi),(%dx)
+    646c98b0:	xor    (%rdx),%esi
+    646c98b2:	sub    $0x2d686573,%eax
+    646c98b7:	jb     646c991e <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x3e>
+    646c98b9:	jbe    646c98eb <__RUNTIME_PSEUDO_RELOC_LIST_END__+0xb>
+    646c98bb:	sub    $0x20,%al
+    646c98bd:	rex.X jne 646c9929 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x49>
+    646c98c0:	insb   (%dx),%es:(%rdi)
+    646c98c1:	je     646c98e3 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x3>
+    646c98c3:	(bad)
+    646c98c4:	jns    646c98e6 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x6>
+    646c98c6:	imul   $0x36572d57,0x47(%r14),%r13
+    646c98ce:	xor    $0x20,%al
+    646c98d0:	jo     646c9944 <__RUNTIME_PSEUDO_RELOC_LIST_END__+0x64>
+    646c98d2:	outsl  %ds:(%rsi),(%dx)
+    646c98d3:	push   $0x65
+    646c98d5:	movsxd 0x20(%rcx,%rbp,1),%esi
+    646c98d9:	cmp    %ch,(%rsi)
+    646c98db:	xor    %ebp,(%rsi)
+    646c98dd:	xor    %al,(%rax)
 	...
 
 Disassembly of section .pdata:
 
 00000000646ca000 <.pdata>:
     646ca000:	add    %dl,(%rax)
     646ca002:	add    %al,(%rax)
@@ -11921,15 +11718,15 @@
     646ca211:	(bad)
     646ca212:	add    %al,(%rax)
     646ca214:	cs xor %al,(%rax)
     646ca217:	add    %dh,%al
     646ca219:	mov    $0x0,%cl
     646ca21b:	add    %ch,(%rsi)
     646ca21d:	xor    %al,(%rax)
-    646ca21f:	add    %bh,0x31(%rbx)
+    646ca21f:	add    %bh,0x31(%rbp)
     646ca222:	add    %al,(%rax)
     646ca224:	cld
     646ca225:	mov    $0x0,%cl
 	...
 
 00000000646ca228 <.pdata>:
     646ca228:	xorb   $0x0,(%rcx)
@@ -11981,389 +11778,400 @@
     646ca2a5:	rex.XB add %al,(%r8)
     646ca2a8:	test   %dh,0x43dd0000(%rdx)
     646ca2ae:	add    %al,(%rax)
     646ca2b0:	nop
     646ca2b1:	add    %r8b,(%rax)
     646ca2b4:	nop
     646ca2b5:	mov    $0x0,%dl
-    646ca2b7:	add    %dl,0x1d000044(%rax)
+    646ca2b7:	add    %dl,0x1f000044(%rax)
     646ca2bd:	add    %r8b,(%r8)
     646ca2c0:	pushf
     646ca2c1:	mov    $0x0,%dl
-    646ca2c3:	add    %bl,-0x34ffffbb(%rip)        # 2f6ca30e <__size_of_stack_reserve__+0x2f4ca30e>
-    646ca2c9:	rex.RX add %r8b,(%rax)
+    646ca2c3:	add    %bl,(%rdi)
+    646ca2c5:	add    %r8b,(%r8)
+    646ca2c8:	int    $0x46
+    646ca2ca:	add    %al,(%rax)
     646ca2cc:	test   $0xb2,%al
 	...
 
 00000000646ca2d0 <.pdata>:
     646ca2d0:	rolb   0x0(%rsi)
     646ca2d3:	add    %bh,0x47(%rdi)
     646ca2d6:	add    %al,(%rax)
     646ca2d8:	mov    $0xb2,%ah
 	...
 
 00000000646ca2dc <.pdata>:
     646ca2dc:	addb   $0x0,0x0(%rdi)
-    646ca2e0:	in     $0x47,%eax
+    646ca2e0:	out    %al,$0x47
     646ca2e2:	add    %al,(%rax)
-    646ca2e4:	shlb   $0x0,0x47e50000(%rdx)
-    646ca2eb:	add    %bl,-0x33ffffb4(%rbx)
+    646ca2e4:	shlb   $0x0,0x47e60000(%rdx)
+    646ca2eb:	add    %cl,(%rdx)
+    646ca2ed:	rex.WR add %r8b,(%rax)
+    646ca2f0:	int3
     646ca2f1:	mov    $0x0,%dl
-    646ca2f3:	add    %bl,-0x41ffffb4(%rbx)
-    646ca2f9:	rex.WR add %r8b,(%rax)
-    646ca2fc:	fdivs  0x4cbe0000(%rdx)
-    646ca302:	add    %al,(%rax)
-    646ca304:	sbb    %cl,0x0(%rbp)
-    646ca307:	add    %ah,%ah
-    646ca309:	mov    $0x0,%dl
+    646ca2f3:	add    %cl,(%rdx)
+    646ca2f5:	rex.WR add %r8b,(%rax)
+    646ca2f8:	sub    $0xd800004c,%eax
+    646ca2fd:	mov    $0x0,%dl
+    646ca2ff:	add    %ch,-0x78ffffb4(%rip)        # ffffffffeb6ca351 <.debug_str+0xffffffff86ff2351>
+    646ca305:	rex.WR add %r8b,(%rax)
+    646ca308:	in     $0xb2,%al
 	...
 
 00000000646ca30c <.pdata>:
-    646ca30c:	and    %cl,0x0(%rbp)
-    646ca30f:	add    %dh,-0xfffffb2(%rax)
-    646ca315:	mov    $0x0,%dl
-    646ca317:	add    %dh,-0x4effffb2(%rax)
-    646ca31d:	push   %rax
-    646ca31e:	add    %al,(%rax)
+    646ca30c:	nop
+    646ca30d:	rex.WR add %r8b,(%rax)
+    646ca310:	(bad)
+    646ca311:	rex.WRB add %r8b,(%r8)
+    646ca314:	lock mov $0x0,%dl
+    646ca317:	add    %cl,(%rsi)
+    646ca319:	rex.WRB add %r8b,(%r8)
+    646ca31c:	(bad)
+    646ca31d:	rex.WRB add %r8b,(%r8)
     646ca320:	cld
     646ca321:	mov    $0x0,%dl
-    646ca323:	add    %dh,0x18000050(%rcx)
-    646ca329:	push   %rcx
-    646ca32a:	add    %al,(%rax)
-    646ca32c:	or     %dh,0x51200000(%rbx)
+    646ca323:	add    %dl,%ch
+    646ca325:	rex.WRB add %r8b,(%r8)
+    646ca328:	cmp    %ecx,0x0(%rsi)
+    646ca32b:	add    %cl,(%rax)
+    646ca32d:	mov    $0x0,%bl
+	...
 
 00000000646ca330 <.pdata>:
-    646ca330:	and    %dl,0x0(%rcx)
-    646ca333:	add    %bl,-0x4cec0000(%rbx,%rdx,2)
+    646ca330:	rex
+    646ca331:	rex.WRX add %r8b,(%rax)
+    646ca334:	mov    $0x50,%dh
+    646ca336:	add    %al,(%rax)
+    646ca338:	adc    $0xb3,%al
     646ca33a:	add    %al,(%rax)
-    646ca33c:	pushf
-    646ca33d:	push   %rbx
+    646ca33c:	mov    $0x50,%dh
     646ca33e:	add    %al,(%rax)
-    646ca340:	test   %dl,0x0(%rax,%rax,1)
+    646ca340:	sahf
+    646ca341:	push   %rcx
+    646ca342:	add    %al,(%rax)
     646ca344:	and    $0xb3,%al
 	...
 
 00000000646ca348 <.pdata>:
-    646ca348:	movabs 0x30000054d5000054,%al
-    646ca351:	mov    $0x0,%bl
-    646ca353:	add    %ah,%al
-    646ca355:	push   %rsp
+    646ca348:	mov    $0x51,%al
+    646ca34a:	add    %al,(%rax)
+    646ca34c:	in     $0x51,%eax
+    646ca34e:	add    %al,(%rax)
+    646ca350:	xor    %dh,0x51f00000(%rbx)
     646ca356:	add    %al,(%rax)
-    646ca358:	rex.RX push %rbp
+    646ca358:	push   %rsi
+    646ca359:	push   %rdx
     646ca35a:	add    %al,(%rax)
-    646ca35c:	cmp    %dh,0x55500000(%rbx)
+    646ca35c:	cmp    %dh,0x52600000(%rbx)
     646ca362:	add    %al,(%rax)
-    646ca364:	outsl  %ds:(%rsi),(%dx)
-    646ca365:	push   %rbp
+    646ca364:	jg     646ca3b8 <.pdata+0x10>
     646ca366:	add    %al,(%rax)
     646ca368:	rex.R mov $0x0,%bl
 	...
 
 00000000646ca36c <.pdata>:
-    646ca36c:	jo     646ca3c3 <.pdata.unlikely+0x3>
-    646ca36e:	add    %al,(%rax)
-    646ca370:	rex.RX push %rsi
+    646ca36c:	adcb   $0x0,0x0(%rdx)
+    646ca370:	push   %rsi
+    646ca371:	push   %rbx
     646ca372:	add    %al,(%rax)
     646ca374:	rex.W mov $0x0,%bl
-    646ca377:	add    %dl,0x56(%rax)
+    646ca377:	add    %ah,0x53(%rax)
     646ca37a:	add    %al,(%rax)
-    646ca37c:	rex.W push %rdi
+    646ca37c:	pop    %rax
+    646ca37d:	push   %rsp
     646ca37e:	add    %al,(%rax)
     646ca380:	pop    %rax
     646ca381:	mov    $0x0,%bl
 	...
 
 00000000646ca384 <.pdata>:
-    646ca384:	push   %rax
-    646ca385:	push   %rdi
+    646ca384:	(bad)
+    646ca385:	push   %rsp
     646ca386:	add    %al,(%rax)
-    646ca388:	jg     646ca3e1 <.pdata+0x15>
+    646ca388:	(bad)
+    646ca389:	push   %rsp
     646ca38a:	add    %al,(%rax)
-    646ca38c:	push   $0xffffffff800000b3
-    646ca391:	push   %rdi
+    646ca38c:	push   $0xffffffff900000b3
+    646ca391:	push   %rsp
     646ca392:	add    %al,(%rax)
-    646ca394:	repz push %rdi
-    646ca396:	add    %al,(%rax)
-    646ca398:	jo     646ca34d <.pdata+0x5>
+    646ca394:	add    0x0(%rbp),%edx
+    646ca397:	add    %dh,-0x4d(%rax)
     646ca39a:	add    %al,(%rax)
-    646ca39c:	add    %bl,0x0(%rax)
-    646ca39f:	add    %al,(%rbx)
-    646ca3a1:	pop    %rax
+    646ca39c:	adc    %dl,0x0(%rbp)
+    646ca39f:	add    %dl,(%rbx)
+    646ca3a1:	push   %rbp
     646ca3a2:	add    %al,(%rax)
     646ca3a4:	jl     646ca359 <.pdata+0x11>
 	...
 
 00000000646ca3a8 <.pdata>:
-    646ca3a8:	adc    %bl,0x0(%rax)
-    646ca3ab:	add    %dl,(%rax,%rbx,2)
-    646ca3ae:	add    %al,(%rax)
-    646ca3b0:	xorb   $0x0,0x58200000(%rbx)
-    646ca3b7:	add    %ah,(%rax,%rbx,2)
-    646ca3ba:	add    %al,(%rax)
-    646ca3bc:	test   %dh,0x58300000(%rbx)
+    646ca3a8:	and    %dl,0x0(%rbp)
+    646ca3ab:	add    %ah,-0x4c800000(,%rdx,2)
+    646ca3b2:	add    %al,(%rax)
+    646ca3b4:	xor    %dl,0x0(%rbp)
+    646ca3b7:	add    %dh,-0x4c7c0000(,%rdx,2)
+	...
 
 00000000646ca3c0 <.pdata.unlikely>:
-    646ca3c0:	xor    %bl,0x0(%rax)
-    646ca3c3:	add    %bh,%ch
-    646ca3c5:	pop    %rcx
-    646ca3c6:	add    %al,(%rax)
-    646ca3c8:	xchg   %eax,%esp
+    646ca3c0:	rex push %rbp
+    646ca3c2:	add    %al,(%rax)
+    646ca3c4:	or     $0x94000057,%eax
     646ca3c9:	mov    $0x0,%bl
 	...
 
 00000000646ca3cc <.pdata>:
-    646ca3cc:	add    %bl,0x0(%rdx)
-    646ca3cf:	add    %bh,-0x5bffffa4(%rbx)
+    646ca3cc:	adc    %dl,0x0(%rdi)
+    646ca3cf:	add    %cl,%bl
+    646ca3d1:	pop    %rcx
+    646ca3d2:	add    %al,(%rax)
+    646ca3d4:	movsb  %ds:(%rsi),%es:(%rdi)
     646ca3d5:	mov    $0x0,%bl
-    646ca3d7:	add    %al,%al
-    646ca3d9:	pop    %rsp
+    646ca3d7:	add    %dl,%al
+    646ca3d9:	pop    %rcx
     646ca3da:	add    %al,(%rax)
-    646ca3dc:	(bad)
-    646ca3dd:	pop    %rsi
+    646ca3dc:	jo     646ca439 <.pdata+0x1>
     646ca3de:	add    %al,(%rax)
-    646ca3e0:	mov    $0x600000b3,%esp
+    646ca3e0:	mov    $0x700000b3,%esp
 
 00000000646ca3e4 <.pdata>:
-    646ca3e4:	(bad)
-    646ca3e5:	pop    %rsi
+    646ca3e4:	jo     646ca441 <.pdata+0x9>
     646ca3e6:	add    %al,(%rax)
-    646ca3e8:	rex.WR pop %rdi
+    646ca3e8:	pop    %rsp
+    646ca3e9:	pop    %rsp
     646ca3ea:	add    %al,(%rax)
     646ca3ec:	(bad)
     646ca3ed:	mov    $0x0,%bl
-    646ca3ef:	add    %dl,0x5f(%rax)
+    646ca3ef:	add    %ah,0x5c(%rax)
     646ca3f2:	add    %al,(%rax)
-    646ca3f4:	(bad)
-    646ca3f5:	(bad)
+    646ca3f4:	rex.RXB pop %r14
     646ca3f6:	add    %al,(%rax)
     646ca3f8:	(bad)
     646ca3f9:	mov    $0x0,%bl
-    646ca3fb:	add    %al,0x61(%rax)
+    646ca3fb:	add    %dl,0x5e(%rax)
     646ca3fe:	add    %al,(%rax)
-    646ca400:	stos   %al,%es:(%rdi)
-    646ca401:	(bad)
-    646ca402:	add    %al,(%rax)
-    646ca404:	fdivl  0x61b00000(%rbx)
+    646ca400:	mov    $0xdc00005e,%edx
+    646ca405:	mov    $0x0,%bl
+	...
 
 00000000646ca408 <.pdata>:
-    646ca408:	mov    $0x61,%al
-    646ca40a:	add    %al,(%rax)
+    646ca408:	rcrb   $0x0,0x0(%rsi)
     646ca40c:	(bad)
-    646ca40d:	(bad)
+    646ca40d:	pop    %rdi
     646ca40e:	add    %al,(%rax)
     646ca410:	in     (%dx),%al
     646ca411:	mov    $0x0,%bl
-    646ca413:	add    %dh,(%rax)
-    646ca415:	(bad)
+    646ca413:	add    %al,0x5f(%rax)
     646ca416:	add    %al,(%rax)
-    646ca418:	shlb   0x0(%rdx)
-    646ca41b:	add    %bh,%ah
+    646ca418:	loopne 646ca479 <.pdata+0x41>
+    646ca41a:	add    %al,(%rax)
+    646ca41c:	cld
     646ca41d:	mov    $0x0,%bl
-    646ca41f:	add    %dl,%al
-    646ca421:	(bad)
+    646ca41f:	add    %ah,%al
+    646ca421:	pop    %rdi
     646ca422:	add    %al,(%rax)
-    646ca424:	stos   %al,%es:(%rdi)
-    646ca425:	movsxd (%rax),%eax
-    646ca427:	add    %al,(%rsp,%rsi,4)
-    646ca42a:	add    %al,(%rax)
-    646ca42c:	mov    $0x63,%al
+    646ca424:	mov    $0x4000060,%edx
+    646ca429:	mov    $0x0,%ah
+    646ca42b:	add    %al,%al
+    646ca42d:	(bad)
     646ca42e:	add    %al,(%rax)
-    646ca430:	(bad)
-    646ca431:	movsxd (%rax),%eax
+    646ca430:	fisubs 0x0(%rax)
     646ca433:	add    %cl,(%rsp,%rsi,4)
 	...
 
 00000000646ca438 <.pdata>:
-    646ca438:	shlb   0x0(%rbx)
-    646ca43b:	add    %ah,%dl
-    646ca43d:	movsxd (%rax),%eax
-    646ca43f:	add    %dl,(%rax)
-    646ca441:	mov    $0x0,%ah
-    646ca443:	add    %dh,%al
-    646ca445:	movsxd (%rax),%eax
-    646ca447:	add    %dh,(%rsp,%riz,2)
-    646ca44a:	add    %al,(%rax)
-    646ca44c:	adc    $0xb4,%al
+    646ca438:	loopne 646ca49a <.pdata+0x62>
+    646ca43a:	add    %al,(%rax)
+    646ca43c:	repnz (bad)
+    646ca43e:	add    %al,(%rax)
+    646ca440:	adc    %dh,0x610000(%rax,%rax,1)
+    646ca447:	add    %al,0x0(%rcx,%riz,2)
+    646ca44b:	add    %dl,(%rsp,%rsi,4)
     646ca44e:	add    %al,(%rax)
-    646ca450:	rex
-    646ca451:	add    %al,%fs:(%rax)
-    646ca454:	int    $0x64
-    646ca456:	add    %al,(%rax)
-    646ca458:	sbb    %dh,0x64d000(%rax,%rax,1)
-    646ca45f:	add    %al,0x0(%rbp,%riz,2)
-    646ca463:	add    %ah,(%rsp,%rsi,4)
+    646ca450:	push   %rax
+    646ca451:	(bad)
+    646ca452:	add    %al,(%rax)
+    646ca454:	frstor 0x0(%rcx)
+    646ca457:	add    %bl,(%rax)
+    646ca459:	mov    $0x0,%ah
+    646ca45b:	add    %ah,%al
+    646ca45d:	(bad)
+    646ca45e:	add    %al,(%rax)
+    646ca460:	push   %rsp
+    646ca461:	(bad)
+    646ca462:	add    %al,(%rax)
+    646ca464:	and    $0xb4,%al
     646ca466:	add    %al,(%rax)
-    646ca468:	push   %rax
-    646ca469:	add    %al,%gs:(%rax)
-    646ca46c:	mov    0x0(%rbp),%fs
-    646ca46f:	add    %ch,(%rsp,%rsi,4)
+    646ca468:	(bad)
+    646ca469:	(bad)
+    646ca46a:	add    %al,(%rax)
+    646ca46c:	sahf
+    646ca46d:	(bad)
+    646ca46e:	add    %al,(%rax)
+    646ca470:	sub    $0xb4,%al
     646ca472:	add    %al,(%rax)
-    646ca474:	nop
-    646ca475:	add    %al,%gs:(%rax)
-    646ca478:	jmp    *0x0(%rbp)
-    646ca47b:	add    %dh,(%rsp,%rsi,4)
-    646ca47e:	add    %al,(%rax)
-    646ca480:	add    %ah,0x0(%rsi)
-    646ca483:	add    %dh,(%rdi)
-    646ca485:	data16 add %al,(%rax)
+    646ca474:	movabs 0x340000630f000062,%al
+    646ca47d:	mov    $0x0,%ah
+    646ca47f:	add    %dl,(%rax)
+    646ca481:	movsxd (%rax),%eax
+    646ca483:	add    %al,0x63(%rdi)
+    646ca486:	add    %al,(%rax)
     646ca488:	cmp    $0xb4,%al
     646ca48a:	add    %al,(%rax)
-    646ca48c:	rex
-    646ca48d:	data16 add %al,(%rax)
-    646ca490:	shll   0x0(%rsi)
+    646ca48c:	push   %rax
+    646ca48d:	movsxd (%rax),%eax
+    646ca48f:	add    %ah,%cl
+    646ca491:	movsxd (%rax),%eax
     646ca493:	add    %al,0x0(%rsp,%rsi,4)
-    646ca497:	add    %ah,%al
-    646ca499:	data16 add %al,(%rax)
-    646ca49c:	xchg   %ah,0x0(%rdi)
-    646ca49f:	add    %cl,0x0(%rsp,%rsi,4)
-    646ca4a3:	add    %dl,-0x6cffff99(%rax)
-    646ca4a9:	add    %al,(%eax)
+    646ca497:	add    %dh,%al
+    646ca499:	movsxd (%rax),%eax
+    646ca49b:	add    %dl,0x4c000064(%rsi)
+    646ca4a1:	mov    $0x0,%ah
+    646ca4a3:	add    %ah,-0x5cffff9c(%rax)
+    646ca4a9:	add    %al,%fs:(%rax)
     646ca4ac:	push   %rsp
     646ca4ad:	mov    $0x0,%ah
 	...
 
 00000000646ca4b0 <.pdata>:
-    646ca4b0:	loopne 646ca519 <.pdata+0x9>
-    646ca4b2:	add    %al,(%rax)
-    646ca4b4:	out    %al,$0x67
-    646ca4b6:	add    %al,(%rax)
+    646ca4b0:	lock add %al,%fs:(%rax)
+    646ca4b4:	mulb   0x0(%rax,%rax,1)
     646ca4b8:	pop    %rax
     646ca4b9:	mov    $0x0,%ah
 	...
 
 00000000646ca4bc <.pdata>:
-    646ca4bc:	lock add %al,(%eax)
-    646ca4c0:	mulb   0x0(%rdi)
-    646ca4c3:	add    %bl,0x0(%rsp,%rsi,4)
+    646ca4bc:	add    %ah,0x0(%rbp)
+    646ca4bf:	add    %al,(%rsi)
+    646ca4c1:	add    %al,%gs:(%rax)
+    646ca4c4:	pop    %rsp
+    646ca4c5:	mov    $0x0,%ah
 	...
 
 00000000646ca4c8 <.pdata>:
-    646ca4c8:	add    %ch,0x0(%rax)
-    646ca4cb:	add    %dl,0x0(%rax,%rbp,2)
+    646ca4c8:	adc    %ah,0x0(%rbp)
+    646ca4cb:	add    %ah,0x0(%rbp,%riz,2)
     646ca4cf:	add    %ah,-0x4c(%rax)
 	...
 
 00000000646ca4d4 <.pdata>:
-    646ca4d4:	(bad)
-    646ca4d5:	push   $0x69860000
-    646ca4da:	add    %al,(%rax)
+    646ca4d4:	jo     646ca53b <.pdata+0x13>
+    646ca4d6:	add    %al,(%rax)
+    646ca4d8:	xchg   %eax,%esi
+    646ca4d9:	data16 add %al,(%rax)
     646ca4dc:	fs mov $0x0,%ah
 	...
 
 00000000646ca4e0 <.pdata>:
-    646ca4e0:	nop
-    646ca4e1:	imul   $0x699500,(%rax),%eax
-    646ca4e7:	add    %dh,-0x4c(%rax)
+    646ca4e0:	movabs 0x70000066a5000066,%al
+    646ca4e9:	mov    $0x0,%ah
 	...
 
 00000000646ca4ec <.pdata>:
-    646ca4ec:	movabs 0x7400006a77000069,%al
-    646ca4f5:	mov    $0x0,%ah
+    646ca4ec:	mov    $0x66,%al
+    646ca4ee:	add    %al,(%rax)
+    646ca4f0:	xchg   %esp,0x0(%rdi)
+    646ca4f3:	add    %dh,0x0(%rsp,%rsi,4)
 	...
 
 00000000646ca4f8 <.pdata>:
-    646ca4f8:	subb   $0x0,0x0(%rdx)
-    646ca4fc:	je     646ca569 <.pdata+0x11>
-    646ca4fe:	add    %al,(%rax)
-    646ca500:	js     646ca4b6 <.pdata+0x6>
+    646ca4f8:	nop
+    646ca4f9:	add    %al,(%eax)
+    646ca4fc:	test   %ch,0x0(%rax)
+    646ca4ff:	add    %bh,-0x4c(%rax)
 	...
 
 00000000646ca504 <.pdata>:
-    646ca504:	mov    $0x6b,%al
-    646ca506:	add    %al,(%rax)
-    646ca508:	xchg   %eax,%esp
-    646ca509:	insl   (%dx),%es:(%rdi)
-    646ca50a:	add    %al,(%rax)
-    646ca50c:	test   %dh,0x6da000(%rax,%rax,1)
+    646ca504:	shrb   $0x0,0x0(%rax)
+    646ca508:	movsb  %ds:(%rsi),%es:(%rdi)
+    646ca509:	push   $0x0
+    646ca50b:	add    %al,0x6ab00000(%rsp,%rsi,4)
 
 00000000646ca510 <.pdata>:
-    646ca510:	movabs 0x9000006ec000006d,%al
-    646ca519:	mov    $0x0,%ah
-	...
+    646ca510:	mov    $0x6a,%al
+    646ca512:	add    %al,(%rax)
+    646ca514:	shrb   0x0(%rbx)
+    646ca517:	add    %dl,-0x2fffff4c(%rax)
 
 00000000646ca51c <.pdata>:
-    646ca51c:	shrb   $0x0,0x0(%rsi)
-    646ca520:	push   %rsi
-    646ca521:	outsl  %ds:(%rsi),(%dx)
+    646ca51c:	shrb   0x0(%rbx)
+    646ca51f:	add    %ah,0x6c(%rsi)
     646ca522:	add    %al,(%rax)
     646ca524:	pushf
     646ca525:	mov    $0x0,%ah
 	...
 
 00000000646ca528 <.pdata>:
-    646ca528:	(bad)
-    646ca529:	outsl  %ds:(%rsi),(%dx)
+    646ca528:	jo     646ca596 <.pdata+0xe>
     646ca52a:	add    %al,(%rax)
-    646ca52c:	mov    $0x74,%bh
-    646ca52e:	add    %al,(%rax)
-    646ca530:	movsb  %ds:(%rsi),%es:(%rdi)
-    646ca531:	mov    $0x0,%ah
-    646ca533:	add    %al,%al
-    646ca535:	je     646ca537 <.pdata+0xf>
-    646ca537:	add    %bh,(%rsi)
-    646ca539:	ja     646ca53b <.pdata+0x13>
+    646ca52c:	(bad)
+    646ca52d:	jno    646ca52f <.pdata+0x7>
+    646ca52f:	add    %ah,0x71d00000(%rsp,%rsi,4)
+    646ca536:	add    %al,(%rax)
+    646ca538:	rex.WRX je 646ca53b <.pdata+0x13>
     646ca53b:	add    %al,%al
     646ca53d:	mov    $0x0,%ah
 	...
 
 00000000646ca540 <.pdata>:
-    646ca540:	adc    %bh,0x0(%rax)
-    646ca543:	add    %cl,%dh
-    646ca545:	js     646ca547 <.pdata+0x7>
+    646ca540:	and    %dh,0x0(%rbp)
+    646ca543:	add    %bl,%dh
+    646ca545:	jne    646ca547 <.pdata+0x7>
     646ca547:	add    %cl,%ah
     646ca549:	mov    $0x0,%ah
 	...
 
 00000000646ca54c <.pdata>:
-    646ca54c:	lock jns 646ca54f <.pdata+0x3>
-    646ca54f:	add    %dl,-0x2bffff86(%rip)        # 386ca5cf <__size_of_stack_reserve__+0x384ca5cf>
+    646ca54c:	add    %dh,0x0(%rdi)
+    646ca54f:	add    %ah,-0x2bffff89(%rip)        # 386ca5cc <__size_of_stack_reserve__+0x384ca5cc>
     646ca555:	mov    $0x0,%ah
 	...
 
 00000000646ca558 <.pdata>:
-    646ca558:	and    %bh,0x0(%rdx)
-    646ca55b:	add    %ch,%al
-    646ca55d:	jp     646ca55f <.pdata+0x7>
+    646ca558:	xor    %dh,0x0(%rdi)
+    646ca55b:	add    %bh,%al
+    646ca55d:	ja     646ca55f <.pdata+0x7>
     646ca55f:	add    %bl,%al
     646ca561:	mov    $0x0,%ah
-    646ca563:	add    %dh,%al
-    646ca565:	jp     646ca567 <.pdata+0xf>
-    646ca567:	add    %bl,0x7b(%rdi)
+    646ca563:	add    %al,(%rax)
+    646ca565:	js     646ca567 <.pdata+0xf>
+    646ca567:	add    %ch,0x78(%rdi)
     646ca56a:	add    %al,(%rax)
-    646ca56c:	call   c46ca625 <.debug_str+0x5fff2625>
-    646ca571:	jnp    646ca573 <.pdata+0x1b>
-    646ca573:	add    %bh,0x7b(%rdi)
-    646ca576:	add    %al,(%rax)
-    646ca578:	hlt
+    646ca56c:	call   d46ca625 <.debug_str+0x6fff2625>
+    646ca571:	js     646ca573 <.pdata+0x1b>
+    646ca573:	add    %cl,-0xbffff88(%rdi)
     646ca579:	mov    $0x0,%ah
 	...
 
 00000000646ca57c <.pdata>:
-    646ca57c:	push   %rax
-    646ca57d:	jl     646ca57f <.pdata+0x3>
-    646ca57f:	add    %dl,-0x3ffff84(%rcx)
+    646ca57c:	(bad)
+    646ca57d:	jns    646ca57f <.pdata+0x3>
+    646ca57f:	add    %ah,-0x3ffff87(%rcx)
     646ca585:	mov    $0x0,%ah
 	...
 
 00000000646ca588 <.pdata>:
-    646ca588:	movabs 0x400007cac00007c,%al
+    646ca588:	mov    $0x79,%al
+    646ca58a:	add    %al,(%rax)
+    646ca58c:	mov    $0x4000079,%esp
     646ca591:	mov    $0x0,%ch
-    646ca593:	add    %dh,-0x53ffff84(%rax)
-    646ca599:	jge    646ca59b <.pdata+0x13>
-    646ca59b:	add    %cl,(%rax)
-    646ca59d:	mov    $0x0,%ch
-    646ca59f:	add    %al,%al
-    646ca5a1:	jge    646ca5a3 <.pdata+0x1b>
-    646ca5a3:	add    %ch,(%rcx)
-    646ca5a5:	jle    646ca5a7 <.pdata+0x1f>
-    646ca5a7:	add    %cl,0x300000b3(%rax)
+    646ca593:	add    %al,%al
+    646ca595:	jns    646ca597 <.pdata+0xf>
+    646ca597:	add    %bh,-0x4af80000(%rdx,%rdi,2)
+    646ca59e:	add    %al,(%rax)
+    646ca5a0:	sarb   0x0(%rdx)
+    646ca5a3:	add    %bh,(%rcx)
+    646ca5a5:	jnp    646ca5a7 <.pdata+0x1f>
+    646ca5a7:	add    %cl,0x400000b3(%rax)
 
 00000000646ca5ac <.pdata.startup>:
-    646ca5ac:	xor    %bh,0x0(%rsi)
-    646ca5af:	add    %dh,0x2000007e(%rip)        # 846ca633 <.debug_str+0x1fff2633>
+    646ca5ac:	rex jnp 646ca5af <.pdata.startup+0x3>
+    646ca5af:	add    %al,0x7b(%rbp)
+    646ca5b2:	add    %al,(%rax)
+    646ca5b4:	.byte 0x20
     646ca5b5:	mov    $0x0,%ch
 	...
 
 Disassembly of section .xdata:
 
 00000000646cb000 <.xdata>:
     646cb000:	add    %eax,(%rax)
@@ -12639,30 +12447,30 @@
     646cb2e5:	or     %al,(%rbx)
     646cb2e7:	add    $0x3043208,%eax
     646cb2ec:	add    %edx,0x0(%rax)
 	...
 
 00000000646cb2f0 <.xdata>:
     646cb2f0:	add    %ecx,(%rax)
-    646cb2f2:	add    0x3043208(%rip),%eax        # 6770e500 <.debug_str+0x3036500>
+    646cb2f2:	add    0x3041208(%rip),%eax        # 6770c500 <.debug_str+0x3034500>
     646cb2f8:	add    %edx,0x0(%rax)
     646cb2fb:	add    %al,(%rcx)
     646cb2fd:	or     %al,(%rbx)
     646cb2ff:	add    $0x3045208,%eax
     646cb304:	add    %edx,0x0(%rax)
     646cb307:	add    %al,(%rcx)
     646cb309:	or     %al,(%rbx)
     646cb30b:	add    $0x3045208,%eax
     646cb310:	add    %edx,0x0(%rax)
 	...
 
 00000000646cb314 <.xdata>:
     646cb314:	add    %edx,(%rcx)
     646cb316:	add    $0x9031185,%eax
-    646cb31b:	add    %edx,(%rcx)
+    646cb31b:	add    %edx,(%rdi)
     646cb31d:	add    %al,(%rdx)
     646cb31f:	xor    %al,(%rcx)
     646cb321:	push   %rax
     646cb322:	add    %al,(%rax)
     646cb324:	add    %ecx,(%rax)
     646cb326:	add    0x3047208(%rip),%eax        # 67712534 <.debug_str+0x303a534>
     646cb32c:	add    %edx,0x0(%rax)
@@ -13084,216 +12892,224 @@
 	...
 
 Disassembly of section .edata:
 
 00000000646cd000 <.edata>:
     646cd000:	add    %al,(%rax)
     646cd002:	add    %al,(%rax)
-    646cd004:	mov    $0x27,%dh
-    646cd006:	outsb  %ds:(%rsi),(%dx)
+    646cd004:	ss loope 646cd07c <.edata+0x7c>
     646cd007:	add    %al,%fs:(%rax)
     646cd00a:	add    %al,(%rax)
     646cd00c:	mov    %dl,%dl
     646cd00e:	add    %al,(%rax)
     646cd010:	add    %eax,(%rax)
     646cd012:	add    %al,(%rax)
     646cd014:	cmp    $0x3d000000,%eax
     646cd019:	add    %al,(%rax)
     646cd01b:	add    %ch,(%rax)
     646cd01d:	rolb   (%rax)
     646cd01f:	add    %bl,(%rcx,%rdx,8)
     646cd022:	add    %al,(%rax)
     646cd024:	adc    %dl,%dl
     646cd026:	add    %al,(%rax)
-    646cd028:	mov    $0x4e,%al
-    646cd02a:	add    %al,(%rax)
-    646cd02c:	sub    %eax,0x0(%rbx)
-    646cd02f:	add    %ah,%dl
-    646cd031:	sbb    %al,(%rax)
-    646cd033:	add    %al,(%rdi,%rdx,1)
+    646cd028:	sub    %eax,0x0(%rbx)
+    646cd02b:	add    %ah,%dl
+    646cd02d:	sbb    %al,(%rax)
+    646cd02f:	add    %al,(%rdi,%rdx,1)
+    646cd032:	add    %al,(%rax)
+    646cd034:	mov    $0x13,%al
     646cd036:	add    %al,(%rax)
-    646cd038:	mov    $0x13,%al
-    646cd03a:	add    %al,(%rax)
-    646cd03c:	rex.XB adc $0x278e0000,%eax
+    646cd038:	rex.XB adc $0x278e0000,%eax
+    646cd03e:	add    %al,(%rax)
+    646cd040:	push   %rdx
+    646cd041:	(bad)
     646cd042:	add    %al,(%rax)
-    646cd044:	push   %rdx
-    646cd045:	(bad)
+    646cd044:	(bad)  (%rsi)
     646cd046:	add    %al,(%rax)
-    646cd048:	(bad)  (%rsi)
+    646cd048:	(bad)
+    646cd049:	(bad)
     646cd04a:	add    %al,(%rax)
-    646cd04c:	(bad)
-    646cd04d:	(bad)
-    646cd04e:	add    %al,(%rax)
-    646cd050:	rex.WR and %r8b,(%rax)
-    646cd053:	add    %dl,0x0(%rsi,%rbx,1)
-    646cd057:	add    %cl,%bh
-    646cd059:	sbb    (%rax),%al
-    646cd05b:	add    %bh,0x1c(%rdx)
-    646cd05e:	add    %al,(%rax)
-    646cd060:	rex.WX
-    646cd061:	es add %al,(%rax)
-    646cd064:	mov    $0x25,%ch
-    646cd066:	add    %al,(%rax)
-    646cd068:	lea    (%rax,%rax,1),%esp
-    646cd06b:	add    %ah,(%rax)
-    646cd06d:	and    $0x28c60000,%eax
-    646cd072:	add    %al,(%rax)
-    646cd074:	push   $0xffffffffca000028
-    646cd079:	(bad)
-    646cd07a:	add    %al,(%rax)
-    646cd07c:	(bad)
-    646cd07d:	sub    %al,(%rax)
-    646cd07f:	add    %al,(%rcx)
-    646cd081:	and    $0x0,%al
-    646cd083:	add    %dh,0x23(%rcx)
-    646cd086:	add    %al,(%rax)
-    646cd088:	push   %rbx
+    646cd04c:	rex.WR and %r8b,(%rax)
+    646cd04f:	add    %dl,0x0(%rsi,%rbx,1)
+    646cd053:	add    %cl,%bh
+    646cd055:	sbb    (%rax),%al
+    646cd057:	add    %bh,0x1c(%rdx)
+    646cd05a:	add    %al,(%rax)
+    646cd05c:	rex.WX
+    646cd05d:	es add %al,(%rax)
+    646cd060:	mov    $0x25,%ch
+    646cd062:	add    %al,(%rax)
+    646cd064:	lea    (%rax,%rax,1),%esp
+    646cd067:	add    %ah,(%rax)
+    646cd069:	and    $0x28c60000,%eax
+    646cd06e:	add    %al,(%rax)
+    646cd070:	push   $0xffffffffca000028
+    646cd075:	(bad)
+    646cd076:	add    %al,(%rax)
+    646cd078:	(bad)
+    646cd079:	sub    %al,(%rax)
+    646cd07b:	add    %al,(%rcx)
+    646cd07d:	and    $0x0,%al
+    646cd07f:	add    %dh,0x23(%rcx)
+    646cd082:	add    %al,(%rax)
+    646cd084:	push   %rbx
+    646cd085:	and    (%rax),%al
+    646cd087:	add    %ah,%cl
     646cd089:	and    (%rax),%al
-    646cd08b:	add    %ah,%cl
-    646cd08d:	and    (%rax),%al
-    646cd08f:	add    %cl,%al
-    646cd091:	sub    %eax,(%rax)
-    646cd093:	add    %ch,0x29(%rsi)
-    646cd096:	add    %al,(%rax)
-    646cd098:	cs sub %eax,(%rax)
-    646cd09b:	add    %cl,0x0(%rcx,%rbp,1)
-    646cd09f:	add    %ah,(%rdi,%rbp,1)
-    646cd0a2:	add    %al,(%rax)
-    646cd0a4:	cs xor %al,(%rax)
-    646cd0a7:	add    %al,%al
-    646cd0a9:	cs add %al,(%rax)
-    646cd0ac:	addl   $0x38c700,0x0(%rbx)
-    646cd0b3:	add    %bh,0x3a(%rbx)
-    646cd0b6:	add    %al,(%rax)
-    646cd0b8:	pop    %rbp
-    646cd0b9:	xor    (%rax),%al
-    646cd0bb:	add    %bl,0x1a00003f(%rax)
-    646cd0c1:	cmp    $0x0,%al
-    646cd0c3:	add    %dl,-0x51ffffbc(%rax)
-    646cd0c9:	sub    (%rax),%al
-    646cd0cb:	add    %bl,0x2d(%rsi)
+    646cd08b:	add    %cl,%al
+    646cd08d:	sub    %eax,(%rax)
+    646cd08f:	add    %ch,0x29(%rsi)
+    646cd092:	add    %al,(%rax)
+    646cd094:	cs sub %eax,(%rax)
+    646cd097:	add    %cl,0x0(%rcx,%rbp,1)
+    646cd09b:	add    %ah,(%rdi,%rbp,1)
+    646cd09e:	add    %al,(%rax)
+    646cd0a0:	cs xor %al,(%rax)
+    646cd0a3:	add    %al,%al
+    646cd0a5:	cs add %al,(%rax)
+    646cd0a8:	addl   $0x38c700,0x0(%rbx)
+    646cd0af:	add    %bh,0x3a(%rbx)
+    646cd0b2:	add    %al,(%rax)
+    646cd0b4:	pop    %rbp
+    646cd0b5:	xor    (%rax),%al
+    646cd0b7:	add    %bl,0x1a00003f(%rax)
+    646cd0bd:	cmp    $0x0,%al
+    646cd0bf:	add    %dl,-0x51ffffbc(%rax)
+    646cd0c5:	sub    (%rax),%al
+    646cd0c7:	add    %bl,0x2d(%rsi)
+    646cd0ca:	add    %al,(%rax)
+    646cd0cc:	mov    $0x2d,%dl
     646cd0ce:	add    %al,(%rax)
-    646cd0d0:	mov    $0x2d,%dl
-    646cd0d2:	add    %al,(%rax)
-    646cd0d4:	stos   %al,%es:(%rdi)
+    646cd0d0:	stos   %al,%es:(%rdi)
+    646cd0d1:	sub    $0x0,%al
+    646cd0d3:	add    %dh,%ah
     646cd0d5:	sub    $0x0,%al
-    646cd0d7:	add    %dh,%ah
-    646cd0d9:	sub    $0x0,%al
-    646cd0db:	add    %ch,0x2c(%rbp)
+    646cd0d7:	add    %ch,0x2c(%rbp)
+    646cd0da:	add    %al,(%rax)
+    646cd0dc:	xor    %ch,(%rdx)
     646cd0de:	add    %al,(%rax)
-    646cd0e0:	xor    %ch,(%rdx)
-    646cd0e2:	add    %al,(%rax)
+    646cd0e0:	(bad)
+    646cd0e1:	cs add %al,(%rax)
     646cd0e4:	(bad)
-    646cd0e5:	cs add %al,(%rax)
+    646cd0e5:	rex.WRB add %r8b,(%r8)
     646cd0e8:	fldl   0x0(%rbx)
-    646cd0eb:	add    %dh,-0x2fffffb0(%rcx)
-    646cd0f1:	rex.RX add %r8b,(%rax)
-    646cd0f4:	xorb   $0x0,(%rcx)
-    646cd0f7:	add    %dh,(%rcx)
+    646cd0eb:	add    %dl,%ch
+    646cd0ed:	rex.WRB add %r8b,(%r8)
+    646cd0f0:	rolb   0x0(%rsi)
+    646cd0f3:	add    %al,0x31000031(%rax)
     646cd0f9:	xor    (%rax),%al
-    646cd0fb:	add    %bl,-0x7fffffbb(%rip)        # ffffffffe46cd146 <.debug_str+0xffffffff7fff5146>
-    646cd101:	rex.RXB add %r8b,(%r8)
-    646cd104:	in     $0x47,%eax
+    646cd0fb:	add    %bl,(%rdi)
+    646cd0fd:	add    %r8b,(%r8)
+    646cd100:	addb   $0x0,0x0(%rdi)
+    646cd104:	out    %al,$0x47
     646cd106:	add    %al,(%rax)
-    646cd108:	fwait
-    646cd109:	rex.WR add %r8b,(%rax)
-    646cd10c:	mov    $0x20000034,%ecx
-    646cd111:	rex.WRB add %r8b,(%r8)
-    646cd114:	pushf
-    646cd115:	push   %rbx
+    646cd108:	or     0x0(%rax,%rax,1),%cl
+    646cd10c:	mov    $0x90000034,%ecx
+    646cd111:	rex.WR add %r8b,(%rax)
+    646cd114:	mov    $0x50,%dh
     646cd116:	add    %al,(%rax)
-    646cd118:	and    %dl,0x0(%rcx)
-    646cd11b:	add    %dl,-0x5cffff2e(%rdi)
-    646cd121:	rolb   %cl,(%rax)
-    646cd123:	add    %ch,-0x42ffff2e(%rdx)
+    646cd118:	rex
+    646cd119:	rex.WRX add %r8b,(%rax)
+    646cd11c:	xchg   %eax,%edi
+    646cd11d:	rolb   %cl,(%rax)
+    646cd11f:	add    %bl,-0x4effff2e(%rsi)
+    646cd125:	rolb   %cl,(%rax)
+    646cd127:	add    %al,%bl
     646cd129:	rolb   %cl,(%rax)
-    646cd12b:	add    %cl,%bh
+    646cd12b:	add    %dl,%bl
     646cd12d:	rolb   %cl,(%rax)
-    646cd12f:	add    %bl,%bh
+    646cd12f:	add    %ch,%cl
     646cd131:	rolb   %cl,(%rax)
-    646cd133:	add    %dh,%ch
+    646cd133:	add    %bh,%ch
     646cd135:	rolb   %cl,(%rax)
-    646cd137:	add    %cl,(%rcx)
+    646cd137:	add    %dl,(%rax)
     646cd139:	roll   %cl,(%rax)
-    646cd13b:	add    %bl,(%rbx,%rdx,8)
-    646cd13e:	add    %al,(%rax)
-    646cd140:	sub    $0x440000d3,%eax
-    646cd145:	roll   %cl,(%rax)
-    646cd147:	add    %dl,-0x2d(%rdi)
-    646cd14a:	add    %al,(%rax)
-    646cd14c:	imul   $0xd3790000,%ebx,%edx
-    646cd152:	add    %al,(%rax)
-    646cd154:	(bad)
-    646cd155:	roll   %cl,(%rax)
-    646cd157:	add    %ah,-0x4bffff2d(%rdx)
-    646cd15d:	roll   %cl,(%rax)
-    646cd15f:	add    %al,%ah
+    646cd13b:	add    %ah,(%rcx)
+    646cd13d:	roll   %cl,(%rax)
+    646cd13f:	add    %bh,(%rax)
+    646cd141:	roll   %cl,(%rax)
+    646cd143:	add    %cl,-0x2d(%rbx)
+    646cd146:	add    %al,(%rax)
+    646cd148:	pop    %rbp
+    646cd149:	roll   %cl,(%rax)
+    646cd14b:	add    %ch,-0x2d(%rbp)
+    646cd14e:	add    %al,(%rax)
+    646cd150:	adc    $0x0,%ebx
+    646cd153:	add    %dl,-0x57ffff2d(%rsi)
+    646cd159:	roll   %cl,(%rax)
+    646cd15b:	add    %bh,-0x31ffff2d(%rax)
     646cd161:	roll   %cl,(%rax)
-    646cd163:	add    %bl,%dl
+    646cd163:	add    %ah,%cl
     646cd165:	roll   %cl,(%rax)
-    646cd167:	add    %ch,%ch
+    646cd167:	add    %dh,%bl
     646cd169:	roll   %cl,(%rax)
-    646cd16b:	add    %bh,%bh
-    646cd16d:	roll   %cl,(%rax)
-    646cd16f:	add    %cl,(%rdi)
-    646cd171:	(bad)
+    646cd16b:	add    %al,(%rbx)
+    646cd16d:	(bad)
+    646cd16e:	add    %al,(%rax)
+    646cd170:	adc    $0xd4,%al
     646cd172:	add    %al,(%rax)
-    646cd174:	and    %dl,%ah
+    646cd174:	(bad)
+    646cd175:	(bad)
     646cd176:	add    %al,(%rax)
-    646cd178:	xor    %esp,%edx
+    646cd178:	cmp    %edx,%esp
     646cd17a:	add    %al,(%rax)
-    646cd17c:	rex.RB (bad)
+    646cd17c:	rex.WB (bad)
     646cd17e:	add    %al,(%rax)
-    646cd180:	push   %rbp
+    646cd180:	pop    %rdi
     646cd181:	(bad)
     646cd182:	add    %al,(%rax)
-    646cd184:	imul   $0x0,%esp,%edx
-    646cd187:	add    %bh,-0x2c(%rdx)
+    646cd184:	outsb  %ds:(%rsi),(%dx)
+    646cd185:	(bad)
+    646cd186:	add    %al,(%rax)
+    646cd188:	jl     646cd15e <.edata+0x15e>
     646cd18a:	add    %al,(%rax)
     646cd18c:	mov    %dl,%ah
     646cd18e:	add    %al,(%rax)
-    646cd190:	xchg   %eax,%esp
+    646cd190:	xchg   %eax,%ebp
     646cd191:	(bad)
     646cd192:	add    %al,(%rax)
-    646cd194:	movabs 0xb70000d4ab0000d4,%eax
-    646cd19d:	(bad)
-    646cd19e:	add    %al,(%rax)
-    646cd1a0:	(bad)
+    646cd194:	lahf
+    646cd195:	(bad)
+    646cd196:	add    %al,(%rax)
+    646cd198:	stos   %eax,%es:(%rdi)
+    646cd199:	(bad)
+    646cd19a:	add    %al,(%rax)
+    646cd19c:	mov    $0xc30000d4,%edx
     646cd1a1:	(bad)
     646cd1a2:	add    %al,(%rax)
-    646cd1a4:	iret
-    646cd1a5:	(bad)
+    646cd1a4:	rcl    %esp
     646cd1a6:	add    %al,(%rax)
-    646cd1a8:	fst    %st(4)
+    646cd1a8:	jrcxz  646cd17e <.edata+0x17e>
     646cd1aa:	add    %al,(%rax)
-    646cd1ac:	out    %eax,(%dx)
-    646cd1ad:	(bad)
+    646cd1ac:	not    %esp
     646cd1ae:	add    %al,(%rax)
-    646cd1b0:	add    %ebp,%edx
+    646cd1b0:	or     %dl,%ch
     646cd1b2:	add    %al,(%rax)
-    646cd1b4:	adc    $0xd5,%al
+    646cd1b4:	sbb    %ch,%dl
     646cd1b6:	add    %al,(%rax)
-    646cd1b8:	es (bad)
-    646cd1ba:	add    %al,(%rax)
-    646cd1bc:	xor    %edx,%ebp
+    646cd1b8:	and    $0x360000d5,%eax
+    646cd1bd:	(bad)
     646cd1be:	add    %al,(%rax)
-    646cd1c0:	rex.X (bad)
+    646cd1c0:	rex.WB (bad)
     646cd1c2:	add    %al,(%rax)
-    646cd1c4:	push   %rbp
-    646cd1c5:	(bad)
+    646cd1c4:	(bad)
     646cd1c6:	add    %al,(%rax)
-    646cd1c8:	outsb  %ds:(%rsi),(%dx)
-    646cd1c9:	(bad)
+    646cd1c8:	je     646cd19f <.edata+0x19f>
     646cd1ca:	add    %al,(%rax)
-    646cd1cc:	adc    $0x0,%ch
-    646cd1cf:	add    %bl,-0x4fffff2b(%rax)
-    646cd1d5:	(bad)
+    646cd1cc:	mov    %ss,%ebp
+    646cd1ce:	add    %al,(%rax)
+    646cd1d0:	movsb  %ds:(%rsi),%es:(%rdi)
+    646cd1d1:	(bad)
+    646cd1d2:	add    %al,(%rax)
+    646cd1d4:	mov    $0xd5,%cl
     646cd1d6:	add    %al,(%rax)
-    646cd1d8:	mov    $0xd30000d5,%ebp
-    646cd1dd:	(bad)
+    646cd1d8:	(bad)
+    646cd1d9:	(bad)
+    646cd1da:	add    %al,(%rax)
+    646cd1dc:	rcl    %cl,%ebp
     646cd1de:	add    %al,(%rax)
     646cd1e0:	(bad)
     646cd1e2:	add    %al,(%rax)
     646cd1e4:	in     $0xd5,%eax
     646cd1e6:	add    %al,(%rax)
     646cd1e8:	lock (bad)
     646cd1ea:	add    %al,(%rax)
@@ -13309,18 +13125,18 @@
     646cd1fc:	cmp    $0xd6,%al
     646cd1fe:	add    %al,(%rax)
     646cd200:	rex.WB (bad)
     646cd202:	add    %al,(%rax)
     646cd204:	pop    %rax
     646cd205:	(bad)
     646cd206:	add    %al,(%rax)
-    646cd208:	pop    %rbp
+    646cd208:	(bad)
     646cd209:	(bad)
     646cd20a:	add    %al,(%rax)
-    646cd20c:	data16 (bad)
+    646cd20c:	push   $0xffffffffffffffd6
     646cd20e:	add    %al,(%rax)
     646cd210:	add    %al,(%rax)
     646cd212:	add    %eax,(%rax)
     646cd214:	add    (%rax),%al
     646cd216:	add    (%rax),%eax
     646cd218:	add    $0x0,%al
     646cd21a:	add    $0x7000600,%eax
@@ -13368,429 +13184,429 @@
     646cd28a:	jne    646cd2ef <.edata+0x2ef>
     646cd28c:	pop    %rdi
     646cd28d:	jae    646cd2f6 <.edata+0x2f6>
     646cd28f:	jae    646cd2fa <.edata+0x2fa>
     646cd291:	insl   (%dx),%es:(%rdi)
     646cd292:	cs fs insb (%dx),%es:(%rdi)
     646cd295:	insb   (%dx),%es:(%rdi)
-    646cd296:	add    %dl,0x61(%rax)
-    646cd299:	jb     646cd30f <.edata+0x30f>
-    646cd29b:	imul   $0x64326e,0x6f(%rcx,%rbp,2),%esi
+    646cd296:	add    %ah,0x72(%rcx)
+    646cd299:	(bad)
+    646cd29a:	outsb  %ds:(%rsi),(%dx)
+    646cd29b:	add    %ah,%gs:0x5f(%ebx)
+    646cd2a0:	(bad)
+    646cd2a1:	jb     646cd315 <.edata+0x315>
     646cd2a3:	(bad)
-    646cd2a4:	jb     646cd307 <.edata+0x307>
-    646cd2a6:	outsb  %ds:(%rsi),(%dx)
-    646cd2a7:	add    %ah,%gs:0x5f(%ebx)
-    646cd2ac:	(bad)
-    646cd2ad:	jb     646cd321 <.edata+0x321>
-    646cd2af:	(bad)
-    646cd2b0:	jns    646cd311 <.edata+0x311>
-    646cd2b2:	insl   (%dx),%es:(%rdi)
+    646cd2a4:	jns    646cd305 <.edata+0x305>
+    646cd2a6:	insl   (%dx),%es:(%rdi)
+    646cd2a7:	(bad)
+    646cd2a8:	js     646cd309 <.edata+0x309>
+    646cd2aa:	outsl  %fs:(%rsi),(%dx)
+    646cd2ac:	jne    646cd310 <.edata+0x310>
+    646cd2ae:	insb   (%dx),%es:(%rdi)
+    646cd2af:	add    %ah,%gs:0x5f(%rbx)
     646cd2b3:	(bad)
-    646cd2b4:	js     646cd315 <.edata+0x315>
-    646cd2b6:	outsl  %fs:(%rsi),(%dx)
-    646cd2b8:	jne    646cd31c <.edata+0x31c>
-    646cd2ba:	insb   (%dx),%es:(%rdi)
-    646cd2bb:	add    %ah,%gs:0x5f(%rbx)
-    646cd2bf:	(bad)
-    646cd2c0:	jb     646cd334 <.edata+0x334>
-    646cd2c2:	(bad)
-    646cd2c3:	jns    646cd324 <.edata+0x324>
-    646cd2c5:	insl   (%dx),%es:(%rdi)
-    646cd2c6:	(bad)
-    646cd2c7:	js     646cd328 <.edata+0x328>
-    646cd2c9:	data16 insb (%dx),%es:(%rdi)
-    646cd2cb:	outsl  %ds:(%rsi),(%dx)
+    646cd2b4:	jb     646cd328 <.edata+0x328>
+    646cd2b6:	(bad)
+    646cd2b7:	jns    646cd318 <.edata+0x318>
+    646cd2b9:	insl   (%dx),%es:(%rdi)
+    646cd2ba:	(bad)
+    646cd2bb:	js     646cd31c <.edata+0x31c>
+    646cd2bd:	data16 insb (%dx),%es:(%rdi)
+    646cd2bf:	outsl  %ds:(%rsi),(%dx)
+    646cd2c0:	(bad)
+    646cd2c1:	je     646cd2c3 <.edata+0x2c3>
+    646cd2c3:	movsxd 0x61(%rdi),%ebx
+    646cd2c6:	jb     646cd33a <.edata+0x33a>
+    646cd2c8:	(bad)
+    646cd2c9:	jns    646cd32a <.edata+0x32a>
+    646cd2cb:	insl   (%dx),%es:(%rdi)
     646cd2cc:	(bad)
-    646cd2cd:	je     646cd2cf <.edata+0x2cf>
-    646cd2cf:	movsxd 0x61(%rdi),%ebx
-    646cd2d2:	jb     646cd346 <.edata+0x346>
-    646cd2d4:	(bad)
-    646cd2d5:	jns    646cd336 <.edata+0x336>
-    646cd2d7:	insl   (%dx),%es:(%rdi)
+    646cd2cd:	js     646cd32e <.edata+0x32e>
+    646cd2cf:	imul   $0x615f6300,0x74(%rsi),%ebp
+    646cd2d6:	jb     646cd34a <.edata+0x34a>
     646cd2d8:	(bad)
-    646cd2d9:	js     646cd33a <.edata+0x33a>
-    646cd2db:	imul   $0x615f6300,0x74(%rsi),%ebp
-    646cd2e2:	jb     646cd356 <.edata+0x356>
-    646cd2e4:	(bad)
-    646cd2e5:	jns    646cd346 <.edata+0x346>
-    646cd2e7:	insl   (%dx),%es:(%rdi)
-    646cd2e8:	(bad)
-    646cd2e9:	js     646cd34a <.edata+0x34a>
-    646cd2eb:	insb   (%dx),%es:(%rdi)
-    646cd2ec:	outsl  %ds:(%rsi),(%dx)
-    646cd2ed:	outsb  %ds:(%rsi),(%dx)
-    646cd2ee:	addr32 pop %rdi
-    646cd2f0:	insb   (%dx),%es:(%rdi)
-    646cd2f1:	outsl  %ds:(%rsi),(%dx)
-    646cd2f2:	outsb  %ds:(%rsi),(%dx)
-    646cd2f3:	add    %ah,0x5f(%ebx)
-    646cd2f7:	(bad)
-    646cd2f8:	jb     646cd36c <.edata+0x36c>
-    646cd2fa:	(bad)
-    646cd2fb:	jns    646cd35c <.edata+0x35c>
-    646cd2fd:	insl   (%dx),%es:(%rdi)
-    646cd2fe:	gs (bad)
-    646cd300:	outsb  %ds:(%rsi),(%dx)
-    646cd301:	pop    %rdi
-    646cd302:	outsl  %fs:(%rsi),(%dx)
-    646cd304:	jne    646cd368 <.edata+0x368>
-    646cd306:	insb   (%dx),%es:(%rdi)
-    646cd307:	add    %ah,%gs:0x5f(%rbx)
-    646cd30b:	(bad)
-    646cd30c:	jb     646cd380 <.edata+0x380>
-    646cd30e:	(bad)
-    646cd30f:	jns    646cd370 <.edata+0x370>
-    646cd311:	insl   (%dx),%es:(%rdi)
-    646cd312:	gs (bad)
-    646cd314:	outsb  %ds:(%rsi),(%dx)
-    646cd315:	pop    %rdi
-    646cd316:	data16 insb (%dx),%es:(%rdi)
-    646cd318:	outsl  %ds:(%rsi),(%dx)
-    646cd319:	(bad)
-    646cd31a:	je     646cd31c <.edata+0x31c>
-    646cd31c:	movsxd 0x61(%rdi),%ebx
-    646cd31f:	jb     646cd393 <.edata+0x393>
-    646cd321:	(bad)
-    646cd322:	jns    646cd383 <.edata+0x383>
-    646cd324:	insl   (%dx),%es:(%rdi)
-    646cd325:	gs (bad)
-    646cd327:	outsb  %ds:(%rsi),(%dx)
-    646cd328:	pop    %rdi
-    646cd329:	imul   $0x615f6300,0x74(%rsi),%ebp
-    646cd330:	jb     646cd3a4 <.edata+0x3a4>
-    646cd332:	(bad)
-    646cd333:	jns    646cd394 <.edata+0x394>
-    646cd335:	insl   (%dx),%es:(%rdi)
-    646cd336:	gs (bad)
-    646cd338:	outsb  %ds:(%rsi),(%dx)
-    646cd339:	pop    %rdi
-    646cd33a:	insb   (%dx),%es:(%rdi)
-    646cd33b:	outsl  %ds:(%rsi),(%dx)
-    646cd33c:	outsb  %ds:(%rsi),(%dx)
-    646cd33d:	addr32 pop %rdi
-    646cd33f:	insb   (%dx),%es:(%rdi)
-    646cd340:	outsl  %ds:(%rsi),(%dx)
-    646cd341:	outsb  %ds:(%rsi),(%dx)
-    646cd342:	add    %ah,0x5f(%ebx)
-    646cd346:	(bad)
-    646cd347:	jb     646cd3bb <.edata+0x3bb>
-    646cd349:	(bad)
-    646cd34a:	jns    646cd3ab <.edata+0x3ab>
-    646cd34c:	insl   (%dx),%es:(%rdi)
-    646cd34d:	imul   $0x62756f64,0x5f(%rsi),%ebp
-    646cd354:	insb   (%dx),%es:(%rdi)
-    646cd355:	add    %ah,%gs:0x5f(%rbx)
-    646cd359:	(bad)
-    646cd35a:	jb     646cd3ce <.edata+0x3ce>
-    646cd35c:	(bad)
-    646cd35d:	jns    646cd3be <.edata+0x3be>
-    646cd35f:	insl   (%dx),%es:(%rdi)
-    646cd360:	imul   $0x616f6c66,0x5f(%rsi),%ebp
-    646cd367:	je     646cd369 <.edata+0x369>
-    646cd369:	movsxd 0x61(%rdi),%ebx
-    646cd36c:	jb     646cd3e0 <.edata+0x3e0>
-    646cd36e:	(bad)
-    646cd36f:	jns    646cd3d0 <.edata+0x3d0>
-    646cd371:	insl   (%dx),%es:(%rdi)
-    646cd372:	imul   $0x746e69,0x5f(%rsi),%ebp
-    646cd379:	movsxd 0x61(%rdi),%ebx
-    646cd37c:	jb     646cd3f0 <.edata+0x3f0>
-    646cd37e:	(bad)
-    646cd37f:	jns    646cd3e0 <.edata+0x3e0>
-    646cd381:	insl   (%dx),%es:(%rdi)
-    646cd382:	imul   $0x676e6f6c,0x5f(%rsi),%ebp
-    646cd389:	pop    %rdi
-    646cd38a:	insb   (%dx),%es:(%rdi)
-    646cd38b:	outsl  %ds:(%rsi),(%dx)
-    646cd38c:	outsb  %ds:(%rsi),(%dx)
-    646cd38d:	add    %ah,0x5f(%ebx)
-    646cd391:	(bad)
-    646cd392:	jb     646cd406 <.edata+0x406>
-    646cd394:	(bad)
-    646cd395:	jns    646cd3f6 <.edata+0x3f6>
-    646cd397:	jae    646cd40d <.edata+0x40d>
-    646cd399:	fs pop %rdi
-    646cd39b:	outsl  %fs:(%rsi),(%dx)
-    646cd39d:	jne    646cd401 <.edata+0x401>
-    646cd39f:	insb   (%dx),%es:(%rdi)
-    646cd3a0:	add    %ah,%gs:0x5f(%rbx)
-    646cd3a4:	(bad)
-    646cd3a5:	jb     646cd419 <.edata+0x419>
-    646cd3a7:	(bad)
-    646cd3a8:	jns    646cd409 <.edata+0x409>
-    646cd3aa:	jae    646cd420 <.edata+0x420>
-    646cd3ac:	fs pop %rdi
-    646cd3ae:	data16 insb (%dx),%es:(%rdi)
-    646cd3b0:	outsl  %ds:(%rsi),(%dx)
-    646cd3b1:	(bad)
-    646cd3b2:	je     646cd3b4 <.edata+0x3b4>
-    646cd3b4:	movsxd 0x61(%rdi),%ebx
-    646cd3b7:	jb     646cd42b <.edata+0x42b>
-    646cd3b9:	(bad)
-    646cd3ba:	jns    646cd41b <.edata+0x41b>
-    646cd3bc:	jae    646cd432 <.edata+0x432>
-    646cd3be:	fs pop %rdi
-    646cd3c0:	imul   $0x615f6300,0x74(%rsi),%ebp
-    646cd3c7:	jb     646cd43b <.edata+0x43b>
-    646cd3c9:	(bad)
-    646cd3ca:	jns    646cd42b <.edata+0x42b>
-    646cd3cc:	jae    646cd442 <.edata+0x442>
-    646cd3ce:	fs pop %rdi
-    646cd3d0:	insb   (%dx),%es:(%rdi)
-    646cd3d1:	outsl  %ds:(%rsi),(%dx)
-    646cd3d2:	outsb  %ds:(%rsi),(%dx)
-    646cd3d3:	addr32 pop %rdi
-    646cd3d5:	insb   (%dx),%es:(%rdi)
-    646cd3d6:	outsl  %ds:(%rsi),(%dx)
-    646cd3d7:	outsb  %ds:(%rsi),(%dx)
-    646cd3d8:	add    %ah,0x5f(%ebx)
-    646cd3dc:	(bad)
-    646cd3dd:	jb     646cd451 <.edata+0x451>
-    646cd3df:	(bad)
-    646cd3e0:	jns    646cd441 <.edata+0x441>
-    646cd3e2:	jae    646cd459 <.edata+0x459>
-    646cd3e4:	insl   (%dx),%es:(%rdi)
-    646cd3e5:	pop    %rdi
-    646cd3e6:	outsl  %fs:(%rsi),(%dx)
-    646cd3e8:	jne    646cd44c <.edata+0x44c>
-    646cd3ea:	insb   (%dx),%es:(%rdi)
-    646cd3eb:	add    %ah,%gs:0x5f(%rbx)
-    646cd3ef:	(bad)
-    646cd3f0:	jb     646cd464 <.edata+0x464>
-    646cd3f2:	(bad)
-    646cd3f3:	jns    646cd454 <.edata+0x454>
-    646cd3f5:	jae    646cd46c <.edata+0x46c>
-    646cd3f7:	insl   (%dx),%es:(%rdi)
-    646cd3f8:	pop    %rdi
-    646cd3f9:	data16 insb (%dx),%es:(%rdi)
-    646cd3fb:	outsl  %ds:(%rsi),(%dx)
-    646cd3fc:	(bad)
-    646cd3fd:	je     646cd3ff <.edata+0x3ff>
-    646cd3ff:	movsxd 0x61(%rdi),%ebx
-    646cd402:	jb     646cd476 <.edata+0x476>
-    646cd404:	(bad)
-    646cd405:	jns    646cd466 <.edata+0x466>
-    646cd407:	jae    646cd47e <.edata+0x47e>
-    646cd409:	insl   (%dx),%es:(%rdi)
-    646cd40a:	pop    %rdi
-    646cd40b:	imul   $0x615f6300,0x74(%rsi),%ebp
-    646cd412:	jb     646cd486 <.edata+0x486>
-    646cd414:	(bad)
-    646cd415:	jns    646cd476 <.edata+0x476>
-    646cd417:	jae    646cd48e <.edata+0x48e>
-    646cd419:	insl   (%dx),%es:(%rdi)
-    646cd41a:	pop    %rdi
-    646cd41b:	insb   (%dx),%es:(%rdi)
-    646cd41c:	outsl  %ds:(%rsi),(%dx)
-    646cd41d:	outsb  %ds:(%rsi),(%dx)
-    646cd41e:	add    %ah,0x5f(%ebx)
-    646cd422:	(bad)
-    646cd423:	jb     646cd497 <.edata+0x497>
-    646cd425:	(bad)
-    646cd426:	jns    646cd487 <.edata+0x487>
-    646cd428:	jbe    646cd48b <.edata+0x48b>
-    646cd42a:	jb     646cd48b <.edata+0x48b>
-    646cd42c:	outsl  %fs:(%rsi),(%dx)
-    646cd42e:	jne    646cd492 <.edata+0x492>
-    646cd430:	insb   (%dx),%es:(%rdi)
-    646cd431:	add    %ah,%gs:0x5f(%rbx)
-    646cd435:	(bad)
-    646cd436:	jb     646cd4aa <.edata+0x4aa>
-    646cd438:	(bad)
-    646cd439:	jns    646cd49a <.edata+0x49a>
-    646cd43b:	jbe    646cd49e <.edata+0x49e>
-    646cd43d:	jb     646cd49e <.edata+0x49e>
-    646cd43f:	data16 insb (%dx),%es:(%rdi)
-    646cd441:	outsl  %ds:(%rsi),(%dx)
-    646cd442:	(bad)
-    646cd443:	je     646cd445 <.edata+0x445>
-    646cd445:	movsxd 0x61(%rdi),%ebx
-    646cd448:	jb     646cd4bc <.edata+0x4bc>
-    646cd44a:	(bad)
-    646cd44b:	jns    646cd4ac <.edata+0x4ac>
-    646cd44d:	jbe    646cd4b0 <.edata+0x4b0>
-    646cd44f:	jb     646cd4b0 <.edata+0x4b0>
-    646cd451:	imul   $0x615f6300,0x74(%rsi),%ebp
-    646cd458:	jb     646cd4cc <.edata+0x4cc>
-    646cd45a:	(bad)
-    646cd45b:	jns    646cd4bc <.edata+0x4bc>
-    646cd45d:	jbe    646cd4c0 <.edata+0x4c0>
-    646cd45f:	jb     646cd4c0 <.edata+0x4c0>
-    646cd461:	insb   (%dx),%es:(%rdi)
-    646cd462:	outsl  %ds:(%rsi),(%dx)
-    646cd463:	outsb  %ds:(%rsi),(%dx)
-    646cd464:	addr32 pop %rdi
-    646cd466:	insb   (%dx),%es:(%rdi)
-    646cd467:	outsl  %ds:(%rsi),(%dx)
-    646cd468:	outsb  %ds:(%rsi),(%dx)
-    646cd469:	add    %ah,0x6d(%ebx)
-    646cd46d:	jo     646cd4d5 <.edata+0x4d5>
-    646cd46f:	jne    646cd4df <.edata+0x4df>
-    646cd471:	movsxd 0x64(%rdi),%ebx
-    646cd474:	outsl  %ds:(%rsi),(%dx)
-    646cd475:	jne    646cd4d9 <.edata+0x4d9>
+    646cd2d9:	jns    646cd33a <.edata+0x33a>
+    646cd2db:	insl   (%dx),%es:(%rdi)
+    646cd2dc:	(bad)
+    646cd2dd:	js     646cd33e <.edata+0x33e>
+    646cd2df:	insb   (%dx),%es:(%rdi)
+    646cd2e0:	outsl  %ds:(%rsi),(%dx)
+    646cd2e1:	outsb  %ds:(%rsi),(%dx)
+    646cd2e2:	addr32 pop %rdi
+    646cd2e4:	insb   (%dx),%es:(%rdi)
+    646cd2e5:	outsl  %ds:(%rsi),(%dx)
+    646cd2e6:	outsb  %ds:(%rsi),(%dx)
+    646cd2e7:	add    %ah,0x5f(%ebx)
+    646cd2eb:	(bad)
+    646cd2ec:	jb     646cd360 <.edata+0x360>
+    646cd2ee:	(bad)
+    646cd2ef:	jns    646cd350 <.edata+0x350>
+    646cd2f1:	insl   (%dx),%es:(%rdi)
+    646cd2f2:	gs (bad)
+    646cd2f4:	outsb  %ds:(%rsi),(%dx)
+    646cd2f5:	pop    %rdi
+    646cd2f6:	outsl  %fs:(%rsi),(%dx)
+    646cd2f8:	jne    646cd35c <.edata+0x35c>
+    646cd2fa:	insb   (%dx),%es:(%rdi)
+    646cd2fb:	add    %ah,%gs:0x5f(%rbx)
+    646cd2ff:	(bad)
+    646cd300:	jb     646cd374 <.edata+0x374>
+    646cd302:	(bad)
+    646cd303:	jns    646cd364 <.edata+0x364>
+    646cd305:	insl   (%dx),%es:(%rdi)
+    646cd306:	gs (bad)
+    646cd308:	outsb  %ds:(%rsi),(%dx)
+    646cd309:	pop    %rdi
+    646cd30a:	data16 insb (%dx),%es:(%rdi)
+    646cd30c:	outsl  %ds:(%rsi),(%dx)
+    646cd30d:	(bad)
+    646cd30e:	je     646cd310 <.edata+0x310>
+    646cd310:	movsxd 0x61(%rdi),%ebx
+    646cd313:	jb     646cd387 <.edata+0x387>
+    646cd315:	(bad)
+    646cd316:	jns    646cd377 <.edata+0x377>
+    646cd318:	insl   (%dx),%es:(%rdi)
+    646cd319:	gs (bad)
+    646cd31b:	outsb  %ds:(%rsi),(%dx)
+    646cd31c:	pop    %rdi
+    646cd31d:	imul   $0x615f6300,0x74(%rsi),%ebp
+    646cd324:	jb     646cd398 <.edata+0x398>
+    646cd326:	(bad)
+    646cd327:	jns    646cd388 <.edata+0x388>
+    646cd329:	insl   (%dx),%es:(%rdi)
+    646cd32a:	gs (bad)
+    646cd32c:	outsb  %ds:(%rsi),(%dx)
+    646cd32d:	pop    %rdi
+    646cd32e:	insb   (%dx),%es:(%rdi)
+    646cd32f:	outsl  %ds:(%rsi),(%dx)
+    646cd330:	outsb  %ds:(%rsi),(%dx)
+    646cd331:	addr32 pop %rdi
+    646cd333:	insb   (%dx),%es:(%rdi)
+    646cd334:	outsl  %ds:(%rsi),(%dx)
+    646cd335:	outsb  %ds:(%rsi),(%dx)
+    646cd336:	add    %ah,0x5f(%ebx)
+    646cd33a:	(bad)
+    646cd33b:	jb     646cd3af <.edata+0x3af>
+    646cd33d:	(bad)
+    646cd33e:	jns    646cd39f <.edata+0x39f>
+    646cd340:	insl   (%dx),%es:(%rdi)
+    646cd341:	imul   $0x62756f64,0x5f(%rsi),%ebp
+    646cd348:	insb   (%dx),%es:(%rdi)
+    646cd349:	add    %ah,%gs:0x5f(%rbx)
+    646cd34d:	(bad)
+    646cd34e:	jb     646cd3c2 <.edata+0x3c2>
+    646cd350:	(bad)
+    646cd351:	jns    646cd3b2 <.edata+0x3b2>
+    646cd353:	insl   (%dx),%es:(%rdi)
+    646cd354:	imul   $0x616f6c66,0x5f(%rsi),%ebp
+    646cd35b:	je     646cd35d <.edata+0x35d>
+    646cd35d:	movsxd 0x61(%rdi),%ebx
+    646cd360:	jb     646cd3d4 <.edata+0x3d4>
+    646cd362:	(bad)
+    646cd363:	jns    646cd3c4 <.edata+0x3c4>
+    646cd365:	insl   (%dx),%es:(%rdi)
+    646cd366:	imul   $0x746e69,0x5f(%rsi),%ebp
+    646cd36d:	movsxd 0x61(%rdi),%ebx
+    646cd370:	jb     646cd3e4 <.edata+0x3e4>
+    646cd372:	(bad)
+    646cd373:	jns    646cd3d4 <.edata+0x3d4>
+    646cd375:	insl   (%dx),%es:(%rdi)
+    646cd376:	imul   $0x676e6f6c,0x5f(%rsi),%ebp
+    646cd37d:	pop    %rdi
+    646cd37e:	insb   (%dx),%es:(%rdi)
+    646cd37f:	outsl  %ds:(%rsi),(%dx)
+    646cd380:	outsb  %ds:(%rsi),(%dx)
+    646cd381:	add    %ah,0x5f(%ebx)
+    646cd385:	(bad)
+    646cd386:	jb     646cd3fa <.edata+0x3fa>
+    646cd388:	(bad)
+    646cd389:	jns    646cd3ea <.edata+0x3ea>
+    646cd38b:	jae    646cd401 <.edata+0x401>
+    646cd38d:	fs pop %rdi
+    646cd38f:	outsl  %fs:(%rsi),(%dx)
+    646cd391:	jne    646cd3f5 <.edata+0x3f5>
+    646cd393:	insb   (%dx),%es:(%rdi)
+    646cd394:	add    %ah,%gs:0x5f(%rbx)
+    646cd398:	(bad)
+    646cd399:	jb     646cd40d <.edata+0x40d>
+    646cd39b:	(bad)
+    646cd39c:	jns    646cd3fd <.edata+0x3fd>
+    646cd39e:	jae    646cd414 <.edata+0x414>
+    646cd3a0:	fs pop %rdi
+    646cd3a2:	data16 insb (%dx),%es:(%rdi)
+    646cd3a4:	outsl  %ds:(%rsi),(%dx)
+    646cd3a5:	(bad)
+    646cd3a6:	je     646cd3a8 <.edata+0x3a8>
+    646cd3a8:	movsxd 0x61(%rdi),%ebx
+    646cd3ab:	jb     646cd41f <.edata+0x41f>
+    646cd3ad:	(bad)
+    646cd3ae:	jns    646cd40f <.edata+0x40f>
+    646cd3b0:	jae    646cd426 <.edata+0x426>
+    646cd3b2:	fs pop %rdi
+    646cd3b4:	imul   $0x615f6300,0x74(%rsi),%ebp
+    646cd3bb:	jb     646cd42f <.edata+0x42f>
+    646cd3bd:	(bad)
+    646cd3be:	jns    646cd41f <.edata+0x41f>
+    646cd3c0:	jae    646cd436 <.edata+0x436>
+    646cd3c2:	fs pop %rdi
+    646cd3c4:	insb   (%dx),%es:(%rdi)
+    646cd3c5:	outsl  %ds:(%rsi),(%dx)
+    646cd3c6:	outsb  %ds:(%rsi),(%dx)
+    646cd3c7:	addr32 pop %rdi
+    646cd3c9:	insb   (%dx),%es:(%rdi)
+    646cd3ca:	outsl  %ds:(%rsi),(%dx)
+    646cd3cb:	outsb  %ds:(%rsi),(%dx)
+    646cd3cc:	add    %ah,0x5f(%ebx)
+    646cd3d0:	(bad)
+    646cd3d1:	jb     646cd445 <.edata+0x445>
+    646cd3d3:	(bad)
+    646cd3d4:	jns    646cd435 <.edata+0x435>
+    646cd3d6:	jae    646cd44d <.edata+0x44d>
+    646cd3d8:	insl   (%dx),%es:(%rdi)
+    646cd3d9:	pop    %rdi
+    646cd3da:	outsl  %fs:(%rsi),(%dx)
+    646cd3dc:	jne    646cd440 <.edata+0x440>
+    646cd3de:	insb   (%dx),%es:(%rdi)
+    646cd3df:	add    %ah,%gs:0x5f(%rbx)
+    646cd3e3:	(bad)
+    646cd3e4:	jb     646cd458 <.edata+0x458>
+    646cd3e6:	(bad)
+    646cd3e7:	jns    646cd448 <.edata+0x448>
+    646cd3e9:	jae    646cd460 <.edata+0x460>
+    646cd3eb:	insl   (%dx),%es:(%rdi)
+    646cd3ec:	pop    %rdi
+    646cd3ed:	data16 insb (%dx),%es:(%rdi)
+    646cd3ef:	outsl  %ds:(%rsi),(%dx)
+    646cd3f0:	(bad)
+    646cd3f1:	je     646cd3f3 <.edata+0x3f3>
+    646cd3f3:	movsxd 0x61(%rdi),%ebx
+    646cd3f6:	jb     646cd46a <.edata+0x46a>
+    646cd3f8:	(bad)
+    646cd3f9:	jns    646cd45a <.edata+0x45a>
+    646cd3fb:	jae    646cd472 <.edata+0x472>
+    646cd3fd:	insl   (%dx),%es:(%rdi)
+    646cd3fe:	pop    %rdi
+    646cd3ff:	imul   $0x615f6300,0x74(%rsi),%ebp
+    646cd406:	jb     646cd47a <.edata+0x47a>
+    646cd408:	(bad)
+    646cd409:	jns    646cd46a <.edata+0x46a>
+    646cd40b:	jae    646cd482 <.edata+0x482>
+    646cd40d:	insl   (%dx),%es:(%rdi)
+    646cd40e:	pop    %rdi
+    646cd40f:	insb   (%dx),%es:(%rdi)
+    646cd410:	outsl  %ds:(%rsi),(%dx)
+    646cd411:	outsb  %ds:(%rsi),(%dx)
+    646cd412:	add    %ah,0x5f(%ebx)
+    646cd416:	(bad)
+    646cd417:	jb     646cd48b <.edata+0x48b>
+    646cd419:	(bad)
+    646cd41a:	jns    646cd47b <.edata+0x47b>
+    646cd41c:	jbe    646cd47f <.edata+0x47f>
+    646cd41e:	jb     646cd47f <.edata+0x47f>
+    646cd420:	outsl  %fs:(%rsi),(%dx)
+    646cd422:	jne    646cd486 <.edata+0x486>
+    646cd424:	insb   (%dx),%es:(%rdi)
+    646cd425:	add    %ah,%gs:0x5f(%rbx)
+    646cd429:	(bad)
+    646cd42a:	jb     646cd49e <.edata+0x49e>
+    646cd42c:	(bad)
+    646cd42d:	jns    646cd48e <.edata+0x48e>
+    646cd42f:	jbe    646cd492 <.edata+0x492>
+    646cd431:	jb     646cd492 <.edata+0x492>
+    646cd433:	data16 insb (%dx),%es:(%rdi)
+    646cd435:	outsl  %ds:(%rsi),(%dx)
+    646cd436:	(bad)
+    646cd437:	je     646cd439 <.edata+0x439>
+    646cd439:	movsxd 0x61(%rdi),%ebx
+    646cd43c:	jb     646cd4b0 <.edata+0x4b0>
+    646cd43e:	(bad)
+    646cd43f:	jns    646cd4a0 <.edata+0x4a0>
+    646cd441:	jbe    646cd4a4 <.edata+0x4a4>
+    646cd443:	jb     646cd4a4 <.edata+0x4a4>
+    646cd445:	imul   $0x615f6300,0x74(%rsi),%ebp
+    646cd44c:	jb     646cd4c0 <.edata+0x4c0>
+    646cd44e:	(bad)
+    646cd44f:	jns    646cd4b0 <.edata+0x4b0>
+    646cd451:	jbe    646cd4b4 <.edata+0x4b4>
+    646cd453:	jb     646cd4b4 <.edata+0x4b4>
+    646cd455:	insb   (%dx),%es:(%rdi)
+    646cd456:	outsl  %ds:(%rsi),(%dx)
+    646cd457:	outsb  %ds:(%rsi),(%dx)
+    646cd458:	addr32 pop %rdi
+    646cd45a:	insb   (%dx),%es:(%rdi)
+    646cd45b:	outsl  %ds:(%rsi),(%dx)
+    646cd45c:	outsb  %ds:(%rsi),(%dx)
+    646cd45d:	add    %ah,0x6d(%ebx)
+    646cd461:	jo     646cd4c9 <.edata+0x4c9>
+    646cd463:	jne    646cd4d3 <.edata+0x4d3>
+    646cd465:	movsxd 0x64(%rdi),%ebx
+    646cd468:	outsl  %ds:(%rsi),(%dx)
+    646cd469:	jne    646cd4cd <.edata+0x4cd>
+    646cd46b:	insb   (%dx),%es:(%rdi)
+    646cd46c:	add    %ah,%gs:0x6d(%rbx)
+    646cd470:	jo     646cd4d8 <.edata+0x4d8>
+    646cd472:	jne    646cd4e2 <.edata+0x4e2>
+    646cd474:	movsxd 0x66(%rdi),%ebx
     646cd477:	insb   (%dx),%es:(%rdi)
-    646cd478:	add    %ah,%gs:0x6d(%rbx)
-    646cd47c:	jo     646cd4e4 <.edata+0x4e4>
-    646cd47e:	jne    646cd4ee <.edata+0x4ee>
-    646cd480:	movsxd 0x66(%rdi),%ebx
-    646cd483:	insb   (%dx),%es:(%rdi)
-    646cd484:	outsl  %ds:(%rsi),(%dx)
-    646cd485:	(bad)
+    646cd478:	outsl  %ds:(%rsi),(%dx)
+    646cd479:	(bad)
+    646cd47a:	je     646cd47c <.edata+0x47c>
+    646cd47c:	movsxd 0x70(%rbp),%ebp
+    646cd47f:	data16 jne 646cd4f0 <.edata+0x4f0>
+    646cd482:	movsxd 0x69(%rdi),%ebx
+    646cd485:	outsb  %ds:(%rsi),(%dx)
     646cd486:	je     646cd488 <.edata+0x488>
     646cd488:	movsxd 0x70(%rbp),%ebp
     646cd48b:	data16 jne 646cd4fc <.edata+0x4fc>
-    646cd48e:	movsxd 0x69(%rdi),%ebx
-    646cd491:	outsb  %ds:(%rsi),(%dx)
-    646cd492:	je     646cd494 <.edata+0x494>
-    646cd494:	movsxd 0x70(%rbp),%ebp
-    646cd497:	data16 jne 646cd508 <.edata+0x508>
-    646cd49a:	movsxd 0x6c(%rdi),%ebx
-    646cd49d:	outsl  %ds:(%rsi),(%dx)
-    646cd49e:	outsb  %ds:(%rsi),(%dx)
-    646cd49f:	add    %ah,0x6f(%ebx)
-    646cd4a3:	jbe    646cd504 <.edata+0x504>
-    646cd4a5:	insl   (%dx),%es:(%rdi)
-    646cd4a6:	outsl  %ds:(%rsi),(%dx)
-    646cd4a7:	fs gs insb (%dx),%es:(%rdi)
-    646cd4aa:	add    %ah,0x6f(%rbx)
+    646cd48e:	movsxd 0x6c(%rdi),%ebx
+    646cd491:	outsl  %ds:(%rsi),(%dx)
+    646cd492:	outsb  %ds:(%rsi),(%dx)
+    646cd493:	add    %ah,0x6f(%ebx)
+    646cd497:	jbe    646cd4f8 <.edata+0x4f8>
+    646cd499:	insl   (%dx),%es:(%rdi)
+    646cd49a:	outsl  %ds:(%rsi),(%dx)
+    646cd49b:	fs gs insb (%dx),%es:(%rdi)
+    646cd49e:	add    %ah,0x6f(%rbx)
+    646cd4a1:	jbe    646cd502 <.edata+0x502>
+    646cd4a3:	insl   (%dx),%es:(%rdi)
+    646cd4a4:	outsl  %ds:(%rsi),(%dx)
+    646cd4a5:	fs gs insb (%dx),%es:(%rdi)
+    646cd4a8:	xor    0x63(%rax,%rax,1),%ah
+    646cd4ac:	outsl  %ds:(%rsi),(%dx)
     646cd4ad:	jbe    646cd50e <.edata+0x50e>
     646cd4af:	insl   (%dx),%es:(%rdi)
     646cd4b0:	outsl  %ds:(%rsi),(%dx)
     646cd4b1:	fs gs insb (%dx),%es:(%rdi)
-    646cd4b4:	xor    0x63(%rax,%rax,1),%ah
-    646cd4b8:	outsl  %ds:(%rsi),(%dx)
-    646cd4b9:	jbe    646cd51a <.edata+0x51a>
-    646cd4bb:	insl   (%dx),%es:(%rdi)
-    646cd4bc:	outsl  %ds:(%rsi),(%dx)
-    646cd4bd:	fs gs insb (%dx),%es:(%rdi)
-    646cd4c0:	pop    %rdi
-    646cd4c1:	imul   $0x5f640074,0x69(%rsi),%ebp
-    646cd4c8:	(bad)
-    646cd4c9:	jb     646cd52c <.edata+0x52c>
-    646cd4cb:	outsb  %ds:(%rsi),(%dx)
-    646cd4cc:	add    %ah,%gs:0x69(%esi)
-    646cd4d1:	outsb  %ds:(%rsi),(%dx)
-    646cd4d2:	fs pop %rdi
-    646cd4d4:	outsb  %ds:(%rsi),(%dx)
-    646cd4d5:	imul   $0x726f62,%gs:0x68(%rdi),%esp
-    646cd4dd:	imul   $0x67,0x69(%rdx),%esi
-    646cd4e1:	gs pop %rdi
-    646cd4e3:	insl   (%dx),%es:(%rdi)
-    646cd4e4:	gs insl (%dx),%es:(%rdi)
-    646cd4e6:	outsl  %ds:(%rsi),(%dx)
-    646cd4e7:	jb     646cd562 <.edata+0x562>
-    646cd4e9:	pop    %rdi
-    646cd4ea:	data16 jb 646cd552 <.edata+0x552>
-    646cd4ed:	add    %ch,%gs:0x72(%rbx)
-    646cd4f1:	imul   $0x7261705f,0x65(%rdi),%esp
-    646cd4f8:	(bad)
-    646cd4f9:	insl   (%dx),%es:(%rdi)
-    646cd4fa:	pop    %rdi
-    646cd4fb:	jae    646cd562 <.edata+0x562>
-    646cd4fd:	je     646cd573 <.edata+0x573>
-    646cd4ff:	imul   $0x5f756c00,0x67(%rsi),%ebp
-    646cd506:	fs movsxd %gs:0x6d(%rdi),%ebp
-    646cd50b:	jo     646cd57c <.edata+0x57c>
-    646cd50d:	jae    646cd578 <.edata+0x578>
-    646cd50f:	je     646cd57a <.edata+0x57a>
-    646cd511:	outsl  %ds:(%rsi),(%dx)
-    646cd512:	outsb  %ds:(%rsi),(%dx)
-    646cd513:	add    %ch,0x5f(%rbp,%rsi,2)
-    646cd517:	imul   $0x65737265,0x76(%rsi),%ebp
-    646cd51e:	pop    %rdi
-    646cd51f:	jae    646cd590 <.edata+0x590>
-    646cd521:	insb   (%dx),%es:(%rdi)
-    646cd522:	jbe    646cd589 <.edata+0x589>
-    646cd524:	jb     646cd526 <.edata+0x526>
-    646cd526:	insl   (%dx),%es:(%rdi)
-    646cd527:	(bad)
-    646cd528:	je     646cd59c <.edata+0x59c>
-    646cd52a:	imul   $0x6d726f,0x66(%rax),%edi
-    646cd531:	insl   (%dx),%es:(%rdi)
-    646cd532:	je     646cd565 <.edata+0x565>
-    646cd534:	cmp    %edi,(%rcx)
-    646cd536:	xor    (%rdi),%esi
-    646cd538:	pop    %rdi
-    646cd539:	outsb  %gs:(%esi),(%dx)
-    646cd53c:	gs jb  646cd5a0 <.edata+0x5a0>
-    646cd53f:	je     646cd5a6 <.edata+0x5a6>
-    646cd541:	add    %ch,0x74(%rbp)
-    646cd544:	xor    %edi,(%rcx)
-    646cd546:	cmp    %esi,(%rbx)
-    646cd548:	(bad)
-    646cd549:	pop    %rdi
-    646cd54a:	addr32 gs je 646cd5ad <.edata+0x5ad>
-    646cd54e:	outsl  %fs:(%rsi),(%dx)
-    646cd550:	jne    646cd5b4 <.edata+0x5b4>
-    646cd552:	insb   (%dx),%es:(%rdi)
-    646cd553:	add    %ch,%gs:0x74(%rbp)
-    646cd557:	xor    %edi,(%rcx)
-    646cd559:	cmp    %esi,(%rbx)
-    646cd55b:	(bad)
-    646cd55c:	pop    %rdi
-    646cd55d:	addr32 gs je 646cd5c0 <.edata+0x5c0>
-    646cd561:	outsl  %fs:(%rsi),(%dx)
-    646cd563:	jne    646cd5c7 <.edata+0x5c7>
-    646cd565:	insb   (%dx),%es:(%rdi)
-    646cd566:	gs pop %rdi
-    646cd568:	jb     646cd5cb <.edata+0x5cb>
-    646cd56a:	outsb  %ds:(%rsi),(%dx)
-    646cd56b:	add    %ch,%gs:0x74(%ebp)
-    646cd570:	xor    %edi,(%rcx)
-    646cd572:	cmp    %esi,(%rbx)
-    646cd574:	(bad)
-    646cd575:	pop    %rdi
-    646cd576:	addr32 gs je 646cd5d9 <.edata+0x5d9>
-    646cd57a:	data16 insb (%dx),%es:(%rdi)
-    646cd57c:	outsl  %ds:(%rsi),(%dx)
-    646cd57d:	(bad)
-    646cd57e:	je     646cd580 <.edata+0x580>
-    646cd580:	insl   (%dx),%es:(%rdi)
-    646cd581:	je     646cd5b4 <.edata+0x5b4>
-    646cd583:	cmp    %edi,(%rcx)
-    646cd585:	xor    (%rdi),%esi
-    646cd587:	pop    %rdi
-    646cd588:	addr32 gs je 646cd5eb <.edata+0x5eb>
-    646cd58c:	data16 insb (%dx),%es:(%rdi)
-    646cd58e:	outsl  %ds:(%rsi),(%dx)
-    646cd58f:	(bad)
-    646cd590:	je     646cd5f1 <.edata+0x5f1>
-    646cd592:	jb     646cd5f5 <.edata+0x5f5>
-    646cd594:	outsb  %ds:(%rsi),(%dx)
-    646cd595:	add    %ch,%gs:0x74(%ebp)
-    646cd59a:	xor    %edi,(%rcx)
-    646cd59c:	cmp    %esi,(%rbx)
-    646cd59e:	(bad)
-    646cd59f:	pop    %rdi
-    646cd5a0:	addr32 gs je 646cd603 <.edata+0x603>
-    646cd5a4:	imul   $0x725f3233,0x74(%rsi),%ebp
-    646cd5ab:	(bad)
-    646cd5ac:	outsb  %ds:(%rsi),(%dx)
-    646cd5ad:	add    %ch,%gs:0x74(%ebp)
-    646cd5b2:	xor    %edi,(%rcx)
-    646cd5b4:	cmp    %esi,(%rbx)
-    646cd5b6:	(bad)
-    646cd5b7:	pop    %rdi
-    646cd5b8:	imul   $0x746d0074,0x69(%rsi),%ebp
-    646cd5bf:	xor    %edi,(%rcx)
-    646cd5c1:	cmp    %esi,(%rbx)
-    646cd5c3:	(bad)
-    646cd5c4:	pop    %rdi
-    646cd5c5:	jb     646cd628 <.edata+0x628>
-    646cd5c7:	outsb  %ds:(%rsi),(%dx)
-    646cd5c8:	outsl  %fs:(%rsi),(%dx)
-    646cd5ca:	insl   (%dx),%es:(%rdi)
-    646cd5cb:	pop    %rdi
-    646cd5cc:	outsb  %ds:(%rsi),(%dx)
-    646cd5cd:	outsl  %ds:(%rsi),(%dx)
-    646cd5ce:	jb     646cd63d <.edata+0x63d>
-    646cd5d0:	(bad)
-    646cd5d1:	insb   (%dx),%es:(%rdi)
-    646cd5d2:	add    %dh,0x64(%rax)
+    646cd4b4:	pop    %rdi
+    646cd4b5:	imul   $0x5f640074,0x69(%rsi),%ebp
+    646cd4bc:	(bad)
+    646cd4bd:	jb     646cd520 <.edata+0x520>
+    646cd4bf:	outsb  %ds:(%rsi),(%dx)
+    646cd4c0:	add    %ah,%gs:0x69(%esi)
+    646cd4c5:	outsb  %ds:(%rsi),(%dx)
+    646cd4c6:	fs pop %rdi
+    646cd4c8:	outsb  %ds:(%rsi),(%dx)
+    646cd4c9:	imul   $0x726f62,%gs:0x68(%rdi),%esp
+    646cd4d1:	imul   $0x67,0x69(%rdx),%esi
+    646cd4d5:	gs pop %rdi
+    646cd4d7:	insl   (%dx),%es:(%rdi)
+    646cd4d8:	gs insl (%dx),%es:(%rdi)
+    646cd4da:	outsl  %ds:(%rsi),(%dx)
+    646cd4db:	jb     646cd556 <.edata+0x556>
+    646cd4dd:	pop    %rdi
+    646cd4de:	data16 jb 646cd546 <.edata+0x546>
+    646cd4e1:	add    %ch,%gs:0x72(%rbx)
+    646cd4e5:	imul   $0x7261705f,0x65(%rdi),%esp
+    646cd4ec:	(bad)
+    646cd4ed:	insl   (%dx),%es:(%rdi)
+    646cd4ee:	pop    %rdi
+    646cd4ef:	jae    646cd556 <.edata+0x556>
+    646cd4f1:	je     646cd567 <.edata+0x567>
+    646cd4f3:	imul   $0x5f756c00,0x67(%rsi),%ebp
+    646cd4fa:	fs movsxd %gs:0x6d(%rdi),%ebp
+    646cd4ff:	jo     646cd570 <.edata+0x570>
+    646cd501:	jae    646cd56c <.edata+0x56c>
+    646cd503:	je     646cd56e <.edata+0x56e>
+    646cd505:	outsl  %ds:(%rsi),(%dx)
+    646cd506:	outsb  %ds:(%rsi),(%dx)
+    646cd507:	add    %ch,0x5f(%rbp,%rsi,2)
+    646cd50b:	imul   $0x65737265,0x76(%rsi),%ebp
+    646cd512:	pop    %rdi
+    646cd513:	jae    646cd584 <.edata+0x584>
+    646cd515:	insb   (%dx),%es:(%rdi)
+    646cd516:	jbe    646cd57d <.edata+0x57d>
+    646cd518:	jb     646cd51a <.edata+0x51a>
+    646cd51a:	insl   (%dx),%es:(%rdi)
+    646cd51b:	(bad)
+    646cd51c:	je     646cd590 <.edata+0x590>
+    646cd51e:	imul   $0x6d726f,0x66(%rax),%edi
+    646cd525:	insl   (%dx),%es:(%rdi)
+    646cd526:	je     646cd559 <.edata+0x559>
+    646cd528:	cmp    %edi,(%rcx)
+    646cd52a:	xor    (%rdi),%esi
+    646cd52c:	pop    %rdi
+    646cd52d:	outsb  %gs:(%esi),(%dx)
+    646cd530:	gs jb  646cd594 <.edata+0x594>
+    646cd533:	je     646cd59a <.edata+0x59a>
+    646cd535:	add    %ch,0x74(%rbp)
+    646cd538:	xor    %edi,(%rcx)
+    646cd53a:	cmp    %esi,(%rbx)
+    646cd53c:	(bad)
+    646cd53d:	pop    %rdi
+    646cd53e:	addr32 gs je 646cd5a1 <.edata+0x5a1>
+    646cd542:	outsl  %fs:(%rsi),(%dx)
+    646cd544:	jne    646cd5a8 <.edata+0x5a8>
+    646cd546:	insb   (%dx),%es:(%rdi)
+    646cd547:	add    %ch,%gs:0x74(%rbp)
+    646cd54b:	xor    %edi,(%rcx)
+    646cd54d:	cmp    %esi,(%rbx)
+    646cd54f:	(bad)
+    646cd550:	pop    %rdi
+    646cd551:	addr32 gs je 646cd5b4 <.edata+0x5b4>
+    646cd555:	outsl  %fs:(%rsi),(%dx)
+    646cd557:	jne    646cd5bb <.edata+0x5bb>
+    646cd559:	insb   (%dx),%es:(%rdi)
+    646cd55a:	gs pop %rdi
+    646cd55c:	jb     646cd5bf <.edata+0x5bf>
+    646cd55e:	outsb  %ds:(%rsi),(%dx)
+    646cd55f:	add    %ch,%gs:0x74(%ebp)
+    646cd564:	xor    %edi,(%rcx)
+    646cd566:	cmp    %esi,(%rbx)
+    646cd568:	(bad)
+    646cd569:	pop    %rdi
+    646cd56a:	addr32 gs je 646cd5cd <.edata+0x5cd>
+    646cd56e:	data16 insb (%dx),%es:(%rdi)
+    646cd570:	outsl  %ds:(%rsi),(%dx)
+    646cd571:	(bad)
+    646cd572:	je     646cd574 <.edata+0x574>
+    646cd574:	insl   (%dx),%es:(%rdi)
+    646cd575:	je     646cd5a8 <.edata+0x5a8>
+    646cd577:	cmp    %edi,(%rcx)
+    646cd579:	xor    (%rdi),%esi
+    646cd57b:	pop    %rdi
+    646cd57c:	addr32 gs je 646cd5df <.edata+0x5df>
+    646cd580:	data16 insb (%dx),%es:(%rdi)
+    646cd582:	outsl  %ds:(%rsi),(%dx)
+    646cd583:	(bad)
+    646cd584:	je     646cd5e5 <.edata+0x5e5>
+    646cd586:	jb     646cd5e9 <.edata+0x5e9>
+    646cd588:	outsb  %ds:(%rsi),(%dx)
+    646cd589:	add    %ch,%gs:0x74(%ebp)
+    646cd58e:	xor    %edi,(%rcx)
+    646cd590:	cmp    %esi,(%rbx)
+    646cd592:	(bad)
+    646cd593:	pop    %rdi
+    646cd594:	addr32 gs je 646cd5f7 <.edata+0x5f7>
+    646cd598:	imul   $0x725f3233,0x74(%rsi),%ebp
+    646cd59f:	(bad)
+    646cd5a0:	outsb  %ds:(%rsi),(%dx)
+    646cd5a1:	add    %ch,%gs:0x74(%ebp)
+    646cd5a6:	xor    %edi,(%rcx)
+    646cd5a8:	cmp    %esi,(%rbx)
+    646cd5aa:	(bad)
+    646cd5ab:	pop    %rdi
+    646cd5ac:	imul   $0x746d0074,0x69(%rsi),%ebp
+    646cd5b3:	xor    %edi,(%rcx)
+    646cd5b5:	cmp    %esi,(%rbx)
+    646cd5b7:	(bad)
+    646cd5b8:	pop    %rdi
+    646cd5b9:	jb     646cd61c <.edata+0x61c>
+    646cd5bb:	outsb  %ds:(%rsi),(%dx)
+    646cd5bc:	outsl  %fs:(%rsi),(%dx)
+    646cd5be:	insl   (%dx),%es:(%rdi)
+    646cd5bf:	pop    %rdi
+    646cd5c0:	outsb  %ds:(%rsi),(%dx)
+    646cd5c1:	outsl  %ds:(%rsi),(%dx)
+    646cd5c2:	jb     646cd631 <.edata+0x631>
+    646cd5c4:	(bad)
+    646cd5c5:	insb   (%dx),%es:(%rdi)
+    646cd5c6:	add    %dh,0x61(%rax)
+    646cd5c9:	jb     646cd63f <.edata+0x63f>
+    646cd5cb:	imul   $0x64326e,0x6f(%rcx,%rbp,2),%esi
+    646cd5d3:	jo     646cd639 <.edata+0x639>
     646cd5d5:	imul   $0x69757100,0x74(%rbx),%esi
     646cd5dc:	movsxd 0x73(%rbx),%ebp
     646cd5df:	outsl  %ds:(%rsi),(%dx)
     646cd5e0:	jb     646cd656 <.edata+0x656>
     646cd5e2:	xor    0x72(%rax,%rax,1),%ah
     646cd5e6:	(bad)
     646cd5e7:	outsb  %ds:(%rsi),(%dx)
@@ -13837,25 +13653,27 @@
     646cd644:	data16 jb 646cd6ac <__bss_end__+0xb1c>
     646cd647:	add    %dh,%gs:0x69(%rbx)
     646cd64b:	insl   (%dx),%es:(%rdi)
     646cd64c:	jo     646cd6ba <__bss_end__+0xb2a>
     646cd64e:	gs pop %rdi
     646cd650:	imul   $0x67,0x69(%rdx),%esi
     646cd654:	imul   $0x61777300,0x67(%rsi),%ebp
-    646cd65b:	jo     646cd65d <.edata+0x65d>
-    646cd65d:	jbe    646cd6c0 <__bss_end__+0xb30>
-    646cd65f:	jb     646cd6ca <__bss_end__+0xb3a>
-    646cd661:	(bad)
-    646cd662:	outsb  %ds:(%rsi),(%dx)
-    646cd663:	movsxd 0x0(%rbp),%esp
-    646cd666:	jbe    646cd6c9 <__bss_end__+0xb39>
-    646cd668:	jb     646cd6d3 <__bss_end__+0xb43>
-    646cd66a:	outsl  %ds:(%rsi),(%dx)
-    646cd66b:	addr32 jb 646cd6cf <__bss_end__+0xb3f>
-    646cd66e:	insl   (%dx),%es:(%rdi)
+    646cd65b:	jo     646cd6cf <__bss_end__+0xb3f>
+    646cd65d:	outsl  %ds:(%rsi),(%dx)
+    646cd65e:	ja     646cd6d3 <__bss_end__+0xb43>
+    646cd660:	add    %dh,0x61(%rsi)
+    646cd663:	jb     646cd6ce <__bss_end__+0xb3e>
+    646cd665:	(bad)
+    646cd666:	outsb  %ds:(%rsi),(%dx)
+    646cd667:	movsxd 0x0(%rbp),%esp
+    646cd66a:	jbe    646cd6cd <__bss_end__+0xb3d>
+    646cd66c:	jb     646cd6d7 <__bss_end__+0xb47>
+    646cd66e:	outsl  %ds:(%rsi),(%dx)
+    646cd66f:	addr32 jb 646cd6d3 <__bss_end__+0xb43>
+    646cd672:	insl   (%dx),%es:(%rdi)
 	...
 
 Disassembly of section .idata:
 
 00000000646ce000 <_head_lib64_libkernel32_a>:
     646ce000:	cmp    $0xe0,%al
 	...
@@ -15138,21 +14956,23 @@
 00000000646cf020 <__xi_z>:
 	...
 
 00000000646cf028 <___crt_xi_end__>:
 	...
 
 00000000646cf030 <__xl_c>:
-    646cf030:	adcb   $0x64,0x6c(%rdi)
-    646cf034:	add    %al,(%rax)
+    646cf030:	nop
+    646cf031:	push   %rsp
+    646cf032:	insb   (%dx),%es:(%rdi)
+    646cf033:	add    %al,%fs:(%rax)
 	...
 
 00000000646cf038 <__xl_d>:
-    646cf038:	push   %rax
-    646cf039:	push   %rdi
+    646cf038:	(bad)
+    646cf039:	push   %rsp
     646cf03a:	insb   (%dx),%es:(%rdi)
     646cf03b:	add    %al,%fs:(%rax)
 	...
 
 00000000646cf040 <__xl_z>:
 	...
 
@@ -15172,36 +14992,36 @@
 
 Disassembly of section .reloc:
 
 00000000646d1000 <.reloc>:
     646d1000:	add    %dh,0x0(%rax)
     646d1003:	add    %cl,(%rax,%rax,1)
     646d1006:	add    %al,(%rax)
-    646d1008:	rex.W scas %es:(%rdi),%al
+    646d1008:	pop    %rax
+    646d1009:	stos   %eax,%es:(%rdi)
     646d100a:	add    %al,(%rax)
     646d100c:	add    %al,0x140000(%rax)
     646d1012:	add    %al,(%rax)
     646d1014:	add    %ah,-0x5fa75fb0(%rax)
     646d101a:	(bad)
     646d101b:	movabs 0x90000000a070,%al
     646d1024:	xor    $0x0,%al
     646d1026:	add    %al,(%rax)
-    646d1028:	andb   $0xc0,-0x5e5f5e78(%rcx)
-    646d102f:	movabs 0xa5e0a1d8a1d0a1c8,%eax
-    646d1038:	lock movsl %ds:(%rsi),%es:(%rdi)
-    646d103a:	add    %ah,-0x59df59f0(%rsi)
-    646d1040:	xor    %ah,-0x59af59c0(%rsi)
-    646d1046:	(bad)
-    646d1047:	cmpsb  %es:(%rdi),%ds:(%rsi)
-    646d1048:	jo     646d0ff0 <___tls_end__+0xfe0>
-    646d104a:	andb   $0xb0,-0x595f5970(%rsi)
-    646d1051:	cmpsb  %es:(%rdi),%ds:(%rsi)
-    646d1052:	add    %al,(%rax)
-    646d1054:	add    %dh,%al
-    646d1056:	add    %al,(%rax)
+    646d1028:	jo     646d0fcb <___tls_end__+0xfbb>
+    646d102a:	js     646d0fcd <___tls_end__+0xfbd>
+    646d102c:	andb   $0xb0,-0x5e575e60(%rcx)
+    646d1033:	movabs 0xa5e0a5d0a5c0a1b8,%eax
+    646d103c:	lock movsl %ds:(%rsi),%es:(%rdi)
+    646d103e:	add    %ah,-0x59df59f0(%rsi)
+    646d1044:	xor    %ah,-0x59af59c0(%rsi)
+    646d104a:	(bad)
+    646d104b:	cmpsb  %es:(%rdi),%ds:(%rsi)
+    646d104c:	jo     646d0ff4 <___tls_end__+0xfe4>
+    646d104e:	andb   $0x0,0xa690(%rsi)
+    646d1055:	lock add %al,(%rax)
     646d1058:	adc    %al,(%rax)
     646d105a:	add    %al,(%rax)
     646d105c:	sbb    %ah,-0x5fc75fd0(%rax)
 	...
 
 Disassembly of section .debug_aranges:
 
@@ -15210,15 +15030,19 @@
     646d2002:	add    %al,(%rax)
     646d2004:	add    (%rax),%al
     646d2006:	add    %al,(%rax)
     646d2008:	add    %al,(%rax)
     646d200a:	or     %al,(%rax)
     646d200c:	add    %al,(%rax)
     646d200e:	add    %al,(%rax)
-    646d2010:	movabs 0x3200000000646c67,%al
+    646d2010:	mov    $0x64,%al
+    646d2012:	insb   (%dx),%es:(%rdi)
+    646d2013:	add    %al,%fs:(%rax)
+    646d2016:	add    %al,(%rax)
+    646d2018:	xor    (%rax),%al
 	...
 
 00000000646d2030 <.debug_aranges>:
     646d2030:	sbb    $0x0,%al
     646d2032:	add    %al,(%rax)
     646d2034:	add    (%rax),%al
     646d2036:	cs add %al,(%rax)
@@ -15232,16 +15056,20 @@
     646d3002:	add    %al,(%rax)
     646d3004:	add    (%rax),%al
     646d3006:	add    %al,(%rax)
     646d3008:	add    %al,(%rax)
     646d300a:	or     %al,(%rcx)
     646d300c:	add    %al,(%rax)
     646d300e:	add    %al,(%rax)
-    646d3010:	movabs 0xd200000000646c67,%al
-    646d3019:	insb   (%dx),%es:(%edi)
+    646d3010:	mov    $0x64,%al
+    646d3012:	insb   (%dx),%es:(%rdi)
+    646d3013:	add    %al,%fs:(%rax)
+    646d3016:	add    %al,(%rax)
+    646d3018:	loop   646d307e <.debug_info+0x50>
+    646d301a:	insb   (%dx),%es:(%rdi)
     646d301b:	add    %al,%fs:(%rax)
     646d301e:	add    %al,(%rax)
     646d3020:	add    %al,(%rax)
     646d3022:	add    %al,(%rax)
     646d3024:	cmp    %eax,(%rax)
     646d3026:	add    %al,(%rax)
     646d3028:	pop    (%rax)
@@ -19357,22 +19185,22 @@
     646d4ed8:	pop    %rdi
     646d4ed9:	add    %cl,(%rax,%rsi,1)
     646d4edc:	adc    %edi,0x0(%rsi,%rbx,1)
     646d4ee0:	add    %bl,(%rax)
     646d4ee2:	xchg   %ebx,(%rsi)
     646d4ee4:	add    %al,(%rax)
     646d4ee6:	or     $0x90a0939,%eax
-    646d4eeb:	add    0x7e(%rax),%eax
+    646d4eeb:	add    0x7b(%rax),%edx
     646d4eee:	insb   (%dx),%es:(%rdi)
     646d4eef:	add    %al,%fs:(%rax)
     646d4ef2:	add    %al,(%rax)
     646d4ef4:	sbb    %bl,0xd00001e(%rbp)
     646d4efa:	cmp    (%rcx),%cl
     646d4efc:	or     (%rcx),%cl
-    646d4efe:	add    0x7e(%rax),%ebx
+    646d4efe:	add    0x7b(%rax),%ebp
     646d4f01:	insb   (%dx),%es:(%rdi)
     646d4f02:	add    %al,%fs:(%rax)
     646d4f05:	add    %al,(%rax)
 	...
 
 Disassembly of section .debug_abbrev:
 
@@ -19547,16 +19375,19 @@
     646d604f:	ja     646d60ba <.debug_line+0x3f>
     646d6051:	outsb  %ds:(%rsi),(%dx)
     646d6052:	cs push %rbx
     646d6054:	add    %al,(%rcx)
     646d6056:	add    %al,(%rax)
     646d6058:	add    %al,(%rax)
     646d605a:	or     %eax,(%rdx)
-    646d605c:	movabs 0x300000000646c67,%al
-    646d6065:	hlt
+    646d605c:	mov    $0x64,%al
+    646d605e:	insb   (%dx),%es:(%rdi)
+    646d605f:	add    %al,%fs:(%rax)
+    646d6062:	add    %al,(%rax)
+    646d6064:	add    %esp,%esi
     646d6066:	add    %al,(%rcx)
     646d6068:	and    (%rdx),%ah
     646d606a:	addr32 pop %rcx
     646d606c:	xor    %dh,0x4b(%rbp)
     646d606f:	addr32 xor %bh,0x222224c(%eip)        # 668f82c3 <.debug_str+0x22202c3>
     646d6077:	add    %eax,(%rax)
     646d6079:	add    %eax,(%rcx)
@@ -19717,19 +19548,23 @@
     646d700d:	or     $0x7,%al
     646d700f:	or     %ah,0x1(%rax)
     646d7015:	add    %al,(%rax)
     646d7017:	add    %ch,(%rax,%rax,1)
     646d701a:	add    %al,(%rax)
     646d701c:	add    %al,(%rax)
     646d701e:	add    %al,(%rax)
-    646d7020:	movabs 0x3200000000646c67,%al
-    646d7029:	add    %al,(%rax)
-    646d702b:	add    %al,(%rax)
-    646d702d:	add    %al,(%rax)
-    646d702f:	add    %al,0xe(%rcx)
+    646d7020:	mov    $0x64,%al
+    646d7022:	insb   (%dx),%es:(%rdi)
+    646d7023:	add    %al,%fs:(%rax)
+    646d7026:	add    %al,(%rax)
+    646d7028:	xor    (%rax),%al
+    646d702a:	add    %al,(%rax)
+    646d702c:	add    %al,(%rax)
+    646d702e:	add    %al,(%rax)
+    646d7030:	rex.B (bad)
     646d7032:	adc    %al,0x180e4102(%rdx)
     646d7038:	addb   $0x6e,(%rbx)
     646d703b:	(bad)
     646d703c:	adc    %al,%al
     646d703e:	rex.B (bad)
     646d7040:	or     %al,%dl
     646d7042:	add    %al,(%rax)
```

### Comparing `uc_sgsim-1.2.1/uc_sgsim/c_core/uc_sgsim.so` & `uc_sgsim-1.2.2/uc_sgsim/c_core/uc_sgsim.so`

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

 * *Files 4% similar despite different names*

#### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x1aa0
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          35232 (bytes into file)
+  Start of section headers:          35240 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         7
   Size of section headers:           64 (bytes)
   Number of section headers:         28
   Section header string table index: 27
```

#### readelf --wide --program-header {}

```diff
@@ -1,19 +1,19 @@
 
 Elf file type is DYN (Shared object file)
 Entry point 0x1aa0
 There are 7 program headers, starting at offset 64
 
 Program Headers:
   Type           Offset   VirtAddr           PhysAddr           FileSiz  MemSiz   Flg Align
-  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x006860 0x006860 R E 0x200000
+  LOAD           0x000000 0x0000000000000000 0x0000000000000000 0x0065b0 0x0065b0 R E 0x200000
   LOAD           0x006e00 0x0000000000206e00 0x0000000000206e00 0x000380 0x000670 RW  0x200000
   DYNAMIC        0x006e10 0x0000000000206e10 0x0000000000206e10 0x0001d0 0x0001d0 RW  0x8
   NOTE           0x0001c8 0x00000000000001c8 0x00000000000001c8 0x000024 0x000024 R   0x4
-  GNU_EH_FRAME   0x005e20 0x0000000000005e20 0x0000000000005e20 0x00020c 0x00020c R   0x4
+  GNU_EH_FRAME   0x005b70 0x0000000000005b70 0x0000000000005b70 0x00020c 0x00020c R   0x4
   GNU_STACK      0x000000 0x0000000000000000 0x0000000000000000 0x000000 0x000000 RW  0x10
   GNU_RELRO      0x006e00 0x0000000000206e00 0x0000000000206e00 0x000200 0x000200 R   0x1
 
  Section to Segment mapping:
   Segment Sections...
    00     .note.gnu.build-id .gnu.hash .dynsym .dynstr .gnu.version .gnu.version_r .rela.dyn .rela.plt .init .plt .plt.got .text .fini .rodata .eh_frame_hdr .eh_frame 
    01     .init_array .fini_array .dynamic .got .got.plt .data .bss
```

#### readelf --wide --sections {}

```diff
@@ -1,37 +1,37 @@
-There are 28 section headers, starting at offset 0x89a0:
+There are 28 section headers, starting at offset 0x89a8:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.build-id NOTE            00000000000001c8 0001c8 000024 00   A  0   0  4
   [ 2] .gnu.hash         GNU_HASH        00000000000001f0 0001f0 000268 00   A  3   0  8
   [ 3] .dynsym           DYNSYM          0000000000000458 000458 0008a0 18   A  4   1  8
-  [ 4] .dynstr           STRTAB          0000000000000cf8 000cf8 0004f1 00   A  0   0  1
-  [ 5] .gnu.version      VERSYM          00000000000011ea 0011ea 0000b8 02   A  3   0  2
+  [ 4] .dynstr           STRTAB          0000000000000cf8 000cf8 0004f5 00   A  0   0  1
+  [ 5] .gnu.version      VERSYM          00000000000011ee 0011ee 0000b8 02   A  3   0  2
   [ 6] .gnu.version_r    VERNEED         00000000000012a8 0012a8 000030 00   A  4   1  8
   [ 7] .rela.dyn         RELA            00000000000012d8 0012d8 0000a8 18   A  3   0  8
   [ 8] .rela.plt         RELA            0000000000001380 001380 000420 18  AI  3  21  8
   [ 9] .init             PROGBITS        00000000000017a0 0017a0 000017 00  AX  0   0  4
   [10] .plt              PROGBITS        00000000000017c0 0017c0 0002d0 10  AX  0   0 16
   [11] .plt.got          PROGBITS        0000000000001a90 001a90 000008 08  AX  0   0  8
-  [12] .text             PROGBITS        0000000000001aa0 001aa0 0041d9 00  AX  0   0 16
-  [13] .fini             PROGBITS        0000000000005c7c 005c7c 000009 00  AX  0   0  4
-  [14] .rodata           PROGBITS        0000000000005c90 005c90 000190 00   A  0   0 16
-  [15] .eh_frame_hdr     PROGBITS        0000000000005e20 005e20 00020c 00   A  0   0  4
-  [16] .eh_frame         PROGBITS        0000000000006030 006030 000830 00   A  0   0  8
+  [12] .text             PROGBITS        0000000000001aa0 001aa0 003f44 00  AX  0   0 16
+  [13] .fini             PROGBITS        00000000000059e4 0059e4 000009 00  AX  0   0  4
+  [14] .rodata           PROGBITS        00000000000059f0 0059f0 000180 00   A  0   0 16
+  [15] .eh_frame_hdr     PROGBITS        0000000000005b70 005b70 00020c 00   A  0   0  4
+  [16] .eh_frame         PROGBITS        0000000000005d80 005d80 000830 00   A  0   0  8
   [17] .init_array       INIT_ARRAY      0000000000206e00 006e00 000008 08  WA  0   0  8
   [18] .fini_array       FINI_ARRAY      0000000000206e08 006e08 000008 08  WA  0   0  8
   [19] .dynamic          DYNAMIC         0000000000206e10 006e10 0001d0 10  WA  4   0  8
   [20] .got              PROGBITS        0000000000206fe0 006fe0 000020 08  WA  0   0  8
   [21] .got.plt          PROGBITS        0000000000207000 007000 000178 08  WA  0   0  8
   [22] .data             PROGBITS        0000000000207178 007178 000008 00  WA  0   0  8
   [23] .bss              NOBITS          0000000000207180 007180 0002f0 00  WA  0   0 32
   [24] .comment          PROGBITS        0000000000000000 007180 000029 01  MS  0   0  1
   [25] .symtab           SYMTAB          0000000000000000 0071b0 000f60 18     26  73  8
-  [26] .strtab           STRTAB          0000000000000000 008110 00079f 00      0   0  1
-  [27] .shstrtab         STRTAB          0000000000000000 0088af 0000f1 00      0   0  1
+  [26] .strtab           STRTAB          0000000000000000 008110 0007a3 00      0   0  1
+  [27] .shstrtab         STRTAB          0000000000000000 0088b3 0000f1 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

#### readelf --wide --symbols {}

```diff
@@ -28,51 +28,51 @@
     24: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@GLIBC_2.2.5 (2)
     25: 0000000000003451    71 FUNC    GLOBAL DEFAULT   12 mt19937_get_double
     26: 0000000000004af2    88 FUNC    GLOBAL DEFAULT   12 d_arange
     27: 0000000000002eb5    46 FUNC    GLOBAL DEFAULT   12 c_array_mean_double
     28: 0000000000002a4d   134 FUNC    GLOBAL DEFAULT   12 c_array_var_long_long
     29: 0000000000002f28    73 FUNC    GLOBAL DEFAULT   12 c_array_sum_long
     30: 0000000000002bdb   151 FUNC    GLOBAL DEFAULT   12 c_array_std_int
-    31: 0000000000004f02   109 FUNC    GLOBAL DEFAULT   12 sgsim_init
-    32: 00000000000058b6   737 FUNC    GLOBAL DEFAULT   12 variogram
+    31: 0000000000004f02   110 FUNC    GLOBAL DEFAULT   12 sgsim_init
+    32: 00000000000055d2   816 FUNC    GLOBAL DEFAULT   12 variogram
     33: 0000000000002fc7    86 FUNC    GLOBAL DEFAULT   12 c_array_sum_double
     34: 0000000000002b59   130 FUNC    GLOBAL DEFAULT   12 c_array_var_double
     35: 0000000000003f7d   435 FUNC    GLOBAL DEFAULT   12 find_neighbor
     36: 0000000000002c72   153 FUNC    GLOBAL DEFAULT   12 c_array_std_long_long
     37: 000000000000303b    34 FUNC    GLOBAL DEFAULT   12 cmpfunc_long
     38: 0000000000002ee3    69 FUNC    GLOBAL DEFAULT   12 c_array_sum_int
-    39: 0000000000005658   508 FUNC    GLOBAL DEFAULT   12 Partition2d
-    40: 000000000000335f    68 FUNC    GLOBAL DEFAULT   12 mt19937_get_int32_range
+    39: 000000000000335f    68 FUNC    GLOBAL DEFAULT   12 mt19937_get_int32_range
+    40: 00000000000054b1   194 FUNC    GLOBAL DEFAULT   12 partition2d
     41: 0000000000002d0b   153 FUNC    GLOBAL DEFAULT   12 c_array_std_float
-    42: 0000000000005c7c     0 FUNC    GLOBAL DEFAULT   13 _fini
+    42: 00000000000059e4     0 FUNC    GLOBAL DEFAULT   13 _fini
     43: 0000000000003589   109 FUNC    GLOBAL DEFAULT   12 cov_model_init
     44: 000000000000317c   483 FUNC    GLOBAL DEFAULT   12 mt19937_generate
     45: 0000000000004a9e    84 FUNC    GLOBAL DEFAULT   12 arange
     46: 000000000000427c  1153 FUNC    GLOBAL DEFAULT   12 lu_inverse_solver
     47: 0000000000002da4   149 FUNC    GLOBAL DEFAULT   12 c_array_std_double
     48: 00000000000017a0     0 FUNC    GLOBAL DEFAULT    9 _init
     49: 0000000000003847   177 FUNC    GLOBAL DEFAULT   12 sampling_state_init
     50: 00000000000029c9   132 FUNC    GLOBAL DEFAULT   12 c_array_var_int
     51: 0000000000002412   466 FUNC    GLOBAL DEFAULT   12 c_array_min_long_long
-    52: 000000000000545e    31 FUNC    GLOBAL DEFAULT   12 sgsim_t_free
+    52: 00000000000053ca    31 FUNC    GLOBAL DEFAULT   12 sgsim_t_free
     53: 000000000000305d    82 FUNC    GLOBAL DEFAULT   12 cmpfunc_float
     54: 0000000000002094   475 FUNC    GLOBAL DEFAULT   12 c_array_max_double
     55: 0000000000004e48   186 FUNC    GLOBAL DEFAULT   12 randompath
-    56: 0000000000005854    98 FUNC    GLOBAL DEFAULT   12 quicksort2d
+    56: 0000000000005573    95 FUNC    GLOBAL DEFAULT   12 quicksort2d
     57: 0000000000004b4a   171 FUNC    GLOBAL DEFAULT   12 pdist
     58: 0000000000001d05   441 FUNC    GLOBAL DEFAULT   12 c_array_max_long_long
     59: 00000000000046fd   929 FUNC    GLOBAL DEFAULT   12 lu_decomposition
-    60: 0000000000004f6f  1263 FUNC    GLOBAL DEFAULT   12 sgsim_run
+    60: 0000000000004f70  1114 FUNC    GLOBAL DEFAULT   12 sgsim_run
     61: 0000000000003103   121 FUNC    GLOBAL DEFAULT   12 mt19937_init
     62: 00000000000027d4   501 FUNC    GLOBAL DEFAULT   12 c_array_min_double
-    63: 0000000000005b97   226 FUNC    GLOBAL DEFAULT   12 variance
+    63: 0000000000005902   226 FUNC    GLOBAL DEFAULT   12 variance
     64: 0000000000004bf5   135 FUNC    GLOBAL DEFAULT   12 matrixform
-    65: 00000000000054cf   393 FUNC    GLOBAL DEFAULT   12 swap
-    66: 0000000000002f71    86 FUNC    GLOBAL DEFAULT   12 c_array_sum_float
-    67: 00000000000030af    84 FUNC    GLOBAL DEFAULT   12 cmpfunc_double
+    65: 0000000000002f71    86 FUNC    GLOBAL DEFAULT   12 c_array_sum_float
+    66: 00000000000030af    84 FUNC    GLOBAL DEFAULT   12 cmpfunc_double
+    67: 000000000000543b   118 FUNC    GLOBAL DEFAULT   12 swaprows
     68: 0000000000002ad3   134 FUNC    GLOBAL DEFAULT   12 c_array_var_float
     69: 00000000002072e0   144 OBJECT  GLOBAL DEFAULT   23 st
     70: 0000000000003498   104 FUNC    GLOBAL DEFAULT   12 mt19937_get_double_range
     71: 0000000000002e39    40 FUNC    GLOBAL DEFAULT   12 c_array_mean_int
     72: 000000000000301d    30 FUNC    GLOBAL DEFAULT   12 cmpfunc_int
     73: 0000000000207180     0 NOTYPE  GLOBAL DEFAULT   22 _edata
     74: 00000000000038f8    43 FUNC    GLOBAL DEFAULT   12 sampling_state_update
@@ -97,26 +97,26 @@
 Symbol table '.symtab' contains 164 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 00000000000001c8     0 SECTION LOCAL  DEFAULT    1 .note.gnu.build-id
      2: 00000000000001f0     0 SECTION LOCAL  DEFAULT    2 .gnu.hash
      3: 0000000000000458     0 SECTION LOCAL  DEFAULT    3 .dynsym
      4: 0000000000000cf8     0 SECTION LOCAL  DEFAULT    4 .dynstr
-     5: 00000000000011ea     0 SECTION LOCAL  DEFAULT    5 .gnu.version
+     5: 00000000000011ee     0 SECTION LOCAL  DEFAULT    5 .gnu.version
      6: 00000000000012a8     0 SECTION LOCAL  DEFAULT    6 .gnu.version_r
      7: 00000000000012d8     0 SECTION LOCAL  DEFAULT    7 .rela.dyn
      8: 0000000000001380     0 SECTION LOCAL  DEFAULT    8 .rela.plt
      9: 00000000000017a0     0 SECTION LOCAL  DEFAULT    9 .init
     10: 00000000000017c0     0 SECTION LOCAL  DEFAULT   10 .plt
     11: 0000000000001a90     0 SECTION LOCAL  DEFAULT   11 .plt.got
     12: 0000000000001aa0     0 SECTION LOCAL  DEFAULT   12 .text
-    13: 0000000000005c7c     0 SECTION LOCAL  DEFAULT   13 .fini
-    14: 0000000000005c90     0 SECTION LOCAL  DEFAULT   14 .rodata
-    15: 0000000000005e20     0 SECTION LOCAL  DEFAULT   15 .eh_frame_hdr
-    16: 0000000000006030     0 SECTION LOCAL  DEFAULT   16 .eh_frame
+    13: 00000000000059e4     0 SECTION LOCAL  DEFAULT   13 .fini
+    14: 00000000000059f0     0 SECTION LOCAL  DEFAULT   14 .rodata
+    15: 0000000000005b70     0 SECTION LOCAL  DEFAULT   15 .eh_frame_hdr
+    16: 0000000000005d80     0 SECTION LOCAL  DEFAULT   16 .eh_frame
     17: 0000000000206e00     0 SECTION LOCAL  DEFAULT   17 .init_array
     18: 0000000000206e08     0 SECTION LOCAL  DEFAULT   18 .fini_array
     19: 0000000000206e10     0 SECTION LOCAL  DEFAULT   19 .dynamic
     20: 0000000000206fe0     0 SECTION LOCAL  DEFAULT   20 .got
     21: 0000000000207000     0 SECTION LOCAL  DEFAULT   21 .got.plt
     22: 0000000000207178     0 SECTION LOCAL  DEFAULT   22 .data
     23: 0000000000207180     0 SECTION LOCAL  DEFAULT   23 .bss
@@ -154,109 +154,109 @@
     55: 00000000002073a0    24 OBJECT  LOCAL  DEFAULT   23 u_array
     56: 00000000002073c0    24 OBJECT  LOCAL  DEFAULT   23 sampled
     57: 00000000002073e0    24 OBJECT  LOCAL  DEFAULT   23 variogram_array
     58: 0000000000207400    24 OBJECT  LOCAL  DEFAULT   23 sgsim_array
     59: 0000000000207420    72 OBJECT  LOCAL  DEFAULT   23 _sampling
     60: 0000000000207468     4 OBJECT  LOCAL  DEFAULT   23 flag
     61: 000000000020746c     4 OBJECT  LOCAL  DEFAULT   23 count
-    62: 000000000000547d    82 FUNC    LOCAL  DEFAULT   12 sgsim_memory_free
+    62: 00000000000053e9    82 FUNC    LOCAL  DEFAULT   12 sgsim_memory_free
     63: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS sort_tools.c
     64: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS variogram.c
     65: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS crtstuff.c
-    66: 000000000000685c     0 OBJECT  LOCAL  DEFAULT   16 __FRAME_END__
+    66: 00000000000065ac     0 OBJECT  LOCAL  DEFAULT   16 __FRAME_END__
     67: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS 
     68: 0000000000207178     0 OBJECT  LOCAL  DEFAULT   22 __dso_handle
     69: 0000000000206e10     0 OBJECT  LOCAL  DEFAULT   19 _DYNAMIC
-    70: 0000000000005e20     0 NOTYPE  LOCAL  DEFAULT   15 __GNU_EH_FRAME_HDR
+    70: 0000000000005b70     0 NOTYPE  LOCAL  DEFAULT   15 __GNU_EH_FRAME_HDR
     71: 0000000000207180     0 OBJECT  LOCAL  DEFAULT   22 __TMC_END__
     72: 0000000000207000     0 OBJECT  LOCAL  DEFAULT   21 _GLOBAL_OFFSET_TABLE_
     73: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND free@@GLIBC_2.2.5
     74: 0000000000001ebe   470 FUNC    GLOBAL DEFAULT   12 c_array_max_float
     75: 00000000000029c9   132 FUNC    GLOBAL DEFAULT   12 c_array_var_int
     76: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __errno_location@@GLIBC_2.2.5
     77: 0000000000002f71    86 FUNC    GLOBAL DEFAULT   12 c_array_sum_float
     78: 000000000000301d    30 FUNC    GLOBAL DEFAULT   12 cmpfunc_int
-    79: 0000000000005854    98 FUNC    GLOBAL DEFAULT   12 quicksort2d
+    79: 0000000000005573    95 FUNC    GLOBAL DEFAULT   12 quicksort2d
     80: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_deregisterTMCloneTable
     81: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND mkdir@@GLIBC_2.2.5
     82: 0000000000002ee3    69 FUNC    GLOBAL DEFAULT   12 c_array_sum_int
     83: 0000000000004e48   186 FUNC    GLOBAL DEFAULT   12 randompath
     84: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND ceil
     85: 0000000000207180     0 NOTYPE  GLOBAL DEFAULT   22 _edata
     86: 000000000000427c  1153 FUNC    GLOBAL DEFAULT   12 lu_inverse_solver
     87: 00000000000038f8    43 FUNC    GLOBAL DEFAULT   12 sampling_state_update
     88: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fclose@@GLIBC_2.2.5
-    89: 0000000000004f6f  1263 FUNC    GLOBAL DEFAULT   12 sgsim_run
-    90: 0000000000005c7c     0 FUNC    GLOBAL DEFAULT   13 _fini
+    89: 0000000000004f70  1114 FUNC    GLOBAL DEFAULT   12 sgsim_run
+    90: 00000000000059e4     0 FUNC    GLOBAL DEFAULT   13 _fini
     91: 00000000002072e0   144 OBJECT  GLOBAL DEFAULT   23 st
     92: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND __stack_chk_fail@@GLIBC_2.4
     93: 0000000000004c7c   460 FUNC    GLOBAL DEFAULT   12 save_1darray
     94: 0000000000002b59   130 FUNC    GLOBAL DEFAULT   12 c_array_var_double
     95: 0000000000002e39    40 FUNC    GLOBAL DEFAULT   12 c_array_mean_int
     96: 00000000000025e4   496 FUNC    GLOBAL DEFAULT   12 c_array_min_float
     97: 00000000000036fb   332 FUNC    GLOBAL DEFAULT   12 cov_model2d
     98: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND printf@@GLIBC_2.2.5
     99: 0000000000003f7d   435 FUNC    GLOBAL DEFAULT   12 find_neighbor
    100: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND snprintf@@GLIBC_2.2.5
    101: 00000000000030af    84 FUNC    GLOBAL DEFAULT   12 cmpfunc_double
    102: 00000000000046fd   929 FUNC    GLOBAL DEFAULT   12 lu_decomposition
    103: 0000000000004af2    88 FUNC    GLOBAL DEFAULT   12 d_arange
-   104: 0000000000005658   508 FUNC    GLOBAL DEFAULT   12 Partition2d
-   105: 00000000000033ea   103 FUNC    GLOBAL DEFAULT   12 mt19937_get_float_range
-   106: 00000000000035f6   261 FUNC    GLOBAL DEFAULT   12 cov_model
-   107: 0000000000004bf5   135 FUNC    GLOBAL DEFAULT   12 matrixform
-   108: 000000000000317c   483 FUNC    GLOBAL DEFAULT   12 mt19937_generate
-   109: 0000000000002e61    42 FUNC    GLOBAL DEFAULT   12 c_array_mean_long_long
-   110: 0000000000005b97   226 FUNC    GLOBAL DEFAULT   12 variance
-   111: 0000000000002a4d   134 FUNC    GLOBAL DEFAULT   12 c_array_var_long_long
-   112: 0000000000002bdb   151 FUNC    GLOBAL DEFAULT   12 c_array_std_int
-   113: 0000000000003500   137 FUNC    GLOBAL DEFAULT   12 mt19937_random_normal
-   114: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND calloc@@GLIBC_2.2.5
-   115: 00000000000027d4   501 FUNC    GLOBAL DEFAULT   12 c_array_min_double
-   116: 0000000000003589   109 FUNC    GLOBAL DEFAULT   12 cov_model_init
-   117: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fprintf@@GLIBC_2.2.5
-   118: 000000000000545e    31 FUNC    GLOBAL DEFAULT   12 sgsim_t_free
-   119: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
-   120: 000000000000226f   419 FUNC    GLOBAL DEFAULT   12 c_array_min_int
-   121: 0000000000002da4   149 FUNC    GLOBAL DEFAULT   12 c_array_std_double
-   122: 0000000000001b7a   395 FUNC    GLOBAL DEFAULT   12 c_array_max_int
-   123: 0000000000003923   602 FUNC    GLOBAL DEFAULT   12 krige_param_setting
-   124: 0000000000002f28    73 FUNC    GLOBAL DEFAULT   12 c_array_sum_long
-   125: 0000000000003103   121 FUNC    GLOBAL DEFAULT   12 mt19937_init
-   126: 000000000000305d    82 FUNC    GLOBAL DEFAULT   12 cmpfunc_float
-   127: 0000000000003b7d  1024 FUNC    GLOBAL DEFAULT   12 simple_kriging
-   128: 0000000000002e8b    42 FUNC    GLOBAL DEFAULT   12 c_array_mean_float
-   129: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@@GLIBC_2.2.5
-   130: 0000000000004a9e    84 FUNC    GLOBAL DEFAULT   12 arange
-   131: 0000000000004130   332 FUNC    GLOBAL DEFAULT   12 krige_memory_free
-   132: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND exp
-   133: 0000000000207470     0 NOTYPE  GLOBAL DEFAULT   23 _end
-   134: 0000000000002ad3   134 FUNC    GLOBAL DEFAULT   12 c_array_var_float
-   135: 0000000000207180     0 NOTYPE  GLOBAL DEFAULT   23 __bss_start
-   136: 00000000000058b6   737 FUNC    GLOBAL DEFAULT   12 variogram
-   137: 0000000000002094   475 FUNC    GLOBAL DEFAULT   12 c_array_max_double
-   138: 0000000000002412   466 FUNC    GLOBAL DEFAULT   12 c_array_min_long_long
-   139: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND cos
+   104: 00000000000033ea   103 FUNC    GLOBAL DEFAULT   12 mt19937_get_float_range
+   105: 00000000000035f6   261 FUNC    GLOBAL DEFAULT   12 cov_model
+   106: 0000000000004bf5   135 FUNC    GLOBAL DEFAULT   12 matrixform
+   107: 000000000000317c   483 FUNC    GLOBAL DEFAULT   12 mt19937_generate
+   108: 0000000000002e61    42 FUNC    GLOBAL DEFAULT   12 c_array_mean_long_long
+   109: 0000000000005902   226 FUNC    GLOBAL DEFAULT   12 variance
+   110: 0000000000002a4d   134 FUNC    GLOBAL DEFAULT   12 c_array_var_long_long
+   111: 0000000000002bdb   151 FUNC    GLOBAL DEFAULT   12 c_array_std_int
+   112: 0000000000003500   137 FUNC    GLOBAL DEFAULT   12 mt19937_random_normal
+   113: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND calloc@@GLIBC_2.2.5
+   114: 00000000000027d4   501 FUNC    GLOBAL DEFAULT   12 c_array_min_double
+   115: 0000000000003589   109 FUNC    GLOBAL DEFAULT   12 cov_model_init
+   116: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fprintf@@GLIBC_2.2.5
+   117: 00000000000053ca    31 FUNC    GLOBAL DEFAULT   12 sgsim_t_free
+   118: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND __gmon_start__
+   119: 000000000000226f   419 FUNC    GLOBAL DEFAULT   12 c_array_min_int
+   120: 0000000000002da4   149 FUNC    GLOBAL DEFAULT   12 c_array_std_double
+   121: 0000000000001b7a   395 FUNC    GLOBAL DEFAULT   12 c_array_max_int
+   122: 0000000000003923   602 FUNC    GLOBAL DEFAULT   12 krige_param_setting
+   123: 0000000000002f28    73 FUNC    GLOBAL DEFAULT   12 c_array_sum_long
+   124: 0000000000003103   121 FUNC    GLOBAL DEFAULT   12 mt19937_init
+   125: 000000000000305d    82 FUNC    GLOBAL DEFAULT   12 cmpfunc_float
+   126: 0000000000003b7d  1024 FUNC    GLOBAL DEFAULT   12 simple_kriging
+   127: 0000000000002e8b    42 FUNC    GLOBAL DEFAULT   12 c_array_mean_float
+   128: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND malloc@@GLIBC_2.2.5
+   129: 0000000000004a9e    84 FUNC    GLOBAL DEFAULT   12 arange
+   130: 0000000000004130   332 FUNC    GLOBAL DEFAULT   12 krige_memory_free
+   131: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND exp
+   132: 0000000000207470     0 NOTYPE  GLOBAL DEFAULT   23 _end
+   133: 0000000000002ad3   134 FUNC    GLOBAL DEFAULT   12 c_array_var_float
+   134: 0000000000207180     0 NOTYPE  GLOBAL DEFAULT   23 __bss_start
+   135: 00000000000055d2   816 FUNC    GLOBAL DEFAULT   12 variogram
+   136: 0000000000002094   475 FUNC    GLOBAL DEFAULT   12 c_array_max_double
+   137: 0000000000002412   466 FUNC    GLOBAL DEFAULT   12 c_array_min_long_long
+   138: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND cos
+   139: 00000000000054b1   194 FUNC    GLOBAL DEFAULT   12 partition2d
    140: 000000000000335f    68 FUNC    GLOBAL DEFAULT   12 mt19937_get_int32_range
    141: 0000000000003847   177 FUNC    GLOBAL DEFAULT   12 sampling_state_init
    142: 0000000000003498   104 FUNC    GLOBAL DEFAULT   12 mt19937_get_double_range
-   143: 0000000000004f02   109 FUNC    GLOBAL DEFAULT   12 sgsim_init
+   143: 0000000000004f02   110 FUNC    GLOBAL DEFAULT   12 sgsim_init
    144: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND log
    145: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND fopen@@GLIBC_2.2.5
    146: 0000000000003451    71 FUNC    GLOBAL DEFAULT   12 mt19937_get_double
    147: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND pow
    148: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND perror@@GLIBC_2.2.5
    149: 00000000000033a3    71 FUNC    GLOBAL DEFAULT   12 mt19937_get_float
    150: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND log10
    151: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND sqrt
    152: 000000000000303b    34 FUNC    GLOBAL DEFAULT   12 cmpfunc_long
    153: 0000000000004b4a   171 FUNC    GLOBAL DEFAULT   12 pdist
    154: 0000000000002c72   153 FUNC    GLOBAL DEFAULT   12 c_array_std_long_long
    155: 0000000000000000     0 FUNC    GLOBAL DEFAULT  UND exit@@GLIBC_2.2.5
    156: 0000000000000000     0 NOTYPE  WEAK   DEFAULT  UND _ITM_registerTMCloneTable
-   157: 00000000000054cf   393 FUNC    GLOBAL DEFAULT   12 swap
-   158: 0000000000002eb5    46 FUNC    GLOBAL DEFAULT   12 c_array_mean_double
-   159: 0000000000002d0b   153 FUNC    GLOBAL DEFAULT   12 c_array_std_float
-   160: 0000000000001d05   441 FUNC    GLOBAL DEFAULT   12 c_array_max_long_long
-   161: 0000000000002fc7    86 FUNC    GLOBAL DEFAULT   12 c_array_sum_double
-   162: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@@GLIBC_2.2.5
-   163: 00000000000017a0     0 FUNC    GLOBAL DEFAULT    9 _init
+   157: 0000000000002eb5    46 FUNC    GLOBAL DEFAULT   12 c_array_mean_double
+   158: 0000000000002d0b   153 FUNC    GLOBAL DEFAULT   12 c_array_std_float
+   159: 0000000000001d05   441 FUNC    GLOBAL DEFAULT   12 c_array_max_long_long
+   160: 0000000000002fc7    86 FUNC    GLOBAL DEFAULT   12 c_array_sum_double
+   161: 0000000000000000     0 FUNC    WEAK   DEFAULT  UND __cxa_finalize@@GLIBC_2.2.5
+   162: 00000000000017a0     0 FUNC    GLOBAL DEFAULT    9 _init
+   163: 000000000000543b   118 FUNC    GLOBAL DEFAULT   12 swaprows
```

#### readelf --wide --relocs {}

```diff
@@ -9,49 +9,49 @@
 0000000000206ff0  0000001700000006 R_X86_64_GLOB_DAT      0000000000000000 _ITM_registerTMCloneTable + 0
 0000000000206ff8  0000001800000006 R_X86_64_GLOB_DAT      0000000000000000 __cxa_finalize@GLIBC_2.2.5 + 0
 
 Relocation section '.rela.plt' at offset 0x1380 contains 44 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000207018  0000000100000007 R_X86_64_JUMP_SLOT     0000000000000000 free@GLIBC_2.2.5 + 0
 0000000000207020  0000000200000007 R_X86_64_JUMP_SLOT     0000000000000000 __errno_location@GLIBC_2.2.5 + 0
-0000000000207028  0000003800000007 R_X86_64_JUMP_SLOT     0000000000005854 quicksort2d + 0
+0000000000207028  0000003800000007 R_X86_64_JUMP_SLOT     0000000000005573 quicksort2d + 0
 0000000000207030  0000000400000007 R_X86_64_JUMP_SLOT     0000000000000000 mkdir@GLIBC_2.2.5 + 0
 0000000000207038  0000003700000007 R_X86_64_JUMP_SLOT     0000000000004e48 randompath + 0
 0000000000207040  0000000500000007 R_X86_64_JUMP_SLOT     0000000000000000 ceil + 0
 0000000000207048  0000002e00000007 R_X86_64_JUMP_SLOT     000000000000427c lu_inverse_solver + 0
 0000000000207050  0000004a00000007 R_X86_64_JUMP_SLOT     00000000000038f8 sampling_state_update + 0
 0000000000207058  0000000600000007 R_X86_64_JUMP_SLOT     0000000000000000 fclose@GLIBC_2.2.5 + 0
 0000000000207060  0000000700000007 R_X86_64_JUMP_SLOT     0000000000000000 __stack_chk_fail@GLIBC_2.4 + 0
 0000000000207068  0000005600000007 R_X86_64_JUMP_SLOT     0000000000004c7c save_1darray + 0
 0000000000207070  0000005700000007 R_X86_64_JUMP_SLOT     00000000000036fb cov_model2d + 0
 0000000000207078  0000000800000007 R_X86_64_JUMP_SLOT     0000000000000000 printf@GLIBC_2.2.5 + 0
 0000000000207080  0000002300000007 R_X86_64_JUMP_SLOT     0000000000003f7d find_neighbor + 0
 0000000000207088  0000000900000007 R_X86_64_JUMP_SLOT     0000000000000000 snprintf@GLIBC_2.2.5 + 0
 0000000000207090  0000003b00000007 R_X86_64_JUMP_SLOT     00000000000046fd lu_decomposition + 0
 0000000000207098  0000001a00000007 R_X86_64_JUMP_SLOT     0000000000004af2 d_arange + 0
-00000000002070a0  0000002700000007 R_X86_64_JUMP_SLOT     0000000000005658 Partition2d + 0
-00000000002070a8  0000005b00000007 R_X86_64_JUMP_SLOT     00000000000035f6 cov_model + 0
-00000000002070b0  0000004000000007 R_X86_64_JUMP_SLOT     0000000000004bf5 matrixform + 0
-00000000002070b8  0000002c00000007 R_X86_64_JUMP_SLOT     000000000000317c mt19937_generate + 0
-00000000002070c0  0000005400000007 R_X86_64_JUMP_SLOT     0000000000003500 mt19937_random_normal + 0
-00000000002070c8  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 calloc@GLIBC_2.2.5 + 0
-00000000002070d0  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000000000 fprintf@GLIBC_2.2.5 + 0
-00000000002070d8  0000005900000007 R_X86_64_JUMP_SLOT     0000000000003923 krige_param_setting + 0
-00000000002070e0  0000003d00000007 R_X86_64_JUMP_SLOT     0000000000003103 mt19937_init + 0
-00000000002070e8  0000004b00000007 R_X86_64_JUMP_SLOT     0000000000003b7d simple_kriging + 0
-00000000002070f0  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
-00000000002070f8  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000004a9e arange + 0
-0000000000207100  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000004130 krige_memory_free + 0
-0000000000207108  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 exp + 0
-0000000000207110  0000002000000007 R_X86_64_JUMP_SLOT     00000000000058b6 variogram + 0
-0000000000207118  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 cos + 0
+00000000002070a0  0000005b00000007 R_X86_64_JUMP_SLOT     00000000000035f6 cov_model + 0
+00000000002070a8  0000004000000007 R_X86_64_JUMP_SLOT     0000000000004bf5 matrixform + 0
+00000000002070b0  0000002c00000007 R_X86_64_JUMP_SLOT     000000000000317c mt19937_generate + 0
+00000000002070b8  0000005400000007 R_X86_64_JUMP_SLOT     0000000000003500 mt19937_random_normal + 0
+00000000002070c0  0000000a00000007 R_X86_64_JUMP_SLOT     0000000000000000 calloc@GLIBC_2.2.5 + 0
+00000000002070c8  0000000b00000007 R_X86_64_JUMP_SLOT     0000000000000000 fprintf@GLIBC_2.2.5 + 0
+00000000002070d0  0000005900000007 R_X86_64_JUMP_SLOT     0000000000003923 krige_param_setting + 0
+00000000002070d8  0000003d00000007 R_X86_64_JUMP_SLOT     0000000000003103 mt19937_init + 0
+00000000002070e0  0000004b00000007 R_X86_64_JUMP_SLOT     0000000000003b7d simple_kriging + 0
+00000000002070e8  0000000d00000007 R_X86_64_JUMP_SLOT     0000000000000000 malloc@GLIBC_2.2.5 + 0
+00000000002070f0  0000002d00000007 R_X86_64_JUMP_SLOT     0000000000004a9e arange + 0
+00000000002070f8  0000004c00000007 R_X86_64_JUMP_SLOT     0000000000004130 krige_memory_free + 0
+0000000000207100  0000000e00000007 R_X86_64_JUMP_SLOT     0000000000000000 exp + 0
+0000000000207108  0000002000000007 R_X86_64_JUMP_SLOT     00000000000055d2 variogram + 0
+0000000000207110  0000000f00000007 R_X86_64_JUMP_SLOT     0000000000000000 cos + 0
+0000000000207118  0000002800000007 R_X86_64_JUMP_SLOT     00000000000054b1 partition2d + 0
 0000000000207120  0000003100000007 R_X86_64_JUMP_SLOT     0000000000003847 sampling_state_init + 0
 0000000000207128  0000001000000007 R_X86_64_JUMP_SLOT     0000000000000000 log + 0
 0000000000207130  0000001100000007 R_X86_64_JUMP_SLOT     0000000000000000 fopen@GLIBC_2.2.5 + 0
 0000000000207138  0000001900000007 R_X86_64_JUMP_SLOT     0000000000003451 mt19937_get_double + 0
 0000000000207140  0000001200000007 R_X86_64_JUMP_SLOT     0000000000000000 pow + 0
 0000000000207148  0000001300000007 R_X86_64_JUMP_SLOT     0000000000000000 perror@GLIBC_2.2.5 + 0
 0000000000207150  0000001400000007 R_X86_64_JUMP_SLOT     0000000000000000 log10 + 0
 0000000000207158  0000001500000007 R_X86_64_JUMP_SLOT     0000000000000000 sqrt + 0
 0000000000207160  0000003900000007 R_X86_64_JUMP_SLOT     0000000000004b4a pdist + 0
 0000000000207168  0000001600000007 R_X86_64_JUMP_SLOT     0000000000000000 exit@GLIBC_2.2.5 + 0
-0000000000207170  0000004100000007 R_X86_64_JUMP_SLOT     00000000000054cf swap + 0
+0000000000207170  0000004300000007 R_X86_64_JUMP_SLOT     000000000000543b swaprows + 0
```

#### readelf --wide --dynamic {}

```diff
@@ -1,28 +1,28 @@
 
 Dynamic section at offset 0x6e10 contains 25 entries:
   Tag        Type                         Name/Value
  0x0000000000000001 (NEEDED)             Shared library: [libc.so.6]
  0x000000000000000e (SONAME)             Library soname: [uc_sgsim.so]
  0x000000000000000c (INIT)               0x17a0
- 0x000000000000000d (FINI)               0x5c7c
+ 0x000000000000000d (FINI)               0x59e4
  0x0000000000000019 (INIT_ARRAY)         0x206e00
  0x000000000000001b (INIT_ARRAYSZ)       8 (bytes)
  0x000000000000001a (FINI_ARRAY)         0x206e08
  0x000000000000001c (FINI_ARRAYSZ)       8 (bytes)
  0x000000006ffffef5 (GNU_HASH)           0x1f0
  0x0000000000000005 (STRTAB)             0xcf8
  0x0000000000000006 (SYMTAB)             0x458
- 0x000000000000000a (STRSZ)              1265 (bytes)
+ 0x000000000000000a (STRSZ)              1269 (bytes)
  0x000000000000000b (SYMENT)             24 (bytes)
  0x0000000000000003 (PLTGOT)             0x207000
  0x0000000000000002 (PLTRELSZ)           1056 (bytes)
  0x0000000000000014 (PLTREL)             RELA
  0x0000000000000017 (JMPREL)             0x1380
  0x0000000000000007 (RELA)               0x12d8
  0x0000000000000008 (RELASZ)             168 (bytes)
  0x0000000000000009 (RELAENT)            24 (bytes)
  0x000000006ffffffe (VERNEED)            0x12a8
  0x000000006fffffff (VERNEEDNUM)         1
- 0x000000006ffffff0 (VERSYM)             0x11ea
+ 0x000000006ffffff0 (VERSYM)             0x11ee
  0x000000006ffffff9 (RELACOUNT)          3
  0x0000000000000000 (NULL)               0x0
```

#### readelf --wide --notes {}

```diff
@@ -1,4 +1,4 @@
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: a9d1358c10911257af561997e012a3f6d7611e2d
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 335c44964a141f1462109ca13cc3a3de1efdf43c
```

#### readelf --wide --version-info {}

```diff
@@ -1,10 +1,10 @@
 
 Version symbols section '.gnu.version' contains 92 entries:
- Addr: 0x00000000000011ea  Offset: 0x000011ea  Link: 3 (.dynsym)
+ Addr: 0x00000000000011ee  Offset: 0x000011ee  Link: 3 (.dynsym)
   000:   0 (*local*)       2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   0 (*local*)    
   004:   2 (GLIBC_2.2.5)   0 (*local*)       2 (GLIBC_2.2.5)   3 (GLIBC_2.4)  
   008:   2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)   2 (GLIBC_2.2.5)
   00c:   0 (*local*)       2 (GLIBC_2.2.5)   0 (*local*)       0 (*local*)    
   010:   0 (*local*)       2 (GLIBC_2.2.5)   0 (*local*)       2 (GLIBC_2.2.5)
   014:   0 (*local*)       0 (*local*)       2 (GLIBC_2.2.5)   0 (*local*)    
   018:   2 (GLIBC_2.2.5)   1 (*global*)      1 (*global*)      1 (*global*)
```

#### readelf --wide --debug-dump=frames {}

```diff
@@ -616,109 +616,111 @@
   DW_CFA_advance_loc: 3 to 0000000000004e4c
   DW_CFA_def_cfa_register: r6 (rbp)
   DW_CFA_advance_loc1: 181 to 0000000000004f01
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000708 000000000000001c 0000070c FDE cie=00000000 pc=0000000000004f02..0000000000004f6f
+00000708 000000000000001c 0000070c FDE cie=00000000 pc=0000000000004f02..0000000000004f70
   DW_CFA_advance_loc: 1 to 0000000000004f03
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
   DW_CFA_advance_loc: 3 to 0000000000004f06
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 104 to 0000000000004f6e
+  DW_CFA_advance_loc1: 105 to 0000000000004f6f
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000728 000000000000001c 0000072c FDE cie=00000000 pc=0000000000004f6f..000000000000545e
-  DW_CFA_advance_loc: 1 to 0000000000004f70
+00000728 000000000000001c 0000072c FDE cie=00000000 pc=0000000000004f70..00000000000053ca
+  DW_CFA_advance_loc: 1 to 0000000000004f71
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000004f73
+  DW_CFA_advance_loc: 3 to 0000000000004f74
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 1258 to 000000000000545d
+  DW_CFA_advance_loc2: 1109 to 00000000000053c9
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
 
-00000748 000000000000001c 0000074c FDE cie=00000000 pc=000000000000545e..000000000000547d
-  DW_CFA_advance_loc: 1 to 000000000000545f
+00000748 000000000000001c 0000074c FDE cie=00000000 pc=00000000000053ca..00000000000053e9
+  DW_CFA_advance_loc: 1 to 00000000000053cb
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000005462
+  DW_CFA_advance_loc: 3 to 00000000000053ce
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 26 to 000000000000547c
+  DW_CFA_advance_loc: 26 to 00000000000053e8
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
 
-00000768 000000000000001c 0000076c FDE cie=00000000 pc=000000000000547d..00000000000054cf
-  DW_CFA_advance_loc: 1 to 000000000000547e
+00000768 000000000000001c 0000076c FDE cie=00000000 pc=00000000000053e9..000000000000543b
+  DW_CFA_advance_loc: 1 to 00000000000053ea
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000005481
+  DW_CFA_advance_loc: 3 to 00000000000053ed
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 77 to 00000000000054ce
+  DW_CFA_advance_loc1: 77 to 000000000000543a
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-00000788 000000000000001c 0000078c FDE cie=00000000 pc=00000000000054cf..0000000000005658
-  DW_CFA_advance_loc: 1 to 00000000000054d0
+00000788 000000000000001c 0000078c FDE cie=00000000 pc=000000000000543b..00000000000054b1
+  DW_CFA_advance_loc: 1 to 000000000000543c
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000054d3
+  DW_CFA_advance_loc: 3 to 000000000000543f
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 388 to 0000000000005657
+  DW_CFA_advance_loc1: 113 to 00000000000054b0
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
+  DW_CFA_nop
 
-000007a8 000000000000001c 000007ac FDE cie=00000000 pc=0000000000005658..0000000000005854
-  DW_CFA_advance_loc: 1 to 0000000000005659
+000007a8 000000000000001c 000007ac FDE cie=00000000 pc=00000000000054b1..0000000000005573
+  DW_CFA_advance_loc: 1 to 00000000000054b2
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 000000000000565c
+  DW_CFA_advance_loc: 3 to 00000000000054b5
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc2: 503 to 0000000000005853
+  DW_CFA_advance_loc1: 189 to 0000000000005572
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
+  DW_CFA_nop
 
-000007c8 000000000000001c 000007cc FDE cie=00000000 pc=0000000000005854..00000000000058b6
-  DW_CFA_advance_loc: 1 to 0000000000005855
+000007c8 000000000000001c 000007cc FDE cie=00000000 pc=0000000000005573..00000000000055d2
+  DW_CFA_advance_loc: 1 to 0000000000005574
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000005858
+  DW_CFA_advance_loc: 3 to 0000000000005577
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 93 to 00000000000058b5
+  DW_CFA_advance_loc1: 90 to 00000000000055d1
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-000007e8 0000000000000020 000007ec FDE cie=00000000 pc=00000000000058b6..0000000000005b97
-  DW_CFA_advance_loc: 1 to 00000000000058b7
+000007e8 0000000000000020 000007ec FDE cie=00000000 pc=00000000000055d2..0000000000005902
+  DW_CFA_advance_loc: 1 to 00000000000055d3
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 00000000000058ba
+  DW_CFA_advance_loc: 3 to 00000000000055d6
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc: 8 to 00000000000058c2
+  DW_CFA_advance_loc: 8 to 00000000000055de
   DW_CFA_offset: r3 (rbx) at cfa-24
-  DW_CFA_advance_loc2: 724 to 0000000000005b96
+  DW_CFA_advance_loc2: 803 to 0000000000005901
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
-0000080c 000000000000001c 00000810 FDE cie=00000000 pc=0000000000005b97..0000000000005c79
-  DW_CFA_advance_loc: 1 to 0000000000005b98
+0000080c 000000000000001c 00000810 FDE cie=00000000 pc=0000000000005902..00000000000059e4
+  DW_CFA_advance_loc: 1 to 0000000000005903
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r6 (rbp) at cfa-16
-  DW_CFA_advance_loc: 3 to 0000000000005b9b
+  DW_CFA_advance_loc: 3 to 0000000000005906
   DW_CFA_def_cfa_register: r6 (rbp)
-  DW_CFA_advance_loc1: 221 to 0000000000005c78
+  DW_CFA_advance_loc1: 221 to 00000000000059e3
   DW_CFA_def_cfa: r7 (rsp) ofs 8
   DW_CFA_nop
   DW_CFA_nop
 
 0000082c ZERO terminator
```

#### strings --all --bytes=8 {}

```diff
@@ -57,15 +57,16 @@
 snprintf
 __errno_location
 randompath
 sgsim_init
 sgsim_run
 variogram
 sgsim_t_free
-Partition2d
+swaprows
+partition2d
 variance
 libc.so.6
 __bss_start
 uc_sgsim.so
 GLIBC_2.4
 GLIBC_2.2.5
 %s%s%%0%dd.txt
@@ -132,15 +133,14 @@
 c_array_min_float
 cov_model2d
 find_neighbor
 snprintf@@GLIBC_2.2.5
 cmpfunc_double
 lu_decomposition
 d_arange
-Partition2d
 mt19937_get_float_range
 cov_model
 matrixform
 mt19937_generate
 c_array_mean_long_long
 variance
 c_array_var_long_long
@@ -164,14 +164,15 @@
 malloc@@GLIBC_2.2.5
 krige_memory_free
 c_array_var_float
 __bss_start
 variogram
 c_array_max_double
 c_array_min_long_long
+partition2d
 mt19937_get_int32_range
 sampling_state_init
 mt19937_get_double_range
 sgsim_init
 fopen@@GLIBC_2.2.5
 mt19937_get_double
 perror@@GLIBC_2.2.5
@@ -181,14 +182,15 @@
 exit@@GLIBC_2.2.5
 _ITM_registerTMCloneTable
 c_array_mean_double
 c_array_std_float
 c_array_max_long_long
 c_array_sum_double
 __cxa_finalize@@GLIBC_2.2.5
+swaprows
 .shstrtab
 .note.gnu.build-id
 .gnu.hash
 .gnu.version
 .gnu.version_r
 .rela.dyn
 .rela.plt
```

#### readelf --wide --decompress --hex-dump=.gnu.hash {}

```diff
@@ -1,42 +1,42 @@
 
 Hex dump of section '.gnu.hash':
   0x000001f0 43000000 19000000 08000000 09000000 C...............
-  0x00000200 10e08c22 91803852 09004848 10c20000 ..."..8R..HH....
+  0x00000200 10e0ac22 91803856 08004048 10c20000 ..."..8V..@H....
   0x00000210 bd501a05 81000cb2 00080008 01128218 .P..............
-  0x00000220 a0010000 04200800 18670c10 0c000329 ..... ...g.....)
-  0x00000230 44301940 001a4719 9a406109 e0072005 D0.@..G..@a... .
+  0x00000220 a0010000 04200800 18670c11 0c080329 ..... ...g.....)
+  0x00000230 44301940 001a4719 9a406109 e0070005 D0.@..G..@a.....
   0x00000240 19000000 1a000000 1b000000 00000000 ................
   0x00000250 1c000000 1e000000 20000000 00000000 ........ .......
   0x00000260 00000000 00000000 00000000 00000000 ................
   0x00000270 22000000 00000000 25000000 00000000 ".......%.......
-  0x00000280 26000000 27000000 29000000 00000000 &...'...).......
+  0x00000280 26000000 27000000 28000000 00000000 &...'...(.......
   0x00000290 2a000000 2b000000 00000000 2c000000 *...+.......,...
   0x000002a0 00000000 2e000000 30000000 31000000 ........0...1...
   0x000002b0 00000000 32000000 33000000 00000000 ....2...3.......
   0x000002c0 34000000 37000000 38000000 3b000000 4...7...8...;...
   0x000002d0 00000000 3c000000 00000000 3e000000 ....<.......>...
-  0x000002e0 3f000000 00000000 40000000 41000000 ?.......@...A...
-  0x000002f0 42000000 00000000 44000000 45000000 B.......D...E...
+  0x000002e0 3f000000 00000000 40000000 00000000 ?.......@.......
+  0x000002f0 41000000 00000000 44000000 45000000 A.......D...E...
   0x00000300 47000000 00000000 48000000 00000000 G.......H.......
   0x00000310 00000000 00000000 4b000000 4d000000 ........K...M...
   0x00000320 4f000000 00000000 51000000 52000000 O.......Q...R...
   0x00000330 00000000 53000000 54000000 55000000 ....S...T...U...
   0x00000340 56000000 5a000000 5b000000 ed523622 V...Z...[....R6"
   0x00000350 575ed140 81082768 aced6b56 49a556a6 W^.@..'h..kVI.V.
   0x00000360 9a7eccea dbeee89d 2c0fda6c 35a6ef83 .~......,..l5...
   0x00000370 e8ad9f13 529b421c cfd54cbf 21e6ec38 ....R.B...L.!..8
-  0x00000380 c583c4ed f44b86b6 8dbd42ad 8522afcf .....K....B.."..
+  0x00000380 c583c4ed 8dbd42ad 14f41c62 8522afcf ......B....b."..
   0x00000390 ebd3ef0e d14bcb53 bc728bf5 936569f2 .....K.S.r...ei.
   0x000003a0 7a11a928 4bb922c1 b98df10e 938ebb25 z..(K."........%
   0x000003b0 f98766a6 27ae3cfe bcc077d4 e6751b56 ..f.'.<...w..u.V
   0x000003c0 0591cb78 93a872c6 80869b07 685c2210 ...x..r.....h\".
   0x000003d0 a9d740ac 23e77c8f bc64c1e5 8761bfcb ..@.#.|..d...a..
-  0x000003e0 43c81ce2 4fa56b9e 0ffc3a64 41269e7c C...O.k...:dA&.|
-  0x000003f0 2e1abd70 cb781915 63fbf0d9 8c795900 ...p.x..c....yY.
+  0x000003e0 43c81ce2 4fa56b9e 0ffc3a64 2e1abd70 C...O.k...:d...p
+  0x000003f0 ca781915 6bb10750 63fbf0d9 8c795900 .x..k..Pc....yY.
   0x00000400 79e3bb76 91293232 ba859a85 4245d5ec y..v.)22....BE..
   0x00000410 8398f89e 18728efc b163b564 fa622b87 .....r...c.d.b+.
   0x00000420 e70f0566 34f806f2 bbe3927c b330011b ...f4......|.0..
   0x00000430 45614063 5fb6b6ef db2bd0ec e16e6e8f Ea@c_....+...nn.
   0x00000440 a61cc108 3226666d 3248fb03 059e6eb0 ....2&fm2H....n.
   0x00000450 d971581c 1da4accf                   .qX.....
```

#### readelf --wide --decompress --hex-dump=.dynstr {}

```diff
@@ -69,15 +69,15 @@
   0x00001118 6e746600 6d6b6469 72005f5f 6572726e ntf.mkdir.__errn
   0x00001128 6f5f6c6f 63617469 6f6e0066 6f70656e o_location.fopen
   0x00001138 00706572 726f7200 65786974 00667072 .perror.exit.fpr
   0x00001148 696e7466 0066636c 6f736500 72616e64 intf.fclose.rand
   0x00001158 6f6d7061 74680073 6773696d 5f696e69 ompath.sgsim_ini
   0x00001168 74007367 73696d5f 72756e00 76617269 t.sgsim_run.vari
   0x00001178 6f677261 6d007367 73696d5f 745f6672 ogram.sgsim_t_fr
-  0x00001188 65650073 77617000 50617274 6974696f ee.swap.Partitio
-  0x00001198 6e326400 76617269 616e6365 006c6962 n2d.variance.lib
-  0x000011a8 632e736f 2e36005f 65646174 61005f5f c.so.6._edata.__
-  0x000011b8 6273735f 73746172 74005f65 6e640075 bss_start._end.u
-  0x000011c8 635f7367 73696d2e 736f0047 4c494243 c_sgsim.so.GLIBC
-  0x000011d8 5f322e34 00474c49 42435f32 2e322e35 _2.4.GLIBC_2.2.5
-  0x000011e8 00                                  .
+  0x00001188 65650073 77617072 6f777300 70617274 ee.swaprows.part
+  0x00001198 6974696f 6e326400 76617269 616e6365 ition2d.variance
+  0x000011a8 006c6962 632e736f 2e36005f 65646174 .libc.so.6._edat
+  0x000011b8 61005f5f 6273735f 73746172 74005f65 a.__bss_start._e
+  0x000011c8 6e640075 635f7367 73696d2e 736f0047 nd.uc_sgsim.so.G
+  0x000011d8 4c494243 5f322e34 00474c49 42435f32 LIBC_2.4.GLIBC_2
+  0x000011e8 2e322e35 00                         .2.5.
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.plt {}

```diff
@@ -89,90 +89,90 @@
 	jmp    17c0 <.plt>
 
 00000000000018d0 <d_arange@plt>:
 	jmp    *0x2057c2(%rip)        
 	push   $0x10
 	jmp    17c0 <.plt>
 
-00000000000018e0 <Partition2d@plt>:
+00000000000018e0 <cov_model@plt>:
 	jmp    *0x2057ba(%rip)        
 	push   $0x11
 	jmp    17c0 <.plt>
 
-00000000000018f0 <cov_model@plt>:
+00000000000018f0 <matrixform@plt>:
 	jmp    *0x2057b2(%rip)        
 	push   $0x12
 	jmp    17c0 <.plt>
 
-0000000000001900 <matrixform@plt>:
+0000000000001900 <mt19937_generate@plt>:
 	jmp    *0x2057aa(%rip)        
 	push   $0x13
 	jmp    17c0 <.plt>
 
-0000000000001910 <mt19937_generate@plt>:
+0000000000001910 <mt19937_random_normal@plt>:
 	jmp    *0x2057a2(%rip)        
 	push   $0x14
 	jmp    17c0 <.plt>
 
-0000000000001920 <mt19937_random_normal@plt>:
+0000000000001920 <calloc@plt>:
 	jmp    *0x20579a(%rip)        
 	push   $0x15
 	jmp    17c0 <.plt>
 
-0000000000001930 <calloc@plt>:
+0000000000001930 <fprintf@plt>:
 	jmp    *0x205792(%rip)        
 	push   $0x16
 	jmp    17c0 <.plt>
 
-0000000000001940 <fprintf@plt>:
+0000000000001940 <krige_param_setting@plt>:
 	jmp    *0x20578a(%rip)        
 	push   $0x17
 	jmp    17c0 <.plt>
 
-0000000000001950 <krige_param_setting@plt>:
+0000000000001950 <mt19937_init@plt>:
 	jmp    *0x205782(%rip)        
 	push   $0x18
 	jmp    17c0 <.plt>
 
-0000000000001960 <mt19937_init@plt>:
+0000000000001960 <simple_kriging@plt>:
 	jmp    *0x20577a(%rip)        
 	push   $0x19
 	jmp    17c0 <.plt>
 
-0000000000001970 <simple_kriging@plt>:
+0000000000001970 <malloc@plt>:
 	jmp    *0x205772(%rip)        
 	push   $0x1a
 	jmp    17c0 <.plt>
 
-0000000000001980 <malloc@plt>:
+0000000000001980 <arange@plt>:
 	jmp    *0x20576a(%rip)        
 	push   $0x1b
 	jmp    17c0 <.plt>
 
-0000000000001990 <arange@plt>:
+0000000000001990 <krige_memory_free@plt>:
 	jmp    *0x205762(%rip)        
 	push   $0x1c
 	jmp    17c0 <.plt>
 
-00000000000019a0 <krige_memory_free@plt>:
+00000000000019a0 <exp@plt>:
 	jmp    *0x20575a(%rip)        
 	push   $0x1d
 	jmp    17c0 <.plt>
 
-00000000000019b0 <exp@plt>:
+00000000000019b0 <variogram@plt>:
 	jmp    *0x205752(%rip)        
 	push   $0x1e
 	jmp    17c0 <.plt>
 
-00000000000019c0 <variogram@plt>:
+00000000000019c0 <cos@plt>:
 	jmp    *0x20574a(%rip)        
 	push   $0x1f
 	jmp    17c0 <.plt>
 
-00000000000019d0 <cos@plt>:
+00000000000019d0 <partition2d@plt>:
 	jmp    *0x205742(%rip)        
 	push   $0x20
 	jmp    17c0 <.plt>
 
 00000000000019e0 <sampling_state_init@plt>:
 	jmp    *0x20573a(%rip)        
 	push   $0x21
@@ -219,11 +219,11 @@
 	jmp    17c0 <.plt>
 
 0000000000001a70 <exit@plt>:
 	jmp    *0x2056f2(%rip)        
 	push   $0x2a
 	jmp    17c0 <.plt>
 
-0000000000001a80 <swap@plt>:
+0000000000001a80 <swaprows@plt>:
 	jmp    *0x2056ea(%rip)        
 	push   $0x2b
 	jmp    17c0 <.plt>
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -314,17 +314,17 @@
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x28(%rbp)
 	mov    %esi,-0x2c(%rbp)
 	mov    -0x2c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x4(%rbp)
-	movss  0x3dbe(%rip),%xmm0        
+	movss  0x3b1e(%rip),%xmm0        
 	movss  %xmm0,-0x18(%rbp)
-	movss  0x3db5(%rip),%xmm0        
+	movss  0x3b15(%rip),%xmm0        
 	movss  %xmm0,-0x14(%rbp)
 	cmpl   $0x0,-0x4(%rbp)
 	je     1ef6 <c_array_max_float+0x38>
 	subl   $0x1,-0x2c(%rbp)
 	mov    -0x28(%rbp),%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x10(%rbp)
@@ -435,17 +435,17 @@
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x38(%rbp)
 	mov    %esi,-0x3c(%rbp)
 	mov    -0x3c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x24(%rbp)
-	movsd  0x3bf0(%rip),%xmm0        
+	movsd  0x3950(%rip),%xmm0        
 	movsd  %xmm0,-0x20(%rbp)
-	movsd  0x3beb(%rip),%xmm0        
+	movsd  0x394b(%rip),%xmm0        
 	movsd  %xmm0,-0x18(%rbp)
 	cmpl   $0x0,-0x24(%rbp)
 	je     20cc <c_array_max_double+0x38>
 	subl   $0x1,-0x3c(%rbp)
 	mov    -0x38(%rbp),%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x10(%rbp)
@@ -661,16 +661,16 @@
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	mov    %eax,-0x14(%rbp)
-	lea    0x3894(%rip),%rdx        
-	lea    0x3891(%rip),%rax        
+	lea    0x35f4(%rip),%rdx        
+	lea    0x35f1(%rip),%rax        
 	cmp    %rax,%rdx
 	jne    240d <c_array_min_int+0x19e>
 	mov    -0x18(%rbp),%eax
 	jmp    2410 <c_array_min_int+0x1a1>
 	mov    -0x14(%rbp),%eax
 	pop    %rbp
 	ret
@@ -787,16 +787,16 @@
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,-0x18(%rbp)
-	lea    0x36c4(%rip),%rdx        
-	lea    0x36c1(%rip),%rax        
+	lea    0x3424(%rip),%rdx        
+	lea    0x3421(%rip),%rax        
 	cmp    %rax,%rdx
 	jne    25de <c_array_min_long_long+0x1cc>
 	mov    -0x20(%rbp),%rax
 	jmp    25e2 <c_array_min_long_long+0x1d0>
 	mov    -0x18(%rbp),%rax
 	pop    %rbp
 	ret
@@ -806,17 +806,17 @@
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x28(%rbp)
 	mov    %esi,-0x2c(%rbp)
 	mov    -0x2c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x4(%rbp)
-	movss  0x3698(%rip),%xmm0        
+	movss  0x33f8(%rip),%xmm0        
 	movss  %xmm0,-0x18(%rbp)
-	movss  0x368f(%rip),%xmm0        
+	movss  0x33ef(%rip),%xmm0        
 	movss  %xmm0,-0x14(%rbp)
 	cmpl   $0x0,-0x4(%rbp)
 	je     261c <c_array_min_float+0x38>
 	subl   $0x1,-0x2c(%rbp)
 	mov    -0x28(%rbp),%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x10(%rbp)
@@ -914,16 +914,16 @@
 	mov    -0x2c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	movss  %xmm0,-0x14(%rbp)
-	lea    0x34d6(%rip),%rdx        
-	lea    0x34d3(%rip),%rax        
+	lea    0x3236(%rip),%rdx        
+	lea    0x3233(%rip),%rax        
 	cmp    %rax,%rdx
 	jne    27cd <c_array_min_float+0x1e9>
 	movss  -0x18(%rbp),%xmm0
 	jmp    27d2 <c_array_min_float+0x1ee>
 	movss  -0x14(%rbp),%xmm0
 	pop    %rbp
 	ret
@@ -933,17 +933,17 @@
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x38(%rbp)
 	mov    %esi,-0x3c(%rbp)
 	mov    -0x3c(%rbp),%eax
 	and    $0x1,%eax
 	mov    %eax,-0x24(%rbp)
-	movsd  0x34b0(%rip),%xmm0        
+	movsd  0x3210(%rip),%xmm0        
 	movsd  %xmm0,-0x20(%rbp)
-	movsd  0x34ab(%rip),%xmm0        
+	movsd  0x320b(%rip),%xmm0        
 	movsd  %xmm0,-0x18(%rbp)
 	cmpl   $0x0,-0x24(%rbp)
 	je     280c <c_array_min_double+0x38>
 	subl   $0x1,-0x3c(%rbp)
 	mov    -0x38(%rbp),%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x10(%rbp)
@@ -1041,16 +1041,16 @@
 	mov    -0x3c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  %xmm0,-0x18(%rbp)
-	lea    0x32e1(%rip),%rdx        
-	lea    0x32de(%rip),%rax        
+	lea    0x3041(%rip),%rdx        
+	lea    0x303e(%rip),%rax        
 	cmp    %rax,%rdx
 	jne    29c2 <c_array_min_double+0x1ee>
 	movsd  -0x20(%rbp),%xmm0
 	jmp    29c7 <c_array_min_double+0x1f3>
 	movsd  -0x18(%rbp),%xmm0
 	pop    %rbp
 	ret
@@ -1071,15 +1071,15 @@
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	cvtsi2sd %eax,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x329a(%rip),%xmm1        
+	movsd  0x2ffa(%rip),%xmm1        
 	call   1a20 <pow@plt>
 	movapd %xmm0,%xmm1
 	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
@@ -1108,15 +1108,15 @@
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	cvtsi2sd %rax,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x3214(%rip),%xmm1        
+	movsd  0x2f74(%rip),%xmm1        
 	call   1a20 <pow@plt>
 	movapd %xmm0,%xmm1
 	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
@@ -1145,15 +1145,15 @@
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	cvtss2sd %xmm0,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x318e(%rip),%xmm1        
+	movsd  0x2eee(%rip),%xmm1        
 	call   1a20 <pow@plt>
 	movapd %xmm0,%xmm1
 	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
@@ -1181,15 +1181,15 @@
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x310c(%rip),%xmm1        
+	movsd  0x2e6c(%rip),%xmm1        
 	call   1a20 <pow@plt>
 	movapd %xmm0,%xmm1
 	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
@@ -1218,15 +1218,15 @@
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	cvtsi2sd %eax,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x3088(%rip),%xmm1        
+	movsd  0x2de8(%rip),%xmm1        
 	call   1a20 <pow@plt>
 	movapd %xmm0,%xmm1
 	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
@@ -1259,15 +1259,15 @@
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	cvtsi2sd %rax,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x2fef(%rip),%xmm1        
+	movsd  0x2d4f(%rip),%xmm1        
 	call   1a20 <pow@plt>
 	movapd %xmm0,%xmm1
 	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
@@ -1300,15 +1300,15 @@
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movss  (%rax),%xmm0
 	cvtss2sd %xmm0,%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x2f56(%rip),%xmm1        
+	movsd  0x2cb6(%rip),%xmm1        
 	call   1a20 <pow@plt>
 	movapd %xmm0,%xmm1
 	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
@@ -1340,15 +1340,15 @@
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	subsd  -0x28(%rbp),%xmm0
-	movsd  0x2ec1(%rip),%xmm1        
+	movsd  0x2c21(%rip),%xmm1        
 	call   1a20 <pow@plt>
 	movapd %xmm0,%xmm1
 	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
@@ -1792,15 +1792,15 @@
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	mov    %esi,-0xc(%rbp)
 	mov    %edx,-0x10(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    %rax,%rdi
-	call   1910 <mt19937_generate@plt>
+	call   1900 <mt19937_generate@plt>
 	mov    %rax,%rdx
 	mov    -0x10(%rbp),%eax
 	sub    -0xc(%rbp),%eax
 	add    $0x1,%eax
 	movslq %eax,%rcx
 	mov    %rdx,%rax
 	mov    $0x0,%edx
@@ -1816,52 +1816,52 @@
 mt19937_get_float():
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    %rax,%rdi
-	call   1910 <mt19937_generate@plt>
+	call   1900 <mt19937_generate@plt>
 	test   %rax,%rax
 	js     33c7 <mt19937_get_float+0x24>
 	cvtsi2ss %rax,%xmm0
 	jmp    33dc <mt19937_get_float+0x39>
 	mov    %rax,%rdx
 	shr    %rdx
 	and    $0x1,%eax
 	or     %rax,%rdx
 	cvtsi2ss %rdx,%xmm0
 	addss  %xmm0,%xmm0
-	movss  0x28d4(%rip),%xmm1        
+	movss  0x2634(%rip),%xmm1        
 	divss  %xmm1,%xmm0
 	leave
 	ret
 
 00000000000033ea <mt19937_get_float_range>:
 mt19937_get_float_range():
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	movss  %xmm0,-0xc(%rbp)
 	movss  %xmm1,-0x10(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    %rax,%rdi
-	call   1910 <mt19937_generate@plt>
+	call   1900 <mt19937_generate@plt>
 	test   %rax,%rax
 	js     3418 <mt19937_get_float_range+0x2e>
 	cvtsi2ss %rax,%xmm0
 	jmp    342d <mt19937_get_float_range+0x43>
 	mov    %rax,%rdx
 	shr    %rdx
 	and    $0x1,%eax
 	or     %rax,%rdx
 	cvtsi2ss %rdx,%xmm0
 	addss  %xmm0,%xmm0
-	movss  0x2883(%rip),%xmm1        
+	movss  0x25e3(%rip),%xmm1        
 	divss  %xmm1,%xmm0
 	movaps %xmm0,%xmm1
 	movss  -0x10(%rbp),%xmm0
 	subss  -0xc(%rbp),%xmm0
 	mulss  %xmm1,%xmm0
 	addss  -0xc(%rbp),%xmm0
 	leave
@@ -1871,52 +1871,52 @@
 mt19937_get_double():
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    %rax,%rdi
-	call   1910 <mt19937_generate@plt>
+	call   1900 <mt19937_generate@plt>
 	test   %rax,%rax
 	js     3475 <mt19937_get_double+0x24>
 	cvtsi2sd %rax,%xmm0
 	jmp    348a <mt19937_get_double+0x39>
 	mov    %rax,%rdx
 	shr    %rdx
 	and    $0x1,%eax
 	or     %rax,%rdx
 	cvtsi2sd %rdx,%xmm0
 	addsd  %xmm0,%xmm0
-	movsd  0x282e(%rip),%xmm1        
+	movsd  0x258e(%rip),%xmm1        
 	divsd  %xmm1,%xmm0
 	leave
 	ret
 
 0000000000003498 <mt19937_get_double_range>:
 mt19937_get_double_range():
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x20,%rsp
 	mov    %rdi,-0x8(%rbp)
 	movsd  %xmm0,-0x10(%rbp)
 	movsd  %xmm1,-0x18(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    %rax,%rdi
-	call   1910 <mt19937_generate@plt>
+	call   1900 <mt19937_generate@plt>
 	test   %rax,%rax
 	js     34c6 <mt19937_get_double_range+0x2e>
 	cvtsi2sd %rax,%xmm0
 	jmp    34db <mt19937_get_double_range+0x43>
 	mov    %rax,%rdx
 	shr    %rdx
 	and    $0x1,%eax
 	or     %rax,%rdx
 	cvtsi2sd %rdx,%xmm0
 	addsd  %xmm0,%xmm0
-	movsd  0x27dd(%rip),%xmm1        
+	movsd  0x253d(%rip),%xmm1        
 	divsd  %xmm1,%xmm0
 	movapd %xmm0,%xmm1
 	movsd  -0x18(%rbp),%xmm0
 	subsd  -0x10(%rbp),%xmm0
 	mulsd  %xmm1,%xmm0
 	addsd  -0x10(%rbp),%xmm0
 	leave
@@ -1939,22 +1939,22 @@
 	movq   %xmm0,%rax
 	mov    %rax,-0x10(%rbp)
 	mov    -0x18(%rbp),%rax
 	mov    %rax,-0x30(%rbp)
 	movsd  -0x30(%rbp),%xmm0
 	call   19f0 <log@plt>
 	movapd %xmm0,%xmm1
-	movsd  0x2774(%rip),%xmm0        
+	movsd  0x24d4(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
 	call   1a50 <sqrt@plt>
 	movsd  %xmm0,-0x30(%rbp)
 	movsd  -0x10(%rbp),%xmm1
-	movsd  0x2761(%rip),%xmm0        
+	movsd  0x24c1(%rip),%xmm0        
 	mulsd  %xmm1,%xmm0
-	call   19d0 <cos@plt>
+	call   19c0 <cos@plt>
 	mulsd  -0x30(%rbp),%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
 	leave
 	ret
 
 0000000000003589 <cov_model_init>:
@@ -2018,25 +2018,25 @@
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	mulsd  %xmm1,%xmm0
-	movsd  0x2668(%rip),%xmm1        
+	movsd  0x23c8(%rip),%xmm1        
 	mulsd  %xmm1,%xmm0
 	mov    -0x40(%rbp),%rax
 	movsd  0x10(%rax),%xmm2
 	mov    -0x40(%rbp),%rax
 	movsd  0x10(%rax),%xmm1
 	mulsd  %xmm2,%xmm1
 	divsd  %xmm1,%xmm0
-	call   19b0 <exp@plt>
+	call   19a0 <exp@plt>
 	movapd %xmm0,%xmm1
-	movsd  0x2641(%rip),%xmm0        
+	movsd  0x23a1(%rip),%xmm0        
 	subsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	mov    -0x40(%rbp),%rax
 	movsd  0x18(%rax),%xmm1
 	movsd  -0x10(%rbp),%xmm0
 	mulsd  -0x8(%rbp),%xmm0
 	subsd  %xmm0,%xmm1
@@ -2069,14 +2069,15 @@
 	mov    %rcx,-0x40(%rbp)
 	mov    -0x40(%rbp),%rax
 	movsd  0x18(%rax),%xmm0
 	mov    -0x40(%rbp),%rax
 	movsd  0x20(%rax),%xmm1
 	subsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x10(%rbp)
+	movl   $0x0,-0x1c(%rbp)
 	movl   $0x0,-0x18(%rbp)
 	jmp    3838 <cov_model2d+0x13d>
 	movl   $0x0,-0x14(%rbp)
 	jmp    3828 <cov_model2d+0x12d>
 	mov    -0x18(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
@@ -2096,54 +2097,51 @@
 	mov    (%rax),%rax
 	mov    -0x14(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	mulsd  %xmm1,%xmm0
-	movsd  0x2537(%rip),%xmm1        
+	movsd  0x2290(%rip),%xmm1        
 	mulsd  %xmm1,%xmm0
 	mov    -0x40(%rbp),%rax
 	movsd  0x10(%rax),%xmm2
 	mov    -0x40(%rbp),%rax
 	movsd  0x10(%rax),%xmm1
 	mulsd  %xmm2,%xmm1
 	divsd  %xmm1,%xmm0
-	call   19b0 <exp@plt>
+	call   19a0 <exp@plt>
 	movapd %xmm0,%xmm1
-	movsd  0x2510(%rip),%xmm0        
+	movsd  0x2269(%rip),%xmm0        
 	subsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	mov    -0x40(%rbp),%rax
 	movsd  0x18(%rax),%xmm1
 	movsd  -0x10(%rbp),%xmm0
 	mulsd  -0x8(%rbp),%xmm0
 	subsd  %xmm0,%xmm1
 	movapd %xmm1,%xmm0
 	mov    -0x40(%rbp),%rax
 	movsd  0x20(%rax),%xmm1
-	mov    -0x34(%rbp),%eax
-	imul   -0x18(%rbp),%eax
-	mov    %eax,%edx
-	mov    -0x14(%rbp),%eax
-	add    %edx,%eax
+	mov    -0x1c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x30(%rbp),%rax
 	add    %rdx,%rax
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
+	addl   $0x1,-0x1c(%rbp)
 	addl   $0x1,-0x14(%rbp)
 	mov    -0x14(%rbp),%eax
 	cmp    -0x34(%rbp),%eax
-	jl     3745 <cov_model2d+0x4a>
+	jl     374c <cov_model2d+0x51>
 	addl   $0x1,-0x18(%rbp)
 	mov    -0x18(%rbp),%eax
 	cmp    -0x34(%rbp),%eax
-	jl     3739 <cov_model2d+0x3e>
+	jl     3740 <cov_model2d+0x45>
 	nop
 	leave
 	ret
 
 0000000000003847 <sampling_state_init>:
 sampling_state_init():
 	push   %rbp
@@ -2168,15 +2166,15 @@
 	movslq %eax,%rdx
 	mov    -0x8(%rbp),%rax
 	mov    %rdx,0x28(%rax)
 	mov    -0xc(%rbp),%eax
 	cltq
 	mov    $0x8,%esi
 	mov    %rax,%rdi
-	call   1930 <calloc@plt>
+	call   1920 <calloc@plt>
 	mov    %rax,%rdx
 	mov    -0x8(%rbp),%rax
 	mov    %rdx,0x18(%rax)
 	mov    -0xc(%rbp),%eax
 	movslq %eax,%rdx
 	mov    -0x8(%rbp),%rax
 	mov    %rdx,0x38(%rax)
@@ -2184,15 +2182,15 @@
 	movslq %eax,%rdx
 	mov    -0x8(%rbp),%rax
 	mov    %rdx,0x40(%rax)
 	mov    -0xc(%rbp),%eax
 	cltq
 	mov    $0x8,%esi
 	mov    %rax,%rdi
-	call   1930 <calloc@plt>
+	call   1920 <calloc@plt>
 	mov    %rax,%rdx
 	mov    -0x8(%rbp),%rax
 	mov    %rdx,0x30(%rax)
 	nop
 	leave
 	ret
 
@@ -2226,101 +2224,101 @@
 	mov    -0x30(%rbp),%rax
 	movsd  0x10(%rax),%xmm0
 	movsd  %xmm0,0x203849(%rip)        
 	movq   $0xa,0x20386e(%rip)        
 	movq   $0xa,0x20386b(%rip)        
 	mov    $0x8,%esi
 	mov    $0xa,%edi
-	call   1930 <calloc@plt>
+	call   1920 <calloc@plt>
 	mov    %rax,0x203845(%rip)        
 	movq   $0xa,0x203862(%rip)        
 	movq   $0xa,0x20385f(%rip)        
 	mov    $0x8,%esi
 	mov    $0xa,%edi
-	call   1930 <calloc@plt>
+	call   1920 <calloc@plt>
 	mov    %rax,0x203839(%rip)        
 	movq   $0xa,0x203876(%rip)        
 	movq   $0xa,0x203873(%rip)        
 	mov    $0x8,%esi
 	mov    $0xa,%edi
-	call   1930 <calloc@plt>
+	call   1920 <calloc@plt>
 	mov    %rax,0x20384d(%rip)        
 	movq   $0xa,0x20388a(%rip)        
 	movq   $0xa,0x203887(%rip)        
 	mov    $0x8,%esi
 	mov    $0xa,%edi
-	call   1930 <calloc@plt>
+	call   1920 <calloc@plt>
 	mov    %rax,0x203861(%rip)        
 	movq   $0x64,0x20383e(%rip)        
 	movq   $0x64,0x20383b(%rip)        
 	mov    $0x8,%esi
 	mov    $0x64,%edi
-	call   1930 <calloc@plt>
+	call   1920 <calloc@plt>
 	mov    %rax,0x203815(%rip)        
 	movq   $0xa,0x2037d2(%rip)        
 	movq   $0xa,0x2037cf(%rip)        
 	mov    $0x8,%esi
 	mov    $0xa,%edi
-	call   1930 <calloc@plt>
+	call   1920 <calloc@plt>
 	mov    %rax,0x2037a9(%rip)        
 	movq   $0xa,0x203846(%rip)        
 	movq   $0xa,0x203843(%rip)        
 	mov    $0x50,%edi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,0x203822(%rip)        
 	movl   $0x0,-0x1c(%rbp)
 	jmp    3aad <krige_param_setting+0x18a>
 	mov    0x203812(%rip),%rax        
 	mov    -0x1c(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	lea    (%rax,%rdx,1),%rbx
 	mov    $0x50,%edi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0x1c(%rbp)
 	cmpl   $0x9,-0x1c(%rbp)
 	jle    3a87 <krige_param_setting+0x164>
 	movq   $0xa,0x20380a(%rip)        
 	movq   $0xa,0x203807(%rip)        
 	mov    $0x50,%edi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,0x2037e6(%rip)        
 	movl   $0x0,-0x18(%rbp)
 	jmp    3b09 <krige_param_setting+0x1e6>
 	mov    0x2037d6(%rip),%rax        
 	mov    -0x18(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	lea    (%rax,%rdx,1),%rbx
 	mov    $0x50,%edi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0x18(%rbp)
 	cmpl   $0x9,-0x18(%rbp)
 	jle    3ae3 <krige_param_setting+0x1c0>
 	mov    -0x24(%rbp),%eax
 	cltq
 	mov    %rax,0x20376d(%rip)        
 	movq   $0x3,0x20376a(%rip)        
 	mov    -0x24(%rbp),%eax
 	cltq
 	shl    $0x3,%rax
 	mov    %rax,%rdi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,0x203742(%rip)        
 	movl   $0x0,-0x14(%rbp)
 	jmp    3b6d <krige_param_setting+0x24a>
 	mov    0x203732(%rip),%rax        
 	mov    -0x14(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	lea    (%rax,%rdx,1),%rbx
 	mov    $0x18,%edi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0x14(%rbp)
 	mov    -0x14(%rbp),%eax
 	cmp    -0x24(%rbp),%eax
 	jl     3b47 <krige_param_setting+0x224>
 	nop
 	add    $0x28,%rsp
@@ -2462,22 +2460,22 @@
 	call   1880 <cov_model2d@plt>
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%edx
 	mov    0x203537(%rip),%rcx        
 	mov    0x2034b0(%rip),%rax        
 	mov    %rcx,%rsi
 	mov    %rax,%rdi
-	call   1900 <matrixform@plt>
+	call   18f0 <matrixform@plt>
 	mov    0x2033ee(%rip),%rcx        
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%edx
 	mov    0x203431(%rip),%rsi        
 	mov    0x20346a(%rip),%rax        
 	mov    %rax,%rdi
-	call   18f0 <cov_model@plt>
+	call   18e0 <cov_model@plt>
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%eax
 	test   %eax,%eax
 	jle    3deb <simple_kriging+0x26e>
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%ecx
 	mov    0x20348b(%rip),%rdx        
@@ -2541,18 +2539,18 @@
 	pxor   %xmm0,%xmm0
 	ucomisd %xmm1,%xmm0
 	jbe    3f03 <simple_kriging+0x386>
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,0x2032a5(%rip)        
 	mov    -0x28(%rbp),%rax
 	mov    %rax,%rdi
-	call   1920 <mt19937_random_normal@plt>
+	call   1910 <mt19937_random_normal@plt>
 	movsd  %xmm0,-0x30(%rbp)
 	mov    0x20328d(%rip),%rax        
-	movsd  0x1dcd(%rip),%xmm0        
+	movsd  0x1b2d(%rip),%xmm0        
 	movapd %xmm0,%xmm1
 	mov    %rax,-0x38(%rbp)
 	movsd  -0x38(%rbp),%xmm0
 	call   1a20 <pow@plt>
 	mulsd  -0x30(%rbp),%xmm0
 	movsd  %xmm0,0x20326e(%rip)        
 	movsd  0x203256(%rip),%xmm1        
@@ -2581,15 +2579,15 @@
 	mov    %rdx,-0x28(%rbp)
 	mov    -0x20(%rbp),%rax
 	mov    (%rax),%eax
 	test   %eax,%eax
 	jne    400c <find_neighbor+0x8f>
 	mov    -0x28(%rbp),%rax
 	mov    %rax,%rdi
-	call   1920 <mt19937_random_normal@plt>
+	call   1910 <mt19937_random_normal@plt>
 	movapd %xmm0,%xmm1
 	mov    0x2031de(%rip),%rax        
 	movsd  0x18(%rax),%xmm0
 	mov    -0x20(%rbp),%rax
 	movsd  0x10(%rax),%xmm2
 	cvttsd2si %xmm2,%eax
 	cltq
@@ -2625,40 +2623,40 @@
 	subsd  %xmm1,%xmm0
 	mov    -0x20(%rbp),%rax
 	mov    0x30(%rax),%rax
 	mov    -0x4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movq   0x1c9e(%rip),%xmm1        
+	movq   0x19fe(%rip),%xmm1        
 	andpd  %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
 	mov    -0x20(%rbp),%rax
 	mov    0x30(%rax),%rax
 	mov    -0x4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
 	movsd  0x20310d(%rip),%xmm2        
-	movsd  0x1c7d(%rip),%xmm0        
+	movsd  0x19dd(%rip),%xmm0        
 	mulsd  %xmm2,%xmm0
 	ucomisd %xmm1,%xmm0
 	jbe    40a1 <find_neighbor+0x124>
 	addl   $0x1,-0x8(%rbp)
 	addl   $0x1,-0x4(%rbp)
 	mov    -0x20(%rbp),%rax
 	mov    0x4(%rax),%eax
 	cmp    %eax,-0x4(%rbp)
 	jl     401f <find_neighbor+0xa2>
 	cmpl   $0x0,-0x8(%rbp)
 	jne    4129 <find_neighbor+0x1ac>
 	mov    -0x28(%rbp),%rax
 	mov    %rax,%rdi
-	call   1920 <mt19937_random_normal@plt>
+	call   1910 <mt19937_random_normal@plt>
 	movapd %xmm0,%xmm1
 	mov    0x2030be(%rip),%rax        
 	movsd  0x18(%rax),%xmm0
 	mov    -0x20(%rbp),%rax
 	movsd  0x10(%rax),%xmm2
 	cvttsd2si %xmm2,%eax
 	cltq
@@ -2779,43 +2777,43 @@
 	mov    %ecx,-0xec(%rbp)
 	mov    %fs:0x28,%rax
 	mov    %rax,-0x18(%rbp)
 	xor    %eax,%eax
 	movq   $0xa,-0xa8(%rbp)
 	movq   $0xa,-0xa0(%rbp)
 	mov    $0x50,%edi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,-0xb0(%rbp)
 	movl   $0x0,-0xd0(%rbp)
 	jmp    4311 <lu_inverse_solver+0x95>
 	mov    -0xb0(%rbp),%rax
 	mov    -0xd0(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	lea    (%rax,%rdx,1),%rbx
 	mov    $0x50,%edi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0xd0(%rbp)
 	cmpl   $0x9,-0xd0(%rbp)
 	jle    42e5 <lu_inverse_solver+0x69>
 	movq   $0xa,-0x88(%rbp)
 	movq   $0xa,-0x80(%rbp)
 	mov    $0x50,%edi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,-0x90(%rbp)
 	movl   $0x0,-0xcc(%rbp)
 	jmp    4376 <lu_inverse_solver+0xfa>
 	mov    -0x90(%rbp),%rax
 	mov    -0xcc(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	lea    (%rax,%rdx,1),%rbx
 	mov    $0x50,%edi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,(%rbx)
 	addl   $0x1,-0xcc(%rbp)
 	cmpl   $0x9,-0xcc(%rbp)
 	jle    434a <lu_inverse_solver+0xce>
 	mov    -0x90(%rbp),%rdx
 	mov    -0xb0(%rbp),%rsi
 	mov    -0xec(%rbp),%ecx
@@ -3138,15 +3136,15 @@
 	mov    -0x38(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x8(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movsd  0x146e(%rip),%xmm0        
+	movsd  0x11ce(%rip),%xmm0        
 	movsd  %xmm0,(%rax)
 	jmp    4a7b <lu_decomposition+0x37e>
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
@@ -3262,15 +3260,15 @@
 	mov    %rsp,%rbp
 	sub    $0x20,%rsp
 	mov    %edi,-0x14(%rbp)
 	mov    -0x14(%rbp),%eax
 	cltq
 	shl    $0x2,%rax
 	mov    %rax,%rdi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
 	jmp    4ae4 <arange+0x46>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,4),%rdx
 	mov    -0x8(%rbp),%rax
@@ -3291,15 +3289,15 @@
 	mov    %rsp,%rbp
 	sub    $0x20,%rsp
 	mov    %edi,-0x14(%rbp)
 	mov    -0x14(%rbp),%eax
 	cltq
 	shl    $0x3,%rax
 	mov    %rax,%rdi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,-0x8(%rbp)
 	movl   $0x0,-0xc(%rbp)
 	jmp    4b3c <d_arange+0x4a>
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x8(%rbp),%rax
@@ -3344,15 +3342,15 @@
 	mov    -0x20(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    -0x4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movq   0x11b2(%rip),%xmm1        
+	movq   0xf12(%rip),%xmm1        
 	andpd  %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
 	addl   $0x1,-0x4(%rbp)
 	mov    -0x4(%rbp),%eax
 	cmp    -0x24(%rbp),%eax
 	jl     4b6e <pdist+0x24>
 	addl   $0x1,-0x8(%rbp)
@@ -3366,23 +3364,20 @@
 0000000000004bf5 <matrixform>:
 matrixform():
 	push   %rbp
 	mov    %rsp,%rbp
 	mov    %rdi,-0x18(%rbp)
 	mov    %rsi,-0x20(%rbp)
 	mov    %edx,-0x24(%rbp)
+	movl   $0x0,-0xc(%rbp)
 	movl   $0x0,-0x8(%rbp)
 	jmp    4c71 <matrixform+0x7c>
 	movl   $0x0,-0x4(%rbp)
 	jmp    4c65 <matrixform+0x70>
-	mov    -0x24(%rbp),%eax
-	imul   -0x8(%rbp),%eax
-	mov    %eax,%edx
-	mov    -0x4(%rbp),%eax
-	add    %edx,%eax
+	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rax,%rdx
 	mov    -0x8(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rcx
@@ -3391,22 +3386,23 @@
 	mov    (%rax),%rax
 	mov    -0x4(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x3,%rcx
 	add    %rcx,%rax
 	movsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rax)
+	addl   $0x1,-0xc(%rbp)
 	addl   $0x1,-0x4(%rbp)
 	mov    -0x4(%rbp),%eax
 	cmp    -0x24(%rbp),%eax
-	jl     4c16 <matrixform+0x21>
+	jl     4c1d <matrixform+0x28>
 	addl   $0x1,-0x8(%rbp)
 	mov    -0x8(%rbp),%eax
 	cmp    -0x24(%rbp),%eax
-	jl     4c0d <matrixform+0x18>
+	jl     4c14 <matrixform+0x1f>
 	nop
 	pop    %rbp
 	ret
 
 0000000000004c7c <save_1darray>:
 save_1darray():
 	push   %rbp
@@ -3430,47 +3426,47 @@
 	mov    -0x1ac(%rbp),%esi
 	mov    -0x1c8(%rbp),%rcx
 	mov    -0x1d0(%rbp),%rdx
 	lea    -0x1a0(%rbp),%rax
 	mov    %esi,%r9d
 	mov    %rcx,%r8
 	mov    %rdx,%rcx
-	lea    0x1017(%rip),%rdx        
+	lea    0xd77(%rip),%rdx        
 	mov    $0xc8,%esi
 	mov    %rax,%rdi
 	mov    $0x0,%eax
 	call   18b0 <snprintf@plt>
 	mov    -0x1d0(%rbp),%rax
 	mov    $0x1f8,%esi
 	mov    %rax,%rdi
 	call   1800 <mkdir@plt>
 	cmp    $0xffffffff,%eax
 	jne    4d51 <save_1darray+0xd5>
 	call   17e0 <__errno_location@plt>
 	mov    (%rax),%eax
 	cmp    $0x11,%eax
 	je     4d51 <save_1darray+0xd5>
-	lea    0xfe8(%rip),%rdi        
+	lea    0xd48(%rip),%rdi        
 	mov    $0x0,%eax
 	call   1890 <printf@plt>
 	mov    -0x1d4(%rbp),%ecx
 	lea    -0x1a0(%rbp),%rdx
 	lea    -0xd0(%rbp),%rax
 	mov    $0xc8,%esi
 	mov    %rax,%rdi
 	mov    $0x0,%eax
 	call   18b0 <snprintf@plt>
 	lea    -0xd0(%rbp),%rax
-	lea    0xfc0(%rip),%rsi        
+	lea    0xd20(%rip),%rsi        
 	mov    %rax,%rdi
 	call   1a00 <fopen@plt>
 	mov    %rax,-0x1a8(%rbp)
 	cmpq   $0x0,-0x1a8(%rbp)
 	jne    4db4 <save_1darray+0x138>
-	lea    0xfa2(%rip),%rdi        
+	lea    0xd02(%rip),%rdi        
 	call   1a30 <perror@plt>
 	mov    $0x1,%edi
 	call   1a70 <exit@plt>
 	movl   $0x0,-0x1b0(%rbp)
 	jmp    4e14 <save_1darray+0x198>
 	mov    -0x1b0(%rbp),%eax
 	cltq
@@ -3478,18 +3474,18 @@
 	mov    -0x1b8(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rcx
 	mov    -0x1b0(%rbp),%edx
 	mov    -0x1a8(%rbp),%rax
 	mov    %rcx,-0x1e0(%rbp)
 	movsd  -0x1e0(%rbp),%xmm0
-	lea    0xf5f(%rip),%rsi        
+	lea    0xcbf(%rip),%rsi        
 	mov    %rax,%rdi
 	mov    $0x1,%eax
-	call   1940 <fprintf@plt>
+	call   1930 <fprintf@plt>
 	addl   $0x1,-0x1b0(%rbp)
 	mov    -0x1b0(%rbp),%eax
 	cmp    -0x1bc(%rbp),%eax
 	jl     4dc0 <save_1darray+0x144>
 	mov    -0x1a8(%rbp),%rax
 	mov    %rax,%rdi
 	call   1850 <fclose@plt>
@@ -3511,15 +3507,15 @@
 	mov    %rdx,-0x28(%rbp)
 	mov    -0x1c(%rbp),%eax
 	sub    $0x1,%eax
 	mov    %eax,-0xc(%rbp)
 	jmp    4ef2 <randompath+0xaa>
 	mov    -0x28(%rbp),%rax
 	mov    %rax,%rdi
-	call   1910 <mt19937_generate@plt>
+	call   1900 <mt19937_generate@plt>
 	mov    %rax,%rdx
 	mov    -0xc(%rbp),%eax
 	movslq %eax,%rcx
 	mov    %rdx,%rax
 	mov    $0x0,%edx
 	div    %rcx
 	mov    %rdx,%rax
@@ -3573,33 +3569,33 @@
 	mov    -0x18(%rbp),%rax
 	mov    -0x20(%rbp),%edx
 	mov    %edx,0x4(%rax)
 	mov    -0x18(%rbp),%rax
 	mov    -0x24(%rbp),%edx
 	mov    %edx,0x8(%rax)
 	cmpl   $0x1,-0x28(%rbp)
-	jne    4f6c <sgsim_init+0x6a>
+	jne    4f6d <sgsim_init+0x6b>
 	mov    -0x1c(%rbp),%eax
 	movslq %eax,%rdx
 	mov    -0x20(%rbp),%eax
 	cltq
 	imul   %rdx,%rax
 	mov    %rax,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
-	shl    $0x3,%rax
+	mov    $0x8,%esi
 	mov    %rax,%rdi
-	call   1980 <malloc@plt>
+	call   1920 <calloc@plt>
 	mov    %rax,%rdx
 	mov    -0x18(%rbp),%rax
 	mov    %rdx,0x10(%rax)
 	nop
 	leave
 	ret
 
-0000000000004f6f <sgsim_run>:
+0000000000004f70 <sgsim_run>:
 sgsim_run():
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0xa00,%rsp
 	mov    %rdi,-0x9e8(%rbp)
 	mov    %rsi,-0x9f0(%rbp)
 	mov    %edx,-0x9f4(%rbp)
@@ -3608,579 +3604,390 @@
 	xor    %eax,%eax
 	mov    -0x9e8(%rbp),%rax
 	mov    0x8(%rax),%eax
 	mov    %eax,%edx
 	lea    -0x9d0(%rbp),%rax
 	mov    %edx,%esi
 	mov    %rax,%rdi
-	call   1960 <mt19937_init@plt>
+	call   1950 <mt19937_init@plt>
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	mov    %eax,%esi
-	lea    0x202454(%rip),%rdi        
+	lea    0x202453(%rip),%rdi        
 	call   19e0 <sampling_state_init@plt>
 	mov    -0x9f0(%rbp),%rax
 	mov    0x8(%rax),%eax
 	cltq
-	mov    %rax,0x202404(%rip)        
+	mov    %rax,0x202403(%rip)        
 	mov    -0x9f0(%rbp),%rax
 	mov    0x8(%rax),%eax
 	cltq
-	mov    %rax,0x2023f9(%rip)        
+	mov    %rax,0x2023f8(%rip)        
 	mov    -0x9f0(%rbp),%rax
 	mov    0x8(%rax),%eax
 	cltq
 	mov    $0x8,%esi
 	mov    %rax,%rdi
-	call   1930 <calloc@plt>
-	mov    %rax,0x2023c9(%rip)        
+	call   1920 <calloc@plt>
+	mov    %rax,0x2023c8(%rip)        
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	cltq
-	mov    %rax,0x2023df(%rip)        
+	mov    %rax,0x2023de(%rip)        
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	cltq
-	mov    %rax,0x2023d5(%rip)        
+	mov    %rax,0x2023d4(%rip)        
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	cltq
 	mov    $0x8,%esi
 	mov    %rax,%rdi
-	call   1930 <calloc@plt>
-	mov    %rax,0x2023a6(%rip)        
+	call   1920 <calloc@plt>
+	mov    %rax,0x2023a5(%rip)        
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	mov    -0x9f0(%rbp),%rdx
 	mov    %rdx,%rsi
 	mov    %eax,%edi
-	call   1950 <krige_param_setting@plt>
+	call   1940 <krige_param_setting@plt>
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	mov    %eax,%edi
-	call   1990 <arange@plt>
-	mov    %rax,0x2022f5(%rip)        
-	movl   $0x0,0x2023d7(%rip)        
-	jmp    541b <sgsim_run+0x4ac>
-	mov    0x2023cc(%rip),%eax        
+	call   1980 <arange@plt>
+	mov    %rax,0x2022f4(%rip)        
+	movl   $0x0,0x2023d6(%rip)        
+	jmp    5387 <sgsim_run+0x417>
+	mov    0x2023cb(%rip),%eax        
 	mov    %eax,%esi
-	lea    0xce7(%rip),%rdi        
+	lea    0xa46(%rip),%rdi        
 	mov    $0x0,%eax
 	call   1890 <printf@plt>
-	movl   $0x0,0x202367(%rip)        
-	movl   $0x0,0x202359(%rip)        
-	movl   $0x0,0x202397(%rip)        
+	movl   $0x0,0x202366(%rip)        
+	movl   $0x0,0x202358(%rip)        
+	movl   $0x0,0x202396(%rip)        
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%ecx
-	mov    0x20229f(%rip),%rax        
+	mov    0x20229e(%rip),%rax        
 	lea    -0x9d0(%rbp),%rdx
 	mov    %ecx,%esi
 	mov    %rax,%rdi
 	call   1810 <randompath@plt>
-	mov    %rax,0x202287(%rip)        
-	movl   $0x0,-0x9d8(%rbp)
-	jmp    516d <sgsim_run+0x1fe>
-	mov    0x2022f4(%rip),%rax        
-	mov    -0x9d8(%rbp),%edx
-	movslq %edx,%rdx
-	shl    $0x3,%rdx
-	add    %rdx,%rax
-	pxor   %xmm0,%xmm0
-	movsd  %xmm0,(%rax)
-	mov    0x20230d(%rip),%rax        
-	mov    -0x9d8(%rbp),%edx
-	movslq %edx,%rdx
-	shl    $0x3,%rdx
-	add    %rdx,%rax
-	pxor   %xmm0,%xmm0
-	movsd  %xmm0,(%rax)
-	mov    0x202306(%rip),%rax        
-	mov    -0x9d8(%rbp),%edx
-	movslq %edx,%rdx
-	shl    $0x3,%rdx
-	add    %rdx,%rax
-	movsd  0xc7e(%rip),%xmm0        
-	movsd  %xmm0,(%rax)
-	addl   $0x1,-0x9d8(%rbp)
-	mov    -0x9e8(%rbp),%rax
-	mov    (%rax),%eax
-	cmp    %eax,-0x9d8(%rbp)
-	jl     5105 <sgsim_run+0x196>
+	mov    %rax,0x202286(%rip)        
 	movl   $0x0,-0x9d4(%rbp)
-	jmp    5318 <sgsim_run+0x3a9>
-	mov    0x2021ec(%rip),%rax        
+	jmp    5294 <sgsim_run+0x324>
+	mov    0x202270(%rip),%rax        
 	mov    -0x9d4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x2,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%eax
 	cvtsi2sd %eax,%xmm0
 	mov    -0x9d4(%rbp),%eax
 	mov    %eax,%esi
-	lea    0x202267(%rip),%rdi        
+	lea    0x2022eb(%rip),%rdi        
 	call   1840 <sampling_state_update@plt>
-	mov    0x20223b(%rip),%rax        
+	mov    0x2022bf(%rip),%rax        
 	lea    -0x9d0(%rbp),%rdx
-	lea    0x20224d(%rip),%rsi        
+	lea    0x2022d1(%rip),%rsi        
 	mov    %rax,%rdi
-	call   1970 <simple_kriging@plt>
-	mov    0x20221e(%rip),%rax        
-	mov    0x202197(%rip),%rdx        
+	call   1960 <simple_kriging@plt>
+	mov    0x2022a2(%rip),%rax        
+	mov    0x20221b(%rip),%rdx        
 	mov    -0x9d4(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x2,%rcx
 	add    %rcx,%rdx
 	mov    (%rdx),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rax,%rdx
 	mov    -0x9e8(%rbp),%rax
 	mov    0x10(%rax),%rcx
-	mov    0x202169(%rip),%rax        
+	mov    0x2021ed(%rip),%rax        
 	mov    -0x9d4(%rbp),%esi
 	movslq %esi,%rsi
 	shl    $0x2,%rsi
 	add    %rsi,%rax
 	mov    (%rax),%esi
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%edi
-	mov    0x202234(%rip),%eax        
+	mov    0x2022b8(%rip),%eax        
 	imul   %edi,%eax
 	add    %esi,%eax
 	cltq
 	shl    $0x3,%rax
 	add    %rcx,%rax
 	movsd  (%rdx),%xmm0
 	movsd  %xmm0,(%rax)
-	mov    0x2021cc(%rip),%eax        
+	mov    0x202250(%rip),%eax        
 	cmp    $0x7,%eax
-	jg     5268 <sgsim_run+0x2f9>
-	mov    0x2021c1(%rip),%eax        
+	jg     51e4 <sgsim_run+0x274>
+	mov    0x202245(%rip),%eax        
 	add    $0x1,%eax
-	mov    %eax,0x2021b8(%rip)        
-	mov    0x202111(%rip),%rax        
+	mov    %eax,0x20223c(%rip)        
+	mov    0x202195(%rip),%rax        
 	mov    -0x9d4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x2,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%ecx
-	mov    0x2021b0(%rip),%rax        
+	mov    0x202234(%rip),%rax        
 	mov    -0x9d4(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	cvtsi2sd %ecx,%xmm0
 	movsd  %xmm0,(%rax)
-	mov    0x20217e(%rip),%eax        
+	mov    0x202202(%rip),%eax        
 	add    $0x1,%eax
-	mov    %eax,0x202175(%rip)        
-	mov    0x20214a(%rip),%rax        
-	mov    0x2020c3(%rip),%rdx        
+	mov    %eax,0x2021f9(%rip)        
+	mov    0x2021ce(%rip),%rax        
+	mov    0x202147(%rip),%rdx        
 	mov    -0x9d4(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x2,%rcx
 	add    %rcx,%rdx
 	mov    (%rdx),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
-	movq   0xb0b(%rip),%xmm0        
+	movq   0x8df(%rip),%xmm0        
 	andpd  %xmm1,%xmm0
-	movsd  0xb0f(%rip),%xmm1        
+	movsd  0x8e3(%rip),%xmm1        
 	ucomisd %xmm0,%xmm1
 	setb   %al
 	xor    $0x1,%eax
 	movzbl %al,%eax
 	test   %eax,%eax
-	jne    5311 <sgsim_run+0x3a2>
-	mov    0x202160(%rip),%eax        
+	jne    528d <sgsim_run+0x31d>
+	mov    0x2021e4(%rip),%eax        
 	add    $0x1,%eax
-	mov    %eax,0x202157(%rip)        
+	mov    %eax,0x2021db(%rip)        
 	addl   $0x1,-0x9d4(%rbp)
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%eax
 	cmp    %eax,-0x9d4(%rbp)
-	jl     518d <sgsim_run+0x21e>
-	mov    0x202139(%rip),%eax        
-	add    $0x1,%eax
-	mov    %eax,0x202130(%rip)        
+	jl     5109 <sgsim_run+0x199>
 	cmpl   $0x1,-0x9f4(%rbp)
-	jne    537b <sgsim_run+0x40c>
+	jne    52e8 <sgsim_run+0x378>
 	mov    -0x9f0(%rbp),%rax
 	mov    0x4(%rax),%edi
 	mov    -0x9f0(%rbp),%rax
 	mov    0x8(%rax),%ecx
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%edx
-	mov    0x202077(%rip),%rsi        
-	mov    0x202090(%rip),%rax        
+	mov    0x20210a(%rip),%rsi        
+	mov    0x202123(%rip),%rax        
 	mov    %edi,%r8d
 	mov    %rax,%rdi
-	call   19c0 <variogram@plt>
-	mov    0x2020e7(%rip),%eax        
+	call   19b0 <variogram@plt>
+	mov    0x20217a(%rip),%eax        
 	test   %eax,%eax
-	jle    5399 <sgsim_run+0x42a>
-	mov    0x2020e1(%rip),%eax        
-	sub    $0x1,%eax
-	mov    %eax,0x2020d8(%rip)        
-	jmp    541b <sgsim_run+0x4ac>
-	mov    0x2020cd(%rip),%ecx        
+	jne    5387 <sgsim_run+0x417>
+	mov    0x202170(%rip),%ecx        
 	mov    -0x9e8(%rbp),%rax
 	mov    0x4(%rax),%edx
 	mov    -0x9e8(%rbp),%rax
 	mov    (%rax),%esi
-	mov    0x202047(%rip),%rax        
+	mov    0x2020ea(%rip),%rax        
 	mov    %ecx,%r9d
 	mov    %edx,%r8d
-	lea    0x9d7(%rip),%rcx        
-	lea    0x9e0(%rip),%rdx        
+	lea    0x7da(%rip),%rcx        
+	lea    0x7e3(%rip),%rdx        
 	mov    %rax,%rdi
 	call   1870 <save_1darray@plt>
 	cmpl   $0x1,-0x9f4(%rbp)
-	jne    541b <sgsim_run+0x4ac>
-	mov    0x202088(%rip),%ecx        
+	jne    5378 <sgsim_run+0x408>
+	mov    0x20212b(%rip),%ecx        
 	mov    -0x9e8(%rbp),%rax
 	mov    0x4(%rax),%edx
 	mov    -0x9f0(%rbp),%rax
 	mov    0x8(%rax),%esi
-	mov    0x201fe1(%rip),%rax        
+	mov    0x202084(%rip),%rax        
 	mov    %ecx,%r9d
 	mov    %edx,%r8d
-	lea    0x9ae(%rip),%rcx        
-	lea    0x9c1(%rip),%rdx        
+	lea    0x7b1(%rip),%rcx        
+	lea    0x7c4(%rip),%rdx        
 	mov    %rax,%rdi
 	call   1870 <save_1darray@plt>
+	mov    0x2020ee(%rip),%eax        
+	add    $0x1,%eax
+	mov    %eax,0x2020e5(%rip)        
 	mov    -0x9e8(%rbp),%rax
 	mov    0x4(%rax),%edx
-	mov    0x202041(%rip),%eax        
+	mov    0x2020d5(%rip),%eax        
 	cmp    %eax,%edx
-	jg     509a <sgsim_run+0x12b>
+	jg     509b <sgsim_run+0x12b>
 	mov    $0x0,%eax
-	call   19a0 <krige_memory_free@plt>
+	call   1990 <krige_memory_free@plt>
 	mov    $0x0,%eax
-	call   547d <sgsim_memory_free>
+	call   53e9 <sgsim_memory_free>
 	nop
 	mov    -0x8(%rbp),%rax
 	xor    %fs:0x28,%rax
-	je     545c <sgsim_run+0x4ed>
+	je     53c8 <sgsim_run+0x458>
 	call   1860 <__stack_chk_fail@plt>
 	leave
 	ret
 
-000000000000545e <sgsim_t_free>:
+00000000000053ca <sgsim_t_free>:
 sgsim_t_free():
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x10,%rsp
 	mov    %rdi,-0x8(%rbp)
 	mov    -0x8(%rbp),%rax
 	mov    0x10(%rax),%rax
 	mov    %rax,%rdi
 	call   17d0 <free@plt>
 	nop
 	leave
 	ret
 
-000000000000547d <sgsim_memory_free>:
+00000000000053e9 <sgsim_memory_free>:
 sgsim_memory_free():
 	push   %rbp
 	mov    %rsp,%rbp
-	mov    0x201fb0(%rip),%rax        
+	mov    0x202044(%rip),%rax        
 	mov    %rax,%rdi
 	call   17d0 <free@plt>
-	mov    0x201fb9(%rip),%rax        
+	mov    0x20204d(%rip),%rax        
 	mov    %rax,%rdi
 	call   17d0 <free@plt>
-	mov    0x201f5a(%rip),%rax        
+	mov    0x201fee(%rip),%rax        
 	mov    %rax,%rdi
 	call   17d0 <free@plt>
-	mov    0x201ecb(%rip),%rax        
+	mov    0x201f5f(%rip),%rax        
 	mov    %rax,%rdi
 	call   17d0 <free@plt>
-	mov    0x201f1c(%rip),%rax        
+	mov    0x201fb0(%rip),%rax        
 	mov    %rax,%rdi
 	call   17d0 <free@plt>
 	nop
 	pop    %rbp
 	ret
 
-00000000000054cf <swap>:
-swap():
+000000000000543b <swaprows>:
+swaprows():
 	push   %rbp
 	mov    %rsp,%rbp
-	mov    %rdi,-0x28(%rbp)
-	mov    %esi,-0x2c(%rbp)
-	mov    %edx,-0x30(%rbp)
-	mov    -0x30(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x28(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	movsd  (%rax),%xmm0
-	movsd  %xmm0,-0x18(%rbp)
-	mov    -0x30(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x28(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	movsd  0x8(%rax),%xmm0
-	movsd  %xmm0,-0x10(%rbp)
-	mov    -0x30(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x28(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	movsd  0x10(%rax),%xmm0
-	movsd  %xmm0,-0x8(%rbp)
-	mov    -0x2c(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x28(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rdx
-	mov    -0x30(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rcx
-	mov    -0x28(%rbp),%rax
-	add    %rcx,%rax
-	mov    (%rax),%rax
-	movsd  (%rdx),%xmm0
-	movsd  %xmm0,(%rax)
-	mov    -0x2c(%rbp),%eax
+	mov    %rdi,-0x18(%rbp)
+	mov    %esi,-0x1c(%rbp)
+	mov    %edx,-0x20(%rbp)
+	mov    -0x20(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x28(%rbp),%rax
+	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
-	mov    -0x30(%rbp),%edx
-	movslq %edx,%rdx
-	lea    0x0(,%rdx,8),%rcx
-	mov    -0x28(%rbp),%rdx
-	add    %rcx,%rdx
-	mov    (%rdx),%rdx
-	add    $0x8,%rdx
-	movsd  0x8(%rax),%xmm0
-	movsd  %xmm0,(%rdx)
-	mov    -0x2c(%rbp),%eax
+	mov    %rax,-0x8(%rbp)
+	mov    -0x1c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x28(%rbp),%rax
+	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
-	mov    (%rax),%rax
-	mov    -0x30(%rbp),%edx
+	mov    -0x20(%rbp),%edx
 	movslq %edx,%rdx
 	lea    0x0(,%rdx,8),%rcx
-	mov    -0x28(%rbp),%rdx
+	mov    -0x18(%rbp),%rdx
 	add    %rcx,%rdx
-	mov    (%rdx),%rdx
-	add    $0x10,%rdx
-	movsd  0x10(%rax),%xmm0
-	movsd  %xmm0,(%rdx)
-	mov    -0x2c(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x28(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	movsd  -0x18(%rbp),%xmm0
-	movsd  %xmm0,(%rax)
-	mov    -0x2c(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x28(%rbp),%rax
-	add    %rdx,%rax
 	mov    (%rax),%rax
-	add    $0x8,%rax
-	movsd  -0x10(%rbp),%xmm0
-	movsd  %xmm0,(%rax)
-	mov    -0x2c(%rbp),%eax
+	mov    %rax,(%rdx)
+	mov    -0x1c(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x28(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	add    $0x10,%rax
-	movsd  -0x8(%rbp),%xmm0
-	movsd  %xmm0,(%rax)
+	mov    -0x18(%rbp),%rax
+	add    %rax,%rdx
+	mov    -0x8(%rbp),%rax
+	mov    %rax,(%rdx)
 	nop
 	pop    %rbp
 	ret
 
-0000000000005658 <Partition2d>:
-Partition2d():
+00000000000054b1 <partition2d>:
+partition2d():
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x20,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	mov    %edx,-0x20(%rbp)
-	mov    -0x20(%rbp),%eax
-	sub    -0x1c(%rbp),%eax
-	mov    %eax,%edx
-	shr    $0x1f,%edx
-	add    %edx,%eax
-	sar    %eax
-	mov    %eax,%edx
 	mov    -0x1c(%rbp),%eax
-	add    %edx,%eax
-	mov    %eax,-0xc(%rbp)
-	mov    -0x1c(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x18(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	add    $0x10,%rax
-	movsd  (%rax),%xmm0
-	mov    -0x20(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x18(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	add    $0x10,%rax
-	movsd  (%rax),%xmm1
-	ucomisd %xmm1,%xmm0
-	jbe    56db <Partition2d+0x83>
-	mov    -0x20(%rbp),%edx
-	mov    -0x1c(%rbp),%ecx
-	mov    -0x18(%rbp),%rax
-	mov    %ecx,%esi
-	mov    %rax,%rdi
-	call   1a80 <swap@plt>
-	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
-	add    $0x10,%rax
-	movsd  (%rax),%xmm0
+	movsd  0x10(%rax),%xmm0
+	movsd  %xmm0,-0x8(%rbp)
+	mov    -0x1c(%rbp),%eax
+	sub    $0x1,%eax
+	mov    %eax,-0x10(%rbp)
 	mov    -0x20(%rbp),%eax
+	add    $0x1,%eax
+	mov    %eax,-0xc(%rbp)
+	addl   $0x1,-0x10(%rbp)
+	mov    -0x10(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    $0x10,%rax
 	movsd  (%rax),%xmm1
+	movsd  -0x8(%rbp),%xmm0
 	ucomisd %xmm1,%xmm0
-	jbe    5733 <Partition2d+0xdb>
-	mov    -0x20(%rbp),%edx
-	mov    -0xc(%rbp),%ecx
-	mov    -0x18(%rbp),%rax
-	mov    %ecx,%esi
-	mov    %rax,%rdi
-	call   1a80 <swap@plt>
+	ja     54f6 <partition2d+0x45>
+	subl   $0x1,-0xc(%rbp)
 	mov    -0xc(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x18(%rbp),%rax
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	add    $0x10,%rax
 	movsd  (%rax),%xmm0
-	mov    -0x1c(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x18(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	add    $0x10,%rax
-	movsd  (%rax),%xmm1
-	ucomisd %xmm1,%xmm0
-	jbe    578b <Partition2d+0x133>
-	mov    -0x1c(%rbp),%edx
-	mov    -0xc(%rbp),%ecx
-	mov    -0x18(%rbp),%rax
-	mov    %ecx,%esi
-	mov    %rax,%rdi
-	call   1a80 <swap@plt>
-	mov    -0x1c(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x18(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	movsd  0x10(%rax),%xmm0
-	movsd  %xmm0,-0x8(%rbp)
-	jmp    5843 <Partition2d+0x1eb>
-	subl   $0x1,-0x20(%rbp)
-	mov    -0x1c(%rbp),%eax
-	cmp    -0x20(%rbp),%eax
-	jge    57e3 <Partition2d+0x18b>
-	mov    -0x20(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x18(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	add    $0x10,%rax
-	movsd  (%rax),%xmm0
 	ucomisd -0x8(%rbp),%xmm0
-	jae    57b1 <Partition2d+0x159>
-	mov    -0x20(%rbp),%edx
-	mov    -0x1c(%rbp),%ecx
-	mov    -0x18(%rbp),%rax
-	mov    %ecx,%esi
-	mov    %rax,%rdi
-	call   1a80 <swap@plt>
-	jmp    57fd <Partition2d+0x1a5>
-	addl   $0x1,-0x1c(%rbp)
-	mov    -0x1c(%rbp),%eax
-	cmp    -0x20(%rbp),%eax
-	jge    582f <Partition2d+0x1d7>
-	mov    -0x1c(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x18(%rbp),%rax
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	add    $0x10,%rax
-	movsd  (%rax),%xmm1
-	movsd  -0x8(%rbp),%xmm0
-	ucomisd %xmm1,%xmm0
-	jae    57f9 <Partition2d+0x1a1>
-	mov    -0x20(%rbp),%edx
-	mov    -0x1c(%rbp),%ecx
+	ja     5524 <partition2d+0x73>
+	mov    -0x10(%rbp),%eax
+	cmp    -0xc(%rbp),%eax
+	jl     555b <partition2d+0xaa>
+	mov    -0xc(%rbp),%eax
+	jmp    5571 <partition2d+0xc0>
+	mov    -0xc(%rbp),%edx
+	mov    -0x10(%rbp),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   1a80 <swap@plt>
-	mov    -0x1c(%rbp),%eax
-	cmp    -0x20(%rbp),%eax
-	jl     57b5 <Partition2d+0x15d>
-	mov    -0x1c(%rbp),%eax
+	call   1a80 <swaprows@plt>
+	jmp    54f6 <partition2d+0x45>
 	leave
 	ret
 
-0000000000005854 <quicksort2d>:
+0000000000005573 <quicksort2d>:
 quicksort2d():
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x20,%rsp
 	mov    %rdi,-0x18(%rbp)
 	mov    %esi,-0x1c(%rbp)
 	mov    %edx,-0x20(%rbp)
 	mov    -0x1c(%rbp),%eax
 	cmp    -0x20(%rbp),%eax
-	jge    58b3 <quicksort2d+0x5f>
+	jge    55cf <quicksort2d+0x5c>
 	mov    -0x20(%rbp),%edx
 	mov    -0x1c(%rbp),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
-	call   18e0 <Partition2d@plt>
+	call   19d0 <partition2d@plt>
 	mov    %eax,-0x4(%rbp)
-	mov    -0x4(%rbp),%eax
-	lea    -0x1(%rax),%edx
+	mov    -0x4(%rbp),%edx
 	mov    -0x1c(%rbp),%ecx
 	mov    -0x18(%rbp),%rax
 	mov    %ecx,%esi
 	mov    %rax,%rdi
 	call   17f0 <quicksort2d@plt>
 	mov    -0x4(%rbp),%eax
 	lea    0x1(%rax),%ecx
@@ -4189,244 +3996,238 @@
 	mov    %ecx,%esi
 	mov    %rax,%rdi
 	call   17f0 <quicksort2d@plt>
 	nop
 	leave
 	ret
 
-00000000000058b6 <variogram>:
+00000000000055d2 <variogram>:
 variogram():
 	push   %rbp
 	mov    %rsp,%rbp
 	push   %rbx
-	sub    $0x98,%rsp
-	mov    %rdi,-0x88(%rbp)
-	mov    %rsi,-0x90(%rbp)
-	mov    %edx,-0x94(%rbp)
-	mov    %ecx,-0x98(%rbp)
-	mov    %r8d,-0x9c(%rbp)
+	sub    $0xb8,%rsp
+	mov    %rdi,-0xa8(%rbp)
+	mov    %rsi,-0xb0(%rbp)
+	mov    %edx,-0xb4(%rbp)
+	mov    %ecx,-0xb8(%rbp)
+	mov    %r8d,-0xbc(%rbp)
 	mov    %fs:0x28,%rax
 	mov    %rax,-0x18(%rbp)
 	xor    %eax,%eax
-	mov    -0x94(%rbp),%eax
+	mov    -0xb4(%rbp),%eax
 	cltq
 	mov    %rax,-0x28(%rbp)
-	mov    -0x94(%rbp),%eax
+	mov    -0xb4(%rbp),%eax
 	cltq
 	mov    %rax,-0x20(%rbp)
-	mov    -0x94(%rbp),%eax
+	mov    -0xb4(%rbp),%eax
 	cltq
 	shl    $0x3,%rax
 	mov    %rax,%rdi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,-0x30(%rbp)
-	movl   $0x0,-0x74(%rbp)
-	jmp    5958 <variogram+0xa2>
-	mov    -0x94(%rbp),%eax
+	movl   $0x0,-0x9c(%rbp)
+	jmp    567d <variogram+0xab>
+	mov    -0xb4(%rbp),%eax
 	cltq
 	shl    $0x3,%rax
 	mov    -0x30(%rbp),%rdx
-	mov    -0x74(%rbp),%ecx
+	mov    -0x9c(%rbp),%ecx
 	movslq %ecx,%rcx
 	shl    $0x3,%rcx
 	lea    (%rdx,%rcx,1),%rbx
 	mov    %rax,%rdi
-	call   1980 <malloc@plt>
+	call   1970 <malloc@plt>
 	mov    %rax,(%rbx)
-	addl   $0x1,-0x74(%rbp)
-	mov    -0x74(%rbp),%eax
-	cmp    -0x94(%rbp),%eax
-	jl     592b <variogram+0x75>
-	mov    -0x94(%rbp),%eax
+	addl   $0x1,-0x9c(%rbp)
+	mov    -0x9c(%rbp),%eax
+	cmp    -0xb4(%rbp),%eax
+	jl     564a <variogram+0x78>
+	mov    -0xb4(%rbp),%eax
 	mov    %eax,%edi
 	call   18d0 <d_arange@plt>
 	mov    %rax,-0x50(%rbp)
 	mov    -0x30(%rbp),%rcx
 	mov    -0x50(%rbp),%rax
-	mov    -0x94(%rbp),%edx
+	mov    -0xb4(%rbp),%edx
 	mov    %rcx,%rsi
 	mov    %rax,%rdi
 	call   1a60 <pdist@plt>
-	movl   $0x0,-0x70(%rbp)
-	jmp    5b19 <variogram+0x263>
+	movl   $0x0,-0x98(%rbp)
+	jmp    5875 <variogram+0x2a3>
 	pxor   %xmm0,%xmm0
-	movsd  %xmm0,-0x60(%rbp)
+	movsd  %xmm0,-0x88(%rbp)
 	pxor   %xmm0,%xmm0
-	movsd  %xmm0,-0x58(%rbp)
-	movl   $0x0,-0x6c(%rbp)
-	jmp    5ac1 <variogram+0x20b>
-	mov    -0x6c(%rbp),%eax
-	add    $0x1,%eax
-	mov    %eax,-0x68(%rbp)
-	jmp    5aae <variogram+0x1f8>
-	mov    -0x30(%rbp),%rax
-	mov    -0x6c(%rbp),%edx
-	movslq %edx,%rdx
-	shl    $0x3,%rdx
-	add    %rdx,%rax
-	mov    (%rax),%rax
-	mov    -0x68(%rbp),%edx
-	movslq %edx,%rdx
-	shl    $0x3,%rdx
-	add    %rdx,%rax
-	movsd  (%rax),%xmm1
-	mov    -0x70(%rbp),%eax
-	sub    -0x9c(%rbp),%eax
+	movsd  %xmm0,-0x80(%rbp)
+	mov    -0x98(%rbp),%eax
+	sub    -0xbc(%rbp),%eax
 	cvtsi2sd %eax,%xmm0
-	ucomisd %xmm0,%xmm1
-	jb     5aaa <variogram+0x1f4>
+	movsd  %xmm0,-0x78(%rbp)
+	mov    -0x98(%rbp),%edx
+	mov    -0xbc(%rbp),%eax
+	add    %edx,%eax
+	cvtsi2sd %eax,%xmm0
+	movsd  %xmm0,-0x70(%rbp)
+	movl   $0x0,-0x94(%rbp)
+	jmp    580e <variogram+0x23c>
+	mov    -0x94(%rbp),%eax
+	cltq
+	lea    0x0(,%rax,8),%rdx
+	mov    -0xa8(%rbp),%rax
+	add    %rdx,%rax
+	movsd  (%rax),%xmm0
+	movsd  %xmm0,-0x68(%rbp)
+	movl   $0x0,-0x90(%rbp)
+	jmp    57f5 <variogram+0x223>
 	mov    -0x30(%rbp),%rax
-	mov    -0x6c(%rbp),%edx
+	mov    -0x94(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
-	mov    -0x68(%rbp),%edx
+	mov    -0x90(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
-	movsd  (%rax),%xmm1
-	mov    -0x70(%rbp),%edx
-	mov    -0x9c(%rbp),%eax
-	add    %edx,%eax
-	cvtsi2sd %eax,%xmm0
-	ucomisd %xmm1,%xmm0
-	jb     5aaa <variogram+0x1f4>
-	mov    -0x6c(%rbp),%eax
-	cltq
-	lea    0x0(,%rax,8),%rdx
-	mov    -0x88(%rbp),%rax
-	add    %rdx,%rax
 	movsd  (%rax),%xmm0
-	mov    -0x68(%rbp),%eax
+	movsd  %xmm0,-0x60(%rbp)
+	movsd  -0x60(%rbp),%xmm0
+	ucomisd -0x78(%rbp),%xmm0
+	jb     57ee <variogram+0x21c>
+	movsd  -0x70(%rbp),%xmm0
+	ucomisd -0x60(%rbp),%xmm0
+	jb     57ee <variogram+0x21c>
+	mov    -0x90(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x88(%rbp),%rax
+	mov    -0xa8(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm1
+	movsd  -0x68(%rbp),%xmm0
 	subsd  %xmm1,%xmm0
-	movsd  0x38b(%rip),%xmm1        
-	call   1a20 <pow@plt>
-	movapd %xmm0,%xmm1
-	movsd  -0x60(%rbp),%xmm0
+	movsd  %xmm0,-0x58(%rbp)
+	movsd  -0x58(%rbp),%xmm0
+	mulsd  -0x58(%rbp),%xmm0
+	movsd  -0x88(%rbp),%xmm1
 	addsd  %xmm1,%xmm0
-	movsd  %xmm0,-0x60(%rbp)
-	movsd  -0x58(%rbp),%xmm1
-	movsd  0x36f(%rip),%xmm0        
+	movsd  %xmm0,-0x88(%rbp)
+	movsd  -0x80(%rbp),%xmm1
+	movsd  0x373(%rip),%xmm0        
 	addsd  %xmm1,%xmm0
-	movsd  %xmm0,-0x58(%rbp)
-	addl   $0x1,-0x68(%rbp)
-	mov    -0x68(%rbp),%eax
-	cmp    -0x94(%rbp),%eax
-	jl     59c5 <variogram+0x10f>
-	addl   $0x1,-0x6c(%rbp)
-	mov    -0x6c(%rbp),%eax
+	movsd  %xmm0,-0x80(%rbp)
+	addl   $0x1,-0x90(%rbp)
+	mov    -0x90(%rbp),%eax
 	cmp    -0x94(%rbp),%eax
-	jl     59b7 <variogram+0x101>
-	movsd  -0x60(%rbp),%xmm0
-	ucomisd 0x33b(%rip),%xmm0        
-	jb     5b10 <variogram+0x25a>
-	movsd  -0x58(%rbp),%xmm0
+	jl     5746 <variogram+0x174>
+	addl   $0x1,-0x94(%rbp)
+	mov    -0x94(%rbp),%eax
+	cmp    -0xb4(%rbp),%eax
+	jl     5714 <variogram+0x142>
+	movsd  -0x88(%rbp),%xmm0
+	ucomisd 0x330(%rip),%xmm0        
+	jb     5869 <variogram+0x297>
+	movsd  -0x80(%rbp),%xmm0
 	addsd  %xmm0,%xmm0
-	mov    -0x70(%rbp),%eax
+	mov    -0x98(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
-	mov    -0x90(%rbp),%rax
+	mov    -0xb0(%rbp),%rax
 	add    %rdx,%rax
-	movsd  -0x60(%rbp),%xmm1
+	movsd  -0x88(%rbp),%xmm1
 	divsd  %xmm0,%xmm1
 	movapd %xmm1,%xmm0
 	movsd  %xmm0,(%rax)
-	mov    -0x9c(%rbp),%eax
-	add    %eax,-0x70(%rbp)
-	mov    -0x70(%rbp),%eax
-	cmp    -0x98(%rbp),%eax
-	jl     5999 <variogram+0xe3>
+	mov    -0xbc(%rbp),%eax
+	add    %eax,-0x98(%rbp)
+	mov    -0x98(%rbp),%eax
+	cmp    -0xb8(%rbp),%eax
+	jl     56c4 <variogram+0xf2>
 	mov    -0x50(%rbp),%rax
 	mov    %rax,%rdi
 	call   17d0 <free@plt>
-	movl   $0x0,-0x64(%rbp)
-	jmp    5b5d <variogram+0x2a7>
+	movl   $0x0,-0x8c(%rbp)
+	jmp    58c5 <variogram+0x2f3>
 	mov    -0x30(%rbp),%rax
-	mov    -0x64(%rbp),%edx
+	mov    -0x8c(%rbp),%edx
 	movslq %edx,%rdx
 	shl    $0x3,%rdx
 	add    %rdx,%rax
 	mov    (%rax),%rax
 	mov    %rax,%rdi
 	call   17d0 <free@plt>
-	addl   $0x1,-0x64(%rbp)
-	mov    -0x64(%rbp),%eax
+	addl   $0x1,-0x8c(%rbp)
+	mov    -0x8c(%rbp),%eax
 	movslq %eax,%rdx
 	mov    -0x28(%rbp),%rax
 	cmp    %rax,%rdx
-	jb     5b3d <variogram+0x287>
+	jb     589f <variogram+0x2cd>
 	mov    -0x30(%rbp),%rax
 	mov    %rax,%rdi
 	call   17d0 <free@plt>
 	nop
 	mov    -0x18(%rbp),%rax
 	xor    %fs:0x28,%rax
-	je     5b8d <variogram+0x2d7>
+	je     58f8 <variogram+0x326>
 	call   1860 <__stack_chk_fail@plt>
-	add    $0x98,%rsp
+	add    $0xb8,%rsp
 	pop    %rbx
 	pop    %rbp
 	ret
 
-0000000000005b97 <variance>:
+0000000000005902 <variance>:
 variance():
 	push   %rbp
 	mov    %rsp,%rbp
 	sub    $0x30,%rsp
 	mov    %rdi,-0x28(%rbp)
 	mov    %esi,-0x2c(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x10(%rbp)
 	pxor   %xmm0,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movl   $0x0,-0x18(%rbp)
-	jmp    5beb <variance+0x54>
+	jmp    5956 <variance+0x54>
 	mov    -0x18(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	movsd  -0x10(%rbp),%xmm1
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x10(%rbp)
 	addl   $0x1,-0x18(%rbp)
 	mov    -0x18(%rbp),%eax
 	cmp    -0x2c(%rbp),%eax
-	jl     5bc1 <variance+0x2a>
+	jl     592c <variance+0x2a>
 	cvtsi2sdl -0x2c(%rbp),%xmm0
 	movsd  -0x10(%rbp),%xmm1
 	divsd  %xmm0,%xmm1
 	movapd %xmm1,%xmm0
 	movsd  %xmm0,-0x10(%rbp)
 	movl   $0x0,-0x14(%rbp)
-	jmp    5c53 <variance+0xbc>
+	jmp    59be <variance+0xbc>
 	mov    -0x14(%rbp),%eax
 	cltq
 	lea    0x0(,%rax,8),%rdx
 	mov    -0x28(%rbp),%rax
 	add    %rdx,%rax
 	movsd  (%rax),%xmm0
 	subsd  -0x10(%rbp),%xmm0
-	movsd  0x1d0(%rip),%xmm1        
+	movsd  0x1c5(%rip),%xmm1        
 	call   1a20 <pow@plt>
 	movapd %xmm0,%xmm1
 	movsd  -0x8(%rbp),%xmm0
 	addsd  %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	addl   $0x1,-0x14(%rbp)
 	mov    -0x14(%rbp),%eax
 	cmp    -0x2c(%rbp),%eax
-	jl     5c13 <variance+0x7c>
+	jl     597e <variance+0x7c>
 	cvtsi2sdl -0x2c(%rbp),%xmm0
 	movsd  -0x8(%rbp),%xmm1
 	divsd  %xmm0,%xmm1
 	movapd %xmm1,%xmm0
 	movsd  %xmm0,-0x8(%rbp)
 	movsd  -0x8(%rbp),%xmm0
 	leave
```

#### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.fini {}

```diff
@@ -1,10 +1,10 @@
 
 
 
 Disassembly of section .fini:
 
-0000000000005c7c <_fini>:
+00000000000059e4 <_fini>:
 _fini():
 	sub    $0x8,%rsp
 	add    $0x8,%rsp
 	ret
```

#### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,28 +1,27 @@
 
 Hex dump of section '.rodata':
-  0x00005c90 6d696e00 6d617800 000080cb ffff7f4b min.max........K
-  0x00005ca0 00000000 000070c3 00000000 00007043 ......p.......pC
-  0x00005cb0 00000000 00000040 0000804f 00000000 .......@...O....
-  0x00005cc0 00000000 0000f041 00000000 000000c0 .......A........
-  0x00005cd0 182d4454 fb211940 00000000 000008c0 .-DT.!.@........
-  0x00005ce0 00000000 0000f03f 00000000 00000000 .......?........
-  0x00005cf0 00000000 0000e03f 00000000 00000000 .......?........
-  0x00005d00 ffffffff ffffff7f 00000000 00000000 ................
-  0x00005d10 83c0caa1 45b6fb3f 00000000 00000000 ....E..?........
-  0x00005d20 25732573 25253025 64642e74 78740046 %s%s%%0%dd.txt.F
-  0x00005d30 6f6c6465 7220616c 72656164 79206578 older already ex
-  0x00005d40 69737421 00770046 61696c65 6420746f ist!.w.Failed to
-  0x00005d50 206f7065 6e207468 65206669 6c650025  open the file.%
-  0x00005d60 6409252e 3130660a 00000000 00000000 d.%.10f.........
-  0x00005d70 00000000 0000f03f 00000000 00000000 .......?........
-  0x00005d80 ffffffff ffffff7f 00000000 00000000 ................
-  0x00005d90 4e756d62 6572203d 2025640a 002e2f52 Number = %d.../R
-  0x00005da0 65616c69 7a617469 6f6e732f 00526561 ealizations/.Rea
-  0x00005db0 6c697a61 74696f6e 73002e2f 5265616c lizations../Real
-  0x00005dc0 697a6174 696f6e73 2f566172 696f6772 izations/Variogr
-  0x00005dd0 616d2f00 56617269 6f677261 6d000000 am/.Variogram...
-  0x00005de0 00000000 0000f0bf 00000000 00000000 ................
-  0x00005df0 ffffffff ffffff7f 00000000 00000000 ................
-  0x00005e00 ffffffff ffffef7f 00000000 00000040 ...............@
-  0x00005e10 00000000 0000f03f 8dedb5a0 f7c6b03e .......?.......>
+  0x000059f0 6d696e00 6d617800 000080cb ffff7f4b min.max........K
+  0x00005a00 00000000 000070c3 00000000 00007043 ......p.......pC
+  0x00005a10 00000000 00000040 0000804f 00000000 .......@...O....
+  0x00005a20 00000000 0000f041 00000000 000000c0 .......A........
+  0x00005a30 182d4454 fb211940 00000000 000008c0 .-DT.!.@........
+  0x00005a40 00000000 0000f03f 00000000 00000000 .......?........
+  0x00005a50 00000000 0000e03f 00000000 00000000 .......?........
+  0x00005a60 ffffffff ffffff7f 00000000 00000000 ................
+  0x00005a70 83c0caa1 45b6fb3f 00000000 00000000 ....E..?........
+  0x00005a80 25732573 25253025 64642e74 78740046 %s%s%%0%dd.txt.F
+  0x00005a90 6f6c6465 7220616c 72656164 79206578 older already ex
+  0x00005aa0 69737421 00770046 61696c65 6420746f ist!.w.Failed to
+  0x00005ab0 206f7065 6e207468 65206669 6c650025  open the file.%
+  0x00005ac0 6409252e 3130660a 00000000 00000000 d.%.10f.........
+  0x00005ad0 00000000 0000f03f 00000000 00000000 .......?........
+  0x00005ae0 ffffffff ffffff7f 00000000 00000000 ................
+  0x00005af0 4e756d62 6572203d 2025640a 002e2f52 Number = %d.../R
+  0x00005b00 65616c69 7a617469 6f6e732f 00526561 ealizations/.Rea
+  0x00005b10 6c697a61 74696f6e 73002e2f 5265616c lizations../Real
+  0x00005b20 697a6174 696f6e73 2f566172 696f6772 izations/Variogr
+  0x00005b30 616d2f00 56617269 6f677261 6d000000 am/.Variogram...
+  0x00005b40 ffffffff ffffff7f 00000000 00000000 ................
+  0x00005b50 ffffffff ffffef7f 00000000 0000f03f ...............?
+  0x00005b60 8dedb5a0 f7c6b03e 00000000 00000040 .......>.......@
```

#### readelf --wide --decompress --hex-dump=.eh_frame_hdr {}

```diff
@@ -1,36 +1,36 @@
 
 Hex dump of section '.eh_frame_hdr':
-  0x00005e20 011b033b 0c020000 40000000 a0b9ffff ...;....@.......
-  0x00005e30 28020000 70bcffff 50020000 5abdffff (...p...P...Z...
-  0x00005e40 68020000 e5beffff 88020000 9ec0ffff h...............
-  0x00005e50 a8020000 74c2ffff c8020000 4fc4ffff ....t.......O...
-  0x00005e60 e8020000 f2c5ffff 08030000 c4c7ffff ................
-  0x00005e70 28030000 b4c9ffff 48030000 a9cbffff (.......H.......
-  0x00005e80 68030000 2dccffff 88030000 b3ccffff h...-...........
-  0x00005e90 a8030000 39cdffff c8030000 bbcdffff ....9...........
-  0x00005ea0 e8030000 52ceffff 08040000 ebceffff ....R...........
-  0x00005eb0 28040000 84cfffff 48040000 19d0ffff (.......H.......
-  0x00005ec0 68040000 41d0ffff 88040000 6bd0ffff h...A.......k...
-  0x00005ed0 a8040000 95d0ffff c8040000 c3d0ffff ................
-  0x00005ee0 e8040000 08d1ffff 08050000 51d1ffff ............Q...
-  0x00005ef0 28050000 a7d1ffff 48050000 fdd1ffff (.......H.......
-  0x00005f00 68050000 1bd2ffff 88050000 3dd2ffff h...........=...
-  0x00005f10 a8050000 8fd2ffff c8050000 e3d2ffff ................
-  0x00005f20 e8050000 5cd3ffff 08060000 3fd5ffff ....\.......?...
-  0x00005f30 28060000 83d5ffff 48060000 cad5ffff (.......H.......
-  0x00005f40 68060000 31d6ffff 88060000 78d6ffff h...1.......x...
-  0x00005f50 a8060000 e0d6ffff c8060000 69d7ffff ............i...
-  0x00005f60 e8060000 d6d7ffff 08070000 dbd8ffff ................
-  0x00005f70 28070000 27daffff 48070000 d8daffff (...'...H.......
-  0x00005f80 68070000 03dbffff 88070000 5dddffff h...........]...
-  0x00005f90 ac070000 5de1ffff cc070000 10e3ffff ....]...........
-  0x00005fa0 ec070000 5ce4ffff 10080000 dde8ffff ....\...........
-  0x00005fb0 34080000 7eecffff 54080000 d2ecffff 4...~...T.......
-  0x00005fc0 74080000 2aedffff 94080000 d5edffff t...*...........
-  0x00005fd0 b4080000 5ceeffff d4080000 28f0ffff ....\.......(...
-  0x00005fe0 f8080000 e2f0ffff 18090000 4ff1ffff ............O...
-  0x00005ff0 38090000 3ef6ffff 58090000 5df6ffff 8...>...X...]...
-  0x00006000 78090000 aff6ffff 98090000 38f8ffff x...........8...
-  0x00006010 b8090000 34faffff d8090000 96faffff ....4...........
-  0x00006020 f8090000 77fdffff 1c0a0000          ....w.......
+  0x00005b70 011b033b 0c020000 40000000 50bcffff ...;....@...P...
+  0x00005b80 28020000 20bfffff 50020000 0ac0ffff (... ...P.......
+  0x00005b90 68020000 95c1ffff 88020000 4ec3ffff h...........N...
+  0x00005ba0 a8020000 24c5ffff c8020000 ffc6ffff ....$...........
+  0x00005bb0 e8020000 a2c8ffff 08030000 74caffff ............t...
+  0x00005bc0 28030000 64ccffff 48030000 59ceffff (...d...H...Y...
+  0x00005bd0 68030000 ddceffff 88030000 63cfffff h...........c...
+  0x00005be0 a8030000 e9cfffff c8030000 6bd0ffff ............k...
+  0x00005bf0 e8030000 02d1ffff 08040000 9bd1ffff ................
+  0x00005c00 28040000 34d2ffff 48040000 c9d2ffff (...4...H.......
+  0x00005c10 68040000 f1d2ffff 88040000 1bd3ffff h...............
+  0x00005c20 a8040000 45d3ffff c8040000 73d3ffff ....E.......s...
+  0x00005c30 e8040000 b8d3ffff 08050000 01d4ffff ................
+  0x00005c40 28050000 57d4ffff 48050000 add4ffff (...W...H.......
+  0x00005c50 68050000 cbd4ffff 88050000 edd4ffff h...............
+  0x00005c60 a8050000 3fd5ffff c8050000 93d5ffff ....?...........
+  0x00005c70 e8050000 0cd6ffff 08060000 efd7ffff ................
+  0x00005c80 28060000 33d8ffff 48060000 7ad8ffff (...3...H...z...
+  0x00005c90 68060000 e1d8ffff 88060000 28d9ffff h...........(...
+  0x00005ca0 a8060000 90d9ffff c8060000 19daffff ................
+  0x00005cb0 e8060000 86daffff 08070000 8bdbffff ................
+  0x00005cc0 28070000 d7dcffff 48070000 88ddffff (.......H.......
+  0x00005cd0 68070000 b3ddffff 88070000 0de0ffff h...............
+  0x00005ce0 ac070000 0de4ffff cc070000 c0e5ffff ................
+  0x00005cf0 ec070000 0ce7ffff 10080000 8debffff ................
+  0x00005d00 34080000 2eefffff 54080000 82efffff 4.......T.......
+  0x00005d10 74080000 daefffff 94080000 85f0ffff t...............
+  0x00005d20 b4080000 0cf1ffff d4080000 d8f2ffff ................
+  0x00005d30 f8080000 92f3ffff 18090000 00f4ffff ................
+  0x00005d40 38090000 5af8ffff 58090000 79f8ffff 8...Z...X...y...
+  0x00005d50 78090000 cbf8ffff 98090000 41f9ffff x...........A...
+  0x00005d60 b8090000 03faffff d8090000 62faffff ............b...
+  0x00005d70 f8090000 92fdffff 1c0a0000          ............
```

#### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,134 +1,134 @@
 
 Hex dump of section '.eh_frame':
-  0x00006030 14000000 00000000 017a5200 01781001 .........zR..x..
-  0x00006040 1b0c0708 90010000 24000000 1c000000 ........$.......
-  0x00006050 70b7ffff d0020000 000e1046 0e184a0f p..........F..J.
-  0x00006060 0b770880 003f1a3b 2a332422 00000000 .w...?.;*3$"....
-  0x00006070 14000000 44000000 18baffff 08000000 ....D...........
-  0x00006080 00000000 00000000 1c000000 5c000000 ............\...
-  0x00006090 eabaffff 8b010000 00410e10 8602430d .........A....C.
-  0x000060a0 06038601 0c070800 1c000000 7c000000 ............|...
-  0x000060b0 55bcffff b9010000 00410e10 8602430d U........A....C.
-  0x000060c0 0603b401 0c070800 1c000000 9c000000 ................
-  0x000060d0 eebdffff d6010000 00410e10 8602430d .........A....C.
-  0x000060e0 0603d101 0c070800 1c000000 bc000000 ................
-  0x000060f0 a4bfffff db010000 00410e10 8602430d .........A....C.
-  0x00006100 0603d601 0c070800 1c000000 dc000000 ................
-  0x00006110 5fc1ffff a3010000 00410e10 8602430d _........A....C.
-  0x00006120 06039e01 0c070800 1c000000 fc000000 ................
-  0x00006130 e2c2ffff d2010000 00410e10 8602430d .........A....C.
-  0x00006140 0603cd01 0c070800 1c000000 1c010000 ................
-  0x00006150 94c4ffff f0010000 00410e10 8602430d .........A....C.
-  0x00006160 0603eb01 0c070800 1c000000 3c010000 ............<...
-  0x00006170 64c6ffff f5010000 00410e10 8602430d d........A....C.
-  0x00006180 0603f001 0c070800 1c000000 5c010000 ............\...
-  0x00006190 39c8ffff 84000000 00410e10 8602430d 9........A....C.
-  0x000061a0 06027f0c 07080000 1c000000 7c010000 ............|...
-  0x000061b0 9dc8ffff 86000000 00410e10 8602430d .........A....C.
-  0x000061c0 0602810c 07080000 1c000000 9c010000 ................
-  0x000061d0 03c9ffff 86000000 00410e10 8602430d .........A....C.
-  0x000061e0 0602810c 07080000 1c000000 bc010000 ................
-  0x000061f0 69c9ffff 82000000 00410e10 8602430d i........A....C.
-  0x00006200 06027d0c 07080000 1c000000 dc010000 ..}.............
-  0x00006210 cbc9ffff 97000000 00410e10 8602430d .........A....C.
-  0x00006220 0602920c 07080000 1c000000 fc010000 ................
-  0x00006230 42caffff 99000000 00410e10 8602430d B........A....C.
-  0x00006240 0602940c 07080000 1c000000 1c020000 ................
-  0x00006250 bbcaffff 99000000 00410e10 8602430d .........A....C.
-  0x00006260 0602940c 07080000 1c000000 3c020000 ............<...
-  0x00006270 34cbffff 95000000 00410e10 8602430d 4........A....C.
-  0x00006280 0602900c 07080000 1c000000 5c020000 ............\...
-  0x00006290 a9cbffff 28000000 00410e10 8602430d ....(....A....C.
-  0x000062a0 06630c07 08000000 1c000000 7c020000 .c..........|...
-  0x000062b0 b1cbffff 2a000000 00410e10 8602430d ....*....A....C.
-  0x000062c0 06650c07 08000000 1c000000 9c020000 .e..............
-  0x000062d0 bbcbffff 2a000000 00410e10 8602430d ....*....A....C.
-  0x000062e0 06650c07 08000000 1c000000 bc020000 .e..............
-  0x000062f0 c5cbffff 2e000000 00410e10 8602430d .........A....C.
-  0x00006300 06690c07 08000000 1c000000 dc020000 .i..............
-  0x00006310 d3cbffff 45000000 00410e10 8602430d ....E....A....C.
-  0x00006320 0602400c 07080000 1c000000 fc020000 ..@.............
-  0x00006330 f8cbffff 49000000 00410e10 8602430d ....I....A....C.
-  0x00006340 0602440c 07080000 1c000000 1c030000 ..D.............
-  0x00006350 21ccffff 56000000 00410e10 8602430d !...V....A....C.
-  0x00006360 0602510c 07080000 1c000000 3c030000 ..Q.........<...
-  0x00006370 57ccffff 56000000 00410e10 8602430d W...V....A....C.
-  0x00006380 0602510c 07080000 1c000000 5c030000 ..Q.........\...
-  0x00006390 8dccffff 1e000000 00410e10 8602430d .........A....C.
-  0x000063a0 06590c07 08000000 1c000000 7c030000 .Y..........|...
-  0x000063b0 8bccffff 22000000 00410e10 8602430d ...."....A....C.
-  0x000063c0 065d0c07 08000000 1c000000 9c030000 .]..............
-  0x000063d0 8dccffff 52000000 00410e10 8602430d ....R....A....C.
-  0x000063e0 06024d0c 07080000 1c000000 bc030000 ..M.............
-  0x000063f0 bfccffff 54000000 00410e10 8602430d ....T....A....C.
-  0x00006400 06024f0c 07080000 1c000000 dc030000 ..O.............
-  0x00006410 f3ccffff 79000000 00410e10 8602430d ....y....A....C.
-  0x00006420 0602740c 07080000 1c000000 fc030000 ..t.............
-  0x00006430 4ccdffff e3010000 00410e10 8602430d L........A....C.
-  0x00006440 0603de01 0c070800 1c000000 1c040000 ................
-  0x00006450 0fcfffff 44000000 00410e10 8602430d ....D....A....C.
-  0x00006460 067f0c07 08000000 1c000000 3c040000 ............<...
-  0x00006470 33cfffff 47000000 00410e10 8602430d 3...G....A....C.
-  0x00006480 0602420c 07080000 1c000000 5c040000 ..B.........\...
-  0x00006490 5acfffff 67000000 00410e10 8602430d Z...g....A....C.
-  0x000064a0 0602620c 07080000 1c000000 7c040000 ..b.........|...
-  0x000064b0 a1cfffff 47000000 00410e10 8602430d ....G....A....C.
-  0x000064c0 0602420c 07080000 1c000000 9c040000 ..B.............
-  0x000064d0 c8cfffff 68000000 00410e10 8602430d ....h....A....C.
-  0x000064e0 0602630c 07080000 1c000000 bc040000 ..c.............
-  0x000064f0 10d0ffff 89000000 00410e10 8602430d .........A....C.
-  0x00006500 0602840c 07080000 1c000000 dc040000 ................
-  0x00006510 79d0ffff 6d000000 00410e10 8602430d y...m....A....C.
-  0x00006520 0602680c 07080000 1c000000 fc040000 ..h.............
-  0x00006530 c6d0ffff 05010000 00410e10 8602430d .........A....C.
-  0x00006540 06030001 0c070800 1c000000 1c050000 ................
-  0x00006550 abd1ffff 4c010000 00410e10 8602430d ....L....A....C.
-  0x00006560 06034701 0c070800 1c000000 3c050000 ..G.........<...
-  0x00006570 d7d2ffff b1000000 00410e10 8602430d .........A....C.
-  0x00006580 0602ac0c 07080000 1c000000 5c050000 ............\...
-  0x00006590 68d3ffff 2b000000 00410e10 8602430d h...+....A....C.
-  0x000065a0 06660c07 08000000 20000000 7c050000 .f...... ...|...
-  0x000065b0 73d3ffff 5a020000 00410e10 8602430d s...Z....A....C.
-  0x000065c0 06458303 0350020c 07080000 1c000000 .E...P..........
-  0x000065d0 a0050000 a9d5ffff 00040000 00410e10 .............A..
-  0x000065e0 8602430d 0603fb03 0c070800 1c000000 ..C.............
-  0x000065f0 c0050000 89d9ffff b3010000 00410e10 .............A..
-  0x00006600 8602430d 0603ae01 0c070800 20000000 ..C......... ...
-  0x00006610 e0050000 1cdbffff 4c010000 00410e10 ........L....A..
-  0x00006620 8602430d 06034701 0c070800 00000000 ..C...G.........
-  0x00006630 20000000 04060000 44dcffff 81040000  .......D.......
-  0x00006640 00410e10 8602430d 06488303 0374040c .A....C..H...t..
-  0x00006650 07080000 1c000000 28060000 a1e0ffff ........(.......
-  0x00006660 a1030000 00410e10 8602430d 06039c03 .....A....C.....
-  0x00006670 0c070800 1c000000 48060000 22e4ffff ........H..."...
-  0x00006680 54000000 00410e10 8602430d 06024f0c T....A....C...O.
-  0x00006690 07080000 1c000000 68060000 56e4ffff ........h...V...
-  0x000066a0 58000000 00410e10 8602430d 0602530c X....A....C...S.
-  0x000066b0 07080000 1c000000 88060000 8ee4ffff ................
-  0x000066c0 ab000000 00410e10 8602430d 0602a60c .....A....C.....
-  0x000066d0 07080000 1c000000 a8060000 19e5ffff ................
-  0x000066e0 87000000 00410e10 8602430d 0602820c .....A....C.....
-  0x000066f0 07080000 20000000 c8060000 80e5ffff .... ...........
-  0x00006700 cc010000 00410e10 8602430d 0603c701 .....A....C.....
-  0x00006710 0c070800 00000000 1c000000 ec060000 ................
-  0x00006720 28e7ffff ba000000 00410e10 8602430d (........A....C.
-  0x00006730 0602b50c 07080000 1c000000 0c070000 ................
-  0x00006740 c2e7ffff 6d000000 00410e10 8602430d ....m....A....C.
-  0x00006750 0602680c 07080000 1c000000 2c070000 ..h.........,...
-  0x00006760 0fe8ffff ef040000 00410e10 8602430d .........A....C.
-  0x00006770 0603ea04 0c070800 1c000000 4c070000 ............L...
-  0x00006780 deecffff 1f000000 00410e10 8602430d .........A....C.
-  0x00006790 065a0c07 08000000 1c000000 6c070000 .Z..........l...
-  0x000067a0 ddecffff 52000000 00410e10 8602430d ....R....A....C.
-  0x000067b0 06024d0c 07080000 1c000000 8c070000 ..M.............
-  0x000067c0 0fedffff 89010000 00410e10 8602430d .........A....C.
-  0x000067d0 06038401 0c070800 1c000000 ac070000 ................
-  0x000067e0 78eeffff fc010000 00410e10 8602430d x........A....C.
-  0x000067f0 0603f701 0c070800 1c000000 cc070000 ................
-  0x00006800 54f0ffff 62000000 00410e10 8602430d T...b....A....C.
-  0x00006810 06025d0c 07080000 20000000 ec070000 ..]..... .......
-  0x00006820 96f0ffff e1020000 00410e10 8602430d .........A....C.
-  0x00006830 06488303 03d4020c 07080000 1c000000 .H..............
-  0x00006840 10080000 53f3ffff e2000000 00410e10 ....S........A..
-  0x00006850 8602430d 0602dd0c 07080000 00000000 ..C.............
+  0x00005d80 14000000 00000000 017a5200 01781001 .........zR..x..
+  0x00005d90 1b0c0708 90010000 24000000 1c000000 ........$.......
+  0x00005da0 20baffff d0020000 000e1046 0e184a0f  ..........F..J.
+  0x00005db0 0b770880 003f1a3b 2a332422 00000000 .w...?.;*3$"....
+  0x00005dc0 14000000 44000000 c8bcffff 08000000 ....D...........
+  0x00005dd0 00000000 00000000 1c000000 5c000000 ............\...
+  0x00005de0 9abdffff 8b010000 00410e10 8602430d .........A....C.
+  0x00005df0 06038601 0c070800 1c000000 7c000000 ............|...
+  0x00005e00 05bfffff b9010000 00410e10 8602430d .........A....C.
+  0x00005e10 0603b401 0c070800 1c000000 9c000000 ................
+  0x00005e20 9ec0ffff d6010000 00410e10 8602430d .........A....C.
+  0x00005e30 0603d101 0c070800 1c000000 bc000000 ................
+  0x00005e40 54c2ffff db010000 00410e10 8602430d T........A....C.
+  0x00005e50 0603d601 0c070800 1c000000 dc000000 ................
+  0x00005e60 0fc4ffff a3010000 00410e10 8602430d .........A....C.
+  0x00005e70 06039e01 0c070800 1c000000 fc000000 ................
+  0x00005e80 92c5ffff d2010000 00410e10 8602430d .........A....C.
+  0x00005e90 0603cd01 0c070800 1c000000 1c010000 ................
+  0x00005ea0 44c7ffff f0010000 00410e10 8602430d D........A....C.
+  0x00005eb0 0603eb01 0c070800 1c000000 3c010000 ............<...
+  0x00005ec0 14c9ffff f5010000 00410e10 8602430d .........A....C.
+  0x00005ed0 0603f001 0c070800 1c000000 5c010000 ............\...
+  0x00005ee0 e9caffff 84000000 00410e10 8602430d .........A....C.
+  0x00005ef0 06027f0c 07080000 1c000000 7c010000 ............|...
+  0x00005f00 4dcbffff 86000000 00410e10 8602430d M........A....C.
+  0x00005f10 0602810c 07080000 1c000000 9c010000 ................
+  0x00005f20 b3cbffff 86000000 00410e10 8602430d .........A....C.
+  0x00005f30 0602810c 07080000 1c000000 bc010000 ................
+  0x00005f40 19ccffff 82000000 00410e10 8602430d .........A....C.
+  0x00005f50 06027d0c 07080000 1c000000 dc010000 ..}.............
+  0x00005f60 7bccffff 97000000 00410e10 8602430d {........A....C.
+  0x00005f70 0602920c 07080000 1c000000 fc010000 ................
+  0x00005f80 f2ccffff 99000000 00410e10 8602430d .........A....C.
+  0x00005f90 0602940c 07080000 1c000000 1c020000 ................
+  0x00005fa0 6bcdffff 99000000 00410e10 8602430d k........A....C.
+  0x00005fb0 0602940c 07080000 1c000000 3c020000 ............<...
+  0x00005fc0 e4cdffff 95000000 00410e10 8602430d .........A....C.
+  0x00005fd0 0602900c 07080000 1c000000 5c020000 ............\...
+  0x00005fe0 59ceffff 28000000 00410e10 8602430d Y...(....A....C.
+  0x00005ff0 06630c07 08000000 1c000000 7c020000 .c..........|...
+  0x00006000 61ceffff 2a000000 00410e10 8602430d a...*....A....C.
+  0x00006010 06650c07 08000000 1c000000 9c020000 .e..............
+  0x00006020 6bceffff 2a000000 00410e10 8602430d k...*....A....C.
+  0x00006030 06650c07 08000000 1c000000 bc020000 .e..............
+  0x00006040 75ceffff 2e000000 00410e10 8602430d u........A....C.
+  0x00006050 06690c07 08000000 1c000000 dc020000 .i..............
+  0x00006060 83ceffff 45000000 00410e10 8602430d ....E....A....C.
+  0x00006070 0602400c 07080000 1c000000 fc020000 ..@.............
+  0x00006080 a8ceffff 49000000 00410e10 8602430d ....I....A....C.
+  0x00006090 0602440c 07080000 1c000000 1c030000 ..D.............
+  0x000060a0 d1ceffff 56000000 00410e10 8602430d ....V....A....C.
+  0x000060b0 0602510c 07080000 1c000000 3c030000 ..Q.........<...
+  0x000060c0 07cfffff 56000000 00410e10 8602430d ....V....A....C.
+  0x000060d0 0602510c 07080000 1c000000 5c030000 ..Q.........\...
+  0x000060e0 3dcfffff 1e000000 00410e10 8602430d =........A....C.
+  0x000060f0 06590c07 08000000 1c000000 7c030000 .Y..........|...
+  0x00006100 3bcfffff 22000000 00410e10 8602430d ;..."....A....C.
+  0x00006110 065d0c07 08000000 1c000000 9c030000 .]..............
+  0x00006120 3dcfffff 52000000 00410e10 8602430d =...R....A....C.
+  0x00006130 06024d0c 07080000 1c000000 bc030000 ..M.............
+  0x00006140 6fcfffff 54000000 00410e10 8602430d o...T....A....C.
+  0x00006150 06024f0c 07080000 1c000000 dc030000 ..O.............
+  0x00006160 a3cfffff 79000000 00410e10 8602430d ....y....A....C.
+  0x00006170 0602740c 07080000 1c000000 fc030000 ..t.............
+  0x00006180 fccfffff e3010000 00410e10 8602430d .........A....C.
+  0x00006190 0603de01 0c070800 1c000000 1c040000 ................
+  0x000061a0 bfd1ffff 44000000 00410e10 8602430d ....D....A....C.
+  0x000061b0 067f0c07 08000000 1c000000 3c040000 ............<...
+  0x000061c0 e3d1ffff 47000000 00410e10 8602430d ....G....A....C.
+  0x000061d0 0602420c 07080000 1c000000 5c040000 ..B.........\...
+  0x000061e0 0ad2ffff 67000000 00410e10 8602430d ....g....A....C.
+  0x000061f0 0602620c 07080000 1c000000 7c040000 ..b.........|...
+  0x00006200 51d2ffff 47000000 00410e10 8602430d Q...G....A....C.
+  0x00006210 0602420c 07080000 1c000000 9c040000 ..B.............
+  0x00006220 78d2ffff 68000000 00410e10 8602430d x...h....A....C.
+  0x00006230 0602630c 07080000 1c000000 bc040000 ..c.............
+  0x00006240 c0d2ffff 89000000 00410e10 8602430d .........A....C.
+  0x00006250 0602840c 07080000 1c000000 dc040000 ................
+  0x00006260 29d3ffff 6d000000 00410e10 8602430d )...m....A....C.
+  0x00006270 0602680c 07080000 1c000000 fc040000 ..h.............
+  0x00006280 76d3ffff 05010000 00410e10 8602430d v........A....C.
+  0x00006290 06030001 0c070800 1c000000 1c050000 ................
+  0x000062a0 5bd4ffff 4c010000 00410e10 8602430d [...L....A....C.
+  0x000062b0 06034701 0c070800 1c000000 3c050000 ..G.........<...
+  0x000062c0 87d5ffff b1000000 00410e10 8602430d .........A....C.
+  0x000062d0 0602ac0c 07080000 1c000000 5c050000 ............\...
+  0x000062e0 18d6ffff 2b000000 00410e10 8602430d ....+....A....C.
+  0x000062f0 06660c07 08000000 20000000 7c050000 .f...... ...|...
+  0x00006300 23d6ffff 5a020000 00410e10 8602430d #...Z....A....C.
+  0x00006310 06458303 0350020c 07080000 1c000000 .E...P..........
+  0x00006320 a0050000 59d8ffff 00040000 00410e10 ....Y........A..
+  0x00006330 8602430d 0603fb03 0c070800 1c000000 ..C.............
+  0x00006340 c0050000 39dcffff b3010000 00410e10 ....9........A..
+  0x00006350 8602430d 0603ae01 0c070800 20000000 ..C......... ...
+  0x00006360 e0050000 ccddffff 4c010000 00410e10 ........L....A..
+  0x00006370 8602430d 06034701 0c070800 00000000 ..C...G.........
+  0x00006380 20000000 04060000 f4deffff 81040000  ...............
+  0x00006390 00410e10 8602430d 06488303 0374040c .A....C..H...t..
+  0x000063a0 07080000 1c000000 28060000 51e3ffff ........(...Q...
+  0x000063b0 a1030000 00410e10 8602430d 06039c03 .....A....C.....
+  0x000063c0 0c070800 1c000000 48060000 d2e6ffff ........H.......
+  0x000063d0 54000000 00410e10 8602430d 06024f0c T....A....C...O.
+  0x000063e0 07080000 1c000000 68060000 06e7ffff ........h.......
+  0x000063f0 58000000 00410e10 8602430d 0602530c X....A....C...S.
+  0x00006400 07080000 1c000000 88060000 3ee7ffff ............>...
+  0x00006410 ab000000 00410e10 8602430d 0602a60c .....A....C.....
+  0x00006420 07080000 1c000000 a8060000 c9e7ffff ................
+  0x00006430 87000000 00410e10 8602430d 0602820c .....A....C.....
+  0x00006440 07080000 20000000 c8060000 30e8ffff .... .......0...
+  0x00006450 cc010000 00410e10 8602430d 0603c701 .....A....C.....
+  0x00006460 0c070800 00000000 1c000000 ec060000 ................
+  0x00006470 d8e9ffff ba000000 00410e10 8602430d .........A....C.
+  0x00006480 0602b50c 07080000 1c000000 0c070000 ................
+  0x00006490 72eaffff 6e000000 00410e10 8602430d r...n....A....C.
+  0x000064a0 0602690c 07080000 1c000000 2c070000 ..i.........,...
+  0x000064b0 c0eaffff 5a040000 00410e10 8602430d ....Z....A....C.
+  0x000064c0 06035504 0c070800 1c000000 4c070000 ..U.........L...
+  0x000064d0 faeeffff 1f000000 00410e10 8602430d .........A....C.
+  0x000064e0 065a0c07 08000000 1c000000 6c070000 .Z..........l...
+  0x000064f0 f9eeffff 52000000 00410e10 8602430d ....R....A....C.
+  0x00006500 06024d0c 07080000 1c000000 8c070000 ..M.............
+  0x00006510 2befffff 76000000 00410e10 8602430d +...v....A....C.
+  0x00006520 0602710c 07080000 1c000000 ac070000 ..q.............
+  0x00006530 81efffff c2000000 00410e10 8602430d .........A....C.
+  0x00006540 0602bd0c 07080000 1c000000 cc070000 ................
+  0x00006550 23f0ffff 5f000000 00410e10 8602430d #..._....A....C.
+  0x00006560 06025a0c 07080000 20000000 ec070000 ..Z..... .......
+  0x00006570 62f0ffff 30030000 00410e10 8602430d b...0....A....C.
+  0x00006580 06488303 0323030c 07080000 1c000000 .H...#..........
+  0x00006590 10080000 6ef3ffff e2000000 00410e10 ....n........A..
+  0x000065a0 8602430d 0602dd0c 07080000 00000000 ..C.............
```

#### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -60,49 +60,49 @@
   0x00000390 5f6d6561 6e5f696e 7400635f 61727261 _mean_int.c_arra
   0x000003a0 795f6d69 6e5f666c 6f617400 636f765f y_min_float.cov_
   0x000003b0 6d6f6465 6c326400 66696e64 5f6e6569 model2d.find_nei
   0x000003c0 6768626f 7200736e 7072696e 74664040 ghbor.snprintf@@
   0x000003d0 474c4942 435f322e 322e3500 636d7066 GLIBC_2.2.5.cmpf
   0x000003e0 756e635f 646f7562 6c65006c 755f6465 unc_double.lu_de
   0x000003f0 636f6d70 6f736974 696f6e00 645f6172 composition.d_ar
-  0x00000400 616e6765 00506172 74697469 6f6e3264 ange.Partition2d
-  0x00000410 006d7431 39393337 5f676574 5f666c6f .mt19937_get_flo
-  0x00000420 61745f72 616e6765 00636f76 5f6d6f64 at_range.cov_mod
-  0x00000430 656c006d 61747269 78666f72 6d006d74 el.matrixform.mt
-  0x00000440 31393933 375f6765 6e657261 74650063 19937_generate.c
-  0x00000450 5f617272 61795f6d 65616e5f 6c6f6e67 _array_mean_long
-  0x00000460 5f6c6f6e 67007661 7269616e 63650063 _long.variance.c
-  0x00000470 5f617272 61795f76 61725f6c 6f6e675f _array_var_long_
-  0x00000480 6c6f6e67 00635f61 72726179 5f737464 long.c_array_std
-  0x00000490 5f696e74 006d7431 39393337 5f72616e _int.mt19937_ran
-  0x000004a0 646f6d5f 6e6f726d 616c0063 616c6c6f dom_normal.callo
-  0x000004b0 63404047 4c494243 5f322e32 2e350063 c@@GLIBC_2.2.5.c
-  0x000004c0 5f617272 61795f6d 696e5f64 6f75626c _array_min_doubl
-  0x000004d0 6500636f 765f6d6f 64656c5f 696e6974 e.cov_model_init
-  0x000004e0 00667072 696e7466 4040474c 4942435f .fprintf@@GLIBC_
-  0x000004f0 322e322e 35007367 73696d5f 745f6672 2.2.5.sgsim_t_fr
-  0x00000500 6565005f 5f676d6f 6e5f7374 6172745f ee.__gmon_start_
-  0x00000510 5f00635f 61727261 795f6d69 6e5f696e _.c_array_min_in
-  0x00000520 7400635f 61727261 795f7374 645f646f t.c_array_std_do
-  0x00000530 75626c65 00635f61 72726179 5f6d6178 uble.c_array_max
-  0x00000540 5f696e74 006b7269 67655f70 6172616d _int.krige_param
-  0x00000550 5f736574 74696e67 00635f61 72726179 _setting.c_array
-  0x00000560 5f73756d 5f6c6f6e 67006d74 31393933 _sum_long.mt1993
-  0x00000570 375f696e 69740063 6d706675 6e635f66 7_init.cmpfunc_f
-  0x00000580 6c6f6174 0073696d 706c655f 6b726967 loat.simple_krig
-  0x00000590 696e6700 635f6172 7261795f 6d65616e ing.c_array_mean
-  0x000005a0 5f666c6f 6174006d 616c6c6f 63404047 _float.malloc@@G
-  0x000005b0 4c494243 5f322e32 2e35006b 72696765 LIBC_2.2.5.krige
-  0x000005c0 5f6d656d 6f72795f 66726565 00657870 _memory_free.exp
-  0x000005d0 005f656e 6400635f 61727261 795f7661 ._end.c_array_va
-  0x000005e0 725f666c 6f617400 5f5f6273 735f7374 r_float.__bss_st
-  0x000005f0 61727400 76617269 6f677261 6d00635f art.variogram.c_
-  0x00000600 61727261 795f6d61 785f646f 75626c65 array_max_double
-  0x00000610 00635f61 72726179 5f6d696e 5f6c6f6e .c_array_min_lon
-  0x00000620 675f6c6f 6e670063 6f73006d 74313939 g_long.cos.mt199
+  0x00000400 616e6765 006d7431 39393337 5f676574 ange.mt19937_get
+  0x00000410 5f666c6f 61745f72 616e6765 00636f76 _float_range.cov
+  0x00000420 5f6d6f64 656c006d 61747269 78666f72 _model.matrixfor
+  0x00000430 6d006d74 31393933 375f6765 6e657261 m.mt19937_genera
+  0x00000440 74650063 5f617272 61795f6d 65616e5f te.c_array_mean_
+  0x00000450 6c6f6e67 5f6c6f6e 67007661 7269616e long_long.varian
+  0x00000460 63650063 5f617272 61795f76 61725f6c ce.c_array_var_l
+  0x00000470 6f6e675f 6c6f6e67 00635f61 72726179 ong_long.c_array
+  0x00000480 5f737464 5f696e74 006d7431 39393337 _std_int.mt19937
+  0x00000490 5f72616e 646f6d5f 6e6f726d 616c0063 _random_normal.c
+  0x000004a0 616c6c6f 63404047 4c494243 5f322e32 alloc@@GLIBC_2.2
+  0x000004b0 2e350063 5f617272 61795f6d 696e5f64 .5.c_array_min_d
+  0x000004c0 6f75626c 6500636f 765f6d6f 64656c5f ouble.cov_model_
+  0x000004d0 696e6974 00667072 696e7466 4040474c init.fprintf@@GL
+  0x000004e0 4942435f 322e322e 35007367 73696d5f IBC_2.2.5.sgsim_
+  0x000004f0 745f6672 6565005f 5f676d6f 6e5f7374 t_free.__gmon_st
+  0x00000500 6172745f 5f00635f 61727261 795f6d69 art__.c_array_mi
+  0x00000510 6e5f696e 7400635f 61727261 795f7374 n_int.c_array_st
+  0x00000520 645f646f 75626c65 00635f61 72726179 d_double.c_array
+  0x00000530 5f6d6178 5f696e74 006b7269 67655f70 _max_int.krige_p
+  0x00000540 6172616d 5f736574 74696e67 00635f61 aram_setting.c_a
+  0x00000550 72726179 5f73756d 5f6c6f6e 67006d74 rray_sum_long.mt
+  0x00000560 31393933 375f696e 69740063 6d706675 19937_init.cmpfu
+  0x00000570 6e635f66 6c6f6174 0073696d 706c655f nc_float.simple_
+  0x00000580 6b726967 696e6700 635f6172 7261795f kriging.c_array_
+  0x00000590 6d65616e 5f666c6f 6174006d 616c6c6f mean_float.mallo
+  0x000005a0 63404047 4c494243 5f322e32 2e35006b c@@GLIBC_2.2.5.k
+  0x000005b0 72696765 5f6d656d 6f72795f 66726565 rige_memory_free
+  0x000005c0 00657870 005f656e 6400635f 61727261 .exp._end.c_arra
+  0x000005d0 795f7661 725f666c 6f617400 5f5f6273 y_var_float.__bs
+  0x000005e0 735f7374 61727400 76617269 6f677261 s_start.variogra
+  0x000005f0 6d00635f 61727261 795f6d61 785f646f m.c_array_max_do
+  0x00000600 75626c65 00635f61 72726179 5f6d696e uble.c_array_min
+  0x00000610 5f6c6f6e 675f6c6f 6e670063 6f730070 _long_long.cos.p
+  0x00000620 61727469 74696f6e 3264006d 74313939 artition2d.mt199
   0x00000630 33375f67 65745f69 6e743332 5f72616e 37_get_int32_ran
   0x00000640 67650073 616d706c 696e675f 73746174 ge.sampling_stat
   0x00000650 655f696e 6974006d 74313939 33375f67 e_init.mt19937_g
   0x00000660 65745f64 6f75626c 655f7261 6e676500 et_double_range.
   0x00000670 73677369 6d5f696e 6974006c 6f670066 sgsim_init.log.f
   0x00000680 6f70656e 4040474c 4942435f 322e322e open@@GLIBC_2.2.
   0x00000690 35006d74 31393933 375f6765 745f646f 5.mt19937_get_do
@@ -110,16 +110,17 @@
   0x000006b0 40474c49 42435f32 2e322e35 006d7431 @GLIBC_2.2.5.mt1
   0x000006c0 39393337 5f676574 5f666c6f 6174006c 9937_get_float.l
   0x000006d0 6f673130 00737172 7400636d 7066756e og10.sqrt.cmpfun
   0x000006e0 635f6c6f 6e670070 64697374 00635f61 c_long.pdist.c_a
   0x000006f0 72726179 5f737464 5f6c6f6e 675f6c6f rray_std_long_lo
   0x00000700 6e670065 78697440 40474c49 42435f32 ng.exit@@GLIBC_2
   0x00000710 2e322e35 005f4954 4d5f7265 67697374 .2.5._ITM_regist
-  0x00000720 6572544d 436c6f6e 65546162 6c650073 erTMCloneTable.s
-  0x00000730 77617000 635f6172 7261795f 6d65616e wap.c_array_mean
-  0x00000740 5f646f75 626c6500 635f6172 7261795f _double.c_array_
-  0x00000750 7374645f 666c6f61 7400635f 61727261 std_float.c_arra
-  0x00000760 795f6d61 785f6c6f 6e675f6c 6f6e6700 y_max_long_long.
-  0x00000770 635f6172 7261795f 73756d5f 646f7562 c_array_sum_doub
-  0x00000780 6c65005f 5f637861 5f66696e 616c697a le.__cxa_finaliz
-  0x00000790 65404047 4c494243 5f322e32 2e3500   e@@GLIBC_2.2.5.
+  0x00000720 6572544d 436c6f6e 65546162 6c650063 erTMCloneTable.c
+  0x00000730 5f617272 61795f6d 65616e5f 646f7562 _array_mean_doub
+  0x00000740 6c650063 5f617272 61795f73 74645f66 le.c_array_std_f
+  0x00000750 6c6f6174 00635f61 72726179 5f6d6178 loat.c_array_max
+  0x00000760 5f6c6f6e 675f6c6f 6e670063 5f617272 _long_long.c_arr
+  0x00000770 61795f73 756d5f64 6f75626c 65005f5f ay_sum_double.__
+  0x00000780 6378615f 66696e61 6c697a65 4040474c cxa_finalize@@GL
+  0x00000790 4942435f 322e322e 35007377 6170726f IBC_2.2.5.swapro
+  0x000007a0 777300                              ws.
```

### Comparing `uc_sgsim-1.2.1/uc_sgsim/cov_model/base.py` & `uc_sgsim-1.2.2/uc_sgsim/cov_model/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-from scipy.spatial.distance import pdist, squareform
+from scipy.spatial.distance import cdist
 
 
 class CovModel:
     def __init__(
         self,
         bandwidth_len: float,
         bandwidth_step: float,
@@ -53,22 +53,21 @@
         var = np.empty(len(x))
         for i in range(len(x)):
             var[i] = self.model(x[i])
 
         return var
 
     def variogram(self, x: np.array) -> np.array:
-        dist = squareform(pdist(x[:, :1]))
+        dist = cdist(x[:, :1], x[:, :1])
         variogram = []
+        # variogram = np.zeros(len(self.__bandwidth))
 
-        for h in self.__bandwidth:
-            z = []
-            for i in range(len(dist[:, 0])):
-                for j in range(i + 1, len(dist[:, 0])):
-                    if (dist[i, j] >= h - self.__bandwidth_step) and (
-                        dist[i, j] <= h + self.__bandwidth_step
-                    ):
-                        z.append(np.power(x[i, 1] - x[j, 1], 2))
-            if np.sum(z) >= 1e-7:
-                variogram.append(np.sum(z) / (2 * len(z)))
+        for idx, h in enumerate(self.__bandwidth):
+            indices = np.where(
+                (dist >= h - self.__bandwidth_step) & (dist <= h + self.__bandwidth_step),
+            )
+            z = np.power(x[indices[0], 1] - x[indices[1], 1], 2)
+            z_sum = np.sum(z)
+            if z_sum >= 1e-7:
+                variogram.append(z_sum / (2 * len(z)))
 
         return np.array(variogram)
```

### Comparing `uc_sgsim-1.2.1/uc_sgsim/cov_model/model.py` & `uc_sgsim-1.2.2/uc_sgsim/cov_model/model.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.1/uc_sgsim/krige/base.py` & `uc_sgsim-1.2.2/uc_sgsim/krige/base.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.1/uc_sgsim/krige/kriging.py` & `uc_sgsim-1.2.2/uc_sgsim/krige/kriging.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         if neighbor is not None:
             dist = abs(x[:, 0] - unsampled)
             dist = dist.reshape(len(dist), 1)
             has_neighbor = self.find_neighbor(dist, neighbor)
             if has_neighbor:
                 return has_neighbor
             x = np.hstack([x, dist])
-            x = np.array(sorted(x, key=lambda itr: itr[2])[:neighbor])
+            sorted_indices = np.argsort(x[:, 2])
+            x = x[sorted_indices][:neighbor]
 
         estimation, krige_std = self.prediction(x, unsampled)
 
         random_fix = np.random.normal(0, krige_std, 1)
         return estimation + random_fix
 
     def find_neighbor(self, dist: list[float], neighbor: int) -> float:
```

### Comparing `uc_sgsim-1.2.1/uc_sgsim/plot/base.py` & `uc_sgsim-1.2.2/uc_sgsim/plot/base.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.1/uc_sgsim/plot/plot.py` & `uc_sgsim-1.2.2/uc_sgsim/plot/plot.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,35 @@
-import time
-
 import matplotlib.pyplot as plt
 import numpy as np
 from uc_sgsim.plot.base import PlotBase
-from uc_sgsim.cov_model.base import CovModel
 
 
 class Visualize(PlotBase):
     xlabel = 'Distance(-)'
 
-    def __init__(self, model: CovModel, random_field: np.array):
-        super().__init__(model, random_field)
-
-    def mean_plot(self, n, mean=0) -> None:
+    def plot(self, realizations: list[int] = None, mean=0) -> None:
         realization_number = len(self.random_field[:, 0])
-        if n == 'ALL':
+        if realizations is None:
             for i in range(realization_number):
                 plt.figure(77879, figsize=self.figsize)
                 plt.plot(self.random_field[i, :] + mean)
                 plt.title('Realizations: ' + self.model_name, fontsize=20)
                 plt.xlabel(self.xlabel, fontsize=20)
                 plt.axhline(y=mean, color='r', linestyle='--', zorder=1)
                 plt.ylabel('Y', fontsize=20)
-
         else:
-            for item in n:
+            for item in realizations:
                 plt.figure(77879, figsize=self.figsize)
                 plt.plot(self.random_field[:, item] + mean)
                 plt.title('Realizations: ' + self.model_name, fontsize=20)
                 plt.xlabel(self.xlabel, fontsize=20)
                 plt.axhline(y=mean, color='r', linestyle='--', zorder=1)
                 plt.ylabel('Y', fontsize=20)
 
-    def variance_plot(self, mean=0) -> None:
+    def mean_plot(self, mean=0) -> None:
         zmean = np.zeros(len(self.random_field[0, :]))
         for i in range(len(self.random_field[0, :])):
             zmean[i] = np.mean(self.random_field[:, i] + mean)
 
         plt.figure(5212, figsize=self.figsize)
         plt.plot(
             zmean,
@@ -46,16 +39,16 @@
             markerfacecolor='y',
         )
         plt.xlabel(self.xlabel, fontsize=20)
         plt.ylabel('Mean', fontsize=20)
         plt.axhline(y=mean, color='r', linestyle='--', zorder=1)
         plt.xticks(fontsize=17), plt.yticks(fontsize=17)
 
+    def variance_plot(self) -> None:
         zvar = np.zeros(len(self.random_field[0, :]))
-
         for i in range(len(self.random_field[0, :])):
             zvar[i] = np.var(self.random_field[:, i])
 
         plt.figure(52712, figsize=self.figsize)
         plt.plot(
             zvar,
             '-o',
@@ -65,25 +58,23 @@
         )
         plt.xlabel(self.xlabel, fontsize=20)
         plt.ylabel('Variance', fontsize=20)
         plt.axhline(y=self.model.sill, color='b', linestyle='--', zorder=1)
         plt.xticks(fontsize=17), plt.yticks(fontsize=17)
 
     def cdf_plot(self, x_location: int) -> None:
-
-        X = self.random_field[:, x_location]
-
-        mu = np.mean(X)
-        sigma = np.std(X)
+        x = self.random_field[:, x_location]
+        mu = np.mean(x)
+        sigma = np.std(x)
         n_bins = 50
 
         _, ax = plt.subplots(figsize=(8, 4))
 
         _, bins, _ = ax.hist(
-            X,
+            x,
             n_bins,
             density=True,
             histtype='step',
             cumulative=True,
             label='Empirical',
         )
 
@@ -98,64 +89,51 @@
         ax.grid(True)
         ax.legend(loc='right')
         ax.set_title('Cumulative step histograms, x = ' + str(x_location))
         ax.set_xlabel('Random Variable (mm)')
         ax.set_ylabel('Occurrence')
 
     def hist_plot(self, x_location: int) -> None:
-
-        X = self.random_field[:, x_location]
-
-        mu = np.mean(X)
-        sigma = np.std(X)
-
+        x = self.random_field[:, x_location]
+        mu = np.mean(x)
+        sigma = np.std(x)
         num_bins = 50
         plt.figure(num=1151)
         _, bins, _ = plt.hist(
-            X,
+            x,
             num_bins,
             density=1,
             color='blue',
             alpha=0.5,
             edgecolor='k',
         )
 
         y = (1 / (np.sqrt(2 * np.pi) * sigma)) * np.exp(
             -0.5 * (1 / sigma * (bins - mu)) ** 2,
         )
 
         plt.plot(bins, y, '--', color='black')
-
         plt.xlabel('X-Axis')
         plt.ylabel('Y-Axis')
-
         plt.title('Histogram, x = ' + str(x_location))
 
     def variogram_plot(self, variogram: np.array) -> None:
-        start_time = time.time()
         for i in range(self.realization_number):
             plt.figure(123456, figsize=(10, 6))
             plt.plot(variogram[i, :], alpha=0.1)
             plt.title('Model: ' + self.model_name, fontsize=20)
             plt.xlabel('Lag(m)', fontsize=20)
             plt.ylabel('Variogram', fontsize=20)
             plt.xticks(fontsize=17), plt.yticks(fontsize=17)
-            print('Progress = %.2f' % (i / self.realization_number * 100) + '%', end='\r')
 
         plt.plot(
             self.model.var_compute(self.bandwidth),
             'o',
             markeredgecolor='k',
             markerfacecolor='w',
         )
 
         Vario_mean = np.zeros(len(self.bandwidth))
         for i in range(len(self.bandwidth)):
             Vario_mean[i] = np.mean(variogram[:, i])
 
         plt.plot(Vario_mean, '--', color='blue')
-
-        print('Progress = %.2f' % 100 + '%\n', end='\r')
-
-        end_time = time.time()
-
-        print('Time = ', end_time - start_time, 's')
```

### Comparing `uc_sgsim-1.2.1/uc_sgsim/random_field.py` & `uc_sgsim-1.2.2/uc_sgsim/random_field.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.1/uc_sgsim/sgsim.py` & `uc_sgsim-1.2.2/uc_sgsim/sgsim.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import time
-from typing import Union
 import sys
 from pathlib import Path
 from ctypes import CDLL, POINTER, c_double, c_int
 from multiprocessing import Pool
 
 import numpy as np
 from uc_sgsim.exception import VariogramDoesNotCompute
@@ -35,15 +34,15 @@
         if self.krige_method == 'SimpleKrige':
             self.krige = SimpleKrige(self.model)
 
         counts = 0
 
         start_time = time.time()
         np.random.seed(self.randomseed)
-        while counts < self.realization_number // self.n_process:
+        for _ in range(self.realization_number // self.n_process):
             unsampled = np.linspace(1, self.x_size - 2, self.x_size - 2)
             y_value = np.random.normal(0, self.model.sill**0.5, 2).reshape(2, 1)
             x_grid = np.array([0, self.x_size - 1]).reshape(2, 1)
             z = np.zeros(self.x_size)
             z[0], z[-1] = y_value[0], y_value[1]
             neigh = 0
 
@@ -81,67 +80,65 @@
 
     def compute(self, n_process: int, randomseed: int) -> np.array:
         pool = Pool(processes=n_process)
         self.n_process = n_process
         self.realization_number = self.realization_number * n_process
         self.random_field = np.empty([self.realization_number, self.x_size])
 
-        rand_list = []
-        parallel = []
-        for i in range(n_process):
-            s = randomseed + int(i)
-            rand_list.append(int(s))
-            parallel.append(True)
+        rand_list = [randomseed + i for i in range(n_process)]
+        parallel = [True] * n_process
 
         z = pool.starmap(self._process, zip(rand_list, parallel))
         pool.close()
         # use pool.join() to measure the coverage of sub process
         pool.join()
 
         for i in range(n_process):
-            for j in range(int(self.realization_number / n_process)):
-                start = int(i * self.realization_number / n_process)
-                self.random_field[j + start, :] = z[i][j, :]
+            start = int(i * self.realization_number / n_process)
+            end = int((i + 1) * self.realization_number / n_process)
+            self.random_field[start:end, :] = z[i][: end - start, :]
 
         return self.random_field
 
     def variogram_compute(self, n_process: int = 1) -> None:
         pool = Pool(processes=n_process)
         model_len = self.x_size
         x = np.linspace(0, self.x_size - 1, model_len).reshape(model_len, 1)
 
-        grid = []
-        for i in range(self.realization_number):
-            grid.append(
-                np.hstack([x, self.random_field[i, :].reshape(model_len, 1)]),
-            )
-
+        grid = [
+            np.hstack([x, self.random_field[i, :].reshape(model_len, 1)])
+            for i in range(self.realization_number)
+        ]
         self.variogram = pool.starmap(self.model.variogram, zip(grid))
         pool.close()
         # use pool.join() to measure the coverage of sub process
         pool.join()
         self.variogram = np.array(self.variogram)
 
-    def mean_plot(self, n: Union[str, list[int]], mean: float = 0) -> None:
+    def plot(self, realizations: list[int] = None, mean: float = 0):
+        plot = Visualize(self.model, self.random_field)
+        plot.plot(realizations, mean)
+
+    def mean_plot(self, mean: float = 0) -> None:
         m_plot = Visualize(self.model, self.random_field)
-        m_plot.mean_plot(n, mean)
+        m_plot.mean_plot(mean)
 
-    def variance_plot(self, mean: float = 0) -> None:
+    def variance_plot(self) -> None:
         s_plot = Visualize(self.model, self.random_field)
-        s_plot.variance_plot(mean)
+        s_plot.variance_plot()
 
     def cdf_plot(self, x_location: int) -> None:
         c_plot = Visualize(self.model, self.random_field)
         c_plot.cdf_plot(x_location)
 
     def hist_plot(self, x_location: int) -> None:
         h_plot = Visualize(self.model, self.random_field)
         h_plot.hist_plot(x_location)
 
-    def vario_plot(self) -> None:
+    def variogram_plot(self) -> None:
         if type(self.variogram) == int:
             raise VariogramDoesNotCompute()
         v_plot = Visualize(self.model, self.random_field)
         v_plot.variogram_plot(self.variogram)
 
 
 class UCSgsimDLL(UCSgsim):
@@ -212,29 +209,26 @@
         self.n_process = n_process
 
         if n_process > 1:
             self.realization_number = self.realization_number * n_process
 
         self.random_field = np.empty([self.realization_number, self.x_size])
 
-        rand_list = []
-        for i in range(n_process):
-            s = randomseed + int(i)
-            rand_list.append(int(s))
+        rand_list = [randomseed + i for i in range(n_process)]
 
         z = pool.starmap(self._cpdll, zip(rand_list))
 
         pool.close()
         # use pool.join() to measure the coverage of sub process
         pool.join()
 
         for i in range(n_process):
-            for j in range(int(self.realization_number / n_process)):
-                start = int(i * self.realization_number / n_process)
-                self.random_field[j + start, :] = z[i][j, :]
+            start = int(i * self.realization_number / n_process)
+            end = int((i + 1) * self.realization_number / n_process)
+            self.random_field[start:end, :] = z[i][: end - start, :]
 
         return self.random_field
 
     def _variogram_cpdll(self, n_process: int) -> np.array:
         lib = self._lib_read()
         vario = lib.variogram
         vario.argtypes = (
@@ -263,21 +257,16 @@
 
         return variogram
 
     def variogram_compute(self, n_process: int = 1) -> np.array:
         pool = Pool(processes=n_process)
         self.n_process = n_process
 
-        if n_process > 1:
-            self.realization_number = self.realization_number * n_process
-
         self.variogram = np.empty([self.realization_number, len(self.bandwidth)])
-        cpu_number = []
-        for i in range(self.n_process):
-            cpu_number.append(i)
+        cpu_number = [i for i in range(self.n_process)]
 
         z = pool.starmap(self._variogram_cpdll, zip(cpu_number))
         pool.close()
         # use pool.join() to measure the coverage of sub process
         pool.join()
 
         for i in range(n_process):
```

### Comparing `uc_sgsim-1.2.1/uc_sgsim/utils.py` & `uc_sgsim-1.2.2/uc_sgsim/utils.py`

 * *Files identical despite different names*

### Comparing `uc_sgsim-1.2.1/uc_sgsim.egg-info/PKG-INFO` & `uc_sgsim-1.2.2/uc_sgsim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uc-sgsim
-Version: 1.2.1
+Version: 1.2.2
 Summary: Random Field Generation
 Home-page: https://github.com/Zncl2222/Stochastic_UC_SGSIM
 Author: Zncl2222
 Author-email: 3002shinning@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -98,80 +98,74 @@
 ## Installation
 ```bash
 pip install uc-sgsim
 ```
 
 ## Features
 * One dimensional unconditional randomfield generation with sequential gaussian simulation algorithm
-* Enable to use muti-cores to run the simulation (mutiprocessing)
+* Muti-cores simulation (mutiprocessing)
 * Run C to generate randomfield in python via ctype interface, or just generate randomfield in python with numpy and scipy library.
 
-
-
 ## Example
 ```py
 import matplotlib.pyplot as plt
 import uc_sgsim as uc
 from uc_sgsim.cov_model import Gaussian
 
 if __name__ == '__main__':
     x = 151  # Model grid, only 1D case is support now
+
     bw_s = 1  # lag step
     bw_l = 35  # lag range
-    randomseed = 12321  # randomseed for simulation
-    a = 17.32  # effective range of covariance model
-    C0 = 1  # sill of covariance model
+    randomseed = 151  # randomseed for simulation
+    k_range = 17.32  # effective range of covariance model
+    sill = 1  # sill of covariance model
 
     nR = 10  # numbers of realizations in each CPU cores,
     # if nR = 1 n_process = 8
     # than you will compute total 8 realizations
 
     # Create Covariance model first
-    Cov_model = Gaussian(bw_l, bw_s, a, C0)
+    cov_model = Gaussian(bw_l, bw_s, k_range, sill)
 
     # Create simulation and input the Cov model
-    sgsim = uc.UCSgsim(X, Cov_model, nR)  # Create class instance that generate field in python
-    sgsim_c = uc.UCSgsimDLL(x, Cov_model, nR) # Create class instance that generate field in c
+    sgsim_py = uc.UCSgsim(x, cov_model, nR) # run sgsim with python
+    sgsim_c = uc.UCSgsimDLL(x, cov_model, nR) # run sgsim with c
 
     # Start compute with n CPUs
-    sgsim.compute_async(n_process=8, randomseed=454) # Generate field (python)
-    sgsim_c.compute(n_process=2, randomseed=151) # Generate field (c)
+    sgsim_c.compute(n_process=2, randomseed=randomseed)
+    sgsim_py.compute(n_process=2, randomseed=987654)
 
-    sgsim.mean_plot('ALL')  # Plot mean
-    sgsim.variance_plot()  # Plot variance
-    sgsim.cdf_plot(x_location=10)  # CDF
-    sgsim.hist_plot(x_location=10)  # Hist
-    sgsim.variogram_compute(n_process=2)  # Compute variogram before plotting
+    sgsim_c.mean_plot('ALL')  # Plot mean
+    sgsim_c.variance_plot()  # Plot variance
+    sgsim_c.cdf_plot(x_location=10)  # CDF
+    sgsim_c.hist_plot(x_location=10)  # Hist
+    sgsim_c.variogram_compute(n_process=2)  # Compute variogram before plotting
     # Plot variogram and mean variogram for validation
-    sgsim.vario_plot()
+    sgsim_c.vario_plot()
     # Save random_field and variogram
-    sgsim.save_random_field('randomfield.csv', save_single=True) # save in single file
-    sgsim.save_variogram('') # save each field individually
+    sgsim_c.save_random_field('randomfields.csv', save_single=True)
+    sgsim_c.save_variogram('variograms.csv', save_single=True)
 
-    # plt.show() to show the matplotlib plot
+    # show figure
     plt.show()
-
-    # Please note that the parameter "n_realizations" means the number of realizations calculate in each process,
-    # so this case will generate total 20 * 4(process) = 80 realizations
-
 ```
 
-
 <p align="center">
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Realizations.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Mean.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variance.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/Variogram.png"  width="50%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/HIST.png"  width="40%"/>
    <img src="https://github.com/Zncl2222/Stochastic_SGSIM/blob/main/figure/CDF.png"  width="50%"/>
 </p>
 
 ## Future plans
 * 2D unconditional randomfield generation
-* GUI mode in pyhton
+* GUI (pyhton)
 * More covariance models
 * More kriging methods (etc. Oridinary Kriging)
 * Performance enhancement
 * More completely documents and easy to use designs.
 
 ## Performance
 <p align="center">
```

### Comparing `uc_sgsim-1.2.1/uc_sgsim.egg-info/SOURCES.txt` & `uc_sgsim-1.2.2/uc_sgsim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

