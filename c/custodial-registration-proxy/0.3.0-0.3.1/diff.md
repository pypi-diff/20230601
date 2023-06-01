# Comparing `tmp/custodial-registration-proxy-0.3.0.tar.gz` & `tmp/custodial-registration-proxy-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodial-registration-proxy-0.3.0.tar", last modified: Thu Jun  1 05:26:16 2023, max compression
+gzip compressed data, was "custodial-registration-proxy-0.3.1.tar", last modified: Thu Jun  1 05:32:19 2023, max compression
```

## Comparing `custodial-registration-proxy-0.3.0.tar` & `custodial-registration-proxy-0.3.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 05:26:16.598795 custodial-registration-proxy-0.3.0/
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       24 2023-06-01 05:22:15.000000 custodial-registration-proxy-0.3.0/MANIFEST.in
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      903 2023-06-01 05:26:16.598795 custodial-registration-proxy-0.3.0/PKG-INFO
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      329 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.3.0/README.md
-drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 05:26:16.597795 custodial-registration-proxy-0.3.0/custodial_registration_proxy/
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      122 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.3.0/custodial_registration_proxy/__init__.py
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     2181 2023-05-29 14:48:29.000000 custodial-registration-proxy-0.3.0/custodial_registration_proxy/custodial_registration_proxy.py
-drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 05:26:16.598795 custodial-registration-proxy-0.3.0/custodial_registration_proxy/runnable/
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     3824 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.3.0/custodial_registration_proxy/runnable/publish.py
-drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 05:26:16.598795 custodial-registration-proxy-0.3.0/custodial_registration_proxy.egg-info/
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      903 2023-06-01 05:26:16.000000 custodial-registration-proxy-0.3.0/custodial_registration_proxy.egg-info/PKG-INFO
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      522 2023-06-01 05:26:16.000000 custodial-registration-proxy-0.3.0/custodial_registration_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)        1 2023-06-01 05:26:16.000000 custodial-registration-proxy-0.3.0/custodial_registration_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      112 2023-06-01 05:26:16.000000 custodial-registration-proxy-0.3.0/custodial_registration_proxy.egg-info/entry_points.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       38 2023-06-01 05:26:16.000000 custodial-registration-proxy-0.3.0/custodial_registration_proxy.egg-info/requires.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       29 2023-06-01 05:26:16.000000 custodial-registration-proxy-0.3.0/custodial_registration_proxy.egg-info/top_level.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       37 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.3.0/requirements.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     1199 2023-06-01 05:26:16.599795 custodial-registration-proxy-0.3.0/setup.cfg
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      383 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.3.0/setup.py
+drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 05:32:19.230431 custodial-registration-proxy-0.3.1/
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       24 2023-06-01 05:22:15.000000 custodial-registration-proxy-0.3.1/MANIFEST.in
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      903 2023-06-01 05:32:19.230431 custodial-registration-proxy-0.3.1/PKG-INFO
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      329 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.3.1/README.md
+drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 05:32:19.229431 custodial-registration-proxy-0.3.1/custodial_registration_proxy/
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      122 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.3.1/custodial_registration_proxy/__init__.py
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     2181 2023-05-29 14:48:29.000000 custodial-registration-proxy-0.3.1/custodial_registration_proxy/custodial_registration_proxy.py
+drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 05:32:19.230431 custodial-registration-proxy-0.3.1/custodial_registration_proxy/runnable/
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     3520 2023-06-01 05:30:38.000000 custodial-registration-proxy-0.3.1/custodial_registration_proxy/runnable/publish.py
+drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 05:32:19.229431 custodial-registration-proxy-0.3.1/custodial_registration_proxy.egg-info/
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      903 2023-06-01 05:32:19.000000 custodial-registration-proxy-0.3.1/custodial_registration_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      522 2023-06-01 05:32:19.000000 custodial-registration-proxy-0.3.1/custodial_registration_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)        1 2023-06-01 05:32:19.000000 custodial-registration-proxy-0.3.1/custodial_registration_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      112 2023-06-01 05:32:19.000000 custodial-registration-proxy-0.3.1/custodial_registration_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       38 2023-06-01 05:32:19.000000 custodial-registration-proxy-0.3.1/custodial_registration_proxy.egg-info/requires.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       29 2023-06-01 05:32:19.000000 custodial-registration-proxy-0.3.1/custodial_registration_proxy.egg-info/top_level.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       37 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.3.1/requirements.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     1199 2023-06-01 05:32:19.230431 custodial-registration-proxy-0.3.1/setup.cfg
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      383 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.3.1/setup.py
```

### Comparing `custodial-registration-proxy-0.3.0/PKG-INFO` & `custodial-registration-proxy-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: custodial-registration-proxy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 Home-page: https://github.com/grassrootseconomics/custodial-registration-proxy
 Author: Mohamed Sohail
 Author-email: sohail@grassecon.org
 License: AGPLv3+
 Description: Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 Keywords: ethereum
```

### Comparing `custodial-registration-proxy-0.3.0/custodial_registration_proxy/custodial_registration_proxy.py` & `custodial-registration-proxy-0.3.1/custodial_registration_proxy/custodial_registration_proxy.py`

 * *Files identical despite different names*

### Comparing `custodial-registration-proxy-0.3.0/custodial_registration_proxy/runnable/publish.py` & `custodial-registration-proxy-0.3.1/custodial_registration_proxy/runnable/publish.py`

 * *Files 11% similar despite different names*

```diff
@@ -39,27 +39,25 @@
 
 logging.basicConfig(level=logging.WARNING)
 logg = logging.getLogger()
 
 def process_config_local(config, arg, args, flags):
     config.add(args.proxy_eth_faucet_address, 'PROXY_ETH_FAUCET_ADDRESS')
     config.add(args.proxy_custodial_account_index_address, 'PROXY_CUSTODIAL_ACCOUNT_INDEX_ADDRESS')
-    config.add(args.proxy_training_voucher_address, 'PROXY_TRAINING_VOUCHER_ADDRESS')
     config.add(args.proxy_system_account_address, 'PROXY_SYSTEM_ACCOUNT_ADDRESS')
     return config
 
 arg_flags = ArgFlag()
 arg = Arg(arg_flags)
 flags = arg_flags.STD_WRITE 
 
 argparser = chainlib.eth.cli.ArgumentParser()
 argparser = process_args(argparser, arg, flags)
 argparser.add_argument('--eth-faucet-address', dest='proxy_eth_faucet_address', type=str, help='Faucet address')
 argparser.add_argument('--account-index-address', dest='proxy_custodial_account_index_address', type=str, help='Account index address')
-argparser.add_argument('--training-voucher-address', dest='proxy_training_voucher_address', type=str, help='Training voucher address')
 argparser.add_argument('--system-account-address', dest='proxy_system_account_address', type=str, help='System account address')
 args = argparser.parse_args()
 
 logg = process_log(args, logg)
 
 config = Config()
 config = process_config(config, arg, args, flags)
@@ -80,15 +78,14 @@
             gas_oracle=settings.get('FEE_ORACLE'),
             nonce_oracle=settings.get('NONCE_ORACLE'),
             )
 
     c_args = CustodialRegistrationProxySettings()
     c_args.eth_faucet_address = config.get('PROXY_ETH_FAUCET_ADDRESS')
     c_args.custodial_account_index_address = config.get('PROXY_CUSTODIAL_ACCOUNT_INDEX_ADDRESS')
-    c_args.training_voucher_address = config.get('PROXY_TRAINING_VOUCHER_ADDRESS')
     c_args.system_account_address = config.get('PROXY_SYSTEM_ACCOUNT_ADDRESS')
 
     (tx_hash_hex, o) = c.constructor(
             settings.get('SENDER_ADDRESS'),
             c_args,
             )
```

### Comparing `custodial-registration-proxy-0.3.0/custodial_registration_proxy.egg-info/PKG-INFO` & `custodial-registration-proxy-0.3.1/custodial_registration_proxy.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: custodial-registration-proxy
-Version: 0.3.0
+Version: 0.3.1
 Summary: Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 Home-page: https://github.com/grassrootseconomics/custodial-registration-proxy
 Author: Mohamed Sohail
 Author-email: sohail@grassecon.org
 License: AGPLv3+
 Description: Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 Keywords: ethereum
```

### Comparing `custodial-registration-proxy-0.3.0/custodial_registration_proxy.egg-info/SOURCES.txt` & `custodial-registration-proxy-0.3.1/custodial_registration_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `custodial-registration-proxy-0.3.0/setup.cfg` & `custodial-registration-proxy-0.3.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = custodial-registration-proxy
-version = 0.3.0
+version = 0.3.1
 description = Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 long_description = Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 author = Mohamed Sohail
 author_email = sohail@grassecon.org
 url = https://github.com/grassrootseconomics/custodial-registration-proxy
 keywords = 
 	ethereum
```

