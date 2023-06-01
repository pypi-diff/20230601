# Comparing `tmp/landmarkclassifier-2.0.5.tar.gz` & `tmp/landmarkclassifier-2.0.6.tar.gz`

## Comparing `landmarkclassifier-2.0.5.tar` & `landmarkclassifier-2.0.6.tar`

### file list

```diff
@@ -1,20 +1,23 @@
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/environment.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LANDMark/LANDMark.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LANDMark/__init__.py
--rw-r--r--   0        0        0    13597 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LANDMark/lm_base_clfs.py
--rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LANDMark/tree.py
--rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LANDMark/utils.py
--rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/docs/API.md
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/tests/__init__.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/tests/test_landmark.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/.gitignore
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LICENSE
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/environment.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     9153 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/LANDMark.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/__init__.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/lm_dtree_clfs.py
+-rw-r--r--   0        0        0     3700 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/lm_linear_clfs.py
+-rw-r--r--   0        0        0     3933 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/lm_nnet_clfs.py
+-rw-r--r--   0        0        0     1738 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/lm_oracle_clfs.py
+-rw-r--r--   0        0        0    24183 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/tree.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LANDMark/utils.py
+-rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/docs/API.md
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     3468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/tests/test_landmark.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/.gitignore
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/LICENSE
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/README.md
+-rw-r--r--   0        0        0     1959 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.6/PKG-INFO
```

### Comparing `landmarkclassifier-2.0.5/.github/ISSUE_TEMPLATE/bug_report.md` & `landmarkclassifier-2.0.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.5/.github/ISSUE_TEMPLATE/feature_request.md` & `landmarkclassifier-2.0.6/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.5/.github/workflows/ci.yml` & `landmarkclassifier-2.0.6/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.5/.github/workflows/python-publish.yml` & `landmarkclassifier-2.0.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.5/LANDMark/LANDMark.py` & `landmarkclassifier-2.0.6/LANDMark/LANDMark.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from __future__ import annotations
 
 import numpy as np
 
 from .utils import Ensemble
 from .tree import MTree
 
-from sklearn.base import ClassifierMixin, BaseEstimator, TransformerMixin
+from sklearn.base import ClassifierMixin, BaseEstimator
 from sklearn.metrics import balanced_accuracy_score
 from sklearn.utils import check_X_y
 from sklearn.utils.validation import check_is_fitted
 
-from typing import Optional
+from typing import Optional, List
 
 
 class LANDMarkClassifier(BaseEstimator, ClassifierMixin):
 
     def __init__(
         self,
         n_estimators: int = 64,
@@ -146,15 +146,15 @@
         for estimator in self.estimators_.estimators_:
             tree_mats.append(estimator.proximity(X))
 
         emb = np.hstack(tree_mats)
 
         return emb
 
-    def _check_params(self, X: np.ndarray, y: np.ndarray):
+    def _check_params(self, X: np.ndarray, y: np.ndarray) -> List[np.ndarray, np.ndarray]:
         SUPPORTED_IMPURITY = {"gain", "gain-ratio", "tsallis", "tsallis-gain-ratio"}
 
         # Check that X and y meet the minimum requirements
         X_conv, y_conv = check_X_y(X, y, accept_sparse=False)
 
         if not isinstance(self.n_estimators, int):
             raise TypeError("'n_estimators' must be an integer.")
@@ -224,22 +224,23 @@
 
         if isinstance(self.nnet_min_samples, int):
             if self.nnet_min_samples <= 0:
                 raise ValueError("'nnet_min_samples' must be greater than zero.")
 
         if not isinstance(self.use_etc, bool):
             raise TypeError("'use_etc' must be True or False.")
-
-        if not isinstance(self.etc_max_depth, int):
-            raise TypeError("'etc_max_depth' must be an integer.")
-
+            
         if isinstance(self.etc_max_depth, int):
             if self.etc_max_depth <= 0:
                 raise ValueError("'etc_max_depth' must be greater than zero.")
 
+        else:
+            if not isinstance(self.etc_max_depth, type(None)):
+                raise TypeError("'etc_max_depth' must be an integer.")
+
         if not isinstance(self.etc_max_trees, int):
             raise TypeError("'etc_max_trees' must be an integer.")
 
         if isinstance(self.etc_max_trees, int):
             if self.etc_max_trees <= 0:
                 raise ValueError("'etc_max_trees' must be greater than zero.")
```

### Comparing `landmarkclassifier-2.0.5/LANDMark/tree.py` & `landmarkclassifier-2.0.6/LANDMark/tree.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 from scipy.stats import entropy
 
 from random import choice
 
 from sklearn.base import ClassifierMixin, BaseEstimator, clone
 from sklearn.metrics import balanced_accuracy_score
 
-from .lm_base_clfs import (
-    LMClassifier,
-    RandomOracle,
-    ANNClassifier,
-    ETClassifier,
-)
+from .lm_linear_clfs import LMClassifier
+from .lm_oracle_clfs import RandomOracle
+from .lm_dtree_clfs import ETClassifier
+from .lm_nnet_clfs import ANNClassifier
 
 
 def tsallis_fun(N, N_lab, L, R, y, mode, q):
     if q == 1:  # Special case
         if "ratio" in mode.split("-"):
             return entropy_fun(N, N_lab, L, R, y, "gain-ratio")
 
@@ -252,16 +250,21 @@
                         LMClassifier(model_type="lsvc", n_feat=max_features),
                     ]:
                         model, D = clf.fit(X, y)
 
                         if D.ndim > 1:
                             D = D[:, self.c_choice]
 
-                        L = np.where(D > 0, True, False)
-                        R = np.where(D <= 0, True, False)
+                        if model.y_min > 6:
+                            L = np.where(D > 0, True, False)
+                            R = np.where(D <= 0, True, False)
+
+                        else:
+                            L = np.where(D > 0.5, True, False)
+                            R = np.where(D <= 0.5, True, False)
 
                         X_L_n = X[L].shape[0]
                         X_R_n = X[R].shape[0]
 
                         # Calculate Information Gain
                         if X_L_n > 0 and X_R_n > 0:
                             IG = purity_function(
@@ -279,16 +282,21 @@
                         LMClassifier(model_type="sgd_l1", n_feat=max_features),
                     ]:
                         model, D = clf.fit(X, y)
 
                         if D.ndim > 1:
                             D = D[:, self.c_choice]
 
-                        L = np.where(D > 0, True, False)
-                        R = np.where(D <= 0, True, False)
+                        if model.y_min > 6:
+                            L = np.where(D > 0, True, False)
+                            R = np.where(D <= 0, True, False)
+
+                        else:
+                            L = np.where(D > 0.5, True, False)
+                            R = np.where(D <= 0.5, True, False)
 
                         X_L_n = X[L].shape[0]
                         X_R_n = X[R].shape[0]
 
                         # Calculate Information Gain
                         if X_L_n > 0 and X_R_n > 0:
                             IG = purity_function(
@@ -547,14 +555,37 @@
 
                 if D.ndim > 1:
                     D = D[:, node.c_choice]
 
                 L = np.where(D > 0.5, True, False)
                 R = np.where(D <= 0.5, True, False)
 
+            elif type(node.splitter) == ETClassifier:
+                D = node.splitter.decision_function(X)
+
+                if D.ndim > 1:
+                    D = D[:, node.c_choice]
+
+                L = np.where(D > 0.5, True, False)
+                R = np.where(D <= 0.5, True, False)
+
+            elif type(node.splitter) == LMClassifier:
+                D = node.splitter.decision_function(X)
+
+                if D.ndim > 1:
+                    D = D[:, node.c_choice]
+
+                if node.splitter.y_min > 6:
+                    L = np.where(D > 0, True, False)
+                    R = np.where(D <= 0, True, False)
+
+                else:
+                    L = np.where(D > 0.5, True, False)
+                    R = np.where(D <= 0.5, True, False)
+
             else:
                 D = node.splitter.decision_function(X)
 
                 if D.ndim > 1:
                     D = D[:, node.c_choice]
 
                 L = np.where(D > 0, True, False)
@@ -629,14 +660,37 @@
 
                 if D.ndim > 1:
                     D = D[:, node.c_choice]
 
                 L = np.where(D > 0.5, True, False)
                 R = np.where(D <= 0.5, True, False)
 
+            elif type(node.splitter) == ETClassifier:
+                D = node.splitter.decision_function(X)
+
+                if D.ndim > 1:
+                    D = D[:, node.c_choice]
+
+                L = np.where(D > 0.5, True, False)
+                R = np.where(D <= 0.5, True, False)
+
+            elif type(node.splitter) == LMClassifier:
+                D = node.splitter.decision_function(X)
+
+                if D.ndim > 1:
+                    D = D[:, node.c_choice]
+
+                if node.splitter.y_min > 6:
+                    L = np.where(D > 0, True, False)
+                    R = np.where(D <= 0, True, False)
+
+                else:
+                    L = np.where(D > 0.5, True, False)
+                    R = np.where(D <= 0.5, True, False)
+
             else:
                 D = node.splitter.decision_function(X)
 
                 if D.ndim > 1:
                     D = D[:, node.c_choice]
 
                 L = np.where(D > 0, True, False)
```

### Comparing `landmarkclassifier-2.0.5/docs/API.md` & `landmarkclassifier-2.0.6/docs/API.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.5/docs/CONTRIBUTING.md` & `landmarkclassifier-2.0.6/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.5/.gitignore` & `landmarkclassifier-2.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.5/LICENSE` & `landmarkclassifier-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.5/README.md` & `landmarkclassifier-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.5/pyproject.toml` & `landmarkclassifier-2.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "LANDMarkClassifier"
-version = "2.0.5"
+version = "2.0.6"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "Teresita M. Porter"},
     {name = "Michael Wright"},
     {name = "G. Brian Golding"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
@@ -35,18 +35,18 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
 dependencies = [
     "numpy == 1.23.5",
     "scikit-learn >= 1.1.2",
     "joblib >= 1.2.0",
-    "tensorflow_addons >= 0.17.1",
-    "tensorflow >= 2.9.1",
     "pandas >= 1.5.0",
     "scipy >= 1.8.1",
+    "skorch >= 0.13.0",
+    "torch >= 2.0.1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/jrudar/LANDMark"
 "Repository" = "https://github.com/jrudar/LANDMark.git"
 "Bug Tracker" = "https://github.com/jrudar/LANDMark/issues"
```

### Comparing `landmarkclassifier-2.0.5/PKG-INFO` & `landmarkclassifier-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LANDMarkClassifier
-Version: 2.0.5
+Version: 2.0.6
 Summary: LANDMark: An ensemble approach to the supervised selection of biomarkers in high-throughput sequencing data
 Project-URL: Homepage, https://github.com/jrudar/LANDMark
 Project-URL: Repository, https://github.com/jrudar/LANDMark.git
 Project-URL: Bug Tracker, https://github.com/jrudar/LANDMark/issues
 Author: Teresita M. Porter, Michael Wright, G. Brian Golding
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
@@ -43,16 +43,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: joblib>=1.2.0
 Requires-Dist: numpy==1.23.5
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: scikit-learn>=1.1.2
 Requires-Dist: scipy>=1.8.1
-Requires-Dist: tensorflow-addons>=0.17.1
-Requires-Dist: tensorflow>=2.9.1
+Requires-Dist: skorch>=0.13.0
+Requires-Dist: torch>=2.0.1
 Provides-Extra: dev
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: ruff; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
```

