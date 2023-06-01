# Comparing `tmp/quantplay-1.2.91.tar.gz` & `tmp/quantplay-1.2.92.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantplay-1.2.91.tar", last modified: Wed May 31 03:19:03 2023, max compression
+gzip compressed data, was "quantplay-1.2.92.tar", last modified: Thu Jun  1 01:35:57 2023, max compression
```

## Comparing `quantplay-1.2.91.tar` & `quantplay-1.2.92.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.366793 quantplay-1.2.91/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-05-31 03:19:03.366861 quantplay-1.2.91/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.2.91/README.md
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.350043 quantplay-1.2.91/quantplay/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.351212 quantplay-1.2.91/quantplay/backtest/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/backtest/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.2.91/quantplay/backtest/backtest_trades.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.354021 quantplay-1.2.91/quantplay/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/angelone.py
--rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/broker_client.py
--rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/client.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.354472 quantplay-1.2.91/quantplay/broker/finvasia_utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/finvasia_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.2.91/quantplay/broker/finvasia_utils/shoonya.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.354867 quantplay-1.2.91/quantplay/broker/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.2.91/quantplay/broker/generics/broker.py
--rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.2.91/quantplay/broker/iifl.py
--rw-r--r--   0 ashok      (502) staff       (20)      587 2023-05-10 06:43:57.000000 quantplay-1.2.91/quantplay/broker/iifl_xts.py
--rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/kite_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/motilal.py
--rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.2.91/quantplay/broker/shoonya.py
--rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.2.91/quantplay/broker/symphony.py
--rw-r--r--   0 ashok      (502) staff       (20)    17888 2023-05-31 03:18:14.000000 quantplay-1.2.91/quantplay/broker/xts.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.356357 quantplay-1.2.91/quantplay/broker/xts_utils/
--rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.2.91/quantplay/broker/xts_utils/Connect.py
--rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/xts_utils/Exception.py
--rw-r--r--   0 ashok      (502) staff       (20)     6450 2023-05-19 15:50:30.000000 quantplay-1.2.91/quantplay/broker/xts_utils/InteractiveSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/xts_utils/MarketDataSocketClient.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/broker/xts_utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    17192 2023-05-23 09:41:25.000000 quantplay-1.2.91/quantplay/broker/zerodha.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.356482 quantplay-1.2.91/quantplay/brokerage/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/brokerage/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.356718 quantplay-1.2.91/quantplay/brokerage/angelone/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/brokerage/angelone/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/brokerage/angelone/angel_broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.357176 quantplay-1.2.91/quantplay/brokerage/generics/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/brokerage/generics/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.2.91/quantplay/brokerage/generics/broker.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.357887 quantplay-1.2.91/quantplay/brokerage/zerodha/
--rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.2.91/quantplay/brokerage/zerodha/ZBroker.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/brokerage/zerodha/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.358078 quantplay-1.2.91/quantplay/config/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/config/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/config/qplay_config.py
--rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/create_sample_data.py
--rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.2.91/quantplay/data_modify_script.py
--rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-04-19 06:37:00.000000 quantplay-1.2.91/quantplay/date_fix.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.358347 quantplay-1.2.91/quantplay/exception/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/exception/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/exception/exceptions.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.358646 quantplay-1.2.91/quantplay/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.359259 quantplay-1.2.91/quantplay/indicators/
--rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/indicators/Indicator.py
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/indicators/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/indicators/atr.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.359434 quantplay-1.2.91/quantplay/model/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/model/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.360071 quantplay-1.2.91/quantplay/model/exchange/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/model/exchange/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/model/exchange/instrument.py
--rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.2.91/quantplay/model/exchange/order.py
--rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/model/exchange/tick.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.360325 quantplay-1.2.91/quantplay/model/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/model/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/model/strategy/strategy_response.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.360462 quantplay-1.2.91/quantplay/oms/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/oms/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.360843 quantplay-1.2.91/quantplay/order_execution/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/order_execution/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/order_execution/execution_algorithm.py
--rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/order_execution/mean_price.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.361267 quantplay-1.2.91/quantplay/reporting/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/reporting/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    10780 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/reporting/strategy_report.py
--rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.2.91/quantplay/reporting/visuals.py
--rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.2.91/quantplay/service.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.362042 quantplay-1.2.91/quantplay/services/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/services/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.2.91/quantplay/services/market.py
--rw-r--r--   0 ashok      (502) staff       (20)    11801 2023-05-31 03:18:14.000000 quantplay-1.2.91/quantplay/services/tradelens.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.362203 quantplay-1.2.91/quantplay/strategies/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.91/quantplay/strategies/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.362297 quantplay-1.2.91/quantplay/strategies/equities/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.91/quantplay/strategies/equities/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.362391 quantplay-1.2.91/quantplay/strategies/equities/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.91/quantplay/strategies/equities/intraday/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.362486 quantplay-1.2.91/quantplay/strategies/equities/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.91/quantplay/strategies/equities/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.362588 quantplay-1.2.91/quantplay/strategies/futures/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.91/quantplay/strategies/futures/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.362682 quantplay-1.2.91/quantplay/strategies/futures/overnight/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.91/quantplay/strategies/futures/overnight/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.362768 quantplay-1.2.91/quantplay/strategies/options/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.91/quantplay/strategies/options/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.363537 quantplay-1.2.91/quantplay/strategies/options/intraday/
--rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.91/quantplay/strategies/options/intraday/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.91/quantplay/strategies/options/intraday/ladder.py
--rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.91/quantplay/strategies/options/intraday/musk.py
--rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.91/quantplay/strategies/options/intraday/short_straddle.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.363904 quantplay-1.2.91/quantplay/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.2.91/quantplay/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.91/quantplay/strategy_run.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.365484 quantplay-1.2.91/quantplay/utils/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/utils/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/utils/config_util.py
--rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.2.91/quantplay/utils/constant.py
--rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.2.91/quantplay/utils/data_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/utils/exchange.py
--rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/utils/number_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/utils/pickle_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/utils/selenium_utils.py
--rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.2.91/quantplay/utils/transaction_utils.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.350963 quantplay-1.2.91/quantplay.egg-info/
--rw-r--r--   0 ashok      (502) staff       (20)      663 2023-05-31 03:19:03.000000 quantplay-1.2.91/quantplay.egg-info/PKG-INFO
--rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-05-31 03:19:03.000000 quantplay-1.2.91/quantplay.egg-info/SOURCES.txt
--rw-r--r--   0 ashok      (502) staff       (20)        1 2023-05-31 03:19:03.000000 quantplay-1.2.91/quantplay.egg-info/dependency_links.txt
--rw-r--r--   0 ashok      (502) staff       (20)      221 2023-05-31 03:19:03.000000 quantplay-1.2.91/quantplay.egg-info/requires.txt
--rw-r--r--   0 ashok      (502) staff       (20)       15 2023-05-31 03:19:03.000000 quantplay-1.2.91/quantplay.egg-info/top_level.txt
--rw-r--r--   0 ashok      (502) staff       (20)       49 2023-05-31 03:19:03.367089 quantplay-1.2.91/setup.cfg
--rw-r--r--   0 ashok      (502) staff       (20)      876 2023-05-31 03:18:51.000000 quantplay-1.2.91/setup.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.365728 quantplay-1.2.91/test/
--rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.91/test/__init__.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.365973 quantplay-1.2.91/test/broker/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/test/broker/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.2.91/test/broker/finvasia.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.366203 quantplay-1.2.91/test/executor/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/test/executor/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.2.91/test/executor/strategy_executor.py
-drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-05-31 03:19:03.366636 quantplay-1.2.91/test/strategy/
--rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.91/test/strategy/__init__.py
--rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.2.91/test/strategy/base.py
--rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.2.91/test/strategy/sample_strategy.py
--rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.2.91/test/test_motilal.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.034473 quantplay-1.2.92/
+-rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-01 01:35:57.034535 quantplay-1.2.92/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)      494 2023-04-19 06:36:45.000000 quantplay-1.2.92/README.md
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.020378 quantplay-1.2.92/quantplay/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.021294 quantplay-1.2.92/quantplay/backtest/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/backtest/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17605 2023-05-17 07:17:28.000000 quantplay-1.2.92/quantplay/backtest/backtest_trades.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.023444 quantplay-1.2.92/quantplay/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10902 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/angelone.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3738 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/broker_client.py
+-rw-r--r--   0 ashok      (502) staff       (20)       87 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/client.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.024034 quantplay-1.2.92/quantplay/broker/finvasia_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/finvasia_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2576 2023-05-11 13:49:53.000000 quantplay-1.2.92/quantplay/broker/finvasia_utils/shoonya.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.024354 quantplay-1.2.92/quantplay/broker/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28802 2023-05-26 07:56:12.000000 quantplay-1.2.92/quantplay/broker/generics/broker.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3897 2023-05-17 07:17:28.000000 quantplay-1.2.92/quantplay/broker/iifl.py
+-rw-r--r--   0 ashok      (502) staff       (20)      588 2023-06-01 01:35:25.000000 quantplay-1.2.92/quantplay/broker/iifl_xts.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2002 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/kite_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)    31836 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/motilal.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19618 2023-05-11 13:57:44.000000 quantplay-1.2.92/quantplay/broker/shoonya.py
+-rw-r--r--   0 ashok      (502) staff       (20)      515 2023-04-19 06:37:00.000000 quantplay-1.2.92/quantplay/broker/symphony.py
+-rw-r--r--   0 ashok      (502) staff       (20)    19042 2023-06-01 01:35:25.000000 quantplay-1.2.92/quantplay/broker/xts.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.025424 quantplay-1.2.92/quantplay/broker/xts_utils/
+-rw-r--r--   0 ashok      (502) staff       (20)    33446 2023-04-24 08:10:10.000000 quantplay-1.2.92/quantplay/broker/xts_utils/Connect.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3046 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/xts_utils/Exception.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6450 2023-05-19 15:50:30.000000 quantplay-1.2.92/quantplay/broker/xts_utils/InteractiveSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)     9106 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/xts_utils/MarketDataSocketClient.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/broker/xts_utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    17192 2023-05-23 09:41:25.000000 quantplay-1.2.92/quantplay/broker/zerodha.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.025512 quantplay-1.2.92/quantplay/brokerage/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/brokerage/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.025811 quantplay-1.2.92/quantplay/brokerage/angelone/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/brokerage/angelone/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10989 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/brokerage/angelone/angel_broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.026089 quantplay-1.2.92/quantplay/brokerage/generics/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/brokerage/generics/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    28081 2023-04-26 18:39:03.000000 quantplay-1.2.92/quantplay/brokerage/generics/broker.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.026578 quantplay-1.2.92/quantplay/brokerage/zerodha/
+-rw-r--r--   0 ashok      (502) staff       (20)    17690 2023-04-24 06:31:05.000000 quantplay-1.2.92/quantplay/brokerage/zerodha/ZBroker.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/brokerage/zerodha/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.026845 quantplay-1.2.92/quantplay/config/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/config/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1461 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/config/qplay_config.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1127 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/create_sample_data.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1725 2023-04-19 06:37:00.000000 quantplay-1.2.92/quantplay/data_modify_script.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3481 2023-04-19 06:37:00.000000 quantplay-1.2.92/quantplay/date_fix.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.027137 quantplay-1.2.92/quantplay/exception/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/exception/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2162 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/exception/exceptions.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.027449 quantplay-1.2.92/quantplay/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     6064 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.027984 quantplay-1.2.92/quantplay/indicators/
+-rw-r--r--   0 ashok      (502) staff       (20)     1747 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/indicators/Indicator.py
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/indicators/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      455 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/indicators/atr.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.028139 quantplay-1.2.92/quantplay/model/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/model/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.028655 quantplay-1.2.92/quantplay/model/exchange/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/model/exchange/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1472 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/model/exchange/instrument.py
+-rw-r--r--   0 ashok      (502) staff       (20)     8794 2023-05-17 08:03:33.000000 quantplay-1.2.92/quantplay/model/exchange/order.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3238 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/model/exchange/tick.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.028895 quantplay-1.2.92/quantplay/model/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/model/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      206 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/model/strategy/strategy_response.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.029024 quantplay-1.2.92/quantplay/oms/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/oms/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.029362 quantplay-1.2.92/quantplay/order_execution/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/order_execution/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2048 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/order_execution/execution_algorithm.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1281 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/order_execution/mean_price.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.029722 quantplay-1.2.92/quantplay/reporting/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/reporting/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    10780 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/reporting/strategy_report.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1521 2023-04-19 06:37:00.000000 quantplay-1.2.92/quantplay/reporting/visuals.py
+-rw-r--r--   0 ashok      (502) staff       (20)      231 2023-04-24 06:31:05.000000 quantplay-1.2.92/quantplay/service.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.030171 quantplay-1.2.92/quantplay/services/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/services/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    18366 2023-05-26 07:55:13.000000 quantplay-1.2.92/quantplay/services/market.py
+-rw-r--r--   0 ashok      (502) staff       (20)    11801 2023-05-31 03:18:14.000000 quantplay-1.2.92/quantplay/services/tradelens.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.030283 quantplay-1.2.92/quantplay/strategies/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:41.000000 quantplay-1.2.92/quantplay/strategies/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.030375 quantplay-1.2.92/quantplay/strategies/equities/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:09.000000 quantplay-1.2.92/quantplay/strategies/equities/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.030464 quantplay-1.2.92/quantplay/strategies/equities/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:48:26.000000 quantplay-1.2.92/quantplay/strategies/equities/intraday/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.030555 quantplay-1.2.92/quantplay/strategies/equities/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-23 06:49:47.000000 quantplay-1.2.92/quantplay/strategies/equities/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.030647 quantplay-1.2.92/quantplay/strategies/futures/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:42.000000 quantplay-1.2.92/quantplay/strategies/futures/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.030752 quantplay-1.2.92/quantplay/strategies/futures/overnight/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-24 08:54:48.000000 quantplay-1.2.92/quantplay/strategies/futures/overnight/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.030850 quantplay-1.2.92/quantplay/strategies/options/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:35:52.000000 quantplay-1.2.92/quantplay/strategies/options/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.031540 quantplay-1.2.92/quantplay/strategies/options/intraday/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-06-22 07:36:03.000000 quantplay-1.2.92/quantplay/strategies/options/intraday/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1958 2022-09-14 18:05:01.000000 quantplay-1.2.92/quantplay/strategies/options/intraday/ladder.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2675 2022-06-25 11:41:44.000000 quantplay-1.2.92/quantplay/strategies/options/intraday/musk.py
+-rw-r--r--   0 ashok      (502) staff       (20)      403 2022-09-17 07:36:48.000000 quantplay-1.2.92/quantplay/strategies/options/intraday/short_straddle.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.031848 quantplay-1.2.92/quantplay/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)    12759 2023-05-17 07:17:28.000000 quantplay-1.2.92/quantplay/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)      214 2022-06-28 09:52:29.000000 quantplay-1.2.92/quantplay/strategy_run.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.033225 quantplay-1.2.92/quantplay/utils/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/utils/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      723 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/utils/config_util.py
+-rw-r--r--   0 ashok      (502) staff       (20)    24181 2023-04-24 06:31:05.000000 quantplay-1.2.92/quantplay/utils/constant.py
+-rw-r--r--   0 ashok      (502) staff       (20)     5433 2023-04-19 06:37:00.000000 quantplay-1.2.92/quantplay/utils/data_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      711 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/utils/exchange.py
+-rw-r--r--   0 ashok      (502) staff       (20)      517 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/utils/number_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)      458 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/utils/pickle_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     1181 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/utils/selenium_utils.py
+-rw-r--r--   0 ashok      (502) staff       (20)     4094 2023-04-19 06:36:45.000000 quantplay-1.2.92/quantplay/utils/transaction_utils.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.021091 quantplay-1.2.92/quantplay.egg-info/
+-rw-r--r--   0 ashok      (502) staff       (20)      663 2023-06-01 01:35:56.000000 quantplay-1.2.92/quantplay.egg-info/PKG-INFO
+-rw-r--r--   0 ashok      (502) staff       (20)     3391 2023-06-01 01:35:57.000000 quantplay-1.2.92/quantplay.egg-info/SOURCES.txt
+-rw-r--r--   0 ashok      (502) staff       (20)        1 2023-06-01 01:35:56.000000 quantplay-1.2.92/quantplay.egg-info/dependency_links.txt
+-rw-r--r--   0 ashok      (502) staff       (20)      221 2023-06-01 01:35:56.000000 quantplay-1.2.92/quantplay.egg-info/requires.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       15 2023-06-01 01:35:56.000000 quantplay-1.2.92/quantplay.egg-info/top_level.txt
+-rw-r--r--   0 ashok      (502) staff       (20)       49 2023-06-01 01:35:57.034743 quantplay-1.2.92/setup.cfg
+-rw-r--r--   0 ashok      (502) staff       (20)      876 2023-06-01 01:35:50.000000 quantplay-1.2.92/setup.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.033476 quantplay-1.2.92/test/
+-rw-------   0 ashok      (502) staff       (20)        0 2022-04-15 16:22:35.000000 quantplay-1.2.92/test/__init__.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.033710 quantplay-1.2.92/test/broker/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/test/broker/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      220 2023-04-19 06:36:45.000000 quantplay-1.2.92/test/broker/finvasia.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.033950 quantplay-1.2.92/test/executor/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/test/executor/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      304 2023-04-19 06:36:45.000000 quantplay-1.2.92/test/executor/strategy_executor.py
+drwxr-xr-x   0 ashok      (502) staff       (20)        0 2023-06-01 01:35:57.034325 quantplay-1.2.92/test/strategy/
+-rw-r--r--   0 ashok      (502) staff       (20)        0 2023-04-19 06:36:45.000000 quantplay-1.2.92/test/strategy/__init__.py
+-rw-r--r--   0 ashok      (502) staff       (20)      292 2023-04-19 06:36:45.000000 quantplay-1.2.92/test/strategy/base.py
+-rw-r--r--   0 ashok      (502) staff       (20)     2194 2023-04-19 06:36:45.000000 quantplay-1.2.92/test/strategy/sample_strategy.py
+-rw-r--r--   0 ashok      (502) staff       (20)     3302 2023-04-19 06:36:45.000000 quantplay-1.2.92/test/test_motilal.py
```

### Comparing `quantplay-1.2.91/PKG-INFO` & `quantplay-1.2.92/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.2.91
+Version: 1.2.92
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.91/quantplay/backtest/backtest_trades.py` & `quantplay-1.2.92/quantplay/backtest/backtest_trades.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/angelone.py` & `quantplay-1.2.92/quantplay/broker/angelone.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/broker_client.py` & `quantplay-1.2.92/quantplay/broker/broker_client.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/finvasia_utils/shoonya.py` & `quantplay-1.2.92/quantplay/broker/finvasia_utils/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/generics/broker.py` & `quantplay-1.2.92/quantplay/broker/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/iifl.py` & `quantplay-1.2.92/quantplay/broker/iifl.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/iifl_xts.py` & `quantplay-1.2.92/quantplay/broker/iifl_xts.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,9 +10,9 @@
     def __init__(self, api_secret=None, api_key=None, wrapper=None, ClientID=None):
         super().__init__(
             api_secret=api_secret,
             api_key=api_key,
             root_interactive=self.xts_interactive,
             root_market=self.xts_market,
             wrapper=wrapper,
-            ClientID=ClientID
+            ClientID=ClientID,
         )
```

### Comparing `quantplay-1.2.91/quantplay/broker/kite_utils.py` & `quantplay-1.2.92/quantplay/broker/kite_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/motilal.py` & `quantplay-1.2.92/quantplay/broker/motilal.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/shoonya.py` & `quantplay-1.2.92/quantplay/broker/shoonya.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/symphony.py` & `quantplay-1.2.92/quantplay/broker/symphony.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/xts.py` & `quantplay-1.2.92/quantplay/broker/xts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import traceback
 import json
 
 import pandas as pd
 import numpy as np
 import pickle
 import codecs
+from datetime import datetime
 
 from quantplay.broker.generics.broker import Broker
 from quantplay.utils.constant import Constants, timeit, OrderType
 from quantplay.broker.xts_utils.Connect import XTSConnect
 from quantplay.utils.pickle_utils import PickleUtils
 from quantplay.exception.exceptions import InvalidArgumentException
 from quantplay.broker.xts_utils.InteractiveSocketClient import OrderSocket_io
@@ -61,29 +62,51 @@
 
     def set_wrapper(self, serialized_wrapper):
         self.wrapper = pickle.loads(
             codecs.decode(serialized_wrapper.encode(), "base64")
         )
 
     def initialize_symbol_data(self):
+        # TODO: Check for Futures
         try:
             self.symbol_data = PickleUtils.load_data("xts_instruments")
             Constants.logger.info("[LOADING_INSTRUMENTS] loading data from cache")
         except Exception as e:
             instruments = pd.read_csv(
                 "https://quantplay-public-data.s3.ap-south-1.amazonaws.com/symbol_data/instruments.csv"
             )
             instruments = instruments.to_dict("records")
             self.symbol_data = {}
 
             for instrument in instruments:
                 exchange = instrument["exchange"]
                 tradingsymbol = instrument["tradingsymbol"]
+                # NIFTY 08JUN2023 PE 17850 <- NIFTY2360817850PE
+                # 2023-06-27 -> 08JUN2023
+                # For FUTURES : EURINR23AUGFUT -> EURINR 23AUG2023 FUT
+                
+                ins_type = instrument["instrument_type"]
+                name = instrument["name"]
+                if ins_type in ["CE","PE"]:
+                    expiry  = datetime.strftime(datetime.strptime(str(instrument["expiry"]), "%Y-%m-%d"), "%d%b%Y").upper()
+                    strike = str(instrument["strike"]).rstrip("0")
+                    if strike[-1] == ".":
+                        strike = strike[:-1]
+                    instrument["broker_symbol"] = f"{name} {expiry} {ins_type} {strike}"
+                elif ins_type == "FUT":
+                    expiry  = datetime.strftime(datetime.strptime(str(instrument["expiry"]), "%Y-%m-%d"), "%d%b%Y").upper()
+                    instrument["broker_symbol"] = f"{name} {expiry} FUT"
+                else:
+                    instrument["broker_symbol"] = tradingsymbol
+                    
+
                 self.symbol_data["{}:{}".format(exchange, tradingsymbol)] = instrument
 
+            self.initialize_broker_symbol_map()
+
             PickleUtils.save_data(self.symbol_data, "xts_instruments")
             Constants.logger.info("[LOADING_INSTRUMENTS] loading data from server")
 
     def login(self):
         response_interact = self.wrapper.interactive_login()
         self.wrapper.marketdata_login()
 
@@ -500,18 +523,18 @@
             new_ord["tradingsymbol"] = order["TradingSymbol"]
 
             if new_ord["exchange"] == "NSEFO":
                 new_ord["exchange"] = "NFO"
             elif new_ord["exchange"] == "NSECM":
                 new_ord["exchange"] = "NSE"
 
-            # if new_ord["exchange"] in ["NFO", "MCX"]:
-            #     new_ord["tradingsymbol"] = self.broker_symbol_map[
-            #         order["tradingsymbol"]
-            #     ]
+            if new_ord["exchange"] in ["NFO", "MCX"]:
+                new_ord["tradingsymbol"] = self.broker_symbol_map[
+                    order["tradingsymbol"]
+                ]
 
             new_ord["order_type"] = order["OrderType"].upper()
             new_ord["product"] = order["ProductType"].upper()
             new_ord["transaction_type"] = order["OrderSide"].upper()
             new_ord["quantity"] = int(order["OrderQuantity"])
 
             if "OrderStopPrice" in order:
```

### Comparing `quantplay-1.2.91/quantplay/broker/xts_utils/Connect.py` & `quantplay-1.2.92/quantplay/broker/xts_utils/Connect.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/xts_utils/Exception.py` & `quantplay-1.2.92/quantplay/broker/xts_utils/Exception.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/xts_utils/InteractiveSocketClient.py` & `quantplay-1.2.92/quantplay/broker/xts_utils/InteractiveSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/xts_utils/MarketDataSocketClient.py` & `quantplay-1.2.92/quantplay/broker/xts_utils/MarketDataSocketClient.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/broker/zerodha.py` & `quantplay-1.2.92/quantplay/broker/zerodha.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/brokerage/angelone/angel_broker.py` & `quantplay-1.2.92/quantplay/brokerage/angelone/angel_broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/brokerage/generics/broker.py` & `quantplay-1.2.92/quantplay/brokerage/generics/broker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/brokerage/zerodha/ZBroker.py` & `quantplay-1.2.92/quantplay/brokerage/zerodha/ZBroker.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/config/qplay_config.py` & `quantplay-1.2.92/quantplay/config/qplay_config.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/create_sample_data.py` & `quantplay-1.2.92/quantplay/create_sample_data.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/data_modify_script.py` & `quantplay-1.2.92/quantplay/data_modify_script.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/date_fix.py` & `quantplay-1.2.92/quantplay/date_fix.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/exception/exceptions.py` & `quantplay-1.2.92/quantplay/exception/exceptions.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/executor/strategy_executor.py` & `quantplay-1.2.92/quantplay/executor/strategy_executor.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/indicators/Indicator.py` & `quantplay-1.2.92/quantplay/indicators/Indicator.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/model/exchange/instrument.py` & `quantplay-1.2.92/quantplay/model/exchange/instrument.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/model/exchange/order.py` & `quantplay-1.2.92/quantplay/model/exchange/order.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/model/exchange/tick.py` & `quantplay-1.2.92/quantplay/model/exchange/tick.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/order_execution/execution_algorithm.py` & `quantplay-1.2.92/quantplay/order_execution/execution_algorithm.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/order_execution/mean_price.py` & `quantplay-1.2.92/quantplay/order_execution/mean_price.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/reporting/strategy_report.py` & `quantplay-1.2.92/quantplay/reporting/strategy_report.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/reporting/visuals.py` & `quantplay-1.2.92/quantplay/reporting/visuals.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/services/market.py` & `quantplay-1.2.92/quantplay/services/market.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/services/tradelens.py` & `quantplay-1.2.92/quantplay/services/tradelens.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/strategies/options/intraday/ladder.py` & `quantplay-1.2.92/quantplay/strategies/options/intraday/ladder.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/strategies/options/intraday/musk.py` & `quantplay-1.2.92/quantplay/strategies/options/intraday/musk.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/strategy/base.py` & `quantplay-1.2.92/quantplay/strategy/base.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/utils/config_util.py` & `quantplay-1.2.92/quantplay/utils/config_util.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/utils/constant.py` & `quantplay-1.2.92/quantplay/utils/constant.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/utils/data_utils.py` & `quantplay-1.2.92/quantplay/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/utils/exchange.py` & `quantplay-1.2.92/quantplay/utils/exchange.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/utils/number_utils.py` & `quantplay-1.2.92/quantplay/utils/number_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/utils/selenium_utils.py` & `quantplay-1.2.92/quantplay/utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay/utils/transaction_utils.py` & `quantplay-1.2.92/quantplay/utils/transaction_utils.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/quantplay.egg-info/PKG-INFO` & `quantplay-1.2.92/quantplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quantplay
-Version: 1.2.91
+Version: 1.2.92
 Summary: This python package will be stored in AWS CodeArtifact
 Home-page: 
 Author: 
 Author-email: 
 License: MIT
 
 # Quantplay Alpha playground
```

### Comparing `quantplay-1.2.91/quantplay.egg-info/SOURCES.txt` & `quantplay-1.2.92/quantplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/setup.py` & `quantplay-1.2.92/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     for line in Path("requirements.txt").read_text().splitlines()
     if is_requirement(line)
 ]
 
 setup(
     name="quantplay",
     long_description=Path("README.md").read_text(),
-    version="1.2.91",
+    version="1.2.92",
     setup_requires=["pytest-runner"],
     install_requires=requirements,
     tests_require=[],
     packages=find_packages(),
     url="",
     license="MIT",
     author="",
```

### Comparing `quantplay-1.2.91/test/strategy/sample_strategy.py` & `quantplay-1.2.92/test/strategy/sample_strategy.py`

 * *Files identical despite different names*

### Comparing `quantplay-1.2.91/test/test_motilal.py` & `quantplay-1.2.92/test/test_motilal.py`

 * *Files identical despite different names*

