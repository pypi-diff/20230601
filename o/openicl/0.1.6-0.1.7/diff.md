# Comparing `tmp/openicl-0.1.6.tar.gz` & `tmp/openicl-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openicl-0.1.6.tar", last modified: Tue Mar 28 09:26:17 2023, max compression
+gzip compressed data, was "openicl-0.1.7.tar", last modified: Thu Jun  1 10:30:56 2023, max compression
```

## Comparing `openicl-0.1.6.tar` & `openicl-0.1.7.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-03-28 09:26:17.886513 openicl-0.1.6/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    11357 2023-03-03 05:33:05.000000 openicl-0.1.6/LICENSE
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     4375 2023-03-28 09:26:17.876513 openicl-0.1.6/PKG-INFO
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3746 2023-03-28 09:14:58.000000 openicl-0.1.6/README.md
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-03-28 09:26:17.876513 openicl-0.1.6/openicl/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      182 2023-03-06 07:33:42.000000 openicl-0.1.6/openicl/__init__.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    11390 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_dataset_reader.py
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-03-28 09:26:17.876513 openicl-0.1.6/openicl/icl_evaluator/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      276 2023-03-01 07:54:05.000000 openicl-0.1.6/openicl/icl_evaluator/__init__.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      855 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_evaluator/icl_acc_evaluator.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      486 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_evaluator/icl_api_evaluator.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      207 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_evaluator/icl_base_evaluator.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      456 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_evaluator/icl_bleu_evaluator.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      454 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_evaluator/icl_rouge_evaluator.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      712 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_evaluator/icl_squad_evaluator.py
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-03-28 09:26:17.876513 openicl-0.1.6/openicl/icl_inferencer/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      186 2023-03-01 07:54:05.000000 openicl-0.1.6/openicl/icl_inferencer/__init__.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    13246 2023-03-28 09:10:54.000000 openicl-0.1.6/openicl/icl_inferencer/icl_base_inferencer.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7887 2023-03-28 09:22:25.000000 openicl-0.1.6/openicl/icl_inferencer/icl_cot_inferencer.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7691 2023-03-28 09:20:03.000000 openicl-0.1.6/openicl/icl_inferencer/icl_gen_inferencer.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     9631 2023-03-28 05:42:46.000000 openicl-0.1.6/openicl/icl_inferencer/icl_ppl_inferencer.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     8639 2023-03-28 05:42:46.000000 openicl-0.1.6/openicl/icl_prompt_template.py
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-03-28 09:26:17.876513 openicl-0.1.6/openicl/icl_retriever/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      370 2023-03-09 05:12:30.000000 openicl-0.1.6/openicl/icl_retriever/__init__.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     8148 2023-03-28 05:42:46.000000 openicl-0.1.6/openicl/icl_retriever/icl_base_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3504 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_retriever/icl_bm25_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     6538 2023-03-13 05:42:49.000000 openicl-0.1.6/openicl/icl_retriever/icl_dpp_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7594 2023-03-28 05:42:46.000000 openicl-0.1.6/openicl/icl_retriever/icl_mdl_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2774 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_retriever/icl_random_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     6165 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_retriever/icl_topk_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     5279 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_retriever/icl_votek_retriever.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2024 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/icl_retriever/icl_zero_retriever.py
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-03-28 09:26:17.876513 openicl-0.1.6/openicl/utils/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)       23 2023-03-06 10:38:54.000000 openicl-0.1.6/openicl/utils/__init__.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3523 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/utils/api_service.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      218 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/utils/calculate.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1150 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/utils/check_type.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1931 2023-03-01 07:54:05.000000 openicl-0.1.6/openicl/utils/collators.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2224 2023-03-16 06:06:21.000000 openicl-0.1.6/openicl/utils/icl_common_utils.py
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1108 2023-03-13 09:11:56.000000 openicl-0.1.6/openicl/utils/logging.py
-drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-03-28 09:26:17.876513 openicl-0.1.6/openicl.egg-info/
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     4375 2023-03-28 09:26:17.000000 openicl-0.1.6/openicl.egg-info/PKG-INFO
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1358 2023-03-28 09:26:17.000000 openicl-0.1.6/openicl.egg-info/SOURCES.txt
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)        1 2023-03-28 09:26:17.000000 openicl-0.1.6/openicl.egg-info/dependency_links.txt
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      230 2023-03-28 09:26:17.000000 openicl-0.1.6/openicl.egg-info/requires.txt
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)        8 2023-03-28 09:26:17.000000 openicl-0.1.6/openicl.egg-info/top_level.txt
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)       38 2023-03-28 09:26:17.886513 openicl-0.1.6/setup.cfg
--rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1745 2023-03-28 09:13:32.000000 openicl-0.1.6/setup.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.939597 openicl-0.1.7/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    11357 2023-03-03 05:33:05.000000 openicl-0.1.7/LICENSE
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     4375 2023-06-01 10:30:56.939597 openicl-0.1.7/PKG-INFO
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3746 2023-06-01 10:18:08.000000 openicl-0.1.7/README.md
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.929597 openicl-0.1.7/openicl/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      182 2023-03-06 07:33:42.000000 openicl-0.1.7/openicl/__init__.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    11390 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_dataset_reader.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.929597 openicl-0.1.7/openicl/icl_evaluator/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      276 2023-03-01 07:54:05.000000 openicl-0.1.7/openicl/icl_evaluator/__init__.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      855 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_acc_evaluator.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      486 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_api_evaluator.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      207 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_base_evaluator.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      456 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_bleu_evaluator.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      454 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_rouge_evaluator.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      712 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_evaluator/icl_squad_evaluator.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.929597 openicl-0.1.7/openicl/icl_inferencer/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      240 2023-04-11 06:15:47.000000 openicl-0.1.7/openicl/icl_inferencer/__init__.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)    13690 2023-06-01 10:29:50.000000 openicl-0.1.7/openicl/icl_inferencer/icl_base_inferencer.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     5410 2023-04-11 06:15:47.000000 openicl-0.1.7/openicl/icl_inferencer/icl_channel_inferencer.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7887 2023-03-28 09:22:25.000000 openicl-0.1.7/openicl/icl_inferencer/icl_cot_inferencer.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7691 2023-03-28 09:20:03.000000 openicl-0.1.7/openicl/icl_inferencer/icl_gen_inferencer.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     9631 2023-03-28 05:42:46.000000 openicl-0.1.7/openicl/icl_inferencer/icl_ppl_inferencer.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     8639 2023-03-28 05:42:46.000000 openicl-0.1.7/openicl/icl_prompt_template.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.929597 openicl-0.1.7/openicl/icl_retriever/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      370 2023-03-09 05:12:30.000000 openicl-0.1.7/openicl/icl_retriever/__init__.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     8148 2023-03-28 05:42:46.000000 openicl-0.1.7/openicl/icl_retriever/icl_base_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3504 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_retriever/icl_bm25_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     6538 2023-03-13 05:42:49.000000 openicl-0.1.7/openicl/icl_retriever/icl_dpp_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     7594 2023-03-28 05:42:46.000000 openicl-0.1.7/openicl/icl_retriever/icl_mdl_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2774 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_retriever/icl_random_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     6165 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_retriever/icl_topk_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     5279 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_retriever/icl_votek_retriever.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2024 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/icl_retriever/icl_zero_retriever.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.939597 openicl-0.1.7/openicl/utils/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)       23 2023-03-06 10:38:54.000000 openicl-0.1.7/openicl/utils/__init__.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     3523 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/utils/api_service.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      218 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/utils/calculate.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1150 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/utils/check_type.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1931 2023-03-01 07:54:05.000000 openicl-0.1.7/openicl/utils/collators.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     2224 2023-03-16 06:06:21.000000 openicl-0.1.7/openicl/utils/icl_common_utils.py
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1108 2023-03-13 09:11:56.000000 openicl-0.1.7/openicl/utils/logging.py
+drwxr-xr-x   0 zhangyudejia  (1000) zhangyudejia  (1000)        0 2023-06-01 10:30:56.929597 openicl-0.1.7/openicl.egg-info/
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     4375 2023-06-01 10:30:56.000000 openicl-0.1.7/openicl.egg-info/PKG-INFO
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1407 2023-06-01 10:30:56.000000 openicl-0.1.7/openicl.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)        1 2023-06-01 10:30:56.000000 openicl-0.1.7/openicl.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)      222 2023-06-01 10:30:56.000000 openicl-0.1.7/openicl.egg-info/requires.txt
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)        8 2023-06-01 10:30:56.000000 openicl-0.1.7/openicl.egg-info/top_level.txt
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)       38 2023-06-01 10:30:56.939597 openicl-0.1.7/setup.cfg
+-rw-r--r--   0 zhangyudejia  (1000) zhangyudejia  (1000)     1737 2023-06-01 10:15:55.000000 openicl-0.1.7/setup.py
```

### Comparing `openicl-0.1.6/LICENSE` & `openicl-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/PKG-INFO` & `openicl-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openicl
-Version: 0.1.6
+Version: 0.1.7
 Summary: An open source framework for in-context learning.
 Home-page: https://github.com/Shark-NLP/OpenICL
 Author: Zhenyu Wu, Yaoxiang Wang, Zhiyong Wu, Jiacheng Ye
 Keywords: AI,NLP,in-context learning
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,15 +26,15 @@
   <a href="#installation">Installation</a> •
   <a href="https://arxiv.org/abs/2303.02913">Paper</a> •
   <a href="https://github.com/Shark-NLP/OpenICL/tree/main/examples">Examples</a> •
   <a href="https://openicl.readthedocs.io/en/latest/index.html">Docs</a> •
   <a href="#citation">Citation</a> 
 </p>
 
-![version](https://img.shields.io/badge/version-0.1.6-blue)
+![version](https://img.shields.io/badge/version-0.1.7-blue)
 
 
 ## Overview
 OpenICL provides an easy interface for in-context learning, with many state-of-the-art retrieval and inference methods built in to facilitate systematic comparison of LMs and fast research prototyping. Users can easily incorporate different retrieval and inference methods, as well as different prompt instructions into their workflow. 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg"  border="0" />
 </div>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: openicl Version: 0.1.6 Summary: An open source
+Metadata-Version: 2.1 Name: openicl Version: 0.1.7 Summary: An open source
 framework for in-context learning. Home-page: https://github.com/Shark-NLP/
 OpenICL Author: Zhenyu Wu, Yaoxiang Wang, Zhiyong Wu, Jiacheng Ye Keywords:
 AI,NLP,in-context learning Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Requires-Python: >=3.8.0 Description-Content-Type: text/
 markdown License-File: LICENSE
                  [https://s1.ax1x.com/2023/03/07/ppZfEmq.png]
 ------
     Overview â¢ Installation â¢ Paper â¢ Examples â¢ Docs â¢ Citation
-![version](https://img.shields.io/badge/version-0.1.6-blue) ## Overview OpenICL
+![version](https://img.shields.io/badge/version-0.1.7-blue) ## Overview OpenICL
 provides an easy interface for in-context learning, with many state-of-the-art
 retrieval and inference methods built in to facilitate systematic comparison of
 LMs and fast research prototyping. Users can easily incorporate different
 retrieval and inference methods, as well as different prompt instructions into
 their workflow.
                  [https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg]
 ## Installation Note: OpenICL requires Python 3.8+ **Using Pip** ``` pip
```

### Comparing `openicl-0.1.6/README.md` & `openicl-0.1.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   <a href="#installation">Installation</a> •
   <a href="https://arxiv.org/abs/2303.02913">Paper</a> •
   <a href="https://github.com/Shark-NLP/OpenICL/tree/main/examples">Examples</a> •
   <a href="https://openicl.readthedocs.io/en/latest/index.html">Docs</a> •
   <a href="#citation">Citation</a> 
 </p>
 
-![version](https://img.shields.io/badge/version-0.1.6-blue)
+![version](https://img.shields.io/badge/version-0.1.7-blue)
 
 
 ## Overview
 OpenICL provides an easy interface for in-context learning, with many state-of-the-art retrieval and inference methods built in to facilitate systematic comparison of LMs and fast research prototyping. Users can easily incorporate different retrieval and inference methods, as well as different prompt instructions into their workflow. 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg"  border="0" />
 </div>
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
                  [https://s1.ax1x.com/2023/03/07/ppZfEmq.png]
 ------
     Overview â¢ Installation â¢ Paper â¢ Examples â¢ Docs â¢ Citation
-![version](https://img.shields.io/badge/version-0.1.6-blue) ## Overview OpenICL
+![version](https://img.shields.io/badge/version-0.1.7-blue) ## Overview OpenICL
 provides an easy interface for in-context learning, with many state-of-the-art
 retrieval and inference methods built in to facilitate systematic comparison of
 LMs and fast research prototyping. Users can easily incorporate different
 retrieval and inference methods, as well as different prompt instructions into
 their workflow.
                  [https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg]
 ## Installation Note: OpenICL requires Python 3.8+ **Using Pip** ``` pip
```

### Comparing `openicl-0.1.6/openicl/icl_dataset_reader.py` & `openicl-0.1.7/openicl/icl_dataset_reader.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_evaluator/icl_acc_evaluator.py` & `openicl-0.1.7/openicl/icl_evaluator/icl_acc_evaluator.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_evaluator/icl_squad_evaluator.py` & `openicl-0.1.7/openicl/icl_evaluator/icl_squad_evaluator.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_inferencer/icl_base_inferencer.py` & `openicl-0.1.7/openicl/icl_inferencer/icl_base_inferencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import torch
 from openicl import BaseRetriever, PromptTemplate
 from openicl.utils.api_service import *
 from openicl.icl_evaluator import *
 from transformers import AutoTokenizer, AutoModelForCausalLM, PretrainedConfig, GPT2Tokenizer, AutoConfig, \
     T5ForConditionalGeneration
-from typing import List, Union, Optional
+from typing import List, Union, Optional, Any
 from accelerate import Accelerator
 from accelerate import init_empty_weights, infer_auto_device_map
 
 
 class BaseInferencer:
     """Basic In-context Learning Inferencer Class
         Base class of In-context Learning Inferencer, with no inference method.
@@ -28,16 +28,16 @@
         call_api (:obj:`bool`): If ``True``, an API for LM models will be used, determined by :obj:`api_name`.   
     """
     model = None
     tokenizer = None
     call_api = False
 
     def __init__(self,
-                 model_name: Optional[str] = 'gpt2-xl',
-                 tokenizer_name: Optional[str] = None,
+                 model_name: Optional[Union[str, Any]] = 'gpt2-xl',
+                 tokenizer_name: Optional[Union[str, Any]] = None,
                  max_model_token_num: Optional[int] = None,
                  model_config: Optional[PretrainedConfig] = None,
                  batch_size: Optional[int] = 1,
                  accelerator: Optional[Accelerator] = None,
                  output_json_filepath: Optional[str] = "./icl_inference_output",
                  output_json_filename: Optional[str] = "predictions",
                  api_name: Optional[str] = None,
@@ -93,14 +93,17 @@
 
         Returns:
             :obj:`List:` A list of string, each representing the results of one inference.
         """
         raise NotImplementedError("Method hasn't been implemented yet")
 
     def __init_model(self, model_name, model_config, model_parallel, device_map, no_split_module_classes):
+        if not isinstance(model_name, str):
+            self.model = model_name
+            return
         if not model_parallel:
             if model_config is not None:
                 self.model = self.__get_hf_model_from_config(model_name, model_config)
             else:
                 self.model = self.__get_hf_model_from_name(model_name)
         else:
             if model_config is None:
@@ -128,15 +131,18 @@
         else:
             return AutoModelForCausalLM.from_config(model_config)
 
     def __init_tokenizer(self, tokenizer_name):
         if self.api_name == 'opt-175b':
             self.tokenizer = GPT2Tokenizer.from_pretrained("facebook/opt-30b", use_fast=False)
         else:
-            self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
+            if not isinstance(tokenizer_name, str):
+                self.tokenizer = tokenizer_name
+            else:
+                self.tokenizer = AutoTokenizer.from_pretrained(tokenizer_name)
         self.tokenizer.pad_token = self.tokenizer.eos_token
         self.tokenizer.pad_token_id = self.tokenizer.eos_token_id
         self.tokenizer.padding_side = "left"
 
     def __init_api(self, **kwargs):
         if self.api_name == None:
             return
@@ -190,14 +196,15 @@
         if self.accelerator is not None and self.accelerator.is_main_process:
             for pid in range(self.accelerator.num_processes):
                 with open(f'{output_json_filepath}/process{pid}_{output_json_filename}.json', 'r',
                           encoding='utf-8') as json_file:
                     subprocess_results_dict = json.load(json_file)
                     self.results_dict.update(subprocess_results_dict)
                     json_file.close()
+            self.results_dict = dict(sorted(self.results_dict.items(), key=lambda x: int(x[0])))
 
     def save_orgin_prompts(self, origin_prompts: List[str]):
         for idx, origin_prompt in enumerate(origin_prompts):
             if self.accelerator is not None:
                 idx = idx * self.accelerator.num_processes + self.accelerator.process_index
             self.origin_prompt_dict[str(idx)] = origin_prompt
 
@@ -233,14 +240,15 @@
         if self.accelerator is not None and self.accelerator.is_main_process:
             for pid in range(self.accelerator.num_processes):
                 with open(f'{output_json_filepath}/process{pid}_{output_json_filename}.json', 'r',
                           encoding='utf-8') as json_file:
                     subprocess_results_dict = json.load(json_file)
                     self.results_dict.update(subprocess_results_dict)
                     json_file.close()
+            self.results_dict = dict(sorted(self.results_dict.items(), key=lambda x: int(x[0])))
 
     def save_ice(self, ice):
         for idx, example in enumerate(ice):
             if self.accelerator is not None:
                 idx = idx * self.accelerator.num_processes + self.accelerator.process_index
             if str(idx) not in self.results_dict.keys():
                 self.results_dict[str(idx)] = {}
```

### Comparing `openicl-0.1.6/openicl/icl_inferencer/icl_cot_inferencer.py` & `openicl-0.1.7/openicl/icl_inferencer/icl_cot_inferencer.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_inferencer/icl_gen_inferencer.py` & `openicl-0.1.7/openicl/icl_inferencer/icl_gen_inferencer.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_inferencer/icl_ppl_inferencer.py` & `openicl-0.1.7/openicl/icl_inferencer/icl_ppl_inferencer.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_prompt_template.py` & `openicl-0.1.7/openicl/icl_prompt_template.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_retriever/icl_base_retriever.py` & `openicl-0.1.7/openicl/icl_retriever/icl_base_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_retriever/icl_bm25_retriever.py` & `openicl-0.1.7/openicl/icl_retriever/icl_bm25_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_retriever/icl_dpp_retriever.py` & `openicl-0.1.7/openicl/icl_retriever/icl_dpp_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_retriever/icl_mdl_retriever.py` & `openicl-0.1.7/openicl/icl_retriever/icl_mdl_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_retriever/icl_random_retriever.py` & `openicl-0.1.7/openicl/icl_retriever/icl_random_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_retriever/icl_topk_retriever.py` & `openicl-0.1.7/openicl/icl_retriever/icl_topk_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_retriever/icl_votek_retriever.py` & `openicl-0.1.7/openicl/icl_retriever/icl_votek_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/icl_retriever/icl_zero_retriever.py` & `openicl-0.1.7/openicl/icl_retriever/icl_zero_retriever.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/utils/api_service.py` & `openicl-0.1.7/openicl/utils/api_service.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/utils/check_type.py` & `openicl-0.1.7/openicl/utils/check_type.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/utils/collators.py` & `openicl-0.1.7/openicl/utils/collators.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/utils/icl_common_utils.py` & `openicl-0.1.7/openicl/utils/icl_common_utils.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl/utils/logging.py` & `openicl-0.1.7/openicl/utils/logging.py`

 * *Files identical despite different names*

### Comparing `openicl-0.1.6/openicl.egg-info/PKG-INFO` & `openicl-0.1.7/openicl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openicl
-Version: 0.1.6
+Version: 0.1.7
 Summary: An open source framework for in-context learning.
 Home-page: https://github.com/Shark-NLP/OpenICL
 Author: Zhenyu Wu, Yaoxiang Wang, Zhiyong Wu, Jiacheng Ye
 Keywords: AI,NLP,in-context learning
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -26,15 +26,15 @@
   <a href="#installation">Installation</a> •
   <a href="https://arxiv.org/abs/2303.02913">Paper</a> •
   <a href="https://github.com/Shark-NLP/OpenICL/tree/main/examples">Examples</a> •
   <a href="https://openicl.readthedocs.io/en/latest/index.html">Docs</a> •
   <a href="#citation">Citation</a> 
 </p>
 
-![version](https://img.shields.io/badge/version-0.1.6-blue)
+![version](https://img.shields.io/badge/version-0.1.7-blue)
 
 
 ## Overview
 OpenICL provides an easy interface for in-context learning, with many state-of-the-art retrieval and inference methods built in to facilitate systematic comparison of LMs and fast research prototyping. Users can easily incorporate different retrieval and inference methods, as well as different prompt instructions into their workflow. 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg"  border="0" />
 </div>
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: openicl Version: 0.1.6 Summary: An open source
+Metadata-Version: 2.1 Name: openicl Version: 0.1.7 Summary: An open source
 framework for in-context learning. Home-page: https://github.com/Shark-NLP/
 OpenICL Author: Zhenyu Wu, Yaoxiang Wang, Zhiyong Wu, Jiacheng Ye Keywords:
 AI,NLP,in-context learning Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Science/Research Requires-Python: >=3.8.0 Description-Content-Type: text/
 markdown License-File: LICENSE
                  [https://s1.ax1x.com/2023/03/07/ppZfEmq.png]
 ------
     Overview â¢ Installation â¢ Paper â¢ Examples â¢ Docs â¢ Citation
-![version](https://img.shields.io/badge/version-0.1.6-blue) ## Overview OpenICL
+![version](https://img.shields.io/badge/version-0.1.7-blue) ## Overview OpenICL
 provides an easy interface for in-context learning, with many state-of-the-art
 retrieval and inference methods built in to facilitate systematic comparison of
 LMs and fast research prototyping. Users can easily incorporate different
 retrieval and inference methods, as well as different prompt instructions into
 their workflow.
                  [https://s1.ax1x.com/2023/03/07/ppZWjmt.jpg]
 ## Installation Note: OpenICL requires Python 3.8+ **Using Pip** ``` pip
```

### Comparing `openicl-0.1.6/openicl.egg-info/SOURCES.txt` & `openicl-0.1.7/openicl.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 openicl/icl_evaluator/icl_api_evaluator.py
 openicl/icl_evaluator/icl_base_evaluator.py
 openicl/icl_evaluator/icl_bleu_evaluator.py
 openicl/icl_evaluator/icl_rouge_evaluator.py
 openicl/icl_evaluator/icl_squad_evaluator.py
 openicl/icl_inferencer/__init__.py
 openicl/icl_inferencer/icl_base_inferencer.py
+openicl/icl_inferencer/icl_channel_inferencer.py
 openicl/icl_inferencer/icl_cot_inferencer.py
 openicl/icl_inferencer/icl_gen_inferencer.py
 openicl/icl_inferencer/icl_ppl_inferencer.py
 openicl/icl_retriever/__init__.py
 openicl/icl_retriever/icl_base_retriever.py
 openicl/icl_retriever/icl_bm25_retriever.py
 openicl/icl_retriever/icl_dpp_retriever.py
```

### Comparing `openicl-0.1.6/setup.py` & `openicl-0.1.7/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,28 +6,28 @@
     def run(self):
         self.do_egg_install()
         import nltk
         nltk.download('punkt')
 
 
 REQUIRES = """
-accelerate==0.15.0
-datasets==2.7.1
-evaluate==0.3.0
-faiss_gpu==1.7.2
-nltk==3.8
-numpy==1.23.4
-openai==0.27.1
-rank_bm25==0.2.2
-requests==2.28.1
-scikit_learn==1.2.1
-sentence_transformers==2.2.2
-torch>=1.13.1
-tqdm==4.64.1
 transformers
+accelerate
+datasets>=2.7.1
+evaluate>=0.3.0
+faiss_gpu>=1.7.2
+nltk>=3.8
+numpy>=1.23.4
+openai>=0.27.1
+rank_bm25>=0.2.2
+requests>=2.28.1
+scikit_learn>=1.2.1
+sentence_transformers>=2.2.2
+torch>=1.13.1
+tqdm>=4.64.1
 """
 
 
 def get_install_requires():
     reqs = [req for req in REQUIRES.split("\n") if len(req) > 0]
     return reqs
 
@@ -35,15 +35,15 @@
 with open("README.md") as f:
     readme = f.read()
 
 
 def do_setup():
     setup(
         name="openicl",
-        version='0.1.6',
+        version='0.1.7',
         description="An open source framework for in-context learning.",
         url="https://github.com/Shark-NLP/OpenICL",
         author='Zhenyu Wu, Yaoxiang Wang, Zhiyong Wu, Jiacheng Ye',
         long_description=readme,
         long_description_content_type="text/markdown",
         cmdclass={'download_nltk': DownloadNLTK},
         install_requires=get_install_requires(),
```

