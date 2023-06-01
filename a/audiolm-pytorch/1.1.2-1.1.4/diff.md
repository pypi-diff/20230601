# Comparing `tmp/audiolm-pytorch-1.1.2.tar.gz` & `tmp/audiolm-pytorch-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiolm-pytorch-1.1.2.tar", last modified: Wed May 31 04:12:38 2023, max compression
+gzip compressed data, was "audiolm-pytorch-1.1.4.tar", last modified: Thu Jun  1 03:08:09 2023, max compression
```

## Comparing `audiolm-pytorch-1.1.2.tar` & `audiolm-pytorch-1.1.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:12:38.251283 audiolm-pytorch-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-31 04:12:38.251283 audiolm-pytorch-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18271 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:12:38.251283 audiolm-pytorch-1.1.2/audiolm_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    65656 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/audiolm_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/encodec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/hubert_kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/soundstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/audiolm_pytorch/vq_wav2vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 04:12:38.251283 audiolm-pytorch-1.1.2/audiolm_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-31 04:12:38.000000 audiolm-pytorch-1.1.2/audiolm_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-31 04:12:38.000000 audiolm-pytorch-1.1.2/audiolm_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 04:12:38.000000 audiolm-pytorch-1.1.2/audiolm_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-31 04:12:38.000000 audiolm-pytorch-1.1.2/audiolm_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-31 04:12:38.000000 audiolm-pytorch-1.1.2/audiolm_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 04:12:38.251283 audiolm-pytorch-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-31 04:12:27.000000 audiolm-pytorch-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:08:09.608938 audiolm-pytorch-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-01 03:08:09.608938 audiolm-pytorch-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18271 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:08:09.608938 audiolm-pytorch-1.1.4/audiolm_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65767 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/audiolm_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/encodec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/hubert_kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30270 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/soundstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2548 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42310 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/audiolm_pytorch/vq_wav2vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 03:08:09.608938 audiolm-pytorch-1.1.4/audiolm_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-06-01 03:08:09.000000 audiolm-pytorch-1.1.4/audiolm_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-01 03:08:09.000000 audiolm-pytorch-1.1.4/audiolm_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 03:08:09.000000 audiolm-pytorch-1.1.4/audiolm_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-01 03:08:09.000000 audiolm-pytorch-1.1.4/audiolm_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 03:08:09.000000 audiolm-pytorch-1.1.4/audiolm_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 03:08:09.608938 audiolm-pytorch-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-06-01 03:07:55.000000 audiolm-pytorch-1.1.4/setup.py
```

### Comparing `audiolm-pytorch-1.1.2/LICENSE` & `audiolm-pytorch-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/PKG-INFO` & `audiolm-pytorch-1.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.1.2
+Version: 1.1.4
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.1.2/README.md` & `audiolm-pytorch-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch/__init__.py` & `audiolm-pytorch-1.1.4/audiolm_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch/audiolm_pytorch.py` & `audiolm-pytorch-1.1.4/audiolm_pytorch/audiolm_pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1117,14 +1117,17 @@
         self.eos_id = transformer.eos_id
         self.mask_prob = mask_prob
 
     @property
     def device(self):
         return next(self.parameters()).device
 
+    def embed_text(self, text):
+        return self.transformer.embed_text(text, output_device = self.device)
+
     @eval_decorator
     @torch.no_grad()
     @beartype
     def generate(
         self,
         *,
         max_length,
```

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch/data.py` & `audiolm-pytorch-1.1.4/audiolm_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch/encodec.py` & `audiolm-pytorch-1.1.4/audiolm_pytorch/encodec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch/hubert_kmeans.py` & `audiolm-pytorch-1.1.4/audiolm_pytorch/hubert_kmeans.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch/optimizer.py` & `audiolm-pytorch-1.1.4/audiolm_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch/soundstream.py` & `audiolm-pytorch-1.1.4/audiolm_pytorch/soundstream.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch/t5.py` & `audiolm-pytorch-1.1.4/audiolm_pytorch/t5.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch/trainer.py` & `audiolm-pytorch-1.1.4/audiolm_pytorch/trainer.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch/vq_wav2vec.py` & `audiolm-pytorch-1.1.4/audiolm_pytorch/vq_wav2vec.py`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch.egg-info/PKG-INFO` & `audiolm-pytorch-1.1.4/audiolm_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audiolm-pytorch
-Version: 1.1.2
+Version: 1.1.4
 Summary: AudioLM - Language Modeling Approach to Audio Generation from Google Research - Pytorch
 Home-page: https://github.com/lucidrains/audiolm-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,audio generation
 Classifier: Development Status :: 4 - Beta
```

### Comparing `audiolm-pytorch-1.1.2/audiolm_pytorch.egg-info/SOURCES.txt` & `audiolm-pytorch-1.1.4/audiolm_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `audiolm-pytorch-1.1.2/setup.py` & `audiolm-pytorch-1.1.4/setup.py`

 * *Files identical despite different names*

