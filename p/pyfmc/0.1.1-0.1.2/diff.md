# Comparing `tmp/pyfmc-0.1.1.tar.gz` & `tmp/pyfmc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfmc-0.1.1.tar", last modified: Sun May 28 09:11:42 2023, max compression
+gzip compressed data, was "pyfmc-0.1.2.tar", last modified: Thu Jun  1 15:30:55 2023, max compression
```

## Comparing `pyfmc-0.1.1.tar` & `pyfmc-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-28 09:11:42.903924 pyfmc-0.1.1/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3045 2023-05-28 09:11:42.903924 pyfmc-0.1.1/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1914 2023-05-28 09:08:26.000000 pyfmc-0.1.1/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-28 09:11:42.903924 pyfmc-0.1.1/pyfmc/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-06 13:51:16.000000 pyfmc-0.1.1/pyfmc/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-28 09:11:42.903924 pyfmc-0.1.1/pyfmc/common/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2023-05-06 13:51:16.000000 pyfmc-0.1.1/pyfmc/common/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-05-06 13:51:16.000000 pyfmc-0.1.1/pyfmc/common/historical_data.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-05-06 13:51:16.000000 pyfmc-0.1.1/pyfmc/exceptions.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-28 09:11:42.903924 pyfmc-0.1.1/pyfmc/simulations/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      266 2023-05-06 13:51:16.000000 pyfmc-0.1.1/pyfmc/simulations/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4736 2023-05-28 09:08:26.000000 pyfmc-0.1.1/pyfmc/simulations/gbm.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-28 09:11:42.903924 pyfmc-0.1.1/pyfmc.egg-info/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3045 2023-05-28 09:11:42.000000 pyfmc-0.1.1/pyfmc.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      334 2023-05-28 09:11:42.000000 pyfmc-0.1.1/pyfmc.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-28 09:11:42.000000 pyfmc-0.1.1/pyfmc.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-05-28 09:11:42.000000 pyfmc-0.1.1/pyfmc.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-05-28 09:11:42.000000 pyfmc-0.1.1/pyfmc.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-28 09:11:42.903924 pyfmc-0.1.1/setup.cfg
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      714 2023-05-28 09:11:36.000000 pyfmc-0.1.1/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 15:30:55.990794 pyfmc-0.1.2/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3045 2023-06-01 15:30:55.990794 pyfmc-0.1.2/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1914 2023-05-28 09:08:26.000000 pyfmc-0.1.2/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 15:30:55.986794 pyfmc-0.1.2/pyfmc/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-06 13:51:16.000000 pyfmc-0.1.2/pyfmc/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 15:30:55.986794 pyfmc-0.1.2/pyfmc/common/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      395 2023-05-06 13:51:16.000000 pyfmc-0.1.2/pyfmc/common/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      995 2023-05-06 13:51:16.000000 pyfmc-0.1.2/pyfmc/common/historical_data.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      195 2023-05-06 13:51:16.000000 pyfmc-0.1.2/pyfmc/exceptions.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 15:30:55.990794 pyfmc-0.1.2/pyfmc/simulations/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      266 2023-05-06 13:51:16.000000 pyfmc-0.1.2/pyfmc/simulations/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4804 2023-06-01 15:29:57.000000 pyfmc-0.1.2/pyfmc/simulations/gbm.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-06-01 15:30:55.990794 pyfmc-0.1.2/pyfmc.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3045 2023-06-01 15:30:55.000000 pyfmc-0.1.2/pyfmc.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      334 2023-06-01 15:30:55.000000 pyfmc-0.1.2/pyfmc.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-06-01 15:30:55.000000 pyfmc-0.1.2/pyfmc.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       70 2023-06-01 15:30:55.000000 pyfmc-0.1.2/pyfmc.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        6 2023-06-01 15:30:55.000000 pyfmc-0.1.2/pyfmc.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-06-01 15:30:55.990794 pyfmc-0.1.2/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      734 2023-06-01 15:29:57.000000 pyfmc-0.1.2/setup.py
```

### Comparing `pyfmc-0.1.1/PKG-INFO` & `pyfmc-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Finance Monte-Carlo Simulation using PyTorch
 Home-page: https://github.com/ethanlee928/pyfmc
 Author: Ethan Lee
 Author-email: ethan2000.el@gmail.com
 License: UNKNOWN
 Description: # Finance Monte-Carlo Simulation using PyTorch
```

### Comparing `pyfmc-0.1.1/README.md` & `pyfmc-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pyfmc-0.1.1/pyfmc/common/historical_data.py` & `pyfmc-0.1.2/pyfmc/common/historical_data.py`

 * *Files identical despite different names*

### Comparing `pyfmc-0.1.1/pyfmc/simulations/gbm.py` & `pyfmc-0.1.2/pyfmc/simulations/gbm.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from ..common import HistoricalData, get_device
 
 logger = logging.getLogger("pyfmc.simulations.gbm")
 
 
 class Trajectory:
     def __init__(self, dist: torch.Tensor, label: str = "Trajectory") -> None:
-        self.dist = dist
+        self.dist = dist.numpy()
         self.label = label
 
     def value(self):
         return self.dist
 
     def plot(self, title=None, xlabel=None, ylabel=None):
         fig, ax = plt.subplots()
@@ -102,14 +102,15 @@
         self.n_trajectories = n_trajectories
         if (open_index and close_index) not in df.columns:
             raise SimulationException("Wrong open_index or close_index")
 
     def simulate(self):
         hist_data = HistoricalData(self.df, self.open_index, self.close_index)
         device = get_device() if self.device_acc else torch.device("cpu")
+        logger.info("Using %s for calculation ...", device)
         dtype = torch.float32 if device == torch.device("mps") else torch.float64
         logger.info("Using device: %s", device)
 
         exp_return = torch.tensor(hist_data.return_mean, device=device, dtype=dtype)
         std_return = torch.tensor(hist_data.return_std, device=device, dtype=dtype)
         last_price = hist_data.get_latest_close_price()
```

### Comparing `pyfmc-0.1.1/pyfmc.egg-info/PKG-INFO` & `pyfmc-0.1.2/pyfmc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfmc
-Version: 0.1.1
+Version: 0.1.2
 Summary: Finance Monte-Carlo Simulation using PyTorch
 Home-page: https://github.com/ethanlee928/pyfmc
 Author: Ethan Lee
 Author-email: ethan2000.el@gmail.com
 License: UNKNOWN
 Description: # Finance Monte-Carlo Simulation using PyTorch
```

### Comparing `pyfmc-0.1.1/setup.py` & `pyfmc-0.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import os
 from setuptools import setup, find_packages
 
 
 setup(
     name="pyfmc",
-    version="0.1.1",
+    version=os.environ["VER"],
     author="Ethan Lee",
     author_email="ethan2000.el@gmail.com",
     description="Finance Monte-Carlo Simulation using PyTorch",
     long_description=open("README.md", "r").read(),
     long_description_content_type="text/markdown",
     packages=find_packages("."),
     package_dir={"": "."},
```

