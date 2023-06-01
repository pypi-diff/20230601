# Comparing `tmp/ht_pricing_module-0.2.2.tar.gz` & `tmp/ht_pricing_module-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht_pricing_module-0.2.2.tar", last modified: Wed May 10 08:46:41 2023, max compression
+gzip compressed data, was "ht_pricing_module-0.2.3.tar", last modified: Thu Jun  1 06:42:19 2023, max compression
```

## Comparing `ht_pricing_module-0.2.2.tar` & `ht_pricing_module-0.2.3.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.082676 ht_pricing_module-0.2.2/
--rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0      263 2023-05-10 08:46:41.081678 ht_pricing_module-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.000871 ht_pricing_module-0.2.2/ht_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.2.2/ht_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.008849 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/
--rw-rw-rw-   0        0        0      216 2023-02-17 00:36:34.000000 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/__init__.py
--rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/api.py
--rw-rw-rw-   0        0        0      393 2023-03-23 06:42:27.000000 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/packages.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.010843 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/
--rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:40.988932 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.012838 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/api/
--rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
--rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/api/http.proto
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.014833 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/protobuf/
--rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
--rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
--rw-rw-rw-   0        0        0    45824 2023-04-14 09:34:03.000000 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/pricer.proto
--rw-rw-rw-   0        0        0     3252 2023-03-20 08:23:43.000000 ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.015830 ht_pricing_module-0.2.2/ht_pricing_module/finite_difference_engine/
--rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/finite_difference_engine/__init__.py
--rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.2.2/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.017825 ht_pricing_module-0.2.2/ht_pricing_module/monte_carlo_engine/
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/monte_carlo_engine/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-04-11 05:44:47.000000 ht_pricing_module-0.2.2/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.019820 ht_pricing_module-0.2.2/ht_pricing_module/multi_asset_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.2.2/ht_pricing_module/multi_asset_pricing_module/__init__.py
--rw-rw-rw-   0        0        0     4526 2023-05-09 02:19:35.000000 ht_pricing_module-0.2.2/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.021842 ht_pricing_module-0.2.2/ht_pricing_module/multi_asset_pricing_module/quotient/
--rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.2.2/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.2.2/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.024807 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/
--rw-rw-rw-   0        0        0      365 2023-03-22 13:14:15.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.035777 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/
--rw-rw-rw-   0        0        0      583 2023-04-25 03:15:40.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
--rw-rw-rw-   0        0        0     4091 2023-04-26 06:01:26.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
--rw-rw-rw-   0        0        0     3324 2023-04-26 06:01:26.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
--rw-rw-rw-   0        0        0     4109 2023-04-26 06:05:23.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
--rw-rw-rw-   0        0        0     4851 2023-04-26 06:09:46.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
--rw-rw-rw-   0        0        0     4196 2023-04-26 06:09:46.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4018 2023-04-26 06:09:46.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
--rw-rw-rw-   0        0        0     3372 2023-04-26 06:16:54.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
--rw-rw-rw-   0        0        0     4244 2023-04-26 06:16:54.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4324 2023-04-26 06:16:54.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
--rw-rw-rw-   0        0        0     5008 2023-04-26 06:16:54.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
--rw-rw-rw-   0        0        0     5262 2023-04-26 06:18:03.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.037772 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/airbag/
--rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
--rw-rw-rw-   0        0        0     3933 2023-04-26 06:24:32.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.041761 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/asian/
--rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
--rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
--rw-rw-rw-   0        0        0     2354 2023-03-24 08:39:50.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.051758 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/
--rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
--rw-rw-rw-   0        0        0     6176 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
--rw-rw-rw-   0        0        0     5340 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
--rw-rw-rw-   0        0        0     1876 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
--rw-rw-rw-   0        0        0     1797 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
--rw-rw-rw-   0        0        0     4573 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.054750 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/basket/
--rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-04-26 06:32:51.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
--rw-rw-rw-   0        0        0     2318 2023-04-11 07:04:53.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.058740 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/binary/
--rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
--rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
--rw-rw-rw-   0        0        0     2322 2023-04-11 07:04:53.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
--rw-rw-rw-   0        0        0     2343 2023-03-10 05:05:19.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
--rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.060734 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/forward/
--rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
--rw-rw-rw-   0        0        0      198 2023-04-26 05:49:02.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
--rw-rw-rw-   0        0        0     5680 2023-05-10 08:44:13.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.064724 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/sharkfin/
--rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
--rw-rw-rw-   0        0        0     2555 2023-04-26 06:24:32.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
--rw-rw-rw-   0        0        0     2350 2023-04-11 07:04:54.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
--rw-rw-rw-   0        0        0     3452 2023-04-26 06:24:32.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.066718 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/snowball/
--rw-rw-rw-   0        0        0       37 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
--rw-rw-rw-   0        0        0     7205 2023-05-08 09:57:30.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.068713 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/spread/
--rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
--rw-rw-rw-   0        0        0     2416 2023-04-11 07:04:53.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.072703 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/touch/
--rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
--rw-rw-rw-   0        0        0     1656 2023-03-20 07:48:57.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
--rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
--rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.080681 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/vanilla/
--rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
--rw-rw-rw-   0        0        0     2280 2023-04-11 07:04:53.000000 ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
--rw-rw-rw-   0        0        0    43982 2023-04-14 09:45:29.000000 ht_pricing_module-0.2.2/ht_pricing_module/simple_pricer_engine.py
-drwxrwxrwx   0        0        0        0 2023-05-10 08:46:41.005857 ht_pricing_module-0.2.2/ht_pricing_module.egg-info/
--rw-rw-rw-   0        0        0      263 2023-05-10 08:46:40.000000 ht_pricing_module-0.2.2/ht_pricing_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4957 2023-05-10 08:46:40.000000 ht_pricing_module-0.2.2/ht_pricing_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 08:46:40.000000 ht_pricing_module-0.2.2/ht_pricing_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-05-10 08:46:40.000000 ht_pricing_module-0.2.2/ht_pricing_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-10 08:46:40.000000 ht_pricing_module-0.2.2/ht_pricing_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 08:46:41.082676 ht_pricing_module-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1158 2023-05-10 08:27:42.000000 ht_pricing_module-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.135361 ht_pricing_module-0.2.3/
+-rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0      263 2023-06-01 06:42:19.135361 ht_pricing_module-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-06-01 06:41:58.000000 ht_pricing_module-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.671866 ht_pricing_module-0.2.3/ht_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.2.3/ht_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.698794 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/
+-rw-rw-rw-   0        0        0      258 2023-05-18 02:19:46.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/api.py
+-rw-rw-rw-   0        0        0      468 2023-05-29 08:11:33.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/packages.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.712761 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/
+-rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.660894 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.735699 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/api/
+-rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
+-rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/api/http.proto
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.771826 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/protobuf/
+-rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
+-rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
+-rw-rw-rw-   0        0        0    47780 2023-05-31 11:41:37.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/pricer.proto
+-rw-rw-rw-   0        0        0     3252 2023-05-16 06:25:50.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.784791 ht_pricing_module-0.2.3/ht_pricing_module/finite_difference_engine/
+-rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/finite_difference_engine/__init__.py
+-rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.2.3/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.795762 ht_pricing_module-0.2.3/ht_pricing_module/monte_carlo_engine/
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/monte_carlo_engine/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-04-11 05:44:47.000000 ht_pricing_module-0.2.3/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.807729 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/__init__.py
+-rw-rw-rw-   0        0        0     4526 2023-05-16 06:27:30.000000 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.820695 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/quotient/
+-rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.835655 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/
+-rw-rw-rw-   0        0        0      341 2023-05-11 09:39:17.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.940567 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/
+-rw-rw-rw-   0        0        0      583 2023-04-25 03:15:40.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     4087 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3320 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
+-rw-rw-rw-   0        0        0     4103 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
+-rw-rw-rw-   0        0        0     4843 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
+-rw-rw-rw-   0        0        0     4190 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4014 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3368 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
+-rw-rw-rw-   0        0        0     4238 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4318 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
+-rw-rw-rw-   0        0        0     5002 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
+-rw-rw-rw-   0        0        0     5254 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.953531 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/airbag/
+-rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
+-rw-rw-rw-   0        0        0     5089 2023-05-22 02:39:06.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.985446 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/
+-rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
+-rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
+-rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
+-rw-rw-rw-   0        0        0     2280 2023-05-31 05:05:32.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.012690 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/
+-rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
+-rw-rw-rw-   0        0        0     6174 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
+-rw-rw-rw-   0        0        0     5338 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
+-rw-rw-rw-   0        0        0     1874 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
+-rw-rw-rw-   0        0        0     1795 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     4425 2023-05-31 05:05:32.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.039617 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/
+-rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-04-26 06:32:51.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
+-rw-rw-rw-   0        0        0     2316 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.062556 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/
+-rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
+-rw-rw-rw-   0        0        0     2320 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
+-rw-rw-rw-   0        0        0     2261 2023-05-31 05:04:39.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
+-rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.064551 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/forward/
+-rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-04-26 05:49:02.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
+-rw-rw-rw-   0        0        0     5680 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.076519 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/
+-rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
+-rw-rw-rw-   0        0        0     2526 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
+-rw-rw-rw-   0        0        0     2348 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
+-rw-rw-rw-   0        0        0     3902 2023-05-16 06:54:45.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.086492 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/
+-rw-rw-rw-   0        0        0       95 2023-05-31 06:13:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+-rw-rw-rw-   0        0        0     5712 2023-05-31 11:47:11.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
+-rw-rw-rw-   0        0        0     6593 2023-05-31 05:04:39.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.096465 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/
+-rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
+-rw-rw-rw-   0        0        0     1481 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
+-rw-rw-rw-   0        0        0     2414 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.117410 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/
+-rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
+-rw-rw-rw-   0        0        0     1654 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
+-rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
+-rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.123392 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/
+-rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
+-rw-rw-rw-   0        0        0     2278 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
+-rw-rw-rw-   0        0        0    45281 2023-05-31 06:13:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/simple_pricer_engine.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.683833 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-06-01 06:42:18.000000 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5035 2023-06-01 06:42:18.000000 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 06:42:18.000000 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-01 06:42:18.000000 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 06:42:18.000000 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 06:42:19.136358 ht_pricing_module-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1158 2023-06-01 06:41:57.000000 ht_pricing_module-0.2.3/setup.py
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/api.py` & `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/api.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto` & `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/api/http.proto` & `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto` & `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto` & `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/protos/pricer.proto` & `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/pricer.proto`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,14 @@
     // FORWARD
     FORWARD_AS                          = 17;
 
     // SHARKFIN
     SHARKFIN_AS                         = 18;
     SHARKFIN_SERIES                     = 19;
 
-    // SNOWBALL
     SNOWBALL_MC                         = 20;
 
     // SPREAD
     RATIO_SPREAD_AS                     = 21;
     RATIO_SPREAD_SERIES                 = 22;
 
     // ONETOUCH
@@ -141,14 +140,15 @@
     LINEAR_ACC_AKO_AS                   = 31;
     FIXED_ACC_BARRIER_ENHANCED_AS       = 32;
     LINEAR_ACC_FIXED_ENHANCED_AS        = 33;
     DISCRETE_BINARY_MC                  = 34;
     LINEAR_ACC_FUSING_AS                = 35;
 
     QUOTIENT_AS                         = 36;
+    SNOWBALL_DISCOUNTED_MC              = 37;
 }
 
 message PricerReply {
     PriceType price_type                = 1;
     double result                       = 2;
 }
 
@@ -419,14 +419,16 @@
     double riskfree_rate                = 8;
     double dividend                     = 9;
     int32 year_base                     = 10;
     double barrier_price                = 11;
     double participation_rate           = 12;
     int32 is_knock_in                   = 13;
     double obs_freq                     = 14;
+    double cap_price                    = 15;
+    int32 is_capped                     = 16;
 
 }
 
 // ASIAN
 message AsianRequest {
     PriceType price_type                = 1;
     Asian param                         = 2;
@@ -783,14 +785,42 @@
     double dividend                                 = 15; // 分红率
     int32 year_base                                 = 16;
     repeated KnockObservation knock_in_obs_date     = 17; // 敲入观察序列
     repeated KnockObservation knock_out_obs_date    = 18; // 敲出观察序列
     double participation_rate                       = 19;
 }
 
+// SNOWBALL_DISCOUNTED
+message SnowballDiscountedMcRequest {
+    PriceType price_type                = 1;
+    SnowballDiscountedMc param          = 2;
+}
+
+message SnowballDiscountedMc {
+    double notional                                 = 1; // 单位数量名义金额
+    double spot_price                               = 2; // 当前价
+    double entrance_price                           = 3; // 入场价
+    double knock_in_barrier_price                   = 4; // 敲入价
+    double knock_out_barrier_price                  = 5; // 敲出价
+    int32 expiry_date                               = 6; // 到日期
+    double floor_rate                               = 7; // 保底比例
+    double margin_rate                              = 8; // 保证金比例
+    double bonus_rate                               = 9; // 持有到期绝对票息率
+    OptionType option_type                          = 10; // 正向反向雪球方向
+    int32 is_knock_in                               = 11; // 是否敲入
+    double current_date                             = 12; // 当前日离开仓日天数
+    double volatility                               = 13; // 波动率
+    double riskfree_rate                            = 14; // 无风险利率
+    double dividend                                 = 15; // 分红率
+    int32 year_base                                 = 16;
+    repeated KnockObservation knock_in_obs_date     = 17; // 敲入观察序列
+    repeated KnockObservation knock_out_obs_date    = 18; // 敲出观察序列
+    double knock_in_strike_price                    = 19;
+}
+
 // RATIO SPREAD
 message RatioSpreadRequest {
     PriceType price_type                = 1;
     RatioSpread param                   = 2;
 }
 
 message RatioSpread {
@@ -1135,14 +1165,20 @@
 
     rpc snowballMc (SnowballMcRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/snowball_mc"
         };
     };
 
+        rpc snowballDiscountedMc (SnowballDiscountedMcRequest) returns (PricerReply) {
+        option (google.api.http) = {
+            post: "/pricer/snowball_discounted_mc"
+        };
+    };
+
     rpc ratioSpread (RatioSpreadRequest) returns (PricerReply) {
         option (google.api.http) = {
             post: "/pricer/ratio_spread_as"
         };
     };
 
     rpc ratioSpreadSeries (RatioSpreadSeriesRequest) returns (PricerReply) {
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/api_and_utils/utils.py` & `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 class Struct(dict):
     """
     实现将dict类型转换成结构体类型，可以直接通过 ”.“ 调用其属性。
     服务器定价器接收参数为grpc定义的message类型，定价函数中全部使用 “self.param.” 进行调用。
     为统一标准，传入的参数dict需转化成该结构体类型进行使用。
 
     e.g.
-    param = Struct()
+    param = Params()
     param['spot_price'] = 100 or param.spot_price = 100
     pricer = Vanilla(kwargs)
     pv = pricer.present_value()
     ...
 
     现版本中可接受直接传入dict类型或Struct类型
     """
@@ -61,15 +61,15 @@
         该方法仅在调用蒙特卡洛MC方法时,需要传入指定观察日序列时使用。
         服务端定价器参数通过 ”.“ 调用其属性，直接调用定价函数时，需要使用该方法对传入的观察日dict或DataFrame序列进行转换
         :param input: dict or DataFrame
         :return: [Struct(), Struct(), Struct(), ...]
 
         e.g.
         discrete_asian_mc，param.obs_date参数
-        param = Struct()
+        param = Params()
         param['obs_date'] = RepeatedStruct({'obs_index': [1, 2, 3, ... ],
                                             'obs_price': [100, 99, 100, ...]})
         ...
         """
 
         output = []
         if isinstance(input, dict):
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/finite_difference_engine/fd_grid_generator.py` & `ht_pricing_module-0.2.3/ht_pricing_module/finite_difference_engine/fd_grid_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/monte_carlo_engine/mc_path_generator.py` & `ht_pricing_module-0.2.3/ht_pricing_module/monte_carlo_engine/mc_path_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py` & `ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ..monte_carlo_engine import *
 from ..api_and_utils import *
 
 
 class MultiAssetOptionBase:
 
     def __init__(self, param):
-        self.param = Struct(param) if isinstance(param, dict) else param
+        self.param = Params(param) if isinstance(param, dict) else param
 
     def __calculate_present_value__(self) -> float:
         raise NotImplementedError()
 
     @lru_cache(maxsize=10)
     def present_value(self) -> float:
         return self.__calculate_present_value__()
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
         barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP, OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
@@ -28,15 +28,15 @@
             param['barrier_type'] = barrier_type
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
             param['rebate'] = 0
             param['obs_freq'] = self.param.obs_freq
             barrier1 = DiscreteBarrier(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,28 @@
     def __calculate_present_value__(self) -> float:
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             vanilla1 = Vanilla(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,42 +8,42 @@
     def __calculate_present_value__(self) -> float:
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             vanilla1 = Vanilla(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
             binary2 = Binary(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,56 +8,56 @@
     def __calculate_present_value__(self) -> float:
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             vanilla1 = Vanilla(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
             binary2 = Binary(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
             binary3 = Binary(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,42 +9,42 @@
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
         option_type3 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             vanilla1 = Vanilla(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['payoff'] = self.param.payoff
             param['year_base'] = self.param.year_base
             binary2 = Binary(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type3
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
         barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP, OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
@@ -27,15 +27,15 @@
             param['barrier_type'] = barrier_type
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
             param['rebate'] = 0
             param['obs_freq'] = self.param.obs_freq
             barrier1 = DiscreteBarrier(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,28 +8,28 @@
     def __calculate_present_value__(self) -> float:
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             vanilla1 = Vanilla(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,42 +9,42 @@
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
         option_type3 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             vanilla1 = Vanilla(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             sharkfin2 = Sharkfin(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type3
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,42 +10,42 @@
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
         option_type3 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             vanilla1 = Vanilla(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['year_base'] = self.param.year_base
             sharkfin2 = Sharkfin(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type3
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         option_type2 = {OptionType.ACCUMULATOR: OptionType.CALL, OptionType.DECUMULATOR: OptionType.PUT}[self.param.option_type]
         barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP, OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
@@ -27,15 +27,15 @@
             param['barrier_type'] = barrier_type
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
             param['rebate'] = 0
             param['obs_freq'] = self.param.obs_freq
             barrier1 = DiscreteBarrier(param)
 
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type2
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
@@ -48,15 +48,15 @@
             param['is_knock_in'] = 0
             param['rebate'] = self.param.payoff
             param['obs_freq'] = self.param.obs_freq
             barrier2 = DiscreteBarrier(param)
 
             rst = rst + self.param.base_quantity * (-self.param.leverage * barrier1.present_value() + barrier2.present_value())
 
-        param = Struct({})
+        param = Params()
         param['option_type'] = option_type1
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         rst = 0
 
         option_type1 = {OptionType.ACCUMULATOR: OptionType.PUT, OptionType.DECUMULATOR: OptionType.CALL}[self.param.option_type]
         barrier_type = {OptionType.ACCUMULATOR: BarrierType.UP, OptionType.DECUMULATOR: BarrierType.DOWN}[self.param.option_type]
         cp = {OptionType.ACCUMULATOR: 1, OptionType.DECUMULATOR: -1}[self.param.option_type]
 
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = option_type1
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
@@ -29,15 +29,15 @@
             param['barrier_type'] = barrier_type
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
             param['rebate'] = 0
             param['obs_freq'] = self.param.obs_freq
             barrier1 = DiscreteBarrier(param)
 
-            param = Struct({})
+            param = Params()
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['barrier_price'] = self.param.barrier_price
             param['riskfree_rate'] = self.param.riskfree_rate
             param['dividend'] = self.param.dividend
             param['volatility'] = self.param.volatility
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
@@ -46,22 +46,22 @@
             param['knock_type'] = KnockType.OUT
             param['is_knock_in'] = 0
             param['rebate_type'] = RebateType.PAH
             param['rebate'] = cp * (self.param.entrance_price - self.param.strike_price)
             param['obs_freq'] = self.param.obs_freq
             touch2 = DiscreteOneTouch(param)
 
-            param = Struct({})
+            param = Params()
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.entrance_price
             forward3 = Forward(param)
 
             rst = rst + self.param.base_quantity * (-(self.param.leverage - 1) * barrier1.present_value() + touch2.present_value() + cp * forward3.present_value())
 
-        param = Struct({})
+        param = Params()
         param['option_type'] = option_type1
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
     def __calculate_present_value__(self):
         phi = {OptionType.STANDARD: 1, OptionType.REVERSE: -1}[self.param.option_type]
 
         if self.param.strike_price == self.param.barrier_price or self.param.is_knock_in or\
                 (self.param.option_type == OptionType.STANDARD and self.param.spot_price <= self.param.barrier_price) or\
                 (self.param.option_type == OptionType.REVERSE and self.param.spot_price >= self.param.barrier_price):
-            param = Struct({})
+            param = Params()
             param['spot_price'] = self.param.spot_price
             param['strike_price'] = self.param.strike_price
             forward = Forward(param=param)
             return phi * forward.present_value()
 
         barrier_type = {OptionType.STANDARD: BarrierType.DOWN, OptionType.REVERSE: BarrierType.UP}[self.param.option_type]
         option_type = {OptionType.STANDARD: OptionType.CALL, OptionType.REVERSE: OptionType.PUT}[self.param.option_type]
 
-        param = Struct({})
+        param = Params()
         param['option_type'] = OptionType.CALL
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
@@ -35,15 +35,15 @@
         param['barrier_type'] = barrier_type
         param['knock_type'] = KnockType.IN
         param['is_knock_in'] = self.param.is_knock_in
         param['rebate'] = 0
         param['obs_freq'] = self.param.obs_freq
         barrier1 = DiscreteBarrier(param)
 
-        param = Struct({})
+        param = Params()
         param['option_type'] = OptionType.PUT
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
@@ -54,15 +54,15 @@
         param['barrier_type'] = barrier_type
         param['knock_type'] = KnockType.IN
         param['is_knock_in'] = self.param.is_knock_in
         param['rebate'] = 0
         param['obs_freq'] = self.param.obs_freq
         barrier2 = DiscreteBarrier(param)
 
-        param = Struct({})
+        param = Params()
         param['option_type'] = option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
@@ -73,8 +73,30 @@
         param['barrier_type'] = barrier_type
         param['knock_type'] = KnockType.OUT
         param['is_knock_in'] = self.param.is_knock_in
         param['rebate'] = 0
         param['obs_freq'] = self.param.obs_freq
         barrier3 = DiscreteBarrier(param)
 
+        if self.param.is_capped:
+            param = Params()
+            param['option_type'] = option_type
+            param['exercise_type'] = self.param.exercise_type
+            param['spot_price'] = self.param.spot_price
+            param['strike_price'] = self.param.cap_price
+            param['barrier_price'] = self.param.barrier_price
+            param['riskfree_rate'] = self.param.riskfree_rate
+            param['dividend'] = self.param.dividend
+            param['volatility'] = self.param.volatility
+            param['expiry_date'] = self.param.expiry_date
+            param['current_date'] = self.param.current_date
+            param['year_base'] = self.param.year_base
+            param['barrier_type'] = barrier_type
+            param['knock_type'] = KnockType.OUT
+            param['is_knock_in'] = self.param.is_knock_in
+            param['rebate'] = 0
+            param['obs_freq'] = self.param.obs_freq
+            barrier4 = DiscreteBarrier(param)
+
+            return phi * (barrier1.present_value() - barrier2.present_value()) + self.param.participation_rate * (barrier3.present_value() - barrier4.present_value())
+
         return phi * (barrier1.present_value() - barrier2.present_value()) + self.param.participation_rate * barrier3.present_value()
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 from ..one_asset_option_base import *
 
 
-class DiscreteAsianMc(OneAssetOptionBase):
+def __mc_asian__(option_type, spot_price, strike_price, running_avg, riskfree_rate, dividend, volatility,
+                 residual_intraday, expiry_date, year_base, obs):
     """
     算术平均离散亚视期权MC
-    :param obs_date: 离散观测日，包括：历史观测日及已实现价格和未来观测日
+    :param obs: 离散观测日，包括：历史观测日及已实现价格和未来观测日
     """
 
+    cp = 1 if option_type == OptionType.CALL else - 1
+    rst = 0
+    if expiry_date <= 0:
+        rst = max(cp * (np.mean(running_avg) - strike_price), 0)
+    else:
+        intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
+        gmb = McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
+                                       intraday=intraday, expiry_date=expiry_date, year_base=year_base, random_seed=0)
+        price = spot_price * gmb
+        obs = np.array(obs)
+        obs_index_arr = obs[obs[:, 0] >= 0][:, 0].astype(int)
+        obs_price_arr = obs[obs[:, 0] < 0][:, 1]
+
+        discount_factor = np.exp(-1 * riskfree_rate * (expiry_date - intraday) / year_base)
+        avg_price_arr = np.mean(np.concatenate((np.tile(obs_price_arr, (len(price), 1)), price[:, obs_index_arr]), axis=1), axis=1)
+        rst = np.mean(discount_factor * np.maximum(cp * (avg_price_arr - strike_price), 0))
+    return rst
+
+
+class DiscreteAsianMc(OneAssetOptionBase):
+
     def __calculate_present_value__(self) -> float:
         residual_intraday = round(math.ceil(self.param.current_date) - self.param.current_date, 4)
         current_date_index = math.floor(self.param.current_date)
-        return self.mc_asian(
+        return __mc_asian__(
             option_type=self.param.option_type,
             spot_price=self.param.spot_price,
             strike_price=self.param.strike_price,
             running_avg=self.param.running_avg,
             riskfree_rate=self.param.riskfree_rate,
             dividend=self.param.dividend,
             volatility=self.param.volatility,
             residual_intraday=residual_intraday,
             expiry_date=self.param.expiry_date - current_date_index,
             year_base=self.param.year_base,
             obs=[[obs.obs_index - current_date_index, obs.obs_price]for obs in self.param.obs_date]
         )
-
-    def mc_asian(self, option_type, spot_price, strike_price, running_avg, riskfree_rate, dividend, volatility,
-                 residual_intraday, expiry_date, year_base, obs):
-
-        cp = 1 if option_type == OptionType.CALL else - 1
-        rst = 0
-        if expiry_date <= 0:
-            rst = max(cp * (np.mean(running_avg) - strike_price), 0)
-        else:
-            intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
-            gmb = McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
-                                           intraday=intraday, expiry_date=expiry_date, year_base=year_base, random_seed=0)
-            price = spot_price * gmb
-            obs = np.array(obs)
-            obs_index_arr = obs[obs[:, 0] >= 0][:, 0].astype(int)
-            obs_price_arr = obs[obs[:, 0] < 0][:, 1]
-
-            discount_factor = np.exp(-1 * riskfree_rate * (expiry_date - intraday) / year_base)
-            avg_price_arr = np.mean(np.concatenate((np.tile(obs_price_arr, (len(price), 1)), price[:, obs_index_arr]), axis=1), axis=1)
-            rst = np.mean(discount_factor * np.maximum(cp * (avg_price_arr - strike_price), 0))
-        return rst
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                     return max(cp * (self.param.spot_price - self.param.strike_price), 0)
         else:
             """存续"""
             if self.param.knock_type == KnockType.IN:
                 if self.param.is_knock_in or u_knock_flag or d_knock_flag:
                     """敲入"""
 
-                    param = Struct({})
+                    param = Params()
                     param['option_type'] = self.param.option_type
                     param['exercise_type'] = self.param.exercise_type
                     param['spot_price'] = self.param.spot_price
                     param['strike_price'] = self.param.strike_price
                     param['expiry_date'] = self.param.expiry_date
                     param['current_date'] = self.param.current_date
                     param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
                     return self.param.payoff if cp * (self.param.spot_price - self.param.strike_price) >= 0 else 0
         else:
             """存续"""
             if self.param.knock_type == KnockType.IN:
                 if self.param.is_knock_in or u_knock_flag or d_knock_flag:
                     """敲入"""
 
-                    param = Struct({})
+                    param = Params()
                     param['option_type'] = self.param.option_type
                     param['exercise_type'] = self.param.exercise_type
                     param['spot_price'] = self.param.spot_price
                     param['strike_price'] = self.param.strike_price
                     param['expiry_date'] = self.param.expiry_date
                     param['current_date'] = self.param.current_date
                     param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         adjust = 0.5826 * self.param.volatility * math.sqrt(dt)
         if self.param.barrier_type == BarrierType.UP and time_to_expiry > 0:
             self.param.barrier_price = self.param.barrier_price * np.exp(adjust)
         elif self.param.barrier_type == BarrierType.DOWN and time_to_expiry > 0:
             self.param.barrier_price = self.param.barrier_price * np.exp(-adjust)
 
     def __calculate_present_value__(self) -> float:
-        param = Struct({})
+        param = Params()
         param['option_type'] = self.param.option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         adjust = 0.5826 * self.param.volatility * math.sqrt(dt)
         if self.param.barrier_type == BarrierType.UP and time_to_expiry > 0:
             self.param.barrier_price = self.param.barrier_price * np.exp(adjust)
         elif self.param.barrier_type == BarrierType.DOWN and time_to_expiry > 0:
             self.param.barrier_price = self.param.barrier_price * np.exp(-adjust)
 
     def __calculate_present_value__(self) -> float:
-        param = Struct({})
+        param = Params()
         param['option_type'] = self.param.option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['barrier_price'] = self.param.barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,65 @@
 from ..one_asset_option_base import *
 from ..vanilla.vanilla_as import Vanilla
 
 
-class DiscreteBarrierMc(OneAssetOptionBase):
+def __mc_barrier__(option_type, knock_type, barrier_type, spot_price, strike_price, barrier_price, rebate,
+                   riskfree_rate, dividend, volatility, residual_intraday, expiry_date, year_base, obs):
     """
     离散障碍期权MC
-    :param obs_date: 离散观测日
+    :param obs: 离散观测日
     """
 
+    cp = {OptionType.CALL: 1, OptionType.PUT: -1}[option_type]
+    io = {KnockType.IN: 1, KnockType.OUT: -1}[knock_type]
+    ud = {BarrierType.UP: 1, BarrierType.DOWN: -1}[barrier_type]
+    rst = 0
+
+    if expiry_date <= 0:
+        knock = 1 if ud * (spot_price - barrier_price) >= 0 else -1
+        if knock * io == 1:
+            rst = max(cp * (spot_price - strike_price), 0)
+        elif knock * io == -1:
+            rst = (0 if io == 1 else 1) * rebate
+    else:
+        intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
+        gbm = McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
+                                       intraday=intraday, expiry_date=expiry_date, year_base=year_base, random_seed=0)
+
+        price = spot_price * gbm
+
+        obs_arr = np.array(obs).astype(int)
+        obs_arr = obs_arr[obs_arr >= 0]
+
+        knock_flag = ud * (price[:, obs_arr] - barrier_price) >= 0
+        knock_index = (np.insert(knock_flag, 0, np.zeros(len(knock_flag)), axis=1)).argmax(axis=1)
+
+        if io == 1:
+            knock_index = np.where(knock_index > 0, 1, 0)
+            discount_factor = np.exp(-1 * riskfree_rate * (expiry_date - intraday) / year_base)
+            value = np.multiply(knock_index.T, np.maximum(cp * (price[:, -1] - strike_price), 0))
+            value = value + np.multiply((1 - knock_index).T, rebate)
+            rst = np.mean(discount_factor * value)
+        else:
+            discount_factor_arr = np.exp(-1 * riskfree_rate * (obs_arr - intraday) / year_base)
+            discount_factor_arr = np.insert(discount_factor_arr, 0, 0)[knock_index]
+            discount_factor = np.exp(-1 * riskfree_rate * (expiry_date - intraday) / year_base)
+            knock_index = np.where(knock_index > 0, 1, 0)
+            value = np.multiply(discount_factor_arr.T, rebate * knock_index)
+            value = value + discount_factor * np.multiply((1 - knock_index).T, np.maximum(cp * (price[:, -1] - strike_price), 0))
+            rst = np.mean(value)
+    return rst
+
+
+class DiscreteBarrierMc(OneAssetOptionBase):
+
     def __calculate_present_value__(self) -> float:
         if self.param.is_knock_in and self.param.knock_type == KnockType.IN:
             # vanilla
-            param = Struct({})
+            param = Params()
             param['option_type'] = self.param.option_type
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = self.param.expiry_date
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
@@ -24,15 +68,15 @@
             param['year_base'] = self.param.year_base
             vanilla = Vanilla(param)
             return vanilla.present_value()
         else:
             # mc
             residual_intraday = round(math.ceil(self.param.current_date) - self.param.current_date, 4)
             current_date_index = math.floor(self.param.current_date)
-            return self.mc_barrier(
+            return __mc_barrier__(
                 option_type=self.param.option_type,
                 knock_type=self.param.knock_type,
                 barrier_type=self.param.barrier_type,
                 spot_price=self.param.spot_price,
                 strike_price=self.param.strike_price,
                 barrier_price=self.param.barrier_price,
                 rebate=self.param.rebate,
@@ -40,50 +84,7 @@
                 dividend=self.param.dividend,
                 volatility=self.param.volatility,
                 residual_intraday=residual_intraday,
                 expiry_date=self.param.expiry_date - current_date_index,
                 year_base=self.param.year_base,
                 obs=[obs.obs_index - current_date_index for obs in self.param.obs_date]
             )
-
-    def mc_barrier(self, option_type, knock_type, barrier_type, spot_price, strike_price, barrier_price, rebate,
-                   riskfree_rate, dividend, volatility, residual_intraday, expiry_date, year_base, obs):
-
-        cp = {OptionType.CALL: 1, OptionType.PUT: -1}[option_type]
-        io = {KnockType.IN: 1, KnockType.OUT: -1}[knock_type]
-        ud = {BarrierType.UP: 1, BarrierType.DOWN: -1}[barrier_type]
-        rst = 0
-
-        if expiry_date <= 0:
-            knock = 1 if ud * (spot_price - barrier_price) >= 0 else -1
-            if knock * io == 1:
-                rst = max(cp * (spot_price - strike_price), 0)
-            elif knock * io == -1:
-                rst = (0 if io == 1 else 1) * rebate
-        else:
-            intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
-            gbm = McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
-                                           intraday=intraday, expiry_date=expiry_date, year_base=year_base, random_seed=0)
-
-            price = spot_price * gbm
-
-            obs_arr = np.array(obs).astype(int)
-            obs_arr = obs_arr[obs_arr >= 0]
-
-            knock_flag = ud * (price[:, obs_arr] - barrier_price) >= 0
-            knock_index = (np.insert(knock_flag, 0, np.zeros(len(knock_flag)), axis=1)).argmax(axis=1)
-
-            if io == 1:
-                knock_index = np.where(knock_index > 0, 1, 0)
-                discount_factor = np.exp(-1 * riskfree_rate * (expiry_date - intraday) / year_base)
-                value = np.multiply(knock_index.T, np.maximum(cp * (price[:, -1] - strike_price), 0))
-                value = value + np.multiply((1 - knock_index).T, rebate)
-                rst = np.mean(discount_factor * value)
-            else:
-                discount_factor_arr = np.exp(-1 * riskfree_rate * (obs_arr - intraday) / year_base)
-                discount_factor_arr = np.insert(discount_factor_arr, 0, 0)[knock_index]
-                discount_factor = np.exp(-1 * riskfree_rate * (expiry_date - intraday) / year_base)
-                knock_index = np.where(knock_index > 0, 1, 0)
-                value = np.multiply(discount_factor_arr.T, rebate * knock_index)
-                value = value + discount_factor * np.multiply((1 - knock_index).T, np.maximum(cp * (price[:, -1] - strike_price), 0))
-                rst = np.mean(value)
-        return rst
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class BasketVanillaSeries(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = self.param.option_type
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class BinarySeries(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = self.param.option_type
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,51 +1,52 @@
 from ..one_asset_option_base import *
 
 
-class DiscreteBinaryMc(OneAssetOptionBase):
+def __mc_binary__(option_type, spot_price, strike_price, payoff, riskfree_rate, dividend, volatility,
+                  residual_intraday, expiry_date, year_base, obs):
     """
     离散观测二元MC
-    :param obs_date: 离散观测日
+    :param obs: 离散观测日
     """
 
+    cp = {OptionType.CALL: 1, OptionType.PUT: -1}[option_type]
+    rst = 0
+
+    if expiry_date <= 0:
+        rst = payoff if cp * (spot_price - strike_price) >= 0 else 0
+    else:
+        intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
+        gbm = McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
+                                       intraday=intraday, expiry_date=expiry_date, year_base=year_base,
+                                       random_seed=0)
+
+        price = spot_price * gbm
+
+        obs_arr = np.array(obs).astype(int)
+        obs_arr = obs_arr[obs_arr >= 0]
+
+        payoff_flag = cp * (price[:, obs_arr] - strike_price) >= 0
+        payoff_index = (np.insert(payoff_flag, 0, np.zeros(len(payoff_flag)), axis=1)).argmax(axis=1)
+        discount_factor_arr = np.exp(-1 * riskfree_rate * (obs_arr - intraday) / year_base)
+        discount_factor_arr = np.insert(discount_factor_arr, 0, 0)[payoff_index]
+        rst = np.mean(payoff * discount_factor_arr)
+    return rst
+
+
+class DiscreteBinaryMc(OneAssetOptionBase):
+
     def __calculate_present_value__(self) -> float:
         residual_intraday = round(math.ceil(self.param.current_date) - self.param.current_date, 4)
         current_date_index = math.floor(self.param.current_date)
-        return self.mc_binary(
+        return __mc_binary__(
             option_type=self.param.option_type,
             spot_price=self.param.spot_price,
             strike_price=self.param.strike_price,
             payoff=self.param.payoff,
             riskfree_rate=self.param.riskfree_rate,
             dividend=self.param.dividend,
             volatility=self.param.volatility,
             residual_intraday=residual_intraday,
             expiry_date=self.param.expiry_date - current_date_index,
             year_base=self.param.year_base,
             obs=[obs.obs_index - current_date_index for obs in self.param.obs_date]
         )
-
-    def mc_binary(self, option_type, spot_price, strike_price, payoff, riskfree_rate, dividend, volatility,
-                  residual_intraday, expiry_date, year_base, obs):
-
-        cp = {OptionType.CALL: 1, OptionType.PUT: -1}[option_type]
-        rst = 0
-
-        if expiry_date <= 0:
-            rst = payoff if cp * (spot_price - strike_price) >= 0 else 0
-        else:
-            intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
-            gbm = McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
-                                           intraday=intraday, expiry_date=expiry_date, year_base=year_base,
-                                           random_seed=0)
-
-            price = spot_price * gbm
-
-            obs_arr = np.array(obs).astype(int)
-            obs_arr = obs_arr[obs_arr >= 0]
-
-            payoff_flag = cp * (price[:, obs_arr] - strike_price) >= 0
-            payoff_index = (np.insert(payoff_flag, 0, np.zeros(len(payoff_flag)), axis=1)).argmax(axis=1)
-            discount_factor_arr = np.exp(-1 * riskfree_rate * (obs_arr - intraday) / year_base)
-            discount_factor_arr = np.insert(discount_factor_arr, 0, 0)[payoff_index]
-            rst = np.mean(payoff * discount_factor_arr)
-        return rst
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from ..monte_carlo_engine import *
 from ..api_and_utils import *
 
 
 class OneAssetOptionBase:
 
     def __init__(self, param):
-        self.param = Struct(param) if isinstance(param, dict) else param
+        self.param = Params(param) if isinstance(param, dict) else param
 
     def __calculate_present_value__(self) -> float:
         raise NotImplementedError()
 
     @lru_cache(maxsize=10)
     def present_value(self) -> float:
         return self.__calculate_present_value__()
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 class Sharkfin(OneAssetOptionBase):
         
     def __calculate_present_value__(self):
         if self.param.strike_price == self.param.barrier_price:
             return 0
 
-        param = Struct({})
+        param = Params()
         param['option_type'] = self.param.option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
         param['volatility'] = self.param.volatility
@@ -21,30 +21,30 @@
         param['dividend'] = self.param.dividend
         param['year_base'] = self.param.year_base
         vanilla1 = Vanilla(param)
 
         cp = {OptionType.CALL: 1, OptionType.PUT: -1}[self.param.option_type]
         gt = 1 if (self.param.strike_price - self.param.barrier_price) > 0 else -1
         if cp * gt > 0:
-            return vanilla1.present_value()
+            return 0
 
-        param = Struct({})
+        param = Params()
         param['option_type'] = self.param.option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.barrier_price
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
         param['volatility'] = self.param.volatility
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
         param['year_base'] = self.param.year_base
         vanilla2 = Vanilla(param)
 
-        param = Struct({})
+        param = Params()
         param['option_type'] = self.param.option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.barrier_price
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
         param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class SharkfinSeries(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = self.param.option_type
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['barrier_price'] = self.param.barrier_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,95 @@
 from ..one_asset_option_base import *
 
 
-class SnowballMc(OneAssetOptionBase):
+def __mc_snowball__(notional, spot_price, entrance_price, knock_in_barrier_price, knock_out_barrier_price,
+                    floor_rate, margin_rate, bonus_rate, option_type, is_knock_in, riskfree_rate, dividend, volatility,
+                    residual_intraday, expiry_date, year_base, knock_in_obs, knock_out_obs, participation_rate=0):
     """
     雪球期权
-    :param knock_in_obs_date 敲入观测日, 包括obs_index观测日期，adjust(对障碍价格进行比率调整，1为原始输入敲入价格)
-    :param knock_out_obs_date 敲出观测日，包括obs_index观测日期，adjust(对障碍价格进行比率调整，1为原始输入敲出价格)，coupon_rate票息(已经过敲出日期调整)
+    :param knock_in_obs 敲入观测日, 包括obs_index观测日期，adjust(对障碍价格进行比率调整，1为原始输入敲入价格)
+    :param knock_out_obs 敲出观测日，包括obs_index观测日期，adjust(对障碍价格进行比率调整，1为原始输入敲出价格)，coupon_rate票息(已经过敲出日期调整)
     :param floor_rate 保护价
     :param margin_rate 保证金率
-    :param bouns_rate 到期收益(非年化)
+    :param bonus_rate 到期收益(非年化)
     """
 
+    phi = {OptionType.STANDARD: 1, OptionType.REVERSE: -1}[option_type]
+    if expiry_date <= 0:
+        # 判断最后一天敲入敲出
+        ki_adj = knock_in_obs['adjust_rate'][np.where(knock_in_obs['obs_index'] == expiry_date)]
+        ki_flag = phi * (spot_price - knock_in_barrier_price * ki_adj) <= 0
+        ki_flag = False if len(ki_flag) == 0 else ki_flag[0]
+
+        ko_adj = knock_out_obs['adjust_rate'][np.where(knock_out_obs['obs_index'] == expiry_date)]
+        ko_flag = phi * (spot_price - knock_out_barrier_price * ko_adj) >= 0
+        ko_flag = False if len(ko_flag) == 0 else ko_flag[0]
+        if ko_flag:
+            # 敲出损益
+            rst = notional * knock_out_obs['coupon_rate'][np.where(knock_out_obs['obs_index'] == expiry_date)][0]
+        elif is_knock_in or ki_flag:
+            # 敲入损益
+            rst = notional * max((floor_rate - 1), min(phi * (spot_price / entrance_price - 1), 0))
+        else:
+            # 未敲入未敲出
+            rst = notional * bonus_rate
+        return rst
+
+    intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
+    price = spot_price * McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
+                                                  intraday=intraday, expiry_date=expiry_date, year_base=year_base, random_seed=0)
+    M = len(price)
+
+    ki_obs_idx = np.where(knock_in_obs['obs_index'] >= 0)
+    ki_adj = knock_in_obs['adjust_rate'][ki_obs_idx]
+    ki_obs_idx = knock_in_obs['obs_index'][ki_obs_idx].astype(int)
+
+    ko_obs_idx = np.where(knock_out_obs['obs_index'] >= 0)
+    ko_adj = knock_out_obs['adjust_rate'][ko_obs_idx]
+    ko_coupon = knock_out_obs['coupon_rate'][ko_obs_idx]
+    ko_obs_idx = knock_out_obs['obs_index'][ko_obs_idx].astype(int)
+
+    t_arr = np.hstack([0, np.arange(1, expiry_date + 1, 1) - intraday])
+    assert round(expiry_date - intraday, 4) == round(t_arr[-1], 4)
+
+    knock_in_barrier_price = knock_in_barrier_price * ki_adj
+    knock_out_barrier_price = knock_out_barrier_price * ko_adj
+
+    ki_mat_flag = np.zeros((M, 1), dtype=bool) if len(ki_obs_idx) == 0 else phi * (price[:, ki_obs_idx] - knock_in_barrier_price) <= 0
+    ko_mat_flag = np.zeros((M, 1), dtype=bool) if len(ko_obs_idx) == 0 else phi * (price[:, ko_obs_idx] - knock_out_barrier_price) >= 0
+    ko_idx = ko_mat_flag.argmax(axis=1)
+
+    # 敲出
+    discount_factor = 1 / np.exp(riskfree_rate * t_arr[ko_obs_idx][ko_idx] / year_base)
+    ko_arr_flag = np.max(ko_mat_flag, axis=1)
+    ko_payoff = ko_arr_flag * discount_factor * notional * (ko_coupon[ko_idx] + phi * participation_rate * ((price[:, ko_obs_idx] / knock_out_barrier_price - 1)[np.arange(M), ko_idx])
+                                                            - margin_rate * (np.exp(riskfree_rate * t_arr[ko_obs_idx][ko_idx] / year_base) - 1))
+
+    # 敲入未敲出
+    discount_factor = 1 / np.exp(riskfree_rate * (expiry_date - intraday) / year_base)
+    ki_arr_flag = np.logical_or(is_knock_in, np.max(ki_mat_flag, axis=1))
+    ki_no_ko_arr_flag = np.logical_and(ki_arr_flag, np.logical_not(ko_arr_flag))
+    ki_no_ko_payoff = ki_no_ko_arr_flag * discount_factor * notional * (np.maximum((floor_rate - 1), np.minimum(phi * (price[:, -1] / entrance_price - 1), 0))
+                                                                        - margin_rate * (1 / discount_factor - 1))
+
+    # 未敲入未敲出
+    discount_factor = 1 / np.exp(riskfree_rate * (expiry_date - intraday) / year_base)
+    no_ki_no_ko_arr_flag = np.logical_and(np.logical_not(ki_arr_flag), np.logical_not(ko_arr_flag))
+    no_ki_no_ko_payoff = no_ki_no_ko_arr_flag * discount_factor * notional * (bonus_rate - margin_rate * (1 / discount_factor - 1))
+
+    rst = np.round(np.mean(ko_payoff + ki_no_ko_payoff + no_ki_no_ko_payoff), 8)
+    return rst
+
+
+class SnowballMc(OneAssetOptionBase):
+
     def __calculate_present_value__(self) -> float:
         residual_intraday = round(math.ceil(self.param.current_date) - self.param.current_date, 4)
         current_date_index = math.floor(self.param.current_date)
-        return self.mc_snowball(
+        return __mc_snowball__(
             notional=self.param.notional,
             spot_price=self.param.spot_price,
             entrance_price=self.param.entrance_price,
             knock_in_barrier_price=self.param.knock_in_barrier_price,
             knock_out_barrier_price=self.param.knock_out_barrier_price,
             floor_rate=self.param.floor_rate,
             margin_rate=self.param.margin_rate,
@@ -34,91 +105,7 @@
             participation_rate=self.param.participation_rate,
             knock_in_obs={'obs_index': np.array([obs.obs_index - current_date_index for obs in self.param.knock_in_obs_date]),
                           'adjust_rate': np.array([obs.adjust_rate for obs in self.param.knock_in_obs_date])},
             knock_out_obs={'obs_index': np.array([obs.obs_index - current_date_index for obs in self.param.knock_out_obs_date]),
                            'adjust_rate': np.array([obs.adjust_rate for obs in self.param.knock_out_obs_date]),
                            'coupon_rate': np.array([obs.coupon_rate for obs in self.param.knock_out_obs_date])}
         )
-
-    def mc_snowball(self, notional, spot_price, entrance_price, knock_in_barrier_price, knock_out_barrier_price,
-                    floor_rate, margin_rate, bonus_rate, option_type, is_knock_in, riskfree_rate, dividend, volatility,
-                    residual_intraday, expiry_date, year_base, knock_in_obs, knock_out_obs,
-                    participation_rate=0):
-
-        phi = {OptionType.STANDARD: 1, OptionType.REVERSE: -1}[option_type]
-        if expiry_date <= 0:
-            # 判断最后一天敲入敲出
-            ki_adj = knock_in_obs['adjust_rate'][np.where(knock_in_obs['obs_index'] == expiry_date)]
-            ki_flag = phi * (spot_price - knock_in_barrier_price * ki_adj) <= 0
-            ki_flag = False if len(ki_flag) == 0 else ki_flag[0]
-
-            ko_adj = knock_out_obs['adjust_rate'][np.where(knock_out_obs['obs_index'] == expiry_date)]
-            ko_flag = phi * (spot_price - knock_out_barrier_price * ko_adj) >= 0
-            ko_flag = False if len(ko_flag) == 0 else ko_flag[0]
-            if ko_flag:
-                # 敲出损益
-                rst = notional * knock_out_obs['coupon_rate'][np.where(knock_out_obs['obs_index'] == expiry_date)][0]
-            elif is_knock_in or ki_flag:
-                # 敲入损益
-                rst = notional * max((floor_rate - 1), min(phi * (spot_price / entrance_price - 1), 0))
-            else:
-                # 未敲入未敲出
-                rst = notional * bonus_rate
-            return rst
-
-        intraday = round(math.ceil(residual_intraday) - residual_intraday, 4)
-        gbm = McPathGenerator.generate(riskfree_rate=riskfree_rate, dividend=dividend, volatility=volatility,
-                                       intraday=intraday, expiry_date=expiry_date, year_base=year_base, random_seed=0)
-        price = spot_price * gbm
-
-        M = len(price)
-
-        ki_obs_idx = np.where(knock_in_obs['obs_index'] >= 0)
-        ki_adj = knock_in_obs['adjust_rate'][ki_obs_idx]
-        ki_obs_idx = knock_in_obs['obs_index'][ki_obs_idx]
-
-        ko_obs_idx = np.where(knock_out_obs['obs_index'] >= 0)
-        ko_adj = knock_out_obs['adjust_rate'][ko_obs_idx]
-        ko_coupon = knock_out_obs['coupon_rate'][ko_obs_idx]
-        ko_obs_idx = knock_out_obs['obs_index'][ko_obs_idx]
-
-        t_arr = np.hstack([0, np.arange(1, expiry_date + 1, 1) - intraday])
-
-        assert round(expiry_date - intraday, 6) == round(t_arr[-1], 6)
-
-        knock_in_barrier_price = knock_in_barrier_price * ki_adj
-        knock_out_barrier_price = knock_out_barrier_price * ko_adj
-
-        ki_mat_flag = np.zeros((M, 1), dtype=bool) if len(ki_obs_idx) == 0 else phi * (price[:, ki_obs_idx] - knock_in_barrier_price) <= 0
-        ko_mat_flag = np.zeros((M, 1), dtype=bool) if len(ko_obs_idx) == 0 else phi * (price[:, ko_obs_idx] - knock_out_barrier_price) >= 0
-        ko_idx = (np.insert(ko_mat_flag, 0, np.zeros(M), axis=1)).argmax(axis=1)
-
-        # 敲出
-        dis_factor = 1 / np.exp(riskfree_rate * t_arr[ko_obs_idx] / year_base)
-        dis_factor = np.insert(dis_factor, 0, 0)[ko_idx]
-
-        ko_obs_price_ret = price[:, ko_obs_idx] / knock_out_barrier_price - 1
-        ko_obs_price_ret = np.insert(ko_obs_price_ret, 0, np.zeros(M), axis=1)[np.arange(M), ko_idx]
-
-        ko_payoff = dis_factor * notional * (np.where(ko_idx == 0, 0, ko_coupon[ko_idx - 1])
-                                             + np.where(ko_idx == 0, 0, phi * ko_obs_price_ret * participation_rate)
-                                             - margin_rate * np.where(ko_idx == 0, 0, np.exp(riskfree_rate * t_arr[ko_obs_idx][ko_idx - 1] / year_base) - 1))
-
-        # 敲入未敲出
-        comp_factor = np.exp(riskfree_rate * (expiry_date - intraday) / year_base)
-        dis_factor = 1 / comp_factor
-
-        ki_no_ko_arr_flag = np.logical_and(np.logical_or(is_knock_in, np.max(ki_mat_flag, axis=1)),
-                                           np.logical_not(np.max(ko_mat_flag, axis=1)))
-
-        ki_no_ko_payoff = ki_no_ko_arr_flag * dis_factor * notional * (np.maximum((floor_rate - 1), np.minimum(phi * (price[:, -1] / entrance_price - 1), 0))
-                                                                       - margin_rate * (comp_factor - 1))
-
-        # 未敲入未敲出
-        no_ki_no_ko_arr_flag = np.logical_and(np.logical_and(1 - is_knock_in, np.logical_not(np.max(ki_mat_flag, axis=1))),
-                                              np.logical_not(np.max(ko_mat_flag, axis=1)))
-
-        no_ki_no_ko_payoff = no_ki_no_ko_arr_flag * dis_factor * notional * (bonus_rate
-                                                                             - margin_rate * (comp_factor - 1))
-
-        rst = np.round(np.mean(ko_payoff + ki_no_ko_payoff + no_ki_no_ko_payoff), 8)
-        return rst
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from ..one_asset_option_base import *
 from ..vanilla.vanilla_as import Vanilla
 
 
 class RatioSpread(OneAssetOptionBase):
 
     def __calculate_present_value__(self):
-        param = Struct({})
+        param = Params()
         param['option_type'] = self.param.option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.spot_price
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
         param['volatility'] = self.param.volatility
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
         param['year_base'] = self.param.year_base
         vanilla1 = Vanilla(param)
 
-        param = Struct({})
+        param = Params()
         param['option_type'] = self.param.option_type
         param['exercise_type'] = self.param.exercise_type
         param['spot_price'] = self.param.spot_price
         param['strike_price'] = self.param.strike_price
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
         param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class RatioSpreadSeries(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = self.param.option_type
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['leverage'] = self.param.leverage
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         adjust = 0.5826 * self.param.volatility * math.sqrt(dt)
         if self.param.barrier_type == BarrierType.UP and time_to_expiry > 0:
             self.param.barrier_price = self.param.barrier_price * np.exp(adjust)
         elif self.param.barrier_type == BarrierType.DOWN and time_to_expiry > 0:
             self.param.barrier_price = self.param.barrier_price * np.exp(-adjust)
 
     def __calculate_present_value__(self) -> float:
-        param = Struct({})
+        param = Params()
         param['spot_price'] = self.param.spot_price
         param['barrier_price'] = self.param.barrier_price
         param['riskfree_rate'] = self.param.riskfree_rate
         param['dividend'] = self.param.dividend
         param['volatility'] = self.param.volatility
         param['expiry_date'] = self.param.expiry_date
         param['current_date'] = self.param.current_date
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py` & `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class VanillaSeries(OneAssetOptionBase):
 
     def __calculate_present_value__(self) -> float:
         rst = 0
         for obs in self.param.obs_date:
-            param = Struct({})
+            param = Params()
             param['option_type'] = self.param.option_type
             param['exercise_type'] = self.param.exercise_type
             param['spot_price'] = obs.obs_price if self.param.current_date > obs.obs_index else self.param.spot_price
             param['strike_price'] = self.param.strike_price
             param['expiry_date'] = obs.obs_index
             param['current_date'] = self.param.current_date
             param['volatility'] = self.param.volatility
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module/simple_pricer_engine.py` & `ht_pricing_module-0.2.3/ht_pricing_module/simple_pricer_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -250,15 +250,15 @@
         :param riskfree_rate: 无风险利率
         :param dividend: 分红率
         :param year_base: 年化天数
         :param barrier_price: 障碍价格
         :param rebate: 回扣
         :param obs_freq: 离散障碍解析解观测频率
         :param obs_date: 离散障碍MC观测日，dict， Dataframe类型
-               或RepeatedStruct返回结果: [Struct(), ...], Struct().obs_index离散观测日
+               或RepeatedStruct返回结果: [Params(), ...], Params().obs_index离散观测日
         :param is_knock_in: 1为已敲入0为未敲入
         :return: 障碍期权定价引擎
         """
 
         assert is_knock_in in [0, 1], "param: is_knock_in should be either 0 or 1"
 
         param = {}
@@ -289,15 +289,15 @@
         # DiscreteBarrier
         elif obs_type == ObsType.DISCRETE and pricing_method == PricingMethod.AS:
             param['obs_freq'] = obs_freq
             return DiscreteBarrier(param)
 
         # DiscreteBarrierMc
         elif obs_type == ObsType.DISCRETE and pricing_method == PricingMethod.MC:
-            param['obs_date'] = Struct.RepeatedStruct(obs_date)
+            param['obs_date'] = Params.RepeatedStruct(obs_date)
             return DiscreteBarrierMc(param)
 
     @classmethod
     def barrier_binary(
             cls,
             option_type:                int,
             barrier_type:               int,
@@ -401,15 +401,15 @@
         :param volatility: 波动率
         :param riskfree_rate: 无风险利率
         :param dividend: 分红率
         :param year_base: 年化天数
         :param running_avg: 已实现平均价格
         :param obs_start_date: 价格平均观测期开始日期
         :param obs_date: 离散亚式MC观测日，dict， Dataframe类型
-               或RepeatedStruct返回结果: [Struct(), ...], Struct().obs_index离散观测日，Struct().obs_price为已实现价格日
+               或RepeatedStruct返回结果: [Params(), ...], Params().obs_index离散观测日，Params().obs_price为已实现价格日
         :return: 亚式期权定价引擎
         """
 
         param = {}
         param['option_type'] = option_type
         param['exercise_type'] = exercise_type
         param['spot_price'] = spot_price
@@ -426,15 +426,15 @@
         # Asian
         if obs_type == ObsType.CONTINUOUS and pricing_method == PricingMethod.AS:
             return Asian(param)
 
         # DiscreteAsianMc
         elif obs_type == ObsType.DISCRETE and pricing_method == PricingMethod.MC:
             assert obs_date is not None, "obs_date & obs_price are required for DiscreteAsianMc"
-            param['obs_date'] = Struct.RepeatedStruct(obs_date)
+            param['obs_date'] = Params.RepeatedStruct(obs_date)
             return DiscreteAsianMc(param)
         # DiscreteAsianHhm
         elif obs_type == ObsType.DISCRETE and pricing_method == PricingMethod.AS:
             return DiscreteAsianHhm(param)
 
     @classmethod
     def basket_vanilla(
@@ -514,15 +514,15 @@
         :param current_date: 当前日
         :param volatility: 波动率
         :param riskfree_rate: 无风险利率
         :param dividend: 分红率
         :param year_base: 年化天数
         :param payoff: 到期赔付
         :param obs_date: 离散亚式MC观测日，dict， Dataframe类型
-               或RepeatedStruct返回结果: [Struct(), ...], Struct().obs_index离散观测日，Struct().obs_price为已实现价格日
+               或RepeatedStruct返回结果: [Params(), ...], Params().obs_index离散观测日，Params().obs_price为已实现价格日
         :param obs_freq 默认等于1
         :return: 二元期权定价引擎
         """
 
         param = {}
         param['option_type'] = option_type
         param['exercise_type'] = exercise_type
@@ -540,23 +540,22 @@
             obs_date = np.hstack([np.arange(math.floor(current_date) + obs_freq, expiry_date, obs_freq), expiry_date])
             obs_date = {'obs_index': obs_date}
 
         # Binary
         if obs_type == ObsType.CONTINUOUS and pricing_method == PricingMethod.AS:
             return Binary(param)
         elif obs_type == ObsType.DISCRETE and pricing_method == PricingMethod.MC:
-            param['obs_date'] = Struct.RepeatedStruct(obs_date)
+            param['obs_date'] = Params.RepeatedStruct(obs_date)
             return DiscreteBinaryMc(param)
 
     @classmethod
     def snowball(
             cls,
             notional:                   Union[int, float],
             spot_price:                 Union[int, float],
-            entrance_price:             Union[int, float],
             knock_in_barrier_price:     Union[int, float],
             knock_out_barrier_price:    Union[int, float],
             current_date:               Union[int, float],
             expiry_date:                Union[int, float],
             volatility:                 Union[int, float],
             riskfree_rate:              Union[int, float],
             dividend:                   Union[int, float],
@@ -565,15 +564,18 @@
             bonus_rate:                 Union[int, float],
             participation_rate:         Union[int, float],
             year_base:                  int,
             knock_in_obs_date:          Union[dict, list, DataFrame],
             knock_out_obs_date:         Union[dict, list, DataFrame],
             is_knock_in:                Union[int] = 0,
             option_type:                int = OptionType.STANDARD,
-            pricing_method:             int = PricingMethod.MC
+            pricing_method:             int = PricingMethod.MC,
+            is_discount:                Union[int] = 0,
+            entrance_price:             Union[int, float] = None,
+            knock_in_strike_price:      Union[int, float] = None,
     ):
         """
 
         :param option_type: 期权类型OptionType属性, STANDARD(正向), REVERSE(反向)
         :param pricing_method: 模型方法PricingMethod属性
         :param notional: 名义本金
         :param spot_price: 标的价格
@@ -586,49 +588,63 @@
         :param riskfree_rate: 无风险利率
         :param dividend: 分红率
         :param floor_rate 保护价
         :param margin_rate 保证金率
         :param bonus_rate: 到期收益率(非年化)
         :param year_base: 年化天数
         :param knock_in_obs_date: 雪球MC敲入观测日，dict， Dataframe类型
-               或RepeatedStruct返回结果: [Struct(), ...], Struct(obs_index, adjust_rate)
+               或RepeatedStruct返回结果: [Params(), ...], Struct(obs_index, adjust_rate)
         :param knock_out_obs_date: 雪球MC敲出观测日，dict， Dataframe类型
-               或RepeatedStruct返回结果: [Struct(), ...], Struct(obs_index, adjust_rate, coupon_rate)
+               或RepeatedStruct返回结果: [Params(), ...], Struct(obs_index, adjust_rate, coupon_rate)
         :param is_knock_in: 1为已敲入0为未敲入
         :param participation_rate: 增强雪球敲出参与率
+        :param is_discount: 是否为折价减仓雪球
+        :param knock_in_strike_price 折价建仓雪球执行价
         :return: 雪球期权定价引擎
         """
 
         assert is_knock_in in [0, 1], "param: is_knock_in should be either 0 or 1"
+        assert is_discount in [0, 1], "param: is_discount should be either 0 or 1"
         assert option_type in [OptionType.STANDARD, OptionType.REVERSE], option_type
 
         param = {}
         param['option_type'] = option_type
         param['notional'] = notional
         param['spot_price'] = spot_price
-        param['entrance_price'] = entrance_price
         param['knock_in_barrier_price'] = knock_in_barrier_price
         param['knock_out_barrier_price'] = knock_out_barrier_price
         param['floor_rate'] = floor_rate
         param['margin_rate'] = margin_rate
         param['bonus_rate'] = bonus_rate
         param['is_knock_in'] = is_knock_in
         param['riskfree_rate'] = riskfree_rate
         param['dividend'] = dividend
         param['volatility'] = volatility
         param['current_date'] = current_date
         param['expiry_date'] = expiry_date
         param['year_base'] = year_base
-        param['knock_in_obs_date'] = Struct.RepeatedStruct(knock_in_obs_date)
-        param['knock_out_obs_date'] = Struct.RepeatedStruct(knock_out_obs_date)
+        param['knock_in_obs_date'] = Params.RepeatedStruct(knock_in_obs_date)
+        param['knock_out_obs_date'] = Params.RepeatedStruct(knock_out_obs_date)
         param['participation_rate'] = participation_rate
 
+        if entrance_price is None:
+            param['entrance_price'] = spot_price
+        else:
+            param['entrance_price'] = entrance_price
+
         # SnowballMc
-        if pricing_method == PricingMethod.MC:
+        if not is_discount and pricing_method == PricingMethod.MC:
             return SnowballMc(param)
+        # SnowballDiscountMc
+        elif is_discount and pricing_method == PricingMethod.MC:
+            if knock_in_strike_price is None:
+                param['knock_in_strike_price'] = knock_in_barrier_price
+            else:
+                param['knock_in_strike_price'] = knock_in_strike_price
+            return SnowballDiscountedMc(param)
 
     @classmethod
     def airbag(
             cls,
             spot_price:                 Union[int, float],
             strike_price:               Union[int, float],
             barrier_price:              Union[int, float],
@@ -636,14 +652,16 @@
             current_date:               Union[int, float],
             volatility:                 Union[int, float],
             riskfree_rate:              Union[int, float],
             dividend:                   Union[int, float],
             year_base:                  int,
             participation_rate:         Union[int, float],
             is_knock_in:                Union[int] = 0,
+            is_capped:                  Union[int] = 0,
+            cap_price:                  Union[int, float] = None,
             obs_freq:                   Union[float, int] = 1,
             option_type:                int = OptionType.STANDARD,
             exercise_type:              int = ExerciseType.EUROPEAN,
             pricing_method:             int = PricingMethod.AS,
             obs_type:                   int = ObsType.DISCRETE
     ):
         """
@@ -660,18 +678,22 @@
         :param riskfree_rate: 无风险利率
         :param dividend: 分红率
         :param year_base: 年化天数
         :param participation_rate 参与率
         :param barrier_price: 障碍价格
         :param obs_freq: 离散障碍解析解观测频率
         :param is_knock_in: 1为已敲入0为未敲入
+        :param is_capped: 是否对收益封顶
+        :param cap_price: 封顶价格
         :return: 安全气囊期权定价引擎
         """
 
         assert is_knock_in in [0, 1], "param: is_knock_in should be either 0 or 1"
+        assert is_capped in [0, 1], "param: is_capped should be either 0 or 1"
+        assert (is_capped == 1 and cap_price is not None) or not is_capped, "cap price should be given"
         assert option_type in [OptionType.STANDARD, OptionType.REVERSE], option_type
 
         param = {}
         param['option_type'] = option_type
         param['exercise_type'] = exercise_type
         param['spot_price'] = spot_price
         param['strike_price'] = strike_price
@@ -680,14 +702,16 @@
         param['volatility'] = volatility
         param['riskfree_rate'] = riskfree_rate
         param['dividend'] = dividend
         param['year_base'] = year_base
         param['barrier_price'] = barrier_price
         param['participation_rate'] = participation_rate
         param['is_knock_in'] = is_knock_in
+        param['is_capped'] = is_capped
+        param['cap_price'] = cap_price
 
         # Airbag
         if obs_type == ObsType.DISCRETE and pricing_method == PricingMethod.AS:
             param['obs_freq'] = obs_freq
             return Airbag(param)
 
     @classmethod
@@ -728,15 +752,15 @@
         :param dividend: 分红率
         :param leverage: 杠杆倍数
         :param year_base: 年化天数
         :param barrier_price: "LinearAcc，FixedAccBarrier, LinearAccAko, FixedAccAko, FixedAccEnhanced, LinearAccEnhanced必填参数" 障碍价格
         :param payoff: "FixedAcc，FixedAccBarrier, FixedAccAko, FixedAccEnhanced, LinearAccAko必填参数" rebate
         :param final_position_multiplier: 熔断累计到期日建仓乘数
         :param obs_date: 观测日，dict， Dataframe类型，默认每天到期一笔
-               或RepeatedStruct返回结果: [Struct(), ...], Struct().obs_index离散观测日，Struct().obs_price为已实现价格日
+               或RepeatedStruct返回结果: [Params(), ...], Params().obs_index离散观测日，Params().obs_price为已实现价格日
         :param obs_freq 默认为1，每天到期一笔
         :param base_quantity 每日观察数量
         :return: 累计期权定价引擎
         """
 
         assert option_type in [OptionType.ACCUMULATOR, OptionType.DECUMULATOR], option_type
 
@@ -756,15 +780,15 @@
         param['dividend'] = dividend
         param['leverage'] = leverage
         param['year_base'] = year_base
 
         if obs_date is None:
             obs_date = np.hstack([np.arange(math.floor(current_date) + obs_freq, expiry_date, obs_freq), expiry_date])
             obs_date = {'obs_index': obs_date, 'obs_price': np.ones_like(obs_date) * spot_price}
-        param['obs_date'] = Struct.RepeatedStruct(obs_date)
+        param['obs_date'] = Params.RepeatedStruct(obs_date)
 
         # LinearAcc
         if pricing_method == PricingMethod.AS and accumulator_type == AccumulatorType.LINEAR_ACC:
             assert barrier_price is not None, "barrier is required for LinearAcc"
             param['barrier_price'] = barrier_price
             return LinearAcc(param)
 
@@ -876,15 +900,15 @@
         param['strike_price'] = strike_price
         param['expiry_date'] = expiry_date
         param['current_date'] = current_date
         param['volatility'] = volatility
         param['riskfree_rate'] = riskfree_rate
         param['dividend'] = dividend
         param['year_base'] = year_base
-        param['obs_date'] = Struct.RepeatedStruct(obs_date)
+        param['obs_date'] = Params.RepeatedStruct(obs_date)
 
         # enhanced_asian
         if pricing_method == PricingMethod.AS:
             return VanillaSeries(param)
 
     @classmethod
     def touch(
```

### Comparing `ht_pricing_module-0.2.2/ht_pricing_module.egg-info/SOURCES.txt` & `ht_pricing_module-0.2.3/ht_pricing_module.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 ht_pricing_module/one_asset_pricing_module/forward/__init__.py
 ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
 ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
 ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
 ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
 ht_pricing_module/one_asset_pricing_module/spread/__init__.py
 ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
 ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
 ht_pricing_module/one_asset_pricing_module/touch/__init__.py
 ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
 ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
```

### Comparing `ht_pricing_module-0.2.2/setup.py` & `ht_pricing_module-0.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.2.2"
+VERSION = "0.2.3"
 
 
 def filter_package():
     packages = []
     packages_all = find_packages()
     for i in packages_all:
         if i.split(".")[0] == 'ht_pricing_module':
```

