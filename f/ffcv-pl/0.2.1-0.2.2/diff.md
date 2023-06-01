# Comparing `tmp/ffcv_pl-0.2.1.tar.gz` & `tmp/ffcv_pl-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffcv_pl-0.2.1.tar", last modified: Thu May 18 07:51:12 2023, max compression
+gzip compressed data, was "ffcv_pl-0.2.2.tar", last modified: Thu Jun  1 12:19:44 2023, max compression
```

## Comparing `ffcv_pl-0.2.1.tar` & `ffcv_pl-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-18 07:51:11.997060 ffcv_pl-0.2.1/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-05-18 07:51:11.997060 ffcv_pl-0.2.1/PKG-INFO
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-18 07:51:11.997060 ffcv_pl-0.2.1/ffcv_pl/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:34.000000 ffcv_pl-0.2.1/ffcv_pl/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)    11040 2023-05-17 14:35:34.000000 ffcv_pl-0.2.1/ffcv_pl/data_loading.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-18 07:51:11.997060 ffcv_pl-0.2.1/ffcv_pl/ffcv_utils/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.2.1/ffcv_pl/ffcv_utils/__init__.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     1083 2023-01-24 08:22:00.000000 ffcv_pl-0.2.1/ffcv_pl/ffcv_utils/augmentations.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      935 2023-05-17 14:39:06.000000 ffcv_pl-0.2.1/ffcv_pl/ffcv_utils/decoders.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      446 2023-05-10 14:49:01.000000 ffcv_pl-0.2.1/ffcv_pl/ffcv_utils/utils.py
--rw-rw-r--   0 dserez    (1001) dserez    (1001)     2304 2023-05-17 12:45:28.000000 ffcv_pl-0.2.1/ffcv_pl/generate_dataset.py
-drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-05-18 07:51:11.997060 ffcv_pl-0.2.1/ffcv_pl.egg-info/
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-05-18 07:51:11.000000 ffcv_pl-0.2.1/ffcv_pl.egg-info/PKG-INFO
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      360 2023-05-18 07:51:11.000000 ffcv_pl-0.2.1/ffcv_pl.egg-info/SOURCES.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-05-18 07:51:11.000000 ffcv_pl-0.2.1/ffcv_pl.egg-info/dependency_links.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-05-18 07:51:11.000000 ffcv_pl-0.2.1/ffcv_pl.egg-info/not-zip-safe
--rw-rw-r--   0 dserez    (1001) dserez    (1001)        8 2023-05-18 07:51:11.000000 ffcv_pl-0.2.1/ffcv_pl.egg-info/top_level.txt
--rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-05-18 07:51:11.997060 ffcv_pl-0.2.1/setup.cfg
--rw-rw-r--   0 dserez    (1001) dserez    (1001)      433 2023-05-18 07:50:56.000000 ffcv_pl-0.2.1/setup.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/PKG-INFO
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/ffcv_pl/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:34.000000 ffcv_pl-0.2.2/ffcv_pl/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)    12002 2023-06-01 12:19:28.000000 ffcv_pl-0.2.2/ffcv_pl/data_loading.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        0 2023-01-24 09:47:44.000000 ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/__init__.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     1083 2023-01-24 08:22:00.000000 ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/augmentations.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      935 2023-05-17 14:39:06.000000 ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/decoders.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      446 2023-05-10 14:49:01.000000 ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/utils.py
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)     2304 2023-05-17 12:45:28.000000 ffcv_pl-0.2.2/ffcv_pl/generate_dataset.py
+drwxrwxr-x   0 dserez    (1001) dserez    (1001)        0 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/ffcv_pl.egg-info/
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      318 2023-06-01 12:19:44.000000 ffcv_pl-0.2.2/ffcv_pl.egg-info/PKG-INFO
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      360 2023-06-01 12:19:44.000000 ffcv_pl-0.2.2/ffcv_pl.egg-info/SOURCES.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-06-01 12:19:44.000000 ffcv_pl-0.2.2/ffcv_pl.egg-info/dependency_links.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        1 2023-06-01 12:19:44.000000 ffcv_pl-0.2.2/ffcv_pl.egg-info/not-zip-safe
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)        8 2023-06-01 12:19:44.000000 ffcv_pl-0.2.2/ffcv_pl.egg-info/top_level.txt
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)       38 2023-06-01 12:19:44.655077 ffcv_pl-0.2.2/setup.cfg
+-rw-rw-r--   0 dserez    (1001) dserez    (1001)      433 2023-06-01 12:19:28.000000 ffcv_pl-0.2.2/setup.py
```

### Comparing `ffcv_pl-0.2.1/ffcv_pl/data_loading.py` & `ffcv_pl-0.2.2/ffcv_pl/data_loading.py`

 * *Files 7% similar despite different names*

```diff
@@ -138,14 +138,39 @@
                     v_value = None
 
                 if t_value is not None:
                     self.train_pipeline[f'{f}_{i}'] = t_value
                 if v_value is not None:
                     self.val_pipeline[f'{f}_{i}'] = v_value
 
+        elif stage == 'train':
+
+            for i, f in enumerate(self.fields):
+                if f == 'image':
+                    value = self.train_decoders.image_transforms
+                elif f == 'bytes':
+                    value = self.train_decoders.bytes_transforms
+                elif f == 'int':
+                    value = self.train_decoders.int_transforms
+                elif f == 'float':
+                    value = self.train_decoders.float_transforms
+                elif f == 'array':
+                    value = self.train_decoders.array_transforms
+                elif f == 'json':
+                    value = self.train_decoders.json_transforms
+                elif f == 'tensor':
+                    value = self.train_decoders.tensor_transforms
+                else:
+                    value = None
+
+                if value is not None:
+                    pipeline[f'{f}_{i}'] = value
+
+            self.train_pipeline = pipeline
+
         elif stage == 'validate':
 
             for i, f in enumerate(self.fields):
                 if f == 'image':
                     value = self.val_decoders.image_transforms
                 elif f == 'bytes':
                     value = self.val_decoders.bytes_transforms
```

### Comparing `ffcv_pl-0.2.1/ffcv_pl/ffcv_utils/augmentations.py` & `ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/augmentations.py`

 * *Files identical despite different names*

### Comparing `ffcv_pl-0.2.1/ffcv_pl/ffcv_utils/decoders.py` & `ffcv_pl-0.2.2/ffcv_pl/ffcv_utils/decoders.py`

 * *Files identical despite different names*

### Comparing `ffcv_pl-0.2.1/ffcv_pl/generate_dataset.py` & `ffcv_pl-0.2.2/ffcv_pl/generate_dataset.py`

 * *Files identical despite different names*

