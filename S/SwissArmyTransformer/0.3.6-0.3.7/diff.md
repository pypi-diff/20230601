# Comparing `tmp/SwissArmyTransformer-0.3.6.tar.gz` & `tmp/SwissArmyTransformer-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SwissArmyTransformer-0.3.6.tar", last modified: Wed May 17 07:48:01 2023, max compression
+gzip compressed data, was "/home/mingding/SwissArmyTransformer/dist/.tmp-txtcgohx/SwissArmyTransformer-0.3.7.tar", last modified: Thu Jun  1 06:56:48 2023, max compression
```

## Comparing `SwissArmyTransformer-0.3.6.tar` & `SwissArmyTransformer-0.3.7.tar`

### file list

```diff
@@ -1,148 +1,149 @@
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.265412 SwissArmyTransformer-0.3.6/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.3.6/LICENSE
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      125 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/MANIFEST.in
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-05-17 07:48:01.265412 SwissArmyTransformer-0.3.6/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9410 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/README.md
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.249413 SwissArmyTransformer-0.3.6/SwissArmyTransformer.egg-info/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-05-17 07:48:01.000000 SwissArmyTransformer-0.3.6/SwissArmyTransformer.egg-info/PKG-INFO
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4188 2023-05-17 07:48:01.000000 SwissArmyTransformer-0.3.6/SwissArmyTransformer.egg-info/SOURCES.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-05-17 07:48:01.000000 SwissArmyTransformer-0.3.6/SwissArmyTransformer.egg-info/dependency_links.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       84 2023-05-17 07:48:01.000000 SwissArmyTransformer-0.3.6/SwissArmyTransformer.egg-info/requires.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-05-17 07:48:01.000000 SwissArmyTransformer-0.3.6/SwissArmyTransformer.egg-info/top_level.txt
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       83 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/requirements.txt
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.249413 SwissArmyTransformer-0.3.6/sat/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      433 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24930 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/arguments.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.249413 SwissArmyTransformer-0.3.6/sat/data_utils/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/data_utils/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15315 2023-05-14 16:32:50.000000 SwissArmyTransformer-0.3.6/sat/data_utils/configure_data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3720 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/data_utils/datasets.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.3.6/sat/data_utils/hf_dataset.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/data_utils/samplers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.253413 SwissArmyTransformer-0.3.6/sat/generation/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/generation/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5998 2023-05-14 16:34:09.000000 SwissArmyTransformer-0.3.6/sat/generation/autoregressive_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/generation/cuda2d_sampling.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/generation/magnify.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.253413 SwissArmyTransformer-0.3.6/sat/generation/sampling_strategies/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/generation/sampling_strategies/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3782 2023-05-15 19:21:25.000000 SwissArmyTransformer-0.3.6/sat/generation/sampling_strategies/base_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7377 2023-05-15 19:45:51.000000 SwissArmyTransformer-0.3.6/sat/generation/sampling_strategies/beam_search_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.3.6/sat/generation/utils.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5187 2023-05-16 12:24:16.000000 SwissArmyTransformer-0.3.6/sat/helpers.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.253413 SwissArmyTransformer-0.3.6/sat/model/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      214 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/model/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13873 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/model/base_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1753 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/cached_autoregressive_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5479 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/model/encoder_decoder_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.253413 SwissArmyTransformer-0.3.6/sat/model/finetune/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/finetune/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/finetune/adapter.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/finetune/ffadd.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/finetune/lora.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7648 2023-05-09 11:55:50.000000 SwissArmyTransformer-0.3.6/sat/model/finetune/lora_mixin.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/finetune/mlp_head.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/finetune/prompt_tuning.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      367 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/mixins.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.253413 SwissArmyTransformer-0.3.6/sat/model/official/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      598 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1882 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/bert_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/cait_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    12358 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/model/official/chatglm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7294 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/model/official/clip_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9612 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/model/official/cuda2d_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/distill_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/dpr_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.3.6/sat/model/official/eva2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    13912 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/model/official/glm130B_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.6/sat/model/official/glm_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/gpt2_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/gptneo_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/mae_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/roberta_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/t5_model.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     8013 2023-04-23 13:57:58.000000 SwissArmyTransformer-0.3.6/sat/model/official/vit_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/official/yolos_model.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.253413 SwissArmyTransformer-0.3.6/sat/model/position_embedding/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/position_embedding/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5402 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/model/position_embedding/rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/position_embedding/sincos2d.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-05-16 18:46:06.000000 SwissArmyTransformer-0.3.6/sat/model/position_embedding/vision_rotary_embeddings.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      819 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/model/registry.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    27066 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/model/transformer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.253413 SwissArmyTransformer-0.3.6/sat/mpu/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2216 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/mpu/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/mpu/cross_entropy.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/mpu/data.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4926 2023-05-16 13:17:56.000000 SwissArmyTransformer-0.3.6/sat/mpu/initialize.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14251 2023-05-16 05:12:03.000000 SwissArmyTransformer-0.3.6/sat/mpu/layers.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/mpu/mappings.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3483 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/mpu/utils.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.257413 SwissArmyTransformer-0.3.6/sat/ops/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      264 2023-05-14 15:42:12.000000 SwissArmyTransformer-0.3.6/sat/ops/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/ops/layernorm.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/ops/local_attention_function.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-05-14 16:02:16.000000 SwissArmyTransformer-0.3.6/sat/ops/scaled_mask_softmax.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.257413 SwissArmyTransformer-0.3.6/sat/quantization/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       29 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.6/sat/quantization/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    18674 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.6/sat/quantization/kernels.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.257413 SwissArmyTransformer-0.3.6/sat/resources/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/resources/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2522 2023-05-14 16:44:58.000000 SwissArmyTransformer-0.3.6/sat/resources/download.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2881 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/resources/urls.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.257413 SwissArmyTransformer-0.3.6/sat/tokenization/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.3.6/sat/tokenization/__init__.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.257413 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/templates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/unified_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.257413 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/vqvae/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/vqvae/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/vqvae/api.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/vqvae/vqvae_zc.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/cogview/vqvae_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.249413 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.257413 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/chinese_sentencepiece/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.261412 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.261412 SwissArmyTransformer-0.3.6/sat/tokenization/glm/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/glm/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/glm/sp_tokenizer.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/glm/tokenization.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/glm/tokenization_gpt2.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/glm/tokenization_wordpiece.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/hf_tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.261412 SwissArmyTransformer-0.3.6/sat/tokenization/icetk_glm_130B/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/icetk_glm_130B/__init__.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/tokenization/icetk_glm_130B/tokenizer.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.265412 SwissArmyTransformer-0.3.6/sat/training/
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/training/__init__.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23052 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/training/deepspeed_training.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/training/deepspeed_zero0.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/training/deepspeed_zero1.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/sat/training/deepspeed_zero2.json
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.3.6/sat/training/learning_rates.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)    10019 2023-05-14 16:37:56.000000 SwissArmyTransformer-0.3.6/sat/training/model_io.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.3.6/sat/training/utils.py
--rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7072 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.6/sat/transformer_defaults.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-05-17 07:48:01.265412 SwissArmyTransformer-0.3.6/setup.cfg
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-05-17 07:45:58.000000 SwissArmyTransformer-0.3.6/setup.py
-drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:48:01.265412 SwissArmyTransformer-0.3.6/tests/
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/tests/test_base_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.6/tests/test_inference.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.6/tests/test_list_info.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.6/tests/test_nested_model.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.6/tests/test_train.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-17 07:43:42.000000 SwissArmyTransformer-0.3.6/tests/test_train_dp.py
--rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.6/tests/test_train_nested.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.333936 SwissArmyTransformer-0.3.7/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    11338 2023-04-06 14:24:30.000000 SwissArmyTransformer-0.3.7/LICENSE
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      125 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/MANIFEST.in
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-06-01 06:56:48.333936 SwissArmyTransformer-0.3.7/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9410 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/README.md
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9782 2023-06-01 06:56:48.000000 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/PKG-INFO
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4203 2023-06-01 06:56:48.000000 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        1 2023-06-01 06:56:48.000000 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       84 2023-06-01 06:56:48.000000 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/requires.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)        4 2023-06-01 06:56:48.000000 SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/top_level.txt
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       83 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/requirements.txt
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      433 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    24867 2023-05-27 05:04:41.000000 SwissArmyTransformer-0.3.7/sat/arguments.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/data_utils/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      288 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/data_utils/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    15315 2023-05-14 16:32:50.000000 SwissArmyTransformer-0.3.7/sat/data_utils/configure_data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3720 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/data_utils/datasets.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1894 2023-05-14 16:34:50.000000 SwissArmyTransformer-0.3.7/sat/data_utils/hf_dataset.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7028 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/data_utils/samplers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/generation/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/generation/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5998 2023-05-14 16:34:09.000000 SwissArmyTransformer-0.3.7/sat/generation/autoregressive_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3218 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/generation/cuda2d_sampling.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1709 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/generation/magnify.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      161 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4025 2023-05-27 05:35:24.000000 SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/base_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7377 2023-05-15 19:45:51.000000 SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/beam_search_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2270 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/iterative_entfilter_strategy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3201 2023-04-28 08:57:23.000000 SwissArmyTransformer-0.3.7/sat/generation/utils.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5187 2023-05-16 12:24:16.000000 SwissArmyTransformer-0.3.7/sat/helpers.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/model/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      214 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13873 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/base_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1753 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/cached_autoregressive_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5479 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/encoder_decoder_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.313936 SwissArmyTransformer-0.3.7/sat/model/finetune/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      187 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2659 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/adapter.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2019 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/ffadd.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3879 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/lora.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    13473 2023-06-01 06:34:25.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/lora2.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1110 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/mlp_head.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1604 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/finetune/prompt_tuning.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      367 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/mixins.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/model/official/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      598 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1882 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/bert_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    10409 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/cait_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    12358 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/official/chatglm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7294 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/official/clip_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     9612 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/official/cuda2d_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1310 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/distill_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3942 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/dpr_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     7369 2023-05-14 14:59:40.000000 SwissArmyTransformer-0.3.7/sat/model/official/eva2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    13912 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/official/glm130B_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3751 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.7/sat/model/official/glm_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     3488 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/gpt2_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4648 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/gptneo_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     8336 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/mae_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      262 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/roberta_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14715 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/t5_model.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     6254 2023-05-27 05:12:45.000000 SwissArmyTransformer-0.3.7/sat/model/official/vit_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2969 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/official/yolos_model.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/model/position_embedding/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      296 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/position_embedding/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5402 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/position_embedding/rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/position_embedding/sincos2d.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     5021 2023-05-16 18:46:06.000000 SwissArmyTransformer-0.3.7/sat/model/position_embedding/vision_rotary_embeddings.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      819 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/model/registry.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    27066 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/model/transformer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/mpu/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2216 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/mpu/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4716 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/mpu/cross_entropy.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4018 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/mpu/data.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4926 2023-05-16 13:17:56.000000 SwissArmyTransformer-0.3.7/sat/mpu/initialize.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    14251 2023-05-16 05:12:03.000000 SwissArmyTransformer-0.3.7/sat/mpu/layers.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4136 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/mpu/mappings.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3483 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/mpu/utils.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/ops/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      264 2023-05-14 15:42:12.000000 SwissArmyTransformer-0.3.7/sat/ops/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1159 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/ops/layernorm.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2067 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/ops/local_attention_function.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      389 2023-05-14 16:02:16.000000 SwissArmyTransformer-0.3.7/sat/ops/scaled_mask_softmax.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/quantization/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       29 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.7/sat/quantization/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    18674 2023-05-16 09:41:04.000000 SwissArmyTransformer-0.3.7/sat/quantization/kernels.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/resources/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       33 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/resources/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2522 2023-05-14 16:44:58.000000 SwissArmyTransformer-0.3.7/sat/resources/download.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2881 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/resources/urls.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.317936 SwissArmyTransformer-0.3.7/sat/tokenization/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3810 2023-05-14 16:27:55.000000 SwissArmyTransformer-0.3.7/sat/tokenization/__init__.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.321936 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      303 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     5092 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1767 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/templates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7095 2023-05-14 16:38:45.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/unified_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.321936 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      167 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7691 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/api.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    30392 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/vqvae_diffusion.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    12917 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/vqvae_zc.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     2453 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.309936 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.325935 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/chinese_sentencepiece/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1021864 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   723078 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.329936 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   231508 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)  1042301 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   456318 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)   898823 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.329936 SwissArmyTransformer-0.3.7/sat/tokenization/glm/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)       87 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/glm/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3272 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/glm/sp_tokenizer.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23223 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    13844 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization_gpt2.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)    14571 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization_wordpiece.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3271 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/hf_tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.329936 SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       40 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/__init__.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     9661 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/ice_tokenizer.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2295 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/tokenizer.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.329936 SwissArmyTransformer-0.3.7/sat/training/
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/training/__init__.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    23052 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/training/deepspeed_training.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      354 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/training/deepspeed_zero0.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)      970 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/training/deepspeed_zero1.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     1029 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/sat/training/deepspeed_zero2.json
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     3475 2023-05-14 16:38:27.000000 SwissArmyTransformer-0.3.7/sat/training/learning_rates.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)    10019 2023-05-14 16:37:56.000000 SwissArmyTransformer-0.3.7/sat/training/model_io.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     4488 2023-05-14 16:28:13.000000 SwissArmyTransformer-0.3.7/sat/training/utils.py
+-rwxrwxr-x   0 mingding  (1001) mingding  (1001)     7072 2023-05-17 07:45:01.000000 SwissArmyTransformer-0.3.7/sat/transformer_defaults.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)       38 2023-06-01 06:56:48.333936 SwissArmyTransformer-0.3.7/setup.cfg
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      880 2023-06-01 06:38:59.000000 SwissArmyTransformer-0.3.7/setup.py
+drwxrwxr-x   0 mingding  (1001) mingding  (1001)        0 2023-06-01 06:56:48.329936 SwissArmyTransformer-0.3.7/tests/
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2000 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/tests/test_base_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     1530 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.7/tests/test_inference.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      290 2023-04-21 12:58:30.000000 SwissArmyTransformer-0.3.7/tests/test_list_info.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     2134 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.7/tests/test_nested_model.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)      611 2023-05-18 18:05:46.000000 SwissArmyTransformer-0.3.7/tests/test_speed.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-04-21 12:58:44.000000 SwissArmyTransformer-0.3.7/tests/test_train.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4078 2023-05-17 07:43:42.000000 SwissArmyTransformer-0.3.7/tests/test_train_dp.py
+-rw-rw-r--   0 mingding  (1001) mingding  (1001)     4336 2023-05-10 18:09:38.000000 SwissArmyTransformer-0.3.7/tests/test_train_nested.py
```

### Comparing `SwissArmyTransformer-0.3.6/LICENSE` & `SwissArmyTransformer-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/PKG-INFO` & `SwissArmyTransformer-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.3.6
+Version: 0.3.7
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.3.6/README.md` & `SwissArmyTransformer-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/SwissArmyTransformer.egg-info/PKG-INFO` & `SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SwissArmyTransformer
-Version: 0.3.6
+Version: 0.3.7
 Summary: A transformer-based framework with finetuning as the first class citizen.
 Home-page: https://github.com/THUDM/SwissArmyTransformer
 Author: Ming Ding, et al.
 Author-email: dm_thu@qq.com
 License: Apache 2.0 license
 Requires-Python: >=3.5
 Description-Content-Type: text/markdown
```

### Comparing `SwissArmyTransformer-0.3.6/SwissArmyTransformer.egg-info/SOURCES.txt` & `SwissArmyTransformer-0.3.7/SwissArmyTransformer.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 sat/model/mixins.py
 sat/model/registry.py
 sat/model/transformer.py
 sat/model/finetune/__init__.py
 sat/model/finetune/adapter.py
 sat/model/finetune/ffadd.py
 sat/model/finetune/lora.py
-sat/model/finetune/lora_mixin.py
+sat/model/finetune/lora2.py
 sat/model/finetune/mlp_head.py
 sat/model/finetune/prompt_tuning.py
 sat/model/official/__init__.py
 sat/model/official/bert_model.py
 sat/model/official/cait_model.py
 sat/model/official/chatglm_model.py
 sat/model/official/clip_model.py
@@ -113,10 +113,11 @@
 sat/training/learning_rates.py
 sat/training/model_io.py
 sat/training/utils.py
 tests/test_base_model.py
 tests/test_inference.py
 tests/test_list_info.py
 tests/test_nested_model.py
+tests/test_speed.py
 tests/test_train.py
 tests/test_train_dp.py
 tests/test_train_nested.py
```

### Comparing `SwissArmyTransformer-0.3.6/sat/arguments.py` & `SwissArmyTransformer-0.3.7/sat/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -424,16 +424,15 @@
         config = json.load(f)
     # expand relative path
     folder = os.path.dirname(path)
     for k in config:
         # all the relative paths in config are based on the folder
         if k.endswith('_path'): 
             config[k] = os.path.join(folder, config[k])
-            if args.rank == 0:
-                print_rank0(f'> parsing relative path {k} in model_config as {config[k]}.')
+            print_rank0(f'> parsing relative path {k} in model_config as {config[k]}.')
     args = vars(args)
     for k in list(args.keys()):
         if k in config:
             del args[k]
     args = argparse.Namespace(**config, **args)
     return args
 
@@ -481,15 +480,14 @@
     
     if args.world_size == 1:
         from sat.helpers import get_free_port
         default_master_port = str(get_free_port())
     else:
         default_master_port = '6000'
     args.master_port = os.getenv('MASTER_PORT', default_master_port)
-    print(args.master_port)
     init_method += args.master_ip + ':' + args.master_port
     torch.distributed.init_process_group(
         backend=args.distributed_backend,
         world_size=args.world_size, rank=args.rank,
         init_method=init_method)
 
     # Set the model-parallel / data-parallel communicators.
```

### Comparing `SwissArmyTransformer-0.3.6/sat/data_utils/configure_data.py` & `SwissArmyTransformer-0.3.7/sat/data_utils/configure_data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/data_utils/datasets.py` & `SwissArmyTransformer-0.3.7/sat/data_utils/datasets.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/data_utils/hf_dataset.py` & `SwissArmyTransformer-0.3.7/sat/data_utils/hf_dataset.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/data_utils/samplers.py` & `SwissArmyTransformer-0.3.7/sat/data_utils/samplers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/generation/autoregressive_sampling.py` & `SwissArmyTransformer-0.3.7/sat/generation/autoregressive_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/generation/cuda2d_sampling.py` & `SwissArmyTransformer-0.3.7/sat/generation/cuda2d_sampling.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/generation/magnify.py` & `SwissArmyTransformer-0.3.7/sat/generation/magnify.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/generation/sampling_strategies/base_strategy.py` & `SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/base_strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import os
 import sys
 import math
 import random
 import torch
 import torch.nn.functional as F
 
-
 def top_k_logits(logits, top_k=0, top_p=0.0, filter_value=-65504):
     # This function has been mostly taken from huggingface conversational ai code at
     # https://medium.com/huggingface/how-to-build-a-state-of-the-art-conversational-ai-with-transfer-learning-2d818ac26313
 
     if top_k > 0:
         # Remove all tokens with a probability less than the last token of the top-k
         indices_to_remove = logits < torch.topk(logits, top_k)[0][..., -1, None]
@@ -64,20 +63,24 @@
         self._is_done = False
         self.context_length = None
 
     @property
     def is_done(self) -> bool:
         return self._is_done
 
-    def forward(self, logits, tokens, mems, temperature=None):
+    def forward(self, logits, tokens, mems, temperature=None, nan_default_token=None):
         if self.context_length is None:
             self.context_length = tokens.shape[-1]
         if temperature is None:
             temperature = self.temperature
-        # logits = logits.float() / temperature
+        if torch.isnan(logits).any():
+            if nan_default_token is None:
+                raise ValueError('nan in logits, set nan_default_token to proceed in BaseStrategy.forward.')
+            logits.fill_(-1000)
+            logits[..., nan_default_token] = 0
         # apply repetition penalty
         penalty_mat = torch.ones_like(logits).float()
         if tokens.shape[-1]> self.context_length:
             penalty_mat.scatter_(1, 
             tokens[:, self.context_length:], torch.ones_like(tokens[:, self.context_length:]).float() * self.repetition_penalty)
         penalty_mat *= temperature
         logits = logits.float() / penalty_mat
```

### Comparing `SwissArmyTransformer-0.3.6/sat/generation/sampling_strategies/beam_search_strategy.py` & `SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/beam_search_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/generation/sampling_strategies/iterative_entfilter_strategy.py` & `SwissArmyTransformer-0.3.7/sat/generation/sampling_strategies/iterative_entfilter_strategy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/generation/utils.py` & `SwissArmyTransformer-0.3.7/sat/generation/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/helpers.py` & `SwissArmyTransformer-0.3.7/sat/helpers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/base_model.py` & `SwissArmyTransformer-0.3.7/sat/model/base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/cached_autoregressive_model.py` & `SwissArmyTransformer-0.3.7/sat/model/cached_autoregressive_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/encoder_decoder_model.py` & `SwissArmyTransformer-0.3.7/sat/model/encoder_decoder_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/finetune/adapter.py` & `SwissArmyTransformer-0.3.7/sat/model/finetune/adapter.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/finetune/ffadd.py` & `SwissArmyTransformer-0.3.7/sat/model/finetune/ffadd.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/finetune/lora.py` & `SwissArmyTransformer-0.3.7/sat/model/finetune/lora.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/finetune/mlp_head.py` & `SwissArmyTransformer-0.3.7/sat/model/finetune/mlp_head.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/finetune/prompt_tuning.py` & `SwissArmyTransformer-0.3.7/sat/model/finetune/prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/__init__.py` & `SwissArmyTransformer-0.3.7/sat/model/official/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/bert_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/bert_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/cait_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/cait_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/chatglm_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/chatglm_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/clip_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/clip_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/cuda2d_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/cuda2d_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/distill_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/distill_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/dpr_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/dpr_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/eva2_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/eva2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/glm130B_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/glm130B_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/glm_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/glm_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/gpt2_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/gpt2_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/gptneo_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/gptneo_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/mae_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/mae_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/t5_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/t5_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/vit_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/vit_model.py`

 * *Files 20% similar despite different names*

```diff
@@ -36,67 +36,34 @@
         self.post_len = post_len
         self.seq_len = self.pre_len + self.num_patches + self.post_len
 
 
 class ImagePatchEmbeddingMixin(BaseMixin):
     def __init__(self, in_channels, hidden_size, property):
         super(ImagePatchEmbeddingMixin, self).__init__()
-        self.property = property
         self.proj = nn.Conv2d(in_channels, hidden_size, kernel_size=property.patch_size, stride=property.patch_size)
 
     def word_embedding_forward(self, input_ids, **kwargs):
         """
         Input:
         * input_ids with shape (batch_size, pre_len+post_len)
         * kwargs["image"] with shape (B, C, H, W)
         Output:
         * (batch_size, hidden_size)
         """
         images = kwargs["image"]
         embeddings = self.proj(images)
         embeddings = embeddings.flatten(2).transpose(1, 2)
-        pre_word_embeddings = self.transformer.word_embeddings(input_ids[:,:self.property.pre_len])
-        post_word_embeddings = self.transformer.word_embeddings(input_ids[:,self.property.pre_len:self.property.pre_len+self.property.post_len])
+        pre_word_embeddings = self.transformer.word_embeddings(input_ids[:,:self.transformer.property.pre_len])
+        post_word_embeddings = self.transformer.word_embeddings(input_ids[:,self.transformer.property.pre_len:self.transformer.property.pre_len+self.transformer.property.post_len])
         embeddings = torch.cat([pre_word_embeddings, embeddings, post_word_embeddings], dim=1)
         return embeddings
 
 
 class InterpolatedPositionEmbeddingMixin(BaseMixin):
-    def __init__(self, property, init_method_std=0.02):
-        super(InterpolatedPositionEmbeddingMixin, self).__init__()
-        self.property = property
-        self.init_method_std = init_method_std
-
-    def interpolate_pos_encoding(self, height, width):
-        """
-        Adapted from https://github.com/huggingface/transformers/blob/master/src/transformers/models/vit/modeling_vit.py#L79
-        This method allows to interpolate the pre-trained position encodings, to be able to use the model on higher
-        resolution images.
-        Source:
-        https://github.com/facebookresearch/dino/blob/de9ee3df6cf39fac952ab558447af1fa1365362a/vision_transformer.py#L174
-        """
-        pre_pos_embed = self.transformer.position_embeddings.weight[:self.property.pre_len]
-        patch_pos_embed = self.transformer.position_embeddings.weight[self.property.pre_len:self.property.pre_len+self.property.num_patches]
-        post_pos_embed = self.transformer.position_embeddings.weight[self.property.pre_len+self.property.num_patches:]
-        dim = self.transformer.position_embeddings.weight.shape[-1]
-        h0 = height
-        w0 = width
-        # we add a small number to avoid floating point error in the interpolation
-        # see discussion at https://github.com/facebookresearch/dino/issues/8
-        h0, w0 = h0 + 0.1, w0 + 0.1
-        patch_pos_embed = F.interpolate(
-            patch_pos_embed.reshape(1, self.property.grid_size[0], self.property.grid_size[1], dim).permute(0, 3, 1, 2),
-            scale_factor=(h0 / self.property.grid_size[0], w0 / self.property.grid_size[1]),
-            mode="bicubic",
-            align_corners=False,
-        )
-        assert int(h0) == patch_pos_embed.shape[-2] and int(w0) == patch_pos_embed.shape[-1]
-        patch_pos_embed = patch_pos_embed.permute(0, 2, 3, 1).view(-1, dim)
-        return torch.cat((pre_pos_embed, patch_pos_embed, post_pos_embed), dim=0)
-    
     def position_embedding_forward(self, position_ids, **kwargs):
         """
         There are two modes for position_embedding:
         * offline mode: You have reinited position_embeddings to a pre-defined new seq_len.
         * online mode: You need to interpolate position_embeddings for every forward pass.
 
         Input:
@@ -108,24 +75,24 @@
 
     def reinit(self, parent_model=None, property=None):
         """
         new pre_len, new num_patches and new post_len should all be larger or equal than the old ones.
         """
         assert property is not None
         old_weight = self.transformer.position_embeddings.weight.data
-        pre_weight = old_weight[:self.property.pre_len]
-        post_weight = old_weight[self.property.pre_len+self.property.num_patches:]
-        image_weight = old_weight[self.property.pre_len:self.property.pre_len+self.property.num_patches].reshape(1, self.property.grid_size[0], self.property.grid_size[1], -1).permute(0, 3, 1, 2)
+        pre_weight = old_weight[:self.transformer.property.pre_len]
+        post_weight = old_weight[self.transformer.property.pre_len+self.transformer.property.num_patches:]
+        image_weight = old_weight[self.transformer.property.pre_len:self.transformer.property.pre_len+self.transformer.property.num_patches].reshape(1, self.transformer.property.grid_size[0], self.transformer.property.grid_size[1], -1).permute(0, 3, 1, 2)
         image_weight = F.interpolate(image_weight, size=property.grid_size, mode='bicubic', align_corners=False).permute(0, 2, 3, 1).reshape(property.num_patches, -1)
         self.transformer.position_embeddings = torch.nn.Embedding(property.seq_len, old_weight.shape[1]).type(old_weight.dtype).to(old_weight.device)
-        torch.nn.init.normal_(self.transformer.position_embeddings.weight, mean=0.0, std=self.init_method_std)
-        self.transformer.position_embeddings.weight.data[:self.property.pre_len] = pre_weight
+        torch.nn.init.normal_(self.transformer.position_embeddings.weight, mean=0.0, std=0.02)
+        self.transformer.position_embeddings.weight.data[:self.transformer.property.pre_len] = pre_weight
         self.transformer.position_embeddings.weight.data[property.pre_len:property.pre_len+property.num_patches] = image_weight
-        self.transformer.position_embeddings.weight.data[property.pre_len+property.num_patches:property.pre_len+property.num_patches+self.property.post_len] = post_weight
-        self.property = property
+        self.transformer.position_embeddings.weight.data[property.pre_len+property.num_patches:property.pre_len+property.num_patches+self.transformer.property.post_len] = post_weight
+        self.transformer.property = property
 
 
 class ClsMixin(BaseMixin):
     def __init__(self, hidden_size, num_classes):
         super().__init__()
         self.classifier = nn.Linear(hidden_size, num_classes)
 
@@ -137,16 +104,17 @@
 class ViTModel(BaseModel):
     def __init__(self, args, transformer=None, parallel_output=True, **kwargs):
         property = ViTProperty(args.image_size, args.patch_size, args.pre_len, args.post_len)
         args.max_sequence_length = property.pre_len + property.num_patches + property.post_len
         if 'activation_func' not in kwargs:
             kwargs['activation_func'] = gelu
         super().__init__(args, transformer=transformer, parallel_output=parallel_output, **kwargs)
+        self.transformer.property = property
         self.add_mixin("patch_embedding", ImagePatchEmbeddingMixin(args.in_channels, args.hidden_size, property))
-        self.add_mixin("pos_embedding", InterpolatedPositionEmbeddingMixin(property))
+        self.add_mixin("pos_embedding", InterpolatedPositionEmbeddingMixin())
         self.add_mixin("cls", ClsMixin(args.hidden_size, args.num_classes))
 
     @classmethod
     def add_model_specific_args(cls, parser):
         group = parser.add_argument_group('ViT', 'ViT Configurations')
         group.add_argument('--image-size', nargs='+', type=int, default=[224, 224])
         group.add_argument('--pre-len', type=int, default=1) # [cls] by default
```

### Comparing `SwissArmyTransformer-0.3.6/sat/model/official/yolos_model.py` & `SwissArmyTransformer-0.3.7/sat/model/official/yolos_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/position_embedding/rotary_embeddings.py` & `SwissArmyTransformer-0.3.7/sat/model/position_embedding/rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/position_embedding/sincos2d.py` & `SwissArmyTransformer-0.3.7/sat/model/position_embedding/sincos2d.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/position_embedding/vision_rotary_embeddings.py` & `SwissArmyTransformer-0.3.7/sat/model/position_embedding/vision_rotary_embeddings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/registry.py` & `SwissArmyTransformer-0.3.7/sat/model/registry.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/model/transformer.py` & `SwissArmyTransformer-0.3.7/sat/model/transformer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/mpu/__init__.py` & `SwissArmyTransformer-0.3.7/sat/mpu/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/mpu/cross_entropy.py` & `SwissArmyTransformer-0.3.7/sat/mpu/cross_entropy.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/mpu/data.py` & `SwissArmyTransformer-0.3.7/sat/mpu/data.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/mpu/initialize.py` & `SwissArmyTransformer-0.3.7/sat/mpu/initialize.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/mpu/layers.py` & `SwissArmyTransformer-0.3.7/sat/mpu/layers.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/mpu/mappings.py` & `SwissArmyTransformer-0.3.7/sat/mpu/mappings.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/mpu/utils.py` & `SwissArmyTransformer-0.3.7/sat/mpu/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/ops/layernorm.py` & `SwissArmyTransformer-0.3.7/sat/ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/ops/local_attention_function.py` & `SwissArmyTransformer-0.3.7/sat/ops/local_attention_function.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/quantization/kernels.py` & `SwissArmyTransformer-0.3.7/sat/quantization/kernels.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/resources/download.py` & `SwissArmyTransformer-0.3.7/sat/resources/download.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/resources/urls.py` & `SwissArmyTransformer-0.3.7/sat/resources/urls.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/__init__.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/cogview/sp_tokenizer.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/cogview/templates.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/templates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/cogview/unified_tokenizer.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/unified_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/cogview/vqvae/api.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/api.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/cogview/vqvae/vqvae_diffusion.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/vqvae_diffusion.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/cogview/vqvae/vqvae_zc.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae/vqvae_zc.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/cogview/vqvae_tokenizer.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/cogview/vqvae_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model` & `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.model`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab` & `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/chinese_sentencepiece/cog-pretrain.vocab`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt` & `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/bert-base-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt` & `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/bert-large-uncased-vocab.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt` & `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/gpt2-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json` & `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/gpt2-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt` & `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/roberta-merges.txt`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json` & `SwissArmyTransformer-0.3.7/sat/tokenization/embed_assets/english_tokenizer/roberta-vocab.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/glm/sp_tokenizer.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/glm/sp_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/glm/tokenization.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/glm/tokenization_gpt2.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization_gpt2.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/glm/tokenization_wordpiece.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/glm/tokenization_wordpiece.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/hf_tokenizer.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/hf_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/icetk_glm_130B/ice_tokenizer.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/ice_tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/tokenization/icetk_glm_130B/tokenizer.py` & `SwissArmyTransformer-0.3.7/sat/tokenization/icetk_glm_130B/tokenizer.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/training/deepspeed_training.py` & `SwissArmyTransformer-0.3.7/sat/training/deepspeed_training.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/training/deepspeed_zero1.json` & `SwissArmyTransformer-0.3.7/sat/training/deepspeed_zero1.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/training/deepspeed_zero2.json` & `SwissArmyTransformer-0.3.7/sat/training/deepspeed_zero2.json`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/training/learning_rates.py` & `SwissArmyTransformer-0.3.7/sat/training/learning_rates.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/training/model_io.py` & `SwissArmyTransformer-0.3.7/sat/training/model_io.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/training/utils.py` & `SwissArmyTransformer-0.3.7/sat/training/utils.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/sat/transformer_defaults.py` & `SwissArmyTransformer-0.3.7/sat/transformer_defaults.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/setup.py` & `SwissArmyTransformer-0.3.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 
 def _requirements():
     return Path("requirements.txt").read_text()
 
 setup(
     name="SwissArmyTransformer",
-    version='0.3.6',
+    version='0.3.7',
     description="A transformer-based framework with finetuning as the first class citizen.",
     long_description=Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     install_requires=_requirements(),
     entry_points={},
     packages=find_packages(),
     url="https://github.com/THUDM/SwissArmyTransformer",
```

### Comparing `SwissArmyTransformer-0.3.6/tests/test_base_model.py` & `SwissArmyTransformer-0.3.7/tests/test_base_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/tests/test_inference.py` & `SwissArmyTransformer-0.3.7/tests/test_inference.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/tests/test_nested_model.py` & `SwissArmyTransformer-0.3.7/tests/test_nested_model.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/tests/test_train.py` & `SwissArmyTransformer-0.3.7/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/tests/test_train_dp.py` & `SwissArmyTransformer-0.3.7/tests/test_train_dp.py`

 * *Files identical despite different names*

### Comparing `SwissArmyTransformer-0.3.6/tests/test_train_nested.py` & `SwissArmyTransformer-0.3.7/tests/test_train_nested.py`

 * *Files identical despite different names*

