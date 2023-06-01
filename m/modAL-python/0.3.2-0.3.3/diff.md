# Comparing `tmp/modAL-python-0.3.2.tar.gz` & `tmp/modAL-python-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modAL-python-0.3.2.tar", last modified: Thu Jun  1 10:51:48 2023, max compression
+gzip compressed data, was "modAL-python-0.3.3.tar", last modified: Thu Jun  1 10:52:44 2023, max compression
```

## Comparing `modAL-python-0.3.2.tar` & `modAL-python-0.3.3.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:51:48.281441 modAL-python-0.3.2/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1070 2018-11-26 15:41:43.000000 modAL-python-0.3.2/LICENSE
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:51:48.281441 modAL-python-0.3.2/PKG-INFO
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10893 2018-11-26 15:41:43.000000 modAL-python-0.3.2/README.md
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:51:48.281441 modAL-python-0.3.2/modAL/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      128 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     5665 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/acquisition.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     9965 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/batch.py
--rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/cluster.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1762 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/density.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     7735 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/disagreement.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:51:48.281441 modAL-python-0.3.2/modAL/models/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      180 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/models/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    14622 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/models/base.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    20666 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/models/learners.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     8792 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/multilabel.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     5955 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/uncertainty.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:51:48.281441 modAL-python-0.3.2/modAL/utils/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      417 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/utils/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3651 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/utils/combination.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      702 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/utils/data.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1331 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/utils/selection.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1920 2018-11-26 15:41:43.000000 modAL-python-0.3.2/modAL/utils/validation.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:51:48.281441 modAL-python-0.3.2/modAL_python.egg-info/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:51:48.000000 modAL-python-0.3.2/modAL_python.egg-info/PKG-INFO
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      559 2023-06-01 10:51:48.000000 modAL-python-0.3.2/modAL_python.egg-info/SOURCES.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        1 2023-06-01 10:51:48.000000 modAL-python-0.3.2/modAL_python.egg-info/dependency_links.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       43 2023-06-01 10:51:48.000000 modAL-python-0.3.2/modAL_python.egg-info/requires.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        6 2023-06-01 10:51:48.000000 modAL-python-0.3.2/modAL_python.egg-info/top_level.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       79 2023-06-01 10:51:48.285441 modAL-python-0.3.2/setup.cfg
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      478 2023-06-01 10:51:43.000000 modAL-python-0.3.2/setup.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:52:44.977365 modAL-python-0.3.3/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1070 2018-11-30 09:42:20.000000 modAL-python-0.3.3/LICENSE
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:52:44.977365 modAL-python-0.3.3/PKG-INFO
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10893 2018-11-30 09:42:20.000000 modAL-python-0.3.3/README.md
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:52:44.977365 modAL-python-0.3.3/modAL/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      128 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     5665 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/acquisition.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     9965 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/batch.py
+-rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/cluster.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1762 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/density.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     7735 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/disagreement.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     2719 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/expected_error.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:52:44.977365 modAL-python-0.3.3/modAL/models/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      180 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/models/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    14622 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/models/base.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    20666 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/models/learners.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     8792 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/multilabel.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     6972 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/uncertainty.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:52:44.977365 modAL-python-0.3.3/modAL/utils/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      417 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/utils/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3651 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/utils/combination.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      712 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/utils/data.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1331 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/utils/selection.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1920 2018-11-30 09:42:20.000000 modAL-python-0.3.3/modAL/utils/validation.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:52:44.977365 modAL-python-0.3.3/modAL_python.egg-info/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:52:44.000000 modAL-python-0.3.3/modAL_python.egg-info/PKG-INFO
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      583 2023-06-01 10:52:44.000000 modAL-python-0.3.3/modAL_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        1 2023-06-01 10:52:44.000000 modAL-python-0.3.3/modAL_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       43 2023-06-01 10:52:44.000000 modAL-python-0.3.3/modAL_python.egg-info/requires.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        6 2023-06-01 10:52:44.000000 modAL-python-0.3.3/modAL_python.egg-info/top_level.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       79 2023-06-01 10:52:44.977365 modAL-python-0.3.3/setup.cfg
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      478 2023-06-01 10:52:37.000000 modAL-python-0.3.3/setup.py
```

### Comparing `modAL-python-0.3.2/LICENSE` & `modAL-python-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/README.md` & `modAL-python-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -144,21 +144,21 @@
 <p align="center">
  <img src="https://modal-python.readthedocs.io/en/latest/_images/gp-final.png">
 </p>
 
 ## Additional examples<a name="additional-examples"></a>
 Including this, many examples are available:
 - [Pool-based sampling](https://modal-python.readthedocs.io/en/latest/content/examples/pool-based_sampling.html)  
-- [Stream-based sampling](https://modal-python.readthedocs.io/en/latest/content/examples/Stream-based-sampling.html)  
+- [Stream-based sampling](https://modal-python.readthedocs.io/en/latest/content/examples/stream-based_sampling.html)  
 - [Active regression](https://modal-python.readthedocs.io/en/latest/content/examples/active_regression.html)  
 - [Ensemble regression](https://modal-python.readthedocs.io/en/latest/content/examples/ensemble_regression.html)  
 - [Bayesian optimization](https://modal-python.readthedocs.io/en/latest/content/examples/bayesian_optimization.html)  
-- [Query by committee](https://modal-python.readthedocs.io/en/latest/content/examples/Query-by-committee.html)  
-- [Bootstrapping and bagging](https://modal-python.readthedocs.io/en/latest/content/examples/Bootstrapping-and-bagging.html)  
-- [Keras integration](https://modal-python.readthedocs.io/en/latest/content/examples/Keras-integration.html)
+- [Query by committee](https://modal-python.readthedocs.io/en/latest/content/examples/query_by_committee.html)  
+- [Bootstrapping and bagging](https://modal-python.readthedocs.io/en/latest/content/examples/bootstrapping_and_bagging.html)  
+- [Keras integration](https://modal-python.readthedocs.io/en/latest/content/examples/Keras_integration.html)
 
 # Installation<a name="installation"></a>
 modAL requires
 - Python >= 3.5
 - NumPy >= 1.13
 - SciPy >= 0.18
 - scikit-learn >= 0.18
```

### Comparing `modAL-python-0.3.2/modAL/acquisition.py` & `modAL-python-0.3.3/modAL/acquisition.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/modAL/batch.py` & `modAL-python-0.3.3/modAL/batch.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/modAL/density.py` & `modAL-python-0.3.3/modAL/density.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/modAL/disagreement.py` & `modAL-python-0.3.3/modAL/disagreement.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/modAL/models/base.py` & `modAL-python-0.3.3/modAL/models/base.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/modAL/models/learners.py` & `modAL-python-0.3.3/modAL/models/learners.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/modAL/multilabel.py` & `modAL-python-0.3.3/modAL/multilabel.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/modAL/uncertainty.py` & `modAL-python-0.3.3/modAL/uncertainty.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,62 @@
 from sklearn.exceptions import NotFittedError
 from sklearn.base import BaseEstimator
 
 from modAL.utils.selection import multi_argmax
 from modAL.utils.data import modALinput
 
 
+def _proba_uncertainty(proba: np.ndarray) -> np.ndarray:
+    """
+    Calculates the uncertainty of the prediction probabilities.
+
+    Args:
+        proba: Prediction probabilities.
+
+    Returns:
+        Uncertainty of the prediction probabilities.
+    """
+
+    return 1 - np.max(proba, axis=1)
+
+
+def _proba_margin(proba: np.ndarray) -> np.ndarray:
+    """
+    Calculates the margin of the prediction probabilities.
+
+    Args:
+        proba: Prediction probabilities.
+
+    Returns:
+        Margin of the prediction probabilities.
+    """
+
+    if proba.shape[1] == 1:
+        return np.zeros(shape=len(proba))
+
+    part = np.partition(-proba, 1, axis=1)
+    margin = - part[:, 0] + part[:, 1]
+
+    return margin
+
+
+def _proba_entropy(proba: np.ndarray) -> np.ndarray:
+    """
+    Calculates the entropy of the prediction probabilities.
+
+    Args:
+        proba: Prediction probabilities.
+
+    Returns:
+        Uncertainty of the prediction probabilities.
+    """
+
+    return np.transpose(entropy(np.transpose(proba)))
+
+
 def classifier_uncertainty(classifier: BaseEstimator, X: modALinput, **predict_proba_kwargs) -> np.ndarray:
     """
     Classification uncertainty of the classifier for the provided samples.
 
     Args:
         classifier: The classifier for which the uncertainty is to be measured.
         X: The samples for which the uncertainty of classification is to be measured.
```

### Comparing `modAL-python-0.3.2/modAL/utils/combination.py` & `modAL-python-0.3.3/modAL/utils/combination.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/modAL/utils/data.py` & `modAL-python-0.3.3/modAL/utils/data.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import Union
+from typing import Union, Container
 from itertools import chain
 
 import numpy as np
 import scipy.sparse as sp
 
 
 modALinput = Union[list, np.ndarray, sp.csr_matrix]
 
 
-def data_vstack(blocks: modALinput) -> modALinput:
+def data_vstack(blocks: Container) -> modALinput:
     """
     Stack vertically both sparse and dense arrays.
 
     Args:
         blocks: Sequence of modALinput objects.
 
     Returns:
```

### Comparing `modAL-python-0.3.2/modAL/utils/selection.py` & `modAL-python-0.3.3/modAL/utils/selection.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/modAL/utils/validation.py` & `modAL-python-0.3.3/modAL/utils/validation.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.2/modAL_python.egg-info/SOURCES.txt` & `modAL-python-0.3.3/modAL_python.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 modAL/__init__.py
 modAL/acquisition.py
 modAL/batch.py
 modAL/cluster.py
 modAL/density.py
 modAL/disagreement.py
+modAL/expected_error.py
 modAL/multilabel.py
 modAL/uncertainty.py
 modAL/models/__init__.py
 modAL/models/base.py
 modAL/models/learners.py
 modAL/utils/__init__.py
 modAL/utils/combination.py
```

