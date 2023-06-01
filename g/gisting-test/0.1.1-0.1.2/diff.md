# Comparing `tmp/gisting_test-0.1.1.tar.gz` & `tmp/gisting_test-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gisting_test-0.1.1.tar", last modified: Thu Jun  1 17:50:55 2023, max compression
+gzip compressed data, was "gisting_test-0.1.2.tar", last modified: Thu Jun  1 18:29:52 2023, max compression
```

## Comparing `gisting_test-0.1.1.tar` & `gisting_test-0.1.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:50:55.273925 gisting_test-0.1.1/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-01 17:50:55.273828 gisting_test-0.1.1/PKG-INFO
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:50:55.269913 gisting_test-0.1.1/gisting_test/
--rw-r--r--   0 owaiszahid   (501) staff       (20)       18 2023-06-01 17:36:38.000000 gisting_test-0.1.1/gisting_test/__init__.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:50:55.273123 gisting_test-0.1.1/gisting_test/src/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:49:51.000000 gisting_test-0.1.1/gisting_test/src/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/arguments.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/benchmarking.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8804 2023-06-01 17:19:37.000000 gisting_test-0.1.1/gisting_test/src/compress.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:50:55.273620 gisting_test-0.1.1/gisting_test/src/data/
--rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/data/__init__.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/data/gist.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/data/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/generation_utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/gist_caching.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/gist_llama.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/gist_t5.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/integrations.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/metrics.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/train.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/trainer_seq2seq.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/utils.py
--rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 23:00:39.000000 gisting_test-0.1.1/gisting_test/src/weight_diff.py
-drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:50:55.270424 gisting_test-0.1.1/gisting_test.egg-info/
--rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-01 17:50:55.000000 gisting_test-0.1.1/gisting_test.egg-info/PKG-INFO
--rw-r--r--   0 owaiszahid   (501) staff       (20)      703 2023-06-01 17:50:55.000000 gisting_test-0.1.1/gisting_test.egg-info/SOURCES.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-06-01 17:50:55.000000 gisting_test-0.1.1/gisting_test.egg-info/dependency_links.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       52 2023-06-01 17:50:55.000000 gisting_test-0.1.1/gisting_test.egg-info/top_level.txt
--rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-06-01 17:50:55.273960 gisting_test-0.1.1/setup.cfg
--rw-r--r--   0 owaiszahid   (501) staff       (20)      411 2023-06-01 17:50:48.000000 gisting_test-0.1.1/setup.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-01 18:29:52.479542 gisting_test-0.1.2/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-01 18:29:52.479421 gisting_test-0.1.2/PKG-INFO
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-01 18:29:52.471924 gisting_test-0.1.2/gisting_test/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       18 2023-06-01 17:36:38.000000 gisting_test-0.1.2/gisting_test/__init__.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-01 18:29:52.478736 gisting_test-0.1.2/gisting_test/src/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-06-01 17:49:51.000000 gisting_test-0.1.2/gisting_test/src/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    11076 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/arguments.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     3462 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/benchmarking.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8782 2023-06-01 18:29:20.000000 gisting_test-0.1.2/gisting_test/src/compress.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-01 18:29:52.479192 gisting_test-0.1.2/gisting_test/src/data/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        0 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/data/__init__.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     8550 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/data/gist.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      554 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/data/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    21595 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/generation_utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4748 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/gist_caching.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    34287 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/gist_llama.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    41427 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/gist_t5.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     2954 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/integrations.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     4277 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/metrics.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    13819 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/train.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)    52559 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/trainer_seq2seq.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      426 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/utils.py
+-rw-r--r--   0 owaiszahid   (501) staff       (20)     7880 2023-05-30 23:00:39.000000 gisting_test-0.1.2/gisting_test/src/weight_diff.py
+drwxr-xr-x   0 owaiszahid   (501) staff       (20)        0 2023-06-01 18:29:52.472642 gisting_test-0.1.2/gisting_test.egg-info/
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      288 2023-06-01 18:29:52.000000 gisting_test-0.1.2/gisting_test.egg-info/PKG-INFO
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      703 2023-06-01 18:29:52.000000 gisting_test-0.1.2/gisting_test.egg-info/SOURCES.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)        1 2023-06-01 18:29:52.000000 gisting_test-0.1.2/gisting_test.egg-info/dependency_links.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       52 2023-06-01 18:29:52.000000 gisting_test-0.1.2/gisting_test.egg-info/top_level.txt
+-rw-r--r--   0 owaiszahid   (501) staff       (20)       38 2023-06-01 18:29:52.479589 gisting_test-0.1.2/setup.cfg
+-rw-r--r--   0 owaiszahid   (501) staff       (20)      411 2023-06-01 18:29:39.000000 gisting_test-0.1.2/setup.py
```

### Comparing `gisting_test-0.1.1/gisting_test/src/arguments.py` & `gisting_test-0.1.2/gisting_test/src/arguments.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/benchmarking.py` & `gisting_test-0.1.2/gisting_test/src/benchmarking.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/compress.py` & `gisting_test-0.1.2/gisting_test/src/compress.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,20 +94,19 @@
         model, _ = weight_diff.recover(
             path_raw=base_llama_path,
             path_diff=model_name_or_path,
             test_inference=False,
             cache_dir=cache_dir,
         )
     else:
-        model = model_cls.from_pretrained(
+        model = torch.nn.DataParallel(model_cls.from_pretrained(
             model_name_or_path,
             config=config,
             cache_dir=cache_dir,
-        )
-        model = torch.nn.DataParallel(model, device_ids=[0, 1, 2])
+        ), device_ids=[0, 1, 2])
 
     dtypes = {
         "bf16": torch.bfloat16,
         "fp16": torch.float16,
         "fp32": torch.float,
     }
     model = model.to(dtypes[precision]).cuda().eval()
```

### Comparing `gisting_test-0.1.1/gisting_test/src/data/gist.py` & `gisting_test-0.1.2/gisting_test/src/data/gist.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/data/utils.py` & `gisting_test-0.1.2/gisting_test/src/data/utils.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/generation_utils.py` & `gisting_test-0.1.2/gisting_test/src/generation_utils.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/gist_caching.py` & `gisting_test-0.1.2/gisting_test/src/gist_caching.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/gist_llama.py` & `gisting_test-0.1.2/gisting_test/src/gist_llama.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/gist_t5.py` & `gisting_test-0.1.2/gisting_test/src/gist_t5.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/integrations.py` & `gisting_test-0.1.2/gisting_test/src/integrations.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/metrics.py` & `gisting_test-0.1.2/gisting_test/src/metrics.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/train.py` & `gisting_test-0.1.2/gisting_test/src/train.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/trainer_seq2seq.py` & `gisting_test-0.1.2/gisting_test/src/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test/src/weight_diff.py` & `gisting_test-0.1.2/gisting_test/src/weight_diff.py`

 * *Files identical despite different names*

### Comparing `gisting_test-0.1.1/gisting_test.egg-info/SOURCES.txt` & `gisting_test-0.1.2/gisting_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

