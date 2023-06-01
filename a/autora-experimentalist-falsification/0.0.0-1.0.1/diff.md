# Comparing `tmp/autora-experimentalist-falsification-0.0.0.tar.gz` & `tmp/autora-experimentalist-falsification-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-experimentalist-falsification-0.0.0.tar", last modified: Wed May 31 19:28:25 2023, max compression
+gzip compressed data, was "autora-experimentalist-falsification-1.0.1.tar", last modified: Thu Jun  1 00:40:35 2023, max compression
```

## Comparing `autora-experimentalist-falsification-0.0.0.tar` & `autora-experimentalist-falsification-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:28:25.793054 autora-experimentalist-falsification-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-31 19:28:25.789054 autora-experimentalist-falsification-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-31 19:28:14.000000 autora-experimentalist-falsification-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-31 19:28:14.000000 autora-experimentalist-falsification-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 19:28:25.793054 autora-experimentalist-falsification-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:28:25.789054 autora-experimentalist-falsification-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:28:25.789054 autora-experimentalist-falsification-0.0.0/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:28:25.789054 autora-experimentalist-falsification-0.0.0/src/autora/experimentalist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:28:25.789054 autora-experimentalist-falsification-0.0.0/src/autora/experimentalist/pooler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:28:25.789054 autora-experimentalist-falsification-0.0.0/src/autora/experimentalist/pooler/falsification/
--rw-r--r--   0 runner    (1001) docker     (123)    18027 2023-05-31 19:28:14.000000 autora-experimentalist-falsification-0.0.0/src/autora/experimentalist/pooler/falsification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:28:25.789054 autora-experimentalist-falsification-0.0.0/src/autora/experimentalist/sampler/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:28:25.789054 autora-experimentalist-falsification-0.0.0/src/autora/experimentalist/sampler/falsification/
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-05-31 19:28:14.000000 autora-experimentalist-falsification-0.0.0/src/autora/experimentalist/sampler/falsification/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:28:25.789054 autora-experimentalist-falsification-0.0.0/src/autora_experimentalist_falsification.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-31 19:28:25.000000 autora-experimentalist-falsification-0.0.0/src/autora_experimentalist_falsification.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-31 19:28:25.000000 autora-experimentalist-falsification-0.0.0/src/autora_experimentalist_falsification.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 19:28:25.000000 autora-experimentalist-falsification-0.0.0/src/autora_experimentalist_falsification.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-31 19:28:25.000000 autora-experimentalist-falsification-0.0.0/src/autora_experimentalist_falsification.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-31 19:28:25.000000 autora-experimentalist-falsification-0.0.0/src/autora_experimentalist_falsification.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 19:28:25.789054 autora-experimentalist-falsification-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-05-31 19:28:14.000000 autora-experimentalist-falsification-0.0.0/tests/test_exp_falsification_pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-05-31 19:28:14.000000 autora-experimentalist-falsification-0.0.0/tests/test_exp_falsification_sampler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.642196 autora-experimentalist-falsification-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.642196 autora-experimentalist-falsification-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   352733 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/basic-usage-pooler.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   349559 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/basic-usage-sampler.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/index-pooler.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/index-sampler.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.642196 autora-experimentalist-falsification-1.0.1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/javascripts/mathjax.js
+-rw-r--r--   0 runner    (1001) docker     (123)    58500 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/pooler-model-vs-data.png
+-rw-r--r--   0 runner    (1001) docker     (123)    60582 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/pooler-mse.png
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/docs/quickstart-pooler.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/mkdocs/gen_ref_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/mkdocs_pooler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/mkdocs_sampler.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/pooler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/pooler/falsification/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/pooler/falsification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.638196 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/sampler/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/sampler/falsification/
+-rw-r--r--   0 runner    (1001) docker     (123)     9725 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/sampler/falsification/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-01 00:40:35.000000 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-01 00:40:35.000000 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 00:40:35.000000 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 00:40:35.000000 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 00:40:35.000000 autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:35.646196 autora-experimentalist-falsification-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5149 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/tests/test_exp_falsification_pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-06-01 00:40:14.000000 autora-experimentalist-falsification-1.0.1/tests/test_exp_falsification_sampler.py
```

### Comparing `autora-experimentalist-falsification-0.0.0/PKG-INFO` & `autora-experimentalist-falsification-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-falsification
-Version: 0.0.0
+Version: 1.0.1
 Summary: AutoRA Falsification Experimentalist
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-falsification
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <3.11,>=3.8.10
```

### Comparing `autora-experimentalist-falsification-0.0.0/README.md` & `autora-experimentalist-falsification-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-0.0.0/src/autora/experimentalist/pooler/falsification/__init__.py` & `autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/pooler/falsification/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -386,35 +386,35 @@
     plot_input = plot_input[plot_input_order]
     popper_target = popper_target[plot_input_order]
     # popper_prediction = popper_prediction[plot_input_order]
     plt.plot(popper_input_full, popper_prediction.detach().numpy(), label="Predicted MSE of the Model")
     plt.scatter(
         plot_input, popper_target.detach().numpy(), s=20, c="red", label="True MSE of the Model"
     )
-    plt.xlabel("x")
+    plt.xlabel("Experimental Condition X")
     plt.ylabel("MSE of Model")
-    plt.title("Prediction of Falsification Sampler")
+    plt.title("Prediction of Falsification Network")
     plt.legend()
     plt.show()
 
     # CONVERGENCE PLOT
     plt.plot(losses)
     plt.xlabel("Epoch")
     plt.ylabel("Loss")
-    plt.title("Loss for the Popper Network")
+    plt.title("Loss for the Falsification Network")
     plt.show()
 
     # MODEL PREDICTION PLOT
     model_prediction = model_prediction[plot_input_order]
     target = target[plot_input_order]
     plt.plot(plot_input, model_prediction, label="Model Prediction")
     plt.scatter(plot_input, target, s=20, c="red", label="Data")
-    plt.xlabel("x")
-    plt.ylabel("y")
-    plt.title("Model Prediction vs. Data")
+    plt.xlabel("Experimental Condition X")
+    plt.ylabel("Observation Y")
+    plt.title("Model Prediction Vs. Data")
     plt.legend()
     plt.show()
 
 
 # define the network
 class PopperNet(nn.Module):
     def __init__(self, n_input: torch.Tensor, n_output: torch.Tensor):
```

### Comparing `autora-experimentalist-falsification-0.0.0/src/autora/experimentalist/sampler/falsification/__init__.py` & `autora-experimentalist-falsification-1.0.1/src/autora/experimentalist/sampler/falsification/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -67,31 +67,83 @@
         try:
             predicted_observations = np.array(predicted_observations)
         except Exception:
             raise Exception("Model prediction must be convertable to numpy array.")
     if predicted_observations.ndim == 1:
         predicted_observations = predicted_observations.reshape(-1, 1)
 
-    new_conditions, scores = falsification_score_sampler(
+    new_conditions, scores = falsification_score_sampler_from_predictions(
         condition_pool,
         predicted_observations,
         reference_conditions,
         reference_observations,
         metadata,
         num_samples,
         training_epochs,
         training_lr,
         plot,
     )
 
     return new_conditions
 
-
 def falsification_score_sampler(
     condition_pool,
+    model,
+    reference_conditions: np.ndarray,
+    reference_observations: np.ndarray,
+    metadata: Optional[VariableCollection] = None,
+    num_samples: Optional[int] = None,
+    training_epochs: int = 1000,
+    training_lr: float = 1e-3,
+    plot: bool = False,
+):
+    """
+    A Sampler that generates samples of experimental conditions with the objective of maximizing the
+    (approximated) loss of a model relating experimental conditions to observations. The samples are generated by first
+    training a neural network to approximate the loss of a model for all patterns in the training data.
+    Once trained, the network is then provided with the candidate samples of experimental conditions and the selects
+    those with the highest loss.
+
+    Args:
+        condition_pool: The candidate samples of experimental conditions to be evaluated.
+        model: Scikit-learn model, could be either a classification or regression model
+        reference_conditions: Experimental conditions that the model was trained on
+        reference_observations: Observations that the model was trained to predict
+        metadata: Meta-data about the dependent and independent variables specifying the experimental conditions
+        num_samples: Number of samples to return
+        training_epochs: Number of epochs to train the popper network for approximating the
+        error of the model
+        training_lr: Learning rate for training the popper network
+        plot: Print out the prediction of the popper network as well as its training loss
+
+    Returns:
+        new_conditions: Samples of experimental conditions with the highest loss
+        scores: Normalized falsification scores for the samples
+
+    """
+
+    reference_conditions = np.array(reference_conditions)
+    if len(reference_conditions.shape) == 1:
+        reference_conditions = reference_conditions.reshape(-1, 1)
+
+    predicted_observations = model.predict(reference_conditions)
+
+    return falsification_score_sampler_from_predictions(condition_pool,
+                                                        predicted_observations,
+                                                        reference_conditions,
+                                                        reference_observations,
+                                                        metadata,
+                                                        num_samples,
+                                                        training_epochs,
+                                                        training_lr,
+                                                        plot)
+
+
+def falsification_score_sampler_from_predictions(
+    condition_pool,
     predicted_observations: np.ndarray,
     reference_conditions: np.ndarray,
     reference_observations: np.ndarray,
     metadata: Optional[VariableCollection] = None,
     num_samples: Optional[int] = None,
     training_epochs: int = 1000,
     training_lr: float = 1e-3,
```

### Comparing `autora-experimentalist-falsification-0.0.0/src/autora_experimentalist_falsification.egg-info/PKG-INFO` & `autora-experimentalist-falsification-1.0.1/src/autora_experimentalist_falsification.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-experimentalist-falsification
-Version: 0.0.0
+Version: 1.0.1
 Summary: AutoRA Falsification Experimentalist
 Author-email: Sebastian Musslick <sebastian@musslick.de>
 License: MIT License
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-experimentalist-falsification
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <3.11,>=3.8.10
```

### Comparing `autora-experimentalist-falsification-0.0.0/tests/test_exp_falsification_pooler.py` & `autora-experimentalist-falsification-1.0.1/tests/test_exp_falsification_pooler.py`

 * *Files identical despite different names*

### Comparing `autora-experimentalist-falsification-0.0.0/tests/test_exp_falsification_sampler.py` & `autora-experimentalist-falsification-1.0.1/tests/test_exp_falsification_sampler.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import torch
 from sklearn.linear_model import LinearRegression, LogisticRegression
 
 from autora.experimentalist.pipeline import Pipeline
 from autora.experimentalist.sampler.falsification import (
     falsification_sampler,
     falsification_score_sampler,
+    falsification_score_sampler_from_predictions,
 )
 from autora.variable import DV, IV, ValueType, VariableCollection
 from tests.test_exp_falsification_pooler import get_sin_data, get_xor_data
 
 x_min_regression = 0
 x_max_regression = 6
 
@@ -213,15 +214,15 @@
     model = LinearRegression()
     model.fit(X_train, Y_train)
 
     # compute model predictions for trained conditions
     Y_predicted = model.predict(X_train)
 
     # get scores from falsification sampler
-    X_selected, scores = falsification_score_sampler(
+    X_selected, scores = falsification_score_sampler_from_predictions(
         condition_pool=X,
         predicted_observations=Y_predicted,
         reference_conditions=X_train,
         reference_observations=Y_train,
         training_epochs=1000,
         training_lr=1e-3,
         plot=False,
@@ -250,15 +251,15 @@
     # generate sampled conditions
     X_train = np.linspace(x_min_regression, x_max_regression, 100)
 
     # generate reconstructed data (this data may be produced by an autoencoder)
     X_reconstructed = X_train + np.sin(X_train)
 
     # get scores from falsification sampler
-    X_selected, scores = falsification_score_sampler(
+    X_selected, scores = falsification_score_sampler_from_predictions(
         condition_pool=X,
         predicted_observations=X_reconstructed,
         reference_conditions=X_train,
         reference_observations=X_train,
         training_epochs=1000,
         training_lr=1e-3,
         plot=False,
@@ -270,7 +271,59 @@
 
     # check if the scores are properly ordered
     assert scores[0] > scores[1]
 
     # check if the data points with the highest predicted error were selected
     assert np.round(X_selected[0, 0], 4) == 1.8 or np.round(X_selected[0, 0], 4) == 4.8
     assert np.round(X_selected[1, 0], 4) == 1.8 or np.round(X_selected[1, 0], 4) == 4.8
+
+
+def test_doc_example():
+    # Specify X and Y
+    X = np.linspace(0, 2 * np.pi, 100)
+    Y = np.sin(X)
+    X_prime = np.linspace(0, 6.5, 14)
+
+    # We need to provide the pooler with some metadata specifying the independent and dependent variables
+    # Specify independent variable
+    iv = IV(
+        name="x",
+        value_range=(0, 2 * np.pi),
+    )
+
+    # specify dependent variable
+    dv = DV(
+        name="y",
+        type=ValueType.REAL,
+    )
+
+    # Variable collection with ivs and dvs
+    metadata = VariableCollection(
+        independent_variables=[iv],
+        dependent_variables=[dv],
+    )
+
+    # Fit a linear regression to the data
+    model = LinearRegression()
+    model.fit(X.reshape(-1, 1), Y)
+
+    # Sample four novel conditions
+    X_selected = falsification_sampler(
+        condition_pool=X_prime,
+        model=model,
+        reference_conditions=X,
+        reference_observations=Y,
+        metadata=metadata,
+        num_samples=4,
+    )
+
+    # convert Iterable to numpy array
+    X_selected = np.array(list(X_selected))
+
+    # We may also obtain samples along with their z-scored novelty scores
+    X_selected, scores = falsification_score_sampler(
+        condition_pool=X_prime,
+        model=model,
+        reference_conditions=X,
+        reference_observations=Y,
+        metadata=metadata,
+        num_samples=4)
```

