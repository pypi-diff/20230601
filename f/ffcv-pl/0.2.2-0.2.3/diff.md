# Comparing `tmp/ffcv_pl-0.2.2.tar.gz` & `tmp/ffcv_pl-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffcv_pl-0.2.2.tar", last modified: Thu Jun  1 12:19:44 2023, max compression
+gzip compressed data, was "ffcv_pl-0.2.3.tar", last modified: Thu Jun  1 13:21:24 2023, max compression
```

## Comparing `ffcv_pl-0.2.2.tar` & `ffcv_pl-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/PKG-INFO
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/ffcv_pl/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:34.000000 ffcv_pl-0.2.2/ffcv_pl/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    12002 2023-06-01 12:19:28.000000 ffcv_pl-0.2.2/ffcv_pl/data_loading.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     1083 2023-01-24 08:22:00.000000 ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/augmentations.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      935 2023-05-17 14:39:06.000000 ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/decoders.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      446 2023-05-10 14:49:01.000000 ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/utils.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     2304 2023-05-17 12:45:28.000000 ffcv_pl-0.2.2/ffcv_pl/generate_dataset.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/ffcv_pl.egg-info/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-06-01 12:19:44.000000 ffcv_pl-0.2.2/ffcv_pl.egg-info/PKG-INFO
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      360 2023-06-01 12:19:44.000000 ffcv_pl-0.2.2/ffcv_pl.egg-info/SOURCES.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-06-01 12:19:44.000000 ffcv_pl-0.2.2/ffcv_pl.egg-info/dependency_links.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-06-01 12:19:44.000000 ffcv_pl-0.2.2/ffcv_pl.egg-info/not-zip-safe
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        8 2023-06-01 12:19:44.000000 ffcv_pl-0.2.2/ffcv_pl.egg-info/top_level.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/setup.cfg
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      433 2023-06-01 12:19:28.000000 ffcv_pl-0.2.2/setup.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 13:21:24.249804 ffcv_pl-0.2.3/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-06-01 13:21:24.245804 ffcv_pl-0.2.3/PKG-INFO
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 13:21:24.245804 ffcv_pl-0.2.3/ffcv_pl/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:34.000000 ffcv_pl-0.2.3/ffcv_pl/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    11222 2023-06-01 13:21:01.000000 ffcv_pl-0.2.3/ffcv_pl/data_loading.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 13:21:24.245804 ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1083 2023-01-24 08:22:00.000000 ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/augmentations.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      935 2023-05-17 14:39:06.000000 ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/decoders.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      446 2023-05-10 14:49:01.000000 ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/utils.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     2304 2023-05-17 12:45:28.000000 ffcv_pl-0.2.3/ffcv_pl/generate_dataset.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 13:21:24.245804 ffcv_pl-0.2.3/ffcv_pl.egg-info/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-06-01 13:21:24.000000 ffcv_pl-0.2.3/ffcv_pl.egg-info/PKG-INFO
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      360 2023-06-01 13:21:24.000000 ffcv_pl-0.2.3/ffcv_pl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-06-01 13:21:24.000000 ffcv_pl-0.2.3/ffcv_pl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-06-01 12:19:44.000000 ffcv_pl-0.2.3/ffcv_pl.egg-info/not-zip-safe
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        8 2023-06-01 13:21:24.000000 ffcv_pl-0.2.3/ffcv_pl.egg-info/top_level.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-06-01 13:21:24.249804 ffcv_pl-0.2.3/setup.cfg
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      433 2023-06-01 13:21:19.000000 ffcv_pl-0.2.3/setup.py
```

### Comparing `ffcv_pl-0.2.2/ffcv_pl/data_loading.py` & `ffcv_pl-0.2.3/ffcv_pl/data_loading.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytorch_lightning as pl
+from pytorch_lightning.trainer.trainer import TrainerFn
 from ffcv.fields import Field
 from ffcv.loader import Loader, OrderOption
 import warnings
 from ffcv_pl.ffcv_utils.decoders import FFCVDecoders
 from ffcv_pl.ffcv_utils.utils import field_to_str
 
 
@@ -102,15 +103,15 @@
         """
         pass
 
     def setup(self, stage: str) -> None:
 
         pipeline = {}
 
-        if stage == 'fit':
+        if stage == 'fit' or stage == TrainerFn.FITTING:
 
             self.train_pipeline = {}
             self.val_pipeline = {}
 
             for i, f in enumerate(self.fields):
                 if f == 'image':
                     t_value = self.train_decoders.image_transforms
@@ -138,40 +139,15 @@
                     v_value = None
 
                 if t_value is not None:
                     self.train_pipeline[f'{f}_{i}'] = t_value
                 if v_value is not None:
                     self.val_pipeline[f'{f}_{i}'] = v_value
 
-        elif stage == 'train':
-
-            for i, f in enumerate(self.fields):
-                if f == 'image':
-                    value = self.train_decoders.image_transforms
-                elif f == 'bytes':
-                    value = self.train_decoders.bytes_transforms
-                elif f == 'int':
-                    value = self.train_decoders.int_transforms
-                elif f == 'float':
-                    value = self.train_decoders.float_transforms
-                elif f == 'array':
-                    value = self.train_decoders.array_transforms
-                elif f == 'json':
-                    value = self.train_decoders.json_transforms
-                elif f == 'tensor':
-                    value = self.train_decoders.tensor_transforms
-                else:
-                    value = None
-
-                if value is not None:
-                    pipeline[f'{f}_{i}'] = value
-
-            self.train_pipeline = pipeline
-
-        elif stage == 'validate':
+        elif stage == 'validate' or stage == TrainerFn.VALIDATING:
 
             for i, f in enumerate(self.fields):
                 if f == 'image':
                     value = self.val_decoders.image_transforms
                 elif f == 'bytes':
                     value = self.val_decoders.bytes_transforms
                 elif f == 'int':
@@ -188,15 +164,15 @@
                     value = None
 
                 if value is not None:
                     pipeline[f'{f}_{i}'] = value
 
             self.val_pipeline = pipeline
 
-        elif stage == 'test':
+        elif stage == 'test' or stage == TrainerFn.TESTING:
 
             for i, f in enumerate(self.fields):
                 if f == 'image':
                     value = self.test_decoders.image_transforms
                 elif f == 'bytes':
                     value = self.test_decoders.bytes_transforms
                 elif f == 'int':
@@ -213,15 +189,15 @@
                     value = None
 
                 if value is not None:
                     pipeline[f'{f}_{i}'] = value
 
             self.test_pipeline = pipeline
 
-        elif stage == 'predict':
+        elif stage == 'predict' or stage == TrainerFn.PREDICTING:
 
             for i, f in enumerate(self.fields):
                 if f == 'image':
                     value = self.predict_decoders.image_transforms
                 elif f == 'bytes':
                     value = self.predict_decoders.bytes_transforms
                 elif f == 'int':
```

### Comparing `ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/augmentations.py` & `ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/decoders.py` & `ffcv_pl-0.2.3/ffcv_pl/ffcv_utils/decoders.py`

 * *Files identical despite different names*

### Comparing `ffcv_pl-0.2.2/ffcv_pl/generate_dataset.py` & `ffcv_pl-0.2.3/ffcv_pl/generate_dataset.py`

 * *Files identical despite different names*

