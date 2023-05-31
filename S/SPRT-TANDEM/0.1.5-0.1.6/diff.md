# Comparing `tmp/SPRT-TANDEM-0.1.5.tar.gz` & `tmp/SPRT-TANDEM-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SPRT-TANDEM-0.1.5.tar", last modified: Wed May 31 20:45:26 2023, max compression
+gzip compressed data, was "SPRT-TANDEM-0.1.6.tar", last modified: Wed May 31 23:47:55 2023, max compression
```

## Comparing `SPRT-TANDEM-0.1.5.tar` & `SPRT-TANDEM-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/
--rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.5/LICENSE
--rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/PKG-INFO
--rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 12:20:47.000000 SPRT-TANDEM-0.1.5/README.md
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/
--rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 20:45:26.000000 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/PKG-INFO
--rw-rw-r--   0 afe       (1000) afe       (1000)      675 2023-05-31 20:45:26.000000 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/SOURCES.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 20:45:26.000000 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/dependency_links.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       30 2023-05-31 20:45:26.000000 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/requires.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 20:45:26.000000 SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/top_level.txt
--rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/setup.cfg
--rw-r--r--   0 afe       (1000) afe       (1000)     1167 2023-05-31 20:45:20.000000 SPRT-TANDEM-0.1.5/setup.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/tandem/
--rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 05:14:48.000000 SPRT-TANDEM-0.1.5/tandem/__init__.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/tandem/config/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.5/tandem/config/__init__.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    11204 2023-05-31 20:04:18.000000 SPRT-TANDEM-0.1.5/tandem/config/config_definition.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/tandem/data/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.5/tandem/data/__init__.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/tandem/models/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.5/tandem/models/__init__.py
--rw-r--r--   0 afe       (1000) afe       (1000)    14111 2023-05-31 05:13:13.000000 SPRT-TANDEM-0.1.5/tandem/models/losses.py
--rwxr--r--   0 afe       (1000) afe       (1000)     1417 2023-05-31 05:14:34.000000 SPRT-TANDEM-0.1.5/tandem/models/optimizers.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 05:17:50.000000 SPRT-TANDEM-0.1.5/tandem/models/temporal_integrators.py
--rwxr--r--   0 afe       (1000) afe       (1000)     2822 2023-05-31 05:19:38.000000 SPRT-TANDEM-0.1.5/tandem/sprt_tandem_main.py
-drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 20:45:26.208594 SPRT-TANDEM-0.1.5/tandem/utils/
--rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 19:47:27.000000 SPRT-TANDEM-0.1.5/tandem/utils/__init__.py
--rwxr--r--   0 afe       (1000) afe       (1000)     6340 2023-05-31 05:18:03.000000 SPRT-TANDEM-0.1.5/tandem/utils/checkpoint.py
--rw-r--r--   0 afe       (1000) afe       (1000)    22645 2023-05-31 05:22:17.000000 SPRT-TANDEM-0.1.5/tandem/utils/data_processing.py
--rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 05:18:23.000000 SPRT-TANDEM-0.1.5/tandem/utils/hyperparameter_tuning.py
--rwxr--r--   0 afe       (1000) afe       (1000)    24962 2023-05-31 05:18:36.000000 SPRT-TANDEM-0.1.5/tandem/utils/logging.py
--rwxr--r--   0 afe       (1000) afe       (1000)    20082 2023-05-31 20:23:06.000000 SPRT-TANDEM-0.1.5/tandem/utils/misc.py
--rw-r--r--   0 afe       (1000) afe       (1000)    49570 2023-05-31 05:18:56.000000 SPRT-TANDEM-0.1.5/tandem/utils/performance_metrics.py
--rw-r--r--   0 afe       (1000) afe       (1000)    10223 2023-05-31 20:06:33.000000 SPRT-TANDEM-0.1.5/tandem/utils/training.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.950892 SPRT-TANDEM-0.1.6/
+-rw-r--r--   0 afe       (1000) afe       (1000)     1095 2023-05-01 05:13:22.000000 SPRT-TANDEM-0.1.6/LICENSE
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/PKG-INFO
+-rw-r--r--   0 afe       (1000) afe       (1000)    13560 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/README.md
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/
+-rw-rw-r--   0 afe       (1000) afe       (1000)    14145 2023-05-31 23:47:55.000000 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/PKG-INFO
+-rw-rw-r--   0 afe       (1000) afe       (1000)      675 2023-05-31 23:47:55.000000 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        1 2023-05-31 23:47:55.000000 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       35 2023-05-31 23:47:55.000000 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/requires.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)        7 2023-05-31 23:47:55.000000 SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/top_level.txt
+-rw-rw-r--   0 afe       (1000) afe       (1000)       38 2023-05-31 23:47:55.950892 SPRT-TANDEM-0.1.6/setup.cfg
+-rw-r--r--   0 afe       (1000) afe       (1000)     1175 2023-05-31 23:47:49.000000 SPRT-TANDEM-0.1.6/setup.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/tandem/
+-rw-r--r--   0 afe       (1000) afe       (1000)      356 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/tandem/config/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/config/__init__.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    11204 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/config/config_definition.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/tandem/data/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/data/__init__.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/tandem/models/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/models/__init__.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    14098 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/models/losses.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)     1417 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/models/optimizers.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26287 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/models/temporal_integrators.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)     2822 2023-05-31 23:37:43.000000 SPRT-TANDEM-0.1.6/tandem/sprt_tandem_main.py
+drwxrwxr-x   0 afe       (1000) afe       (1000)        0 2023-05-31 23:47:55.946892 SPRT-TANDEM-0.1.6/tandem/utils/
+-rw-r--r--   0 afe       (1000) afe       (1000)        0 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/__init__.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)     6340 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/checkpoint.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    22639 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/data_processing.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    26821 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/hyperparameter_tuning.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    24962 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/logging.py
+-rwxr-xr-x   0 afe       (1000) afe       (1000)    20082 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/misc.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    49601 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/performance_metrics.py
+-rw-r--r--   0 afe       (1000) afe       (1000)    10210 2023-05-31 23:37:27.000000 SPRT-TANDEM-0.1.6/tandem/utils/training.py
```

### Comparing `SPRT-TANDEM-0.1.5/LICENSE` & `SPRT-TANDEM-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/PKG-INFO` & `SPRT-TANDEM-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.5
+Version: 0.1.6
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `SPRT-TANDEM-0.1.5/README.md` & `SPRT-TANDEM-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/PKG-INFO` & `SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SPRT-TANDEM
-Version: 0.1.5
+Version: 0.1.6
 Summary: SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.
 Home-page: https://github.com/Akinori-F-Ebihara/SPRT-TANDEM-PyTorch
 Author: Akinori F. Ebihara
 Author-email: aebihara@nec.com
 License: MIT
 Keywords: Sequential Probability Ratio Test,likelihood ratio,density ratio estimation,early classification,artificial intelligence,machine learning
 Platform: UNKNOWN
```

### Comparing `SPRT-TANDEM-0.1.5/SPRT_TANDEM.egg-info/SOURCES.txt` & `SPRT-TANDEM-0.1.6/SPRT_TANDEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/setup.py` & `SPRT-TANDEM-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(
     path.join(path.abspath(path.dirname(__file__)), "README.md"), encoding="utf-8"
 ) as f:
     long_description = f.read()
 
 setup(
     name="SPRT-TANDEM",
-    version="0.1.5",
+    version="0.1.6",
     license="MIT",
     description="SPRT-TANDEM for sequential density ratio estimation to simultaneously optimize both speed and accuracy of early-classification.",
     author="Akinori F. Ebihara",
     author_email="aebihara@nec.com",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -26,10 +26,10 @@
         "Sequential Probability Ratio Test",
         "likelihood ratio",
         "density ratio estimation",
         "early classification",
         "artificial intelligence",
         "machine learning",
     ],
-    install_requires=["torch", "torchinfo", "optuna", "loguru"],
+    install_requires=["torch", "torchinfo", "optuna", "loguru", "tqdm"],
     python_requires=">=3.8",
 )
```

### Comparing `SPRT-TANDEM-0.1.5/tandem/config/config_definition.py` & `SPRT-TANDEM-0.1.6/tandem/config/config_definition.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/tandem/models/losses.py` & `SPRT-TANDEM-0.1.6/tandem/models/losses.py`

 * *Files 0% similar despite different names*

```diff
@@ -288,15 +288,15 @@
     total_loss = 0.0
     for i, (loss, const) in enumerate(zip(losses, constant_weights)):
         weight = torch.finfo(torch.float32).eps + model.adaptive_loss_weights[i] ** 2
         total_loss += 0.5 * loss * const / weight + torch.log(weight)
     return total_loss
 
 
-def compute_loss_and_metrics(model, x, labels, global_step, config):
+def compute_loss_and_metrics(model, x, labels, config):
     """Calculate loss and gradients.
     Args:
         model: A tf.keras.Model object.
         x: A Tensor. A batch of time-series input data
             without sequential_slice and sequential_concat.
         y: A Tensor. A batch of labels
             without sequential_slice and sequential_concat.
```

### Comparing `SPRT-TANDEM-0.1.5/tandem/models/optimizers.py` & `SPRT-TANDEM-0.1.6/tandem/models/optimizers.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/tandem/models/temporal_integrators.py` & `SPRT-TANDEM-0.1.6/tandem/models/temporal_integrators.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/tandem/sprt_tandem_main.py` & `SPRT-TANDEM-0.1.6/tandem/sprt_tandem_main.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/tandem/utils/checkpoint.py` & `SPRT-TANDEM-0.1.6/tandem/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/tandem/utils/data_processing.py` & `SPRT-TANDEM-0.1.6/tandem/utils/data_processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,43 +53,43 @@
 
 
 def move_data_to_device(
     data: Union[
         Tuple[Tensor, Tensor],
         Tuple[Tensor, Tensor, Tensor],
     ],
+    device: str,
 ) -> Union[Tuple[Tensor, Tensor], Tuple[Tensor, Tensor, Tensor]]:
     """
     Move the input data to the specified device based on the length of the input data tuple.
 
     Args:
         data: Tuple containing either (x_batch, y_batch, gt_llrs_batch) or (x_batch, y_batch).
         device: The device to move the data to.
 
     Returns:
         A tuple with data moved to the specified device.
 
     Raises:
         ValueError: If the length of the input data tuple is not 2 or 3.
     """
-    rank = dist.get_rank()
 
     if len(data) == 3:
         # if the dataset contains ground-truth log likelihood ratio.
         # Casting is required to explicitly show the type to mypy. Note that it does not do any actual runtime checks.
         x_batch, y_batch, gt_llrs_batch = cast(Tuple[Tensor, Tensor, Tensor], data)
         x_batch, y_batch, gt_llrs_batch = move_to_device(
-            rank, x_batch, y_batch, gt_llrs_batch
+            device, x_batch, y_batch, gt_llrs_batch
         )
         return x_batch, y_batch, gt_llrs_batch
     elif len(data) == 2:
         # Data and label only: typical real-world data.
         # Casting is required to explicitly show the type to mypy. Note that it does not do any actual runtime checks.
         x_batch, y_batch = cast(Tuple[Tensor, Tensor], data)
-        x_batch, y_batch = move_to_device(rank, x_batch, y_batch)
+        x_batch, y_batch = move_to_device(device, x_batch, y_batch)
         return x_batch, y_batch
     else:
         raise ValueError(
             "data tuple length is expected either to be "
             f"3 (x, y, llr) or 2 (x, y) but got {len(data)=}!"
         )
```

### Comparing `SPRT-TANDEM-0.1.5/tandem/utils/hyperparameter_tuning.py` & `SPRT-TANDEM-0.1.6/tandem/utils/hyperparameter_tuning.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/tandem/utils/logging.py` & `SPRT-TANDEM-0.1.6/tandem/utils/logging.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/tandem/utils/misc.py` & `SPRT-TANDEM-0.1.6/tandem/utils/misc.py`

 * *Files identical despite different names*

### Comparing `SPRT-TANDEM-0.1.5/tandem/utils/performance_metrics.py` & `SPRT-TANDEM-0.1.6/tandem/utils/performance_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,28 +115,29 @@
         raise ValueError("Unknown phase!")
     performance_metrics = initialize_performance_metrics()
 
     return is_train, iter_num, performance_metrics, barcolor
 
 
 def accumulate_performance(
-    performance_metrics, y_batch, gt_llrs_batch, monitored_values, phase_manager
+    performance_metrics, y_batch, gt_llrs_batch, monitored_values, phase_manager=None
 ):
     """ """
 
     performance_metrics["losses"].append(monitored_values["losses"])
     performance_metrics["mean_abs_error"].append(
         calc_llr_abserr(monitored_values["llrs"], gt_llrs_batch)
     )  # (batch_size, time_steps)
     performance_metrics["seqconfmx_llr"] += llr_sequential_confmx(
         monitored_values["llrs"], y_batch
     )
     performance_metrics["hitting_time"].append(monitored_values["mht"])
     performance_metrics["sns_conf"].append(monitored_values["sns_from_confmx"])
-    performance_metrics["grad_norm"].append(phase_manager.grad_norm)
+    if phase_manager:
+        performance_metrics["grad_norm"].append(phase_manager.grad_norm)
 
     return performance_metrics
 
 
 def summarize_performance(performance_metrics):
     """ """
```

### Comparing `SPRT-TANDEM-0.1.5/tandem/utils/training.py` & `SPRT-TANDEM-0.1.6/tandem/utils/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
         # Train phase: run preprocesses (model.train(), optimizer.zero_grad()) and postprocesses (optimizer.step(), loss.backward())
         # Eval phase: run preprocesses (model.eval()), enter torch.no_grad() mode, no postprocess
         with PyTorchPhaseManager(
             model,
             optimizer,
             phase=phase,
             loss_func=compute_loss_and_metrics,
-            loss_args=(x_batch, y_batch, global_step),
+            loss_args=(x_batch, y_batch),
             config=config,
         ) as p:
             monitored_values = p.call_loss()
             p.loss = monitored_values["losses"]["total_loss"]
 
         # Store performance metrics
         performance_metrics = accumulate_performance(
```

