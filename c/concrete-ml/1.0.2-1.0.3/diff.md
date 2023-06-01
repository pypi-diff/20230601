# Comparing `tmp/concrete_ml-1.0.2-py3-none-any.whl.zip` & `tmp/concrete_ml-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,58 @@
-Zip file size: 168452 bytes, number of entries: 55
+Zip file size: 178062 bytes, number of entries: 56
 -rw-r--r--  2.0 unx      284 b- defN 80-Jan-01 00:00 concrete/__init__.py
--rw-r--r--  2.0 unx     1722 b- defN 80-Jan-01 00:00 concrete/ml/__init__.py
+-rw-r--r--  2.0 unx       51 b- defN 80-Jan-01 00:00 concrete/ml/__init__.py
 -rw-r--r--  2.0 unx       95 b- defN 80-Jan-01 00:00 concrete/ml/common/__init__.py
 -rw-r--r--  2.0 unx     2519 b- defN 80-Jan-01 00:00 concrete/ml/common/check_inputs.py
 -rw-r--r--  2.0 unx      101 b- defN 80-Jan-01 00:00 concrete/ml/common/debugging/__init__.py
 -rw-r--r--  2.0 unx     2377 b- defN 80-Jan-01 00:00 concrete/ml/common/debugging/custom_assert.py
--rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/__init__.py
--rw-r--r--  2.0 unx     1318 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/dumpers.py
--rw-r--r--  2.0 unx     2018 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/encoder.py
--rw-r--r--  2.0 unx     2888 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/loaders.py
--rw-r--r--  2.0 unx    17217 b- defN 80-Jan-01 00:00 concrete/ml/common/utils.py
+-rw-r--r--  2.0 unx     1221 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/__init__.py
+-rw-r--r--  2.0 unx     8204 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/decoder.py
+-rw-r--r--  2.0 unx      601 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/dumpers.py
+-rw-r--r--  2.0 unx    12166 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/encoder.py
+-rw-r--r--  2.0 unx      743 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/loaders.py
+-rw-r--r--  2.0 unx    18125 b- defN 80-Jan-01 00:00 concrete/ml/common/utils.py
 -rw-r--r--  2.0 unx      235 b- defN 80-Jan-01 00:00 concrete/ml/deployment/Dockerfile.server
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 concrete/ml/deployment/__init__.py
--rw-r--r--  2.0 unx    17843 b- defN 80-Jan-01 00:00 concrete/ml/deployment/deploy_to_aws.py
+-rw-r--r--  2.0 unx    17918 b- defN 80-Jan-01 00:00 concrete/ml/deployment/deploy_to_aws.py
 -rw-r--r--  2.0 unx     3800 b- defN 80-Jan-01 00:00 concrete/ml/deployment/deploy_to_docker.py
--rw-r--r--  2.0 unx    15084 b- defN 80-Jan-01 00:00 concrete/ml/deployment/fhe_client_server.py
+-rw-r--r--  2.0 unx    13873 b- defN 80-Jan-01 00:00 concrete/ml/deployment/fhe_client_server.py
 -rw-r--r--  2.0 unx     2590 b- defN 80-Jan-01 00:00 concrete/ml/deployment/server.py
 -rw-r--r--  2.0 unx       33 b- defN 80-Jan-01 00:00 concrete/ml/deployment/server_requirements.txt
 -rw-r--r--  2.0 unx     3293 b- defN 80-Jan-01 00:00 concrete/ml/deployment/utils.py
 -rw-r--r--  2.0 unx       19 b- defN 80-Jan-01 00:00 concrete/ml/onnx/__init__.py
 -rw-r--r--  2.0 unx     3472 b- defN 80-Jan-01 00:00 concrete/ml/onnx/convert.py
 -rw-r--r--  2.0 unx     9401 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_impl_utils.py
 -rw-r--r--  2.0 unx     9685 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_model_manipulations.py
 -rw-r--r--  2.0 unx    20192 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_utils.py
 -rw-r--r--  2.0 unx    58079 b- defN 80-Jan-01 00:00 concrete/ml/onnx/ops_impl.py
 -rw-r--r--  2.0 unx      101 b- defN 80-Jan-01 00:00 concrete/ml/pytest/__init__.py
--rw-r--r--  2.0 unx    42036 b- defN 80-Jan-01 00:00 concrete/ml/pytest/torch_models.py
--rw-r--r--  2.0 unx     8786 b- defN 80-Jan-01 00:00 concrete/ml/pytest/utils.py
+-rw-r--r--  2.0 unx    43914 b- defN 80-Jan-01 00:00 concrete/ml/pytest/torch_models.py
+-rw-r--r--  2.0 unx    14823 b- defN 80-Jan-01 00:00 concrete/ml/pytest/utils.py
 -rw-r--r--  2.0 unx     1081 b- defN 80-Jan-01 00:00 concrete/ml/quantization/__init__.py
--rw-r--r--  2.0 unx    35262 b- defN 80-Jan-01 00:00 concrete/ml/quantization/base_quantized_op.py
--rw-r--r--  2.0 unx    43525 b- defN 80-Jan-01 00:00 concrete/ml/quantization/post_training.py
--rw-r--r--  2.0 unx    24352 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_module.py
--rw-r--r--  2.0 unx    80991 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_ops.py
--rw-r--r--  2.0 unx    37549 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantizers.py
+-rw-r--r--  2.0 unx    41430 b- defN 80-Jan-01 00:00 concrete/ml/quantization/base_quantized_op.py
+-rw-r--r--  2.0 unx    43710 b- defN 80-Jan-01 00:00 concrete/ml/quantization/post_training.py
+-rw-r--r--  2.0 unx    26450 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_module.py
+-rw-r--r--  2.0 unx    81014 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_ops.py
+-rw-r--r--  2.0 unx    35671 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantizers.py
 -rw-r--r--  2.0 unx       77 b- defN 80-Jan-01 00:00 concrete/ml/search_parameters/__init__.py
 -rw-r--r--  2.0 unx    21193 b- defN 80-Jan-01 00:00 concrete/ml/search_parameters/p_error_search.py
 -rw-r--r--  2.0 unx     4679 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/__init__.py
--rw-r--r--  2.0 unx    62708 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/base.py
--rw-r--r--  2.0 unx    13633 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/glm.py
--rw-r--r--  2.0 unx    25212 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/linear_model.py
--rw-r--r--  2.0 unx    13342 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/qnn.py
--rw-r--r--  2.0 unx    12572 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/qnn_module.py
--rw-r--r--  2.0 unx    12243 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/rf.py
--rw-r--r--  2.0 unx    10614 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/svm.py
--rw-r--r--  2.0 unx    10394 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/tree.py
+-rw-r--r--  2.0 unx    64073 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/base.py
+-rw-r--r--  2.0 unx    12899 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/glm.py
+-rw-r--r--  2.0 unx    21814 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/linear_model.py
+-rw-r--r--  2.0 unx    32152 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/qnn.py
+-rw-r--r--  2.0 unx    12803 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/qnn_module.py
+-rw-r--r--  2.0 unx    11043 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/rf.py
+-rw-r--r--  2.0 unx     9155 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/svm.py
+-rw-r--r--  2.0 unx     9191 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/tree.py
 -rw-r--r--  2.0 unx    10923 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/tree_to_numpy.py
--rw-r--r--  2.0 unx    20074 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/xgb.py
+-rw-r--r--  2.0 unx    18962 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/xgb.py
 -rw-r--r--  2.0 unx       83 b- defN 80-Jan-01 00:00 concrete/ml/torch/__init__.py
--rw-r--r--  2.0 unx    17531 b- defN 80-Jan-01 00:00 concrete/ml/torch/compile.py
+-rw-r--r--  2.0 unx    19083 b- defN 80-Jan-01 00:00 concrete/ml/torch/compile.py
 -rw-r--r--  2.0 unx     3174 b- defN 80-Jan-01 00:00 concrete/ml/torch/numpy_module.py
 -rw-r--r--  2.0 unx      124 b- defN 80-Jan-01 00:00 concrete/ml/version.py
--rw-r--r--  2.0 unx     1546 b- defN 80-Jan-01 00:00 concrete_ml-1.0.2.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 concrete_ml-1.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11617 b- defN 16-Jan-01 00:00 concrete_ml-1.0.2.dist-info/METADATA
-?rw-r--r--  2.0 unx     4967 b- defN 16-Jan-01 00:00 concrete_ml-1.0.2.dist-info/RECORD
-55 files, 704863 bytes uncompressed, 160484 bytes compressed:  77.2%
+-rw-r--r--  2.0 unx     1546 b- defN 80-Jan-01 00:00 concrete_ml-1.0.3.dist-info/LICENSE
+?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 concrete_ml-1.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11617 b- defN 16-Jan-01 00:00 concrete_ml-1.0.3.dist-info/METADATA
+?rw-r--r--  2.0 unx     5066 b- defN 16-Jan-01 00:00 concrete_ml-1.0.3.dist-info/RECORD
+56 files, 747137 bytes uncompressed, 169932 bytes compressed:  77.3%
```

## zipnote {}

```diff
@@ -15,14 +15,17 @@
 
 Filename: concrete/ml/common/debugging/custom_assert.py
 Comment: 
 
 Filename: concrete/ml/common/serialization/__init__.py
 Comment: 
 
+Filename: concrete/ml/common/serialization/decoder.py
+Comment: 
+
 Filename: concrete/ml/common/serialization/dumpers.py
 Comment: 
 
 Filename: concrete/ml/common/serialization/encoder.py
 Comment: 
 
 Filename: concrete/ml/common/serialization/loaders.py
@@ -147,20 +150,20 @@
 
 Filename: concrete/ml/torch/numpy_module.py
 Comment: 
 
 Filename: concrete/ml/version.py
 Comment: 
 
-Filename: concrete_ml-1.0.2.dist-info/LICENSE
+Filename: concrete_ml-1.0.3.dist-info/LICENSE
 Comment: 
 
-Filename: concrete_ml-1.0.2.dist-info/WHEEL
+Filename: concrete_ml-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: concrete_ml-1.0.2.dist-info/METADATA
+Filename: concrete_ml-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: concrete_ml-1.0.2.dist-info/RECORD
+Filename: concrete_ml-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concrete/ml/__init__.py

```diff
@@ -1,48 +1,3 @@
 """ML module."""
-import os
 
 from .version import __version__
-
-# If the use of skops needs to be disabled.
-# This could be useful when loading a model with Python 3.7 with a higher version
-USE_SKOPS = int(os.environ.get("USE_SKOPS", 1))
-
-# These are all the trusted types that are considered by skops
-TRUSTED_SKOPS = [
-    "numpy.int64",
-    "numpy.float64",
-    "numpy.int32",
-    "xgboost.core.Booster",
-    "xgboost.sklearn.XGBClassifier",
-    "xgboost.sklearn.XGBRegressor",
-    "sklearn._loss.glm_distribution.DistributionBoundary",
-    "sklearn._loss.glm_distribution.TweedieDistribution",
-    "sklearn._loss.glm_distribution.GammaDistribution",
-    "sklearn._loss.glm_distribution.PoissonDistribution",
-    "sklearn.linear_model._glm.link.LogLink",
-    "sklearn.linear_model._glm.link.IdentityLink",
-    "sklearn._loss.link.IdentityLink",
-    "sklearn._loss.link.Interval",
-    "sklearn._loss.link.LogLink",
-    "sklearn._loss.link.LogLink",
-    "sklearn._loss._loss.CyHalfTweedieLossIdentity",
-    "sklearn._loss.loss.HalfTweedieLossIdentity",
-    "sklearn._loss._loss.CyHalfPoissonLoss",
-    "sklearn._loss.loss.HalfPoissonLoss",
-    "sklearn._loss._loss.CyHalfGammaLoss",
-    "sklearn._loss.loss.HalfGammaLoss",
-    "sklearn._loss._loss.CyHalfTweedieLoss",
-    "sklearn._loss.loss.HalfTweedieLoss",
-]
-
-# If USE_SKOPS is False or skops can't be imported we default to pickle
-try:
-    if USE_SKOPS:
-        from skops.io import dumps as dumps_sklearn
-        from skops.io import loads as loads_sklearn
-    else:  # pragma: no cover
-        raise ImportError()
-except ImportError:  # pragma: no cover
-    USE_SKOPS = False
-    from pickle import dumps as dumps_sklearn
-    from pickle import loads as loads_sklearn
```

## concrete/ml/common/serialization/__init__.py

```diff
@@ -0,0 +1,77 @@
+00000000: 2222 2253 6572 6961 6c69 7a61 7469 6f6e  """Serialization
+00000010: 206d 6f64 756c 652e 2222 220a 696d 706f   module.""".impo
+00000020: 7274 206f 730a 0a66 726f 6d20 746f 7263  rt os..from torc
+00000030: 682e 6e6e 2e6d 6f64 756c 6573 2069 6d70  h.nn.modules imp
+00000040: 6f72 7420 6163 7469 7661 7469 6f6e 0a0a  ort activation..
+00000050: 2320 4966 2074 6865 2075 7365 206f 6620  # If the use of 
+00000060: 536b 6f70 7320 6e65 6564 7320 746f 2062  Skops needs to b
+00000070: 6520 6469 7361 626c 6564 2e0a 5553 455f  e disabled..USE_
+00000080: 534b 4f50 5320 3d20 626f 6f6c 286f 732e  SKOPS = bool(os.
+00000090: 656e 7669 726f 6e2e 6765 7428 2255 5345  environ.get("USE
+000000a0: 5f53 4b4f 5053 222c 2031 2929 0a0a 2320  _SKOPS", 1))..# 
+000000b0: 4465 6669 6e65 2061 6c6c 2063 7572 7265  Define all curre
+000000c0: 6e74 6c79 2073 7570 706f 7274 6564 2054  ntly supported T
+000000d0: 6f72 6368 2061 6374 6976 6174 696f 6e20  orch activation 
+000000e0: 6675 6e63 7469 6f6e 730a 5355 5050 4f52  functions.SUPPOR
+000000f0: 5445 445f 544f 5243 485f 4143 5449 5641  TED_TORCH_ACTIVA
+00000100: 5449 4f4e 5320 3d20 5b0a 2020 2020 6163  TIONS = [.    ac
+00000110: 7469 7661 7469 6f6e 2e43 454c 552c 0a20  tivation.CELU,. 
+00000120: 2020 2061 6374 6976 6174 696f 6e2e 454c     activation.EL
+00000130: 552c 0a20 2020 2061 6374 6976 6174 696f  U,.    activatio
+00000140: 6e2e 4745 4c55 2c0a 2020 2020 6163 7469  n.GELU,.    acti
+00000150: 7661 7469 6f6e 2e48 6172 6473 6872 696e  vation.Hardshrin
+00000160: 6b2c 0a20 2020 2061 6374 6976 6174 696f  k,.    activatio
+00000170: 6e2e 4861 7264 7369 676d 6f69 642c 0a20  n.Hardsigmoid,. 
+00000180: 2020 2061 6374 6976 6174 696f 6e2e 4861     activation.Ha
+00000190: 7264 7377 6973 682c 0a20 2020 2061 6374  rdswish,.    act
+000001a0: 6976 6174 696f 6e2e 4861 7264 7461 6e68  ivation.Hardtanh
+000001b0: 2c0a 2020 2020 6163 7469 7661 7469 6f6e  ,.    activation
+000001c0: 2e4c 6561 6b79 5265 4c55 2c0a 2020 2020  .LeakyReLU,.    
+000001d0: 6163 7469 7661 7469 6f6e 2e4c 6f67 5369  activation.LogSi
+000001e0: 676d 6f69 642c 0a20 2020 2061 6374 6976  gmoid,.    activ
+000001f0: 6174 696f 6e2e 4c6f 6753 6f66 746d 6178  ation.LogSoftmax
+00000200: 2c0a 2020 2020 6163 7469 7661 7469 6f6e  ,.    activation
+00000210: 2e4d 6973 682c 0a20 2020 2061 6374 6976  .Mish,.    activ
+00000220: 6174 696f 6e2e 5052 654c 552c 0a20 2020  ation.PReLU,.   
+00000230: 2061 6374 6976 6174 696f 6e2e 5265 4c55   activation.ReLU
+00000240: 2c0a 2020 2020 6163 7469 7661 7469 6f6e  ,.    activation
+00000250: 2e52 654c 5536 2c0a 2020 2020 6163 7469  .ReLU6,.    acti
+00000260: 7661 7469 6f6e 2e53 454c 552c 0a20 2020  vation.SELU,.   
+00000270: 2061 6374 6976 6174 696f 6e2e 5369 4c55   activation.SiLU
+00000280: 2c0a 2020 2020 6163 7469 7661 7469 6f6e  ,.    activation
+00000290: 2e53 6967 6d6f 6964 2c0a 2020 2020 6163  .Sigmoid,.    ac
+000002a0: 7469 7661 7469 6f6e 2e53 6f66 746d 696e  tivation.Softmin
+000002b0: 2c0a 2020 2020 6163 7469 7661 7469 6f6e  ,.    activation
+000002c0: 2e53 6f66 7470 6c75 732c 0a20 2020 2061  .Softplus,.    a
+000002d0: 6374 6976 6174 696f 6e2e 536f 6674 7368  ctivation.Softsh
+000002e0: 7269 6e6b 2c0a 2020 2020 6163 7469 7661  rink,.    activa
+000002f0: 7469 6f6e 2e53 6f66 7473 6967 6e2c 0a20  tion.Softsign,. 
+00000300: 2020 2061 6374 6976 6174 696f 6e2e 5461     activation.Ta
+00000310: 6e68 2c0a 2020 2020 6163 7469 7661 7469  nh,.    activati
+00000320: 6f6e 2e54 616e 6873 6872 696e 6b2c 0a20  on.Tanhshrink,. 
+00000330: 2020 2061 6374 6976 6174 696f 6e2e 5468     activation.Th
+00000340: 7265 7368 6f6c 642c 0a5d 0a0a 2320 536f  reshold,.]..# So
+00000350: 6d65 2054 6f72 6368 2061 6374 6976 6174  me Torch activat
+00000360: 696f 6e20 6675 6e63 7469 6f6e 7320 6172  ion functions ar
+00000370: 6520 6375 7272 656e 746c 7920 6e6f 7420  e currently not 
+00000380: 7375 7070 6f72 7465 6420 696e 2043 6f6e  supported in Con
+00000390: 6372 6574 6520 4d4c 0a23 2046 4958 4d45  crete ML.# FIXME
+000003a0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+000003b0: 2e63 6f6d 2f7a 616d 612d 6169 2f63 6f6e  .com/zama-ai/con
+000003c0: 6372 6574 652d 6d6c 2d69 6e74 6572 6e61  crete-ml-interna
+000003d0: 6c2f 6973 7375 6573 2f33 3335 0a23 2046  l/issues/335.# F
+000003e0: 4958 4d45 3a20 6874 7470 733a 2f2f 6769  IXME: https://gi
+000003f0: 7468 7562 2e63 6f6d 2f7a 616d 612d 6169  thub.com/zama-ai
+00000400: 2f63 6f6e 6372 6574 652d 6d6c 2d69 6e74  /concrete-ml-int
+00000410: 6572 6e61 6c2f 6973 7375 6573 2f33 3531  ernal/issues/351
+00000420: 380a 554e 5355 5050 4f52 5445 445f 544f  8.UNSUPPORTED_TO
+00000430: 5243 485f 4143 5449 5641 5449 4f4e 5320  RCH_ACTIVATIONS 
+00000440: 3d20 5b0a 2020 2020 6163 7469 7661 7469  = [.    activati
+00000450: 6f6e 2e47 4c55 2c0a 2020 2020 6163 7469  on.GLU,.    acti
+00000460: 7661 7469 6f6e 2e4d 756c 7469 6865 6164  vation.Multihead
+00000470: 4174 7465 6e74 696f 6e2c 0a20 2020 2061  Attention,.    a
+00000480: 6374 6976 6174 696f 6e2e 5252 654c 552c  ctivation.RReLU,
+00000490: 0a20 2020 2061 6374 6976 6174 696f 6e2e  .    activation.
+000004a0: 536f 6674 6d61 782c 0a20 2020 2061 6374  Softmax,.    act
+000004b0: 6976 6174 696f 6e2e 536f 6674 6d61 7832  ivation.Softmax2
+000004c0: 642c 0a5d 0a                             d,.].
```

## concrete/ml/common/serialization/dumpers.py

```diff
@@ -1,53 +1,28 @@
 """Dump functions for serialization."""
 import json
-from typing import Any, TextIO, Union
+from typing import Any, TextIO
 
-from numpy.random import RandomState
+from .encoder import ConcreteEncoder
 
-# pylint: disable=relative-beyond-top-level
-from .encoder import CustomEncoder
 
-
-def dumps_random_state(random_state: Union[RandomState, int, None]) -> str:
-    """Dump random state to string.
+def dumps(obj: Any) -> str:
+    """Dump any object as a string.
 
     Arguments:
-        random_state (Union[RandomState, int, None]): a random state
+        obj (Any): Object to dump.
 
     Returns:
-        str: a serialized version of the random state
+        str: A string representation of the object.
     """
 
-    if isinstance(random_state, int):
-        return str(random_state)
-    if random_state is None:
-        return "null"
-    return json.dumps(random_state.get_state(), cls=CustomEncoder)
+    return json.dumps(obj, cls=ConcreteEncoder)
 
 
 def dump(obj: Any, file: TextIO):
-    """Dump any Concrete ML object that has a dump method.
+    """Dump any Concrete ML object in a file.
 
     Arguments:
-        obj (Any): the object to dump.
-        file (TextIO): a file containing the serialized object.
+        obj (Any): The object to dump.
+        file (TextIO): The file to dump the serialized object into.
     """
     file.write(dumps(obj))
-
-
-def dumps(obj: Any) -> str:
-    """Dump as string any object.
-
-    If the object has some `dumps` method then it uses that.
-    Otherwise the object is casted as `str`.
-
-    Arguments:
-        obj (Any): any object.
-
-    Returns:
-        str: a string representation of the object.
-    """
-
-    if hasattr(obj, "dumps"):
-        return obj.dumps()
-    return json.dumps(obj, cls=CustomEncoder)
```

## concrete/ml/common/serialization/encoder.py

```diff
@@ -1,75 +1,275 @@
 """Custom encoder for serialization."""
+import inspect
 import json
-from typing import Any
+from json.encoder import _make_iterencode  # type: ignore[attr-defined]
+from json.encoder import encode_basestring  # type: ignore[attr-defined]
+from json.encoder import encode_basestring_ascii  # type: ignore[attr-defined]
+from json.encoder import INFINITY, JSONEncoder
+from typing import Any, Callable, Dict, Generator, Type
 
 import numpy
 import onnx
 import sklearn
+import torch
 from numpy.random import RandomState
+from skorch.dataset import ValidSplit
 
 from concrete import fhe
 
-from ... import dumps_sklearn
+from . import USE_SKOPS
 
+# If USE_SKOPS is False or Skops can't be imported, default to pickle
+try:
+    if USE_SKOPS:
+        from skops.io import dumps as pickle_or_skops_dumps
+    else:  # pragma: no cover
+        raise ImportError()
+except ImportError:  # pragma: no cover
+    USE_SKOPS = False
+    from pickle import dumps as pickle_or_skops_dumps
+
+
+def dump_name_and_value(name: str, value: Any, **kwargs) -> Dict:
+    """Dump the value into a custom dict format.
+
+    Args:
+        name (str): The custom name to use. This name should be unique for each type to encode, as
+            it is used in the ConcreteDecoder class to detect the initial type and apply the proper
+            load method to the serialized object.
+        value (Any): The serialized value to dump.
+        **kwargs (dict): Additional arguments to dump.
 
-# Register all models
-class CustomEncoder(json.JSONEncoder):
-    """CustomEncoder: custom json encoder to handle non-native types."""
+    Returns:
+        Dict: The serialized custom format that includes both the serialized value and its type
+            name.
+    """
+    name_and_value = {
+        "type_name": name,
+        "serialized_value": value,
+    }
+
+    assert "type_name" not in kwargs and "serialized_value" not in kwargs
+
+    name_and_value.update(kwargs)
+    return name_and_value
+
+
+class ConcreteEncoder(JSONEncoder):
+    """Custom json encoder to handle non-native types found in serialized Concrete ML objects.
+
+    Non-native types are serialized manually and dumped in a custom dict format that stores both the
+    serialization value of the object and its associated type name.
+
+    The name should be unique for each type, as it is used in the ConcreteDecoder class to detect
+    the initial type and apply the proper load method to the serialized object. The serialized
+    value is the value that was serialized manually in a native type. Additional arguments such
+    as a numpy array's dtype are also properly serialized. If an object has an unexpected type or
+    is not serializable, an error is thrown.
+
+    The ConcreteEncoder is only meant to encode Concrete-ML's built-in models and therefore only
+    supports the necessary types. For example, torch.Tensor objects are not serializable using this
+    encoder as built-in models only use numpy arrays. However, the list of supported types might
+    expand in future releases if new models are added and need new types.
+    """
+
+    @staticmethod
+    def isinstance(o: Any, cls: Type) -> bool:
+        """Define a custom isinstance method.
+
+        Natively, among other types, the JSONENcoder handles integers, floating points and tuples.
+        However, a numpy.integer (resp. numpy.floating) object is automatically casted to a built-in
+        int (resp. float) object, without keeping their dtype information. Similarly, a tuple is
+        casted to a list, meaning that it will then be loaded as a list, which notably does not have
+        the uniqueness property and therefore might cause issues in complex structures such as
+        QuantizedModule instances. This is an issue as JSONEncoder only calls its customizable
+        `default` method at the end of the parsing. We thus need to provide this custom isinstance
+        method in order to make the encoder avoid handling these specific types until `default` is
+        reached (where they are properly serialized using our custom format).
+
+        Args:
+            o (Any): The object to serialize.
+            cls (Type): The type to compare the object with.
+
+        Returns:
+            bool: If the object is of the given type. False if it is a numpy.floating, numpy.integer
+                or a tuple.
+        """
+        if isinstance(o, numpy.floating):
+            return False
+
+        if isinstance(o, numpy.integer):
+            return False
+
+        if isinstance(o, tuple):
+            return False
+
+        return isinstance(o, cls)
+
+    # Coverage is disabled many times in the following method as it is a slightly modified version
+    # of JSONEncoder's iterencode and thus should not be fully tested
+    def iterencode(self, o: Any, _one_shot: bool = False) -> Generator:
+        """Encode the given object and yield each string representation as available.
+
+        This method overrides the JSONEncoder's native iterencode one in order to pass our custom
+        isinstance method to the `_make_iterencode` function. More information in `isinstance`'s
+        docstring. For simplicity, iterencode does not give the ability to use the initial
+        `c_make_encoder` function, as it would required to override it in C.
+
+        Args:
+            o (Any): The object to serialize.
+            _one_shot (bool): This parameter is not used since the `_make_iterencode` function has
+                been removed from the method.
 
-    # pylint: disable-next=too-many-return-statements
+        Returns:
+            Generator: Yield each string representation as available.
+        """
+        if self.check_circular:
+            markers = {}  # type: ignore[var-annotated]
+        else:
+            markers = None  # pragma: no cover
+        if self.ensure_ascii:
+            _encoder = encode_basestring_ascii
+        else:
+            _encoder = encode_basestring  # pragma: no cover
+
+        def floatstr(
+            o, allow_nan=self.allow_nan, _repr=float.__repr__, _inf=INFINITY, _neginf=-INFINITY
+        ):
+            # Check for specials.  Note that this type of test is processor
+            # and/or platform-specific, so do tests which don't depend on the
+            # internals.
+
+            # pylint: disable-next=comparison-with-itself
+            if o != o:
+                text = "NaN"
+            elif o == _inf:
+                text = "Infinity"  # pragma: no cover
+            elif o == _neginf:
+                text = "-Infinity"  # pragma: no cover
+            else:
+                return _repr(o)
+
+            if not allow_nan:
+                raise ValueError(  # pragma: no cover
+                    "Out of range float values are not JSON compliant: " + repr(o)
+                )
+
+            return text
+
+        # Force `_make_iterencode` to use our custom `isinstance` method
+        _iterencode = _make_iterencode(
+            markers,
+            self.default,
+            _encoder,
+            self.indent,
+            floatstr,
+            self.key_separator,
+            self.item_separator,
+            self.sort_keys,
+            self.skipkeys,
+            False,
+            isinstance=self.isinstance,
+        )
+        return _iterencode(o, 0)
+
+    # pylint: disable-next=too-many-return-statements, too-many-branches
     def default(self, o: Any) -> Any:
-        """Overload default serialization.
+        """Define a custom default method that enables dumping any supported serialized values.
 
         Arguments:
-            o (Any): the object to serialize.
+            o (Any): The object to serialize.
 
         Returns:
-            The serialized object.
+            Any: The serialized object. Non-native types are returned as a dict of a specific
+                format.
 
         Raises:
-            NotImplementedError: if a fhe.Circuit is given.
+            NotImplementedError: If a fhe.Circuit, a Callable or a Generator object is given.
         """
 
-        # Use __getstate__, __setstate__ if RandomState, either easy
+        # Serializing a Circuit object is currently not supported
+        # FIXME: https://github.com/zama-ai/concrete-numpy-internal/issues/1841
+        if isinstance(o, fhe.Circuit):
+            raise NotImplementedError("Concrete Circuit object serialization is not implemented.")
+
         if isinstance(o, RandomState):
-            return o.get_state()
+            return dump_name_and_value("RandomState", o.get_state())
 
-        if isinstance(o, sklearn.base.BaseEstimator):
-            return dumps_sklearn(o).hex()
+        # scikit-learn does not provide a particular dumping/loading method. We thus need to dump
+        # these models using either Skops or pickle as a hexadecimal byte string. Additionally,
+        # Concrete ML models, which currently inherit from scikit-learn models, have their own
+        # serialization methods. We therefore make sure that they do not get serialized here
+        if isinstance(o, sklearn.base.BaseEstimator) and not hasattr(o, "_is_a_public_cml_model"):
+            return dump_name_and_value("sklearn_model", pickle_or_skops_dumps(o).hex())
 
         if isinstance(o, onnx.ModelProto):
-            return dumps_onnx(o)
+            return dump_name_and_value("onnx_model", o.SerializeToString().hex())
 
+        # The list is sorted before being serialized in order to be able to properly compare two
+        # JSON strings, as sets do not have any order notion but lists do.
+        if isinstance(o, set):
+            return dump_name_and_value("set", sorted(list(o)))
+
+        if isinstance(o, tuple):
+            return dump_name_and_value("tuple", list(o))
+
+        # Dump the numpy integer value along its dtype
         if isinstance(o, numpy.integer):
-            return int(o)
+            kwargs = {"dtype": str(o.dtype)}
+            return dump_name_and_value("numpy_integer", int(o), **kwargs)
 
-        if isinstance(o, type):
-            return o.__name__
+        # Dump the numpy float value along its dtype
+        if isinstance(o, numpy.floating):
+            kwargs = {"dtype": str(o.dtype)}
+            return dump_name_and_value("numpy_float", float(o), **kwargs)
 
-        # Match all the types you want to handle in your converter
+        # Dump the numpy array along its dtype
         if isinstance(o, numpy.ndarray):
-            return o.tolist()
-
-        if hasattr(o, "dump_dict"):
-            return o.dump_dict()
+            kwargs = {"dtype": str(o.dtype)}
+            return dump_name_and_value("numpy_array", o.tolist(), **kwargs)
 
-        # FIXME: https://github.com/zama-ai/concrete-numpy-internal/issues/1841
-        if isinstance(o, fhe.Circuit):  # pragma: no cover
-            raise NotImplementedError(
-                "Concrete Circuit object serialization is not implemented yet"
-            )
+        # This specific type is widely used in QuantizedModule instances and therefore is treated
+        # separately
+        # pylint: disable-next=protected-access
+        if o is inspect._empty:
+            return dump_name_and_value("inspect_empty", "inspect._empty")
+
+        # Ideally, serializing type objects should be avoided as it either requires to import all
+        # supported types when loading or specify each trusted object to Skops, which can become
+        # very exhaustive. However, QNNs still provide few type objects (mostly coming from skorch)
+        if isinstance(o, type):
+            return dump_name_and_value("type", pickle_or_skops_dumps(o).hex())
 
-        # Call the default method for other types
-        return json.JSONEncoder.default(self, o)  # pragma: no cover
+        if isinstance(o, torch.device):
+            return dump_name_and_value("torch_device", str(o))
 
+        # A ValidSplit instance is used by default when initializing a QNN but skorch does not
+        # provide any simple ways for serializing it. Since this such an instance is used by
+        # default, ValidSplit instances are treated manually as well. However, this does not work
+        # if the cross-validation strategy is set using a Generator object (see below)
+        if isinstance(o, ValidSplit):
+            if isinstance(o.cv, Generator):
+                raise NotImplementedError(
+                    "Serializing a custom Generator object is not secure and is therefore "
+                    "disabled. Please choose a different cross-validation splitting strategy."
+                )
+            return dump_name_and_value("valid_split", vars(o))
 
-def dumps_onnx(onnx_model: onnx.ModelProto) -> str:
-    """Dump onnx model as string.
+        # All serializable classes from Concrete ML provide a `dump_dict` method that serializes
+        # their attributes
+        if hasattr(o, "dump_dict"):
+            return dump_name_and_value(type(o).__name__, o.dump_dict())
 
-    Arguments:
-        onnx_model (onnx.ModelProto): an onnx model.
+        # Serializing Callable and Generator objects is disabled as it cannot be done securely. More
+        # precisely, anyone could modify the json file after dumping such object and therefore make
+        # the JSONDecoder load any undesired function
+        # Disable mypy as running isinstance with a Callable type unexpectedly raises an issue:
+        # https://github.com/python/mypy/issues/3060
+        if isinstance(o, (Callable, Generator)):  # type: ignore[arg-type]
+            raise NotImplementedError(
+                "Serializing a custom Callable or Generator object is not secure and is therefore "
+                f"disabled. Got {str(o)}."
+            )
 
-    Returns:
-        str: a serialized version of the onnx model.
-    """
-    return onnx_model.SerializeToString().hex()
+        # Call the default method for other native types (e.g., dict, str, bool, ...)
+        return json.JSONEncoder.default(self, o)
```

## concrete/ml/common/serialization/loaders.py

```diff
@@ -1,104 +1,30 @@
 """Load functions for serialization."""
 import json
-from typing import Any, Callable, Dict, TextIO, Union
+from typing import IO, Any, Union
 
-import onnx
-from numpy.random import RandomState
+from .decoder import ConcreteDecoder
 
-# pylint: disable=relative-beyond-top-level
-from ...quantization.quantizers import QuantizedArray, UniformQuantizer
-from ...sklearn.base import _ALL_SKLEARN_MODELS
 
-# pylint: disable=invalid-name
-LOADS_METHODS: Dict[str, Callable] = {}
-
-
-def load_dict(metadata: Dict[str, Any]) -> Any:
-    """Load any Concrete ML object that has a dump method.
-
-    Arguments:
-        metadata (Dict[str, Any]): a dict of a serialized object.
-
-    Returns:
-        Any: the object itself.
-
-    Raises:
-        ValueError: if "cml_dumped_class_name" key is not in the serialized object.
-    """
-    # pylint: disable-next=global-statement
-    global LOADS_METHODS
-    if not LOADS_METHODS:
-        LOADS_METHODS = {
-            model_class.__name__: model_class.load_dict
-            for model_class in _ALL_SKLEARN_MODELS
-            if hasattr(model_class, "load_dict")
-        }
-        LOADS_METHODS["QuantizedArray"] = QuantizedArray.load_dict
-        LOADS_METHODS["UniformQuantizer"] = UniformQuantizer.load_dict
-
-    try:
-        class_name = metadata["cml_dumped_class_name"]
-    except KeyError as exception:
-        raise ValueError("The content provided is not a Concrete ML dumped model.") from exception
-
-    return LOADS_METHODS[class_name](metadata)
-
-
-def loads(content: str) -> Any:
-    """Load any Concrete ML object that has a dump method.
+def loads(content: Union[str, bytes]) -> Any:
+    """Load any Concrete ML object that provide a `dump_dict` method.
 
     Arguments:
-        content (str): a serialized object.
+        content (Union[str, bytes]): A serialized object.
 
     Returns:
-        Any: the object itself.
+        Any: The object itself.
     """
-    parsed = json.loads(content)
-    return load_dict(parsed)
+    return json.loads(content, cls=ConcreteDecoder)
 
 
-def load(file: TextIO):
-    """Load any Concrete ML object that has a dump method.
+def load(file: Union[IO[str], IO[bytes]]):
+    """Load any Concrete ML object that provide a `load_dict` method.
 
     Arguments:
-        file (TextIO): a file containing the serialized object.
+        file (Union[IO[str], IO[bytes]): The file containing the serialized object.
 
     Returns:
-        Any: the object itself.
+        Any: The object itself.
     """
     content = file.read()
     return loads(content)
-
-
-def loads_onnx(serialized_onnx: str) -> onnx.ModelProto:
-    """Load serialized onnx model.
-
-    Arguments:
-        serialized_onnx (str): a serialized onnx model.
-
-    Returns:
-        onnx.ModelProto: the onnx model
-    """
-
-    return onnx.load_model_from_string(bytes.fromhex(serialized_onnx))
-
-
-def loads_random_state(serialized_random_state: str) -> Union[RandomState, int, None]:
-    """Load random state from string.
-
-    Arguments:
-        serialized_random_state (str): a serialized version of the random state
-
-    Returns:
-        random_state (Union[RandomState, int, None]): a random state
-
-
-    """
-    deserialized = json.loads(serialized_random_state)
-    if isinstance(deserialized, int) or (deserialized is None):
-        return deserialized
-    assert isinstance(deserialized, list)
-    deserialized = tuple(deserialized)
-    random_state = RandomState()
-    random_state.set_state(deserialized)
-    return random_state
```

## concrete/ml/common/utils.py

```diff
@@ -26,14 +26,16 @@
 SUPPORTED_INT_TYPES = {
     "int64": torch.int64,
     "int32": torch.int32,
     "int16": torch.int16,
     "int8": torch.int8,
 }
 
+SUPPORTED_TYPES = {**SUPPORTED_FLOAT_TYPES, **SUPPORTED_INT_TYPES}
+
 MAX_BITWIDTH_BACKWARD_COMPATIBLE = 8
 
 
 class FheMode(str, enum.Enum):
     """Enum representing the execution mode.
 
     This enum inherits from str in order to be able to easily compare a string parameter to its
@@ -512,30 +514,58 @@
     if not isinstance(x, tuple):
         return (x,)
 
     return x
 
 
 def all_values_are_integers(*values: Any) -> bool:
-    """Indicate that all unpacked values are of a supported integer dtype.
+    """Indicate if all unpacked values are of a supported integer dtype.
 
     Args:
         *values (Any): The values to consider.
 
     Returns:
         bool: Whether all values are supported integers or not.
 
     """
     return all(_is_of_dtype(value, SUPPORTED_INT_TYPES) for value in values)
 
 
 def all_values_are_floats(*values: Any) -> bool:
-    """Indicate that all unpacked values are of a supported float dtype.
+    """Indicate if all unpacked values are of a supported float dtype.
 
     Args:
         *values (Any): The values to consider.
 
     Returns:
         bool: Whether all values are supported floating points or not.
 
     """
     return all(_is_of_dtype(value, SUPPORTED_FLOAT_TYPES) for value in values)
+
+
+def all_values_are_of_dtype(*values: Any, dtypes: Union[str, List[str]]) -> bool:
+    """Indicate if all unpacked values are of the specified dtype(s).
+
+    Args:
+        *values (Any): The values to consider.
+        dtypes (Union[str, List[str]]): The dtype(s) to consider.
+
+    Returns:
+        bool: Whether all values are of the specified dtype(s) or not.
+
+    """
+    if isinstance(dtypes, str):
+        dtypes = [dtypes]
+
+    supported_dtypes = {}
+    for dtype in dtypes:
+        supported_dtype = SUPPORTED_TYPES.get(dtype, None)
+
+        assert supported_dtype is not None, (
+            f"The given dtype is not supported. Expected one of {SUPPORTED_TYPES.keys()}, "
+            f"got {dtype}."
+        )
+
+        supported_dtypes[dtype] = supported_dtype
+
+    return all(_is_of_dtype(value, supported_dtypes) for value in values)
```

## concrete/ml/deployment/deploy_to_aws.py

```diff
@@ -10,14 +10,15 @@
 It then launches the server.
 """
 
 import argparse
 import json
 import subprocess
 import time
+import uuid
 import zipfile
 from contextlib import closing
 from datetime import datetime
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 import boto3
@@ -122,15 +123,19 @@
     """
     open_port = int(open_port)
 
     # Create client/resource objects
     with closing(boto3.client("ec2", region_name=region_name)) as client:
         resources = boto3.resource("ec2", region_name=region_name)
         str_now = datetime.now().strftime(DATE_FORMAT)
-        name = f"deploy-cml-{str_now}" if instance_name is None else f"{instance_name}-{str_now}"
+        name = (
+            f"deploy-cml-{str_now}-{uuid.uuid4()}"
+            if instance_name is None
+            else f"{instance_name}-{str_now}"
+        )
 
         # Get VPC
         vpc_id: str = client.describe_vpcs().get("Vpcs", [{}])[0].get("VpcId", "")
         # OPTION 1: get fist vpc available
         if vpc_id:
             vpc = resources.Vpc(vpc_id)
         # OPTION 2: create VPC (not possible if too many VPCs)
```

## concrete/ml/deployment/fhe_client_server.py

```diff
@@ -7,62 +7,18 @@
 from typing import Any, Optional
 
 import numpy
 
 from concrete import fhe
 
 from ..common.debugging.custom_assert import assert_true
-from ..common.serialization.encoder import CustomEncoder
-from ..common.serialization.loaders import load_dict
-from ..quantization.quantized_module import QuantizedModule
-from ..sklearn import (
-    DecisionTreeClassifier,
-    DecisionTreeRegressor,
-    ElasticNet,
-    GammaRegressor,
-    Lasso,
-    LinearRegression,
-    LinearSVC,
-    LinearSVR,
-    LogisticRegression,
-    NeuralNetClassifier,
-    NeuralNetRegressor,
-    PoissonRegressor,
-    RandomForestClassifier,
-    RandomForestRegressor,
-    Ridge,
-    TweedieRegressor,
-    XGBClassifier,
-    XGBRegressor,
-)
+from ..common.serialization.dumpers import dump
+from ..common.serialization.loaders import load
 from ..version import __version__ as CML_VERSION
 
-AVAILABLE_MODEL = [
-    RandomForestClassifier,
-    RandomForestRegressor,
-    XGBClassifier,
-    XGBRegressor,
-    LinearRegression,
-    Lasso,
-    Ridge,
-    ElasticNet,
-    LogisticRegression,
-    LinearSVC,
-    LinearSVR,
-    DecisionTreeClassifier,
-    DecisionTreeRegressor,
-    NeuralNetClassifier,
-    NeuralNetRegressor,
-    TweedieRegressor,
-    GammaRegressor,
-    PoissonRegressor,
-    QuantizedModule,
-]
-
-
 try:
     # 3.8 and above
     # pylint: disable-next=no-name-in-module
     from importlib.metadata import version
 except ImportError:  # pragma: no cover
     # 3.7 and below
     # pylint: disable-next=no-name-in-module
@@ -167,29 +123,29 @@
     def _export_model_to_json(self) -> Path:
         """Export the quantizers to a json file.
 
         Returns:
             Path: the path to the json file
         """
         serialized_processing = {
-            "model_type": self.model.__class__.__name__,
+            "model_type": self.model.__class__,
             "model_post_processing_params": self.model.post_processing_params,
             "input_quantizers": self.model.input_quantizers,
             "output_quantizers": self.model.output_quantizers,
             "cml_version": CML_VERSION,
         }
 
         # Export the `is_fitted` attribute for built-in models
         if hasattr(self.model, "is_fitted"):
             serialized_processing["is_fitted"] = self.model.is_fitted
 
         # Dump json
         json_path = Path(self.path_dir).joinpath("serialized_processing.json")
         with open(json_path, "w", encoding="utf-8") as file:
-            json.dump(serialized_processing, file, cls=CustomEncoder)
+            dump(serialized_processing, file)
         return json_path
 
     def save(self, via_mlir: bool = False):
         """Export all needed artifacts for the client and server.
 
         Arguments:
             via_mlir (bool): serialize with `via_mlir` option from Concrete-Python.
@@ -280,15 +236,15 @@
             ValueError: if mismatch in versions between serialized file and runtime
         """
         self.client = fhe.Client.load(Path(self.path_dir).joinpath("client.zip"), self.key_dir)
 
         # Load the quantizers
         with zipfile.ZipFile(Path(self.path_dir).joinpath("client.zip")) as client_zip:
             with client_zip.open("serialized_processing.json", mode="r") as file:
-                serialized_processing = json.load(file)
+                serialized_processing = load(file)
 
         # Load versions for checking
         with zipfile.ZipFile(Path(self.path_dir).joinpath("client.zip")) as client_zip:
             with client_zip.open("versions.json", mode="r") as file:
                 versions = json.load(file)
 
         errors = []
@@ -309,25 +265,18 @@
         assert_true(
             serialized_processing["cml_version"] == CML_VERSION,
             f"The version of Concrete ML library ({CML_VERSION}) is different "
             f"from the one used to save the model ({serialized_processing['cml_version']}). "
             "Please update to the proper Concrete ML version.",
         )
 
-        # Create dict with available models along with their name
-        model_dict = {model_type().__class__.__name__: model_type for model_type in AVAILABLE_MODEL}
-
         # Initialize the model
-        self.model = model_dict[serialized_processing["model_type"]]()
-        self.model.input_quantizers = [
-            load_dict(elt) for elt in serialized_processing["input_quantizers"]
-        ]
-        self.model.output_quantizers = [
-            load_dict(elt) for elt in serialized_processing["output_quantizers"]
-        ]
+        self.model = serialized_processing["model_type"]()
+        self.model.input_quantizers = serialized_processing["input_quantizers"]
+        self.model.output_quantizers = serialized_processing["output_quantizers"]
 
         # Load the `_is_fitted` private attribute for built-in models
         if "is_fitted" in serialized_processing:
             # This private access should be temporary as the Client-Server interface could benefit
             # from built-in serialization load/dump methods
             # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3243
             # pylint: disable-next=protected-access
```

## concrete/ml/pytest/torch_models.py

```diff
@@ -345,14 +345,69 @@
             the output of the NN
         """
         x = self.layer1(x)
         y = self.layer2(y)
         return self.layer1(x + y)
 
 
+class MultiInputNNDifferentSize(nn.Module):
+    """Torch model to test multiple inputs with different shape in the forward pass."""
+
+    def __init__(
+        self,
+        input_output,
+        activation_function=None,
+        is_brevitas_qat=False,
+        n_bits=3,
+    ):  # pylint: disable=unused-argument
+        super().__init__()
+
+        # input_output is expected to be a list of two integers representing in and out features
+        # for both x and y
+        if is_brevitas_qat:
+            # n_bits is used for quantizing both the inputs and the weights, therefore we need
+            # to make sure that it is at least 2 bits
+            assert n_bits > 1, "Weights cannot be quantized over a single bit"
+
+            self.quant1 = qnn.QuantIdentity(bit_width=n_bits)
+            self.quant2 = qnn.QuantIdentity(bit_width=n_bits)
+            self.quant3 = qnn.QuantIdentity(bit_width=n_bits)
+            self.layer1 = qnn.QuantLinear(
+                input_output[0], input_output[0], bias=False, weight_bit_width=n_bits
+            )
+            self.layer2 = qnn.QuantLinear(
+                input_output[1], input_output[0], bias=False, weight_bit_width=n_bits
+            )
+
+        else:
+            self.layer1 = nn.Linear(input_output[0], input_output[0])
+            self.layer2 = nn.Linear(input_output[1], input_output[0])
+
+        self.is_brevitas_qat = is_brevitas_qat
+
+    def forward(self, x, y):
+        """Forward pass.
+
+        Args:
+            x: The first input of the NN.
+            y: The second input of the NN.
+
+        Returns:
+            The output of the NN.
+        """
+        if self.is_brevitas_qat:
+            x = self.layer1(self.quant1(x))
+            y = self.layer2(self.quant2(y))
+            return self.layer1(self.quant3(x + y))
+
+        x = self.layer1(x)
+        y = self.layer2(y)
+        return self.layer1(x + y)
+
+
 class BranchingModule(nn.Module):
     """Torch model with some branching and skip connections."""
 
     # pylint: disable-next=unused-argument
     def __init__(self, input_output, activation_function):
         super().__init__()
```

## concrete/ml/pytest/utils.py

```diff
@@ -1,17 +1,21 @@
 """Common functions or lists for test files, which can't be put in fixtures."""
+import io
 from functools import partial
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 import numpy
 import pytest
 import torch
+from numpy.random import RandomState
 from torch import nn
 
+from ..common.serialization.dumpers import dump, dumps
+from ..common.serialization.loaders import load, loads
 from ..common.utils import get_model_class, get_model_name, is_model_class_in_a_list, is_pandas_type
 from ..sklearn import (
     DecisionTreeClassifier,
     DecisionTreeRegressor,
     ElasticNet,
     GammaRegressor,
     Lasso,
@@ -53,14 +57,15 @@
         module__n_w_bits=2,
         module__n_a_bits=2,
         module__n_accum_bits=7,  # Stay with 7 bits for test exec time
         module__n_hidden_neurons_multiplier=1,
         module__activation_function=nn.ReLU,
         max_epochs=10,
         verbose=0,
+        callbacks="disable",
     ),
 ]
 
 _classifier_models = [
     DecisionTreeClassifier,
     RandomForestClassifier,
     XGBClassifier,
@@ -68,14 +73,15 @@
     LogisticRegression,
     partial(
         NeuralNetClassifier,
         module__n_layers=3,
         module__activation_function=nn.ReLU,
         max_epochs=10,
         verbose=0,
+        callbacks="disable",
     ),
 ]
 
 # Get the data-sets. The data generation is seeded in load_data.
 _classifiers_and_datasets = [
     pytest.param(
         model,
@@ -170,20 +176,20 @@
 
         model = model_class(**extra_kwargs)
 
     # Else, set the model using n_bits
     else:
         model = model_class(n_bits=n_bits)
 
-    # Seed the model
+    # Seed the model if it handles "random_state" as a parameter
     model_params = model.get_params()
     if "random_state" in model_params:
         model_params["random_state"] = numpy.random.randint(0, 2**15)
 
-    model.set_params(**model_params)
+        model.set_params(**model_params)
 
     return model
 
 
 def get_torchvision_dataset(
     param: Dict,
     train_set: bool,
@@ -287,7 +293,160 @@
         if isinstance(state_dict_or_path, (str, Path)):
             state_dict = torch.load(state_dict_or_path, map_location=device)
         else:
             state_dict = state_dict_or_path
         model.load_state_dict(state_dict)
 
     return model
+
+
+# pylint: disable-next=too-many-return-statements
+def values_are_equal(value_1: Any, value_2: Any) -> bool:
+    """Indicate if two values are equal.
+
+    This method takes into account objects of type None, numpy.ndarray, numpy.floating,
+    numpy.integer, numpy.random.RandomState or any instance that provides a `__eq__` method.
+
+    Args:
+        value_2 (Any): The first value to consider.
+        value_1 (Any): The second value to consider.
+
+    Returns:
+        bool: If the two values are equal.
+    """
+    if value_1 is None:
+        return value_2 is None
+
+    if isinstance(value_1, numpy.ndarray):
+        return (
+            isinstance(value_2, numpy.ndarray)
+            and numpy.array_equal(value_1, value_2)
+            and value_1.dtype == value_2.dtype
+        )
+
+    if isinstance(value_1, (numpy.floating, numpy.integer)):
+        return (
+            isinstance(value_2, (numpy.floating, numpy.integer))
+            and value_1 == value_2
+            and value_1.dtype == value_2.dtype
+        )
+
+    if isinstance(value_1, RandomState):
+        if isinstance(value_2, RandomState):
+            state_1, state_2 = value_1.get_state(), value_2.get_state()
+
+            # Check that values from both states are equal
+            for elt_1, elt_2 in zip(state_1, state_2):
+                if not numpy.array_equal(elt_1, elt_2):
+                    return False
+            return True
+        return False
+
+    return value_1 == value_2
+
+
+def check_serialization(
+    object_to_serialize: Any,
+    expected_type: Type,
+    equal_method: Optional[Callable] = None,
+    check_str: bool = True,
+):
+    """Check that the given object can properly be serialized.
+
+    This function serializes all objects using the `dump`, `dumps`, `load` and `loads` functions
+    from Concrete ML. If the given object provides a `dump` and `dumps` method, they are also
+    serialized using these.
+
+    Args:
+        object_to_serialize (Any): The object to serialize.
+        expected_type (Type): The object's expected type.
+        equal_method (Optional[Callable]): The function to use to compare the two loaded objects.
+            Default to `values_are_equal`.
+        check_str (bool): If the JSON strings should also be checked. Default to True.
+    """
+    # apidocs does not work properly when the function is directly in the default value.
+    if equal_method is None:
+        equal_method = values_are_equal
+
+    assert (
+        isinstance(object_to_serialize, expected_type)
+        if expected_type is not None
+        else object_to_serialize is None
+    )
+
+    dump_method_to_test = [False]
+
+    # If the given object provides a `dump`, `dumps` `dump_dict` method (which indicates that they
+    # are Concrete ML serializable classes), run the check using these as well
+    if (
+        hasattr(object_to_serialize, "dump")
+        and hasattr(object_to_serialize, "dumps")
+        and hasattr(object_to_serialize, "dump_dict")
+    ):
+        dump_method_to_test.append(True)
+
+    for use_dump_method in dump_method_to_test:
+
+        # Dump the object into a string
+        if use_dump_method:
+            dumped_str = object_to_serialize.dumps()
+        else:
+            dumped_str = dumps(object_to_serialize)
+
+        # Load the object using a string
+        loaded = loads(dumped_str)
+
+        # Assert that the loaded object is equal to the initial one
+        assert isinstance(loaded, expected_type) if expected_type is not None else loaded is None, (
+            f"Loaded object (from string) is not of the expected type. Expected {expected_type}, "
+            f"got {type(loaded)}."
+        )
+        assert equal_method(object_to_serialize, loaded), (
+            "Loaded object (from string) is not equal to the initial one, using equal method "
+            f"{equal_method}."
+        )
+
+        if check_str:
+            # Dump the loaded object into a string
+            if use_dump_method:
+                re_dumped_str = loaded.dumps()
+            else:
+                re_dumped_str = dumps(loaded)
+
+            # Assert that both JSON strings are equal. This will not work if some objects were
+            # dumped using Skops or pickle (such as a scikit-learn model or a Type object)
+            assert isinstance(dumped_str, str) and isinstance(re_dumped_str, str), (
+                f"One of the dumped strings is not a string. Got {type(dumped_str)} and "
+                f"{type(re_dumped_str)}."
+            )
+            assert dumped_str == re_dumped_str, (
+                "Dumped strings are not equal. This could come from objects that were serialized "
+                "in binary strings using Skops or pickle. If this cannot be avoided, please set "
+                "`check_str` to False."
+            )
+
+        # Define a buffer to test serialization in a file
+        with io.StringIO() as buffer:
+            buffer.seek(0, 0)
+
+            # Dump the object in a file
+            if use_dump_method:
+                object_to_serialize.dump(buffer)
+            else:
+                dump(object_to_serialize, buffer)
+
+            buffer.seek(0, 0)
+
+            # Load the object from the file
+            loaded = load(buffer)
+
+            # Assert that the loaded object is equal to the initial one
+            assert (
+                isinstance(loaded, expected_type) if expected_type is not None else loaded is None
+            ), (
+                "Loaded object (from file) is not of the expected type. Expected "
+                f"{expected_type}, got {type(loaded)}."
+            )
+            assert equal_method(object_to_serialize, loaded), (
+                "Loaded object (from file) is not equal to the initial one, using equal method "
+                f"{equal_method}."
+            )
```

## concrete/ml/quantization/base_quantized_op.py

```diff
@@ -1,18 +1,19 @@
 """Base Quantized Op class that implements quantization for a float numpy op."""
 
 from copy import deepcopy
 from inspect import Parameter, _empty, signature
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Type, Union, cast
+from typing import Any, Callable, Dict, List, Optional, Set, TextIO, Tuple, Type, Union, cast
 
 import numpy
 
 from concrete import fhe
 
 from ..common.debugging import assert_false, assert_true
+from ..common.serialization.dumpers import dump, dumps
 from ..common.utils import compute_bits_precision
 from ..onnx.onnx_utils import ONNX_OPS_TO_NUMPY_IMPL
 from ..onnx.ops_impl import ONNXMixedFunction, RawOpOutput
 from .quantizers import (
     MinMaxQuantizationStats,
     QuantizationOptions,
     QuantizedArray,
@@ -65,15 +66,15 @@
     output_quant_params: Optional[UniformQuantizationParameters]
     output_quant_stats: Optional[MinMaxQuantizationStats]
     input_quant_opts: QuantizationOptions
 
     constant_inputs: Dict[int, Any]
     attrs: Dict[str, Any] = {}
     _authorized_attr_names: Set[str] = set()
-    # This can be used for custom implementations of some missing or (god forbid) buggy operators.
+    # This can be used for custom implementations of some missing or buggy operators
     _impl_for_op_named: Optional[str] = None
     _default_attrs: Dict[str, Any] = {}
     _params_name_to_input_idx: Dict[str, int] = {}
     _input_idx_to_params_name: Dict[int, str] = {}
     _params_that_are_onnx_inputs: Set[str] = set()
     _params_that_are_onnx_var_inputs: Set[str] = set()
     _params_that_are_required_onnx_inputs: Set[str] = set()
@@ -133,15 +134,24 @@
         # recommended usage. We use "0" since this is a common ONNX tensor name for inputs.
         self._int_input_names = {"0"} if int_input_names is None else int_input_names
 
         constant_inputs_per_name: Dict[str, Any] = {}
 
         def _convert_input_name_or_idx_to_input_name(input_name_or_idx: Union[str, int]) -> str:
             if isinstance(input_name_or_idx, str):
-                return input_name_or_idx
+
+                # When serializing constant inputs using a JSONEncoder, integer indexes are
+                # automatically converted to strings. We therefore need to put these indexes back
+                # to integers by checking if the current string can be converted to an integer
+                # object.
+                if input_name_or_idx.isdigit():
+                    input_name_or_idx = int(input_name_or_idx)
+                else:
+                    return input_name_or_idx
+
             return self._input_idx_to_params_name[input_name_or_idx]
 
         if constant_inputs is not None:
             # Convert input idx to op input names if needed
             constant_inputs_per_name.update(
                 (
                     _convert_input_name_or_idx_to_input_name(input_name_or_idx),
@@ -181,29 +191,161 @@
         if self.can_fuse():
             self.input_quant_opts.is_qat = False
 
         # Set the operation's name, which is used to identify this op in the Concrete ML op graph
         # with respect to the ONNX graph (usually we keep use ONNX op name)
         self.op_instance_name = op_instance_name
 
+    def dump_dict(self) -> Dict:
+        """Dump itself to a dict.
+
+        Returns:
+            metadata (Dict): Dict of serialized objects.
+        """
+        metadata: Dict[str, Any] = {}
+
+        metadata["_impl_for_op_named"] = self._impl_for_op_named
+
+        # Attributes needed for instantiating a quantized operator
+        metadata["n_bits"] = self.n_bits
+        metadata["op_instance_name"] = self.op_instance_name
+        metadata["_int_input_names"] = self.int_input_names
+        metadata["constant_inputs"] = self.constant_inputs
+        metadata["input_quant_opts"] = self.input_quant_opts
+        metadata["attrs"] = self.attrs
+
+        # Output quantization attributes
+        metadata["output_quant_params"] = self.output_quant_params
+        metadata["output_quant_stats"] = self.output_quant_stats
+        if hasattr(self, "output_quant_opts"):
+            metadata["output_quant_opts"] = self.output_quant_opts
+
+        # QuantizedOp attributes
+        # Set attributes are converted to list since set are not serializable. Additionally, in
+        # order to be able to properly compare identical serialized objects, these lists are sorted
+        metadata["_authorized_attr_names"] = self._authorized_attr_names
+        metadata["_default_attrs"] = self._default_attrs
+        metadata["_params_name_to_input_idx"] = self._params_name_to_input_idx
+        metadata["_input_idx_to_params_name"] = self._input_idx_to_params_name
+        metadata["_params_that_are_onnx_inputs"] = self._params_that_are_onnx_inputs
+        metadata["_params_that_are_onnx_var_inputs"] = self._params_that_are_onnx_var_inputs
+        metadata[
+            "_params_that_are_required_onnx_inputs"
+        ] = self._params_that_are_required_onnx_inputs
+        metadata["_has_attr"] = self._has_attr
+        metadata["_inputs_not_quantized"] = self._inputs_not_quantized
+        metadata[
+            "quantize_inputs_with_model_outputs_precision"
+        ] = self.quantize_inputs_with_model_outputs_precision
+        metadata["produces_graph_output"] = self.produces_graph_output
+        metadata["produces_raw_output"] = self.produces_raw_output
+        metadata["error_tracker"] = self.error_tracker
+        metadata["debug_value_tracker"] = self.debug_value_tracker
+
+        # Additional attributes specific to some quantized operators
+        for attribute_name in vars(self):
+            attribute_value = getattr(self, attribute_name)
+
+            if attribute_name not in metadata:
+                metadata[attribute_name] = attribute_value
+
+        return metadata
+
+    @staticmethod
+    def load_dict(metadata: Dict):
+        """Load itself from a string.
+
+        Args:
+            metadata (Dict): Dict of serialized objects.
+
+        Returns:
+            QuantizedOp: The loaded object.
+        """
+
+        # Instantiate the quantized operator
+        quantized_op = ONNX_OPS_TO_QUANTIZED_IMPL[metadata.pop("_impl_for_op_named")]
+        obj = quantized_op(
+            n_bits_output=metadata.pop("n_bits"),
+            op_instance_name=metadata.pop("op_instance_name"),
+            int_input_names=metadata.pop("_int_input_names"),
+            constant_inputs=metadata.pop("constant_inputs"),
+            input_quant_opts=metadata.pop("input_quant_opts"),
+            **metadata.pop("attrs"),
+        )
+
+        # Output quantization attributes
+        obj.output_quant_params = metadata.pop("output_quant_params")
+        obj.output_quant_stats = metadata.pop("output_quant_stats")
+        if "output_quant_opts" in metadata:
+            assert hasattr(
+                obj, "output_quant_opts"
+            ), f"{obj.__class__.__name__} has no output_quant_opts attribute."
+
+            obj.output_quant_opts = metadata.pop("output_quant_opts")  # type: ignore[arg-type]
+
+        # QuantizedOp attributes
+        # pylint: disable=protected-access
+        obj._authorized_attr_names = metadata.pop("_authorized_attr_names")
+        obj._default_attrs = metadata.pop("_default_attrs")
+        obj._params_name_to_input_idx = metadata.pop("_params_name_to_input_idx")
+        obj._input_idx_to_params_name = metadata.pop("_input_idx_to_params_name")
+        obj._params_that_are_onnx_inputs = metadata.pop("_params_that_are_onnx_inputs")
+        obj._params_that_are_onnx_var_inputs = metadata.pop("_params_that_are_onnx_var_inputs")
+        obj._params_that_are_required_onnx_inputs = metadata.pop(
+            "_params_that_are_required_onnx_inputs"
+        )
+        obj._has_attr = metadata.pop("_has_attr")
+        obj._inputs_not_quantized = metadata.pop("_inputs_not_quantized")
+        obj.quantize_inputs_with_model_outputs_precision = metadata.pop(
+            "quantize_inputs_with_model_outputs_precision"
+        )
+        obj.produces_graph_output = metadata.pop("produces_graph_output")
+        obj.produces_raw_output = metadata.pop("produces_raw_output")
+        obj.error_tracker = metadata.pop("error_tracker")
+        obj.debug_value_tracker = metadata.pop("debug_value_tracker")
+        # pylint: enable=protected-access
+
+        # Additional attributes specific to some quantized operators
+        for attribute in metadata:
+            if hasattr(obj, attribute):
+                setattr(obj, attribute, metadata[attribute])
+
+        return obj
+
+    def dumps(self) -> str:
+        """Dump itself to a string.
+
+        Returns:
+            metadata (str): String of the serialized object.
+        """
+        return dumps(self)
+
+    def dump(self, file: TextIO) -> None:
+        """Dump itself to a file.
+
+        Args:
+            file (TextIO): The file to dump the serialized object into.
+        """
+        dump(self, file)
+
     @classmethod
     def op_type(cls):
         """Get the type of this operation.
 
         Returns:
             op_type (str): The type of this operation, in the ONNX referential
         """
         return cls._impl_for_op_named
 
     @property
     def int_input_names(self):
         """Get the names of encrypted integer tensors that are used by this op.
 
         Returns:
-            List[str]: the names of the tensors
+            Set[str]: the names of the tensors
 
         """
 
         return self._int_input_names
 
     # Register node to our internal categories
     def __init_subclass__(cls, is_utility=False, **kwargs):
```

## concrete/ml/quantization/post_training.py

```diff
@@ -590,17 +590,22 @@
         # First transform all parameters to their quantized version
         self._quantize_params()
 
         self._quantize_layers(*calibration_data)
 
         # Create quantized module from self.quant_layers_dict
         quantized_module = QuantizedModule(
-            (graph_input.name for graph_input in self.numpy_model.onnx_model.graph.input),
-            (graph_output.name for graph_output in self.numpy_model.onnx_model.graph.output),
-            self.quant_ops_dict,
+            ordered_module_input_names=(
+                graph_input.name for graph_input in self.numpy_model.onnx_model.graph.input
+            ),
+            ordered_module_output_names=(
+                graph_output.name for graph_output in self.numpy_model.onnx_model.graph.output
+            ),
+            quant_layers_dict=self.quant_ops_dict,
+            onnx_model=self.numpy_model.onnx_model,
         )
 
         self._process_input_quantizers(quantized_module, calibration_data)
 
         return quantized_module
 
     def _process_input_quantizers(
```

## concrete/ml/quantization/quantized_module.py

```diff
@@ -1,25 +1,28 @@
 """QuantizedModule API."""
 import copy
 import re
-from typing import Any, Dict, Generator, Iterable, List, Optional, Tuple, Union
+from typing import Any, Dict, Generator, Iterable, List, Optional, TextIO, Tuple, Union
 
 import numpy
+import onnx
 from concrete.fhe.compilation.artifacts import DebugArtifacts
 from concrete.fhe.compilation.circuit import Circuit
 from concrete.fhe.compilation.compiler import Compiler
 from concrete.fhe.compilation.configuration import Configuration
 
 from ..common.debugging import assert_true
+from ..common.serialization.dumpers import dump, dumps
 from ..common.utils import (
     SUPPORTED_FLOAT_TYPES,
     SUPPORTED_INT_TYPES,
     FheMode,
     all_values_are_floats,
     all_values_are_integers,
+    all_values_are_of_dtype,
     check_there_is_no_p_error_options_in_configuration,
     generate_proxy_function,
     manage_parameters_for_pbs_errors,
     to_tuple,
 )
 from .base_quantized_op import ONNXOpInputOutputType, QuantizedOp
 from .quantizers import QuantizedArray, UniformQuantizer
@@ -84,23 +87,24 @@
     fhe_circuit: Union[None, Circuit]
 
     def __init__(
         self,
         ordered_module_input_names: Iterable[str] = None,
         ordered_module_output_names: Iterable[str] = None,
         quant_layers_dict: Dict[str, Tuple[Tuple[str, ...], QuantizedOp]] = None,
+        onnx_model: onnx.ModelProto = None,
     ):
         # Set base attributes for API consistency. This could be avoided if an abstract base class
         # is created for both Concrete ML models and QuantizedModule
         # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/2899
         self.fhe_circuit = None
         self._is_compiled = False
         self.input_quantizers = []
         self.output_quantizers = []
-        self._onnx_model = None
+        self._onnx_model = onnx_model
         self._post_processing_params: Dict[str, Any] = {}
 
         # If any of the arguments are not provided, skip the init
         if not all([ordered_module_input_names, ordered_module_output_names, quant_layers_dict]):
             return
 
         # for mypy
@@ -117,14 +121,75 @@
             f"got {num_outputs}",
         )
 
         assert quant_layers_dict is not None
         self.quant_layers_dict = copy.deepcopy(quant_layers_dict)
         self.output_quantizers = self._set_output_quantizers()
 
+    def dump_dict(self) -> Dict:
+        """Dump itself to a dict.
+
+        Returns:
+            metadata (Dict): Dict of serialized objects.
+        """
+        metadata: Dict[str, Any] = {}
+
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["_onnx_model"] = self._onnx_model
+        metadata["_post_processing_params"] = self._post_processing_params
+        metadata["ordered_module_input_names"] = self.ordered_module_input_names
+        metadata["ordered_module_output_names"] = self.ordered_module_output_names
+        metadata["quant_layers_dict"] = self.quant_layers_dict
+
+        return metadata
+
+    @staticmethod
+    def load_dict(metadata: Dict):
+        """Load itself from a string.
+
+        Args:
+            metadata (Dict): Dict of serialized objects.
+
+        Returns:
+            QuantizedModule: The loaded object.
+        """
+
+        # Instantiate the module
+        obj = QuantizedModule()
+
+        # pylint: disable=protected-access
+        obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.output_quantizers = metadata["output_quantizers"]
+        obj._onnx_model = metadata["_onnx_model"]
+        obj.ordered_module_input_names = metadata["ordered_module_input_names"]
+        obj.ordered_module_output_names = metadata["ordered_module_output_names"]
+        obj.quant_layers_dict = metadata["quant_layers_dict"]
+        # pylint: enable=protected-access
+
+        return obj
+
+    def dumps(self) -> str:
+        """Dump itself to a string.
+
+        Returns:
+            metadata (str): String of the serialized object.
+        """
+        return dumps(self)
+
+    def dump(self, file: TextIO) -> None:
+        """Dump itself to a file.
+
+        Args:
+            file (TextIO): The file to dump the serialized object into.
+        """
+        dump(self, file)
+
     @property
     def is_compiled(self) -> bool:
         """Indicate if the model is compiled.
 
         Returns:
             bool: If the model is compiled.
         """
@@ -204,18 +269,14 @@
         .. # noqa: DAR201
 
         Returns:
            _onnx_model (onnx.ModelProto): the ONNX model
         """
         return self._onnx_model
 
-    @onnx_model.setter
-    def onnx_model(self, value):
-        self._onnx_model = value
-
     def __call__(self, *x: numpy.ndarray):
         """Define the QuantizedModule's call method.
 
         This method is a forward method executed in the clear.
 
         Args:
             *x (numpy.ndarray): Input float values to consider.
@@ -459,15 +520,16 @@
             f"Got {n_values} inputs, expected {n_inputs}. Either the quantized module has not been "
             "properly initialized or the input data has been changed since its initialization.",
             ValueError,
         )
 
         q_x = tuple(self.input_quantizers[idx].quant(x[idx]) for idx in range(len(x)))
 
-        assert numpy.array(q_x).dtype == numpy.int64, "Inputs were not quantized to int64 x"
+        # Make sure all inputs are quantized to int64
+        assert all_values_are_of_dtype(*q_x, dtypes="int64"), "Inputs were not quantized to int64"
 
         return q_x[0] if len(q_x) == 1 else q_x
 
     def dequantize_output(self, q_y_preds: numpy.ndarray) -> numpy.ndarray:
         """Take the last layer q_out and use its de-quant function.
 
         Args:
@@ -562,16 +624,16 @@
 
         # Quantize the inputs
         q_inputs = self.quantize_input(*inputs)
 
         # Generate the input-set with proper dimensions
         inputset = _get_inputset_generator(q_inputs)
 
-        # Don't let the user shoot in her foot, by having p_error or global_p_error set in both
-        # configuration and in direct arguments
+        # Check that p_error or global_p_error is not set in both the configuration and in the
+        # direct parameters
         check_there_is_no_p_error_options_in_configuration(configuration)
 
         # Find the right way to set parameters for compiler, depending on the way we want to default
         p_error, global_p_error = manage_parameters_for_pbs_errors(p_error, global_p_error)
 
         self.fhe_circuit = compiler.compile(
             inputset,
```

## concrete/ml/quantization/quantized_ops.py

```diff
@@ -1705,29 +1705,29 @@
             not self.is_signed and self.is_narrow,
             "Can not use narrow range for non-signed Brevitas quantizers",
         )
 
         # To ensure de-quantization produces floats, the following parameters must be float.
         # This should be default export setting in Brevitas
         check_float(
-            constant_inputs is not None
+            self.constant_inputs is not None
             and self.constant_inputs[self._params_name_to_input_idx["scale"]],
             "Scale of Brevitas Quant op must be float",
         )
         check_float(
-            constant_inputs is not None
+            self.constant_inputs is not None
             and self.constant_inputs[self._params_name_to_input_idx["zero_point"]],
             "Zero Point of Brevitas Quant op must be float",
         )
 
         # For mypy
-        assert constant_inputs is not None
+        assert self.constant_inputs is not None
 
-        # The constant inputs can have either int or str keys, here it is int
-        n_bits = constant_inputs[3]  # type: ignore
+        # The constant inputs can have either int or str keys, here it is an int
+        n_bits = self.constant_inputs[3]  # type: ignore
 
         # Set the QAT flag on the output of this operation, so that the
         # following operation in the graph is aware of this flag and can
         # just copy the quantization
         self.output_quant_opts = self._get_output_quant_opts()
         self.output_quant_opts.n_bits = n_bits
         self.output_quant_opts.is_qat = True
```

## concrete/ml/quantization/quantizers.py

```diff
@@ -1,19 +1,18 @@
 """Quantization utilities for a numpy array/tensor."""
 # pylint: disable=too-many-lines
 from __future__ import annotations
 
-import json
 from copy import deepcopy
-from typing import IO, Any, Dict, Optional, Union, get_type_hints
+from typing import Any, Dict, Optional, TextIO, Union, get_type_hints
 
 import numpy
 
 from ..common.debugging import assert_true
-from ..common.serialization.encoder import CustomEncoder
+from ..common.serialization.dumpers import dump, dumps
 
 STABILITY_CONST = 10**-6
 
 
 def fill_from_kwargs(obj, klass, **kwargs):
     """Fill a parameter set structure from kwargs parameters.
 
@@ -110,94 +109,75 @@
 
         # QAT quantization is not symmetric
         assert_true(not self.is_qat or not self.is_symmetric)
 
         # Symmetric quantization is signed
         assert_true(not self.is_symmetric or self.is_signed)
 
+    def __eq__(self, other) -> bool:
+        return (
+            other.n_bits == self.n_bits
+            and other.is_signed == self.is_signed
+            and other.is_symmetric == self.is_symmetric
+            and other.is_qat == self.is_qat
+            and other.is_narrow == self.is_narrow
+            and other.is_precomputed_qat == self.is_precomputed_qat
+        )
+
     def dump_dict(self) -> Dict:
         """Dump itself to a dict.
 
         Returns:
-            metadata (Dict): dict of serialized object
+            metadata (Dict): Dict of serialized objects.
         """
         metadata: Dict[str, Any] = {}
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+
         metadata["n_bits"] = self.n_bits
         metadata["is_signed"] = self.is_signed
         metadata["is_symmetric"] = self.is_symmetric
         metadata["is_qat"] = self.is_qat
         metadata["is_narrow"] = self.is_narrow
         metadata["is_precomputed_qat"] = self.is_precomputed_qat
         return metadata
 
-    def dumps(self) -> str:
-        """Dump itself to a string.
-
-        Returns:
-            metadata (str): string of serialized object
-        """
-
-        return json.dumps(self.dump_dict(), cls=CustomEncoder)
-
-    def dump(self, file: IO[str]):
-        """Dump itself to a file.
-
-        Args:
-            file (IO[str]): file of where to dump.
-        """
-        metadata = self.dump_dict()
-        json.dump(metadata, file, cls=CustomEncoder)
-
-    # Loading
     @staticmethod
     def load_dict(metadata: Dict):
         """Load itself from a string.
 
         Args:
-            metadata (Dict): dict of serialized object
+            metadata (Dict): Dict of serialized objects.
 
         Returns:
-            QuantizationOptions: the loaded object
+            QuantizationOptions: The loaded object.
         """
-        to_return = QuantizationOptions(
+        obj = QuantizationOptions(
             n_bits=metadata["n_bits"],
             is_symmetric=metadata["is_symmetric"],
             is_signed=metadata["is_signed"],
             is_qat=metadata["is_qat"],
         )
         for attr_name in ["is_narrow", "is_precomputed_qat"]:
-            setattr(to_return, attr_name, metadata[attr_name])
-        return to_return
-
-    @staticmethod
-    def load(file: IO[str]) -> QuantizationOptions:
-        """Load itself from a file.
+            setattr(obj, attr_name, metadata[attr_name])
+        return obj
 
-        Args:
-            file (IO[str]): file of serialized object
+    def dumps(self) -> str:
+        """Dump itself to a string.
 
         Returns:
-            QuantizationOptions: the loaded object
+            metadata (str): String of the serialized object.
         """
-        metadata = json.load(file)
-        return QuantizationOptions.load_dict(metadata=metadata)
+        return dumps(self)
 
-    @staticmethod
-    def loads(metadata: str) -> QuantizationOptions:
-        """Load itself from a string.
+    def dump(self, file: TextIO) -> None:
+        """Dump itself to a file.
 
         Args:
-            metadata (str): serialized object
-
-        Returns:
-            QuantizationOptions: the loaded object
+            file (TextIO): The file to dump the serialized object into.
         """
-        _metadata: Dict = json.loads(metadata)
-        return QuantizationOptions.load_dict(metadata=_metadata)
+        dump(self, file)
 
     def copy_opts(self, opts):
         """Copy the options from a different structure.
 
         Args:
             opts (QuantizationOptions): structure to copy parameters from.
         """
@@ -259,89 +239,68 @@
         rmin: Optional[float] = None,
         uvalues: Optional[numpy.ndarray] = None,
     ):
         self.rmax = rmax
         self.rmin = rmin
         self.uvalues = uvalues
 
+    def __eq__(self, other) -> bool:
+        # Disable mypy as numpy.array_equal properly handles None types
+        return (
+            other.rmax == self.rmax
+            and other.rmin == self.rmin
+            and numpy.array_equal(other.uvalues, self.uvalues)  # type: ignore[arg-type]
+        )
+
     def dump_dict(self) -> Dict:
         """Dump itself to a dict.
 
         Returns:
-            metadata (Dict): dict of serialized object
+            metadata (Dict): Dict of serialized objects.
         """
         metadata: Dict[str, Any] = {}
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+
         metadata["rmax"] = self.rmax
         metadata["rmin"] = self.rmin
         metadata["uvalues"] = self.uvalues
         return metadata
 
-    def dumps(self) -> str:
-        """Dump itself to a string.
-
-        Returns:
-            metadata (str): string of serialized object
-        """
-
-        return json.dumps(self.dump_dict(), cls=CustomEncoder)
-
-    def dump(self, file: IO[str]):
-        """Dump itself to a file.
-
-        Args:
-            file (IO[str]): file of where to dump.
-        """
-        metadata = self.dump_dict()
-        json.dump(metadata, file, cls=CustomEncoder)
-
-    # Loading
     @staticmethod
     def load_dict(metadata: Dict):
         """Load itself from a string.
 
         Args:
-            metadata (Dict): dict of serialized object
+            metadata (Dict): Dict of serialized objects.
 
         Returns:
-            QuantizationOptions: the loaded object
+            QuantizationOptions: The loaded object.
         """
         to_return = MinMaxQuantizationStats(
             rmax=metadata["rmax"],
             rmin=metadata["rmin"],
-            uvalues=numpy.array(metadata["uvalues"]),
+            uvalues=metadata["uvalues"],
         )
 
         return to_return
 
-    @staticmethod
-    def load(file: IO[str]) -> MinMaxQuantizationStats:
-        """Load itself from a file.
-
-        Args:
-            file (IO[str]): file of serialized object
+    def dumps(self) -> str:
+        """Dump itself to a string.
 
         Returns:
-            MinMaxQuantizationStats: the loaded object
+            metadata (str): String of the serialized object.
         """
-        metadata = json.load(file)
-        return MinMaxQuantizationStats.load_dict(metadata=metadata)
+        return dumps(self)
 
-    @staticmethod
-    def loads(metadata: str) -> MinMaxQuantizationStats:
-        """Load itself from a string.
+    def dump(self, file: TextIO) -> None:
+        """Dump itself to a file.
 
         Args:
-            metadata (str): serialized object
-
-        Returns:
-            MinMaxQuantizationStats: the loaded object
+            file (TextIO): The file to dump the serialized object into.
         """
-        _metadata: Dict = json.loads(metadata)
-        return MinMaxQuantizationStats.load_dict(metadata=_metadata)
+        dump(self, file)
 
     def compute_quantization_stats(self, values: numpy.ndarray) -> None:
         """Compute the calibration set quantization statistics.
 
         Args:
             values (numpy.ndarray): Calibration set on which to compute statistics.
         """
@@ -429,88 +388,66 @@
         zero_point: Optional[Union[int, float, numpy.ndarray]] = None,
         offset: Optional[int] = None,
     ):
         self.scale = scale
         self.zero_point = zero_point
         self.offset = offset
 
+    def __eq__(self, other) -> bool:
+        return (
+            other.scale == self.scale
+            and other.zero_point == self.zero_point
+            and other.offset == self.offset
+        )
+
     def dump_dict(self) -> Dict:
         """Dump itself to a dict.
 
         Returns:
-            metadata (Dict): dict of serialized object
+            metadata (Dict): Dict of serialized objects.
         """
         metadata: Dict[str, Any] = {}
-        metadata["cml_dumped_class_name"] = type(self).__name__
+
         metadata["scale"] = self.scale
         metadata["zero_point"] = self.zero_point
         metadata["offset"] = self.offset
         return metadata
 
-    def dumps(self) -> str:
-        """Dump itself to a string.
-
-        Returns:
-            metadata (str): string of serialized object
-        """
-
-        return json.dumps(self.dump_dict(), cls=CustomEncoder)
-
-    def dump(self, file: IO[str]):
-        """Dump itself to a file.
-
-        Args:
-            file (IO[str]): file of where to dump.
-        """
-        metadata = self.dump_dict()
-        json.dump(metadata, file, cls=CustomEncoder)
-
-    # Loading
     @staticmethod
     def load_dict(metadata: Dict) -> UniformQuantizationParameters:
         """Load itself from a string.
 
         Args:
-            metadata (Dict): dict of serialized object
+            metadata (Dict): Dict of serialized objects.
 
         Returns:
-            UniformQuantizationParameters: the loaded object
+            UniformQuantizationParameters: The loaded object.
         """
         to_return = UniformQuantizationParameters(
             scale=metadata["scale"],
             zero_point=metadata["zero_point"],
             offset=metadata["offset"],
         )
         return to_return
 
-    @staticmethod
-    def load(file: IO[str]) -> UniformQuantizationParameters:
-        """Load itself from a file.
-
-        Args:
-            file (IO[str]): file of serialized object
+    def dumps(self) -> str:
+        """Dump itself to a string.
 
         Returns:
-            UniformQuantizationParameters: the loaded object
+            metadata (str): String of the serialized object.
         """
-        metadata = json.load(file)
-        return UniformQuantizationParameters.load_dict(metadata=metadata)
+        return dumps(self)
 
-    @staticmethod
-    def loads(metadata: str) -> UniformQuantizationParameters:
-        """Load itself from a string.
+    def dump(self, file: TextIO) -> None:
+        """Dump itself to a file.
 
         Args:
-            metadata (str): serialized object
-
-        Returns:
-            UniformQuantizationParameters: the loaded object
+            file (TextIO): The file to dump the serialized object into.
         """
-        _metadata: Dict = json.loads(metadata)
-        return UniformQuantizationParameters.load_dict(metadata=_metadata)
+        dump(self, file)
 
     def copy_params(self, params) -> None:
         """Copy the parameters from a different structure.
 
         Args:
             params (UniformQuantizationParameters): parameter structure to copy
         """
@@ -672,14 +609,126 @@
 
         self.no_clipping = no_clipping
 
         # Force scale to be a float64
         if self.scale is not None:
             self.scale = numpy.float64(self.scale)
 
+    def __eq__(self, other) -> bool:
+
+        is_equal = other.no_clipping == self.no_clipping
+
+        for attribute in [
+            "n_bits",
+            "is_signed",
+            "is_symmetric",
+            "is_qat",
+            "is_narrow",
+            "is_precomputed_qat",
+            "rmax",
+            "rmin",
+            "uvalues",
+            "scale",
+            "zero_point",
+            "offset",
+        ]:
+            # All possible attributes in a UniformQuantizer object are not necessarily available
+            value_1, value_2 = getattr(other, attribute, None), getattr(self, attribute, None)
+
+            if isinstance(value_1, numpy.ndarray):
+                is_equal &= isinstance(value_2, numpy.ndarray) and numpy.array_equal(
+                    value_1, value_2
+                )
+            else:
+                is_equal &= value_1 == value_2
+
+        return is_equal
+
+    def dump_dict(self) -> Dict:
+        """Dump itself to a dict.
+
+        Returns:
+            metadata (Dict): Dict of serialized objects.
+        """
+        metadata: Dict[str, Any] = {}
+
+        for attribute in [
+            "n_bits",
+            "is_signed",
+            "is_symmetric",
+            "is_qat",
+            "is_narrow",
+            "is_precomputed_qat",
+            "rmax",
+            "rmin",
+            "uvalues",
+            "scale",
+            "zero_point",
+            "offset",
+            "no_clipping",
+        ]:
+            if hasattr(self, attribute):
+                metadata[attribute] = getattr(self, attribute)
+
+        return metadata
+
+    @staticmethod
+    def load_dict(metadata: Dict) -> UniformQuantizer:
+        """Load itself from a string.
+
+        Args:
+            metadata (Dict): Dict of serialized objects.
+
+        Returns:
+            UniformQuantizer: The loaded object.
+        """
+
+        # Instantiate the quantizer
+        obj = UniformQuantizer()
+
+        for attribute in [
+            "n_bits",
+            "is_signed",
+            "is_symmetric",
+            "is_qat",
+            "is_narrow",
+            "is_precomputed_qat",
+            "rmax",
+            "rmin",
+            "uvalues",
+            "scale",
+            "zero_point",
+            "offset",
+            "no_clipping",
+        ]:
+            if attribute in metadata:
+                setattr(obj, attribute, metadata[attribute])
+
+        # The `uvalues` attribute needs to be put back to a numpy.array object
+        if "uvalues" in metadata:
+            obj.uvalues = metadata["uvalues"]
+
+        return obj
+
+    def dumps(self) -> str:
+        """Dump itself to a string.
+
+        Returns:
+            metadata (str): String of the serialized object.
+        """
+        return dumps(self)
+
+    def dump(self, file: TextIO) -> None:
+        """Dump itself to a file.
+
+        Args:
+            file (TextIO): The file to dump the serialized object into.
+        """
+        dump(self, file)
+
     def quant(self, values: numpy.ndarray) -> numpy.ndarray:
         """Quantize values.
 
         Args:
             values (numpy.ndarray): float values to quantize
 
         Returns:
@@ -735,90 +784,14 @@
             + ((" " + str(self.scale.dtype)) if isinstance(self.scale, numpy.ndarray) else ""),
         )
 
         ans = self.scale * (qvalues - numpy.asarray(self.zero_point, dtype=numpy.float64))
 
         return ans
 
-    def dump_dict(self) -> Dict:
-        """Dump itself to a dict.
-
-        Returns:
-            metadata (Dict): dict of serialized object
-        """
-        metadata: Dict[str, Any] = {}
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
-
-        for attribute in ["zero_point", "scale", "offset", "n_bits"]:
-            if hasattr(self, attribute):
-                metadata[attribute] = getattr(self, attribute)
-        return metadata
-
-    def dumps(self) -> str:
-        """Dump itself to a string.
-
-        Returns:
-            metadata (str): string of serialized object
-        """
-        metadata = self.dump_dict()
-        return json.dumps(metadata, cls=CustomEncoder)
-
-    def dump(self, file: IO[str]) -> None:
-        """Dump itself to a file.
-
-        Args:
-            file (IO[str]): file of where to dump.
-        """
-        metadata = self.dump_dict()
-        json.dump(metadata, file, cls=CustomEncoder)
-
-    # Loading
-    @staticmethod
-    def load_dict(metadata: Dict) -> UniformQuantizer:
-        """Load itself from a string.
-
-        Args:
-            metadata (Dict): dict of serialized object
-
-        Returns:
-            UniformQuantizer: the loaded object
-        """
-        obj = UniformQuantizer()
-
-        for attribute in ["zero_point", "scale", "offset", "n_bits"]:
-            if attribute in metadata:
-                setattr(obj, attribute, metadata[attribute])
-        return obj
-
-    @staticmethod
-    def load(file: IO[str]) -> UniformQuantizer:
-        """Load itself from a file.
-
-        Args:
-            file (IO[str]): file of serialized object
-
-        Returns:
-            UniformQuantizer: the loaded object
-        """
-        metadata = json.load(file)
-        return UniformQuantizer.load_dict(metadata=metadata)
-
-    @staticmethod
-    def loads(metadata: str) -> UniformQuantizer:
-        """Load itself from a string.
-
-        Args:
-            metadata (str): serialized object
-
-        Returns:
-            UniformQuantizer: the loaded object
-        """
-        _metadata: Dict = json.loads(metadata)
-        return UniformQuantizer.load_dict(metadata=_metadata)
-
 
 class QuantizedArray:
     """Abstraction of quantized array.
 
     Contains float values and their quantized integer counter-parts. Quantization is performed
     by the quantizer member object. Float and int values are kept in sync. Having both types
     of values is useful since quantized operators in Concrete ML graphs might need one or the other
@@ -837,16 +810,14 @@
         stats (Optional[MinMaxQuantizationStats]): Quantization batch statistics set
         params (Optional[UniformQuantizationParameters]): Quantization parameters set
             (scale, zero-point)
         kwargs: Any member of the options, stats, params sets as a key-value pair. The parameter
             sets need to be completely parametrized if their members appear in kwargs.
     """
 
-    STABILITY_CONST = 10**-6
-
     quantizer: UniformQuantizer
     values: numpy.ndarray
     qvalues: numpy.ndarray
 
     def __init__(
         self,
         n_bits,
@@ -877,14 +848,22 @@
         # Create the quantizer from the provided parameter sets
         # Some parameters could be None and are computed below
         self.quantizer = UniformQuantizer(options, stats, params)
 
         if values is not None:
             self._values_setup(values, value_is_float, options, stats, params)
 
+    def __eq__(self, other):
+        is_equal = other.n_bits == self.n_bits and other.quantizer == self.quantizer
+
+        for attribute in ["values", "qvalues"]:
+            is_equal &= numpy.array_equal(getattr(other, attribute), getattr(self, attribute))
+
+        return is_equal
+
     def _values_setup(
         self,
         values: numpy.ndarray,
         value_is_float: bool,
         options: QuantizationOptions = None,
         stats: Optional[MinMaxQuantizationStats] = None,
         params: Optional[UniformQuantizationParameters] = None,
@@ -943,14 +922,62 @@
 
             # Populate self.values
             self.dequant()
 
     def __call__(self) -> Optional[numpy.ndarray]:
         return self.qvalues
 
+    def dump_dict(self) -> Dict:
+        """Dump itself to a dict.
+
+        Returns:
+            metadata (Dict): Dict of serialized objects.
+        """
+        metadata: Dict[str, Any] = {}
+
+        metadata["quantizer"] = self.quantizer
+        metadata["n_bits"] = self.n_bits
+        metadata["values"] = self.values
+        metadata["qvalues"] = self.qvalues
+        return metadata
+
+    @staticmethod
+    def load_dict(metadata: Dict) -> QuantizedArray:
+        """Load itself from a string.
+
+        Args:
+            metadata (Dict): Dict of serialized objects.
+
+        Returns:
+            QuantizedArray: The loaded object.
+        """
+        obj = QuantizedArray(n_bits=metadata["n_bits"], values=metadata["values"])
+
+        obj.quantizer = metadata["quantizer"]
+        obj.values = metadata["values"]
+        obj.qvalues = metadata["qvalues"]
+
+        return obj
+
+    def dumps(self) -> str:
+        """Dump itself to a string.
+
+        Returns:
+            metadata (str): String of the serialized object.
+        """
+        return dumps(self)
+
+    def dump(self, file: TextIO) -> None:
+        """Dump itself to a file.
+
+        Args:
+            file (TextIO): The file to dump the serialized object into.
+        """
+        dump(self, file)
+
     def update_values(self, values: numpy.ndarray) -> numpy.ndarray:
         """Update values to get their corresponding qvalues using the related quantized parameters.
 
         Args:
             values (numpy.ndarray): Values to replace self.values
 
         Returns:
@@ -991,87 +1018,7 @@
         """
         self.values = self.quantizer.dequant(self.qvalues)
         assert_true(
             not isinstance(self.values, numpy.ndarray) or self.values.dtype == numpy.float64,
             "De-quantized values must be float64",
         )
         return self.values
-
-    def dump_dict(self) -> Dict:
-        """Dump itself to a dict.
-
-        Returns:
-            metadata (Dict): dict of serialized object
-        """
-        metadata: Dict[str, Any] = {}
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
-        metadata["STABILITY_CONST"] = self.STABILITY_CONST
-        metadata["quantizer"] = self.quantizer
-        metadata["n_bits"] = self.n_bits
-        metadata["values"] = self.values
-        metadata["qvalues"] = self.qvalues
-        metadata["values"] = self.values
-        return metadata
-
-    def dumps(self) -> str:
-        """Dump itself to a string.
-
-        Returns:
-            metadata (str): string of serialized object
-        """
-        metadata = self.dump_dict()
-        return json.dumps(metadata, cls=CustomEncoder)
-
-    def dump(self, file: IO[str]) -> None:
-        """Dump itself to a file.
-
-        Args:
-            file (IO[str]): file of where to dump.
-        """
-        metadata = self.dump_dict()
-        json.dump(metadata, file, cls=CustomEncoder)
-
-    # Loading
-    @staticmethod
-    def load_dict(metadata: Dict) -> QuantizedArray:
-        """Load itself from a string.
-
-        Args:
-            metadata (Dict): dict of serialized object
-
-        Returns:
-            QuantizedArray: the loaded object
-        """
-        obj = QuantizedArray(n_bits=metadata["n_bits"], values=metadata["values"])
-        # pylint: disable-next=invalid-name
-        obj.STABILITY_CONST = metadata["STABILITY_CONST"]
-        obj.quantizer = metadata["quantizer"]
-        obj.values = metadata["values"]
-        obj.qvalues = metadata["qvalues"]
-
-        return obj
-
-    @staticmethod
-    def load(file: IO[str]) -> QuantizedArray:
-        """Load itself from a file.
-
-        Args:
-            file (IO[str]): file of serialized object
-
-        Returns:
-            QuantizedArray: the loaded object
-        """
-        metadata = json.load(file)
-        return QuantizedArray.load_dict(metadata=metadata)
-
-    @staticmethod
-    def loads(metadata: str) -> QuantizedArray:
-        """Load itself from a string.
-
-        Args:
-            metadata (str): serialized object
-
-        Returns:
-            QuantizedArray: the loaded object
-        """
-        _metadata: Dict = json.loads(metadata)
-        return QuantizedArray.load_dict(metadata=_metadata)
```

## concrete/ml/sklearn/base.py

```diff
@@ -1,38 +1,37 @@
 """Base classes for all estimators."""
 from __future__ import annotations
 
-import json
 import tempfile
 
 # Disable pylint as some names like X and q_X are used, following scikit-Learn's standard. The file
 # is also more than 1000 lines long.
 # pylint: disable=too-many-lines,invalid-name
 import warnings
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import IO, Any, Callable, Dict, List, Optional, Set, Type, Union
+from typing import Any, Callable, Dict, List, Optional, Set, TextIO, Type, Union
 
 import brevitas.nn as qnn
 import numpy
 import onnx
 import sklearn
+import skorch.net
 import torch
 from brevitas.export.onnx.qonnx.manager import QONNXManager as BrevitasONNXManager
 from concrete.fhe.compilation.artifacts import DebugArtifacts
 from concrete.fhe.compilation.circuit import Circuit
 from concrete.fhe.compilation.compiler import Compiler
 from concrete.fhe.compilation.configuration import Configuration
 from concrete.fhe.dtypes.integer import Integer
 from sklearn.base import clone
-from skorch.net import NeuralNet as SkorchNeuralNet
 
 from ..common.check_inputs import check_array_and_assert, check_X_y_and_assert_multi_output
 from ..common.debugging.custom_assert import assert_true
-from ..common.serialization.encoder import CustomEncoder
+from ..common.serialization.dumpers import dump, dumps
 from ..common.utils import (
     FheMode,
     check_there_is_no_p_error_options_in_configuration,
     generate_proxy_function,
     manage_parameters_for_pbs_errors,
 )
 from ..onnx.convert import OPSET_VERSION_FOR_ONNX_EXPORT
@@ -133,14 +132,98 @@
 
         #: Indicate if the model is compiled.
         self._is_compiled: bool = False
 
         self.fhe_circuit_: Optional[Circuit] = None
         self.onnx_model_: Optional[onnx.ModelProto] = None
 
+    def __getattr__(self, attr: str):
+        """Get the model's attribute.
+
+        If the attribute's name ends with an underscore ("_"), get the attribute from the underlying
+        scikit-learn model as it represents a training attribute:
+        https://scikit-learn.org/stable/glossary.html#term-attributes
+
+        This method is only called if the attribute has not been found in the class instance:
+        https://docs.python.org/3/reference/datamodel.html?highlight=getattr#object.__getattr__
+
+        Args:
+            attr (str): The attribute's name.
+
+        Returns:
+            The attribute value.
+
+        Raises:
+            AttributeError: If the attribute cannot be found or is not a training attribute.
+        """
+
+        # If the attribute ends with a single underscore and can be found in the underlying
+        # scikit-learn model (once fitted), retrieve its value
+        if (
+            attr.endswith("_")
+            and not attr.endswith("__")
+            and getattr(self, "sklearn_model", None) is not None
+        ):
+            return getattr(self.sklearn_model, attr)
+
+        raise AttributeError(
+            f"Attribute {attr} cannot be found in the Concrete ML {self.__class__.__name__} object "
+            f"and is not a training attribute from the underlying scikit-learn "
+            f"{self.sklearn_model_class} one."
+        )
+
+    # We need to specifically call the default __setattr__ method as QNN models still inherit from
+    # skorch, which provides its own __setattr__ implementation and creates a cyclic loop
+    # with __getattr__. Removing this inheritance once and for all should fix the issue
+    # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3373
+    def __setattr__(self, name: str, value: Any):
+        """Set the value as a model attribute.
+
+        Args:
+            name (str): The attribute's name to consider.
+            value (Any): The attribute's value to consider.
+        """
+        object.__setattr__(self, name, value)
+
+    @abstractmethod
+    def dump_dict(self) -> Dict[str, Any]:
+        """Dump the object as a dict.
+
+        Returns:
+            Dict[str, Any]: Dict of serialized objects.
+        """
+
+    @classmethod
+    @abstractmethod
+    def load_dict(cls, metadata: Dict[str, Any]) -> BaseEstimator:
+        """Load itself from a dict.
+
+        Args:
+            metadata (Dict[str, Any]): Dict of serialized objects.
+
+        Returns:
+            BaseEstimator: The loaded object.
+        """
+
+    def dumps(self) -> str:
+        """Dump itself to a string.
+
+        Returns:
+            metadata (str): String of the serialized object.
+        """
+        return dumps(self)
+
+    def dump(self, file: TextIO) -> None:
+        """Dump itself to a file.
+
+        Args:
+            file (TextIO): The file to dump the serialized object into.
+        """
+        dump(self, file)
+
     @property
     def onnx_model(self) -> Optional[onnx.ModelProto]:
         """Get the ONNX model.
 
         Is None if the model is not fitted.
 
         Returns:
@@ -568,78 +651,14 @@
             y_preds (numpy.ndarray): The de-quantized predictions to post-process.
 
         Returns:
             numpy.ndarray: The post-processed predictions.
         """
         return y_preds
 
-    @abstractmethod
-    def dump_dict(self) -> Dict[str, Any]:
-        """Dump the object as a dict.
-
-        Returns:
-            Dict[str, Any]: a dict representing the object
-        """
-
-    def dumps(self) -> str:
-        """Dump itself to a string.
-
-        Returns:
-            metadata (str): string of serialized object
-        """
-        metadata: Dict[str, Any] = self.dump_dict()
-        return json.dumps(metadata, cls=CustomEncoder)
-
-    def dump(self, file: IO[str]) -> None:
-        """Dump itself to a file.
-
-        Args:
-            file (IO[str]): file of where to dump.
-        """
-        metadata: Dict[str, Any] = self.dump_dict()
-        json.dump(metadata, file, cls=CustomEncoder)
-
-    @classmethod
-    @abstractmethod
-    def load_dict(cls, metadata: Dict[str, Any]) -> BaseEstimator:
-        """Load itself from a dict.
-
-        Args:
-            metadata (Dict[str, Any]): dict of metadata of the object
-
-        Returns:
-            BaseEstimator: the loaded object
-        """
-
-    @classmethod
-    def load(cls, file: IO[str]) -> BaseEstimator:
-        """Load itself from a file.
-
-        Args:
-            file (IO[str]): file of serialized object
-
-        Returns:
-            BaseEstimator: the loaded object
-        """
-        metadata: Dict[str, Any] = json.load(file)
-        return cls.load_dict(metadata=metadata)
-
-    @classmethod
-    def loads(cls, metadata: str) -> BaseEstimator:
-        """Load itself from a string.
-
-        Args:
-            metadata (str): serialized object
-
-        Returns:
-            BaseEstimator: the loaded object
-        """
-        _metadata: Dict = json.loads(metadata)
-        return cls.load_dict(metadata=_metadata)
-
 
 # This class only is an equivalent of BaseEstimator applied to classifiers, therefore not all
 # methods are implemented and we need to disable pylint from checking that
 # pylint: disable-next=abstract-method
 class BaseClassifier(BaseEstimator):
     """Base class for linear and tree-based classifiers in Concrete ML.
 
@@ -726,16 +745,18 @@
         # Else, apply the softmax operator
         else:
             y_preds = numpy_softmax(y_preds)[0]
 
         return y_preds
 
 
-# QNNs do not support serialization yet
-# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3134
+# Pylint complains that this method does not override the `dump_dict` and `load_dict` methods. This
+# is expected as the QuantizedTorchEstimatorMixin class is not supposed to be used as such. This
+# disable could probably be removed when refactoring the serialization of models
+# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3250
 # pylint: disable-next=abstract-method
 class QuantizedTorchEstimatorMixin(BaseEstimator):
     """Mixin that provides quantization for a torch module and follows the Estimator API."""
 
     def __init_subclass__(cls):
         for klass in cls.__mro__:
             # pylint: disable-next=protected-access
@@ -750,15 +771,15 @@
 
         #: The input dimension in the underlying model
         self.module__input_dim: Optional[int] = None
 
         #: The number of outputs in the underlying model
         self.module__n_outputs: Optional[int] = None
 
-        super().__init__()
+        BaseEstimator.__init__(self)
 
     @property
     def base_module(self) -> SparseQuantNeuralNetwork:
         """Get the Torch module.
 
         Returns:
             SparseQuantNeuralNetwork: The fitted underlying module.
@@ -907,22 +928,20 @@
             self.base_module,
             input_shape=X[[0], ::].shape,
             export_path=str(output_onnx_file_path),
             keep_initializers_as_inputs=False,
             opset_version=OPSET_VERSION_FOR_ONNX_EXPORT,
         )
 
-        onnx_model = onnx.load(str(output_onnx_file_path))
+        self.onnx_model_ = onnx.load(str(output_onnx_file_path))
 
         output_onnx_file_path.unlink()
 
         # Create corresponding numpy model
-        numpy_model = NumpyModule(onnx_model, torch.tensor(X[[0], ::]))
-
-        self.onnx_model_ = numpy_model.onnx_model
+        numpy_model = NumpyModule(self.onnx_model_, torch.tensor(X[[0], ::]))
 
         # Set the quantization bits for import
         # Note that the ONNXConverter will use a default value for network input bits
         # Furthermore, Brevitas ONNX contains bit-widths in the ONNX file
         # which override the bit-width that we pass here
         # Thus, this parameter is only used to check consistency during import (onnx file vs import)
         n_bits = self.base_module.n_a_bits
@@ -972,19 +991,19 @@
                 # added as well
                 else:
                     activation_name = f"act{layer_index}"
                     float_module.add_module(activation_name, module)
 
         return float_module
 
-    def _get_equivalent_float_estimator(self) -> SkorchNeuralNet:
+    def _get_equivalent_float_estimator(self) -> skorch.net.NeuralNet:
         """Initialize a topologically equivalent estimator that can be used on floating points.
 
         Returns:
-            float_estimator (SkorchNeuralNet): An instance of the equivalent float estimator.
+            float_estimator (skorch.net.NeuralNet): An instance of the equivalent float estimator.
         """
         # Retrieve the skorch estimator's init parameters
         sklearn_params = self.get_params()
 
         # Retrieve all parameters related to the module
         module_param_names = [name for name in sklearn_params if "module__" in name]
```

## concrete/ml/sklearn/glm.py

```diff
@@ -1,23 +1,19 @@
 """Implement sklearn's Generalized Linear Models (GLM)."""
 from __future__ import annotations
 
 from abc import abstractmethod
 from typing import Any, Dict, Union
 
 import numpy
-from sklearn.linear_model import GammaRegressor as SklearnGammaRegressor
-from sklearn.linear_model import PoissonRegressor as SklearnPoissonRegressor
-from sklearn.linear_model import TweedieRegressor as SklearnTweedieRegressor
+import sklearn.linear_model
 
-from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
 from ..common.debugging.custom_assert import assert_true
 from ..common.utils import FheMode
 from ..onnx.onnx_model_manipulations import clean_graph_after_node_op_type
-from ..quantization.quantizers import UniformQuantizer
 from .base import Data, SklearnLinearRegressorMixin
 
 
 # pylint: disable-next=too-many-instance-attributes
 class _GeneralizedLinearRegressor(SklearnLinearRegressorMixin):
     """Regression via a penalized Generalized Linear Model (GLM) with FHE.
 
@@ -80,67 +76,59 @@
             y_preds (numpy.ndarray): The input data.
         """
 
     def dump_dict(self) -> Dict:
         assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
         metadata: Dict[str, Any] = {}
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["sklearn_model_class"] = self.sklearn_model_class
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["fhe_circuit"] = self.fhe_circuit
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["_weight_quantizer"] = self._weight_quantizer
+        metadata["output_quantizers"] = self.output_quantizers
         metadata["onnx_model_"] = self.onnx_model_
         metadata["_q_weights"] = self._q_weights
         metadata["_q_bias"] = self._q_bias
+        metadata["post_processing_params"] = self.post_processing_params
 
+        # Scikit-Learn
         metadata["alpha"] = self.alpha
         metadata["fit_intercept"] = self.fit_intercept
         metadata["solver"] = self.solver
         metadata["max_iter"] = self.max_iter
         metadata["tol"] = self.tol
         metadata["warm_start"] = self.warm_start
         metadata["verbose"] = self.verbose
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = cls(n_bits=metadata["n_bits"])
-
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
 
-        obj.post_processing_params = metadata["post_processing_params"]
+        # Instantiate the model
+        obj = cls(n_bits=metadata["n_bits"])
 
-        obj.fhe_circuit = metadata["fhe_circuit"]
+        # Concrete-ML
+        obj.n_bits = metadata["n_bits"]
+        obj.sklearn_model = metadata["sklearn_model"]
         obj.onnx_model_ = metadata["onnx_model_"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj._weight_quantizer = metadata["_weight_quantizer"]
+        obj.output_quantizers = metadata["output_quantizers"]
         obj._q_weights = metadata["_q_weights"]
         obj._q_bias = metadata["_q_bias"]
+        obj.post_processing_params = metadata["post_processing_params"]
 
-        obj.n_bits = metadata["n_bits"]
+        # Scikit-Learn
         obj.alpha = metadata["alpha"]
         obj.fit_intercept = metadata["fit_intercept"]
         obj.solver = metadata["solver"]
         obj.max_iter = metadata["max_iter"]
         obj.tol = metadata["tol"]
         obj.warm_start = metadata["warm_start"]
         obj.verbose = metadata["verbose"]
@@ -160,15 +148,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on PoissonRegressor please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.PoissonRegressor.html
     """
 
-    sklearn_model_class = SklearnPoissonRegressor
+    sklearn_model_class = sklearn.linear_model.PoissonRegressor
     _is_a_public_cml_model = True
 
     def __init__(
         self,
         *,
         n_bits: Union[int, dict] = 8,
         alpha: float = 1.0,
@@ -204,15 +192,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on GammaRegressor please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.GammaRegressor.html
     """
 
-    sklearn_model_class = SklearnGammaRegressor
+    sklearn_model_class = sklearn.linear_model.GammaRegressor
     _is_a_public_cml_model = True
 
     def __init__(
         self,
         *,
         n_bits: Union[int, dict] = 8,
         alpha: float = 1.0,
@@ -249,15 +237,15 @@
             - op_weights: number of bits to quantize the learned parameters
             Default to 8.
 
     For more details on TweedieRegressor please refer to the scikit-learn documentation:
     https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.TweedieRegressor.html
     """
 
-    sklearn_model_class = SklearnTweedieRegressor
+    sklearn_model_class = sklearn.linear_model.TweedieRegressor
     _is_a_public_cml_model = True
 
     def __init__(
         self,
         *,
         n_bits: Union[int, dict] = 8,
         power: float = 0.0,
@@ -313,58 +301,64 @@
 
         return y_preds
 
     def dump_dict(self) -> Dict:
         assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
         metadata: Dict[str, Any] = {}
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["sklearn_model_class"] = self.sklearn_model_class
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["fhe_circuit"] = self.fhe_circuit
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["_weight_quantizer"] = self._weight_quantizer
+        metadata["output_quantizers"] = self.output_quantizers
         metadata["onnx_model_"] = self.onnx_model_
         metadata["_q_weights"] = self._q_weights
         metadata["_q_bias"] = self._q_bias
-
+        metadata["post_processing_params"] = self.post_processing_params
         metadata["power"] = self.power
         metadata["link"] = self.link
 
+        # Scikit-Learn
+        metadata["alpha"] = self.alpha
+        metadata["fit_intercept"] = self.fit_intercept
+        metadata["solver"] = self.solver
+        metadata["max_iter"] = self.max_iter
+        metadata["tol"] = self.tol
+        metadata["warm_start"] = self.warm_start
+        metadata["verbose"] = self.verbose
+
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = cls(n_bits=metadata["n_bits"])
 
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
-
-        obj.post_processing_params = metadata["post_processing_params"]
+        # Instantiate the model
+        obj = cls(n_bits=metadata["n_bits"])
 
-        obj.fhe_circuit = metadata["fhe_circuit"]
+        # Concrete-ML
+        obj.sklearn_model = metadata["sklearn_model"]
         obj.onnx_model_ = metadata["onnx_model_"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj._weight_quantizer = metadata["_weight_quantizer"]
+        obj.output_quantizers = metadata["output_quantizers"]
         obj._q_weights = metadata["_q_weights"]
         obj._q_bias = metadata["_q_bias"]
-
         obj.power = metadata["power"]
         obj.link = metadata["link"]
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Scikit-Learn
+        obj.alpha = metadata["alpha"]
+        obj.fit_intercept = metadata["fit_intercept"]
+        obj.solver = metadata["solver"]
+        obj.max_iter = metadata["max_iter"]
+        obj.tol = metadata["tol"]
+        obj.warm_start = metadata["warm_start"]
+        obj.verbose = metadata["verbose"]
 
         return obj
```

## concrete/ml/sklearn/linear_model.py

```diff
@@ -1,16 +1,12 @@
 """Implement sklearn linear model."""
 from typing import Any, Dict
 
-import numpy
-import sklearn
 import sklearn.linear_model
 
-from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
-from ..quantization.quantizers import UniformQuantizer
 from .base import SklearnLinearClassifierMixin, SklearnLinearRegressorMixin
 
 
 # pylint: disable=invalid-name,too-many-instance-attributes
 class LinearRegression(SklearnLinearRegressorMixin):
     """A linear regression model with FHE.
 
@@ -50,68 +46,56 @@
         self.positive = positive
 
     def dump_dict(self) -> Dict[str, Any]:
         assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = type(self).__name__
-
-        # Linear
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["sklearn_model_class"] = self.sklearn_model_class
-        metadata["fhe_circuit"] = self.fhe_circuit
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["_weight_quantizer"] = self._weight_quantizer
+        metadata["output_quantizers"] = self.output_quantizers
         metadata["onnx_model_"] = self.onnx_model_
         metadata["_q_weights"] = self._q_weights
         metadata["_q_bias"] = self._q_bias
+        metadata["post_processing_params"] = self.post_processing_params
 
+        # Scikit-Learn
         metadata["fit_intercept"] = self.fit_intercept
         metadata["normalize"] = self.normalize
         metadata["copy_X"] = self.copy_X
         metadata["n_jobs"] = self.n_jobs
         metadata["positive"] = self.positive
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = LinearRegression()
-        obj.post_processing_params = metadata["post_processing_params"]
 
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
+        # Instantiate the model
+        obj = LinearRegression()
 
-        # Linear
+        # Concrete-ML
         obj.n_bits = metadata["n_bits"]
-        obj.sklearn_model_class = metadata["sklearn_model_class"]
-        obj.fhe_circuit = metadata["fhe_circuit"]
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
-        obj.onnx_model_ = metadata["onnx_model_"]
+        obj.sklearn_model = metadata["sklearn_model"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.output_quantizers = metadata["output_quantizers"]
+        obj._weight_quantizer = metadata["_weight_quantizer"]
+        obj.onnx_model_ = metadata["onnx_model_"]
         obj._q_weights = metadata["_q_weights"]
         obj._q_bias = metadata["_q_bias"]
+        obj.post_processing_params = metadata["post_processing_params"]
 
-        # Custom
+        # Scikit-Learn
         obj.fit_intercept = metadata["fit_intercept"]
         obj.normalize = metadata["normalize"]
         obj.copy_X = metadata["copy_X"]
         obj.n_jobs = metadata["n_jobs"]
         obj.positive = metadata["positive"]
         return obj
 
@@ -169,31 +153,28 @@
         self.selection = selection
 
     def dump_dict(self) -> Dict[str, Any]:
         assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = type(self).__name__
-
-        # Linear
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["sklearn_model_class"] = self.sklearn_model_class
-        metadata["fhe_circuit"] = self.fhe_circuit
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["_weight_quantizer"] = self._weight_quantizer
+        metadata["output_quantizers"] = self.output_quantizers
         metadata["onnx_model_"] = self.onnx_model_
         metadata["_q_weights"] = self._q_weights
         metadata["_q_bias"] = self._q_bias
+        metadata["post_processing_params"] = self.post_processing_params
 
+        # Scikit-Learn
         metadata["alpha"] = self.alpha
         metadata["l1_ratio"] = self.l1_ratio
         metadata["fit_intercept"] = self.fit_intercept
         metadata["normalize"] = self.normalize
         metadata["copy_X"] = self.copy_X
         metadata["positive"] = self.positive
         metadata["precompute"] = self.precompute
@@ -203,40 +184,32 @@
         metadata["random_state"] = self.random_state
         metadata["selection"] = self.selection
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = ElasticNet()
-        obj.post_processing_params = metadata["post_processing_params"]
 
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
+        # Instantiate the model
+        obj = ElasticNet()
 
-        # Linear
+        # Concrete-ML
         obj.n_bits = metadata["n_bits"]
-        obj.sklearn_model_class = metadata["sklearn_model_class"]
-        obj.fhe_circuit = metadata["fhe_circuit"]
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
-        obj.onnx_model_ = metadata["onnx_model_"]
+        obj.sklearn_model = metadata["sklearn_model"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.output_quantizers = metadata["output_quantizers"]
+        obj._weight_quantizer = metadata["_weight_quantizer"]
+        obj.onnx_model_ = metadata["onnx_model_"]
         obj._q_weights = metadata["_q_weights"]
         obj._q_bias = metadata["_q_bias"]
+        obj.post_processing_params = metadata["post_processing_params"]
 
+        # Scikit-Learn
         obj.alpha = metadata["alpha"]
         obj.l1_ratio = metadata["l1_ratio"]
         obj.fit_intercept = metadata["fit_intercept"]
         obj.normalize = metadata["normalize"]
         obj.copy_X = metadata["copy_X"]
         obj.positive = metadata["positive"]
         obj.precompute = metadata["precompute"]
@@ -300,31 +273,28 @@
         self.random_state = random_state
 
     def dump_dict(self) -> Dict[str, Any]:
         assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = type(self).__name__
-
-        # Linear
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["sklearn_model_class"] = self.sklearn_model_class
-        metadata["fhe_circuit"] = self.fhe_circuit
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["_weight_quantizer"] = self._weight_quantizer
+        metadata["output_quantizers"] = self.output_quantizers
         metadata["onnx_model_"] = self.onnx_model_
         metadata["_q_weights"] = self._q_weights
         metadata["_q_bias"] = self._q_bias
+        metadata["post_processing_params"] = self.post_processing_params
 
+        # Scikit-Learn
         metadata["alpha"] = self.alpha
         metadata["fit_intercept"] = self.fit_intercept
         metadata["normalize"] = self.normalize
         metadata["copy_X"] = self.copy_X
         metadata["positive"] = self.positive
         metadata["max_iter"] = self.max_iter
         metadata["warm_start"] = self.warm_start
@@ -333,40 +303,32 @@
         metadata["precompute"] = self.precompute
         metadata["random_state"] = self.random_state
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = Lasso()
-        obj.post_processing_params = metadata["post_processing_params"]
 
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
+        # Instantiate the model
+        obj = Lasso()
 
-        # Linear
+        # Concrete-ML
         obj.n_bits = metadata["n_bits"]
-        obj.sklearn_model_class = metadata["sklearn_model_class"]
-        obj.fhe_circuit = metadata["fhe_circuit"]
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
-        obj.onnx_model_ = metadata["onnx_model_"]
+        obj.sklearn_model = metadata["sklearn_model"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.output_quantizers = metadata["output_quantizers"]
+        obj._weight_quantizer = metadata["_weight_quantizer"]
+        obj.onnx_model_ = metadata["onnx_model_"]
         obj._q_weights = metadata["_q_weights"]
         obj._q_bias = metadata["_q_bias"]
+        obj.post_processing_params = metadata["post_processing_params"]
 
+        # Scikit-Learn
         obj.alpha = metadata["alpha"]
         obj.fit_intercept = metadata["fit_intercept"]
         obj.normalize = metadata["normalize"]
         obj.copy_X = metadata["copy_X"]
         obj.positive = metadata["positive"]
         obj.max_iter = metadata["max_iter"]
         obj.warm_start = metadata["warm_start"]
@@ -425,71 +387,60 @@
         self.random_state = random_state
 
     def dump_dict(self) -> Dict[str, Any]:
         assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = type(self).__name__
-
-        # Linear
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["sklearn_model_class"] = self.sklearn_model_class
-        metadata["fhe_circuit"] = self.fhe_circuit
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["_weight_quantizer"] = self._weight_quantizer
+        metadata["output_quantizers"] = self.output_quantizers
         metadata["onnx_model_"] = self.onnx_model_
         metadata["_q_weights"] = self._q_weights
         metadata["_q_bias"] = self._q_bias
+        metadata["post_processing_params"] = self.post_processing_params
 
+        # Scikit-Learn
         metadata["alpha"] = self.alpha
         metadata["fit_intercept"] = self.fit_intercept
         metadata["normalize"] = self.normalize
         metadata["copy_X"] = self.copy_X
         metadata["positive"] = self.positive
         metadata["max_iter"] = self.max_iter
         metadata["tol"] = self.tol
         metadata["solver"] = self.solver
         metadata["random_state"] = self.random_state
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = Ridge()
-        obj.post_processing_params = metadata["post_processing_params"]
 
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
+        # Instantiate the model
+        obj = Ridge()
 
-        # Linear
+        # Concrete-ML
         obj.n_bits = metadata["n_bits"]
-        obj.sklearn_model_class = metadata["sklearn_model_class"]
-        obj.fhe_circuit = metadata["fhe_circuit"]
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
-        obj.onnx_model_ = metadata["onnx_model_"]
+        obj.sklearn_model = metadata["sklearn_model"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.output_quantizers = metadata["output_quantizers"]
+        obj._weight_quantizer = metadata["_weight_quantizer"]
+        obj.onnx_model_ = metadata["onnx_model_"]
         obj._q_weights = metadata["_q_weights"]
         obj._q_bias = metadata["_q_bias"]
+        obj.post_processing_params = metadata["post_processing_params"]
 
+        # Scikit-Learn
         obj.alpha = metadata["alpha"]
         obj.fit_intercept = metadata["fit_intercept"]
         obj.normalize = metadata["normalize"]
         obj.copy_X = metadata["copy_X"]
         obj.positive = metadata["positive"]
         obj.max_iter = metadata["max_iter"]
         obj.tol = metadata["tol"]
@@ -557,37 +508,32 @@
         self.l1_ratio = l1_ratio
 
     def dump_dict(self) -> Dict[str, Any]:
         assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = type(self).__name__
-
-        # Classifier
-        metadata["classes_"] = self.target_classes_
-        metadata["n_classes_"] = self.n_classes_
-        metadata["cml_dumped_class_name"] = type(self).__name__
-
-        # Linear
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["sklearn_model_class"] = self.sklearn_model_class
-        metadata["fhe_circuit"] = self.fhe_circuit
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["_weight_quantizer"] = self._weight_quantizer
+        metadata["output_quantizers"] = self.output_quantizers
         metadata["onnx_model_"] = self.onnx_model_
         metadata["_q_weights"] = self._q_weights
         metadata["_q_bias"] = self._q_bias
+        metadata["post_processing_params"] = self.post_processing_params
 
-        # Specific
+        # Classifier
+        metadata["target_classes_"] = self.target_classes_
+        metadata["n_classes_"] = self.n_classes_
+
+        # Scikit-Learn
         metadata["penalty"] = self.penalty
         metadata["dual"] = self.dual
         metadata["tol"] = self.tol
         metadata["C"] = self.C
         metadata["fit_intercept"] = self.fit_intercept
         metadata["intercept_scaling"] = self.intercept_scaling
         metadata["class_weight"] = self.class_weight
@@ -600,44 +546,35 @@
         metadata["n_jobs"] = self.n_jobs
         metadata["l1_ratio"] = self.l1_ratio
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
+        # Instantiate the model
         obj = LogisticRegression()
-        obj.post_processing_params = metadata["post_processing_params"]
-
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
-
-        # Classifier
-        obj.target_classes_ = numpy.array(metadata["classes_"])
-        obj.n_classes_ = metadata["n_classes_"]
 
-        # Linear
+        # Concrete-ML
         obj.n_bits = metadata["n_bits"]
-        obj.sklearn_model_class = metadata["sklearn_model_class"]
-        obj.fhe_circuit = metadata["fhe_circuit"]
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
-        obj.onnx_model_ = metadata["onnx_model_"]
+        obj.sklearn_model = metadata["sklearn_model"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.output_quantizers = metadata["output_quantizers"]
+        obj._weight_quantizer = metadata["_weight_quantizer"]
+        obj.onnx_model_ = metadata["onnx_model_"]
         obj._q_weights = metadata["_q_weights"]
         obj._q_bias = metadata["_q_bias"]
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Classifier
+        obj.target_classes_ = metadata["target_classes_"]
+        obj.n_classes_ = metadata["n_classes_"]
 
+        # Scikit-Learn
         obj.penalty = metadata["penalty"]
         obj.dual = metadata["dual"]
         obj.tol = metadata["tol"]
         obj.C = metadata["C"]
         obj.fit_intercept = metadata["fit_intercept"]
         obj.intercept_scaling = metadata["intercept_scaling"]
         obj.class_weight = metadata["class_weight"]
```

## concrete/ml/sklearn/qnn.py

```diff
@@ -1,30 +1,56 @@
 """Scikit-learn interface for fully-connected quantized neural networks."""
 
 # Disable pylint invalid name since scikit learn uses "X" as variable name for data
 # pylint: disable=invalid-name
 
-from typing import Any, Dict, Union
+import io
+from typing import Any, Callable, Dict, Union
 
 import numpy
+import skorch.classifier
+import skorch.regressor
 import torch
-from skorch.classifier import NeuralNetClassifier as SkorchNeuralNetClassifier
 from skorch.dataset import Dataset, ValidSplit
-from skorch.regressor import NeuralNetRegressor as SkorchNeuralNetRegressor
 from torch.utils.data import DataLoader
 
 from ..common.debugging import assert_true
 from ..common.utils import FheMode, check_dtype_and_cast
 from .base import QNN_AUTO_KWARGS, BaseClassifier, Data, QuantizedTorchEstimatorMixin, Target
 
 # Define the QNN's support float and int dtypes
 QNN_FLOAT_DTYPE = numpy.float32
 QNN_INT_DTYPE = numpy.int64
 
+# The different init parameters for the SparseQuantNeuralNetwork module
+OPTIONAL_MODULE_PARAMS = [
+    "n_hidden_neurons_multiplier",
+    "n_w_bits",
+    "n_a_bits",
+    "n_accum_bits",
+    "n_prune_neurons_percentage",
+    "activation_function",
+    "quant_narrow",
+    "quant_signed",
+]
+
+# skorch's special attribute prefixes, which can be found in:
+# https://skorch.readthedocs.io/en/v0.10.0/user/neuralnet.html#special-arguments
+# Criterion and optimizer are handled separately using skorch's native `save_params` and
+# `load_params` methods
+ATTRIBUTE_PREFIXES = [
+    "iterator_train",
+    "iterator_valid",
+    "callbacks",
+    "dataset",
+]
 
+
+# We should also check that the `module__n_layers` parameter is properly set
+# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3553
 def _check_qnn_kwargs(input_kwargs: Dict[str, Any]) -> None:
     """Check that a QNN model is not constructed with automatically computed parameters.
 
     Args:
         input_kwargs (dict): The keyword arguments to check.
 
     Raises:
@@ -43,37 +69,35 @@
             "Setting `module` manually is forbidden. The module is set automatically when "
             "initializing the instance."
         )
 
     for auto_kwarg in QNN_AUTO_KWARGS:
         if auto_kwarg in input_kwargs:
             raise ValueError(
-                f" Setting `{auto_kwarg}` manually is forbidden. The number of inputs and outputs "
+                f"Setting `{auto_kwarg}` manually is forbidden. The number of inputs and outputs "
                 "of the neural network are determined automatically in .fit, based on the data-set."
             )
 
 
-# QNNs do not support serialization yet
-# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3134
-# pylint: disable-next=too-many-instance-attributes, abstract-method
-class NeuralNetRegressor(QuantizedTorchEstimatorMixin, SkorchNeuralNetRegressor):
+# pylint: disable-next=too-many-instance-attributes
+class NeuralNetRegressor(QuantizedTorchEstimatorMixin, skorch.regressor.NeuralNetRegressor):
     """A Fully-Connected Neural Network regressor with FHE.
 
     This class wraps a quantized neural network implemented using Torch tools as a scikit-learn
     estimator. The skorch package allows to handle training and scikit-learn compatibility,
     and adds quantization as well as compilation functionalities. The neural network implemented
     by this class is a multi layer fully connected network trained with Quantization Aware Training
     (QAT).
 
     Inputs and targets that are float64 will be casted to float32 before training as Torch does not
     handle float64 types properly. Thus should not have a significant impact on the model's
     performances. An error is raised if these values are not floating points.
     """
 
-    sklearn_model_class = SkorchNeuralNetRegressor
+    sklearn_model_class = skorch.regressor.NeuralNetRegressor
     _is_a_public_cml_model = True
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         criterion=torch.nn.MSELoss,
         optimizer=torch.optim.Adam,
@@ -169,34 +193,216 @@
         X = check_dtype_and_cast(X, "float32", error_information="Neural Network regressor input")
 
         # Call BaseEstimator's predict method and cast values to float32
         y_preds = super().predict(X, fhe=fhe)
         y_preds = self.post_processing(y_preds)
         return y_preds
 
+    def dump_dict(self) -> Dict[str, Any]:
+        metadata: Dict[str, Any] = {}
+
+        # Save the model's weights/biases, optimizer and criterion attributes as well as their
+        # related special arguments
+        if self.sklearn_model is not None:
+
+            # skorch's native `save_params` method dumps the objects into a file by default. In
+            # order to avoid creating new files, we instead provide the method a buffer that we
+            # then convert to a byte string and save it in the serialized json
+            with io.BytesIO() as params, io.BytesIO() as optimizer, io.BytesIO() as criterion:
+
+                # Make pruning permanent by removing weights associated to pruned neurons as Torch
+                # does not allow to easily load and save pruned networks
+                # https://discuss.pytorch.org/t/proper-way-to-load-a-pruned-network/77694
+                self.base_module.make_pruning_permanent()
+
+                # We follow skorch's recommendation for saving and loading their models:
+                # https://skorch.readthedocs.io/en/stable/user/save_load.html
+                self.sklearn_model.save_params(
+                    f_params=params,
+                    f_optimizer=optimizer,
+                    f_criterion=criterion,
+                )
+
+                metadata["params"] = params.getvalue().hex()
+                metadata["optimizer"] = optimizer.getvalue().hex()
+                metadata["criterion"] = criterion.getvalue().hex()
+
+        # Concrete-ML
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["quantized_module_"] = self.quantized_module_
+        metadata["post_processing_params"] = self.post_processing_params
+
+        # skorch attributes that cannot be serialized
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3550
+        # Disable mypy as running isinstance with a Callable type unexpectedly raises an issue:
+        # https://github.com/python/mypy/issues/3060
+        if isinstance(self.train_split, Callable) and not isinstance(  # type: ignore[arg-type]
+            self.train_split, ValidSplit
+        ):
+            raise NotImplementedError(
+                "Serializing a custom Callable object is not secure and is therefore disabled. "
+                "Please set `train_split` to either None or a ValidSplit instance."
+            )
+
+        if self.callbacks != "disable":
+            raise NotImplementedError(
+                "Serializing a custom Callable object is not secure and is therefore disabled. "
+                "Additionally, the serialization of skorch's different callback classes is not "
+                f"supported. Please set `callbacks` to 'disable'. Got {self.callbacks}."
+            )
+
+        # Disable mypy as running isinstance with a Callable type unexpectedly raises an issue:
+        # https://github.com/python/mypy/issues/3060
+        if isinstance(self.predict_nonlinearity, Callable):  # type: ignore[arg-type]
+            raise NotImplementedError(
+                "Serializing a custom Callable object is not secure and is therefore disabled. "
+                "Please set`predict_nonlinearity` to either None or 'auto'."
+            )
+
+        # skorch
+        metadata["lr"] = self.lr
+        metadata["max_epochs"] = self.max_epochs
+        metadata["batch_size"] = self.batch_size
+        metadata["iterator_train"] = self.iterator_train
+        metadata["iterator_valid"] = self.iterator_valid
+        metadata["dataset"] = self.dataset
+        metadata["train_split"] = self.train_split
+        metadata["callbacks"] = self.callbacks
+        metadata["predict_nonlinearity"] = self.predict_nonlinearity
+        metadata["warm_start"] = self.warm_start
+        metadata["verbose"] = self.verbose
+        metadata["device"] = self.device
+        metadata["history_"] = self.history_
+        metadata["initialized_"] = self.initialized_
+        metadata["virtual_params_"] = self.virtual_params_
+
+        assert hasattr(
+            self, "module__n_layers"
+        ), f"{self.__class__.__name__} was not properly initialized."
+
+        # skorch special argument (mandatory) for module : SparseQuantNeuralNetwork
+        # pylint: disable-next=no-member
+        metadata["module__n_layers"] = self.module__n_layers
+        metadata["module__input_dim"] = self.module__input_dim
+        metadata["module__n_outputs"] = self.module__n_outputs
+
+        # skorch special argument (optional) for module : SparseQuantNeuralNetwork
+        for module_param in OPTIONAL_MODULE_PARAMS:
+            module_attribute = f"module__{module_param}"
+            if hasattr(self, module_attribute):
+                metadata[module_attribute] = getattr(self, module_attribute)
+
+        # skorch special arguments
+        # Coverage is disabled here as refactoring the serialization feature should remove this
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3250
+        for attribute_prefix in ATTRIBUTE_PREFIXES:  # pragma: no cover
+            for qnn_attribute in vars(self):
+                if qnn_attribute.startswith(f"{attribute_prefix}__"):
+                    metadata[qnn_attribute] = getattr(self, qnn_attribute)
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        # Instantiate the model
+        obj = NeuralNetRegressor(
+            module__n_layers=metadata["module__n_layers"],
+        )
+
+        # Concrete-ML
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.output_quantizers = metadata["output_quantizers"]
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj.quantized_module_ = metadata["quantized_module_"]
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # skorch
+        obj.lr = metadata["lr"]
+        obj.max_epochs = metadata["max_epochs"]
+        obj.batch_size = metadata["batch_size"]
+        obj.iterator_train = metadata["iterator_train"]
+        obj.iterator_valid = metadata["iterator_valid"]
+        obj.dataset = metadata["dataset"]
+        obj.train_split = metadata["train_split"]
+        obj.callbacks = metadata["callbacks"]
+        obj.predict_nonlinearity = metadata["predict_nonlinearity"]
+        obj.warm_start = metadata["warm_start"]
+        obj.verbose = metadata["verbose"]
+        obj.device = metadata["device"]
+        obj.history_ = metadata["history_"]
+        obj.initialized_ = metadata["initialized_"]
+        obj.virtual_params_ = metadata["virtual_params_"]
+
+        # skorch special argument (mandatory) for module : SparseQuantNeuralNetwork
+        obj.module__input_dim = metadata["module__input_dim"]
+        obj.module__n_outputs = metadata["module__n_outputs"]
+
+        # skorch special argument (optional) for module : SparseQuantNeuralNetwork
+        for module_param in OPTIONAL_MODULE_PARAMS:
+            module_attribute = f"module__{module_param}"
+            if module_attribute in metadata:
+                setattr(obj, module_attribute, metadata[module_attribute])
+
+        # skorch special arguments
+        # Coverage is disabled here as refactoring the serialization feature should remove this
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3250
+        for attribute_prefix in ATTRIBUTE_PREFIXES:  # pragma: no cover
+            for qnn_attribute, qnn_value in metadata.items():
+                if qnn_attribute.startswith(f"{attribute_prefix}__"):
+                    setattr(obj, qnn_attribute, qnn_value)
+
+        if "params" in metadata and "optimizer" in metadata and "criterion" in metadata:
+            # Initialize the underlying model
+            # We follow skorch's recommendation for saving and loading their models:
+            # https://skorch.readthedocs.io/en/stable/user/save_load.html
+            params = obj.get_sklearn_params()
+            obj.sklearn_model = obj.sklearn_model_class(**params)
+            obj.sklearn_model.initialize()
+
+            # Make pruning permanent by removing weights associated to pruned neurons as Torch
+            # does not allow to easily load and save pruned networks
+            # https://discuss.pytorch.org/t/proper-way-to-load-a-pruned-network/77694
+            obj.base_module.make_pruning_permanent()
+
+            # Load the model's weights/biases, optimizer and criterion attributes as well as their
+            # related special arguments
+            obj.sklearn_model.load_params(
+                f_params=io.BytesIO(bytes.fromhex(metadata["params"])),
+                f_optimizer=io.BytesIO(bytes.fromhex(metadata["optimizer"])),
+                f_criterion=io.BytesIO(bytes.fromhex(metadata["criterion"])),
+            )
+
+        return obj
+
 
-# QNNs do not support serialization yet
-# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3134
-# pylint: disable-next=too-many-instance-attributes, abstract-method
-class NeuralNetClassifier(BaseClassifier, QuantizedTorchEstimatorMixin, SkorchNeuralNetClassifier):
+# pylint: disable-next=too-many-instance-attributes
+class NeuralNetClassifier(
+    BaseClassifier, QuantizedTorchEstimatorMixin, skorch.classifier.NeuralNetClassifier
+):
     """A Fully-Connected Neural Network classifier with FHE.
 
     This class wraps a quantized neural network implemented using Torch tools as a scikit-learn
     estimator. The skorch package allows to handle training and scikit-learn compatibility,
     and adds quantization as well as compilation functionalities. The neural network implemented
     by this class is a multi layer fully connected network trained with Quantization Aware Training
     (QAT).
 
     Inputs that are float64 will be casted to float32 before training as Torch does not
     handle float64 types properly. Thus should not have a significant impact on the model's
     performances. If the targets are integers of lower bit-width, they will be safely casted to
     int64. Else, an error is raised.
     """
 
-    sklearn_model_class = SkorchNeuralNetClassifier
+    sklearn_model_class = skorch.classifier.NeuralNetClassifier
     _is_a_public_cml_model = True
 
     # pylint: disable=too-many-arguments
     def __init__(
         self,
         criterion=torch.nn.CrossEntropyLoss,
         optimizer=torch.optim.Adam,
@@ -297,7 +503,197 @@
     def predict(self, X: Data, fhe: Union[FheMode, str] = FheMode.DISABLE) -> numpy.ndarray:
         # Check that inputs are float32. If they are float64, they will be casted to float32 as
         # this should not have a great impact on the model's performances. Else, an error is raised.
         X = check_dtype_and_cast(X, "float32", error_information="Neural Network classifier input")
 
         # Call BaseClassifier's predict method
         return super().predict(X, fhe=fhe)
+
+    def dump_dict(self) -> Dict[str, Any]:
+        metadata: Dict[str, Any] = {}
+
+        # Save the model's weights/biases, optimizer and criterion attributes as well as their
+        # related special arguments
+        if self.sklearn_model is not None:
+
+            # skorch's native `save_params` method dumps the objects into a file by default. In
+            # order to avoid creating new files, we instead provide the method a buffer that we
+            # then convert to a byte string and save it in the serialized json
+            with io.BytesIO() as params, io.BytesIO() as optimizer, io.BytesIO() as criterion:
+
+                # Make pruning permanent by removing weights associated to pruned neurons as Torch
+                # does not allow to easily load and save pruned networks
+                # https://discuss.pytorch.org/t/proper-way-to-load-a-pruned-network/77694
+                self.base_module.make_pruning_permanent()
+
+                # We follow skorch's recommendation for saving and loading their models:
+                # https://skorch.readthedocs.io/en/stable/user/save_load.html
+                self.sklearn_model.save_params(
+                    f_params=params,
+                    f_optimizer=optimizer,
+                    f_criterion=criterion,
+                )
+
+                metadata["params"] = params.getvalue().hex()
+                metadata["optimizer"] = optimizer.getvalue().hex()
+                metadata["criterion"] = criterion.getvalue().hex()
+
+        # Concrete-ML
+        metadata["_is_fitted"] = self._is_fitted
+        metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["onnx_model_"] = self.onnx_model_
+        metadata["quantized_module_"] = self.quantized_module_
+        metadata["post_processing_params"] = self.post_processing_params
+
+        # Classifier
+        metadata["target_classes_"] = self.target_classes_
+        metadata["n_classes_"] = self.n_classes_
+
+        # skorch attributes that cannot be serialized
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3550
+        # Disable mypy as running isinstance with a Callable type unexpectedly raises an issue:
+        # https://github.com/python/mypy/issues/3060
+        if isinstance(self.train_split, Callable) and not isinstance(  # type: ignore[arg-type]
+            self.train_split, ValidSplit
+        ):
+            raise NotImplementedError(
+                "Serializing a custom Callable object is not secure and is therefore disabled. "
+                "Please set `train_split` to either None or a ValidSplit instance."
+            )
+
+        if self.callbacks != "disable":
+            raise NotImplementedError(
+                "Serializing a custom Callable object is not secure and is therefore disabled. "
+                "Additionally, the serialization of skorch's different callback classes is not "
+                f"supported. Please set `callbacks` to 'disable'. Got {self.callbacks}."
+            )
+
+        # Disable mypy as running isinstance with a Callable type unexpectedly raises an issue:
+        # https://github.com/python/mypy/issues/3060
+        if isinstance(self.predict_nonlinearity, Callable):  # type: ignore[arg-type]
+            raise NotImplementedError(
+                "Serializing a custom Callable object is not secure and is therefore disabled. "
+                "Please set`predict_nonlinearity` to either None or 'auto'."
+            )
+
+        # skorch
+        metadata["lr"] = self.lr
+        metadata["max_epochs"] = self.max_epochs
+        metadata["batch_size"] = self.batch_size
+        metadata["iterator_train"] = self.iterator_train
+        metadata["iterator_valid"] = self.iterator_valid
+        metadata["dataset"] = self.dataset
+        metadata["train_split"] = self.train_split
+        metadata["callbacks"] = self.callbacks
+        metadata["predict_nonlinearity"] = self.predict_nonlinearity
+        metadata["warm_start"] = self.warm_start
+        metadata["verbose"] = self.verbose
+        metadata["device"] = self.device
+        metadata["history_"] = self.history_
+        metadata["initialized_"] = self.initialized_
+        metadata["virtual_params_"] = self.virtual_params_
+
+        assert hasattr(
+            self, "module__n_layers"
+        ), f"{self.__class__.__name__} was not properly initialized."
+
+        # skorch special argument (mandatory) for module : SparseQuantNeuralNetwork
+        # pylint: disable-next=no-member
+        metadata["module__n_layers"] = self.module__n_layers
+        metadata["module__input_dim"] = self.module__input_dim
+        metadata["module__n_outputs"] = self.module__n_outputs
+
+        # skorch special argument (optional) for module : SparseQuantNeuralNetwork
+        for module_param in OPTIONAL_MODULE_PARAMS:
+            module_attribute = f"module__{module_param}"
+            if hasattr(self, module_attribute):
+                metadata[module_attribute] = getattr(self, module_attribute)
+
+        # skorch special arguments
+        # Coverage is disabled here as refactoring the serialization feature should remove this
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3250
+        for attribute_prefix in ATTRIBUTE_PREFIXES:  # pragma: no cover
+            for qnn_attribute in vars(self):
+                if qnn_attribute.startswith(f"{attribute_prefix}__"):
+                    metadata[qnn_attribute] = getattr(self, qnn_attribute)
+
+        return metadata
+
+    @classmethod
+    def load_dict(cls, metadata: Dict):
+        # Instantiate the model
+        obj = NeuralNetClassifier(
+            module__n_layers=metadata["module__n_layers"],
+        )
+
+        # Concrete-ML
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.output_quantizers = metadata["output_quantizers"]
+        obj.onnx_model_ = metadata["onnx_model_"]
+        obj.quantized_module_ = metadata["quantized_module_"]
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Classifier
+        obj.target_classes_ = metadata["target_classes_"]
+        obj.n_classes_ = metadata["n_classes_"]
+
+        # skorch
+        obj.lr = metadata["lr"]
+        obj.max_epochs = metadata["max_epochs"]
+        obj.batch_size = metadata["batch_size"]
+        obj.iterator_train = metadata["iterator_train"]
+        obj.iterator_valid = metadata["iterator_valid"]
+        obj.dataset = metadata["dataset"]
+        obj.train_split = metadata["train_split"]
+        obj.callbacks = metadata["callbacks"]
+        obj.predict_nonlinearity = metadata["predict_nonlinearity"]
+        obj.warm_start = metadata["warm_start"]
+        obj.verbose = metadata["verbose"]
+        obj.device = metadata["device"]
+        obj.history_ = metadata["history_"]
+        obj.initialized_ = metadata["initialized_"]
+        obj.virtual_params_ = metadata["virtual_params_"]
+
+        # skorch special argument (mandatory) for module : SparseQuantNeuralNetwork
+        obj.module__input_dim = metadata["module__input_dim"]
+        obj.module__n_outputs = metadata["module__n_outputs"]
+
+        # skorch special argument (optional) for module : SparseQuantNeuralNetwork
+        for module_param in OPTIONAL_MODULE_PARAMS:
+            module_attribute = f"module__{module_param}"
+            if module_attribute in metadata:
+                setattr(obj, module_attribute, metadata[module_attribute])
+
+        # skorch special arguments
+        # Coverage is disabled here as refactoring the serialization feature should remove this
+        # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/3250
+        for attribute_prefix in ATTRIBUTE_PREFIXES:  # pragma: no cover
+            for qnn_attribute, qnn_value in metadata.items():
+                if qnn_attribute.startswith(f"{attribute_prefix}__"):
+                    setattr(obj, qnn_attribute, qnn_value)
+
+        if "params" in metadata and "optimizer" in metadata and "criterion" in metadata:
+            # Initialize the underlying model
+            # We follow skorch's recommendation for saving and loading their models:
+            # https://skorch.readthedocs.io/en/stable/user/save_load.html
+            params = obj.get_sklearn_params()
+            obj.sklearn_model = obj.sklearn_model_class(**params)
+            obj.sklearn_model.initialize()
+
+            # Make pruning permanent by removing weights associated to pruned neurons as Torch
+            # does not allow to easily load and save pruned networks
+            # https://discuss.pytorch.org/t/proper-way-to-load-a-pruned-network/77694
+            obj.base_module.make_pruning_permanent()
+
+            # Load the model's weights/biases, optimizer and criterion attributes as well as their
+            # related special arguments
+            obj.sklearn_model.load_params(
+                f_params=io.BytesIO(bytes.fromhex(metadata["params"])),
+                f_optimizer=io.BytesIO(bytes.fromhex(metadata["optimizer"])),
+                f_criterion=io.BytesIO(bytes.fromhex(metadata["criterion"])),
+            )
+
+        return obj
```

## concrete/ml/sklearn/qnn_module.py

```diff
@@ -1,8 +1,10 @@
 """Sparse Quantized Neural Network torch module."""
+from typing import Set, Type
+
 import brevitas.nn as qnn
 import numpy
 import torch
 import torch.nn.utils.prune as pruning
 from torch import nn
 
 from ..common.debugging import assert_true
@@ -14,57 +16,58 @@
 
     This class implements an MLP that is compatible with FHE constraints. The weights and
     activations are quantized to low bit-width and pruning is used to ensure accumulators do not
     surpass an user-provided accumulator bit-width. The number of classes and number of layers
     are specified by the user, as well as the breadth of the network
     """
 
+    # pylint: disable-next=too-many-arguments
     def __init__(
         self,
-        input_dim,
-        n_layers,
-        n_outputs,
-        n_hidden_neurons_multiplier=4,
-        n_w_bits=3,
-        n_a_bits=3,
-        n_accum_bits=MAX_BITWIDTH_BACKWARD_COMPATIBLE,
-        n_prune_neurons_percentage=0.0,
-        activation_function=nn.ReLU,
-        quant_narrow=False,
-        quant_signed=True,
-    ):  # pylint: disable=too-many-arguments
+        input_dim: int,
+        n_layers: int,
+        n_outputs: int,
+        n_hidden_neurons_multiplier: int = 4,
+        n_w_bits: int = 3,
+        n_a_bits: int = 3,
+        n_accum_bits: int = MAX_BITWIDTH_BACKWARD_COMPATIBLE,
+        n_prune_neurons_percentage: float = 0.0,
+        activation_function: Type = nn.ReLU,
+        quant_narrow: bool = False,
+        quant_signed: bool = True,
+    ):
         """Sparse Quantized Neural Network constructor.
 
         Args:
-            input_dim: Number of dimensions of the input data
-            n_layers: Number of linear layers for this network
-            n_outputs: Number of output classes or regression targets
-            n_w_bits: Number of weight bits
-            n_a_bits: Number of activation and input bits
-            n_accum_bits: Maximal allowed bit-width of intermediate accumulators
-            n_hidden_neurons_multiplier: The number of neurons on the hidden will be the number
-                of dimensions of the input multiplied by `n_hidden_neurons_multiplier`. Note that
-                pruning is used to adjust the accumulator size to attempt to
-                keep the maximum accumulator bit-width to
-                `n_accum_bits`, meaning that not all hidden layer neurons will be active.
-                The default value for `n_hidden_neurons_multiplier` is chosen for small dimensions
-                of the input. Reducing this value decreases the FHE inference time considerably
-                but also decreases the robustness and accuracy of model training.
-            n_prune_neurons_percentage: How many neurons to prune on the hidden layers. This
-                should be used mostly through the dedicated `.prune()` mechanism. This can
-                be used in when setting `n_hidden_neurons_multiplier` high (3-4), once good accuracy
-                is obtained, to speed up the model in FHE.
-            activation_function: a torch class that is used to construct activation functions in
-                the network (eg torch.ReLU, torch.SELU, torch.Sigmoid, etc)
-            quant_narrow : whether this network should use narrow range quantized integer values
-            quant_signed : whether to use signed quantized integer values
+            input_dim (int): Number of dimensions of the input data.
+            n_layers (int): Number of linear layers for this network.
+            n_outputs (int): Number of output classes or regression targets.
+            n_w_bits (int): Number of weight bits.
+            n_a_bits (int): Number of activation and input bits.
+            n_accum_bits (int): Maximal allowed bit-width of intermediate accumulators.
+            n_hidden_neurons_multiplier (int): The number of neurons on the hidden will be the
+                number of dimensions of the input multiplied by `n_hidden_neurons_multiplier`. Note
+                that pruning is used to adjust the accumulator size to attempt to keep the maximum
+                accumulator bit-width to `n_accum_bits`, meaning that not all hidden layer neurons
+                will be active. The default value for `n_hidden_neurons_multiplier` is chosen for
+                small dimensions of the input. Reducing this value decreases the FHE inference time
+                considerably but also decreases the robustness and accuracy of model training.
+            n_prune_neurons_percentage (float): The percentage of neurons to prune in the hidden
+                layers. This can be used when setting `n_hidden_neurons_multiplier` with a high
+                number (3-4), once good accuracy is obtained, in order to speed up the model in FHE.
+            activation_function (Type): The activation function to use in the network
+                (e.g., torch.ReLU, torch.SELU, torch.Sigmoid, ...).
+            quant_narrow (bool): Whether this network should quantize the values using narrow range
+                (e.g a 2-bits signed quantization uses [-1, 0, 1] instead of [-2, -1, 0, 1]).
+            quant_signed (bool): Whether this network should quantize the values using signed
+                integers.
 
         Raises:
-            ValueError: if the parameters have invalid values or the computed accumulator bit-width
-                        is zero
+            ValueError: If the parameters have invalid values or the computed accumulator bit-width
+                is zero.
         """
 
         super().__init__()
 
         self.features = nn.Sequential()
         in_features = input_dim
 
@@ -124,30 +127,30 @@
         self.n_prune_neurons_percentage = n_prune_neurons_percentage
 
         assert_true(
             self.n_prune_neurons_percentage >= 0 and self.n_prune_neurons_percentage < 1.0,
             "Pruning percentage must be expressed as a fraction between 0 and 1. A value of "
             " zero (0) means pruning is disabled",
         )
-        self.pruned_layers = set()
+        self.pruned_layers: Set[nn.Module] = set()
 
         self.enable_pruning()
 
     def max_active_neurons(self) -> int:
         """Compute the maximum number of active (non-zero weight) neurons.
 
         The computation is done using the quantization parameters passed to the constructor.
         Warning: With the current quantization algorithm (asymmetric) the value returned by this
         function is not guaranteed to ensure FHE compatibility. For some weight distributions,
         weights that are 0 (which are pruned weights) will not be quantized to 0.
         Therefore the total number of active quantized neurons will not be equal to
         max_active_neurons.
 
         Returns:
-            n (int): maximum number of active neurons
+            int: The maximum number of active neurons.
         """
 
         return int(
             numpy.floor(
                 (2**self.n_accum_bits - 1) / (2**self.n_w_bits - 1) / (2**self.n_a_bits - 1)
             )
         )
@@ -222,15 +225,15 @@
             "Not all layers in the network were examined as candidates for pruning",
         )
 
     def enable_pruning(self) -> None:
         """Enable pruning in the network. Pruning must be made permanent to recover pruned weights.
 
         Raises:
-            ValueError: if the quantization parameters are invalid
+            ValueError: If the quantization parameters are invalid.
         """
         max_neuron_connections = self.max_active_neurons()
 
         if max_neuron_connections == 0:
             raise ValueError(
                 "The maximum accumulator bit-width is too low "
                 "for the quantization parameters requested. No neurons would be created in the "
```

## concrete/ml/sklearn/rf.py

```diff
@@ -1,25 +1,22 @@
 """Implement RandomForest models."""
 from typing import Any, Dict
 
 import numpy
-from sklearn.ensemble import RandomForestClassifier as SklearnRandomForestClassifier
-from sklearn.ensemble import RandomForestRegressor as SklearnRandomForestRegressor
+import sklearn.ensemble
 
-from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
-from ..quantization.quantizers import UniformQuantizer
 from ..sklearn.tree_to_numpy import tree_to_numpy
 from .base import BaseTreeClassifierMixin, BaseTreeEstimatorMixin, BaseTreeRegressorMixin
 
 
 # pylint: disable=too-many-instance-attributes
 class RandomForestClassifier(BaseTreeClassifierMixin):
     """Implements the RandomForest classifier."""
 
-    sklearn_model_class = SklearnRandomForestClassifier
+    sklearn_model_class = sklearn.ensemble.RandomForestClassifier
     framework = "sklearn"
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         n_bits: int = 6,
@@ -73,30 +70,30 @@
         # RandomForestClassifier models directly computes probabilities and therefore don't require
         # to apply a sigmoid or softmax in post-processing
         return BaseTreeEstimatorMixin.post_processing(self, y_preds)
 
     def dump_dict(self) -> Dict[str, Any]:
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
-        metadata["sklearn_model_class"] = self.sklearn_model_class
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["onnx_model_"] = self.onnx_model_
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["onnx_model_"] = self.onnx_model_
         metadata["framework"] = self.framework
+        metadata["post_processing_params"] = self.post_processing_params
 
         # Classifier
-        metadata["classes_"] = self.target_classes_
+        metadata["target_classes_"] = self.target_classes_
         metadata["n_classes_"] = self.n_classes_
 
+        # Scikit-Learn
         metadata["n_estimators"] = self.n_estimators
         metadata["bootstrap"] = self.bootstrap
         metadata["oob_score"] = self.oob_score
         metadata["n_jobs"] = self.n_jobs
         metadata["random_state"] = self.random_state
         metadata["verbose"] = self.verbose
         metadata["warm_start"] = self.warm_start
@@ -112,47 +109,36 @@
         metadata["min_impurity_decrease"] = self.min_impurity_decrease
         metadata["ccp_alpha"] = self.ccp_alpha
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
+        # Instantiate the model
         obj = RandomForestClassifier(n_bits=metadata["n_bits"])
 
-        # Tree
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
-
+        # Concrete-ML
+        obj.sklearn_model = metadata["sklearn_model"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
         obj.framework = metadata["framework"]
-
         obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
             obj.sklearn_model,
             numpy.zeros((len(obj.input_quantizers),))[None, ...],
             framework=obj.framework,
             output_n_bits=obj.n_bits,
         )
-
         obj.post_processing_params = metadata["post_processing_params"]
-        obj._is_fitted = metadata["_is_fitted"]
-        obj._is_compiled = metadata["_is_compiled"]
 
         # Classifier
-        obj.target_classes_ = numpy.array(metadata["classes_"])
+        obj.target_classes_ = metadata["target_classes_"]
         obj.n_classes_ = metadata["n_classes_"]
 
+        # Scikit-Learn
         obj.n_estimators = metadata["n_estimators"]
         obj.bootstrap = metadata["bootstrap"]
         obj.oob_score = metadata["oob_score"]
         obj.n_jobs = metadata["n_jobs"]
         obj.random_state = metadata["random_state"]
         obj.verbose = metadata["verbose"]
         obj.warm_start = metadata["warm_start"]
@@ -171,15 +157,15 @@
         return obj
 
 
 # pylint: disable=too-many-instance-attributes
 class RandomForestRegressor(BaseTreeRegressorMixin):
     """Implements the RandomForest regressor."""
 
-    sklearn_model_class = SklearnRandomForestRegressor
+    sklearn_model_class = sklearn.ensemble.RandomForestRegressor
     framework = "sklearn"
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         n_bits: int = 6,
@@ -225,26 +211,26 @@
         self.max_leaf_nodes = max_leaf_nodes
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
 
     def dump_dict(self) -> Dict[str, Any]:
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
-        metadata["sklearn_model_class"] = self.sklearn_model_class
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["onnx_model_"] = self.onnx_model_
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["onnx_model_"] = self.onnx_model_
         metadata["framework"] = self.framework
+        metadata["post_processing_params"] = self.post_processing_params
 
+        # Scikit-Learn
         metadata["n_estimators"] = self.n_estimators
         metadata["bootstrap"] = self.bootstrap
         metadata["oob_score"] = self.oob_score
         metadata["n_jobs"] = self.n_jobs
         metadata["random_state"] = self.random_state
         metadata["verbose"] = self.verbose
         metadata["warm_start"] = self.warm_start
@@ -259,43 +245,33 @@
         metadata["min_impurity_decrease"] = self.min_impurity_decrease
         metadata["ccp_alpha"] = self.ccp_alpha
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = RandomForestRegressor(n_bits=metadata["n_bits"])
 
-        # Tree
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
+        # Instantiate the model
+        obj = RandomForestRegressor(n_bits=metadata["n_bits"])
 
+        # Concrete-ML
+        obj.sklearn_model = metadata["sklearn_model"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
         obj.framework = metadata["framework"]
-
         obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
             obj.sklearn_model,
             numpy.zeros((len(obj.input_quantizers),))[None, ...],
             framework=obj.framework,
             output_n_bits=obj.n_bits,
         )
-
         obj.post_processing_params = metadata["post_processing_params"]
-        obj._is_fitted = metadata["_is_fitted"]
-        obj._is_compiled = metadata["_is_compiled"]
 
+        # Scikit-Learn
         obj.n_estimators = metadata["n_estimators"]
         obj.bootstrap = metadata["bootstrap"]
         obj.oob_score = metadata["oob_score"]
         obj.n_jobs = metadata["n_jobs"]
         obj.random_state = metadata["random_state"]
         obj.verbose = metadata["verbose"]
         obj.warm_start = metadata["warm_start"]
```

## concrete/ml/sklearn/svm.py

```diff
@@ -1,15 +1,12 @@
 """Implement Support Vector Machine."""
 from typing import Any, Dict
 
-import numpy
-import sklearn.linear_model
+import sklearn.svm
 
-from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
-from ..quantization.quantizers import UniformQuantizer
 from .base import SklearnLinearClassifierMixin, SklearnLinearRegressorMixin
 
 
 # pylint: disable=invalid-name,too-many-instance-attributes
 class LinearSVR(SklearnLinearRegressorMixin):
     """A Regression Support Vector Machine (SVM).
 
@@ -59,31 +56,28 @@
         self.max_iter = max_iter
 
     def dump_dict(self) -> Dict[str, Any]:
         assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = type(self).__name__
-
-        # Linear
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["sklearn_model_class"] = self.sklearn_model_class
-        metadata["fhe_circuit"] = self.fhe_circuit
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
-        metadata["onnx_model_"] = self.onnx_model_
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["_weight_quantizer"] = self._weight_quantizer
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["onnx_model_"] = self.onnx_model_
         metadata["_q_weights"] = self._q_weights
         metadata["_q_bias"] = self._q_bias
+        metadata["post_processing_params"] = self.post_processing_params
 
+        # Scikit-Learn
         metadata["epsilon"] = self.epsilon
         metadata["tol"] = self.tol
         metadata["C"] = self.C
         metadata["loss"] = self.loss
         metadata["fit_intercept"] = self.fit_intercept
         metadata["intercept_scaling"] = self.intercept_scaling
         metadata["dual"] = self.dual
@@ -91,40 +85,32 @@
         metadata["random_state"] = self.random_state
         metadata["max_iter"] = self.max_iter
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = LinearSVR()
-        obj.post_processing_params = metadata["post_processing_params"]
 
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
+        # Instantiate the model
+        obj = LinearSVR()
 
-        # Linear
+        # Concrete-ML
         obj.n_bits = metadata["n_bits"]
-        obj.sklearn_model_class = metadata["sklearn_model_class"]
-        obj.fhe_circuit = metadata["fhe_circuit"]
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
-        obj.onnx_model_ = metadata["onnx_model_"]
+        obj.sklearn_model = metadata["sklearn_model"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.output_quantizers = metadata["output_quantizers"]
+        obj._weight_quantizer = metadata["_weight_quantizer"]
+        obj.onnx_model_ = metadata["onnx_model_"]
         obj._q_weights = metadata["_q_weights"]
         obj._q_bias = metadata["_q_bias"]
+        obj.post_processing_params = metadata["post_processing_params"]
 
+        # Scikit-Learn
         obj.epsilon = metadata["epsilon"]
         obj.tol = metadata["tol"]
         obj.C = metadata["C"]
         obj.loss = metadata["loss"]
         obj.fit_intercept = metadata["fit_intercept"]
         obj.intercept_scaling = metadata["intercept_scaling"]
         obj.dual = metadata["dual"]
@@ -189,36 +175,32 @@
         self.max_iter = max_iter
 
     def dump_dict(self) -> Dict[str, Any]:
         assert self._weight_quantizer is not None, self._is_not_fitted_error_message()
 
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = type(self).__name__
-
-        # Classifier
-        metadata["classes_"] = self.target_classes_
-        metadata["n_classes_"] = self.n_classes_
-        metadata["cml_dumped_class_name"] = type(self).__name__
-
-        # Linear
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["sklearn_model_class"] = self.sklearn_model_class
-        metadata["fhe_circuit"] = self.fhe_circuit
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["_weight_quantizer"] = self._weight_quantizer.dumps()
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
-        metadata["onnx_model_"] = self.onnx_model_
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["_weight_quantizer"] = self._weight_quantizer
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["onnx_model_"] = self.onnx_model_
         metadata["_q_weights"] = self._q_weights
         metadata["_q_bias"] = self._q_bias
+        metadata["post_processing_params"] = self.post_processing_params
+
+        # Classifier
+        metadata["target_classes_"] = self.target_classes_
+        metadata["n_classes_"] = self.n_classes_
 
+        # Scikit-Learn
         metadata["penalty"] = self.penalty
         metadata["loss"] = self.loss
         metadata["dual"] = self.dual
         metadata["tol"] = self.tol
         metadata["C"] = self.C
         metadata["multi_class"] = self.multi_class
         metadata["fit_intercept"] = self.fit_intercept
@@ -228,44 +210,36 @@
         metadata["random_state"] = self.random_state
         metadata["max_iter"] = self.max_iter
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = LinearSVC()
-        obj.post_processing_params = metadata["post_processing_params"]
 
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
-
-        # Classifier
-        obj.target_classes_ = numpy.array(metadata["classes_"])
-        obj.n_classes_ = metadata["n_classes_"]
+        # Instantiate the model
+        obj = LinearSVC()
 
-        # Linear
+        # Concrete-ML
         obj.n_bits = metadata["n_bits"]
-        obj.sklearn_model_class = metadata["sklearn_model_class"]
-        obj.fhe_circuit = metadata["fhe_circuit"]
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-        obj._weight_quantizer = UniformQuantizer.loads(metadata["_weight_quantizer"])
-        obj.onnx_model_ = metadata["onnx_model_"]
+        obj.sklearn_model = metadata["sklearn_model"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.output_quantizers = metadata["output_quantizers"]
+        obj._weight_quantizer = metadata["_weight_quantizer"]
+        obj.onnx_model_ = metadata["onnx_model_"]
         obj._q_weights = metadata["_q_weights"]
         obj._q_bias = metadata["_q_bias"]
+        obj.post_processing_params = metadata["post_processing_params"]
+
+        # Classifier
+        obj.target_classes_ = metadata["target_classes_"]
+        obj.n_classes_ = metadata["n_classes_"]
 
+        # Scikit-Learn
         obj.penalty = metadata["penalty"]
         obj.loss = metadata["loss"]
         obj.dual = metadata["dual"]
         obj.tol = metadata["tol"]
         obj.C = metadata["C"]
         obj.multi_class = metadata["multi_class"]
         obj.fit_intercept = metadata["fit_intercept"]
```

## concrete/ml/sklearn/tree.py

```diff
@@ -1,25 +1,22 @@
 """Implement DecisionTree models."""
 from typing import Any, Dict
 
 import numpy
-from sklearn.tree import DecisionTreeClassifier as SklearnDecisionTreeClassifier
-from sklearn.tree import DecisionTreeRegressor as SklearnDecisionTreeRegressor
+import sklearn.tree
 
-from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
-from ..quantization.quantizers import UniformQuantizer
 from ..sklearn.tree_to_numpy import tree_to_numpy
 from .base import BaseTreeClassifierMixin, BaseTreeEstimatorMixin, BaseTreeRegressorMixin
 
 
 # pylint: disable-next=too-many-instance-attributes
 class DecisionTreeClassifier(BaseTreeClassifierMixin):
     """Implements the sklearn DecisionTreeClassifier."""
 
-    sklearn_model_class = SklearnDecisionTreeClassifier
+    sklearn_model_class = sklearn.tree.DecisionTreeClassifier
     framework = "sklearn"
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         criterion="gini",
@@ -62,30 +59,30 @@
         # DecisionTreeClassifier models directly computes probabilities and therefore don't require
         # to apply a sigmoid or softmax in post-processing
         return BaseTreeEstimatorMixin.post_processing(self, y_preds)
 
     def dump_dict(self) -> Dict[str, Any]:
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
-        metadata["sklearn_model_class"] = self.sklearn_model_class
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["onnx_model_"] = self.onnx_model_
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["onnx_model_"] = self.onnx_model_
         metadata["framework"] = self.framework
+        metadata["post_processing_params"] = self.post_processing_params
 
         # Classifier
-        metadata["classes_"] = self.target_classes_
+        metadata["target_classes_"] = self.target_classes_
         metadata["n_classes_"] = self.n_classes_
 
+        # Scikit-Learn
         metadata["criterion"] = self.criterion
         metadata["splitter"] = self.splitter
         metadata["max_depth"] = self.max_depth
         metadata["min_samples_split"] = self.min_samples_split
         metadata["min_samples_leaf"] = self.min_samples_leaf
         metadata["min_weight_fraction_leaf"] = self.min_weight_fraction_leaf
         metadata["max_features"] = self.max_features
@@ -95,47 +92,37 @@
         metadata["min_impurity_decrease"] = self.min_impurity_decrease
         metadata["ccp_alpha"] = self.ccp_alpha
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = cls(n_bits=metadata["n_bits"])
 
-        # Tree
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
+        # Instantiate the model
+        obj = cls(n_bits=metadata["n_bits"])
 
+        # Concrete-ML
+        obj.sklearn_model = metadata["sklearn_model"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
         obj.framework = metadata["framework"]
-
         obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
             obj.sklearn_model,
             numpy.zeros((len(obj.input_quantizers),))[None, ...],
             framework=obj.framework,
             output_n_bits=obj.n_bits,
         )
-
         obj.post_processing_params = metadata["post_processing_params"]
-        obj._is_fitted = metadata["_is_fitted"]
-        obj._is_compiled = metadata["_is_compiled"]
 
         # Classifier
-        obj.target_classes_ = numpy.array(metadata["classes_"])
+        obj.target_classes_ = metadata["target_classes_"]
         obj.n_classes_ = metadata["n_classes_"]
 
+        # Scikit-Learn
         obj.criterion = metadata["criterion"]
         obj.splitter = metadata["splitter"]
         obj.max_depth = metadata["max_depth"]
         obj.min_samples_split = metadata["min_samples_split"]
         obj.min_samples_leaf = metadata["min_samples_leaf"]
         obj.min_weight_fraction_leaf = metadata["min_weight_fraction_leaf"]
         obj.max_features = metadata["max_features"]
@@ -148,15 +135,15 @@
         return obj
 
 
 # pylint: disable-next=too-many-instance-attributes
 class DecisionTreeRegressor(BaseTreeRegressorMixin):
     """Implements the sklearn DecisionTreeClassifier."""
 
-    sklearn_model_class = SklearnDecisionTreeRegressor
+    sklearn_model_class = sklearn.tree.DecisionTreeRegressor
     framework = "sklearn"
     _is_a_public_cml_model = True
 
     # pylint: disable-next=too-many-arguments
     def __init__(
         self,
         criterion="squared_error",
@@ -191,26 +178,26 @@
         self.random_state = random_state
         self.min_impurity_decrease = min_impurity_decrease
         self.ccp_alpha = ccp_alpha
 
     def dump_dict(self) -> Dict[str, Any]:
         metadata: Dict[str, Any] = {}
 
-        metadata["post_processing_params"] = self.post_processing_params
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
-        metadata["sklearn_model_class"] = self.sklearn_model_class
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["onnx_model_"] = self.onnx_model_
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["onnx_model_"] = self.onnx_model_
         metadata["framework"] = self.framework
+        metadata["post_processing_params"] = self.post_processing_params
 
+        # Scikit-Learn
         metadata["criterion"] = self.criterion
         metadata["splitter"] = self.splitter
         metadata["max_depth"] = self.max_depth
         metadata["min_samples_split"] = self.min_samples_split
         metadata["min_samples_leaf"] = self.min_samples_leaf
         metadata["min_weight_fraction_leaf"] = self.min_weight_fraction_leaf
         metadata["max_features"] = self.max_features
@@ -219,43 +206,33 @@
         metadata["min_impurity_decrease"] = self.min_impurity_decrease
         metadata["ccp_alpha"] = self.ccp_alpha
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = cls(n_bits=metadata["n_bits"])
 
-        # Tree
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
+        # Instantiate the model
+        obj = cls(n_bits=metadata["n_bits"])
 
+        # Concrete-ML
+        obj.sklearn_model = metadata["sklearn_model"]
+        obj._is_fitted = metadata["_is_fitted"]
+        obj._is_compiled = metadata["_is_compiled"]
+        obj.input_quantizers = metadata["input_quantizers"]
         obj.framework = metadata["framework"]
-
         obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
             obj.sklearn_model,
             numpy.zeros((len(obj.input_quantizers),))[None, ...],
             framework=obj.framework,
             output_n_bits=obj.n_bits,
         )
-
         obj.post_processing_params = metadata["post_processing_params"]
-        obj._is_fitted = metadata["_is_fitted"]
-        obj._is_compiled = metadata["_is_compiled"]
 
+        # Scikit-Learn
         obj.criterion = metadata["criterion"]
         obj.splitter = metadata["splitter"]
         obj.max_depth = metadata["max_depth"]
         obj.min_samples_split = metadata["min_samples_split"]
         obj.min_samples_leaf = metadata["min_samples_leaf"]
         obj.min_weight_fraction_leaf = metadata["min_weight_fraction_leaf"]
         obj.max_features = metadata["max_features"]
```

## concrete/ml/sklearn/xgb.py

```diff
@@ -2,17 +2,15 @@
 import platform
 import warnings
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import numpy
 import xgboost.sklearn
 
-from .. import TRUSTED_SKOPS, USE_SKOPS, loads_sklearn
 from ..common.debugging.custom_assert import assert_true
-from ..quantization.quantizers import UniformQuantizer
 from ..sklearn.tree_to_numpy import tree_to_numpy
 from .base import BaseTreeClassifierMixin, BaseTreeRegressorMixin
 
 
 # Disabling invalid-name to use uppercase X
 # pylint: disable=invalid-name,too-many-instance-attributes
 class XGBClassifier(BaseTreeClassifierMixin):
@@ -113,29 +111,30 @@
         self.use_label_encoder = use_label_encoder
         self.random_state = random_state
         self.verbosity = verbosity
 
     def dump_dict(self) -> Dict[str, Any]:
         metadata: Dict[str, Any] = {}
 
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
-        metadata["sklearn_model_class"] = self.sklearn_model_class
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["onnx_model_"] = self.onnx_model_
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["onnx_model_"] = self.onnx_model_
         metadata["framework"] = self.framework
+        metadata["post_processing_params"] = self.post_processing_params
 
         # Classifier
-        metadata["classes_"] = self.target_classes_
+        metadata["target_classes_"] = self.target_classes_
         metadata["n_classes_"] = self.n_classes_
 
+        # XGBoost
         metadata["max_depth"] = self.max_depth
         metadata["learning_rate"] = self.learning_rate
         metadata["n_estimators"] = self.n_estimators
         metadata["objective"] = self.objective
         metadata["booster"] = self.booster
         metadata["tree_method"] = self.tree_method
         metadata["n_jobs"] = self.n_jobs
@@ -158,51 +157,42 @@
         metadata["gpu_id"] = self.gpu_id
         metadata["validate_parameters"] = self.validate_parameters
         metadata["predictor"] = self.predictor
         metadata["enable_categorical"] = self.enable_categorical
         metadata["use_label_encoder"] = self.use_label_encoder
         metadata["random_state"] = self.random_state
         metadata["verbosity"] = self.verbosity
-        metadata["post_processing_params"] = self.post_processing_params
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = XGBClassifier(n_bits=metadata["n_bits"])
 
-        # Tree
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
+        # Instantiate the model
+        obj = XGBClassifier(n_bits=metadata["n_bits"])
 
-        obj.framework = metadata["framework"]
+        # Concrete-ML
+        obj.sklearn_model = metadata["sklearn_model"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
-
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.framework = metadata["framework"]
         obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
             obj.sklearn_model,
             numpy.zeros((len(obj.input_quantizers),))[None, ...],
             framework=obj.framework,
             output_n_bits=obj.n_bits,
         )
+        obj.post_processing_params = metadata["post_processing_params"]
 
         # Classifier
-        obj.target_classes_ = numpy.array(metadata["classes_"])
+        obj.target_classes_ = metadata["target_classes_"]
         obj.n_classes_ = metadata["n_classes_"]
 
+        # XGBoost
         obj.max_depth = metadata["max_depth"]
         obj.learning_rate = metadata["learning_rate"]
         obj.n_estimators = metadata["n_estimators"]
         obj.objective = metadata["objective"]
         obj.booster = metadata["booster"]
         obj.tree_method = metadata["tree_method"]
         obj.n_jobs = metadata["n_jobs"]
@@ -225,15 +215,14 @@
         obj.gpu_id = metadata["gpu_id"]
         obj.validate_parameters = metadata["validate_parameters"]
         obj.predictor = metadata["predictor"]
         obj.enable_categorical = metadata["enable_categorical"]
         obj.use_label_encoder = metadata["use_label_encoder"]
         obj.random_state = metadata["random_state"]
         obj.verbosity = metadata["verbosity"]
-        obj.post_processing_params = metadata["post_processing_params"]
 
         return obj
 
 
 # Disabling invalid-name to use uppercase X
 # pylint: disable=invalid-name,too-many-instance-attributes
 class XGBRegressor(BaseTreeRegressorMixin):
@@ -349,26 +338,26 @@
         # Call BaseTreeEstimatorMixin's fit method
         super().fit(X, y, *args, **kwargs)
         return self
 
     def dump_dict(self) -> Dict[str, Any]:
         metadata: Dict[str, Any] = {}
 
-        metadata["cml_dumped_class_name"] = str(type(self).__name__)
+        # Concrete-ML
         metadata["n_bits"] = self.n_bits
-        metadata["input_quantizers"] = [elt.dumps() for elt in self.input_quantizers]
-        metadata["output_quantizers"] = [elt.dumps() for elt in self.output_quantizers]
-        metadata["sklearn_model_class"] = self.sklearn_model_class
         metadata["sklearn_model"] = self.sklearn_model
-        metadata["onnx_model_"] = self.onnx_model_
         metadata["_is_fitted"] = self._is_fitted
         metadata["_is_compiled"] = self._is_compiled
+        metadata["input_quantizers"] = self.input_quantizers
+        metadata["output_quantizers"] = self.output_quantizers
+        metadata["onnx_model_"] = self.onnx_model_
         metadata["framework"] = self.framework
+        metadata["post_processing_params"] = self.post_processing_params
 
-        # Specific
+        # XGBoost
         metadata["max_depth"] = self.max_depth
         metadata["learning_rate"] = self.learning_rate
         metadata["n_estimators"] = self.n_estimators
         metadata["objective"] = self.objective
         metadata["booster"] = self.booster
         metadata["tree_method"] = self.tree_method
         metadata["n_jobs"] = self.n_jobs
@@ -391,47 +380,38 @@
         metadata["gpu_id"] = self.gpu_id
         metadata["validate_parameters"] = self.validate_parameters
         metadata["predictor"] = self.predictor
         metadata["enable_categorical"] = self.enable_categorical
         metadata["use_label_encoder"] = self.use_label_encoder
         metadata["random_state"] = self.random_state
         metadata["verbosity"] = self.verbosity
-        metadata["post_processing_params"] = self.post_processing_params
 
         return metadata
 
     @classmethod
     def load_dict(cls, metadata: Dict):
-        obj = XGBRegressor(n_bits=metadata["n_bits"])
 
-        # Tree
-        obj.input_quantizers = [UniformQuantizer.loads(elt) for elt in metadata["input_quantizers"]]
-        obj.output_quantizers = [
-            UniformQuantizer.loads(elt) for elt in metadata["output_quantizers"]
-        ]
-
-        # Load the underlying fitted model
-        loads_sklearn_kwargs = {}
-        if USE_SKOPS:
-            loads_sklearn_kwargs["trusted"] = TRUSTED_SKOPS
-        obj.sklearn_model = loads_sklearn(
-            bytes.fromhex(metadata["sklearn_model"]), **loads_sklearn_kwargs
-        )
+        # Instantiate the model
+        obj = XGBRegressor(n_bits=metadata["n_bits"])
 
-        obj.framework = metadata["framework"]
+        # Concrete-ML
+        obj.sklearn_model = metadata["sklearn_model"]
         obj._is_fitted = metadata["_is_fitted"]
         obj._is_compiled = metadata["_is_compiled"]
-
+        obj.input_quantizers = metadata["input_quantizers"]
+        obj.framework = metadata["framework"]
         obj._tree_inference, obj.output_quantizers, obj.onnx_model_ = tree_to_numpy(
             obj.sklearn_model,
             numpy.zeros((len(obj.input_quantizers),))[None, ...],
             framework=obj.framework,
             output_n_bits=obj.n_bits,
         )
+        obj.post_processing_params = metadata["post_processing_params"]
 
+        # XGBoost
         obj.max_depth = metadata["max_depth"]
         obj.learning_rate = metadata["learning_rate"]
         obj.n_estimators = metadata["n_estimators"]
         obj.objective = metadata["objective"]
         obj.booster = metadata["booster"]
         obj.tree_method = metadata["tree_method"]
         obj.n_jobs = metadata["n_jobs"]
@@ -454,10 +434,9 @@
         obj.gpu_id = metadata["gpu_id"]
         obj.validate_parameters = metadata["validate_parameters"]
         obj.predictor = metadata["predictor"]
         obj.enable_categorical = metadata["enable_categorical"]
         obj.use_label_encoder = metadata["use_label_encoder"]
         obj.random_state = metadata["random_state"]
         obj.verbosity = metadata["verbosity"]
-        obj.post_processing_params = metadata["post_processing_params"]
 
         return obj
```

## concrete/ml/torch/compile.py

```diff
@@ -45,14 +45,65 @@
     return (
         torch_tensor_or_numpy_array
         if isinstance(torch_tensor_or_numpy_array, numpy.ndarray)
         else torch_tensor_or_numpy_array.cpu().numpy()
     )
 
 
+def build_quantized_module(
+    model: Union[torch.nn.Module, onnx.ModelProto],
+    torch_inputset: Dataset,
+    import_qat: bool = False,
+    n_bits=MAX_BITWIDTH_BACKWARD_COMPATIBLE,
+    rounding_threshold_bits: Optional[int] = None,
+) -> QuantizedModule:
+    """Build a quantized module from a Torch or ONNX model.
+
+    Take a model in torch or ONNX, turn it to numpy, quantize its inputs / weights / outputs and
+    retrieve the associated quantized module.
+
+    Args:
+        model (Union[torch.nn.Module, onnx.ModelProto]): The model to quantize, either in torch or
+            in ONNX.
+        torch_inputset (Dataset): the calibration input-set, can contain either torch
+            tensors or numpy.ndarray
+        import_qat (bool): Flag to signal that the network being imported contains quantizers in
+            in its computation graph and that Concrete ML should not re-quantize it
+        n_bits: the number of bits for the quantization
+        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
+            to the given bits of precision
+
+    Returns:
+        QuantizedModule: The resulting QuantizedModule.
+    """
+    inputset_as_numpy_tuple = tuple(
+        convert_torch_tensor_or_numpy_array_to_numpy_array(val) for val in to_tuple(torch_inputset)
+    )
+
+    # Tracing needs to be done with the batch size of 1 since we compile our models to FHE with
+    # this batch size. The input set contains many examples, to determine a representative
+    # bit-width, but for tracing we only take a single one. We need the ONNX tracing batch size to
+    # match the batch size during FHE inference which can only be 1 for the moment.
+    dummy_input_for_tracing = tuple(
+        torch.from_numpy(val[[0], ::]).float() for val in inputset_as_numpy_tuple
+    )
+
+    # Create corresponding numpy model
+    numpy_model = NumpyModule(model, dummy_input_for_tracing)
+
+    # Quantize with post-training static method, to have a model with integer weights
+    post_training = PostTrainingQATImporter if import_qat else PostTrainingAffineQuantization
+    post_training_quant = post_training(n_bits, numpy_model, rounding_threshold_bits)
+
+    # Build the quantized module
+    quantized_module = post_training_quant.quantize_module(*inputset_as_numpy_tuple)
+
+    return quantized_module
+
+
 # pylint: disable-next=too-many-arguments
 def _compile_torch_or_onnx_model(
     model: Union[torch.nn.Module, onnx.ModelProto],
     torch_inputset: Dataset,
     import_qat: bool = False,
     configuration: Optional[Configuration] = None,
     artifacts: Optional[DebugArtifacts] = None,
@@ -91,36 +142,25 @@
         QuantizedModule: The resulting compiled QuantizedModule.
     """
 
     inputset_as_numpy_tuple = tuple(
         convert_torch_tensor_or_numpy_array_to_numpy_array(val) for val in to_tuple(torch_inputset)
     )
 
-    # Tracing needs to be done with the batch size of 1 since we compile our models to FHE with
-    # this batch size. The input set contains many examples, to determine a representative
-    # bit-width, but for tracing we only take a single one. We need the ONNX tracing batch size to
-    # match the batch size during FHE inference which can only be 1 for the moment.
-    # Use batch size > 1 in FHE once it is available
-    # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/758
-    dummy_input_for_tracing = tuple(
-        torch.from_numpy(val[[0], ::]).float() for val in inputset_as_numpy_tuple
+    # Build the quantized module
+    quantized_module = build_quantized_module(
+        model=model,
+        torch_inputset=inputset_as_numpy_tuple,
+        import_qat=import_qat,
+        n_bits=n_bits,
+        rounding_threshold_bits=rounding_threshold_bits,
     )
 
-    # Create corresponding numpy model
-    numpy_model = NumpyModule(model, dummy_input_for_tracing)
-    onnx_model = numpy_model.onnx_model
-
-    # Quantize with post-training static method, to have a model with integer weights
-    post_training = PostTrainingQATImporter if import_qat else PostTrainingAffineQuantization
-    post_training_quant = post_training(n_bits, numpy_model, rounding_threshold_bits)
-
-    quantized_module = post_training_quant.quantize_module(*inputset_as_numpy_tuple)
-
-    # Don't let the user shoot in her foot, by having p_error or global_p_error set in both
-    # configuration and in direct arguments
+    # Check that p_error or global_p_error is not set in both the configuration and in the direct
+    # parameters
     check_there_is_no_p_error_options_in_configuration(configuration)
 
     # Find the right way to set parameters for compiler, depending on the way we want to default
     p_error, global_p_error = manage_parameters_for_pbs_errors(p_error, global_p_error)
 
     quantized_module.compile(
         inputset_as_numpy_tuple,
@@ -128,16 +168,14 @@
         artifacts,
         show_mlir=show_mlir,
         p_error=p_error,
         global_p_error=global_p_error,
         verbose=verbose,
     )
 
-    quantized_module.onnx_model = onnx_model
-
     return quantized_module
 
 
 # pylint: disable-next=too-many-arguments
 def compile_torch_model(
     torch_model: torch.nn.Module,
     torch_inputset: Dataset,
@@ -358,20 +396,21 @@
     exporter = BrevitasONNXManager()
     # Here we add a "eliminate_nop_pad" optimization step for onnxoptimizer
     # https://github.com/onnx/optimizer/blob/master/onnxoptimizer/passes/eliminate_nop_pad.h#L5
     # It deletes 0-values padding.
     # This is needed because AvgPool2d adds a 0-Pad operation that then breaks the compilation
     # A list of steps that can be added can be found in the following link
     # https://github.com/onnx/optimizer/blob/master/onnxoptimizer/pass_registry.h
+    # In the export function, the `args` parameter is used instead of the `input_shape` one in
+    # order to be able to handle multi-inputs models
     exporter.onnx_passes.append("eliminate_nop_pad")
     exporter.onnx_passes.append("fuse_pad_into_conv")
-
     onnx_model = exporter.export(
         torch_model,
-        input_shape=dummy_input_for_tracing[0].shape,
+        args=dummy_input_for_tracing,
         export_path=str(output_onnx_file_path),
         keep_initializers_as_inputs=False,
         opset_version=OPSET_VERSION_FOR_ONNX_EXPORT,
     )
     onnx_model = remove_initializer_from_input(onnx_model)
 
     if n_bits is None:
@@ -386,17 +425,17 @@
             "model_inputs": n_bits,
             "op_weights": n_bits,
             "op_inputs": n_bits,
             "model_outputs": n_bits,
         }
     elif isinstance(n_bits, dict):
         assert_true(
-            isinstance(n_bits, dict) and set(n_bits.keys()) == {"model_inputs", "model_outputs"},
-            "When importing a Brevitas QAT network, n_bits can only contain the following keys: "
-            '"model_inputs", "model_outputs"',
+            set(n_bits.keys()) == {"model_inputs", "model_outputs"},
+            "When importing a Brevitas QAT network, n_bits should only contain the following keys: "
+            f'"model_inputs", "model_outputs". Instead, got {n_bits.keys()}',
         )
 
         n_bits = {
             "model_inputs": n_bits["model_inputs"],
             "op_weights": n_bits["model_inputs"],
             "op_inputs": n_bits["model_inputs"],
             "model_outputs": n_bits["model_outputs"],
```

## concrete/ml/version.py

```diff
@@ -1,3 +1,3 @@
 """File to manage the version of the package."""
 # Auto-generated by "make set_version" do not modify
-__version__ = "1.0.2"
+__version__ = "1.0.3"
```

## Comparing `concrete_ml-1.0.2.dist-info/LICENSE` & `concrete_ml-1.0.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `concrete_ml-1.0.2.dist-info/METADATA` & `concrete_ml-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concrete-ml
-Version: 1.0.2
+Version: 1.0.3
 Summary: Concrete ML is an open-source set of tools which aims to simplify the use of fully homomorphic encryption (FHE) for data scientists.
 Home-page: https://zama.ai/concrete-ml/
 License: BSD-3-Clause-Clear
 Keywords: FHE,homomorphic encryption,privacy,security
 Author: Zama
 Author-email: hello@zama.ai
 Requires-Python: >=3.8.1,<3.11
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: concrete-ml Version: 1.0.2 Summary: Concrete ML is
+Metadata-Version: 2.1 Name: concrete-ml Version: 1.0.3 Summary: Concrete ML is
 an open-source set of tools which aims to simplify the use of fully homomorphic
 encryption (FHE) for data scientists. Home-page: https://zama.ai/concrete-ml/
 License: BSD-3-Clause-Clear Keywords: FHE,homomorphic
 encryption,privacy,security Author: Zama Author-email: hello@zama.ai Requires-
 Python: >=3.8.1,<3.11 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `concrete_ml-1.0.2.dist-info/RECORD` & `concrete_ml-1.0.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 concrete/__init__.py,sha256=MXQ2ILkTW4ziKnd7dVxTEVOpHe8clGF34EXxmBCF_pk,284
-concrete/ml/__init__.py,sha256=T19QQpjz-kkkO5Dov4vPfmYN7bB5LH-EOQjJLTNrFmg,1722
+concrete/ml/__init__.py,sha256=crXWoSiJuk0P98zSqYPaxNsuzbZzJNayFtjZIBH6Gik,51
 concrete/ml/common/__init__.py,sha256=dXaklwVfEYsMLqyH_YFOjGuxnyzoZuApIm8dKLefybw,95
 concrete/ml/common/check_inputs.py,sha256=wj_oyESYWHemVsPRBC25OQc8a2pX2j7fYGpw8lCeKUA,2519
 concrete/ml/common/debugging/__init__.py,sha256=_eh1MBBmnk2o1M4YGbH0Cbr_cEPjFOVz5wsp080HonE,101
 concrete/ml/common/debugging/custom_assert.py,sha256=H5ESt7cYnDT2PnUXvDaAvUJR2CKHwsHQ4QWtMLvcLZw,2377
-concrete/ml/common/serialization/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-concrete/ml/common/serialization/dumpers.py,sha256=BnoB6S1_TW3tebA0ZQxDFUN3XUnsfVUfsk8yoUXyVW0,1318
-concrete/ml/common/serialization/encoder.py,sha256=TsZ4_FnfWpgk87CpeQDCyqANGmsJ3OlEKmWXBG9fiJk,2018
-concrete/ml/common/serialization/loaders.py,sha256=-ea3oVuHdVRnpMmNFqIHQg71DRfkAGHzaDjwCI2qJKI,2888
-concrete/ml/common/utils.py,sha256=vwPkVK9tItA0k36H_4twivAHJTrlLBKLA_xkXscQh4c,17217
+concrete/ml/common/serialization/__init__.py,sha256=SM3rIzYbRIfp7gDilx5LrrxQ7bpr0ArNkvfhoOpFxGs,1221
+concrete/ml/common/serialization/decoder.py,sha256=Vcus-zDeSA13IwzZGOBfVQy7kPSFz4uHhvR7oX4LCZ4,8204
+concrete/ml/common/serialization/dumpers.py,sha256=uXdo0YHc8WnrlI7NQ78oGdBijpD0vatjgjBEIjrSGF0,601
+concrete/ml/common/serialization/encoder.py,sha256=HJK4huhGwD4Xyooo87v70xAXLfMlzGHHb_fb2QJYxjY,12166
+concrete/ml/common/serialization/loaders.py,sha256=Jz10aCeuvOUIlkmKaChGgSmBR0KDsNgAmKj-UBYod6E,743
+concrete/ml/common/utils.py,sha256=rvDn2roYXJwWoU3OMJ1m72tV9N_66L-tgnzShl5zu0Y,18125
 concrete/ml/deployment/Dockerfile.server,sha256=TbSoyy195L9ttQnEf4YJ70yMuphZRHZvGep1GI4kRlM,235
 concrete/ml/deployment/__init__.py,sha256=jgaPZMSlsJy1KF45EI92rQ7e2CKEpmLdaWcwwFEPeZ8,121
-concrete/ml/deployment/deploy_to_aws.py,sha256=zQO20lozs8X6E3u11bpfK-0KOgT0UXYJvPPDAIqnCZs,17843
+concrete/ml/deployment/deploy_to_aws.py,sha256=P94YtL5e_r50eoNHoiklMQmlsFoRHXw9ge6Tn_7dV9c,17918
 concrete/ml/deployment/deploy_to_docker.py,sha256=c7N9XhbgBajyLiu_TvPRke5kSi6_GdmRtOOPSl-LpoE,3800
-concrete/ml/deployment/fhe_client_server.py,sha256=F8qKjip0-sxOsF-73VUNN1MGuXjfyicl2EKp9_KW4PI,15084
+concrete/ml/deployment/fhe_client_server.py,sha256=OAFnz7scJSIjNvgBeWI5VpRgjrJ4MT8nNFlrj0B06PQ,13873
 concrete/ml/deployment/server.py,sha256=CB6y1v9NPq3NqOE0spzKUMNywFNmhEta8zsn5YIu42o,2590
 concrete/ml/deployment/server_requirements.txt,sha256=gyd07Mp8qZPWhuz7QI1kgYS3JbjcPbZK4cL9RDOR_x8,33
 concrete/ml/deployment/utils.py,sha256=aZFmDRUW58JHAJLK5c--UANMx1sN8C-ioz4JPcPQV-Q,3293
 concrete/ml/onnx/__init__.py,sha256=LiK0TOCAo7c5-TBk4zcO3PEQmdASN0NgLDYIYUXl464,19
 concrete/ml/onnx/convert.py,sha256=LC1YtDL_miK0QKYXzwYwLyBt1PTOXqk247BPS714EnA,3472
 concrete/ml/onnx/onnx_impl_utils.py,sha256=cQ5mfY0VCUMClOy3OGVeddISjWsdoylLu8GundXC4JY,9401
 concrete/ml/onnx/onnx_model_manipulations.py,sha256=fjy-Vqa7Cl6F-O4sft1xKa0z1LZu6X6SnrXj7UtadDQ,9685
 concrete/ml/onnx/onnx_utils.py,sha256=V39Fip97h4F85PlhiQduQPFnNizpGjyGyCHFYOHPon8,20192
 concrete/ml/onnx/ops_impl.py,sha256=Z3yj5zjyllykLmjWus6TSNvMQpPrA7fKGRFFNOYKke0,58079
 concrete/ml/pytest/__init__.py,sha256=5Zk0w3T-MYPF3485ir5kZ1dP7x_VoMIreDMKnJuyBCo,101
-concrete/ml/pytest/torch_models.py,sha256=M9cNkChOKRNYHgQbJ-oHYpQdfswzJxHC21fDG12kqeU,42036
-concrete/ml/pytest/utils.py,sha256=wU1jyx00hZt7m0fn7ljHzHYsepLMpjoPL1KneGqlIdc,8786
+concrete/ml/pytest/torch_models.py,sha256=gRcaixzmf04PwLfVgGCok3uRDdwGmQpoNlnZN2QjvXY,43914
+concrete/ml/pytest/utils.py,sha256=HJF_4OB6WK8fcsQWXe3VSMCMs8CDpSfG3eJnlz2zHlw,14823
 concrete/ml/quantization/__init__.py,sha256=AMEpmLBppr9jRyHOaz9X6dND-u6urnDnkW06X_80JWQ,1081
-concrete/ml/quantization/base_quantized_op.py,sha256=LVJvV56XGK7mHmjzvt-V7V4Rjc9wNfcQDyitV24xTS4,35262
-concrete/ml/quantization/post_training.py,sha256=bxQjVU1UBp2-Y0DB9j9JzezO88D6mGI18gkEJOY0K1I,43525
-concrete/ml/quantization/quantized_module.py,sha256=2k4PzzRxISm9z6IHYMj-EsesoeW6A986Ef-muINR-3A,24352
-concrete/ml/quantization/quantized_ops.py,sha256=PgpCUZlm5byWCL39wMFfIeBuyEq9AvXVyyQKXkylL4Y,80991
-concrete/ml/quantization/quantizers.py,sha256=wlDKxzcFV4EyPhijGcj-EugIMuS_yINCbTg5i_6fEAQ,37549
+concrete/ml/quantization/base_quantized_op.py,sha256=uixLiZ9cz5Uy7zqMNgUKa5RKgAwZqssPU_RVHtPACBo,41430
+concrete/ml/quantization/post_training.py,sha256=mIMTmh7pLUl1RYmrji1nQzpCjyjUm9UYetMP85OZkDQ,43710
+concrete/ml/quantization/quantized_module.py,sha256=IsseO3F9uOPU3EFDKh3cQFyqcFuq36sf9I11wqt-ek8,26450
+concrete/ml/quantization/quantized_ops.py,sha256=orROqe4H0FF8vFIbMqMEW7ojmR3-HGpx2Y63NsQyAzY,81014
+concrete/ml/quantization/quantizers.py,sha256=9qpikdq4EPHB0jKwpM6IqvjO3SddaOGJfNj9lkkRxAE,35671
 concrete/ml/search_parameters/__init__.py,sha256=-TGfmte3AvAn2ajLxLd-FCbru6_Ml9DiKeG7ooR819Q,77
 concrete/ml/search_parameters/p_error_search.py,sha256=SnQ1eIzHNQqIGWPbNMg4obDuN4jV0KDsPPVuCpJbkMU,21193
 concrete/ml/sklearn/__init__.py,sha256=PPR2RuegE_0-OOA9QhYyZ75lxm7rZiAWI4MqeQwRoCo,4679
-concrete/ml/sklearn/base.py,sha256=TEnFPsOpq-0uESbAuunxgiOcF-WWx5LaRIMAbmllLA0,62708
-concrete/ml/sklearn/glm.py,sha256=xca19CFi-QhSTNm9I3anlK7PxEqDx2e1Z9MXw_NKJF8,13633
-concrete/ml/sklearn/linear_model.py,sha256=kQOGeIZjXUUmpSvxCWe-XKd02iY5MuXebvakEWJScvA,25212
-concrete/ml/sklearn/qnn.py,sha256=yyXbHBvhK5eFjVAiSz3pTZwOjNDZJslVSSvJjh833s8,13342
-concrete/ml/sklearn/qnn_module.py,sha256=ZHYlY5N_-UOkooYlQbwNzXKYZCSTyvwO01AFcWl1v1Y,12572
-concrete/ml/sklearn/rf.py,sha256=QSqXnHua77SLFX5crYe5s-XWsmz4AR06QTWSC7uuIOU,12243
-concrete/ml/sklearn/svm.py,sha256=bmfwiJcb28LzPbfiaGiNeHtEug8tzmoBHes_ee4cNgs,10614
-concrete/ml/sklearn/tree.py,sha256=1d2uOLER4HfVWb3tr3nHMEyFTQdpaoq2bjrSPkSHDD8,10394
+concrete/ml/sklearn/base.py,sha256=YZLdnQgAR3T1PsHaI8ssYAVXAI7KK69rd1KDGaqFtAY,64073
+concrete/ml/sklearn/glm.py,sha256=sXbrxrSJ8_lBH6YaWEP4-5_EUbfjZyWUXNuVJ2gfsZY,12899
+concrete/ml/sklearn/linear_model.py,sha256=fIakrELdme6IQWjOr9uYHOnh4uc-Pavtxyvl2IfNHF4,21814
+concrete/ml/sklearn/qnn.py,sha256=4qkIiQK13nw7yVw8-0ZBpmEfGt-zK53BUsJaVj_Wn3k,32152
+concrete/ml/sklearn/qnn_module.py,sha256=y4LQIjDRkCq91Q6ajiNJ7IRb31eezxrrs1tfZvgGZE8,12803
+concrete/ml/sklearn/rf.py,sha256=Qe_mI_A9nEDMDjlqWqibFz_BYq4BvMVJdCAgugXfdHQ,11043
+concrete/ml/sklearn/svm.py,sha256=iHzFYX-u66PRbJjLE-0YvKvGJ4I1cJc_jLDaP4L6RXA,9155
+concrete/ml/sklearn/tree.py,sha256=4Ws9GDjv_G2oe8OGmM6ZM4fBlPcQGFG4XiJqMxavgeo,9191
 concrete/ml/sklearn/tree_to_numpy.py,sha256=NU79gTlaSVqDbIYSNlL9Mo5kB0aQBejegy_P_iFExgQ,10923
-concrete/ml/sklearn/xgb.py,sha256=A_QcoICqydvF5JINuOtd2HISf88RJ_fF96ZEmgZjSHs,20074
+concrete/ml/sklearn/xgb.py,sha256=mvSwn5Kbtl_Pwe0N_2SsseShri4rAo1ByUSps2W7vV4,18962
 concrete/ml/torch/__init__.py,sha256=aUQ25-hJdirZCa20KqaVMrt2PnpnSXBCVw7QvLQ_BoQ,83
-concrete/ml/torch/compile.py,sha256=FFYscm4Wwv9ZUjHQ7J6v86OpSRKUlMsvURXa8GiqxJI,17531
+concrete/ml/torch/compile.py,sha256=Z_Y3zYKjyquQWa9mw-9qlWH72vDI9f7d3G37ltfh3lA,19083
 concrete/ml/torch/numpy_module.py,sha256=PKJmuGL0Q7nzfXsbwz9Mr1J-w5MDGkpzRnZY86TylOI,3174
-concrete/ml/version.py,sha256=1G8dcv4zTVJNlc29PbnHT3oWD-4oWJu2mMVstLHlHrU,124
-concrete_ml-1.0.2.dist-info/LICENSE,sha256=Q2TUW9iqL5JOnEcNTstSvNPYRnF-iQi24FUla8oUEwE,1546
-concrete_ml-1.0.2.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
-concrete_ml-1.0.2.dist-info/METADATA,sha256=usze0z21NQdvyc3uRWfMzE9AUm-ZBuqFYEhvHIVPaSU,11617
-concrete_ml-1.0.2.dist-info/RECORD,,
+concrete/ml/version.py,sha256=2LQo2Ai4U1G5VSXVPXYu54OfSZw7S16Et044wfBHXEA,124
+concrete_ml-1.0.3.dist-info/LICENSE,sha256=Q2TUW9iqL5JOnEcNTstSvNPYRnF-iQi24FUla8oUEwE,1546
+concrete_ml-1.0.3.dist-info/WHEEL,sha256=vxFmldFsRN_Hx10GDvsdv1wroKq8r5Lzvjp6GZ4OO8c,88
+concrete_ml-1.0.3.dist-info/METADATA,sha256=x2AK_So4XtdfuyoZ5bZ5i577_JBWZoDeJQv0uIXX0a8,11617
+concrete_ml-1.0.3.dist-info/RECORD,,
```

