# Comparing `tmp/flaxsr-0.0.3a0.tar.gz` & `tmp/flaxsr-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flaxsr-0.0.3a0.tar", last modified: Tue May 30 16:13:36 2023, max compression
+gzip compressed data, was "flaxsr-0.0.4.tar", last modified: Thu Jun  1 08:20:35 2023, max compression
```

## Comparing `flaxsr-0.0.3a0.tar` & `flaxsr-0.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-05-30 16:13:36.282866 flaxsr-0.0.3a0/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)    11313 2023-05-12 09:22:40.000000 flaxsr-0.0.3a0/LICENSE
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1869 2023-05-30 16:13:36.282866 flaxsr-0.0.3a0/PKG-INFO
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1243 2023-05-17 15:37:00.000000 flaxsr-0.0.3a0/README.md
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-05-30 16:13:36.282866 flaxsr-0.0.3a0/flaxsr/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      111 2023-05-17 15:18:45.000000 flaxsr-0.0.3a0/flaxsr/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      661 2023-05-12 10:02:07.000000 flaxsr-0.0.3a0/flaxsr/_utils.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-05-30 16:13:36.282866 flaxsr-0.0.3a0/flaxsr/layers/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      179 2023-05-12 09:22:40.000000 flaxsr-0.0.3a0/flaxsr/layers/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1651 2023-05-16 13:28:13.000000 flaxsr-0.0.3a0/flaxsr/layers/stochastic.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1673 2023-05-16 13:28:27.000000 flaxsr-0.0.3a0/flaxsr/layers/upscale.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-05-30 16:13:36.282866 flaxsr-0.0.3a0/flaxsr/losses/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      785 2023-05-22 10:19:54.000000 flaxsr-0.0.3a0/flaxsr/losses/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4136 2023-05-17 15:02:42.000000 flaxsr-0.0.3a0/flaxsr/losses/adversarial_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2298 2023-05-16 15:02:06.000000 flaxsr-0.0.3a0/flaxsr/losses/perceptual_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1745 2023-05-12 13:40:32.000000 flaxsr-0.0.3a0/flaxsr/losses/pixel_wise_losses.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2464 2023-05-17 15:10:31.000000 flaxsr-0.0.3a0/flaxsr/losses/utils.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-05-30 16:13:36.282866 flaxsr-0.0.3a0/flaxsr/models/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      355 2023-05-12 09:22:40.000000 flaxsr-0.0.3a0/flaxsr/models/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3749 2023-05-12 09:48:06.000000 flaxsr-0.0.3a0/flaxsr/models/edsr.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      922 2023-05-12 09:48:06.000000 flaxsr-0.0.3a0/flaxsr/models/espcn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1138 2023-05-12 09:48:06.000000 flaxsr-0.0.3a0/flaxsr/models/fsrcnn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     6677 2023-05-12 09:48:06.000000 flaxsr-0.0.3a0/flaxsr/models/nafssr.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      994 2023-05-12 09:48:06.000000 flaxsr-0.0.3a0/flaxsr/models/ncnet.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1078 2023-05-12 09:49:43.000000 flaxsr-0.0.3a0/flaxsr/models/srcnn.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2205 2023-05-12 09:49:43.000000 flaxsr-0.0.3a0/flaxsr/models/srgan.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      954 2023-05-12 09:50:48.000000 flaxsr-0.0.3a0/flaxsr/models/vdsr.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-05-30 16:13:36.282866 flaxsr-0.0.3a0/flaxsr/training/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      149 2023-05-17 15:18:04.000000 flaxsr-0.0.3a0/flaxsr/training/__init__.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      552 2023-05-17 15:18:04.000000 flaxsr-0.0.3a0/flaxsr/training/train_states.py
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      913 2023-05-17 15:14:40.000000 flaxsr-0.0.3a0/flaxsr/training/train_step.py
-drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-05-30 16:13:36.282866 flaxsr-0.0.3a0/flaxsr.egg-info/
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1869 2023-05-30 16:13:36.000000 flaxsr-0.0.3a0/flaxsr.egg-info/PKG-INFO
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      745 2023-05-30 16:13:36.000000 flaxsr-0.0.3a0/flaxsr.egg-info/SOURCES.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        1 2023-05-30 16:13:36.000000 flaxsr-0.0.3a0/flaxsr.egg-info/dependency_links.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       40 2023-05-30 16:13:36.000000 flaxsr-0.0.3a0/flaxsr.egg-info/requires.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        7 2023-05-30 16:13:36.000000 flaxsr-0.0.3a0/flaxsr.egg-info/top_level.txt
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       38 2023-05-30 16:13:36.282866 flaxsr-0.0.3a0/setup.cfg
--rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      945 2023-05-30 16:12:34.000000 flaxsr-0.0.3a0/setup.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)    11313 2023-05-12 09:22:40.000000 flaxsr-0.0.4/LICENSE
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2807 2023-06-01 08:20:35.954687 flaxsr-0.0.4/PKG-INFO
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2183 2023-06-01 08:16:14.000000 flaxsr-0.0.4/README.md
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      111 2023-05-17 15:18:45.000000 flaxsr-0.0.4/flaxsr/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      661 2023-05-12 10:02:07.000000 flaxsr-0.0.4/flaxsr/_utils.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr/layers/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      179 2023-05-12 09:22:40.000000 flaxsr-0.0.4/flaxsr/layers/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1651 2023-05-16 13:28:13.000000 flaxsr-0.0.4/flaxsr/layers/stochastic.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1673 2023-05-16 13:28:27.000000 flaxsr-0.0.4/flaxsr/layers/upscale.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr/losses/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      921 2023-06-01 00:47:20.000000 flaxsr-0.0.4/flaxsr/losses/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4441 2023-05-31 15:44:50.000000 flaxsr-0.0.4/flaxsr/losses/adversarial_losses.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2295 2023-05-31 15:35:59.000000 flaxsr-0.0.4/flaxsr/losses/perceptual_losses.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1664 2023-05-31 15:35:14.000000 flaxsr-0.0.4/flaxsr/losses/pixel_wise_losses.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4390 2023-06-01 00:50:10.000000 flaxsr-0.0.4/flaxsr/losses/utils.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr/models/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      355 2023-05-12 09:22:40.000000 flaxsr-0.0.4/flaxsr/models/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     3749 2023-05-12 09:48:06.000000 flaxsr-0.0.4/flaxsr/models/edsr.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      922 2023-05-12 09:48:06.000000 flaxsr-0.0.4/flaxsr/models/espcn.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1138 2023-05-12 09:48:06.000000 flaxsr-0.0.4/flaxsr/models/fsrcnn.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     6677 2023-05-12 09:48:06.000000 flaxsr-0.0.4/flaxsr/models/nafssr.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      994 2023-05-12 09:48:06.000000 flaxsr-0.0.4/flaxsr/models/ncnet.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1078 2023-05-12 09:49:43.000000 flaxsr-0.0.4/flaxsr/models/srcnn.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     4129 2023-05-30 16:42:22.000000 flaxsr-0.0.4/flaxsr/models/srgan.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      954 2023-05-12 09:50:48.000000 flaxsr-0.0.4/flaxsr/models/vdsr.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr/training/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      149 2023-06-01 05:21:42.000000 flaxsr-0.0.4/flaxsr/training/__init__.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      503 2023-06-01 00:48:20.000000 flaxsr-0.0.4/flaxsr/training/train_states.py
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     1345 2023-06-01 05:25:08.000000 flaxsr-0.0.4/flaxsr/training/train_step.py
+drwxrwxr-x   0 dslisleedh  (1007) dslisleedh  (1007)        0 2023-06-01 08:20:35.954687 flaxsr-0.0.4/flaxsr.egg-info/
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)     2807 2023-06-01 08:20:35.000000 flaxsr-0.0.4/flaxsr.egg-info/PKG-INFO
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      745 2023-06-01 08:20:35.000000 flaxsr-0.0.4/flaxsr.egg-info/SOURCES.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        1 2023-06-01 08:20:35.000000 flaxsr-0.0.4/flaxsr.egg-info/dependency_links.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       46 2023-06-01 08:20:35.000000 flaxsr-0.0.4/flaxsr.egg-info/requires.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)        7 2023-06-01 08:20:35.000000 flaxsr-0.0.4/flaxsr.egg-info/top_level.txt
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)       38 2023-06-01 08:20:35.954687 flaxsr-0.0.4/setup.cfg
+-rw-rw-r--   0 dslisleedh  (1007) dslisleedh  (1007)      961 2023-06-01 08:15:31.000000 flaxsr-0.0.4/setup.py
```

### Comparing `flaxsr-0.0.3a0/LICENSE` & `flaxsr-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/PKG-INFO` & `flaxsr-0.0.4/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: flaxsr
-Version: 0.0.3a0
-Summary: Super Resolution models with Jax/Flax
-Home-page: https://github.com/dslisleedh/FlaxSR
-Author: dslisleedh
-Author-email: dslisleedh@gmail.com
-Project-URL: Bug Tracker, https://github.com/dslisleedh/FlaxSR/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Image Processing
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # FlaxSR
 
 Super Resolution models with Jax/Flax
 
 ## HOW TO USE
 
 ### Install
@@ -66,14 +49,49 @@
 # Or you can use flaxsr.get function
 metric = flaxsr.get("losses", "l1", "mean")
 loss_get = metric(hr, sr)
 
 np.allclose(loss, loss_get)
 ```
 
+<b> You can easily load model/losses and train model using custom train_states. </b>
+
+ - Train example
+```python
+import flaxsr
+import jax
+import jax.numpy as jnp
+import numpy as np
+import optax
+
+model_kwargs = {
+    'n_filters': 64, 'n_blocks': 8, 'scale': 4
+}
+model = flaxsr.get("models", "vdsr", **model_kwargs)
+losses = flaxsr.losses.LossWrapper(
+    losses=['l1', 'l2'], weights=[1.0, 1.0]
+)
+params = model.init(jax.random.PRNGKey(0), jnp.ones((1, 8, 8, 3), dtype=jnp.float32))
+tx = optax.adam(1e-3)
+
+state = flaxsr.training.TrainState.create(
+    apply_fn=model.apply, params=params, tx=tx, losses=losses
+)
+
+hr = jnp.ones((1, 32, 32, 3), dtype=jnp.float32)
+lr = jnp.ones((1, 8, 8, 3), dtype=jnp.float32)
+batch = (lr, hr)
+
+state_new, loss = flaxsr.training.discriminative_train_step(state, batch)
+
+assert state_new.step == 1
+np.not_equal(state_new.params['params']['Conv_0']['kernel'], state.params['params']['Conv_0']['kernel'])
+```
+
+
 ## Models implemented
  - SRCNN
  - FSRCNN
  - ESPCN
  - VDSR
  - EDSR, MDSR,
  - NCNet
```

### Comparing `flaxsr-0.0.3a0/flaxsr/_utils.py` & `flaxsr-0.0.4/flaxsr/_utils.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/flaxsr/layers/stochastic.py` & `flaxsr-0.0.4/flaxsr/layers/stochastic.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/flaxsr/layers/upscale.py` & `flaxsr-0.0.4/flaxsr/layers/upscale.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/flaxsr/losses/__init__.py` & `flaxsr-0.0.4/flaxsr/losses/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,12 +13,16 @@
     least_square_generator_loss as least_square_generator_loss,
     relativistic_discriminator_loss as relativistic_discriminator_loss,
     relativistic_generator_loss as relativistic_generator_loss,
 )
 from .utils import (
     check_vgg_params_exists as check_vgg_params_exists,
     load_vgg19_params as load_vgg19_params,
+    # get_loss_wrapper as get_loss_wrapper,
+    # compute_loss as compute_loss,
+    Reduces as Reduces,
+    LossWrapper as LossWrapper,
 )
 
 
 check_vgg_params_exists()
 del check_vgg_params_exists
```

### Comparing `flaxsr-0.0.3a0/flaxsr/losses/adversarial_losses.py` & `flaxsr-0.0.4/flaxsr/losses/adversarial_losses.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,134 +7,143 @@
 
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal
 
-from flaxsr.losses.utils import reduce_fn
+from flaxsr.losses.utils import reduce_fn, Reduces
 from flaxsr._utils import register
 
 
 def minmax_discriminator_loss(
-        true: jnp.ndarray, fake: jnp.ndarray, mode: Literal['mean', 'sum', None] = 'mean',
+        true: jnp.ndarray, fake: jnp.ndarray, reduces: str | Reduces = 'mean',
         from_logits: bool = True, *args, **kwargs
 ):
     if from_logits:
         true_loss = -jax.nn.log_sigmoid(true)
         fake_loss = -jax.nn.log_sigmoid(-fake)
     else:
         true_loss = -jnp.log(true)
         fake_loss = -jnp.log(1. - fake)
 
     loss = true_loss + fake_loss
-    return reduce_fn(loss, mode)
+    return reduce_fn(loss, reduces)
 
 
 def minmax_generator_loss(
-        fake: jnp.ndarray, mode: Literal['mean', 'sum', None] = 'mean', from_logits: bool = True,
+        fake: jnp.ndarray, reduces: str | Reduces = 'mean', from_logits: bool = True,
         *args, **kwargs
 ):
     if from_logits:
         loss = -jax.nn.log_sigmoid(fake)
     else:
         loss = -jnp.log(fake)
 
-    return reduce_fn(loss, mode)
+    return reduce_fn(loss, reduces)
 
 
 @register('losses', 'minmax_discriminator')
 class MinmaxDiscriminatorLoss:
-    def __init__(self, from_logits: bool = True, mode: Literal['mean', 'sum', None] = 'mean'):
+    def __init__(self, from_logits: bool = True, reduces: str | Reduces = 'mean'):
         self.from_logits = from_logits
-        self.mode = mode
+        self.reduces = reduces
 
     def __call__(self, true: jnp.ndarray, fake: jnp.ndarray):
-        return minmax_discriminator_loss(true, fake, self.mode, self.from_logits)
+        return minmax_discriminator_loss(true, fake, self.reduces, self.from_logits)
 
 
 @register('losses', 'minmax_generator')
 class MinmaxGeneratorLoss:
-    def __init__(self, from_logits: bool = True, mode: Literal['mean', 'sum', None] = 'mean'):
+    def __init__(self, from_logits: bool = True, reduces: str | Reduces = 'mean'):
         self.from_logits = from_logits
-        self.mode = mode
+        self.reduces = reduces
 
     def __call__(self, fake: jnp.ndarray):
-        return minmax_generator_loss(fake, self.mode, self.from_logits)
+        return minmax_generator_loss(fake, self.reduces, self.from_logits)
 
 
 def least_square_discriminator_loss(
-        true: jnp.ndarray, fake: jnp.ndarray, mode: Literal['mean', 'sum', None] = 'mean',
+        true: jnp.ndarray, fake: jnp.ndarray, from_logits: bool = True, reduces: str | Reduces = 'mean',
         *args, **kwargs
 ):
+    if from_logits:
+        true = jax.nn.sigmoid(true)
+        fake = jax.nn.sigmoid(fake)
+
     true_loss = .5 * jnp.square(true - 1.)
     fake_loss = .5 * jnp.square(fake)
 
     loss = true_loss + fake_loss
-    return reduce_fn(loss, mode)
+    return reduce_fn(loss, reduces)
 
 
 def least_square_generator_loss(
-        fake: jnp.ndarray, mode: Literal['mean', 'sum', None] = 'mean',
+        fake: jnp.ndarray, from_logits: bool = True, reduces: str | Reduces = 'mean',
         *args, **kwargs
 ):
+    if from_logits:
+        fake = jax.nn.sigmoid(fake)
+
     loss = .5 * jnp.square(fake - 1.)
 
-    return reduce_fn(loss, mode)
+    return reduce_fn(loss, reduces)
 
 
 @register('losses', 'least_square_discriminator')
 class LeastSquareDiscriminatorLoss:
-    def __init__(self, mode: Literal['mean', 'sum', None] = 'mean'):
-        self.mode = mode
+    def __init__(self, from_logits: bool = True, reduces: str | Reduces = 'mean'):
+        self.from_logits = from_logits
+        self.reduces = reduces
 
     def __call__(self, true: jnp.ndarray, fake: jnp.ndarray):
-        return least_square_discriminator_loss(true, fake, self.mode)
+        return least_square_discriminator_loss(true, fake, self.from_logits, self.reduces)
 
 
 @register('losses', 'least_square_generator')
 class LeastSquareGeneratorLoss:
-    def __init__(self, mode: Literal['mean', 'sum', None] = 'mean'):
-        self.mode = mode
+    def __init__(self, from_logits: bool = True, reduces: str | Reduces = 'mean'):
+        self.from_logits = from_logits
+        self.reduces = reduces
 
     def __call__(self, fake: jnp.ndarray):
-        return least_square_generator_loss(fake, self.mode)
+        return least_square_generator_loss(fake, self.from_logits, self.reduces)
 
 
 def relativistic_discriminator_loss(
-        true: jnp.ndarray, fake: jnp.ndarray, mode: Literal['mean', 'sum', None] = 'mean',
+        true: jnp.ndarray, fake: jnp.ndarray, reduces: str | Reduces = 'mean',
         *args, **kwargs
 ):
     true_loss = -jax.nn.log_sigmoid(true - jnp.mean(fake))
     fake_loss = -jax.nn.log_sigmoid(-fake + jnp.mean(true))
 
     loss = true_loss + fake_loss
-    return reduce_fn(loss, mode)
+    return reduce_fn(loss, reduces)
 
 
 def relativistic_generator_loss(
-        true: jnp.ndarray, fake: jnp.ndarray, mode: Literal['mean', 'sum', None] = 'mean',
+        true: jnp.ndarray, fake: jnp.ndarray, reduces: str | Reduces = 'mean',
         *args, **kwargs
 ):
     true_loss = -jax.nn.log_sigmoid(-true + jnp.mean(fake))
     fake_loss = -jax.nn.log_sigmoid(fake - jnp.mean(true))
 
     loss = true_loss + fake_loss
-    return reduce_fn(loss, mode)
+    return reduce_fn(loss, reduces)
 
 
 @register('losses', 'relativistic_discriminator')
 class RelativisticDiscriminatorLoss:
-    def __init__(self, mode: Literal['mean', 'sum', None] = 'mean'):
-        self.mode = mode
+    def __init__(self, reduces: str | Reduces = 'mean'):
+        self.reduces = reduces
 
     def __call__(self, true: jnp.ndarray, fake: jnp.ndarray):
-        return relativistic_discriminator_loss(true, fake, self.mode)
+        return relativistic_discriminator_loss(true, fake, self.reduces)
 
 
 @register('losses', 'relativistic_generator')
 class RelativisticGeneratorLoss:
-    def __init__(self, mode: Literal['mean', 'sum', None] = 'mean'):
-        self.mode = mode
+    def __init__(self, reduces: str | Reduces = 'mean'):
+        self.reduces = reduces
 
     def __call__(self, true: jnp.ndarray, fake: jnp.ndarray):
-        return relativistic_generator_loss(true, fake, self.mode)
+        return relativistic_generator_loss(true, fake, self.reduces)
```

### Comparing `flaxsr-0.0.3a0/flaxsr/losses/perceptual_losses.py` & `flaxsr-0.0.4/flaxsr/losses/perceptual_losses.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal
 
-from flaxsr.losses.utils import reduce_fn
+from flaxsr.losses.utils import reduce_fn, Reduces
 from flaxsr._utils import register
 
 
 Pytree = any
 
 
 def _conv(x: jnp.ndarray, weights: jnp.ndarray, bias: jnp.ndarray):
@@ -48,37 +48,37 @@
     outputs.append(x)
     return outputs
 
 
 @partial(jax.jit, static_argnums=(3, 4, 5,))
 def vgg_loss(
         hr: jnp.ndarray, sr: jnp.ndarray, vgg_params: Pytree,
-        feats_from: Sequence[int], before_act: bool = False, mode: Literal['mean', 'sum', None] = 'mean'
+        feats_from: Sequence[int], before_act: bool = False, reduces: str | Reduces = 'mean'
 ) -> jnp.ndarray:
     hr_feats = _get_feats_from_vgg19(hr, vgg_params, before_act)
     sr_feats = _get_feats_from_vgg19(sr, vgg_params, before_act)
 
     loss = 0.
     for i, (hr_feats, sr_feats) in enumerate(zip(hr_feats, sr_feats)):
         if i in feats_from:
             loss += jnp.mean((hr_feats - sr_feats) ** 2, axis=(1, 2, 3))
-    return reduce_fn(loss, mode)
+    return reduce_fn(loss, reduces)
 
 
 @register('losses', 'vgg')
 class VGGLoss:
     def __init__(
-            self, feats_from: Sequence[int], before_act: bool = False, mode: Literal['mean', 'sum', None] = 'mean'
+            self, feats_from: Sequence[int], before_act: bool = False, reduces: str | Reduces = 'mean'
     ):
         self.feats_from = feats_from
         self.before_act = before_act
-        self.mode = mode
+        self.reduces = reduces
 
     def __call__(self, hr: jnp.ndarray, sr: jnp.ndarray, vgg_params: Pytree) -> jnp.ndarray:
-        return vgg_loss(hr, sr, vgg_params, self.feats_from, self.before_act, self.mode)
+        return vgg_loss(hr, sr, vgg_params, self.feats_from, self.before_act, self.reduces)
 
 
 """
 Maybe Implement Style Loss in the future?
 1. _gram_matrix
 2. style_loss
 3. StyleLoss
```

### Comparing `flaxsr-0.0.3a0/flaxsr/models/edsr.py` & `flaxsr-0.0.4/flaxsr/models/edsr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/flaxsr/models/espcn.py` & `flaxsr-0.0.4/flaxsr/models/espcn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/flaxsr/models/fsrcnn.py` & `flaxsr-0.0.4/flaxsr/models/fsrcnn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/flaxsr/models/nafssr.py` & `flaxsr-0.0.4/flaxsr/models/nafssr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/flaxsr/models/ncnet.py` & `flaxsr-0.0.4/flaxsr/models/ncnet.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/flaxsr/models/srcnn.py` & `flaxsr-0.0.4/flaxsr/models/srcnn.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/flaxsr/models/vdsr.py` & `flaxsr-0.0.4/flaxsr/models/vdsr.py`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/flaxsr/training/train_step.py` & `flaxsr-0.0.4/flaxsr/training/train_step.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,26 +9,42 @@
 import numpy as np
 import einops
 
 from functools import partial
 from typing import Sequence, Literal
 
 from flaxsr._utils import register
-from flaxsr.losses.utils import compute_loss
+
 
 
 @register('train_step', 'discriminative')
 def discriminative_train_step(state: TrainState, batch: Sequence[jnp.ndarray]) -> Sequence:
     if len(batch) == 2:
         lr, hr = batch
     else:
         lr, hr, mask = batch
 
     def loss_fn(params):
         _sr = state.apply_fn(params, lr)
-        _loss = compute_loss(hr, _sr, state.losses, state.reduce, mask if len(batch) == 3 else None)
+        _loss = state.losses(hr, _sr, mask if len(batch) == 3 else None)
         return _loss, _sr
 
     grad_fn = jax.value_and_grad(loss_fn, has_aux=True)
     (loss, sr), grad = grad_fn(state.params)
     state = state.apply_gradients(grads=grad)
     return state, loss
+
+
+# @register('train_step', 'generative')
+# def generative_train_step(state: TrainState, batch: Sequence[jnp.ndarray]) -> Sequence:
+#     if len(batch) == 2:
+#         lr, hr = batch
+#     else:
+#         lr, hr, mask = batch
+#
+#     def loss_fn(params):
+#         _sr = state.apply_fn(params, lr)
+#         _loss = compute_loss(hr, _sr, state.losses, state.reduce, mask if len(batch) == 3 else None)
+#         return _loss, _sr
+#
+#     state = state.apply_gradients(grads=grad)
+#     return state, loss
```

### Comparing `flaxsr-0.0.3a0/flaxsr.egg-info/PKG-INFO` & `flaxsr-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flaxsr
-Version: 0.0.3a0
+Version: 0.0.4
 Summary: Super Resolution models with Jax/Flax
 Home-page: https://github.com/dslisleedh/FlaxSR
 Author: dslisleedh
 Author-email: dslisleedh@gmail.com
 Project-URL: Bug Tracker, https://github.com/dslisleedh/FlaxSR/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
@@ -66,14 +66,49 @@
 # Or you can use flaxsr.get function
 metric = flaxsr.get("losses", "l1", "mean")
 loss_get = metric(hr, sr)
 
 np.allclose(loss, loss_get)
 ```
 
+<b> You can easily load model/losses and train model using custom train_states. </b>
+
+ - Train example
+```python
+import flaxsr
+import jax
+import jax.numpy as jnp
+import numpy as np
+import optax
+
+model_kwargs = {
+    'n_filters': 64, 'n_blocks': 8, 'scale': 4
+}
+model = flaxsr.get("models", "vdsr", **model_kwargs)
+losses = flaxsr.losses.LossWrapper(
+    losses=['l1', 'l2'], weights=[1.0, 1.0]
+)
+params = model.init(jax.random.PRNGKey(0), jnp.ones((1, 8, 8, 3), dtype=jnp.float32))
+tx = optax.adam(1e-3)
+
+state = flaxsr.training.TrainState.create(
+    apply_fn=model.apply, params=params, tx=tx, losses=losses
+)
+
+hr = jnp.ones((1, 32, 32, 3), dtype=jnp.float32)
+lr = jnp.ones((1, 8, 8, 3), dtype=jnp.float32)
+batch = (lr, hr)
+
+state_new, loss = flaxsr.training.discriminative_train_step(state, batch)
+
+assert state_new.step == 1
+np.not_equal(state_new.params['params']['Conv_0']['kernel'], state.params['params']['Conv_0']['kernel'])
+```
+
+
 ## Models implemented
  - SRCNN
  - FSRCNN
  - ESPCN
  - VDSR
  - EDSR, MDSR,
  - NCNet
```

### Comparing `flaxsr-0.0.3a0/flaxsr.egg-info/SOURCES.txt` & `flaxsr-0.0.4/flaxsr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flaxsr-0.0.3a0/setup.py` & `flaxsr-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import setuptools
 
 
 setuptools.setup(
     name="flaxsr",
-    version="0.0.3a",
+    version="0.0.4",
     author="dslisleedh",
     author_email="dslisleedh@gmail.com",
     description="Super Resolution models with Jax/Flax",
     long_description=open('README.md', 'rt').read(),
     long_description_content_type="text/markdown",
     url="https://github.com/dslisleedh/FlaxSR",
     project_urls={
@@ -22,12 +22,13 @@
     ],
     install_requires=[
         "jax",
         "jaxlib",
         "flax",
         "einops",
         "tensorflow",
-        "numpy"
+        "numpy",
+        "optax"
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
 )
```

