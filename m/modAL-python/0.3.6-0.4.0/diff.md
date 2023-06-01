# Comparing `tmp/modAL-python-0.3.6.tar.gz` & `tmp/modAL-python-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modAL-python-0.3.6.tar", last modified: Thu Jun  1 10:56:38 2023, max compression
+gzip compressed data, was "modAL-python-0.4.0.tar", last modified: Thu Jun  1 10:58:25 2023, max compression
```

## Comparing `modAL-python-0.3.6.tar` & `modAL-python-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:56:38.205052 modAL-python-0.3.6/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1070 2020-08-21 06:11:02.000000 modAL-python-0.3.6/LICENSE
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:56:38.205052 modAL-python-0.3.6/PKG-INFO
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10892 2020-08-21 06:11:02.000000 modAL-python-0.3.6/README.md
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:56:38.201052 modAL-python-0.3.6/modAL/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      128 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     5740 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/acquisition.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10891 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/batch.py
--rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/cluster.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1762 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/density.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     9195 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/disagreement.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3171 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/expected_error.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:56:38.201052 modAL-python-0.3.6/modAL/models/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      180 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/models/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    15148 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/models/base.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    21572 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/models/learners.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    11028 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/multilabel.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     8084 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/uncertainty.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:56:38.205052 modAL-python-0.3.6/modAL/utils/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      417 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/utils/__init__.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3651 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/utils/combination.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      787 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/utils/data.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     2389 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/utils/selection.py
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1920 2020-08-21 06:11:02.000000 modAL-python-0.3.6/modAL/utils/validation.py
-drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:56:38.205052 modAL-python-0.3.6/modAL_python.egg-info/
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:56:38.000000 modAL-python-0.3.6/modAL_python.egg-info/PKG-INFO
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      583 2023-06-01 10:56:38.000000 modAL-python-0.3.6/modAL_python.egg-info/SOURCES.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        1 2023-06-01 10:56:38.000000 modAL-python-0.3.6/modAL_python.egg-info/dependency_links.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       43 2023-06-01 10:56:38.000000 modAL-python-0.3.6/modAL_python.egg-info/requires.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        6 2023-06-01 10:56:38.000000 modAL-python-0.3.6/modAL_python.egg-info/top_level.txt
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       79 2023-06-01 10:56:38.205052 modAL-python-0.3.6/setup.cfg
--rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      478 2023-06-01 10:56:30.000000 modAL-python-0.3.6/setup.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:58:25.092908 modAL-python-0.4.0/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1070 2020-11-01 08:39:01.000000 modAL-python-0.4.0/LICENSE
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:58:25.092908 modAL-python-0.4.0/PKG-INFO
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10828 2020-11-01 08:39:01.000000 modAL-python-0.4.0/README.md
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:58:25.092908 modAL-python-0.4.0/modAL/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      128 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     5560 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/acquisition.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10985 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/batch.py
+-rwxr-xr-x   0 tivadar   (1000) tivadar   (1000)      416 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/cluster.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1762 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/density.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     8883 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/disagreement.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3071 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/expected_error.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:58:25.092908 modAL-python-0.4.0/modAL/models/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      180 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/models/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    19706 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/models/base.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    23061 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/models/learners.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)    10447 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/multilabel.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     7850 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/uncertainty.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:58:25.092908 modAL-python-0.4.0/modAL/utils/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      417 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/utils/__init__.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     3607 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/utils/combination.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     4725 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/utils/data.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     2389 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/utils/selection.py
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)     1920 2020-11-01 08:39:01.000000 modAL-python-0.4.0/modAL/utils/validation.py
+drwxrwxr-x   0 tivadar   (1000) tivadar   (1000)        0 2023-06-01 10:58:25.092908 modAL-python-0.4.0/modAL_python.egg-info/
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      289 2023-06-01 10:58:25.000000 modAL-python-0.4.0/modAL_python.egg-info/PKG-INFO
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      583 2023-06-01 10:58:25.000000 modAL-python-0.4.0/modAL_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        1 2023-06-01 10:58:25.000000 modAL-python-0.4.0/modAL_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       57 2023-06-01 10:58:25.000000 modAL-python-0.4.0/modAL_python.egg-info/requires.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)        6 2023-06-01 10:58:25.000000 modAL-python-0.4.0/modAL_python.egg-info/top_level.txt
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)       79 2023-06-01 10:58:25.092908 modAL-python-0.4.0/setup.cfg
+-rw-rw-r--   0 tivadar   (1000) tivadar   (1000)      495 2023-06-01 10:58:19.000000 modAL-python-0.4.0/setup.py
```

### Comparing `modAL-python-0.3.6/LICENSE` & `modAL-python-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.6/README.md` & `modAL-python-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -96,20 +96,19 @@
 To see modAL in *real* action, let's consider an active regression problem with Gaussian Processes! In this example, we shall try to learn the *noisy sine* function:
 ```python
 import numpy as np
 
 X = np.random.choice(np.linspace(0, 20, 10000), size=200, replace=False).reshape(-1, 1)
 y = np.sin(X) + np.random.normal(scale=0.3, size=X.shape)
 ```
-For active learning, we shall define a custom query strategy tailored to Gaussian processes. In a nutshell, a *query stategy* in modAL is a function taking (at least) two arguments (an estimator object and a pool of examples), outputting the index of the queried instance and the instance itself. In our case, the arguments are ```regressor``` and ```X```.
+For active learning, we shall define a custom query strategy tailored to Gaussian processes. In a nutshell, a *query stategy* in modAL is a function taking (at least) two arguments (an estimator object and a pool of examples), outputting the index of the queried instance. In our case, the arguments are ```regressor``` and ```X```.
 ```python
 def GP_regression_std(regressor, X):
     _, std = regressor.predict(X, return_std=True)
-    query_idx = np.argmax(std)
-    return query_idx, X[query_idx]
+    return np.argmax(std)
 ```
 After setting up the query strategy and the data, the active learner can be initialized.
 ```python
 from modAL.models import ActiveLearner
 from sklearn.gaussian_process import GaussianProcessRegressor
 from sklearn.gaussian_process.kernels import WhiteKernel, RBF
```

### Comparing `modAL-python-0.3.6/modAL/acquisition.py` & `modAL-python-0.4.0/modAL/acquisition.py`

 * *Files 6% similar despite different names*

```diff
@@ -100,64 +100,58 @@
 --------------------------------------------
 Query strategies using acquisition functions
 --------------------------------------------
 """
 
 
 def max_PI(optimizer: BaseLearner, X: modALinput, tradeoff: float = 0,
-           n_instances: int = 1) -> Tuple[np.ndarray, modALinput]:
+           n_instances: int = 1) -> np.ndarray:
     """
     Maximum PI query strategy. Selects the instance with highest probability of improvement.
 
     Args:
         optimizer: The :class:`~modAL.models.BayesianOptimizer` object for which the utility is to be calculated.
         X: The samples for which the probability of improvement is to be calculated.
         tradeoff: Value controlling the tradeoff parameter.
         n_instances: Number of samples to be queried.
 
     Returns:
         The indices of the instances from X chosen to be labelled; the instances from X chosen to be labelled.
     """
     pi = optimizer_PI(optimizer, X, tradeoff=tradeoff)
-    query_idx = multi_argmax(pi, n_instances=n_instances)
-
-    return query_idx, X[query_idx]
+    return multi_argmax(pi, n_instances=n_instances)
 
 
 def max_EI(optimizer: BaseLearner, X: modALinput, tradeoff: float = 0,
-           n_instances: int = 1) -> Tuple[np.ndarray, modALinput]:
+           n_instances: int = 1) -> np.ndarray:
     """
     Maximum EI query strategy. Selects the instance with highest expected improvement.
 
     Args:
         optimizer: The :class:`~modAL.models.BayesianOptimizer` object for which the utility is to be calculated.
         X: The samples for which the expected improvement is to be calculated.
         tradeoff: Value controlling the tradeoff parameter.
         n_instances: Number of samples to be queried.
 
     Returns:
         The indices of the instances from X chosen to be labelled; the instances from X chosen to be labelled.
     """
     ei = optimizer_EI(optimizer, X, tradeoff=tradeoff)
-    query_idx = multi_argmax(ei, n_instances=n_instances)
-
-    return query_idx, X[query_idx]
+    return multi_argmax(ei, n_instances=n_instances)
 
 
 def max_UCB(optimizer: BaseLearner, X: modALinput, beta: float = 1,
-            n_instances: int = 1) -> Tuple[np.ndarray, modALinput]:
+            n_instances: int = 1) -> np.ndarray:
     """
     Maximum UCB query strategy. Selects the instance with highest upper confidence bound.
 
     Args:
         optimizer: The :class:`~modAL.models.BayesianOptimizer` object for which the utility is to be calculated.
         X: The samples for which the maximum upper confidence bound is to be calculated.
         beta: Value controlling the beta parameter.
         n_instances: Number of samples to be queried.
 
     Returns:
         The indices of the instances from X chosen to be labelled; the instances from X chosen to be labelled.
     """
     ucb = optimizer_UCB(optimizer, X, beta=beta)
-    query_idx = multi_argmax(ucb, n_instances=n_instances)
-
-    return query_idx, X[query_idx]
+    return multi_argmax(ucb, n_instances=n_instances)
```

### Comparing `modAL-python-0.3.6/modAL/batch.py` & `modAL-python-0.4.0/modAL/batch.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
     # Isolate and return our best instance for labeling as the one with the largest score.
     best_instance_index_in_unlabeled = np.argmax(scores)
     n_pool, *rest = X_pool.shape
     unlabeled_indices = [i for i in range(n_pool) if mask[i]]
     best_instance_index = unlabeled_indices[best_instance_index_in_unlabeled]
     mask[best_instance_index] = 0
-    return best_instance_index, np.expand_dims(X_pool[best_instance_index], axis=0), mask
+    return best_instance_index, X_pool[[best_instance_index]], mask
 
 
 def ranked_batch(classifier: Union[BaseLearner, BaseCommittee],
                  unlabeled: modALinput,
                  uncertainty_scores: np.ndarray,
                  n_instances: int,
                  metric: Union[str, Callable],
@@ -138,19 +138,24 @@
         n_jobs: This parameter is passed to :func:`~sklearn.metrics.pairwise.pairwise_distances`.
 
     Returns:
         The indices of the top n_instances ranked unlabelled samples.
     """
     # Make a local copy of our classifier's training data.
     # Define our record container and record the best cold start instance in the case of cold start.
+
+    # transform unlabeled data if needed
+    if classifier.on_transformed:
+        unlabeled = classifier.transform_without_estimating(unlabeled)
+
     if classifier.X_training is None:
         best_coldstart_instance_index, labeled = select_cold_start_instance(X=unlabeled, metric=metric, n_jobs=n_jobs)
         instance_index_ranking = [best_coldstart_instance_index]
     elif classifier.X_training.shape[0] > 0:
-        labeled = classifier.X_training[:]
+        labeled = classifier.Xt_training[:] if classifier.on_transformed else classifier.X_training[:]
         instance_index_ranking = []
     
     # The maximum number of records to sample.
     ceiling = np.minimum(unlabeled.shape[0], n_instances) - len(instance_index_ranking)
 
     # mask for unlabeled initialized as transparent
     mask = np.ones(unlabeled.shape[0], np.bool)
@@ -176,15 +181,15 @@
 
 def uncertainty_batch_sampling(classifier: Union[BaseLearner, BaseCommittee],
                                X: Union[np.ndarray, sp.csr_matrix],
                                n_instances: int = 20,
                                metric: Union[str, Callable] = 'euclidean',
                                n_jobs: Optional[int] = None,
                                **uncertainty_measure_kwargs
-                               ) -> Tuple[np.ndarray, Union[np.ndarray, sp.csr_matrix]]:
+                               ) -> np.ndarray:
     """
     Batch sampling query strategy. Selects the least sure instances for labelling.
 
     This strategy differs from :func:`~modAL.uncertainty.uncertainty_sampling` because, although it is supported,
     traditional active learning query strategies suffer from sub-optimal record selection when passing
     `n_instances` > 1. This sampling strategy extends the interactive uncertainty query sampling by allowing for
     batch-mode uncertainty query sampling. Furthermore, it also enforces a ranking -- that is, which records among the
@@ -202,10 +207,10 @@
             distances between samples. Otherwise it is passed to :func:`~sklearn.metrics.pairwise.pairwise_distances`.
         **uncertainty_measure_kwargs: Keyword arguments to be passed for the :meth:`predict_proba` of the classifier.
 
     Returns:
         Indices of the instances from `X` chosen to be labelled; records from `X` chosen to be labelled.
     """
     uncertainty = classifier_uncertainty(classifier, X, **uncertainty_measure_kwargs)
-    query_indices = ranked_batch(classifier, unlabeled=X, uncertainty_scores=uncertainty,
+    return ranked_batch(classifier, unlabeled=X, uncertainty_scores=uncertainty,
                                  n_instances=n_instances, metric=metric, n_jobs=n_jobs)
-    return query_indices, X[query_indices]
+
```

### Comparing `modAL-python-0.3.6/modAL/density.py` & `modAL-python-0.4.0/modAL/density.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.6/modAL/disagreement.py` & `modAL-python-0.4.0/modAL/disagreement.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         learner_KL_div[:, learner_idx] = entropy(np.transpose(p_vote[:, learner_idx, :]), qk=np.transpose(p_consensus))
 
     return np.max(learner_KL_div, axis=1)
 
 
 def vote_entropy_sampling(committee: BaseCommittee, X: modALinput,
                           n_instances: int = 1, random_tie_break=False,
-                          **disagreement_measure_kwargs) -> Tuple[np.ndarray, modALinput]:
+                          **disagreement_measure_kwargs) -> np.ndarray:
     """
     Vote entropy sampling strategy.
 
     Args:
         committee: The committee for which the labels are to be queried.
         X: The pool of samples to query from.
         n_instances: Number of samples to be queried.
@@ -120,24 +120,22 @@
     Returns:
         The indices of the instances from X chosen to be labelled;
          the instances from X chosen to be labelled.
     """
     disagreement = vote_entropy(committee, X, **disagreement_measure_kwargs)
 
     if not random_tie_break:
-        query_idx = multi_argmax(disagreement, n_instances=n_instances)
-    else:
-        query_idx = shuffled_argmax(disagreement, n_instances=n_instances)
+        return multi_argmax(disagreement, n_instances=n_instances)
 
-    return query_idx, X[query_idx]
+    return shuffled_argmax(disagreement, n_instances=n_instances)
 
 
 def consensus_entropy_sampling(committee: BaseCommittee, X: modALinput,
                                n_instances: int = 1, random_tie_break=False,
-                               **disagreement_measure_kwargs) -> Tuple[np.ndarray, modALinput]:
+                               **disagreement_measure_kwargs) -> np.ndarray:
     """
     Consensus entropy sampling strategy.
 
     Args:
         committee: The committee for which the labels are to be queried.
         X: The pool of samples to query from.
         n_instances: Number of samples to be queried.
@@ -149,24 +147,22 @@
     Returns:
         The indices of the instances from X chosen to be labelled;
         the instances from X chosen to be labelled.
     """
     disagreement = consensus_entropy(committee, X, **disagreement_measure_kwargs)
 
     if not random_tie_break:
-        query_idx = multi_argmax(disagreement, n_instances=n_instances)
-    else:
-        query_idx = shuffled_argmax(disagreement, n_instances=n_instances)
+        return multi_argmax(disagreement, n_instances=n_instances)
 
-    return query_idx, X[query_idx]
+    return shuffled_argmax(disagreement, n_instances=n_instances)
 
 
 def max_disagreement_sampling(committee: BaseCommittee, X: modALinput,
                               n_instances: int = 1, random_tie_break=False,
-                              **disagreement_measure_kwargs) -> Tuple[np.ndarray, modALinput]:
+                              **disagreement_measure_kwargs) -> np.ndarray:
     """
     Maximum disagreement sampling strategy.
 
     Args:
         committee: The committee for which the labels are to be queried.
         X: The pool of samples to query from.
         n_instances: Number of samples to be queried.
@@ -178,24 +174,22 @@
     Returns:
         The indices of the instances from X chosen to be labelled;
         the instances from X chosen to be labelled.
     """
     disagreement = KL_max_disagreement(committee, X, **disagreement_measure_kwargs)
 
     if not random_tie_break:
-        query_idx = multi_argmax(disagreement, n_instances=n_instances)
-    else:
-        query_idx = shuffled_argmax(disagreement, n_instances=n_instances)
+        return multi_argmax(disagreement, n_instances=n_instances)
 
-    return query_idx, X[query_idx]
+    return shuffled_argmax(disagreement, n_instances=n_instances)
 
 
 def max_std_sampling(regressor: BaseEstimator, X: modALinput,
                      n_instances: int = 1,  random_tie_break=False,
-                     **predict_kwargs) -> Tuple[np.ndarray, modALinput]:
+                     **predict_kwargs) -> np.ndarray:
     """
     Regressor standard deviation sampling strategy.
 
     Args:
         regressor: The regressor for which the labels are to be queried.
         X: The pool of samples to query from.
         n_instances: Number of samples to be queried.
@@ -207,12 +201,10 @@
         The indices of the instances from X chosen to be labelled;
         the instances from X chosen to be labelled.
     """
     _, std = regressor.predict(X, return_std=True, **predict_kwargs)
     std = std.reshape(X.shape[0], )
 
     if not random_tie_break:
-        query_idx = multi_argmax(std, n_instances=n_instances)
-    else:
-        query_idx = shuffled_argmax(std, n_instances=n_instances)
+        return multi_argmax(std, n_instances=n_instances)
 
-    return query_idx, X[query_idx]
+    return shuffled_argmax(std, n_instances=n_instances)
```

### Comparing `modAL-python-0.3.6/modAL/expected_error.py` & `modAL-python-0.4.0/modAL/expected_error.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 import numpy as np
 
 from sklearn.base import clone
 from sklearn.exceptions import NotFittedError
 
 from modAL.models import ActiveLearner
-from modAL.utils.data import modALinput, data_vstack
+from modAL.utils.data import modALinput, data_vstack, enumerate_data, drop_rows, data_shape, add_row
 from modAL.utils.selection import multi_argmax, shuffled_argmax
 from modAL.uncertainty import _proba_uncertainty, _proba_entropy
 
 
 def expected_error_reduction(learner: ActiveLearner, X: modALinput, loss: str = 'binary',
                              p_subsample: np.float = 1.0, n_instances: int = 1,
-                             random_tie_break: bool = False) -> Tuple[np.ndarray, modALinput]:
+                             random_tie_break: bool = False) -> np.ndarray:
     """
     Expected error reduction query strategy.
 
     References:
         Roy and McCallum, 2001 (http://groups.csail.mit.edu/rrg/papers/icml01.pdf)
 
     Args:
@@ -34,39 +34,38 @@
             for large sample pools.
         n_instances: The number of instances to be sampled.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
 
 
     Returns:
-        The indices of the instances from X chosen to be labelled;
-        the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled.
     """
 
     assert 0.0 <= p_subsample <= 1.0, 'p_subsample subsampling keep ratio must be between 0.0 and 1.0'
     assert loss in ['binary', 'log'], 'loss must be \'binary\' or \'log\''
 
-    expected_error = np.zeros(shape=(len(X), ))
+    expected_error = np.zeros(shape=(data_shape(X)[0],))
     possible_labels = np.unique(learner.y_training)
 
     try:
         X_proba = learner.predict_proba(X)
     except NotFittedError:
         # TODO: implement a proper cold-start
-        return 0, X[0]
+        return np.array([0])
 
     cloned_estimator = clone(learner.estimator)
 
-    for x_idx, x in enumerate(X):
+    for x_idx, x in enumerate_data(X):
         # subsample the data if needed
         if np.random.rand() <= p_subsample:
-            X_reduced = np.delete(X, x_idx, axis=0)
+            X_reduced = drop_rows(X, x_idx)
             # estimate the expected error
             for y_idx, y in enumerate(possible_labels):
-                X_new = data_vstack((learner.X_training, np.expand_dims(x, axis=0)))
+                X_new = add_row(learner.X_training, x)
                 y_new = data_vstack((learner.y_training, np.array(y).reshape(1,)))
 
                 cloned_estimator.fit(X_new, y_new)
                 refitted_proba = cloned_estimator.predict_proba(X_reduced)
                 if loss is 'binary':
                     nloss = _proba_uncertainty(refitted_proba)
                 elif loss is 'log':
@@ -74,12 +73,10 @@
 
                 expected_error[x_idx] += np.sum(nloss)*X_proba[x_idx, y_idx]
 
         else:
             expected_error[x_idx] = np.inf
 
     if not random_tie_break:
-        query_idx = multi_argmax(-expected_error, n_instances)
-    else:
-        query_idx = shuffled_argmax(-expected_error, n_instances)
+        return multi_argmax(-expected_error, n_instances)
 
-    return query_idx, X[query_idx]
+    return shuffled_argmax(-expected_error, n_instances)
```

### Comparing `modAL-python-0.3.6/modAL/models/base.py` & `modAL-python-0.4.0/modAL/models/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """
 Base classes for active learning algorithms
 ------------------------------------------
 """
 
 import abc
 import sys
+import warnings
 from typing import Union, Callable, Optional, Tuple, List, Iterator, Any
 
 import numpy as np
 from sklearn.base import BaseEstimator
+from sklearn.ensemble._base import _BaseHeterogeneousEnsemble
+from sklearn.pipeline import Pipeline
 from sklearn.utils import check_X_y
 
-from modAL.utils.data import data_vstack, modALinput
+import scipy.sparse as sp
 
+from modAL.utils.data import data_vstack, data_hstack, modALinput, retrieve_rows
 
 if sys.version_info >= (3, 4):
     ABC = abc.ABC
 else:
     ABC = abc.ABCMeta('ABC', (), {})
 
 
@@ -30,14 +34,16 @@
             for instance, modAL.uncertainty.uncertainty_sampling.
         X_training: Initial training samples, if available.
         y_training: Initial training labels corresponding to initial training samples.
         force_all_finite: When True, forces all values of the data finite.
             When False, accepts np.nan and np.inf values.
         bootstrap_init: If initial training data is available, bootstrapping can be done during the first training.
             Useful when building Committee models with bagging.
+        on_transformed: Whether to transform samples with the pipeline defined by the estimator
+            when applying the query strategy.
         **fit_kwargs: keyword arguments.
 
     Attributes:
         estimator: The estimator to be used in the active learning loop.
         query_strategy: Function providing the query strategy for the active learning loop.
         X_training: If the model hasn't been fitted yet it is None, otherwise it contains the samples
             which the model has been trained on.
@@ -45,26 +51,30 @@
     """
     def __init__(self,
                  estimator: BaseEstimator,
                  query_strategy: Callable,
                  X_training: Optional[modALinput] = None,
                  y_training: Optional[modALinput] = None,
                  bootstrap_init: bool = False,
+                 on_transformed: bool = False,
                  force_all_finite: bool = True,
                  **fit_kwargs
                  ) -> None:
         assert callable(query_strategy), 'query_strategy must be callable'
 
         self.estimator = estimator
         self.query_strategy = query_strategy
+        self.on_transformed = on_transformed
 
         self.X_training = X_training
+        self.Xt_training = None
         self.y_training = y_training
         if X_training is not None:
             self._fit_to_known(bootstrap=bootstrap_init, **fit_kwargs)
+            self.Xt_training = self.transform_without_estimating(self.X_training) if self.on_transformed else None
 
         assert isinstance(force_all_finite, bool), 'force_all_finite must be a bool'
         self.force_all_finite = force_all_finite
 
     def _add_training_data(self, X: modALinput, y: modALinput) -> None:
         """
         Adds the new data and label to the known data, but does not retrain the model.
@@ -78,23 +88,69 @@
             classifier has seen.
         """
         check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
                   force_all_finite=self.force_all_finite)
 
         if self.X_training is None:
             self.X_training = X
+            self.Xt_training = self.transform_without_estimating(self.X_training) if self.on_transformed else None
             self.y_training = y
         else:
             try:
                 self.X_training = data_vstack((self.X_training, X))
+                self.Xt_training = data_vstack((
+                    self.Xt_training,
+                    self.transform_without_estimating(X)
+                )) if self.on_transformed else None
                 self.y_training = data_vstack((self.y_training, y))
             except ValueError:
                 raise ValueError('the dimensions of the new training data and label must'
                                  'agree with the training data and labels provided so far')
 
+    def transform_without_estimating(self, X: modALinput) -> Union[np.ndarray, sp.csr_matrix]:
+        """
+        Transforms the data as supplied to the estimator.
+
+        * In case the estimator is an skearn pipeline, it applies all pipeline components but the last one.
+        * In case the estimator is an ensemble, it concatenates the transformations for each classfier
+            (pipeline) in the ensemble.
+        * Otherwise returns the non-transformed dataset X
+        Args:
+            X: dataset to be transformed
+
+        Returns:
+            Transformed data set
+        """
+        Xt = []
+        pipes = [self.estimator]
+
+        if isinstance(self.estimator, _BaseHeterogeneousEnsemble):
+            pipes = self.estimator.estimators_
+
+        ################################
+        # transform data with pipelines used by estimator
+        for pipe in pipes:
+            if isinstance(pipe, Pipeline):
+                # NOTE: The used pipeline class might be an extension to sklearn's!
+                #       Create a new instance of the used pipeline class with all
+                #       components but the final estimator, which is replaced by an empty (passthrough) component.
+                #       This prevents any special handling of the final transformation pipe, which is usually
+                #       expected to be an estimator.
+                transformation_pipe = pipe.__class__(steps=[*pipe.steps[:-1], ('passthrough', 'passthrough')])
+                Xt.append(transformation_pipe.transform(X))
+
+        # in case no transformation pipelines are used by the estimator,
+        # return the original, non-transfored data
+        if not Xt:
+            return X
+
+        ################################
+        # concatenate all transformations and return
+        return data_hstack(Xt)
+
     def _fit_to_known(self, bootstrap: bool = False, **fit_kwargs) -> 'BaseLearner':
         """
         Fits self.estimator to the training data and labels provided to it so far.
 
         Args:
             bootstrap: If True, the method trains the model on a set bootstrapped from the known training instances.
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
@@ -153,14 +209,15 @@
 
         Returns:
             self
         """
         check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
                   force_all_finite=self.force_all_finite)
         self.X_training, self.y_training = X, y
+        self.Xt_training = self.transform_without_estimating(self.X_training) if self.on_transformed else None
         return self._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
 
     def predict(self, X: modALinput, **predict_kwargs) -> Any:
         """
         Estimator predictions for X. Interface with the predict method of the estimator.
 
         Args:
@@ -181,31 +238,39 @@
             **predict_proba_kwargs: Keyword arguments to be passed to the predict_proba method of the classifier.
 
         Returns:
             Class probabilities for X.
         """
         return self.estimator.predict_proba(X, **predict_proba_kwargs)
 
-    def query(self, *query_args, **query_kwargs) -> Union[Tuple, modALinput]:
+    def query(self, X_pool, *query_args, **query_kwargs) -> Union[Tuple, modALinput]:
         """
         Finds the n_instances most informative point in the data provided by calling the query_strategy function.
 
         Args:
+            X_pool: Pool of unlabeled instances to retrieve most informative instances from
             *query_args: The arguments for the query strategy. For instance, in the case of
                 :func:`~modAL.uncertainty.uncertainty_sampling`, it is the pool of samples from which the query strategy
                 should choose instances to request labels.
             **query_kwargs: Keyword arguments for the query strategy function.
 
         Returns:
             Value of the query_strategy function. Should be the indices of the instances from the pool chosen to be
             labelled and the instances themselves. Can be different in other cases, for instance only the instance to be
             labelled upon query synthesis.
         """
-        query_result = self.query_strategy(self, *query_args, **query_kwargs)
-        return query_result
+        query_result = self.query_strategy(self, X_pool, *query_args, **query_kwargs)
+
+        if isinstance(query_result, tuple):
+            warnings.warn("Query strategies should no longer return the selected instances, "
+                          "this is now handled by the query method. "
+                          "Please return only the indices of the selected instances.", DeprecationWarning)
+            return query_result
+
+        return query_result, retrieve_rows(X_pool, query_result)
 
     def score(self, X: modALinput, y: modALinput, **score_kwargs) -> Any:
         """
         Interface for the score method of the predictor.
 
         Args:
             X: The samples for which prediction accuracy is to be calculated.
@@ -225,20 +290,25 @@
 class BaseCommittee(ABC, BaseEstimator):
     """
     Base class for query-by-committee setup.
 
     Args:
         learner_list: List of ActiveLearner objects to form committee.
         query_strategy: Function to query labels.
+        on_transformed: Whether to transform samples with the pipeline defined by each learner's estimator
+            when applying the query strategy.
     """
-    def __init__(self, learner_list: List[BaseLearner], query_strategy: Callable) -> None:
+    def __init__(self, learner_list: List[BaseLearner], query_strategy: Callable, on_transformed: bool = False) -> None:
         assert type(learner_list) == list, 'learners must be supplied in a list'
 
         self.learner_list = learner_list
         self.query_strategy = query_strategy
+        self.on_transformed = on_transformed
+        # TODO: update training data when using fit() and teach() methods
+        self.X_training = None
 
     def __iter__(self) -> Iterator[BaseLearner]:
         for learner in self.learner_list:
             yield learner
 
     def __len__(self) -> int:
         return len(self.learner_list)
@@ -297,31 +367,50 @@
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
         """
         for learner in self.learner_list:
             learner.fit(X, y, **fit_kwargs)
 
         return self
 
-    def query(self, *query_args, **query_kwargs) -> Union[Tuple, modALinput]:
+    def transform_without_estimating(self, X: modALinput) -> Union[np.ndarray, sp.csr_matrix]:
+        """
+        Transforms the data as supplied to each learner's estimator and concatenates transformations.
+        Args:
+            X: dataset to be transformed
+
+        Returns:
+            Transformed data set
+        """
+        return data_hstack([learner.transform_without_estimating(X) for learner in self.learner_list])
+
+    def query(self, X_pool, *query_args, **query_kwargs) -> Union[Tuple, modALinput]:
         """
         Finds the n_instances most informative point in the data provided by calling the query_strategy function.
 
         Args:
+            X_pool: Pool of unlabeled instances to retrieve most informative instances from
             *query_args: The arguments for the query strategy. For instance, in the case of
                 :func:`~modAL.disagreement.max_disagreement_sampling`, it is the pool of samples from which the query.
                 strategy should choose instances to request labels.
             **query_kwargs: Keyword arguments for the query strategy function.
 
         Returns:
             Return value of the query_strategy function. Should be the indices of the instances from the pool chosen to
             be labelled and the instances themselves. Can be different in other cases, for instance only the instance to
             be labelled upon query synthesis.
         """
-        query_result = self.query_strategy(self, *query_args, **query_kwargs)
-        return query_result
+        query_result = self.query_strategy(self, X_pool, *query_args, **query_kwargs)
+
+        if isinstance(query_result, tuple):
+            warnings.warn("Query strategies should no longer return the selected instances, "
+                          "this is now handled by the query method. "
+                          "Please return only the indices of the selected instances", DeprecationWarning)
+            return query_result
+
+        return query_result, retrieve_rows(X_pool, query_result)
 
     def rebag(self, **fit_kwargs) -> None:
         """
         Refits every learner with a dataset bootstrapped from its training instances. Contrary to .bag(), it bootstraps
         the training data for each learner based on its own examples.
 
         Todo:
```

### Comparing `modAL-python-0.3.6/modAL/models/learners.py` & `modAL-python-0.4.0/modAL/models/learners.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Callable, Optional, Tuple, List, Any
 
 from sklearn.base import BaseEstimator
 from sklearn.metrics import accuracy_score
 
 from modAL.models.base import BaseLearner, BaseCommittee
 from modAL.utils.validation import check_class_labels, check_class_proba
-from modAL.utils.data import modALinput
+from modAL.utils.data import modALinput, retrieve_rows
 from modAL.uncertainty import uncertainty_sampling
 from modAL.disagreement import vote_entropy_sampling, max_std_sampling
 from modAL.acquisition import max_EI
 
 """
 Classes for active learning algorithms
 --------------------------------------
@@ -26,14 +26,16 @@
         estimator: The estimator to be used in the active learning loop.
         query_strategy: Function providing the query strategy for the active learning loop,
             for instance, modAL.uncertainty.uncertainty_sampling.
         X_training: Initial training samples, if available.
         y_training: Initial training labels corresponding to initial training samples.
         bootstrap_init: If initial training data is available, bootstrapping can be done during the first training.
             Useful when building Committee models with bagging.
+        on_transformed: Whether to transform samples with the pipeline defined by the estimator
+            when applying the query strategy.
         **fit_kwargs: keyword arguments.
 
     Attributes:
         estimator: The estimator to be used in the active learning loop.
         query_strategy: Function providing the query strategy for the active learning loop.
         X_training: If the model hasn't been fitted yet it is None, otherwise it contains the samples
             which the model has been trained on. If provided, the method fit() of estimator is called during __init__()
@@ -69,18 +71,19 @@
 
     def __init__(self,
                  estimator: BaseEstimator,
                  query_strategy: Callable = uncertainty_sampling,
                  X_training: Optional[modALinput] = None,
                  y_training: Optional[modALinput] = None,
                  bootstrap_init: bool = False,
+                 on_transformed: bool = False,
                  **fit_kwargs
                  ) -> None:
         super().__init__(estimator, query_strategy,
-                         X_training, y_training, bootstrap_init, **fit_kwargs)
+                         X_training, y_training, bootstrap_init, on_transformed, **fit_kwargs)
 
     def teach(self, X: modALinput, y: modALinput, bootstrap: bool = False, only_new: bool = False, **fit_kwargs) -> None:
         """
         Adds X and y to the known training data and retrains the predictor with the augmented dataset.
 
         Args:
             X: The new samples for which the labels are supplied by the expert.
@@ -173,32 +176,33 @@
     """
     def __init__(self,
                  estimator: BaseEstimator,
                  query_strategy: Callable = max_EI,
                  X_training: Optional[modALinput] = None,
                  y_training: Optional[modALinput] = None,
                  bootstrap_init: bool = False,
+                 on_transformed: bool = False,
                  **fit_kwargs) -> None:
         super(BayesianOptimizer, self).__init__(estimator, query_strategy,
-                                                X_training, y_training, bootstrap_init, **fit_kwargs)
+                                                X_training, y_training, bootstrap_init, on_transformed, **fit_kwargs)
         # setting the maximum value
         if self.y_training is not None:
             max_idx = np.argmax(self.y_training)
-            self.X_max = self.X_training[max_idx]
+            self.X_max = retrieve_rows(self.X_training, max_idx)
             self.y_max = self.y_training[max_idx]
         else:
             self.X_max = None
             self.y_max = -np.inf
 
     def _set_max(self, X: modALinput, y: modALinput) -> None:
         max_idx = np.argmax(y)
         y_max = y[max_idx]
         if y_max > self.y_max:
             self.y_max = y_max
-            self.X_max = X[max_idx]
+            self.X_max = retrieve_rows(X, max_idx)
 
     def get_max(self) -> Tuple:
         """
         Gives the highest value so far.
 
         Returns:
             The location of the currently best value and the value itself.
@@ -240,14 +244,16 @@
     """
     This class is an abstract model of a committee-based active learning algorithm.
 
     Args:
         learner_list: A list of ActiveLearners forming the Committee.
         query_strategy: Query strategy function. Committee supports disagreement-based query strategies from
             :mod:`modAL.disagreement`, but uncertainty-based ones from :mod:`modAL.uncertainty` are also supported.
+        on_transformed: Whether to transform samples with the pipeline defined by each learner's estimator
+            when applying the query strategy.
 
     Attributes:
         classes_: Class labels known by the Committee.
         n_classes_: Number of classes known by the Committee.
 
     Examples:
 
@@ -280,16 +286,17 @@
         >>>
         >>> # teaching newly labelled examples
         >>> committee.teach(
         ...     X=iris['data'][query_idx].reshape(1, -1),
         ...     y=iris['target'][query_idx].reshape(1, )
         ... )
     """
-    def __init__(self, learner_list: List[ActiveLearner], query_strategy: Callable = vote_entropy_sampling) -> None:
-        super().__init__(learner_list, query_strategy)
+    def __init__(self, learner_list: List[ActiveLearner], query_strategy: Callable = vote_entropy_sampling,
+                 on_transformed: bool = False) -> None:
+        super().__init__(learner_list, query_strategy, on_transformed)
         self._set_classes()
 
     def _set_classes(self):
         """
         Checks the known class labels by each learner, merges the labels and returns a mapping which maps the learner's
         classes to the complete label list.
         """
@@ -308,26 +315,41 @@
             axis=0
         )
         self.n_classes_ = len(self.classes_)
 
     def _add_training_data(self, X: modALinput, y: modALinput):
         super()._add_training_data(X, y)
 
+    def fit(self, X: modALinput, y: modALinput, **fit_kwargs) -> 'BaseCommittee':
+        """
+        Fits every learner to a subset sampled with replacement from X. Calling this method makes the learner forget the
+        data it has seen up until this point and replaces it with X! If you would like to perform bootstrapping on each
+        learner using the data it has seen, use the method .rebag()!
+
+        Calling this method makes the learner forget the data it has seen up until this point and replaces it with X!
+
+        Args:
+            X: The samples to be fitted on.
+            y: The corresponding labels.
+            **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
+        """
+        super().fit(X, y, **fit_kwargs)
+        self._set_classes()
+
     def teach(self, X: modALinput, y: modALinput, bootstrap: bool = False, only_new: bool = False, **fit_kwargs) -> None:
         """
         Adds X and y to the known training data for each learner and retrains learners with the augmented dataset.
 
         Args:
             X: The new samples for which the labels are supplied by the expert.
             y: Labels corresponding to the new instances in X.
             bootstrap: If True, trains each learner on a bootstrapped set. Useful when building the ensemble by bagging.
             only_new: If True, the model is retrained using only X and y, ignoring the previously provided examples.
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
         """
-
         super().teach(X, y, bootstrap=bootstrap, only_new=only_new, **fit_kwargs)
         self._set_classes()
 
     def predict(self, X: modALinput, **predict_proba_kwargs) -> Any:
         """
         Predicts the class of the samples by picking the consensus prediction.
 
@@ -433,14 +455,16 @@
 class CommitteeRegressor(BaseCommittee):
     """
     This class is an abstract model of a committee-based active learning regression.
 
     Args:
         learner_list: A list of ActiveLearners forming the CommitteeRegressor.
         query_strategy: Query strategy function.
+        on_transformed: Whether to transform samples with the pipeline defined by each learner's estimator
+            when applying the query strategy.
 
     Examples:
 
         >>> import numpy as np
         >>> import matplotlib.pyplot as plt
         >>> from sklearn.gaussian_process import GaussianProcessRegressor
         >>> from sklearn.gaussian_process.kernels import WhiteKernel, RBF
@@ -462,31 +486,31 @@
         ...                         X_training=X[idx].reshape(-1, 1), y_training=y[idx].reshape(-1, 1)
         ...                 )
         ...                 for idx in initial_idx]
         >>>
         >>> # query strategy for regression
         >>> def ensemble_regression_std(regressor, X):
         ...     _, std = regressor.predict(X, return_std=True)
-        ...     query_idx = np.argmax(std)
-        ...     return query_idx, X[query_idx]
+        ...     return np.argmax(std)
         >>>
         >>> # initializing the CommitteeRegressor
         >>> committee = CommitteeRegressor(
         ...     learner_list=learner_list,
         ...     query_strategy=ensemble_regression_std
         ... )
         >>>
         >>> # active regression
         >>> n_queries = 10
         >>> for idx in range(n_queries):
         ...     query_idx, query_instance = committee.query(X.reshape(-1, 1))
         ...     committee.teach(X[query_idx].reshape(-1, 1), y[query_idx].reshape(-1, 1))
     """
-    def __init__(self, learner_list: List[ActiveLearner], query_strategy: Callable = max_std_sampling) -> None:
-        super().__init__(learner_list, query_strategy)
+    def __init__(self, learner_list: List[ActiveLearner], query_strategy: Callable = max_std_sampling,
+                 on_transformed: bool = False) -> None:
+        super().__init__(learner_list, query_strategy, on_transformed)
 
     def predict(self, X: modALinput, return_std: bool = False, **predict_kwargs) -> Any:
         """
         Predicts the values of the samples by averaging the prediction of each regressor.
 
         Args:
             X: The samples to be predicted.
```

### Comparing `modAL-python-0.3.6/modAL/multilabel.py` & `modAL-python-0.4.0/modAL/multilabel.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
             cls_mtx[inst_idx, most_certain_class] = 1
 
         cls_loss = np.maximum(1 - np.multiply(cls_mtx, predictions), 0).sum(axis=1)
         return cls_loss
 
 
 def SVM_binary_minimum(classifier: ActiveLearner, X_pool: modALinput,
-                       random_tie_break: bool = False) -> Tuple[np.ndarray, modALinput]:
+                       random_tie_break: bool = False) -> np.ndarray:
     """
     SVM binary minimum multilabel active learning strategy. For details see the paper
     Klaus Brinker, On Active Learning in Multi-label Classification
     (https://link.springer.com/chapter/10.1007%2F3-540-31314-1_24)
 
     Args:
         classifier: The multilabel classifier for which the labels are to be queried. Must be an SVM model
@@ -63,23 +63,21 @@
 
     decision_function = np.array([svm.decision_function(X_pool)
                                   for svm in classifier.estimator.estimators_]).T
 
     min_abs_dist = np.min(np.abs(decision_function), axis=1)
 
     if not random_tie_break:
-        query_idx = np.argmin(min_abs_dist)
-    else:
-        query_idx = shuffled_argmax(min_abs_dist)
+        return np.argmin(min_abs_dist)
 
-    return query_idx, X_pool[query_idx]
+    return shuffled_argmax(min_abs_dist)
 
 
 def max_loss(classifier: OneVsRestClassifier, X_pool: modALinput,
-             n_instances: int = 1, random_tie_break: bool = False) -> Tuple[np.ndarray, modALinput]:
+             n_instances: int = 1, random_tie_break: bool = False) -> np.ndarray:
 
     """
     Max Loss query strategy for SVM multilabel classification.
 
     For more details on this query strategy, see
     Li et al., Multilabel SVM active learning for image classification
     (http://dx.doi.org/10.1109/ICIP.2004.1421535)
@@ -99,23 +97,21 @@
 
     assert len(X_pool) >= n_instances, 'n_instances cannot be larger than len(X_pool)'
 
     most_certain_classes = classifier.predict_proba(X_pool).argmax(axis=1)
     loss = _SVM_loss(classifier, X_pool, most_certain_classes=most_certain_classes)
 
     if not random_tie_break:
-        query_idx = multi_argmax(loss, n_instances)
-    else:
-        query_idx = shuffled_argmax(loss, n_instances)
+        return multi_argmax(loss, n_instances)
 
-    return query_idx, X_pool[query_idx]
+    return shuffled_argmax(loss, n_instances)
 
 
 def mean_max_loss(classifier: OneVsRestClassifier, X_pool: modALinput,
-                  n_instances: int = 1, random_tie_break: bool = False) -> Tuple[np.ndarray, modALinput]:
+                  n_instances: int = 1, random_tie_break: bool = False) -> np.ndarray:
     """
     Mean Max Loss query strategy for SVM multilabel classification.
 
     For more details on this query strategy, see
     Li et al., Multilabel SVM active learning for image classification
     (http://dx.doi.org/10.1109/ICIP.2004.1421535)
 
@@ -132,23 +128,21 @@
         the instance from X_pool chosen to be labelled.
     """
 
     assert len(X_pool) >= n_instances, 'n_instances cannot be larger than len(X_pool)'
     loss = _SVM_loss(classifier, X_pool)
 
     if not random_tie_break:
-        query_idx = multi_argmax(loss, n_instances)
-    else:
-        query_idx = shuffled_argmax(loss, n_instances)
+        return multi_argmax(loss, n_instances)
 
-    return query_idx, X_pool[query_idx]
+    return shuffled_argmax(loss, n_instances)
 
 
 def min_confidence(classifier: OneVsRestClassifier, X_pool: modALinput,
-                   n_instances: int = 1, random_tie_break: bool = False) -> Tuple[np.ndarray, modALinput]:
+                   n_instances: int = 1, random_tie_break: bool = False) -> np.ndarray:
     """
     MinConfidence query strategy for multilabel classification.
 
     For more details on this query strategy, see
     Esuli and Sebastiani., Active Learning Strategies for Multi-Label Text Classification
     (http://dx.doi.org/10.1007/978-3-642-00958-7_12)
 
@@ -163,23 +157,21 @@
         the instance from X_pool chosen to be labelled.
     """
 
     classwise_confidence = classifier.predict_proba(X_pool)
     classwise_min = np.min(classwise_confidence, axis=1)
 
     if not random_tie_break:
-        query_idx = multi_argmax(-classwise_min, n_instances)
-    else:
-        query_idx = shuffled_argmax(-classwise_min, n_instances)
+        return multi_argmax(-classwise_min, n_instances)
 
-    return query_idx, X_pool[query_idx]
+    return shuffled_argmax(-classwise_min, n_instances)
 
 
 def avg_confidence(classifier: OneVsRestClassifier, X_pool: modALinput,
-                   n_instances: int = 1, random_tie_break: bool = False) -> Tuple[np.ndarray, modALinput]:
+                   n_instances: int = 1, random_tie_break: bool = False) -> np.ndarray:
     """
     AvgConfidence query strategy for multilabel classification.
 
     For more details on this query strategy, see
     Esuli and Sebastiani., Active Learning Strategies for Multi-Label Text Classification
     (http://dx.doi.org/10.1007/978-3-642-00958-7_12)
 
@@ -194,23 +186,21 @@
         the instance from X_pool chosen to be labelled.
     """
 
     classwise_confidence = classifier.predict_proba(X_pool)
     classwise_mean = np.mean(classwise_confidence, axis=1)
 
     if not random_tie_break:
-        query_idx = multi_argmax(classwise_mean, n_instances)
-    else:
-        query_idx = shuffled_argmax(classwise_mean, n_instances)
+        return multi_argmax(classwise_mean, n_instances)
 
-    return query_idx, X_pool[query_idx]
+    return shuffled_argmax(classwise_mean, n_instances)
 
 
 def max_score(classifier: OneVsRestClassifier, X_pool: modALinput,
-              n_instances: int = 1, random_tie_break: bool = 1) -> Tuple[np.ndarray, modALinput]:
+              n_instances: int = 1, random_tie_break: bool = 1) -> np.ndarray:
     """
     MaxScore query strategy for multilabel classification.
 
     For more details on this query strategy, see
     Esuli and Sebastiani., Active Learning Strategies for Multi-Label Text Classification
     (http://dx.doi.org/10.1007/978-3-642-00958-7_12)
 
@@ -227,23 +217,21 @@
 
     classwise_confidence = classifier.predict_proba(X_pool)
     classwise_predictions = classifier.predict(X_pool)
     classwise_scores = classwise_confidence*(classwise_predictions - 1/2)
     classwise_max = np.max(classwise_scores, axis=1)
 
     if not random_tie_break:
-        query_idx = multi_argmax(classwise_max, n_instances)
-    else:
-        query_idx = shuffled_argmax(classwise_max, n_instances)
+        return multi_argmax(classwise_max, n_instances)
 
-    return query_idx, X_pool[query_idx]
+    return shuffled_argmax(classwise_max, n_instances)
 
 
 def avg_score(classifier: OneVsRestClassifier, X_pool: modALinput,
-              n_instances: int = 1, random_tie_break: bool = False) -> Tuple[np.ndarray, modALinput]:
+              n_instances: int = 1, random_tie_break: bool = False) -> np.ndarray:
     """
     AvgScore query strategy for multilabel classification.
 
     For more details on this query strategy, see
     Esuli and Sebastiani., Active Learning Strategies for Multi-Label Text Classification
     (http://dx.doi.org/10.1007/978-3-642-00958-7_12)
 
@@ -260,12 +248,10 @@
 
     classwise_confidence = classifier.predict_proba(X_pool)
     classwise_predictions = classifier.predict(X_pool)
     classwise_scores = classwise_confidence*(classwise_predictions-1/2)
     classwise_mean = np.mean(classwise_scores, axis=1)
 
     if not random_tie_break:
-        query_idx = multi_argmax(classwise_mean, n_instances)
-    else:
-        query_idx = shuffled_argmax(classwise_mean, n_instances)
+        return multi_argmax(classwise_mean, n_instances)
 
-    return query_idx, X_pool[query_idx]
+    return shuffled_argmax(classwise_mean, n_instances)
```

### Comparing `modAL-python-0.3.6/modAL/uncertainty.py` & `modAL-python-0.4.0/modAL/uncertainty.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,15 +128,15 @@
         return np.zeros(shape=(X.shape[0], ))
 
     return np.transpose(entropy(np.transpose(classwise_uncertainty)))
 
 
 def uncertainty_sampling(classifier: BaseEstimator, X: modALinput,
                          n_instances: int = 1, random_tie_break: bool = False,
-                         **uncertainty_measure_kwargs) -> Tuple[np.ndarray, modALinput]:
+                         **uncertainty_measure_kwargs) -> np.ndarray:
     """
     Uncertainty sampling query strategy. Selects the least sure instances for labelling.
 
     Args:
         classifier: The classifier for which the labels are to be queried.
         X: The pool of samples to query from.
         n_instances: Number of samples to be queried.
@@ -148,24 +148,22 @@
     Returns:
         The indices of the instances from X chosen to be labelled;
         the instances from X chosen to be labelled.
     """
     uncertainty = classifier_uncertainty(classifier, X, **uncertainty_measure_kwargs)
 
     if not random_tie_break:
-        query_idx = multi_argmax(uncertainty, n_instances=n_instances)
-    else:
-        query_idx = shuffled_argmax(uncertainty, n_instances=n_instances)
+        return multi_argmax(uncertainty, n_instances=n_instances)
 
-    return query_idx, X[query_idx]
+    return shuffled_argmax(uncertainty, n_instances=n_instances)
 
 
 def margin_sampling(classifier: BaseEstimator, X: modALinput,
                     n_instances: int = 1, random_tie_break: bool = False,
-                    **uncertainty_measure_kwargs) -> Tuple[np.ndarray, modALinput]:
+                    **uncertainty_measure_kwargs) -> np.ndarray:
     """
     Margin sampling query strategy. Selects the instances where the difference between
     the first most likely and second most likely classes are the smallest.
     Args:
         classifier: The classifier for which the labels are to be queried.
         X: The pool of samples to query from.
         n_instances: Number of samples to be queried.
@@ -176,24 +174,22 @@
     Returns:
         The indices of the instances from X chosen to be labelled;
         the instances from X chosen to be labelled.
     """
     margin = classifier_margin(classifier, X, **uncertainty_measure_kwargs)
 
     if not random_tie_break:
-        query_idx = multi_argmax(-margin, n_instances=n_instances)
-    else:
-        query_idx = shuffled_argmax(-margin, n_instances=n_instances)
+        return multi_argmax(-margin, n_instances=n_instances)
 
-    return query_idx, X[query_idx]
+    return shuffled_argmax(-margin, n_instances=n_instances)
 
 
 def entropy_sampling(classifier: BaseEstimator, X: modALinput,
                      n_instances: int = 1, random_tie_break: bool = False,
-                     **uncertainty_measure_kwargs) -> Tuple[np.ndarray, modALinput]:
+                     **uncertainty_measure_kwargs) -> np.ndarray:
     """
     Entropy sampling query strategy. Selects the instances where the class probabilities
     have the largest entropy.
 
     Args:
         classifier: The classifier for which the labels are to be queried.
         X: The pool of samples to query from.
@@ -206,12 +202,10 @@
     Returns:
         The indices of the instances from X chosen to be labelled;
         the instances from X chosen to be labelled.
     """
     entropy = classifier_entropy(classifier, X, **uncertainty_measure_kwargs)
 
     if not random_tie_break:
-        query_idx = multi_argmax(entropy, n_instances=n_instances)
-    else:
-        query_idx = shuffled_argmax(entropy, n_instances=n_instances)
+        return multi_argmax(entropy, n_instances=n_instances)
 
-    return query_idx, X[query_idx]
+    return shuffled_argmax(entropy, n_instances=n_instances)
```

### Comparing `modAL-python-0.3.6/modAL/utils/combination.py` & `modAL-python-0.4.0/modAL/utils/combination.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,11 +74,10 @@
             array containing the queried items.
 
     Returns:
         A function which returns queried instances given a classifier and an unlabelled pool.
     """
     def query_strategy(classifier: BaseEstimator, X: modALinput) -> Tuple:
         utility = utility_measure(classifier, X)
-        query_idx = selector(utility)
-        return query_idx, X[query_idx]
+        return selector(utility)
 
     return query_strategy
```

### Comparing `modAL-python-0.3.6/modAL/utils/selection.py` & `modAL-python-0.4.0/modAL/utils/selection.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.6/modAL/utils/validation.py` & `modAL-python-0.4.0/modAL/utils/validation.py`

 * *Files identical despite different names*

### Comparing `modAL-python-0.3.6/modAL_python.egg-info/SOURCES.txt` & `modAL-python-0.4.0/modAL_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

