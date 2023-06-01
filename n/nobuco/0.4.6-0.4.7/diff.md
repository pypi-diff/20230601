# Comparing `tmp/nobuco-0.4.6.tar.gz` & `tmp/nobuco-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nobuco-0.4.6.tar", last modified: Wed May 17 10:53:17 2023, max compression
+gzip compressed data, was "nobuco-0.4.7.tar", last modified: Thu Jun  1 14:22:09 2023, max compression
```

## Comparing `nobuco-0.4.6.tar` & `nobuco-0.4.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.679828 nobuco-0.4.6/
--rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.6/LICENSE
--rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-05-17 10:53:17.679828 nobuco-0.4.6/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)    20237 2023-05-17 10:50:20.000000 nobuco-0.4.6/README.md
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco/
--rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/commons.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    13631 2023-04-25 18:12:50.000000 nobuco-0.4.6/nobuco/convert.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco/converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/channel_ordering.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/node_converter.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2091 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/tensor.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/type_cast.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3874 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/converters/validation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco/entity/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/entity/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/entity/keras.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.4.6/nobuco/entity/pytorch.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/funcs.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco/layers/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/layers/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/layers/channel_order.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/layers/container.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/layers/stub.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/layers/weight.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco/locate/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/locate/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/locate/link.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/locate/locate.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.679828 nobuco-0.4.6/nobuco/node_converters/
--rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/__init__.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     6206 2023-05-04 09:06:58.000000 nobuco-0.4.6/nobuco/node_converters/activation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/boolean.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/boolean_mask.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3352 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/comparison.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.4.6/nobuco/node_converters/convolution.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/dropout.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/interpolation.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.6/nobuco/node_converters/linear.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11116 2023-05-04 09:33:42.000000 nobuco-0.4.6/nobuco/node_converters/math.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.4.6/nobuco/node_converters/misc.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     2434 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/normalization.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/padding.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3095 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/pooling.py
--rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/recurrent.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/node_converters/slice.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.4.6/nobuco/node_converters/tensor_cast.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3161 2023-05-16 10:06:21.000000 nobuco-0.4.6/nobuco/node_converters/tensor_creation.py
--rw-rw-r--   0 alex      (1000) alex      (1000)    11126 2023-05-17 10:49:15.000000 nobuco-0.4.6/nobuco/node_converters/tensor_manipulation.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.679828 nobuco-0.4.6/nobuco/trace/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/trace/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/trace/tensor_storage.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/trace/trace.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/util.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.679828 nobuco-0.4.6/nobuco/vis/
--rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/vis/__init__.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/vis/console_stylizer.py
--rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.6/nobuco/vis/html_stylizer.py
-drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-05-17 10:53:17.675828 nobuco-0.4.6/nobuco.egg-info/
--rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-05-17 10:53:17.000000 nobuco-0.4.6/nobuco.egg-info/PKG-INFO
--rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-05-17 10:53:17.000000 nobuco-0.4.6/nobuco.egg-info/SOURCES.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-05-17 10:53:17.000000 nobuco-0.4.6/nobuco.egg-info/dependency_links.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-05-17 10:53:17.000000 nobuco-0.4.6/nobuco.egg-info/requires.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-05-17 10:53:17.000000 nobuco-0.4.6/nobuco.egg-info/top_level.txt
--rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-05-17 10:51:39.000000 nobuco-0.4.6/pyproject.toml
--rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-05-17 10:53:17.679828 nobuco-0.4.6/setup.cfg
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.274314 nobuco-0.4.7/
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1074 2023-04-25 18:07:04.000000 nobuco-0.4.7/LICENSE
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-01 14:22:09.274314 nobuco-0.4.7/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)    20237 2023-05-17 10:50:20.000000 nobuco-0.4.7/README.md
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.266314 nobuco-0.4.7/nobuco/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      533 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1270 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/commons.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    13631 2023-04-25 18:12:50.000000 nobuco-0.4.7/nobuco/convert.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.270314 nobuco-0.4.7/nobuco/converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/converters/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2397 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/converters/channel_ordering.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1761 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/converters/node_converter.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2131 2023-05-17 15:16:26.000000 nobuco-0.4.7/nobuco/converters/tensor.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1322 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/converters/type_cast.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     4060 2023-06-01 13:59:37.000000 nobuco-0.4.7/nobuco/converters/validation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.270314 nobuco-0.4.7/nobuco/entity/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/entity/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      739 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/entity/keras.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    14874 2023-05-17 10:49:40.000000 nobuco-0.4.7/nobuco/entity/pytorch.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1316 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/funcs.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.270314 nobuco-0.4.7/nobuco/layers/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/layers/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4992 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/layers/channel_order.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     4524 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/layers/container.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      313 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/layers/stub.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      910 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/layers/weight.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.270314 nobuco-0.4.7/nobuco/locate/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/locate/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      785 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/locate/link.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      599 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/locate/locate.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.274314 nobuco-0.4.7/nobuco/node_converters/
+-rw-rw-r--   0 alex      (1000) alex      (1000)      210 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/__init__.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     6206 2023-05-04 09:06:58.000000 nobuco-0.4.7/nobuco/node_converters/activation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)      901 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/boolean.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1211 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/boolean_mask.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3504 2023-06-01 14:17:46.000000 nobuco-0.4.7/nobuco/node_converters/comparison.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)    20101 2023-05-03 16:03:42.000000 nobuco-0.4.7/nobuco/node_converters/convolution.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)      754 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/dropout.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1343 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/interpolation.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     5086 2023-05-01 12:01:37.000000 nobuco-0.4.7/nobuco/node_converters/linear.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    13828 2023-06-01 14:04:11.000000 nobuco-0.4.7/nobuco/node_converters/math.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1814 2023-05-16 10:06:23.000000 nobuco-0.4.7/nobuco/node_converters/misc.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     1638 2023-05-17 15:16:26.000000 nobuco-0.4.7/nobuco/node_converters/normalization.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1357 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/padding.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     2879 2023-05-17 15:16:26.000000 nobuco-0.4.7/nobuco/node_converters/pooling.py
+-rwxrwxr-x   0 alex      (1000) alex      (1000)     3332 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/node_converters/recurrent.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     6824 2023-05-23 14:56:11.000000 nobuco-0.4.7/nobuco/node_converters/slice.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3895 2023-05-17 10:46:04.000000 nobuco-0.4.7/nobuco/node_converters/tensor_cast.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3161 2023-05-16 10:06:21.000000 nobuco-0.4.7/nobuco/node_converters/tensor_creation.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)    11126 2023-05-17 10:49:15.000000 nobuco-0.4.7/nobuco/node_converters/tensor_manipulation.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.274314 nobuco-0.4.7/nobuco/trace/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/trace/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1409 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/trace/tensor_storage.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     9421 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/trace/trace.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     2776 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/util.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.274314 nobuco-0.4.7/nobuco/vis/
+-rw-rw-r--   0 alex      (1000) alex      (1000)        0 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/vis/__init__.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1934 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/vis/console_stylizer.py
+-rw-rw-r--   0 alex      (1000) alex      (1000)     3158 2023-04-25 18:07:04.000000 nobuco-0.4.7/nobuco/vis/html_stylizer.py
+drwxrwxr-x   0 alex      (1000) alex      (1000)        0 2023-06-01 14:22:09.270314 nobuco-0.4.7/nobuco.egg-info/
+-rw-rw-r--   0 alex      (1000) alex      (1000)    22071 2023-06-01 14:22:09.000000 nobuco-0.4.7/nobuco.egg-info/PKG-INFO
+-rw-rw-r--   0 alex      (1000) alex      (1000)     1589 2023-06-01 14:22:09.000000 nobuco-0.4.7/nobuco.egg-info/SOURCES.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        1 2023-06-01 14:22:09.000000 nobuco-0.4.7/nobuco.egg-info/dependency_links.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)       17 2023-06-01 14:22:09.000000 nobuco-0.4.7/nobuco.egg-info/requires.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)        7 2023-06-01 14:22:09.000000 nobuco-0.4.7/nobuco.egg-info/top_level.txt
+-rw-rw-r--   0 alex      (1000) alex      (1000)      770 2023-06-01 14:21:20.000000 nobuco-0.4.7/pyproject.toml
+-rw-rw-r--   0 alex      (1000) alex      (1000)       38 2023-06-01 14:22:09.274314 nobuco-0.4.7/setup.cfg
```

### Comparing `nobuco-0.4.6/LICENSE` & `nobuco-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/PKG-INFO` & `nobuco-0.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.6
+Version: 0.4.7
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.4.6/README.md` & `nobuco-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/__init__.py` & `nobuco-0.4.7/nobuco/__init__.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/commons.py` & `nobuco-0.4.7/nobuco/commons.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/convert.py` & `nobuco-0.4.7/nobuco/convert.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/converters/channel_ordering.py` & `nobuco-0.4.7/nobuco/converters/channel_ordering.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/converters/node_converter.py` & `nobuco-0.4.7/nobuco/converters/node_converter.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/converters/tensor.py` & `nobuco-0.4.7/nobuco/converters/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
 
 def _dims_make_positive(dims, n_dims, add_one=False):
     return [_dim_make_positive(d, n_dims, add_one) for d in dims]
 
 
 def dim_pytorch2keras(dim, num_dims):
+    if dim is None:
+        return dim
+
     dim = _dim_make_positive(dim, num_dims)
     if dim == 0:
         return dim
     elif dim == 1:
         return num_dims - 1
     else:
         return dim - 1
```

### Comparing `nobuco-0.4.6/nobuco/converters/type_cast.py` & `nobuco-0.4.7/nobuco/converters/type_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/converters/validation.py` & `nobuco-0.4.7/nobuco/converters/validation.py`

 * *Files 6% similar despite different names*

```diff
@@ -74,14 +74,17 @@
     outputs_tf = collect_recursively(outputs_tf, TF_TENSOR_CLASSES)
     outputs_tf_converted = [t_keras2pytorch(t, restore_channel_order=True) for t in outputs_tf]
 
     # with torch.no_grad():
     #     outputs_pt = pytorch_op(*args_pt, **kwargs_pt)
     #     outputs_pt = collect_recursively(outputs_pt, torch.Tensor)
 
+    if len(outputs_tf_converted) != len(outputs_pt):
+        raise Exception(f"Number of outputs do not match: (Pytorch) {len(outputs_pt)} vs {len(outputs_tf_converted)} (Tensorflow)")
+
     for t_tf, t_pt in zip(outputs_tf_converted, outputs_pt):
         if t_tf.shape != t_pt.shape:
             raise Exception(f"Tensor shapes don't match: (Pytorch) {list(t_pt.shape)} vs {list(t_tf.shape)} (Tensorflow)")
 
         if t_tf.dtype != t_pt.dtype:
             raise Exception(f"Tensor dtypes don't match: (Pytorch) {t_pt.dtype} vs {t_tf.dtype} (Tensorflow)")
```

### Comparing `nobuco-0.4.6/nobuco/entity/keras.py` & `nobuco-0.4.7/nobuco/entity/keras.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/entity/pytorch.py` & `nobuco-0.4.7/nobuco/entity/pytorch.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/funcs.py` & `nobuco-0.4.7/nobuco/funcs.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/layers/channel_order.py` & `nobuco-0.4.7/nobuco/layers/channel_order.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/layers/container.py` & `nobuco-0.4.7/nobuco/layers/container.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/layers/weight.py` & `nobuco-0.4.7/nobuco/layers/weight.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/locate/link.py` & `nobuco-0.4.7/nobuco/locate/link.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/locate/locate.py` & `nobuco-0.4.7/nobuco/locate/locate.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/activation.py` & `nobuco-0.4.7/nobuco/node_converters/activation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/boolean.py` & `nobuco-0.4.7/nobuco/node_converters/boolean.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/boolean_mask.py` & `nobuco-0.4.7/nobuco/node_converters/boolean_mask.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/comparison.py` & `nobuco-0.4.7/nobuco/node_converters/comparison.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,15 +63,18 @@
     def func(self, dim=-1, descending=False):
         if get_channel_order(self) == ChannelOrder.TENSORFLOW:
             dim = dim_pytorch2keras(dim, n_dims)
         if descending:
             direction = 'DESCENDING'
         else:
             direction = 'ASCENDING'
-        return tf.sort(self, axis=dim, direction=direction)
+        sorted = tf.sort(self, axis=dim, direction=direction)
+        argsorted = tf.argsort(self, axis=dim, direction=direction)
+        argsorted = tf.cast(argsorted, tf.int64)
+        return sorted, argsorted
     return func
 
 
 @converter(torch.unique, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_unique(input, sorted=True, return_inverse=False, return_counts=False, dim=None):
     def func(input, sorted=True, return_inverse=False, return_counts=False, dim=None):
         assert len(input.shape) == 1
```

### Comparing `nobuco-0.4.6/nobuco/node_converters/convolution.py` & `nobuco-0.4.7/nobuco/node_converters/convolution.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/dropout.py` & `nobuco-0.4.7/nobuco/node_converters/dropout.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/interpolation.py` & `nobuco-0.4.7/nobuco/node_converters/interpolation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/linear.py` & `nobuco-0.4.7/nobuco/node_converters/linear.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/math.py` & `nobuco-0.4.7/nobuco/node_converters/math.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Optional, Union, List, Tuple, Sequence, Any
 
 from torch import Tensor
-from torch.types import _int, _bool, Number, _dtype, _size
+from torch.types import _int, _bool, Number, _dtype, _size, _layout, _device
 
 import tensorflow as tf
 import torch
 
 from nobuco.commons import ChannelOrder, ChannelOrderingStrategy
 from nobuco.converters.channel_ordering import set_channel_order, get_channel_order
 from nobuco.converters.node_converter import converter
-from nobuco.converters.tensor import _dim_make_positive, dim_pytorch2keras, perm_keras2pytorch, _permute
+from nobuco.converters.tensor import _dim_make_positive, dim_pytorch2keras, perm_keras2pytorch, _permute, \
+    perm_pytorch2keras
 
 
 @converter(torch.sum, torch.Tensor.sum, channel_ordering_strategy=ChannelOrderingStrategy.MANUAL)
 def converter_sum(input: Tensor, dim: Sequence, keepdim: _bool=False, *, dtype: Optional[_dtype]=None, out: Optional[Tensor]=None):
     n_dims = input.dim()
 
     def func(input, dim, keepdim=False, *, dtype=None, out=None):
@@ -55,26 +56,29 @@
                 perm = perm_keras2pytorch(n_dims)
                 input = _permute(perm)(input)
             out = tf.reduce_mean(input, axis=dim, keepdims=keepdim)
             out = set_channel_order(out, ChannelOrder.PYTORCH)
             return out
     return func
 
+
 @converter(torch.sin, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_sin(input, *args, **kwargs):
     def func(input, *args, **kwargs):
         return tf.math.sin(input)
     return func
 
+
 @converter(torch.cos, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_cos(input, *args, **kwargs):
     def func(input, *args, **kwargs):
         return tf.math.cos(input)
     return func
 
+
 @converter(torch.Tensor.add, torch.Tensor.__add__, torch.Tensor.__iadd__, torch.Tensor.__radd__, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS_OR_PYTORCH, autocast=True)
 def converter_add(input, other, *args, **kwargs):
     def func(input, other, *args, **kwargs):
         return input + other
     return func
 
 
@@ -226,38 +230,92 @@
 @converter(torch.clamp, torch.Tensor.clamp, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_clamp(input: Tensor, min: Optional[Number]=None, max: Optional[Number]=None, *, out: Optional[Tensor]=None):
     def func(input, min=None, max=None, *, out=None):
         return tf.keras.backend.clip(input, min_value=min, max_value=max)
     return func
 
 
-@converter(torch.min, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+@converter(torch.minimum, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_minimum(input: Tensor, other: Tensor, *, out: Optional[Tensor]=None):
+    def func(input, other, *, out=None):
+        return tf.minimum(input, other)
+    return func
+
+
+@converter(torch.maximum, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_maximum(input: Tensor, other: Tensor, *, out: Optional[Tensor]=None):
+    def func(input, other, *, out=None):
+        return tf.maximum(input, other)
+    return func
+
+
+@converter(torch.min, torch.Tensor.min, channel_ordering_strategy=ChannelOrderingStrategy.MANUAL)
 def converter_min(input: Tensor, dim=None, keepdim: _bool=False, *, out: Union[Tensor, Tuple[Tensor, ...], List[Tensor]]=None):
     n_dims = input.dim()
 
+    if isinstance(dim, Tensor):
+        return converter_minimum.convert(input, dim, out=out)
+
     def func(input, dim=None, keepdim=False, *, out=None):
-        if dim is not None and get_channel_order(input) == ChannelOrder.TENSORFLOW:
-            dim = dim_pytorch2keras(dim, n_dims)
-        return tf.keras.backend.min(input, axis=dim, keepdims=keepdim)
+        if dim is None:
+            x = tf.keras.backend.min(input, axis=dim, keepdims=keepdim)
+            return set_channel_order(x, get_channel_order(input))
+        else:
+            if get_channel_order(input) == ChannelOrder.TENSORFLOW:
+                input = _permute(perm_keras2pytorch(n_dims))(input)
+                input = set_channel_order(input, ChannelOrder.PYTORCH)
+            x = tf.keras.backend.min(input, axis=dim, keepdims=keepdim)
+            a = tf.keras.backend.argmin(input, axis=dim)
+            order = get_channel_order(input)
+            return set_channel_order(x, order), set_channel_order(a, order)
     return func
 
 
-@converter(torch.max, torch.Tensor.max, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+@converter(torch.max, torch.Tensor.max, channel_ordering_strategy=ChannelOrderingStrategy.MANUAL)
 def converter_max(input: Tensor, dim=None, keepdim: _bool=False, *, out: Union[Tensor, Tuple[Tensor, ...], List[Tensor]]=None):
     n_dims = input.dim()
 
+    if isinstance(dim, Tensor):
+        return converter_maximum.convert(input, dim, out=out)
+
+    def func(input, dim=None, keepdim=False, *, out=None):
+        if dim is None:
+            x = tf.keras.backend.max(input, axis=dim, keepdims=keepdim)
+            return set_channel_order(x, get_channel_order(input))
+        else:
+            if get_channel_order(input) == ChannelOrder.TENSORFLOW:
+                input = _permute(perm_keras2pytorch(n_dims))(input)
+                input = set_channel_order(input, ChannelOrder.PYTORCH)
+            x = tf.keras.backend.max(input, axis=dim, keepdims=keepdim)
+            a = tf.keras.backend.argmax(input, axis=dim)
+            order = get_channel_order(input)
+            return set_channel_order(x, order), set_channel_order(a, order)
+    return func
+
+
+@converter(torch.argmin, torch.Tensor.argmin, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_argmin(input: Tensor, dim: Optional[_int]=None, keepdim: _bool=False, *, out: Optional[Tensor]=None):
+    n_dims = input.dim()
+
     def func(input, dim=None, keepdim=False, *, out=None):
-        if dim is not None and get_channel_order(input) == ChannelOrder.TENSORFLOW:
+        if get_channel_order(input) == ChannelOrder.TENSORFLOW:
             dim = dim_pytorch2keras(dim, n_dims)
-        return tf.keras.backend.max(input, axis=dim, keepdims=keepdim)
+        return tf.keras.backend.argmin(input, axis=dim)
     return func
 
 
 @converter(torch.argmax, torch.Tensor.argmax, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
 def converter_argmax(input: Tensor, dim: Optional[_int]=None, keepdim: _bool=False, *, out: Optional[Tensor]=None):
     n_dims = input.dim()
 
     def func(input, dim=None, keepdim=False, *, out=None):
-        if dim is not None and get_channel_order(input) == ChannelOrder.TENSORFLOW:
+        if get_channel_order(input) == ChannelOrder.TENSORFLOW:
             dim = dim_pytorch2keras(dim, n_dims)
         return tf.keras.backend.argmax(input, axis=dim)
     return func
+
+
+@converter(torch.arange, channel_ordering_strategy=ChannelOrderingStrategy.MINIMUM_TRANSPOSITIONS)
+def converter_arange(start: Number, end: Number, step: Number=1, *, out: Optional[Tensor]=None, dtype: Optional[_dtype]=None, layout: Optional[_layout]=None, device: Optional[Union[_device, str, None]]=None, pin_memory: Optional[_bool]=False, requires_grad: Optional[_bool]=False):
+    def func(start, end, step=1, *, out=None, dtype=None, layout=None, device=None, pin_memory=False, requires_grad=False):
+        return tf.range(start, limit=end, delta=step)
+    return func
```

### Comparing `nobuco-0.4.6/nobuco/node_converters/misc.py` & `nobuco-0.4.7/nobuco/node_converters/misc.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/normalization.py` & `nobuco-0.4.7/nobuco/node_converters/normalization.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,31 +25,14 @@
     return layer
 
     # def func(input, *args, **kwargs):
     #     return (input - running_mean) / (tf.sqrt(running_var + epsilon)) * weight + bias
     # return func
 
 
-# @converter(F.batch_norm)
-# def converter_batch_norm(input: Tensor,
-#                running_mean: Optional[Tensor], running_var: Optional[Tensor],
-#                weight: Optional[Tensor] = None, bias: Optional[Tensor] = None,
-#                training: bool = False, momentum: float = 0.1, eps: float = 1e-5):
-#     weight = weight.detach().numpy()
-#     bias = bias.detach().numpy()
-#     running_mean = running_mean.detach().numpy()
-#     running_var = running_var.detach().numpy()
-#     bn = keras.layers.BatchNormalization(momentum=1 - momentum, epsilon=eps, weights=[weight, bias, running_mean, running_var])
-#
-#     def func(input, *args, **kwargs):
-#         return bn(input)
-#         # return (input - running_mean) / (tf.sqrt(running_var + eps)) * weight + bias
-#     return func
-
-
 @converter(F.layer_norm, channel_ordering_strategy=ChannelOrderingStrategy.FORCE_PYTORCH_ORDER)
 def converter_layer_norm(input: Tensor,
                normalized_shape: List[int],
                weight: Optional[Tensor] = None,
                bias: Optional[Tensor] = None,
                eps: float = 1e-5
                ):
```

### Comparing `nobuco-0.4.6/nobuco/node_converters/padding.py` & `nobuco-0.4.7/nobuco/node_converters/padding.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/pooling.py` & `nobuco-0.4.7/nobuco/node_converters/pooling.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,14 @@
 from tensorflow import keras
 import torch
 import torch.nn.functional as F
 
 from nobuco.converters.node_converter import converter
 
 
-# @converter(nn.MaxPool2d)
-# def converter_MaxPool2D(self, input: Tensor):
-#     kernel_size = self.kernel_size
-#     stride = self.stride
-#     return keras.layers.MaxPool2D(pool_size=kernel_size, strides=stride)
-
-
 @converter(torch.max_pool2d)
 def converter_max_pool_2d(input: Tensor, kernel_size: Union[_int, _size], stride: Union[_int, _size]=(), padding: Union[_int, _size]=0, dilation: Union[_int, _size]=1, ceil_mode: _bool=False):
     if isinstance(kernel_size, numbers.Number):
         kernel_size = (kernel_size, kernel_size)
 
     if isinstance(dilation, numbers.Number):
         dilation = (dilation, dilation)
```

### Comparing `nobuco-0.4.6/nobuco/node_converters/recurrent.py` & `nobuco-0.4.7/nobuco/node_converters/recurrent.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/slice.py` & `nobuco-0.4.7/nobuco/node_converters/slice.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/tensor_cast.py` & `nobuco-0.4.7/nobuco/node_converters/tensor_cast.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/tensor_creation.py` & `nobuco-0.4.7/nobuco/node_converters/tensor_creation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/node_converters/tensor_manipulation.py` & `nobuco-0.4.7/nobuco/node_converters/tensor_manipulation.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/trace/tensor_storage.py` & `nobuco-0.4.7/nobuco/trace/tensor_storage.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/trace/trace.py` & `nobuco-0.4.7/nobuco/trace/trace.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/util.py` & `nobuco-0.4.7/nobuco/util.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/vis/console_stylizer.py` & `nobuco-0.4.7/nobuco/vis/console_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco/vis/html_stylizer.py` & `nobuco-0.4.7/nobuco/vis/html_stylizer.py`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/nobuco.egg-info/PKG-INFO` & `nobuco-0.4.7/nobuco.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nobuco
-Version: 0.4.6
+Version: 0.4.7
 Summary: Pytorch to Tensorflow conversion made somewhat easy
 Author-email: Alexander Lutsenko <lex.lutsenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Alexander Lutsenko
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nobuco-0.4.6/nobuco.egg-info/SOURCES.txt` & `nobuco-0.4.7/nobuco.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nobuco-0.4.6/pyproject.toml` & `nobuco-0.4.7/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nobuco"
-version = "0.4.6"
+version = "0.4.7"
 description = "Pytorch to Tensorflow conversion made somewhat easy"
 readme = "README.md"
 authors = [
   { name="Alexander Lutsenko", email="lex.lutsenko@gmail.com" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

