# Comparing `tmp/dialogy-2.0.7.tar.gz` & `tmp/dialogy-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialogy-2.0.7.tar", max compression
+gzip compressed data, was "dialogy-2.0.8.tar", max compression
```

## Comparing `dialogy-2.0.7.tar` & `dialogy-2.0.8.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1069 2023-05-23 03:34:05.535176 dialogy-2.0.7/LICENSE.md
--rw-r--r--   0        0        0        0 2023-05-23 03:34:05.535176 dialogy-2.0.7/dialogy/__init__.py
--rw-r--r--   0        0        0      183 2023-05-23 03:34:05.535176 dialogy-2.0.7/dialogy/base/__init__.py
--rw-r--r--   0        0        0     4949 2023-05-23 03:34:05.535176 dialogy-2.0.7/dialogy/base/entity_extractor/__init__.py
--rw-r--r--   0        0        0     9777 2023-05-23 03:34:05.535176 dialogy-2.0.7/dialogy/base/input/__init__.py
--rw-r--r--   0        0        0     4595 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/base/output/__init__.py
--rw-r--r--   0        0        0    15685 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/base/plugin/__init__.py
--rw-r--r--   0        0        0     3908 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/cli/__init__.py
--rw-r--r--   0        0        0     2587 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/cli/project.py
--rw-r--r--   0        0        0     1865 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/cli/workflow.py
--rw-r--r--   0        0        0     5017 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/constants/__init__.py
--rw-r--r--   0        0        0     2011 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/registry.py
--rw-r--r--   0        0        0        0 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/__init__.py
--rw-r--r--   0        0        0     4001 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/address_parser/__init__.py
--rw-r--r--   0        0        0     1406 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/address_parser/mapmyindia.py
--rw-r--r--   0        0        0     4978 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/address_parser/maps.py
--rw-r--r--   0        0        0        0 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/calibration/__init__.py
--rw-r--r--   0        0        0     8880 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/calibration/xgb.py
--rw-r--r--   0        0        0     3802 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/canonicalization/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/classification/__init__.py
--rw-r--r--   0        0        0    11811 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/classification/mlp.py
--rw-r--r--   0        0        0     1185 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/classification/retain_intent.py
--rw-r--r--   0        0        0       58 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/classification/tokenizers.py
--rw-r--r--   0        0        0    16717 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/classification/xlmr.py
--rw-r--r--   0        0        0     7682 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/combine_date_time/__init__.py
--rw-r--r--   0        0        0    38996 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/duckling_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/error_recovery/__init__.py
--rw-r--r--   0        0        0    20340 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/error_recovery/error_recovery.py
--rw-r--r--   0        0        0    12306 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/__init__.py
--rw-r--r--   0        0        0      743 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
--rw-r--r--   0        0        0      797 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/const.py
--rw-r--r--   0        0        0      313 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/registry.py
--rw-r--r--   0        0        0     1804 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/lb_plugin/__init__.py
--rw-r--r--   0        0        0    14135 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/list_entity_plugin/__init__.py
--rw-r--r--   0        0        0    11529 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/list_search_plugin/__init__.py
--rw-r--r--   0        0        0     4841 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/list_search_plugin/sample_config.yaml
--rw-r--r--   0        0        0     4711 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/merge_asr_output/__init__.py
--rw-r--r--   0        0        0     3013 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/oos_filter/__init__.py
--rw-r--r--   0        0        0     4259 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/qc_plugin/__init__.py
--rw-r--r--   0        0        0      833 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/slot_filler/__init__.py
--rw-r--r--   0        0        0     4154 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/slot_filler/rule_slot_filler.py
--rw-r--r--   0        0        0        0 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/plugins/text/voting/__init__.py
--rw-r--r--   0        0        0     1862 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/__init__.py
--rw-r--r--   0        0        0      170 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/__init__.py
--rw-r--r--   0        0        0      914 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/address/__init__.py
--rw-r--r--   0        0        0     1811 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/amount_of_money/__init__.py
--rw-r--r--   0        0        0     7361 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/base_entity/__init__.py
--rw-r--r--   0        0        0     2281 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/credit_card_number/__init__.py
--rw-r--r--   0        0        0     3637 2023-05-23 03:34:05.539177 dialogy-2.0.7/dialogy/types/entity/deserialize/__init__.py
--rw-r--r--   0        0        0     4432 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/duration/__init__.py
--rw-r--r--   0        0        0      975 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/keyword/__init__.py
--rw-r--r--   0        0        0     4698 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/numerical/__init__.py
--rw-r--r--   0        0        0     2271 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/people/__init__.py
--rw-r--r--   0        0        0      910 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/pincode/__init__.py
--rw-r--r--   0        0        0    13534 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/time/__init__.py
--rw-r--r--   0        0        0     8803 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/entity/time_interval/__init__.py
--rw-r--r--   0        0        0     8893 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/intent/__init__.py
--rw-r--r--   0        0        0      154 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/signal/__init__.py
--rw-r--r--   0        0        0      194 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/signal/signal.py
--rw-r--r--   0        0        0      991 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/slots/__init__.py
--rw-r--r--   0        0        0      191 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/types/utterances/__init__.py
--rw-r--r--   0        0        0      638 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/__init__.py
--rw-r--r--   0        0        0    10660 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/config.py
--rw-r--r--   0        0        0     2180 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/datetime.py
--rw-r--r--   0        0        0     3437 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/file_handler.py
--rw-r--r--   0        0        0      808 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/logger.py
--rw-r--r--   0        0        0     2880 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/misc.py
--rw-r--r--   0        0        0      584 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/naive_lang_detect.py
--rw-r--r--   0        0        0     8236 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/normalize_utterance.py
--rw-r--r--   0        0        0     3605 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/utils/temperature_scaling.py
--rw-r--r--   0        0        0       47 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/workflow/__init__.py
--rw-r--r--   0        0        0     7069 2023-05-23 03:34:05.543177 dialogy-2.0.7/dialogy/workflow/workflow.py
--rw-r--r--   0        0        0     1536 2023-05-23 03:34:25.671321 dialogy-2.0.7/pyproject.toml
--rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 dialogy-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-01 09:12:29.521725 dialogy-2.0.8/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-06-01 09:12:29.521725 dialogy-2.0.8/dialogy/__init__.py
+-rw-r--r--   0        0        0      183 2023-06-01 09:12:29.521725 dialogy-2.0.8/dialogy/base/__init__.py
+-rw-r--r--   0        0        0     4949 2023-06-01 09:12:29.521725 dialogy-2.0.8/dialogy/base/entity_extractor/__init__.py
+-rw-r--r--   0        0        0     9777 2023-06-01 09:12:29.521725 dialogy-2.0.8/dialogy/base/input/__init__.py
+-rw-r--r--   0        0        0     4595 2023-06-01 09:12:29.521725 dialogy-2.0.8/dialogy/base/output/__init__.py
+-rw-r--r--   0        0        0    15685 2023-06-01 09:12:29.521725 dialogy-2.0.8/dialogy/base/plugin/__init__.py
+-rw-r--r--   0        0        0     3908 2023-06-01 09:12:29.521725 dialogy-2.0.8/dialogy/cli/__init__.py
+-rw-r--r--   0        0        0     2587 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/cli/project.py
+-rw-r--r--   0        0        0     1865 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/cli/workflow.py
+-rw-r--r--   0        0        0     5017 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/constants/__init__.py
+-rw-r--r--   0        0        0     2011 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/registry.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/__init__.py
+-rw-r--r--   0        0        0     4001 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/address_parser/__init__.py
+-rw-r--r--   0        0        0     1406 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/address_parser/mapmyindia.py
+-rw-r--r--   0        0        0     4978 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/address_parser/maps.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/calibration/__init__.py
+-rw-r--r--   0        0        0     8880 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/calibration/xgb.py
+-rw-r--r--   0        0        0     3802 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/canonicalization/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/classification/__init__.py
+-rw-r--r--   0        0        0    11811 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/classification/mlp.py
+-rw-r--r--   0        0        0     1185 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/classification/retain_intent.py
+-rw-r--r--   0        0        0       58 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/classification/tokenizers.py
+-rw-r--r--   0        0        0    16717 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/classification/xlmr.py
+-rw-r--r--   0        0        0     7682 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/combine_date_time/__init__.py
+-rw-r--r--   0        0        0    38996 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/duckling_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/error_recovery/__init__.py
+-rw-r--r--   0        0        0    20340 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/error_recovery/error_recovery.py
+-rw-r--r--   0        0        0    12306 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/intent_entity_mutator/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
+-rw-r--r--   0        0        0      797 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/intent_entity_mutator/const.py
+-rw-r--r--   0        0        0      313 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/intent_entity_mutator/registry.py
+-rw-r--r--   0        0        0     1804 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/lb_plugin/__init__.py
+-rw-r--r--   0        0        0    14135 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/list_entity_plugin/__init__.py
+-rw-r--r--   0        0        0    11529 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/list_search_plugin/__init__.py
+-rw-r--r--   0        0        0     4841 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/list_search_plugin/sample_config.yaml
+-rw-r--r--   0        0        0     4711 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/merge_asr_output/__init__.py
+-rw-r--r--   0        0        0     3013 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/oos_filter/__init__.py
+-rw-r--r--   0        0        0     4259 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/qc_plugin/__init__.py
+-rw-r--r--   0        0        0      833 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/slot_filler/__init__.py
+-rw-r--r--   0        0        0     4154 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/slot_filler/rule_slot_filler.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/plugins/text/voting/__init__.py
+-rw-r--r--   0        0        0     1862 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/__init__.py
+-rw-r--r--   0        0        0      170 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/address/__init__.py
+-rw-r--r--   0        0        0     1811 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/amount_of_money/__init__.py
+-rw-r--r--   0        0        0     7361 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/base_entity/__init__.py
+-rw-r--r--   0        0        0     2281 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/credit_card_number/__init__.py
+-rw-r--r--   0        0        0     3637 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/deserialize/__init__.py
+-rw-r--r--   0        0        0     4432 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/duration/__init__.py
+-rw-r--r--   0        0        0      975 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/keyword/__init__.py
+-rw-r--r--   0        0        0     4698 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/numerical/__init__.py
+-rw-r--r--   0        0        0     2271 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/people/__init__.py
+-rw-r--r--   0        0        0      910 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/pincode/__init__.py
+-rw-r--r--   0        0        0    13534 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/time/__init__.py
+-rw-r--r--   0        0        0     8803 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/entity/time_interval/__init__.py
+-rw-r--r--   0        0        0     8893 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/intent/__init__.py
+-rw-r--r--   0        0        0      154 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/signal/__init__.py
+-rw-r--r--   0        0        0      194 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/signal/signal.py
+-rw-r--r--   0        0        0      991 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/slots/__init__.py
+-rw-r--r--   0        0        0      191 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/types/utterances/__init__.py
+-rw-r--r--   0        0        0      638 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/utils/__init__.py
+-rw-r--r--   0        0        0    10969 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/utils/config.py
+-rw-r--r--   0        0        0     2180 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/utils/datetime.py
+-rw-r--r--   0        0        0     3437 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/utils/file_handler.py
+-rw-r--r--   0        0        0      808 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/utils/logger.py
+-rw-r--r--   0        0        0     2880 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/utils/misc.py
+-rw-r--r--   0        0        0      584 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/utils/naive_lang_detect.py
+-rw-r--r--   0        0        0     8236 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/utils/normalize_utterance.py
+-rw-r--r--   0        0        0     3605 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/utils/temperature_scaling.py
+-rw-r--r--   0        0        0       47 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/workflow/__init__.py
+-rw-r--r--   0        0        0     7069 2023-06-01 09:12:29.525722 dialogy-2.0.8/dialogy/workflow/workflow.py
+-rw-r--r--   0        0        0     1536 2023-06-01 09:12:46.237486 dialogy-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 dialogy-2.0.8/PKG-INFO
```

### Comparing `dialogy-2.0.7/LICENSE.md` & `dialogy-2.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/base/entity_extractor/__init__.py` & `dialogy-2.0.8/dialogy/base/entity_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/base/input/__init__.py` & `dialogy-2.0.8/dialogy/base/input/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/base/output/__init__.py` & `dialogy-2.0.8/dialogy/base/output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/base/plugin/__init__.py` & `dialogy-2.0.8/dialogy/base/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/cli/__init__.py` & `dialogy-2.0.8/dialogy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/cli/project.py` & `dialogy-2.0.8/dialogy/cli/project.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/cli/workflow.py` & `dialogy-2.0.8/dialogy/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/constants/__init__.py` & `dialogy-2.0.8/dialogy/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/registry.py` & `dialogy-2.0.8/dialogy/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/address_parser/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/address_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/address_parser/mapmyindia.py` & `dialogy-2.0.8/dialogy/plugins/text/address_parser/mapmyindia.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/address_parser/maps.py` & `dialogy-2.0.8/dialogy/plugins/text/address_parser/maps.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/calibration/xgb.py` & `dialogy-2.0.8/dialogy/plugins/text/calibration/xgb.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/canonicalization/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/canonicalization/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/classification/mlp.py` & `dialogy-2.0.8/dialogy/plugins/text/classification/mlp.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/classification/retain_intent.py` & `dialogy-2.0.8/dialogy/plugins/text/classification/retain_intent.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/classification/xlmr.py` & `dialogy-2.0.8/dialogy/plugins/text/classification/xlmr.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/combine_date_time/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/combine_date_time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/duckling_plugin/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/duckling_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/error_recovery/error_recovery.py` & `dialogy-2.0.8/dialogy/plugins/text/error_recovery/error_recovery.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/intent_entity_mutator/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py` & `dialogy-2.0.8/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/intent_entity_mutator/const.py` & `dialogy-2.0.8/dialogy/plugins/text/intent_entity_mutator/const.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/lb_plugin/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/lb_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/list_entity_plugin/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/list_entity_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/list_search_plugin/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/list_search_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/list_search_plugin/sample_config.yaml` & `dialogy-2.0.8/dialogy/plugins/text/list_search_plugin/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/merge_asr_output/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/merge_asr_output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/oos_filter/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/oos_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/qc_plugin/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/qc_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/slot_filler/__init__.py` & `dialogy-2.0.8/dialogy/plugins/text/slot_filler/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/plugins/text/slot_filler/rule_slot_filler.py` & `dialogy-2.0.8/dialogy/plugins/text/slot_filler/rule_slot_filler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/__init__.py` & `dialogy-2.0.8/dialogy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/address/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/address/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/amount_of_money/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/amount_of_money/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/base_entity/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/base_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/credit_card_number/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/credit_card_number/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/deserialize/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/deserialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/duration/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/keyword/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/numerical/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/people/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/people/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/pincode/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/pincode/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/time/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/entity/time_interval/__init__.py` & `dialogy-2.0.8/dialogy/types/entity/time_interval/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/intent/__init__.py` & `dialogy-2.0.8/dialogy/types/intent/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/types/slots/__init__.py` & `dialogy-2.0.8/dialogy/types/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/utils/__init__.py` & `dialogy-2.0.8/dialogy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/utils/config.py` & `dialogy-2.0.8/dialogy/utils/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,19 +4,23 @@
 # type: ignore
 import os
 from typing import Any, Dict, List, Optional, Set, Union
 
 import attr
 import yaml
 import glob
+from loguru import logger
+import traceback
+import sys
 
 import dialogy.constants as const
 from dialogy.utils.misc import traverse_dict
 
 
+
 class BaseConfig:
     def get(self, attribute: str) -> Any:
         # handles nested attributes
         if "." in attribute:
             levels = attribute.split(".")
             first, rest = levels[0], ".".join(levels[1:])
             first_accessed_val = vars(self).get(first)
@@ -269,23 +273,28 @@
     config = resolve_expressions(config)
     return config
 
 
 def read_project_configs(
     project_artifacts_root: str, filter_list: Optional[List[str]] = None
 ) -> Dict[str, Config]:
-    print(project_artifacts_root)
     # TODO: raise exception if root is empty
     all_project_configs = {}
+    logger.debug(f"Loading configs from {project_artifacts_root}")
     for project in os.listdir(project_artifacts_root):
         # hidden files from editors / OS like .idea
         if project.startswith("."):
             continue
         if filter_list and project not in filter_list:
             continue
-        print(project)
-        config = fetch_project_config(project, project_artifacts_root)
+        logger.debug(f"Loading config for {project}")
+        config = None
+        try:
+            config = fetch_project_config(project, project_artifacts_root)
+        except Exception as e:
+            traceback.print_exception(*sys.exc_info())
+            logger.debug(f"Failed to load config for {project}")
         if not config:
             continue
         all_project_configs.update({project: config})
 
     return all_project_configs
```

### Comparing `dialogy-2.0.7/dialogy/utils/datetime.py` & `dialogy-2.0.8/dialogy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/utils/file_handler.py` & `dialogy-2.0.8/dialogy/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/utils/logger.py` & `dialogy-2.0.8/dialogy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/utils/misc.py` & `dialogy-2.0.8/dialogy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/utils/naive_lang_detect.py` & `dialogy-2.0.8/dialogy/utils/naive_lang_detect.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/utils/normalize_utterance.py` & `dialogy-2.0.8/dialogy/utils/normalize_utterance.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/utils/temperature_scaling.py` & `dialogy-2.0.8/dialogy/utils/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/dialogy/workflow/workflow.py` & `dialogy-2.0.8/dialogy/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.7/pyproject.toml` & `dialogy-2.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialogy"
-version = "2.0.7"
+version = "2.0.8"
 description = "Dialogy is a library for building and managing SLU applications."
 authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>", "Daksh Varshneya <dakshvar22@gmail.com"]
 license = "MIT"
 repository = "https://github.com/skit-ai/dialogy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `dialogy-2.0.7/PKG-INFO` & `dialogy-2.0.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialogy
-Version: 2.0.7
+Version: 2.0.8
 Summary: Dialogy is a library for building and managing SLU applications.
 Home-page: https://github.com/skit-ai/dialogy
 License: MIT
 Author: Amresh Venugopal
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

