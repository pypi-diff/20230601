# Comparing `tmp/starknet_devnet-0.5.2.tar.gz` & `tmp/starknet_devnet-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starknet_devnet-0.5.2.tar", max compression
+gzip compressed data, was "starknet_devnet-0.5.3.tar", max compression
```

## Comparing `starknet_devnet-0.5.2.tar` & `starknet_devnet-0.5.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1067 2023-05-19 17:45:57.572392 starknet_devnet-0.5.2/LICENSE
--rw-r--r--   0        0        0     1054 2023-05-19 17:45:57.572392 starknet_devnet-0.5.2/README.md
--rw-r--r--   0        0        0     1820 2023-05-19 17:45:57.584392 starknet_devnet-0.5.2/pyproject.toml
--rw-r--r--   0        0        0   208485 2023-05-19 17:45:57.588392 starknet_devnet-0.5.2/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
--rw-r--r--   0        0        0    32739 2023-05-19 17:45:57.588392 starknet_devnet-0.5.2/starknet_devnet/MockStarknetMessaging.json
--rw-r--r--   0        0        0    35645 2023-05-19 17:45:57.588392 starknet_devnet-0.5.2/starknet_devnet/UDC_OZ_0.5.0.json
--rw-r--r--   0        0        0     2958 2023-05-19 17:45:57.588392 starknet_devnet-0.5.2/starknet_devnet/__init__.py
--rw-r--r--   0        0        0     2130 2023-05-19 17:45:57.588392 starknet_devnet-0.5.2/starknet_devnet/account.py
--rw-r--r--   0        0        0     3784 2023-05-19 17:45:57.588392 starknet_devnet-0.5.2/starknet_devnet/account_util.py
--rw-r--r--   0        0        0     2692 2023-05-19 17:45:57.588392 starknet_devnet-0.5.2/starknet_devnet/accounts.py
--rw-r--r--   0        0        0   118818 2023-05-19 17:45:57.588392 starknet_devnet-0.5.2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
--rw-r--r--   0        0        0     1784 2023-05-19 17:45:57.588392 starknet_devnet-0.5.2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
--rw-r--r--   0        0        0     1866 2023-05-19 17:45:57.588392 starknet_devnet-0.5.2/starknet_devnet/block_info_generator.py
--rw-r--r--   0        0        0    12337 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blocks.py
--rw-r--r--   0        0        0        0 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/__init__.py
--rw-r--r--   0        0        0     7523 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/base.py
--rw-r--r--   0        0        0    14072 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/feeder_gateway.py
--rw-r--r--   0        0        0     2228 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/gateway.py
--rw-r--r--   0        0        0     3959 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/postman.py
--rw-r--r--   0        0        0        0 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/__init__.py
--rw-r--r--   0        0        0     2138 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/blocks.py
--rw-r--r--   0        0        0     2136 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/call.py
--rw-r--r--   0        0        0     2195 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/classes.py
--rw-r--r--   0        0        0     6135 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/misc.py
--rw-r--r--   0        0        0     4878 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/routes.py
--rw-r--r--   0        0        0    95612 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/rpc_spec.py
--rw-r--r--   0        0        0     5804 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/rpc_spec_write.py
--rw-r--r--   0        0        0     6925 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/schema.py
--rw-r--r--   0        0        0     1144 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/state.py
--rw-r--r--   0        0        0      929 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/storage.py
--rw-r--r--   0        0        0        0 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/structures/__init__.py
--rw-r--r--   0        0        0    27958 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/structures/payloads.py
--rw-r--r--   0        0        0     6544 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/structures/responses.py
--rw-r--r--   0        0        0     3457 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/structures/types.py
--rw-r--r--   0        0        0     6779 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/transactions.py
--rw-r--r--   0        0        0     3542 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/utils.py
--rw-r--r--   0        0        0      899 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/blueprints/shared.py
--rw-r--r--   0        0        0    24763 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/cairo_rs_py_patch.py
--rw-r--r--   0        0        0      877 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/chargeable_account.py
--rw-r--r--   0        0        0     4989 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/compiler.py
--rw-r--r--   0        0        0     1239 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/constants.py
--rw-r--r--   0        0        0      646 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/contract_class_wrapper.py
--rw-r--r--   0        0        0    14596 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/devnet_config.py
--rw-r--r--   0        0        0      784 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/dump.py
--rw-r--r--   0        0        0     5592 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/fee_token.py
--rw-r--r--   0        0        0     6911 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/forked_state.py
--rw-r--r--   0        0        0     1640 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/general_config.py
--rw-r--r--   0        0        0     9005 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/origin.py
--rw-r--r--   0        0        0    10009 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/postman_wrapper.py
--rw-r--r--   0        0        0     1970 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/predeployed_contract_wrapper.py
--rw-r--r--   0        0        0     4275 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/server.py
--rw-r--r--   0        0        0    39209 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/starknet_wrapper.py
--rw-r--r--   0        0        0     1988 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/state.py
--rw-r--r--   0        0        0     2573 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/state_archive.py
--rw-r--r--   0        0        0    11617 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/transactions.py
--rw-r--r--   0        0        0     1626 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/udc.py
--rw-r--r--   0        0        0     8580 2023-05-19 17:45:57.592393 starknet_devnet-0.5.2/starknet_devnet/util.py
--rw-r--r--   0        0        0     2437 1970-01-01 00:00:00.000000 starknet_devnet-0.5.2/setup.py
--rw-r--r--   0        0        0     2191 1970-01-01 00:00:00.000000 starknet_devnet-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-01 14:55:07.944823 starknet_devnet-0.5.3/LICENSE
+-rw-r--r--   0        0        0     1054 2023-06-01 14:55:07.944823 starknet_devnet-0.5.3/README.md
+-rw-r--r--   0        0        0     1818 2023-06-01 14:55:07.956824 starknet_devnet-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0   208485 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json
+-rw-r--r--   0        0        0    32739 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/MockStarknetMessaging.json
+-rw-r--r--   0        0        0    35645 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/UDC_OZ_0.5.0.json
+-rw-r--r--   0        0        0     2958 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/__init__.py
+-rw-r--r--   0        0        0     2130 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/account.py
+-rw-r--r--   0        0        0     3784 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/account_util.py
+-rw-r--r--   0        0        0     2692 2023-06-01 14:55:07.960824 starknet_devnet-0.5.3/starknet_devnet/accounts.py
+-rw-r--r--   0        0        0   118818 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json
+-rw-r--r--   0        0        0     1784 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json
+-rw-r--r--   0        0        0     1866 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/block_info_generator.py
+-rw-r--r--   0        0        0    12337 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blocks.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/__init__.py
+-rw-r--r--   0        0        0     7523 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/base.py
+-rw-r--r--   0        0        0    14072 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/feeder_gateway.py
+-rw-r--r--   0        0        0     2228 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/gateway.py
+-rw-r--r--   0        0        0     3959 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/postman.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/__init__.py
+-rw-r--r--   0        0        0     2138 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/blocks.py
+-rw-r--r--   0        0        0     2120 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/call.py
+-rw-r--r--   0        0        0     2195 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/classes.py
+-rw-r--r--   0        0        0     6257 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/misc.py
+-rw-r--r--   0        0        0     4878 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/routes.py
+-rw-r--r--   0        0        0   116673 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/rpc_spec.py
+-rw-r--r--   0        0        0     6049 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/rpc_spec_write.py
+-rw-r--r--   0        0        0     6925 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/schema.py
+-rw-r--r--   0        0        0     1144 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/state.py
+-rw-r--r--   0        0        0      929 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/storage.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/__init__.py
+-rw-r--r--   0        0        0    28429 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/payloads.py
+-rw-r--r--   0        0        0     6544 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/responses.py
+-rw-r--r--   0        0        0     3457 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/types.py
+-rw-r--r--   0        0        0     7212 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/transactions.py
+-rw-r--r--   0        0        0     3542 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/utils.py
+-rw-r--r--   0        0        0      899 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/blueprints/shared.py
+-rw-r--r--   0        0        0    24763 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/cairo_rs_py_patch.py
+-rw-r--r--   0        0        0      877 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/chargeable_account.py
+-rw-r--r--   0        0        0     5133 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/compiler.py
+-rw-r--r--   0        0        0     1239 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/constants.py
+-rw-r--r--   0        0        0      646 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/contract_class_wrapper.py
+-rw-r--r--   0        0        0    14596 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/devnet_config.py
+-rw-r--r--   0        0        0      784 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/dump.py
+-rw-r--r--   0        0        0     5592 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/fee_token.py
+-rw-r--r--   0        0        0     8161 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/forked_state.py
+-rw-r--r--   0        0        0     1640 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/general_config.py
+-rw-r--r--   0        0        0     9005 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/origin.py
+-rw-r--r--   0        0        0    10015 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/postman_wrapper.py
+-rw-r--r--   0        0        0     1970 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/predeployed_contract_wrapper.py
+-rw-r--r--   0        0        0     4275 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/server.py
+-rw-r--r--   0        0        0    39769 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/starknet_wrapper.py
+-rw-r--r--   0        0        0     1988 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/state.py
+-rw-r--r--   0        0        0     2573 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/state_archive.py
+-rw-r--r--   0        0        0    11617 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/transactions.py
+-rw-r--r--   0        0        0     1626 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/udc.py
+-rw-r--r--   0        0        0     8580 2023-06-01 14:55:07.964824 starknet_devnet-0.5.3/starknet_devnet/util.py
+-rw-r--r--   0        0        0     2435 1970-01-01 00:00:00.000000 starknet_devnet-0.5.3/setup.py
+-rw-r--r--   0        0        0     2189 1970-01-01 00:00:00.000000 starknet_devnet-0.5.3/PKG-INFO
```

### Comparing `starknet_devnet-0.5.2/LICENSE` & `starknet_devnet-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/README.md` & `starknet_devnet-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/pyproject.toml` & `starknet_devnet-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "starknet_devnet"
-version = "0.5.2"
+version = "0.5.3"
 description = "A local testnet for Starknet"
 authors = ["FabijanC <fabijan.corak@gmail.com>"]
 license = "MIT"
 
 readme = "README.md"
 repository = "https://github.com/0xSpaceShard/starknet-devnet"
 homepage = "https://github.com/0xSpaceShard/starknet-devnet"
 keywords = ["starknet", "cairo", "testnet", "local", "server"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.10"
 Flask = {extras = ["async"], version = "~2.0.3"}
 flask-cors = "~3.0.10"
-cairo-lang = "0.11.1.1"
+cairo-lang = "0.11.2"
 Werkzeug = "~2.0.3"
 cloudpickle = "~2.1.0"
 crypto-cpp-py = "~1.4.0"
 marshmallow = "~3.17.0"
 typing-extensions = "~4.3.0"
 gunicorn = "~20.1.0"
 marshmallow-dataclass = "~8.4"
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json` & `starknet_devnet-0.5.3/starknet_devnet/ERC20_Mintable_OZ_0.2.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/MockStarknetMessaging.json` & `starknet_devnet-0.5.3/starknet_devnet/MockStarknetMessaging.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/UDC_OZ_0.5.0.json` & `starknet_devnet-0.5.3/starknet_devnet/UDC_OZ_0.5.0.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/__init__.py` & `starknet_devnet-0.5.3/starknet_devnet/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # pylint: disable=unused-import
 # pylint: disable=import-outside-toplevel
 
 import os
 import sys
 
-__version__ = "0.5.2"
+__version__ = "0.5.3"
 
 
 def _patch_pedersen_hash():
     """
     Improves performance by substituting the default Python implementation of Pedersen hash
     with Software Mansion's Python wrapper of C++ implementation.
     """
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/account.py` & `starknet_devnet-0.5.3/starknet_devnet/account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/account_util.py` & `starknet_devnet-0.5.3/starknet_devnet/account_util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/accounts.py` & `starknet_devnet-0.5.3/starknet_devnet/accounts.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json` & `starknet_devnet-0.5.3/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json` & `starknet_devnet-0.5.3/starknet_devnet/accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/Account_abi.json`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/block_info_generator.py` & `starknet_devnet-0.5.3/starknet_devnet/block_info_generator.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blocks.py` & `starknet_devnet-0.5.3/starknet_devnet/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/base.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/base.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/feeder_gateway.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/feeder_gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/gateway.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/gateway.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/postman.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/postman.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/blocks.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/blocks.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/call.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/call.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,18 +50,18 @@
         result = await state.starknet_wrapper.call(
             transaction=make_call_function(request),
             block_id=block_id,
         )
         return [rpc_felt(res) for res in result["result"]]
     except StarkException as ex:
         if ex.code.name == "TRANSACTION_FAILED" and ex.code.value == 39:
-            raise RpcError.from_spec_name("INVALID_CALL_DATA") from ex
+            raise RpcError.from_spec_name("CONTRACT_ERROR") from ex
         if (
             f"Entry point {gateway_felt(request['entry_point_selector'])} not found"
             in ex.message
         ):
-            raise RpcError.from_spec_name("INVALID_MESSAGE_SELECTOR") from ex
+            raise RpcError.from_spec_name("CONTRACT_ERROR") from ex
         if "While handling calldata" in ex.message:
-            raise RpcError.from_spec_name("INVALID_CALL_DATA") from ex
+            raise RpcError.from_spec_name("CONTRACT_ERROR") from ex
         raise RpcError(
             code=PredefinedRpcErrorCode.INTERNAL_ERROR.value, message=ex.message
         ) from ex
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/classes.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/classes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/misc.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,18 @@
 )
 from starknet_devnet.state import state
 
 
 def check_address(address, event):
     """
     Check address.
+
+    If no address is set in the filter, it returns True.
     """
-    return event.from_address == int(address, 0)
+    return address is None or event.from_address == int(address, 0)
 
 
 def _check_keys(keys: List[List[Felt]], event):
     """
     Check keys.
 
     Check every key in an event against related list of accepted values.
@@ -131,16 +133,18 @@
     In our implementation continuation_token is just a number.
 
     In state.starknet_wrapper.get_state().events there is no relation between blocks.
     This is why we need to iterate block by block, take all events,
     and chunk it later which is not an optimal solution.
     """
     # Required parameters
-    from_block = await get_block_by_block_id(filter.get("from_block"))
-    to_block = await get_block_by_block_id(filter.get("to_block"))
+    from_block = await get_block_by_block_id(
+        filter.get("from_block", {"block_number": 0})
+    )
+    to_block = await get_block_by_block_id(filter.get("to_block", "latest"))
     block_range = await _get_events_range(from_block, to_block)
 
     try:
         chunk_size = int(filter.get("chunk_size"))
     except ValueError as ex:
         raise RpcError(
             code=PredefinedRpcErrorCode.INVALID_PARAMS.value,
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/routes.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/routes.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/rpc_spec.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/rpc_spec.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # pylint: disable=too-many-lines, missing-module-docstring
-# NOTE: This is modified version of 0.3.0-rc1 spec
+# NOTE: This is modified version of 0.3.0 spec
 # All usages of "oneOf" have been replaced by "anyOf"
+# and the required field from STRUCT_MEMBER was removed.
 RPC_SPECIFICATION = r"""
 {
     "openrpc": "1.0.0-rc1",
     "info": {
         "version": "0.50.0",
         "title": "StarkNet Node API",
         "license": {}
@@ -16,27 +17,31 @@
             "summary": "Get block information with transaction hashes given the block id",
             "params": [
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "description": "The resulting block information with transaction hashes",
                 "schema": {
+                    "title": "Starknet get block hash with tx hashes result",
                     "anyOf": [
                         {
+                            "title": "Block with transaction hashes",
                             "$ref": "#/components/schemas/BLOCK_WITH_TX_HASHES"
                         },
                         {
+                            "title": "Pending block with transaction hashes",
                             "$ref": "#/components/schemas/PENDING_BLOCK_WITH_TX_HASHES"
                         }
                     ]
                 }
             },
             "errors": [
                 {
@@ -49,27 +54,31 @@
             "summary": "Get block information with full transactions given the block id",
             "params": [
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "description": "The resulting block information with full transactions",
                 "schema": {
+                    "title": "Starknet get block with txs result",
                     "anyOf": [
                         {
+                            "title": "Block with transactions",
                             "$ref": "#/components/schemas/BLOCK_WITH_TXS"
                         },
                         {
+                            "title": "Pending block with transactions",
                             "$ref": "#/components/schemas/PENDING_BLOCK_WITH_TXS"
                         }
                     ]
                 }
             },
             "errors": [
                 {
@@ -82,27 +91,31 @@
             "summary": "Get the information about the result of executing the requested block",
             "params": [
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "description": "The information about the state update of the requested block",
                 "schema": {
+                    "title": "Starknet get state update result",
                     "anyOf": [
                         {
+                            "title": "State update",
                             "$ref": "#/components/schemas/STATE_UPDATE"
                         },
                         {
+                            "title": "Pending state update",
                             "$ref": "#/components/schemas/PENDING_STATE_UPDATE"
                         }
                     ]
                 }
             },
             "errors": [
                 {
@@ -116,40 +129,44 @@
             "params": [
                 {
                     "name": "contract_address",
                     "description": "The address of the contract to read from",
                     "summary": "The address of the contract to read from",
                     "required": true,
                     "schema": {
+                        "title": "Address",
                         "$ref": "#/components/schemas/ADDRESS"
                     }
                 },
                 {
                     "name": "key",
                     "description": "The key to the storage value for the given contract",
                     "summary": "The key to the storage value for the given contract",
                     "required": true,
                     "schema": {
+                        "title": "Storage key",
                         "$ref": "#/components/schemas/STORAGE_KEY"
                     }
                 },
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "description": "The value at the given key for the given contract. 0 if no value is found",
                 "summary": "The value at the given key for the given contract.",
                 "schema": {
+                    "title": "Field element",
                     "$ref": "#/components/schemas/FELT"
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/CONTRACT_NOT_FOUND"
                 },
@@ -164,21 +181,23 @@
             "paramStructure": "by-name",
             "params": [
                 {
                     "name": "transaction_hash",
                     "summary": "The hash of the requested transaction",
                     "required": true,
                     "schema": {
+                        "title": "Transaction hash",
                         "$ref": "#/components/schemas/TXN_HASH"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "schema": {
+                    "title": "Transaction",
                     "$ref": "#/components/schemas/TXN"
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/TXN_HASH_NOT_FOUND"
                 }
@@ -190,30 +209,33 @@
             "description": "Get the details of the transaction given by the identified block and index in that block. If no transaction is found, null is returned.",
             "params": [
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 },
                 {
                     "name": "index",
                     "summary": "The index in the block to search for the transaction",
                     "required": true,
                     "schema": {
+                        "title": "Index",
                         "type": "integer",
                         "minimum": 0
                     }
                 }
             ],
             "result": {
                 "name": "transactionResult",
                 "schema": {
+                    "title": "Transaction",
                     "$ref": "#/components/schemas/TXN"
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/BLOCK_NOT_FOUND"
                 },
@@ -228,21 +250,23 @@
             "paramStructure": "by-name",
             "params": [
                 {
                     "name": "transaction_hash",
                     "summary": "The hash of the requested transaction",
                     "required": true,
                     "schema": {
+                        "title": "Transaction hash",
                         "$ref": "#/components/schemas/TXN_HASH"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "schema": {
+                    "title": "Transaction receipt",
                     "$ref": "#/components/schemas/TXN_RECEIPT"
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/TXN_HASH_NOT_FOUND"
                 }
@@ -253,35 +277,40 @@
             "summary": "Get the contract class definition in the given block associated with the given hash",
             "params": [
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 },
                 {
                     "name": "class_hash",
                     "description": "The hash of the requested contract class",
                     "required": true,
                     "schema": {
+                        "title": "Field element",
                         "$ref": "#/components/schemas/FELT"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "description": "The contract class, if found",
                 "schema": {
+                    "title": "Starknet get class result",
                     "anyOf": [
                         {
+                            "title": "Deprecated contract class",
                             "$ref": "#/components/schemas/DEPRECATED_CONTRACT_CLASS"
                         },
                         {
+                            "title": "Contract class",
                             "$ref": "#/components/schemas/CONTRACT_CLASS"
                         }
                     ]
                 }
             },
             "errors": [
                 {
@@ -297,30 +326,33 @@
             "summary": "Get the contract class hash in the given block for the contract deployed at the given address",
             "params": [
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 },
                 {
                     "name": "contract_address",
                     "description": "The address of the contract whose class hash will be returned",
                     "required": true,
                     "schema": {
+                        "title": "Address",
                         "$ref": "#/components/schemas/ADDRESS"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "description": "The class hash of the given contract",
                 "schema": {
+                    "title": "Field element",
                     "$ref": "#/components/schemas/FELT"
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/BLOCK_NOT_FOUND"
                 },
@@ -334,35 +366,40 @@
             "summary": "Get the contract class definition in the given block at the given address",
             "params": [
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 },
                 {
                     "name": "contract_address",
                     "description": "The address of the contract whose class definition will be returned",
                     "required": true,
                     "schema": {
+                        "title": "Address",
                         "$ref": "#/components/schemas/ADDRESS"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "description": "The contract class",
                 "schema": {
+                    "title": "Starknet get class at result",
                     "anyOf": [
                         {
+                            "title": "Deprecated contract class",
                             "$ref": "#/components/schemas/DEPRECATED_CONTRACT_CLASS"
                         },
                         {
+                            "title": "Contract class",
                             "$ref": "#/components/schemas/CONTRACT_CLASS"
                         }
                     ]
                 }
             },
             "errors": [
                 {
@@ -379,23 +416,25 @@
             "description": "Returns the number of transactions in the designated block.",
             "params": [
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "description": "The number of transactions in the designated block",
                 "summary": "The number of transactions in the designated block",
                 "schema": {
+                    "title": "Block transaction count",
                     "type": "integer",
                     "minimum": 0
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/BLOCK_NOT_FOUND"
@@ -407,49 +446,46 @@
             "summary": "call a starknet function without creating a StarkNet transaction",
             "description": "Calls a function in a contract and returns the return value.  Using this call will not create a transaction; hence, will not change the state",
             "params": [
                 {
                     "name": "request",
                     "summary": "The details of the function call",
                     "schema": {
+                        "title": "Function call",
                         "$ref": "#/components/schemas/FUNCTION_CALL"
                     },
                     "required": true
                 },
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag, for the block referencing the state or call the transaction on.",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "summary": "The function's return value",
                 "description": "The function's return value, as defined in the Cairo output",
                 "schema": {
                     "type": "array",
+                    "title": "Field element",
                     "items": {
                         "$ref": "#/components/schemas/FELT"
                     }
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/CONTRACT_NOT_FOUND"
                 },
                 {
-                    "$ref": "#/components/errors/INVALID_MESSAGE_SELECTOR"
-                },
-                {
-                    "$ref": "#/components/errors/INVALID_CALL_DATA"
-                },
-                {
                     "$ref": "#/components/errors/CONTRACT_ERROR"
                 },
                 {
                     "$ref": "#/components/errors/BLOCK_NOT_FOUND"
                 }
             ]
         },
@@ -460,51 +496,48 @@
             "params": [
                 {
                     "name": "request",
                     "summary": "The transaction to estimate",
                     "schema": {
                         "type": "array",
                         "description": "a sequence of transactions to estimate, running each transaction on the state resulting from applying all the previous ones",
+                        "title": "Broadcasted transaction",
                         "items": {
                             "$ref": "#/components/schemas/BROADCASTED_TXN"
                         }
                     },
                     "required": true
                 },
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag, for the block referencing the state or call the transaction on.",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "description": "the fee estimations",
                 "schema": {
+                    "title": "Estimation",
                     "type": "array",
                     "description": "a sequence of fee estimatione where the i'th estimate corresponds to the i'th transaction",
                     "items": {
                         "$ref": "#/components/schemas/FEE_ESTIMATE"
                     }
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/CONTRACT_NOT_FOUND"
                 },
                 {
-                    "$ref": "#/components/errors/INVALID_MESSAGE_SELECTOR"
-                },
-                {
-                    "$ref": "#/components/errors/INVALID_CALL_DATA"
-                },
-                {
                     "$ref": "#/components/errors/CONTRACT_ERROR"
                 },
                 {
                     "$ref": "#/components/errors/BLOCK_NOT_FOUND"
                 }
             ]
         },
@@ -512,14 +545,15 @@
             "name": "starknet_blockNumber",
             "summary": "Get the most recent accepted block number",
             "params": [],
             "result": {
                 "name": "result",
                 "description": "The latest block number",
                 "schema": {
+                    "title": "Block number",
                     "$ref": "#/components/schemas/BLOCK_NUMBER"
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/NO_BLOCKS"
                 }
@@ -529,23 +563,30 @@
             "name": "starknet_blockHashAndNumber",
             "summary": "Get the most recent accepted block hash and number",
             "params": [],
             "result": {
                 "name": "result",
                 "description": "The latest block hash and number",
                 "schema": {
+                    "title": "Starknet block hash and number result",
                     "type": "object",
                     "properties": {
                         "block_hash": {
+                            "title": "Block hash",
                             "$ref": "#/components/schemas/BLOCK_HASH"
                         },
                         "block_number": {
+                            "title": "Block number",
                             "$ref": "#/components/schemas/BLOCK_NUMBER"
                         }
-                    }
+                    },
+                    "required": [
+                        "block_hash",
+                        "block_number"
+                    ]
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/NO_BLOCKS"
                 }
             ]
@@ -554,14 +595,15 @@
             "name": "starknet_chainId",
             "summary": "Return the currently configured StarkNet chain id",
             "params": [],
             "result": {
                 "name": "result",
                 "description": "The chain id this node is connected to",
                 "schema": {
+                    "title": "Chain id",
                     "$ref": "#/components/schemas/CHAIN_ID"
                 }
             }
         },
         {
             "name": "starknet_pendingTransactions",
             "summary": "Returns the transactions in the transaction pool, recognized by this sequencer",
@@ -582,20 +624,23 @@
             "summary": "Returns an object about the sync status, or false if the node is not synching",
             "params": [],
             "result": {
                 "name": "syncing",
                 "summary": "The state of the synchronization, or false if the node is not synchronizing",
                 "description": "The status of the node, if it is currently synchronizing state. FALSE otherwise",
                 "schema": {
+                    "title": "SyncingStatus",
                     "anyOf": [
                         {
                             "type": "boolean",
+                            "title": "False",
                             "description": "only legal value is FALSE here"
                         },
                         {
+                            "title": "Sync status",
                             "$ref": "#/components/schemas/SYNC_STATUS"
                         }
                     ]
                 }
             }
         },
         {
@@ -604,29 +649,33 @@
             "description": "Returns all event objects matching the conditions in the provided filter",
             "params": [
                 {
                     "name": "filter",
                     "summary": "The conditions used to filter the returned events",
                     "required": true,
                     "schema": {
+                        "title": "Event emitter",
                         "allOf": [
                             {
+                                "title": "Event filter",
                                 "$ref": "#/components/schemas/EVENT_FILTER"
                             },
                             {
+                                "title": "Result page request",
                                 "$ref": "#/components/schemas/RESULT_PAGE_REQUEST"
                             }
                         ]
                     }
                 }
             ],
             "result": {
                 "name": "events",
                 "description": "All the event objects matching the filter",
                 "schema": {
+                    "title": "Events chunk",
                     "$ref": "#/components/schemas/EVENTS_CHUNK"
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/PAGE_SIZE_TOO_BIG"
                 },
@@ -646,30 +695,33 @@
             "summary": "Get the nonce associated with the given address in the given block",
             "params": [
                 {
                     "name": "block_id",
                     "description": "The hash of the requested block, or number (height) of the requested block, or a block tag",
                     "required": true,
                     "schema": {
+                        "title": "Block id",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     }
                 },
                 {
                     "name": "contract_address",
                     "description": "The address of the contract whose nonce we're seeking",
                     "required": true,
                     "schema": {
+                        "title": "Address",
                         "$ref": "#/components/schemas/ADDRESS"
                     }
                 }
             ],
             "result": {
                 "name": "result",
                 "description": "The last nonce used for the given contract.",
                 "schema": {
+                    "title": "Field element",
                     "$ref": "#/components/schemas/FELT"
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/BLOCK_NOT_FOUND"
                 },
@@ -679,125 +731,142 @@
             ]
         }
     ],
     "components": {
         "contentDescriptors": {},
         "schemas": {
             "EVENTS_CHUNK": {
+                "title": "Events chunk",
                 "type": "object",
                 "properties": {
                     "events": {
                         "type": "array",
                         "title": "Matching Events",
                         "items": {
                             "$ref": "#/components/schemas/EMITTED_EVENT"
                         }
                     },
                     "continuation_token": {
+                        "title": "Continuation token",
                         "description": "Use this token in a subsequent query to obtain the next page. Should not appear if there are no more pages.",
                         "type": "string"
                     }
                 },
                 "required": [
                     "events"
                 ]
             },
             "RESULT_PAGE_REQUEST": {
+                "title": "Result page request",
                 "type": "object",
                 "properties": {
                     "continuation_token": {
+                        "title": "Continuation token",
                         "description": "The token returned from the previous query. If no token is provided the first page is returned.",
                         "type": "string"
                     },
                     "chunk_size": {
+                        "title": "Chunk size",
                         "type": "integer",
                         "minimum": 1
                     }
                 },
                 "required": [
                     "chunk_size"
                 ]
             },
             "EMITTED_EVENT": {
-                "title": "An event emitted as a result of transaction execution",
-                "description": "Event information decorated with metadata on where it was emitted",
+                "title": "Emitted event",
+                "description": "Event information decorated with metadata on where it was emitted / An event emitted as a result of transaction execution",
                 "allOf": [
                     {
-                        "title": "The event information",
+                        "title": "Event",
+                        "description": "The event information",
                         "$ref": "#/components/schemas/EVENT"
                     },
                     {
-                        "title": "The event emission information",
+                        "title": "Event context",
+                        "description": "The event emission information",
                         "type": "object",
                         "properties": {
                             "block_hash": {
-                                "title": "The hash of the block in which the event was emitted",
+                                "title": "Block hash",
+                                "description": "The hash of the block in which the event was emitted",
                                 "$ref": "#/components/schemas/BLOCK_HASH"
                             },
                             "block_number": {
-                                "title": "The number of the block in which the event was emitted",
+                                "title": "Block number",
+                                "description": "The number of the block in which the event was emitted",
                                 "$ref": "#/components/schemas/BLOCK_NUMBER"
                             },
                             "transaction_hash": {
-                                "title": "The transaction that emitted the event",
+                                "title": "Transaction hash",
+                                "description": "The transaction that emitted the event",
                                 "$ref": "#/components/schemas/TXN_HASH"
                             }
                         },
                         "required": [
                             "block_hash",
                             "block_number",
                             "transaction_hash"
                         ]
                     }
                 ]
             },
             "EVENT": {
-                "title": "A StarkNet event",
+                "title": "Event",
+                "description": "A StarkNet event",
                 "allOf": [
                     {
+                        "title": "Event emitter",
                         "type": "object",
                         "properties": {
                             "from_address": {
+                                "title": "From address",
                                 "$ref": "#/components/schemas/ADDRESS"
                             }
                         },
                         "required": [
                             "from_address"
                         ]
                     },
                     {
+                        "title": "Event content",
                         "$ref": "#/components/schemas/EVENT_CONTENT"
                     }
                 ]
             },
             "EVENT_CONTENT": {
-                "title": "Event Content",
+                "title": "Event content",
                 "description": "The content of an event",
                 "type": "object",
                 "properties": {
                     "keys": {
                         "type": "array",
+                        "title": "Keys",
                         "items": {
                             "$ref": "#/components/schemas/FELT"
                         }
                     },
                     "data": {
                         "type": "array",
+                        "title": "Data",
                         "items": {
                             "$ref": "#/components/schemas/FELT"
                         }
                     }
                 },
                 "required": [
                     "keys",
                     "data"
                 ]
             },
             "EVENT_FILTER": {
-                "title": "An event filter/query",
+                "title": "Event filter",
+                "description": "An event filter/query",
                 "type": "object",
                 "properties": {
                     "from_block": {
                         "title": "from block",
                         "$ref": "#/components/schemas/BLOCK_ID"
                     },
                     "to_block": {
@@ -805,222 +874,256 @@
                         "$ref": "#/components/schemas/BLOCK_ID"
                     },
                     "address": {
                         "title": "from contract",
                         "$ref": "#/components/schemas/ADDRESS"
                     },
                     "keys": {
-                        "title": "filter key values",
+                        "title": "Keys",
                         "description": "The values used to filter the events",
                         "type": "array",
                         "items": {
-                            "title": "Possible values, per key",
+                            "title": "Keys",
                             "description": "Per key (by position), designate the possible values to be matched for events to be returned. Empty array designates 'any' value",
                             "type": "array",
                             "items": {
                                 "$ref": "#/components/schemas/FELT"
                             }
                         }
                     }
                 },
-                "required": [
-                    "from_block",
-                    "to_block",
-                    "address",
-                    "keys"
-                ]
+                "required": []
             },
             "BLOCK_ID": {
-                "title": "Block hash, number or tag",
+                "title": "Block id",
+                "description": "Block hash, number or tag",
                 "anyOf": [
                     {
+                        "title": "Block hash",
                         "type": "object",
                         "properties": {
                             "block_hash": {
+                                "title": "Block hash",
                                 "$ref": "#/components/schemas/BLOCK_HASH"
                             }
                         },
                         "required": [
                             "block_hash"
                         ]
                     },
                     {
+                        "title": "Block number",
                         "type": "object",
                         "properties": {
                             "block_number": {
+                                "title": "Block number",
                                 "$ref": "#/components/schemas/BLOCK_NUMBER"
                             }
                         },
                         "required": [
                             "block_number"
                         ]
                     },
                     {
+                        "title": "Block tag",
                         "$ref": "#/components/schemas/BLOCK_TAG"
                     }
                 ]
             },
             "BLOCK_TAG": {
+                "title": "Block tag",
                 "type": "string",
                 "description": "A tag specifying a dynamic reference to a block",
                 "enum": [
                     "latest",
                     "pending"
                 ]
             },
             "SYNC_STATUS": {
+                "title": "Sync status",
                 "type": "object",
                 "description": "An object describing the node synchronization status",
                 "properties": {
                     "starting_block_hash": {
+                        "title": "Starting block hash",
                         "description": "The hash of the block from which the sync started",
                         "$ref": "#/components/schemas/BLOCK_HASH"
                     },
                     "starting_block_num": {
+                        "title": "Starting block number",
                         "description": "The number (height) of the block from which the sync started",
                         "$ref": "#/components/schemas/NUM_AS_HEX"
                     },
                     "current_block_hash": {
+                        "title": "Current block hash",
                         "description": "The hash of the current block being synchronized",
                         "$ref": "#/components/schemas/BLOCK_HASH"
                     },
                     "current_block_num": {
+                        "title": "Current block number",
                         "description": "The number (height) of the current block being synchronized",
                         "$ref": "#/components/schemas/NUM_AS_HEX"
                     },
                     "highest_block_hash": {
+                        "title": "Highest block hash",
                         "description": "The hash of the estimated highest block to be synchronized",
                         "$ref": "#/components/schemas/BLOCK_HASH"
                     },
                     "highest_block_num": {
+                        "title": "Highest block number",
                         "description": "The number (height) of the estimated highest block to be synchronized",
                         "$ref": "#/components/schemas/NUM_AS_HEX"
                     }
                 },
                 "required": [
                     "starting_block_hash",
                     "starting_block_num",
                     "current_block_hash",
                     "current_block_num",
                     "highest_block_hash",
                     "highest_block_num"
                 ]
             },
             "NUM_AS_HEX": {
-                "title": "An integer number in hex format (0x...)",
+                "title": "Number as hex",
+                "description": "An integer number in hex format (0x...)",
                 "type": "string",
                 "pattern": "^0x[a-fA-F0-9]+$"
             },
             "CHAIN_ID": {
-                "title": "chainId",
+                "title": "Chain id",
                 "description": "StarkNet chain id, given in hex representation.",
                 "type": "string",
                 "pattern": "^0x[a-fA-F0-9]+$"
             },
             "STATE_UPDATE": {
+                "title": "State update",
                 "type": "object",
                 "allOf": [
                     {
+                        "title": "Event emitter",
                         "type": "object",
                         "properties": {
                             "block_hash": {
+                                "title": "Block hash",
                                 "$ref": "#/components/schemas/BLOCK_HASH"
                             },
                             "new_root": {
+                                "title": "New root",
                                 "description": "The new global state root",
                                 "$ref": "#/components/schemas/FELT"
                             }
                         },
                         "required": [
                             "block_hash",
                             "new_root"
                         ]
                     },
                     {
+                        "title": "Pending state update",
                         "$ref": "#/components/schemas/PENDING_STATE_UPDATE"
                     }
                 ]
             },
             "PENDING_STATE_UPDATE": {
+                "title": "Pending state update",
+                "description": "Pending state update",
                 "type": "object",
                 "properties": {
                     "old_root": {
+                        "title": "Old root",
                         "description": "The previous global state root",
                         "$ref": "#/components/schemas/FELT"
                     },
                     "state_diff": {
+                        "title": "State diff",
                         "description": "The change in state applied in this block, given as a mapping of addresses to the new values and/or new contracts",
                         "type": "object",
                         "properties": {
                             "storage_diffs": {
+                                "title": "Storage diffs",
                                 "type": "array",
                                 "items": {
                                     "description": "The changes in the storage per contract address",
                                     "$ref": "#/components/schemas/CONTRACT_STORAGE_DIFF_ITEM"
                                 }
                             },
                             "deprecated_declared_classes": {
+                                "title": "Deprecated declared classes",
                                 "type": "array",
                                 "items": {
                                     "description": "The hash of the declared class",
                                     "$ref": "#/components/schemas/FELT"
                                 }
                             },
                             "declared_classes": {
+                                "title": "Declared classes",
                                 "type": "array",
                                 "items": {
-                                    "description": "The declared class hash and compiled class hash",
+                                    "title": "Event emitter",
                                     "type": "object",
+                                    "description": "The declared class hash and compiled class hash",
                                     "properties": {
                                         "class_hash": {
+                                            "title": "Class hash",
                                             "description": "The hash of the declared class",
                                             "$ref": "#/components/schemas/FELT"
                                         },
                                         "compiled_class_hash": {
+                                            "title": "Compiled class hash",
                                             "description": "The Cairo assembly hash corresponding to the declared class",
                                             "$ref": "#/components/schemas/FELT"
                                         }
                                     }
                                 }
                             },
                             "deployed_contracts": {
+                                "title": "Deployed contracts",
                                 "type": "array",
                                 "items": {
                                     "description": "A new contract deployed as part of the state update",
                                     "$ref": "#/components/schemas/DEPLOYED_CONTRACT_ITEM"
                                 }
                             },
                             "replaced_classes": {
+                                "title": "Replaced classes",
                                 "type": "array",
                                 "items": {
                                     "description": "The list of contracts whose class was replaced",
+                                    "title": "Event emitter",
                                     "type": "object",
                                     "properties": {
                                         "contract_address": {
+                                            "title": "Contract address",
                                             "description": "The address of the contract whose class was replaced",
                                             "$ref": "#/components/schemas/ADDRESS"
                                         },
                                         "class_hash": {
+                                            "title": "Class hash",
                                             "description": "The new class hash",
                                             "$ref": "#/components/schemas/FELT"
                                         }
                                     }
                                 }
                             },
                             "nonces": {
+                                "title": "Nonces",
                                 "type": "array",
                                 "items": {
+                                    "title": "Event emitter",
                                     "description": "The updated nonce per contract address",
                                     "type": "object",
                                     "properties": {
                                         "contract_address": {
+                                            "title": "Contract address",
                                             "description": "The address of the contract",
                                             "$ref": "#/components/schemas/ADDRESS"
                                         },
                                         "nonce": {
+                                            "title": "Nonce",
                                             "description": "The nonce for the given address at the end of the block",
                                             "$ref": "#/components/schemas/FELT"
                                         }
                                     }
                                 }
                             }
                         },
@@ -1036,247 +1139,293 @@
                 },
                 "required": [
                     "old_root",
                     "state_diff"
                 ]
             },
             "ADDRESS": {
+                "title": "Address",
                 "$ref": "#/components/schemas/FELT"
             },
             "STORAGE_KEY": {
                 "type": "string",
-                "title": "A storage key",
+                "title": "Storage key",
                 "$comment": "A storage key, represented as a string of hex digits",
                 "description": "A storage key. Represented as up to 62 hex digits, 3 bits, and 5 leading zeroes.",
                 "pattern": "^0x0[0-7]{1}[a-fA-F0-9]{0,62}$"
             },
             "ETH_ADDRESS": {
+                "title": "Ethereum address",
                 "type": "string",
                 "$comment": "An ethereum address",
                 "description": "an ethereum address represented as 40 hex digits",
                 "pattern": "^0x[a-fA-F0-9]{40}$"
             },
             "TXN_HASH": {
                 "$ref": "#/components/schemas/FELT",
                 "description": "The transaction hash, as assigned in StarkNet",
-                "title": "A transaction's hash"
+                "title": "Transaction hash"
             },
             "FELT": {
                 "type": "string",
                 "title": "Field element",
                 "description": "A field element. represented by at most 63 hex digits",
                 "pattern": "^0x(0|[a-fA-F1-9]{1}[a-fA-F0-9]{0,62})$"
             },
             "BLOCK_NUMBER": {
+                "title": "Block number",
                 "description": "The block's number (its height)",
                 "type": "integer",
                 "minimum": 0
             },
             "BLOCK_HASH": {
+                "title": "Block hash",
                 "$ref": "#/components/schemas/FELT"
             },
             "BLOCK_BODY_WITH_TX_HASHES": {
+                "title": "Block body with transaction hashes",
                 "type": "object",
                 "properties": {
                     "transactions": {
+                        "title": "Transaction",
                         "description": "The hashes of the transactions included in this block",
                         "type": "array",
                         "items": {
                             "description": "The hash of a single transaction",
                             "$ref": "#/components/schemas/TXN_HASH"
                         }
                     }
                 },
                 "required": [
                     "transactions"
                 ]
             },
             "BLOCK_BODY_WITH_TXS": {
+                "title": "Block body with transactions",
                 "type": "object",
                 "properties": {
                     "transactions": {
+                        "title": "Transactions",
                         "description": "The transactions in this block",
                         "type": "array",
                         "items": {
                             "$ref": "#/components/schemas/TXN"
                         }
                     }
                 },
                 "required": [
                     "transactions"
                 ]
             },
             "BLOCK_HEADER": {
+                "title": "Block header",
                 "type": "object",
                 "properties": {
                     "block_hash": {
+                        "title": "Block hash",
                         "$ref": "#/components/schemas/BLOCK_HASH"
                     },
                     "parent_hash": {
+                        "title": "Parent hash",
                         "description": "The hash of this block's parent",
                         "$ref": "#/components/schemas/BLOCK_HASH"
                     },
                     "block_number": {
+                        "title": "Block number",
                         "description": "The block number (its height)",
                         "$ref": "#/components/schemas/BLOCK_NUMBER"
                     },
                     "new_root": {
+                        "title": "New root",
                         "description": "The new global state root",
                         "$ref": "#/components/schemas/FELT"
                     },
                     "timestamp": {
+                        "title": "Timestamp",
                         "description": "The time in which the block was created, encoded in Unix time",
                         "type": "integer",
                         "minimum": 0
                     },
                     "sequencer_address": {
+                        "title": "Sequencer address",
                         "description": "The StarkNet identity of the sequencer submitting this block",
                         "$ref": "#/components/schemas/FELT"
                     }
                 },
                 "required": [
                     "block_hash",
                     "parent_hash",
                     "block_number",
                     "new_root",
                     "timestamp",
                     "sequencer_address"
                 ]
             },
             "BLOCK_WITH_TX_HASHES": {
-                "title": "The block object",
+                "title": "Block with transaction hashes",
+                "description": "The block object",
                 "allOf": [
                     {
+                        "title": "Event emitter",
                         "type": "object",
                         "properties": {
                             "status": {
+                                "title": "Status",
                                 "$ref": "#/components/schemas/BLOCK_STATUS"
                             }
                         },
                         "required": [
                             "status"
                         ]
                     },
                     {
+                        "title": "Block header",
                         "$ref": "#/components/schemas/BLOCK_HEADER"
                     },
                     {
+                        "title": "Block body with transaction hashes",
                         "$ref": "#/components/schemas/BLOCK_BODY_WITH_TX_HASHES"
                     }
                 ]
             },
             "BLOCK_WITH_TXS": {
-                "title": "The block object",
+                "title": "Block with transactions",
+                "description": "The block object",
                 "allOf": [
                     {
+                        "title": "Event emitter",
                         "type": "object",
                         "properties": {
                             "status": {
+                                "title": "Status",
                                 "$ref": "#/components/schemas/BLOCK_STATUS"
                             }
                         },
                         "required": [
                             "status"
                         ]
                     },
                     {
+                        "title": "Block header",
                         "$ref": "#/components/schemas/BLOCK_HEADER"
                     },
                     {
+                        "title": "Block body with transactions",
                         "$ref": "#/components/schemas/BLOCK_BODY_WITH_TXS"
                     }
                 ]
             },
             "PENDING_BLOCK_WITH_TX_HASHES": {
+                "title": "Pending block with transaction hashes",
                 "description": "The dynamic block being constructed by the sequencer. Note that this object will be deprecated upon decentralization.",
                 "allOf": [
                     {
+                        "title": "Block body with transactions hashes",
                         "$ref": "#/components/schemas/BLOCK_BODY_WITH_TX_HASHES"
                     },
                     {
+                        "title": "Event emitter",
                         "type": "object",
                         "properties": {
                             "timestamp": {
+                                "title": "Timestamp",
                                 "description": "The time in which the block was created, encoded in Unix time",
                                 "type": "integer",
                                 "minimum": 0
                             },
                             "sequencer_address": {
+                                "title": "Sequencer address",
                                 "description": "The StarkNet identity of the sequencer submitting this block",
                                 "$ref": "#/components/schemas/FELT"
                             },
                             "parent_hash": {
+                                "title": "Parent hash",
                                 "description": "The hash of this block's parent",
                                 "$ref": "#/components/schemas/BLOCK_HASH"
                             }
                         }
                     }
                 ]
             },
             "PENDING_BLOCK_WITH_TXS": {
+                "title": "Pending block with transactions",
                 "description": "The dynamic block being constructed by the sequencer. Note that this object will be deprecated upon decentralization.",
                 "allOf": [
                     {
+                        "title": "Block body with transactions",
                         "$ref": "#/components/schemas/BLOCK_BODY_WITH_TXS"
                     },
                     {
                         "type": "object",
+                        "title": "Event emitter",
                         "properties": {
                             "timestamp": {
+                                "title": "Timestamp",
                                 "description": "The time in which the block was created, encoded in Unix time",
                                 "type": "integer",
                                 "minimum": 0
                             },
                             "sequencer_address": {
+                                "title": "Sequencer address",
                                 "description": "The StarkNet identity of the sequencer submitting this block",
                                 "$ref": "#/components/schemas/FELT"
                             },
                             "parent_hash": {
+                                "title": "Parent hash",
                                 "description": "The hash of this block's parent",
                                 "$ref": "#/components/schemas/BLOCK_HASH"
                             }
                         }
                     }
                 ]
             },
             "DEPLOYED_CONTRACT_ITEM": {
+                "title": "Deployed contract item",
                 "type": "object",
                 "properties": {
                     "address": {
+                        "title": "Address",
                         "description": "The address of the contract",
                         "$ref": "#/components/schemas/FELT"
                     },
                     "class_hash": {
+                        "title": "Class hash",
                         "description": "The hash of the contract code",
                         "$ref": "#/components/schemas/FELT"
                     }
                 },
                 "required": [
                     "address",
                     "class_hash"
                 ]
             },
             "CONTRACT_STORAGE_DIFF_ITEM": {
+                "title": "Contract storage diff item",
                 "type": "object",
                 "properties": {
                     "address": {
+                        "title": "Address",
                         "description": "The contract address for which the storage changed",
                         "$ref": "#/components/schemas/FELT"
                     },
                     "storage_entries": {
+                        "title": "Storage entries",
                         "description": "The changes in the storage of the contract",
                         "type": "array",
                         "items": {
+                            "title": "Event emitter",
                             "type": "object",
                             "properties": {
                                 "key": {
+                                    "title": "Key",
                                     "description": "The key of the changed value",
                                     "$ref": "#/components/schemas/FELT"
                                 },
                                 "value": {
+                                    "title": "Value",
                                     "description": "The new value applied to the given address",
                                     "$ref": "#/components/schemas/FELT"
                                 }
                             }
                         }
                     }
                 },
@@ -1286,267 +1435,334 @@
                 ]
             },
             "TXN": {
                 "title": "Transaction",
                 "description": "The transaction schema, as it appears inside a block",
                 "anyOf": [
                     {
+                        "title": "Invoke transaction",
                         "$ref": "#/components/schemas/INVOKE_TXN"
                     },
                     {
+                        "title": "L1 handler transaction",
                         "$ref": "#/components/schemas/L1_HANDLER_TXN"
                     },
                     {
+                        "title": "Declare transaction",
                         "$ref": "#/components/schemas/DECLARE_TXN"
                     },
                     {
+                        "title": "Deploy transaction",
                         "$ref": "#/components/schemas/DEPLOY_TXN"
                     },
                     {
+                        "title": "Deploy account transaction",
                         "$ref": "#/components/schemas/DEPLOY_ACCOUNT_TXN"
                     }
                 ]
             },
             "BROADCASTED_TXN": {
+                "title": "Broadcasted transaction",
                 "description": "the transaction's representation when it's sent to the sequencer (but not yet in a block)",
-                "title": "Transaction",
                 "anyOf": [
                     {
+                        "title": "Broadcasted invoke transaction",
                         "$ref": "#/components/schemas/BROADCASTED_INVOKE_TXN"
                     },
                     {
+                        "title": "Broadcasted declare transaction",
                         "$ref": "#/components/schemas/BROADCASTED_DECLARE_TXN"
                     },
                     {
+                        "title": "Broadcasted deploy account transaction",
                         "$ref": "#/components/schemas/BROADCASTED_DEPLOY_ACCOUNT_TXN"
                     }
                 ]
             },
             "SIGNATURE": {
-                "title": "A transaction signature",
+                "title": "Signature",
+                "description": "A transaction signature",
                 "type": "array",
                 "items": {
                     "$ref": "#/components/schemas/FELT"
                 }
             },
             "BROADCASTED_TXN_COMMON_PROPERTIES": {
+                "title": "Broadcasted transaction common properties",
                 "type": "object",
                 "description": "common properties of a transaction that is sent to the sequencer (but is not yet in a block)",
                 "properties": {
                     "max_fee": {
+                        "title": "Max fee",
                         "$ref": "#/components/schemas/FELT",
                         "description": "The maximal fee that can be charged for including the transaction"
                     },
                     "version": {
+                        "title": "Version",
                         "description": "Version of the transaction scheme",
                         "$ref": "#/components/schemas/NUM_AS_HEX"
                     },
                     "signature": {
+                        "title": "Signature",
                         "$ref": "#/components/schemas/SIGNATURE"
                     },
                     "nonce": {
+                        "title": "Nonce",
                         "$ref": "#/components/schemas/FELT"
                     }
                 },
                 "required": [
                     "max_fee",
                     "version",
                     "signature",
                     "nonce"
                 ]
             },
             "COMMON_TXN_PROPERTIES": {
+                "title": "Common transaction properties",
                 "allOf": [
                     {
                         "type": "object",
+                        "title": "Transaction hash",
                         "properties": {
                             "transaction_hash": {
+                                "title": "Transaction hash",
                                 "$ref": "#/components/schemas/TXN_HASH",
                                 "description": "The hash identifying the transaction"
                             }
                         },
                         "required": [
                             "transaction_hash"
                         ]
                     },
                     {
+                        "title": "Broadcasted transaction common properties",
                         "$ref": "#/components/schemas/BROADCASTED_TXN_COMMON_PROPERTIES"
                     }
                 ]
             },
             "DECLARE_TXN": {
+                "title": "Declare transaction",
                 "anyOf": [
                     {
+                        "title": "Declare transaction V1",
                         "$ref": "#/components/schemas/DECLARE_TXN_V1"
                     },
                     {
+                        "title": "Declare transaction V2",
                         "$ref": "#/components/schemas/DECLARE_TXN_V2"
                     }
                 ]
             },
             "DECLARE_TXN_V1": {
-                "title": "Declare Contract Transaction",
+                "title": "Declare Contract Transaction V1",
+                "description": "Declare Contract Transaction V1",
                 "allOf": [
                     {
+                        "title": "Common transaction properties",
                         "$ref": "#/components/schemas/COMMON_TXN_PROPERTIES"
                     },
                     {
                         "type": "object",
+                        "title": "Event emitter",
                         "properties": {
                             "type": {
+                                "title": "Declare",
                                 "type": "string",
                                 "enum": [
                                     "DECLARE"
                                 ]
                             },
                             "class_hash": {
+                                "title": "Class hash",
                                 "description": "The hash of the declared class",
                                 "$ref": "#/components/schemas/FELT"
                             },
                             "sender_address": {
+                                "title": "Sender address",
                                 "description": "The address of the account contract sending the declaration transaction",
                                 "$ref": "#/components/schemas/ADDRESS"
                             }
                         },
                         "required": [
                             "type",
                             "class_hash",
                             "sender_address"
                         ]
                     }
                 ]
             },
             "DECLARE_TXN_V2": {
-                "title": "Declare Contract Transaction",
+                "title": "Declare Transaction V2",
+                "description": "Declare Contract Transaction V2",
                 "allOf": [
                     {
+                        "title": "Declare transaction V1",
                         "$ref": "#/components/schemas/DECLARE_TXN_V1"
                     },
                     {
                         "type": "object",
+                        "title": "Event emitter",
                         "properties": {
                             "compiled_class_hash": {
+                                "title": "Compiled class hash",
                                 "description": "The hash of the Cairo assembly resulting from the Sierra compilation",
                                 "$ref": "#/components/schemas/FELT"
                             }
-                        }
+                        },
+                        "required": [
+                            "compiled_class_hash"
+                        ]
                     }
                 ]
             },
             "BROADCASTED_DECLARE_TXN": {
+                "title": "Broadcasted declare transaction",
                 "anyOf": [
                     {
+                        "title": "Broadcasted declare transaction V1",
                         "$ref": "#/components/schemas/BROADCASTED_DECLARE_TXN_V1"
                     },
                     {
+                        "title": "Broadcasted declare transaction V2",
                         "$ref": "#/components/schemas/BROADCASTED_DECLARE_TXN_V2"
                     }
                 ]
             },
             "BROADCASTED_DECLARE_TXN_V1": {
-                "title": "mempool representation of a declare transaction",
+                "title": "Broadcasted declare transaction V1",
+                "description": "mempool representation of a declare transaction",
                 "allOf": [
                     {
+                        "title": "Broadcasted transaction common properties",
                         "$ref": "#/components/schemas/BROADCASTED_TXN_COMMON_PROPERTIES"
                     },
                     {
                         "type": "object",
+                        "title": "Declare v1",
                         "properties": {
+                            "type": {
+                                "title": "Declare",
+                                "type": "string",
+                                "enum": [
+                                    "DECLARE"
+                                ]
+                            },
                             "contract_class": {
+                                "title": "Contract class",
                                 "description": "The class to be declared",
                                 "$ref": "#/components/schemas/DEPRECATED_CONTRACT_CLASS"
                             },
                             "sender_address": {
+                                "title": "Sender address",
                                 "description": "The address of the account contract sending the declaration transaction",
                                 "$ref": "#/components/schemas/ADDRESS"
                             }
                         }
                     }
                 ]
             },
             "BROADCASTED_DECLARE_TXN_V2": {
-                "title": "mempool representation of a declare transaction",
+                "title": "Broadcasted declare transaction V2",
+                "description": "mempool representation of a declare transaction V2",
                 "allOf": [
                     {
+                        "title": "Broadcasted transaction common properties",
                         "$ref": "#/components/schemas/BROADCASTED_TXN_COMMON_PROPERTIES"
                     },
                     {
                         "type": "object",
+                        "title": "Event emitter",
                         "properties": {
                             "type": {
+                                "title": "Declare",
                                 "type": "string",
                                 "enum": [
                                     "DECLARE"
                                 ]
                             },
                             "contract_class": {
+                                "title": "Contract class",
                                 "description": "The class to be declared",
                                 "$ref": "#/components/schemas/CONTRACT_CLASS"
                             },
                             "sender_address": {
+                                "title": "Sender address",
                                 "description": "The address of the account contract sending the declaration transaction",
                                 "$ref": "#/components/schemas/ADDRESS"
                             },
                             "compiled_class_hash": {
+                                "title": "Compiled class hash",
                                 "description": "The hash of the Cairo assembly resulting from the Sierra compilation",
                                 "$ref": "#/components/schemas/FELT"
                             }
                         },
                         "required": [
                             "type",
                             "contract_class",
-                            "sender_address"
+                            "sender_address",
+                            "compiled_class_hash"
                         ]
                     }
                 ]
             },
             "DEPLOY_ACCOUNT_TXN": {
-                "title": "Deploy Account Transaction",
+                "title": "Deploy account transaction",
                 "description": "Deploys an account contract, charges fee from the pre-funded account addresses",
                 "allOf": [
                     {
+                        "title": "Common transaction properties",
                         "$ref": "#/components/schemas/COMMON_TXN_PROPERTIES"
                     },
                     {
+                        "title": "Deploy account transaction properties",
                         "$ref": "#/components/schemas/DEPLOY_ACCOUNT_TXN_PROPERTIES"
                     }
                 ]
             },
             "BROADCASTED_DEPLOY_ACCOUNT_TXN": {
+                "title": "Broadcasted deploy account transaction",
                 "description": "Mempool representation of a deploy account transaction",
                 "allOf": [
                     {
+                        "title": "Broadcasted transaction common properties",
                         "$ref": "#/components/schemas/BROADCASTED_TXN_COMMON_PROPERTIES"
                     },
                     {
+                        "title": "Deploy account transaction properties",
                         "$ref": "#/components/schemas/DEPLOY_ACCOUNT_TXN_PROPERTIES"
                     }
                 ]
             },
             "DEPLOY_ACCOUNT_TXN_PROPERTIES": {
+                "title": "Deploy account transaction properties",
                 "type": "object",
                 "properties": {
                     "type": {
+                        "title": "Deploy account",
                         "type": "string",
                         "enum": [
                             "DEPLOY_ACCOUNT"
                         ]
                     },
                     "contract_address_salt": {
+                        "title": "Contract address salt",
                         "description": "The salt for the address of the deployed contract",
                         "$ref": "#/components/schemas/FELT"
                     },
                     "constructor_calldata": {
                         "type": "array",
                         "description": "The parameters passed to the constructor",
+                        "title": "Constructor calldata",
                         "items": {
                             "$ref": "#/components/schemas/FELT"
                         }
                     },
                     "class_hash": {
+                        "title": "Class hash",
                         "description": "The hash of the deployed contract's class",
                         "$ref": "#/components/schemas/FELT"
                     }
                 },
                 "required": [
                     "type",
                     "contract_address_salt",
@@ -1556,223 +1772,262 @@
             },
             "DEPLOY_TXN": {
                 "title": "Deploy Contract Transaction",
                 "description": "The structure of a deploy transaction. Note that this transaction type is deprecated and will no longer be supported in future versions",
                 "allOf": [
                     {
                         "type": "object",
+                        "title": "Event emitter",
                         "properties": {
                             "transaction_hash": {
+                                "title": "Transaction hash",
                                 "$ref": "#/components/schemas/TXN_HASH",
                                 "description": "The hash identifying the transaction"
                             },
                             "class_hash": {
+                                "title": "Class hash",
                                 "description": "The hash of the deployed contract's class",
                                 "$ref": "#/components/schemas/FELT"
                             }
                         },
                         "required": [
                             "transaction_hash",
                             "class_hash"
                         ]
                     },
                     {
+                        "title": "Deploy transaction properties",
                         "$ref": "#/components/schemas/DEPLOY_TXN_PROPERTIES"
                     }
                 ]
             },
             "DEPLOY_TXN_PROPERTIES": {
+                "title": "Deploy transaction properties",
                 "type": "object",
                 "properties": {
                     "version": {
+                        "title": "Version",
                         "description": "Version of the transaction scheme",
                         "$ref": "#/components/schemas/NUM_AS_HEX"
                     },
                     "type": {
+                        "title": "Deploy",
                         "type": "string",
                         "enum": [
                             "DEPLOY"
                         ]
                     },
                     "contract_address_salt": {
                         "description": "The salt for the address of the deployed contract",
+                        "title": "Contract address salt",
                         "$ref": "#/components/schemas/FELT"
                     },
                     "constructor_calldata": {
                         "type": "array",
+                        "title": "Constructor calldata",
                         "description": "The parameters passed to the constructor",
                         "items": {
                             "$ref": "#/components/schemas/FELT"
                         }
                     }
                 },
                 "required": [
                     "version",
                     "type",
                     "contract_address_salt",
                     "constructor_calldata"
                 ]
             },
             "INVOKE_TXN_V0": {
-                "title": "version 0 invoke transaction",
+                "title": "Invoke transaction V0",
                 "description": "invokes a specific function in the desired contract (not necessarily an account)",
                 "$ref": "#/components/schemas/FUNCTION_CALL"
             },
             "INVOKE_TXN_V1": {
-                "title": "version 1 invoke transaction",
+                "title": "Invoke transaction V1",
                 "description": "initiates a transaction from a given account",
                 "type": "object",
                 "properties": {
                     "sender_address": {
+                        "title": "sender address",
                         "$ref": "#/components/schemas/ADDRESS"
                     },
                     "calldata": {
                         "type": "array",
+                        "title": "calldata",
                         "description": "The data expected by the account's `execute` function (in most usecases, this includes the called contract address and a function selector)",
                         "items": {
                             "$ref": "#/components/schemas/FELT"
                         }
                     }
                 },
                 "required": [
                     "sender_address",
                     "calldata"
                 ]
             },
             "INVOKE_TXN": {
-                "title": "Initiate a transaction from an account",
+                "title": "Invoke transaction",
+                "description": "Initiate a transaction from an account",
                 "allOf": [
                     {
+                        "title": "Common transaction properties",
                         "$ref": "#/components/schemas/COMMON_TXN_PROPERTIES"
                     },
                     {
                         "type": "object",
+                        "title": "Type",
                         "properties": {
                             "type": {
+                                "title": "Type",
                                 "type": "string",
                                 "enum": [
                                     "INVOKE"
                                 ]
                             }
                         },
                         "required": [
                             "type"
                         ]
                     },
                     {
+                        "title": "Invoke transaction properties",
                         "anyOf": [
                             {
+                                "title": "Invoke transaction V0",
                                 "$ref": "#/components/schemas/INVOKE_TXN_V0"
                             },
                             {
+                                "title": "Invoke transaction V1",
                                 "$ref": "#/components/schemas/INVOKE_TXN_V1"
                             }
                         ]
                     }
                 ]
             },
             "BROADCASTED_INVOKE_TXN": {
+                "title": "Broadcasted invoke transaction",
                 "description": "mempool representation of an invoke transaction",
                 "allOf": [
                     {
+                        "title": "Broadcasted transaction common properties",
                         "$ref": "#/components/schemas/BROADCASTED_TXN_COMMON_PROPERTIES"
                     },
                     {
+                        "title": "Event emitter",
                         "type": "object",
                         "properties": {
                             "type": {
+                                "title": "Type",
                                 "type": "string",
                                 "enum": [
                                     "INVOKE"
                                 ]
                             }
                         },
                         "required": [
                             "type"
                         ]
                     },
                     {
+                        "title": "Invoke transaction properties",
                         "anyOf": [
                             {
+                                "title": "Invoke transaction V0",
                                 "$ref": "#/components/schemas/INVOKE_TXN_V0"
                             },
                             {
+                                "title": "Invoke transaction V1",
                                 "$ref": "#/components/schemas/INVOKE_TXN_V1"
                             }
                         ]
                     }
                 ]
             },
             "L1_HANDLER_TXN": {
+                "title": "L1 Handler transaction",
                 "allOf": [
                     {
                         "type": "object",
-                        "title": "l1-->l2 message transaction",
+                        "title": "L1 handler transaction",
                         "description": "a call to an l1_handler on an L2 contract induced by a message from L1",
                         "properties": {
                             "transaction_hash": {
+                                "title": "Transaction hash",
                                 "$ref": "#/components/schemas/TXN_HASH",
                                 "description": "The hash identifying the transaction"
                             },
                             "version": {
+                                "title": "Version",
                                 "description": "Version of the transaction scheme",
                                 "$ref": "#/components/schemas/NUM_AS_HEX"
                             },
                             "type": {
+                                "title": "type",
                                 "type": "string",
                                 "enum": [
                                     "L1_HANDLER"
                                 ]
                             },
                             "nonce": {
+                                "title": "Nonce",
                                 "description": "The L1->L2 message nonce field of the SN Core L1 contract at the time the transaction was sent",
                                 "$ref": "#/components/schemas/NUM_AS_HEX"
                             }
                         },
                         "required": [
                             "transaction_hash",
                             "version",
                             "type",
                             "nonce"
                         ]
                     },
                     {
+                        "title": "Function call",
                         "$ref": "#/components/schemas/FUNCTION_CALL"
                     }
                 ]
             },
             "COMMON_RECEIPT_PROPERTIES": {
-                "title": "Common properties for a transaction receipt",
+                "title": "Common receipt properties",
+                "description": "Common properties for a transaction receipt",
                 "type": "object",
                 "properties": {
                     "transaction_hash": {
+                        "title": "Transaction hash",
                         "$ref": "#/components/schemas/TXN_HASH",
                         "description": "The hash identifying the transaction"
                     },
                     "actual_fee": {
+                        "title": "Actual fee",
                         "$ref": "#/components/schemas/FELT",
                         "description": "The fee that was charged by the sequencer"
                     },
                     "status": {
+                        "title": "Status",
                         "$ref": "#/components/schemas/TXN_STATUS"
                     },
                     "block_hash": {
+                        "title": "Block hash",
                         "$ref": "#/components/schemas/BLOCK_HASH"
                     },
                     "block_number": {
+                        "title": "Block number",
                         "$ref": "#/components/schemas/BLOCK_NUMBER"
                     },
                     "messages_sent": {
                         "type": "array",
+                        "title": "Messages sent",
                         "items": {
                             "$ref": "#/components/schemas/MSG_TO_L1"
                         }
                     },
                     "events": {
                         "description": "The events emitted as part of this transaction",
+                        "title": "Events",
                         "type": "array",
                         "items": {
                             "$ref": "#/components/schemas/EVENT"
                         }
                     }
                 },
                 "required": [
@@ -1785,70 +2040,80 @@
                     "events"
                 ]
             },
             "INVOKE_TXN_RECEIPT": {
                 "title": "Invoke Transaction Receipt",
                 "allOf": [
                     {
+                        "title": "Type",
                         "type": "object",
                         "properties": {
                             "type": {
+                                "title": "Type",
                                 "type": "string",
                                 "enum": [
                                     "INVOKE"
                                 ]
                             }
                         },
                         "required": [
                             "type"
                         ]
                     },
                     {
+                        "title": "Common receipt properties",
                         "$ref": "#/components/schemas/COMMON_RECEIPT_PROPERTIES"
                     }
                 ]
             },
             "DECLARE_TXN_RECEIPT": {
                 "title": "Declare Transaction Receipt",
                 "allOf": [
                     {
+                        "title": "Event emitter",
                         "type": "object",
                         "properties": {
                             "type": {
+                                "title": "Declare",
                                 "type": "string",
                                 "enum": [
                                     "DECLARE"
                                 ]
                             }
                         },
                         "required": [
                             "type"
                         ]
                     },
                     {
+                        "title": "Common receipt properties",
                         "$ref": "#/components/schemas/COMMON_RECEIPT_PROPERTIES"
                     }
                 ]
             },
             "DEPLOY_ACCOUNT_TXN_RECEIPT": {
                 "title": "Deploy Account Transaction Receipt",
                 "allOf": [
                     {
+                        "title": "Common receipt properties",
                         "$ref": "#/components/schemas/COMMON_RECEIPT_PROPERTIES"
                     },
                     {
+                        "title": "Event emitter",
                         "type": "object",
                         "properties": {
                             "type": {
+                                "title": "Deploy account",
                                 "type": "string",
                                 "enum": [
                                     "DEPLOY_ACCOUNT"
                                 ]
                             },
                             "contract_address": {
+                                "title": "Contract address",
                                 "description": "The address of the deployed contract",
                                 "$ref": "#/components/schemas/FELT"
                             }
                         },
                         "required": [
                             "type",
                             "contract_address"
@@ -1856,508 +2121,649 @@
                     }
                 ]
             },
             "DEPLOY_TXN_RECEIPT": {
                 "title": "Deploy Transaction Receipt",
                 "allOf": [
                     {
+                        "title": "Common receipt properties",
                         "$ref": "#/components/schemas/COMMON_RECEIPT_PROPERTIES"
                     },
                     {
+                        "title": "Event emitter",
                         "type": "object",
                         "properties": {
                             "type": {
+                                "title": "Deploy",
                                 "type": "string",
                                 "enum": [
                                     "DEPLOY"
                                 ]
                             },
                             "contract_address": {
+                                "title": "Contract address",
                                 "description": "The address of the deployed contract",
                                 "$ref": "#/components/schemas/FELT"
                             }
                         },
                         "required": [
                             "type",
                             "contract_address"
                         ]
                     }
                 ]
             },
             "L1_HANDLER_TXN_RECEIPT": {
-                "title": "receipt for l1 handler transaction",
+                "title": "L1 Handler Transaction Receipt",
+                "description": "receipt for l1 handler transaction",
                 "allOf": [
                     {
+                        "title": "Event emitter",
                         "type": "object",
                         "properties": {
                             "type": {
+                                "title": "type",
                                 "type": "string",
                                 "enum": [
                                     "L1_HANDLER"
                                 ]
                             }
                         },
                         "required": [
                             "type"
                         ]
                     },
                     {
+                        "title": "Common receipt properties",
                         "$ref": "#/components/schemas/COMMON_RECEIPT_PROPERTIES"
                     }
                 ]
             },
             "TXN_RECEIPT": {
+                "title": "Transaction Receipt",
                 "anyOf": [
                     {
+                        "title": "Invoke transaction receipt",
                         "$ref": "#/components/schemas/INVOKE_TXN_RECEIPT"
                     },
                     {
+                        "title": "L1 handler transaction receipt",
                         "$ref": "#/components/schemas/L1_HANDLER_TXN_RECEIPT"
                     },
                     {
+                        "title": "Declare transaction receipt",
                         "$ref": "#/components/schemas/DECLARE_TXN_RECEIPT"
                     },
                     {
+                        "title": "Deploy transaction receipt",
                         "$ref": "#/components/schemas/DEPLOY_TXN_RECEIPT"
                     },
                     {
+                        "title": "Deploy account transaction receipt",
                         "$ref": "#/components/schemas/DEPLOY_ACCOUNT_TXN_RECEIPT"
                     },
                     {
+                        "title": "Pending transaction receipt",
                         "$ref": "#/components/schemas/PENDING_TXN_RECEIPT"
                     }
                 ]
             },
             "PENDING_COMMON_RECEIPT_PROPERTIES": {
-                "title": "Common properties for a pending transaction receipt",
+                "title": "Pending common receipt properties",
+                "description": "Common properties for a pending transaction receipt",
                 "type": "object",
                 "properties": {
                     "transaction_hash": {
+                        "title": "Transaction hash",
                         "$ref": "#/components/schemas/TXN_HASH",
                         "description": "The hash identifying the transaction"
                     },
                     "actual_fee": {
+                        "title": "Actual fee",
                         "$ref": "#/components/schemas/FELT",
                         "description": "The fee that was charged by the sequencer"
                     },
                     "type": {
+                        "title": "Transaction type",
                         "$ref": "#/components/schemas/TXN_TYPE"
                     },
                     "messages_sent": {
                         "type": "array",
+                        "title": "Messages sent",
                         "items": {
                             "$ref": "#/components/schemas/MSG_TO_L1"
                         }
                     },
                     "events": {
                         "description": "The events emitted as part of this transaction",
+                        "title": "Events",
                         "type": "array",
                         "items": {
                             "$ref": "#/components/schemas/EVENT"
                         }
                     }
                 },
                 "required": [
                     "transaction_hash",
                     "actual_fee",
+                    "type",
                     "messages_sent",
                     "events"
                 ]
             },
             "PENDING_DEPLOY_TXN_RECEIPT": {
                 "title": "Pending deploy Transaction Receipt",
                 "allOf": [
                     {
+                        "title": "Common receipt properties",
                         "$ref": "#/components/schemas/PENDING_COMMON_RECEIPT_PROPERTIES"
                     },
                     {
                         "type": "object",
+                        "title": "Event emitter",
                         "properties": {
                             "contract_address": {
+                                "title": "Contract address",
                                 "description": "The address of the deployed contract",
                                 "$ref": "#/components/schemas/FELT"
                             }
                         }
                     }
                 ]
             },
             "PENDING_TXN_RECEIPT": {
+                "title": "Pending Transaction Receipt",
                 "anyOf": [
                     {
+                        "title": "Pending deploy transaction receipt",
                         "$ref": "#/components/schemas/PENDING_DEPLOY_TXN_RECEIPT"
                     },
                     {
+                        "title": "Pending common receipt properties",
                         "$comment": "Used for pending invoke and declare transaction receipts",
                         "$ref": "#/components/schemas/PENDING_COMMON_RECEIPT_PROPERTIES"
                     }
                 ]
             },
             "MSG_TO_L1": {
+                "title": "Message to L1",
                 "type": "object",
                 "properties": {
+                    "from_address": {
+                        "description": "The address of the L2 contract sending the message",
+                        "$ref": "#/components/schemas/FELT"
+                    },
                     "to_address": {
+                        "title": "To address",
                         "description": "The target L1 address the message is sent to",
                         "$ref": "#/components/schemas/FELT"
                     },
                     "payload": {
                         "description": "The payload of the message",
+                        "title": "Payload",
                         "type": "array",
                         "items": {
                             "$ref": "#/components/schemas/FELT"
                         }
                     }
                 },
                 "required": [
+                    "from_address",
                     "to_address",
                     "payload"
                 ]
             },
             "TXN_STATUS": {
+                "title": "Transaction status",
                 "type": "string",
                 "enum": [
                     "PENDING",
                     "ACCEPTED_ON_L2",
                     "ACCEPTED_ON_L1",
                     "REJECTED"
                 ],
                 "description": "The status of the transaction"
             },
             "TXN_TYPE": {
+                "title": "Transaction type",
                 "type": "string",
                 "enum": [
                     "DECLARE",
                     "DEPLOY",
                     "DEPLOY_ACCOUNT",
                     "INVOKE",
                     "L1_HANDLER"
                 ],
                 "description": "The type of the transaction"
             },
             "BLOCK_STATUS": {
+                "title": "Block status",
                 "type": "string",
                 "enum": [
                     "PENDING",
                     "ACCEPTED_ON_L2",
                     "ACCEPTED_ON_L1",
                     "REJECTED"
                 ],
                 "description": "The status of the block"
             },
             "FUNCTION_CALL": {
+                "title": "Function call",
                 "type": "object",
-                "title": "Function call information",
+                "description": "Function call information",
                 "properties": {
                     "contract_address": {
+                        "title": "Contract address",
                         "$ref": "#/components/schemas/ADDRESS"
                     },
                     "entry_point_selector": {
+                        "title": "Entry point selector",
                         "$ref": "#/components/schemas/FELT"
                     },
                     "calldata": {
+                        "title": "Calldata",
                         "type": "array",
                         "description": "The parameters passed to the function",
                         "items": {
                             "$ref": "#/components/schemas/FELT"
                         }
                     }
                 },
                 "required": [
                     "contract_address",
                     "entry_point_selector",
                     "calldata"
                 ]
             },
             "CONTRACT_CLASS": {
+                "title": "Contract class",
                 "type": "object",
                 "properties": {
                     "sierra_program": {
+                        "title": "Sierra program",
                         "type": "array",
                         "description": "The list of Sierra instructions of which the program consists",
                         "items": {
                             "$ref": "#/components/schemas/FELT"
                         }
                     },
                     "contract_class_version": {
+                        "title": "Contract class version",
                         "type": "string",
                         "description": "The version of the contract class object. Currently, the Starknet OS supports version 0.1.0"
                     },
                     "entry_points_by_type": {
+                        "title": "Entry points by type",
                         "type": "object",
                         "properties": {
                             "CONSTRUCTOR": {
                                 "type": "array",
+                                "title": "Constructor",
                                 "items": {
                                     "$ref": "#/components/schemas/SIERRA_ENTRY_POINT"
                                 }
                             },
                             "EXTERNAL": {
+                                "title": "External",
                                 "type": "array",
                                 "items": {
                                     "$ref": "#/components/schemas/SIERRA_ENTRY_POINT"
                                 }
                             },
                             "L1_HANDLER": {
+                                "title": "L1 handler",
                                 "type": "array",
                                 "items": {
                                     "$ref": "#/components/schemas/SIERRA_ENTRY_POINT"
                                 }
                             }
-                        }
+                        },
+                        "required": [
+                            "CONSTRUCTOR",
+                            "EXTERNAL",
+                            "L1_HANDLER"
+                        ]
                     },
                     "abi": {
+                        "title": "ABI",
                         "type": "string",
-                        "descripition": "The class ABI, as supplied by the user declaring the class"
+                        "description": "The class ABI, as supplied by the user declaring the class"
                     }
                 },
                 "required": [
                     "sierra_program",
                     "contract_class_version",
                     "entry_points_by_type"
                 ]
             },
             "DEPRECATED_CONTRACT_CLASS": {
-                "title": "The definition of a StarkNet contract class",
+                "title": "Deprecated contract class",
+                "description": "The definition of a StarkNet contract class",
                 "type": "object",
                 "properties": {
                     "program": {
                         "type": "string",
+                        "title": "Program",
                         "description": "A base64 representation of the compressed program code",
                         "pattern": "^(?:[A-Za-z0-9+/]{4})*(?:[A-Za-z0-9+/]{3}=|[A-Za-z0-9+/]{2}==)?$"
                     },
                     "entry_points_by_type": {
                         "type": "object",
+                        "title": "Deprecated entry points by type",
                         "properties": {
                             "CONSTRUCTOR": {
                                 "type": "array",
+                                "title": "Deprecated constructor",
                                 "items": {
                                     "$ref": "#/components/schemas/DEPRECATED_CAIRO_ENTRY_POINT"
                                 }
                             },
                             "EXTERNAL": {
                                 "type": "array",
+                                "title": "Deprecated external",
                                 "items": {
                                     "$ref": "#/components/schemas/DEPRECATED_CAIRO_ENTRY_POINT"
                                 }
                             },
                             "L1_HANDLER": {
                                 "type": "array",
+                                "title": "Deprecated L1 handler",
                                 "items": {
                                     "$ref": "#/components/schemas/DEPRECATED_CAIRO_ENTRY_POINT"
                                 }
                             }
                         }
                     },
                     "abi": {
+                        "title": "Contract ABI",
                         "$ref": "#/components/schemas/CONTRACT_ABI"
                     }
                 },
                 "required": [
                     "program",
                     "entry_points_by_type"
                 ]
             },
             "DEPRECATED_CAIRO_ENTRY_POINT": {
+                "title": "Deprecated Cairo entry point",
                 "type": "object",
                 "properties": {
                     "offset": {
+                        "title": "Offset",
                         "description": "The offset of the entry point in the program",
                         "$ref": "#/components/schemas/NUM_AS_HEX"
                     },
                     "selector": {
+                        "title": "Selector",
                         "description": "A unique identifier of the entry point (function) in the program",
                         "$ref": "#/components/schemas/FELT"
                     }
-                }
+                },
+                "required": [
+                    "offset",
+                    "selector"
+                ]
             },
             "SIERRA_ENTRY_POINT": {
+                "title": "Sierra entry point",
                 "type": "object",
                 "properties": {
                     "selector": {
+                        "title": "Selector",
                         "description": "A unique identifier of the entry point (function) in the program",
                         "$ref": "#/components/schemas/FELT"
                     },
                     "function_idx": {
+                        "title": "Function index",
                         "description": "The index of the function in the program",
                         "type": "integer"
                     }
-                }
+                },
+                "required": [
+                    "selector",
+                    "function_idx"
+                ]
             },
             "CONTRACT_ABI": {
+                "title": "Contract ABI",
                 "type": "array",
                 "items": {
                     "$ref": "#/components/schemas/CONTRACT_ABI_ENTRY"
                 }
             },
             "CONTRACT_ABI_ENTRY": {
+                "title": "Contract ABI entry",
                 "anyOf": [
                     {
+                        "title": "Function ABI entry",
                         "$ref": "#/components/schemas/FUNCTION_ABI_ENTRY"
                     },
                     {
+                        "title": "Event ABI entry",
                         "$ref": "#/components/schemas/EVENT_ABI_ENTRY"
                     },
                     {
+                        "title": "Struct ABI entry",
                         "$ref": "#/components/schemas/STRUCT_ABI_ENTRY"
                     }
                 ]
             },
             "STRUCT_ABI_TYPE": {
+                "title": "Struct ABI type",
                 "type": "string",
                 "enum": [
                     "struct"
                 ]
             },
             "EVENT_ABI_TYPE": {
+                "title": "Event ABI type",
                 "type": "string",
                 "enum": [
                     "event"
                 ]
             },
             "FUNCTION_ABI_TYPE": {
+                "title": "Function ABI type",
                 "type": "string",
                 "enum": [
                     "function",
                     "l1_handler",
                     "constructor"
                 ]
             },
             "STRUCT_ABI_ENTRY": {
+                "title": "Struct ABI entry",
                 "type": "object",
                 "properties": {
                     "type": {
+                        "title": "Struct ABI type",
                         "$ref": "#/components/schemas/STRUCT_ABI_TYPE"
                     },
                     "name": {
+                        "title": "Struct name",
                         "description": "The struct name",
                         "type": "string"
                     },
                     "size": {
+                        "title": "Size",
                         "type": "integer",
                         "minimum": 1
                     },
                     "members": {
                         "type": "array",
+                        "title": "Members",
                         "items": {
                             "$ref": "#/components/schemas/STRUCT_MEMBER"
                         }
                     }
-                }
+                },
+                "required": [
+                    "type",
+                    "name",
+                    "size",
+                    "members"
+                ]
             },
             "STRUCT_MEMBER": {
+                "title": "Struct member",
                 "allOf": [
                     {
+                        "title": "Typed parameter",
                         "$ref": "#/components/schemas/TYPED_PARAMETER"
                     },
                     {
                         "type": "object",
+                        "title": "Event emitter",
                         "properties": {
                             "offset": {
+                                "title": "Offset",
                                 "description": "offset of this property within the struct",
                                 "type": "integer"
                             }
                         }
                     }
                 ]
             },
             "EVENT_ABI_ENTRY": {
+                "title": "Event ABI entry",
                 "type": "object",
                 "properties": {
                     "type": {
+                        "title": "Event ABI type",
                         "$ref": "#/components/schemas/EVENT_ABI_TYPE"
                     },
                     "name": {
+                        "title": "Event name",
                         "description": "The event name",
                         "type": "string"
                     },
                     "keys": {
                         "type": "array",
+                        "title": "Typed parameter",
                         "items": {
                             "$ref": "#/components/schemas/TYPED_PARAMETER"
                         }
                     },
                     "data": {
                         "type": "array",
+                        "title": "Typed parameter",
                         "items": {
                             "$ref": "#/components/schemas/TYPED_PARAMETER"
                         }
                     }
-                }
+                },
+                "required": [
+                    "type",
+                    "name",
+                    "keys",
+                    "data"
+                ]
+            },
+            "FUNCTION_STATE_MUTABILITY": {
+                "title": "Function state mutability type",
+                "type": "string",
+                "enum": [
+                    "view"
+                ]
             },
             "FUNCTION_ABI_ENTRY": {
+                "title": "Function ABI entry",
                 "type": "object",
                 "properties": {
                     "type": {
+                        "title": "Function ABI type",
                         "$ref": "#/components/schemas/FUNCTION_ABI_TYPE"
                     },
                     "name": {
+                        "title": "Function name",
                         "description": "The function name",
                         "type": "string"
                     },
                     "inputs": {
                         "type": "array",
+                        "title": "Typed parameter",
                         "items": {
                             "$ref": "#/components/schemas/TYPED_PARAMETER"
                         }
                     },
                     "outputs": {
                         "type": "array",
+                        "title": "Typed parameter",
                         "items": {
                             "$ref": "#/components/schemas/TYPED_PARAMETER"
                         }
+                    },
+                    "stateMutability": {
+                        "title": "Function state mutability",
+                        "$ref": "#/components/schemas/FUNCTION_STATE_MUTABILITY"
                     }
-                }
+                },
+                "required": [
+                    "type",
+                    "name",
+                    "inputs",
+                    "outputs"
+                ]
             },
             "TYPED_PARAMETER": {
+                "title": "Typed parameter",
                 "type": "object",
                 "properties": {
                     "name": {
+                        "title": "Parameter name",
                         "description": "The parameter's name",
                         "type": "string"
                     },
                     "type": {
+                        "title": "Parameter type",
                         "description": "The parameter's type",
                         "type": "string"
                     }
-                }
+                },
+                "required": [
+                    "name",
+                    "type"
+                ]
             },
             "FEE_ESTIMATE": {
+                "title": "Fee estimation",
                 "type": "object",
                 "properties": {
                     "gas_consumed": {
+                        "title": "Gas consumed",
                         "description": "The Ethereum gas cost of the transaction (see https://docs.starknet.io/docs/Fees/fee-mechanism for more info)",
                         "$ref": "#/components/schemas/NUM_AS_HEX"
                     },
                     "gas_price": {
+                        "title": "Gas price",
                         "description": "The gas price (in gwei) that was used in the cost estimation",
                         "$ref": "#/components/schemas/NUM_AS_HEX"
                     },
                     "overall_fee": {
+                        "title": "Overall fee",
                         "description": "The estimated fee for the transaction (in gwei), product of gas_consumed and gas_price",
                         "$ref": "#/components/schemas/NUM_AS_HEX"
                     }
-                }
+                },
+                "required": [
+                    "gas_consumed",
+                    "gas_price",
+                    "overall_fee"
+                ]
             }
         },
         "errors": {
             "FAILED_TO_RECEIVE_TXN": {
                 "code": 1,
                 "message": "Failed to write transaction"
             },
             "CONTRACT_NOT_FOUND": {
                 "code": 20,
                 "message": "Contract not found"
             },
-            "INVALID_MESSAGE_SELECTOR": {
-                "code": 21,
-                "message": "Invalid message selector"
-            },
-            "INVALID_CALL_DATA": {
-                "code": 22,
-                "message": "Invalid call data"
-            },
             "BLOCK_NOT_FOUND": {
                 "code": 24,
                 "message": "Block not found"
             },
             "TXN_HASH_NOT_FOUND": {
                 "code": 25,
                 "message": "Transaction hash not found"
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/rpc_spec_write.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/rpc_spec_write.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,17 @@
                         }
                     }
                 }
             },
             "errors": [
                 {
                     "$ref": "#/components/errors/INVALID_CONTRACT_CLASS"
+                },
+                {
+                    "$ref": "#/components/errors/CLASS_ALREADY_DECLARED"
                 }
             ]
         },
         {
             "name": "starknet_addDeployAccountTransaction",
             "summary": "Submit a new deploy account transaction",
             "params": [
@@ -145,12 +148,16 @@
         "errors": {
             "INVALID_CONTRACT_CLASS": {
                 "code": 50,
                 "message": "Invalid contract class"
             },
             "CLASS_HASH_NOT_FOUND": {
                 "$ref": "./api/starknet_api_openrpc.json#/components/errors/CLASS_HASH_NOT_FOUND"
+            },
+            "CLASS_ALREADY_DECLARED": {
+                "code": 51,
+                "message": "Class already declared"
             }
         }
     }
 }
 """
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/schema.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/schema.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/state.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/storage.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/storage.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/structures/payloads.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/payloads.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 
 from __future__ import annotations
 
 from typing import Callable, Dict, List, Optional, Union
 
 from marshmallow.exceptions import MarshmallowError
+from starkware.starknet.definitions.constants import QUERY_VERSION_BASE
 from starkware.starknet.definitions.general_config import StarknetGeneralConfig
 from starkware.starknet.public.abi import AbiEntryType
 from starkware.starknet.services.api.contract_class.contract_class import (
     ContractClass,
     ContractEntryPoint,
     DeprecatedCompiledClass,
     EntryPointType,
@@ -35,15 +36,15 @@
     InvokeFunction,
 )
 from starkware.starknet.services.api.gateway.transaction_utils import (
     compress_program,
     decompress_program,
 )
 from starkware.starkware_utils.error_handling import StarkException
-from typing_extensions import Literal, TypedDict
+from typing_extensions import Literal, NotRequired, TypedDict
 
 from starknet_devnet.blueprints.rpc.structures.types import (
     Address,
     BlockHash,
     BlockNumber,
     Felt,
     NumAsHex,
@@ -493,17 +494,24 @@
     )
 
 
 def make_declare(
     declare_transaction: RpcBroadcastedDeclareTxn,
 ) -> Union[Declare, DeprecatedDeclare]:
     """Convert RpcBroadcastedDeclareTxn to Declare or DeprecatedDeclare"""
-    if int(declare_transaction["version"], 0) == SUPPORTED_RPC_DECLARE_TX_VERSION:
+    version = int(declare_transaction["version"], 0)
+    if version in (
+        SUPPORTED_RPC_DECLARE_TX_VERSION,
+        SUPPORTED_RPC_DECLARE_TX_VERSION + QUERY_VERSION_BASE,
+    ):
         return make_declare_v2(declare_transaction)
-    if int(declare_transaction["version"], 0) == DEPRECATED_RPC_DECLARE_TX_VERSION:
+    if version in (
+        DEPRECATED_RPC_DECLARE_TX_VERSION,
+        DEPRECATED_RPC_DECLARE_TX_VERSION + QUERY_VERSION_BASE,
+    ):
         return make_declare_v1(declare_transaction)
 
     raise RpcError(
         code=-1,
         message=f"Declare transaction version {declare_transaction['version']} is not supported by devnet",
     )
 
@@ -573,24 +581,25 @@
 
 
 class StructMember(TypedDict):
     """TypedDict for StructMember"""
 
     name: str
     type: str
-    offset: int
+    offset: Optional[int]
 
 
 class FunctionAbiEntry(TypedDict):
     """TypedDict for FunctionAbiEntry"""
 
     type: FunctionAbiType
     name: str
     inputs: List[TypedParameter]
     outputs: List[TypedParameter]
+    stateMutability: NotRequired[Literal["view"]]
 
 
 class EventAbiEntry(TypedDict):
     """TypedDict for EventAbiEntry"""
 
     type: EventAbiType
     name: str
@@ -610,21 +619,26 @@
 AbiEntry = Union[FunctionAbiEntry, EventAbiEntry, StructAbiEntry]
 
 
 def function_abi_entry(abi_entry: AbiEntryType) -> FunctionAbiEntry:
     """
     Convert function gateway abi entry to rpc FunctionAbiEntry
     """
-    return FunctionAbiEntry(
+    rpc_function_abi_entry = FunctionAbiEntry(
         type=abi_entry["type"],
         name=abi_entry["name"],
         inputs=abi_entry["inputs"],
         outputs=abi_entry["outputs"],
     )
 
+    if "stateMutability" in abi_entry:
+        rpc_function_abi_entry["stateMutability"] = abi_entry["stateMutability"]
+
+    return rpc_function_abi_entry
+
 
 def struct_abi_entry(abi_entry: AbiEntryType) -> StructAbiEntry:
     """
     Convert struct gateway abi entry to rpc StructAbiEntry
     """
     return StructAbiEntry(
         type=abi_entry["type"],
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/structures/responses.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/responses.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/structures/types.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/structures/types.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/transactions.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/transactions.py`

 * *Files 3% similar despite different names*

```diff
@@ -123,14 +123,26 @@
     """
     if int(declare_transaction["version"], 0) == LEGACY_TX_VERSION:
         raise RpcError.from_spec_name("INVALID_CONTRACT_CLASS")
 
     class_hash, transaction_hash = await state.starknet_wrapper.declare(
         external_tx=make_declare(declare_transaction)
     )
+    status_response = await state.starknet_wrapper.transactions.get_transaction_status(
+        hex(transaction_hash)
+    )
+
+    if status_response["tx_status"] == "REJECTED":
+        error_message = status_response["tx_failure_reason"].error_message
+        if (
+            "Class with hash" in error_message
+            and "is already declared" in error_message
+        ):
+            raise RpcError.from_spec_name("CLASS_ALREADY_DECLARED")
+
     return RpcDeclareTransactionResult(
         transaction_hash=rpc_felt(transaction_hash),
         class_hash=rpc_felt(class_hash),
     )
 
 
 @validate_schema("addDeployAccountTransaction")
@@ -189,15 +201,15 @@
         _, fee_response = await state.starknet_wrapper.calculate_traces_and_fees(
             transactions,
             skip_validate=False,
             block_id=block_id,
         )
     except StarkException as ex:
         if "Entry point" in ex.message and "not found" in ex.message:
-            raise RpcError.from_spec_name("INVALID_MESSAGE_SELECTOR") from ex
+            raise RpcError.from_spec_name("CONTRACT_ERROR") from ex
         if "While handling calldata" in ex.message:
-            raise RpcError.from_spec_name("INVALID_CALL_DATA") from ex
+            raise RpcError.from_spec_name("CONTRACT_ERROR") from ex
         if "is not deployed" in ex.message:
             raise RpcError.from_spec_name("CONTRACT_NOT_FOUND") from ex
         raise RpcError(code=-1, message=ex.message) from ex
 
     return rpc_fee_estimate(fee_response)
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/rpc/utils.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/blueprints/shared.py` & `starknet_devnet-0.5.3/starknet_devnet/blueprints/shared.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/cairo_rs_py_patch.py` & `starknet_devnet-0.5.3/starknet_devnet/cairo_rs_py_patch.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/chargeable_account.py` & `starknet_devnet-0.5.3/starknet_devnet/chargeable_account.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/compiler.py` & `starknet_devnet-0.5.3/starknet_devnet/compiler.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,35 +25,37 @@
     """Base class of contract class compilers"""
 
     def compile_contract_class(self, contract_class: ContractClass) -> CompiledClass:
         """Take the sierra and return the compiled instance"""
         raise NotImplementedError
 
 
+COMPILATION_ERROR_MSG = """
+Failed compilation from Sierra to Casm! Make sure you compiled the contract with the same compiler version Devnet is using for recompilation.
+Find more info in https://0xspaceshard.github.io/starknet-devnet/docs/guide/cairo1-support/"""
+
+
 class DefaultContractClassCompiler(ContractClassCompiler):
     """Uses the default internal cairo-lang compiler"""
 
     def compile_contract_class(self, contract_class: ContractClass) -> CompiledClass:
-        custom_err_msg = """
-Failed compilation from Sierra to Casm! Read more about starting Devnet with --cairo-compiler-manifest or --sierra-compiler-path"""
-
         try:
             return compile_contract_class(
                 contract_class,
                 compiler_args="--add-pythonic-hints --allowed-libfuncs-list-name experimental_v0.1.0",
             )
         except PermissionError as permission_error:
             raise StarknetDevnetException(
                 code=StarknetErrorCode.COMPILATION_FAILED,
-                message=permission_error + custom_err_msg,
+                message=str(permission_error) + COMPILATION_ERROR_MSG,
             ) from permission_error
         except StarkException as stark_exception:
             raise StarknetDevnetException(
-                code=stark_exception.code,
-                message=stark_exception.message + custom_err_msg,
+                code=StarknetErrorCode.COMPILATION_FAILED,
+                message=(stark_exception.message or "") + COMPILATION_ERROR_MSG,
             ) from stark_exception
 
 
 class CustomContractClassCompiler(ContractClassCompiler):
     """Uses the compiler according to the compiler_manifest provided in initialization"""
 
     @abstractmethod
@@ -81,15 +83,15 @@
             compilation = subprocess.run(
                 compilation_args, capture_output=True, check=False
             )
             if compilation.returncode:
                 stderr = compilation.stderr.decode("utf-8")
                 raise StarknetDevnetException(
                     code=StarknetErrorCode.UNEXPECTED_FAILURE,
-                    message=f"Failed compilation to casm! {stderr}",
+                    message=f"{stderr} {COMPILATION_ERROR_MSG}",
                 )
 
             with open(contract_casm, encoding="utf-8") as casm_file:
                 compiled_class = CompiledClass.loads(casm_file.read())
             return compiled_class
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/constants.py` & `starknet_devnet-0.5.3/starknet_devnet/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 OLD_SUPPORTED_VERSIONS = [0]
 
 # account used by Starknet CLI; calculated using
 # poetry run python scripts/compute_compiled_class_hash.py \
 #   ~/.cache/pypoetry/virtualenvs/<YOUR_VENV>/lib/python3.9/site-packages/starkware/starknet/third_party/open_zeppelin/account.json
 STARKNET_CLI_ACCOUNT_CLASS_HASH = (
-    0x1D28D8D8874CEA14193F70EDCDF501F9AE137BE2A41E258A29CBD05558D8EB6
+    0x7AB95E820D92B974797C8F139AD72F8550ADAA068FEBE4E38DA9A4A9539A81D
 )
 
 # starkware.starknet.public.abi.get_selector_from_name("replace_class")
 REPLACE_CLASS_SELECTOR = (
     0x217DF192877EED2921E241046523F8D8DA7981F0A3DDAFE0E7517F6523276D2
 )
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/contract_class_wrapper.py` & `starknet_devnet-0.5.3/starknet_devnet/contract_class_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/devnet_config.py` & `starknet_devnet-0.5.3/starknet_devnet/devnet_config.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/dump.py` & `starknet_devnet-0.5.3/starknet_devnet/dump.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/fee_token.py` & `starknet_devnet-0.5.3/starknet_devnet/fee_token.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/forked_state.py` & `starknet_devnet-0.5.3/starknet_devnet/forked_state.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,14 +61,41 @@
         self,
         feeder_gateway_client: FeederGatewayClient,
         block_number: int,
     ):
         self.__feeder_gateway_client = feeder_gateway_client
         self.__block_number = block_number
 
+    async def get_compiled_class_by_class_hash(
+        self, class_hash: int
+    ) -> CompiledClassBase:
+        """
+        Returns the compiled class of the given class hash. Handles both class versions.
+        """
+        # nothing is fetched by this value, it's just used to determine if cairo 0 or 1
+        compiled_class_hash = await self.get_compiled_class_hash(class_hash=class_hash)
+        if compiled_class_hash != 0:
+            # The class appears in the class commitment tree, it must be of version > 0.
+            # But it's not present locally if we are here
+            compiled_class = await self.get_compiled_class(
+                compiled_class_hash=class_hash
+            )
+            assert isinstance(
+                compiled_class, CompiledClass
+            ), "Class of version 0 cannot be committed."
+        else:
+            # The class is not committed; treat it as version 0.
+            # Note that 'get_compiled_class' should fail if it's not declared.
+            compiled_class = await self._get_class_by_hash(class_hash=class_hash)
+            assert isinstance(
+                compiled_class, DeprecatedCompiledClass
+            ), "Class of version > 0 must be committed."
+
+        return compiled_class
+
     async def _get_class_by_hash(self, class_hash: int) -> CompiledClassBase:
         try:
             with suppress_feeder_gateway_client_logger:
                 class_dict = await self.__feeder_gateway_client.get_class_by_hash(
                     class_hash=hex(class_hash), block_number=self.__block_number
                 )
             return _load_compiled_class(class_dict)
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/general_config.py` & `starknet_devnet-0.5.3/starknet_devnet/general_config.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/origin.py` & `starknet_devnet-0.5.3/starknet_devnet/origin.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/postman_wrapper.py` & `starknet_devnet-0.5.3/starknet_devnet/postman_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
             "address": self.__postman_wrapper.mock_starknet_messaging_contract.address,
         }
 
     async def flush(self, state) -> Tuple[dict, list]:
         """Handles all pending L1 <> L2 messages and sends them to the other layer."""
 
         if self.__postman_wrapper is None:
-            return {}
+            return ({}, [])
 
         postman = self.__postman_wrapper.postman
 
         l1_to_l2_messages = json.loads(
             Web3.to_json(
                 self.__postman_wrapper.l1_to_l2_message_filter.get_new_entries()
             )
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/predeployed_contract_wrapper.py` & `starknet_devnet-0.5.3/starknet_devnet/predeployed_contract_wrapper.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/server.py` & `starknet_devnet-0.5.3/starknet_devnet/server.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/starknet_wrapper.py` & `starknet_devnet-0.5.3/starknet_devnet/starknet_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,14 +172,15 @@
             await self.accounts.deploy()
             await self.__deploy_chargeable_account()
             await self.__predeclare_starknet_cli_account()
             await self.__udc.deploy()
 
             await self.__preserve_current_state(starknet.state.state)
             await self.__create_genesis_block()
+            self.__latest_state = self.get_state().copy()
             self.__initialized = True
 
     async def __create_genesis_block(self):
         """Create genesis block"""
         transactions: List[DevnetTransaction] = []
         transaction_hash = 1
 
@@ -647,16 +648,24 @@
     async def get_compiled_class_by_class_hash(self, class_hash: int) -> CompiledClass:
         """
         Return compiled class given the class hash (sierra hash).
         Should report an undeclared class if given the hash of a deprecated class
         """
         state = self.get_state().state
 
+        # first handle the case of artifact being locally present
+        if class_hash in self._contract_classes:
+            compiled_class_hash = await state.get_compiled_class_hash(class_hash)
+            return await state.get_compiled_class(compiled_class_hash)
+
         try:
-            compiled_class = await state.get_compiled_class_by_class_hash(class_hash)
+            # directly on state_reader to ensure overridden method is called if forking
+            compiled_class = await state.state_reader.get_compiled_class_by_class_hash(
+                class_hash
+            )
             if isinstance(compiled_class, CompiledClass):
                 return compiled_class
         except AssertionError:
             # the received hash is compiled_class_hash of a cairo1 class
             pass
 
         raise UndeclaredClassDevnetException(class_hash)
@@ -756,27 +765,28 @@
 
     async def postman_flush(self) -> dict:
         """Handles all pending L1 <> L2 messages and sends them to the other layer."""
 
         state = self.get_state()
         # Generate transactions in PostmanWrapper
         parsed_l1_l2_messages, transactions_to_execute = await self.l1l2.flush(state)
+        tx_hashes = []
 
         # Execute transactions inside StarknetWrapper
-        tx_hashes = []
-        for transaction in transactions_to_execute:
-            tx_hashes.append(hex(transaction.hash_value))
-            async with self.__get_transaction_handler() as tx_handler:
-                tx_handler.internal_tx = transaction
-                tx_handler.execution_info = await state.execute_tx(
-                    tx_handler.internal_tx
-                )
-                tx_handler.internal_calls = (
-                    tx_handler.execution_info.call_info.internal_calls
-                )
+        if parsed_l1_l2_messages and transactions_to_execute:
+            for transaction in transactions_to_execute:
+                tx_hashes.append(hex(transaction.hash_value))
+                async with self.__get_transaction_handler() as tx_handler:
+                    tx_handler.internal_tx = transaction
+                    tx_handler.execution_info = await state.execute_tx(
+                        tx_handler.internal_tx
+                    )
+                    tx_handler.internal_calls = (
+                        tx_handler.execution_info.call_info.internal_calls
+                    )
 
         parsed_l1_l2_messages["generated_l2_transactions"] = tx_hashes
         return parsed_l1_l2_messages
 
     async def update_pending_block(self, state_update: BlockStateUpdate = None):
         """Update pending block"""
         await self.blocks.generate_pending(
```

### Comparing `starknet_devnet-0.5.2/starknet_devnet/state.py` & `starknet_devnet-0.5.3/starknet_devnet/state.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/state_archive.py` & `starknet_devnet-0.5.3/starknet_devnet/state_archive.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/transactions.py` & `starknet_devnet-0.5.3/starknet_devnet/transactions.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/udc.py` & `starknet_devnet-0.5.3/starknet_devnet/udc.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/starknet_devnet/util.py` & `starknet_devnet-0.5.3/starknet_devnet/util.py`

 * *Files identical despite different names*

### Comparing `starknet_devnet-0.5.2/setup.py` & `starknet_devnet-0.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 package_data = \
 {'': ['*'],
  'starknet_devnet': ['accounts_artifacts/OpenZeppelin/0.5.1/Account.cairo/*']}
 
 install_requires = \
 ['Flask[async]>=2.0.3,<2.1.0',
  'Werkzeug>=2.0.3,<2.1.0',
- 'cairo-lang==0.11.1.1',
+ 'cairo-lang==0.11.2',
  'cloudpickle>=2.1.0,<2.2.0',
  'crypto-cpp-py>=1.4.0,<1.5.0',
  'flask-cors>=3.0.10,<3.1.0',
  'gunicorn>=20.1.0,<20.2.0',
  'jsonschema>=4.17.0,<4.18.0',
  'marshmallow-dataclass>=8.4,<8.5',
  'marshmallow>=3.17.0,<3.18.0',
@@ -27,15 +27,15 @@
  'web3>=6.0.0,<6.1.0']
 
 entry_points = \
 {'console_scripts': ['starknet-devnet = starknet_devnet.server:main']}
 
 setup_kwargs = {
     'name': 'starknet-devnet',
-    'version': '0.5.2',
+    'version': '0.5.3',
     'description': 'A local testnet for Starknet',
     'long_description': '<!-- logo / title -->\n<p align="center" style="margin-bottom: 0px !important">\n  <img width="200" src="https://user-images.githubusercontent.com/2848732/193076972-da6fa36e-11f7-4cb3-aa29-673224f8576d.png" alt="Devnet" align="center">\n</p>\n<h1 align="center" style="margin-top: 0px !important">Starknet Devnet</h1>\n\nA Flask wrapper of Starknet state. Similar in purpose to Ganache.\n\nAims to mimic Starknet\'s Alpha testnet, but with simplified functionality.\n\n## 🌐 Docs\n\nOn the following links you can find the documentation of:\n\n- [the latest official release](https://0xspaceshard.github.io/starknet-devnet/)\n- [the latest master commit (not officially released)](https://github.com/0xSpaceShard/starknet-devnet/tree/master/page/docs)\n\n## ✏️ Contributing\n\nWe ❤️ and encourage all contributions!\n\n[Click here](https://0xspaceshard.github.io/starknet-devnet/docs/guide/development) for the development guide.\n\n## 🙌 Special Thanks\n\nSpecial thanks to all the [contributors](https://github.com/0xSpaceShard/starknet-devnet/graphs/contributors)!\n',
     'author': 'FabijanC',
     'author_email': 'fabijan.corak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/0xSpaceShard/starknet-devnet',
```

### Comparing `starknet_devnet-0.5.2/PKG-INFO` & `starknet_devnet-0.5.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: starknet-devnet
-Version: 0.5.2
+Version: 0.5.3
 Summary: A local testnet for Starknet
 Home-page: https://github.com/0xSpaceShard/starknet-devnet
 License: MIT
 Keywords: starknet,cairo,testnet,local,server
 Author: FabijanC
 Author-email: fabijan.corak@gmail.com
 Requires-Python: >=3.9,<3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask[async] (>=2.0.3,<2.1.0)
 Requires-Dist: Werkzeug (>=2.0.3,<2.1.0)
-Requires-Dist: cairo-lang (==0.11.1.1)
+Requires-Dist: cairo-lang (==0.11.2)
 Requires-Dist: cloudpickle (>=2.1.0,<2.2.0)
 Requires-Dist: crypto-cpp-py (>=1.4.0,<1.5.0)
 Requires-Dist: flask-cors (>=3.0.10,<3.1.0)
 Requires-Dist: gunicorn (>=20.1.0,<20.2.0)
 Requires-Dist: jsonschema (>=4.17.0,<4.18.0)
 Requires-Dist: marshmallow (>=3.17.0,<3.18.0)
 Requires-Dist: marshmallow-dataclass (>=8.4,<8.5)
```

