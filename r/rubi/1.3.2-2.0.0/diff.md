# Comparing `tmp/rubi-1.3.2.tar.gz` & `tmp/rubi-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-1.3.2.tar", max compression
+gzip compressed data, was "rubi-2.0.0.tar", max compression
```

## Comparing `rubi-1.3.2.tar` & `rubi-2.0.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-1.3.2/LICENSE
--rw-r--r--   0        0        0     1282 2023-05-24 19:25:18.033040 rubi-1.3.2/README.md
--rw-r--r--   0        0        0      676 2023-05-24 19:27:47.087742 rubi-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      734 2023-05-24 19:25:18.036048 rubi-1.3.2/rubi/README.md
--rw-r--r--   0        0        0       25 2023-02-09 17:21:21.760544 rubi-1.3.2/rubi/__init__.py
--rw-r--r--   0        0        0       22 2023-02-09 17:21:21.760681 rubi-1.3.2/rubi/book/__init__.py
--rw-r--r--   0        0        0     6750 2023-02-09 17:21:21.760791 rubi-1.3.2/rubi/book/book.py
--rw-r--r--   0        0        0      183 2023-02-14 16:34:53.715874 rubi-1.3.2/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61065 2023-02-14 16:34:53.716268 rubi-1.3.2/rubi/contracts/aid.py
--rw-r--r--   0        0        0       69 2023-02-09 17:21:21.761424 rubi-1.3.2/rubi/contracts/helper/__init__.py
--rw-r--r--   0        0        0     6735 2023-02-09 17:21:21.761755 rubi-1.3.2/rubi/contracts/helper/abis/ERC20.json
--rw-r--r--   0        0        0    17057 2023-02-09 17:21:21.762046 rubi-1.3.2/rubi/contracts/helper/abis/MarketAid.json
--rw-r--r--   0        0        0     2649 2023-02-09 17:21:21.762146 rubi-1.3.2/rubi/contracts/helper/abis/MarketAidFactory.json
--rw-r--r--   0        0        0    37232 2023-02-09 17:21:21.762272 rubi-1.3.2/rubi/contracts/helper/abis/RubiconMarket.json
--rw-r--r--   0        0        0    15314 2023-02-09 17:21:21.762375 rubi-1.3.2/rubi/contracts/helper/abis/RubiconRouter.json
--rw-r--r--   0        0        0    22002 2023-02-14 16:34:53.716553 rubi-1.3.2/rubi/contracts/helper/erc20.py
--rw-r--r--   0        0        0     5371 2023-02-14 16:34:53.716723 rubi-1.3.2/rubi/contracts/helper/rolodex.py
--rw-r--r--   0        0        0    38518 2023-02-14 16:34:53.716886 rubi-1.3.2/rubi/contracts/market.py
--rw-r--r--   0        0        0    11564 2023-02-14 16:34:53.717077 rubi-1.3.2/rubi/contracts/router.py
--rw-r--r--   0        0        0      206 2023-02-14 16:34:53.717196 rubi-1.3.2/rubi/data/README.md
--rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-1.3.2/rubi/data/__init__.py
--rw-r--r--   0        0        0     3932 2023-02-14 16:34:53.717374 rubi-1.3.2/rubi/data/data.py
--rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-1.3.2/rubi/data/processing/README.md
--rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-1.3.2/rubi/data/processing/__init__.py
--rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-1.3.2/rubi/data/processing/aid.py
--rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-1.3.2/rubi/data/processing/helper/__init__.py
--rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-1.3.2/rubi/data/processing/helper/processing.py
--rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-1.3.2/rubi/data/processing/user.py
--rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-1.3.2/rubi/data/sources/__init__.py
--rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-1.3.2/rubi/data/sources/aid.py
--rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-1.3.2/rubi/data/sources/helper/README.md
--rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-1.3.2/rubi/data/sources/helper/__init__.py
--rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-1.3.2/rubi/data/sources/helper/gas.py
--rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-1.3.2/rubi/data/sources/helper/price.py
--rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-1.3.2/rubi/data/sources/helper/rolodex.py
--rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-1.3.2/rubi/data/sources/market.py
--rw-r--r--   0        0        0     8258 2023-05-24 19:15:33.694846 rubi-1.3.2/rubi/rubi.py
--rw-r--r--   0        0        0     2102 1970-01-01 00:00:00.000000 rubi-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2757 2023-06-01 18:59:40.461664 rubi-2.0.0/README.md
+-rw-r--r--   0        0        0      713 2023-06-01 18:59:40.471784 rubi-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-06-01 18:59:40.472105 rubi-2.0.0/rubi/__init__.py
+-rw-r--r--   0        0        0    27357 2023-06-01 18:59:40.472316 rubi-2.0.0/rubi/client.py
+-rw-r--r--   0        0        0      154 2023-06-01 18:59:40.472446 rubi-2.0.0/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.0/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    11606 2023-06-01 18:59:40.472881 rubi-2.0.0/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0    16248 2023-06-01 18:59:40.473031 rubi-2.0.0/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24182 2023-06-01 18:59:40.473250 rubi-2.0.0/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14668 2023-06-01 18:59:40.473453 rubi-2.0.0/rubi/contracts/router.py
+-rw-r--r--   0        0        0       22 2023-06-01 18:59:40.473528 rubi-2.0.0/rubi/contracts/types/__init__.py
+-rw-r--r--   0        0        0    16011 2023-06-01 18:59:40.473629 rubi-2.0.0/rubi/contracts/types/events.py
+-rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.0/rubi/data/README.md
+-rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.0/rubi/data/__init__.py
+-rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.0/rubi/data/data.py
+-rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.0/rubi/data/processing/README.md
+-rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.0/rubi/data/processing/__init__.py
+-rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.0/rubi/data/processing/aid.py
+-rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.0/rubi/data/processing/helper/__init__.py
+-rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.0/rubi/data/processing/helper/processing.py
+-rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.0/rubi/data/processing/user.py
+-rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.0/rubi/data/sources/__init__.py
+-rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.0/rubi/data/sources/aid.py
+-rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.0/rubi/data/sources/helper/README.md
+-rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.0/rubi/data/sources/helper/__init__.py
+-rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.0/rubi/data/sources/helper/gas.py
+-rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.0/rubi/data/sources/helper/price.py
+-rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.0/rubi/data/sources/helper/rolodex.py
+-rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.0/rubi/data/sources/market.py
+-rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.0/rubi/network/__init__.py
+-rw-r--r--   0        0        0     7589 2023-06-01 18:59:40.474413 rubi-2.0.0/rubi/network/network.py
+-rw-r--r--   0        0        0       66 2023-06-01 18:59:40.474481 rubi-2.0.0/rubi/types/__init__.py
+-rw-r--r--   0        0        0    12515 2023-06-01 18:59:40.474581 rubi-2.0.0/rubi/types/order.py
+-rw-r--r--   0        0        0     5719 2023-06-01 18:59:40.474684 rubi-2.0.0/rubi/types/orderbook.py
+-rw-r--r--   0        0        0     2707 2023-06-01 18:59:40.474750 rubi-2.0.0/rubi/types/pair.py
+-rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 rubi-2.0.0/PKG-INFO
```

### Comparing `rubi-1.3.2/LICENSE` & `rubi-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-1.3.2/pyproject.toml` & `rubi-2.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 [tool.poetry]
 name = "rubi"
-version = "1.3.2"
-description = "a python SDK for the Rubicon Protocol"
-authors = ["denver <denver@rubicon.finance>"]
+version = "2.0.0"
+description = "A python SDK for the Rubicon Protocol"
+authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sphinx = "7.0.1"
-web3 = "^6.4.0"
-hexbytes = "^0.3.0"
-attributedict = "^0.3.0"
-eth-abi = "^4.0.0"
-pytest = "^7.3.1"
-eth-tester = "^0.9.0b1"
-py-evm = "^0.7.0a2"
-eth-utils = "^2.1.0"
-subgrounds = { version = "^1.5.1", extras = ["dash"] }
+web3 = "6.4.0"
+hexbytes = "0.3.0"
+attributedict = "0.3.0"
+eth-abi = "4.0.0"
+pytest = "7.3.1"
+eth-tester = "0.9.0b1"
+py-evm = "0.7.0a2"
+eth-utils = "2.1.0"
+subgrounds = { version = "1.6.0", extras = ["dash"] }
+pyyaml = "6.0.0"
 
 [tool.poetry.group.dev.dependencies]
-python-dotenv = "^0.21.0"
-ipykernel = "^6.5.0"
-jupyter = "^1.0.0"
+python-dotenv = "0.21.1"
+ipykernel = "6.23.1"
+jupyter = "1.0.0"
 
 [tool.poetry.extras]
 docs = ["sphinx"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rubi-1.3.2/rubi/contracts/aid.py` & `rubi-2.0.0/rubi/contracts/aid.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,34 @@
 import os
-import json 
+import json
 import hexbytes
 import logging as log
 from eth_abi import decode
 from eth_abi.codec import ABICodec
 from web3._utils.events import get_event_data
 
 from rubi.contracts.helper import networks
 
+
+# DEPRECATED
+# TODO: this is the old implementation for the RubiconMarketAidFactory and RubiconMarketAid. It needs to be updated in
+#  line with all the other contracts in this repo. Usage is not recommended in it's current state and it is not included
+#  in any of the __init__.py files.
 class FactoryAid:
     """this class represents the MarketAidFactory.sol contract and has read functionality for the contract
     
     :param w3: Web3 instance
     :type w3: Web3
     :param contract: an optional contract instance, if not provided, the contract will be instantiated using the address and abi from the networks.py file given the chain id of the w3 instance
     :type contract: Web3 object, optional
     """
 
     def __init__(self, w3, contract=None):
         """constructor method"""
+        raise DeprecationWarning()
 
         chain = w3.eth.chain_id
 
         if contract:
             self.contract = contract
             self.address = self.contract.address
         else:
@@ -42,34 +48,34 @@
     # admin()
     def admin(self):
         """returns the admin address of the contract
 
         :return: the admin address
         :rtype: str
         """
-            
-        try: 
+
+        try:
             admin = self.contract.functions.admin().call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
-        return admin             
+        return admin
 
     # getUserMarketAids(user (address))
     def get_user_market_aids(self, user):
         """returns the market aid addresses for a given user
 
         :return: an array of market aid addresses
         :rtype: list
         """
 
-        try: 
+        try:
             aids = self.contract.functions.getUserMarketAids(user).call()
-        except ValueError: 
+        except ValueError:
             aids = self.contract.functions.getUserMarketAids(self.w3.to_checksum_address(user)).call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return aids
 
@@ -77,20 +83,20 @@
     def rubicon_market(self):
         """returns the address of the RubiconMarket contract
 
         :return: rubicon market address
         :rtype: str
         """
 
-        try: 
+        try:
             rubicon_market = self.contract.functions.rubiconMarket().call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return rubicon_market
 
 class FactoryAidSigner(FactoryAid):
     """this class represents the MarketAidFactory.sol contract and has read and write functionality for the contract. this class inherits from the FactoryAid class
     
     :param w3: a web3 instance
     :type w3: Web3
@@ -125,15 +131,15 @@
         :rtype: dict, None
         """
 
         if nonce is None:
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
-        
+
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
         txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
 
         try:
             create = self.contract.functions.createMarketAidInstance().build_transaction(txn)
@@ -145,29 +151,30 @@
                 if self.w3.eth.wait_for_transaction_receipt(create.hash)['status'] == 0:
                     log.error(f"create_market_aid_instance transaction failed: {create.hash.hex()}")
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return create
 
-class MarketAid: 
+class MarketAid:
 
     # init function
     # TODO: possibly allow a chain variable to be passed in
     def __init__(self, w3, address, contract=None):
+        raise DeprecationWarning()
 
         # load in the aid abi 
         path = f"{os.path.dirname(os.path.realpath(__file__))}/helper/abis/MarketAid.json"
         with open(path) as f:
             aid_abi = json.load(f)
         f.close()
-    
+
         # create contract instance or set based upon initiliazation
         if contract:
             self.contract = contract
             self.address = self.contract.address
             chain = w3.eth.chain_id
         else:
             chain = w3.eth.chain_id
@@ -193,15 +200,15 @@
     def rubicon_market_address(self):
         """this function returns the address of the RubiconMarket contract
 
         :return: the address of the RubiconMarket contract
         :rtype: str
         """
 
-        try: 
+        try:
             rubicon_market_address = self.contract.functions.RubiconMarketAddress().call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
 
         return rubicon_market_address
 
@@ -209,60 +216,60 @@
     def admin(self):
         """this function returns the address of the admin
 
         :return: the address of the admin
         :rtype: str
         """
 
-        try: 
+        try:
             admin = self.contract.functions.admin().call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return admin
 
     # approvedStrategists()
     def approved_strategists(self, address):
         """this function returns the list of approved strategists
 
         :return: the list of approved strategists
         :rtype: list
         """
 
-        try: 
+        try:
             approved_strategists = self.contract.functions.approvedStrategists(address).call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return approved_strategists
-    
+
     # getOutstandingStrategistTrades(asset (address), quote (address), strategist (address))
     def get_outstanding_strategist_trades(self, asset, quote, strategist):
         """this function returns the list of outstanding trades for a strategist
 
         :param asset: the address of the asset
         :type asset: str
         :param quote: the address of the quote
         :type quote: str
         :param strategist: the address of the strategist
         :type strategist: str
         :return: the list of outstanding trades for a strategist
         :rtype: list
         """
 
-        try: 
+        try:
             outstanding_strategist_trades = self.contract.functions.getOutstandingStrategistTrades(asset, quote, strategist).call()
-        except ValueError: 
+        except ValueError:
             outstanding_strategist_trades = self.contract.functions.getOutstandingStrategistTrades(self.w3.to_checksum_address(asset), self.w3.to_checksum_address(quote), self.w3.to_checksum_address(strategist)).call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return outstanding_strategist_trades
 
     # getStrategistTotalLiquidity(asset (address), quote (address), strategist (address))
     def get_strategist_total_liquidity(self, asset, quote, strategist):
         """this function returns the total liquidity for a strategist 
 
         :param asset: the address of the asset
@@ -271,42 +278,42 @@
         :type quote: str
         :param strategist: the address of the strategist
         :type strategist: str
         :return: the total liquidity for a strategist
         :rtype: int
         """
 
-        try: 
+        try:
             strategist_total_liquidity = self.contract.functions.getStrategistTotalLiquidity(asset, quote, strategist).call()
-        except ValueError: 
+        except ValueError:
             strategist_total_liquidity = self.contract.functions.getStrategistTotalLiquidity(self.w3.to_checksum_address(asset), self.w3.to_checksum_address(quote), self.w3.to_checksum_address(strategist)).call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return strategist_total_liquidity
 
     # isApprovedStrategist(strategist (address))
     def is_approved_strategist(self, strategist):
         """this function returns whether or not a strategist is approved
 
         :param strategist: the address of the strategist
         :type strategist: str
         :return: whether or not a strategist is approved
         :rtype: bool
         """
 
-        try: 
+        try:
             is_approved_strategist = self.contract.functions.isApprovedStrategist(strategist).call()
-        except ValueError: 
+        except ValueError:
             is_approved_strategist = self.contract.functions.isApprovedStrategist(self.w3.to_checksum_address(strategist)).call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return is_approved_strategist
 
     def get_strategist_trade(self, trade_id):
         """this function returns a strategist trade
 
         :param trade_id: the id of the trade
         :type trade_id: int
@@ -315,35 +322,35 @@
         """
 
         # check that the trade id is an integer
         if not isinstance(trade_id, int):
             log.error("trade id is not an integer")
             return None
 
-        try: 
+        try:
             strategist_trade = self.contract.functions.strategistTrades(trade_id).call()
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return strategist_trade
 
     ######################################################################
     # events & helpers
     ######################################################################
 
     # TODO: today the event signature is hardcoded, but we should be able to get it from the contract
     # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis 
     def get_log_strategist_trade_hash(self):
         return self.w3.keccak(text="LogStrategistTrade(uint256,bytes32,bytes32,address,address,uint256,address)").hex()
 
     # TODO: determine if this is the right assumtption to make about how the data is being received 
     # this assumes that the function is being used directly in the context of being passed raw data from a websocket stream that has been loaded and converted to an AttributeDict
     # TODO: i feel like this could be done much faster... tracing will tell us
-    def stream_log_strategist_trade(self, data): 
+    def stream_log_strategist_trade(self, data):
 
         # load the data into an attribute dictionary that web3 can use
         # data = AttributeDict(json.loads(data))
 
         # convert the topics, transaction hash, and block hash to hex strings
         data['params']['result']['topics'] = [hexbytes.HexBytes(topic) for topic in data['params']['result']['topics']]
         data['params']['result']['transactionHash'] = hexbytes.HexBytes(data['params']['result']['transactionHash'])
@@ -359,28 +366,28 @@
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
                     'id': trade_id,
                     'txn': event['transactionHash'].hex(),
                     'event': event['event'],
-                    'ask_id': event['args']['askId'],  
+                    'ask_id': event['args']['askId'],
                     'bid_id': event['args']['bidId'],
                     'ask_asset': event['args']['askAsset'],
                     'bid_asset': event['args']['bidAsset'],
                     'timestamp': event['args']['timestamp'],
                     'owner': event['args']['strategist']
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
-            return None 
+            return None
 
-    def parse_log_strategist_trade(self, log): 
+    def parse_log_strategist_trade(self, log):
 
         # get the event data from the log
         try:
             event = get_event_data(self.codec, self.log_strategist_trade_abi, log['params']['result'])
 
             # decode the offer id
             # TODO: there is probably a way to do this that does not hardcode the type of the id
@@ -388,26 +395,26 @@
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
                     'id': trade_id,
                     'txn': event['transactionHash'].hex(),
                     'event': event['event'],
-                    'ask_id': event['args']['askId'],  
+                    'ask_id': event['args']['askId'],
                     'bid_id': event['args']['bidId'],
                     'ask_asset': event['args']['askAsset'],
                     'bid_asset': event['args']['bidAsset'],
                     'timestamp': event['args']['timestamp'],
                     'owner': event['args']['strategist']
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
-            return None 
+            return None
 
     '''
     event LogScrubbedStratTrade(
         uint256 strategistIDScrubbed,
         uint256 assetFill,
         address bathAssetAddress,
         uint256 quoteFill,
@@ -419,15 +426,15 @@
     # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis 
     def get_log_scrubbed_strat_trade_hash(self):
         return self.w3.keccak(text="LogStrategistTrade(uint256,uint256,address,uint256,address)").hex()
 
     # TODO: determine if this is the right assumtption to make about how the data is being received 
     # this assumes that the function is being used directly in the context of being passed raw data from a websocket stream that has been loaded and converted to an AttributeDict
     # TODO: i feel like this could be done much faster... tracing will tell us
-    def stream_log_scrubbed_strat_trade(self, data): 
+    def stream_log_scrubbed_strat_trade(self, data):
 
         # load the data into an attribute dictionary that web3 can use
         # data = AttributeDict(json.loads(data))
 
         # convert the topics, transaction hash, and block hash to hex strings
         data['params']['result']['topics'] = [hexbytes.HexBytes(topic) for topic in data['params']['result']['topics']]
         data['params']['result']['transactionHash'] = hexbytes.HexBytes(data['params']['result']['transactionHash'])
@@ -443,26 +450,26 @@
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
                     'id': trade_id,
                     'txn': event['transactionHash'].hex(),
                     'event': event['event'],
-                    'asset_fill': event['args']['assetFill'],  
+                    'asset_fill': event['args']['assetFill'],
                     'bath_asset_address': event['args']['bathAssetAddress'],
                     'quote_fill': event['args']['quoteFill'],
                     'quote_address': event['args']['quoteAddress']
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
-            return None 
-        
-    def parse_log_scrubbed_strat_trade(self, log): 
+            return None
+
+    def parse_log_scrubbed_strat_trade(self, log):
 
         # get the event data from the log
         try:
             event = get_event_data(self.codec, self.log_scrubbed_strat_trade_abi, log['params']['result'])
 
             # decode the offer id
             # TODO: there is probably a way to do this that does not hardcode the type of the id
@@ -470,24 +477,24 @@
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
                     'id': trade_id,
                     'txn': event['transactionHash'].hex(),
                     'event': event['event'],
-                    'asset_fill': event['args']['assetFill'],  
+                    'asset_fill': event['args']['assetFill'],
                     'bath_asset_address': event['args']['bathAssetAddress'],
                     'quote_fill': event['args']['quoteFill'],
                     'quote_address': event['args']['quoteAddress']
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
-            return None 
+            return None
 
     '''
     event LogStrategistRewardClaim(
         address strategist,
         address asset,
         uint256 amountOfReward,
         uint256 timestamp
@@ -504,15 +511,15 @@
     # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis 
     def get_log_batch_market_making_trades_hash(self):
         return self.w3.keccak(text="LogBatchMarketMakingTrades(address,uint256[])").hex()
 
     # TODO: determine if this is the right assumtption to make about how the data is being received 
     # this assumes that the function is being used directly in the context of being passed raw data from a websocket stream that has been loaded and converted to an AttributeDict
     # TODO: i feel like this could be done much faster... tracing will tell us
-    def stream_log_batch_market_making_trades(self, data): 
+    def stream_log_batch_market_making_trades(self, data):
 
         # load the data into an attribute dictionary that web3 can use
         # data = AttributeDict(json.loads(data))
 
         # convert the topics, transaction hash, and block hash to hex strings
         data['params']['result']['topics'] = [hexbytes.HexBytes(topic) for topic in data['params']['result']['topics']]
         data['params']['result']['transactionHash'] = hexbytes.HexBytes(data['params']['result']['transactionHash'])
@@ -523,42 +530,42 @@
             event = get_event_data(self.codec, self.log_batch_market_making_trades_abi, data['params']['result'])
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
                     'txn': event['transactionHash'].hex(),
                     'event': event['event'],
-                    'strategist': event['args']['strategist'],  
+                    'strategist': event['args']['strategist'],
                     'trades': event['args']['trades']
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
-            return None 
-        
-    def parse_log_batch_market_making_trades(self, log): 
+            return None
+
+    def parse_log_batch_market_making_trades(self, log):
 
         # get the event data from the log
         try:
             event = get_event_data(self.codec, self.log_batch_market_making_trades_abi, log['params']['result'])
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
                     'txn': event['transactionHash'].hex(),
                     'event': event['event'],
-                    'strategist': event['args']['strategist'],  
+                    'strategist': event['args']['strategist'],
                     'trades': event['args']['trades']
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
-            return None 
+            return None
 
     '''
         event LogRequote(
         address strategist,
         uint256 scrubbedOfferID,
         uint256 newOfferID
     );
@@ -567,15 +574,15 @@
     # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis 
     def get_log_requote_hash(self):
         return self.w3.keccak(text="LogRequote(address,uint256,uint256)").hex()
 
     # TODO: determine if this is the right assumtption to make about how the data is being received 
     # this assumes that the function is being used directly in the context of being passed raw data from a websocket stream that has been loaded and converted to an AttributeDict
     # TODO: i feel like this could be done much faster... tracing will tell us
-    def stream_log_requote(self, data): 
+    def stream_log_requote(self, data):
 
         # load the data into an attribute dictionary that web3 can use
         # data = AttributeDict(json.loads(data))
 
         # convert the topics, transaction hash, and block hash to hex strings
         data['params']['result']['topics'] = [hexbytes.HexBytes(topic) for topic in data['params']['result']['topics']]
         data['params']['result']['transactionHash'] = hexbytes.HexBytes(data['params']['result']['transactionHash'])
@@ -592,25 +599,25 @@
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
                     'id': trade_id,
                     'txn': event['transactionHash'].hex(),
                     'event': event['event'],
-                    'strategist': event['args']['strategist'],  
+                    'strategist': event['args']['strategist'],
                     'scrub_trade_id': scrub_trade_id,
                     'trade_id': trade_id
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
-            return None 
-    
-    def parse_log_requote(self, log): 
+            return None
+
+    def parse_log_requote(self, log):
 
         # get the event data from the log
         try:
             event = get_event_data(self.codec, self.log_requote_abi, log['params']['result'])
 
             # decode the offer id
             # TODO: there is probably a way to do this that does not hardcode the type of the id
@@ -619,36 +626,36 @@
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
                     'id': trade_id,
                     'txn': event['transactionHash'].hex(),
                     'event': event['event'],
-                    'strategist': event['args']['strategist'],  
+                    'strategist': event['args']['strategist'],
                     'scrub_trade_id': scrub_trade_id,
                     'trade_id': trade_id
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
-            return None 
+            return None
 
     '''
     event LogBatchRequoteOffers(address strategist, uint256[] scrubbedOfferIDs);
-    ''' 
+    '''
     # TODO: today the event signature is hardcoded, but we should be able to get it from the contract
     # the graph does something similar to this when you run codegen, it should be a simple string manipulation problem from the abis 
     def get_log_batch_requote_offers_hash(self):
         return self.w3.keccak(text="LogBatchRequoteOffers(address,uint256[])").hex()
 
     # TODO: determine if this is the right assumtption to make about how the data is being received 
     # this assumes that the function is being used directly in the context of being passed raw data from a websocket stream that has been loaded and converted to an AttributeDict
     # TODO: i feel like this could be done much faster... tracing will tell us
-    def stream_log_batch_requote_offers(self, data): 
+    def stream_log_batch_requote_offers(self, data):
 
         # load the data into an attribute dictionary that web3 can use
         # data = AttributeDict(json.loads(data))
 
         # convert the topics, transaction hash, and block hash to hex strings
         data['params']['result']['topics'] = [hexbytes.HexBytes(topic) for topic in data['params']['result']['topics']]
         data['params']['result']['transactionHash'] = hexbytes.HexBytes(data['params']['result']['transactionHash'])
@@ -659,43 +666,43 @@
             event = get_event_data(self.codec, self.log_batch_requote_offers_abi, data['params']['result'])
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
                     'txn': event['transactionHash'].hex(),
                     'event': event['event'],
-                    'strategist': event['args']['strategist'],  
+                    'strategist': event['args']['strategist'],
                     'scrub_trade_id': event['args']['scrubbedOfferIDs']
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
-            return None 
-    
-    def parse_log_batch_requote_offers(self, log): 
+            return None
+
+    def parse_log_batch_requote_offers(self, log):
 
         # get the event data from the log
         try:
             event = get_event_data(self.codec, self.log_batch_requote_offers_abi, log['params']['result'])
 
             # now pass an offer back in the form of a dictionary
             # TODO: this is probably not the most performant, we will optimize later
             trade = {
                     'txn': event['transactionHash'].hex(),
                     'event': event['event'],
-                    'strategist': event['args']['strategist'],  
+                    'strategist': event['args']['strategist'],
                     'scrub_trade_id': event['args']['scrubbedOfferIDs']
             }
             return trade
 
         except Exception as e:
             log.error(e, exc_info=True)
-            return None 
-     
+            return None
+
 
 class MarketAidSigner(MarketAid):
     """this class represents a MarketAid.sol contract with read and write functionality. it inherits from the MarketAid class and adds the ability to sign transactions.
 
     :param w3: a web3 instance
     :type w3: Web3
     :param address: the address of the contract
@@ -767,15 +774,15 @@
                 if self.w3.eth.wait_for_transaction_receipt(max_approve.hash)['status'] == 0:
                     log.error(f'admin_max_approve_target transaction {max_approve.hash.hex()} failed')
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return max_approve
 
     # adminPullAllFunds(erc20s address[])
     def admin_pull_all_funds(self, erc20s, nonce=None, gas=3000000, gas_price=None):
         """this function pulls all funds from the contract
         
         :param erc20s: a list of erc20 addresses
@@ -790,18 +797,18 @@
         :rtype: dict, None
         """
 
         if nonce is None:
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
-        
+
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
-        
+
         txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
 
         try:
             pull_all_funds = self.contract.functions.adminPullAllFunds(erc20s).build_transaction(txn)
             pull_all_funds = self.w3.eth.account.sign_transaction(pull_all_funds, self.key)
             self.w3.eth.send_raw_transaction(pull_all_funds.rawTransaction)
 
@@ -835,15 +842,15 @@
         :rtype: dict, None
         """
 
         if nonce is None:
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
-        
+
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
         txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
 
         try:
             rebalance = self.contract.functions.adminRebalanceFunds(asset_to_sell, amount_to_sell, asset_to_target).build_transaction(txn)
@@ -867,15 +874,15 @@
                 if self.w3.eth.wait_for_transaction_receipt(rebalance.hash)['status'] == 0:
                     log.error(f'admin_rebalance_funds transaction {rebalance.hash.hex()} failed')
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return rebalance
 
     # approveStrategist(strategist (address))
     def approve_strategist(self, strategist, nonce=None, gas=3000000, gas_price=None):
         """this function approves a strategist to use the aid contract instance
 
         :param strategist: the address of the strategist to approve
@@ -890,15 +897,15 @@
         :rtype: dict, None
         """
 
         if nonce is None:
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
-        
+
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
         txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
 
         try:
             approve = self.contract.functions.approveStrategist(strategist).build_transaction(txn)
@@ -922,15 +929,15 @@
                 if self.w3.eth.wait_for_transaction_receipt(approve.hash)['status'] == 0:
                     log.error(f'approve_strategist transaction {approve.hash.hex()} failed')
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return approve
 
     # batchMarketMakingTrades(tokenPairs (address[2]), askNumerators (uint256[]), askDenominators (uint256[]), bidNumerators (uint256[]), bidDenominators (uint256[]))
     def batch_market_making_trades(self, token_pairs, ask_numerators, ask_denominators, bid_numerators, bid_denominators, nonce=None, gas=3000000, gas_price=None):
         """this function executes a batch of market making trades on the RubiconMarket
 
         :param token_pairs: the token pairs to trade [token0, token1]
@@ -953,15 +960,15 @@
         :rtype: dict, None
         """
 
         if nonce is None:
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
-        
+
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
         txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
 
         try:
             batch = self.contract.functions.batchMarketMakingTrades(token_pairs, ask_numerators, ask_denominators, bid_numerators, bid_denominators).build_transaction(txn)
@@ -973,17 +980,17 @@
                 if self.w3.eth.wait_for_transaction_receipt(batch.hash)['status'] == 0:
                     log.error(f'batch_market_making_trades transaction {batch.hash.hex()} failed')
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return batch
-    
+
     # batchRequoteAllOffers(tokenPair (address[2]), askNumerators (uint256[]), askDenominators (uint256[]), bidNumerators (uint256[]), bidDenominators (uint256[]))
     def batch_requote_all_offers(self, token_pair, ask_numerators, ask_denominators, bid_numerators, bid_denominators, nonce=None, gas=3000000, gas_price=None):
         """this function executes a batch requote while clearing all offers the strategist has on the RubiconMarket
 
         :param token_pair: the token pair to trade [token0, token1]
         :type token_pair: list
         :param ask_numerators: the numerators of the ask prices
@@ -1004,15 +1011,15 @@
         :rtype: dict, None
         """
 
         if nonce is None:
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
-        
+
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
         txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
 
         try:
             batch = self.contract.functions.batchRequoteAllOffers(token_pair, ask_numerators, ask_denominators, bid_numerators, bid_denominators).build_transaction(txn)
@@ -1024,15 +1031,15 @@
                 if self.w3.eth.wait_for_transaction_receipt(batch.hash)['status'] == 0:
                     log.error(f'batch_requote_all_offers transaction {batch.hash.hex()} failed')
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return batch
 
     # batchRequoteOffers(ids (uint256[]), tokenPair (address[2]), askNumerators (uint256[]), askDenominators (uint256[]), bidNumerators (uint256[]), bidDenominators (uint256[]))
     def batch_requote_offers(self, ids, token_pair, ask_numerators, ask_denominators, bid_numerators, bid_denominators, nonce=None, gas=3000000, gas_price=None):
         """this function executes a batch requote of all offers that are provided in the ids array
         
         :param ids: the ids of the offers to requote
@@ -1057,15 +1064,15 @@
         :rtype: dict, None
         """
 
         if nonce is None:
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
-        
+
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
         txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
 
         try:
             batch = self.contract.functions.batchRequoteOffers(ids, token_pair, ask_numerators, ask_denominators, bid_numerators, bid_denominators).build_transaction(txn)
@@ -1077,15 +1084,15 @@
                 if self.w3.eth.wait_for_transaction_receipt(batch.hash)['status'] == 0:
                     log.error(f'batch_requote_offers transaction {batch.hash.hex()} failed')
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return batch
 
     # placeMarketMakingTrades(tokenPair (address[2]), askNumerator (uint256), askDenominator (uint256), bidNumerator (uint256), bidDenominator (uint256))
     # aid.batch_market_making_trades([weth.address, usdc.address], [the amount of the asset you will sell], [the amount of the quote you will receive], [the amount of quote you will pay], [the amount of asset you would receive])
     def place_market_making_trades(self, token_pair, ask_numerator, ask_denominator, bid_numerator, bid_denominator, nonce=None, gas=3000000, gas_price=None):
         """this function executes a market making trade on the RubiconMarket
         
@@ -1109,35 +1116,35 @@
         :rtype: dict, None
         """
 
         if nonce is None:
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
-        
+
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
         txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
 
-        try: 
+        try:
             trade = self.contract.functions.placeMarketMakingTrades(token_pair, ask_numerator, ask_denominator, bid_numerator, bid_denominator).build_transaction(txn)
             trade = self.w3.eth.account.sign_transaction(trade, self.key)
             self.w3.eth.send_raw_transaction(trade.rawTransaction)
 
             # if a user is not providing a nonce, wait for the transaction to either be confirmed or rejected before continuing
             if nonce is None:
                 if self.w3.eth.wait_for_transaction_receipt(trade.hash)['status'] == 0:
                     log.error(f'place_market_making_trades transaction {trade.hash.hex()} failed')
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return trade
 
     # removeStrategist(strategist (address))
     def remove_strategist(self, strategist, nonce=None, gas=3000000, gas_price=None):
         """this function removes a strategist from the approved strategist list on the market aid contract
         
         :param strategist: the address of the strategist to remove
@@ -1220,15 +1227,15 @@
         if nonce is None:
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
 
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
-        
+
         txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
 
         try:
             requote = self.contract.functions.requote(id, token_pair, ask_numerator, ask_denominator, bid_numerator, bid_denominator).build_transaction(txn)
             requote = self.w3.eth.account.sign_transaction(requote, self.key)
             self.w3.eth.send_raw_transaction(requote.rawTransaction)
 
@@ -1278,15 +1285,15 @@
                 if self.w3.eth.wait_for_transaction_receipt(scrub.hash)['status'] == 0:
                     log.error(f'scrub_strategist_trade transaction {scrub.hash.hex()} failed')
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return scrub
 
     # scrubStrategistTrades(ids (uint256[]))
     def scrub_strategist_trades(self, ids, nonce=None, gas=3000000, gas_price=None):
         """this function scrubs a list of strategist trades from the RubiconMarket contract
 
         :param ids: the ids of the trades to scrub
@@ -1301,15 +1308,15 @@
         :rtype: dict, None
         """
 
         if nonce is None:
             txn_nonce = self.w3.eth.get_transaction_count(self.wallet)
         else:
             txn_nonce = nonce
-        
+
         if gas_price is None:
             gas_price = self.w3.eth.gas_price
 
         txn = {'chainId': self.chain, 'gas' : gas, 'gasPrice': gas_price, 'nonce': txn_nonce}
 
         try:
             scrub = self.contract.functions.scrubStrategistTrades(ids).build_transaction(txn)
@@ -1321,9 +1328,9 @@
                 if self.w3.eth.wait_for_transaction_receipt(scrub.hash)['status'] == 0:
                     log.error(f'scrub_strategist_trades transaction {scrub.hash.hex()} failed')
                     raise SystemExit()
 
         except Exception as e:
             log.error(e, exc_info=True)
             return None
-        
+
         return scrub
```

### Comparing `rubi-1.3.2/rubi/data/data.py` & `rubi-2.0.0/rubi/data/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from subgrounds import Subgrounds
 from rubi.data.sources.aid import AidData, SuperAidData
 from rubi.data.sources.market import MarketData
 from rubi.data.sources.helper import Gas, Price, networks 
 from rubi.data.processing.user import User, SuperUser
 from rubi.data.processing.aid import AidProcessing
 
+# TODO this needs significant love.
 class Data: 
     """this class acts as the main access point to a variety of data and data tooling for the Rubicon protocol. it acts as a data processing layer built using the subgrounds library and the subgraphs maintained at the follwing repo: https://github.com/RubiconDeFi/rubi-subgraphs
     """
 
     def __init__(self, super=False): 
         """constructor method. creates a subgrounds object that is then used to initialize a variety of data sources and tooling
```

### Comparing `rubi-1.3.2/rubi/data/processing/README.md` & `rubi-2.0.0/rubi/data/processing/README.md`

 * *Files identical despite different names*

### Comparing `rubi-1.3.2/rubi/data/processing/aid.py` & `rubi-2.0.0/rubi/data/processing/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.2/rubi/data/processing/helper/processing.py` & `rubi-2.0.0/rubi/data/processing/helper/processing.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.2/rubi/data/processing/user.py` & `rubi-2.0.0/rubi/data/processing/user.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.2/rubi/data/sources/aid.py` & `rubi-2.0.0/rubi/data/sources/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.2/rubi/data/sources/helper/README.md` & `rubi-2.0.0/rubi/data/sources/helper/README.md`

 * *Files identical despite different names*

### Comparing `rubi-1.3.2/rubi/data/sources/helper/gas.py` & `rubi-2.0.0/rubi/data/sources/helper/gas.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.2/rubi/data/sources/helper/price.py` & `rubi-2.0.0/rubi/data/sources/helper/price.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.2/rubi/data/sources/helper/rolodex.py` & `rubi-2.0.0/rubi/data/sources/helper/rolodex.py`

 * *Files identical despite different names*

### Comparing `rubi-1.3.2/rubi/data/sources/market.py` & `rubi-2.0.0/rubi/data/sources/market.py`

 * *Files identical despite different names*

