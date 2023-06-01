# Comparing `tmp/modAL-python-0.4.0.tar.gz` & `tmp/modAL-python-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modAL-python-0.4.0.tar", last modified: Thu Jun  1 10:58:25 2023, max compression
+gzip compressed data, was "modAL-python-0.4.1.tar", last modified: Thu Jun  1 11:00:00 2023, max compression
```

## Comparing `modAL-python-0.4.0.tar` & `modAL-python-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:58:25.092908 modAL-python-0.4.0/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1070 2020-11-01 08:39:01.000000 modAL-python-0.4.0/LICENSE
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:58:25.092908 modAL-python-0.4.0/PKG-INFO
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10828 2020-11-01 08:39:01.000000 modAL-python-0.4.0/README.md
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:58:25.092908 modAL-python-0.4.0/modAL/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      128 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     5560 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/acquisition.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10985 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/batch.py
--rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/cluster.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1762 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/density.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     8883 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/disagreement.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3071 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/expected_error.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:58:25.092908 modAL-python-0.4.0/modAL/models/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      180 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/models/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    19706 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/models/base.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    23061 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/models/learners.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10447 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/multilabel.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     7850 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/uncertainty.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:58:25.092908 modAL-python-0.4.0/modAL/utils/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      417 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/utils/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3607 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/utils/combination.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     4725 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/utils/data.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     2389 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/utils/selection.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1920 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/utils/validation.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:58:25.092908 modAL-python-0.4.0/modAL_python.egg-info/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:58:25.000000 modAL-python-0.4.0/modAL_python.egg-info/PKG-INFO
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      583 2023-06-01 10:58:25.000000 modAL-python-0.4.0/modAL_python.egg-info/SOURCES.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        1 2023-06-01 10:58:25.000000 modAL-python-0.4.0/modAL_python.egg-info/dependency_links.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       57 2023-06-01 10:58:25.000000 modAL-python-0.4.0/modAL_python.egg-info/requires.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        6 2023-06-01 10:58:25.000000 modAL-python-0.4.0/modAL_python.egg-info/top_level.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       79 2023-06-01 10:58:25.092908 modAL-python-0.4.0/setup.cfg
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      495 2023-06-01 10:58:19.000000 modAL-python-0.4.0/setup.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 11:00:00.576779 modAL-python-0.4.1/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1070 2021-01-07 09:40:40.000000 modAL-python-0.4.1/LICENSE
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 11:00:00.576779 modAL-python-0.4.1/PKG-INFO
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10828 2021-01-07 09:40:40.000000 modAL-python-0.4.1/README.md
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 11:00:00.576779 modAL-python-0.4.1/modAL/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      128 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     5560 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/acquisition.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    11062 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/batch.py
+-rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/cluster.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1762 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/density.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     8825 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/disagreement.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3071 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/expected_error.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 11:00:00.576779 modAL-python-0.4.1/modAL/models/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      180 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/models/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    19137 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/models/base.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    23061 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/models/learners.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10447 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/multilabel.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     7850 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/uncertainty.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 11:00:00.576779 modAL-python-0.4.1/modAL/utils/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      417 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/utils/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3607 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/utils/combination.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     4725 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/utils/data.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     2389 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/utils/selection.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1920 2021-01-07 09:40:40.000000 modAL-python-0.4.1/modAL/utils/validation.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 11:00:00.576779 modAL-python-0.4.1/modAL_python.egg-info/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 11:00:00.000000 modAL-python-0.4.1/modAL_python.egg-info/PKG-INFO
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      583 2023-06-01 11:00:00.000000 modAL-python-0.4.1/modAL_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        1 2023-06-01 11:00:00.000000 modAL-python-0.4.1/modAL_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       57 2023-06-01 11:00:00.000000 modAL-python-0.4.1/modAL_python.egg-info/requires.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        6 2023-06-01 11:00:00.000000 modAL-python-0.4.1/modAL_python.egg-info/top_level.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       79 2023-06-01 11:00:00.576779 modAL-python-0.4.1/setup.cfg
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      495 2023-06-01 10:59:44.000000 modAL-python-0.4.1/setup.py
```

### Comparing `modAL-python-0.4.0/LICENSE` & `modAL-python-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/README.md` & `modAL-python-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL/acquisition.py` & `modAL-python-0.4.1/modAL/acquisition.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL/batch.py` & `modAL-python-0.4.1/modAL/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from typing import Callable, Optional, Tuple, Union
 
 import numpy as np
 import scipy.sparse as sp
 from sklearn.metrics.pairwise import pairwise_distances, pairwise_distances_argmin_min
 
-from modAL.utils.data import data_vstack, modALinput
+from modAL.utils.data import data_vstack, modALinput, data_shape
 from modAL.models.base import BaseCommittee, BaseLearner
 from modAL.uncertainty import classifier_uncertainty
 
 
 def select_cold_start_instance(X: modALinput,
                                metric: Union[str, Callable],
                                n_jobs: Union[int, None]) -> Tuple[int, modALinput]:
@@ -146,16 +146,18 @@
     # transform unlabeled data if needed
     if classifier.on_transformed:
         unlabeled = classifier.transform_without_estimating(unlabeled)
 
     if classifier.X_training is None:
         best_coldstart_instance_index, labeled = select_cold_start_instance(X=unlabeled, metric=metric, n_jobs=n_jobs)
         instance_index_ranking = [best_coldstart_instance_index]
-    elif classifier.X_training.shape[0] > 0:
-        labeled = classifier.Xt_training[:] if classifier.on_transformed else classifier.X_training[:]
+    elif data_shape(classifier.X_training)[0] > 0:
+        labeled = classifier.transform_without_estimating(
+            classifier.X_training
+        ) if classifier.on_transformed else classifier.X_training[:]
         instance_index_ranking = []
     
     # The maximum number of records to sample.
     ceiling = np.minimum(unlabeled.shape[0], n_instances) - len(instance_index_ranking)
 
     # mask for unlabeled initialized as transparent
     mask = np.ones(unlabeled.shape[0], np.bool)
```

### Comparing `modAL-python-0.4.0/modAL/density.py` & `modAL-python-0.4.1/modAL/density.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL/disagreement.py` & `modAL-python-0.4.1/modAL/disagreement.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,24 +31,22 @@
     n_learners = len(committee)
     try:
         votes = committee.vote(X, **predict_proba_kwargs)
     except NotFittedError:
         return np.zeros(shape=(X.shape[0],))
 
     p_vote = np.zeros(shape=(X.shape[0], len(committee.classes_)))
-    entr = np.zeros(shape=(X.shape[0],))
 
     for vote_idx, vote in enumerate(votes):
         vote_counter = Counter(vote)
 
         for class_idx, class_label in enumerate(committee.classes_):
             p_vote[vote_idx, class_idx] = vote_counter[class_label]/n_learners
 
-        entr[vote_idx] = entropy(p_vote[vote_idx])
-
+    entr = entropy(p_vote, axis=1)
     return entr
 
 
 def consensus_entropy(committee: BaseCommittee, X: modALinput, **predict_proba_kwargs) -> np.ndarray:
     """
     Calculates the consensus entropy for the Committee. First it computes the class probabilties of X for each learner
     in the Committee, then calculates the consensus probability distribution by averaging the individual class
```

### Comparing `modAL-python-0.4.0/modAL/expected_error.py` & `modAL-python-0.4.1/modAL/expected_error.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL/models/base.py` & `modAL-python-0.4.1/modAL/models/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,19 +62,17 @@
         assert callable(query_strategy), 'query_strategy must be callable'
 
         self.estimator = estimator
         self.query_strategy = query_strategy
         self.on_transformed = on_transformed
 
         self.X_training = X_training
-        self.Xt_training = None
         self.y_training = y_training
         if X_training is not None:
             self._fit_to_known(bootstrap=bootstrap_init, **fit_kwargs)
-            self.Xt_training = self.transform_without_estimating(self.X_training) if self.on_transformed else None
 
         assert isinstance(force_all_finite, bool), 'force_all_finite must be a bool'
         self.force_all_finite = force_all_finite
 
     def _add_training_data(self, X: modALinput, y: modALinput) -> None:
         """
         Adds the new data and label to the known data, but does not retrain the model.
@@ -88,23 +86,18 @@
             classifier has seen.
         """
         check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
                   force_all_finite=self.force_all_finite)
 
         if self.X_training is None:
             self.X_training = X
-            self.Xt_training = self.transform_without_estimating(self.X_training) if self.on_transformed else None
             self.y_training = y
         else:
             try:
                 self.X_training = data_vstack((self.X_training, X))
-                self.Xt_training = data_vstack((
-                    self.Xt_training,
-                    self.transform_without_estimating(X)
-                )) if self.on_transformed else None
                 self.y_training = data_vstack((self.y_training, y))
             except ValueError:
                 raise ValueError('the dimensions of the new training data and label must'
                                  'agree with the training data and labels provided so far')
 
     def transform_without_estimating(self, X: modALinput) -> Union[np.ndarray, sp.csr_matrix]:
         """
@@ -209,15 +202,14 @@
 
         Returns:
             self
         """
         check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
                   force_all_finite=self.force_all_finite)
         self.X_training, self.y_training = X, y
-        self.Xt_training = self.transform_without_estimating(self.X_training) if self.on_transformed else None
         return self._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
 
     def predict(self, X: modALinput, **predict_kwargs) -> Any:
         """
         Estimator predictions for X. Interface with the predict method of the estimator.
 
         Args:
```

### Comparing `modAL-python-0.4.0/modAL/models/learners.py` & `modAL-python-0.4.1/modAL/models/learners.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL/multilabel.py` & `modAL-python-0.4.1/modAL/multilabel.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL/uncertainty.py` & `modAL-python-0.4.1/modAL/uncertainty.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL/utils/combination.py` & `modAL-python-0.4.1/modAL/utils/combination.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL/utils/data.py` & `modAL-python-0.4.1/modAL/utils/data.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL/utils/selection.py` & `modAL-python-0.4.1/modAL/utils/selection.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL/utils/validation.py` & `modAL-python-0.4.1/modAL/utils/validation.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.4.0/modAL_python.egg-info/SOURCES.txt` & `modAL-python-0.4.1/modAL_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

