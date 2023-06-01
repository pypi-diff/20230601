# Comparing `tmp/breathXplorer-0.1.5.tar.gz` & `tmp/breathXplorer-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "breathXplorer-0.1.5.tar", last modified: Thu Apr 20 21:16:09 2023, max compression
+gzip compressed data, was "breathXplorer-0.1.6.tar", last modified: Thu Jun  1 18:46:03 2023, max compression
```

## Comparing `breathXplorer-0.1.5.tar` & `breathXplorer-0.1.6.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 21:16:09.893903 breathXplorer-0.1.5/
--rw-r--r--   0 wangyk     (501) staff       (20)     1067 2023-04-12 00:06:18.000000 breathXplorer-0.1.5/LICENSE
--rw-r--r--   0 wangyk     (501) staff       (20)     1867 2023-04-20 21:16:09.893738 breathXplorer-0.1.5/PKG-INFO
--rw-r--r--   0 wangyk     (501) staff       (20)     1185 2023-04-19 23:51:39.000000 breathXplorer-0.1.5/README.md
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 21:16:09.892137 breathXplorer-0.1.5/breathXplorer/
--rw-r--r--   0 wangyk     (501) staff       (20)       60 2023-04-19 22:11:13.000000 breathXplorer-0.1.5/breathXplorer/__init__.py
--rw-r--r--   0 wangyk     (501) staff       (20)     2972 2023-04-12 17:21:22.000000 breathXplorer-0.1.5/breathXplorer/cluster.py
--rw-r--r--   0 wangyk     (501) staff       (20)     1858 2023-04-19 23:07:11.000000 breathXplorer-0.1.5/breathXplorer/extract.py
--rw-r--r--   0 wangyk     (501) staff       (20)     5045 2023-04-19 22:06:06.000000 breathXplorer-0.1.5/breathXplorer/file_io.py
--rw-r--r--   0 wangyk     (501) staff       (20)     6018 2023-04-12 17:21:22.000000 breathXplorer-0.1.5/breathXplorer/find_peak.py
--rw-r--r--   0 wangyk     (501) staff       (20)     2392 2023-04-20 20:29:08.000000 breathXplorer-0.1.5/breathXplorer/utils.py
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 21:16:09.893170 breathXplorer-0.1.5/breathXplorer.egg-info/
--rw-r--r--   0 wangyk     (501) staff       (20)     1867 2023-04-20 21:16:09.000000 breathXplorer-0.1.5/breathXplorer.egg-info/PKG-INFO
--rw-r--r--   0 wangyk     (501) staff       (20)      383 2023-04-20 21:16:09.000000 breathXplorer-0.1.5/breathXplorer.egg-info/SOURCES.txt
--rw-r--r--   0 wangyk     (501) staff       (20)        1 2023-04-20 21:16:09.000000 breathXplorer-0.1.5/breathXplorer.egg-info/dependency_links.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       53 2023-04-20 21:16:09.000000 breathXplorer-0.1.5/breathXplorer.egg-info/requires.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       14 2023-04-20 21:16:09.000000 breathXplorer-0.1.5/breathXplorer.egg-info/top_level.txt
--rw-r--r--   0 wangyk     (501) staff       (20)       38 2023-04-20 21:16:09.893961 breathXplorer-0.1.5/setup.cfg
--rw-r--r--   0 wangyk     (501) staff       (20)      957 2023-04-20 20:24:13.000000 breathXplorer-0.1.5/setup.py
-drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-04-20 21:16:09.893351 breathXplorer-0.1.5/tests/
--rw-r--r--   0 wangyk     (501) staff       (20)      985 2023-04-20 20:29:28.000000 breathXplorer-0.1.5/tests/test_extract.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-01 18:46:03.228761 breathXplorer-0.1.6/
+-rw-r--r--   0 wangyk     (501) staff       (20)     1067 2023-04-12 00:06:18.000000 breathXplorer-0.1.6/LICENSE
+-rw-r--r--   0 wangyk     (501) staff       (20)     6822 2023-06-01 18:46:03.228546 breathXplorer-0.1.6/PKG-INFO
+-rw-r--r--   0 wangyk     (501) staff       (20)     6141 2023-06-01 18:38:02.000000 breathXplorer-0.1.6/README.md
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-01 18:46:03.226377 breathXplorer-0.1.6/breathXplorer/
+-rw-r--r--   0 wangyk     (501) staff       (20)       85 2023-06-01 18:11:03.000000 breathXplorer-0.1.6/breathXplorer/__init__.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     2972 2023-04-12 17:21:22.000000 breathXplorer-0.1.6/breathXplorer/cluster.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     2763 2023-05-31 22:39:26.000000 breathXplorer-0.1.6/breathXplorer/container.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     1939 2023-05-30 23:11:26.000000 breathXplorer-0.1.6/breathXplorer/extract.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     5589 2023-05-30 23:09:12.000000 breathXplorer-0.1.6/breathXplorer/file_io.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     6081 2023-06-01 18:11:03.000000 breathXplorer-0.1.6/breathXplorer/find_peak.py
+-rw-r--r--   0 wangyk     (501) staff       (20)     2392 2023-05-04 19:00:37.000000 breathXplorer-0.1.6/breathXplorer/utils.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-01 18:46:03.227748 breathXplorer-0.1.6/breathXplorer.egg-info/
+-rw-r--r--   0 wangyk     (501) staff       (20)     6822 2023-06-01 18:46:03.000000 breathXplorer-0.1.6/breathXplorer.egg-info/PKG-INFO
+-rw-r--r--   0 wangyk     (501) staff       (20)      410 2023-06-01 18:46:03.000000 breathXplorer-0.1.6/breathXplorer.egg-info/SOURCES.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)        1 2023-06-01 18:46:03.000000 breathXplorer-0.1.6/breathXplorer.egg-info/dependency_links.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       53 2023-06-01 18:46:03.000000 breathXplorer-0.1.6/breathXplorer.egg-info/requires.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       14 2023-06-01 18:46:03.000000 breathXplorer-0.1.6/breathXplorer.egg-info/top_level.txt
+-rw-r--r--   0 wangyk     (501) staff       (20)       38 2023-06-01 18:46:03.228828 breathXplorer-0.1.6/setup.cfg
+-rw-r--r--   0 wangyk     (501) staff       (20)      957 2023-05-31 00:33:00.000000 breathXplorer-0.1.6/setup.py
+drwxr-xr-x   0 wangyk     (501) staff       (20)        0 2023-06-01 18:46:03.227920 breathXplorer-0.1.6/tests/
+-rw-r--r--   0 wangyk     (501) staff       (20)      523 2023-06-01 18:32:19.000000 breathXplorer-0.1.6/tests/test_extract.py
```

### Comparing `breathXplorer-0.1.5/LICENSE` & `breathXplorer-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.5/breathXplorer/cluster.py` & `breathXplorer-0.1.6/breathXplorer/cluster.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.5/breathXplorer/extract.py` & `breathXplorer-0.1.6/breathXplorer/extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from pathlib import Path
 from typing import Sequence, List, Union
 
 import pandas as pd
 
 from .cluster import cluster_merge
+from .container import FeatureSet, Sample
 from .file_io import cluster_ms, gen_df
 from .utils import score, time_union, interpolate_time
 
 
 # a single task
-def find_feature(ms: Union[Path, str], line: bool, quantity: float, method: str, n_peak: int = 1) -> pd.DataFrame:
+def find_feature(ms: Union[Path, str], line: bool, quantity: float, method: str, n_peak: int = 1) -> FeatureSet:
     """
     Calculate the feature table of a single mzML file.
     :param ms:  Path of the mzML file.
     :param line:  Whether to use line mode.
     :param quantity: control the quality of peak
     :param method:  The method used to find peaks ('Topological' or 'Gaussian').
     :param n_peak:  Number of peaks to be picked
@@ -21,33 +22,33 @@
     """
     ms = Path(ms)
     scanned = cluster_ms(str(ms.absolute()), line, quantity, method, n_peak)
     try:
         scores = score(scanned, scanned['peak_time'])
     except ZeroDivisionError:
         scores = score(scanned)
-    return gen_df(scanned, [('intensity', scores)])
+    return FeatureSet(gen_df(scanned, [('intensity', scores)]))
 
 
 # merge all the result files of single tasks in the target folder
-def merge_result(tbs: Sequence[pd.DataFrame], names: List[str]) -> pd.DataFrame:
+def merge_result(tbs: Sequence[FeatureSet], names: List[str]) -> Sample:
     """
     Merge the feature tables of multiple mzML files.
     :param tbs:  Feature tables
     :param names:  Names of the mzML files
     :return:  Merged feature table
     """
-    sub_results = [dict(zip(tb.index, tb['intensity'])) for tb in tbs]
+    sub_results = [dict(zip(tb.mz, tb.intensity)) for tb in tbs]
     result = cluster_merge(sub_results)
-    return pd.DataFrame(data=list(result.values()), index=list(result.keys()), columns=names)
+    return Sample(pd.DataFrame(data=list(result.values()), index=list(result.keys()), columns=names))
 
 
-def time_align(tbs: Sequence[pd.DataFrame]) -> Sequence[pd.DataFrame]:
+def time_align(tbs: Sequence[FeatureSet]) -> Sequence[FeatureSet]:
     """
     Align the time of multiple feature tables.
     :param tbs:  Feature tables
     :return:  Aligned feature tables
     """
     if len(tbs) == 1:
         return tbs
-    common_time = time_union(tbs)
-    return [interpolate_time(tb, common_time) for tb in tbs]
+    common_time = time_union([tb.table for tb in tbs])
+    return [FeatureSet(interpolate_time(tb.table, common_time)) for tb in tbs]
```

### Comparing `breathXplorer-0.1.5/breathXplorer/file_io.py` & `breathXplorer-0.1.6/breathXplorer/file_io.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from functools import reduce
-from typing import Tuple, List
+from pathlib import Path
+from typing import Tuple, List, Union
 
 import numpy as np
 import pandas as pd
 from pyteomics import mzml
 from scipy import signal, sparse
 
 from .cluster import cluster_mz, __drop_zero_near
+from .container import FeatureSet, TandemMS
 from .find_peak import time_with_peak
 
 
 def __purify(mz: np.ndarray, ints: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
     """
     Filter the m/z values and intensities by removing noise.
     :param mz: m/z values
@@ -83,15 +85,15 @@
     tb.columns = times.index
     return tb
 
 
 def cluster_ms(ms: str, line: bool, dense: float, method: str, n_peak=1) -> dict:
     """
     Find all bars in the time to m/z heatmap.:param ms: mzML file path
-    :param line: Whether the mzML file is a line spectra file
+    :param line: Whether the mzML file is a line spectra mzML
     :param dense: Control the quality of peak
     :param method: Peak picking method
     :param n_peak: Number of peaks
     :return: Dictionary with time, intensities, TIC, and peak time information
     """
     tb = read_sparse(ms, line)
     times = tb.columns.values
@@ -119,7 +121,23 @@
     """
     mat = np.array(list(scanned_file['intensities'].values()))
     otb = pd.DataFrame(data=mat, index=list(scanned_file['intensities'].keys()), columns=scanned_file['time'])
     for name, ndc in new_inf:
         ntb = pd.DataFrame({name: list(ndc.values())}, index=list(ndc.keys()))
         otb = pd.concat([ntb, otb], axis='columns', ignore_index=False)
     return otb
+
+
+def retrieve_tandem(file: Union[str, Path], feature: FeatureSet, radium: float) -> TandemMS:
+    """
+    Retrieve tandem MS information from an zML mzML.
+
+    :param file: mzML file path
+    :param feature: result FeatureSet
+    :param radium: Radium of the feature
+    :return: TandemMS object
+    """
+    file = Path(file)
+    tandem = TandemMS(feature.mz)
+    with mzml.read(str(file.absolute())) as handle:
+        tandem.build(handle, radium)
+    return tandem
```

### Comparing `breathXplorer-0.1.5/breathXplorer/find_peak.py` & `breathXplorer-0.1.6/breathXplorer/find_peak.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,16 @@
 
 def find_peak(x: np.ndarray, y: np.ndarray) -> list:
     """
     Finds the x's range of each peak using the 'Topological' method.
 
     :param x: An array of time points.
     :param y: An array of corresponding values (e.g. concentration or intensity).
-    :return: A list of tuples containing the start and end x values of the ranges, and the y values at the peaks.
+    :return: A list of tuples containing the start and end time point values of the ranges, and the maximum
+     intensity values of the peaks.
     """
     f = interpolate.interp1d(x, y, kind='cubic')
     n_x = np.union1d(np.linspace(np.min(x), np.max(x), max(1000, len(x))), x)  # can influence effect of finding range
     n_y = f(n_x)
     ori_range = __find_all_range(n_x, n_y)
     merged_ranges = __merge_ranges(ori_range)
     return merged_ranges
@@ -138,15 +139,16 @@
 def find_gaussian(x: np.ndarray, y: np.ndarray, n: int) -> list:
     """
     Uses the Gaussian Mixture Model to find the range of each peak.
 
     :param x: An array of time points.
     :param y: An array of corresponding values (e.g. concentration or intensity).
     :param n: The number of peaks to consider.
-    :return: A list of tuples containing the start and end x values of the ranges, and the y values at the peaks.
+    :return: A list of tuples containing the start and end time point values of the ranges, and the maximum
+        intensity values of the peaks.
     """
     ny = y.copy()
     ny -= ny.min()
     ny /= ny.sum()
     samples = x[np.random.choice(len(ny), size=5000, p=ny)]
     gmm = GaussianMixture(n_components=n)
     gmm.fit(samples.reshape(-1, 1))
```

### Comparing `breathXplorer-0.1.5/breathXplorer/utils.py` & `breathXplorer-0.1.6/breathXplorer/utils.py`

 * *Files identical despite different names*

### Comparing `breathXplorer-0.1.5/setup.py` & `breathXplorer-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirement.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="breathXplorer",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=required_packages,
     author="wykswr",
     author_email="bifocal.above.0y@icloud.com",
     description="A toolkit for breath metabolomics analysis",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

