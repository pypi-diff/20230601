# Comparing `tmp/auto_gptq-0.1.0.tar.gz` & `tmp/auto_gptq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto_gptq-0.1.0.tar", last modified: Thu May  4 16:21:38 2023, max compression
+gzip compressed data, was "auto_gptq-0.2.0.tar", last modified: Thu Jun  1 16:04:13 2023, max compression
```

## Comparing `auto_gptq-0.1.0.tar` & `auto_gptq-0.2.0.tar`

### file list

```diff
@@ -1,56 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/
--rw-rw-rw-   0        0        0     1096 2023-04-13 14:32:51.000000 auto_gptq-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      126 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     9775 2023-05-04 16:15:32.000000 auto_gptq-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.489776 auto_gptq-0.1.0/auto_gptq/
--rw-rw-rw-   0        0        0       85 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.514701 auto_gptq-0.1.0/auto_gptq/eval_tasks/
--rw-rw-rw-   0        0        0      124 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/__init__.py
--rw-rw-rw-   0        0        0     2259 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/_base.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.519734 auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/
--rw-rw-rw-   0        0        0        0 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/__init__.py
--rw-rw-rw-   0        0        0     1165 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/classification_utils.py
--rw-rw-rw-   0        0        0     1486 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/generation_utils.py
--rw-rw-rw-   0        0        0     1262 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/language_modeling_task.py
--rw-rw-rw-   0        0        0     3760 2023-04-23 15:46:04.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/sequence_classification_task.py
--rw-rw-rw-   0        0        0     2646 2023-04-24 12:51:09.000000 auto_gptq-0.1.0/auto_gptq/eval_tasks/text_summarization_task.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.534543 auto_gptq-0.1.0/auto_gptq/modeling/
--rw-rw-rw-   0        0        0      233 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/__init__.py
--rw-rw-rw-   0        0        0    23514 2023-05-04 13:51:26.000000 auto_gptq-0.1.0/auto_gptq/modeling/_base.py
--rw-rw-rw-   0        0        0      427 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/_const.py
--rw-rw-rw-   0        0        0     4720 2023-05-04 14:09:44.000000 auto_gptq-0.1.0/auto_gptq/modeling/_utils.py
--rw-rw-rw-   0        0        0     2677 2023-04-29 12:44:45.000000 auto_gptq-0.1.0/auto_gptq/modeling/auto.py
--rw-rw-rw-   0        0        0      490 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/bloom.py
--rw-rw-rw-   0        0        0      409 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/gpt2.py
--rw-rw-rw-   0        0        0      478 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/gpt_neox.py
--rw-rw-rw-   0        0        0      423 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/modeling/gptj.py
--rw-rw-rw-   0        0        0      469 2023-04-28 15:06:27.000000 auto_gptq-0.1.0/auto_gptq/modeling/llama.py
--rw-rw-rw-   0        0        0      395 2023-04-29 02:36:14.000000 auto_gptq-0.1.0/auto_gptq/modeling/moss.py
--rw-rw-rw-   0        0        0      581 2023-04-28 15:06:27.000000 auto_gptq-0.1.0/auto_gptq/modeling/opt.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.553323 auto_gptq-0.1.0/auto_gptq/nn_modules/
--rw-rw-rw-   0        0        0        0 2023-04-26 13:22:55.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/__init__.py
--rw-rw-rw-   0        0        0     9254 2023-04-30 12:35:15.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/layernorm_triton.py
--rw-rw-rw-   0        0        0    10285 2023-05-04 14:09:44.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/qlinear.py
--rw-rw-rw-   0        0        0    11608 2023-05-04 14:16:08.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/qlinear_old.py
--rw-rw-rw-   0        0        0    19259 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/qlinear_triton.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.559832 auto_gptq-0.1.0/auto_gptq/nn_modules/triton_utils/
--rw-rw-rw-   0        0        0        0 2023-04-26 13:22:55.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/triton_utils/__init__.py
--rw-rw-rw-   0        0        0     7099 2023-04-26 13:22:55.000000 auto_gptq-0.1.0/auto_gptq/nn_modules/triton_utils/custom_autotune.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/auto_gptq/quantization/
--rw-rw-rw-   0        0        0       47 2023-04-26 13:22:55.000000 auto_gptq-0.1.0/auto_gptq/quantization/__init__.py
--rw-rw-rw-   0        0        0     6007 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/quantization/gptq.py
--rw-rw-rw-   0        0        0     4408 2023-04-26 13:22:55.000000 auto_gptq-0.1.0/auto_gptq/quantization/quantizer.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/auto_gptq/utils/
--rw-rw-rw-   0        0        0        0 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/utils/__init__.py
--rw-rw-rw-   0        0        0    11389 2023-04-28 14:56:43.000000 auto_gptq-0.1.0/auto_gptq/utils/data_utils.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.499744 auto_gptq-0.1.0/auto_gptq.egg-info/
--rw-rw-rw-   0        0        0      126 2023-05-04 16:21:38.000000 auto_gptq-0.1.0/auto_gptq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1399 2023-05-04 16:21:38.000000 auto_gptq-0.1.0/auto_gptq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 16:21:38.000000 auto_gptq-0.1.0/auto_gptq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      141 2023-05-04 16:21:38.000000 auto_gptq-0.1.0/auto_gptq.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-04 16:21:38.000000 auto_gptq-0.1.0/auto_gptq.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/quant_cuda/
--rw-rw-rw-   0        0        0     6642 2023-05-04 13:51:26.000000 auto_gptq-0.1.0/quant_cuda/quant_cuda.cpp
--rw-rw-rw-   0        0        0    40650 2023-05-04 14:33:51.000000 auto_gptq-0.1.0/quant_cuda/quant_cuda_kernel.cu
--rw-rw-rw-   0        0        0       42 2023-05-04 16:21:38.589723 auto_gptq-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1599 2023-05-04 16:18:50.000000 auto_gptq-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.581488 auto_gptq-0.2.0/
+-rw-rw-rw-   0        0        0     1096 2023-04-13 14:32:51.000000 auto_gptq-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0      880 2023-06-01 16:04:13.581488 auto_gptq-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14761 2023-06-01 15:16:42.000000 auto_gptq-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.565865 auto_gptq-0.2.0/auto_gptq/
+-rw-rw-rw-   0        0        0       85 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.565865 auto_gptq-0.2.0/auto_gptq/eval_tasks/
+-rw-rw-rw-   0        0        0      124 2023-04-28 14:56:43.000000 auto_gptq-0.2.0/auto_gptq/eval_tasks/__init__.py
+-rw-rw-rw-   0        0        0     2259 2023-04-28 14:56:43.000000 auto_gptq-0.2.0/auto_gptq/eval_tasks/_base.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.565865 auto_gptq-0.2.0/auto_gptq/eval_tasks/_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-23 15:46:04.000000 auto_gptq-0.2.0/auto_gptq/eval_tasks/_utils/__init__.py
+-rw-rw-rw-   0        0        0     1165 2023-04-23 15:46:04.000000 auto_gptq-0.2.0/auto_gptq/eval_tasks/_utils/classification_utils.py
+-rw-rw-rw-   0        0        0     1486 2023-04-23 15:46:04.000000 auto_gptq-0.2.0/auto_gptq/eval_tasks/_utils/generation_utils.py
+-rw-rw-rw-   0        0        0     1262 2023-04-23 15:46:04.000000 auto_gptq-0.2.0/auto_gptq/eval_tasks/language_modeling_task.py
+-rw-rw-rw-   0        0        0     3760 2023-04-23 15:46:04.000000 auto_gptq-0.2.0/auto_gptq/eval_tasks/sequence_classification_task.py
+-rw-rw-rw-   0        0        0     2646 2023-04-24 12:51:09.000000 auto_gptq-0.2.0/auto_gptq/eval_tasks/text_summarization_task.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.581488 auto_gptq-0.2.0/auto_gptq/modeling/
+-rw-rw-rw-   0        0        0      304 2023-05-28 08:23:38.000000 auto_gptq-0.2.0/auto_gptq/modeling/__init__.py
+-rw-rw-rw-   0        0        0    36750 2023-05-31 14:11:16.000000 auto_gptq-0.2.0/auto_gptq/modeling/_base.py
+-rw-rw-rw-   0        0        0      474 2023-05-28 08:23:38.000000 auto_gptq-0.2.0/auto_gptq/modeling/_const.py
+-rw-rw-rw-   0        0        0     7090 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/modeling/_utils.py
+-rw-rw-rw-   0        0        0     3970 2023-05-29 23:38:06.000000 auto_gptq-0.2.0/auto_gptq/modeling/auto.py
+-rw-rw-rw-   0        0        0      490 2023-04-28 14:56:43.000000 auto_gptq-0.2.0/auto_gptq/modeling/bloom.py
+-rw-rw-rw-   0        0        0      404 2023-05-28 08:23:38.000000 auto_gptq-0.2.0/auto_gptq/modeling/codegen.py
+-rw-rw-rw-   0        0        0      409 2023-04-28 14:56:43.000000 auto_gptq-0.2.0/auto_gptq/modeling/gpt2.py
+-rw-rw-rw-   0        0        0      469 2023-05-28 08:23:38.000000 auto_gptq-0.2.0/auto_gptq/modeling/gpt_bigcode.py
+-rw-rw-rw-   0        0        0      478 2023-04-28 14:56:43.000000 auto_gptq-0.2.0/auto_gptq/modeling/gpt_neox.py
+-rw-rw-rw-   0        0        0      569 2023-05-14 08:23:32.000000 auto_gptq-0.2.0/auto_gptq/modeling/gptj.py
+-rw-rw-rw-   0        0        0     1042 2023-05-20 07:21:20.000000 auto_gptq-0.2.0/auto_gptq/modeling/llama.py
+-rw-rw-rw-   0        0        0      395 2023-04-29 02:36:14.000000 auto_gptq-0.2.0/auto_gptq/modeling/moss.py
+-rw-rw-rw-   0        0        0      581 2023-04-28 15:06:27.000000 auto_gptq-0.2.0/auto_gptq/modeling/opt.py
+-rw-rw-rw-   0        0        0      443 2023-05-28 08:23:38.000000 auto_gptq-0.2.0/auto_gptq/modeling/rw.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.581488 auto_gptq-0.2.0/auto_gptq/nn_modules/
+-rw-rw-rw-   0        0        0        0 2023-04-26 13:22:55.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/__init__.py
+-rw-rw-rw-   0        0        0      885 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/_fused_base.py
+-rw-rw-rw-   0        0        0    11220 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/fused_gptj_attn.py
+-rw-rw-rw-   0        0        0     7564 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/fused_llama_attn.py
+-rw-rw-rw-   0        0        0    13669 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/fused_llama_mlp.py
+-rw-rw-rw-   0        0        0    10956 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/qlinear.py
+-rw-rw-rw-   0        0        0    11178 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/qlinear_old.py
+-rw-rw-rw-   0        0        0     6097 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/qlinear_triton.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.581488 auto_gptq-0.2.0/auto_gptq/nn_modules/triton_utils/
+-rw-rw-rw-   0        0        0        0 2023-05-20 09:01:53.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/triton_utils/__init__.py
+-rw-rw-rw-   0        0        0     7099 2023-04-26 13:22:55.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/triton_utils/custom_autotune.py
+-rw-rw-rw-   0        0        0    14201 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/triton_utils/kernels.py
+-rw-rw-rw-   0        0        0      117 2023-05-20 09:01:53.000000 auto_gptq-0.2.0/auto_gptq/nn_modules/triton_utils/mixin.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.581488 auto_gptq-0.2.0/auto_gptq/quantization/
+-rw-rw-rw-   0        0        0       47 2023-04-26 13:22:55.000000 auto_gptq-0.2.0/auto_gptq/quantization/__init__.py
+-rw-rw-rw-   0        0        0     6016 2023-05-14 05:13:14.000000 auto_gptq-0.2.0/auto_gptq/quantization/gptq.py
+-rw-rw-rw-   0        0        0     4408 2023-04-26 13:22:55.000000 auto_gptq-0.2.0/auto_gptq/quantization/quantizer.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.581488 auto_gptq-0.2.0/auto_gptq/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-28 14:56:43.000000 auto_gptq-0.2.0/auto_gptq/utils/__init__.py
+-rw-rw-rw-   0        0        0    11389 2023-04-28 14:56:43.000000 auto_gptq-0.2.0/auto_gptq/utils/data_utils.py
+-rw-rw-rw-   0        0        0     1089 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/auto_gptq/utils/import_utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.565865 auto_gptq-0.2.0/auto_gptq.egg-info/
+-rw-rw-rw-   0        0        0      880 2023-06-01 16:04:13.000000 auto_gptq-0.2.0/auto_gptq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1736 2023-06-01 16:04:13.000000 auto_gptq-0.2.0/auto_gptq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 16:04:13.000000 auto_gptq-0.2.0/auto_gptq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-06-01 16:04:13.000000 auto_gptq-0.2.0/auto_gptq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-06-01 16:04:13.000000 auto_gptq-0.2.0/auto_gptq.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 16:04:13.581488 auto_gptq-0.2.0/autogptq_cuda/
+-rw-rw-rw-   0        0        0     6642 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/autogptq_cuda/autogptq_cuda.cpp
+-rw-rw-rw-   0        0        0    40741 2023-05-29 23:02:56.000000 auto_gptq-0.2.0/autogptq_cuda/autogptq_cuda_kernel.cu
+-rw-rw-rw-   0        0        0       42 2023-06-01 16:04:13.581488 auto_gptq-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     3329 2023-06-01 16:03:43.000000 auto_gptq-0.2.0/setup.py
```

### Comparing `auto_gptq-0.1.0/LICENSE` & `auto_gptq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq/eval_tasks/_base.py` & `auto_gptq-0.2.0/auto_gptq/eval_tasks/_base.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/classification_utils.py` & `auto_gptq-0.2.0/auto_gptq/eval_tasks/_utils/classification_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq/eval_tasks/_utils/generation_utils.py` & `auto_gptq-0.2.0/auto_gptq/eval_tasks/_utils/generation_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq/eval_tasks/language_modeling_task.py` & `auto_gptq-0.2.0/auto_gptq/eval_tasks/language_modeling_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq/eval_tasks/sequence_classification_task.py` & `auto_gptq-0.2.0/auto_gptq/eval_tasks/sequence_classification_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq/eval_tasks/text_summarization_task.py` & `auto_gptq-0.2.0/auto_gptq/eval_tasks/text_summarization_task.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq/modeling/auto.py` & `auto_gptq-0.2.0/auto_gptq/modeling/auto.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-from typing import Optional
+from inspect import signature
+from typing import Dict, Optional, Union
 
 from ._base import BaseQuantizeConfig, BaseGPTQForCausalLM
 from ._utils import check_and_get_model_type
 from .bloom import BloomGPTQForCausalLM
+from .codegen import CodeGenGPTQForCausalLM
 from .gpt_neox import GPTNeoXGPTQForCausalLM
 from .gptj import GPTJGPTQForCausalLM
 from .gpt2 import GPT2GPTQForCausalLM
 from .llama import LlamaGPTQForCausalLM
 from .moss import MOSSGPTQForCausalLM
 from .opt import OPTGPTQForCausalLM
+from .rw import RWGPTQForCausalLM
+from .gpt_bigcode import GPTBigCodeGPTQForCausalLM
 
 
 GPTQ_CAUSAL_LM_MODEL_MAP = {
     "bloom": BloomGPTQForCausalLM,
     "gpt_neox": GPTNeoXGPTQForCausalLM,
     "gptj": GPTJGPTQForCausalLM,
     "gpt2": GPT2GPTQForCausalLM,
     "llama": LlamaGPTQForCausalLM,
     "opt": OPTGPTQForCausalLM,
-    "moss": MOSSGPTQForCausalLM
+    "moss": MOSSGPTQForCausalLM,
+    "gpt_bigcode": GPTBigCodeGPTQForCausalLM,
+    "codegen": CodeGenGPTQForCausalLM,
+    "RefinedWebModel": RWGPTQForCausalLM,
+    "RefinedWeb":RWGPTQForCausalLM
 }
 
 
 class AutoGPTQForCausalLM:
     def __init__(self):
         raise EnvironmentError(
             "AutoGPTQModelForCausalLM is designed to be instantiated\n"
@@ -32,45 +40,63 @@
 
     @classmethod
     def from_pretrained(
         cls,
         pretrained_model_name_or_path: str,
         quantize_config: BaseQuantizeConfig,
         max_memory: Optional[dict] = None,
+        trust_remote_code: bool = False,
         **model_init_kwargs
     ) -> BaseGPTQForCausalLM:
-        model_type = check_and_get_model_type(pretrained_model_name_or_path)
+        model_type = check_and_get_model_type(pretrained_model_name_or_path, trust_remote_code)
         return GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_pretrained(
             pretrained_model_name_or_path=pretrained_model_name_or_path,
             quantize_config=quantize_config,
             max_memory=max_memory,
+            trust_remote_code=trust_remote_code,
             **model_init_kwargs
         )
 
     @classmethod
     def from_quantized(
         cls,
-        save_dir: str,
-        device: str = "cpu",
-        use_safetensors: bool = False,
-        use_triton: bool = False,
+        model_name_or_path: Optional[str] = None,
+        save_dir: Optional[str] = None,
+        device_map: Optional[Union[str, Dict[str, Union[str, int]]]] = None,
         max_memory: Optional[dict] = None,
-        device_map: Optional[str] = None,
+        device: Optional[Union[str, int]] = None,
+        low_cpu_mem_usage: bool = False,
+        use_triton: bool = False,
+        inject_fused_attention: bool = True,
+        inject_fused_mlp: bool = True,
+        use_cuda_fp16: bool = True,
         quantize_config: Optional[BaseQuantizeConfig] = None,
         model_basename: Optional[str] = None,
-        trust_remote_code: bool = False
+        use_safetensors: bool = False,
+        trust_remote_code: bool = False,
+        warmup_triton: bool = False,
+        **kwargs
     ) -> BaseGPTQForCausalLM:
-        model_type = check_and_get_model_type(save_dir)
-        return GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_quantized(
+        model_type = check_and_get_model_type(save_dir or model_name_or_path, trust_remote_code)
+        quant_func = GPTQ_CAUSAL_LM_MODEL_MAP[model_type].from_quantized
+        keywords = {key: kwargs[key] for key in signature(quant_func).parameters if key in kwargs}
+        return quant_func(
+            model_name_or_path=model_name_or_path,
             save_dir=save_dir,
+            device_map=device_map,
+            max_memory=max_memory,
             device=device,
-            use_safetensors=use_safetensors,
+            low_cpu_mem_usage=low_cpu_mem_usage,
             use_triton=use_triton,
-            max_memory=max_memory,
-            device_map=device_map,
+            inject_fused_attention=inject_fused_attention,
+            inject_fused_mlp=inject_fused_mlp,
+            use_cuda_fp16=use_cuda_fp16,
             quantize_config=quantize_config,
             model_basename=model_basename,
-            trust_remote_code=trust_remote_code
+            use_safetensors=use_safetensors,
+            trust_remote_code=trust_remote_code,
+            warmup_triton=warmup_triton,
+            **keywords
         )
 
 
 __all__ = ["AutoGPTQForCausalLM"]
```

### Comparing `auto_gptq-0.1.0/auto_gptq/modeling/opt.py` & `auto_gptq-0.2.0/auto_gptq/modeling/opt.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq/nn_modules/qlinear.py` & `auto_gptq-0.2.0/auto_gptq/nn_modules/qlinear.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,57 +5,57 @@
 import torch
 import torch.nn as nn
 import transformers
 
 logger = getLogger(__name__)
 
 try:
-    import quant_cuda
+    import autogptq_cuda
 
-    _quant_cuda_available = True
+    _autogptq_cuda_available = True
 except ImportError:
     logger.warning('CUDA extension not installed.')
-    _quant_cuda_available = False
+    _autogptq_cuda_available = False
 
 
 class QuantLinear(nn.Module):
     def __init__(
         self,
         bits,
-        groupsize,
+        group_size,
         infeatures,
         outfeatures,
         bias,
         kernel_switch_threshold=128,
     ):
         super().__init__()
         if bits not in [2, 3, 4, 8]:
             raise NotImplementedError("Only 2,3,4,8 bits are supported.")
 
         self.infeatures = infeatures
         self.outfeatures = outfeatures
         self.bits = bits
-        self.groupsize = groupsize if groupsize != -1 else infeatures
+        self.group_size = group_size if group_size != -1 else infeatures
         self.maxq = 2 ** self.bits - 1
 
         self.register_buffer(
             'qweight',
             torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
         )
         self.register_buffer(
             'qzeros',
-            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures // 32 * self.bits), dtype=torch.int32)
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
         )
         self.register_buffer(
             'scales',
-            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures), dtype=torch.float16)
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
         )
         self.register_buffer(
             'g_idx',
-            torch.tensor([i // self.groupsize for i in range(infeatures)], dtype=torch.int32)
+            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
         )
         if bias:
             self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
         else:
             self.bias = None
 
         # is performed by unpacking the weights and using torch.matmul
@@ -68,17 +68,17 @@
                     [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
                     [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
                 ],
                 dtype=torch.int32
             ).reshape(1, 3, 12)
 
         self.kernel_switch_threshold = kernel_switch_threshold
-        self.quant_cuda_available = _quant_cuda_available
+        self.autogptq_cuda_available = _autogptq_cuda_available
         if infeatures % 256 != 0 or outfeatures % 256 != 0:
-            self.quant_cuda_available = False
+            self.autogptq_cuda_available = False
 
     def pack(self, linear, scales, zeros, g_idx=None):
         W = linear.weight.data.clone()
         if isinstance(linear, nn.Conv2d):
             W = W.flatten(1)
         if isinstance(linear, transformers.pytorch_utils.Conv1D):
             W = W.t()
@@ -175,29 +175,28 @@
 
         qzeros = qzeros.astype(np.int32)
         self.qzeros = torch.from_numpy(qzeros)
 
     def forward(self, x: torch.Tensor):
         out_shape = x.shape[:-1] + (self.outfeatures,)
         x = x.reshape(-1, x.shape[-1])
-        if self.quant_cuda_available and (
+        if self.autogptq_cuda_available and (
             self.kernel_switch_threshold == 0 or x.shape[0] < self.kernel_switch_threshold
         ):
             out = torch.zeros((x.shape[0], self.outfeatures), device=x.device, dtype=torch.float32)
             if self.bits == 2:
-                quant_cuda.vecquant2matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+                autogptq_cuda.vecquant2matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
             elif self.bits == 3:
-                quant_cuda.vecquant3matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+                autogptq_cuda.vecquant3matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
             elif self.bits == 4:
-                quant_cuda.vecquant4matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+                autogptq_cuda.vecquant4matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
             elif self.bits == 8:
-                quant_cuda.vecquant8matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
+                autogptq_cuda.vecquant8matmul(x.float(), self.qweight, out, self.scales.float(), self.qzeros, self.g_idx)
             else:
                 raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-            out = out.half()
         else:
             if self.wf.device != self.qzeros.device:
                 self.wf = self.wf.to(self.qzeros.device)
 
             if self.bits in [2, 4, 8]:
                 zeros = torch.bitwise_right_shift(
                     torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits),
@@ -234,16 +233,27 @@
                 weight[:, 1, 11] = (weight[:, 1, 11] & 0x1) | ((weight[:, 2, 0] << 1) & 0x6)
                 weight = weight & 0x7
                 weight = torch.cat([weight[:, 0, :11], weight[:, 1, 1:12], weight[:, 2, 1:11]], dim=1)
             else:
                 raise NotImplementedError("Only 2,3,4,8 bits are supported.")
 
             weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
-
-            weights = (self.scales[self.g_idx.long()] * (weight - zeros[self.g_idx.long()]))
+            num_itr = self.g_idx.shape[0]//x.shape[-1]
+            if num_itr == 1:
+                weights = (self.scales[self.g_idx.long()] * (weight - zeros[self.g_idx.long()]))
+            else:
+                num_dim = self.g_idx.shape[0]//num_itr
+                weights = []
+                for i in range(num_itr):
+                    scale_i = self.scales[:,i*num_dim:(i+1)*num_dim]
+                    weight_i = weight[:,i*num_dim:(i+1)*num_dim]
+                    zeros_i = zeros[:,i*num_dim:(i+1)*num_dim]
+                    g_idx_i = self.g_idx[i*num_dim:(i+1)*num_dim]
+                    weights.append(scale_i[g_idx_i.long()] * (weight_i - zeros_i[g_idx_i.long()]))
+                weights = torch.cat(weights,dim=1)
             out = torch.matmul(x.half(), weights)
-        out = out.reshape(out_shape)
+        out = out.half().reshape(out_shape)
         out = out + self.bias if self.bias is not None else out
         return out
 
 
 __all__ = ["QuantLinear"]
```

### Comparing `auto_gptq-0.1.0/auto_gptq/nn_modules/qlinear_old.py` & `auto_gptq-0.2.0/auto_gptq/nn_modules/qlinear_old.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,94 +5,96 @@
 import torch
 import torch.nn as nn
 import transformers
 
 logger = getLogger(__name__)
 
 try:
-    import quant_cuda
+    import autogptq_cuda
 
-    _quant_cuda_available = True
+    _autogptq_cuda_available = True
 except ImportError:
     logger.warning('CUDA extension not installed.')
-    _quant_cuda_available = False
-
+    _autogptq_cuda_available = False
 
 class QuantLinear(nn.Module):
     def __init__(
         self,
         bits,
-        groupsize,
+        group_size,
         infeatures,
         outfeatures,
         bias,
-        faster=True,
+        use_cuda_fp16=True,
         kernel_switch_threshold=128
     ):
+
         super().__init__()
         if bits not in [2, 3, 4, 8]:
             raise NotImplementedError("Only 2,3,4,8 bits are supported.")
         self.infeatures = infeatures
         self.outfeatures = outfeatures
         self.bits = bits
-        self.groupsize = groupsize if groupsize != -1 else infeatures
+        self.group_size = group_size if group_size != -1 else infeatures
         self.maxq = 2 ** self.bits - 1
 
         self.register_buffer(
             'qweight',
             torch.zeros((infeatures // 32 * self.bits, outfeatures), dtype=torch.int32)
         )
         self.register_buffer(
             'qzeros',
-            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures // 32 * self.bits), dtype=torch.int32)
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures // 32 * self.bits), dtype=torch.int32)
         )
         self.register_buffer(
             'scales',
-            torch.zeros((math.ceil(infeatures / self.groupsize), outfeatures), dtype=torch.float16)
+            torch.zeros((math.ceil(infeatures / self.group_size), outfeatures), dtype=torch.float16)
         )
         self.register_buffer(
             'g_idx',
-            torch.tensor([i // self.groupsize for i in range(infeatures)], dtype=torch.int32)
+            torch.tensor([i // self.group_size for i in range(infeatures)], dtype=torch.int32)
         )
+
         if bias:
             self.register_buffer('bias', torch.zeros((outfeatures), dtype=torch.float16))
         else:
             self.bias = None
         self.half_indim = self.infeatures // 2
-        self.faster = faster if bits != 8 else False
 
+        self.use_cuda_fp16 = use_cuda_fp16 if bits != 8 else False
+        
         # is performed by unpacking the weights and using torch.matmul
         if self.bits in [2, 4, 8]:
             self.wf = torch.tensor(list(range(0, 32, self.bits)), dtype=torch.int32).unsqueeze(0)
         elif self.bits == 3:
             self.wf = torch.tensor(
                 [
                     [0, 3, 6, 9, 12, 15, 18, 21, 24, 27, 30, 0],
                     [0, 1, 4, 7, 10, 13, 16, 19, 22, 25, 28, 31],
                     [0, 2, 5, 8, 11, 14, 17, 20, 23, 26, 29, 0],
                 ],
                 dtype=torch.int32
             ).reshape(1, 3, 12)
 
         self.kernel_switch_threshold = kernel_switch_threshold
-        self.quant_cuda_available = _quant_cuda_available
+        self.autogptq_cuda_available = _autogptq_cuda_available
         if infeatures % 256 != 0 or outfeatures % 256 != 0:
-            self.quant_cuda_available = False
+            self.autogptq_cuda_available = False
 
     def pack(self, linear, scales, zeros, g_idx):
         scales = scales.t().contiguous()
         zeros = zeros.t().contiguous()
         scale_zeros = zeros * scales
         self.scales = scales.clone().half()
         if linear.bias is not None:
             self.bias = linear.bias.clone().half()
 
         intweight = []
         for idx in range(self.infeatures):
-            g_idx = idx // self.groupsize
+            g_idx = idx // self.group_size
             intweight.append(
                 torch.round(
                     (linear.weight.data[:, idx] + scale_zeros[g_idx]) / self.scales[g_idx]
                 ).to(torch.int)[:, None]
             )
         intweight = torch.cat(intweight, dim=1)
         intweight = intweight.t().contiguous()
@@ -169,109 +171,84 @@
 
         qzeros = qzeros.astype(np.int32)
         self.qzeros = torch.from_numpy(qzeros)
 
     def forward(self, x):
         out_shape = x.shape[:-1] + (self.outfeatures,)
         x = x.reshape(-1, x.shape[-1])
-        if self.quant_cuda_available is True and (
+        if self.autogptq_cuda_available is True and (
             self.kernel_switch_threshold is False or x.shape[0] < self.kernel_switch_threshold
         ):
             out = torch.zeros(x.shape[0], out_shape[-1], dtype=torch.float, device=x.device)
-
-            if self.faster:
+            if self.use_cuda_fp16:
                 x = x.half()
                 if self.bits == 2:
-                    quant_cuda.vecquant2matmul_faster_old(
-                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize, self.half_indim
-                    )
+                    autogptq_cuda.vecquant2matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
                 elif self.bits == 3:
-                    quant_cuda.vecquant3matmul_faster_old(
-                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize, self.half_indim
-                    )
+                    autogptq_cuda.vecquant3matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
                 elif self.bits == 4:
-                    quant_cuda.vecquant4matmul_faster_old(
-                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize, self.half_indim
-                    )
+                    autogptq_cuda.vecquant4matmul_faster_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size, self.half_indim)
+
                 else:
                     raise NotImplementedError("Only 2,3,4 bits are supported.")
             else:
                 x = x.float()
                 if self.bits == 2:
-                    quant_cuda.vecquant2matmul_old(
-                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize
-                    )
+                    autogptq_cuda.vecquant2matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
                 elif self.bits == 3:
-                    quant_cuda.vecquant3matmul_old(
-                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize
-                    )
+                    autogptq_cuda.vecquant3matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
                 elif self.bits == 4:
-                    quant_cuda.vecquant4matmul_old(
-                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize
-                    )
+                    autogptq_cuda.vecquant4matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
                 elif self.bits == 8:
-                    quant_cuda.vecquant8matmul_old(
-                        x, self.qweight, out, self.scales.float(), self.qzeros, self.groupsize
-                    )
+                    autogptq_cuda.vecquant8matmul_old(x, self.qweight, out, self.scales.float(), self.qzeros, self.group_size)
                 else:
                     raise NotImplementedError("Only 2,3,4,8 bits are supported.")
         else:
             if self.wf.device != self.qzeros.device:
-                self.wf = self.wf.to(self.qzeros.device)
-
-            if self.bits in [2, 4, 8]:
-                zeros = torch.bitwise_right_shift(
-                    torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits),
-                    self.wf.unsqueeze(0)
-                ).to(torch.int16 if self.bits == 8 else torch.int8)
-                torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
-
-                zeros = zeros + 1
-                zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2])
-
-                scales = self.scales
-                scales = scales.reshape(-1, 1, scales.shape[-1])
-
-                weight = torch.bitwise_right_shift(
-                    torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1),
-                    self.wf.unsqueeze(-1)
-                ).to(torch.int16 if self.bits == 8 else torch.int8)
-                torch.bitwise_and(weight, (2 ** self.bits) - 1, out=weight)
-                weight = weight.reshape(-1, self.groupsize, weight.shape[2])
+               self.wf = self.wf.to(self.qzeros.device)
+                
+            if self.bits in [2,4,8]:
+               zeros = torch.bitwise_right_shift(torch.unsqueeze(self.qzeros, 2).expand(-1, -1, 32 // self.bits), self.wf.unsqueeze(0)).to(torch.int16 if self.bits == 8 else torch.int8)
+               torch.bitwise_and(zeros, (2 ** self.bits) - 1, out=zeros)
+                   
+               zeros = zeros + 1
+               zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2])
+   
+               scales = self.scales
+               scales = scales.reshape(-1, 1, scales.shape[-1])
+                
+               weight = torch.bitwise_right_shift(torch.unsqueeze(self.qweight, 1).expand(-1, 32 // self.bits, -1), self.wf.unsqueeze(-1)).to(torch.int16 if self.bits == 8 else torch.int8)
+               torch.bitwise_and(weight,(2 ** self.bits) - 1, out=weight)
+               weight = weight.reshape(-1, self.group_size, weight.shape[2])
             elif self.bits == 3:
-                zeros = self.qzeros.reshape(
-                    self.qzeros.shape[0], self.qzeros.shape[1] // 3, 3, 1
-                ).expand(-1, -1, -1, 12)
-                zeros = (zeros >> self.wf.unsqueeze(0))
-                zeros[:, :, 0, 10] = (zeros[:, :, 0, 10] & 0x3) | ((zeros[:, :, 1, 0] << 2) & 0x4)
-                zeros[:, :, 1, 11] = (zeros[:, :, 1, 11] & 0x1) | ((zeros[:, :, 2, 0] << 1) & 0x6)
-                zeros = zeros & 0x7
-                zeros = torch.cat([zeros[:, :, 0, :11], zeros[:, :, 1, 1:12], zeros[:, :, 2, 1:11]], dim=2)
-
-                zeros = zeros + 1
-                zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2])
-
-                scales = self.scales
-                scales = scales.reshape(-1, 1, scales.shape[-1])
-
-                weight = self.qweight.reshape(
-                    self.qweight.shape[0] // 3, 3, 1, self.qweight.shape[1]
-                ).expand(-1, -1, 12, -1)
-                weight = (weight >> self.wf.unsqueeze(-1)) & 0x7
-                weight[:, 0, 10] = (weight[:, 0, 10] & 0x3) | ((weight[:, 1, 0] << 2) & 0x4)
-                weight[:, 1, 11] = (weight[:, 1, 11] & 0x1) | ((weight[:, 2, 0] << 1) & 0x6)
-                weight = weight & 0x7
-                weight = torch.cat([weight[:, 0, :11], weight[:, 1, 1:12], weight[:, 2, 1:11]], dim=1)
-                weight = weight.reshape(-1, self.groupsize, weight.shape[2])
+               zeros = self.qzeros.reshape(self.qzeros.shape[0], self.qzeros.shape[1]//3, 3, 1).expand(-1, -1, -1, 12)
+               zeros = (zeros >> self.wf.unsqueeze(0))
+               zeros[:,:,0,10] = (zeros[:,:,0,10]&0x3) | ((zeros[:,:,1,0] << 2)&0x4)
+               zeros[:,:,1,11] = (zeros[:,:,1,11]&0x1) | ((zeros[:,:,2,0] << 1)&0x6)
+               zeros = zeros & 0x7
+               zeros = torch.cat([zeros[:,:,0,:11], zeros[:,:,1,1:12], zeros[:,:,2,1:11]], dim=2)
+                
+               zeros = zeros + 1
+               zeros = zeros.reshape(-1, 1, zeros.shape[1] * zeros.shape[2]) 
+               
+               scales = self.scales
+               scales = scales.reshape(-1, 1, scales.shape[-1])
+                
+               weight = self.qweight.reshape(self.qweight.shape[0]//3, 3, 1, self.qweight.shape[1]).expand(-1, -1, 12, -1)
+               weight = (weight >> self.wf.unsqueeze(-1))&0x7
+               weight[:,0,10] = (weight[:,0,10]&0x3) | ((weight[:,1,0] << 2)&0x4)
+               weight[:,1,11] = (weight[:,1,11]&0x1) | ((weight[:,2,0] << 1)&0x6)
+               weight = weight & 0x7
+               weight = torch.cat([weight[:,0,:11], weight[:,1,1:12], weight[:,2,1:11]], dim=1)
+               weight = weight.reshape(-1, self.group_size, weight.shape[2])
             else:
-                raise NotImplementedError("Only 2,3,4,8 bits are supported.")
-
+               raise NotImplementedError("Only 2,3,4,8 bits are supported.")
             weight = (scales * (weight - zeros))
             weight = weight.reshape(weight.shape[0] * weight.shape[1], weight.shape[2])
 
             out = torch.matmul(x.half(), weight)
-        out = out.reshape(out_shape)
+        out = out.half().reshape(out_shape)
         out = out + self.bias if self.bias is not None else out
         return out
 
 
 __all__ = ["QuantLinear"]
```

### Comparing `auto_gptq-0.1.0/auto_gptq/nn_modules/triton_utils/custom_autotune.py` & `auto_gptq-0.2.0/auto_gptq/nn_modules/triton_utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq/quantization/gptq.py` & `auto_gptq-0.2.0/auto_gptq/quantization/gptq.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         self.nsamples += tmp
         # inp = inp.float()
         inp = math.sqrt(2 / self.nsamples) * inp.float()
         # self.H += 2 / self.nsamples * inp.matmul(inp.t())
         self.H += inp.matmul(inp.t())
 
     def fasterquant(
-        self, blocksize=128, percdamp=.01, groupsize=-1, actorder=False
+        self, blocksize=128, percdamp=.01, group_size=-1, actorder=False
     ):
         W = self.layer.weight.data.clone()
         if isinstance(self.layer, nn.Conv2d):
             W = W.flatten(1)
         if isinstance(self.layer, transformers.Conv1D):
             W = W.t()
         W = W.float()
@@ -111,19 +111,19 @@
             Losses1 = torch.zeros_like(W1)
             Hinv1 = Hinv[i1:i2, i1:i2]
 
             for i in range(count):
                 w = W1[:, i]
                 d = Hinv1[i, i]
 
-                if groupsize != -1:
-                    if (i1 + i) % groupsize == 0:
-                        self.quantizer.find_params(W[:, (i1 + i):(i1 + i + groupsize)], weight=True)
+                if group_size != -1:
+                    if (i1 + i) % group_size == 0:
+                        self.quantizer.find_params(W[:, (i1 + i):(i1 + i + group_size)], weight=True)
 
-                    if ((i1 + i) // groupsize) - now_idx == -1:
+                    if ((i1 + i) // group_size) - now_idx == -1:
                         scale.append(self.quantizer.scale)
                         zero.append(self.quantizer.zero)
                         now_idx += 1
 
                 q = self.quantizer.quantize(w.unsqueeze(1)).flatten()
                 Q1[:, i] = q
                 Losses1[:, i] = (w - q) ** 2 / d ** 2
@@ -143,16 +143,16 @@
                 logger.debug(torch.sum((self.layer(self.inp1) - self.out1) ** 2))
                 logger.debug(torch.sum(Losses))
 
         torch.cuda.synchronize()
         logger.info(f'duration: {(time.time() - tick)}')
         logger.info(f'avg loss: {torch.sum(Losses).item() / self.nsamples}')
 
-        groupsize = groupsize if groupsize != -1 else self.columns
-        g_idx = [i // groupsize for i in range(self.columns)]
+        group_size = group_size if group_size != -1 else self.columns
+        g_idx = [i // group_size for i in range(self.columns)]
         g_idx = torch.tensor(g_idx, dtype=torch.int32, device=Q.device)
         if actorder:
             invperm = torch.argsort(perm)
             Q = Q[:, invperm]
             g_idx = g_idx[invperm]
 
         if isinstance(self.layer, transformers.Conv1D):
```

### Comparing `auto_gptq-0.1.0/auto_gptq/quantization/quantizer.py` & `auto_gptq-0.2.0/auto_gptq/quantization/quantizer.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq/utils/data_utils.py` & `auto_gptq-0.2.0/auto_gptq/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/auto_gptq.egg-info/SOURCES.txt` & `auto_gptq-0.2.0/auto_gptq.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,27 +17,36 @@
 auto_gptq/eval_tasks/_utils/generation_utils.py
 auto_gptq/modeling/__init__.py
 auto_gptq/modeling/_base.py
 auto_gptq/modeling/_const.py
 auto_gptq/modeling/_utils.py
 auto_gptq/modeling/auto.py
 auto_gptq/modeling/bloom.py
+auto_gptq/modeling/codegen.py
 auto_gptq/modeling/gpt2.py
+auto_gptq/modeling/gpt_bigcode.py
 auto_gptq/modeling/gpt_neox.py
 auto_gptq/modeling/gptj.py
 auto_gptq/modeling/llama.py
 auto_gptq/modeling/moss.py
 auto_gptq/modeling/opt.py
+auto_gptq/modeling/rw.py
 auto_gptq/nn_modules/__init__.py
-auto_gptq/nn_modules/layernorm_triton.py
+auto_gptq/nn_modules/_fused_base.py
+auto_gptq/nn_modules/fused_gptj_attn.py
+auto_gptq/nn_modules/fused_llama_attn.py
+auto_gptq/nn_modules/fused_llama_mlp.py
 auto_gptq/nn_modules/qlinear.py
 auto_gptq/nn_modules/qlinear_old.py
 auto_gptq/nn_modules/qlinear_triton.py
 auto_gptq/nn_modules/triton_utils/__init__.py
 auto_gptq/nn_modules/triton_utils/custom_autotune.py
+auto_gptq/nn_modules/triton_utils/kernels.py
+auto_gptq/nn_modules/triton_utils/mixin.py
 auto_gptq/quantization/__init__.py
 auto_gptq/quantization/gptq.py
 auto_gptq/quantization/quantizer.py
 auto_gptq/utils/__init__.py
 auto_gptq/utils/data_utils.py
-quant_cuda/quant_cuda.cpp
-quant_cuda/quant_cuda_kernel.cu
+auto_gptq/utils/import_utils.py
+autogptq_cuda/autogptq_cuda.cpp
+autogptq_cuda/autogptq_cuda_kernel.cu
```

### Comparing `auto_gptq-0.1.0/quant_cuda/quant_cuda.cpp` & `auto_gptq-0.2.0/autogptq_cuda/autogptq_cuda.cpp`

 * *Files identical despite different names*

### Comparing `auto_gptq-0.1.0/quant_cuda/quant_cuda_kernel.cu` & `auto_gptq-0.2.0/autogptq_cuda/autogptq_cuda_kernel.cu`

 * *Files 4% similar despite different names*

```diff
@@ -35,60 +35,60 @@
     const  scalar_t* __restrict__ vec,
     const       int* __restrict__ mat,
            scalar_t* __restrict__ mul,
     const  scalar_t* __restrict__ scales,
     const  		int* __restrict__ zeros,
 	const  	    int* __restrict__ g_idx,
     int batch,
-    int vec_height,
+    int vec_height, 	
     int height,
     int width,
 	int zero_width
 );
 
 template <typename scalar_t>
 __global__ void VecQuant3MatMulKernel(
     const  scalar_t* __restrict__ vec,
     const       int* __restrict__ mat,
            scalar_t* __restrict__ mul,
     const  scalar_t* __restrict__ scales,
     const  		int* __restrict__ zeros,
 	const  	    int* __restrict__ g_idx,
     int batch,
-    int vec_height,
+    int vec_height, 	
     int height,
     int width,
 	int zero_width
 );
 
 template <typename scalar_t>
 __global__ void VecQuant4MatMulKernel(
     const  scalar_t* __restrict__ vec,
     const       int* __restrict__ mat,
            scalar_t* __restrict__ mul,
     const  scalar_t* __restrict__ scales,
     const  		int* __restrict__ zeros,
 	const  	    int* __restrict__ g_idx,
     int batch,
-    int vec_height,
+    int vec_height, 	
     int height,
     int width,
 	int zero_width
 );
 
 template <typename scalar_t>
 __global__ void VecQuant8MatMulKernel(
     const  scalar_t* __restrict__ vec,
     const       int* __restrict__ mat,
            scalar_t* __restrict__ mul,
     const  scalar_t* __restrict__ scales,
     const  		int* __restrict__ zeros,
 	const  	    int* __restrict__ g_idx,
     int batch,
-    int vec_height,
+    int vec_height, 	
     int height,
     int width,
 	int zero_width
 );
 
 template <typename scalar_t>
 __global__ void VecQuant2MatMulKernel_old(
@@ -228,15 +228,15 @@
   );
   dim3 threads(BLOCKWIDTH);
 
   AT_DISPATCH_FLOATING_TYPES(
     vec.type(), "vecquant2matmul_cuda", ([&] {
       VecQuant2MatMulKernel<<<blocks, threads>>>(
         vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
         batch, vec_height, height, width, zero_width
       );
     })
   );
 }
 
 template <typename scalar_t>
@@ -251,47 +251,47 @@
     int vec_height,
     int height,
     int width,
 	int zero_width
 ) {
   int h = BLOCKHEIGHT2 * blockIdx.x;
   int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
+  
   __shared__ scalar_t blockvec[BLOCKWIDTH];
   int i = width * h + w;
   int g_h = h * 16;
   int k;
   unsigned int g;
   scalar_t w_tmp;
-
-  int z_w = w / 16;
+  
+  int z_w = w / 16; 
   int z_mod = (w % 16) * 2;
-
+  
   float weight[BLOCKWIDTH];
-
-  for (k = 0; k <  BLOCKWIDTH; ++k){
-	int k_w = (k / 16);
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 16); 
 	int k_bit = (k % 16) * 2;
-
+	
     g = as_int(g_idx[g_h + k]);
     scalar_t scale = scales[g * width + w];
     scalar_t zero = scalar_t((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod & 0x3) + 1);
-
+	
     w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x3);
-
+    
 	weight[k] = scale * (w_tmp - zero);
   }
 
   scalar_t res;
-  for (int b = 0; b < batch; ++b){
+  for (int b = 0; b < batch; ++b){	
 	res = 0;
-
+	
     blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
     __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
 	  res += weight[k] * blockvec[k];
     }
     atomicAdd(&mul[b * width + w], res);
     __syncthreads();
   }
 }
 
@@ -315,15 +315,15 @@
   );
   dim3 threads(BLOCKWIDTH);
 
   AT_DISPATCH_FLOATING_TYPES(
     vec.type(), "vecquant3matmul_cuda", ([&] {
       VecQuant3MatMulKernel<<<blocks, threads>>>(
         vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
         batch, vec_height, height, width, zero_width
       );
     })
   );
 }
 
 template <typename scalar_t>
@@ -338,23 +338,23 @@
     int vec_height,
     int height,
     int width,
 	int zero_width
 ) {
   int h = BLOCKHEIGHT3 * blockIdx.x;
   int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
+  
   __shared__ scalar_t blockvec[BLOCKWIDTH];
   int i = width * h + w;
   int g_h = (h / 3) * 32;
   int k;
   unsigned int g;
   scalar_t w_tmp;
-
-  int z_w = (w / 32) * 3;
+  
+  int z_w = (w / 32) * 3; 
   int z_mod = w % 32;
   int z_bit;
   unsigned int z_tmp;
   if (z_mod != 10){
     if (z_mod != 21){
       z_bit = z_mod;
       if (z_bit > 21){
@@ -370,22 +370,22 @@
       } else {
         z_bit *= 3;
       }
     } else {
       z_w += 1;
     }
   }
-
+  
   float weight[BLOCKWIDTH];
-
-  for (k = 0; k <  BLOCKWIDTH; ++k){
-	int k_w = (k / 32) * 3;
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 32) * 3; 
 	int k_mod = k % 32;
 	int k_bit;
-
+	  
 	if (k_mod != 10){
 	  if (k_mod != 21){
         k_bit = k_mod;
         if (k_bit > 21){
 		  k_bit -= 22;
 		  k_bit *= 3;
 		  k_bit += 2;
@@ -398,45 +398,45 @@
         } else {
 		  k_bit *= 3;
         }
 	  } else {
         k_w += 1;
 	  }
 	}
-
+	
     g = as_int(g_idx[g_h + k]);
     scalar_t scale = scales[g * width + w];
     scalar_t zero;
     if (z_mod == 10) {
       z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 30) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 2) & 0x4);
       zero = scalar_t((z_tmp) + 1);
     } else if (z_mod == 21){
       z_tmp = (as_unsigned(zeros[g * zero_width + z_w]) >> 31) | ((as_unsigned(zeros[g * zero_width + (z_w + 1)]) << 1) & 0x6);
       zero = scalar_t((z_tmp) + 1);
     } else {
       zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_bit) & 0x7) + 1);
     }
-
+	
     if (k_mod == 10) {
       w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 30) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 2) & 0x4);
     } else if (k_mod == 21){
       w_tmp = (as_unsigned(mat[i + (k_w * width)]) >> 31) | ((as_unsigned(mat[i + ((k_w + 1)* width)]) << 1) & 0x6);
     } else {
       w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0x7);
     }
 	weight[k] = scale * (w_tmp - zero);
   }
 
   scalar_t res;
-  for (int b = 0; b < batch; ++b){
+  for (int b = 0; b < batch; ++b){	
 	res = 0;
-
+	
     blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
     __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
 	  res += weight[k] * blockvec[k];
     }
     atomicAdd(&mul[b * width + w], res);
     __syncthreads();
   }
 }
 
@@ -460,15 +460,15 @@
   );
   dim3 threads(BLOCKWIDTH);
 
   AT_DISPATCH_FLOATING_TYPES(
     vec.type(), "vecquant4matmul_cuda", ([&] {
       VecQuant4MatMulKernel<<<blocks, threads>>>(
         vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
         batch, vec_height, height, width, zero_width
       );
     })
   );
 }
 
 template <typename scalar_t>
@@ -483,48 +483,48 @@
     int vec_height,
     int height,
     int width,
 	int zero_width
 ) {
   int h = BLOCKHEIGHT4 * blockIdx.x;
   int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
+  
   __shared__ scalar_t blockvec[BLOCKWIDTH];
   int i = width * h + w;
   int g_h = h * 8;
   int k;
   unsigned int g;
   scalar_t w_tmp;
+  
 
-
-  int z_w = w / 8;
+  int z_w = w / 8; 
   int z_mod = (w % 8) * 4;
-
+  
   float weight[BLOCKWIDTH];
-
-  for (k = 0; k <  BLOCKWIDTH; ++k){
-	int k_w = (k / 8);
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 8); 
 	int k_bit = (k % 8) * 4;
-
+	
     g = as_int(g_idx[g_h + k]);
     scalar_t scale = scales[g * width + w];
     scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xF) + 1);
-
+	
     w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xF);
-
+    
 	weight[k] = scale * (w_tmp - zero);
   }
 
   scalar_t res;
-  for (int b = 0; b < batch; ++b){
+  for (int b = 0; b < batch; ++b){	
 	res = 0;
-
+	
     blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
     __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
 	  res += weight[k] * blockvec[k];
     }
     atomicAdd(&mul[b * width + w], res);
     __syncthreads();
   }
 }
 
@@ -548,15 +548,15 @@
   );
   dim3 threads(BLOCKWIDTH);
 
   AT_DISPATCH_FLOATING_TYPES(
     vec.type(), "vecquant8matmul_cuda", ([&] {
       VecQuant8MatMulKernel<<<blocks, threads>>>(
         vec.data<scalar_t>(), mat.data<int>(), mul.data<scalar_t>(),
-        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(),
+        scales.data<scalar_t>(), zeros.data<int>(), g_idx.data<int>(), 
         batch, vec_height, height, width, zero_width
       );
     })
   );
 }
 
 template <typename scalar_t>
@@ -571,47 +571,47 @@
     int vec_height,
     int height,
     int width,
 	int zero_width
 ) {
   int h = BLOCKHEIGHT8 * blockIdx.x;
   int w = BLOCKWIDTH * blockIdx.y + threadIdx.x;
-
+  
   __shared__ scalar_t blockvec[BLOCKWIDTH];
   int i = width * h + w;
   int g_h = h * 4;
   int k;
   unsigned int g;
   scalar_t w_tmp;
-
-  int z_w = w / 4;
+  
+  int z_w = w / 4; 
   int z_mod = (w % 4) * 8;
-
+  
   float weight[BLOCKWIDTH];
-
-  for (k = 0; k <  BLOCKWIDTH; ++k){
-	int k_w = (k / 4);
+  
+  for (k = 0; k <  BLOCKWIDTH; ++k){	
+	int k_w = (k / 4); 
 	int k_bit = (k % 4) * 8;
-
+	
     g = as_int(g_idx[g_h + k]);
     scalar_t scale = scales[g * width + w];
     scalar_t zero = scalar_t(((as_unsigned(zeros[g * zero_width + z_w]) >> z_mod) & 0xFF) + 1);
-
+	
     w_tmp = ((as_unsigned(mat[i + (k_w * width)]) >> k_bit) & 0xFF);
-
+    
 	weight[k] = scale * (w_tmp - zero);
   }
 
   scalar_t res;
-  for (int b = 0; b < batch; ++b){
+  for (int b = 0; b < batch; ++b){	
 	res = 0;
-
+	
     blockvec[threadIdx.x] = vec[b * vec_height + blockIdx.x * BLOCKWIDTH + threadIdx.x];
     __syncthreads();
-	for (k = 0; k <  BLOCKWIDTH; ++k){
+	for (k = 0; k <  BLOCKWIDTH; ++k){	
 	  res += weight[k] * blockvec[k];
     }
     atomicAdd(&mul[b * width + w], res);
     __syncthreads();
   }
 }
```

