# Comparing `tmp/rubi-2.0.0.tar.gz` & `tmp/rubi-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rubi-2.0.0.tar", max compression
+gzip compressed data, was "rubi-2.0.1.tar", max compression
```

## Comparing `rubi-2.0.0.tar` & `rubi-2.0.1.tar`

### file list

```diff
@@ -1,37 +1,51 @@
--rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.0/LICENSE
--rw-r--r--   0        0        0     2757 2023-06-01 18:59:40.461664 rubi-2.0.0/README.md
--rw-r--r--   0        0        0      713 2023-06-01 18:59:40.471784 rubi-2.0.0/pyproject.toml
--rw-r--r--   0        0        0       96 2023-06-01 18:59:40.472105 rubi-2.0.0/rubi/__init__.py
--rw-r--r--   0        0        0    27357 2023-06-01 18:59:40.472316 rubi-2.0.0/rubi/client.py
--rw-r--r--   0        0        0      154 2023-06-01 18:59:40.472446 rubi-2.0.0/rubi/contracts/__init__.py
--rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.0/rubi/contracts/aid.py
--rw-r--r--   0        0        0    11606 2023-06-01 18:59:40.472881 rubi-2.0.0/rubi/contracts/base_contract.py
--rw-r--r--   0        0        0    16248 2023-06-01 18:59:40.473031 rubi-2.0.0/rubi/contracts/erc20.py
--rw-r--r--   0        0        0    24182 2023-06-01 18:59:40.473250 rubi-2.0.0/rubi/contracts/market.py
--rw-r--r--   0        0        0    14668 2023-06-01 18:59:40.473453 rubi-2.0.0/rubi/contracts/router.py
--rw-r--r--   0        0        0       22 2023-06-01 18:59:40.473528 rubi-2.0.0/rubi/contracts/types/__init__.py
--rw-r--r--   0        0        0    16011 2023-06-01 18:59:40.473629 rubi-2.0.0/rubi/contracts/types/events.py
--rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.0/rubi/data/README.md
--rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.0/rubi/data/__init__.py
--rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.0/rubi/data/data.py
--rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.0/rubi/data/processing/README.md
--rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.0/rubi/data/processing/__init__.py
--rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.0/rubi/data/processing/aid.py
--rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.0/rubi/data/processing/helper/__init__.py
--rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.0/rubi/data/processing/helper/processing.py
--rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.0/rubi/data/processing/user.py
--rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.0/rubi/data/sources/__init__.py
--rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.0/rubi/data/sources/aid.py
--rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.0/rubi/data/sources/helper/README.md
--rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.0/rubi/data/sources/helper/__init__.py
--rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.0/rubi/data/sources/helper/gas.py
--rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.0/rubi/data/sources/helper/price.py
--rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.0/rubi/data/sources/helper/rolodex.py
--rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.0/rubi/data/sources/market.py
--rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.0/rubi/network/__init__.py
--rw-r--r--   0        0        0     7589 2023-06-01 18:59:40.474413 rubi-2.0.0/rubi/network/network.py
--rw-r--r--   0        0        0       66 2023-06-01 18:59:40.474481 rubi-2.0.0/rubi/types/__init__.py
--rw-r--r--   0        0        0    12515 2023-06-01 18:59:40.474581 rubi-2.0.0/rubi/types/order.py
--rw-r--r--   0        0        0     5719 2023-06-01 18:59:40.474684 rubi-2.0.0/rubi/types/orderbook.py
--rw-r--r--   0        0        0     2707 2023-06-01 18:59:40.474750 rubi-2.0.0/rubi/types/pair.py
--rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 rubi-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-02-09 17:21:21.757346 rubi-2.0.1/LICENSE
+-rw-r--r--   0        0        0     2757 2023-06-01 18:59:40.461664 rubi-2.0.1/README.md
+-rw-r--r--   0        0        0     6735 2023-06-01 18:59:40.464065 rubi-2.0.1/network_config/ERC20.json
+-rw-r--r--   0        0        0     1920 2023-06-01 18:59:40.464275 rubi-2.0.1/network_config/README.md
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.464692 rubi-2.0.1/network_config/abitrum_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.464994 rubi-2.0.1/network_config/abitrum_goerli/abis/router.json
+-rw-r--r--   0        0        0      645 2023-06-01 18:59:40.465341 rubi-2.0.1/network_config/abitrum_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.465638 rubi-2.0.1/network_config/optimism/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.467925 rubi-2.0.1/network_config/optimism/abis/router.json
+-rw-r--r--   0        0        0      664 2023-06-01 18:59:40.468200 rubi-2.0.1/network_config/optimism/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468441 rubi-2.0.1/network_config/optimism_goerli/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.468572 rubi-2.0.1/network_config/optimism_goerli/abis/router.json
+-rw-r--r--   0        0        0      518 2023-06-01 18:59:40.468648 rubi-2.0.1/network_config/optimism_goerli/network.yaml
+-rw-r--r--   0        0        0    32732 2023-06-01 18:59:40.468889 rubi-2.0.1/network_config/polygon_mumbai/abis/market.json
+-rw-r--r--   0        0        0    15157 2023-06-01 18:59:40.469043 rubi-2.0.1/network_config/polygon_mumbai/abis/router.json
+-rw-r--r--   0        0        0      631 2023-06-01 18:59:40.469759 rubi-2.0.1/network_config/polygon_mumbai/network.yaml
+-rw-r--r--   0        0        0      745 2023-06-01 19:24:45.453186 rubi-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-06-01 18:59:40.472105 rubi-2.0.1/rubi/__init__.py
+-rw-r--r--   0        0        0    27357 2023-06-01 18:59:40.472316 rubi-2.0.1/rubi/client.py
+-rw-r--r--   0        0        0      154 2023-06-01 18:59:40.472446 rubi-2.0.1/rubi/contracts/__init__.py
+-rw-r--r--   0        0        0    61077 2023-06-01 18:59:40.472708 rubi-2.0.1/rubi/contracts/aid.py
+-rw-r--r--   0        0        0    11606 2023-06-01 18:59:40.472881 rubi-2.0.1/rubi/contracts/base_contract.py
+-rw-r--r--   0        0        0    16248 2023-06-01 18:59:40.473031 rubi-2.0.1/rubi/contracts/erc20.py
+-rw-r--r--   0        0        0    24182 2023-06-01 18:59:40.473250 rubi-2.0.1/rubi/contracts/market.py
+-rw-r--r--   0        0        0    14668 2023-06-01 18:59:40.473453 rubi-2.0.1/rubi/contracts/router.py
+-rw-r--r--   0        0        0       22 2023-06-01 18:59:40.473528 rubi-2.0.1/rubi/contracts/types/__init__.py
+-rw-r--r--   0        0        0    16011 2023-06-01 18:59:40.473629 rubi-2.0.1/rubi/contracts/types/events.py
+-rw-r--r--   0        0        0      257 2023-06-01 18:59:40.473763 rubi-2.0.1/rubi/data/README.md
+-rw-r--r--   0        0        0       33 2023-02-14 16:34:53.717274 rubi-2.0.1/rubi/data/__init__.py
+-rw-r--r--   0        0        0     3968 2023-06-01 18:59:40.473880 rubi-2.0.1/rubi/data/data.py
+-rw-r--r--   0        0        0     1198 2023-02-14 16:34:53.717485 rubi-2.0.1/rubi/data/processing/README.md
+-rw-r--r--   0        0        0       64 2023-02-14 16:34:53.717551 rubi-2.0.1/rubi/data/processing/__init__.py
+-rw-r--r--   0        0        0    20226 2023-03-28 22:32:44.963776 rubi-2.0.1/rubi/data/processing/aid.py
+-rw-r--r--   0        0        0       31 2023-02-14 16:34:53.717742 rubi-2.0.1/rubi/data/processing/helper/__init__.py
+-rw-r--r--   0        0        0     2292 2023-02-14 16:34:53.717833 rubi-2.0.1/rubi/data/processing/helper/processing.py
+-rw-r--r--   0        0        0    10226 2023-02-14 16:34:53.717931 rubi-2.0.1/rubi/data/processing/user.py
+-rw-r--r--   0        0        0       69 2023-02-14 16:34:53.718073 rubi-2.0.1/rubi/data/sources/__init__.py
+-rw-r--r--   0        0        0    21161 2023-03-28 22:32:44.964336 rubi-2.0.1/rubi/data/sources/aid.py
+-rw-r--r--   0        0        0     1194 2023-02-14 16:34:53.718302 rubi-2.0.1/rubi/data/sources/helper/README.md
+-rw-r--r--   0        0        0       76 2023-02-14 16:34:53.718369 rubi-2.0.1/rubi/data/sources/helper/__init__.py
+-rw-r--r--   0        0        0    12589 2023-02-27 02:08:49.086543 rubi-2.0.1/rubi/data/sources/helper/gas.py
+-rw-r--r--   0        0        0    15373 2023-02-14 16:34:53.718597 rubi-2.0.1/rubi/data/sources/helper/price.py
+-rw-r--r--   0        0        0     7319 2023-02-14 16:34:53.718699 rubi-2.0.1/rubi/data/sources/helper/rolodex.py
+-rw-r--r--   0        0        0    22425 2023-02-14 16:34:53.718888 rubi-2.0.1/rubi/data/sources/market.py
+-rw-r--r--   0        0        0       72 2023-06-01 18:59:40.474197 rubi-2.0.1/rubi/network/__init__.py
+-rw-r--r--   0        0        0     7589 2023-06-01 18:59:40.474413 rubi-2.0.1/rubi/network/network.py
+-rw-r--r--   0        0        0       66 2023-06-01 18:59:40.474481 rubi-2.0.1/rubi/types/__init__.py
+-rw-r--r--   0        0        0    12515 2023-06-01 18:59:40.474581 rubi-2.0.1/rubi/types/order.py
+-rw-r--r--   0        0        0     5719 2023-06-01 18:59:40.474684 rubi-2.0.1/rubi/types/orderbook.py
+-rw-r--r--   0        0        0     2707 2023-06-01 18:59:40.474750 rubi-2.0.1/rubi/types/pair.py
+-rw-r--r--   0        0        0     3545 1970-01-01 00:00:00.000000 rubi-2.0.1/PKG-INFO
```

### Comparing `rubi-2.0.0/LICENSE` & `rubi-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/README.md` & `rubi-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/pyproject.toml` & `rubi-2.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "rubi"
-version = "2.0.0"
+version = "2.0.1"
 description = "A python SDK for the Rubicon Protocol"
 authors = ["denver <denver@rubicon.finance>", "adam <adam@rubicon.finance>"]
 readme = "README.md"
+include = ["network_config/**"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sphinx = "7.0.1"
 web3 = "6.4.0"
 hexbytes = "0.3.0"
 attributedict = "0.3.0"
```

### Comparing `rubi-2.0.0/rubi/client.py` & `rubi-2.0.1/rubi/client.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/contracts/aid.py` & `rubi-2.0.1/rubi/contracts/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/contracts/base_contract.py` & `rubi-2.0.1/rubi/contracts/base_contract.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/contracts/erc20.py` & `rubi-2.0.1/rubi/contracts/erc20.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/contracts/market.py` & `rubi-2.0.1/rubi/contracts/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/contracts/router.py` & `rubi-2.0.1/rubi/contracts/router.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/contracts/types/events.py` & `rubi-2.0.1/rubi/contracts/types/events.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/data.py` & `rubi-2.0.1/rubi/data/data.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/processing/README.md` & `rubi-2.0.1/rubi/data/processing/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/processing/aid.py` & `rubi-2.0.1/rubi/data/processing/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/processing/helper/processing.py` & `rubi-2.0.1/rubi/data/processing/helper/processing.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/processing/user.py` & `rubi-2.0.1/rubi/data/processing/user.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/sources/aid.py` & `rubi-2.0.1/rubi/data/sources/aid.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/sources/helper/README.md` & `rubi-2.0.1/rubi/data/sources/helper/README.md`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/sources/helper/gas.py` & `rubi-2.0.1/rubi/data/sources/helper/gas.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/sources/helper/price.py` & `rubi-2.0.1/rubi/data/sources/helper/price.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/sources/helper/rolodex.py` & `rubi-2.0.1/rubi/data/sources/helper/rolodex.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/data/sources/market.py` & `rubi-2.0.1/rubi/data/sources/market.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/network/network.py` & `rubi-2.0.1/rubi/network/network.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/types/order.py` & `rubi-2.0.1/rubi/types/order.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/types/orderbook.py` & `rubi-2.0.1/rubi/types/orderbook.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/rubi/types/pair.py` & `rubi-2.0.1/rubi/types/pair.py`

 * *Files identical despite different names*

### Comparing `rubi-2.0.0/PKG-INFO` & `rubi-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rubi
-Version: 2.0.0
+Version: 2.0.1
 Summary: A python SDK for the Rubicon Protocol
 Author: denver
 Author-email: denver@rubicon.finance
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

