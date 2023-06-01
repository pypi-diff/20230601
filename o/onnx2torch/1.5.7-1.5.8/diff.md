# Comparing `tmp/onnx2torch-1.5.7.tar.gz` & `tmp/onnx2torch-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx2torch-1.5.7.tar", last modified: Fri May 26 18:18:33 2023, max compression
+gzip compressed data, was "onnx2torch-1.5.8.tar", last modified: Thu Jun  1 16:23:13 2023, max compression
```

## Comparing `onnx2torch-1.5.7.tar` & `onnx2torch-1.5.8.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 seny      (1000) seny      (1000)        0 2023-05-26 18:18:33.982380 onnx2torch-1.5.7/
--rw-r--r--   0 seny      (1000) seny      (1000)    11337 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/LICENSE
--rw-r--r--   0 seny      (1000) seny      (1000)       78 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/MANIFEST.in
--rw-r--r--   0 seny      (1000) seny      (1000)     9032 2023-05-26 18:18:33.982380 onnx2torch-1.5.7/PKG-INFO
--rw-r--r--   0 seny      (1000) seny      (1000)     8601 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/README.md
-drwxr-xr-x   0 seny      (1000) seny      (1000)        0 2023-05-26 18:18:33.980380 onnx2torch-1.5.7/onnx2torch/
--rw-r--r--   0 seny      (1000) seny      (1000)        6 2023-05-26 18:18:01.000000 onnx2torch-1.5.7/onnx2torch/VERSION
--rw-r--r--   0 seny      (1000) seny      (1000)       41 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/__init__.py
--rw-r--r--   0 seny      (1000) seny      (1000)     6995 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/converter.py
-drwxr-xr-x   0 seny      (1000) seny      (1000)        0 2023-05-26 18:18:33.982380 onnx2torch-1.5.7/onnx2torch/node_converters/
--rw-r--r--   0 seny      (1000) seny      (1000)     2749 2023-04-11 04:48:53.000000 onnx2torch-1.5.7/onnx2torch/node_converters/__init__.py
--rw-r--r--   0 seny      (1000) seny      (1000)     9189 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/activations.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2161 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/average_pool.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1314 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/base_element_wise.py
--rw-r--r--   0 seny      (1000) seny      (1000)     3728 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/batch_norm.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2717 2023-02-16 06:35:52.000000 onnx2torch-1.5.7/onnx2torch/node_converters/binary_math_operations.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1980 2023-02-10 09:35:59.000000 onnx2torch-1.5.7/onnx2torch/node_converters/cast.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2965 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/clip.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1837 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/comparisons.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1211 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/concat.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2019 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/constant.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1649 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/constant_of_shape.py
--rw-r--r--   0 seny      (1000) seny      (1000)     3432 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/conv.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2821 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/cumsum.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1895 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/dropout.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1054 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/einsum.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1407 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/expand.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2492 2023-04-11 04:48:53.000000 onnx2torch-1.5.7/onnx2torch/node_converters/eye_like.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1471 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/flatten.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2203 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/functions.py
--rw-r--r--   0 seny      (1000) seny      (1000)     6352 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/gather.py
--rw-r--r--   0 seny      (1000) seny      (1000)     3282 2023-03-15 08:53:08.000000 onnx2torch-1.5.7/onnx2torch/node_converters/gemm.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2444 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/global_average_pool.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1333 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/identity.py
--rw-r--r--   0 seny      (1000) seny      (1000)     3129 2023-03-14 20:36:03.000000 onnx2torch-1.5.7/onnx2torch/node_converters/instance_norm.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2926 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/logical.py
--rw-r--r--   0 seny      (1000) seny      (1000)      894 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/lrn.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1030 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/matmul.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2396 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/max_pool.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1294 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/mean.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1621 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/min_max.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1298 2023-03-14 20:36:37.000000 onnx2torch-1.5.7/onnx2torch/node_converters/mod.py
--rw-r--r--   0 seny      (1000) seny      (1000)      985 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/neg.py
--rw-r--r--   0 seny      (1000) seny      (1000)     4906 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/nms.py
--rw-r--r--   0 seny      (1000) seny      (1000)     4811 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/pad.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2338 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/pow.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1543 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/range.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1008 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/reciprocal.py
--rw-r--r--   0 seny      (1000) seny      (1000)     9559 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/reduce.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1847 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/registry.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1846 2023-03-30 16:47:39.000000 onnx2torch-1.5.7/onnx2torch/node_converters/reshape.py
--rw-r--r--   0 seny      (1000) seny      (1000)     6482 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/resize.py
--rw-r--r--   0 seny      (1000) seny      (1000)     5557 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/roialign.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1386 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/roundings.py
--rw-r--r--   0 seny      (1000) seny      (1000)     3574 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/scatter_nd.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2460 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/shape.py
--rw-r--r--   0 seny      (1000) seny      (1000)     4338 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/slice.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2803 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/split.py
--rw-r--r--   0 seny      (1000) seny      (1000)     3465 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/squeeze.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1211 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/sum.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1423 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/tile.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1813 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/topk.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1712 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/transpose.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2940 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/node_converters/unsqueeze.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1048 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/node_converters/where.py
--rw-r--r--   0 seny      (1000) seny      (1000)     4373 2023-03-15 08:53:08.000000 onnx2torch-1.5.7/onnx2torch/onnx_graph.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2620 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/onnx_node.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1241 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/onnx_tensor.py
-drwxr-xr-x   0 seny      (1000) seny      (1000)        0 2023-05-26 18:18:33.982380 onnx2torch-1.5.7/onnx2torch/utils/
--rw-r--r--   0 seny      (1000) seny      (1000)        0 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/utils/__init__.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2542 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/utils/common.py
--rw-r--r--   0 seny      (1000) seny      (1000)     3193 2023-02-20 05:24:42.000000 onnx2torch-1.5.7/onnx2torch/utils/custom_export_to_onnx.py
--rw-r--r--   0 seny      (1000) seny      (1000)     2247 2023-04-11 04:48:53.000000 onnx2torch-1.5.7/onnx2torch/utils/dtype.py
--rw-r--r--   0 seny      (1000) seny      (1000)      633 2023-02-10 09:35:59.000000 onnx2torch-1.5.7/onnx2torch/utils/indices.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1124 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/utils/padding.py
--rw-r--r--   0 seny      (1000) seny      (1000)     1620 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/onnx2torch/utils/safe_shape_inference.py
-drwxr-xr-x   0 seny      (1000) seny      (1000)        0 2023-05-26 18:18:33.980380 onnx2torch-1.5.7/onnx2torch.egg-info/
--rw-r--r--   0 seny      (1000) seny      (1000)     9032 2023-05-26 18:18:33.000000 onnx2torch-1.5.7/onnx2torch.egg-info/PKG-INFO
--rw-r--r--   0 seny      (1000) seny      (1000)     2714 2023-05-26 18:18:33.000000 onnx2torch-1.5.7/onnx2torch.egg-info/SOURCES.txt
--rw-r--r--   0 seny      (1000) seny      (1000)        1 2023-05-26 18:18:33.000000 onnx2torch-1.5.7/onnx2torch.egg-info/dependency_links.txt
--rw-r--r--   0 seny      (1000) seny      (1000)       58 2023-05-26 18:18:33.000000 onnx2torch-1.5.7/onnx2torch.egg-info/requires.txt
--rw-r--r--   0 seny      (1000) seny      (1000)       17 2023-05-26 18:18:33.000000 onnx2torch-1.5.7/onnx2torch.egg-info/top_level.txt
--rw-r--r--   0 seny      (1000) seny      (1000)      247 2023-02-10 09:35:59.000000 onnx2torch-1.5.7/pyproject.toml
--rw-r--r--   0 seny      (1000) seny      (1000)       58 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/requirements.txt
--rw-r--r--   0 seny      (1000) seny      (1000)       38 2023-05-26 18:18:33.982380 onnx2torch-1.5.7/setup.cfg
--rw-r--r--   0 seny      (1000) seny      (1000)     1435 2022-12-26 09:38:31.000000 onnx2torch-1.5.7/setup.py
+drwxr-xr-x   0 seny      (1000) seny      (1000)        0 2023-06-01 16:23:13.304255 onnx2torch-1.5.8/
+-rw-r--r--   0 seny      (1000) seny      (1000)    11337 2023-06-01 16:22:22.000000 onnx2torch-1.5.8/LICENSE
+-rw-r--r--   0 seny      (1000) seny      (1000)       78 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/MANIFEST.in
+-rw-r--r--   0 seny      (1000) seny      (1000)     9032 2023-06-01 16:23:13.304255 onnx2torch-1.5.8/PKG-INFO
+-rw-r--r--   0 seny      (1000) seny      (1000)     8601 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/README.md
+drwxr-xr-x   0 seny      (1000) seny      (1000)        0 2023-06-01 16:23:13.302255 onnx2torch-1.5.8/onnx2torch/
+-rw-r--r--   0 seny      (1000) seny      (1000)        6 2023-06-01 16:22:32.000000 onnx2torch-1.5.8/onnx2torch/VERSION
+-rw-r--r--   0 seny      (1000) seny      (1000)       41 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/__init__.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     6995 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/converter.py
+drwxr-xr-x   0 seny      (1000) seny      (1000)        0 2023-06-01 16:23:13.304255 onnx2torch-1.5.8/onnx2torch/node_converters/
+-rw-r--r--   0 seny      (1000) seny      (1000)     2749 2023-04-11 04:48:53.000000 onnx2torch-1.5.8/onnx2torch/node_converters/__init__.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     9189 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/activations.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2161 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/average_pool.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1314 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/base_element_wise.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     3728 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/batch_norm.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2717 2023-02-16 06:35:52.000000 onnx2torch-1.5.8/onnx2torch/node_converters/binary_math_operations.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1980 2023-02-10 09:35:59.000000 onnx2torch-1.5.8/onnx2torch/node_converters/cast.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2965 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/clip.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1837 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/comparisons.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1211 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/concat.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2019 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/constant.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1649 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/constant_of_shape.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     3432 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/conv.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2821 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/cumsum.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1895 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/dropout.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1054 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/einsum.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1407 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/expand.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2492 2023-04-11 04:48:53.000000 onnx2torch-1.5.8/onnx2torch/node_converters/eye_like.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1471 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/flatten.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2203 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/functions.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     6352 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/gather.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     3282 2023-03-15 08:53:08.000000 onnx2torch-1.5.8/onnx2torch/node_converters/gemm.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2444 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/global_average_pool.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1333 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/identity.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     3129 2023-03-14 20:36:03.000000 onnx2torch-1.5.8/onnx2torch/node_converters/instance_norm.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2926 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/logical.py
+-rw-r--r--   0 seny      (1000) seny      (1000)      894 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/lrn.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1030 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/matmul.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2396 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/max_pool.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1294 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/mean.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1621 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/min_max.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1298 2023-03-14 20:36:37.000000 onnx2torch-1.5.8/onnx2torch/node_converters/mod.py
+-rw-r--r--   0 seny      (1000) seny      (1000)      985 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/neg.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     4906 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/nms.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     4811 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/pad.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2338 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/pow.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2100 2023-06-01 16:09:16.000000 onnx2torch-1.5.8/onnx2torch/node_converters/range.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1008 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/reciprocal.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     9559 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/reduce.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1847 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/registry.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1846 2023-03-30 16:47:39.000000 onnx2torch-1.5.8/onnx2torch/node_converters/reshape.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     6482 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/resize.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     5557 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/roialign.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1386 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/roundings.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     3574 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/scatter_nd.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2460 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/shape.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     4338 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/slice.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2803 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/split.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     3465 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/squeeze.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1211 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/sum.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1423 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/tile.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1813 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/topk.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1712 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/transpose.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2940 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/node_converters/unsqueeze.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1048 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/node_converters/where.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     4373 2023-03-15 08:53:08.000000 onnx2torch-1.5.8/onnx2torch/onnx_graph.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2620 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/onnx_node.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1241 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/onnx_tensor.py
+drwxr-xr-x   0 seny      (1000) seny      (1000)        0 2023-06-01 16:23:13.304255 onnx2torch-1.5.8/onnx2torch/utils/
+-rw-r--r--   0 seny      (1000) seny      (1000)        0 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/utils/__init__.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2542 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/utils/common.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     3193 2023-02-20 05:24:42.000000 onnx2torch-1.5.8/onnx2torch/utils/custom_export_to_onnx.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     2247 2023-04-11 04:48:53.000000 onnx2torch-1.5.8/onnx2torch/utils/dtype.py
+-rw-r--r--   0 seny      (1000) seny      (1000)      633 2023-02-10 09:35:59.000000 onnx2torch-1.5.8/onnx2torch/utils/indices.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1124 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/utils/padding.py
+-rw-r--r--   0 seny      (1000) seny      (1000)     1620 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/onnx2torch/utils/safe_shape_inference.py
+drwxr-xr-x   0 seny      (1000) seny      (1000)        0 2023-06-01 16:23:13.302255 onnx2torch-1.5.8/onnx2torch.egg-info/
+-rw-r--r--   0 seny      (1000) seny      (1000)     9032 2023-06-01 16:23:13.000000 onnx2torch-1.5.8/onnx2torch.egg-info/PKG-INFO
+-rw-r--r--   0 seny      (1000) seny      (1000)     2714 2023-06-01 16:23:13.000000 onnx2torch-1.5.8/onnx2torch.egg-info/SOURCES.txt
+-rw-r--r--   0 seny      (1000) seny      (1000)        1 2023-06-01 16:23:13.000000 onnx2torch-1.5.8/onnx2torch.egg-info/dependency_links.txt
+-rw-r--r--   0 seny      (1000) seny      (1000)       58 2023-06-01 16:23:13.000000 onnx2torch-1.5.8/onnx2torch.egg-info/requires.txt
+-rw-r--r--   0 seny      (1000) seny      (1000)       17 2023-06-01 16:23:13.000000 onnx2torch-1.5.8/onnx2torch.egg-info/top_level.txt
+-rw-r--r--   0 seny      (1000) seny      (1000)      247 2023-06-01 16:22:22.000000 onnx2torch-1.5.8/pyproject.toml
+-rw-r--r--   0 seny      (1000) seny      (1000)       58 2022-12-26 09:38:31.000000 onnx2torch-1.5.8/requirements.txt
+-rw-r--r--   0 seny      (1000) seny      (1000)       38 2023-06-01 16:23:13.304255 onnx2torch-1.5.8/setup.cfg
+-rw-r--r--   0 seny      (1000) seny      (1000)     1435 2023-06-01 16:21:02.000000 onnx2torch-1.5.8/setup.py
```

### Comparing `onnx2torch-1.5.7/LICENSE` & `onnx2torch-1.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/PKG-INFO` & `onnx2torch-1.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2torch
-Version: 1.5.7
+Version: 1.5.8
 Summary: Nice Onnx to Pytorch converter
 Home-page: https://github.com/ENOT-AutoDL/onnx2torch
 Author: ENOT LLC
 Author-email: enot@enot.ai
 License: apache-2.0
 Keywords: AI,onnx,torch,onnx2torch,converters
 Classifier: Programming Language :: Python :: 3
```

### Comparing `onnx2torch-1.5.7/README.md` & `onnx2torch-1.5.8/README.md`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/converter.py` & `onnx2torch-1.5.8/onnx2torch/converter.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/__init__.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/__init__.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/activations.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/activations.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/average_pool.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/average_pool.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/base_element_wise.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/base_element_wise.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/batch_norm.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/batch_norm.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/binary_math_operations.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/binary_math_operations.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/cast.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/cast.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/clip.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/clip.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/comparisons.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/comparisons.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/concat.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/concat.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/constant.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/constant.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/constant_of_shape.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/constant_of_shape.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/conv.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/conv.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/cumsum.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/cumsum.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/dropout.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/einsum.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/einsum.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/expand.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/expand.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/eye_like.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/eye_like.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/flatten.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/flatten.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/functions.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/functions.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/gather.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/gather.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/gemm.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/gemm.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/global_average_pool.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/global_average_pool.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/identity.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/identity.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/instance_norm.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/instance_norm.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/logical.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/logical.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/lrn.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/lrn.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/matmul.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/matmul.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/max_pool.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/max_pool.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/mean.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/mean.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/min_max.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/min_max.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/mod.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/mod.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/neg.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/neg.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/nms.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/nms.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/pad.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/pad.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/pow.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/pow.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/range.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/range.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,44 +6,58 @@
 
 import torch
 from torch import nn
 
 from onnx2torch.node_converters.registry import add_converter
 from onnx2torch.onnx_graph import OnnxGraph
 from onnx2torch.onnx_node import OnnxNode
-from onnx2torch.utils.common import OnnxToTorchModule
 from onnx2torch.utils.common import OperationConverterResult
 from onnx2torch.utils.common import onnx_mapping_from_node
+from onnx2torch.utils.custom_export_to_onnx import DefaultExportToOnnx
+from onnx2torch.utils.custom_export_to_onnx import OnnxToTorchModuleWithCustomExport
 
 
-class OnnxRange(nn.Module, OnnxToTorchModule):  # pylint: disable=missing-class-docstring
+class OnnxRange(nn.Module, OnnxToTorchModuleWithCustomExport):  # pylint: disable=missing-class-docstring
     def __init__(self):
         super().__init__()
         self.register_buffer('dummy_buffer', torch.Tensor(), persistent=False)
 
     @staticmethod
     def _get_scalar(value) -> Union[float, int]:
         if isinstance(value, torch.Tensor):
             return value.item()
 
         return value
 
-    def forward(  # pylint: disable=missing-function-docstring
+    def _arange(
         self,
         start: Union[torch.Tensor, float, int],
         limit: Union[torch.Tensor, float, int],
         delta: Union[torch.Tensor, float, int],
     ) -> torch.Tensor:
         return torch.arange(
             start=self._get_scalar(start),
             end=self._get_scalar(limit),
             step=self._get_scalar(delta),
             device=self.dummy_buffer.device,
         )
 
+    def forward(  # pylint: disable=missing-function-docstring
+        self,
+        start: Union[torch.Tensor, float, int],
+        limit: Union[torch.Tensor, float, int],
+        delta: Union[torch.Tensor, float, int],
+    ) -> torch.Tensor:
+        forward_lambda = lambda: self._arange(start, limit, delta)
+
+        if torch.onnx.is_in_onnx_export():
+            return DefaultExportToOnnx.export(forward_lambda, 'Range', start, limit, delta, {})
+
+        return forward_lambda()
+
 
 @add_converter(operation_type='Range', version=11)
 def _(node: OnnxNode, graph: OnnxGraph) -> OperationConverterResult:  # pylint: disable=unused-argument
     return OperationConverterResult(
         torch_module=OnnxRange(),
         onnx_mapping=onnx_mapping_from_node(node),
     )
```

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/reciprocal.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/reciprocal.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/reduce.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/reduce.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/registry.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/registry.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/reshape.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/reshape.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/resize.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/resize.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/roialign.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/roialign.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/roundings.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/roundings.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/scatter_nd.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/scatter_nd.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/shape.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/shape.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/slice.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/split.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/split.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/squeeze.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/squeeze.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/sum.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/sum.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/tile.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/tile.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/topk.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/topk.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/transpose.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/transpose.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/unsqueeze.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/unsqueeze.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/node_converters/where.py` & `onnx2torch-1.5.8/onnx2torch/node_converters/where.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/onnx_graph.py` & `onnx2torch-1.5.8/onnx2torch/onnx_graph.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/onnx_node.py` & `onnx2torch-1.5.8/onnx2torch/onnx_node.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/onnx_tensor.py` & `onnx2torch-1.5.8/onnx2torch/onnx_tensor.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/utils/common.py` & `onnx2torch-1.5.8/onnx2torch/utils/common.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/utils/custom_export_to_onnx.py` & `onnx2torch-1.5.8/onnx2torch/utils/custom_export_to_onnx.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/utils/dtype.py` & `onnx2torch-1.5.8/onnx2torch/utils/dtype.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/utils/indices.py` & `onnx2torch-1.5.8/onnx2torch/utils/indices.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/utils/padding.py` & `onnx2torch-1.5.8/onnx2torch/utils/padding.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch/utils/safe_shape_inference.py` & `onnx2torch-1.5.8/onnx2torch/utils/safe_shape_inference.py`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/onnx2torch.egg-info/PKG-INFO` & `onnx2torch-1.5.8/onnx2torch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onnx2torch
-Version: 1.5.7
+Version: 1.5.8
 Summary: Nice Onnx to Pytorch converter
 Home-page: https://github.com/ENOT-AutoDL/onnx2torch
 Author: ENOT LLC
 Author-email: enot@enot.ai
 License: apache-2.0
 Keywords: AI,onnx,torch,onnx2torch,converters
 Classifier: Programming Language :: Python :: 3
```

### Comparing `onnx2torch-1.5.7/onnx2torch.egg-info/SOURCES.txt` & `onnx2torch-1.5.8/onnx2torch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onnx2torch-1.5.7/setup.py` & `onnx2torch-1.5.8/setup.py`

 * *Files identical despite different names*

