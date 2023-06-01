# Comparing `tmp/rubi-2.0.1.tar.gz` & `tmp/rubi-2.0.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.0.1.tar", max compression
+gzip compressed data, was "rubi-2.0.2b1.tar", max compression
```

## Comparing `rubi-2.0.1.tar` & `rubi-2.0.2b1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.1/LICENSE
--rw-r--r--   0        0        0     2757 2023-06-01 18:59:40.461664 rubi-2.0.1/README.md
--rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.1/network_config/ERC20.json
--rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.1/network_config/README.md
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.1/network_config/abitrum_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.1/network_config/abitrum_goerli/abis/router.json
--rw-r--r--   0        0        0      645 2023-06-01 18:59:40.465341 rubi-2.0.1/network_config/abitrum_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.1/network_config/optimism/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.1/network_config/optimism/abis/router.json
--rw-r--r--   0        0        0      664 2023-06-01 18:59:40.468200 rubi-2.0.1/network_config/optimism/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.1/network_config/optimism_goerli/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.1/network_config/optimism_goerli/abis/router.json
--rw-r--r--   0        0        0      518 2023-06-01 18:59:40.468648 rubi-2.0.1/network_config/optimism_goerli/network.yaml
--rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.1/network_config/polygon_mumbai/abis/market.json
--rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.1/network_config/polygon_mumbai/abis/router.json
--rw-r--r--   0        0        0      631 2023-06-01 18:59:40.469759 rubi-2.0.1/network_config/polygon_mumbai/network.yaml
--rw-r--r--   0        0        0      745 2023-06-01 19:24:45.453186 rubi-2.0.1/pyproject.toml
--rw-r--r--   0        0        0       96 2023-06-01 18:59:40.472105 rubi-2.0.1/rubi/__init__.py
--rw-r--r--   0        0        0    27357 2023-06-01 18:59:40.472316 rubi-2.0.1/rubi/client.py
--rw-r--r--   0        0        0      154 2023-06-01 18:59:40.472446 rubi-2.0.1/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.1/rubi/contracts/aid.py
--rw-r--r--   0        0        0    11606 2023-06-01 18:59:40.472881 rubi-2.0.1/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0    16248 2023-06-01 18:59:40.473031 rubi-2.0.1/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24182 2023-06-01 18:59:40.473250 rubi-2.0.1/rubi/contracts/market.py
--rw-r--r--   0        0        0    14668 2023-06-01 18:59:40.473453 rubi-2.0.1/rubi/contracts/router.py
--rw-r--r--   0        0        0       22 2023-06-01 18:59:40.473528 rubi-2.0.1/rubi/contracts/types/__init__.py
--rw-r--r--   0        0        0    16011 2023-06-01 18:59:40.473629 rubi-2.0.1/rubi/contracts/types/events.py
--rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.1/rubi/data/README.md
--rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.1/rubi/data/__init__.py
--rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.1/rubi/data/data.py
--rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.1/rubi/data/processing/README.md
--rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.1/rubi/data/processing/__init__.py
--rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.1/rubi/data/processing/aid.py
--rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.1/rubi/data/processing/helper/__init__.py
--rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.1/rubi/data/processing/helper/processing.py
--rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.1/rubi/data/processing/user.py
--rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.1/rubi/data/sources/__init__.py
--rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.1/rubi/data/sources/aid.py
--rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.1/rubi/data/sources/helper/README.md
--rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.1/rubi/data/sources/helper/__init__.py
--rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.1/rubi/data/sources/helper/gas.py
--rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.1/rubi/data/sources/helper/price.py
--rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.1/rubi/data/sources/helper/rolodex.py
--rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.1/rubi/data/sources/market.py
--rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.1/rubi/network/__init__.py
--rw-r--r--   0        0        0     7589 2023-06-01 18:59:40.474413 rubi-2.0.1/rubi/network/network.py
--rw-r--r--   0        0        0       66 2023-06-01 18:59:40.474481 rubi-2.0.1/rubi/types/__init__.py
--rw-r--r--   0        0        0    12515 2023-06-01 18:59:40.474581 rubi-2.0.1/rubi/types/order.py
--rw-r--r--   0        0        0     5719 2023-06-01 18:59:40.474684 rubi-2.0.1/rubi/types/orderbook.py
--rw-r--r--   0        0        0     2707 2023-06-01 18:59:40.474750 rubi-2.0.1/rubi/types/pair.py
--rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 rubi-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.2b1/LICENSE
+-rw-r--r--   0        0        0     2757 2023-06-01 18:59:40.461664 rubi-2.0.2b1/README.md
+-rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.2b1/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.2b1/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.2b1/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.2b1/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      645 2023-06-01 18:59:40.465341 rubi-2.0.2b1/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.2b1/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.2b1/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      664 2023-06-01 18:59:40.468200 rubi-2.0.2b1/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.2b1/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.2b1/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      518 2023-06-01 18:59:40.468648 rubi-2.0.2b1/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.2b1/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.2b1/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      631 2023-06-01 18:59:40.469759 rubi-2.0.2b1/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0      747 2023-06-01 21:23:08.244797 rubi-2.0.2b1/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-06-01 18:59:40.472105 rubi-2.0.2b1/rubi/__init__.py
+-rw-r--r--   0        0        0    27357 2023-06-01 18:59:40.472316 rubi-2.0.2b1/rubi/client.py
+-rw-r--r--   0        0        0      154 2023-06-01 18:59:40.472446 rubi-2.0.2b1/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.2b1/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    11606 2023-06-01 18:59:40.472881 rubi-2.0.2b1/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0    16235 2023-06-01 21:19:10.962516 rubi-2.0.2b1/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24182 2023-06-01 18:59:40.473250 rubi-2.0.2b1/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14668 2023-06-01 18:59:40.473453 rubi-2.0.2b1/rubi/contracts/router.py
+-rw-r--r--   0        0        0       22 2023-06-01 18:59:40.473528 rubi-2.0.2b1/rubi/contracts/types/__init__.py
+-rw-r--r--   0        0        0    16011 2023-06-01 18:59:40.473629 rubi-2.0.2b1/rubi/contracts/types/events.py
+-rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.2b1/rubi/data/README.md
+-rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.2b1/rubi/data/__init__.py
+-rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.2b1/rubi/data/data.py
+-rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.2b1/rubi/data/processing/README.md
+-rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.2b1/rubi/data/processing/__init__.py
+-rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.2b1/rubi/data/processing/aid.py
+-rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.2b1/rubi/data/processing/helper/__init__.py
+-rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.2b1/rubi/data/processing/helper/processing.py
+-rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.2b1/rubi/data/processing/user.py
+-rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.2b1/rubi/data/sources/__init__.py
+-rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.2b1/rubi/data/sources/aid.py
+-rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.2b1/rubi/data/sources/helper/README.md
+-rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.2b1/rubi/data/sources/helper/__init__.py
+-rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.2b1/rubi/data/sources/helper/gas.py
+-rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.2b1/rubi/data/sources/helper/price.py
+-rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.2b1/rubi/data/sources/helper/rolodex.py
+-rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.2b1/rubi/data/sources/market.py
+-rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.2b1/rubi/network/__init__.py
+-rw-r--r--   0        0        0     7834 2023-06-01 21:11:43.341852 rubi-2.0.2b1/rubi/network/network.py
+-rw-r--r--   0        0        0       66 2023-06-01 18:59:40.474481 rubi-2.0.2b1/rubi/types/__init__.py
+-rw-r--r--   0        0        0    12515 2023-06-01 18:59:40.474581 rubi-2.0.2b1/rubi/types/order.py
+-rw-r--r--   0        0        0     5719 2023-06-01 18:59:40.474684 rubi-2.0.2b1/rubi/types/orderbook.py
+-rw-r--r--   0        0        0     2707 2023-06-01 18:59:40.474750 rubi-2.0.2b1/rubi/types/pair.py
+-rw-r--r--   0        0        0     3547 1970-01-01 00:00:00.000000 rubi-2.0.2b1/PKG-INFO
```

### Comparing `rubi-2.0.1/LICENSE` & `rubi-2.0.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/README.md` & `rubi-2.0.2b1/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/ERC20.json` & `rubi-2.0.2b1/network_config/ERC20.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/README.md` & `rubi-2.0.2b1/network_config/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/abitrum_goerli/abis/market.json` & `rubi-2.0.2b1/network_config/abitrum_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/abitrum_goerli/abis/router.json` & `rubi-2.0.2b1/network_config/abitrum_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/abitrum_goerli/network.yaml` & `rubi-2.0.2b1/network_config/abitrum_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/optimism/abis/market.json` & `rubi-2.0.2b1/network_config/optimism/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/optimism/abis/router.json` & `rubi-2.0.2b1/network_config/optimism/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/optimism/network.yaml` & `rubi-2.0.2b1/network_config/optimism/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/optimism_goerli/abis/market.json` & `rubi-2.0.2b1/network_config/optimism_goerli/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/optimism_goerli/abis/router.json` & `rubi-2.0.2b1/network_config/optimism_goerli/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/optimism_goerli/network.yaml` & `rubi-2.0.2b1/network_config/optimism_goerli/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/polygon_mumbai/abis/market.json` & `rubi-2.0.2b1/network_config/polygon_mumbai/abis/market.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/polygon_mumbai/abis/router.json` & `rubi-2.0.2b1/network_config/polygon_mumbai/abis/router.json`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/network_config/polygon_mumbai/network.yaml` & `rubi-2.0.2b1/network_config/polygon_mumbai/network.yaml`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/pyproject.toml` & `rubi-2.0.2b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rubi"
-version = "2.0.1"
+version = "2.0.2b1"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
 include = ["network_config/**"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `rubi-2.0.1/rubi/client.py` & `rubi-2.0.2b1/rubi/client.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/contracts/aid.py` & `rubi-2.0.2b1/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/contracts/base_contract.py` & `rubi-2.0.2b1/rubi/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/contracts/erc20.py` & `rubi-2.0.2b1/rubi/contracts/erc20.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 from _decimal import Decimal
 from typing import Optional
+from pkg_resources import resource_stream
 
 from eth_typing import ChecksumAddress
 from web3 import Web3
 from web3.contract import Contract
 from web3.types import ABI
 
 from rubi.contracts.base_contract import BaseContract
@@ -71,17 +72,15 @@
 
         if network.token_addresses[name] is None:
             raise Exception(f"{name} in not a valid token according to the network config.")
 
         abi: ABI
 
         try:
-            path = f"{os.path.dirname(os.path.abspath(__file__))}/../../network_config/ERC20.json"
-
-            with open(path) as f:
+            with resource_stream('rubi', "../network_config/ERC20.json") as f:
                 abi = json.load(f)
 
         except FileNotFoundError:
             raise Exception("ERC20.json abi not found. this file should in the network_config folder")
 
         return cls.from_address_and_abi(
             w3=network.w3,
```

### Comparing `rubi-2.0.1/rubi/contracts/market.py` & `rubi-2.0.2b1/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/contracts/router.py` & `rubi-2.0.2b1/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/contracts/types/events.py` & `rubi-2.0.2b1/rubi/contracts/types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/data.py` & `rubi-2.0.2b1/rubi/data/data.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/processing/README.md` & `rubi-2.0.2b1/rubi/data/processing/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/processing/aid.py` & `rubi-2.0.2b1/rubi/data/processing/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/processing/helper/processing.py` & `rubi-2.0.2b1/rubi/data/processing/helper/processing.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/processing/user.py` & `rubi-2.0.2b1/rubi/data/processing/user.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/sources/aid.py` & `rubi-2.0.2b1/rubi/data/sources/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/sources/helper/README.md` & `rubi-2.0.2b1/rubi/data/sources/helper/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/sources/helper/gas.py` & `rubi-2.0.2b1/rubi/data/sources/helper/gas.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/sources/helper/price.py` & `rubi-2.0.2b1/rubi/data/sources/helper/price.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/sources/helper/rolodex.py` & `rubi-2.0.2b1/rubi/data/sources/helper/rolodex.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/data/sources/market.py` & `rubi-2.0.2b1/rubi/data/sources/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/network/network.py` & `rubi-2.0.2b1/rubi/network/network.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 import os
 from enum import Enum
 from typing import Optional
+from pkg_resources import resource_exists, resource_stream
 
 import yaml
 from eth_typing import ChecksumAddress
 from web3 import Web3
 
 
 class NetworkId(Enum):
@@ -111,23 +112,23 @@
         :rtype: Network
         :raises Exception: If no network configuration file is found for the specified network name.
         """
         w3 = Web3(Web3.HTTPProvider(http_node_url))
 
         network_name = NetworkId(w3.eth.chain_id).name.lower()
 
-        try:
-            path = f"{os.path.dirname(os.path.abspath(__file__))}/../../network_config/{network_name}"
-
-            with open(f"{path}/network.yaml") as f:
-                network_data = yaml.safe_load(f)
-                return cls(path=path, w3=w3, custom_token_addresses_file=custom_token_addresses_file, **network_data)
-        except FileNotFoundError:
+        resource_path = f"../network_config/{network_name}/network.yaml"
+        if not resource_exists('rubi', resource_path):
             raise Exception(f"no network config found for {network_name}, there should be a corresponding folder in "
                             f"the network_config directory")
+        with resource_stream('rubi', resource_path) as f:
+            network_data = yaml.safe_load(f)
+            print(f"loaded network config for {network_name} from {resource_path}")
+
+        return cls(path=resource_path, w3=w3, custom_token_addresses_file=custom_token_addresses_file, **network_data)
 
     def __repr__(self):
         items = ("{}={!r}".format(k, self.__dict__[k]) for k in self.__dict__)
         return "{}({})".format(type(self).__name__, ", ".join(items))
 
 
 class RubiconContracts:
@@ -170,15 +171,18 @@
         :param name: The name of the contract.
         :type name: str
         :param address: The address of the contract.
         :type address: str
         """
         self.address = w3.to_checksum_address(address)
 
+        base_dir_path = os.path.dirname(path)
+        file_path = os.path.join(base_dir_path, "abis", f"{name}.json")
+
         try:
-            with open(f"{path}/abis/{name}.json") as f:
+            with resource_stream('rubi', file_path) as f:
                 self.abi = json.load(f)
         except FileNotFoundError:
             self.abi = None
 
     def __repr__(self):
         return f"{type(self).__name__}(address='{self.address}', abi='{'Loaded' if self.abi is not None else 'None'}')"
```

### Comparing `rubi-2.0.1/rubi/types/order.py` & `rubi-2.0.2b1/rubi/types/order.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/types/orderbook.py` & `rubi-2.0.2b1/rubi/types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/rubi/types/pair.py` & `rubi-2.0.2b1/rubi/types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.1/PKG-INFO` & `rubi-2.0.2b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.0.1
+Version: 2.0.2b1
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

