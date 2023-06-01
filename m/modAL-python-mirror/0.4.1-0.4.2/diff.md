# Comparing `tmp/modAL-python-mirror-0.4.1.tar.gz` & `tmp/modAL-python-mirror-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modAL-python-mirror-0.4.1.tar", last modified: Thu Jun  1 13:09:43 2023, max compression
+gzip compressed data, was "modAL-python-mirror-0.4.2.tar", last modified: Thu Jun  1 12:59:56 2023, max compression
```

## Comparing `modAL-python-mirror-0.4.1.tar` & `modAL-python-mirror-0.4.2.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-01 13:09:43.422501 modAL-python-mirror-0.4.1/
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     1070 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.1/LICENSE
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      313 2023-06-01 13:09:43.422501 modAL-python-mirror-0.4.1/PKG-INFO
--rw-rw-r--   0 paolo     (1000) paolo     (1000)    10828 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/README.md
-drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-01 13:09:43.422501 modAL-python-mirror-0.4.1/modAL/
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      128 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/__init__.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     5560 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/acquisition.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)    11062 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/batch.py
--rwxrwxr-x   0 paolo     (1000) paolo     (1000)      416 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.1/modAL/cluster.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     1762 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.1/modAL/density.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     8825 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/disagreement.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     3071 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/expected_error.py
-drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-01 13:09:43.422501 modAL-python-mirror-0.4.1/modAL/models/
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      180 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/models/__init__.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)    19137 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/models/base.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)    23061 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/models/learners.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)    10447 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/multilabel.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     7850 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/uncertainty.py
-drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-01 13:09:43.422501 modAL-python-mirror-0.4.1/modAL/utils/
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      417 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/utils/__init__.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     3607 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/utils/combination.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     4725 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/utils/data.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     2389 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/utils/selection.py
--rw-rw-r--   0 paolo     (1000) paolo     (1000)     1920 2023-06-01 13:08:37.000000 modAL-python-mirror-0.4.1/modAL/utils/validation.py
-drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-01 13:09:43.422501 modAL-python-mirror-0.4.1/modAL_python_mirror.egg-info/
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      313 2023-06-01 13:09:43.000000 modAL-python-mirror-0.4.1/modAL_python_mirror.egg-info/PKG-INFO
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      618 2023-06-01 13:09:43.000000 modAL-python-mirror-0.4.1/modAL_python_mirror.egg-info/SOURCES.txt
--rw-rw-r--   0 paolo     (1000) paolo     (1000)        1 2023-06-01 13:09:43.000000 modAL-python-mirror-0.4.1/modAL_python_mirror.egg-info/dependency_links.txt
--rw-rw-r--   0 paolo     (1000) paolo     (1000)       57 2023-06-01 13:09:43.000000 modAL-python-mirror-0.4.1/modAL_python_mirror.egg-info/requires.txt
--rw-rw-r--   0 paolo     (1000) paolo     (1000)        6 2023-06-01 13:09:43.000000 modAL-python-mirror-0.4.1/modAL_python_mirror.egg-info/top_level.txt
--rw-rw-r--   0 paolo     (1000) paolo     (1000)       79 2023-06-01 13:09:43.422501 modAL-python-mirror-0.4.1/setup.cfg
--rw-rw-r--   0 paolo     (1000) paolo     (1000)      519 2023-06-01 13:09:19.000000 modAL-python-mirror-0.4.1/setup.py
+drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-01 12:59:56.846968 modAL-python-mirror-0.4.2/
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     1070 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/LICENSE
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      313 2023-06-01 12:59:56.850968 modAL-python-mirror-0.4.2/PKG-INFO
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)    10835 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/README.md
+drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-01 12:59:56.846968 modAL-python-mirror-0.4.2/modAL/
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      129 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/__init__.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     5550 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/acquisition.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)    11276 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/batch.py
+-rwxrwxr-x   0 paolo     (1000) paolo     (1000)      416 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/cluster.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     1762 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/density.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     8826 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/disagreement.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)    19660 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/dropout.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     3160 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/expected_error.py
+drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-01 12:59:56.846968 modAL-python-mirror-0.4.2/modAL/models/
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      247 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/models/__init__.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)    15800 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/models/base.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)    31261 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/models/learners.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)    10589 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/multilabel.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     7895 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/uncertainty.py
+drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-01 12:59:56.846968 modAL-python-mirror-0.4.2/modAL/utils/
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      446 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/utils/__init__.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     3606 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/utils/combination.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     5250 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/utils/data.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     3605 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/utils/selection.py
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)     1920 2023-06-01 12:54:37.000000 modAL-python-mirror-0.4.2/modAL/utils/validation.py
+drwxrwxr-x   0 paolo     (1000) paolo     (1000)        0 2023-06-01 12:59:56.846968 modAL-python-mirror-0.4.2/modAL_python_mirror.egg-info/
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      313 2023-06-01 12:59:56.000000 modAL-python-mirror-0.4.2/modAL_python_mirror.egg-info/PKG-INFO
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      635 2023-06-01 12:59:56.000000 modAL-python-mirror-0.4.2/modAL_python_mirror.egg-info/SOURCES.txt
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)        1 2023-06-01 12:59:56.000000 modAL-python-mirror-0.4.2/modAL_python_mirror.egg-info/dependency_links.txt
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)       65 2023-06-01 12:59:56.000000 modAL-python-mirror-0.4.2/modAL_python_mirror.egg-info/requires.txt
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)        6 2023-06-01 12:59:56.000000 modAL-python-mirror-0.4.2/modAL_python_mirror.egg-info/top_level.txt
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)       79 2023-06-01 12:59:56.850968 modAL-python-mirror-0.4.2/setup.cfg
+-rw-rw-r--   0 paolo     (1000) paolo     (1000)      552 2023-06-01 12:59:40.000000 modAL-python-mirror-0.4.2/setup.py
```

### Comparing `modAL-python-mirror-0.4.1/LICENSE` & `modAL-python-mirror-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modAL-python-mirror-0.4.1/README.md` & `modAL-python-mirror-0.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
 - Python >= 3.5
 - NumPy >= 1.13
 - SciPy >= 0.18
 - scikit-learn >= 0.18
 
 You can install modAL directly with pip:  
 ```
-pip install modAL
+pip install modAL-python
 ```
 Alternatively, you can install modAL directly from source:  
 ```
 pip install git+https://github.com/modAL-python/modAL.git
 ```
 
 # Documentation<a name="documentation"></a>
```

### Comparing `modAL-python-mirror-0.4.1/modAL/acquisition.py` & `modAL-python-mirror-0.4.2/modAL/acquisition.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 """
 Acquisition functions for Bayesian optimization.
 """
-from typing import Tuple
 
 import numpy as np
-from scipy.stats import norm
 from scipy.special import ndtr
+from scipy.stats import norm
 from sklearn.exceptions import NotFittedError
 
-from modAL.utils.selection import multi_argmax
-from modAL.utils.data import modALinput
 from modAL.models.base import BaseLearner
+from modAL.utils.data import modALinput
+from modAL.utils.selection import multi_argmax
 
 
 def PI(mean, std, max_val, tradeoff):
     return ndtr((mean - max_val - tradeoff)/std)
 
 
 def EI(mean, std, max_val, tradeoff):
@@ -111,15 +110,17 @@
     Args:
         optimizer: The :class:`~modAL.models.BayesianOptimizer` object for which the utility is to be calculated.
         X: The samples for which the probability of improvement is to be calculated.
         tradeoff: Value controlling the tradeoff parameter.
         n_instances: Number of samples to be queried.
 
     Returns:
-        The indices of the instances from X chosen to be labelled; the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled.
+        The pi metric of the chosen instances.
+
     """
     pi = optimizer_PI(optimizer, X, tradeoff=tradeoff)
     return multi_argmax(pi, n_instances=n_instances)
 
 
 def max_EI(optimizer: BaseLearner, X: modALinput, tradeoff: float = 0,
            n_instances: int = 1) -> np.ndarray:
@@ -129,15 +130,17 @@
     Args:
         optimizer: The :class:`~modAL.models.BayesianOptimizer` object for which the utility is to be calculated.
         X: The samples for which the expected improvement is to be calculated.
         tradeoff: Value controlling the tradeoff parameter.
         n_instances: Number of samples to be queried.
 
     Returns:
-        The indices of the instances from X chosen to be labelled; the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled. 
+        The ei metric of the chosen instances.
+
     """
     ei = optimizer_EI(optimizer, X, tradeoff=tradeoff)
     return multi_argmax(ei, n_instances=n_instances)
 
 
 def max_UCB(optimizer: BaseLearner, X: modALinput, beta: float = 1,
             n_instances: int = 1) -> np.ndarray:
@@ -147,11 +150,13 @@
     Args:
         optimizer: The :class:`~modAL.models.BayesianOptimizer` object for which the utility is to be calculated.
         X: The samples for which the maximum upper confidence bound is to be calculated.
         beta: Value controlling the beta parameter.
         n_instances: Number of samples to be queried.
 
     Returns:
-        The indices of the instances from X chosen to be labelled; the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled. 
+        The ucb metric of the chosen instances.
+
     """
     ucb = optimizer_UCB(optimizer, X, beta=beta)
     return multi_argmax(ucb, n_instances=n_instances)
```

### Comparing `modAL-python-mirror-0.4.1/modAL/batch.py` & `modAL-python-mirror-0.4.2/modAL/batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 Uncertainty measures that explicitly support batch-mode sampling for active learning models.
 """
 
 from typing import Callable, Optional, Tuple, Union
 
 import numpy as np
 import scipy.sparse as sp
-from sklearn.metrics.pairwise import pairwise_distances, pairwise_distances_argmin_min
+from sklearn.metrics.pairwise import (pairwise_distances,
+                                      pairwise_distances_argmin_min)
 
-from modAL.utils.data import data_vstack, modALinput, data_shape
 from modAL.models.base import BaseCommittee, BaseLearner
 from modAL.uncertainty import classifier_uncertainty
+from modAL.utils.data import data_shape, data_vstack, modALinput
 
 
 def select_cold_start_instance(X: modALinput,
                                metric: Union[str, Callable],
                                n_jobs: Union[int, None]) -> Tuple[int, modALinput]:
     """
     Define what to do if our batch-mode sampling doesn't have any labeled data -- a cold start.
@@ -135,14 +136,16 @@
         uncertainty_scores: Our classifier's predictions over the response variable.
         n_instances: Limit on the number of records to query from our unlabeled set.
         metric: This parameter is passed to :func:`~sklearn.metrics.pairwise.pairwise_distances`.
         n_jobs: This parameter is passed to :func:`~sklearn.metrics.pairwise.pairwise_distances`.
 
     Returns:
         The indices of the top n_instances ranked unlabelled samples.
+        The uncertainty scores of the chosen instances. 
+
     """
     # Make a local copy of our classifier's training data.
     # Define our record container and record the best cold start instance in the case of cold start.
 
     # transform unlabeled data if needed
     if classifier.on_transformed:
         unlabeled = classifier.transform_without_estimating(unlabeled)
@@ -156,15 +159,15 @@
         ) if classifier.on_transformed else classifier.X_training[:]
         instance_index_ranking = []
     
     # The maximum number of records to sample.
     ceiling = np.minimum(unlabeled.shape[0], n_instances) - len(instance_index_ranking)
 
     # mask for unlabeled initialized as transparent
-    mask = np.ones(unlabeled.shape[0], np.bool)
+    mask = np.ones(unlabeled.shape[0], bool)
 
     for _ in range(ceiling):
 
         # Receive the instance and corresponding index from our unlabeled copy that scores highest.
         instance_index, instance, mask = select_instance(X_training=labeled, X_pool=unlabeled,
                                                          X_uncertainty=uncertainty_scores, mask=mask,
                                                          metric=metric, n_jobs=n_jobs)
@@ -174,15 +177,15 @@
         # that we don't query the same instance redundantly.
         labeled = data_vstack((labeled, instance))
 
         # Finally, append our instance's index to the bottom of our ranking.
         instance_index_ranking.append(instance_index)
 
     # Return numpy array, not a list.
-    return np.array(instance_index_ranking)
+    return np.array(instance_index_ranking), uncertainty_scores[np.array(instance_index_ranking)]
 
 
 def uncertainty_batch_sampling(classifier: Union[BaseLearner, BaseCommittee],
                                X: Union[np.ndarray, sp.csr_matrix],
                                n_instances: int = 20,
                                metric: Union[str, Callable] = 'euclidean',
                                n_jobs: Optional[int] = None,
@@ -206,13 +209,16 @@
         n_instances: Number of records to return for labeling from `X`.
         metric: This parameter is passed to :func:`~sklearn.metrics.pairwise.pairwise_distances`
         n_jobs: If not set, :func:`~sklearn.metrics.pairwise.pairwise_distances_argmin_min` is used for calculation of
             distances between samples. Otherwise it is passed to :func:`~sklearn.metrics.pairwise.pairwise_distances`.
         **uncertainty_measure_kwargs: Keyword arguments to be passed for the :meth:`predict_proba` of the classifier.
 
     Returns:
-        Indices of the instances from `X` chosen to be labelled; records from `X` chosen to be labelled.
+        Indices of the instances from `X` chosen to be labelled
+        Records from `X` chosen to be labelled.
+        The uncertainty scores of the chosen instances. 
+
     """
     uncertainty = classifier_uncertainty(classifier, X, **uncertainty_measure_kwargs)
     return ranked_batch(classifier, unlabeled=X, uncertainty_scores=uncertainty,
                                  n_instances=n_instances, metric=metric, n_jobs=n_jobs)
```

### Comparing `modAL-python-mirror-0.4.1/modAL/density.py` & `modAL-python-mirror-0.4.2/modAL/density.py`

 * *Files identical despite different names*

### Comparing `modAL-python-mirror-0.4.1/modAL/disagreement.py` & `modAL-python-mirror-0.4.2/modAL/disagreement.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 """
 Disagreement measures and disagreement based query strategies for the Committee model.
 """
 from collections import Counter
-from typing import Tuple
 
 import numpy as np
 from scipy.stats import entropy
-from sklearn.exceptions import NotFittedError
 from sklearn.base import BaseEstimator
+from sklearn.exceptions import NotFittedError
 
+from modAL.models.base import BaseCommittee
 from modAL.utils.data import modALinput
 from modAL.utils.selection import multi_argmax, shuffled_argmax
-from modAL.models.base import BaseCommittee
 
 
 def vote_entropy(committee: BaseCommittee, X: modALinput, **predict_proba_kwargs) -> np.ndarray:
     """
     Calculates the vote entropy for the Committee. First it computes the predictions of X for each learner in the
     Committee, then calculates the probability distribution of the votes. The entropy of this distribution is the vote
     entropy of the Committee, which is returned.
@@ -112,16 +111,17 @@
         n_instances: Number of samples to be queried.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
         **disagreement_measure_kwargs: Keyword arguments to be passed for the disagreement
             measure function.
 
     Returns:
-        The indices of the instances from X chosen to be labelled;
-         the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled.
+        The disagrerment metric of the chosen instances. 
+
     """
     disagreement = vote_entropy(committee, X, **disagreement_measure_kwargs)
 
     if not random_tie_break:
         return multi_argmax(disagreement, n_instances=n_instances)
 
     return shuffled_argmax(disagreement, n_instances=n_instances)
@@ -139,16 +139,17 @@
         n_instances: Number of samples to be queried.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
         **disagreement_measure_kwargs: Keyword arguments to be passed for the disagreement
             measure function.
 
     Returns:
-        The indices of the instances from X chosen to be labelled;
-        the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled.
+        The disagrerment metric of the chosen instances. 
+
     """
     disagreement = consensus_entropy(committee, X, **disagreement_measure_kwargs)
 
     if not random_tie_break:
         return multi_argmax(disagreement, n_instances=n_instances)
 
     return shuffled_argmax(disagreement, n_instances=n_instances)
@@ -166,16 +167,17 @@
         n_instances: Number of samples to be queried.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
         **disagreement_measure_kwargs: Keyword arguments to be passed for the disagreement
          measure function.
 
     Returns:
-        The indices of the instances from X chosen to be labelled;
-        the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled.
+        The disagrerment metric of the chosen instances. 
+
     """
     disagreement = KL_max_disagreement(committee, X, **disagreement_measure_kwargs)
 
     if not random_tie_break:
         return multi_argmax(disagreement, n_instances=n_instances)
 
     return shuffled_argmax(disagreement, n_instances=n_instances)
@@ -192,16 +194,17 @@
         X: The pool of samples to query from.
         n_instances: Number of samples to be queried.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
         **predict_kwargs: Keyword arguments to be passed to :meth:`predict` of the CommiteeRegressor.
 
     Returns:
-        The indices of the instances from X chosen to be labelled;
-        the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled.
+        The standard deviation of the chosen instances. 
+
     """
     _, std = regressor.predict(X, return_std=True, **predict_kwargs)
     std = std.reshape(X.shape[0], )
 
     if not random_tie_break:
         return multi_argmax(std, n_instances=n_instances)
```

### Comparing `modAL-python-mirror-0.4.1/modAL/expected_error.py` & `modAL-python-mirror-0.4.2/modAL/expected_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """
 Expected error reduction framework for active learning.
 """
 
 from typing import Tuple
 
 import numpy as np
-
 from sklearn.base import clone
 from sklearn.exceptions import NotFittedError
 
 from modAL.models import ActiveLearner
-from modAL.utils.data import modALinput, data_vstack, enumerate_data, drop_rows, data_shape, add_row
-from modAL.utils.selection import multi_argmax, shuffled_argmax
-from modAL.uncertainty import _proba_uncertainty, _proba_entropy
+from modAL.uncertainty import _proba_entropy, _proba_uncertainty
+from modAL.utils.data import (add_row, data_shape, data_vstack, drop_rows,
+                              enumerate_data, modALinput)
+from modAL.utils.selection import multi_argmin, shuffled_argmin
 
 
 def expected_error_reduction(learner: ActiveLearner, X: modALinput, loss: str = 'binary',
                              p_subsample: np.float = 1.0, n_instances: int = 1,
                              random_tie_break: bool = False) -> np.ndarray:
     """
     Expected error reduction query strategy.
@@ -35,14 +35,15 @@
         n_instances: The number of instances to be sampled.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
 
 
     Returns:
         The indices of the instances from X chosen to be labelled.
+        The expected error metric of the chosen instances; 
     """
 
     assert 0.0 <= p_subsample <= 1.0, 'p_subsample subsampling keep ratio must be between 0.0 and 1.0'
     assert loss in ['binary', 'log'], 'loss must be \'binary\' or \'log\''
 
     expected_error = np.zeros(shape=(data_shape(X)[0],))
     possible_labels = np.unique(learner.y_training)
@@ -73,10 +74,10 @@
 
                 expected_error[x_idx] += np.sum(nloss)*X_proba[x_idx, y_idx]
 
         else:
             expected_error[x_idx] = np.inf
 
     if not random_tie_break:
-        return multi_argmax(-expected_error, n_instances)
+        return multi_argmin(expected_error, n_instances)
 
-    return shuffled_argmax(-expected_error, n_instances)
+    return shuffled_argmin(expected_error, n_instances)
```

### Comparing `modAL-python-mirror-0.4.1/modAL/models/base.py` & `modAL-python-mirror-0.4.2/modAL/models/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,25 +2,22 @@
 Base classes for active learning algorithms
 ------------------------------------------
 """
 
 import abc
 import sys
 import warnings
-from typing import Union, Callable, Optional, Tuple, List, Iterator, Any
+from typing import Any, Callable, Iterator, List, Tuple, Union
 
 import numpy as np
+import scipy.sparse as sp
+from modAL.utils.data import data_hstack, modALinput, retrieve_rows
 from sklearn.base import BaseEstimator
 from sklearn.ensemble._base import _BaseHeterogeneousEnsemble
 from sklearn.pipeline import Pipeline
-from sklearn.utils import check_X_y
-
-import scipy.sparse as sp
-
-from modAL.utils.data import data_vstack, data_hstack, modALinput, retrieve_rows
 
 if sys.version_info >= (3, 4):
     ABC = abc.ABC
 else:
     ABC = abc.ABCMeta('ABC', (), {})
 
 
@@ -28,81 +25,42 @@
     """
     Core abstraction in modAL.
 
     Args:
         estimator: The estimator to be used in the active learning loop.
         query_strategy: Function providing the query strategy for the active learning loop,
             for instance, modAL.uncertainty.uncertainty_sampling.
-        X_training: Initial training samples, if available.
-        y_training: Initial training labels corresponding to initial training samples.
         force_all_finite: When True, forces all values of the data finite.
             When False, accepts np.nan and np.inf values.
-        bootstrap_init: If initial training data is available, bootstrapping can be done during the first training.
-            Useful when building Committee models with bagging.
         on_transformed: Whether to transform samples with the pipeline defined by the estimator
             when applying the query strategy.
         **fit_kwargs: keyword arguments.
 
     Attributes:
         estimator: The estimator to be used in the active learning loop.
         query_strategy: Function providing the query strategy for the active learning loop.
-        X_training: If the model hasn't been fitted yet it is None, otherwise it contains the samples
-            which the model has been trained on.
-        y_training: The labels corresponding to X_training.
     """
+
     def __init__(self,
                  estimator: BaseEstimator,
                  query_strategy: Callable,
-                 X_training: Optional[modALinput] = None,
-                 y_training: Optional[modALinput] = None,
-                 bootstrap_init: bool = False,
                  on_transformed: bool = False,
                  force_all_finite: bool = True,
                  **fit_kwargs
                  ) -> None:
         assert callable(query_strategy), 'query_strategy must be callable'
 
         self.estimator = estimator
         self.query_strategy = query_strategy
         self.on_transformed = on_transformed
 
-        self.X_training = X_training
-        self.y_training = y_training
-        if X_training is not None:
-            self._fit_to_known(bootstrap=bootstrap_init, **fit_kwargs)
-
-        assert isinstance(force_all_finite, bool), 'force_all_finite must be a bool'
+        assert isinstance(force_all_finite,
+                          bool), 'force_all_finite must be a bool'
         self.force_all_finite = force_all_finite
 
-    def _add_training_data(self, X: modALinput, y: modALinput) -> None:
-        """
-        Adds the new data and label to the known data, but does not retrain the model.
-
-        Args:
-            X: The new samples for which the labels are supplied by the expert.
-            y: Labels corresponding to the new instances in X.
-
-        Note:
-            If the classifier has been fitted, the features in X have to agree with the training samples which the
-            classifier has seen.
-        """
-        check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
-                  force_all_finite=self.force_all_finite)
-
-        if self.X_training is None:
-            self.X_training = X
-            self.y_training = y
-        else:
-            try:
-                self.X_training = data_vstack((self.X_training, X))
-                self.y_training = data_vstack((self.y_training, y))
-            except ValueError:
-                raise ValueError('the dimensions of the new training data and label must'
-                                 'agree with the training data and labels provided so far')
-
     def transform_without_estimating(self, X: modALinput) -> Union[np.ndarray, sp.csr_matrix]:
         """
         Transforms the data as supplied to the estimator.
 
         * In case the estimator is an skearn pipeline, it applies all pipeline components but the last one.
         * In case the estimator is an ensemble, it concatenates the transformations for each classfier
             (pipeline) in the ensemble.
@@ -124,93 +82,53 @@
         for pipe in pipes:
             if isinstance(pipe, Pipeline):
                 # NOTE: The used pipeline class might be an extension to sklearn's!
                 #       Create a new instance of the used pipeline class with all
                 #       components but the final estimator, which is replaced by an empty (passthrough) component.
                 #       This prevents any special handling of the final transformation pipe, which is usually
                 #       expected to be an estimator.
-                transformation_pipe = pipe.__class__(steps=[*pipe.steps[:-1], ('passthrough', 'passthrough')])
+                transformation_pipe = pipe.__class__(
+                    steps=[*pipe.steps[:-1], ('passthrough', 'passthrough')])
                 Xt.append(transformation_pipe.transform(X))
 
         # in case no transformation pipelines are used by the estimator,
         # return the original, non-transfored data
         if not Xt:
             return X
 
         ################################
         # concatenate all transformations and return
         return data_hstack(Xt)
 
-    def _fit_to_known(self, bootstrap: bool = False, **fit_kwargs) -> 'BaseLearner':
-        """
-        Fits self.estimator to the training data and labels provided to it so far.
-
-        Args:
-            bootstrap: If True, the method trains the model on a set bootstrapped from the known training instances.
-            **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
-
-        Returns:
-            self
-        """
-        if not bootstrap:
-            self.estimator.fit(self.X_training, self.y_training, **fit_kwargs)
-        else:
-            n_instances = self.X_training.shape[0]
-            bootstrap_idx = np.random.choice(range(n_instances), n_instances, replace=True)
-            self.estimator.fit(self.X_training[bootstrap_idx], self.y_training[bootstrap_idx], **fit_kwargs)
-
-        return self
-
     def _fit_on_new(self, X: modALinput, y: modALinput, bootstrap: bool = False, **fit_kwargs) -> 'BaseLearner':
         """
         Fits self.estimator to the given data and labels.
 
         Args:
             X: The new samples for which the labels are supplied by the expert.
             y: Labels corresponding to the new instances in X.
             bootstrap: If True, the method trains the model on a set bootstrapped from X.
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
 
         Returns:
             self
         """
-        check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
-                  force_all_finite=self.force_all_finite)
 
         if not bootstrap:
             self.estimator.fit(X, y, **fit_kwargs)
         else:
-            bootstrap_idx = np.random.choice(range(X.shape[0]), X.shape[0], replace=True)
+            bootstrap_idx = np.random.choice(
+                range(X.shape[0]), X.shape[0], replace=True)
             self.estimator.fit(X[bootstrap_idx], y[bootstrap_idx])
 
         return self
 
-    def fit(self, X: modALinput, y: modALinput, bootstrap: bool = False, **fit_kwargs) -> 'BaseLearner':
-        """
-        Interface for the fit method of the predictor. Fits the predictor to the supplied data, then stores it
-        internally for the active learning loop.
-
-        Args:
-            X: The samples to be fitted.
-            y: The corresponding labels.
-            bootstrap: If true, trains the estimator on a set bootstrapped from X.
-                Useful for building Committee models with bagging.
-            **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
-
-        Note:
-            When using scikit-learn estimators, calling this method will make the ActiveLearner forget all training data
-            it has seen!
-
-        Returns:
-            self
-        """
-        check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
-                  force_all_finite=self.force_all_finite)
-        self.X_training, self.y_training = X, y
-        return self._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
+    @abc.abstractmethod
+    def fit(self, *args, **kwargs) -> None:
+        pass
 
     def predict(self, X: modALinput, **predict_kwargs) -> Any:
         """
         Estimator predictions for X. Interface with the predict method of the estimator.
 
         Args:
             X: The samples to be predicted.
@@ -230,39 +148,49 @@
             **predict_proba_kwargs: Keyword arguments to be passed to the predict_proba method of the classifier.
 
         Returns:
             Class probabilities for X.
         """
         return self.estimator.predict_proba(X, **predict_proba_kwargs)
 
-    def query(self, X_pool, *query_args, **query_kwargs) -> Union[Tuple, modALinput]:
+    def query(self, X_pool, *query_args, return_metrics: bool = False, **query_kwargs) -> Union[Tuple, modALinput]:
         """
         Finds the n_instances most informative point in the data provided by calling the query_strategy function.
 
         Args:
             X_pool: Pool of unlabeled instances to retrieve most informative instances from
+            return_metrics: boolean to indicate, if the corresponding query metrics should be (not) returned
             *query_args: The arguments for the query strategy. For instance, in the case of
                 :func:`~modAL.uncertainty.uncertainty_sampling`, it is the pool of samples from which the query strategy
                 should choose instances to request labels.
             **query_kwargs: Keyword arguments for the query strategy function.
 
         Returns:
             Value of the query_strategy function. Should be the indices of the instances from the pool chosen to be
             labelled and the instances themselves. Can be different in other cases, for instance only the instance to be
             labelled upon query synthesis.
+            query_metrics: returns also the corresponding metrics, if return_metrics == True
         """
-        query_result = self.query_strategy(self, X_pool, *query_args, **query_kwargs)
 
-        if isinstance(query_result, tuple):
-            warnings.warn("Query strategies should no longer return the selected instances, "
-                          "this is now handled by the query method. "
-                          "Please return only the indices of the selected instances.", DeprecationWarning)
-            return query_result
-
-        return query_result, retrieve_rows(X_pool, query_result)
+        try:
+            query_result, query_metrics = self.query_strategy(
+                self, X_pool, *query_args, **query_kwargs)
+
+        except:
+            query_metrics = None
+            query_result = self.query_strategy(
+                self, X_pool, *query_args, **query_kwargs)
+
+        if return_metrics:
+            if query_metrics is None: 
+                warnings.warn(
+                "The selected query strategy doesn't support return_metrics")
+            return query_result, retrieve_rows(X_pool, query_result), query_metrics
+        else:
+            return query_result, retrieve_rows(X_pool, query_result)
 
     def score(self, X: modALinput, y: modALinput, **score_kwargs) -> Any:
         """
         Interface for the score method of the predictor.
 
         Args:
             X: The samples for which prediction accuracy is to be calculated.
@@ -278,15 +206,14 @@
     def teach(self, *args, **kwargs) -> None:
         pass
 
 
 class BaseCommittee(ABC, BaseEstimator):
     """
     Base class for query-by-committee setup.
-
     Args:
         learner_list: List of ActiveLearner objects to form committee.
         query_strategy: Function to query labels.
         on_transformed: Whether to transform samples with the pipeline defined by each learner's estimator
             when applying the query strategy.
     """
     def __init__(self, learner_list: List[BaseLearner], query_strategy: Callable, on_transformed: bool = False) -> None:
@@ -304,59 +231,53 @@
 
     def __len__(self) -> int:
         return len(self.learner_list)
 
     def _add_training_data(self, X: modALinput, y: modALinput) -> None:
         """
         Adds the new data and label to the known data for each learner, but does not retrain the model.
-
         Args:
             X: The new samples for which the labels are supplied by the expert.
             y: Labels corresponding to the new instances in X.
-
         Note:
             If the learners have been fitted, the features in X have to agree with the training samples which the
             classifier has seen.
         """
         for learner in self.learner_list:
             learner._add_training_data(X, y)
 
     def _fit_to_known(self, bootstrap: bool = False, **fit_kwargs) -> None:
         """
         Fits all learners to the training data and labels provided to it so far.
-
         Args:
             bootstrap: If True, each estimator is trained on a bootstrapped dataset. Useful when
                 using bagging to build the ensemble.
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
         """
         for learner in self.learner_list:
             learner._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
 
     def _fit_on_new(self, X: modALinput, y: modALinput, bootstrap: bool = False, **fit_kwargs) -> None:
         """
         Fits all learners to the given data and labels.
-
         Args:
             X: The new samples for which the labels are supplied by the expert.
             y: Labels corresponding to the new instances in X.
             bootstrap: If True, the method trains the model on a set bootstrapped from X.
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
         """
         for learner in self.learner_list:
             learner._fit_on_new(X, y, bootstrap=bootstrap, **fit_kwargs)
 
     def fit(self, X: modALinput, y: modALinput, **fit_kwargs) -> 'BaseCommittee':
         """
         Fits every learner to a subset sampled with replacement from X. Calling this method makes the learner forget the
         data it has seen up until this point and replaces it with X! If you would like to perform bootstrapping on each
         learner using the data it has seen, use the method .rebag()!
-
         Calling this method makes the learner forget the data it has seen up until this point and replaces it with X!
-
         Args:
             X: The samples to be fitted on.
             y: The corresponding labels.
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
         """
         for learner in self.learner_list:
             learner.fit(X, y, **fit_kwargs)
@@ -364,63 +285,69 @@
         return self
 
     def transform_without_estimating(self, X: modALinput) -> Union[np.ndarray, sp.csr_matrix]:
         """
         Transforms the data as supplied to each learner's estimator and concatenates transformations.
         Args:
             X: dataset to be transformed
-
         Returns:
             Transformed data set
         """
         return data_hstack([learner.transform_without_estimating(X) for learner in self.learner_list])
 
-    def query(self, X_pool, *query_args, **query_kwargs) -> Union[Tuple, modALinput]:
+    def query(self, X_pool, return_metrics: bool = False, *query_args, **query_kwargs) -> Union[Tuple, modALinput]:
         """
         Finds the n_instances most informative point in the data provided by calling the query_strategy function.
 
         Args:
             X_pool: Pool of unlabeled instances to retrieve most informative instances from
+            return_metrics: boolean to indicate, if the corresponding query metrics should be (not) returned
             *query_args: The arguments for the query strategy. For instance, in the case of
                 :func:`~modAL.disagreement.max_disagreement_sampling`, it is the pool of samples from which the query.
                 strategy should choose instances to request labels.
             **query_kwargs: Keyword arguments for the query strategy function.
 
         Returns:
             Return value of the query_strategy function. Should be the indices of the instances from the pool chosen to
             be labelled and the instances themselves. Can be different in other cases, for instance only the instance to
             be labelled upon query synthesis.
+            query_metrics: returns also the corresponding metrics, if return_metrics == True
         """
-        query_result = self.query_strategy(self, X_pool, *query_args, **query_kwargs)
 
-        if isinstance(query_result, tuple):
-            warnings.warn("Query strategies should no longer return the selected instances, "
-                          "this is now handled by the query method. "
-                          "Please return only the indices of the selected instances", DeprecationWarning)
-            return query_result
-
-        return query_result, retrieve_rows(X_pool, query_result)
+        try:
+            query_result, query_metrics = self.query_strategy(
+                self, X_pool, *query_args, **query_kwargs)
+
+        except:
+            query_metrics = None
+            query_result = self.query_strategy(
+                self, X_pool, *query_args, **query_kwargs)
+
+        if return_metrics:
+            if query_metrics is None: 
+                warnings.warn(
+                "The selected query strategy doesn't support return_metrics")
+            return query_result, retrieve_rows(X_pool, query_result), query_metrics
+        else:
+            return query_result, retrieve_rows(X_pool, query_result)
 
     def rebag(self, **fit_kwargs) -> None:
         """
         Refits every learner with a dataset bootstrapped from its training instances. Contrary to .bag(), it bootstraps
         the training data for each learner based on its own examples.
-
         Todo:
             Where is .bag()?
-
         Args:
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
         """
         self._fit_to_known(bootstrap=True, **fit_kwargs)
 
     def teach(self, X: modALinput, y: modALinput, bootstrap: bool = False, only_new: bool = False, **fit_kwargs) -> None:
         """
         Adds X and y to the known training data for each learner and retrains learners with the augmented dataset.
-
         Args:
             X: The new samples for which the labels are supplied by the expert.
             y: Labels corresponding to the new instances in X.
             bootstrap: If True, trains each learner on a bootstrapped set. Useful when building the ensemble by bagging.
             only_new: If True, the model is retrained using only X and y, ignoring the previously provided examples.
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
         """
@@ -432,8 +359,9 @@
 
     @abc.abstractmethod
     def predict(self, X: modALinput) -> Any:
         pass
 
     @abc.abstractmethod
     def vote(self, X: modALinput) -> Any:  # TODO: clarify typing
-        pass
+        pass
+
```

### Comparing `modAL-python-mirror-0.4.1/modAL/models/learners.py` & `modAL-python-mirror-0.4.2/modAL/models/learners.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-import numpy as np
-
-from typing import Callable, Optional, Tuple, List, Any
+from typing import Any, Callable, List, Optional, Tuple
 
+import numpy as np
+from modAL.acquisition import max_EI
+from modAL.disagreement import max_std_sampling, vote_entropy_sampling
+from modAL.models.base import BaseCommittee, BaseLearner
+from modAL.uncertainty import uncertainty_sampling
+from modAL.utils.data import data_vstack, modALinput, retrieve_rows
+from modAL.utils.validation import check_class_labels, check_class_proba
 from sklearn.base import BaseEstimator
 from sklearn.metrics import accuracy_score
-
-from modAL.models.base import BaseLearner, BaseCommittee
-from modAL.utils.validation import check_class_labels, check_class_proba
-from modAL.utils.data import modALinput, retrieve_rows
-from modAL.uncertainty import uncertainty_sampling
-from modAL.disagreement import vote_entropy_sampling, max_std_sampling
-from modAL.acquisition import max_EI
+from sklearn.utils import check_X_y
 
 """
 Classes for active learning algorithms
 --------------------------------------
 """
 
 
 class ActiveLearner(BaseLearner):
     """
-    This class is an abstract model of a general active learning algorithm.
+    This class is an model of a general classic (machine learning) active learning algorithm.
 
     Args:
         estimator: The estimator to be used in the active learning loop.
         query_strategy: Function providing the query strategy for the active learning loop,
             for instance, modAL.uncertainty.uncertainty_sampling.
         X_training: Initial training samples, if available.
         y_training: Initial training labels corresponding to initial training samples.
@@ -74,16 +73,93 @@
                  query_strategy: Callable = uncertainty_sampling,
                  X_training: Optional[modALinput] = None,
                  y_training: Optional[modALinput] = None,
                  bootstrap_init: bool = False,
                  on_transformed: bool = False,
                  **fit_kwargs
                  ) -> None:
-        super().__init__(estimator, query_strategy,
-                         X_training, y_training, bootstrap_init, on_transformed, **fit_kwargs)
+        super().__init__(estimator, query_strategy, on_transformed, **fit_kwargs)
+
+        self.X_training = X_training
+        self.y_training = y_training
+
+        if X_training is not None:
+            self._fit_to_known(bootstrap=bootstrap_init, **fit_kwargs)
+
+    def _add_training_data(self, X: modALinput, y: modALinput) -> None:
+        """
+        Adds the new data and label to the known data, but does not retrain the model.
+
+        Args:
+            X: The new samples for which the labels are supplied by the expert.
+            y: Labels corresponding to the new instances in X.
+
+        Note:
+            If the classifier has been fitted, the features in X have to agree with the training samples which the
+            classifier has seen.
+        """
+        check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
+                  force_all_finite=self.force_all_finite)
+
+        if self.X_training is None:
+            self.X_training = X
+            self.y_training = y
+        else:
+            try:
+                self.X_training = data_vstack((self.X_training, X))
+                self.y_training = data_vstack((self.y_training, y))
+            except ValueError:
+                raise ValueError('the dimensions of the new training data and label must'
+                                 'agree with the training data and labels provided so far')
+
+    def _fit_to_known(self, bootstrap: bool = False, **fit_kwargs) -> 'BaseLearner':
+        """
+        Fits self.estimator to the training data and labels provided to it so far.
+
+        Args:
+            bootstrap: If True, the method trains the model on a set bootstrapped from the known training instances.
+            **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
+
+        Returns:
+            self
+        """
+        if not bootstrap:
+            self.estimator.fit(self.X_training, self.y_training, **fit_kwargs)
+        else:
+            n_instances = self.X_training.shape[0]
+            bootstrap_idx = np.random.choice(
+                range(n_instances), n_instances, replace=True)
+            self.estimator.fit(
+                self.X_training[bootstrap_idx], self.y_training[bootstrap_idx], **fit_kwargs)
+
+        return self
+
+    def fit(self, X: modALinput, y: modALinput, bootstrap: bool = False, **fit_kwargs) -> 'BaseLearner':
+        """
+        Interface for the fit method of the predictor. Fits the predictor to the supplied data, then stores it
+        internally for the active learning loop.
+
+        Args:
+            X: The samples to be fitted.
+            y: The corresponding labels.
+            bootstrap: If true, trains the estimator on a set bootstrapped from X.
+                Useful for building Committee models with bagging.
+            **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
+
+        Note:
+            When using scikit-learn estimators, calling this method will make the ActiveLearner forget all training data
+            it has seen!
+
+        Returns:
+            self
+        """
+        check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
+                  force_all_finite=self.force_all_finite)
+        self.X_training, self.y_training = X, y
+        return self._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
 
     def teach(self, X: modALinput, y: modALinput, bootstrap: bool = False, only_new: bool = False, **fit_kwargs) -> None:
         """
         Adds X and y to the known training data and retrains the predictor with the augmented dataset.
 
         Args:
             X: The new samples for which the labels are supplied by the expert.
@@ -91,28 +167,146 @@
             bootstrap: If True, training is done on a bootstrapped dataset. Useful for building Committee models
                 with bagging.
             only_new: If True, the model is retrained using only X and y, ignoring the previously provided examples.
                 Useful when working with models where the .fit() method doesn't retrain the model from scratch (e. g. in
                 tensorflow or keras).
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
         """
-        self._add_training_data(X, y)
         if not only_new:
+            self._add_training_data(X, y)
             self._fit_to_known(bootstrap=bootstrap, **fit_kwargs)
         else:
+            check_X_y(X, y, accept_sparse=True, ensure_2d=False, allow_nd=True, multi_output=True, dtype=None,
+                      force_all_finite=self.force_all_finite)
             self._fit_on_new(X, y, bootstrap=bootstrap, **fit_kwargs)
 
 
+class DeepActiveLearner(BaseLearner):
+    """
+    This class is an model of a general deep active learning algorithm.
+    Differences to the classical ActiveLearner are:
+        - Data is no member variable of the DeepActiveLearner class
+        - Misses the initial add/train data methods, therefore always trains on new data
+        - Uses different interfaces to sklearn in some functions
+
+    Args:
+        estimator: The estimator to be used in the active learning loop.
+        query_strategy: Function providing the query strategy for the active learning loop,
+            for instance, modAL.uncertainty.uncertainty_sampling.
+        on_transformed: Whether to transform samples with the pipeline defined by the estimator
+            when applying the query strategy.
+        **fit_kwargs: keyword arguments.
+
+    Attributes:
+        estimator: The estimator to be used in the active learning loop.
+        query_strategy: Function providing the query strategy for the active learning loop.
+    """
+
+    def __init__(self,
+                 estimator: BaseEstimator,
+                 query_strategy: Callable = uncertainty_sampling,
+                 on_transformed: bool = False,
+                 **fit_kwargs
+                 ) -> None:
+        # TODO: Check if given query strategy works for Deep Learning
+        super().__init__(estimator, query_strategy, on_transformed, **fit_kwargs)
+
+        self.estimator.initialize()
+
+    def fit(self, X: modALinput, y: modALinput, bootstrap: bool = False, **fit_kwargs) -> 'BaseLearner':
+        """
+        Interface for the fit method of the predictor. Fits the predictor to the supplied data.
+
+        Args:
+            X: The samples to be fitted.
+            y: The corresponding labels.
+            bootstrap: If true, trains the estimator on a set bootstrapped from X.
+                Useful for building Committee models with bagging.
+            **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
+
+        Returns:
+            self
+        """
+        return self._fit_on_new(X, y, bootstrap=bootstrap, **fit_kwargs)
+
+    def teach(self, X: modALinput, y: modALinput, warm_start: bool = True, bootstrap: bool = False, **fit_kwargs) -> None:
+        """
+        Trains the predictor with the passed data (warm_start decides if params are resetted or not). 
+
+        Args:
+            X: The new samples for which the labels are supplied by the expert.
+            y: Labels corresponding to the new instances in X.
+            warm_start: If False, the model parameters are resetted and the training starts from zero, 
+                otherwise the pre trained model is kept and further trained.
+            bootstrap: If True, training is done on a bootstrapped dataset. Useful for building Committee models
+                with bagging.
+            **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
+        """
+
+        if warm_start:
+            if not bootstrap:
+                self.estimator.partial_fit(X, y, **fit_kwargs)
+            else:
+                bootstrap_idx = np.random.choice(
+                    range(X.shape[0]), X.shape[0], replace=True)
+                self.estimator.partial_fit(
+                    X[bootstrap_idx], y[bootstrap_idx], **fit_kwargs)
+        else:
+            self._fit_on_new(X, y, bootstrap=bootstrap, **fit_kwargs)
+
+    @property
+    def num_epochs(self):
+        """
+        Returns the number of epochs of a single fit cycle.
+        """
+        return self.estimator.max_epochs
+
+    @num_epochs.setter
+    def num_epochs(self, value):
+        """
+        Sets the number of epochs of a single fit cycle. The number of epochs 
+        can be changed at any time, even after the model was trained.
+        """
+        if isinstance(value, int):
+            if 0 < value:
+                self.estimator.max_epochs = value
+            else:
+                raise ValueError("num_epochs must be larger than zero")
+        else:
+            raise TypeError("num_epochs must be of type integer!")
+
+    @property
+    def batch_size(self):
+        """
+        Returns the batch size of a single forward pass.
+        """
+        return self.estimator.batch_size
+
+    @batch_size.setter
+    def batch_size(self, value):
+        """
+        Sets the batch size of a single forward pass. The batch size 
+        can be changed at any time, even after the model was trained.
+        """
+        if isinstance(value, int):
+            if 0 < value:
+                self.estimator.batch_size = value
+            else:
+                raise ValueError("batch size must be larger than 0")
+        else:
+            raise TypeError("batch size must be of type integer!")
+
+
 """
 Classes for Bayesian optimization
 ---------------------------------
 """
 
 
-class BayesianOptimizer(BaseLearner):
+class BayesianOptimizer(ActiveLearner):
     """
     This class is an abstract model of a Bayesian optimizer algorithm.
 
     Args:
         estimator: The estimator to be used in the Bayesian optimization. (For instance, a
             GaussianProcessRegressor.)
         query_strategy: Function providing the query strategy for Bayesian optimization,
@@ -170,14 +364,15 @@
         ...     )
         ...
         ...     for n_query in range(5):
         ...         # query
         ...         query_idx, query_inst = optimizer.query(X)
         ...         optimizer.teach(X[query_idx].reshape(1, -1), y[query_idx].reshape(1, -1))
     """
+
     def __init__(self,
                  estimator: BaseEstimator,
                  query_strategy: Callable = max_EI,
                  X_training: Optional[modALinput] = None,
                  y_training: Optional[modALinput] = None,
                  bootstrap_init: bool = False,
                  on_transformed: bool = False,
@@ -239,28 +434,24 @@
 --------------------------------------
 """
 
 
 class Committee(BaseCommittee):
     """
     This class is an abstract model of a committee-based active learning algorithm.
-
     Args:
         learner_list: A list of ActiveLearners forming the Committee.
         query_strategy: Query strategy function. Committee supports disagreement-based query strategies from
             :mod:`modAL.disagreement`, but uncertainty-based ones from :mod:`modAL.uncertainty` are also supported.
         on_transformed: Whether to transform samples with the pipeline defined by each learner's estimator
             when applying the query strategy.
-
     Attributes:
         classes_: Class labels known by the Committee.
         n_classes_: Number of classes known by the Committee.
-
     Examples:
-
         >>> from sklearn.datasets import load_iris
         >>> from sklearn.neighbors import KNeighborsClassifier
         >>> from sklearn.ensemble import RandomForestClassifier
         >>> from modAL.models import ActiveLearner, Committee
         >>>
         >>> iris = load_iris()
         >>>
@@ -320,114 +511,100 @@
         super()._add_training_data(X, y)
 
     def fit(self, X: modALinput, y: modALinput, **fit_kwargs) -> 'BaseCommittee':
         """
         Fits every learner to a subset sampled with replacement from X. Calling this method makes the learner forget the
         data it has seen up until this point and replaces it with X! If you would like to perform bootstrapping on each
         learner using the data it has seen, use the method .rebag()!
-
         Calling this method makes the learner forget the data it has seen up until this point and replaces it with X!
-
         Args:
             X: The samples to be fitted on.
             y: The corresponding labels.
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
         """
         super().fit(X, y, **fit_kwargs)
         self._set_classes()
 
     def teach(self, X: modALinput, y: modALinput, bootstrap: bool = False, only_new: bool = False, **fit_kwargs) -> None:
         """
         Adds X and y to the known training data for each learner and retrains learners with the augmented dataset.
-
         Args:
             X: The new samples for which the labels are supplied by the expert.
             y: Labels corresponding to the new instances in X.
             bootstrap: If True, trains each learner on a bootstrapped set. Useful when building the ensemble by bagging.
             only_new: If True, the model is retrained using only X and y, ignoring the previously provided examples.
             **fit_kwargs: Keyword arguments to be passed to the fit method of the predictor.
         """
         super().teach(X, y, bootstrap=bootstrap, only_new=only_new, **fit_kwargs)
         self._set_classes()
 
     def predict(self, X: modALinput, **predict_proba_kwargs) -> Any:
         """
         Predicts the class of the samples by picking the consensus prediction.
-
         Args:
             X: The samples to be predicted.
             **predict_proba_kwargs: Keyword arguments to be passed to the :meth:`predict_proba` of the Committee.
-
         Returns:
             The predicted class labels for X.
         """
         # getting average certainties
         proba = self.predict_proba(X, **predict_proba_kwargs)
         # finding the sample-wise max probability
         max_proba_idx = np.argmax(proba, axis=1)
         # translating label indices to labels
         return self.classes_[max_proba_idx]
 
     def predict_proba(self, X: modALinput, **predict_proba_kwargs) -> Any:
         """
         Consensus probabilities of the Committee.
-
         Args:
             X: The samples for which the class probabilities are to be predicted.
             **predict_proba_kwargs: Keyword arguments to be passed to the :meth:`predict_proba` of the Committee.
-
         Returns:
             Class probabilities for X.
         """
         return np.mean(self.vote_proba(X, **predict_proba_kwargs), axis=1)
 
     def score(self, X: modALinput, y: modALinput, sample_weight: List[float] = None) -> Any:
         """
         Returns the mean accuracy on the given test data and labels.
-
         Todo:
             Why accuracy?
-
         Args:
             X: The samples to score.
             y: Ground truth labels corresponding to X.
             sample_weight: Sample weights.
-
         Returns:
             Mean accuracy of the classifiers.
         """
         y_pred = self.predict(X)
         return accuracy_score(y, y_pred, sample_weight=sample_weight)
 
     def vote(self, X: modALinput, **predict_kwargs) -> Any:
         """
         Predicts the labels for the supplied data for each learner in the Committee.
-
         Args:
             X: The samples to cast votes.
             **predict_kwargs: Keyword arguments to be passed to the :meth:`predict` of the learners.
-
         Returns:
             The predicted class for each learner in the Committee and each sample in X.
         """
         prediction = np.zeros(shape=(X.shape[0], len(self.learner_list)))
 
         for learner_idx, learner in enumerate(self.learner_list):
             prediction[:, learner_idx] = learner.predict(X, **predict_kwargs)
 
         return prediction
 
     def vote_proba(self, X: modALinput, **predict_proba_kwargs) -> Any:
         """
         Predicts the probabilities of the classes for each sample and each learner.
-
         Args:
             X: The samples for which class probabilities are to be calculated.
             **predict_proba_kwargs: Keyword arguments for the :meth:`predict_proba` of the learners.
-
         Returns:
             Probabilities of each class for each learner and each instance.
         """
 
         # get dimensions
         n_samples = X.shape[0]
         n_learners = len(self.learner_list)
@@ -451,23 +628,20 @@
 
         return proba
 
 
 class CommitteeRegressor(BaseCommittee):
     """
     This class is an abstract model of a committee-based active learning regression.
-
     Args:
         learner_list: A list of ActiveLearners forming the CommitteeRegressor.
         query_strategy: Query strategy function.
         on_transformed: Whether to transform samples with the pipeline defined by each learner's estimator
             when applying the query strategy.
-
     Examples:
-
         >>> import numpy as np
         >>> import matplotlib.pyplot as plt
         >>> from sklearn.gaussian_process import GaussianProcessRegressor
         >>> from sklearn.gaussian_process.kernels import WhiteKernel, RBF
         >>> from modAL.models import ActiveLearner, CommitteeRegressor
         >>>
         >>> # generating the data
@@ -507,36 +681,32 @@
     def __init__(self, learner_list: List[ActiveLearner], query_strategy: Callable = max_std_sampling,
                  on_transformed: bool = False) -> None:
         super().__init__(learner_list, query_strategy, on_transformed)
 
     def predict(self, X: modALinput, return_std: bool = False, **predict_kwargs) -> Any:
         """
         Predicts the values of the samples by averaging the prediction of each regressor.
-
         Args:
             X: The samples to be predicted.
             **predict_kwargs: Keyword arguments to be passed to the :meth:`vote` method of the CommitteeRegressor.
-
         Returns:
             The predicted class labels for X.
         """
         vote = self.vote(X, **predict_kwargs)
         if not return_std:
             return np.mean(vote, axis=1)
         else:
             return np.mean(vote, axis=1), np.std(vote, axis=1)
 
     def vote(self, X: modALinput, **predict_kwargs):
         """
         Predicts the values for the supplied data for each regressor in the CommitteeRegressor.
-
         Args:
             X: The samples to cast votes.
             **predict_kwargs: Keyword arguments to be passed to :meth:`predict` of the learners.
-
         Returns:
             The predicted value for each regressor in the CommitteeRegressor and each sample in X.
         """
         prediction = np.zeros(shape=(len(X), len(self.learner_list)))
 
         for learner_idx, learner in enumerate(self.learner_list):
             prediction[:, learner_idx] = learner.predict(X, **predict_kwargs).reshape(-1, )
```

### Comparing `modAL-python-mirror-0.4.1/modAL/multilabel.py` & `modAL-python-mirror-0.4.2/modAL/multilabel.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-import numpy as np
+from typing import Optional
 
-from sklearn.base import BaseEstimator
+import numpy as np
 from sklearn.multiclass import OneVsRestClassifier
 
 from modAL.models import ActiveLearner
 from modAL.utils.data import modALinput
-from modAL.utils.selection import multi_argmax, shuffled_argmax
-from typing import Tuple, Optional
-from itertools import combinations
+from modAL.utils.selection import (multi_argmax, multi_argmin, shuffled_argmax,
+                                   shuffled_argmin)
 
 
 def _SVM_loss(multiclass_classifier: ActiveLearner,
               X: modALinput, most_certain_classes: Optional[int] = None) -> np.ndarray:
     """
     Utility function for max_loss and mean_max_loss strategies.
 
@@ -54,15 +53,16 @@
             such as the ones from sklearn.svm.
         X_pool: The pool of samples to query from.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
 
     Returns:
         The index of the instance from X_pool chosen to be labelled;
-        the instance from X_pool chosen to be labelled.
+        The instance from X_pool chosen to be labelled.
+        The Minimum absolute distance metric of the chosen instance; 
     """
 
     decision_function = np.array([svm.decision_function(X_pool)
                                   for svm in classifier.estimator.estimators_]).T
 
     min_abs_dist = np.min(np.abs(decision_function), axis=1)
 
@@ -88,15 +88,17 @@
             the mathematical calculations in Li et al. work only for SVM-s.
         X_pool: The pool of samples to query from.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
 
     Returns:
         The index of the instance from X_pool chosen to be labelled;
-        the instance from X_pool chosen to be labelled.
+        The instance from X_pool chosen to be labelled.
+        The SVM-loss-max metric of the chosen instances; 
+
     """
 
     assert len(X_pool) >= n_instances, 'n_instances cannot be larger than len(X_pool)'
 
     most_certain_classes = classifier.predict_proba(X_pool).argmax(axis=1)
     loss = _SVM_loss(classifier, X_pool, most_certain_classes=most_certain_classes)
 
@@ -120,16 +122,17 @@
             such as the ones from sklearn.svm. Although the function will execute for other models as well,
             the mathematical calculations in Li et al. work only for SVM-s.
         X_pool: The pool of samples to query from.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
 
     Returns:
-        The index of the instance from X_pool chosen to be labelled;
-        the instance from X_pool chosen to be labelled.
+        The index of the instance from X_pool chosen to be labelled.
+        The SVM-loss metric of the chosen instances. 
+
     """
 
     assert len(X_pool) >= n_instances, 'n_instances cannot be larger than len(X_pool)'
     loss = _SVM_loss(classifier, X_pool)
 
     if not random_tie_break:
         return multi_argmax(loss, n_instances)
@@ -149,25 +152,26 @@
     Args:
         classifier: The multilabel classifier for which the labels are to be queried.
         X_pool: The pool of samples to query from.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
 
     Returns:
-        The index of the instance from X_pool chosen to be labelled;
-        the instance from X_pool chosen to be labelled.
+        The index of the instance from X_pool chosen to be labelled.
+        The minimal confidence metric of the chosen instance. 
+
     """
 
     classwise_confidence = classifier.predict_proba(X_pool)
     classwise_min = np.min(classwise_confidence, axis=1)
 
     if not random_tie_break:
-        return multi_argmax(-classwise_min, n_instances)
+        return multi_argmin(classwise_min, n_instances)
 
-    return shuffled_argmax(-classwise_min, n_instances)
+    return shuffled_argmin(classwise_min, n_instances)
 
 
 def avg_confidence(classifier: OneVsRestClassifier, X_pool: modALinput,
                    n_instances: int = 1, random_tie_break: bool = False) -> np.ndarray:
     """
     AvgConfidence query strategy for multilabel classification.
 
@@ -178,16 +182,17 @@
     Args:
         classifier: The multilabel classifier for which the labels are to be queried.
         X_pool: The pool of samples to query from.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
 
     Returns:
-        The index of the instance from X_pool chosen to be labelled;
-        the instance from X_pool chosen to be labelled.
+        The index of the instance from X_pool chosen to be labelled.
+        The average confidence metric of the chosen instances. 
+
     """
 
     classwise_confidence = classifier.predict_proba(X_pool)
     classwise_mean = np.mean(classwise_confidence, axis=1)
 
     if not random_tie_break:
         return multi_argmax(classwise_mean, n_instances)
@@ -207,16 +212,17 @@
     Args:
         classifier: The multilabel classifier for which the labels are to be queried.
         X_pool: The pool of samples to query from.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
 
     Returns:
-        The index of the instance from X_pool chosen to be labelled;
-        the instance from X_pool chosen to be labelled.
+        The index of the instance from X_pool chosen to be labelled.
+        The classwise maximum metric of the chosen instances. 
+
     """
 
     classwise_confidence = classifier.predict_proba(X_pool)
     classwise_predictions = classifier.predict(X_pool)
     classwise_scores = classwise_confidence*(classwise_predictions - 1/2)
     classwise_max = np.max(classwise_scores, axis=1)
 
@@ -238,16 +244,17 @@
     Args:
         classifier: The multilabel classifier for which the labels are to be queried.
         X_pool: The pool of samples to query from.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
 
     Returns:
-        The index of the instance from X_pool chosen to be labelled;
-        the instance from X_pool chosen to be labelled.
+        The index of the instance from X_pool chosen to be labelled.
+        The classwise mean metric of the chosen instances.
+
     """
 
     classwise_confidence = classifier.predict_proba(X_pool)
     classwise_predictions = classifier.predict(X_pool)
     classwise_scores = classwise_confidence*(classwise_predictions-1/2)
     classwise_mean = np.mean(classwise_scores, axis=1)
```

### Comparing `modAL-python-mirror-0.4.1/modAL/uncertainty.py` & `modAL-python-mirror-0.4.2/modAL/uncertainty.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """
 Uncertainty measures and uncertainty based sampling strategies for the active learning models.
 """
-from typing import Tuple
 
 import numpy as np
 from scipy.stats import entropy
-from sklearn.exceptions import NotFittedError
 from sklearn.base import BaseEstimator
+from sklearn.exceptions import NotFittedError
 
 from modAL.utils.data import modALinput
-from modAL.utils.selection import multi_argmax, shuffled_argmax
+from modAL.utils.selection import (multi_argmax, multi_argmin, shuffled_argmax,
+                                   shuffled_argmin)
 
 
 def _proba_uncertainty(proba: np.ndarray) -> np.ndarray:
     """
     Calculates the uncertainty of the prediction probabilities.
 
     Args:
@@ -142,16 +142,16 @@
         n_instances: Number of samples to be queried.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
         **uncertainty_measure_kwargs: Keyword arguments to be passed for the uncertainty
             measure function.
 
     Returns:
-        The indices of the instances from X chosen to be labelled;
-        the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled.
+        The uncertainty metric of the chosen instances. 
     """
     uncertainty = classifier_uncertainty(classifier, X, **uncertainty_measure_kwargs)
 
     if not random_tie_break:
         return multi_argmax(uncertainty, n_instances=n_instances)
 
     return shuffled_argmax(uncertainty, n_instances=n_instances)
@@ -168,23 +168,23 @@
         X: The pool of samples to query from.
         n_instances: Number of samples to be queried.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
         **uncertainty_measure_kwargs: Keyword arguments to be passed for the uncertainty
             measure function.
     Returns:
-        The indices of the instances from X chosen to be labelled;
-        the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled.
+        The margin metric of the chosen instances.
     """
     margin = classifier_margin(classifier, X, **uncertainty_measure_kwargs)
 
     if not random_tie_break:
-        return multi_argmax(-margin, n_instances=n_instances)
+        return multi_argmin(margin, n_instances=n_instances)
 
-    return shuffled_argmax(-margin, n_instances=n_instances)
+    return shuffled_argmin(margin, n_instances=n_instances)
 
 
 def entropy_sampling(classifier: BaseEstimator, X: modALinput,
                      n_instances: int = 1, random_tie_break: bool = False,
                      **uncertainty_measure_kwargs) -> np.ndarray:
     """
     Entropy sampling query strategy. Selects the instances where the class probabilities
@@ -196,16 +196,16 @@
         n_instances: Number of samples to be queried.
         random_tie_break: If True, shuffles utility scores to randomize the order. This
             can be used to break the tie when the highest utility score is not unique.
         **uncertainty_measure_kwargs: Keyword arguments to be passed for the uncertainty
             measure function.
 
     Returns:
-        The indices of the instances from X chosen to be labelled;
-        the instances from X chosen to be labelled.
+        The indices of the instances from X chosen to be labelled.
+        The entropy metric of the chosen instances.
     """
     entropy = classifier_entropy(classifier, X, **uncertainty_measure_kwargs)
 
     if not random_tie_break:
         return multi_argmax(entropy, n_instances=n_instances)
 
     return shuffled_argmax(entropy, n_instances=n_instances)
```

### Comparing `modAL-python-mirror-0.4.1/modAL/utils/combination.py` & `modAL-python-mirror-0.4.2/modAL/utils/combination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Callable, Optional, Sequence, Tuple
 
 import numpy as np
-from sklearn.base import BaseEstimator
-
 from modAL.utils.data import modALinput
+from sklearn.base import BaseEstimator
 
 
 def make_linear_combination(*functions: Callable, weights: Optional[Sequence] = None) -> Callable:
     """
     Takes the given functions and makes a function which returns the linear combination of the output of original
     functions. It works well with functions returning numpy arrays of the same shape.
```

### Comparing `modAL-python-mirror-0.4.1/modAL/utils/selection.py` & `modAL-python-mirror-0.4.2/modAL/utils/selection.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,49 +9,82 @@
     """
     Shuffles the values and sorts them afterwards. This can be used to break
     the tie when the highest utility score is not unique. The shuffle randomizes
     order, which is preserved by the mergesort algorithm.
 
     Args:
         values: Contains the values to be selected from.
-        n_instances: Specifies how many indices to return.
-
+        n_instances: Specifies how many indices and values to return.
     Returns:
-        The indices of the n_instances largest values.
+        The indices and values of the n_instances largest values.
     """
     assert n_instances <= values.shape[0], 'n_instances must be less or equal than the size of utility'
 
     # shuffling indices and corresponding values
     shuffled_idx = np.random.permutation(len(values))
     shuffled_values = values[shuffled_idx]
 
     # getting the n_instances best instance
     # since mergesort is used, the shuffled order is preserved
-    sorted_query_idx = np.argsort(shuffled_values, kind='mergesort')[len(shuffled_values)-n_instances:]
+    sorted_query_idx = np.argsort(shuffled_values, kind='mergesort')[
+        len(shuffled_values)-n_instances:]
 
     # inverting the shuffle
     query_idx = shuffled_idx[sorted_query_idx]
-    return query_idx
 
+    return query_idx, values[query_idx]
 
-def multi_argmax(values: np.ndarray, n_instances: int = 1) -> np.ndarray:
+
+def shuffled_argmin(values: np.ndarray, n_instances: int = 1) -> np.ndarray:
     """
-    Selects the indices of the n_instances highest values.
+    Shuffles the values and sorts them afterwards. This can be used to break
+    the tie when the highest utility score is not unique. The shuffle randomizes
+    order, which is preserved by the mergesort algorithm.
 
     Args:
         values: Contains the values to be selected from.
-        n_instances: Specifies how many indices to return.
+        n_instances: Specifies how many indices and values to return.
+    Returns:
+        The indices and values of the n_instances smallest values.
+    """
+
+    indexes, index_values = shuffled_argmax(-values, n_instances)
 
+    return indexes, -index_values
+
+
+def multi_argmax(values: np.ndarray, n_instances: int = 1) -> np.ndarray:
+    """
+    return the indices and values of the n_instances highest values.
+
+    Args:
+        values: Contains the values to be selected from.
+        n_instances: Specifies how many indices and values to return.
     Returns:
-        The indices of the n_instances largest values.
+        The indices and values of the n_instances largest values.
     """
     assert n_instances <= values.shape[0], 'n_instances must be less or equal than the size of utility'
 
     max_idx = np.argpartition(-values, n_instances-1, axis=0)[:n_instances]
-    return max_idx
+
+    return max_idx, values[max_idx]
+
+
+def multi_argmin(values: np.ndarray, n_instances: int = 1) -> np.ndarray:
+    """
+    return the indices and values of the n_instances smallest values.
+
+    Args:
+        values: Contains the values to be selected from.
+        n_instances: Specifies how many indices and values to return.
+    Returns:
+        The indices and values of the n_instances smallest values.
+    """
+    indexes, index_values = multi_argmax(-values, n_instances)
+    return indexes, -index_values
 
 
 def weighted_random(weights: np.ndarray, n_instances: int = 1) -> np.ndarray:
     """
     Returns n_instances indices based on the weights.
 
     Args:
@@ -61,9 +94,10 @@
     Returns:
         n_instances random indices based on the weights.
     """
     assert n_instances <= weights.shape[0], 'n_instances must be less or equal than the size of utility'
     weight_sum = np.sum(weights)
     assert weight_sum > 0, 'the sum of weights must be larger than zero'
 
-    random_idx = np.random.choice(range(len(weights)), size=n_instances, p=weights/weight_sum, replace=False)
+    random_idx = np.random.choice(
+        range(len(weights)), size=n_instances, p=weights/weight_sum, replace=False)
     return random_idx
```

### Comparing `modAL-python-mirror-0.4.1/modAL/utils/validation.py` & `modAL-python-mirror-0.4.2/modAL/utils/validation.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Sequence
 
 import numpy as np
-from sklearn.exceptions import NotFittedError
 from sklearn.base import BaseEstimator
+from sklearn.exceptions import NotFittedError
 
 
 def check_class_labels(*args: BaseEstimator) -> bool:
     """
     Checks the known class labels for each classifier.
 
     Args:
```

### Comparing `modAL-python-mirror-0.4.1/modAL_python_mirror.egg-info/SOURCES.txt` & `modAL-python-mirror-0.4.2/modAL_python_mirror.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 setup.py
 modAL/__init__.py
 modAL/acquisition.py
 modAL/batch.py
 modAL/cluster.py
 modAL/density.py
 modAL/disagreement.py
+modAL/dropout.py
 modAL/expected_error.py
 modAL/multilabel.py
 modAL/uncertainty.py
 modAL/models/__init__.py
 modAL/models/base.py
 modAL/models/learners.py
 modAL/utils/__init__.py
```

### Comparing `modAL-python-mirror-0.4.1/setup.py` & `modAL-python-mirror-0.4.2/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 setup(
     name='modAL-python-mirror',
-    version='0.4.1',
+    version='0.4.2',
     author='Tivadar Danka',
     author_email='85a5187a@opayq.com',
     description='A modular active learning framework for Python3 (mirror package)',
     license='MIT',
     url='https://modAL-python.github.io/',
     packages=['modAL', 'modAL.models', 'modAL.utils'],
     classifiers=['Development Status :: 4 - Beta'],
-    install_requires=['numpy>=1.13', 'scikit-learn>=0.18', 'scipy>=0.18', 'pandas>=1.1.0'],
+    install_requires=['numpy', 'scikit-learn>=0.18',
+                      'scipy>=0.18', 'pandas>=1.1.0', 'skorch==0.9.0'],
 )
```

