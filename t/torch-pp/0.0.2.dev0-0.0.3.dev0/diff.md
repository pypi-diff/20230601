# Comparing `tmp/torch-pp-0.0.2.dev0.tar.gz` & `tmp/torch-pp-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch-pp-0.0.2.dev0.tar", last modified: Sat May 20 19:35:29 2023, max compression
+gzip compressed data, was "torch-pp-0.0.3.dev0.tar", last modified: Thu Jun  1 17:58:20 2023, max compression
```

## Comparing `torch-pp-0.0.2.dev0.tar` & `torch-pp-0.0.3.dev0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-20 19:35:29.793068 torch-pp-0.0.2.dev0/
--rw-rw-r--   0 roman     (1000) roman     (1000)     1069 2023-05-19 17:45:40.000000 torch-pp-0.0.2.dev0/LICENSE
--rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-05-20 19:35:29.793068 torch-pp-0.0.2.dev0/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)       68 2023-05-20 02:43:14.000000 torch-pp-0.0.2.dev0/README.md
--rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-05-20 19:35:29.793068 torch-pp-0.0.2.dev0/setup.cfg
--rw-rw-r--   0 roman     (1000) roman     (1000)      307 2023-05-20 19:35:28.000000 torch-pp-0.0.2.dev0/setup.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-20 19:35:29.793068 torch-pp-0.0.2.dev0/torch_pp/
--rw-rw-r--   0 roman     (1000) roman     (1000)       43 2023-05-20 02:43:14.000000 torch-pp-0.0.2.dev0/torch_pp/__init__.py
--rw-rw-r--   0 roman     (1000) roman     (1000)     3741 2023-05-20 19:35:11.000000 torch-pp-0.0.2.dev0/torch_pp/standardscaler.py
-drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-05-20 19:35:29.793068 torch-pp-0.0.2.dev0/torch_pp.egg-info/
--rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-05-20 19:35:29.000000 torch-pp-0.0.2.dev0/torch_pp.egg-info/PKG-INFO
--rw-rw-r--   0 roman     (1000) roman     (1000)      202 2023-05-20 19:35:29.000000 torch-pp-0.0.2.dev0/torch_pp.egg-info/SOURCES.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-05-20 19:35:29.000000 torch-pp-0.0.2.dev0/torch_pp.egg-info/dependency_links.txt
--rw-rw-r--   0 roman     (1000) roman     (1000)        9 2023-05-20 19:35:29.000000 torch-pp-0.0.2.dev0/torch_pp.egg-info/top_level.txt
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 17:58:20.116334 torch-pp-0.0.3.dev0/
+-rw-rw-r--   0 roman     (1000) roman     (1000)     1069 2023-05-19 17:45:40.000000 torch-pp-0.0.3.dev0/LICENSE
+-rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-06-01 17:58:20.116334 torch-pp-0.0.3.dev0/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)       68 2023-05-20 02:43:14.000000 torch-pp-0.0.3.dev0/README.md
+-rw-rw-r--   0 roman     (1000) roman     (1000)       38 2023-06-01 17:58:20.116334 torch-pp-0.0.3.dev0/setup.cfg
+-rw-rw-r--   0 roman     (1000) roman     (1000)      307 2023-06-01 17:58:09.000000 torch-pp-0.0.3.dev0/setup.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 17:58:20.116334 torch-pp-0.0.3.dev0/torch_pp/
+-rw-rw-r--   0 roman     (1000) roman     (1000)       43 2023-05-20 02:43:14.000000 torch-pp-0.0.3.dev0/torch_pp/__init__.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)     3799 2023-06-01 17:57:35.000000 torch-pp-0.0.3.dev0/torch_pp/standardscaler.py
+-rw-rw-r--   0 roman     (1000) roman     (1000)      199 2023-05-20 19:59:15.000000 torch-pp-0.0.3.dev0/torch_pp/test_.py
+drwxrwxr-x   0 roman     (1000) roman     (1000)        0 2023-06-01 17:58:20.116334 torch-pp-0.0.3.dev0/torch_pp.egg-info/
+-rw-rw-r--   0 roman     (1000) roman     (1000)      247 2023-06-01 17:58:20.000000 torch-pp-0.0.3.dev0/torch_pp.egg-info/PKG-INFO
+-rw-rw-r--   0 roman     (1000) roman     (1000)      220 2023-06-01 17:58:20.000000 torch-pp-0.0.3.dev0/torch_pp.egg-info/SOURCES.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        1 2023-06-01 17:58:20.000000 torch-pp-0.0.3.dev0/torch_pp.egg-info/dependency_links.txt
+-rw-rw-r--   0 roman     (1000) roman     (1000)        9 2023-06-01 17:58:20.000000 torch-pp-0.0.3.dev0/torch_pp.egg-info/top_level.txt
```

### Comparing `torch-pp-0.0.2.dev0/LICENSE` & `torch-pp-0.0.3.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `torch-pp-0.0.2.dev0/torch_pp/standardscaler.py` & `torch-pp-0.0.3.dev0/torch_pp/standardscaler.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,18 @@
         def fn(value):
             return value if value != 0 else 1
 
         self.scale = self.var.apply_(fn)
         self.scale = torch.sqrt(self.scale)
 
     def transform(self, x: torch.Tensor):
-        return self.__transform(x, lambda v, mean, scale: (v - mean) / scale)
+        return self.__transform(x, forward_)
 
     def inverse_transform(self, x: torch.Tensor):
-        return self.__transform(x, lambda v, mean, scale: mean + v * scale)
+        return self.__transform(x, inverse_)
 
     def __transform(self, x: torch.Tensor, fn):
         x_out = x.clone()
         n_features = x.shape[1]
         for i in range(n_features):
             mean, scale = 0., 1.
             if self.with_mean:
@@ -52,14 +52,22 @@
                 scale = self.scale[i]
             for j in range(self.n_samples_seen):
                 x_out[j, i] = fn(x[j, i], mean, scale)
 
         return x_out
 
 
+def inverse_(v, mean, scale):
+    return mean + v * scale
+
+
+def forward_(v, mean, scale):
+    return (v - mean) / scale
+
+
 def incremental_mean_and_var(x: torch.Tensor, last_mean: torch.Tensor, last_variance: torch.Tensor,
                              last_sample_count: int):
     new_sample_count = x.shape[0]
     n_features = x.shape[1]
     last_sum = last_mean.clone()
     last_sum = torch.mul(last_sum, float(last_sample_count))
     new_sum = torch.zeros(n_features)
```

