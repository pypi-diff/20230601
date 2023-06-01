# Comparing `tmp/torch-pp-0.0.4.dev0.tar.gz` & `tmp/torch-pp-0.0.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-pp-0.0.4.dev0.tar", last modified: Thu Jun  1 18:03:28 2023, max compression
+gzip compressed data, was "torch-pp-0.0.5.dev0.tar", last modified: Thu Jun  1 18:06:17 2023, max compression
```

## Comparing `torch-pp-0.0.4.dev0.tar` & `torch-pp-0.0.5.dev0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:03:28.198741 torch-pp-0.0.4.dev0/
--rw-rw-r--   0 roman     (1000) roman     (1000)     1069 2023-05-19 17:45:40.000000 torch-pp-0.0.4.dev0/LICENSE
--rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-06-01 18:03:28.198741 torch-pp-0.0.4.dev0/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)       68 2023-05-20 02:43:14.000000 torch-pp-0.0.4.dev0/README.md
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-06-01 18:03:28.198741 torch-pp-0.0.4.dev0/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)      307 2023-06-01 18:03:21.000000 torch-pp-0.0.4.dev0/setup.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:03:28.198741 torch-pp-0.0.4.dev0/torch_pp/
--rw-rw-r--   0 roman     (1000) roman     (1000)       43 2023-05-20 02:43:14.000000 torch-pp-0.0.4.dev0/torch_pp/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3804 2023-06-01 18:03:08.000000 torch-pp-0.0.4.dev0/torch_pp/standardscaler.py
--rw-rw-r--   0 roman     (1000) roman     (1000)      199 2023-05-20 19:59:15.000000 torch-pp-0.0.4.dev0/torch_pp/test_.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:03:28.198741 torch-pp-0.0.4.dev0/torch_pp.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-06-01 18:03:28.000000 torch-pp-0.0.4.dev0/torch_pp.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)      220 2023-06-01 18:03:28.000000 torch-pp-0.0.4.dev0/torch_pp.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-06-01 18:03:28.000000 torch-pp-0.0.4.dev0/torch_pp.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        9 2023-06-01 18:03:28.000000 torch-pp-0.0.4.dev0/torch_pp.egg-info/top_level.txt
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:06:17.594335 torch-pp-0.0.5.dev0/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1069 2023-05-19 17:45:40.000000 torch-pp-0.0.5.dev0/LICENSE
+-rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-06-01 18:06:17.594335 torch-pp-0.0.5.dev0/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)       68 2023-05-20 02:43:14.000000 torch-pp-0.0.5.dev0/README.md
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-06-01 18:06:17.594335 torch-pp-0.0.5.dev0/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)      307 2023-06-01 18:06:13.000000 torch-pp-0.0.5.dev0/setup.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:06:17.594335 torch-pp-0.0.5.dev0/torch_pp/
+-rw-rw-r--   0 roman     (1000) roman     (1000)       43 2023-05-20 02:43:14.000000 torch-pp-0.0.5.dev0/torch_pp/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3832 2023-06-01 18:06:06.000000 torch-pp-0.0.5.dev0/torch_pp/standardscaler.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      199 2023-05-20 19:59:15.000000 torch-pp-0.0.5.dev0/torch_pp/test_.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 18:06:17.594335 torch-pp-0.0.5.dev0/torch_pp.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-06-01 18:06:17.000000 torch-pp-0.0.5.dev0/torch_pp.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)      220 2023-06-01 18:06:17.000000 torch-pp-0.0.5.dev0/torch_pp.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-06-01 18:06:17.000000 torch-pp-0.0.5.dev0/torch_pp.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        9 2023-06-01 18:06:17.000000 torch-pp-0.0.5.dev0/torch_pp.egg-info/top_level.txt
```

### Comparing `torch-pp-0.0.4.dev0/LICENSE` & `torch-pp-0.0.5.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-pp-0.0.4.dev0/torch_pp/standardscaler.py` & `torch-pp-0.0.5.dev0/torch_pp/standardscaler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import torch
 
 
 class StandardScaler:
-    n_samples_seen = 0
-    scale, mean, var = None, None, None
-
     def __init__(self, with_mean=True, with_std=True):
         self.with_mean = with_mean
         self.with_std = with_std
 
+        self.n_samples_seen = 0
+        self.scale, self.mean, self.var = None, None, None
+
     def fit_transform(self, _input: torch.Tensor) -> torch.Tensor:
         self.partial_fit(_input)
         return self.transform(_input)
 
     def reset(self):
         self.n_samples_seen = 0
         return self
```

