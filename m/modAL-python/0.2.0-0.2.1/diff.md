# Comparing `tmp/modAL-python-0.2.0.tar.gz` & `tmp/modAL-python-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modAL-python-0.2.0.tar", last modified: Thu Jun  1 10:42:45 2023, max compression
+gzip compressed data, was "modAL-python-0.2.1.tar", last modified: Thu Jun  1 10:45:51 2023, max compression
```

## Comparing `modAL-python-0.2.0.tar` & `modAL-python-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:42:45.874158 modAL-python-0.2.0/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1070 2018-02-10 11:40:02.000000 modAL-python-0.2.0/LICENSE
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      293 2023-06-01 10:42:45.874158 modAL-python-0.2.0/PKG-INFO
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     9879 2018-02-10 11:40:02.000000 modAL-python-0.2.0/README.md
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:42:45.874158 modAL-python-0.2.0/modAL/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      887 2018-02-10 11:40:02.000000 modAL-python-0.2.0/modAL/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1707 2018-02-10 11:40:02.000000 modAL-python-0.2.0/modAL/density.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     8804 2018-02-10 11:40:02.000000 modAL-python-0.2.0/modAL/disagreement.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    27872 2018-02-10 11:40:02.000000 modAL-python-0.2.0/modAL/models.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     7510 2018-02-10 11:40:02.000000 modAL-python-0.2.0/modAL/uncertainty.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:42:45.874158 modAL-python-0.2.0/modAL/utils/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      214 2018-02-10 11:40:02.000000 modAL-python-0.2.0/modAL/utils/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     2649 2018-02-10 11:40:02.000000 modAL-python-0.2.0/modAL/utils/combination.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1430 2018-02-10 11:40:02.000000 modAL-python-0.2.0/modAL/utils/selection.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1875 2018-02-10 11:40:02.000000 modAL-python-0.2.0/modAL/utils/validation.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:42:45.874158 modAL-python-0.2.0/modAL_python.egg-info/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      293 2023-06-01 10:42:45.000000 modAL-python-0.2.0/modAL_python.egg-info/PKG-INFO
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      411 2023-06-01 10:42:45.000000 modAL-python-0.2.0/modAL_python.egg-info/SOURCES.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        1 2023-06-01 10:42:45.000000 modAL-python-0.2.0/modAL_python.egg-info/dependency_links.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       43 2023-06-01 10:42:45.000000 modAL-python-0.2.0/modAL_python.egg-info/requires.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        6 2023-06-01 10:42:45.000000 modAL-python-0.2.0/modAL_python.egg-info/top_level.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       79 2023-06-01 10:42:45.874158 modAL-python-0.2.0/setup.cfg
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      451 2023-06-01 10:39:39.000000 modAL-python-0.2.0/setup.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:45:51.405913 modAL-python-0.2.1/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1070 2018-04-17 12:50:54.000000 modAL-python-0.2.1/LICENSE
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      293 2023-06-01 10:45:51.405913 modAL-python-0.2.1/PKG-INFO
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     9969 2018-04-17 12:50:54.000000 modAL-python-0.2.1/README.md
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:45:51.405913 modAL-python-0.2.1/modAL/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      887 2018-04-17 12:50:54.000000 modAL-python-0.2.1/modAL/__init__.py
+-rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2018-04-17 12:50:54.000000 modAL-python-0.2.1/modAL/cluster.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1707 2018-04-17 12:50:54.000000 modAL-python-0.2.1/modAL/density.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     8784 2018-04-17 12:50:54.000000 modAL-python-0.2.1/modAL/disagreement.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    30114 2018-04-17 12:50:54.000000 modAL-python-0.2.1/modAL/models.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     7500 2018-04-17 12:50:54.000000 modAL-python-0.2.1/modAL/uncertainty.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:45:51.405913 modAL-python-0.2.1/modAL/utils/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      214 2018-04-17 12:50:54.000000 modAL-python-0.2.1/modAL/utils/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     2965 2018-04-17 12:50:54.000000 modAL-python-0.2.1/modAL/utils/combination.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1529 2018-04-17 12:50:54.000000 modAL-python-0.2.1/modAL/utils/selection.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1875 2018-04-17 12:50:54.000000 modAL-python-0.2.1/modAL/utils/validation.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:45:51.405913 modAL-python-0.2.1/modAL_python.egg-info/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      293 2023-06-01 10:45:51.000000 modAL-python-0.2.1/modAL_python.egg-info/PKG-INFO
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      428 2023-06-01 10:45:51.000000 modAL-python-0.2.1/modAL_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        1 2023-06-01 10:45:51.000000 modAL-python-0.2.1/modAL_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       43 2023-06-01 10:45:51.000000 modAL-python-0.2.1/modAL_python.egg-info/requires.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        6 2023-06-01 10:45:51.000000 modAL-python-0.2.1/modAL_python.egg-info/top_level.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       79 2023-06-01 10:45:51.405913 modAL-python-0.2.1/setup.cfg
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      451 2023-06-01 10:45:28.000000 modAL-python-0.2.1/setup.py
```

### Comparing `modAL-python-0.2.0/LICENSE` & `modAL-python-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `modAL-python-0.2.0/README.md` & `modAL-python-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -19,19 +19,23 @@
 
 # Introduction<a name="introduction"></a>
 modAL is an active learning framework for Python3, designed with *modularity, flexibility* and *extensibility* in mind. Built on top of scikit-learn, it allows you to rapidly create active learning workflows with nearly complete freedom. What is more, you can easily replace parts with your custom built solutions, allowing you to design novel algorithms with ease.
 
 # Active learning from bird's-eye view<a name="active-learning"></a>
 With the recent explosion of available data, you have can have millions of unlabelled examples with a high cost to obtain labels. For instance, when trying to predict the sentiment of tweets, obtaining a training set can require immense manual labour. But worry not, active learning comes to the rescue! In general, AL is a framework allowing you to increase classification performance by intelligently querying you to label the most informative instances. To give an example, suppose that you have the following data and classifier with shaded regions signifying the classification probability.
 
-<img src="https://cosmic-cortex.github.io/modAL/img/motivating-example.png" height="600px" width="600px"/>
+<p align="center">
+  <img src="https://cosmic-cortex.github.io/modAL/img/motivating-example.png" height="600px" width="600px"/>
+</p>
 
 Suppose that you can query the label of an unlabelled instance, but it costs you a lot. Which one would you choose? By querying an instance in the uncertain region, surely you obtain more information than querying by random. Active learning gives you a set of tools to handle problems like this. In general, an active learning workflow looks like the following.
 
-![active-learning](https://cosmic-cortex.github.io/modAL/img/active_learning.png)
+<p align="center">
+ <img src="https://cosmic-cortex.github.io/modAL/img/active_learning.png"/>
+</p>
 
 The key components of any workflow are the **model** you choose, the **uncertainty** measure you use and the **query** strategy you apply to request labels. With modAL, instead of choosing from a small set of built-in components, you have the freedom to seamlessly integrate scikit-learn or Keras models into your algorithm and easily tailor your custom query strategies and uncertainty measures.
 
 # modAL in action<a name="modAL-in-action"></a>
 Let's see what modAL can do for you!
 
 ## From zero to one in a few lines of code<a name="initialization"></a>
@@ -118,28 +122,31 @@
 regressor = ActiveLearner(
     estimator=GaussianProcessRegressor(kernel=kernel),
     query_strategy=GP_regression_std,
     X_training=X_training.reshape(-1, 1), y_training=y_training.reshape(-1, 1)
 )
 ```
 The initial regressor is not very accurate.
-
-![gp-initial](https://cosmic-cortex.github.io/modAL/img/gp-initial.png)
+<p align="center">
+  <img src="https://cosmic-cortex.github.io/modAL/img/gp-initial.png">
+</p>
 
 The blue band enveloping the regressor represents the standard deviation of the Gaussian process at the given point. Now we are ready to do active learning!
 ```python
 # active learning
 n_queries = 10
 for idx in range(n_queries):
     query_idx, query_instance = regressor.query(X)
     regressor.teach(X[query_idx].reshape(1, -1), y[query_idx].reshape(1, -1))
 ```
 After a few queries, we can see that the prediction is much improved.
 
-![gp-final](https://cosmic-cortex.github.io/modAL/img/gp-final.png)
+<p align="center">
+ <img src="https://cosmic-cortex.github.io/modAL/img/gp-final.png">
+</p>
 
 ## Additional examples<a name="additional-examples"></a>
 Including this, many examples are available:
 - [Pool-based sampling](https://cosmic-cortex.github.io/modAL/Pool-based-sampling)  
 - [Stream-based sampling](https://cosmic-cortex.github.io/modAL/Stream-based-sampling)  
 - [Active regression](https://cosmic-cortex.github.io/modAL/Active-regression)  
 - [Ensemble regression](https://cosmic-cortex.github.io/modAL/Ensemble-regression)
```

### Comparing `modAL-python-0.2.0/modAL/__init__.py` & `modAL-python-0.2.1/modAL/__init__.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.2.0/modAL/density.py` & `modAL-python-0.2.1/modAL/density.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.2.0/modAL/disagreement.py` & `modAL-python-0.2.1/modAL/disagreement.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,15 +147,15 @@
         Keyword arguments to be passed for the disagreement measure function.
 
     Returns
     -------
     query_idx: numpy.ndarray of shape (n_instances, )
         The indices of the instances from X_pool chosen to be labelled.
 
-    X_pool[query_idx]: numpy.ndarray of shape (n_instances, n_features)
+    X[query_idx]: numpy.ndarray of shape (n_instances, n_features)
         The instances from X_pool chosen to be labelled.
     """
     disagreement = vote_entropy(committee, X, **disagreement_measure_kwargs)
     query_idx = multi_argmax(disagreement, n_instances=n_instances)
 
     return query_idx, X[query_idx]
 
@@ -179,15 +179,15 @@
         Keyword arguments to be passed for the disagreement measure function.
 
     Returns
     -------
     query_idx: numpy.ndarray of shape (n_instances, )
         The indices of the instances from X_pool chosen to be labelled.
 
-    X_pool[query_idx]: numpy.ndarray of shape (n_instances, n_features)
+    X[query_idx]: numpy.ndarray of shape (n_instances, n_features)
         The instances from X_pool chosen to be labelled.
     """
     disagreement = consensus_entropy(committee, X, **disagreement_measure_kwargs)
     query_idx = multi_argmax(disagreement, n_instances=n_instances)
 
     return query_idx, X[query_idx]
 
@@ -211,15 +211,15 @@
         Keyword arguments to be passed for the disagreement measure function.
 
     Returns
     -------
     query_idx: numpy.ndarray of shape (n_instances, )
         The indices of the instances from X_pool chosen to be labelled.
 
-    X_pool[query_idx]: numpy.ndarray of shape (n_instances, n_features)
+    X[query_idx]: numpy.ndarray of shape (n_instances, n_features)
         The instances from X_pool chosen to be labelled.
     """
     disagreement = KL_max_disagreement(committee, X, **disagreement_measure_kwargs)
     query_idx = multi_argmax(disagreement, n_instances=n_instances)
 
     return query_idx, X[query_idx]
 
@@ -240,14 +240,14 @@
         Keyword arguments to be passed for the predict method.
 
     Returns
     -------
     query_idx: numpy.ndarray of shape (n_instances, )
         The indices of the instances from X_pool chosen to be labelled.
 
-    X_pool[query_idx]: numpy.ndarray of shape (n_instances, n_features)
+    X[query_idx]: numpy.ndarray of shape (n_instances, n_features)
         The instances from X_pool chosen to be labelled.
     """
     _, std = regressor.predict(X, return_std=True, **predict_kwargs)
     std = std.reshape(len(X), )
     query_idx = multi_argmax(std, n_instances=n_instances)
     return query_idx, X[query_idx]
```

### Comparing `modAL-python-0.2.0/modAL/models.py` & `modAL-python-0.2.1/modAL/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,29 @@
 """
-Core models for active learning algorithms.
+==========================================
+Core models for active learning algorithms
+==========================================
 """
 
+import abc
+import sys
 import numpy as np
-from abc import ABC, abstractmethod
-from sklearn.utils import check_array
+
 from sklearn.base import BaseEstimator
 from modAL.utils.validation import check_class_labels, check_class_proba
 from modAL.uncertainty import uncertainty_sampling
 from modAL.disagreement import vote_entropy_sampling, max_std_sampling
 
 
+if sys.version_info >= (3, 4):
+    ABC = abc.ABC
+else:
+    ABC = abc.ABCMeta('ABC', (), {})
+
+
 class ActiveLearner(BaseEstimator):
     """
     This class is an abstract model of a general active learning algorithm.
 
     Parameters
     ----------
     estimator: scikit-learn estimator
@@ -97,16 +106,16 @@
         self.estimator = estimator
         self.query_strategy = query_strategy
 
         if type(X_training) == type(None) and type(y_training) == type(None):
             self.X_training = None
             self.y_training = None
         elif type(X_training) != type(None) and type(y_training) != type(None):
-            self.X_training = check_array(X_training)
-            self.y_training = check_array(y_training, ensure_2d=False)
+            self.X_training = X_training
+            self.y_training = y_training
             self._fit_to_known(bootstrap=bootstrap_init, **fit_kwargs)
 
     def _add_training_data(self, X, y):
         """
         Adds the new data and label to the known data, but does
         not retrain the model.
 
@@ -121,15 +130,14 @@
 
         Note
         ----
         If the classifier has been fitted, the features in X
         have to agree with the training samples which the
         classifier has seen.
         """
-        X, y = check_array(X), check_array(y, ensure_2d=False)
         assert len(X) == len(y), 'the number of new data points and number of labels must match'
 
         if type(self.X_training) != type(None):
             try:
                 self.X_training = np.vstack((self.X_training, X))
                 self.y_training = np.concatenate((self.y_training, y))
             except ValueError:
@@ -158,14 +166,43 @@
             return self
         else:
             n_instances = len(self.X_training)
             bootstrap_idx = np.random.choice(range(n_instances), n_instances, replace=True)
             self.estimator.fit(self.X_training[bootstrap_idx], self.y_training[bootstrap_idx], **fit_kwargs)
             return self
 
+    def _fit_on_new(self, X, y, bootstrap=False, **fit_kwargs):
+        """
+        Fits self.estimator to the given data and labels.
+
+        Parameters
+        ----------
+        X: numpy.ndarray of shape (n_samples, n_features)
+            The new samples for which the labels are supplied
+            by the expert.
+
+        y: numpy.ndarray of shape (n_samples, )
+            Labels corresponding to the new instances in X.
+
+        bootstrap: boolean
+            If True, the method trains the model on a set bootstrapped from X.
+
+        fit_kwargs: keyword arguments
+            Keyword arguments to be passed to the fit method of the predictor.
+        """
+        assert len(X) == len(y), 'the length of X and y must match'
+
+        if not bootstrap:
+            self.estimator.fit(X, y, **fit_kwargs)
+            return self
+        else:
+            bootstrap_idx = np.random.choice(range(len(X)), len(X), replace=True)
+            self.estimator.fit(X[bootstrap_idx], y[bootstrap_idx])
+            return self
+
     def fit(self, X, y, bootstrap=False, **fit_kwargs):
         """
         Interface for the fit method of the predictor. Fits the predictor
         to the supplied data, then stores it internally for the active
         learning loop.
 
         Parameters
@@ -253,15 +290,14 @@
         -------
         query_idx: numpy.ndarray of shape (n_instances, )
             The indices of the instances from X_pool chosen to be labelled.
 
         X[query_idx]: numpy.ndarray of shape (n_instances, n_features)
             The instances from X_pool chosen to be labelled.
         """
-        check_array(X, ensure_2d=True)
 
         query_idx, query_instances = self.query_strategy(self.estimator, X, **query_kwargs)
         return query_idx, query_instances
 
     def score(self, X, y, **score_kwargs):
         """
         Interface for the score method of the predictor.
@@ -280,15 +316,15 @@
 
         Returns
         -------
         mean_accuracy: numpy.float containing the mean accuracy of the predictor
         """
         return self.estimator.score(X, y, **score_kwargs)
 
-    def teach(self, X, y, bootstrap=False, **fit_kwargs):
+    def teach(self, X, y, bootstrap=False, only_new=False, **fit_kwargs):
         """
         Adds X and y to the known training data and retrains the predictor
         with the augmented dataset.
 
         Parameters
         ----------
         X: numpy.ndarray of shape (n_samples, n_features)
@@ -298,23 +334,31 @@
         y: numpy.ndarray of shape (n_samples, )
             Labels corresponding to the new instances in X.
 
         bootstrap: boolean
             If True, training is done on a bootstrapped dataset. Useful for building
             Committee models with bagging.
 
+        only_new: boolean
+            If True, the model is retrained using only X and y, ignoring the previously
+            provided examples. Useful when working with models where the .fit() method
+            doesn't retrain the model from scratch. (For example, in tensorflow or keras.)
+
         fit_kwargs: keyword arguments
             Keyword arguments to be passed to the fit method
             of the predictor.
         """
         self._add_training_data(X, y)
-        self._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
+        if not only_new:
+            self._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
+        else:
+            self._fit_on_new(X, y, bootstrap=bootstrap, **fit_kwargs)
 
 
-class BaseCommittee(ABC):
+class BaseCommittee(ABC, BaseEstimator):
     def __init__(
             self,
             learner_list,                                        # list of ActiveLearner objects
             query_strategy                                       # callable to query labels
 
     ):
         assert type(learner_list) == list, 'learners must be supplied in a list'
@@ -364,14 +408,38 @@
 
         fit_kwargs: keyword arguments
             Keyword arguments to be passed to the fit method of the predictor.
         """
         for learner in self.learner_list:
             learner._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
 
+    def _fit_on_new(self, X, y, bootstrap=False, **fit_kwargs):
+        """
+        Fits all learners to the given data and labels.
+
+        Parameters
+        ----------
+        X: numpy.ndarray of shape (n_samples, n_features)
+            The new samples for which the labels are supplied
+            by the expert.
+
+        y: numpy.ndarray of shape (n_samples, )
+            Labels corresponding to the new instances in X.
+
+        bootstrap: boolean
+            If True, the method trains the model on a set bootstrapped from X.
+
+        fit_kwargs: keyword arguments
+            Keyword arguments to be passed to the fit method of the predictor.
+        """
+        assert len(X) == len(y), 'the length of X and y must match'
+
+        for learner in self.learner_list:
+            learner._fit_on_new(X, y, bootstrap=bootstrap, **fit_kwargs)
+
     def fit(self, X, y, **fit_kwargs):
         """
         Fits every learner to a subset sampled with replacement from X.
         Calling this method makes the learner forget the data it has seen up until this point and
         replaces it with X! If you would like to perform bootstrapping on each learner using the
         data it has seen, use the method .rebag()!
 
@@ -412,16 +480,14 @@
         -------
         query_idx: numpy.ndarray of shape (n_instances, )
             The indices of the instances from X_pool chosen to be labelled.
 
         X[query_idx]: numpy.ndarray of shape (n_instances, n_features)
             The instances from X_pool chosen to be labelled.
         """
-        check_array(X, ensure_2d=True)
-
         query_idx, query_instances = self.query_strategy(self, X, **query_kwargs)
         return query_idx, X[query_idx]
 
     def rebag(self, **fit_kwargs):
         """
         Refits every learner with a dataset bootstrapped from its training instances. Contrary to
         .bag(), it bootstraps the training data for each learner based on its own examples.
@@ -429,15 +495,15 @@
         Parameters
         ----------
         fit_kwargs: keyword arguments
             Keyword arguments to be passed to the fit method of the predictor.
         """
         self._fit_to_known(bootstrap=True, **fit_kwargs)
 
-    def teach(self, X, y, bootstrap=False, **fit_kwargs):
+    def teach(self, X, y, bootstrap=False, only_new=False, **fit_kwargs):
         """
         Adds X and y to the known training data for each learner
         and retrains learners with the augmented dataset.
 
         Parameters
         ----------
         X: numpy.ndarray of shape (n_samples, n_features)
@@ -452,26 +518,29 @@
             when building the ensemble by bagging.
 
         fit_kwargs: keyword arguments
             Keyword arguments to be passed to the fit method
             of the predictor.
         """
         self._add_training_data(X, y)
-        self._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
+        if not only_new:
+            self._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
+        else:
+            self._fit_on_new(X, y, bootstrap=bootstrap, **fit_kwargs)
 
-    @abstractmethod
+    @abc.abstractmethod
     def predict(self, X):
         pass
 
-    @abstractmethod
+    @abc.abstractmethod
     def vote(self, X):
         pass
 
 
-class Committee(BaseCommittee, BaseEstimator):
+class Committee(BaseCommittee):
     """
     This class is an abstract model of a committee-based active learning algorithm.
 
     Parameters
     ----------
     learner_list: list
         A list of ActiveLearners forming the Committee.
@@ -612,15 +681,14 @@
 
         Returns
         -------
         vote: numpy.ndarray of shape (n_samples, n_learners)
             The predicted class for each learner in the Committee
             and each sample in X.
         """
-        check_array(X, ensure_2d=True)
         prediction = np.zeros(shape=(X.shape[0], len(self.learner_list)))
 
         for learner_idx, learner in enumerate(self.learner_list):
             prediction[:, learner_idx] = learner.predict(X, **predict_kwargs)
 
         return prediction
 
@@ -639,16 +707,14 @@
         Returns
         -------
         vote_proba: numpy.ndarray of shape (n_samples, n_learners, n_classes)
             Probabilities of each class for each learner and each instance.
 
         """
 
-        check_array(X, ensure_2d=True)
-
         # get dimensions
         n_samples = X.shape[0]
         n_learners = len(self.learner_list)
         proba = np.zeros(shape=(n_samples, n_learners, self.n_classes_))
 
         # checking if the learners in the Committee know the same set of class labels
         if check_class_labels(*[learner.estimator for learner in self.learner_list]):
@@ -665,15 +731,15 @@
                     known_labels=learner.estimator.classes_,
                     all_labels=self.classes_
                 )
 
         return proba
 
 
-class CommitteeRegressor(BaseCommittee, BaseEstimator):
+class CommitteeRegressor(BaseCommittee):
     """
     This class is an abstract model of a committee-based active learning regression.
 
     Parameters
     ----------
     learner_list: list
         A list of ActiveLearners forming the CommitteeRegressor.
@@ -768,15 +834,14 @@
             Keyword arguments to be passed for the learners .predict() method.
 
         Returns
         -------
         vote: numpy.ndarray of shape (n_samples, n_regressors)
             The predicted value for each regressor in the CommitteeRegressor and each sample in X.
         """
-        check_array(X, ensure_2d=True)
         prediction = np.zeros(shape=(len(X), len(self.learner_list)))
 
         for learner_idx, learner in enumerate(self.learner_list):
             prediction[:, learner_idx] = learner.predict(X, **predict_kwargs).reshape(-1, )
 
         return prediction
```

### Comparing `modAL-python-0.2.0/modAL/uncertainty.py` & `modAL-python-0.2.1/modAL/uncertainty.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         Keyword arguments to be passed for the uncertainty measure function.
 
     Returns
     -------
     query_idx: numpy.ndarray of shape (n_instances, )
         The indices of the instances from X_pool chosen to be labelled.
 
-    X_pool[query_idx]: numpy.ndarray of shape (n_instances, n_features)
+    X[query_idx]: numpy.ndarray of shape (n_instances, n_features)
         The instances from X_pool chosen to be labelled.
     """
     margin = classifier_margin(classifier, X, **uncertainty_measure_kwargs)
     query_idx = multi_argmax(-margin, n_instances=n_instances)
 
     return query_idx, X[query_idx]
 
@@ -195,14 +195,14 @@
         Keyword arguments to be passed for the uncertainty measure function.
 
     Returns
     -------
     query_idx: numpy.ndarray of shape (n_instances, )
         The indices of the instances from X_pool chosen to be labelled.
 
-    X_pool[query_idx]: numpy.ndarray of shape (n_instances, n_features)
+    X[query_idx]: numpy.ndarray of shape (n_instances, n_features)
         The instances from X_pool chosen to be labelled.
     """
     entropy = classifier_entropy(classifier, X, **uncertainty_measure_kwargs)
     query_idx = multi_argmax(entropy, n_instances=n_instances)
 
     return query_idx, X[query_idx]
```

### Comparing `modAL-python-0.2.0/modAL/utils/combination.py` & `modAL-python-0.2.1/modAL/utils/combination.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     if weights is None:
         weights = np.ones(shape=(len(functions)))
     else:
         assert len(functions) == len(weights), 'the length of weights must be the ' \
                                                'same as the number of given functions'
 
     def linear_combination(*args, **kwargs):
-        return np.sum([weights[i]*functions[i](*args, **kwargs)
-                       for i in range(len(weights))], axis=0)
+        return np.sum((weights[i]*functions[i](*args, **kwargs)
+                       for i in range(len(weights))), axis=0)
 
     return linear_combination
 
 
 def make_product(*functions, exponents=None):
     """
     Takes the given functions and makes a function which returns the product of the output
@@ -65,7 +65,18 @@
                                                  'same as the number of given functions'
 
     def product_function(*args, **kwargs):
         return np.prod([functions[i](*args, **kwargs)**exponents[i]
                        for i in range(len(exponents))], axis=0)
 
     return product_function
+
+
+def make_query_strategy(utility_measure, selector):
+    # TODO: check for the signatures of utility_measure and selector
+
+    def query_strategy(classifier, X):
+        utility = utility_measure(classifier, X)
+        query_idx = selector(utility)
+        return query_idx, X[query_idx]
+
+    return query_strategy
```

### Comparing `modAL-python-0.2.0/modAL/utils/selection.py` & `modAL-python-0.2.1/modAL/utils/selection.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,10 +43,12 @@
 
     Returns
     -------
     random_idx: numpy.ndarray of shape = (n_instances, 1)
         n_instances random indices based on the weights.
     """
     assert n_instances <= len(weights), 'n_instances must be less or equal than the size of utility'
+    weight_sum = np.sum(weights)
+    assert weight_sum > 0, 'the sum of weights must be larger than zero'
 
-    random_idx = np.random.choice(range(len(weights)), size=n_instances, p=weights / np.sum(weights), replace=False)
+    random_idx = np.random.choice(range(len(weights)), size=n_instances, p=weights/weight_sum, replace=False)
     return random_idx
```

### Comparing `modAL-python-0.2.0/modAL/utils/validation.py` & `modAL-python-0.2.1/modAL/utils/validation.py`

 * *Files identical despite different names*

