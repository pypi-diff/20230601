# Comparing `tmp/landmarkclassifier-2.0.4.tar.gz` & `tmp/landmarkclassifier-2.0.5.tar.gz`

## Comparing `landmarkclassifier-2.0.4.tar` & `landmarkclassifier-2.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/environment.yml
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/LANDMark/LANDMark.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/LANDMark/__init__.py
--rw-r--r--   0        0        0    13472 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/LANDMark/lm_base_clfs.py
--rw-r--r--   0        0        0    24062 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/LANDMark/tree.py
--rw-r--r--   0        0        0     5628 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/LANDMark/utils.py
--rw-r--r--   0        0        0     5664 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/docs/API.md
--rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/tests/__init__.py
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/tests/test_landmark.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/.gitignore
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/LICENSE
--rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/README.md
--rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/environment.yml
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LANDMark/LANDMark.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LANDMark/__init__.py
+-rw-r--r--   0        0        0    13597 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LANDMark/lm_base_clfs.py
+-rw-r--r--   0        0        0    22126 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LANDMark/tree.py
+-rw-r--r--   0        0        0     5543 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LANDMark/utils.py
+-rw-r--r--   0        0        0     5627 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/docs/API.md
+-rw-r--r--   0        0        0     4468 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/tests/__init__.py
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/tests/test_landmark.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/.gitignore
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/LICENSE
+-rw-r--r--   0        0        0     2490 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/README.md
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5437 2020-02-02 00:00:00.000000 landmarkclassifier-2.0.5/PKG-INFO
```

### Comparing `landmarkclassifier-2.0.4/.github/ISSUE_TEMPLATE/bug_report.md` & `landmarkclassifier-2.0.5/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.4/.github/ISSUE_TEMPLATE/feature_request.md` & `landmarkclassifier-2.0.5/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.4/.github/workflows/ci.yml` & `landmarkclassifier-2.0.5/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.4/.github/workflows/python-publish.yml` & `landmarkclassifier-2.0.5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.4/LANDMark/lm_base_clfs.py` & `landmarkclassifier-2.0.5/LANDMark/lm_base_clfs.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 from gc import collect
 
 
 class RandomOracle(ClassifierMixin, BaseEstimator):
     def __init__(self, oracle="Linear", n_feat=0.8):
         self.oracle = "Linear"
         self.n_feat = n_feat
-        
+
     def fit(self, X, y):
         if X.shape[1] >= 4:
             self.features = np.random.choice(
                 [i for i in range(X.shape[1])],
                 size=ceil(X.shape[1] * self.n_feat),
                 replace=False,
             )
@@ -123,16 +123,14 @@
 
         X_re, y_re = resample(X, y, n_samples=X.shape[0], stratify=y)
 
         X_re = X_re[:, self.features]
 
         self.classes_, y_counts = np.unique(y_re, return_counts=True)
 
-        y_min = min(y_counts)
-
         clf_1 = ExtraTreesClassifier(
             n_estimators=self.max_trees, max_depth=self.max_depth
         )
 
         self.model_type = "nonlinear_etc"
 
         self.clf_model = clf_1.fit(X_re, y_re)
@@ -141,21 +139,21 @@
 
     def predict(self, X):
         return self.clf_model.predict(X[:, self.features])
 
     def decision_function(self, X):
         return self.clf_model.predict_proba(X[:, self.features])
 
+
 class LMClassifier(ClassifierMixin, BaseEstimator):
-    def __init__(self, model_type, n_feat = 0.8):
+    def __init__(self, model_type, n_feat=0.8):
         self.model_type = model_type
         self.n_feat = n_feat
 
     def fit(self, X, y):
-
         if X.shape[1] >= 4:
             self.features = np.random.choice(
                 [i for i in range(X.shape[1])],
                 size=ceil(X.shape[1] * self.n_feat),
                 replace=False,
             )
 
@@ -175,15 +173,17 @@
                 self.clf = LogisticRegressionCV(max_iter=2000, cv=5).fit(X_re, y_re)
 
             elif self.model_type == "lr_l1":
                 solver = "liblinear"
                 if X.shape[0] >= 500:
                     solver = "saga"
 
-                self.clf = LogisticRegressionCV(max_iter=2000, cv=5, solver=solver, penalty="l1").fit(X_re, y_re)
+                self.clf = LogisticRegressionCV(
+                    max_iter=2000, cv=5, solver=solver, penalty="l1"
+                ).fit(X_re, y_re)
 
             elif self.model_type == "sgd_l2":
                 self.cv = GridSearchCV(
                     SGDClassifier(max_iter=2000),
                     param_grid={
                         "alpha": [0.001, 0.01, 0.1, 1.0, 10, 100],
                         "loss": ["hinge", "modified_huber"],
@@ -202,15 +202,17 @@
                     },
                     cv=5,
                 ).fit(X_re, y_re)
 
                 self.clf = self.cv.best_estimator_
 
             elif self.model_type == "ridge":
-                self.clf = RidgeClassifierCV(alphas=(0.001, 0.01, 0.1, 1.0, 10, 100, 1000)).fit(X_re, y_re)
+                self.clf = RidgeClassifierCV(
+                    alphas=(0.001, 0.01, 0.1, 1.0, 10, 100, 1000), cv=5
+                ).fit(X_re, y_re)
 
             elif self.model_type == "lsvc":
                 self.cv = GridSearchCV(
                     LinearSVC(max_iter=2000),
                     param_grid={"C": [0.001, 0.01, 0.1, 1.0, 10, 100]},
                     cv=5,
                 ).fit(X_re, y_re)
@@ -222,15 +224,17 @@
                 self.clf = LogisticRegression(max_iter=2000).fit(X_re, y_re)
 
             elif self.model_type == "lr_l1":
                 solver = "liblinear"
                 if X.shape[0] >= 500:
                     solver = "saga"
 
-                self.clf = LogisticRegression(max_iter=2000, solver=solver, penalty="l1").fit(X_re, y_re)
+                self.clf = LogisticRegression(
+                    max_iter=2000, solver=solver, penalty="l1"
+                ).fit(X_re, y_re)
 
             elif self.model_type == "sgd_l2":
                 self.clf = choice(
                     [
                         SGDClassifier(alpha=1.0, loss="hinge", max_iter=2000),
                         SGDClassifier(alpha=1.0, loss="modified_huber", max_iter=2000),
                     ]
@@ -252,15 +256,17 @@
                         ),
                     ]
                 )
 
                 self.clf.fit(X_re, y_re)
 
             elif self.model_type == "ridge":
-                self.clf = RidgeClassifierCV(alphas=(0.001, 0.01, 0.1, 1.0, 10, 100, 1000)).fit(X_re, y_re)
+                self.clf = RidgeClassifierCV(
+                    alphas=(0.001, 0.01, 0.1, 1.0, 10, 100, 1000)
+                ).fit(X_re, y_re)
 
             elif self.model_type == "lsvc":
                 self.clf = LinearSVC(max_iter=2000).fit(X_re, y_re)
 
         return self, self.decision_function(X)
 
     def predict(self, X):
@@ -405,8 +411,8 @@
 
         predictions = np.argmax(predictions, axis=1)
 
         predictions = np.asarray([self.classes_[entry] for entry in predictions])
 
         tf.keras.backend.clear_session()
 
-        return predictions
+        return predictions
```

### Comparing `landmarkclassifier-2.0.4/LANDMark/tree.py` & `landmarkclassifier-2.0.5/LANDMark/tree.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,27 +2,25 @@
 
 from scipy.stats import entropy
 
 from random import choice
 
 from sklearn.base import ClassifierMixin, BaseEstimator, clone
 from sklearn.metrics import balanced_accuracy_score
-from sklearn.utils import resample
 
 from .lm_base_clfs import (
     LMClassifier,
     RandomOracle,
     ANNClassifier,
     ETClassifier,
 )
 
 
 def tsallis_fun(N, N_lab, L, R, y, mode, q):
-
-    if q == 1: #Special case
+    if q == 1:  # Special case
         if "ratio" in mode.split("-"):
             return entropy_fun(N, N_lab, L, R, y, "gain-ratio")
 
         else:
             return entropy_fun(N, N_lab, L, R, y, "gain")
 
     scaler = 1 / (1 - q)
@@ -36,21 +34,20 @@
     H_R = (R_counts.sum() / N) * (scaler * (np.power(R_prob, q).sum() - 1))
 
     H_parent = scaler * (np.power(N_lab, q).sum() - 1)
 
     IG = H_parent - H_R - H_L
 
     if mode == "tsallis":
-
         return IG
 
     else:
         norm_factor = np.asarray([(L_counts.sum() / N), (R_counts.sum() / N)])
         norm_factor = 1 + (scaler * (np.power(norm_factor, q).sum() - 1))
-    
+
         GR = IG / norm_factor
 
         return GR
 
 
 def entropy_fun(N, N_lab, L, R, y, mode):
     L_outcome, L_counts = np.unique(y[L], return_counts=True)
@@ -62,51 +59,45 @@
     H_R = entropy(R_prob) * (R_counts.sum() / N)
 
     H_parent = entropy(N_lab)
 
     IG = H_parent - H_L - H_R
 
     if mode == "gain":
-
         return IG
 
     else:
         norm_factor = np.asarray([(L_counts.sum() / N), (R_counts.sum() / N)])
         norm_factor = 1 + entropy(norm_factor)
-    
+
         GR = IG / norm_factor
 
         return GR
 
 
 def purity_function(N, N_lab, L, R, y, purity_fun, q):
-    
     if purity_fun == "gain" or purity_fun == "gain-ratio":
-
         return entropy_fun(N, N_lab, L, R, y, purity_fun)
 
     elif purity_fun == "tsallis-gain-ratio" or purity_fun == "tsallis":
-
         return tsallis_fun(N, N_lab, L, R, y, purity_fun, q)
 
 
 class PredictData:
     def __init__(self, node_lab):
         self.node_lab = node_lab
 
     def predict(self, X):
         predictions = np.asarray([self.node_lab for i in range(X.shape[0])])
 
         return predictions
 
 
 class Node:
-
     def __init__(self):
-
         # Node parameters
         self.c_choice = None
 
         self.left = None
         self.right = None
 
         self.splitter = None
@@ -115,63 +106,83 @@
         self.split_type = None
 
         self.terminal = False
         self.label = None
         self.node_id = None
 
     # Select the best split point for a dataset
-    def get_split(self, 
-                  X,
-                  y,
-                  min_samples_in_leaf,
-                  max_depth,
-                  max_features,
-                  min_gain,
-                  impurity,
-                  q,
-                  use_lm_l2,
-                  use_lm_l1,
-                  use_nnet,
-                  nnet_min_samples,
-                  use_etc,
-                  etc_max_depth,
-                  etc_max_trees,
-                  N,
-                  current_depth,
-                  use_oracle):
-
+    def get_split(
+        self,
+        X,
+        y,
+        min_samples_in_leaf,
+        max_depth,
+        max_features,
+        min_gain,
+        impurity,
+        q,
+        use_lm_l2,
+        use_lm_l1,
+        use_nnet,
+        nnet_min_samples,
+        use_etc,
+        etc_max_depth,
+        etc_max_trees,
+        N,
+        current_depth,
+        use_oracle,
+    ):
         # Get the ID of the node
         self.node_id = id(self)
 
         # Prepare the list of hyperplanes, gains, and model types
         hyperplane_list = []
         gains = []
         model_type = []
 
         # Determine the counts of each class at this node
         outcomes, counts_tr = np.unique(y, return_counts=True)
         counts_sum = counts_tr.sum()
         counts_prob = counts_tr / counts_sum
         counts_min = np.min(counts_tr)
-        counts_min_prob = counts_min / counts_sum
 
-        # If the node is pure, the maximim depth is reached, or the number of samples is too small, create a leaf
-        if (
-            entropy(counts_prob) == 0
-            or counts_sum < min_samples_in_leaf
-            or (current_depth >= max_depth and max_depth > -1)
-            or counts_min <= 1
-        ):
+        # Check if stopping criteria are met
+        if entropy(counts_prob) == 0:
+            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
+
+            self.label = leaf_predictions.predict
+            self.terminal = True
+
+            return self
+
+        if counts_sum < min_samples_in_leaf:
             leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
 
             self.label = leaf_predictions.predict
             self.terminal = True
 
             return self
 
+        if counts_min <= 1:
+            leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
+
+            self.label = leaf_predictions.predict
+            self.terminal = True
+
+            return self
+
+        if isinstance(max_depth, int):
+            if current_depth >= max_depth:
+                leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
+
+                self.label = leaf_predictions.predict
+                self.terminal = True
+
+                return self
+
         # Otherwise split
         else:
             # Create a Random Oracle Splitter
             if use_oracle:
                 self.splitter = RandomOracle(n_feat=max_features).fit(X, y)
 
                 D = self.splitter.decision_function(X)
@@ -180,65 +191,69 @@
                 R = np.where(D <= 0, True, False)
 
                 IG = purity_function(counts_sum, counts_prob, L, R, y, impurity, q)
 
                 self.gain = IG
 
                 # Recursivly split
-                self.left = Node().get_split(X[L], 
-                                                 y[L],
-                                                 min_samples_in_leaf = min_samples_in_leaf,
-                                                 max_depth = max_depth,
-                                                 max_features = max_features,
-                                                 min_gain = min_gain,
-                                                 impurity = impurity,
-                                                 q = q,
-                                                 use_lm_l2 = use_lm_l2,
-                                                 use_lm_l1 = use_lm_l1,
-                                                 use_nnet = use_nnet,
-                                                 nnet_min_samples = nnet_min_samples,
-                                                 use_etc = use_etc,
-                                                 etc_max_depth = etc_max_depth,
-                                                 etc_max_trees = etc_max_trees,
-                                                 N=X.shape[0],
-                                                 current_depth=current_depth + 1,
-                                                 use_oracle=False)
-
-                self.right = Node().get_split(X[R], 
-                                                  y[R],
-                                                  min_samples_in_leaf = min_samples_in_leaf,
-                                                  max_depth = max_depth,
-                                                  max_features = max_features,
-                                                  min_gain = min_gain,
-                                                  impurity = impurity,
-                                                  q = q,
-                                                  use_lm_l2 = use_lm_l2,
-                                                  use_lm_l1 = use_lm_l1,
-                                                  use_nnet = use_nnet,
-                                                  nnet_min_samples = nnet_min_samples,
-                                                  use_etc = use_etc,
-                                                  etc_max_depth = etc_max_depth,
-                                                  etc_max_trees = etc_max_trees,
-                                                  N=X.shape[0],
-                                                  current_depth=current_depth + 1,
-                                                  use_oracle=False)
+                self.left = Node().get_split(
+                    X[L],
+                    y[L],
+                    min_samples_in_leaf=min_samples_in_leaf,
+                    max_depth=max_depth,
+                    max_features=max_features,
+                    min_gain=min_gain,
+                    impurity=impurity,
+                    q=q,
+                    use_lm_l2=use_lm_l2,
+                    use_lm_l1=use_lm_l1,
+                    use_nnet=use_nnet,
+                    nnet_min_samples=nnet_min_samples,
+                    use_etc=use_etc,
+                    etc_max_depth=etc_max_depth,
+                    etc_max_trees=etc_max_trees,
+                    N=X.shape[0],
+                    current_depth=current_depth + 1,
+                    use_oracle=False,
+                )
+
+                self.right = Node().get_split(
+                    X[R],
+                    y[R],
+                    min_samples_in_leaf=min_samples_in_leaf,
+                    max_depth=max_depth,
+                    max_features=max_features,
+                    min_gain=min_gain,
+                    impurity=impurity,
+                    q=q,
+                    use_lm_l2=use_lm_l2,
+                    use_lm_l1=use_lm_l1,
+                    use_nnet=use_nnet,
+                    nnet_min_samples=nnet_min_samples,
+                    use_etc=use_etc,
+                    etc_max_depth=etc_max_depth,
+                    etc_max_trees=etc_max_trees,
+                    N=X.shape[0],
+                    current_depth=current_depth + 1,
+                    use_oracle=False,
+                )
 
                 return self
 
             # Split using a Linear or Neural Network Models
             else:
                 self.c_choice = choice([i for i in range(outcomes.shape[0])])
 
                 # Train Linear Models - L2
-                if use_lm_l2 == True:
+                if use_lm_l2:
                     for clf in [
-                        LMClassifier(model_type = "lr_l2", n_feat=max_features),
-                        LMClassifier(model_type = "sgd_l2", n_feat=max_features),
-                        LMClassifier(model_type = "ridge", n_feat=max_features),
-                        LMClassifier(model_type = "lsvc", n_feat=max_features),
+                        LMClassifier(model_type="lr_l2", n_feat=max_features),
+                        LMClassifier(model_type="sgd_l2", n_feat=max_features),
+                        LMClassifier(model_type="ridge", n_feat=max_features),
+                        LMClassifier(model_type="lsvc", n_feat=max_features),
                     ]:
                         model, D = clf.fit(X, y)
 
                         if D.ndim > 1:
                             D = D[:, self.c_choice]
 
                         L = np.where(D > 0, True, False)
@@ -254,18 +269,18 @@
                             )
 
                             gains.append(IG)
                             hyperplane_list.append((model, L, R))
                             model_type.append(model.model_type)
 
                 # Train Linear Models - L1 / ElasticNet
-                if use_lm_l1 == True:
+                if use_lm_l1:
                     for clf in [
-                        LMClassifier(model_type = "lr_l1", n_feat=max_features),
-                        LMClassifier(model_type = "sgd_l1", n_feat=max_features),
+                        LMClassifier(model_type="lr_l1", n_feat=max_features),
+                        LMClassifier(model_type="sgd_l1", n_feat=max_features),
                     ]:
                         model, D = clf.fit(X, y)
 
                         if D.ndim > 1:
                             D = D[:, self.c_choice]
 
                         L = np.where(D > 0, True, False)
@@ -281,15 +296,15 @@
                             )
 
                             gains.append(IG)
                             hyperplane_list.append((model, L, R))
                             model_type.append(model.model_type)
 
                 # Train a Neural Network
-                if use_nnet == True:
+                if use_nnet:
                     if X.shape[0] >= nnet_min_samples:
                         for clf in [ANNClassifier(n_feat=max_features)]:
                             model, D = clf.fit(X, y)
 
                             if D.ndim > 1:
                                 D = D[:, self.c_choice]
 
@@ -306,15 +321,15 @@
                                 )
 
                                 gains.append(IG)
                                 hyperplane_list.append((model, L, R))
                                 model_type.append(model.model_type)
 
                 # Train Decision Tree Models
-                if use_etc == True:
+                if use_etc:
                     for clf in [
                         ETClassifier(
                             n_feat=max_features,
                             max_depth=etc_max_depth,
                             max_trees=etc_max_trees,
                         )
                     ]:
@@ -359,51 +374,55 @@
                     L = best_hyperplane[1]
                     R = best_hyperplane[2]
 
                     self.gain = best_gain
                     self.splitter = best_hyperplane[0]
 
                     # Recursivly split
-                    self.left = Node().get_split(X[L], 
-                                                 y[L],
-                                                 min_samples_in_leaf = min_samples_in_leaf,
-                                                 max_depth = max_depth,
-                                                 max_features = max_features,
-                                                 min_gain = min_gain,
-                                                 impurity = impurity,
-                                                 q = q,
-                                                 use_lm_l2 = use_lm_l2,
-                                                 use_lm_l1 = use_lm_l1,
-                                                 use_nnet = use_nnet,
-                                                 nnet_min_samples = nnet_min_samples,
-                                                 use_etc = use_etc,
-                                                 etc_max_depth = etc_max_depth,
-                                                 etc_max_trees = etc_max_trees,
-                                                 N=X.shape[0],
-                                                 current_depth=current_depth + 1,
-                                                 use_oracle=use_oracle)
-
-                    self.right = Node().get_split(X[R], 
-                                                  y[R],
-                                                  min_samples_in_leaf = min_samples_in_leaf,
-                                                  max_depth = max_depth,
-                                                  max_features = max_features,
-                                                  min_gain = min_gain,
-                                                  impurity = impurity,
-                                                  q = q,
-                                                  use_lm_l2 = use_lm_l2,
-                                                  use_lm_l1 = use_lm_l1,
-                                                  use_nnet = use_nnet,
-                                                  nnet_min_samples = nnet_min_samples,
-                                                  use_etc = use_etc,
-                                                  etc_max_depth = etc_max_depth,
-                                                  etc_max_trees = etc_max_trees,
-                                                  N=X.shape[0],
-                                                  current_depth=current_depth + 1,
-                                                  use_oracle=use_oracle)
+                    self.left = Node().get_split(
+                        X[L],
+                        y[L],
+                        min_samples_in_leaf=min_samples_in_leaf,
+                        max_depth=max_depth,
+                        max_features=max_features,
+                        min_gain=min_gain,
+                        impurity=impurity,
+                        q=q,
+                        use_lm_l2=use_lm_l2,
+                        use_lm_l1=use_lm_l1,
+                        use_nnet=use_nnet,
+                        nnet_min_samples=nnet_min_samples,
+                        use_etc=use_etc,
+                        etc_max_depth=etc_max_depth,
+                        etc_max_trees=etc_max_trees,
+                        N=X.shape[0],
+                        current_depth=current_depth + 1,
+                        use_oracle=use_oracle,
+                    )
+
+                    self.right = Node().get_split(
+                        X[R],
+                        y[R],
+                        min_samples_in_leaf=min_samples_in_leaf,
+                        max_depth=max_depth,
+                        max_features=max_features,
+                        min_gain=min_gain,
+                        impurity=impurity,
+                        q=q,
+                        use_lm_l2=use_lm_l2,
+                        use_lm_l1=use_lm_l1,
+                        use_nnet=use_nnet,
+                        nnet_min_samples=nnet_min_samples,
+                        use_etc=use_etc,
+                        etc_max_depth=etc_max_depth,
+                        etc_max_trees=etc_max_trees,
+                        N=X.shape[0],
+                        current_depth=current_depth + 1,
+                        use_oracle=use_oracle,
+                    )
 
                     return self
 
                 # Create a Leaf
                 else:
                     leaf_predictions = PredictData(outcomes[np.argmax(counts_prob)])
 
@@ -426,15 +445,15 @@
         use_lm_l2,
         use_lm_l1,
         use_nnet,
         nnet_min_samples,
         use_etc,
         etc_max_depth,
         etc_max_trees,
-        resampler
+        resampler,
     ):
         self.min_samples_in_leaf = min_samples_in_leaf
         self.max_depth = max_depth
         self.max_features = max_features
         self.min_gain = min_gain
         self.impurity = impurity
         self.q = q
@@ -461,70 +480,72 @@
 
             X_re, y_re = self.resampler.fit_resample(X, y)
 
         # Create the root node
         tree = Node()
 
         # Begin Splitting
-        tree.get_split(X=X_re, 
-                       y=y_re,
-                       min_samples_in_leaf = self.min_samples_in_leaf,
-                       max_depth = self.max_depth,
-                       max_features = self.max_features,
-                       min_gain = self.min_gain,
-                       impurity = self.impurity,
-                       q = self.q,
-                       use_lm_l2 = self.use_lm_l2,
-                       use_lm_l1 = self.use_lm_l1,
-                       use_nnet = self.use_nnet,
-                       nnet_min_samples = self.nnet_min_samples,
-                       use_etc = self.use_etc,
-                       etc_max_depth = self.etc_max_depth,
-                       etc_max_trees = self.etc_max_trees,
-                       N=X.shape[0],
-                       current_depth=1,
-                       use_oracle=self.use_oracle)
+        tree.get_split(
+            X=X_re,
+            y=y_re,
+            min_samples_in_leaf=self.min_samples_in_leaf,
+            max_depth=self.max_depth,
+            max_features=self.max_features,
+            min_gain=self.min_gain,
+            impurity=self.impurity,
+            q=self.q,
+            use_lm_l2=self.use_lm_l2,
+            use_lm_l1=self.use_lm_l1,
+            use_nnet=self.use_nnet,
+            nnet_min_samples=self.nnet_min_samples,
+            use_etc=self.use_etc,
+            etc_max_depth=self.etc_max_depth,
+            etc_max_trees=self.etc_max_trees,
+            N=X.shape[0],
+            current_depth=1,
+            use_oracle=self.use_oracle,
+        )
 
         self.LMTree = tree
 
         # Find all Node Ids
         self.all_ids = list(set(self._get_node_ids(self.LMTree)))
 
         return self
 
     def _get_node_ids(self, node):
         ids = []
 
-        if node.terminal == False:
+        if node.terminal is False:
             ids.extend(self._get_node_ids(node.left))
             ids.extend(self._get_node_ids(node.right))
 
         else:
             ids.append(node.node_id)
 
         return ids
 
     def _predict(self, X, current_node=None, root=True, sample_index=None):
         final_predictions = []
 
         true_index = None
-        if root == True:
+        if root:
             true_index = np.asarray([i for i in range(X.shape[0])])
 
         else:
             true_index = sample_index
 
         node = None
         if not (current_node):
             node = self.LMTree
 
         else:
             node = current_node
 
-        if node.terminal == False:
+        if node.terminal is False:
             if type(node.splitter) == ANNClassifier:
                 D = node.splitter.predict_proba(X)
 
                 if D.ndim > 1:
                     D = D[:, node.c_choice]
 
                 L = np.where(D > 0.5, True, False)
@@ -549,15 +570,15 @@
                 predictions_left = self._predict(X_L, node.left, False, left)
                 final_predictions.extend(predictions_left)
 
             if right.shape[0] > 0:
                 predictions_right = self._predict(X_R, node.right, False, right)
                 final_predictions.extend(predictions_right)
 
-        elif node.terminal == True:
+        elif node.terminal:
             predictions = node.label(X)
             predictions = np.asarray(
                 [
                     (true_index[i], prediction)
                     for i, prediction in enumerate(predictions)
                 ]
             )
@@ -565,19 +586,17 @@
             return predictions
 
         return final_predictions
 
     def predict(self, X):
         if hasattr(self.resampler, "transform"):
             X_trf = self.resampler.transform(X)
-        
+
         else:
             X_trf = X
-        
-        mapping = {class_name: i for i, class_name in enumerate(self.classes_)}
 
         tree_predictions = self._predict(X_trf)
 
         tree_predictions = [(int(entry[0]), entry[1]) for entry in tree_predictions]
         tree_predictions.sort()
 
         return np.asarray(tree_predictions)[:, 1]
@@ -587,28 +606,28 @@
 
         return score
 
     def _proximity(self, X, current_node=None, root=True, sample_index=None):
         final_predictions = []
 
         true_index = None
-        if root == True:
+        if root:
             true_index = np.asarray([i for i in range(X.shape[0])])
 
         else:
             true_index = sample_index
 
         node = None
         if not (current_node):
             node = self.LMTree
 
         else:
             node = current_node
 
-        if node.terminal == False:
+        if node.terminal is False:
             if type(node.splitter) == ANNClassifier:
                 D = node.splitter.predict_proba(X)
 
                 if D.ndim > 1:
                     D = D[:, node.c_choice]
 
                 L = np.where(D > 0.5, True, False)
@@ -633,33 +652,33 @@
                 predictions_left = self._proximity(X_L, node.left, False, left)
                 final_predictions.extend(predictions_left)
 
             if right.shape[0] > 0:
                 predictions_right = self._proximity(X_R, node.right, False, right)
                 final_predictions.extend(predictions_right)
 
-        elif node.terminal == True:
+        elif node.terminal:
             return [(entry, node.node_id) for entry in true_index]
 
         return final_predictions
 
     def proximity(self, X):
         if hasattr(self.resampler, "transform"):
             X_trf = self.resampler.transform(X)
-        
+
         else:
             X_trf = X
-        
+
         tree_predictions = self._proximity(X_trf)
 
         tree_predictions.sort()
 
         col_dict = {col: i for i, col in enumerate(self.all_ids)}
 
-        emb_matrix = np.zeros(shape=(X.shape[0], len(self.all_ids)), dtype=np.int)
+        emb_matrix = np.zeros(shape=(X.shape[0], len(self.all_ids)), dtype=np.ushort)
 
         for entry in tree_predictions:
             row = entry[0]
             col = col_dict[entry[1]]
 
             emb_matrix[row, col] = 1
```

### Comparing `landmarkclassifier-2.0.4/LANDMark/utils.py` & `landmarkclassifier-2.0.5/LANDMark/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,47 @@
 import numpy as np
 
 ##########################################################################################
 # For Bagging Classifier
 from sklearn.base import ClassifierMixin, BaseEstimator, clone
 from scipy.special import softmax
-from joblib import Parallel, delayed, parallel_backend
+from joblib import Parallel, delayed
 
 
 def _parallel_build(estimator, X, y):
-
     return estimator.fit(X, y)
 
 
 class Ensemble(ClassifierMixin, BaseEstimator):
-    def __init__(
-        self, base_estimator, n_estimators, class_names, n_jobs
-    ):
+    def __init__(self, base_estimator, n_estimators, class_names, n_jobs):
         self.base_estimator = base_estimator
         self.n_estimators = n_estimators
         self.classes_ = class_names
         self.n_jobs = n_jobs
 
     def fit(self, X, y):
-
         self.estimators_ = Parallel(n_jobs=self.n_jobs)(
-            delayed(_parallel_build)(
-                clone(self.base_estimator), X, y
-            )
+            delayed(_parallel_build)(clone(self.base_estimator), X, y)
             for i in range(self.n_estimators)
         )
 
         return self
 
     def predict(self, X):
-        
         prediction_probs = self.predict_proba(X)
 
-        max_probs = np.argmax(prediction_probs, axis = 1)
+        max_probs = np.argmax(prediction_probs, axis=1)
 
         predictions = [self.classes_[idx] for idx in max_probs]
 
         predictions = np.asarray(predictions)
 
         return predictions
 
     def predict_proba(self, X):
-
         class_map = {class_name: i for i, class_name in enumerate(self.classes_)}
 
         # Returns an array that of shape (n_estimators, n_samples)
         prediction_results = Parallel(self.n_jobs)(
             delayed(self.estimators_[i].predict)(X) for i in range(self.n_estimators)
         )
 
@@ -75,16 +67,16 @@
                 prediction_probs[sample_num, index] = 1.0
 
             else:
                 for idx, prob in enumerate(probs):
                     index = class_map[class_names[idx]]
                     prediction_probs[sample_num, index] = prob
 
-        #Ensure all probabilities sum to one
-        prediction_probs = softmax(prediction_probs, axis = 1)
+        # Ensure all probabilities sum to one
+        prediction_probs = softmax(prediction_probs, axis=1)
 
         return prediction_probs
 
 
 ##########################################################################################
 # For Neural Network Models
 import tensorflow as tf
```

### Comparing `landmarkclassifier-2.0.4/docs/API.md` & `landmarkclassifier-2.0.5/docs/API.md`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,16 @@
         features are randomly selected at each node.
         
     min_gain: float, default = 0.0
         The minimum gain needed to split a node.
         
     impurity: str, default = "gain"
         The method by which LANDMark calculates the purity of each split.
-        Currently, only information gain is used. Currently the options are
-        'gain', 'tsallis', 'gain-ratio', 'tsallis-gain-ratio'.
+        Currently the options are 'gain', 'tsallis', 'gain-ratio', and 
+        'tsallis-gain-ratio'.
         
     q: float, default = 1.5
         Parameter of the Tsallis entropy function. Smaller values may be more
         important when there are many classes. A value of 1.0 corresponds to
         information gain using Shannon entropy while a value of 2.0 corresponds
         to the gini index. Only used when impurity is set to 'tsallis' or
         'tsallis-gain-ratio'.
```

### Comparing `landmarkclassifier-2.0.4/docs/CONTRIBUTING.md` & `landmarkclassifier-2.0.5/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.4/tests/test_landmark.py` & `landmarkclassifier-2.0.5/tests/test_landmark.py`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.4/.gitignore` & `landmarkclassifier-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.4/LICENSE` & `landmarkclassifier-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.4/README.md` & `landmarkclassifier-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `landmarkclassifier-2.0.4/pyproject.toml` & `landmarkclassifier-2.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "LANDMarkClassifier"
-version = "2.0.4"
+version = "2.0.5"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "Teresita M. Porter"},
     {name = "Michael Wright"},
     {name = "G. Brian Golding"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
```

### Comparing `landmarkclassifier-2.0.4/PKG-INFO` & `landmarkclassifier-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LANDMarkClassifier
-Version: 2.0.4
+Version: 2.0.5
 Summary: LANDMark: An ensemble approach to the supervised selection of biomarkers in high-throughput sequencing data
 Project-URL: Homepage, https://github.com/jrudar/LANDMark
 Project-URL: Repository, https://github.com/jrudar/LANDMark.git
 Project-URL: Bug Tracker, https://github.com/jrudar/LANDMark/issues
 Author: Teresita M. Porter, Michael Wright, G. Brian Golding
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
```

