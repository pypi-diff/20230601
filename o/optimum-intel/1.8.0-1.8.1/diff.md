# Comparing `tmp/optimum-intel-1.8.0.tar.gz` & `tmp/optimum-intel-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimum-intel-1.8.0.tar", last modified: Mon Apr 17 13:06:57 2023, max compression
+gzip compressed data, was "dist/optimum-intel-1.8.1.tar", last modified: Thu Jun  1 17:30:38 2023, max compression
```

## Comparing `optimum-intel-1.8.0.tar` & `optimum-intel-1.8.1.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.671269 optimum-intel-1.8.0/
--rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/LICENSE
--rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/MANIFEST.in
--rw-r--r--   0 ella      (1000) ella      (1000)    11204 2023-04-17 13:06:57.671269 optimum-intel-1.8.0/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     9957 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/README.md
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.641269 optimum-intel-1.8.0/optimum/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.641269 optimum-intel-1.8.0/optimum/commands/
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.651269 optimum-intel-1.8.0/optimum/commands/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/commands/neural_compressor/base.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/commands/neural_compressor/quantize.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.651269 optimum-intel-1.8.0/optimum/commands/register/
--rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/commands/register/register_inc.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.651269 optimum-intel-1.8.0/optimum/intel/
--rw-r--r--   0 ella      (1000) ella      (1000)     6003 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/__init__.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.651269 optimum-intel-1.8.0/optimum/intel/ipex/
--rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/ipex/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     5717 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/ipex/inference.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.651269 optimum-intel-1.8.0/optimum/intel/neural_compressor/
--rw-r--r--   0 ella      (1000) ella      (1000)     1063 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3744 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/launcher.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/neural_coder_adaptor.py
--rw-r--r--   0 ella      (1000) ella      (1000)    27524 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    39116 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)    10813 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/trainer_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3905 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/neural_compressor/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.661269 optimum-intel-1.8.0/optimum/intel/openvino/
--rw-r--r--   0 ella      (1000) ella      (1000)     1514 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3014 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/configuration.py
--rw-r--r--   0 ella      (1000) ella      (1000)    22259 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling.py
--rw-r--r--   0 ella      (1000) ella      (1000)    15305 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling_base.py
--rw-r--r--   0 ella      (1000) ella      (1000)    18165 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling_base_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    19198 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling_decoder.py
--rw-r--r--   0 ella      (1000) ella      (1000)    20602 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling_diffusion.py
--rw-r--r--   0 ella      (1000) ella      (1000)    19620 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/modeling_seq2seq.py
--rw-r--r--   0 ella      (1000) ella      (1000)    13635 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/quantization.py
--rw-r--r--   0 ella      (1000) ella      (1000)    38278 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/trainer.py
--rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/training_args.py
--rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/openvino/utils.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.661269 optimum-intel-1.8.0/optimum/intel/utils/
--rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/__init__.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1278 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/constant.py
--rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/dummy_ipex_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/dummy_neural_compressor_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_objects.py
--rw-r--r--   0 ella      (1000) ella      (1000)     8783 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/optimum/intel/utils/import_utils.py
--rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-04-17 13:04:42.000000 optimum-intel-1.8.0/optimum/intel/version.py
-drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-04-17 13:06:57.671269 optimum-intel-1.8.0/optimum_intel.egg-info/
--rw-r--r--   0 ella      (1000) ella      (1000)    11204 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/PKG-INFO
--rw-r--r--   0 ella      (1000) ella      (1000)     1777 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/SOURCES.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/dependency_links.txt
--rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/entry_points.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/not-zip-safe
--rw-r--r--   0 ella      (1000) ella      (1000)      459 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/requires.txt
--rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-04-17 13:06:57.000000 optimum-intel-1.8.0/optimum_intel.egg-info/top_level.txt
--rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/pyproject.toml
--rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-04-17 13:06:57.671269 optimum-intel-1.8.0/setup.cfg
--rw-r--r--   0 ella      (1000) ella      (1000)     2679 2023-04-17 13:03:50.000000 optimum-intel-1.8.0/setup.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11357 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/LICENSE
+-rw-r--r--   0 ella      (1000) ella      (1000)      651 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/MANIFEST.in
+-rw-r--r--   0 ella      (1000) ella      (1000)    11204 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     9957 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/README.md
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.465065 optimum-intel-1.8.1/optimum/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.465065 optimum-intel-1.8.1/optimum/commands/
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.475065 optimum-intel-1.8.1/optimum/commands/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1023 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/commands/neural_compressor/base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3423 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/commands/neural_compressor/quantize.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.475065 optimum-intel-1.8.1/optimum/commands/register/
+-rw-r--r--   0 ella      (1000) ella      (1000)      690 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/commands/register/register_inc.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.475065 optimum-intel-1.8.1/optimum/intel/
+-rw-r--r--   0 ella      (1000) ella      (1000)     6003 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/__init__.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.475065 optimum-intel-1.8.1/optimum/intel/ipex/
+-rw-r--r--   0 ella      (1000) ella      (1000)       38 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/ipex/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     5717 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/ipex/inference.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.475065 optimum-intel-1.8.1/optimum/intel/neural_compressor/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1063 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3744 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      465 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/launcher.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1127 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/neural_coder_adaptor.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    27524 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    39213 2023-05-31 17:14:49.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    10813 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/trainer_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3905 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/neural_compressor/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/optimum/intel/openvino/
+-rw-r--r--   0 ella      (1000) ella      (1000)     1514 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/openvino/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3014 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/openvino/configuration.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    22259 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    15444 2023-05-31 17:19:54.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling_base.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    18165 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling_base_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    19198 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling_decoder.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    20602 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling_diffusion.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    19620 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/openvino/modeling_seq2seq.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    13635 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/openvino/quantization.py
+-rw-r--r--   0 ella      (1000) ella      (1000)    38687 2023-05-31 17:19:54.000000 optimum-intel-1.8.1/optimum/intel/openvino/trainer.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      816 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/openvino/training_args.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     2492 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/openvino/utils.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/optimum/intel/utils/
+-rw-r--r--   0 ella      (1000) ella      (1000)      974 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/__init__.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1278 2023-05-31 17:06:42.000000 optimum-intel-1.8.1/optimum/intel/utils/constant.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      842 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/dummy_ipex_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     4804 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/dummy_neural_compressor_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1014 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     1906 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_and_nncf_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     3346 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_objects.py
+-rw-r--r--   0 ella      (1000) ella      (1000)     8783 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/optimum/intel/utils/import_utils.py
+-rw-r--r--   0 ella      (1000) ella      (1000)      654 2023-06-01 17:28:46.000000 optimum-intel-1.8.1/optimum/intel/version.py
+drwxr-xr-x   0 ella      (1000) ella      (1000)        0 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/optimum_intel.egg-info/
+-rw-r--r--   0 ella      (1000) ella      (1000)    11204 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/PKG-INFO
+-rw-r--r--   0 ella      (1000) ella      (1000)     1777 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/SOURCES.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/dependency_links.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)       66 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/entry_points.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        1 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/not-zip-safe
+-rw-r--r--   0 ella      (1000) ella      (1000)      464 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/requires.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)        8 2023-06-01 17:30:38.000000 optimum-intel-1.8.1/optimum_intel.egg-info/top_level.txt
+-rw-r--r--   0 ella      (1000) ella      (1000)     1040 2023-05-31 16:48:28.000000 optimum-intel-1.8.1/pyproject.toml
+-rw-r--r--   0 ella      (1000) ella      (1000)      820 2023-06-01 17:30:38.485064 optimum-intel-1.8.1/setup.cfg
+-rw-r--r--   0 ella      (1000) ella      (1000)     2687 2023-05-31 17:19:02.000000 optimum-intel-1.8.1/setup.py
```

### Comparing `optimum-intel-1.8.0/LICENSE` & `optimum-intel-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/MANIFEST.in` & `optimum-intel-1.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/PKG-INFO` & `optimum-intel-1.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.8.0
+Version: 1.8.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-intel-1.8.0/README.md` & `optimum-intel-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/commands/neural_compressor/base.py` & `optimum-intel-1.8.1/optimum/commands/neural_compressor/base.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/commands/neural_compressor/quantize.py` & `optimum-intel-1.8.1/optimum/commands/neural_compressor/quantize.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/commands/register/register_inc.py` & `optimum-intel-1.8.1/optimum/commands/register/register_inc.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/__init__.py` & `optimum-intel-1.8.1/optimum/intel/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/ipex/inference.py` & `optimum-intel-1.8.1/optimum/intel/ipex/inference.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/neural_compressor/__init__.py` & `optimum-intel-1.8.1/optimum/intel/neural_compressor/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/neural_compressor/configuration.py` & `optimum-intel-1.8.1/optimum/intel/neural_compressor/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/neural_compressor/neural_coder_adaptor.py` & `optimum-intel-1.8.1/optimum/intel/neural_compressor/neural_coder_adaptor.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/neural_compressor/quantization.py` & `optimum-intel-1.8.1/optimum/intel/neural_compressor/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/neural_compressor/trainer.py` & `optimum-intel-1.8.1/optimum/intel/neural_compressor/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,16 @@
         self.task = task
         self.quantization_config = quantization_config
         self.pruning_config = pruning_config
         self.distillation_config = distillation_config
         self._compression_manager = None
         self.distillation_callback = None
         self.save_onnx_model = save_onnx_model
+        # TODO : To deprecate once support transformers > 4.30.0
+        self.deepspeed = None
 
         # Attach dtype and architecture to the config
         self.dtype = "int8" if quantization_config is not None else str(get_parameter_dtype(self.model)).split(".")[1]
         self.model.config.torch_dtype = self.dtype
         self.model.config.framework = "pytorch_fx"
         self.model.config.backend = "default"
         self.model.config.architectures = [self.model.__class__.__name__]
```

### Comparing `optimum-intel-1.8.0/optimum/intel/neural_compressor/trainer_seq2seq.py` & `optimum-intel-1.8.1/optimum/intel/neural_compressor/trainer_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/neural_compressor/utils.py` & `optimum-intel-1.8.1/optimum/intel/neural_compressor/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/__init__.py` & `optimum-intel-1.8.1/optimum/intel/openvino/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/configuration.py` & `optimum-intel-1.8.1/optimum/intel/openvino/configuration.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/modeling.py` & `optimum-intel-1.8.1/optimum/intel/openvino/modeling.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/modeling_base.py` & `optimum-intel-1.8.1/optimum/intel/openvino/modeling_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,20 +51,25 @@
     "AUTO:GPU,CPU",
     "MULTI",
     "MULTI:CPU,GPU",
     "MULTI:GPU,CPU",
 }
 
 
+# workaround to enable compatibility between openvino models and transformers pipelines
+class PreTrainedModel(OptimizedModel):
+    pass
+
+
 @add_start_docstrings(
     """
     Base OVModel class.
     """,
 )
-class OVBaseModel(OptimizedModel):
+class OVBaseModel(PreTrainedModel):
     _AUTOMODELS_TO_TASKS = {cls_name: task for task, cls_name in TasksManager._TASKS_TO_AUTOMODELS.items()}
     auto_model_class = None
     export_feature = None
 
     def __init__(
         self,
         model: openvino.runtime.Model,
```

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/modeling_base_seq2seq.py` & `optimum-intel-1.8.1/optimum/intel/openvino/modeling_base_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/modeling_decoder.py` & `optimum-intel-1.8.1/optimum/intel/openvino/modeling_decoder.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/modeling_diffusion.py` & `optimum-intel-1.8.1/optimum/intel/openvino/modeling_diffusion.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/modeling_seq2seq.py` & `optimum-intel-1.8.1/optimum/intel/openvino/modeling_seq2seq.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/quantization.py` & `optimum-intel-1.8.1/optimum/intel/openvino/quantization.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/trainer.py` & `optimum-intel-1.8.1/optimum/intel/openvino/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     logging,
 )
 
 from optimum.exporters import TasksManager
 from optimum.exporters.onnx import OnnxConfig
 
 from ..utils.constant import _TASK_ALIASES
+from ..utils.import_utils import is_transformers_version
 from .configuration import OVConfig
 from .quantization import OVDataLoader
 from .training_args import OVTrainingArguments
 from .utils import (
     MAX_ONNX_OPSET,
     MIN_ONNX_QDQ_OPSET,
     ONNX_WEIGHTS_NAME,
@@ -189,14 +190,16 @@
             nncf_logger.addHandler(nncf_log_file_handler)
             set_log_level(logging.ERROR)
             nncf_logger.setLevel(logging.INFO)
             nncf_log_file_handler.setLevel(logging.INFO)
 
             self.compression_controller, self.model = create_compressed_model(self.model, nncf_config)
             self.model_wrapped = self.model
+            # TODO : To deprecate once support transformers > 4.30.0
+            self.deepspeed = None
 
     def _set_signature_columns_if_needed(self):
         if self._signature_columns is None:
             # Inspect model forward signature to keep only the arguments it accepts.
             if isinstance(self.model, NNCFNetwork):
                 signature = inspect.signature(self.model.get_nncf_wrapped_model().forward)
             else:
@@ -281,17 +284,24 @@
         self.state = TrainerState()
         self.state.is_hyper_param_search = trial is not None
 
         # Activate gradient checkpointing if needed
         if args.gradient_checkpointing:
             self.model.gradient_checkpointing_enable()
 
-        if self.args.local_rank != -1:
-            if self.compression_controller is not None:
-                self.compression_controller.distributed()
+        if is_transformers_version("<", "4.29.0"):
+            is_distributed = self.args.local_rank != -1
+        else:
+            from accelerate.utils import DistributedType
+
+            is_distributed = self.args.distributed_state.distributed_type != DistributedType.NO
+
+        if self.compression_controller is not None and is_distributed:
+            self.compression_controller.distributed()
+
         model = self._wrap_model(self.model_wrapped)
 
         if is_sagemaker_mp_enabled() and resume_from_checkpoint is not None:
             self._load_from_checkpoint(resume_from_checkpoint, model)
 
         # for the rest of this function `model` is the outside model, whether it was wrapped or not
         if model is not self.model:
```

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/training_args.py` & `optimum-intel-1.8.1/optimum/intel/openvino/training_args.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/openvino/utils.py` & `optimum-intel-1.8.1/optimum/intel/openvino/utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/utils/__init__.py` & `optimum-intel-1.8.1/optimum/intel/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/utils/constant.py` & `optimum-intel-1.8.1/optimum/intel/utils/constant.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/utils/dummy_ipex_objects.py` & `optimum-intel-1.8.1/optimum/intel/utils/dummy_ipex_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/utils/dummy_neural_compressor_objects.py` & `optimum-intel-1.8.1/optimum/intel/utils/dummy_neural_compressor_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py` & `optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_and_diffusers_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_and_nncf_objects.py` & `optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_and_nncf_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/utils/dummy_openvino_objects.py` & `optimum-intel-1.8.1/optimum/intel/utils/dummy_openvino_objects.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/utils/import_utils.py` & `optimum-intel-1.8.1/optimum/intel/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/optimum/intel/version.py` & `optimum-intel-1.8.1/optimum/intel/version.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-__version__ = "1.8.0"
+__version__ = "1.8.1"
```

### Comparing `optimum-intel-1.8.0/optimum_intel.egg-info/PKG-INFO` & `optimum-intel-1.8.1/optimum_intel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimum-intel
-Version: 1.8.0
+Version: 1.8.1
 Summary: Optimum Library is an extension of the Hugging Face Transformers library, providing a framework to integrate third-party libraries from Hardware Partners and interface with their specific functionality.
 Home-page: https://www.intel.com
 Author: HuggingFace Inc. Special Ops Team
 Author-email: hardware@huggingface.co
 License: Apache
 Keywords: transformers,quantization,pruning,knowledge distillation,optimization,training
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `optimum-intel-1.8.0/optimum_intel.egg-info/SOURCES.txt` & `optimum-intel-1.8.1/optimum_intel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/pyproject.toml` & `optimum-intel-1.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/setup.cfg` & `optimum-intel-1.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `optimum-intel-1.8.0/setup.py` & `optimum-intel-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
         "onnx",
         "onnxruntime",
         "torch<2.0.0",  # remove after neural-compressor next release
         "intel-extension-for-pytorch<2.0.0",
     ],
     "openvino": ["openvino>=2023.0.0.dev20230217", "onnx", "onnxruntime"],
     "nncf": ["nncf>=2.4.0", "openvino-dev>=2023.0.0.dev20230217"],
-    "ipex": ["intel-extension-for-pytorch"],
+    "ipex": ["intel-extension-for-pytorch", "onnx"],
     "diffusers": ["diffusers"],
     "quality": QUALITY_REQUIRE,
     "tests": TESTS_REQUIRE,
 }
 
 setup(
     name="optimum-intel",
```

