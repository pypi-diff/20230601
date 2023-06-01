# Comparing `tmp/ht_pricing_module-0.2.3.tar.gz` & `tmp/ht_pricing_module-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ht_pricing_module-0.2.3.tar", last modified: Thu Jun  1 06:42:19 2023, max compression
+gzip compressed data, was "ht_pricing_module-0.2.4.tar", last modified: Thu Jun  1 06:55:38 2023, max compression
```

## Comparing `ht_pricing_module-0.2.3.tar` & `ht_pricing_module-0.2.4.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.135361 ht_pricing_module-0.2.3/
--rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.2.3/MANIFEST.in
--rw-rw-rw-   0        0        0      263 2023-06-01 06:42:19.135361 ht_pricing_module-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      142 2023-06-01 06:41:58.000000 ht_pricing_module-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.671866 ht_pricing_module-0.2.3/ht_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.2.3/ht_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.698794 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/
--rw-rw-rw-   0        0        0      258 2023-05-18 02:19:46.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/__init__.py
--rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/api.py
--rw-rw-rw-   0        0        0      468 2023-05-29 08:11:33.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/packages.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.712761 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/
--rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.660894 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.735699 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/api/
--rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
--rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/api/http.proto
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.771826 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/protobuf/
--rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
--rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
--rw-rw-rw-   0        0        0    47780 2023-05-31 11:41:37.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/pricer.proto
--rw-rw-rw-   0        0        0     3252 2023-05-16 06:25:50.000000 ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.784791 ht_pricing_module-0.2.3/ht_pricing_module/finite_difference_engine/
--rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/finite_difference_engine/__init__.py
--rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.2.3/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.795762 ht_pricing_module-0.2.3/ht_pricing_module/monte_carlo_engine/
--rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/monte_carlo_engine/__init__.py
--rw-rw-rw-   0        0        0     3268 2023-04-11 05:44:47.000000 ht_pricing_module-0.2.3/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.807729 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/
--rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/__init__.py
--rw-rw-rw-   0        0        0     4526 2023-05-16 06:27:30.000000 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.820695 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/quotient/
--rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.835655 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/
--rw-rw-rw-   0        0        0      341 2023-05-11 09:39:17.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.940567 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/
--rw-rw-rw-   0        0        0      583 2023-04-25 03:15:40.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
--rw-rw-rw-   0        0        0     4087 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
--rw-rw-rw-   0        0        0     3320 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
--rw-rw-rw-   0        0        0     4103 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
--rw-rw-rw-   0        0        0     4843 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
--rw-rw-rw-   0        0        0     4190 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4014 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
--rw-rw-rw-   0        0        0     3368 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
--rw-rw-rw-   0        0        0     4238 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
--rw-rw-rw-   0        0        0     4318 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
--rw-rw-rw-   0        0        0     5002 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
--rw-rw-rw-   0        0        0     5254 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.953531 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/airbag/
--rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
--rw-rw-rw-   0        0        0     5089 2023-05-22 02:39:06.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.985446 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/
--rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
--rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
--rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
--rw-rw-rw-   0        0        0     2280 2023-05-31 05:05:32.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.012690 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/
--rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
--rw-rw-rw-   0        0        0     6174 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
--rw-rw-rw-   0        0        0     5338 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
--rw-rw-rw-   0        0        0     1874 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
--rw-rw-rw-   0        0        0     1795 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
--rw-rw-rw-   0        0        0     4425 2023-05-31 05:05:32.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.039617 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/
--rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
--rw-rw-rw-   0        0        0     1135 2023-04-26 06:32:51.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
--rw-rw-rw-   0        0        0     2316 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.062556 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/
--rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
--rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
--rw-rw-rw-   0        0        0     2320 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
--rw-rw-rw-   0        0        0     2261 2023-05-31 05:04:39.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
--rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.064551 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/forward/
--rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
--rw-rw-rw-   0        0        0      198 2023-04-26 05:49:02.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
--rw-rw-rw-   0        0        0     5680 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.076519 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/
--rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
--rw-rw-rw-   0        0        0     2526 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
--rw-rw-rw-   0        0        0     2348 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
--rw-rw-rw-   0        0        0     3902 2023-05-16 06:54:45.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.086492 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/
--rw-rw-rw-   0        0        0       95 2023-05-31 06:13:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
--rw-rw-rw-   0        0        0     5712 2023-05-31 11:47:11.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
--rw-rw-rw-   0        0        0     6593 2023-05-31 05:04:39.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.096465 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/
--rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
--rw-rw-rw-   0        0        0     1481 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
--rw-rw-rw-   0        0        0     2414 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.117410 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/
--rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
--rw-rw-rw-   0        0        0     1654 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
--rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
--rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:19.123392 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/
--rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
--rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
--rw-rw-rw-   0        0        0     2278 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
--rw-rw-rw-   0        0        0    45281 2023-05-31 06:13:28.000000 ht_pricing_module-0.2.3/ht_pricing_module/simple_pricer_engine.py
-drwxrwxrwx   0        0        0        0 2023-06-01 06:42:18.683833 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/
--rw-rw-rw-   0        0        0      263 2023-06-01 06:42:18.000000 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     5035 2023-06-01 06:42:18.000000 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 06:42:18.000000 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       94 2023-06-01 06:42:18.000000 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-01 06:42:18.000000 ht_pricing_module-0.2.3/ht_pricing_module.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 06:42:19.136358 ht_pricing_module-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1158 2023-06-01 06:41:57.000000 ht_pricing_module-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:38.022680 ht_pricing_module-0.2.4/
+-rw-rw-rw-   0        0        0       66 2023-02-17 02:37:54.000000 ht_pricing_module-0.2.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      263 2023-06-01 06:55:38.021682 ht_pricing_module-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      142 2023-06-01 06:54:49.000000 ht_pricing_module-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.940898 ht_pricing_module-0.2.4/ht_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-02-20 08:18:37.000000 ht_pricing_module-0.2.4/ht_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.951869 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/
+-rw-rw-rw-   0        0        0      258 2023-05-18 02:19:46.000000 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/__init__.py
+-rw-rw-rw-   0        0        0      719 2023-02-22 11:10:26.000000 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/api.py
+-rw-rw-rw-   0        0        0      468 2023-05-29 08:11:33.000000 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/packages.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.953863 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/
+-rw-rw-rw-   0        0        0      145 2023-02-17 02:31:14.000000 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.930926 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.954861 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/api/
+-rw-rw-rw-   0        0        0     1076 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto
+-rw-rw-rw-   0        0        0    15515 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/api/http.proto
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.956855 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/protobuf/
+-rw-rw-rw-   0        0        0     6072 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto
+-rw-rw-rw-   0        0        0    38952 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto
+-rw-rw-rw-   0        0        0    47780 2023-05-31 11:41:37.000000 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/pricer.proto
+-rw-rw-rw-   0        0        0     3252 2023-05-16 06:25:50.000000 ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.958851 ht_pricing_module-0.2.4/ht_pricing_module/finite_difference_engine/
+-rw-rw-rw-   0        0        0        0 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/finite_difference_engine/__init__.py
+-rw-rw-rw-   0        0        0     4815 2023-02-13 08:19:41.000000 ht_pricing_module-0.2.4/ht_pricing_module/finite_difference_engine/fd_grid_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.960846 ht_pricing_module-0.2.4/ht_pricing_module/monte_carlo_engine/
+-rw-rw-rw-   0        0        0       34 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/monte_carlo_engine/__init__.py
+-rw-rw-rw-   0        0        0     3268 2023-04-11 05:44:47.000000 ht_pricing_module-0.2.4/ht_pricing_module/monte_carlo_engine/mc_path_generator.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.963838 ht_pricing_module-0.2.4/ht_pricing_module/multi_asset_pricing_module/
+-rw-rw-rw-   0        0        0       84 2023-03-22 14:26:39.000000 ht_pricing_module-0.2.4/ht_pricing_module/multi_asset_pricing_module/__init__.py
+-rw-rw-rw-   0        0        0     4526 2023-05-16 06:27:30.000000 ht_pricing_module-0.2.4/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.965832 ht_pricing_module-0.2.4/ht_pricing_module/multi_asset_pricing_module/quotient/
+-rw-rw-rw-   0        0        0       35 2023-03-22 14:53:46.000000 ht_pricing_module-0.2.4/ht_pricing_module/multi_asset_pricing_module/quotient/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-03-23 01:15:31.000000 ht_pricing_module-0.2.4/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.967827 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/
+-rw-rw-rw-   0        0        0      341 2023-05-11 09:39:17.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.981789 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/
+-rw-rw-rw-   0        0        0      583 2023-04-25 03:15:40.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py
+-rw-rw-rw-   0        0        0     4087 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3320 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py
+-rw-rw-rw-   0        0        0     4103 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py
+-rw-rw-rw-   0        0        0     4843 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py
+-rw-rw-rw-   0        0        0     4190 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4014 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py
+-rw-rw-rw-   0        0        0     3368 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py
+-rw-rw-rw-   0        0        0     4238 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py
+-rw-rw-rw-   0        0        0     4318 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py
+-rw-rw-rw-   0        0        0     5002 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py
+-rw-rw-rw-   0        0        0     5254 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.983783 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/airbag/
+-rw-rw-rw-   0        0        0       31 2023-02-13 05:55:38.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/airbag/__init__.py
+-rw-rw-rw-   0        0        0     5089 2023-05-22 02:39:06.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.986775 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/asian/
+-rw-rw-rw-   0        0        0      127 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/asian/__init__.py
+-rw-rw-rw-   0        0        0     4055 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py
+-rw-rw-rw-   0        0        0     3643 2023-03-20 07:54:08.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py
+-rw-rw-rw-   0        0        0     2280 2023-05-31 05:05:32.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.992763 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/
+-rw-rw-rw-   0        0        0      246 2023-02-13 02:54:44.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/__init__.py
+-rw-rw-rw-   0        0        0     6174 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py
+-rw-rw-rw-   0        0        0     5338 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py
+-rw-rw-rw-   0        0        0     1874 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py
+-rw-rw-rw-   0        0        0     1795 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py
+-rw-rw-rw-   0        0        0     4425 2023-05-31 05:05:32.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.995752 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/basket/
+-rw-rw-rw-   0        0        0      102 2023-02-17 01:46:21.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/basket/__init__.py
+-rw-rw-rw-   0        0        0     1135 2023-04-26 06:32:51.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py
+-rw-rw-rw-   0        0        0     2316 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.999741 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/binary/
+-rw-rw-rw-   0        0        0      122 2023-03-10 05:05:19.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/binary/__init__.py
+-rw-rw-rw-   0        0        0     2979 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py
+-rw-rw-rw-   0        0        0     2320 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py
+-rw-rw-rw-   0        0        0     2261 2023-05-31 05:04:39.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py
+-rw-rw-rw-   0        0        0      108 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:38.001735 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/forward/
+-rw-rw-rw-   0        0        0       33 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/forward/__init__.py
+-rw-rw-rw-   0        0        0      198 2023-04-26 05:49:02.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/forward/forward_as.py
+-rw-rw-rw-   0        0        0     5680 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:38.004728 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/sharkfin/
+-rw-rw-rw-   0        0        0       80 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/sharkfin/__init__.py
+-rw-rw-rw-   0        0        0     2526 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py
+-rw-rw-rw-   0        0        0     2348 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py
+-rw-rw-rw-   0        0        0     3902 2023-05-16 06:54:45.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:38.009748 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/snowball/
+-rw-rw-rw-   0        0        0       95 2023-05-31 06:13:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/snowball/__init__.py
+-rw-rw-rw-   0        0        0     5712 2023-05-31 11:47:11.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py
+-rw-rw-rw-   0        0        0     6593 2023-05-31 05:04:39.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:38.012712 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/spread/
+-rw-rw-rw-   0        0        0       94 2023-02-13 03:17:56.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/spread/__init__.py
+-rw-rw-rw-   0        0        0     1481 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py
+-rw-rw-rw-   0        0        0     2414 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:38.017693 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/touch/
+-rw-rw-rw-   0        0        0      138 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/touch/__init__.py
+-rw-rw-rw-   0        0        0     1654 2023-05-16 06:22:28.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py
+-rw-rw-rw-   0        0        0     5949 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py
+-rw-rw-rw-   0        0        0     3942 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:38.019688 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/vanilla/
+-rw-rw-rw-   0        0        0       76 2023-02-11 06:25:49.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/vanilla/__init__.py
+-rw-rw-rw-   0        0        0     1060 2023-03-20 07:48:15.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py
+-rw-rw-rw-   0        0        0     2278 2023-05-16 06:22:27.000000 ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py
+-rw-rw-rw-   0        0        0    45285 2023-06-01 06:53:57.000000 ht_pricing_module-0.2.4/ht_pricing_module/simple_pricer_engine.py
+drwxrwxrwx   0        0        0        0 2023-06-01 06:55:37.946886 ht_pricing_module-0.2.4/ht_pricing_module.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-06-01 06:55:37.000000 ht_pricing_module-0.2.4/ht_pricing_module.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     5035 2023-06-01 06:55:37.000000 ht_pricing_module-0.2.4/ht_pricing_module.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 06:55:37.000000 ht_pricing_module-0.2.4/ht_pricing_module.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       94 2023-06-01 06:55:37.000000 ht_pricing_module-0.2.4/ht_pricing_module.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 06:55:37.000000 ht_pricing_module-0.2.4/ht_pricing_module.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 06:55:38.022680 ht_pricing_module-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     1158 2023-06-01 06:54:49.000000 ht_pricing_module-0.2.4/setup.py
```

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/api.py` & `ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/api.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto` & `ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/api/annotations.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/api/http.proto` & `ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/api/http.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto` & `ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/protobuf/any.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto` & `ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/google/protobuf/descriptor.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/protos/pricer.proto` & `ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/protos/pricer.proto`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/api_and_utils/utils.py` & `ht_pricing_module-0.2.4/ht_pricing_module/api_and_utils/utils.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/finite_difference_engine/fd_grid_generator.py` & `ht_pricing_module-0.2.4/ht_pricing_module/finite_difference_engine/fd_grid_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/monte_carlo_engine/mc_path_generator.py` & `ht_pricing_module-0.2.4/ht_pricing_module/monte_carlo_engine/mc_path_generator.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py` & `ht_pricing_module-0.2.4/ht_pricing_module/multi_asset_pricing_module/multi_asset_option_base.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/multi_asset_pricing_module/quotient/quotient_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/__init__.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_ako_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_barrier_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/fixed_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_ako_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fixed_enhanced_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/accumulator/linear_acc_fusing_trans_forward_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/airbag/airbag_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/asian/asian_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_hhm.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/asian/discrete_asian_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/barrier/discrete_barrier_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/basket/basket_vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/binary/binary_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/binary/binary_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/binary/discrete_binary_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/one_asset_option_base.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/sharkfin/sharkfin_yield_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/snowball/snowball_discounted_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/snowball/snowball_mc.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/spread/ratio_spread_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/touch/discrete_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/touch/double_one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/touch/one_touch_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_as.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py` & `ht_pricing_module-0.2.4/ht_pricing_module/one_asset_pricing_module/vanilla/vanilla_series.py`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module/simple_pricer_engine.py` & `ht_pricing_module-0.2.4/ht_pricing_module/simple_pricer_engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -558,21 +558,21 @@
             expiry_date:                Union[int, float],
             volatility:                 Union[int, float],
             riskfree_rate:              Union[int, float],
             dividend:                   Union[int, float],
             floor_rate:                 Union[int, float],
             margin_rate:                Union[int, float],
             bonus_rate:                 Union[int, float],
-            participation_rate:         Union[int, float],
             year_base:                  int,
             knock_in_obs_date:          Union[dict, list, DataFrame],
             knock_out_obs_date:         Union[dict, list, DataFrame],
             is_knock_in:                Union[int] = 0,
             option_type:                int = OptionType.STANDARD,
             pricing_method:             int = PricingMethod.MC,
+            participation_rate:         Union[int, float] = 0,
             is_discount:                Union[int] = 0,
             entrance_price:             Union[int, float] = None,
             knock_in_strike_price:      Union[int, float] = None,
     ):
         """
 
         :param option_type: 期权类型OptionType属性, STANDARD(正向), REVERSE(反向)
```

### Comparing `ht_pricing_module-0.2.3/ht_pricing_module.egg-info/SOURCES.txt` & `ht_pricing_module-0.2.4/ht_pricing_module.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ht_pricing_module-0.2.3/setup.py` & `ht_pricing_module-0.2.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = "0.2.3"
+VERSION = "0.2.4"
 
 
 def filter_package():
     packages = []
     packages_all = find_packages()
     for i in packages_all:
         if i.split(".")[0] == 'ht_pricing_module':
```

