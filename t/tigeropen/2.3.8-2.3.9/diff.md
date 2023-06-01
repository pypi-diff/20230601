# Comparing `tmp/tigeropen-2.3.8.tar.gz` & `tmp/tigeropen-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-2.3.8.tar", last modified: Tue May  9 12:42:33 2023, max compression
+gzip compressed data, was "tigeropen-2.3.9.tar", last modified: Thu Jun  1 07:01:44 2023, max compression
```

## Comparing `tigeropen-2.3.8.tar` & `tigeropen-2.3.9.tar`

### file list

```diff
@@ -1,207 +1,208 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.050021 tigeropen-2.3.8/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.3.8/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-05-09 12:42:33.049900 tigeropen-2.3.8/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.3.8/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.3.8/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2023-05-09 12:42:33.050056 tigeropen-2.3.8/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-2.3.8/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.021745 tigeropen-2.3.8/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.023597 tigeropen-2.3.8/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.025205 tigeropen-2.3.8/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     4255 2023-03-31 07:32:01.000000 tigeropen-2.3.8/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.3.8/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.3.8/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     2989 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      549 2021-11-16 06:27:09.000000 tigeropen-2.3.8/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.027026 tigeropen-2.3.8/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-2.3.8/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     6676 2023-03-29 02:32:08.000000 tigeropen-2.3.8/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.3.8/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.3.8/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.028027 tigeropen-2.3.8/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.028300 tigeropen-2.3.8/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)     9532 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8402 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.028435 tigeropen-2.3.8/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.028558 tigeropen-2.3.8/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.028794 tigeropen-2.3.8/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.029713 tigeropen-2.3.8/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.3.8/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.3.8/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.030432 tigeropen-2.3.8/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.031873 tigeropen-2.3.8/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7693 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.038467 tigeropen-2.3.8/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1567 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2199 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3433 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2372 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-04-18 06:52:53.000000 tigeropen-2.3.8/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.3.8/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)     8948 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    11569 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.3.8/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.038728 tigeropen-2.3.8/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.040394 tigeropen-2.3.8/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    76884 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.040626 tigeropen-2.3.8/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    33696 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.045946 tigeropen-2.3.8/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.3.8/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.3.8/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1719 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.3.8/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.3.8/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1574 2023-03-02 08:06:25.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2528 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2742 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2463 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_timeline_history_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.3.8/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.3.8/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.3.8/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4953 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.3.8/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-2.3.8/tigeropen/quote/response/warrant_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-2.3.8/tigeropen/quote/response/warrant_filter_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11305 2023-03-10 10:02:27.000000 tigeropen-2.3.8/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-03-23 03:30:06.000000 tigeropen-2.3.8/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.046194 tigeropen-2.3.8/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.047640 tigeropen-2.3.8/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     4529 2023-05-09 12:41:30.000000 tigeropen-2.3.8/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)     9811 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     2257 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.3.8/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.047887 tigeropen-2.3.8/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.8/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    32706 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.049697 tigeropen-2.3.8/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1179 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      961 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4484 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1633 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1163 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1336 2020-06-01 05:09:25.000000 tigeropen-2.3.8/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     6736 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4864 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.3.8/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-2.3.8/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1472 2022-11-30 08:21:30.000000 tigeropen-2.3.8/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    40415 2023-04-18 08:29:36.000000 tigeropen-2.3.8/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-05-09 12:42:33.022603 tigeropen-2.3.8/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-05-09 12:42:33.000000 tigeropen-2.3.8/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     7360 2023-05-09 12:42:33.000000 tigeropen-2.3.8/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2023-05-09 12:42:33.000000 tigeropen-2.3.8/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      130 2023-05-09 12:42:33.000000 tigeropen-2.3.8/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2023-05-09 12:42:33.000000 tigeropen-2.3.8/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.388480 tigeropen-2.3.9/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.3.9/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-01 07:01:44.388336 tigeropen-2.3.9/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.3.9/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.3.9/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2023-06-01 07:01:44.388530 tigeropen-2.3.9/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-2.3.9/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.339447 tigeropen-2.3.9/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.341277 tigeropen-2.3.9/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.343178 tigeropen-2.3.9/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     4255 2023-03-31 07:32:01.000000 tigeropen-2.3.9/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    19190 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.3.9/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.3.9/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2989 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      549 2021-11-16 06:27:09.000000 tigeropen-2.3.9/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.345017 tigeropen-2.3.9/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-05-08 03:14:32.000000 tigeropen-2.3.9/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6676 2023-03-29 02:32:08.000000 tigeropen-2.3.9/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.3.9/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.3.9/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.346112 tigeropen-2.3.9/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.346444 tigeropen-2.3.9/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)    10346 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8402 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.346608 tigeropen-2.3.9/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.346765 tigeropen-2.3.9/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.347072 tigeropen-2.3.9/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.348243 tigeropen-2.3.9/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.3.9/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.3.9/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.348906 tigeropen-2.3.9/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.350367 tigeropen-2.3.9/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7566 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-06-01 06:23:56.000000 tigeropen-2.3.9/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.357590 tigeropen-2.3.9/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1969 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2534 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4388 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2372 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-06-01 02:58:45.000000 tigeropen-2.3.9/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.3.9/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)      661 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/pb/trade_tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8948 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15009 2023-06-01 07:01:36.000000 tigeropen-2.3.9/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.3.9/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.358068 tigeropen-2.3.9/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.360364 tigeropen-2.3.9/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9623 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    76884 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.360653 tigeropen-2.3.9/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    33696 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.370380 tigeropen-2.3.9/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.3.9/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.3.9/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1719 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.3.9/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1805 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.3.9/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1574 2023-03-02 08:06:25.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2528 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2742 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2463 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_timeline_history_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.3.9/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.3.9/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.3.9/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4953 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.3.9/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-2.3.9/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-2.3.9/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11305 2023-06-01 02:40:59.000000 tigeropen-2.3.9/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-06-01 02:40:59.000000 tigeropen-2.3.9/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.370871 tigeropen-2.3.9/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.380371 tigeropen-2.3.9/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4529 2023-05-09 12:41:30.000000 tigeropen-2.3.9/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9811 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2257 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.3.9/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.380855 tigeropen-2.3.9/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.9/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    32706 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.387954 tigeropen-2.3.9/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1179 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      961 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4484 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1633 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1163 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1336 2020-06-01 05:09:25.000000 tigeropen-2.3.9/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6736 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4864 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.3.9/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-2.3.9/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1472 2022-11-30 08:21:30.000000 tigeropen-2.3.9/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    40415 2023-04-18 08:29:36.000000 tigeropen-2.3.9/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-06-01 07:01:44.340288 tigeropen-2.3.9/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-06-01 07:01:44.000000 tigeropen-2.3.9/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     7392 2023-06-01 07:01:44.000000 tigeropen-2.3.9/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2023-06-01 07:01:44.000000 tigeropen-2.3.9/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      130 2023-06-01 07:01:44.000000 tigeropen-2.3.9/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2023-06-01 07:01:44.000000 tigeropen-2.3.9/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-2.3.8/PKG-INFO` & `tigeropen-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.3.8
+Version: 2.3.9
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-2.3.8/README.md` & `tigeropen-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/setup.py` & `tigeropen-2.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/consts/__init__.py` & `tigeropen-2.3.9/tigeropen/common/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/consts/filter_fields.py` & `tigeropen-2.3.9/tigeropen/common/consts/filter_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-2.3.9/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/consts/params.py` & `tigeropen-2.3.9/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/consts/push_types.py` & `tigeropen-2.3.9/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/consts/quote_keys.py` & `tigeropen-2.3.9/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/consts/service_types.py` & `tigeropen-2.3.9/tigeropen/common/consts/service_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/consts/tick_constants.py` & `tigeropen-2.3.9/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/model.py` & `tigeropen-2.3.9/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/request.py` & `tigeropen-2.3.9/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/response.py` & `tigeropen-2.3.9/tigeropen/common/response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/util/common_utils.py` & `tigeropen-2.3.9/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/util/contract_utils.py` & `tigeropen-2.3.9/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/util/order_utils.py` & `tigeropen-2.3.9/tigeropen/common/util/order_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/util/price_util.py` & `tigeropen-2.3.9/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/util/signature_utils.py` & `tigeropen-2.3.9/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/util/string_utils.py` & `tigeropen-2.3.9/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/util/tick_util.py` & `tigeropen-2.3.9/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/common/util/web_utils.py` & `tigeropen-2.3.9/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/examples/client_config.py` & `tigeropen-2.3.9/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/examples/nasdaq100.py` & `tigeropen-2.3.9/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-2.3.9/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/examples/push_client_demo.py` & `tigeropen-2.3.9/tigeropen/examples/push_client_demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from tigeropen.push.pb.OrderStatusData_pb2 import OrderStatusData
 from tigeropen.push.pb.OrderTransactionData_pb2 import OrderTransactionData
 from tigeropen.push.pb.PositionData_pb2 import PositionData
 from tigeropen.push.pb.QuoteBBOData_pb2 import QuoteBBOData
 from tigeropen.push.pb.QuoteBasicData_pb2 import QuoteBasicData
 from tigeropen.push.pb.QuoteDepthData_pb2 import QuoteDepthData
 from tigeropen.push.pb.TradeTickData_pb2 import TradeTickData
+from tigeropen.push.pb.trade_tick import TradeTick
 from tigeropen.push.push_client import PushClient
 from tigeropen.examples.client_config import get_client_config
 
 
 def query_subscribed_callback(data):
     """
     data example:
@@ -148,32 +149,19 @@
       orderCount: 143
       orderCount: 26
     }
     """
     print(f'quote depth changed: {frame}')
 
 
-def on_tick_changed(frame: TradeTickData):
+def on_tick_changed(frame: TradeTick):
     """逐笔成交回调
     example:
-    symbol: "00700"
-    type: "-+"
-    sn: 37998
-    priceBase: 3636
-    priceOffset: 1
-    time: 1677742815311
-    time: 69
-    price: 0
-    price: 2
-    volume: 500
-    volume: 100
-    quoteLevel: "hkStockQuoteLv2"
-    timestamp: 1677742815776
-    secType: "STK"
-
+    TradeTick<{'symbol': '00700', 'sec_type': 'STK', 'quote_level': 'hkStockQuoteLv2', 'timestamp': 1685602618145, 'ticks': [TradeTickItem<{'tick_type': '+', 'price': 316.6, 'volume': 100, 'part_code': None, 'part_code_name': None, 'cond': None, 'time': 1685602617046, 'sn': 42055}>, TradeTickItem<{'tick_type': '-', 'price': 316.4, 'volume': 600, 'part_code': None, 'part_code_name': None, 'cond': None, 'time': 1685602617639, 'sn': 42056}>, TradeTickItem<{'tick_type': '-', 'price': 316.4, 'volume': 200, 'part_code': None, 'part_code_name': None, 'cond': None, 'time': 1685602617639, 'sn': 42057}>]}>
+    TradeTick<{'symbol': 'CLmain', 'sec_type': 'FUT', 'quote_level': '', 'timestamp': 1685602618153, 'ticks': [TradeTickItem<{'tick_type': None, 'price': 68.7, 'volume': 1, 'part_code': None, 'part_code_name': None, 'cond': None, 'time': 1685602616000, 'sn': 109150}>, TradeTickItem<{'tick_type': None, 'price': 68.7, 'volume': 1, 'part_code': None, 'part_code_name': None, 'cond': None, 'time': 1685602616000, 'sn': 109151}>]}>
     """
     print(frame)
 
 
 def on_order_changed(frame: OrderStatusData):
     """订单回调
     {"id":"28875370355884032","account":"736845","symbol":"CL","identifier":"CL2312","multiplier":1000,
```

### Comparing `tigeropen-2.3.8/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-2.3.9/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/examples/quote_client_demo.py` & `tigeropen-2.3.9/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/examples/trade_client_demo.py` & `tigeropen-2.3.9/tigeropen/examples/trade_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/fundamental/request/model.py` & `tigeropen-2.3.9/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-2.3.9/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-2.3.9/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-2.3.9/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-2.3.9/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-2.3.9/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/fundamental/response/industry_response.py` & `tigeropen-2.3.9/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/__init__.py` & `tigeropen-2.3.9/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/network/connect.py` & `tigeropen-2.3.9/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/network/exception.py` & `tigeropen-2.3.9/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/network/listener.py` & `tigeropen-2.3.9/tigeropen/push/network/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,12 @@
                 if diff_receive > self.receive_sleep:
                     # heartbeat timeout
                     logging.warning("heartbeat timeout: diff_receive=%s, time=%s, lastrec=%s",
                                     diff_receive, now, self.received_heartbeat)
                     self.transport.set_connected(False)
                     self.transport.disconnect_socket()
                     self.transport.stop()
-                    for listener in self.transport.listeners.values():
-                        listener.on_heartbeat_timeout()
         self.heartbeat_thread = None
         self.heartbeat_terminate_event.clear()
         if self.heartbeats != (0, 0):
             # don't bother logging this if heartbeats weren't setup to start with
             logging.debug("heartbeat loop ended")
```

### Comparing `tigeropen-2.3.8/tigeropen/push/network/protocal.py` & `tigeropen-2.3.9/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/network/transport.py` & `tigeropen-2.3.9/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/network/utils.py` & `tigeropen-2.3.9/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/AssetData.proto` & `tigeropen-2.3.9/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-2.3.9/tigeropen/push/pb/OrderStatusData.proto`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 syntax = "proto3";
 
 package tigeropen.push.pb;
 
-
 message OrderStatusData {
   sint64 id = 1; // unique order id
   string account = 2; // user account
   string symbol = 3;
-  string identifier = 4;
-  uint32 multiplier = 5; // multiplier for futures, options, warrants and CBBC
-  string action = 6; // BUY or SELL
-  string market = 7; // market. US, HK, etc.
-  string currency = 8; // currency. USD, HKD, etc.
-  string segType = 9; // Securities Category C: (Commodities Futures), S: (Securities Stocks)
-  string secType = 10; // STK Stocks, OPT Options, WAR Warrants, IOPT CBBC, CASH FOREX, FUT Futures, FOP Future Options
+  string expiry = 4; // for options, formate:yyyyMMdd
+  string strike = 5; // for options
+  string right = 6; // for options
+  string identifier = 7;
+  uint32 multiplier = 8; // multiplier for futures, options, warrants and CBBC
+  string action = 9; // BUY or SELL
+  string market = 10; // market. US, HK, etc.
+  string currency = 11; // currency. USD, HKD, etc.
+  string segType = 12; // Securities Category C: (Commodities Futures), S: (Securities Stocks)
+  string secType = 13; // STK Stocks, OPT Options, WAR Warrants, IOPT CBBC, CASH FOREX, FUT Futures, FOP Future Options
 
-  string orderType = 11; // order type
-  bool isLong = 12;
-  sint64 totalQuantity = 13; // total quantity
-  sint32 totalQuantityScale = 14; // total quantity scale
-  sint64 filledQuantity = 15; // filled quantity
-  sint32 filledQuantityScale = 16; // filled quantity scale
-  double avgFillPrice = 17; // average price at which the orders got filled
-  double limitPrice = 18; // limit price（required when orderType is 'LMT'）
-  double realizedPnl = 19; // realized profit and loss
-  string status = 20; // order status
+  string orderType = 14; // order type
+  bool isLong = 15;
+  sint64 totalQuantity = 16; // total quantity
+  sint32 totalQuantityScale = 17; // total quantity scale
+  sint64 filledQuantity = 18; // filled quantity
+  sint32 filledQuantityScale = 19; // filled quantity scale
+  double avgFillPrice = 20; // average price at which the orders got filled
+  double limitPrice = 21; // limit price（required when orderType is 'LMT'）
+  double stopPrice = 22; // stop price（required when orderType is 'STP'）
+  double realizedPnl = 23; // realized profit and loss
+  string status = 24; // order status
+  string replaceStatus = 25; // order replace status
+  string cancelStatus = 26; // order cancel status
 
-  bool outsideRth = 21; // if trade outside regular trading hours (only applicable to U.S. market)
-  bool canModify = 22;
-  bool canCancel = 23;
-  string name = 24; // symbol name
-  string source = 25; // order source(from 'OpenApi', or not)
-  string errorMsg = 26; // error message
-  float commissionAndFee = 27; // commission and fee
-  uint64 openTime = 28; // timestamp when the order is placed
-  uint64 timestamp = 29;
+  bool outsideRth = 27; // if trade outside regular trading hours (only applicable to U.S. market)
+  bool canModify = 28;
+  bool canCancel = 29;
+  bool liquidation = 30;
+  string name = 31; // symbol name
+  string source = 32; // order source(from 'OpenApi', or not)
+  string errorMsg = 33; // error message
+  string attrDesc = 34; // order description
+  float commissionAndFee = 35; // commission and fee
+  uint64 openTime = 36; // timestamp when the order is placed
+  uint64 timestamp = 37;
+  string userMark = 38;
 }
```

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tigeropen/push/pb/OrderStatusData.proto
+# source: tigeropen/push/pb/OrderTransactionData.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\'tigeropen/push/pb/OrderStatusData.proto\x12\x11tigeropen.push.pb\"\xbd\x04\n\x0fOrderStatusData\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0f\n\x07\x61\x63\x63ount\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x12\n\nidentifier\x18\x04 \x01(\t\x12\x12\n\nmultiplier\x18\x05 \x01(\r\x12\x0e\n\x06\x61\x63tion\x18\x06 \x01(\t\x12\x0e\n\x06market\x18\x07 \x01(\t\x12\x10\n\x08\x63urrency\x18\x08 \x01(\t\x12\x0f\n\x07segType\x18\t \x01(\t\x12\x0f\n\x07secType\x18\n \x01(\t\x12\x11\n\torderType\x18\x0b \x01(\t\x12\x0e\n\x06isLong\x18\x0c \x01(\x08\x12\x15\n\rtotalQuantity\x18\r \x01(\x12\x12\x1a\n\x12totalQuantityScale\x18\x0e \x01(\x11\x12\x16\n\x0e\x66illedQuantity\x18\x0f \x01(\x12\x12\x1b\n\x13\x66illedQuantityScale\x18\x10 \x01(\x11\x12\x14\n\x0c\x61vgFillPrice\x18\x11 \x01(\x01\x12\x12\n\nlimitPrice\x18\x12 \x01(\x01\x12\x13\n\x0brealizedPnl\x18\x13 \x01(\x01\x12\x0e\n\x06status\x18\x14 \x01(\t\x12\x12\n\noutsideRth\x18\x15 \x01(\x08\x12\x11\n\tcanModify\x18\x16 \x01(\x08\x12\x11\n\tcanCancel\x18\x17 \x01(\x08\x12\x0c\n\x04name\x18\x18 \x01(\t\x12\x0e\n\x06source\x18\x19 \x01(\t\x12\x10\n\x08\x65rrorMsg\x18\x1a \x01(\t\x12\x18\n\x10\x63ommissionAndFee\x18\x1b \x01(\x02\x12\x10\n\x08openTime\x18\x1c \x01(\x04\x12\x11\n\ttimestamp\x18\x1d \x01(\x04\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,tigeropen/push/pb/OrderTransactionData.proto\x12\x11tigeropen.push.pb\"\xce\x02\n\x14OrderTransactionData\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0f\n\x07orderId\x18\x02 \x01(\x12\x12\x0f\n\x07\x61\x63\x63ount\x18\x03 \x01(\t\x12\x0e\n\x06symbol\x18\x04 \x01(\t\x12\x12\n\nidentifier\x18\x05 \x01(\t\x12\x12\n\nmultiplier\x18\x06 \x01(\r\x12\x0e\n\x06\x61\x63tion\x18\x07 \x01(\t\x12\x0e\n\x06market\x18\x08 \x01(\t\x12\x10\n\x08\x63urrency\x18\t \x01(\t\x12\x0f\n\x07segType\x18\n \x01(\t\x12\x0f\n\x07secType\x18\x0b \x01(\t\x12\x13\n\x0b\x66illedPrice\x18\x0c \x01(\x01\x12\x16\n\x0e\x66illedQuantity\x18\r \x01(\x12\x12\x12\n\ncreateTime\x18\x0e \x01(\x04\x12\x12\n\nupdateTime\x18\x0f \x01(\x04\x12\x14\n\x0ctransactTime\x18\x10 \x01(\x04\x12\x11\n\ttimestamp\x18\x11 \x01(\x04\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.OrderStatusData_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.OrderTransactionData_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _ORDERSTATUSDATA._serialized_start=63
-  _ORDERSTATUSDATA._serialized_end=636
+  _ORDERTRANSACTIONDATA._serialized_start=68
+  _ORDERTRANSACTIONDATA._serialized_end=402
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,57 @@
+from tigeropen.push.pb import SocketCommon_pb2 as _SocketCommon_pb2
+from tigeropen.push.pb import QuoteData_pb2 as _QuoteData_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Optional as _Optional
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
+from tigeropen.push.pb.SocketCommon_pb2 import SocketCommon
+from tigeropen.push.pb.QuoteData_pb2 import QuoteData
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class OrderStatusData(_message.Message):
-    __slots__ = ["account", "action", "avgFillPrice", "canCancel", "canModify", "commissionAndFee", "currency", "errorMsg", "filledQuantity", "filledQuantityScale", "id", "identifier", "isLong", "limitPrice", "market", "multiplier", "name", "openTime", "orderType", "outsideRth", "realizedPnl", "secType", "segType", "source", "status", "symbol", "timestamp", "totalQuantity", "totalQuantityScale"]
-    ACCOUNT_FIELD_NUMBER: _ClassVar[int]
-    ACTION_FIELD_NUMBER: _ClassVar[int]
-    AVGFILLPRICE_FIELD_NUMBER: _ClassVar[int]
-    CANCANCEL_FIELD_NUMBER: _ClassVar[int]
-    CANMODIFY_FIELD_NUMBER: _ClassVar[int]
-    COMMISSIONANDFEE_FIELD_NUMBER: _ClassVar[int]
-    CURRENCY_FIELD_NUMBER: _ClassVar[int]
-    ERRORMSG_FIELD_NUMBER: _ClassVar[int]
-    FILLEDQUANTITYSCALE_FIELD_NUMBER: _ClassVar[int]
-    FILLEDQUANTITY_FIELD_NUMBER: _ClassVar[int]
+class QuoteBasicData(_message.Message):
+    __slots__ = ["amount", "avgPrice", "high", "hourTradingTag", "identifier", "latestPrice", "latestPriceTimestamp", "latestTime", "low", "marketStatus", "mi", "minTick", "open", "openInt", "preClose", "preSettlement", "serverTimestamp", "symbol", "timestamp", "tradeTime", "type", "volume"]
+    AMOUNT_FIELD_NUMBER: _ClassVar[int]
+    AVGPRICE_FIELD_NUMBER: _ClassVar[int]
+    HIGH_FIELD_NUMBER: _ClassVar[int]
+    HOURTRADINGTAG_FIELD_NUMBER: _ClassVar[int]
     IDENTIFIER_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    ISLONG_FIELD_NUMBER: _ClassVar[int]
-    LIMITPRICE_FIELD_NUMBER: _ClassVar[int]
-    MARKET_FIELD_NUMBER: _ClassVar[int]
-    MULTIPLIER_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    OPENTIME_FIELD_NUMBER: _ClassVar[int]
-    ORDERTYPE_FIELD_NUMBER: _ClassVar[int]
-    OUTSIDERTH_FIELD_NUMBER: _ClassVar[int]
-    REALIZEDPNL_FIELD_NUMBER: _ClassVar[int]
-    SECTYPE_FIELD_NUMBER: _ClassVar[int]
-    SEGTYPE_FIELD_NUMBER: _ClassVar[int]
-    SOURCE_FIELD_NUMBER: _ClassVar[int]
-    STATUS_FIELD_NUMBER: _ClassVar[int]
+    LATESTPRICETIMESTAMP_FIELD_NUMBER: _ClassVar[int]
+    LATESTPRICE_FIELD_NUMBER: _ClassVar[int]
+    LATESTTIME_FIELD_NUMBER: _ClassVar[int]
+    LOW_FIELD_NUMBER: _ClassVar[int]
+    MARKETSTATUS_FIELD_NUMBER: _ClassVar[int]
+    MINTICK_FIELD_NUMBER: _ClassVar[int]
+    MI_FIELD_NUMBER: _ClassVar[int]
+    OPENINT_FIELD_NUMBER: _ClassVar[int]
+    OPEN_FIELD_NUMBER: _ClassVar[int]
+    PRECLOSE_FIELD_NUMBER: _ClassVar[int]
+    PRESETTLEMENT_FIELD_NUMBER: _ClassVar[int]
+    SERVERTIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     SYMBOL_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
-    TOTALQUANTITYSCALE_FIELD_NUMBER: _ClassVar[int]
-    TOTALQUANTITY_FIELD_NUMBER: _ClassVar[int]
-    account: str
-    action: str
-    avgFillPrice: float
-    canCancel: bool
-    canModify: bool
-    commissionAndFee: float
-    currency: str
-    errorMsg: str
-    filledQuantity: int
-    filledQuantityScale: int
-    id: int
+    TRADETIME_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    VOLUME_FIELD_NUMBER: _ClassVar[int]
+    amount: float
+    avgPrice: float
+    high: float
+    hourTradingTag: str
     identifier: str
-    isLong: bool
-    limitPrice: float
-    market: str
-    multiplier: int
-    name: str
-    openTime: int
-    orderType: str
-    outsideRth: bool
-    realizedPnl: float
-    secType: str
-    segType: str
-    source: str
-    status: str
+    latestPrice: float
+    latestPriceTimestamp: int
+    latestTime: str
+    low: float
+    marketStatus: str
+    mi: _QuoteData_pb2.QuoteData.Minute
+    minTick: float
+    open: float
+    openInt: int
+    preClose: float
+    preSettlement: float
+    serverTimestamp: int
     symbol: str
     timestamp: int
-    totalQuantity: int
-    totalQuantityScale: int
-    def __init__(self, id: _Optional[int] = ..., account: _Optional[str] = ..., symbol: _Optional[str] = ..., identifier: _Optional[str] = ..., multiplier: _Optional[int] = ..., action: _Optional[str] = ..., market: _Optional[str] = ..., currency: _Optional[str] = ..., segType: _Optional[str] = ..., secType: _Optional[str] = ..., orderType: _Optional[str] = ..., isLong: bool = ..., totalQuantity: _Optional[int] = ..., totalQuantityScale: _Optional[int] = ..., filledQuantity: _Optional[int] = ..., filledQuantityScale: _Optional[int] = ..., avgFillPrice: _Optional[float] = ..., limitPrice: _Optional[float] = ..., realizedPnl: _Optional[float] = ..., status: _Optional[str] = ..., outsideRth: bool = ..., canModify: bool = ..., canCancel: bool = ..., name: _Optional[str] = ..., source: _Optional[str] = ..., errorMsg: _Optional[str] = ..., commissionAndFee: _Optional[float] = ..., openTime: _Optional[int] = ..., timestamp: _Optional[int] = ...) -> None: ...
+    tradeTime: int
+    type: _SocketCommon_pb2.SocketCommon.QuoteType
+    volume: int
+    def __init__(self, symbol: _Optional[str] = ..., type: _Optional[_Union[_SocketCommon_pb2.SocketCommon.QuoteType, str]] = ..., timestamp: _Optional[int] = ..., serverTimestamp: _Optional[int] = ..., avgPrice: _Optional[float] = ..., latestPrice: _Optional[float] = ..., latestPriceTimestamp: _Optional[int] = ..., latestTime: _Optional[str] = ..., preClose: _Optional[float] = ..., volume: _Optional[int] = ..., amount: _Optional[float] = ..., open: _Optional[float] = ..., high: _Optional[float] = ..., low: _Optional[float] = ..., hourTradingTag: _Optional[str] = ..., marketStatus: _Optional[str] = ..., identifier: _Optional[str] = ..., openInt: _Optional[int] = ..., tradeTime: _Optional[int] = ..., preSettlement: _Optional[float] = ..., minTick: _Optional[float] = ..., mi: _Optional[_Union[_QuoteData_pb2.QuoteData.Minute, _Mapping]] = ...) -> None: ...
```

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/PositionData_pb2.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tigeropen/push/pb/OrderTransactionData.proto
+# source: tigeropen/push/pb/PositionData.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,tigeropen/push/pb/OrderTransactionData.proto\x12\x11tigeropen.push.pb\"\xce\x02\n\x14OrderTransactionData\x12\n\n\x02id\x18\x01 \x01(\x12\x12\x0f\n\x07orderId\x18\x02 \x01(\x12\x12\x0f\n\x07\x61\x63\x63ount\x18\x03 \x01(\t\x12\x0e\n\x06symbol\x18\x04 \x01(\t\x12\x12\n\nidentifier\x18\x05 \x01(\t\x12\x12\n\nmultiplier\x18\x06 \x01(\r\x12\x0e\n\x06\x61\x63tion\x18\x07 \x01(\t\x12\x0e\n\x06market\x18\x08 \x01(\t\x12\x10\n\x08\x63urrency\x18\t \x01(\t\x12\x0f\n\x07segType\x18\n \x01(\t\x12\x0f\n\x07secType\x18\x0b \x01(\t\x12\x13\n\x0b\x66illedPrice\x18\x0c \x01(\x01\x12\x16\n\x0e\x66illedQuantity\x18\r \x01(\x12\x12\x12\n\ncreateTime\x18\x0e \x01(\x04\x12\x12\n\nupdateTime\x18\x0f \x01(\x04\x12\x14\n\x0ctransactTime\x18\x10 \x01(\x04\x12\x11\n\ttimestamp\x18\x11 \x01(\x04\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tigeropen/push/pb/PositionData.proto\x12\x11tigeropen.push.pb\"\x8e\x03\n\x0cPositionData\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x0e\n\x06\x65xpiry\x18\x03 \x01(\t\x12\x0e\n\x06strike\x18\x04 \x01(\t\x12\r\n\x05right\x18\x05 \x01(\t\x12\x12\n\nidentifier\x18\x06 \x01(\t\x12\x12\n\nmultiplier\x18\x07 \x01(\r\x12\x0e\n\x06market\x18\x08 \x01(\t\x12\x10\n\x08\x63urrency\x18\t \x01(\t\x12\x0f\n\x07segType\x18\n \x01(\t\x12\x0f\n\x07secType\x18\x0b \x01(\t\x12\x10\n\x08position\x18\x0c \x01(\x12\x12\x15\n\rpositionScale\x18\r \x01(\x11\x12\x13\n\x0b\x61verageCost\x18\x0e \x01(\x01\x12\x13\n\x0blatestPrice\x18\x0f \x01(\x01\x12\x13\n\x0bmarketValue\x18\x10 \x01(\x01\x12\x15\n\runrealizedPnl\x18\x11 \x01(\x01\x12\x0c\n\x04name\x18\x12 \x01(\t\x12\x11\n\ttimestamp\x18\x13 \x01(\x04\x12\x15\n\x08saleable\x18\x14 \x01(\x12H\x00\x88\x01\x01\x42\x0b\n\t_saleableb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.OrderTransactionData_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.PositionData_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _ORDERTRANSACTIONDATA._serialized_start=68
-  _ORDERTRANSACTIONDATA._serialized_end=402
+  _POSITIONDATA._serialized_start=60
+  _POSITIONDATA._serialized_end=458
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/PositionData.proto` & `tigeropen-2.3.9/tigeropen/push/pb/PositionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: tigeropen/push/pb/PositionData.proto
+# source: tigeropen/push/pb/TradeTickData.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tigeropen/push/pb/PositionData.proto\x12\x11tigeropen.push.pb\"\x8e\x03\n\x0cPositionData\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x0e\n\x06\x65xpiry\x18\x03 \x01(\t\x12\x0e\n\x06strike\x18\x04 \x01(\t\x12\r\n\x05right\x18\x05 \x01(\t\x12\x12\n\nidentifier\x18\x06 \x01(\t\x12\x12\n\nmultiplier\x18\x07 \x01(\r\x12\x0e\n\x06market\x18\x08 \x01(\t\x12\x10\n\x08\x63urrency\x18\t \x01(\t\x12\x0f\n\x07segType\x18\n \x01(\t\x12\x0f\n\x07secType\x18\x0b \x01(\t\x12\x10\n\x08position\x18\x0c \x01(\x12\x12\x15\n\rpositionScale\x18\r \x01(\x11\x12\x13\n\x0b\x61verageCost\x18\x0e \x01(\x01\x12\x13\n\x0blatestPrice\x18\x0f \x01(\x01\x12\x13\n\x0bmarketValue\x18\x10 \x01(\x01\x12\x15\n\runrealizedPnl\x18\x11 \x01(\x01\x12\x0c\n\x04name\x18\x12 \x01(\t\x12\x11\n\ttimestamp\x18\x13 \x01(\x04\x12\x15\n\x08saleable\x18\x14 \x01(\x12H\x00\x88\x01\x01\x42\x0b\n\t_saleableb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%tigeropen/push/pb/TradeTickData.proto\x12\x11tigeropen.push.pb\"\xd4\x02\n\rTradeTickData\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0c\n\x04\x63ond\x18\x03 \x01(\t\x12\n\n\x02sn\x18\x04 \x01(\x03\x12\x11\n\tpriceBase\x18\x05 \x01(\x03\x12\x13\n\x0bpriceOffset\x18\x06 \x01(\x05\x12\x0c\n\x04time\x18\x07 \x03(\x03\x12\r\n\x05price\x18\x08 \x03(\x03\x12\x0e\n\x06volume\x18\t \x03(\x03\x12\x10\n\x08partCode\x18\n \x03(\t\x12\x12\n\nquoteLevel\x18\x0b \x01(\t\x12\x11\n\ttimestamp\x18\x0c \x01(\x04\x12\x0f\n\x07secType\x18\r \x01(\t\x12>\n\nmergedVols\x18\x0e \x03(\x0b\x32*.tigeropen.push.pb.TradeTickData.MergedVol\x1a,\n\tMergedVol\x12\x12\n\nmergeTimes\x18\x01 \x01(\x05\x12\x0b\n\x03vol\x18\x02 \x03(\x03\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.PositionData_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.TradeTickData_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  _POSITIONDATA._serialized_start=60
-  _POSITIONDATA._serialized_end=458
+  _TRADETICKDATA._serialized_start=61
+  _TRADETICKDATA._serialized_end=401
+  _TRADETICKDATA_MERGEDVOL._serialized_start=357
+  _TRADETICKDATA_MERGEDVOL._serialized_end=401
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/PushData.proto` & `tigeropen-2.3.9/tigeropen/push/pb/PushData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/PushData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/QuoteData.proto` & `tigeropen-2.3.9/tigeropen/push/pb/QuoteData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/Request.proto` & `tigeropen-2.3.9/tigeropen/push/pb/Request.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/Request_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/Request_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/Request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/Response_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/Response_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/Response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-2.3.9/tigeropen/push/pb/SocketCommon.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-2.3.9/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-2.3.9/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-2.3.9/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/pb/util.py` & `tigeropen-2.3.9/tigeropen/push/pb/util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/push_client.py` & `tigeropen-2.3.9/tigeropen/push/push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/push/stomp_push_client.py` & `tigeropen-2.3.9/tigeropen/push/stomp_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/domain/filter.py` & `tigeropen-2.3.9/tigeropen/quote/domain/filter.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/domain/quote_brief.py` & `tigeropen-2.3.9/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/domain/stock_broker.py` & `tigeropen-2.3.9/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/quote_client.py` & `tigeropen-2.3.9/tigeropen/quote/quote_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/request/model.py` & `tigeropen-2.3.9/tigeropen/quote/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/future_contract_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/market_scanner_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/market_status_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/option_chains_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/option_expirations_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/quote_brief_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/quote_timeline_history_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/quote_timeline_history_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/stock_details_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/stock_details_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/symbols_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/warrant_briefs_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/warrant_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/quote/response/warrant_filter_response.py` & `tigeropen-2.3.9/tigeropen/quote/response/warrant_filter_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/tiger_open_client.py` & `tigeropen-2.3.9/tigeropen/tiger_open_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/tiger_open_config.py` & `tigeropen-2.3.9/tigeropen/tiger_open_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/domain/account.py` & `tigeropen-2.3.9/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/domain/contract.py` & `tigeropen-2.3.9/tigeropen/trade/domain/contract.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/domain/order.py` & `tigeropen-2.3.9/tigeropen/trade/domain/order.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/domain/position.py` & `tigeropen-2.3.9/tigeropen/trade/domain/position.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/domain/prime_account.py` & `tigeropen-2.3.9/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/request/model.py` & `tigeropen-2.3.9/tigeropen/trade/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/__init__.py` & `tigeropen-2.3.9/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/account_profile_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/account_profile_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/analytics_asset_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/assets_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/contracts_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/forex_order_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/order_id_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/order_id_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/order_preview_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/order_preview_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/orders_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/orders_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/positions_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/positions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/response/transactions_response.py` & `tigeropen-2.3.9/tigeropen/trade/response/transactions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen/trade/trade_client.py` & `tigeropen-2.3.9/tigeropen/trade/trade_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.8/tigeropen.egg-info/PKG-INFO` & `tigeropen-2.3.9/tigeropen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.3.8
+Version: 2.3.9
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
```

### Comparing `tigeropen-2.3.8/tigeropen.egg-info/SOURCES.txt` & `tigeropen-2.3.9/tigeropen.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -103,14 +103,15 @@
 tigeropen/push/pb/SocketCommon_pb2.py
 tigeropen/push/pb/SocketCommon_pb2.pyi
 tigeropen/push/pb/TradeTickData.proto
 tigeropen/push/pb/TradeTickData_pb2.py
 tigeropen/push/pb/TradeTickData_pb2.pyi
 tigeropen/push/pb/__init__.py
 tigeropen/push/pb/readme.md
+tigeropen/push/pb/trade_tick.py
 tigeropen/push/pb/util.py
 tigeropen/quote/__init__.py
 tigeropen/quote/quote_client.py
 tigeropen/quote/domain/__init__.py
 tigeropen/quote/domain/bar.py
 tigeropen/quote/domain/capital_distribution.py
 tigeropen/quote/domain/filter.py
```

