# Comparing `tmp/custodial-registration-proxy-0.1.0.tar.gz` & `tmp/custodial-registration-proxy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "custodial-registration-proxy-0.1.0.tar", last modified: Sat Mar 25 10:45:09 2023, max compression
+gzip compressed data, was "custodial-registration-proxy-0.2.0.tar", last modified: Thu Jun  1 04:56:14 2023, max compression
```

## Comparing `custodial-registration-proxy-0.1.0.tar` & `custodial-registration-proxy-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,17 @@
-drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-03-25 10:45:09.671495 custodial-registration-proxy-0.1.0/
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)    34522 2023-03-25 07:14:10.000000 custodial-registration-proxy-0.1.0/LICENSE
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      895 2023-03-25 10:45:09.672495 custodial-registration-proxy-0.1.0/PKG-INFO
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      329 2023-03-25 08:42:04.000000 custodial-registration-proxy-0.1.0/README.md
-drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-03-25 10:45:09.667495 custodial-registration-proxy-0.1.0/custodial_registration_proxy/
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      122 2023-03-25 09:49:07.000000 custodial-registration-proxy-0.1.0/custodial_registration_proxy/__init__.py
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     2281 2023-03-25 10:16:10.000000 custodial-registration-proxy-0.1.0/custodial_registration_proxy/custodial_registration_proxy.py
-drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-03-25 10:45:09.670495 custodial-registration-proxy-0.1.0/custodial_registration_proxy/data/
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     6028 2023-03-25 08:57:06.000000 custodial-registration-proxy-0.1.0/custodial_registration_proxy/data/CustodialRegistrationProxy.bin
-drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-03-25 10:45:09.671495 custodial-registration-proxy-0.1.0/custodial_registration_proxy/runnable/
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     3824 2023-03-25 10:10:07.000000 custodial-registration-proxy-0.1.0/custodial_registration_proxy/runnable/publish.py
-drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-03-25 10:45:09.669495 custodial-registration-proxy-0.1.0/custodial_registration_proxy.egg-info/
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      895 2023-03-25 10:45:09.000000 custodial-registration-proxy-0.1.0/custodial_registration_proxy.egg-info/PKG-INFO
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      566 2023-03-25 10:45:09.000000 custodial-registration-proxy-0.1.0/custodial_registration_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)        1 2023-03-25 10:45:09.000000 custodial-registration-proxy-0.1.0/custodial_registration_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      111 2023-03-25 10:45:09.000000 custodial-registration-proxy-0.1.0/custodial_registration_proxy.egg-info/entry_points.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       38 2023-03-25 10:45:09.000000 custodial-registration-proxy-0.1.0/custodial_registration_proxy.egg-info/requires.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       29 2023-03-25 10:45:09.000000 custodial-registration-proxy-0.1.0/custodial_registration_proxy.egg-info/top_level.txt
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     1199 2023-03-25 10:45:09.673495 custodial-registration-proxy-0.1.0/setup.cfg
--rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      383 2023-03-25 10:22:10.000000 custodial-registration-proxy-0.1.0/setup.py
+drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 04:56:14.331634 custodial-registration-proxy-0.2.0/
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      903 2023-06-01 04:56:14.331634 custodial-registration-proxy-0.2.0/PKG-INFO
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      329 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.2.0/README.md
+drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 04:56:14.330634 custodial-registration-proxy-0.2.0/custodial_registration_proxy/
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      122 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.2.0/custodial_registration_proxy/__init__.py
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     2181 2023-05-29 14:48:29.000000 custodial-registration-proxy-0.2.0/custodial_registration_proxy/custodial_registration_proxy.py
+drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 04:56:14.331634 custodial-registration-proxy-0.2.0/custodial_registration_proxy/runnable/
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     3824 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.2.0/custodial_registration_proxy/runnable/publish.py
+drwxr-xr-x   0 kamikaze  (1000) kamikaze  (1000)        0 2023-06-01 04:56:14.331634 custodial-registration-proxy-0.2.0/custodial_registration_proxy.egg-info/
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      903 2023-06-01 04:56:14.000000 custodial-registration-proxy-0.2.0/custodial_registration_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      493 2023-06-01 04:56:14.000000 custodial-registration-proxy-0.2.0/custodial_registration_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)        1 2023-06-01 04:56:14.000000 custodial-registration-proxy-0.2.0/custodial_registration_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      112 2023-06-01 04:56:14.000000 custodial-registration-proxy-0.2.0/custodial_registration_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       38 2023-06-01 04:56:14.000000 custodial-registration-proxy-0.2.0/custodial_registration_proxy.egg-info/requires.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)       29 2023-06-01 04:56:14.000000 custodial-registration-proxy-0.2.0/custodial_registration_proxy.egg-info/top_level.txt
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)     1199 2023-06-01 04:56:14.332635 custodial-registration-proxy-0.2.0/setup.cfg
+-rw-r--r--   0 kamikaze  (1000) kamikaze  (1000)      383 2023-05-29 14:37:27.000000 custodial-registration-proxy-0.2.0/setup.py
```

### Comparing `custodial-registration-proxy-0.1.0/PKG-INFO` & `custodial-registration-proxy-0.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: custodial-registration-proxy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 Home-page: https://github.com/grassrootseconomics/custodial-registration-proxy
 Author: Mohamed Sohail
 Author-email: sohail@grassecon.org
 License: AGPLv3+
+Description: Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 Keywords: ethereum
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
-License-File: LICENSE
-
-Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
```

### Comparing `custodial-registration-proxy-0.1.0/custodial_registration_proxy/custodial_registration_proxy.py` & `custodial-registration-proxy-0.2.0/custodial_registration_proxy/custodial_registration_proxy.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 moddir = os.path.dirname(__file__)
 datadir = os.path.join(moddir, 'data')
 
 class CustodialRegistrationProxySettings:
     def __init__(self):
         self.eth_faucet_address = None
         self.custodial_account_index_address = None
-        self.training_voucher_address = None
         self.system_account_address = None
 
 class CustodialRegistrationProxy(TxFactory):
     __abi = None
     __bytecode = None
 
     @staticmethod
@@ -57,13 +56,12 @@
         return 2000000
 
     def constructor(self, sender_address, settings):
         code = CustodialRegistrationProxy.bytecode()
         enc = ABIContractEncoder()
         enc.address(settings.eth_faucet_address)
         enc.address(settings.custodial_account_index_address)
-        enc.address(settings.training_voucher_address)
         enc.address(settings.system_account_address)
         code += enc.get()
         tx = self.template(sender_address, None, use_nonce=True)
         tx = self.set_code(tx, code)
         return self.build(tx)
```

### Comparing `custodial-registration-proxy-0.1.0/custodial_registration_proxy/runnable/publish.py` & `custodial-registration-proxy-0.2.0/custodial_registration_proxy/runnable/publish.py`

 * *Files identical despite different names*

### Comparing `custodial-registration-proxy-0.1.0/custodial_registration_proxy.egg-info/PKG-INFO` & `custodial-registration-proxy-0.2.0/custodial_registration_proxy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: custodial-registration-proxy
-Version: 0.1.0
+Version: 0.2.0
 Summary: Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 Home-page: https://github.com/grassrootseconomics/custodial-registration-proxy
 Author: Mohamed Sohail
 Author-email: sohail@grassecon.org
 License: AGPLv3+
+Description: Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 Keywords: ethereum
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
-License-File: LICENSE
-
-Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
```

### Comparing `custodial-registration-proxy-0.1.0/setup.cfg` & `custodial-registration-proxy-0.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = custodial-registration-proxy
-version = 0.1.0
+version = 0.2.0
 description = Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 long_description = Atomically registers a custodial user on-chain and provisions necessary gas and training vouchers.
 author = Mohamed Sohail
 author_email = sohail@grassecon.org
 url = https://github.com/grassrootseconomics/custodial-registration-proxy
 keywords = 
 	ethereum
```

