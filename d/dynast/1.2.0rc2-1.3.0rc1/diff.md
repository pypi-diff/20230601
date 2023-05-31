# Comparing `tmp/dynast-1.2.0rc2.tar.gz` & `tmp/dynast-1.3.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dynast-1.2.0rc2.tar", last modified: Mon Apr 24 23:41:32 2023, max compression
+gzip compressed data, was "dynast-1.3.0rc1.tar", last modified: Wed May 31 22:10:22 2023, max compression
```

## Comparing `dynast-1.2.0rc2.tar` & `dynast-1.3.0rc1.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:32.193252 dynast-1.2.0rc2/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1676 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/LICENSE.md
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-04-24 23:41:32.189252 dynast-1.2.0rc2/PKG-INFO
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13175 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/README.md
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:30.961126 dynast-1.2.0rc2/dynast/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      639 2023-02-09 17:30:13.000000 dynast-1.2.0rc2/dynast/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.117142 dynast-1.2.0rc2/dynast/analytics/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.2.0rc2/dynast/analytics/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3114 2023-02-09 17:30:13.000000 dynast-1.2.0rc2/dynast/analytics/results.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4440 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/analytics/visualize.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4260 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/cli.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      662 2023-02-09 17:30:13.000000 dynast-1.2.0rc2/dynast/common.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4540 2023-04-17 18:37:40.000000 dynast-1.2.0rc2/dynast/dynast_manager.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.149145 dynast-1.2.0rc2/dynast/measure/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.2.0rc2/dynast/measure/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1601 2023-02-09 17:30:13.000000 dynast-1.2.0rc2/dynast/measure/latency.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.197150 dynast-1.2.0rc2/dynast/predictors/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:13.000000 dynast-1.2.0rc2/dynast/predictors/__init__.py
--rwxr-xr-x   0 mszankin (11413730) aipg_labs (17685)     6754 2023-02-09 17:30:13.000000 dynast-1.2.0rc2/dynast/predictors/dynamic_predictor.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1974 2023-02-15 23:55:06.000000 dynast-1.2.0rc2/dynast/predictors/predictor_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      663 2023-02-09 17:30:14.000000 dynast-1.2.0rc2/dynast/python.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.281159 dynast-1.2.0rc2/dynast/search/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.2.0rc2/dynast/search/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9805 2023-02-28 00:09:11.000000 dynast-1.2.0rc2/dynast/search/encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1849 2023-02-09 17:30:14.000000 dynast-1.2.0rc2/dynast/search/evaluation_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16411 2023-03-01 18:19:31.000000 dynast-1.2.0rc2/dynast/search/evolutionary.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    41232 2023-04-24 21:57:09.000000 dynast-1.2.0rc2/dynast/search/search_tactic.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.313162 dynast-1.2.0rc2/dynast/supernetwork/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.2.0rc2/dynast/supernetwork/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.333164 dynast-1.2.0rc2/dynast/supernetwork/image_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:14.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.377169 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.413172 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.437175 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.497181 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      815 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2294 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    11238 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.525184 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.573189 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      847 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    29037 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13827 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.625194 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      912 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14924 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14562 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12722 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3638 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.677199 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1178 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10456 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8794 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8315 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.713203 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      887 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8399 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16263 2023-04-24 21:57:09.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4500 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.789211 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      966 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4597 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24387 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.833215 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      660 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1925 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3552 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9184 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4792 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6956 2023-04-24 21:57:09.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2236 2023-03-01 18:23:06.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    15317 2023-04-24 23:41:02.000000 dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa_interface.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.889221 dynast-1.2.0rc2/dynast/supernetwork/machine_translation/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.2.0rc2/dynast/supernetwork/machine_translation/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24388 2023-03-02 04:20:04.000000 dynast-1.2.0rc2/dynast/supernetwork/machine_translation/modules_supernetwork.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7753 2023-02-09 17:30:14.000000 dynast-1.2.0rc2/dynast/supernetwork/machine_translation/transformer_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    22144 2023-04-24 21:57:09.000000 dynast-1.2.0rc2/dynast/supernetwork/machine_translation/transformer_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    43476 2023-03-06 23:12:11.000000 dynast-1.2.0rc2/dynast/supernetwork/machine_translation/transformer_supernetwork.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.905223 dynast-1.2.0rc2/dynast/supernetwork/recommendation/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:15.000000 dynast-1.2.0rc2/dynast/supernetwork/recommendation/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4812 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/supernetwork/supernetwork_registry.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.969229 dynast-1.2.0rc2/dynast/supernetwork/text_classification/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-04-17 21:20:59.000000 dynast-1.2.0rc2/dynast/supernetwork/text_classification/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5836 2023-04-19 16:16:52.000000 dynast-1.2.0rc2/dynast/supernetwork/text_classification/bert_encoding.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12532 2023-04-24 21:57:09.000000 dynast-1.2.0rc2/dynast/supernetwork/text_classification/bert_interface.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7283 2023-03-06 23:12:11.000000 dynast-1.2.0rc2/dynast/supernetwork/text_classification/bert_supernetwork.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3599 2023-03-02 00:16:55.000000 dynast-1.2.0rc2/dynast/supernetwork/text_classification/sst2_dataloader.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:32.041237 dynast-1.2.0rc2/dynast/utils/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7599 2023-04-13 00:13:03.000000 dynast-1.2.0rc2/dynast/utils/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3441 2023-02-09 17:30:15.000000 dynast-1.2.0rc2/dynast/utils/cache.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9665 2023-04-17 23:29:51.000000 dynast-1.2.0rc2/dynast/utils/datasets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2286 2023-03-01 18:23:06.000000 dynast-1.2.0rc2/dynast/utils/distributed.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6569 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/utils/nn.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6722 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/dynast/utils/reference.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:31.061136 dynast-1.2.0rc2/dynast.egg-info/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-04-24 23:41:30.000000 dynast-1.2.0rc2/dynast.egg-info/PKG-INFO
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4906 2023-04-24 23:41:30.000000 dynast-1.2.0rc2/dynast.egg-info/SOURCES.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)        1 2023-04-24 23:41:30.000000 dynast-1.2.0rc2/dynast.egg-info/dependency_links.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       43 2023-04-24 23:41:30.000000 dynast-1.2.0rc2/dynast.egg-info/entry_points.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      354 2023-04-24 23:41:30.000000 dynast-1.2.0rc2/dynast.egg-info/requires.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       13 2023-04-24 23:41:30.000000 dynast-1.2.0rc2/dynast.egg-info/top_level.txt
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      316 2023-03-06 23:12:04.000000 dynast-1.2.0rc2/pyproject.toml
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       38 2023-04-24 23:41:32.197253 dynast-1.2.0rc2/setup.cfg
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2241 2023-04-24 23:41:26.000000 dynast-1.2.0rc2/setup.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:32.141247 dynast-1.2.0rc2/tests/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:16.000000 dynast-1.2.0rc2/tests/__init__.py
-drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-04-24 23:41:32.177251 dynast-1.2.0rc2/tests/checks/
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-02-09 17:30:16.000000 dynast-1.2.0rc2/tests/checks/__init__.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2104 2023-04-24 21:46:13.000000 dynast-1.2.0rc2/tests/checks/check_license.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1155 2023-02-09 17:30:16.000000 dynast-1.2.0rc2/tests/checks/helpers.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2715 2023-04-17 23:32:40.000000 dynast-1.2.0rc2/tests/functional_reference.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1451 2023-02-09 17:30:16.000000 dynast-1.2.0rc2/tests/test_cache.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1249 2023-02-09 17:30:16.000000 dynast-1.2.0rc2/tests/test_datasets.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3897 2023-04-17 18:37:41.000000 dynast-1.2.0rc2/tests/test_dynast_manager.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      905 2023-02-09 17:30:16.000000 dynast-1.2.0rc2/tests/test_nn.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6136 2023-03-06 23:12:11.000000 dynast-1.2.0rc2/tests/test_utils.py
--rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3149 2023-03-06 23:12:11.000000 dynast-1.2.0rc2/tests/test_utils_distributed.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1676 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/LICENSE.md
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/PKG-INFO
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13175 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/README.md
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.546404 dynast-1.3.0rc1/dynast/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      639 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/analytics/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/analytics/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3111 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/analytics/results.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10039 2023-05-31 17:20:13.000000 dynast-1.3.0rc1/dynast/analytics/visualize.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4860 2023-05-30 21:43:00.000000 dynast-1.3.0rc1/dynast/cli.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      662 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/common.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4540 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/dynast_manager.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/measure/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/measure/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1601 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/measure/latency.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/predictors/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/predictors/__init__.py
+-rwxr-xr-x   0 mszankin (11413730) aipg_labs (17685)     6751 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/predictors/dynamic_predictor.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1974 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/predictors/predictor_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      663 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/python.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/search/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/search/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9805 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/search/encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2609 2023-05-30 21:50:38.000000 dynast-1.3.0rc1/dynast/search/evaluation_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16397 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/search/evolutionary.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    41296 2023-05-30 21:43:00.000000 dynast-1.3.0rc1/dynast/search/search_tactic.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/supernetwork/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.550403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      815 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2294 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    11238 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      847 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    29037 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13827 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      912 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14923 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    14561 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12721 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3638 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1178 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10456 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8793 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8312 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.554403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      887 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     8399 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    16147 2023-05-05 17:45:18.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4500 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.558403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      966 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4597 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24387 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.558403 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      660 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1925 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3552 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     9184 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4792 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6955 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2235 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    15297 2023-05-31 22:09:25.000000 dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa_interface.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.558403 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    24388 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/modules_supernetwork.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7752 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    22141 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    43472 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_supernetwork.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.558403 dynast-1.3.0rc1/dynast/supernetwork/recommendation/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/recommendation/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4812 2023-05-30 21:43:00.000000 dynast-1.3.0rc1/dynast/supernetwork/supernetwork_registry.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.558403 dynast-1.3.0rc1/dynast/supernetwork/text_classification/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/text_classification/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     5836 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_encoding.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    12046 2023-05-30 21:50:38.000000 dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_interface.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7282 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_supernetwork.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3595 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/supernetwork/text_classification/sst2_dataloader.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/dynast/utils/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     7599 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/utils/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3441 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/utils/cache.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    10458 2023-05-30 18:27:20.000000 dynast-1.3.0rc1/dynast/utils/datasets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2286 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/dynast/utils/distributed.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6423 2023-05-18 21:41:10.000000 dynast-1.3.0rc1/dynast/utils/nn.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6734 2023-05-05 17:45:18.000000 dynast-1.3.0rc1/dynast/utils/reference.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.546404 dynast-1.3.0rc1/dynast.egg-info/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)    13692 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/PKG-INFO
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     4906 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/SOURCES.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)        1 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/dependency_links.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       43 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/entry_points.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      295 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/requires.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       13 2023-05-31 22:10:22.000000 dynast-1.3.0rc1/dynast.egg-info/top_level.txt
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      361 2023-05-05 17:45:18.000000 dynast-1.3.0rc1/pyproject.toml
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)       38 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/setup.cfg
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2241 2023-05-31 22:10:04.000000 dynast-1.3.0rc1/setup.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/tests/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/__init__.py
+drwxr-sr-x   0 mszankin (11413730) aipg_labs (17685)        0 2023-05-31 22:10:22.562403 dynast-1.3.0rc1/tests/checks/
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      583 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/checks/__init__.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2104 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/checks/check_license.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1168 2023-05-05 17:45:18.000000 dynast-1.3.0rc1/tests/checks/helpers.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     2715 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/functional_reference.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1451 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/test_cache.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     1873 2023-05-30 20:09:23.000000 dynast-1.3.0rc1/tests/test_datasets.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3897 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/test_dynast_manager.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)      905 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/test_nn.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     6136 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/test_utils.py
+-rw-r--r--   0 mszankin (11413730) aipg_labs (17685)     3149 2023-05-01 19:25:12.000000 dynast-1.3.0rc1/tests/test_utils_distributed.py
```

### Comparing `dynast-1.2.0rc2/LICENSE.md` & `dynast-1.3.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/PKG-INFO` & `dynast-1.3.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynast
-Version: 1.2.0rc2
+Version: 1.3.0rc1
 Summary: DyNAS-T (Dynamic Neural Architecture Search Toolkit) - a SuperNet NAS optimization package
 Author: Maciej Szankin, Sharath Nittur Sridhar, Anthony Sarah, Sairam Sundaresan
 Author-email: maciej.szankin@intel.com, sharath.nittur.sridhar@intel.com, anthony.sarah@intel.com, sairam.sundaresan@intel.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `dynast-1.2.0rc2/README.md` & `dynast-1.3.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/__init__.py` & `dynast-1.3.0rc1/dynast/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/analytics/__init__.py` & `dynast-1.3.0rc1/dynast/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/analytics/results.py` & `dynast-1.3.0rc1/dynast/analytics/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,21 +27,19 @@
 
     csv_path - output csv file name
     manager - ParameterManager object
     search_output - pymoo results object from the SearchAlgoManager
     '''
 
     def __init__(self, csv_path, manager, search_output):
-
         self.csv_path = csv_path
         self.manager = manager
         self.search_output = search_output
 
     def front_to_csv(self, filepath=None, overwrite=True):
-
         if filepath is None:
             filepath = self.csv_path[:-4] + '_front.csv'
 
         if overwrite:
             with open(filepath, 'w') as f:
                 writer = csv.writer(f)
 
@@ -56,15 +54,14 @@
                 date = str(datetime.now())
                 writer.writerow([sample, date, obj_x, -obj_y])
         log.info('Final search population saved to: {}'.format(filepath))
 
         return None
 
     def history_to_csv(self, filepath=None, overwrite=True):
-
         if filepath is None:
             filepath = self.csv_path
 
         if overwrite:
             with open(filepath, 'w') as f:
                 writer = csv.writer(f)
```

### Comparing `dynast-1.2.0rc2/dynast/cli.py` & `dynast-1.3.0rc1/dynast/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,27 @@
+# Copyright (c) 2022 Intel Corporation
+#
+# Licensed under the Apache License, Version 2.0 (the "License");
+# you may not use this file except in compliance with the License.
+# You may obtain a copy of the License at
+#
+#   http://www.apache.org/licenses/LICENSE-2.0
+#
+# Unless required by applicable law or agreed to in writing, software
+# distributed under the License is distributed on an "AS IS" BASIS,
+# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+# See the License for the specific language governing permissions and
+# limitations under the License.
+
 import argparse
 
 from dynast.dynast_manager import DyNAS
 
 
 def _main(args):
-
     agent = DyNAS(
         supernet=args.supernet,
         optimization_metrics=args.optimization_metrics,
         measurements=args.measurements,
         search_tactic=args.search_tactic,
         num_evals=args.num_evals,
         results_path=args.results_path,
@@ -16,15 +29,15 @@
         seed=args.seed,
         population=args.population,
         batch_size=args.batch_size,
         search_algo=args.search_algo,
         verbose=args.verbose,
         supernet_ckpt_path=args.supernet_ckpt_path,
         device=args.device,
-        test_size=args.test_size,
+        test_fraction=args.test_fraction,
         dataloader_workers=args.dataloader_workers,
         distributed=args.distributed,
     )
 
     results = agent.search()
 
     print('Search results: ', results)
@@ -64,18 +77,18 @@
         type=str,
         help='Measurements during search.',
     )
     parser.add_argument('-d', '--device', default='cpu', type=str, help='Target device to run measurements on.')
     parser.add_argument('--num_evals', default=250, type=int, help='Total number of evaluations during search.')
     parser.add_argument('--batch_size', default=128, type=int, help='Batch size for latency measurement calculation.')
     parser.add_argument(
-        '--test_size',
-        default=None,
-        type=int,
-        help='How many batches of data to use when evaluating model\'s accuracy.',
+        '--test_fraction',
+        default=1.0,
+        type=float,
+        help='Fraction of the validation data to be used for testing and evaluation.',
     )
     parser.add_argument('--dataloader_workers', default=4, type=int, help='How many workers to use when loading data.')
     parser.add_argument('--population', default=50, type=int, help='Population size for each generation')
     parser.add_argument('--results_path', required=True, type=str, help='Path to store search results, csv format')
     parser.add_argument('--dataset_path', default='/datasets/imagenet-ilsvrc2012', type=str, help='')
     parser.add_argument('--supernet_ckpt_path', default=None, type=str, help='Path to supernet checkpoint.')
```

### Comparing `dynast-1.2.0rc2/dynast/common.py` & `dynast-1.3.0rc1/dynast/common.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/dynast_manager.py` & `dynast-1.3.0rc1/dynast/dynast_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/measure/__init__.py` & `dynast-1.3.0rc1/dynast/measure/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/measure/latency.py` & `dynast-1.3.0rc1/dynast/measure/latency.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/predictors/__init__.py` & `dynast-1.3.0rc1/dynast/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/predictors/dynamic_predictor.py` & `dynast-1.3.0rc1/dynast/predictors/dynamic_predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,27 +18,25 @@
 from scipy.stats import kendalltau, spearmanr
 from sklearn import linear_model, svm
 from sklearn.metrics import mean_absolute_percentage_error, mean_squared_error
 from sklearn.model_selection import GridSearchCV
 
 
 class Predictor:
-
     DEFAULT_ALPHAS = np.arange(0.1, 10.1, 0.1)
     DEFAULT_COST_FACTORS = np.arange(1.0, 101.0, 1.0)
     DEFAULT_MAX_ITERATIONS = 1000000
 
     def __init__(
         self,
         alphas=DEFAULT_ALPHAS,
         cost_factors=DEFAULT_COST_FACTORS,
         max_iterations=DEFAULT_MAX_ITERATIONS,
         verbose=False,
     ):
-
         SEARCHER_VERBOSITY = 10
 
         # Initialize label normalization factor
         self.normalization_factor = 1.0
 
         # Initialize best searcher index
         self.best_index = 0
@@ -60,15 +58,14 @@
                     n_jobs=-1,
                     scoring='neg_mean_absolute_percentage_error',
                     verbose=SEARCHER_VERBOSITY if (verbose) else 0,
                 )
             )
 
     def train(self, examples, labels):
-
         '''
         Trains the predictor on the specified examples and labels using the underlying regressor.
 
         Parameters
         ----------
             examples: Examples to be used for training.
             labels: Labels to be used for training.
```

### Comparing `dynast-1.2.0rc2/dynast/predictors/predictor_manager.py` & `dynast-1.3.0rc1/dynast/predictors/predictor_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/python.py` & `dynast-1.3.0rc1/dynast/python.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/search/__init__.py` & `dynast-1.3.0rc1/dynast/search/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/search/encoding.py` & `dynast-1.3.0rc1/dynast/search/encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/search/evolutionary.py` & `dynast-1.3.0rc1/dynast/search/evolutionary.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,14 @@
         num_evals=1000,
         warm_pop=None,
         crossover_prob=0.9,
         crossover_eta=15.0,
         mutation_prob=0.02,
         mutation_eta=20.0,
     ):
-
         self.n_gens = num_evals / population
 
         if type(warm_pop) == 'numpy.ndarray':
             log.info('Using warm start population.')
             sample_strategy = warm_pop
         else:
             sample_strategy = IntegerRandomSampling()
@@ -369,21 +368,19 @@
 
     def __init__(self, evaluation_interface, param_count, param_upperbound):
         super().__init__(n_var=param_count, n_obj=1, n_constr=0, xl=0, xu=param_upperbound, type_var=int)
 
         self.evaluation_interface = evaluation_interface
 
     def _evaluate(self, x, out, *args, **kwargs):
-
         # Store results for a given generation for PyMoo
         objective_arr = list()
 
         # Measure new individuals
         for i in range(len(x)):
-
             _, objective = self.evaluation_interface.eval_subnet(x[i])
 
             objective_arr.append(objective)
 
         print('.', end='', flush=True)
 
         # Update PyMoo with evaluation data
@@ -406,21 +403,19 @@
 
     def __init__(self, evaluation_interface, param_count, param_upperbound):
         super().__init__(n_var=param_count, n_obj=2, n_constr=0, xl=0, xu=param_upperbound, type_var=int)
 
         self.evaluation_interface = evaluation_interface
 
     def _evaluate(self, x, out, *args, **kwargs):
-
         # Store results for a given generation for PyMoo
         objective_x_arr, objective_y_arr = list(), list()
 
         # Measure new individuals
         for i in range(len(x)):
-
             _, objective_x, objective_y = self.evaluation_interface.eval_subnet(x[i])
 
             objective_x_arr.append(objective_x)
             objective_y_arr.append(objective_y)
 
         print('.', end='', flush=True)
 
@@ -444,21 +439,19 @@
 
     def __init__(self, evaluation_interface, param_count, param_upperbound):
         super().__init__(n_var=param_count, n_obj=3, n_constr=0, xl=0, xu=param_upperbound, type_var=int)
 
         self.evaluation_interface = evaluation_interface
 
     def _evaluate(self, x, out, *args, **kwargs):
-
         # Store results for a given generation for PyMoo
         objective_x_arr, objective_y_arr, objective_z_arr = list(), list(), list()
 
         # Measure new individuals
         for i in range(len(x)):
-
             _, objective_x, objective_y, objective_z = self.evaluation_interface.eval_subnet(x[i])
 
             objective_x_arr.append(objective_x)
             objective_y_arr.append(objective_y)
             objective_z_arr.append(objective_z)
 
         print('.', end='', flush=True)
```

### Comparing `dynast-1.2.0rc2/dynast/search/search_tactic.py` & `dynast-1.3.0rc1/dynast/search/search_tactic.py`

 * *Files 3% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         seed: int = 42,
         population: int = 50,
         batch_size: int = 1,
         verbose: bool = False,
         search_algo: str = 'nsga2',
         supernet_ckpt_path: str = None,
         device: str = 'cpu',
-        test_size: int = None,
+        test_fraction: float = 1.0,
         dataloader_workers: int = 4,
         **kwargs,
     ):
         """Params:
 
         - dataset_path - (str) Path to the dataset needed by the supernetwork runner (e.g., ImageNet is used by OFA)
         - supernet - (str) Super-network name
@@ -77,25 +77,24 @@
         self.population = population
         self.batch_size = batch_size
         self.verbose = verbose
         self.search_algo = search_algo
         self.supernet_ckpt_path = supernet_ckpt_path
         self.device = device
         self.dataloader_workers = dataloader_workers
-        self.test_size = test_size
+        self.test_fraction = test_fraction
 
         self.verify_measurement_types()
         self.format_csv_header()
         self.init_supernet()
 
         if kwargs:
             log.debug('Passed unused parameters: {}'.format(kwargs))
 
     def verify_measurement_types(self):
-
         # Remove duplicates
         self.optimization_metrics = list(set(self.optimization_metrics))
         self.num_objectives = len(self.optimization_metrics)  # TODO(macsz) Can be a getter
         self.measurements = list(set(self.measurements))
 
         # Check that measurements counts are correct
         if self.num_objectives > 3 or self.num_objectives < 1:
@@ -186,25 +185,26 @@
         ]:
             self.runner_validate = OFARunner(
                 supernet=self.supernet,
                 dataset_path=self.dataset_path,
                 batch_size=self.batch_size,
                 device=self.device,
                 dataloader_workers=self.dataloader_workers,
-                test_size=self.test_size,
-                verbose=self.verbose,
+                test_fraction=self.test_fraction,
             )
         elif self.supernet == 'transformer_lt_wmt_en_de':
+            # TODO(macsz) Add `test_fraction`
             self.runner_validate = TransformerLTRunner(
                 supernet=self.supernet,
                 dataset_path=self.dataset_path,
                 batch_size=self.batch_size,
                 checkpoint_path=self.supernet_ckpt_path,
             )
         elif self.supernet == 'bert_base_sst2':
+            # TODO(macsz) Add `test_fraction`
             self.runner_validate = BertSST2Runner(
                 supernet=self.supernet,
                 dataset_path=self.dataset_path,
                 batch_size=self.batch_size,
                 checkpoint_path=self.supernet_ckpt_path,
                 device=self.device,
             )
@@ -242,15 +242,15 @@
         verbose: bool = False,
         search_algo: str = 'nsga2',
         population: int = 50,
         seed: int = 42,
         batch_size: int = 1,
         supernet_ckpt_path: str = None,
         device: str = 'cpu',
-        test_size: int = None,
+        test_fraction: float = 1.0,
         dataloader_workers: int = 4,
         **kwargs,
     ):
         """Params:
 
         - dataset_path - (str) Path to the dataset needed by the supernetwork runner (e.g., ImageNet is used by OFA)
         - supernet - (str) Super-network name
@@ -273,15 +273,15 @@
             seed=seed,
             population=population,
             batch_size=batch_size,
             verbose=verbose,
             search_algo=search_algo,
             supernet_ckpt_path=supernet_ckpt_path,
             device=device,
-            test_size=test_size,
+            test_fraction=test_fraction,
             dataloader_workers=dataloader_workers,
         )
 
     def train_predictors(self, results_path: str = None):
         """Handles the training of predictors for the LINAS inner-loop based on the
         user-defined optimization metrics.
 
@@ -343,16 +343,15 @@
                     latency_predictor=self.predictor_dict['latency'],
                     macs_predictor=self.predictor_dict['macs'],
                     params_predictor=self.predictor_dict['params'],
                     acc_predictor=self.predictor_dict['accuracy_top1'],
                     dataset_path=self.dataset_path,
                     device=self.device,
                     dataloader_workers=self.dataloader_workers,
-                    test_size=self.test_size,
-                    verbose=self.verbose,
+                    test_fraction=self.test_fraction,
                 )
             elif self.supernet == 'transformer_lt_wmt_en_de':
                 runner_predict = TransformerLTRunner(
                     supernet=self.supernet,
                     latency_predictor=self.predictor_dict['latency'],
                     macs_predictor=self.predictor_dict['macs'],
                     params_predictor=self.predictor_dict['params'],
@@ -492,15 +491,15 @@
         results_path,
         seed=42,
         population=50,
         batch_size=1,
         verbose=False,
         search_algo='nsga2',
         supernet_ckpt_path=None,
-        test_size: int = None,
+        test_fraction: float = 1.0,
         dataloader_workers: int = 4,
         device: str = 'cpu',
         **kwargs,
     ):
         super().__init__(
             dataset_path=dataset_path,
             supernet=supernet,
@@ -511,20 +510,19 @@
             seed=seed,
             population=population,
             batch_size=batch_size,
             verbose=verbose,
             search_algo=search_algo,
             supernet_ckpt_path=supernet_ckpt_path,
             device=device,
-            test_size=test_size,
+            test_fraction=test_fraction,
             dataloader_workers=dataloader_workers,
         )
 
     def search(self):
-
         self._init_search()
 
         # Following sets up the algorithm based on number of objectives
         # Could be refractored at the expense of readability
         if self.num_objectives == 1:
             problem = EvolutionarySingleObjective(
                 evaluation_interface=self.validation_interface,
@@ -630,15 +628,15 @@
         seed=42,
         population=50,
         batch_size=1,
         verbose=False,
         search_algo='nsga2',
         supernet_ckpt_path: str = None,
         device: str = 'cpu',
-        test_size: int = None,
+        test_fraction: float = 1.0,
         dataloader_workers: int = 4,
         **kwargs,
     ):
         super().__init__(
             dataset_path=dataset_path,
             supernet=supernet,
             optimization_metrics=optimization_metrics,
@@ -648,20 +646,19 @@
             seed=seed,
             population=population,
             batch_size=batch_size,
             verbose=verbose,
             search_algo=search_algo,
             supernet_ckpt_path=supernet_ckpt_path,
             device=device,
-            test_size=test_size,
+            test_fraction=test_fraction,
             dataloader_workers=dataloader_workers,
         )
 
     def search(self):
-
         self._init_search()
 
         # Randomly sample search space for initial population
         latest_population = [self.supernet_manager.random_sample() for _ in range(self.population)]
 
         # High-Fidelity Validation measurements
         for _, individual in enumerate(latest_population):
@@ -686,15 +683,15 @@
         verbose: bool = False,
         search_algo: str = 'nsga2',
         population: int = 50,
         seed: int = 42,
         batch_size: int = 1,
         supernet_ckpt_path: str = None,
         device: str = 'cpu',
-        test_size: int = None,
+        test_fraction: float = 1.0,
         dataloader_workers: int = 4,
         **kwargs,
     ):
         self.main_results_path = results_path
         LOCAL_RANK, WORLD_RANK, WORLD_SIZE, DIST_METHOD = get_distributed_vars()
         results_path = get_worker_results_path(results_path, WORLD_RANK)
 
@@ -708,15 +705,15 @@
             seed=seed,
             population=population,
             batch_size=batch_size,
             verbose=verbose,
             search_algo=search_algo,
             supernet_ckpt_path=supernet_ckpt_path,
             device=device,
-            test_size=test_size,
+            test_fraction=test_fraction,
             dataloader_workers=dataloader_workers,
         )
 
     def search(self):
         """Runs the LINAS search"""
 
         self._init_search()
@@ -780,16 +777,15 @@
                         latency_predictor=self.predictor_dict['latency'],
                         macs_predictor=self.predictor_dict['macs'],
                         params_predictor=self.predictor_dict['params'],
                         acc_predictor=self.predictor_dict['accuracy_top1'],
                         dataset_path=self.dataset_path,
                         device=self.device,
                         dataloader_workers=self.dataloader_workers,
-                        test_size=self.test_size,
-                        verbose=self.verbose,
+                        test_fraction=self.test_fraction,
                     )
                 elif self.supernet == 'transformer_lt_wmt_en_de':
                     runner_predict = TransformerLTRunner(
                         supernet=self.supernet,
                         latency_predictor=self.predictor_dict['latency'],
                         macs_predictor=self.predictor_dict['macs'],
                         params_predictor=self.predictor_dict['params'],
@@ -926,15 +922,15 @@
         results_path,
         seed=42,
         population=50,
         batch_size=1,
         verbose=False,
         search_algo='nsga2',
         supernet_ckpt_path: str = None,
-        test_size: int = None,
+        test_fraction: float = 1.0,
         dataloader_workers: int = 4,
         **kwargs,
     ):
         self.main_results_path = results_path
         LOCAL_RANK, WORLD_RANK, WORLD_SIZE, DIST_METHOD = get_distributed_vars()
         results_path = get_worker_results_path(results_path, WORLD_RANK)
 
@@ -947,20 +943,19 @@
             results_path=results_path,
             seed=seed,
             population=population,
             batch_size=batch_size,
             verbose=verbose,
             search_algo=search_algo,
             supernet_ckpt_path=supernet_ckpt_path,
-            test_size=test_size,
+            test_fraction=test_fraction,
             dataloader_workers=dataloader_workers,
         )
 
     def search(self):
-
         self._init_search()
 
         LOCAL_RANK, WORLD_RANK, WORLD_SIZE, DIST_METHOD = get_distributed_vars()
 
         if is_main_process():
             log.info('Creating data')
             # Randomly sample search space for initial population
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/base_provider.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/data_providers/imagenet.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         n_worker=32,
         resize_scale=0.08,
         distort_color=None,
         image_size=224,
         num_replicas=None,
         rank=None,
     ):
-
         warnings.filterwarnings("ignore")
         self._save_path = save_path
 
         self.image_size = image_size  # int or list of int
         self.distort_color = "None" if distort_color is None else distort_color
         self.resize_scale = resize_scale
 
@@ -189,15 +188,15 @@
     def valid_path(self):
         return os.path.join(self.save_path, "val")
 
     @property
     def normalize(self):
         return transforms.Normalize(mean=[0.485, 0.456, 0.406], std=[0.229, 0.224, 0.225])
 
-    def build_train_transform(self, image_size=None, print_log=True):
+    def build_train_transform(self, image_size=None, print_log=False):
         if image_size is None:
             image_size = self.image_size
         if print_log:
             print(
                 "Color jitter: %s, resize_scale: %s, img_size: %s" % (self.distort_color, self.resize_scale, image_size)
             )
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_layers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/modules/dynamic_op.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_mbv3.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,14 @@
         dropout_rate=0.1,
         base_stage_width=None,
         width_mult=1.0,
         ks_list=3,
         expand_ratio_list=6,
         depth_list=4,
     ):
-
         self.width_mult = width_mult
         self.ks_list = val2list(ks_list, 1)
         self.expand_ratio_list = val2list(expand_ratio_list, 1)
         self.depth_list = val2list(depth_list, 1)
 
         self.ks_list.sort()
         self.expand_ratio_list.sort()
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_proxyless.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         dropout_rate=0.1,
         base_stage_width=None,
         width_mult=1.0,
         ks_list=3,
         expand_ratio_list=6,
         depth_list=4,
     ):
-
         self.width_mult = width_mult
         self.ks_list = val2list(ks_list, 1)
         self.expand_ratio_list = val2list(expand_ratio_list, 1)
         self.depth_list = val2list(depth_list, 1)
 
         self.ks_list.sort()
         self.expand_ratio_list.sort()
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/networks/ofa_resnets.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         n_classes=1000,
         bn_param=(0.1, 1e-5),
         dropout_rate=0,
         depth_list=2,
         expand_ratio_list=0.25,
         width_mult_list=1.0,
     ):
-
         self.depth_list = val2list(depth_list)
         self.expand_ratio_list = val2list(expand_ratio_list)
         self.width_mult_list = val2list(width_mult_list)
         # sort
         self.depth_list.sort()
         self.expand_ratio_list.sort()
         self.width_mult_list.sort()
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/elastic_nn/utils.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/mobilenet_v3.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/proxyless_nets.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,14 @@
         bn_param=(0.1, 1e-3),
         dropout_rate=0.2,
         ks=None,
         expand_ratio=None,
         depth_param=None,
         stage_width_list=None,
     ):
-
         ks = 3 if ks is None else ks
         expand_ratio = 6 if expand_ratio is None else expand_ratio
 
         input_channel = 32
         last_channel = 1280
 
         input_channel = make_divisible(input_channel * width_mult, MyNetwork.CHANNEL_DIVISIBLE)
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/networks/resnets.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     set_layer_from_config,
 )
 
 __all__ = ["ResNets", "ResNet50", "ResNet50D"]
 
 
 class ResNets(MyNetwork):
-
     BASE_DEPTH_LIST = [2, 2, 4, 2]
     STAGE_WIDTH_LIST = [256, 512, 1024, 2048]
 
     def __init__(self, input_stem, blocks, classifier):
         super(ResNets, self).__init__()
 
         self.input_stem = nn.ModuleList(input_stem)
@@ -121,15 +120,14 @@
         n_classes=1000,
         width_mult=1.0,
         bn_param=(0.1, 1e-5),
         dropout_rate=0,
         expand_ratio=None,
         depth_param=None,
     ):
-
         expand_ratio = 0.25 if expand_ratio is None else expand_ratio
 
         input_channel = make_divisible(64 * width_mult, MyNetwork.CHANNEL_DIVISIBLE)
         stage_width_list = ResNets.STAGE_WIDTH_LIST.copy()
         for i, width in enumerate(stage_width_list):
             stage_width_list[i] = make_divisible(width * width_mult, MyNetwork.CHANNEL_DIVISIBLE)
 
@@ -184,15 +182,14 @@
         n_classes=1000,
         width_mult=1.0,
         bn_param=(0.1, 1e-5),
         dropout_rate=0,
         expand_ratio=None,
         depth_param=None,
     ):
-
         expand_ratio = 0.25 if expand_ratio is None else expand_ratio
 
         input_channel = make_divisible(64 * width_mult, MyNetwork.CHANNEL_DIVISIBLE)
         mid_input_channel = make_divisible(input_channel // 2, MyNetwork.CHANNEL_DIVISIBLE)
         stage_width_list = ResNets.STAGE_WIDTH_LIST.copy()
         for i, width in enumerate(stage_width_list):
             stage_width_list[i] = make_divisible(width * width_mult, MyNetwork.CHANNEL_DIVISIBLE)
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_config.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/imagenet_classification/run_manager/run_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,20 +73,15 @@
         else:
             self.device = torch.device("cpu")
         # initialize model (default)
         if init:
             init_models(run_config.model_init)
 
         # net info
-        net_info = get_net_info(
-            net=self.net,
-            input_shape=self.run_config.data_provider.data_shape,
-            measure_latency=measure_latency,
-            print_info=self.verbose,
-        )
+        net_info = get_net_info(self.net, self.run_config.data_provider.data_shape, measure_latency)
         with open("%s/net_info.txt" % self.path, "w") as fout:
             fout.write(json.dumps(net_info, indent=4) + "\n")
             # noinspection PyBroadException
             try:
                 fout.write(self.network.module_str + "\n")
             except Exception:
                 pass
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/model_zoo.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/common_tools.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/layers.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_distributed_sampler.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_dataloader/my_random_resize_crop.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/my_modules.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa/utils/pytorch_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,14 @@
 
 def count_parameters(net):
     total_params = sum(p.numel() for p in net.parameters() if p.requires_grad)
     return total_params
 
 
 def count_net_flops(net, data_shape=(1, 3, 224, 224)):
-
     if isinstance(net, nn.DataParallel):
         net = net.module
 
     return get_macs(net, data_shape)
 
 
 def measure_net_latency(net, l_type="gpu8", fast=True, input_shape=(3, 224, 224), clean=False):
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa_encoding.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa_encoding.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         keys = list(set(keys))
         for k in keys:
             if k not in d:
                 d[k] = len(list(d.keys()))
         return d
 
     def onehot_custom(self, ks_list: list, ex_list: list, d_list: list) -> np.ndarray:
-
         ks_map = self.construct_maps(keys=(3, 5, 7))
         ex_map = self.construct_maps(keys=(3, 4, 6))
         dp_map = self.construct_maps(keys=(2, 3, 4))
 
         # This function converts a network config to a feature vector (128-D).
         start = 0
         end = 4
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/image_classification/ofa/ofa_interface.py` & `dynast-1.3.0rc1/dynast/supernetwork/image_classification/ofa/ofa_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,50 +49,49 @@
         acc_predictor: Predictor = None,
         macs_predictor: Predictor = None,
         latency_predictor: Predictor = None,
         params_predictor: Predictor = None,
         batch_size: int = 1,
         dataloader_workers: int = 4,
         device: str = 'cpu',
-        test_size: int = None,
+        test_fraction: float = 1.0,
         verbose: bool = False,
     ):
         self.supernet = supernet
         self.acc_predictor = acc_predictor
         self.macs_predictor = macs_predictor
         self.latency_predictor = latency_predictor
         self.params_predictor = params_predictor
         self.batch_size = batch_size
         self.device = device
-        self.test_size = test_size
-        self.verbose = verbose
+        self.test_fraction = test_fraction
         self.dataset_path = dataset_path
         self.dataloader_workers = dataloader_workers
+        self.verbose = verbose
         ImagenetDataProvider.DEFAULT_PATH = dataset_path
 
         self.ofa_network = ofa_model_zoo.ofa_net(supernet, pretrained=True)
         self.run_config = ImagenetRunConfig(
             test_batch_size=batch_size,
             n_worker=dataloader_workers,
-            valid_size=test_size,
         )
         self._init_data()
 
     def _init_data(self):
+        ImageNet.PATH = self.dataset_path
         if self.dataset_path:
-            ImageNet.PATH = self.dataset_path
             self.dataloader = ImageNet.validation_dataloader(
                 batch_size=self.batch_size,
                 num_workers=self.dataloader_workers,
+                fraction=self.test_fraction,
             )
         else:
             self.dataloader = None
             log.warning('No dataset path provided. Cannot validate sub-networks.')
 
-
     def estimate_accuracy_top1(self, subnet_cfg) -> float:
         top1 = self.acc_predictor.predict(subnet_cfg)
         return top1
 
     def estimate_macs(self, subnet_cfg) -> int:
         macs = self.macs_predictor.predict(subnet_cfg)
         return macs
@@ -121,15 +120,14 @@
 
         # Test sampled subnet
         self.run_config.data_provider.assign_active_img_size(subnet_cfg['r'][0])
 
         loss, top1, top5 = validate_classification(
             model=subnet,
             data_loader=self.dataloader,
-            test_size=self.test_size,
             device=self.device,
         )
 
         return top1
 
     def validate_macs_params(self, subnet_cfg: dict, device: str = None) -> Tuple[int, int]:
         """Measure Torch model's FLOPs/MACs as per FVCore calculation
@@ -189,15 +187,15 @@
             measure_steps=measure_steps,
             device=device,
         )
         return latency_mean, latency_std
 
     def get_subnet(self, subnet_cfg):
         if self.supernet == 'ofa_resnet50':
-            self.ofa_network.set_active_subnet(ks=subnet_cfg['d'], e=subnet_cfg['e'], d=subnet_cfg['w'])
+            self.ofa_network.set_active_subnet(d=subnet_cfg['d'], e=subnet_cfg['e'], w=subnet_cfg['w'])
         else:
             self.ofa_network.set_active_subnet(ks=subnet_cfg['ks'], e=subnet_cfg['e'], d=subnet_cfg['d'])
 
         self.subnet = self.ofa_network.get_active_subnet(preserve_weight=True)
         self.subnet.eval()
         return self.subnet
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/machine_translation/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/machine_translation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/machine_translation/modules_supernetwork.py` & `dynast-1.3.0rc1/dynast/supernetwork/machine_translation/modules_supernetwork.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/machine_translation/transformer_encoding.py` & `dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 
 class TransformerLTEncoding(EncodingBase):
     def __init__(self, param_dict: dict, verbose: bool = False, seed: int = 0):
         super().__init__(param_dict, verbose, seed)
 
     def onehot_custom(self, subnet_cfg, provide_onehot=True, encode_layer_num_int=6):
-
         features = []
         features.extend(subnet_cfg['encoder_embed_dim'])
 
         # Encoder FFN Embed Dim
         encoder_ffn_embed_dim = subnet_cfg['encoder_ffn_embed_dim']
 
         if encode_layer_num_int < 6:
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/machine_translation/transformer_interface.py` & `dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -310,15 +310,14 @@
         end = torch.cuda.Event(enable_timing=True)
 
     model.set_sample_config(config)
 
     model.eval()
 
     with torch.no_grad():
-
         # dry runs
         for _ in range(15):
             encoder_out_test = model.encoder(src_tokens=src_tokens_test, src_lengths=src_lengths_test)
 
         encoder_latencies = []
         log.info('Measuring encoder for dataset generation...')
         for _ in range(args.latiter):
@@ -466,15 +465,14 @@
         acc_predictor=None,
         macs_predictor=None,
         latency_predictor=None,
         params_predictor=None,
         batch_size=1,
         checkpoint_path=None,
     ):
-
         self.supernet = supernet
         self.acc_predictor = acc_predictor
         self.macs_predictor = macs_predictor
         self.latency_predictor = latency_predictor
         self.params_predictor = params_predictor
         self.batch_size = batch_size
         self.device = 'cpu'  # TODO(macsz) It's not used anywhere
@@ -503,15 +501,14 @@
         latency = self.latency_predictor.predict(subnet_cfg)
         return latency
 
     def validate_bleu(
         self,
         subnet_cfg: dict,
     ) -> float:  # pragma: no cover
-
         bleu = compute_bleu(subnet_cfg, self.dataset_path, self.checkpoint_path)
         return bleu
 
     def validate_macs(
         self,
         subnet_cfg: dict,
     ) -> Tuple[float, float]:
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/machine_translation/transformer_supernetwork.py` & `dynast-1.3.0rc1/dynast/supernetwork/machine_translation/transformer_supernetwork.py`

 * *Files 1% similar despite different names*

```diff
@@ -174,15 +174,14 @@
             self.layer_norm = LayerNormSuper(self.super_embed_dim)
         else:
             self.layer_norm = None
 
         self.vocab_original_scaling = False
 
     def set_sample_config(self, config: dict):
-
         self.sample_embed_dim = config['encoder']['encoder_embed_dim']
 
         # Caution: this is a list for all layers
         self.sample_ffn_embed_dim = config['encoder']['encoder_ffn_embed_dim']
 
         self.sample_layer_num = config['encoder']['encoder_layer_num']
 
@@ -405,15 +404,14 @@
 
         self.layer_norm = None
         self.get_attn = False
 
         self.vocab_original_scaling = False
 
     def set_sample_config(self, config: dict):
-
         self.sample_embed_dim = config['decoder']['decoder_embed_dim']
         self.sample_encoder_embed_dim = config['encoder']['encoder_embed_dim']
 
         # Caution: this is a list for all layers
         self.sample_ffn_embed_dim = config['decoder']['decoder_ffn_embed_dim']
 
         # Caution: this is a list for all layers
@@ -714,15 +712,14 @@
         is_identity_layer,
         sample_embed_dim=None,
         sample_ffn_embed_dim_this_layer=None,
         sample_self_attention_heads_this_layer=None,
         sample_dropout=None,
         sample_activation_dropout=None,
     ):
-
         if is_identity_layer:
             self.is_identity_layer = True
             return
 
         self.is_identity_layer = False
 
         self.sample_embed_dim = sample_embed_dim
@@ -915,15 +912,14 @@
         sample_encoder_embed_dim=None,
         sample_ffn_embed_dim_this_layer=None,
         sample_self_attention_heads_this_layer=None,
         sample_ende_attention_heads_this_layer=None,
         sample_dropout=None,
         sample_activation_dropout=None,
     ):
-
         if is_identity_layer:
             self.is_identity_layer = True
             return
 
         self.is_identity_layer = False
 
         self.sample_embed_dim = sample_embed_dim
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/recommendation/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/recommendation/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/supernetwork_registry.py` & `dynast-1.3.0rc1/dynast/supernetwork/supernetwork_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,13 +102,13 @@
 }
 
 SUPERNET_METRICS = {
     'ofa_resnet50': ['params', 'latency', 'macs', 'accuracy_top1'],
     'ofa_mbv3_d234_e346_k357_w1.0': ['params', 'latency', 'macs', 'accuracy_top1'],
     'ofa_mbv3_d234_e346_k357_w1.2': ['params', 'latency', 'macs', 'accuracy_top1'],
     'ofa_proxyless_d234_e346_k357_w1.3': ['params', 'latency', 'macs', 'accuracy_top1'],
-    'transformer_lt_wmt_en_de': ['latency', 'macs', 'params', 'bleu'],
-    'bert_base_sst2': ['latency', 'macs', 'params', 'accuracy_sst2'],
+    'transformer_lt_wmt_en_de': ['params', 'latency', 'macs', 'bleu'],
+    'bert_base_sst2': ['params', 'latency', 'macs', 'accuracy_sst2'],
 }
 
 
 SEARCH_ALGORITHMS = ['linas', 'evolutionary', 'random']
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/text_classification/__init__.py` & `dynast-1.3.0rc1/dynast/supernetwork/text_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/text_classification/bert_encoding.py` & `dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_encoding.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/text_classification/bert_interface.py` & `dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,17 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import copy
-import csv
 import logging
 import time
 import warnings
-from datetime import datetime
 
 import numpy as np
 import torch
 import torchprofile
 from transformers import BertConfig
 
 from dynast.search.evaluation_interface import EvaluationInterface
@@ -31,15 +29,14 @@
 from .bert_supernetwork import BertSupernetForSequenceClassification
 from .sst2_dataloader import prepare_data_loader
 
 warnings.filterwarnings("ignore")
 
 
 def load_supernet(checkpoint_path):
-
     bert_config = BertConfig()
     model = BertSupernetForSequenceClassification(bert_config, num_labels=2)
     model.load_state_dict(
         torch.load(checkpoint_path, map_location='cpu')["model"],
         strict=True,
     )
     return model, bert_config
@@ -57,15 +54,14 @@
     model.to(device)
     model.set_sample_config(config)
 
     preds = None
     out_label_ids = None
 
     for i, (input_ids, input_mask, segment_ids, label_ids) in enumerate(eval_dataloader):
-
         input_ids = input_ids.to(device)
         input_mask = input_mask.to(device)
         segment_ids = segment_ids.to(device)
         label_ids = label_ids.to(device)
 
         with torch.no_grad():
             network_outputs = model(input_ids, attention_mask=input_mask, token_type_ids=segment_ids, labels=label_ids)
@@ -191,15 +187,14 @@
         macs_predictor=None,
         latency_predictor=None,
         params_predictor=None,
         batch_size: int = 16,
         checkpoint_path=None,
         device: str = 'cpu',
     ):
-
         self.supernet = supernet
         self.acc_predictor = acc_predictor
         self.macs_predictor = macs_predictor
         self.latency_predictor = latency_predictor
         self.params_predictor = params_predictor
         self.batch_size = batch_size
         self.dataset_path = dataset_path
@@ -229,15 +224,14 @@
         latency = self.latency_predictor.predict(subnet_cfg)
         return latency
 
     def validate_accuracy_sst2(
         self,
         subnet_cfg: dict,
     ) -> float:  # pragma: no cover
-
         accuracy_sst2 = compute_accuracy_sst2(subnet_cfg, self.eval_dataloader, self.supernet_model, device=self.device)
         return accuracy_sst2
 
     def validate_macs(
         self,
         subnet_cfg: dict,
     ) -> float:
@@ -332,28 +326,19 @@
             if 'latency' in self.measurements:
                 individual_results['latency'], _ = self.evaluator.measure_latency(subnet_sample)
             if 'accuracy_sst2' in self.measurements:
                 individual_results['accuracy_sst2'] = self.evaluator.validate_accuracy_sst2(subnet_sample)
 
         subnet_sample = param_dict
         sample = param_dict
-        # Write result for csv_path
-        if self.csv_path:
-            with open(self.csv_path, 'a') as f:
-                writer = csv.writer(f)
-                date = str(datetime.now())
-                result = [
-                    subnet_sample,
-                    date,
-                    individual_results['params'],
-                    individual_results['latency'],
-                    individual_results['macs'],
-                    individual_results['accuracy_sst2'],
-                ]
-                writer.writerow(result)
+
+        # self.write_results(
+        #     subnet_sample=subnet_sample,
+        # )
+        # exit()
 
         # PyMoo only minimizes objectives, thus accuracy needs to be negative
         individual_results['accuracy_sst2'] = -individual_results['accuracy_sst2']
         # Return results to pymoo
         if len(self.optimization_metrics) == 1:
             return sample, individual_results[self.optimization_metrics[0]]
         elif len(self.optimization_metrics) == 2:
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/text_classification/bert_supernetwork.py` & `dynast-1.3.0rc1/dynast/supernetwork/text_classification/bert_supernetwork.py`

 * *Files 0% similar despite different names*

```diff
@@ -121,15 +121,14 @@
         encoder_attention_mask=None,
         past_key_values=None,
         use_cache=None,
         output_attentions=False,
         output_hidden_states=False,
         return_dict=True,
     ):
-
         for layer_idx, layer_module in enumerate(self.layer):
             if layer_idx >= self.subnet_num_layers:
                 break
 
             layer_head_mask = None
             past_key_value = None
```

### Comparing `dynast-1.2.0rc2/dynast/supernetwork/text_classification/sst2_dataloader.py` & `dynast-1.3.0rc1/dynast/supernetwork/text_classification/sst2_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 def convert_examples_to_features(examples, label_list, max_seq_length, tokenizer):
     """Loads a data file into a list of dictionaries."""
 
     label_map = {label: i for i, label in enumerate(label_list)}
 
     features = []
-    for (ex_index, example) in enumerate(examples):
+    for ex_index, example in enumerate(examples):
         tokens_a = tokenizer.tokenize(example.text_a)
         # Account for [CLS] and [SEP] with "- 2"
         if len(tokens_a) > max_seq_length - 2:
             tokens_a = tokens_a[: (max_seq_length - 2)]
 
         tokens = ["[CLS]"] + tokens_a + ["[SEP]"]
         segment_ids = [0] * len(tokens)
@@ -57,15 +57,14 @@
             {"input_ids": input_ids, "input_mask": input_mask, "segment_ids": segment_ids, "label_id": label_id}
         )
 
     return features
 
 
 def create_tensor_dataset(features):
-
     batch_input_ids = []
     batch_input_mask = []
     batch_segment_ids = []
     batch_label_ids = []
 
     for feature in features:
         batch_input_ids.append(feature["input_ids"])
@@ -78,15 +77,14 @@
         torch.tensor(batch_input_mask, dtype=torch.long),
         torch.tensor(batch_segment_ids, dtype=torch.long),
         torch.tensor(batch_label_ids, dtype=torch.long),
     )
 
 
 def prepare_data_loader(dataset_path, max_seq_length=128, eval_batch_size=16):
-
     tokenizer = BertTokenizer.from_pretrained('bert-base-uncased')
     processor = glue_processors["sst-2"]()
     num_labels = len(processor.get_labels())
 
     eval_examples = processor.get_dev_examples(dataset_path)
 
     eval_features = convert_examples_to_features(
```

### Comparing `dynast-1.2.0rc2/dynast/utils/__init__.py` & `dynast-1.3.0rc1/dynast/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/utils/cache.py` & `dynast-1.3.0rc1/dynast/utils/cache.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/utils/datasets.py` & `dynast-1.3.0rc1/dynast/utils/datasets.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,14 +18,23 @@
 import torchvision
 import torchvision.datasets as datasets
 import torchvision.transforms as transforms
 
 from dynast.utils import measure_time
 
 
+def _dataset_fraction(dataset: torchvision.datasets.DatasetFolder, fraction: float):
+    # Use random subset of validation data if valid fraction specified
+    if (fraction > 0.0) and (fraction < 1.0):
+        random_indices = torch.randperm(len(dataset))
+        example_count = round(fraction * len(dataset))
+        dataset = torch.utils.data.Subset(dataset, random_indices[:example_count])
+    return dataset
+
+
 class Dataset(object):
     PATH = ""
 
     @staticmethod
     def name():
         raise NotImplementedError()
 
@@ -129,22 +138,26 @@
     @measure_time
     def validation_dataloader(
         batch_size: int,
         image_size: int = 224,
         val_dir: str = None,
         shuffle: bool = False,
         num_workers: int = 16,
+        fraction: float = 1.0,
     ) -> torch.utils.data.DataLoader:
         if not val_dir:
             val_dir = os.path.join(ImageNet.PATH, "val")
 
         val_dataset = datasets.ImageFolder(
             val_dir,
             ImageNet.val_transforms(image_size),
         )
+
+        val_dataset = _dataset_fraction(val_dataset, fraction)
+
         val_sampler = torch.utils.data.SequentialSampler(val_dataset)
         val_loader = torch.utils.data.DataLoader(
             val_dataset,
             batch_size=batch_size,
             shuffle=shuffle,
             num_workers=num_workers,
             pin_memory=True if torch.cuda.is_available() else False,
@@ -199,22 +212,26 @@
     @measure_time
     def validation_dataloader(
         batch_size: int,
         image_size: int = 224,
         val_dir: str = None,
         shuffle: bool = False,
         num_workers: int = 16,
+        fraction: float = 1.0,
     ) -> torch.utils.data.DataLoader:
         if not val_dir:
             val_dir = os.path.join(Imagenette.PATH, "val")
 
         val_dataset = datasets.ImageFolder(
             val_dir,
             ImageNet.val_transforms(image_size),
         )
+
+        val_dataset = _dataset_fraction(val_dataset, fraction)
+
         val_sampler = torch.utils.data.SequentialSampler(val_dataset)
         val_loader = torch.utils.data.DataLoader(
             val_dataset,
             batch_size=batch_size,
             shuffle=shuffle,
             num_workers=num_workers,
             pin_memory=True if torch.cuda.is_available() else False,
@@ -272,21 +289,25 @@
 
     @staticmethod
     @measure_time
     def validation_dataloader(
         batch_size: int,
         shuffle: bool = False,
         num_workers=16,
+        fraction: float = 1.0,
     ) -> torch.utils.data.DataLoader:
         testset = torchvision.datasets.CIFAR10(
             root=CIFAR10.PATH,
             train=False,
             download=True,
             transform=CIFAR10.val_transforms(),
         )
+
+        testset = _dataset_fraction(testset, fraction)
+
         testloader = torch.utils.data.DataLoader(
             testset,
             batch_size=batch_size,
             shuffle=shuffle,
             num_workers=num_workers,
             pin_memory=True if torch.cuda.is_available() else False,
         )
@@ -303,15 +324,14 @@
     def train_dataloader(
         train_dir: str,
         batch_size: int,
         data_transforms: transforms.Compose,
         shuffle: bool = True,
         num_workers: int = 16,
     ) -> torch.utils.data.DataLoader:
-
         image_dataset = datasets.ImageFolder(train_dir, data_transforms)
         return torch.utils.data.DataLoader(
             image_dataset,
             batch_size=batch_size,
             shuffle=shuffle,
             num_workers=num_workers,
             pin_memory=True if torch.cuda.is_available() else False,
@@ -321,17 +341,20 @@
     @measure_time
     def validation_dataloader(
         val_dir: str,
         batch_size: int,
         data_transforms: transforms.Compose,
         shuffle: bool = False,
         num_workers: int = 16,
+        fraction: float = 1.0,
     ) -> torch.utils.data.DataLoader:
-
         image_dataset = datasets.ImageFolder(val_dir, data_transforms)
+
+        image_dataset = _dataset_fraction(image_dataset, fraction)
+
         return torch.utils.data.DataLoader(
             image_dataset,
             batch_size=batch_size,
             shuffle=shuffle,
             num_workers=num_workers,
             pin_memory=True if torch.cuda.is_available() else False,
         )
```

### Comparing `dynast-1.2.0rc2/dynast/utils/distributed.py` & `dynast-1.3.0rc1/dynast/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/dynast/utils/nn.py` & `dynast-1.3.0rc1/dynast/utils/nn.py`

 * *Files 4% similar despite different names*

```diff
@@ -65,35 +65,31 @@
         return res
 
 
 @measure_time
 def validate_classification(
     model,
     data_loader,
-    test_size=None,
     device='cpu',
 ):
     test_criterion = nn.CrossEntropyLoss()
 
     model = model.eval()
 
     losses = AverageMeter()
     top1 = AverageMeter()
     top5 = AverageMeter()
 
-    if test_size is not None:
-        total = test_size
-    else:
-        total = len(data_loader)
+    total = len(data_loader)
 
     with torch.no_grad():
-        for epoch, (images, labels) in enumerate(data_loader):
+        for batch, (images, labels) in enumerate(data_loader):
             log.debug(
                 "Validate #{}/{} {}".format(
-                    epoch + 1,
+                    batch + 1,
                     total,
                     {
                         "loss": losses.avg,
                         "top1": top1.avg,
                         "top5": top5.avg,
                         "img_size": images.size(2),
                     },
@@ -105,16 +101,15 @@
 
             loss = test_criterion(output, labels)
             acc1, acc5 = accuracy(output, labels, topk=(1, 5))
 
             losses.update(loss.item(), images.size(0))
             top1.update(acc1, images.size(0))
             top5.update(acc5, images.size(0))
-            if epoch + 1 >= total:
-                break
+
     return losses.avg, top1.avg, top5.avg
 
 
 def get_parameters(
     model: nn.Module,
     device: str = 'cpu',
 ) -> int:
```

### Comparing `dynast-1.2.0rc2/dynast/utils/reference.py` & `dynast-1.3.0rc1/dynast/utils/reference.py`

 * *Files 3% similar despite different names*

```diff
@@ -94,25 +94,25 @@
 
     @measure_time
     def validate(
         self,
         device: str = 'cpu',
         batch_size: int = 128,
         input_size: int = 224,
-        test_size: int = None,
+        test_fraction: float = 1.0,
     ) -> Tuple[float, float, float]:
         model = self.model.to(device)
         loss, top1, top5 = validate_classification(
             model=model,
             device=device,
             data_loader=self.dataset.validation_dataloader(
                 batch_size=batch_size,
                 image_size=input_size,
+                fraction=test_fraction,
             ),
-            test_size=test_size,
         )
         log.info(
             '\'{model_name}\' on \'{dataset_name}\' - top1 {top1} top5 {top5} loss {loss}'.format(
                 model_name=self.model_name,
                 dataset_name=self.dataset.name(),
                 top1=top1,
                 top5=top5,
```

### Comparing `dynast-1.2.0rc2/dynast.egg-info/PKG-INFO` & `dynast-1.3.0rc1/dynast.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dynast
-Version: 1.2.0rc2
+Version: 1.3.0rc1
 Summary: DyNAS-T (Dynamic Neural Architecture Search Toolkit) - a SuperNet NAS optimization package
 Author: Maciej Szankin, Sharath Nittur Sridhar, Anthony Sarah, Sairam Sundaresan
 Author-email: maciej.szankin@intel.com, sharath.nittur.sridhar@intel.com, anthony.sarah@intel.com, sairam.sundaresan@intel.com
 License: Apache 2.0
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
```

### Comparing `dynast-1.2.0rc2/dynast.egg-info/SOURCES.txt` & `dynast-1.3.0rc1/dynast.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/setup.py` & `dynast-1.3.0rc1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # import datetime
 
 from setuptools import find_packages, setup
 
 
 def get_version():
     # TODO(macsz) Replace with __version__
-    return '1.2.0rc2'
+    return '1.3.0rc1'
 
 
 def get_dependencies():
     deps = []
     with open('requirements.txt') as f:
         lines = f.readlines()
         for line in lines:
```

### Comparing `dynast-1.2.0rc2/tests/__init__.py` & `dynast-1.3.0rc1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/tests/checks/__init__.py` & `dynast-1.3.0rc1/tests/checks/__init__.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/tests/checks/check_license.py` & `dynast-1.3.0rc1/tests/checks/check_license.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/tests/checks/helpers.py` & `dynast-1.3.0rc1/tests/checks/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     '.tox',
     'dist',
     '.git',
     'htmlcov',
     'log_dir',
     '.idea',
     '.venv',
+    'build',
 ]
 
 
 def get_python_files(root_dir, exclude_files=None):
     if not exclude_files:
         exclude_files = []
```

### Comparing `dynast-1.2.0rc2/tests/functional_reference.py` & `dynast-1.3.0rc1/tests/functional_reference.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/tests/test_cache.py` & `dynast-1.3.0rc1/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/tests/test_datasets.py` & `dynast-1.3.0rc1/tests/test_datasets.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import os
+
 import pytest
 
 from dynast.utils.datasets import CIFAR10, Dataset, ImageNet, Imagenette
 
 
 def test_dataset_get_by_valid_name():
     valid_dataset_names = [
@@ -33,7 +35,21 @@
 
 
 def test_dataset_invalid_name_exception():
     invalid_dataset_name = "fancy_dataset"
 
     with pytest.raises(Exception):
         Dataset.get(invalid_dataset_name)
+
+
+@pytest.mark.skipif(
+    os.path.exists(not "/datasets/imagenet-ilsvrc2012/val"),
+    reason="ImageNet dataset not found; skipping test (TODO(macsz) should be mocked in the future!)",
+)
+def test_dataset_test_fraction():
+    ImageNet.PATH = "/datasets/imagenet-ilsvrc2012/"
+    dataset = ImageNet()
+    bs = 128
+    imagenet_val_steps = 50000 // bs
+    assert len(dataset.validation_dataloader(bs, fraction=1.0)) == imagenet_val_steps
+    assert len(dataset.validation_dataloader(bs, fraction=0.0)) == imagenet_val_steps
+    assert len(dataset.validation_dataloader(bs, fraction=0.2)) == imagenet_val_steps // 5
```

### Comparing `dynast-1.2.0rc2/tests/test_dynast_manager.py` & `dynast-1.3.0rc1/tests/test_dynast_manager.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/tests/test_nn.py` & `dynast-1.3.0rc1/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/tests/test_utils.py` & `dynast-1.3.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dynast-1.2.0rc2/tests/test_utils_distributed.py` & `dynast-1.3.0rc1/tests/test_utils_distributed.py`

 * *Files identical despite different names*

