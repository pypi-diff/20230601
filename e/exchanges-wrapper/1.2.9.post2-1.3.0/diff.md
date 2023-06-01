# Comparing `tmp/exchanges-wrapper-1.2.9.post2.tar.gz` & `tmp/exchanges-wrapper-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchanges-wrapper-1.2.9.post2.tar", last modified: Sat Feb  4 17:01:11 2023, max compression
+gzip compressed data, was "exchanges-wrapper-1.3.0.tar", last modified: Thu Jun  1 19:17:04 2023, max compression
```

## Comparing `exchanges-wrapper-1.2.9.post2.tar` & `exchanges-wrapper-1.3.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.2.9.post2/.deepsource.toml
--rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.2.9.post2/.dockerignore
--rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.2.9.post2/.github/FUNDING.yml
--rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.2.9.post2/.github/dependabot.yml
--rwxr-xr-x   0        0        0     4533 2023-02-04 15:12:03.486985 exchanges-wrapper-1.2.9.post2/CHANGELOG.md
--rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.2.9.post2/Dockerfile
--rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.2.9.post2/LICENSE.md
--rw-r--r--   0        0        0     6633 2023-02-04 16:54:49.040299 exchanges-wrapper-1.2.9.post2/README.md
--rw-r--r--   0        0        0    14153 2023-02-04 15:12:03.486985 exchanges-wrapper-1.2.9.post2/example/exch_client.py
--rwxr-xr-x   0        0        0      227 2022-06-05 17:07:32.203624 exchanges-wrapper-1.2.9.post2/example/ms_cfg.toml
--rw-r--r--   0        0        0     1289 2023-02-04 15:12:03.486985 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/__init__.py
--rw-r--r--   0        0        0    45676 2022-12-15 14:07:38.807179 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/api_pb2.py
--rw-r--r--   0        0        0    41250 2022-12-15 10:25:18.509000 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/api_pb2_grpc.py
--rw-r--r--   0        0        0    19515 2023-02-04 15:12:03.490966 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/bitfinex_parser.py
--rw-r--r--   0        0        0     5737 2023-02-04 16:52:19.854578 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/c_structures.py
--rw-r--r--   0        0        0    59837 2023-02-04 16:52:30.821726 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/client.py
--rw-r--r--   0        0        0     2601 2023-02-04 15:12:03.490966 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/definitions.py
--rw-r--r--   0        0        0      796 2023-02-04 15:12:03.490966 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/errors.py
--rw-r--r--   0        0        0    12494 2023-02-04 15:12:03.490966 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/events.py
--rwxr-xr-x   0        0        0    43622 2023-02-04 16:47:28.918272 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/exch_srv.py
--rw-r--r--   0        0        0     3673 2023-01-08 11:24:31.803555 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/exch_srv_cfg.toml.template
--rw-r--r--   0        0        0    10470 2023-02-04 15:12:03.494948 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/http_client.py
--rw-r--r--   0        0        0    15723 2023-02-04 15:12:03.494948 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/huobi_parser.py
--rw-r--r--   0        0        0    18411 2023-02-04 15:12:03.494948 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/okx_parser.py
--rw-r--r--   0        0        0    12171 2022-12-15 14:07:38.807179 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/proto/exchanges_wrapper/api.proto
--rw-r--r--   0        0        0    24576 2023-02-04 15:12:03.494948 exchanges-wrapper-1.2.9.post2/exchanges_wrapper/web_sockets.py
--rw-r--r--   0        0        0      940 2022-09-20 08:03:52.893747 exchanges-wrapper-1.2.9.post2/pyproject.toml
--rw-r--r--   0        0        0       74 2022-09-20 08:03:52.885747 exchanges-wrapper-1.2.9.post2/requirements.txt
--rw-r--r--   0        0        0     7456 1970-01-01 00:00:00.000000 exchanges-wrapper-1.2.9.post2/PKG-INFO
+-rw-r--r--   0        0        0      165 2022-06-06 16:51:29.613842 exchanges-wrapper-1.3.0/.deepsource.toml
+-rw-r--r--   0        0        0       78 2022-09-23 15:45:46.921324 exchanges-wrapper-1.3.0/.dockerignore
+-rw-r--r--   0        0        0       71 2022-06-07 10:33:14.780369 exchanges-wrapper-1.3.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      502 2022-09-23 19:36:49.587213 exchanges-wrapper-1.3.0/.github/dependabot.yml
+-rwxr-xr-x   0        0        0     5996 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0      641 2022-09-23 17:33:34.192514 exchanges-wrapper-1.3.0/Dockerfile
+-rw-r--r--   0        0        0     1114 2022-05-29 08:10:10.422624 exchanges-wrapper-1.3.0/LICENSE.md
+-rw-r--r--   0        0        0     6698 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0/README.md
+-rw-r--r--   0        0        0    15398 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/example/exch_client.py
+-rwxr-xr-x   0        0        0      159 2023-02-22 15:25:52.460883 exchanges-wrapper-1.3.0/example/ms_cfg.toml
+-rw-r--r--   0        0        0     1287 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/__init__.py
+-rw-r--r--   0        0        0    45215 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/api_pb2.py
+-rw-r--r--   0        0        0    44445 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/api_pb2_grpc.py
+-rw-r--r--   0        0        0    19618 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/bitfinex_parser.py
+-rw-r--r--   0        0        0     6048 2023-04-01 15:08:34.303021 exchanges-wrapper-1.3.0/exchanges_wrapper/c_structures.py
+-rw-r--r--   0        0        0    61936 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/client.py
+-rw-r--r--   0        0        0     2601 2023-02-04 15:12:03.490966 exchanges-wrapper-1.3.0/exchanges_wrapper/definitions.py
+-rw-r--r--   0        0        0      796 2023-02-04 15:12:03.490966 exchanges-wrapper-1.3.0/exchanges_wrapper/errors.py
+-rw-r--r--   0        0        0    12494 2023-02-24 16:57:17.581054 exchanges-wrapper-1.3.0/exchanges_wrapper/events.py
+-rwxr-xr-x   0        0        0    43798 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/exch_srv.py
+-rw-r--r--   0        0        0     4189 2023-02-22 15:25:52.464921 exchanges-wrapper-1.3.0/exchanges_wrapper/exch_srv_cfg.toml.template
+-rw-r--r--   0        0        0    10270 2023-05-23 10:25:45.286853 exchanges-wrapper-1.3.0/exchanges_wrapper/http_client.py
+-rw-r--r--   0        0        0    15723 2023-02-04 15:12:03.494948 exchanges-wrapper-1.3.0/exchanges_wrapper/huobi_parser.py
+-rw-r--r--   0        0        0    16098 2023-03-02 12:37:56.947270 exchanges-wrapper-1.3.0/exchanges_wrapper/okx_parser.py
+-rw-r--r--   0        0        0    12097 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/proto/exchanges_wrapper/api.proto
+-rw-r--r--   0        0        0    22294 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/exchanges_wrapper/web_sockets.py
+-rw-r--r--   0        0        0      986 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0      105 2023-06-01 19:11:17.054849 exchanges-wrapper-1.3.0/requirements.txt
+-rw-r--r--   0        0        0     7577 1970-01-01 00:00:00.000000 exchanges-wrapper-1.3.0/PKG-INFO
```

### Comparing `exchanges-wrapper-1.2.9.post2/CHANGELOG.md` & `exchanges-wrapper-1.3.0/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,51 @@
+## v1.3.0 - 2023-06-01
+### Fix
+* exchanges_wrapper.client.Client.cancel_all_orders() set correct 'status' for cancelled orders
+
+### Update
+* protobuf format for CancelAllOrders() and OnOrderUpdate(). Now simple use ```result = eval(json.loads(res.result))```
+for unpack incoming message. **Not compatible with earlier versions**
+* dependencies
+
+## v1.2.10-6-HotFix - 2023-04-12
+### Fix
+* Binance: REST API update for endpoint: GET /api/v3/exchangeInfo was changed MIN_NOTIONAL filter
+
+## v1.2.10-5 - 2023-04-05
+### Update
+* Minor improvements
+
+## v1.2.10-4 - 2023-03-04
+### Fix
+* OKX: intersection wss streams for several trades on one client (same account). WSS buffer moved from
+client instance to EventsDataStream instance
+
+## v1.2.10-3 - 2023-03-01
+### Fix
+* OKX: FetchOpenOrders(): getting orders list for all pair per account instead specific one pair
+
+## v1.2.10-2 - 2023-02-26
+### Added for new features
+* CheckStream() method which request active WSS for trade_id
+
+## v1.2.10 - 2023-02-22
+### Added for new features
+* Add method TransferToMaster():
+
+>Send request to transfer asset from subaccount to main account  
+Binance, OKX: not additional settings needed  
+Bitfinex: for subaccount setting 2FA method, set WITHDRAWAL permission for API key,  
+  in config for subaccount set 2FA key and master account EMail  
+Huobi: in config for subaccount set master_name for Main account
+
+### Update
+* Up requirements aiohttp to 3.8.4
+* Some minor improvements
+
 ## v1.2.9-2 - 2023-02-04
 ### Fixed
 * Fix DogsTailFarmer/martin-binance#50
 
 ### Update
 * Remove unnecessary shebang
```

### Comparing `exchanges-wrapper-1.2.9.post2/Dockerfile` & `exchanges-wrapper-1.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post2/LICENSE.md` & `exchanges-wrapper-1.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post2/README.md` & `exchanges-wrapper-1.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 <a href="https://badge.fury.io/py/exchanges-wrapper"><img src="https://badge.fury.io/py/exchanges-wrapper.svg" alt="PyPI version"></a>
 <a href="https://codeclimate.com/github/DogsTailFarmer/exchanges-wrapper/maintainability"><img src="https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/maintainability" /></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=resolved+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=active+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_exchanges-wrapper" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_exchanges-wrapper&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/exchanges-wrapper" target="_blank"><img alt="Downloads" title="Downloads" src="https://pepy.tech/badge/exchanges-wrapper/month"/></a>
 ***
+From 1.2.10 update exch_srv_cfg.toml (see CHANGELOG for details)
 ***
 
 ## exchanges-wrapper vs binance.py
 The main difference is the development of the project for trading with many exchanges.
 
 Next is adding a new module ```exchanges_wrapper/exch_srv.py``` as a multiplexer layer, providing simultaneous async interaction for many accounts
 and many trading pairs through one connection. It's powered by [gRPC](https://grpc.io/about/)
```

#### html2text {}

```diff
@@ -2,47 +2,48 @@
 167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/
                                 Logo%202v3.svg]
 ***
     ****** Crypto exchanges API/WSS wrapper with grpc powered server ******
                   ***** Binance, Bitfinex, Huobi, OKX, *****
                           **** For SPOT markets ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/
-maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** *** ##
-exchanges-wrapper vs binance.py The main difference is the development of the
-project for trading with many exchanges. Next is adding a new module
-```exchanges_wrapper/exch_srv.py``` as a multiplexer layer, providing
-simultaneous async interaction for many accounts and many trading pairs through
-one connection. It's powered by [gRPC](https://grpc.io/about/) Remote Procedure
-Call framework. Warning. Coverage of overridden binance.py packages is
-significant but not complete. Served methods describes into ```example/
-exch_client.py``` ### Initial capabilities (inherited from binance.py) - Covers
-general endpoints (test connectivity and get exchange information's) - Covers
-market data endpoints - Covers Account endpoints (create and manage orders) -
-Covers user data stream (receive real time user updates) - Covers web socket
-streams (receive real time market updates) - Async support - Auto reconnect
-after exchanges API or network failure - Completely free and without
-limitations ### Added Features - Multi exchanges support - Adaptive algorithm
-to ensure maximum performance and avoid exceeding the rates limits -
-Passthrough logging ## Extra exchanges implementation features - Binance REST
-API and WSS are accepted as basic, connection of other exchanges wrapped their
-API to Binance compatible - For other, some data cannot be obtained by directly
-calling one method, it is generated by a synthetic or calculation method - Some
-exchanges have not any testing or "paper trading" features, therefore,
-application development and testing is possible only at real bidding. First,
-run applications on the [Binance Spot Test Network](https://
-testnet.binance.vision/) or Bitfinex test account. ## Get started ### Prepare
-exchange account * Create account on [Binance](https://accounts.binance.com/en/
-register?ref=QCS4OGWR) and get 10% discount on all trading fee * Create account
-on [Bitfinex](https://www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6%
-rebate fee * Create account on [HUOBI](https://www.huobi.com/en-us/topic/
-double-reward/?invite_code=9uaw3223) and get 10% cashback on all trading fee *
-Create account on [OKX](https://www.okx.com/join/2607649) and get Mystery Boxes
-worth up to $10,000 * For test purpose log in at [Binance Spot Test Network]
-(https://testnet.binance.vision/) * Create API Key * After install and first
-run specify api_key and api_secret in ```/home/ubuntu/.MartinBinance/config/
+maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** From
+1.2.10 update exch_srv_cfg.toml (see CHANGELOG for details) *** ## exchanges-
+wrapper vs binance.py The main difference is the development of the project for
+trading with many exchanges. Next is adding a new module ```exchanges_wrapper/
+exch_srv.py``` as a multiplexer layer, providing simultaneous async interaction
+for many accounts and many trading pairs through one connection. It's powered
+by [gRPC](https://grpc.io/about/) Remote Procedure Call framework. Warning.
+Coverage of overridden binance.py packages is significant but not complete.
+Served methods describes into ```example/exch_client.py``` ### Initial
+capabilities (inherited from binance.py) - Covers general endpoints (test
+connectivity and get exchange information's) - Covers market data endpoints -
+Covers Account endpoints (create and manage orders) - Covers user data stream
+(receive real time user updates) - Covers web socket streams (receive real time
+market updates) - Async support - Auto reconnect after exchanges API or network
+failure - Completely free and without limitations ### Added Features - Multi
+exchanges support - Adaptive algorithm to ensure maximum performance and avoid
+exceeding the rates limits - Passthrough logging ## Extra exchanges
+implementation features - Binance REST API and WSS are accepted as basic,
+connection of other exchanges wrapped their API to Binance compatible - For
+other, some data cannot be obtained by directly calling one method, it is
+generated by a synthetic or calculation method - Some exchanges have not any
+testing or "paper trading" features, therefore, application development and
+testing is possible only at real bidding. First, run applications on the
+[Binance Spot Test Network](https://testnet.binance.vision/) or Bitfinex test
+account. ## Get started ### Prepare exchange account * Create account on
+[Binance](https://accounts.binance.com/en/register?ref=QCS4OGWR) and get 10%
+discount on all trading fee * Create account on [Bitfinex](https://
+www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6% rebate fee * Create
+account on [HUOBI](https://www.huobi.com/en-us/topic/double-reward/
+?invite_code=9uaw3223) and get 10% cashback on all trading fee * Create account
+on [OKX](https://www.okx.com/join/2607649) and get Mystery Boxes worth up to
+$10,000 * For test purpose log in at [Binance Spot Test Network](https://
+testnet.binance.vision/) * Create API Key * After install and first run specify
+api_key and api_secret in ```/home/ubuntu/.MartinBinance/config/
 exch_srv_cfg.toml``` ### Use Docker image ```console docker pull ghcr.io/
 dogstailfarmer/exchanges-wrapper:latest ``` #### First run The structure of the
 working directory will be created and the necessary files will be copied: For
 Ubuntu it will be here: ```home/user/.MartinBinance/``` ```console docker run -
 -rm --entrypoint /bin/sh exchanges-wrapper -c "cat ./exchanges_wrapper/
 __init__.py" > init.py && \ docker run --rm --entrypoint /bin/sh exchanges-
 wrapper -c "cat ./exchanges_wrapper/exch_srv_cfg.toml.template" >
```

### Comparing `exchanges-wrapper-1.2.9.post2/example/exch_client.py` & `exchanges-wrapper-1.3.0/example/exch_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 Client example for exchanges-wrapper, examples of use of server methods are given
 """
 
 import asyncio
 import toml
 import uuid
+import simplejson as json
 # noinspection PyPackageRequirements
 import grpc
 # noinspection PyPackageRequirements
 from google.protobuf import json_format
 from exchanges_wrapper import api_pb2, api_pb2_grpc
 
 # For more channel options, please see https://grpc.io/grpc/core/group__grpc__arg__keys.html
@@ -114,21 +115,31 @@
     :param _symbol:
     :return: https://github.com/binance/binance-spot-api-docs/blob/master/user-data-stream.md#order-update
     """
     async for event in _stub.OnOrderUpdate(api_pb2.MarketRequest(
             trade_id=trade_id,
             client_id=_client_id,
             symbol=_symbol)):
-        print(f"on_order_update: {event.symbol}\n"
-              f"order_id: {event.order_id}\n"
-              f"order_status: {event.order_status}\n"
-              f"cumulative_filled_quantity: {event.cumulative_filled_quantity}\n"
-              f"quote_order_quantity: {event.quote_order_quantity}\n"
-              f"quote_asset_transacted: {event.quote_asset_transacted}\n"
-              f"client_order_id: {event.client_order_id}")
+        print(eval(json.loads(event.result)))
+
+
+async def on_balance_update(_stub, _client_id, _symbol, trade_id):
+    """
+    Get data when asset transferred or withdrawal from account
+    :param _stub:
+    :param _client_id:
+    :param _symbol:
+    :param trade_id:
+    :return:
+    """
+    async for res in _stub.OnBalanceUpdate(api_pb2.MarketRequest(
+            trade_id=trade_id,
+            client_id=_client_id,
+            symbol=_symbol)):
+        print(res.balance)
 
 
 async def fetch_open_orders(_stub, _client_id, _symbol):
     """
     Get all open orders on a symbol.
     :param _stub:
     :param _client_id:
@@ -176,15 +187,15 @@
     :param _symbol:
     :return:
      https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md#cancel-all-open-orders-on-a-symbol-trade
     """
     res = await _stub.CancelAllOrders(api_pb2.MarketRequest(
         client_id=_client_id,
         symbol=_symbol))
-    result = json_format.MessageToDict(res)
+    result = eval(json.loads(res.result))
     print(f"cancel_all_orders.result: {result}")
 
 
 async def fetch_account_information(_stub, _client_id):
     """
     Account information (USER_DATA)
     :param _stub:
@@ -302,23 +313,52 @@
         limit=_limit,
         start_time=_start_time_ms)
     )
     trades = json_format.MessageToDict(_trades).get('items', [])
     print(f"fetch_account_trade_list.trades: {trades}")
 
 
+# noinspection PyUnresolvedReferences
+async def transfer2master(_stub, symbol: str, amount: str):
+    """
+    Send request to transfer asset from subaccount to main account
+    Binance, OKX: not additional settings needed
+    Bitfinex: for subaccount setting 2FA method, set WITHDRAWAL permission for API key,
+     in config for subaccount set 2FA key and master account EMail
+    Huobi: in config for subaccount set master_name for Main account
+    :param _stub:
+    :param symbol:
+    :param amount:
+    :return:
+    """
+    try:
+        res = await _stub.TransferToMaster(api_pb2.MarketRequest, symbol=symbol, amount=amount)
+    except asyncio.CancelledError:
+        pass  # Task cancellation should not be logged as an error
+    except grpc.RpcError as ex:
+        status_code = ex.code()
+        print(f"Exception transfer {symbol} to main account: {status_code.name}, {ex.details()}")
+    except Exception as _ex:
+        print(f"Exception transfer {symbol} to main account: {_ex}")
+    else:
+        if res.success:
+            print(f"Sent {amount} {symbol} to main account")
+        else:
+            print(f"Not sent {amount} {symbol} to main account\n,{res.result}")
+
+
 # Server exception handling example for methods where it's realized
 # noinspection PyUnresolvedReferences
 async def create_limit_order(_stub, _client_id, _symbol, _id: int, buy: bool, amount: str, price: str):
     """
     Send in a new Limit order.
     :param _stub:
     :param _client_id:
     :param _symbol:
-    :param _id: A unique id among open orders. Automatically generated if not sent.
+    :param _id: A unique id among open orders. Automatically generated if not sent
     :param buy: True id BUY_side else False
     :param amount: Base asset quantity
     :param price:
     :return: https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md#new-order--trade
     """
     try:
         res = await _stub.CreateLimitOrder(api_pb2.CreateLimitOrderRequest(
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/__init__.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 """
 __authors__ = ["Th0rgal", "Jerry Fedorenko"]
 __license__ = "MIT"
 __maintainer__ = "Jerry Fedorenko"
 __contact__ = "https://github.com/DogsTailFarmer"
 __email__ = "jerry.fedorenko@yahoo.com"
 __credits__ = ["https://github.com/DanyaSWorlD"]
-__version__ = "1.2.9-2"
+__version__ = "1.3.0"
 
 from pathlib import Path
 import shutil
 #
 import platform
 print(f"Python {platform.python_version()}")
 #
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/api_pb2.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/api_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65xchanges_wrapper/api.proto\x12\x06martin\"*\n\x17OnBalanceUpdateResponse\x12\x0f\n\x07\x62\x61lance\x18\x01 \x01(\t\"\x83\x01\n\x19\x46\x65tchFundingWalletRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\r\n\x05\x61sset\x18\x03 \x01(\t\x12\x1a\n\x12need_btc_valuation\x18\x04 \x01(\x08\x12\x16\n\x0ereceive_window\x18\x05 \x01(\x03\"\xd0\x01\n\x1a\x46\x65tchFundingWalletResponse\x12=\n\x08\x62\x61lances\x18\x01 \x03(\x0b\x32+.martin.FetchFundingWalletResponse.Balances\x1as\n\x08\x42\x61lances\x12\r\n\x05\x61sset\x18\x01 \x01(\t\x12\x0c\n\x04\x66ree\x18\x02 \x01(\t\x12\x0e\n\x06locked\x18\x03 \x01(\t\x12\x0e\n\x06\x66reeze\x18\x04 \x01(\t\x12\x13\n\x0bwithdrawing\x18\x05 \x01(\t\x12\x15\n\rbtc_valuation\x18\x06 \x01(\t\"\xc7\x02\n\x13\x43\x61ncelOrderResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x19\n\x11origClientOrderId\x18\x02 \x01(\t\x12\x0f\n\x07orderId\x18\x03 \x01(\x04\x12\x13\n\x0borderListId\x18\x04 \x01(\x05\x12\x15\n\rclientOrderId\x18\x05 \x01(\t\x12\x14\n\x0ctransactTime\x18\x06 \x01(\x04\x12\r\n\x05price\x18\x07 \x01(\t\x12\x0f\n\x07origQty\x18\x08 \x01(\t\x12\x13\n\x0b\x65xecutedQty\x18\t \x01(\t\x12\x1b\n\x13\x63ummulativeQuoteQty\x18\n \x01(\t\x12\x0e\n\x06status\x18\x0b \x01(\t\x12\x13\n\x0btimeInForce\x18\x0c \x01(\t\x12\x0c\n\x04type\x18\r \x01(\t\x12\x0c\n\x04side\x18\x0e \x01(\t\x12\x1f\n\x17selfTradePreventionMode\x18\x0f \x01(\t\"[\n\x12\x43\x61ncelOrderRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08order_id\x18\x04 \x01(\x03\"\xf0\x02\n\x18\x43reateLimitOrderResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x04\x12\x13\n\x0borderListId\x18\x03 \x01(\x11\x12\x15\n\rclientOrderId\x18\x04 \x01(\t\x12\x14\n\x0ctransactTime\x18\x05 \x01(\x04\x12\r\n\x05price\x18\x06 \x01(\t\x12\x0f\n\x07origQty\x18\x07 \x01(\t\x12\x13\n\x0b\x65xecutedQty\x18\x08 \x01(\t\x12\x1b\n\x13\x63ummulativeQuoteQty\x18\t \x01(\t\x12\x0e\n\x06status\x18\n \x01(\t\x12\x13\n\x0btimeInForce\x18\x0b \x01(\t\x12\x0c\n\x04type\x18\x0c \x01(\t\x12\x0c\n\x04side\x18\r \x01(\t\x12\x12\n\nstrategyId\x18\x0e \x01(\x04\x12\x14\n\x0cstrategyType\x18\x0f \x01(\x04\x12\x13\n\x0bworkingTime\x18\x10 \x01(\x12\x12\x1f\n\x17selfTradePreventionMode\x18\x11 \x01(\t\"\x9e\x01\n\x17\x43reateLimitOrderRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08\x62uy_side\x18\x04 \x01(\x08\x12\x10\n\x08quantity\x18\x05 \x01(\t\x12\r\n\x05price\x18\x06 \x01(\t\x12\x1b\n\x13new_client_order_id\x18\x07 \x01(\x03\"\xf8\x05\n\x15OnOrderUpdateResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x17\n\x0f\x63lient_order_id\x18\x02 \x01(\t\x12\x0c\n\x04side\x18\x03 \x01(\t\x12\x12\n\norder_type\x18\x04 \x01(\t\x12\x15\n\rtime_in_force\x18\x05 \x01(\t\x12\x16\n\x0eorder_quantity\x18\x06 \x01(\t\x12\x13\n\x0border_price\x18\x07 \x01(\t\x12\x12\n\nstop_price\x18\x08 \x01(\t\x12\x18\n\x10iceberg_quantity\x18\t \x01(\t\x12\x15\n\rorder_list_id\x18\n \x01(\x11\x12\x1a\n\x12original_client_id\x18\x0b \x01(\t\x12\x16\n\x0e\x65xecution_type\x18\x0c \x01(\t\x12\x14\n\x0corder_status\x18\r \x01(\t\x12\x1b\n\x13order_reject_reason\x18\x0e \x01(\t\x12\x10\n\x08order_id\x18\x0f \x01(\x04\x12\x1e\n\x16last_executed_quantity\x18\x10 \x01(\t\x12\"\n\x1a\x63umulative_filled_quantity\x18\x11 \x01(\t\x12\x1b\n\x13last_executed_price\x18\x12 \x01(\t\x12\x19\n\x11\x63ommission_amount\x18\x13 \x01(\t\x12\x18\n\x10\x63ommission_asset\x18\x14 \x01(\t\x12\x18\n\x10transaction_time\x18\x15 \x01(\x04\x12\x10\n\x08trade_id\x18\x16 \x01(\x12\x12\x10\n\x08ignore_a\x18\x17 \x01(\x04\x12\x15\n\rin_order_book\x18\x18 \x01(\x08\x12\x15\n\ris_maker_side\x18\x19 \x01(\x08\x12\x10\n\x08ignore_b\x18\x1a \x01(\x08\x12\x1b\n\x13order_creation_time\x18\x1b \x01(\x04\x12\x1e\n\x16quote_asset_transacted\x18\x1c \x01(\t\x12#\n\x1blast_quote_asset_transacted\x18\x1d \x01(\t\x12\x1c\n\x14quote_order_quantity\x18\x1e \x01(\t\"&\n\x15OnFundsUpdateResponse\x12\r\n\x05\x66unds\x18\x01 \x01(\t\"t\n\x14OnFundsUpdateRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x12\n\nbase_asset\x18\x04 \x01(\t\x12\x13\n\x0bquote_asset\x18\x05 \x01(\t\"!\n\x0eSimpleResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\"e\n\x16OnTickerUpdateResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x12\n\nopen_price\x18\x02 \x01(\t\x12\x13\n\x0b\x63lose_price\x18\x03 \x01(\t\x12\x12\n\nevent_time\x18\x04 \x01(\x04\"\xbd\x02\n\x18\x41\x63\x63ountTradeListResponse\x12\x35\n\x05items\x18\x01 \x03(\x0b\x32&.martin.AccountTradeListResponse.Trade\x1a\xe9\x01\n\x05Trade\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x04\x12\x0f\n\x07orderId\x18\x03 \x01(\x04\x12\x13\n\x0borderListId\x18\x04 \x01(\x11\x12\r\n\x05price\x18\x05 \x01(\t\x12\x0b\n\x03qty\x18\x06 \x01(\t\x12\x10\n\x08quoteQty\x18\x07 \x01(\t\x12\x12\n\ncommission\x18\x08 \x01(\t\x12\x17\n\x0f\x63ommissionAsset\x18\t \x01(\t\x12\x0c\n\x04time\x18\n \x01(\x04\x12\x0f\n\x07isBuyer\x18\x0b \x01(\x08\x12\x0f\n\x07isMaker\x18\x0c \x01(\x08\x12\x13\n\x0bisBestMatch\x18\r \x01(\x08\"q\n\x17\x41\x63\x63ountTradeListRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\r\n\x05limit\x18\x04 \x01(\r\x12\x12\n\nstart_time\x18\x05 \x01(\x03\"%\n\x13\x46\x65tchKlinesResponse\x12\x0e\n\x06klines\x18\x01 \x03(\t\"J\n\x16OnKlinesUpdateResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x10\n\x08interval\x18\x02 \x01(\t\x12\x0e\n\x06\x63\x61ndle\x18\x03 \x01(\t\"j\n\x12\x46\x65tchKlinesRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08interval\x18\x04 \x01(\t\x12\r\n\x05limit\x18\x05 \x01(\r\"\xb7\x03\n(FetchTickerPriceChangeStatisticsResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x13\n\x0bpriceChange\x18\x02 \x01(\t\x12\x1a\n\x12priceChangePercent\x18\x03 \x01(\t\x12\x18\n\x10weightedAvgPrice\x18\x04 \x01(\t\x12\x16\n\x0eprevClosePrice\x18\x05 \x01(\t\x12\x11\n\tlastPrice\x18\x06 \x01(\t\x12\x0f\n\x07lastQty\x18\x07 \x01(\t\x12\x10\n\x08\x62idPrice\x18\x08 \x01(\t\x12\x0e\n\x06\x62idQty\x18\t \x01(\t\x12\x10\n\x08\x61skPrice\x18\n \x01(\t\x12\x0e\n\x06\x61skQty\x18\x0b \x01(\t\x12\x11\n\topenPrice\x18\x0c \x01(\t\x12\x11\n\thighPrice\x18\r \x01(\t\x12\x10\n\x08lowPrice\x18\x0e \x01(\t\x12\x0e\n\x06volume\x18\x0f \x01(\t\x12\x13\n\x0bquoteVolume\x18\x10 \x01(\t\x12\x10\n\x08openTime\x18\x11 \x01(\x04\x12\x11\n\tcloseTime\x18\x12 \x01(\x04\x12\x0f\n\x07\x66irstId\x18\x13 \x01(\x04\x12\x0e\n\x06lastId\x18\x14 \x01(\x04\x12\r\n\x05\x63ount\x18\x15 \x01(\x04\"?\n\x1e\x46\x65tchSymbolPriceTickerResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\r\n\x05price\x18\x02 \x01(\t\"J\n\x16\x46\x65tchOrderBookResponse\x12\x14\n\x0clastUpdateId\x18\x01 \x01(\x04\x12\x0c\n\x04\x62ids\x18\x02 \x03(\t\x12\x0c\n\x04\x61sks\x18\x03 \x03(\t\"\x96\x01\n\x1b\x46\x65tchAccountBalanceResponse\x12>\n\x08\x62\x61lances\x18\x01 \x03(\x0b\x32,.martin.FetchAccountBalanceResponse.Balances\x1a\x37\n\x08\x42\x61lances\x12\r\n\x05\x61sset\x18\x01 \x01(\t\x12\x0c\n\x04\x66ree\x18\x02 \x01(\t\x12\x0e\n\x06locked\x18\x03 \x01(\t\"\xd8\x13\n\x1f\x46\x65tchExchangeInfoSymbolResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x11\n\tbaseAsset\x18\x03 \x01(\t\x12\x1a\n\x12\x62\x61seAssetPrecision\x18\x04 \x01(\r\x12\x12\n\nquoteAsset\x18\x05 \x01(\t\x12\x16\n\x0equotePrecision\x18\x06 \x01(\r\x12\x1b\n\x13quoteAssetPrecision\x18\x07 \x01(\r\x12\x1f\n\x17\x62\x61seCommissionPrecision\x18\x08 \x01(\r\x12 \n\x18quoteCommissionPrecision\x18\t \x01(\r\x12\x12\n\norderTypes\x18\n \x03(\t\x12\x16\n\x0eicebergAllowed\x18\x0b \x01(\x08\x12\x12\n\nocoAllowed\x18\x0c \x01(\x08\x12\"\n\x1aquoteOrderQtyMarketAllowed\x18\r \x01(\x08\x12\x19\n\x11\x61llowTrailingStop\x18\x0e \x01(\x08\x12\x1c\n\x14\x63\x61ncelReplaceAllowed\x18\x0f \x01(\x08\x12\x1c\n\x14isSpotTradingAllowed\x18\x10 \x01(\x08\x12\x1e\n\x16isMarginTradingAllowed\x18\x11 \x01(\x08\x12@\n\x07\x66ilters\x18\x12 \x01(\x0b\x32/.martin.FetchExchangeInfoSymbolResponse.Filters\x12\x13\n\x0bpermissions\x18\x13 \x03(\t\x12&\n\x1e\x64\x65\x66\x61ultSelfTradePreventionMode\x18\x14 \x01(\t\x12\'\n\x1f\x61llowedSelfTradePreventionModes\x18\x15 \x03(\t\x1a\xd6\x0e\n\x07\x46ilters\x12V\n\x0cprice_filter\x18\x01 \x01(\x0b\x32;.martin.FetchExchangeInfoSymbolResponse.Filters.PriceFilterH\x00\x88\x01\x01\x12X\n\rpercent_price\x18\x02 \x01(\x0b\x32<.martin.FetchExchangeInfoSymbolResponse.Filters.PercentPriceH\x01\x88\x01\x01\x12N\n\x08lot_size\x18\x03 \x01(\x0b\x32\x37.martin.FetchExchangeInfoSymbolResponse.Filters.LotSizeH\x02\x88\x01\x01\x12V\n\x0cmin_notional\x18\x04 \x01(\x0b\x32;.martin.FetchExchangeInfoSymbolResponse.Filters.MinNotionalH\x03\x88\x01\x01\x12X\n\riceberg_parts\x18\x05 \x01(\x0b\x32<.martin.FetchExchangeInfoSymbolResponse.Filters.IcebergPartsH\x04\x88\x01\x01\x12[\n\x0fmarket_lot_size\x18\x06 \x01(\x0b\x32=.martin.FetchExchangeInfoSymbolResponse.Filters.MarketLotSizeH\x05\x88\x01\x01\x12Y\n\x0emax_num_orders\x18\x07 \x01(\x0b\x32<.martin.FetchExchangeInfoSymbolResponse.Filters.MaxNumOrdersH\x06\x88\x01\x01\x12\x62\n\x13max_num_algo_orders\x18\x08 \x01(\x0b\x32@.martin.FetchExchangeInfoSymbolResponse.Filters.MaxNumAlgoOrdersH\x07\x88\x01\x01\x12h\n\x16max_num_iceberg_orders\x18\t \x01(\x0b\x32\x43.martin.FetchExchangeInfoSymbolResponse.Filters.MaxNumIcebergOrdersH\x08\x88\x01\x01\x12V\n\x0cmax_position\x18\n \x01(\x0b\x32;.martin.FetchExchangeInfoSymbolResponse.Filters.MaxPositionH\t\x88\x01\x01\x1aW\n\x0bPriceFilter\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x10\n\x08minPrice\x18\x02 \x01(\t\x12\x10\n\x08maxPrice\x18\x03 \x01(\t\x12\x10\n\x08tickSize\x18\x04 \x01(\t\x1a\x66\n\x0cPercentPrice\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x14\n\x0cmultiplierUp\x18\x02 \x01(\t\x12\x16\n\x0emultiplierDown\x18\x03 \x01(\t\x12\x14\n\x0c\x61vgPriceMins\x18\x04 \x01(\r\x1aO\n\x07LotSize\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x0e\n\x06minQty\x18\x02 \x01(\t\x12\x0e\n\x06maxQty\x18\x03 \x01(\t\x12\x10\n\x08stepSize\x18\x04 \x01(\t\x1a\x63\n\x0bMinNotional\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x13\n\x0bminNotional\x18\x02 \x01(\t\x12\x15\n\rapplyToMarket\x18\x03 \x01(\x08\x12\x14\n\x0c\x61vgPriceMins\x18\x04 \x01(\r\x1a\x31\n\x0cIcebergParts\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x02 \x01(\r\x1aU\n\rMarketLotSize\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x0e\n\x06minQty\x18\x02 \x01(\t\x12\x0e\n\x06maxQty\x18\x03 \x01(\t\x12\x10\n\x08stepSize\x18\x04 \x01(\t\x1a\x38\n\x0cMaxNumOrders\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x14\n\x0cmaxNumOrders\x18\x02 \x01(\r\x1a@\n\x10MaxNumAlgoOrders\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x18\n\x10maxNumAlgoOrders\x18\x02 \x01(\r\x1a\x46\n\x13MaxNumIcebergOrders\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x1b\n\x13maxNumIcebergOrders\x18\x02 \x01(\r\x1a\x36\n\x0bMaxPosition\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x13\n\x0bmaxPosition\x18\x02 \x01(\tB\x0f\n\r_price_filterB\x10\n\x0e_percent_priceB\x0b\n\t_lot_sizeB\x0f\n\r_min_notionalB\x10\n\x0e_iceberg_partsB\x12\n\x10_market_lot_sizeB\x11\n\x0f_max_num_ordersB\x16\n\x14_max_num_algo_ordersB\x19\n\x17_max_num_iceberg_ordersB\x0f\n\r_max_position\"\x97\x03\n\x17\x43\x61ncelAllOrdersResponse\x12:\n\x05items\x18\x01 \x03(\x0b\x32+.martin.CancelAllOrdersResponse.CancelOrder\x1a\xbf\x02\n\x0b\x43\x61ncelOrder\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x19\n\x11origClientOrderId\x18\x02 \x01(\t\x12\x0f\n\x07orderId\x18\x03 \x01(\x04\x12\x13\n\x0borderListId\x18\x04 \x01(\x05\x12\x15\n\rclientOrderId\x18\x05 \x01(\t\x12\x14\n\x0ctransactTime\x18\x06 \x01(\x04\x12\r\n\x05price\x18\x07 \x01(\t\x12\x0f\n\x07origQty\x18\x08 \x01(\t\x12\x13\n\x0b\x65xecutedQty\x18\t \x01(\t\x12\x1b\n\x13\x63ummulativeQuoteQty\x18\n \x01(\t\x12\x0e\n\x06status\x18\x0b \x01(\t\x12\x13\n\x0btimeInForce\x18\x0c \x01(\t\x12\x0c\n\x04type\x18\r \x01(\t\x12\x0c\n\x04side\x18\x0e \x01(\t\x12\x1f\n\x17selfTradePreventionMode\x18\x0f \x01(\t\"v\n\x11\x46\x65tchOrderRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08order_id\x18\x04 \x01(\x03\x12\x1a\n\x12\x66illed_update_call\x18\x05 \x01(\x08\"\xa1\x03\n\x12\x46\x65tchOrderResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x04\x12\x13\n\x0borderListId\x18\x03 \x01(\x11\x12\x15\n\rclientOrderId\x18\x04 \x01(\t\x12\r\n\x05price\x18\x05 \x01(\t\x12\x0f\n\x07origQty\x18\x06 \x01(\t\x12\x13\n\x0b\x65xecutedQty\x18\x07 \x01(\t\x12\x1b\n\x13\x63ummulativeQuoteQty\x18\x08 \x01(\t\x12\x0e\n\x06status\x18\t \x01(\t\x12\x13\n\x0btimeInForce\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x0c\n\x04side\x18\x0c \x01(\t\x12\x11\n\tstopPrice\x18\r \x01(\t\x12\x12\n\nicebergQty\x18\x0e \x01(\t\x12\x0c\n\x04time\x18\x0f \x01(\x04\x12\x12\n\nupdateTime\x18\x10 \x01(\x04\x12\x11\n\tisWorking\x18\x11 \x01(\x08\x12\x13\n\x0bworkingTime\x18\x12 \x01(\x12\x12\x19\n\x11origQuoteOrderQty\x18\x13 \x01(\t\x12\x1f\n\x17selfTradePreventionMode\x18\x14 \x01(\t\"\xfc\x03\n\x17\x46\x65tchOpenOrdersResponse\x12\x14\n\x0crate_limiter\x18\x01 \x01(\x05\x12\x34\n\x05items\x18\x02 \x03(\x0b\x32%.martin.FetchOpenOrdersResponse.Order\x1a\x94\x03\n\x05Order\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x04\x12\x13\n\x0borderListId\x18\x03 \x01(\x11\x12\x15\n\rclientOrderId\x18\x04 \x01(\t\x12\r\n\x05price\x18\x05 \x01(\t\x12\x0f\n\x07origQty\x18\x06 \x01(\t\x12\x13\n\x0b\x65xecutedQty\x18\x07 \x01(\t\x12\x1b\n\x13\x63ummulativeQuoteQty\x18\x08 \x01(\t\x12\x0e\n\x06status\x18\t \x01(\t\x12\x13\n\x0btimeInForce\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x0c\n\x04side\x18\x0c \x01(\t\x12\x11\n\tstopPrice\x18\r \x01(\t\x12\x12\n\nicebergQty\x18\x0e \x01(\t\x12\x0c\n\x04time\x18\x0f \x01(\x04\x12\x12\n\nupdateTime\x18\x10 \x01(\x04\x12\x11\n\tisWorking\x18\x11 \x01(\x08\x12\x19\n\x11origQuoteOrderQty\x18\x12 \x01(\t\x12\x13\n\x0bworkingTime\x18\x13 \x01(\x12\x12\x1f\n\x17selfTradePreventionMode\x18\x14 \x01(\t\"D\n\rMarketRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\"\x81\x01\n\x12StartStreamRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x1b\n\x13market_stream_count\x18\x04 \x01(\x05\x12\x19\n\x11user_stream_count\x18\x05 \x01(\x05\"[\n\x1bOpenClientConnectionRequest\x12\x10\n\x08trade_id\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x02 \x01(\t\x12\x14\n\x0crate_limiter\x18\x03 \x01(\x05\"z\n\x16OpenClientConnectionId\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x13\n\x0bsrv_version\x18\x03 \x01(\t\x12\x14\n\x0crate_limiter\x18\x04 \x01(\x05\x12\x10\n\x08\x65xchange\x18\x05 \x01(\t\"=\n\x16\x46\x65tchServerTimeRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\".\n\x17\x46\x65tchServerTimeResponse\x12\x13\n\x0bserver_time\x18\x01 \x01(\x04\x32\xc7\x0f\n\x06Martin\x12]\n\x14OpenClientConnection\x12#.martin.OpenClientConnectionRequest\x1a\x1e.martin.OpenClientConnectionId\"\x00\x12T\n\x0f\x46\x65tchServerTime\x12\x1e.martin.OpenClientConnectionId\x1a\x1f.martin.FetchServerTimeResponse\"\x00\x12K\n\x0f\x46\x65tchOpenOrders\x12\x15.martin.MarketRequest\x1a\x1f.martin.FetchOpenOrdersResponse\"\x00\x12K\n\x0f\x43\x61ncelAllOrders\x12\x15.martin.MarketRequest\x1a\x1f.martin.FetchOpenOrdersResponse\"\x00\x12[\n\x17\x46\x65tchExchangeInfoSymbol\x12\x15.martin.MarketRequest\x1a\'.martin.FetchExchangeInfoSymbolResponse\"\x00\x12`\n\x17\x46\x65tchAccountInformation\x12\x1e.martin.OpenClientConnectionId\x1a#.martin.FetchAccountBalanceResponse\"\x00\x12I\n\x0e\x46\x65tchOrderBook\x12\x15.martin.MarketRequest\x1a\x1e.martin.FetchOrderBookResponse\"\x00\x12Y\n\x16\x46\x65tchSymbolPriceTicker\x12\x15.martin.MarketRequest\x1a&.martin.FetchSymbolPriceTickerResponse\"\x00\x12m\n FetchTickerPriceChangeStatistics\x12\x15.martin.MarketRequest\x1a\x30.martin.FetchTickerPriceChangeStatisticsResponse\"\x00\x12H\n\x0b\x46\x65tchKlines\x12\x1a.martin.FetchKlinesRequest\x1a\x1b.martin.FetchKlinesResponse\"\x00\x12\\\n\x15\x46\x65tchAccountTradeList\x12\x1f.martin.AccountTradeListRequest\x1a .martin.AccountTradeListResponse\"\x00\x12K\n\x0eOnTickerUpdate\x12\x15.martin.MarketRequest\x1a\x1e.martin.OnTickerUpdateResponse\"\x00\x30\x01\x12N\n\x11OnOrderBookUpdate\x12\x15.martin.MarketRequest\x1a\x1e.martin.FetchOrderBookResponse\"\x00\x30\x01\x12=\n\nStopStream\x12\x15.martin.MarketRequest\x1a\x16.martin.SimpleResponse\"\x00\x12\x43\n\x0bStartStream\x12\x1a.martin.StartStreamRequest\x1a\x16.martin.SimpleResponse\"\x00\x12P\n\rOnFundsUpdate\x12\x1c.martin.OnFundsUpdateRequest\x1a\x1d.martin.OnFundsUpdateResponse\"\x00\x30\x01\x12M\n\x0fOnBalanceUpdate\x12\x15.martin.MarketRequest\x1a\x1f.martin.OnBalanceUpdateResponse\"\x00\x30\x01\x12I\n\rOnOrderUpdate\x12\x15.martin.MarketRequest\x1a\x1d.martin.OnOrderUpdateResponse\"\x00\x30\x01\x12W\n\x10\x43reateLimitOrder\x12\x1f.martin.CreateLimitOrderRequest\x1a .martin.CreateLimitOrderResponse\"\x00\x12H\n\x0b\x43\x61ncelOrder\x12\x1a.martin.CancelOrderRequest\x1a\x1b.martin.CancelOrderResponse\"\x00\x12\x45\n\nFetchOrder\x12\x19.martin.FetchOrderRequest\x1a\x1a.martin.FetchOrderResponse\"\x00\x12J\n\x0eResetRateLimit\x12\x1e.martin.OpenClientConnectionId\x1a\x16.martin.SimpleResponse\"\x00\x12P\n\x0eOnKlinesUpdate\x12\x1a.martin.FetchKlinesRequest\x1a\x1e.martin.OnKlinesUpdateResponse\"\x00\x30\x01\x12]\n\x12\x46\x65tchFundingWallet\x12!.martin.FetchFundingWalletRequest\x1a\".martin.FetchFundingWalletResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65xchanges_wrapper/api.proto\x12\x06martin\"*\n\x17OnBalanceUpdateResponse\x12\x0f\n\x07\x62\x61lance\x18\x01 \x01(\t\"\x83\x01\n\x19\x46\x65tchFundingWalletRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\r\n\x05\x61sset\x18\x03 \x01(\t\x12\x1a\n\x12need_btc_valuation\x18\x04 \x01(\x08\x12\x16\n\x0ereceive_window\x18\x05 \x01(\x03\"\xd0\x01\n\x1a\x46\x65tchFundingWalletResponse\x12=\n\x08\x62\x61lances\x18\x01 \x03(\x0b\x32+.martin.FetchFundingWalletResponse.Balances\x1as\n\x08\x42\x61lances\x12\r\n\x05\x61sset\x18\x01 \x01(\t\x12\x0c\n\x04\x66ree\x18\x02 \x01(\t\x12\x0e\n\x06locked\x18\x03 \x01(\t\x12\x0e\n\x06\x66reeze\x18\x04 \x01(\t\x12\x13\n\x0bwithdrawing\x18\x05 \x01(\t\x12\x15\n\rbtc_valuation\x18\x06 \x01(\t\"\xc7\x02\n\x13\x43\x61ncelOrderResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x19\n\x11origClientOrderId\x18\x02 \x01(\t\x12\x0f\n\x07orderId\x18\x03 \x01(\x04\x12\x13\n\x0borderListId\x18\x04 \x01(\x05\x12\x15\n\rclientOrderId\x18\x05 \x01(\t\x12\x14\n\x0ctransactTime\x18\x06 \x01(\x04\x12\r\n\x05price\x18\x07 \x01(\t\x12\x0f\n\x07origQty\x18\x08 \x01(\t\x12\x13\n\x0b\x65xecutedQty\x18\t \x01(\t\x12\x1b\n\x13\x63ummulativeQuoteQty\x18\n \x01(\t\x12\x0e\n\x06status\x18\x0b \x01(\t\x12\x13\n\x0btimeInForce\x18\x0c \x01(\t\x12\x0c\n\x04type\x18\r \x01(\t\x12\x0c\n\x04side\x18\x0e \x01(\t\x12\x1f\n\x17selfTradePreventionMode\x18\x0f \x01(\t\"[\n\x12\x43\x61ncelOrderRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08order_id\x18\x04 \x01(\x03\"\xf0\x02\n\x18\x43reateLimitOrderResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x04\x12\x13\n\x0borderListId\x18\x03 \x01(\x11\x12\x15\n\rclientOrderId\x18\x04 \x01(\t\x12\x14\n\x0ctransactTime\x18\x05 \x01(\x04\x12\r\n\x05price\x18\x06 \x01(\t\x12\x0f\n\x07origQty\x18\x07 \x01(\t\x12\x13\n\x0b\x65xecutedQty\x18\x08 \x01(\t\x12\x1b\n\x13\x63ummulativeQuoteQty\x18\t \x01(\t\x12\x0e\n\x06status\x18\n \x01(\t\x12\x13\n\x0btimeInForce\x18\x0b \x01(\t\x12\x0c\n\x04type\x18\x0c \x01(\t\x12\x0c\n\x04side\x18\r \x01(\t\x12\x12\n\nstrategyId\x18\x0e \x01(\x04\x12\x14\n\x0cstrategyType\x18\x0f \x01(\x04\x12\x13\n\x0bworkingTime\x18\x10 \x01(\x12\x12\x1f\n\x17selfTradePreventionMode\x18\x11 \x01(\t\"\x9e\x01\n\x17\x43reateLimitOrderRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08\x62uy_side\x18\x04 \x01(\x08\x12\x10\n\x08quantity\x18\x05 \x01(\t\x12\r\n\x05price\x18\x06 \x01(\t\x12\x1b\n\x13new_client_order_id\x18\x07 \x01(\x03\"\xf8\x05\n\x15OnOrderUpdateResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x17\n\x0f\x63lient_order_id\x18\x02 \x01(\t\x12\x0c\n\x04side\x18\x03 \x01(\t\x12\x12\n\norder_type\x18\x04 \x01(\t\x12\x15\n\rtime_in_force\x18\x05 \x01(\t\x12\x16\n\x0eorder_quantity\x18\x06 \x01(\t\x12\x13\n\x0border_price\x18\x07 \x01(\t\x12\x12\n\nstop_price\x18\x08 \x01(\t\x12\x18\n\x10iceberg_quantity\x18\t \x01(\t\x12\x15\n\rorder_list_id\x18\n \x01(\x11\x12\x1a\n\x12original_client_id\x18\x0b \x01(\t\x12\x16\n\x0e\x65xecution_type\x18\x0c \x01(\t\x12\x14\n\x0corder_status\x18\r \x01(\t\x12\x1b\n\x13order_reject_reason\x18\x0e \x01(\t\x12\x10\n\x08order_id\x18\x0f \x01(\x04\x12\x1e\n\x16last_executed_quantity\x18\x10 \x01(\t\x12\"\n\x1a\x63umulative_filled_quantity\x18\x11 \x01(\t\x12\x1b\n\x13last_executed_price\x18\x12 \x01(\t\x12\x19\n\x11\x63ommission_amount\x18\x13 \x01(\t\x12\x18\n\x10\x63ommission_asset\x18\x14 \x01(\t\x12\x18\n\x10transaction_time\x18\x15 \x01(\x04\x12\x10\n\x08trade_id\x18\x16 \x01(\x12\x12\x10\n\x08ignore_a\x18\x17 \x01(\x04\x12\x15\n\rin_order_book\x18\x18 \x01(\x08\x12\x15\n\ris_maker_side\x18\x19 \x01(\x08\x12\x10\n\x08ignore_b\x18\x1a \x01(\x08\x12\x1b\n\x13order_creation_time\x18\x1b \x01(\x04\x12\x1e\n\x16quote_asset_transacted\x18\x1c \x01(\t\x12#\n\x1blast_quote_asset_transacted\x18\x1d \x01(\t\x12\x1c\n\x14quote_order_quantity\x18\x1e \x01(\t\"&\n\x15OnFundsUpdateResponse\x12\r\n\x05\x66unds\x18\x01 \x01(\t\"t\n\x14OnFundsUpdateRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x12\n\nbase_asset\x18\x04 \x01(\t\x12\x13\n\x0bquote_asset\x18\x05 \x01(\t\"1\n\x0eSimpleResponse\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\x0e\n\x06result\x18\x02 \x01(\t\"e\n\x16OnTickerUpdateResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x12\n\nopen_price\x18\x02 \x01(\t\x12\x13\n\x0b\x63lose_price\x18\x03 \x01(\t\x12\x12\n\nevent_time\x18\x04 \x01(\x04\"\xbd\x02\n\x18\x41\x63\x63ountTradeListResponse\x12\x35\n\x05items\x18\x01 \x03(\x0b\x32&.martin.AccountTradeListResponse.Trade\x1a\xe9\x01\n\x05Trade\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\n\n\x02id\x18\x02 \x01(\x04\x12\x0f\n\x07orderId\x18\x03 \x01(\x04\x12\x13\n\x0borderListId\x18\x04 \x01(\x11\x12\r\n\x05price\x18\x05 \x01(\t\x12\x0b\n\x03qty\x18\x06 \x01(\t\x12\x10\n\x08quoteQty\x18\x07 \x01(\t\x12\x12\n\ncommission\x18\x08 \x01(\t\x12\x17\n\x0f\x63ommissionAsset\x18\t \x01(\t\x12\x0c\n\x04time\x18\n \x01(\x04\x12\x0f\n\x07isBuyer\x18\x0b \x01(\x08\x12\x0f\n\x07isMaker\x18\x0c \x01(\x08\x12\x13\n\x0bisBestMatch\x18\r \x01(\x08\"q\n\x17\x41\x63\x63ountTradeListRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\r\n\x05limit\x18\x04 \x01(\r\x12\x12\n\nstart_time\x18\x05 \x01(\x03\"%\n\x13\x46\x65tchKlinesResponse\x12\x0e\n\x06klines\x18\x01 \x03(\t\"J\n\x16OnKlinesUpdateResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x10\n\x08interval\x18\x02 \x01(\t\x12\x0e\n\x06\x63\x61ndle\x18\x03 \x01(\t\"j\n\x12\x46\x65tchKlinesRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08interval\x18\x04 \x01(\t\x12\r\n\x05limit\x18\x05 \x01(\r\"\xb7\x03\n(FetchTickerPriceChangeStatisticsResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x13\n\x0bpriceChange\x18\x02 \x01(\t\x12\x1a\n\x12priceChangePercent\x18\x03 \x01(\t\x12\x18\n\x10weightedAvgPrice\x18\x04 \x01(\t\x12\x16\n\x0eprevClosePrice\x18\x05 \x01(\t\x12\x11\n\tlastPrice\x18\x06 \x01(\t\x12\x0f\n\x07lastQty\x18\x07 \x01(\t\x12\x10\n\x08\x62idPrice\x18\x08 \x01(\t\x12\x0e\n\x06\x62idQty\x18\t \x01(\t\x12\x10\n\x08\x61skPrice\x18\n \x01(\t\x12\x0e\n\x06\x61skQty\x18\x0b \x01(\t\x12\x11\n\topenPrice\x18\x0c \x01(\t\x12\x11\n\thighPrice\x18\r \x01(\t\x12\x10\n\x08lowPrice\x18\x0e \x01(\t\x12\x0e\n\x06volume\x18\x0f \x01(\t\x12\x13\n\x0bquoteVolume\x18\x10 \x01(\t\x12\x10\n\x08openTime\x18\x11 \x01(\x04\x12\x11\n\tcloseTime\x18\x12 \x01(\x04\x12\x0f\n\x07\x66irstId\x18\x13 \x01(\x04\x12\x0e\n\x06lastId\x18\x14 \x01(\x04\x12\r\n\x05\x63ount\x18\x15 \x01(\x04\"?\n\x1e\x46\x65tchSymbolPriceTickerResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\r\n\x05price\x18\x02 \x01(\t\"J\n\x16\x46\x65tchOrderBookResponse\x12\x14\n\x0clastUpdateId\x18\x01 \x01(\x04\x12\x0c\n\x04\x62ids\x18\x02 \x03(\t\x12\x0c\n\x04\x61sks\x18\x03 \x03(\t\"\x96\x01\n\x1b\x46\x65tchAccountBalanceResponse\x12>\n\x08\x62\x61lances\x18\x01 \x03(\x0b\x32,.martin.FetchAccountBalanceResponse.Balances\x1a\x37\n\x08\x42\x61lances\x12\r\n\x05\x61sset\x18\x01 \x01(\t\x12\x0c\n\x04\x66ree\x18\x02 \x01(\t\x12\x0e\n\x06locked\x18\x03 \x01(\t\"\xcb\x15\n\x1f\x46\x65tchExchangeInfoSymbolResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0e\n\x06status\x18\x02 \x01(\t\x12\x11\n\tbaseAsset\x18\x03 \x01(\t\x12\x1a\n\x12\x62\x61seAssetPrecision\x18\x04 \x01(\r\x12\x12\n\nquoteAsset\x18\x05 \x01(\t\x12\x16\n\x0equotePrecision\x18\x06 \x01(\r\x12\x1b\n\x13quoteAssetPrecision\x18\x07 \x01(\r\x12\x1f\n\x17\x62\x61seCommissionPrecision\x18\x08 \x01(\r\x12 \n\x18quoteCommissionPrecision\x18\t \x01(\r\x12\x12\n\norderTypes\x18\n \x03(\t\x12\x16\n\x0eicebergAllowed\x18\x0b \x01(\x08\x12\x12\n\nocoAllowed\x18\x0c \x01(\x08\x12\"\n\x1aquoteOrderQtyMarketAllowed\x18\r \x01(\x08\x12\x19\n\x11\x61llowTrailingStop\x18\x0e \x01(\x08\x12\x1c\n\x14\x63\x61ncelReplaceAllowed\x18\x0f \x01(\x08\x12\x1c\n\x14isSpotTradingAllowed\x18\x10 \x01(\x08\x12\x1e\n\x16isMarginTradingAllowed\x18\x11 \x01(\x08\x12@\n\x07\x66ilters\x18\x12 \x01(\x0b\x32/.martin.FetchExchangeInfoSymbolResponse.Filters\x12\x13\n\x0bpermissions\x18\x13 \x03(\t\x12&\n\x1e\x64\x65\x66\x61ultSelfTradePreventionMode\x18\x14 \x01(\t\x12\'\n\x1f\x61llowedSelfTradePreventionModes\x18\x15 \x03(\t\x1a\xc9\x10\n\x07\x46ilters\x12V\n\x0cprice_filter\x18\x01 \x01(\x0b\x32;.martin.FetchExchangeInfoSymbolResponse.Filters.PriceFilterH\x00\x88\x01\x01\x12X\n\rpercent_price\x18\x02 \x01(\x0b\x32<.martin.FetchExchangeInfoSymbolResponse.Filters.PercentPriceH\x01\x88\x01\x01\x12N\n\x08lot_size\x18\x03 \x01(\x0b\x32\x37.martin.FetchExchangeInfoSymbolResponse.Filters.LotSizeH\x02\x88\x01\x01\x12V\n\x0cmin_notional\x18\x04 \x01(\x0b\x32;.martin.FetchExchangeInfoSymbolResponse.Filters.MinNotionalH\x03\x88\x01\x01\x12X\n\riceberg_parts\x18\x05 \x01(\x0b\x32<.martin.FetchExchangeInfoSymbolResponse.Filters.IcebergPartsH\x04\x88\x01\x01\x12[\n\x0fmarket_lot_size\x18\x06 \x01(\x0b\x32=.martin.FetchExchangeInfoSymbolResponse.Filters.MarketLotSizeH\x05\x88\x01\x01\x12Y\n\x0emax_num_orders\x18\x07 \x01(\x0b\x32<.martin.FetchExchangeInfoSymbolResponse.Filters.MaxNumOrdersH\x06\x88\x01\x01\x12\x62\n\x13max_num_algo_orders\x18\x08 \x01(\x0b\x32@.martin.FetchExchangeInfoSymbolResponse.Filters.MaxNumAlgoOrdersH\x07\x88\x01\x01\x12h\n\x16max_num_iceberg_orders\x18\t \x01(\x0b\x32\x43.martin.FetchExchangeInfoSymbolResponse.Filters.MaxNumIcebergOrdersH\x08\x88\x01\x01\x12V\n\x0cmax_position\x18\n \x01(\x0b\x32;.martin.FetchExchangeInfoSymbolResponse.Filters.MaxPositionH\t\x88\x01\x01\x12O\n\x08notional\x18\x0b \x01(\x0b\x32\x38.martin.FetchExchangeInfoSymbolResponse.Filters.NotionalH\n\x88\x01\x01\x1aW\n\x0bPriceFilter\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x10\n\x08minPrice\x18\x02 \x01(\t\x12\x10\n\x08maxPrice\x18\x03 \x01(\t\x12\x10\n\x08tickSize\x18\x04 \x01(\t\x1a\x66\n\x0cPercentPrice\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x14\n\x0cmultiplierUp\x18\x02 \x01(\t\x12\x16\n\x0emultiplierDown\x18\x03 \x01(\t\x12\x14\n\x0c\x61vgPriceMins\x18\x04 \x01(\r\x1aO\n\x07LotSize\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x0e\n\x06minQty\x18\x02 \x01(\t\x12\x0e\n\x06maxQty\x18\x03 \x01(\t\x12\x10\n\x08stepSize\x18\x04 \x01(\t\x1a\x63\n\x0bMinNotional\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x13\n\x0bminNotional\x18\x02 \x01(\t\x12\x15\n\rapplyToMarket\x18\x03 \x01(\x08\x12\x14\n\x0c\x61vgPriceMins\x18\x04 \x01(\r\x1a\x31\n\x0cIcebergParts\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\r\n\x05limit\x18\x02 \x01(\r\x1aU\n\rMarketLotSize\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x0e\n\x06minQty\x18\x02 \x01(\t\x12\x0e\n\x06maxQty\x18\x03 \x01(\t\x12\x10\n\x08stepSize\x18\x04 \x01(\t\x1a\x38\n\x0cMaxNumOrders\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x14\n\x0cmaxNumOrders\x18\x02 \x01(\r\x1a@\n\x10MaxNumAlgoOrders\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x18\n\x10maxNumAlgoOrders\x18\x02 \x01(\r\x1a\x46\n\x13MaxNumIcebergOrders\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x1b\n\x13maxNumIcebergOrders\x18\x02 \x01(\r\x1a\x36\n\x0bMaxPosition\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x13\n\x0bmaxPosition\x18\x02 \x01(\t\x1a\x92\x01\n\x08Notional\x12\x12\n\nfilterType\x18\x01 \x01(\t\x12\x13\n\x0bminNotional\x18\x02 \x01(\t\x12\x18\n\x10\x61pplyMinToMarket\x18\x03 \x01(\x08\x12\x13\n\x0bmaxNotional\x18\x04 \x01(\t\x12\x18\n\x10\x61pplyMaxToMarket\x18\x05 \x01(\x08\x12\x14\n\x0c\x61vgPriceMins\x18\x06 \x01(\rB\x0f\n\r_price_filterB\x10\n\x0e_percent_priceB\x0b\n\t_lot_sizeB\x0f\n\r_min_notionalB\x10\n\x0e_iceberg_partsB\x12\n\x10_market_lot_sizeB\x11\n\x0f_max_num_ordersB\x16\n\x14_max_num_algo_ordersB\x19\n\x17_max_num_iceberg_ordersB\x0f\n\r_max_positionB\x0b\n\t_notional\"v\n\x11\x46\x65tchOrderRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x10\n\x08order_id\x18\x04 \x01(\x03\x12\x1a\n\x12\x66illed_update_call\x18\x05 \x01(\x08\"\xa1\x03\n\x12\x46\x65tchOrderResponse\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x04\x12\x13\n\x0borderListId\x18\x03 \x01(\x11\x12\x15\n\rclientOrderId\x18\x04 \x01(\t\x12\r\n\x05price\x18\x05 \x01(\t\x12\x0f\n\x07origQty\x18\x06 \x01(\t\x12\x13\n\x0b\x65xecutedQty\x18\x07 \x01(\t\x12\x1b\n\x13\x63ummulativeQuoteQty\x18\x08 \x01(\t\x12\x0e\n\x06status\x18\t \x01(\t\x12\x13\n\x0btimeInForce\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x0c\n\x04side\x18\x0c \x01(\t\x12\x11\n\tstopPrice\x18\r \x01(\t\x12\x12\n\nicebergQty\x18\x0e \x01(\t\x12\x0c\n\x04time\x18\x0f \x01(\x04\x12\x12\n\nupdateTime\x18\x10 \x01(\x04\x12\x11\n\tisWorking\x18\x11 \x01(\x08\x12\x13\n\x0bworkingTime\x18\x12 \x01(\x12\x12\x19\n\x11origQuoteOrderQty\x18\x13 \x01(\t\x12\x1f\n\x17selfTradePreventionMode\x18\x14 \x01(\t\"\xfc\x03\n\x17\x46\x65tchOpenOrdersResponse\x12\x14\n\x0crate_limiter\x18\x01 \x01(\x05\x12\x34\n\x05items\x18\x02 \x03(\x0b\x32%.martin.FetchOpenOrdersResponse.Order\x1a\x94\x03\n\x05Order\x12\x0e\n\x06symbol\x18\x01 \x01(\t\x12\x0f\n\x07orderId\x18\x02 \x01(\x04\x12\x13\n\x0borderListId\x18\x03 \x01(\x11\x12\x15\n\rclientOrderId\x18\x04 \x01(\t\x12\r\n\x05price\x18\x05 \x01(\t\x12\x0f\n\x07origQty\x18\x06 \x01(\t\x12\x13\n\x0b\x65xecutedQty\x18\x07 \x01(\t\x12\x1b\n\x13\x63ummulativeQuoteQty\x18\x08 \x01(\t\x12\x0e\n\x06status\x18\t \x01(\t\x12\x13\n\x0btimeInForce\x18\n \x01(\t\x12\x0c\n\x04type\x18\x0b \x01(\t\x12\x0c\n\x04side\x18\x0c \x01(\t\x12\x11\n\tstopPrice\x18\r \x01(\t\x12\x12\n\nicebergQty\x18\x0e \x01(\t\x12\x0c\n\x04time\x18\x0f \x01(\x04\x12\x12\n\nupdateTime\x18\x10 \x01(\x04\x12\x11\n\tisWorking\x18\x11 \x01(\x08\x12\x19\n\x11origQuoteOrderQty\x18\x12 \x01(\t\x12\x13\n\x0bworkingTime\x18\x13 \x01(\x12\x12\x1f\n\x17selfTradePreventionMode\x18\x14 \x01(\t\"T\n\rMarketRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x0e\n\x06\x61mount\x18\x04 \x01(\t\"\xa0\x01\n\x12StartStreamRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x0e\n\x06symbol\x18\x03 \x01(\t\x12\x1b\n\x13market_stream_count\x18\x04 \x01(\x05\x12\x19\n\x11user_stream_count\x18\x05 \x01(\x05\x12\x1d\n\x15update_max_queue_size\x18\x06 \x01(\x08\"[\n\x1bOpenClientConnectionRequest\x12\x10\n\x08trade_id\x18\x01 \x01(\t\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x02 \x01(\t\x12\x14\n\x0crate_limiter\x18\x03 \x01(\x05\"z\n\x16OpenClientConnectionId\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\x12\x13\n\x0bsrv_version\x18\x03 \x01(\t\x12\x14\n\x0crate_limiter\x18\x04 \x01(\x05\x12\x10\n\x08\x65xchange\x18\x05 \x01(\t\"=\n\x16\x46\x65tchServerTimeRequest\x12\x11\n\tclient_id\x18\x01 \x01(\x03\x12\x10\n\x08trade_id\x18\x02 \x01(\t\".\n\x17\x46\x65tchServerTimeResponse\x12\x13\n\x0bserver_time\x18\x01 \x01(\x04\x32\xbc\x10\n\x06Martin\x12]\n\x14OpenClientConnection\x12#.martin.OpenClientConnectionRequest\x1a\x1e.martin.OpenClientConnectionId\"\x00\x12T\n\x0f\x46\x65tchServerTime\x12\x1e.martin.OpenClientConnectionId\x1a\x1f.martin.FetchServerTimeResponse\"\x00\x12K\n\x0f\x46\x65tchOpenOrders\x12\x15.martin.MarketRequest\x1a\x1f.martin.FetchOpenOrdersResponse\"\x00\x12\x42\n\x0f\x43\x61ncelAllOrders\x12\x15.martin.MarketRequest\x1a\x16.martin.SimpleResponse\"\x00\x12[\n\x17\x46\x65tchExchangeInfoSymbol\x12\x15.martin.MarketRequest\x1a\'.martin.FetchExchangeInfoSymbolResponse\"\x00\x12`\n\x17\x46\x65tchAccountInformation\x12\x1e.martin.OpenClientConnectionId\x1a#.martin.FetchAccountBalanceResponse\"\x00\x12I\n\x0e\x46\x65tchOrderBook\x12\x15.martin.MarketRequest\x1a\x1e.martin.FetchOrderBookResponse\"\x00\x12Y\n\x16\x46\x65tchSymbolPriceTicker\x12\x15.martin.MarketRequest\x1a&.martin.FetchSymbolPriceTickerResponse\"\x00\x12m\n FetchTickerPriceChangeStatistics\x12\x15.martin.MarketRequest\x1a\x30.martin.FetchTickerPriceChangeStatisticsResponse\"\x00\x12H\n\x0b\x46\x65tchKlines\x12\x1a.martin.FetchKlinesRequest\x1a\x1b.martin.FetchKlinesResponse\"\x00\x12\\\n\x15\x46\x65tchAccountTradeList\x12\x1f.martin.AccountTradeListRequest\x1a .martin.AccountTradeListResponse\"\x00\x12K\n\x0eOnTickerUpdate\x12\x15.martin.MarketRequest\x1a\x1e.martin.OnTickerUpdateResponse\"\x00\x30\x01\x12N\n\x11OnOrderBookUpdate\x12\x15.martin.MarketRequest\x1a\x1e.martin.FetchOrderBookResponse\"\x00\x30\x01\x12=\n\nStopStream\x12\x15.martin.MarketRequest\x1a\x16.martin.SimpleResponse\"\x00\x12\x43\n\x0bStartStream\x12\x1a.martin.StartStreamRequest\x1a\x16.martin.SimpleResponse\"\x00\x12P\n\rOnFundsUpdate\x12\x1c.martin.OnFundsUpdateRequest\x1a\x1d.martin.OnFundsUpdateResponse\"\x00\x30\x01\x12M\n\x0fOnBalanceUpdate\x12\x15.martin.MarketRequest\x1a\x1f.martin.OnBalanceUpdateResponse\"\x00\x30\x01\x12\x42\n\rOnOrderUpdate\x12\x15.martin.MarketRequest\x1a\x16.martin.SimpleResponse\"\x00\x30\x01\x12W\n\x10\x43reateLimitOrder\x12\x1f.martin.CreateLimitOrderRequest\x1a .martin.CreateLimitOrderResponse\"\x00\x12H\n\x0b\x43\x61ncelOrder\x12\x1a.martin.CancelOrderRequest\x1a\x1b.martin.CancelOrderResponse\"\x00\x12\x45\n\nFetchOrder\x12\x19.martin.FetchOrderRequest\x1a\x1a.martin.FetchOrderResponse\"\x00\x12J\n\x0eResetRateLimit\x12\x1e.martin.OpenClientConnectionId\x1a\x16.martin.SimpleResponse\"\x00\x12P\n\x0eOnKlinesUpdate\x12\x1a.martin.FetchKlinesRequest\x1a\x1e.martin.OnKlinesUpdateResponse\"\x00\x30\x01\x12]\n\x12\x46\x65tchFundingWallet\x12!.martin.FetchFundingWalletRequest\x1a\".martin.FetchFundingWalletResponse\"\x00\x12\x43\n\x10TransferToMaster\x12\x15.martin.MarketRequest\x1a\x16.martin.SimpleResponse\"\x00\x12>\n\x0b\x43heckStream\x12\x15.martin.MarketRequest\x1a\x16.martin.SimpleResponse\"\x00\x62\x06proto3')
 
 
 
 _ONBALANCEUPDATERESPONSE = DESCRIPTOR.message_types_by_name['OnBalanceUpdateResponse']
 _FETCHFUNDINGWALLETREQUEST = DESCRIPTOR.message_types_by_name['FetchFundingWalletRequest']
 _FETCHFUNDINGWALLETRESPONSE = DESCRIPTOR.message_types_by_name['FetchFundingWalletResponse']
 _FETCHFUNDINGWALLETRESPONSE_BALANCES = _FETCHFUNDINGWALLETRESPONSE.nested_types_by_name['Balances']
@@ -50,16 +50,15 @@
 _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MINNOTIONAL = _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS.nested_types_by_name['MinNotional']
 _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_ICEBERGPARTS = _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS.nested_types_by_name['IcebergParts']
 _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MARKETLOTSIZE = _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS.nested_types_by_name['MarketLotSize']
 _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMORDERS = _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS.nested_types_by_name['MaxNumOrders']
 _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMALGOORDERS = _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS.nested_types_by_name['MaxNumAlgoOrders']
 _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMICEBERGORDERS = _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS.nested_types_by_name['MaxNumIcebergOrders']
 _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXPOSITION = _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS.nested_types_by_name['MaxPosition']
-_CANCELALLORDERSRESPONSE = DESCRIPTOR.message_types_by_name['CancelAllOrdersResponse']
-_CANCELALLORDERSRESPONSE_CANCELORDER = _CANCELALLORDERSRESPONSE.nested_types_by_name['CancelOrder']
+_FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_NOTIONAL = _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS.nested_types_by_name['Notional']
 _FETCHORDERREQUEST = DESCRIPTOR.message_types_by_name['FetchOrderRequest']
 _FETCHORDERRESPONSE = DESCRIPTOR.message_types_by_name['FetchOrderResponse']
 _FETCHOPENORDERSRESPONSE = DESCRIPTOR.message_types_by_name['FetchOpenOrdersResponse']
 _FETCHOPENORDERSRESPONSE_ORDER = _FETCHOPENORDERSRESPONSE.nested_types_by_name['Order']
 _MARKETREQUEST = DESCRIPTOR.message_types_by_name['MarketRequest']
 _STARTSTREAMREQUEST = DESCRIPTOR.message_types_by_name['StartStreamRequest']
 _OPENCLIENTCONNECTIONREQUEST = DESCRIPTOR.message_types_by_name['OpenClientConnectionRequest']
@@ -306,14 +305,21 @@
 
     'MaxPosition' : _reflection.GeneratedProtocolMessageType('MaxPosition', (_message.Message,), {
       'DESCRIPTOR' : _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXPOSITION,
       '__module__' : 'exchanges_wrapper.api_pb2'
       # @@protoc_insertion_point(class_scope:martin.FetchExchangeInfoSymbolResponse.Filters.MaxPosition)
       })
     ,
+
+    'Notional' : _reflection.GeneratedProtocolMessageType('Notional', (_message.Message,), {
+      'DESCRIPTOR' : _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_NOTIONAL,
+      '__module__' : 'exchanges_wrapper.api_pb2'
+      # @@protoc_insertion_point(class_scope:martin.FetchExchangeInfoSymbolResponse.Filters.Notional)
+      })
+    ,
     'DESCRIPTOR' : _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS,
     '__module__' : 'exchanges_wrapper.api_pb2'
     # @@protoc_insertion_point(class_scope:martin.FetchExchangeInfoSymbolResponse.Filters)
     })
   ,
   'DESCRIPTOR' : _FETCHEXCHANGEINFOSYMBOLRESPONSE,
   '__module__' : 'exchanges_wrapper.api_pb2'
@@ -327,29 +333,15 @@
 _sym_db.RegisterMessage(FetchExchangeInfoSymbolResponse.Filters.MinNotional)
 _sym_db.RegisterMessage(FetchExchangeInfoSymbolResponse.Filters.IcebergParts)
 _sym_db.RegisterMessage(FetchExchangeInfoSymbolResponse.Filters.MarketLotSize)
 _sym_db.RegisterMessage(FetchExchangeInfoSymbolResponse.Filters.MaxNumOrders)
 _sym_db.RegisterMessage(FetchExchangeInfoSymbolResponse.Filters.MaxNumAlgoOrders)
 _sym_db.RegisterMessage(FetchExchangeInfoSymbolResponse.Filters.MaxNumIcebergOrders)
 _sym_db.RegisterMessage(FetchExchangeInfoSymbolResponse.Filters.MaxPosition)
-
-CancelAllOrdersResponse = _reflection.GeneratedProtocolMessageType('CancelAllOrdersResponse', (_message.Message,), {
-
-  'CancelOrder' : _reflection.GeneratedProtocolMessageType('CancelOrder', (_message.Message,), {
-    'DESCRIPTOR' : _CANCELALLORDERSRESPONSE_CANCELORDER,
-    '__module__' : 'exchanges_wrapper.api_pb2'
-    # @@protoc_insertion_point(class_scope:martin.CancelAllOrdersResponse.CancelOrder)
-    })
-  ,
-  'DESCRIPTOR' : _CANCELALLORDERSRESPONSE,
-  '__module__' : 'exchanges_wrapper.api_pb2'
-  # @@protoc_insertion_point(class_scope:martin.CancelAllOrdersResponse)
-  })
-_sym_db.RegisterMessage(CancelAllOrdersResponse)
-_sym_db.RegisterMessage(CancelAllOrdersResponse.CancelOrder)
+_sym_db.RegisterMessage(FetchExchangeInfoSymbolResponse.Filters.Notional)
 
 FetchOrderRequest = _reflection.GeneratedProtocolMessageType('FetchOrderRequest', (_message.Message,), {
   'DESCRIPTOR' : _FETCHORDERREQUEST,
   '__module__' : 'exchanges_wrapper.api_pb2'
   # @@protoc_insertion_point(class_scope:martin.FetchOrderRequest)
   })
 _sym_db.RegisterMessage(FetchOrderRequest)
@@ -441,83 +433,81 @@
   _ONORDERUPDATERESPONSE._serialized_start=1384
   _ONORDERUPDATERESPONSE._serialized_end=2144
   _ONFUNDSUPDATERESPONSE._serialized_start=2146
   _ONFUNDSUPDATERESPONSE._serialized_end=2184
   _ONFUNDSUPDATEREQUEST._serialized_start=2186
   _ONFUNDSUPDATEREQUEST._serialized_end=2302
   _SIMPLERESPONSE._serialized_start=2304
-  _SIMPLERESPONSE._serialized_end=2337
-  _ONTICKERUPDATERESPONSE._serialized_start=2339
-  _ONTICKERUPDATERESPONSE._serialized_end=2440
-  _ACCOUNTTRADELISTRESPONSE._serialized_start=2443
-  _ACCOUNTTRADELISTRESPONSE._serialized_end=2760
-  _ACCOUNTTRADELISTRESPONSE_TRADE._serialized_start=2527
-  _ACCOUNTTRADELISTRESPONSE_TRADE._serialized_end=2760
-  _ACCOUNTTRADELISTREQUEST._serialized_start=2762
-  _ACCOUNTTRADELISTREQUEST._serialized_end=2875
-  _FETCHKLINESRESPONSE._serialized_start=2877
-  _FETCHKLINESRESPONSE._serialized_end=2914
-  _ONKLINESUPDATERESPONSE._serialized_start=2916
-  _ONKLINESUPDATERESPONSE._serialized_end=2990
-  _FETCHKLINESREQUEST._serialized_start=2992
-  _FETCHKLINESREQUEST._serialized_end=3098
-  _FETCHTICKERPRICECHANGESTATISTICSRESPONSE._serialized_start=3101
-  _FETCHTICKERPRICECHANGESTATISTICSRESPONSE._serialized_end=3540
-  _FETCHSYMBOLPRICETICKERRESPONSE._serialized_start=3542
-  _FETCHSYMBOLPRICETICKERRESPONSE._serialized_end=3605
-  _FETCHORDERBOOKRESPONSE._serialized_start=3607
-  _FETCHORDERBOOKRESPONSE._serialized_end=3681
-  _FETCHACCOUNTBALANCERESPONSE._serialized_start=3684
-  _FETCHACCOUNTBALANCERESPONSE._serialized_end=3834
+  _SIMPLERESPONSE._serialized_end=2353
+  _ONTICKERUPDATERESPONSE._serialized_start=2355
+  _ONTICKERUPDATERESPONSE._serialized_end=2456
+  _ACCOUNTTRADELISTRESPONSE._serialized_start=2459
+  _ACCOUNTTRADELISTRESPONSE._serialized_end=2776
+  _ACCOUNTTRADELISTRESPONSE_TRADE._serialized_start=2543
+  _ACCOUNTTRADELISTRESPONSE_TRADE._serialized_end=2776
+  _ACCOUNTTRADELISTREQUEST._serialized_start=2778
+  _ACCOUNTTRADELISTREQUEST._serialized_end=2891
+  _FETCHKLINESRESPONSE._serialized_start=2893
+  _FETCHKLINESRESPONSE._serialized_end=2930
+  _ONKLINESUPDATERESPONSE._serialized_start=2932
+  _ONKLINESUPDATERESPONSE._serialized_end=3006
+  _FETCHKLINESREQUEST._serialized_start=3008
+  _FETCHKLINESREQUEST._serialized_end=3114
+  _FETCHTICKERPRICECHANGESTATISTICSRESPONSE._serialized_start=3117
+  _FETCHTICKERPRICECHANGESTATISTICSRESPONSE._serialized_end=3556
+  _FETCHSYMBOLPRICETICKERRESPONSE._serialized_start=3558
+  _FETCHSYMBOLPRICETICKERRESPONSE._serialized_end=3621
+  _FETCHORDERBOOKRESPONSE._serialized_start=3623
+  _FETCHORDERBOOKRESPONSE._serialized_end=3697
+  _FETCHACCOUNTBALANCERESPONSE._serialized_start=3700
+  _FETCHACCOUNTBALANCERESPONSE._serialized_end=3850
   _FETCHACCOUNTBALANCERESPONSE_BALANCES._serialized_start=311
   _FETCHACCOUNTBALANCERESPONSE_BALANCES._serialized_end=366
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE._serialized_start=3837
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE._serialized_end=6357
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS._serialized_start=4479
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS._serialized_end=6357
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_PRICEFILTER._serialized_start=5404
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_PRICEFILTER._serialized_end=5491
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_PERCENTPRICE._serialized_start=5493
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_PERCENTPRICE._serialized_end=5595
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_LOTSIZE._serialized_start=5597
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_LOTSIZE._serialized_end=5676
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MINNOTIONAL._serialized_start=5678
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MINNOTIONAL._serialized_end=5777
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_ICEBERGPARTS._serialized_start=5779
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_ICEBERGPARTS._serialized_end=5828
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MARKETLOTSIZE._serialized_start=5830
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MARKETLOTSIZE._serialized_end=5915
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMORDERS._serialized_start=5917
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMORDERS._serialized_end=5973
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMALGOORDERS._serialized_start=5975
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMALGOORDERS._serialized_end=6039
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMICEBERGORDERS._serialized_start=6041
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMICEBERGORDERS._serialized_end=6111
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXPOSITION._serialized_start=6113
-  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXPOSITION._serialized_end=6167
-  _CANCELALLORDERSRESPONSE._serialized_start=6360
-  _CANCELALLORDERSRESPONSE._serialized_end=6767
-  _CANCELALLORDERSRESPONSE_CANCELORDER._serialized_start=6448
-  _CANCELALLORDERSRESPONSE_CANCELORDER._serialized_end=6767
-  _FETCHORDERREQUEST._serialized_start=6769
-  _FETCHORDERREQUEST._serialized_end=6887
-  _FETCHORDERRESPONSE._serialized_start=6890
-  _FETCHORDERRESPONSE._serialized_end=7307
-  _FETCHOPENORDERSRESPONSE._serialized_start=7310
-  _FETCHOPENORDERSRESPONSE._serialized_end=7818
-  _FETCHOPENORDERSRESPONSE_ORDER._serialized_start=7414
-  _FETCHOPENORDERSRESPONSE_ORDER._serialized_end=7818
-  _MARKETREQUEST._serialized_start=7820
-  _MARKETREQUEST._serialized_end=7888
-  _STARTSTREAMREQUEST._serialized_start=7891
-  _STARTSTREAMREQUEST._serialized_end=8020
-  _OPENCLIENTCONNECTIONREQUEST._serialized_start=8022
-  _OPENCLIENTCONNECTIONREQUEST._serialized_end=8113
-  _OPENCLIENTCONNECTIONID._serialized_start=8115
-  _OPENCLIENTCONNECTIONID._serialized_end=8237
-  _FETCHSERVERTIMEREQUEST._serialized_start=8239
-  _FETCHSERVERTIMEREQUEST._serialized_end=8300
-  _FETCHSERVERTIMERESPONSE._serialized_start=8302
-  _FETCHSERVERTIMERESPONSE._serialized_end=8348
-  _MARTIN._serialized_start=8351
-  _MARTIN._serialized_end=10342
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE._serialized_start=3853
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE._serialized_end=6616
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS._serialized_start=4495
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS._serialized_end=6616
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_PRICEFILTER._serialized_start=5501
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_PRICEFILTER._serialized_end=5588
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_PERCENTPRICE._serialized_start=5590
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_PERCENTPRICE._serialized_end=5692
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_LOTSIZE._serialized_start=5694
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_LOTSIZE._serialized_end=5773
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MINNOTIONAL._serialized_start=5775
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MINNOTIONAL._serialized_end=5874
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_ICEBERGPARTS._serialized_start=5876
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_ICEBERGPARTS._serialized_end=5925
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MARKETLOTSIZE._serialized_start=5927
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MARKETLOTSIZE._serialized_end=6012
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMORDERS._serialized_start=6014
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMORDERS._serialized_end=6070
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMALGOORDERS._serialized_start=6072
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMALGOORDERS._serialized_end=6136
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMICEBERGORDERS._serialized_start=6138
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXNUMICEBERGORDERS._serialized_end=6208
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXPOSITION._serialized_start=6210
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_MAXPOSITION._serialized_end=6264
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_NOTIONAL._serialized_start=6267
+  _FETCHEXCHANGEINFOSYMBOLRESPONSE_FILTERS_NOTIONAL._serialized_end=6413
+  _FETCHORDERREQUEST._serialized_start=6618
+  _FETCHORDERREQUEST._serialized_end=6736
+  _FETCHORDERRESPONSE._serialized_start=6739
+  _FETCHORDERRESPONSE._serialized_end=7156
+  _FETCHOPENORDERSRESPONSE._serialized_start=7159
+  _FETCHOPENORDERSRESPONSE._serialized_end=7667
+  _FETCHOPENORDERSRESPONSE_ORDER._serialized_start=7263
+  _FETCHOPENORDERSRESPONSE_ORDER._serialized_end=7667
+  _MARKETREQUEST._serialized_start=7669
+  _MARKETREQUEST._serialized_end=7753
+  _STARTSTREAMREQUEST._serialized_start=7756
+  _STARTSTREAMREQUEST._serialized_end=7916
+  _OPENCLIENTCONNECTIONREQUEST._serialized_start=7918
+  _OPENCLIENTCONNECTIONREQUEST._serialized_end=8009
+  _OPENCLIENTCONNECTIONID._serialized_start=8011
+  _OPENCLIENTCONNECTIONID._serialized_end=8133
+  _FETCHSERVERTIMEREQUEST._serialized_start=8135
+  _FETCHSERVERTIMEREQUEST._serialized_end=8196
+  _FETCHSERVERTIMERESPONSE._serialized_start=8198
+  _FETCHSERVERTIMERESPONSE._serialized_end=8244
+  _MARTIN._serialized_start=8247
+  _MARTIN._serialized_end=10355
 # @@protoc_insertion_point(module_scope)
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/api_pb2_grpc.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/api_pb2_grpc.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 '/martin.Martin/FetchOpenOrders',
                 request_serializer=exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
                 response_deserializer=exchanges__wrapper_dot_api__pb2.FetchOpenOrdersResponse.FromString,
                 )
         self.CancelAllOrders = channel.unary_unary(
                 '/martin.Martin/CancelAllOrders',
                 request_serializer=exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
-                response_deserializer=exchanges__wrapper_dot_api__pb2.FetchOpenOrdersResponse.FromString,
+                response_deserializer=exchanges__wrapper_dot_api__pb2.SimpleResponse.FromString,
                 )
         self.FetchExchangeInfoSymbol = channel.unary_unary(
                 '/martin.Martin/FetchExchangeInfoSymbol',
                 request_serializer=exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
                 response_deserializer=exchanges__wrapper_dot_api__pb2.FetchExchangeInfoSymbolResponse.FromString,
                 )
         self.FetchAccountInformation = channel.unary_unary(
@@ -98,15 +98,15 @@
                 '/martin.Martin/OnBalanceUpdate',
                 request_serializer=exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
                 response_deserializer=exchanges__wrapper_dot_api__pb2.OnBalanceUpdateResponse.FromString,
                 )
         self.OnOrderUpdate = channel.unary_stream(
                 '/martin.Martin/OnOrderUpdate',
                 request_serializer=exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
-                response_deserializer=exchanges__wrapper_dot_api__pb2.OnOrderUpdateResponse.FromString,
+                response_deserializer=exchanges__wrapper_dot_api__pb2.SimpleResponse.FromString,
                 )
         self.CreateLimitOrder = channel.unary_unary(
                 '/martin.Martin/CreateLimitOrder',
                 request_serializer=exchanges__wrapper_dot_api__pb2.CreateLimitOrderRequest.SerializeToString,
                 response_deserializer=exchanges__wrapper_dot_api__pb2.CreateLimitOrderResponse.FromString,
                 )
         self.CancelOrder = channel.unary_unary(
@@ -130,14 +130,24 @@
                 response_deserializer=exchanges__wrapper_dot_api__pb2.OnKlinesUpdateResponse.FromString,
                 )
         self.FetchFundingWallet = channel.unary_unary(
                 '/martin.Martin/FetchFundingWallet',
                 request_serializer=exchanges__wrapper_dot_api__pb2.FetchFundingWalletRequest.SerializeToString,
                 response_deserializer=exchanges__wrapper_dot_api__pb2.FetchFundingWalletResponse.FromString,
                 )
+        self.TransferToMaster = channel.unary_unary(
+                '/martin.Martin/TransferToMaster',
+                request_serializer=exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
+                response_deserializer=exchanges__wrapper_dot_api__pb2.SimpleResponse.FromString,
+                )
+        self.CheckStream = channel.unary_unary(
+                '/martin.Martin/CheckStream',
+                request_serializer=exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
+                response_deserializer=exchanges__wrapper_dot_api__pb2.SimpleResponse.FromString,
+                )
 
 
 class MartinServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def OpenClientConnection(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -279,14 +289,26 @@
 
     def FetchFundingWallet(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def TransferToMaster(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def CheckStream(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
 
 def add_MartinServicer_to_server(servicer, server):
     rpc_method_handlers = {
             'OpenClientConnection': grpc.unary_unary_rpc_method_handler(
                     servicer.OpenClientConnection,
                     request_deserializer=exchanges__wrapper_dot_api__pb2.OpenClientConnectionRequest.FromString,
                     response_serializer=exchanges__wrapper_dot_api__pb2.OpenClientConnectionId.SerializeToString,
@@ -300,15 +322,15 @@
                     servicer.FetchOpenOrders,
                     request_deserializer=exchanges__wrapper_dot_api__pb2.MarketRequest.FromString,
                     response_serializer=exchanges__wrapper_dot_api__pb2.FetchOpenOrdersResponse.SerializeToString,
             ),
             'CancelAllOrders': grpc.unary_unary_rpc_method_handler(
                     servicer.CancelAllOrders,
                     request_deserializer=exchanges__wrapper_dot_api__pb2.MarketRequest.FromString,
-                    response_serializer=exchanges__wrapper_dot_api__pb2.FetchOpenOrdersResponse.SerializeToString,
+                    response_serializer=exchanges__wrapper_dot_api__pb2.SimpleResponse.SerializeToString,
             ),
             'FetchExchangeInfoSymbol': grpc.unary_unary_rpc_method_handler(
                     servicer.FetchExchangeInfoSymbol,
                     request_deserializer=exchanges__wrapper_dot_api__pb2.MarketRequest.FromString,
                     response_serializer=exchanges__wrapper_dot_api__pb2.FetchExchangeInfoSymbolResponse.SerializeToString,
             ),
             'FetchAccountInformation': grpc.unary_unary_rpc_method_handler(
@@ -370,15 +392,15 @@
                     servicer.OnBalanceUpdate,
                     request_deserializer=exchanges__wrapper_dot_api__pb2.MarketRequest.FromString,
                     response_serializer=exchanges__wrapper_dot_api__pb2.OnBalanceUpdateResponse.SerializeToString,
             ),
             'OnOrderUpdate': grpc.unary_stream_rpc_method_handler(
                     servicer.OnOrderUpdate,
                     request_deserializer=exchanges__wrapper_dot_api__pb2.MarketRequest.FromString,
-                    response_serializer=exchanges__wrapper_dot_api__pb2.OnOrderUpdateResponse.SerializeToString,
+                    response_serializer=exchanges__wrapper_dot_api__pb2.SimpleResponse.SerializeToString,
             ),
             'CreateLimitOrder': grpc.unary_unary_rpc_method_handler(
                     servicer.CreateLimitOrder,
                     request_deserializer=exchanges__wrapper_dot_api__pb2.CreateLimitOrderRequest.FromString,
                     response_serializer=exchanges__wrapper_dot_api__pb2.CreateLimitOrderResponse.SerializeToString,
             ),
             'CancelOrder': grpc.unary_unary_rpc_method_handler(
@@ -402,14 +424,24 @@
                     response_serializer=exchanges__wrapper_dot_api__pb2.OnKlinesUpdateResponse.SerializeToString,
             ),
             'FetchFundingWallet': grpc.unary_unary_rpc_method_handler(
                     servicer.FetchFundingWallet,
                     request_deserializer=exchanges__wrapper_dot_api__pb2.FetchFundingWalletRequest.FromString,
                     response_serializer=exchanges__wrapper_dot_api__pb2.FetchFundingWalletResponse.SerializeToString,
             ),
+            'TransferToMaster': grpc.unary_unary_rpc_method_handler(
+                    servicer.TransferToMaster,
+                    request_deserializer=exchanges__wrapper_dot_api__pb2.MarketRequest.FromString,
+                    response_serializer=exchanges__wrapper_dot_api__pb2.SimpleResponse.SerializeToString,
+            ),
+            'CheckStream': grpc.unary_unary_rpc_method_handler(
+                    servicer.CheckStream,
+                    request_deserializer=exchanges__wrapper_dot_api__pb2.MarketRequest.FromString,
+                    response_serializer=exchanges__wrapper_dot_api__pb2.SimpleResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
             'martin.Martin', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
  # This class is part of an EXPERIMENTAL API.
@@ -476,15 +508,15 @@
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/martin.Martin/CancelAllOrders',
             exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
-            exchanges__wrapper_dot_api__pb2.FetchOpenOrdersResponse.FromString,
+            exchanges__wrapper_dot_api__pb2.SimpleResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def FetchExchangeInfoSymbol(request,
             target,
             options=(),
@@ -714,15 +746,15 @@
             insecure=False,
             compression=None,
             wait_for_ready=None,
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_stream(request, target, '/martin.Martin/OnOrderUpdate',
             exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
-            exchanges__wrapper_dot_api__pb2.OnOrderUpdateResponse.FromString,
+            exchanges__wrapper_dot_api__pb2.SimpleResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def CreateLimitOrder(request,
             target,
             options=(),
@@ -819,7 +851,41 @@
             timeout=None,
             metadata=None):
         return grpc.experimental.unary_unary(request, target, '/martin.Martin/FetchFundingWallet',
             exchanges__wrapper_dot_api__pb2.FetchFundingWalletRequest.SerializeToString,
             exchanges__wrapper_dot_api__pb2.FetchFundingWalletResponse.FromString,
             options, channel_credentials,
             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def TransferToMaster(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/martin.Martin/TransferToMaster',
+            exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
+            exchanges__wrapper_dot_api__pb2.SimpleResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def CheckStream(request,
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/martin.Martin/CheckStream',
+            exchanges__wrapper_dot_api__pb2.MarketRequest.SerializeToString,
+            exchanges__wrapper_dot_api__pb2.SimpleResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/bitfinex_parser.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/bitfinex_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         "SPOT"
       ]
     }
 
     return binance_account_info
 
 
-def order(res: [], response_type=None, wss_te=None) -> {}:
+def order(res: [], response_type=None, wss_te=None, cancelled=False) -> {}:
     # print(f"order.order: {res}")
     symbol = res[3][1:].replace(':', '')
     order_id = res[0]
     order_list_id = -1
     client_order_id = str(res[2]) or str()
     price = str(res[16] or 0.0)
     orig_qty = str(abs(res[7]) or 0.0)
@@ -210,14 +210,16 @@
     #
     if 'CANCELED' in res[13]:
         status = 'CANCELED'
     elif Decimal(orig_qty) > Decimal(executed_qty) > 0:
         status = 'PARTIALLY_FILLED'
     elif  Decimal(executed_qty) >= Decimal(orig_qty):
         status = 'FILLED'
+    elif cancelled:
+        status = 'CANCELED'
     else:
         status = 'NEW'
     #
     _type = "LIMIT"
     # https://docs.bitfinex.com/reference/ws-auth-trades
     if wss_te:
         executed_qty = Decimal(str(0))
@@ -300,18 +302,18 @@
             "type": _type,
             "side": side,
         }
     # print(f"order.binance_order: {binance_order}")
     return binance_order
 
 
-def orders(res: [], response_type=None) -> []:
+def orders(res: [], response_type=None, cancelled=False) -> []:
     binance_orders = []
     for _order in res:
-        i_order = order(_order, response_type=response_type)
+        i_order = order(_order, response_type=response_type, cancelled=cancelled)
         binance_orders.append(i_order)
     return binance_orders
 
 
 def order_book(res: []) -> {}:
     binance_order_book = {"lastUpdateId": int(time.time() * 1000)}
     bids = []
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/c_structures.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/c_structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import hmac
 import hashlib
 import base64
+from decimal import Decimal
 
 
 class OrderUpdateEvent:
     def __init__(self, event_data: {}):
         self.symbol = event_data["symbol"]
         self.client_order_id = event_data["clientOrderId"]
         self.side = event_data["side"]
@@ -31,14 +32,18 @@
         self.in_order_book = True
         self.is_maker_side = False
         self.ignore_b = False
         self.order_creation_time = event_data["time"]
         self.quote_asset_transacted = event_data["cummulativeQuoteQty"]
         self.last_quote_asset_transacted = "0.0"
         self.quote_order_quantity = event_data["origQuoteOrderQty"]
+        if self.order_status == 'FILLED':
+            self.last_executed_quantity = self.cumulative_filled_quantity
+            self.last_executed_price = str(Decimal(self.quote_asset_transacted) /
+                                           Decimal(self.cumulative_filled_quantity))
 
 
 class OrderTradesEvent:
     def __init__(self, event_data: {}):
         self.symbol = event_data["symbol"]
         self.client_order_id = ""
         self.side = "BUY" if event_data["isBuyer"] else "SELL"
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/client.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Union
 import decimal
 import math
 import asyncio
 import logging
 import time
 from collections import defaultdict
+import pyotp
 
 from exchanges_wrapper.http_client import ClientBinance, ClientBFX, ClientHBP, ClientOKX
 from exchanges_wrapper.errors import ExchangePyError
 from exchanges_wrapper.web_sockets import UserEventsDataStream,\
                                             MarketEventsDataStream,\
                                             BfxPrivateEventsDataStream,\
                                             HbpPrivateEventsDataStream,\
@@ -38,39 +39,41 @@
         test_net,
         api_key,
         api_secret,
         endpoint_api_public,
         endpoint_ws_public,
         endpoint_api_auth,
         endpoint_ws_auth,
-        ws_public_mbr=None,
-        passphrase=None,
-        user_agent=None,
-        proxy=str()
+        ws_public_mbr,
+        passphrase,
+        master_email,
+        master_name,
+        two_fa
     ):
         self.exchange = exchange
         self.sub_account = sub_account
         self.test_net = test_net
         self.api_key = api_key
         self.api_secret = api_secret
         self.passphrase = passphrase
         self.endpoint_api_public = endpoint_api_public
         self.endpoint_ws_public = endpoint_ws_public
         self.endpoint_api_auth = endpoint_api_auth
         self.endpoint_ws_auth = endpoint_ws_auth
         self.ws_public_mbr = ws_public_mbr
+        self.master_email = master_email
+        self.master_name = master_name
+        self.two_fa = two_fa
         #
         self.session = aiohttp.ClientSession()
         client_init_params = {
             'api_key': api_key,
             'api_secret': api_secret,
             'passphrase': passphrase,
             'endpoint': endpoint_api_auth,
-            'user_agent': user_agent,
-            'proxy': proxy,
             'session': self.session,
             'exchange': exchange,
             'sub_account': sub_account,
             'test_net': test_net
         }
 
         if exchange == 'binance':
@@ -79,26 +82,28 @@
             self.http = ClientBFX(**client_init_params)
         elif exchange == 'huobi':
             self.http = ClientHBP(**client_init_params)
         elif exchange == 'okx':
             self.http = ClientOKX(**client_init_params)
         else:
             raise UserWarning(f"Exchange {exchange} not yet connected")
-
-        self.user_agent = user_agent
-        self.proxy = proxy
+        #
         self.loaded = False
         self.symbols = {}
         self.highest_precision = None
         self.rate_limits = None
         self.data_streams = defaultdict(set)
         self.active_orders = {}
         self.wss_buffer = {}
         self.stream_queue = defaultdict(set)
+        self.on_order_update_queues = {}
         self.hbp_account_id = None
+        self.hbp_uid = None
+        self.hbp_main_account_id = None
+        self.hbp_main_uid = None
         self.ledgers_id = []
 
     async def load(self):
         infos = await self.fetch_exchange_info()
         if infos.get('serverTime'):
             # load available symbols
             self.highest_precision = 8
@@ -129,78 +134,57 @@
         if not hasattr(self, "_events"):
             # noinspection PyAttributeOutsideInit
             self._events = Events()  # skipcq: PYL-W0201
         return self._events
 
     async def start_user_events_listener(self, _trade_id, symbol):
         logger.info(f"Start '{self.exchange}' user events listener for {_trade_id}")
-
         user_data_stream = None
         if self.exchange == 'binance':
-            user_data_stream = UserEventsDataStream(self,
-                                                    self.endpoint_ws_auth,
-                                                    self.user_agent,
-                                                    self.exchange,
-                                                    _trade_id)
+            user_data_stream = UserEventsDataStream(self, self.endpoint_ws_auth, self.exchange, _trade_id)
         elif self.exchange == 'bitfinex':
-            user_data_stream = BfxPrivateEventsDataStream(self,
-                                                          self.endpoint_ws_auth,
-                                                          self.user_agent,
-                                                          self.exchange,
-                                                          _trade_id)
+            user_data_stream = BfxPrivateEventsDataStream(self, self.endpoint_ws_auth, self.exchange, _trade_id)
         elif self.exchange == 'huobi':
-            user_data_stream = HbpPrivateEventsDataStream(self,
-                                                          self.endpoint_ws_auth,
-                                                          self.user_agent,
-                                                          self.exchange,
-                                                          _trade_id,
-                                                          symbol)
+            user_data_stream = HbpPrivateEventsDataStream(self, self.endpoint_ws_auth, self.exchange, _trade_id, symbol)
         elif self.exchange == 'okx':
             user_data_stream = OkxPrivateEventsDataStream(self,
                                                           self.endpoint_ws_auth,
-                                                          self.user_agent,
                                                           self.exchange,
                                                           _trade_id,
                                                           self.symbol_to_okx(symbol))
         if user_data_stream:
             self.data_streams[_trade_id] |= {user_data_stream}
             await user_data_stream.start()
 
     async def start_market_events_listener(self, _trade_id):
         _events = self.events.registered_streams.get(self.exchange, {}).get(_trade_id, set())
         start_list = []
         if self.exchange == 'binance':
-            market_data_stream = MarketEventsDataStream(self,
-                                                        self.endpoint_ws_public,
-                                                        self.user_agent,
-                                                        self.exchange,
-                                                        _trade_id)
+            market_data_stream = MarketEventsDataStream(self, self.endpoint_ws_public, self.exchange, _trade_id)
             self.data_streams[_trade_id] |= {market_data_stream}
             start_list.append(market_data_stream.start())
         else:
             for channel in _events:
                 market_data_stream = MarketEventsDataStream(self,
                                                             self.endpoint_ws_public,
-                                                            self.user_agent,
-                                                            self.exchange,
-                                                            _trade_id,
+                                                            self.exchange, _trade_id,
                                                             channel)
                 self.data_streams[_trade_id] |= {market_data_stream}
                 start_list.append(market_data_stream.start())
         await asyncio.gather(*start_list, return_exceptions=True)
 
     async def stop_events_listener(self, _trade_id):
         logger.info(f"Stop events listener data streams for {_trade_id}")
         stopped_data_stream = self.data_streams.pop(_trade_id, set())
         for data_stream in stopped_data_stream:
             await data_stream.stop()
 
     def assert_symbol_exists(self, symbol):
         if self.loaded and symbol not in self.symbols:
-            raise ExchangePyError(f"Symbol {symbol} is not valid according to the loaded exchange infos.")
+            raise ExchangePyError(f"Symbol {symbol} is not valid according to the loaded exchange infos")
 
     def symbol_to_bfx(self, symbol) -> str:
         symbol_info = self.symbols.get(symbol)
         base_asset = symbol_info.get('baseAsset')
         quote_asset = symbol_info.get('quoteAsset')
         if len(base_asset) > 3 or len(quote_asset) > 3:
             res = f"t{base_asset}:{quote_asset}"
@@ -307,14 +291,15 @@
             trading_symbols = await self.http.send_api_call("v1/common/symbols")
             if self.hbp_account_id is None:
                 accounts = await self.http.send_api_call("v1/account/accounts", signed=True)
                 for account in accounts:
                     if account.get('type') == 'spot':
                         self.hbp_account_id = account.get('id')
                         break
+                self.hbp_uid = await self.http.send_api_call("v2/user/uid", signed=True)
             binance_res = hbp.exchange_info(server_time.get('serverTime'), trading_symbols)
         elif self.exchange == 'okx':
             params = {'instType': 'SPOT'}
             server_time = await self.fetch_server_time()
             instruments = await self.http.send_api_call("/api/v5/public/instruments", **params)
             tickers = await self.http.send_api_call("/api/v5/market/tickers", **params)
             binance_res = okx.exchange_info(server_time.get('serverTime'), instruments, tickers)
@@ -406,15 +391,15 @@
                       'limit': limit}
             res = await self.http.send_api_call(
                 "v2/account/ledger",
                 signed=True,
                 **params,
             )
             for res_i in res:
-                time_select = (int(time.time() * 1000) - res_i.get('transactTime')) < 1000 * 60
+                time_select = (int(time.time() * 1000) - res_i.get('transactTime', 0)) < 1000 * 60
                 if (time_select and res_i.get('currency').upper() in symbol and
                         res_i.get('transactId') not in self.ledgers_id):
                     self.ledgers_id.append(res_i.get('transactId'))
                     if len(self.ledgers_id) > limit:
                         del self.ledgers_id[0]
                     binance_res = hbp.on_balance_update(res_i)
                     return binance_res
@@ -607,14 +592,18 @@
         elif self.exchange == 'huobi':
             params = {'symbol': symbol.lower()}
             res = await self.http.send_api_call(
                 "market/trade",
                 **params
             )
             binance_res = hbp.fetch_symbol_price_ticker(res, symbol)
+        elif self.exchange == 'okx':
+            params = {'instId': self.symbol_to_okx(symbol)}
+            res = await self.http.send_api_call("/api/v5/market/ticker", **params)
+            binance_res = okx.fetch_symbol_price_ticker(res[0], symbol)
         return binance_res
 
     # https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md#symbol-order-book-ticker
     async def fetch_symbol_order_book_ticker(self, symbol=None):
         if symbol:
             self.assert_symbol_exists(symbol)
         return await self.http.send_api_call(
@@ -776,15 +765,15 @@
                 method="POST",
                 signed=True,
                 **params,
             )
             if res[0].get('sCode') == '0':
                 binance_res = await self.fetch_order(symbol, order_id=res[0].get('ordId'), response_type=False)
             else:
-                raise UserWarning(res[0].get('sMsg'))
+                raise UserWarning(f"Code: {res[0].get('sCode')}: {res[0].get('sMsg')}")
         return binance_res
 
     # https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md#query-order-user_data
     async def fetch_order(  # lgtm [py/similar-function]
         self,
         symbol,
         order_id=None,
@@ -954,54 +943,56 @@
             binance_res = await self.http.send_api_call(
                 "/api/v3/openOrders",
                 "DELETE",
                 params=params,
                 signed=True,
             )
         elif self.exchange == 'bitfinex':
-            orders = await self.fetch_open_orders(symbol=symbol, receive_window=receive_window)
-            orders_id = []
-            for order in orders:
-                orders_id.append(order.get('orderId'))
-            params = {'id': orders_id}
+            params = {'all': 1}
             res = await self.http.send_api_call(
                 "v2/auth/w/order/cancel/multi",
                 method="POST",
                 signed=True,
                 **params,
             )
+            active_orders = 1
+            while active_orders:
+                active_orders = await self.fetch_open_orders(symbol=symbol, receive_window=receive_window)
+                if active_orders:
+                    await asyncio.sleep(STATUS_TIMEOUT / 10)
             if res and res[6] == 'SUCCESS':
-                binance_res = bfx.orders(res[4], response_type=True)
+                res = res[4]
+                binance_res = bfx.orders(res, response_type=True, cancelled=True)
         elif self.exchange == 'huobi':
-            orders_canceled = []
             orders = await self.fetch_open_orders(symbol=symbol, receive_window=receive_window, response_type=True)
             orders_id = []
             for order in orders:
                 orders_id.append(str(order.get('orderId')))
             params = {'order-ids': orders_id}
             res = await self.http.send_api_call(
                 "v1/order/orders/batchcancel",
                 method="POST",
                 signed=True,
                 **params,
             )
-            ids_canceled = res.get('success')
+            orders_id = res.get('success', [])
             for order in orders:
-                if str(order.get('orderId')) in ids_canceled:
-                    orders_canceled.append(order)
-            binance_res = orders_canceled
+                if str(order.get('orderId')) in orders_id:
+                    order['status'] = 'CANCELED'
+                    binance_res.append(order)
         elif self.exchange == 'okx':
             orders = await self.fetch_open_orders(symbol=symbol, receive_window=receive_window, response_type=True)
             _symbol = self.symbol_to_okx(symbol)
             while orders:
                 orders_canceled = []
                 params = []
                 i = 1
                 # 20 is OKX limit fo bulk orders cancel
                 for order in orders:
+                    order['status'] = 'CANCELED'
                     orders_canceled.append(order)
                     params.append({'instId': _symbol, 'ordId': order.get('orderId')})
                     if i >= 20:
                         break
                     i += 1
                 del orders[:20]
                 res = await self.http.send_api_call(
@@ -1046,15 +1037,15 @@
                 "v1/order/openOrders",
                 signed=True,
                 **params,
             )
             # print(f"fetch_open_orders.res: {res}")
             binance_res = hbp.orders(res, response_type=response_type)
         elif self.exchange == 'okx':
-            params = {'instType': 'SPOT'}
+            params = {'instType': 'SPOT', 'instId': self.symbol_to_okx(symbol)}
             res = await self.http.send_api_call(
                 "/api/v5/trade/orders-pending",
                 signed=True,
                 **params,
             )
             # print(f"fetch_open_orders.res: {res}")
             binance_res = okx.orders(res, response_type=response_type)
@@ -1310,14 +1301,83 @@
             params = {}
             if asset:
                 params = {'ccy': self.symbol_to_okx(asset)}
             res = await self.http.send_api_call("/api/v5/asset/balances", signed=True, **params)
             binance_res = okx.funding_wallet(res)
         return binance_res
 
+    # https://binance-docs.github.io/apidocs/spot/en/#transfer-to-master-for-sub-account
+    async def transfer_to_master(self, symbol, quantity, receive_window=None):
+        binance_res = {}
+        if self.exchange == 'binance':
+            params = {"asset": symbol, "amount": quantity}
+            if receive_window:
+                params["recvWindow"] = receive_window
+            binance_res = await self.http.send_api_call(
+                "/sapi/v1/sub-account/transfer/subToMaster",
+                "POST",
+                params=params,
+                signed=True
+            )
+        elif self.exchange == 'bitfinex':
+            if self.master_email is None or self.two_fa is None:
+                raise ValueError("This query requires master_email and 2FA")
+            totp = pyotp.TOTP(self.two_fa)
+            params = {
+                "from": "exchange",
+                "to": "exchange",
+                "currency": symbol,
+                "amount": quantity,
+                "email_dst": self.master_email,
+                "tfaToken": {"method": "otp", "token": totp.now()}
+            }
+            res = await self.http.send_api_call(
+                "v2/auth/w/transfer",
+                method="POST",
+                signed=True,
+                **params,
+            )
+            logger.debug(f"transfer_to_master.res: {res}")
+            if res and isinstance(res, list) and res[6] == 'SUCCESS':
+                binance_res = {"txnId": res[0]}
+        elif self.exchange == 'huobi':
+            params = {
+                'from-user': self.hbp_uid,
+                'from-account-type': "spot",
+                'from-account': self.hbp_account_id,
+                'to-user': self.hbp_main_uid,
+                'to-account-type': "spot",
+                'to-account': self.hbp_main_account_id,
+                'currency': symbol.lower(),
+                'amount': quantity
+            }
+            res = await self.http.send_api_call(
+                "v1/account/transfer",
+                method="POST",
+                signed=True,
+                **params,
+            )
+            binance_res = {"txnId": res.get("transact-id")}
+        elif self.exchange == 'okx':
+            params = {
+                "ccy": symbol,
+                "amt": quantity,
+                "from": '18',
+                "to": '18',
+                "type": '3'
+            }
+            res = await self.http.send_api_call(
+                "/api/v5/asset/transfer",
+                method="POST",
+                signed=True,
+                **params,
+            )
+            binance_res = {"txnId": res[0].get("transId")}
+        return binance_res
+
     # https://github.com/binance/binance-spot-api-docs/blob/master/rest-api.md#account-trade-list-user_data
     async def fetch_account_trade_list(
         self,
         symbol,
         order_id=None,
         start_time=None,
         end_time=None,
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/definitions.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/definitions.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/errors.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/errors.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/events.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/events.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/exch_srv.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/exch_srv.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,18 +32,21 @@
     accounts = config.get('accounts')
     res = ()
     for account in accounts:
         if account.get('name') == _account_name:
             exchange = account['exchange']
             sub_account = account.get('sub_account_name')
             test_net = account['test_net']
+            master_email = account.get('master_email')
+            master_name = account.get('master_name')
             #
             api_key = account['api_key']
             api_secret = account['api_secret']
             passphrase = account.get('passphrase')
+            two_fa = account.get('two_fa')
             #
             endpoint = config['endpoint'][exchange]
             #
             api_public = endpoint['api_public']
             ws_public = endpoint['ws_public']
             api_auth = endpoint['api_test'] if test_net else endpoint['api_auth']
             ws_auth = endpoint['ws_test'] if test_net else endpoint['ws_auth']
@@ -57,41 +60,32 @@
                    api_key,         # 3
                    api_secret,      # 4
                    api_public,      # 5
                    ws_public,       # 6
                    api_auth,        # 7
                    ws_auth,         # 8
                    ws_public_mbr,   # 9
-                   passphrase)      # 10
+                   passphrase,      # 10
+                   master_email,    # 11
+                   master_name,     # 12
+                   two_fa,          # 13
+                   )
             break
     return res
 
 
 class OpenClient:
     open_clients = []
 
     def __init__(self, _account_name: str):
         account = get_account(_account_name)
         if account:
             self.name = _account_name
             self.real_market = not account[2]
-            self.client = Client(
-                account[0],     # exchange
-                account[1],     # sub_account
-                account[2],     # test_net
-                account[3],     # api_key
-                account[4],     # api_secret
-                account[5],     # api_public
-                account[6],     # ws_public
-                account[7],     # api_auth
-                account[8],     # ws_auth
-                account[9],     # ws_public_mbr
-                account[10],    # passphrase
-            )
-            self.on_order_update_queues = {}
+            self.client = Client(*account)
             OpenClient.open_clients.append(self)
         else:
             raise UserWarning
 
     @classmethod
     def get_id(cls, _account_name):
         _id = 0
@@ -124,14 +118,27 @@
                                    _context: grpc.aio.ServicerContext) -> api_pb2.OpenClientConnectionId:
         logger.info(f"OpenClientConnection start trade: {request.account_name}:{request.trade_id}")
         client_id = OpenClient.get_id(request.account_name)
         if not client_id:
             try:
                 open_client = OpenClient(request.account_name)
                 client_id = id(open_client)
+                if open_client.client.master_name == 'Huobi':
+                    # For HuobiPro get master account uid and account_id
+                    main_account = get_account(open_client.client.master_name)
+                    main_client = Client(*main_account)
+                    await main_client.fetch_exchange_info()
+                    if main_client.hbp_uid and main_client.hbp_account_id:
+                        open_client.client.hbp_main_uid = main_client.hbp_uid
+                        open_client.client.hbp_main_account_id = main_client.hbp_account_id
+                        logger.info(f"The values for main Huobi account were received and set:"
+                                    f" UID: {main_client.hbp_uid} and account ID: {main_client.hbp_account_id}")
+                    else:
+                        logger.warning("No account IDs were received for the Huobi master account")
+                    await main_client.close()
             except UserWarning:
                 _context.set_details(f"Account {request.account_name} not registered into"
                                      f" {WORK_PATH}/config/exch_srv_cfg.toml")
                 _context.set_code(grpc.StatusCode.FAILED_PRECONDITION)
             else:
                 try:
                     await open_client.client.load()
@@ -151,19 +158,20 @@
             exchange = OpenClient.get_client(client_id).client.exchange
             # Set rate_limiter
             Martin.rate_limiter = max(Martin.rate_limiter if Martin.rate_limiter else 0, request.rate_limiter)
             return api_pb2.OpenClientConnectionId(client_id=client_id, srv_version=__version__, exchange=exchange)
 
     async def FetchServerTime(self, request: api_pb2.OpenClientConnectionId,
                               _context: grpc.aio.ServicerContext) -> api_pb2.FetchServerTimeResponse:
-        client = OpenClient.get_client(request.client_id).client
+        open_client = OpenClient.get_client(request.client_id)
+        client = open_client.client
         try:
             res = await client.fetch_server_time()
         except Exception as ex:
-            logger.error(f"FetchServerTime for {client.open_client.name} exception: {ex}")
+            logger.error(f"FetchServerTime for {open_client.name} exception: {ex}")
             _context.set_details(f"{ex}")
             _context.set_code(grpc.StatusCode.UNKNOWN)
         else:
             server_time = res.get('serverTime')
             return api_pb2.FetchServerTimeResponse(server_time=server_time)
 
     async def ResetRateLimit(self, request: api_pb2.OpenClientConnectionId,
@@ -232,15 +240,15 @@
         response.rate_limiter = Martin.rate_limiter
         return response
 
     async def FetchOrder(self, request: api_pb2.FetchOrderRequest,
                          _context: grpc.aio.ServicerContext) -> api_pb2.FetchOrderResponse:
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
-        _queue = open_client.on_order_update_queues.get(request.trade_id)
+        _queue = client.on_order_update_queues.get(request.trade_id)
         response = api_pb2.FetchOrderResponse()
         try:
             res = await client.fetch_order(symbol=request.symbol,
                                            order_id=request.order_id,
                                            origin_client_order_id=None,
                                            receive_window=None)
         except asyncio.CancelledError:
@@ -268,34 +276,30 @@
                             event = OrderTradesEvent(trade)
                             _event = weakref.ref(event)
                             await _queue.put(_event())
             json_format.ParseDict(res, response)
         return response
 
     async def CancelAllOrders(self, request: api_pb2.MarketRequest,
-                              _context: grpc.aio.ServicerContext) -> api_pb2.CancelAllOrdersResponse:
+                              _context: grpc.aio.ServicerContext) -> api_pb2.SimpleResponse():
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
-        # message list
-        response = api_pb2.CancelAllOrdersResponse()
-        # Nested dict
-        response_order = api_pb2.CancelAllOrdersResponse.CancelOrder()
+        response = api_pb2.SimpleResponse()
         try:
             res = await client.cancel_all_orders(symbol=request.symbol, receive_window=None)
             # logger.info(f"CancelAllOrders: {res}")
         except asyncio.CancelledError:
             pass  # Task cancellation should not be logged as an error
         except Exception as ex:
             logger.error(f"CancelAllOrder for {open_client.name}:{request.symbol} exception: {ex}")
             _context.set_details(f"{ex}")
             _context.set_code(grpc.StatusCode.UNKNOWN)
         else:
-            for order in res:
-                cancel_order = json_format.ParseDict(order, response_order)
-                response.items.append(cancel_order)
+            response.success = True
+            response.result = json.dumps(str(res))
         return response
 
     async def FetchExchangeInfoSymbol(self, request: api_pb2.MarketRequest,
                                       _context: grpc.aio.ServicerContext
                                       ) -> api_pb2.FetchExchangeInfoSymbolResponse:
         client = OpenClient.get_client(request.client_id).client
         response = api_pb2.FetchExchangeInfoSymbolResponse()
@@ -310,55 +314,49 @@
         filters_res = exchange_info_symbol.pop('filters', [])
         json_format.ParseDict(exchange_info_symbol, response)
         # logger.info(f"filters: {filters_res}")
         filters = response.filters
         for _filter in filters_res:
             if _filter.get('filterType') == 'PRICE_FILTER':
                 new_filter_template = api_pb2.FetchExchangeInfoSymbolResponse.Filters.PriceFilter()
-                new_filter = json_format.ParseDict(_filter, new_filter_template)
-                filters.price_filter.CopyFrom(new_filter)
+                filters.price_filter.CopyFrom(json_format.ParseDict(_filter, new_filter_template))
             elif 'PERCENT_PRICE' in _filter.get('filterType'):
                 if _filter.get('filterType') == 'PERCENT_PRICE_BY_SIDE':
                     _filter['multiplierUp'] = _filter['bidMultiplierUp']
                     _filter['multiplierDown'] = _filter['bidMultiplierDown']
                     _filter.pop('bidMultiplierUp')
                     _filter.pop('bidMultiplierDown')
                     _filter.pop('askMultiplierUp')
                     _filter.pop('askMultiplierDown')
                 new_filter_template = api_pb2.FetchExchangeInfoSymbolResponse.Filters.PercentPrice()
-                new_filter = json_format.ParseDict(_filter, new_filter_template)
-                filters.percent_price.CopyFrom(new_filter)
+                filters.percent_price.CopyFrom(json_format.ParseDict(_filter, new_filter_template))
             elif _filter.get('filterType') == 'LOT_SIZE':
                 new_filter_template = api_pb2.FetchExchangeInfoSymbolResponse.Filters.LotSize()
-                new_filter = json_format.ParseDict(_filter, new_filter_template)
-                filters.lot_size.CopyFrom(new_filter)
+                filters.lot_size.CopyFrom(json_format.ParseDict(_filter, new_filter_template))
             elif _filter.get('filterType') == 'MIN_NOTIONAL':
                 new_filter_template = api_pb2.FetchExchangeInfoSymbolResponse.Filters.MinNotional()
-                new_filter = json_format.ParseDict(_filter, new_filter_template)
-                filters.min_notional.CopyFrom(new_filter)
+                filters.min_notional.CopyFrom(json_format.ParseDict(_filter, new_filter_template))
+            elif _filter.get('filterType') == 'NOTIONAL':
+                new_filter_template = api_pb2.FetchExchangeInfoSymbolResponse.Filters.Notional()
+                filters.notional.CopyFrom(json_format.ParseDict(_filter, new_filter_template))
             elif _filter.get('filterType') == 'ICEBERG_PARTS':
                 new_filter_template = api_pb2.FetchExchangeInfoSymbolResponse.Filters.IcebergParts()
-                new_filter = json_format.ParseDict(_filter, new_filter_template)
-                filters.iceberg_parts.CopyFrom(new_filter)
+                filters.iceberg_parts.CopyFrom(json_format.ParseDict(_filter, new_filter_template))
             elif _filter.get('filterType') == 'MARKET_LOT_SIZE':
                 new_filter_template = api_pb2.FetchExchangeInfoSymbolResponse.Filters.MarketLotSize()
-                new_filter = json_format.ParseDict(_filter, new_filter_template)
-                filters.market_lot_size.CopyFrom(new_filter)
+                filters.market_lot_size.CopyFrom(json_format.ParseDict(_filter, new_filter_template))
             elif _filter.get('filterType') == 'MAX_NUM_ORDERS':
                 new_filter_template = api_pb2.FetchExchangeInfoSymbolResponse.Filters.MaxNumOrders()
-                new_filter = json_format.ParseDict(_filter, new_filter_template)
-                filters.max_num_orders.CopyFrom(new_filter)
+                filters.max_num_orders.CopyFrom(json_format.ParseDict(_filter, new_filter_template))
             elif _filter.get('filterType') == 'MAX_NUM_ICEBERG_ORDERS':
                 new_filter_template = api_pb2.FetchExchangeInfoSymbolResponse.Filters.MaxNumIcebergOrders()
-                new_filter = json_format.ParseDict(_filter, new_filter_template)
-                filters.max_num_iceberg_orders.CopyFrom(new_filter)
+                filters.max_num_iceberg_orders.CopyFrom(json_format.ParseDict(_filter, new_filter_template))
             elif _filter.get('filterType') == 'MAX_POSITION':
                 new_filter_template = api_pb2.FetchExchangeInfoSymbolResponse.Filters.MaxPosition()
-                new_filter = json_format.ParseDict(_filter, new_filter_template)
-                filters.max_position.CopyFrom(new_filter)
+                filters.max_position.CopyFrom(json_format.ParseDict(_filter, new_filter_template))
         return response
 
     async def FetchAccountInformation(self, request: api_pb2.OpenClientConnectionId,
                                       _context: grpc.aio.ServicerContext
                                       ) -> api_pb2.FetchAccountBalanceResponse:
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
@@ -475,15 +473,15 @@
             client.events.register_event(functools.partial(
                 event_handler, _queue, client, request.trade_id, _event_type),
                 _event_type, exchange, request.trade_id)
         while True:
             _event = await _queue.get()
             if isinstance(_event, str) and _event == request.trade_id:
                 client.stream_queue.get(request.trade_id, set()).discard(_queue)
-                logger.info(f"OnKlinesUpdate: Stop market stream for {open_client.name}:{request.symbol}:{_intervals}")
+                logger.info(f"OnKlinesUpdate: Stop loop for {open_client.name}:{request.symbol}:{_intervals}")
                 return
             else:
                 # logger.info(f"OnKlinesUpdate.event: {exchange}:{_event.symbol}:{_event.kline_interval}")
                 response.symbol = _event.symbol
                 response.interval = _event.kline_interval
                 candle = [_event.kline_start_time,
                           _event.kline_open_price,
@@ -535,15 +533,15 @@
         _event_type = f"{_symbol}@miniTicker"
         client.events.register_event(functools.partial(event_handler, _queue, client, request.trade_id, _event_type),
                                      _event_type, client.exchange, request.trade_id)
         while True:
             _event = await _queue.get()
             if isinstance(_event, str) and _event == request.trade_id:
                 client.stream_queue.get(request.trade_id, set()).discard(_queue)
-                logger.info(f"OnTickerUpdate: Stop market stream for {open_client.name}: {request.symbol}")
+                logger.info(f"OnTickerUpdate: Stop loop for {open_client.name}: {request.symbol}")
                 return
             else:
                 # logger.info(f"OnTickerUpdate.event: {_event.symbol}, _event.close_price: {_event.close_price}")
                 ticker_24h = {'symbol': _event.symbol,
                               'open_price': _event.open_price,
                               'close_price': _event.close_price,
                               'event_time': _event.event_time}
@@ -551,30 +549,30 @@
                 yield response
 
     async def OnOrderBookUpdate(self, request: api_pb2.MarketRequest,
                                 _context: grpc.aio.ServicerContext) -> api_pb2.FetchOrderBookResponse:
         response = api_pb2.FetchOrderBookResponse()
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
-        _queue = asyncio.Queue(MAX_QUEUE_SIZE * 10)
+        _queue = asyncio.Queue(MAX_QUEUE_SIZE * 2)
         client.stream_queue[request.trade_id] |= {_queue}
         if client.exchange == 'okx':
             _symbol = client.symbol_to_okx(request.symbol)
         elif client.exchange == 'bitfinex':
             _symbol = client.symbol_to_bfx(request.symbol)
         else:
             _symbol = request.symbol.lower()
         _event_type = f"{_symbol}@depth5"
         client.events.register_event(functools.partial(event_handler, _queue, client, request.trade_id, _event_type),
                                      _event_type, client.exchange, request.trade_id)
         while True:
             _event = await _queue.get()
             if isinstance(_event, str) and _event == request.trade_id:
                 client.stream_queue.get(request.trade_id, set()).discard(_queue)
-                logger.info(f"OnOrderBookUpdate: Stop market stream for {open_client.name}: {request.symbol}")
+                logger.info(f"OnOrderBookUpdate: Stop loop for {open_client.name}: {request.symbol}")
                 return
             else:
                 response.Clear()
                 response.lastUpdateId = _event.last_update_id
                 for bid in _event.bids:
                     response.bids.append(json.dumps(bid))
                 for ask in _event.asks:
@@ -626,74 +624,49 @@
                     balance = await client.fetch_ledgers(request.symbol)
                 except Exception as _ex:
                     logger.warning(f"OnBalanceUpdate: for {open_client.name}:{request.symbol}: {_ex}")
                 else:
                     if balance:
                         _event = client.events.wrap_event(balance)
             if isinstance(_event, events.BalanceUpdateWrapper):
-                logger.debug(f"OnBalanceUpdate: {_event.event_time}:{_event.asset}:{_event.balance_delta}")
+                logger.debug(f"OnBalanceUpdate: {open_client.name}:{_event.event_time}:"
+                             f"{_event.asset}:{_event.balance_delta}")
                 if _event.asset in request.symbol:
                     balance = {
                         "event_time": _event.event_time,
                         "asset": _event.asset,
                         "balance_delta": _event.balance_delta,
                         "clear_time": _event.clear_time
                     }
                     response.balance = json.dumps(balance)
                     yield response
 
     async def OnOrderUpdate(self, request: api_pb2.MarketRequest,
-                            _context: grpc.aio.ServicerContext) -> api_pb2.OnOrderUpdateResponse:
-        response = api_pb2.OnOrderUpdateResponse()
+                            _context: grpc.aio.ServicerContext) -> api_pb2.SimpleResponse:
+        response = api_pb2.SimpleResponse()
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         _queue = asyncio.Queue(MAX_QUEUE_SIZE)
-        open_client.on_order_update_queues.update({request.trade_id: _queue})
+        client.on_order_update_queues.update({request.trade_id: _queue})
         client.stream_queue[request.trade_id] |= {_queue}
         client.events.register_user_event(functools.partial(
             event_handler, _queue, client, request.trade_id, 'executionReport'),
             'executionReport')
         while True:
             _event = await _queue.get()
             if isinstance(_event, str) and _event == request.trade_id:
                 client.stream_queue.get(request.trade_id, set()).discard(_queue)
                 logger.info(f"OnOrderUpdate: Stop user stream for {open_client.name}: {request.symbol}")
                 return
             else:
-                # logger.info(f"OnOrderUpdate:{_event.symbol}:{int(_event.order_id)}:{_event.order_status}")
-                response.symbol = _event.symbol
-                response.client_order_id = _event.client_order_id
-                response.side = _event.side
-                response.order_type = _event.order_type
-                response.time_in_force = _event.time_in_force
-                response.order_quantity = _event.order_quantity
-                response.order_price = _event.order_price
-                response.stop_price = _event.stop_price
-                response.iceberg_quantity = _event.iceberg_quantity
-                response.order_list_id = int(_event.order_list_id)
-                response.original_client_id = _event.original_client_id
-                response.execution_type = _event.execution_type
-                response.order_status = _event.order_status
-                response.order_reject_reason = _event.order_reject_reason
-                response.order_id = int(_event.order_id)
-                response.last_executed_quantity = _event.last_executed_quantity
-                response.cumulative_filled_quantity = _event.cumulative_filled_quantity
-                response.last_executed_price = _event.last_executed_price
-                response.commission_amount = _event.commission_amount
-                response.commission_asset = _event.commission_asset or str()
-                response.transaction_time = int(_event.transaction_time)
-                response.trade_id = int(_event.trade_id)
-                response.ignore_a = _event.ignore_a
-                response.in_order_book = _event.in_order_book
-                response.is_maker_side = bool(_event.is_maker_side)
-                response.ignore_b = _event.ignore_b
-                response.order_creation_time = int(_event.order_creation_time)
-                response.quote_asset_transacted = _event.quote_asset_transacted
-                response.last_quote_asset_transacted = _event.last_quote_asset_transacted
-                response.quote_order_quantity = _event.quote_order_quantity
+                event = vars(_event)
+                # logger.info(f"OnOrderUpdate: {event}")
+                event.pop('handlers', None)
+                response.success = True
+                response.result = json.dumps(str(event))
                 yield response
 
     async def CreateLimitOrder(self, request: api_pb2.CreateLimitOrderRequest,
                                _context: grpc.aio.ServicerContext) -> api_pb2.CreateLimitOrderResponse:
         response = api_pb2.CreateLimitOrderResponse()
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
@@ -757,64 +730,93 @@
             logger.error(f"CancelOrder for {open_client.name}:{request.symbol} exception: {ex}")
             _context.set_details(f"{ex}")
             _context.set_code(grpc.StatusCode.UNKNOWN)
         else:
             json_format.ParseDict(res, response)
         return response
 
+    async def TransferToMaster(self, request: api_pb2.MarketRequest,
+                               _context: grpc.aio.ServicerContext) -> api_pb2.SimpleResponse:
+        response = api_pb2.SimpleResponse()
+        response.success = False
+        open_client = OpenClient.get_client(request.client_id)
+        client = open_client.client
+        try:
+            res = await client.transfer_to_master(symbol=request.symbol, quantity=request.amount)
+        except errors.HTTPError as ex:
+            logger.error(f"TransferToMaster for {open_client.name}: {request.symbol} exception: {ex}")
+            _context.set_details(f"{ex}")
+            _context.set_code(grpc.StatusCode.RESOURCE_EXHAUSTED)
+        except Exception as ex:
+            logger.error(f"TransferToMaster for {open_client.name}: {request.symbol} exception: {ex}")
+            logger.debug(f"TransferToMaster for {open_client.name}: {request.symbol} error: {traceback.format_exc()}")
+            _context.set_details(f"{ex}")
+            _context.set_code(grpc.StatusCode.UNKNOWN)
+        else:
+            if res and res.get("txnId"):
+                response.success = True
+            response.result = json.dumps(res)
+        return response
+
     async def StartStream(self, request: api_pb2.StartStreamRequest,
                           _context: grpc.aio.ServicerContext) -> api_pb2.SimpleResponse:
+        if request.update_max_queue_size:
+            global MAX_QUEUE_SIZE
+            MAX_QUEUE_SIZE += int(MAX_QUEUE_SIZE / 10)
+            logger.info(f"MAX_QUEUE_SIZE was updated: new value is {MAX_QUEUE_SIZE}")
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         response = api_pb2.SimpleResponse()
         _market_stream_count = 0
         while _market_stream_count < request.market_stream_count:
             await asyncio.sleep(HEARTBEAT)
             _market_stream_count = sum(len(k) for k in ([list(i.get(request.trade_id, []))
                                                          for i in list(client.events.registered_streams.values())]))
         logger.info(f"Start WS streams for {open_client.name}")
-        asyncio.create_task(open_client.client.start_market_events_listener(request.trade_id))
-        asyncio.create_task(open_client.client.start_user_events_listener(request.trade_id, request.symbol))
+        asyncio.create_task(client.start_market_events_listener(request.trade_id))
+        asyncio.create_task(client.start_user_events_listener(request.trade_id, request.symbol))
         response.success = True
         return response
 
     async def StopStream(self, request: api_pb2.MarketRequest,
                          _context: grpc.aio.ServicerContext) -> api_pb2.SimpleResponse:
         open_client = OpenClient.get_client(request.client_id)
         client = open_client.client
         logger.info(f"StopStream request for {request.symbol} on {client.exchange}")
         response = api_pb2.SimpleResponse()
         await stop_stream(client, request.trade_id)
-        [await _queue.put(request.trade_id) for _queue in client.stream_queue.get(request.trade_id, [])]
-        not_empty = True
-        while not_empty:
-            await asyncio.sleep(HEARTBEAT)
-            not_empty = False
-            for q in client.stream_queue.get(request.trade_id, []):
-                if isinstance(q, asyncio.Queue) and not q.empty():
-                    not_empty = True
-                    break
-        open_client.on_order_update_queues.pop(request.trade_id, None)
-        client.stream_queue.pop(request.trade_id, None)
         response.success = True
         return response
 
+    async def CheckStream(self, request: api_pb2.MarketRequest,
+                          _context: grpc.aio.ServicerContext) -> api_pb2.SimpleResponse:
+        open_client = OpenClient.get_client(request.client_id)
+        client = open_client.client
+        response = api_pb2.SimpleResponse()
+        response.success = bool(client.data_streams.get(request.trade_id))
+        logger.debug(f"CheckStream request for {request.symbol} on {client.exchange} passed: {response.success}")
+        return response
+
 
 async def stop_stream(client, trade_id):
     await client.stop_events_listener(trade_id)
     client.events.unregister(client.exchange, trade_id)
+    [await _queue.put(trade_id) for _queue in client.stream_queue.get(trade_id, [])]
+    client.on_order_update_queues.pop(trade_id, None)
+    client.stream_queue.pop(trade_id, None)
     gc.collect(generation=2)
 
 
 async def event_handler(_queue, client, trade_id, _event_type, event):
     _event = weakref.ref(event)
     try:
         _queue.put_nowait(_event())
     except asyncio.QueueFull:
         logger.warning(f"For {_event_type} asyncio queue full and wold be closed")
+        client.stream_queue.get(trade_id, set()).discard(_queue)
         await stop_stream(client, trade_id)
 
 
 def is_port_in_use(port: int) -> bool:
     import socket
     # with socket.socket(socket.AF_INET6, socket.SOCK_STREAM) as s:
     with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/exch_srv_cfg.toml.template` & `exchanges-wrapper-1.3.0/exchanges_wrapper/exch_srv_cfg.toml.template`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Parameters for exchanges-wrapper REST API Server exch_srv.py
 # Copyright © 2021 Jerry Fedorenko aka VM
-# __version__ = "1.2.9"
+# __version__ = "1.2.10"
 
+# region endpoint
 [endpoint]
     [endpoint.binance]
         api_public = 'https://api.binance.com'
         api_auth = 'https://api.binance.com'
         ws_public = 'wss://stream.binance.com:9443'
         ws_auth = 'wss://stream.binance.com:9443'
         api_test = 'https://testnet.binance.vision'
@@ -43,19 +44,17 @@
     [endpoint.okx]
         api_public = 'https://aws.okx.com'
         api_auth = 'https://aws.okx.com'
         ws_public = 'wss://wsaws.okx.com:8443/ws/v5/public'
         ws_auth = 'wss://wsaws.okx.com:8443/ws/v5/private'
         api_test = 'https://aws.okx.com'
         ws_test = 'wss://wspap.okx.com:8443/ws/v5/private?brokerId=9999'
+# endregion
 
-# Don't change accounts.exchange field value
-# You can add subaccounts by duplicate records and set name, API and test_net fields
-#
-# Binance.com accounts
+# region Binance.com accounts
 [[accounts]]
     exchange = 'binance'
     name = 'Demo - Binance'
     api_key = '*********** Place API key there ************'
     api_secret = '*********** Place secret API key there ************'
     test_net = true
 
@@ -69,39 +68,57 @@
 # Binance.us accounts
 [[accounts]]
     exchange = 'binance_us'
     name = 'Binance US'
     api_key = '*********** Place API key there ************'
     api_secret = '*********** Place secret API key there ************'
     test_net = false
+# endregion
 
-# Bitfinex accounts
+# region Bitfinex accounts
+# Set up a sub-account two-fa (2FA) key and master_email (Main account EMail)
+# for transfer funds from sub-account to master account
 [[accounts]]
     exchange = 'bitfinex'
     name = 'Demo - Bitfinex'
+    two_fa = '*********** Place 2FA key there ************'
     api_key = '*********** Place API key there ************'
     api_secret = '*********** Place secret API key there ************'
+    master_email = '*********** Place Main account EMail ************'
     test_net = true
 
 [[accounts]]
     exchange = 'bitfinex'
     name = 'Bitfinex'
+    two_fa = ''
     api_key = '*********** Place API key there ************'
     api_secret = '*********** Place secret API key there ************'
+    master_email = ''
     test_net = false
+# endregion
 
-# Huobi accounts
+# region Huobi acconts
 [[accounts]]
     exchange = 'huobi'
     name = 'Huobi'
     api_key = '*********** Place API key there ************'
     api_secret = '*********** Place secret API key there ************'
     test_net = false
 
-# OKX
+[[accounts]]
+    exchange = 'huobi'
+    name = 'HuobiSub1'
+    api_key = '*********** Place API key there ************'
+    api_secret = '*********** Place secret API key there ************'
+    test_net = false
+    master_name = 'Huobi'
+# endregion
+
+# region OKX
 [[accounts]]
     exchange = 'okx'
     name = 'Demo - OKX'
     api_key = '*********** Place API key there ************'
     api_secret = '*********** Place secret API key there ************'
     passphrase = '*********** Place API password there ************'
-    test_net = true
+    test_net = true
+# endregion
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/http_client.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/http_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 from urllib.parse import urlencode, urlparse
-from exchanges_wrapper import __version__
+
+import aiohttp
 import logging
 import time
 from datetime import datetime
 from exchanges_wrapper.c_structures import generate_signature
 from exchanges_wrapper.errors import (
     RateLimitReached,
     ExchangeError,
@@ -21,53 +22,54 @@
 
 class HttpClient:
     def __init__(self, **kwargs):
         self.api_key = kwargs.get('api_key')
         self.api_secret = kwargs.get('api_secret')
         self.passphrase = kwargs.get('passphrase')
         self.endpoint = kwargs.get('endpoint')
-        self.user_agent = kwargs.get('user_agent') or f"exchanges-wrapper, {__version__}"
-        self.proxy = kwargs.get('proxy')
         self.session = kwargs.get('session')
         self.exchange = kwargs.get('exchange')
         self.sub_account = kwargs.get('sub_account')
         self.test_net = kwargs.get('test_net')
         self.rate_limit_reached = False
 
     async def handle_errors(self, response):
         if response.status >= 500:
             raise ExchangeError(f"An issue occurred on exchange's side: {response.status}: {response.url}:"
                                 f" {response.reason}")
         if response.status == 429:
             logger.error(f"handle_errors RateLimitReached:response.url: {response.url}")
             self.rate_limit_reached = self.exchange in ('binance', 'okx')
             raise RateLimitReached(RateLimitReached.message)
-        payload = await response.json()
+        try:
+            payload = await response.json()
+        except aiohttp.ContentTypeError:
+            payload = None
         if self.exchange == 'binance' and payload and "code" in payload:
             # as defined here: https://github.com/binance/binance-spot-api-docs/blob/
             # master/errors.md#error-codes-for-binance-2019-09-25
             raise ExchangeError(payload["msg"])
         if response.status >= 400:
-            logger.debug(f"handle_errors.response.status >= 400: {payload}")
+            logger.debug(f"handle_errors.response: {response.text}")
             if response.status == 400 and payload and payload.get("error", str()) == "ERR_RATE_LIMIT":
                 raise RateLimitReached(RateLimitReached.message)
             elif response.status == 403 and self.exchange != 'okx':
                 raise WAFLimitViolated(WAFLimitViolated.message)
             elif response.status == 418:
                 raise IPAddressBanned(IPAddressBanned.message)
             else:
-                raise HTTPError(f"Malformed request: {payload}")
+                raise HTTPError(f"Malformed request: status: {response.status}, reason: {response.reason}")
         if self.exchange in ('binance', 'bitfinex'):
             return payload
         elif self.exchange == 'huobi' and payload and (payload.get('status') == 'ok' or payload.get('ok')):
             return payload.get('data', payload.get('tick'))
         elif self.exchange == 'okx' and payload and payload.get('code') == '0':
             return payload.get('data', [])
         else:
-            raise HTTPError(f"API request failed: {payload}")
+            raise HTTPError(f"API request failed: {response.status}:{response.reason}:{payload}")
 
     async def send_api_call(self,
                             path,
                             method="GET",
                             signed=False,
                             send_api_key=True,
                             endpoint=None,
@@ -86,29 +88,26 @@
                             endpoint=None,
                             timeout=None,
                             **kwargs):
         if self.rate_limit_reached:
             raise QueryCanceled(QueryCanceled.message)
         _endpoint = endpoint or self.endpoint
         url = f'{_endpoint}{path}'
-        query_kwargs = dict({"headers": {"User-Agent": self.user_agent}}, **kwargs)
+        query_kwargs = dict({"headers": {"Content-Type": AJ}}, **kwargs)
         if send_api_key:
             query_kwargs["headers"]["X-MBX-APIKEY"] = self.api_key
         if signed:
             content = str()
-            query_kwargs["headers"]["Content-Type"] = AJ
             location = "params" if "params" in kwargs else "data"
             query_kwargs[location]["timestamp"] = str(int(time.time() * 1000))
             if "params" in kwargs:
                 content += urlencode(kwargs["params"])
             if "data" in kwargs:
                 content += urlencode(kwargs["data"])
             query_kwargs[location]["signature"] = generate_signature(self.exchange, self.api_secret, content)
-            if self.proxy:
-                query_kwargs["proxy"] = self.proxy
         # print(f"send_api_call.request: url: {url}, query_kwargs: {query_kwargs}")
         async with self.session.request(method, url, timeout=timeout, **query_kwargs) as response:
             # print(f"send_api_call.response: url: {response.url}, status: {response.status}")
             return await self.handle_errors(response)
 
 
 class ClientBFX(HttpClient):
@@ -120,22 +119,20 @@
                             send_api_key=True,
                             endpoint=None,
                             timeout=None,
                             **kwargs):
         if self.rate_limit_reached:
             raise QueryCanceled(QueryCanceled.message)
         _endpoint = endpoint or self.endpoint
-        content = str()
         bfx_post = self.exchange == 'bitfinex' and ((method == 'POST' and kwargs) or "params" in kwargs)
         _params = json.dumps(kwargs) if bfx_post else None
         url = f'{_endpoint}/{path}'
         query_kwargs = {"headers": {"Accept": AJ}}
-        content += urlencode(kwargs, safe='/')
-        if content and not bfx_post:
-            url += f'?{content}'
+        if kwargs and not bfx_post:
+            url += f"?{urlencode(kwargs, safe='/')}"
         if bfx_post and "params" in kwargs:
             query_kwargs.update({'data': _params})
         if signed:
             ts = int(time.time() * 1000)
             query_kwargs["headers"]["Content-Type"] = AJ
             if bfx_post:
                 query_kwargs.update({'data': _params})
@@ -144,15 +141,14 @@
             signature_payload = f'/api/{path}{ts}'
             if _params:
                 signature_payload += f"{_params}"
             query_kwargs["headers"]["bfx-signature"] = generate_signature(self.exchange,
                                                                           self.api_secret,
                                                                           signature_payload)
             query_kwargs["headers"]["bfx-nonce"] = str(ts)
-
         # print(f"send_api_call.request: url: {url}, query_kwargs: {query_kwargs}")
         async with self.session.request(method, url, timeout=timeout, **query_kwargs) as response:
             # print(f"send_api_call.response: url: {response.url}, status: {response.status}")
             return await self.handle_errors(response)
 
 
 class ClientHBP(HttpClient):
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/huobi_parser.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/huobi_parser.py`

 * *Files identical despite different names*

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/okx_parser.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/okx_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -251,14 +251,21 @@
         "firstId": 0,
         "lastId": 1,
         "count": 1,
     }
     return binance_price_ticker
 
 
+def fetch_symbol_price_ticker(res: {}, symbol) -> {}:
+    return {
+        "symbol": symbol,
+        "price": res.get('last')
+    }
+
+
 def ticker(res: {}) -> {}:
     symbol = res.get('instId').replace('-', '')
     msg_binance = {
         'stream': f"{symbol.lower()}@miniTicker",
         'data': {
             "e": "24hrMiniTicker",
             "E": int(int(res.get('ts')) / 1000),
@@ -504,102 +511,7 @@
             "time": trade.get('ts'),
             "isBuyer": bool('buy' == trade.get('side')),
             "isMaker": bool('M' == trade.get('execType')),
             "isBestMatch": True,
         }
         binance_trade_list.append(binance_trade)
     return binance_trade_list
-
-###############################################################################
-
-
-def fetch_symbol_price_ticker(res: {}, symbol) -> {}:
-    return {
-        "symbol": symbol,
-        "price": str(res.get('data')[0].get('price'))
-    }
-
-
-def get_symbols(symbols_details: []) -> str:
-    symbols = []
-    res = ",t"
-    for symbol_details in symbols_details:
-        symbol = symbol_details['pair']
-        if 'f0' not in symbol:
-            symbols.append(symbol.upper())
-    return f"t{res.join(symbols)}"
-
-
-def tick_size(precision, _price):
-    x = int(_price)
-    _price = str(_price)
-    if '.' not in _price:
-        _price += ".0"
-    k = len(_price.split('.')[1])
-    x = len(_price.split('.')[0]) if k and x else 0
-    if k + x - precision > 0:
-        k = precision - x
-    elif k + x - precision < 0:
-        k += precision - x - k
-    res = (1 / 10 ** k) if k else 1
-    return res
-
-
-def symbol_name(_pair: str) -> ():
-    if ':' in _pair:
-        pair = _pair.replace(':', '').upper()
-        base_asset = _pair.split(':')[0].upper()
-        quote_asset = _pair.split(':')[1].upper()
-    else:
-        pair = _pair.upper()
-        base_asset = _pair[0:3].upper()
-        quote_asset = _pair[3:].upper()
-    return pair, base_asset, quote_asset
-
-
-def on_order_trade(res: [], executed_qty: str) -> {}:
-    # print(f"on_order_trade.res: {res}")
-    side = 'BUY' if res[4] > 0 else 'SELL'
-    #
-    status = 'PARTIALLY_FILLED'
-    #
-    last_executed_quantity = str(abs(res[4]))
-    last_executed_price = str(res[5])
-    last_quote_asset = str(Decimal(last_executed_quantity) * Decimal(last_executed_price))
-    msg_binance = {
-        "e": "executionReport",
-        "E": res[2],
-        "s": res[1][1:].replace(':', ''),
-        "c": str(res[11]),
-        "S": side,
-        "o": "LIMIT",
-        "f": "GTC",
-        "q": "0.0",
-        "p": str(res[7]),
-        "P": "0.00000000",
-        "F": "0.00000000",
-        "g": -1,
-        "C": "NEW",
-        "x": "TRADE",
-        "X": status,
-        "r": "NONE",
-        "i": res[3],
-        "l": last_executed_quantity,
-        "z": executed_qty,
-        "L": last_executed_price,
-        "n": str(res[9]),
-        "N": res[10],
-        "T": res[2],
-        "t": res[0],
-        "I": 123456789,
-        "w": True,
-        "m": bool(res[8] == 1),
-        "M": False,
-        "O": res[2],
-        "Z": "0.0",
-        "Y": last_quote_asset,
-        "Q": "0.0"
-    }
-    return msg_binance
-
-
-
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/proto/exchanges_wrapper/api.proto` & `exchanges-wrapper-1.3.0/exchanges_wrapper/proto/exchanges_wrapper/api.proto`

 * *Files 8% similar despite different names*

```diff
@@ -9,35 +9,37 @@
 
 package martin;
 
 service Martin {
   rpc OpenClientConnection (OpenClientConnectionRequest) returns (OpenClientConnectionId) {}
   rpc FetchServerTime (OpenClientConnectionId) returns (FetchServerTimeResponse) {}
   rpc FetchOpenOrders (MarketRequest) returns (FetchOpenOrdersResponse) {}
-  rpc CancelAllOrders (MarketRequest) returns (FetchOpenOrdersResponse) {}
+  rpc CancelAllOrders (MarketRequest) returns (SimpleResponse) {}
   rpc FetchExchangeInfoSymbol (MarketRequest) returns (FetchExchangeInfoSymbolResponse) {}
   rpc FetchAccountInformation (OpenClientConnectionId) returns (FetchAccountBalanceResponse) {}
   rpc FetchOrderBook (MarketRequest) returns (FetchOrderBookResponse) {}
   rpc FetchSymbolPriceTicker (MarketRequest) returns (FetchSymbolPriceTickerResponse) {}
   rpc FetchTickerPriceChangeStatistics (MarketRequest) returns (FetchTickerPriceChangeStatisticsResponse) {}
   rpc FetchKlines (FetchKlinesRequest) returns (FetchKlinesResponse) {}
   rpc FetchAccountTradeList (AccountTradeListRequest) returns (AccountTradeListResponse) {}
   rpc OnTickerUpdate (MarketRequest) returns (stream OnTickerUpdateResponse) {}
   rpc OnOrderBookUpdate (MarketRequest) returns (stream FetchOrderBookResponse) {}
   rpc StopStream (MarketRequest) returns (SimpleResponse) {}
   rpc StartStream (StartStreamRequest) returns (SimpleResponse) {}
   rpc OnFundsUpdate (OnFundsUpdateRequest) returns (stream OnFundsUpdateResponse) {}
   rpc OnBalanceUpdate (MarketRequest) returns (stream OnBalanceUpdateResponse) {}
-  rpc OnOrderUpdate (MarketRequest) returns (stream OnOrderUpdateResponse) {}
+  rpc OnOrderUpdate (MarketRequest) returns (stream SimpleResponse) {}
   rpc CreateLimitOrder (CreateLimitOrderRequest) returns (CreateLimitOrderResponse) {}
   rpc CancelOrder (CancelOrderRequest) returns (CancelOrderResponse) {}
   rpc FetchOrder (FetchOrderRequest) returns (FetchOrderResponse) {}
   rpc ResetRateLimit (OpenClientConnectionId) returns (SimpleResponse) {}
   rpc OnKlinesUpdate(FetchKlinesRequest) returns (stream OnKlinesUpdateResponse) {}
   rpc FetchFundingWallet(FetchFundingWalletRequest) returns (FetchFundingWalletResponse) {}
+  rpc TransferToMaster(MarketRequest) returns (SimpleResponse) {}
+  rpc CheckStream (MarketRequest) returns (SimpleResponse) {}
 }
 
 message OnBalanceUpdateResponse {
   string balance = 1;
 }
 
 message FetchFundingWalletRequest{
@@ -159,14 +161,15 @@
   string symbol = 3;
   string base_asset = 4;
   string quote_asset = 5;
 }
 
 message SimpleResponse {
   bool success = 1;
+  string result = 2;
 }
 
 message OnTickerUpdateResponse {
   string symbol = 1;
   string open_price = 2;
   string close_price = 3;
   uint64 event_time = 4;
@@ -328,14 +331,24 @@
     optional MaxNumIcebergOrders max_num_iceberg_orders = 9;
 
     message MaxPosition {
       string filterType = 1;
       string maxPosition = 2;
     }
     optional MaxPosition max_position = 10;
+
+    message Notional {
+      string filterType = 1;
+      string minNotional = 2;
+      bool applyMinToMarket = 3;
+      string maxNotional = 4;
+      bool applyMaxToMarket = 5;
+      uint32 avgPriceMins = 6;
+    }
+    optional Notional notional = 11;
 }
 
   string symbol = 1;
   string status = 2;
   string baseAsset = 3;
   uint32 baseAssetPrecision = 4;
   string quoteAsset = 5;
@@ -353,35 +366,14 @@
   bool isMarginTradingAllowed = 17;
   Filters filters = 18;
   repeated string permissions = 19;
   string defaultSelfTradePreventionMode = 20;
   repeated string allowedSelfTradePreventionModes = 21;
 }
 
-message CancelAllOrdersResponse {
-  message CancelOrder {
-    string symbol = 1;
-    string origClientOrderId = 2;
-    uint64 orderId = 3;
-    int32 orderListId = 4;
-    string clientOrderId = 5;
-    uint64 transactTime = 6;
-    string price = 7;
-    string origQty = 8;
-    string executedQty = 9;
-    string cummulativeQuoteQty = 10;
-    string status = 11;
-    string timeInForce = 12;
-    string type = 13;
-    string side = 14;
-    string selfTradePreventionMode = 15;
-  }
-  repeated CancelOrder items = 1;
-}
-
 message FetchOrderRequest{
   int64 client_id = 1;
   string trade_id = 2;
   string symbol = 3;
   int64 order_id = 4;
   bool filled_update_call = 5;
 }
@@ -436,22 +428,24 @@
   repeated Order items = 2;
 }
 
 message MarketRequest {
   int64 client_id = 1;
   string trade_id = 2;
   string symbol = 3;
+  string amount = 4;
 }
 
 message StartStreamRequest {
   int64 client_id = 1;
   string trade_id = 2;
   string symbol = 3;
   int32 market_stream_count = 4;
   int32 user_stream_count = 5;
+  bool update_max_queue_size = 6;
 }
 
 message OpenClientConnectionRequest {
   string trade_id = 1;
   string account_name = 2;
   int32 rate_limiter = 3;
 }
```

### Comparing `exchanges-wrapper-1.2.9.post2/exchanges_wrapper/web_sockets.py` & `exchanges-wrapper-1.3.0/exchanges_wrapper/web_sockets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,7 @@
-# __version__ = "1.2.6b4"
-
-from exchanges_wrapper import __version__
-
 import aiohttp
 import asyncio
 import json
 import random
 import logging
 import time
 from decimal import Decimal
@@ -19,26 +15,23 @@
 import exchanges_wrapper.okx_parser as okx
 from exchanges_wrapper.c_structures import generate_signature
 
 logger = logging.getLogger('exch_srv_logger')
 
 
 class EventsDataStream:
-    def __init__(self, client, endpoint, user_agent, exchange, trade_id):
+    def __init__(self, client, endpoint, exchange, trade_id):
         self.client = client
         self.session = client.session
         self.endpoint = endpoint
-        if user_agent:
-            self.user_agent = user_agent
-        else:
-            self.user_agent = f"exchanges-wrapper, {__version__}"
         self.exchange = exchange
         self.trade_id = trade_id
         self.web_socket = None
         self.try_count = 0
+        self.wss_event_buffer = {}
 
     async def start(self):
         try:
             await self.start_wss()
         except (aiohttp.WSServerHandshakeError, aiohttp.ClientConnectionError, asyncio.TimeoutError) as ex:
             self.try_count += 1
             delay = random.randint(2, 10) * self.try_count
@@ -49,15 +42,19 @@
             logger.error(f"WSS start() other exception: {ex}")
             logger.debug(traceback.format_exc())
 
     async def start_wss(self):
         pass  # meant to be overridden in a subclass
 
     async def stop(self):
-        pass  # meant to be overridden in a subclass
+        """
+        Stop data stream
+        """
+        if self.web_socket:
+            await self.web_socket.close()
 
     async def upstream_bitfinex(self, request, symbol=None, ch_type=str()):
         await self.web_socket.send_json(request)
         msg = await self.web_socket.receive_json()
         if msg.get('event') == 'info':
             if msg.get('version') != 2:
                 logger.warning('Change WSS version detected')
@@ -168,81 +165,66 @@
                     raise aiohttp.ClientOSError(f"Reconnecting Huobi user {ch_type} channel")
                 else:
                     logger.debug(f"Huobi undefined WSS: symbol: {symbol}, ch_type: {ch_type}, msg_data: {msg_data}")
 
 
 class MarketEventsDataStream(EventsDataStream):
 
-    def __init__(self, client, endpoint, user_agent, exchange, trade_id, channel=None):
-        super().__init__(client, endpoint, user_agent, exchange, trade_id)
+    def __init__(self, client, endpoint, exchange, trade_id, channel=None):
+        super().__init__(client, endpoint, exchange, trade_id)
         self.channel = channel
         self.candles_max_time = None
 
-    async def stop(self):
-        """
-        Stop market data stream
-        """
-        logger.info(f"Market WSS stop for {self.exchange}:{self.trade_id}:{self.channel}")
-        if self.web_socket:
-            await self.web_socket.close()
-
     async def start_wss(self):
         logger.info(f"Start market WSS {self.channel if self.channel else ''} for {self.exchange}")
         registered_streams = self.client.events.registered_streams.get(self.exchange, {}).get(self.trade_id, set())
         if self.exchange == 'binance':
             combined_streams = "/".join(registered_streams)
-            self.web_socket = await self.session.ws_connect(f"{self.endpoint}/stream?streams={combined_streams}",
-                                                            proxy=self.client.proxy)
+            self.web_socket = await self.session.ws_connect(f"{self.endpoint}/stream?streams={combined_streams}")
             logger.info(f"Combined events stream started: {combined_streams}")
             await self._handle_messages(self.web_socket)
         else:
             symbol = self.channel.split('@')[0]
             ch_type = self.channel.split('@')[1]
             request = {}
             if self.exchange == 'okx':
-                self.web_socket = await self.session.ws_connect(self.endpoint,
-                                                                heartbeat=25,
-                                                                proxy=self.client.proxy)
+                self.web_socket = await self.session.ws_connect(self.endpoint, heartbeat=25)
                 if ch_type == 'miniTicker':
                     _ch_type = 'tickers'
                 elif 'kline_' in ch_type:
                     _ch_type = (f"{ch_type.split('_')[0].replace('kline', 'candle')}"
                                 f"{okx.interval(ch_type.split('_')[1])}")
                 elif ch_type == 'depth5':
                     _ch_type = 'books5'
                 else:
                     _ch_type = None
 
                 request = {"op": 'subscribe',
                            "args": [{"channel": _ch_type,
+                                     "instType": 'SPOT',
                                      "instId": symbol}
                                     ]
                            }
                 await self.web_socket.send_json(request)
                 await self._handle_messages(self.web_socket, symbol=symbol, ch_type=ch_type)
             elif self.exchange == 'bitfinex':
-                self.web_socket = await self.session.ws_connect(self.endpoint,
-                                                                receive_timeout=30,
-                                                                proxy=self.client.proxy)
+                self.web_socket = await self.session.ws_connect(self.endpoint, receive_timeout=30)
                 if ch_type == 'miniTicker':
                     ch_type = 'ticker'
                     request = {'event': 'subscribe', 'channel': ch_type, 'pair': symbol}
                 elif 'kline_' in ch_type:
                     ch_type = ch_type.replace('kline_', 'candles_')
                     tf = ch_type.split('_')[1]
                     request = {'event': 'subscribe', 'channel': 'candles', 'key': f"trade:{tf}:{symbol}"}
                 elif ch_type == 'depth5':
                     ch_type = 'book'
                     request = {'event': 'subscribe', 'channel': ch_type, 'symbol': symbol, 'prec': 'P0', }
                 await self.upstream_bitfinex(request, symbol, ch_type)
             elif self.exchange == 'huobi':
-                self.web_socket = await self.session.ws_connect(self.endpoint,
-                                                                receive_timeout=20,
-                                                                proxy=self.client.proxy,
-                                                                autoping=False)
+                self.web_socket = await self.session.ws_connect(self.endpoint, receive_timeout=20, autoping=False)
                 if ch_type == 'miniTicker':
                     ch_type = 'ticker'
                     request = {'sub': f"market.{symbol}.{ch_type}"}
                 elif 'kline_' in ch_type:
                     tf = ch_type.split('_')[1]
                     request = {'sub': f"market.{symbol}.kline.{hbp.interval(tf)}"}
                 elif ch_type == 'depth5':
@@ -295,30 +277,20 @@
         elif isinstance(content, list):
             for event_content in content:
                 event_content["stream"] = stream_name
                 await self.client.events.wrap_event(event_content).fire(self.trade_id)
 
 
 class HbpPrivateEventsDataStream(EventsDataStream):
-    def __init__(self, client, endpoint, user_agent, exchange, trade_id, symbol):
-        super().__init__(client, endpoint, user_agent, exchange, trade_id)
+    def __init__(self, client, endpoint, exchange, trade_id, symbol):
+        super().__init__(client, endpoint, exchange, trade_id)
         self.symbol = symbol
 
-    async def stop(self):
-        """
-        Stop data stream
-        """
-        if self.web_socket:
-            await self.web_socket.close()
-
     async def start_wss(self):
-        self.web_socket = await self.session.ws_connect(self.endpoint,
-                                                        receive_timeout=30,
-                                                        proxy=self.client.proxy,
-                                                        autoping=False)
+        self.web_socket = await self.session.ws_connect(self.endpoint, receive_timeout=30, autoping=False)
         ts = datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S")
         _params = {
                 "accessKey": self.client.api_key,
                 "signatureMethod": "HmacSHA256",
                 "signatureVersion": "2.1",
                 "timestamp": str(ts)
         }
@@ -358,25 +330,16 @@
         if content:
             logger.debug(f"HbpPrivateEventsDataStream._handle_event.content: {content}")
             await self.client.events.wrap_event(content).fire(self.trade_id)
 
 
 class BfxPrivateEventsDataStream(EventsDataStream):
 
-    async def stop(self):
-        """
-        Stop data stream
-        """
-        if self.web_socket:
-            await self.web_socket.close()
-
     async def start_wss(self):
-        self.web_socket = await self.session.ws_connect(self.endpoint,
-                                                        receive_timeout=30,
-                                                        proxy=self.client.proxy)
+        self.web_socket = await self.session.ws_connect(self.endpoint, receive_timeout=30)
         ts = int(time.time() * 1000)
         data = f"AUTH{ts}"
         request = {
             'event': "auth",
             'apiKey': self.client.api_key,
             'authSig': generate_signature(self.exchange, self.client.api_secret, data),
             'authPayload': data,
@@ -414,29 +377,20 @@
                     executed_qty = self.client.active_orders.get(order_id, {}).get('executedQty', '0')
                     content = bfx.on_order_trade(msg_data[2], executed_qty)
         if content:
             await self.client.events.wrap_event(content).fire(self.trade_id)
 
 
 class OkxPrivateEventsDataStream(EventsDataStream):
-    def __init__(self, client, endpoint, user_agent, exchange, trade_id, symbol):
-        super().__init__(client, endpoint, user_agent, exchange, trade_id)
+    def __init__(self, client, endpoint, exchange, trade_id, symbol):
+        super().__init__(client, endpoint, exchange, trade_id)
         self.symbol = symbol
 
-    async def stop(self):
-        """
-        Stop data stream
-        """
-        if self.web_socket:
-            await self.web_socket.close()
-
     async def start_wss(self):
-        self.web_socket = await self.session.ws_connect(self.endpoint,
-                                                        heartbeat=25,
-                                                        proxy=self.client.proxy)
+        self.web_socket = await self.session.ws_connect(self.endpoint, heartbeat=25)
         ts = int(time.time())
         signature_payload = f"{ts}GET/users/self/verify"
         signature = generate_signature(self.exchange, self.client.api_secret, signature_payload)
         # Login on account
         request = {"op": 'login',
                    "args": [{"apiKey": self.client.api_key,
                              "passphrase": self.client.passphrase,
@@ -463,17 +417,17 @@
         content = None
         if msg_data.get('arg', {}).get('channel') == 'account':
             content = okx.on_funds_update(msg_data.get('data')[0])
         elif msg_data.get('arg', {}).get('channel') == 'orders':
             content = okx.on_order_update(msg_data.get('data')[0])
         elif msg_data.get('arg', {}).get('channel') == 'balance_and_position':
             _data = msg_data.get('data')[0]
-            content, self.client.wss_buffer = okx.on_balance_update(_data.get('balData', []),
-                                                                    self.client.wss_buffer,
-                                                                    bool(_data.get('eventType') == 'transferred'))
+            content, self.wss_event_buffer = okx.on_balance_update(_data.get('balData', []),
+                                                                   self.wss_event_buffer,
+                                                                   bool(_data.get('eventType') == 'transferred'))
             for i in content:
                 await self.client.events.wrap_event(i).fire(self.trade_id)
             content = None
         if content:
             await self.client.events.wrap_event(content).fire(self.trade_id)
 
 
@@ -482,27 +436,17 @@
     async def _heartbeat(self, listen_key, interval=60 * 30):
         # 30 minutes is recommended according to
         # https://github.com/binance-exchange/binance-official-api-docs/blob/master/user-data-stream.md#pingkeep-alive-a-listenkey
         while True:
             await asyncio.sleep(interval)
             await self.client.keep_alive_listen_key(listen_key)
 
-    async def stop(self):
-        """
-        Stop user data stream
-        """
-        # logger.info(f"UserEventsDataStream.stop: handlers: {self.client.events.handlers}")
-        if self.web_socket:
-            await self.web_socket.close()
-
     async def start_wss(self):
         listen_key = (await self.client.create_listen_key())["listenKey"]
-        self.web_socket = await self.session.ws_connect(f"{self.endpoint}/ws/{listen_key}",
-                                                        heartbeat=15,
-                                                        proxy=self.client.proxy)
+        self.web_socket = await self.session.ws_connect(f"{self.endpoint}/ws/{listen_key}", heartbeat=15)
         _task = asyncio.ensure_future(self._heartbeat(listen_key))
         try:
             await self._handle_messages(self.web_socket)
         finally:
             _task.cancel()
 
     async def _handle_event(self, content):
```

### Comparing `exchanges-wrapper-1.2.9.post2/pyproject.toml` & `exchanges-wrapper-1.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -13,19 +13,21 @@
              "Operating System :: Unix",
              "Operating System :: Microsoft :: Windows",
              "Operating System :: MacOS"]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 
 dependencies = [
-    "aiohttp==3.8.1",
-    "grpcio==1.48.1",
-    "grpcio-tools==1.48.1",
+    "aiohttp==3.8.4",
+    "grpcio==1.54.2",
+    "grpcio-tools==1.54.2",
     "toml==0.10.2",
-    "idna==3.3"
+    "idna==3.4",
+    "pyotp~=2.8.0",
+    "simplejson==3.19.1"
 ]
 
 [tool.flit.module]
 name = "exchanges_wrapper"
 
 [project.urls]
 Source = "https://github.com/DogsTailFarmer/exchanges-wrapper"
```

### Comparing `exchanges-wrapper-1.2.9.post2/PKG-INFO` & `exchanges-wrapper-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: exchanges-wrapper
-Version: 1.2.9.post2
+Version: 1.3.0
 Summary: REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
 Author-email: Thomas Marchand <thomas.marchand@tuta.io>, Jerry Fedorenko <jerry.fedorenko@yahoo.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
-Requires-Dist: aiohttp==3.8.1
-Requires-Dist: grpcio==1.48.1
-Requires-Dist: grpcio-tools==1.48.1
+Requires-Dist: aiohttp==3.8.4
+Requires-Dist: grpcio==1.54.2
+Requires-Dist: grpcio-tools==1.54.2
 Requires-Dist: toml==0.10.2
-Requires-Dist: idna==3.3
+Requires-Dist: idna==3.4
+Requires-Dist: pyotp~=2.8.0
+Requires-Dist: simplejson==3.19.1
 Project-URL: Source, https://github.com/DogsTailFarmer/exchanges-wrapper
 
 
 <p align="center"><img src="https://raw.githubusercontent.com/gist/DogsTailFarmer/167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/Logo%202v3.svg" width="300"></p>
 
 ***
 <h1 align="center">Crypto exchanges API/WSS wrapper with grpc powered server</h1>
@@ -32,14 +34,15 @@
 <a href="https://badge.fury.io/py/exchanges-wrapper"><img src="https://badge.fury.io/py/exchanges-wrapper.svg" alt="PyPI version"></a>
 <a href="https://codeclimate.com/github/DogsTailFarmer/exchanges-wrapper/maintainability"><img src="https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/maintainability" /></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=resolved+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper/?ref=repository-badge}" target="_blank"><img alt="DeepSource" title="DeepSource" src="https://deepsource.io/gh/DogsTailFarmer/exchanges-wrapper.svg/?label=active+issues&token=XuG5PmzMiKlDL921-qREIuX_"/></a>
 <a href="https://sonarcloud.io/summary/new_code?id=DogsTailFarmer_exchanges-wrapper" target="_blank"><img alt="sonarcloud" title="sonarcloud" src="https://sonarcloud.io/api/project_badges/measure?project=DogsTailFarmer_exchanges-wrapper&metric=alert_status"/></a>
 <a href="https://pepy.tech/project/exchanges-wrapper" target="_blank"><img alt="Downloads" title="Downloads" src="https://pepy.tech/badge/exchanges-wrapper/month"/></a>
 ***
+From 1.2.10 update exch_srv_cfg.toml (see CHANGELOG for details)
 ***
 
 ## exchanges-wrapper vs binance.py
 The main difference is the development of the project for trading with many exchanges.
 
 Next is adding a new module ```exchanges_wrapper/exch_srv.py``` as a multiplexer layer, providing simultaneous async interaction for many accounts
 and many trading pairs through one connection. It's powered by [gRPC](https://grpc.io/about/)
```

#### html2text {}

```diff
@@ -1,60 +1,62 @@
-Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.2.9.post2 Summary:
-REST API and WebSocket asyncio wrapper with grpc powered multiplexer server
-Author-email: Thomas Marchand
+Metadata-Version: 2.1 Name: exchanges-wrapper Version: 1.3.0 Summary: REST API
+and WebSocket asyncio wrapper with grpc powered multiplexer server Author-
+email: Thomas Marchand
 marchand@tuta.io>, Jerry Fedorenko
 fedorenko@yahoo.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Programming Language :: Python :: 3 Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: Unix Classifier: Operating
 System :: Microsoft :: Windows Classifier: Operating System :: MacOS Requires-
-Dist: aiohttp==3.8.1 Requires-Dist: grpcio==1.48.1 Requires-Dist: grpcio-
-tools==1.48.1 Requires-Dist: toml==0.10.2 Requires-Dist: idna==3.3 Project-URL:
-Source, https://github.com/DogsTailFarmer/exchanges-wrapper
+Dist: aiohttp==3.8.4 Requires-Dist: grpcio==1.54.2 Requires-Dist: grpcio-
+tools==1.54.2 Requires-Dist: toml==0.10.2 Requires-Dist: idna==3.4 Requires-
+Dist: pyotp~=2.8.0 Requires-Dist: simplejson==3.19.1 Project-URL: Source,
+https://github.com/DogsTailFarmer/exchanges-wrapper
             [https://raw.githubusercontent.com/gist/DogsTailFarmer/
 167eaf65cebfe95d954082c7f181a2cc/raw/a67270de8663ad3de4733330ff64c9ba3153f87d/
                                 Logo%202v3.svg]
 ***
     ****** Crypto exchanges API/WSS wrapper with grpc powered server ******
                   ***** Binance, Bitfinex, Huobi, OKX, *****
                           **** For SPOT markets ****
 *** [PyPI_version] [https://api.codeclimate.com/v1/badges/f333ab9b1f3024699e09/
-maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** *** ##
-exchanges-wrapper vs binance.py The main difference is the development of the
-project for trading with many exchanges. Next is adding a new module
-```exchanges_wrapper/exch_srv.py``` as a multiplexer layer, providing
-simultaneous async interaction for many accounts and many trading pairs through
-one connection. It's powered by [gRPC](https://grpc.io/about/) Remote Procedure
-Call framework. Warning. Coverage of overridden binance.py packages is
-significant but not complete. Served methods describes into ```example/
-exch_client.py``` ### Initial capabilities (inherited from binance.py) - Covers
-general endpoints (test connectivity and get exchange information's) - Covers
-market data endpoints - Covers Account endpoints (create and manage orders) -
-Covers user data stream (receive real time user updates) - Covers web socket
-streams (receive real time market updates) - Async support - Auto reconnect
-after exchanges API or network failure - Completely free and without
-limitations ### Added Features - Multi exchanges support - Adaptive algorithm
-to ensure maximum performance and avoid exceeding the rates limits -
-Passthrough logging ## Extra exchanges implementation features - Binance REST
-API and WSS are accepted as basic, connection of other exchanges wrapped their
-API to Binance compatible - For other, some data cannot be obtained by directly
-calling one method, it is generated by a synthetic or calculation method - Some
-exchanges have not any testing or "paper trading" features, therefore,
-application development and testing is possible only at real bidding. First,
-run applications on the [Binance Spot Test Network](https://
-testnet.binance.vision/) or Bitfinex test account. ## Get started ### Prepare
-exchange account * Create account on [Binance](https://accounts.binance.com/en/
-register?ref=QCS4OGWR) and get 10% discount on all trading fee * Create account
-on [Bitfinex](https://www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6%
-rebate fee * Create account on [HUOBI](https://www.huobi.com/en-us/topic/
-double-reward/?invite_code=9uaw3223) and get 10% cashback on all trading fee *
-Create account on [OKX](https://www.okx.com/join/2607649) and get Mystery Boxes
-worth up to $10,000 * For test purpose log in at [Binance Spot Test Network]
-(https://testnet.binance.vision/) * Create API Key * After install and first
-run specify api_key and api_secret in ```/home/ubuntu/.MartinBinance/config/
+maintainability] [DeepSource] [DeepSource] [sonarcloud] [Downloads] *** From
+1.2.10 update exch_srv_cfg.toml (see CHANGELOG for details) *** ## exchanges-
+wrapper vs binance.py The main difference is the development of the project for
+trading with many exchanges. Next is adding a new module ```exchanges_wrapper/
+exch_srv.py``` as a multiplexer layer, providing simultaneous async interaction
+for many accounts and many trading pairs through one connection. It's powered
+by [gRPC](https://grpc.io/about/) Remote Procedure Call framework. Warning.
+Coverage of overridden binance.py packages is significant but not complete.
+Served methods describes into ```example/exch_client.py``` ### Initial
+capabilities (inherited from binance.py) - Covers general endpoints (test
+connectivity and get exchange information's) - Covers market data endpoints -
+Covers Account endpoints (create and manage orders) - Covers user data stream
+(receive real time user updates) - Covers web socket streams (receive real time
+market updates) - Async support - Auto reconnect after exchanges API or network
+failure - Completely free and without limitations ### Added Features - Multi
+exchanges support - Adaptive algorithm to ensure maximum performance and avoid
+exceeding the rates limits - Passthrough logging ## Extra exchanges
+implementation features - Binance REST API and WSS are accepted as basic,
+connection of other exchanges wrapped their API to Binance compatible - For
+other, some data cannot be obtained by directly calling one method, it is
+generated by a synthetic or calculation method - Some exchanges have not any
+testing or "paper trading" features, therefore, application development and
+testing is possible only at real bidding. First, run applications on the
+[Binance Spot Test Network](https://testnet.binance.vision/) or Bitfinex test
+account. ## Get started ### Prepare exchange account * Create account on
+[Binance](https://accounts.binance.com/en/register?ref=QCS4OGWR) and get 10%
+discount on all trading fee * Create account on [Bitfinex](https://
+www.bitfinex.com/sign-up?refcode=v_4az2nCP) and get 6% rebate fee * Create
+account on [HUOBI](https://www.huobi.com/en-us/topic/double-reward/
+?invite_code=9uaw3223) and get 10% cashback on all trading fee * Create account
+on [OKX](https://www.okx.com/join/2607649) and get Mystery Boxes worth up to
+$10,000 * For test purpose log in at [Binance Spot Test Network](https://
+testnet.binance.vision/) * Create API Key * After install and first run specify
+api_key and api_secret in ```/home/ubuntu/.MartinBinance/config/
 exch_srv_cfg.toml``` ### Use Docker image ```console docker pull ghcr.io/
 dogstailfarmer/exchanges-wrapper:latest ``` #### First run The structure of the
 working directory will be created and the necessary files will be copied: For
 Ubuntu it will be here: ```home/user/.MartinBinance/``` ```console docker run -
 -rm --entrypoint /bin/sh exchanges-wrapper -c "cat ./exchanges_wrapper/
 __init__.py" > init.py && \ docker run --rm --entrypoint /bin/sh exchanges-
 wrapper -c "cat ./exchanges_wrapper/exch_srv_cfg.toml.template" >
```

