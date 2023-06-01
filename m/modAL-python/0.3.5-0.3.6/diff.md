# Comparing `tmp/modAL-python-0.3.5.tar.gz` & `tmp/modAL-python-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modAL-python-0.3.5.tar", last modified: Thu Jun  1 10:54:53 2023, max compression
+gzip compressed data, was "modAL-python-0.3.6.tar", last modified: Thu Jun  1 10:56:38 2023, max compression
```

## Comparing `modAL-python-0.3.5.tar` & `modAL-python-0.3.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:54:53.125193 modAL-python-0.3.5/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1070 2019-11-11 10:40:46.000000 modAL-python-0.3.5/LICENSE
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:54:53.125193 modAL-python-0.3.5/PKG-INFO
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10892 2019-11-11 10:40:46.000000 modAL-python-0.3.5/README.md
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:54:53.125193 modAL-python-0.3.5/modAL/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      128 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     5740 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/acquisition.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10891 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/batch.py
--rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/cluster.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1762 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/density.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     9195 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/disagreement.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3171 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/expected_error.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:54:53.125193 modAL-python-0.3.5/modAL/models/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      180 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/models/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    15148 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/models/base.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    20666 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/models/learners.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    11028 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/multilabel.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     8084 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/uncertainty.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:54:53.125193 modAL-python-0.3.5/modAL/utils/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      417 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/utils/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3651 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/utils/combination.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      787 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/utils/data.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     2389 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/utils/selection.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1920 2019-11-11 10:40:46.000000 modAL-python-0.3.5/modAL/utils/validation.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:54:53.125193 modAL-python-0.3.5/modAL_python.egg-info/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:54:53.000000 modAL-python-0.3.5/modAL_python.egg-info/PKG-INFO
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      583 2023-06-01 10:54:53.000000 modAL-python-0.3.5/modAL_python.egg-info/SOURCES.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        1 2023-06-01 10:54:53.000000 modAL-python-0.3.5/modAL_python.egg-info/dependency_links.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       43 2023-06-01 10:54:53.000000 modAL-python-0.3.5/modAL_python.egg-info/requires.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        6 2023-06-01 10:54:53.000000 modAL-python-0.3.5/modAL_python.egg-info/top_level.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       79 2023-06-01 10:54:53.125193 modAL-python-0.3.5/setup.cfg
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      478 2023-06-01 10:54:45.000000 modAL-python-0.3.5/setup.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:56:38.205052 modAL-python-0.3.6/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1070 2020-08-21 06:11:02.000000 modAL-python-0.3.6/LICENSE
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:56:38.205052 modAL-python-0.3.6/PKG-INFO
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10892 2020-08-21 06:11:02.000000 modAL-python-0.3.6/README.md
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:56:38.201052 modAL-python-0.3.6/modAL/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      128 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     5740 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/acquisition.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10891 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/batch.py
+-rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/cluster.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1762 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/density.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     9195 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/disagreement.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3171 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/expected_error.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:56:38.201052 modAL-python-0.3.6/modAL/models/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      180 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/models/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    15148 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/models/base.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    21572 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/models/learners.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    11028 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/multilabel.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     8084 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/uncertainty.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:56:38.205052 modAL-python-0.3.6/modAL/utils/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      417 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/utils/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3651 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/utils/combination.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      787 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/utils/data.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     2389 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/utils/selection.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1920 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/utils/validation.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:56:38.205052 modAL-python-0.3.6/modAL_python.egg-info/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:56:38.000000 modAL-python-0.3.6/modAL_python.egg-info/PKG-INFO
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      583 2023-06-01 10:56:38.000000 modAL-python-0.3.6/modAL_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        1 2023-06-01 10:56:38.000000 modAL-python-0.3.6/modAL_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       43 2023-06-01 10:56:38.000000 modAL-python-0.3.6/modAL_python.egg-info/requires.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        6 2023-06-01 10:56:38.000000 modAL-python-0.3.6/modAL_python.egg-info/top_level.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       79 2023-06-01 10:56:38.205052 modAL-python-0.3.6/setup.cfg
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      478 2023-06-01 10:56:30.000000 modAL-python-0.3.6/setup.py
```

### Comparing `modAL-python-0.3.5/LICENSE` & `modAL-python-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/README.md` & `modAL-python-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/acquisition.py` & `modAL-python-0.3.6/modAL/acquisition.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/batch.py` & `modAL-python-0.3.6/modAL/batch.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/density.py` & `modAL-python-0.3.6/modAL/density.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/disagreement.py` & `modAL-python-0.3.6/modAL/disagreement.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/expected_error.py` & `modAL-python-0.3.6/modAL/expected_error.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/models/base.py` & `modAL-python-0.3.6/modAL/models/base.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/models/learners.py` & `modAL-python-0.3.6/modAL/models/learners.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
             Useful when building Committee models with bagging.
         **fit_kwargs: keyword arguments.
 
     Attributes:
         estimator: The estimator to be used in the active learning loop.
         query_strategy: Function providing the query strategy for the active learning loop.
         X_training: If the model hasn't been fitted yet it is None, otherwise it contains the samples
-            which the model has been trained on.
+            which the model has been trained on. If provided, the method fit() of estimator is called during __init__()
         y_training: The labels corresponding to X_training.
 
     Examples:
 
         >>> from sklearn.datasets import load_iris
         >>> from sklearn.ensemble import RandomForestClassifier
         >>> from modAL.models import ActiveLearner
@@ -307,14 +307,28 @@
             np.concatenate(known_classes, axis=0),
             axis=0
         )
         self.n_classes_ = len(self.classes_)
 
     def _add_training_data(self, X: modALinput, y: modALinput):
         super()._add_training_data(X, y)
+
+    def teach(self, X: modALinput, y: modALinput, bootstrap: bool = False, only_new: bool = False, **fit_kwargs) -> None:
+        """
+        Adds X and y to the known training data for each learner and retrains learners with the augmented dataset.
+
+        Args:
+            X: The new samples for which the labels are supplied by the expert.
+            y: Labels corresponding to the new instances in X.
+            bootstrap: If True, trains each learner on a bootstrapped set. Useful when building the ensemble by bagging.
+            only_new: If True, the model is retrained using only X and y, ignoring the previously provided examples.
+            **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
+        """
+
+        super().teach(X, y, bootstrap=bootstrap, only_new=only_new, **fit_kwargs)
         self._set_classes()
 
     def predict(self, X: modALinput, **predict_proba_kwargs) -> Any:
         """
         Predicts the class of the samples by picking the consensus prediction.
 
         Args:
@@ -499,8 +513,8 @@
             The predicted value for each regressor in the CommitteeRegressor and each sample in X.
         """
         prediction = np.zeros(shape=(len(X), len(self.learner_list)))
 
         for learner_idx, learner in enumerate(self.learner_list):
             prediction[:, learner_idx] = learner.predict(X, **predict_kwargs).reshape(-1, )
 
-        return prediction
+        return prediction
```

### Comparing `modAL-python-0.3.5/modAL/multilabel.py` & `modAL-python-0.3.6/modAL/multilabel.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/uncertainty.py` & `modAL-python-0.3.6/modAL/uncertainty.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/utils/combination.py` & `modAL-python-0.3.6/modAL/utils/combination.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/utils/data.py` & `modAL-python-0.3.6/modAL/utils/data.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/utils/selection.py` & `modAL-python-0.3.6/modAL/utils/selection.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL/utils/validation.py` & `modAL-python-0.3.6/modAL/utils/validation.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.5/modAL_python.egg-info/SOURCES.txt` & `modAL-python-0.3.6/modAL_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

