# Comparing `tmp/gopay-1.3.0.tar.gz` & `tmp/gopay-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gopay-1.3.0.tar", last modified: Thu Jan 12 14:29:51 2023, max compression
+gzip compressed data, was "gopay-1.3.1.tar", last modified: Thu Jun  1 10:15:51 2023, max compression
```

## Comparing `gopay-1.3.0.tar` & `gopay-1.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 standa    (1000) standa    (1000)        0 2023-01-12 14:29:51.015463 gopay-1.3.0/
--rw-rw-r--   0 standa    (1000) standa    (1000)      113 2022-08-10 10:38:48.000000 gopay-1.3.0/CHANGELOG.md
--rw-rw-r--   0 standa    (1000) standa    (1000)     1075 2022-08-10 10:38:48.000000 gopay-1.3.0/LICENSE
--rw-rw-r--   0 standa    (1000) standa    (1000)       50 2022-08-10 10:38:48.000000 gopay-1.3.0/MANIFEST.in
--rw-rw-r--   0 standa    (1000) standa    (1000)     8960 2023-01-12 14:29:51.015463 gopay-1.3.0/PKG-INFO
--rw-rw-r--   0 standa    (1000) standa    (1000)     8195 2022-08-10 10:38:48.000000 gopay-1.3.0/README.md
-drwxrwxr-x   0 standa    (1000) standa    (1000)        0 2023-01-12 14:29:51.007463 gopay-1.3.0/gopay/
--rw-rw-r--   0 standa    (1000) standa    (1000)      709 2022-08-10 10:38:48.000000 gopay-1.3.0/gopay/__init__.py
--rw-rw-r--   0 standa    (1000) standa    (1000)     1741 2022-08-10 10:38:48.000000 gopay-1.3.0/gopay/api.py
--rw-rw-r--   0 standa    (1000) standa    (1000)     5156 2023-01-12 14:15:50.000000 gopay-1.3.0/gopay/enums.py
--rw-rw-r--   0 standa    (1000) standa    (1000)     1256 2022-08-10 10:38:48.000000 gopay-1.3.0/gopay/http.py
--rw-rw-r--   0 standa    (1000) standa    (1000)     2220 2022-08-10 10:38:48.000000 gopay-1.3.0/gopay/oauth2.py
--rw-rw-r--   0 standa    (1000) standa    (1000)     4503 2022-08-10 10:38:48.000000 gopay-1.3.0/gopay/payments.py
-drwxrwxr-x   0 standa    (1000) standa    (1000)        0 2023-01-12 14:29:51.015463 gopay-1.3.0/gopay.egg-info/
--rw-rw-r--   0 standa    (1000) standa    (1000)     8960 2023-01-12 14:29:50.000000 gopay-1.3.0/gopay.egg-info/PKG-INFO
--rw-rw-r--   0 standa    (1000) standa    (1000)      299 2023-01-12 14:29:50.000000 gopay-1.3.0/gopay.egg-info/SOURCES.txt
--rw-rw-r--   0 standa    (1000) standa    (1000)        1 2023-01-12 14:29:50.000000 gopay-1.3.0/gopay.egg-info/dependency_links.txt
--rw-rw-r--   0 standa    (1000) standa    (1000)       27 2023-01-12 14:29:50.000000 gopay-1.3.0/gopay.egg-info/requires.txt
--rw-rw-r--   0 standa    (1000) standa    (1000)        6 2023-01-12 14:29:50.000000 gopay-1.3.0/gopay.egg-info/top_level.txt
--rw-rw-r--   0 standa    (1000) standa    (1000)      108 2023-01-12 14:29:51.019463 gopay-1.3.0/setup.cfg
--rw-rw-r--   0 standa    (1000) standa    (1000)     1122 2023-01-12 14:08:54.000000 gopay-1.3.0/setup.py
+drwxrwxr-x   0 sfoldesi  (1000) sfoldesi  (1000)        0 2023-06-01 10:15:51.355308 gopay-1.3.1/
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)      113 2023-06-01 09:31:18.000000 gopay-1.3.1/CHANGELOG.md
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     1075 2023-06-01 09:31:18.000000 gopay-1.3.1/LICENSE
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)       50 2023-06-01 09:31:18.000000 gopay-1.3.1/MANIFEST.in
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     9011 2023-06-01 10:15:51.355308 gopay-1.3.1/PKG-INFO
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     8194 2023-06-01 10:05:29.000000 gopay-1.3.1/README.md
+drwxrwxr-x   0 sfoldesi  (1000) sfoldesi  (1000)        0 2023-06-01 10:15:51.347308 gopay-1.3.1/gopay/
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)      709 2023-06-01 09:31:18.000000 gopay-1.3.1/gopay/__init__.py
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     1741 2023-06-01 09:31:18.000000 gopay-1.3.1/gopay/api.py
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     5762 2023-06-01 10:05:29.000000 gopay-1.3.1/gopay/enums.py
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     1256 2023-06-01 09:31:18.000000 gopay-1.3.1/gopay/http.py
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     2220 2023-06-01 09:31:18.000000 gopay-1.3.1/gopay/oauth2.py
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     4674 2023-06-01 10:05:29.000000 gopay-1.3.1/gopay/payments.py
+drwxrwxr-x   0 sfoldesi  (1000) sfoldesi  (1000)        0 2023-06-01 10:15:51.355308 gopay-1.3.1/gopay.egg-info/
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     9011 2023-06-01 10:15:51.000000 gopay-1.3.1/gopay.egg-info/PKG-INFO
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)      299 2023-06-01 10:15:51.000000 gopay-1.3.1/gopay.egg-info/SOURCES.txt
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)        1 2023-06-01 10:15:51.000000 gopay-1.3.1/gopay.egg-info/dependency_links.txt
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)       27 2023-06-01 10:15:51.000000 gopay-1.3.1/gopay.egg-info/requires.txt
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)        6 2023-06-01 10:15:51.000000 gopay-1.3.1/gopay.egg-info/top_level.txt
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)      108 2023-06-01 10:15:51.355308 gopay-1.3.1/setup.cfg
+-rw-rw-r--   0 sfoldesi  (1000) sfoldesi  (1000)     1173 2023-06-01 10:08:44.000000 gopay-1.3.1/setup.py
```

### Comparing `gopay-1.3.0/LICENSE` & `gopay-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gopay-1.3.0/PKG-INFO` & `gopay-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: gopay
-Version: 1.3.0
+Version: 1.3.1
 Home-page: https://github.com/gopaycommunity/gopay-python-sdk
 Author: GoPay
 Author-email: integrace@gopay.cz
 License: MIT
 Keywords: gopay payments sdk rest api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # GoPay's Python SDK for Payments REST API
 
 [![Build Status](https://travis-ci.org/gopaycommunity/gopay-python-api.svg?branch=master)](https://travis-ci.org/gopaycommunity/gopay-python-api)
 
 ## Requirements
 
-- Python >= 3.6
+- Python >= 3.7
 - dependencies:
-    - [`requests`](https://github.com/kennethreitz/requests)
-    - [`deprecated`](https://github.com/tantale/deprecated)
+  - [`requests`](https://github.com/kennethreitz/requests)
+  - [`deprecated`](https://github.com/tantale/deprecated)
 
 ## Installation
 
 The simplest way to install SDK is to use [PIP](https://docs.python.org/3/installing/):
 
 ```bash
 pip install gopay
@@ -66,48 +67,47 @@
 ### Configuration
 
 #### Required fields
 
 Required field | Data type | Documentation |
 -------------- | --------- | ----------- |
 `goid` | string | default GoPay account used in `createPayment` if `target` is not specified
-`clientId` | string | https://doc.gopay.com/#access-token |
-`clientSecret` | string | https://doc.gopay.com/#access-token |
+`clientId` | string | <https://doc.gopay.com/#access-token> |
+`clientSecret` | string | <https://doc.gopay.com/#access-token> |
 `gatewayUrl` | string | [test or production environment?](https://help.gopay.com/en/s/uY) |
 
 #### Optional fields
 
 Optional field | Data type | Default value | Documentation |
 -------------- | --------- | ------------- | ------------- |
-`scope` | string | [`GoPay\Definition\TokenScope::ALL`](src/Definition/TokenScope.php) | https://doc.gopay.com/#access-token |
+`scope` | string | [`GoPay\Definition\TokenScope::ALL`](src/Definition/TokenScope.php) | <https://doc.gopay.com/#access-token> |
 `language` | string | [`GoPay\Definition\Language::ENGLISH`](src/Definition/Language.php) | language used in `createPayment` if `lang` is not specified + used for [localization of errors](https://doc.gopay.com/#errors)
 `timeout` | int | 30 | Browser timeout in seconds |
 
-
 ### Available methods
 
 API | SDK method |
 --- | ---------- |
 [Create standard payment](https://doc.gopay.com/#payment-creation) | `$gopay->createPayment(array $payment)` |
 [Status of the payment](https://doc.gopay.com/#payment-status) | `$gopay->getStatus($id)` |
 [Refund of the payment](https://doc.gopay.com/#payment-refund) | `$gopay->refundPayment($id, $amount)` |
 [Create recurring payment](https://doc.gopay.com/#recurring-payments) | `$gopay->createPayment(array $payment)` |
 [Recurring payment on demand](https://doc.gopay.com/#recurring-on-demand) | `$gopay->createRecurrence($id, array $payment)` |
 [Cancellation of the recurring payment](https://doc.gopay.com/#recurring-payment-cancellation) | `$gopay->voidRecurrence($id)` |
 [Create pre-authorized payment](https://doc.gopay.com/#preauthorized-payments) | `$gopay->createPayment(array $payment)` |
 [Charge of pre-authorized payment](https://doc.gopay.com/#capturing-a-preauthorized-payment) | `$gopay->captureAuthorization($id)` |
 [Cancellation of the pre-authorized payment](https://doc.gopay.com/#cancelling-a-preauthorized-payment) | `$gopay->voidAuthorization($id)` |
+
 ### SDK response? Has my call succeed?
 
 SDK returns wrapped API response. Every method returns
 [`GoPay\Http\Response` object](src/Http/Response.php). Structure of `json/__toString`
 should be same as in [documentation](https://doc.gopay.com/en).
 SDK throws no exception. Please create an issue if you catch one.
 
-
 ```python
 response = payments.create_payment({...})
 if response.has_succeed():
     print("hooray, API returned " + str(response))
     return response.json['gw_url'] # url for initiation of gateway
 else:
     # errors format: https://doc.gopay.com/en/?shell#http-result-codes
@@ -117,15 +117,14 @@
 Method | Description |
 ------ | ---------- |
 `response.has_succeed()` | checks if API returns status code _200_ |
 `response.json` | decoded response, returned objects are converted into associative arrays |
 `response.status_code` | HTTP status code |
 `response.__str__()` | raw body from HTTP response |
 
-
 ### Are required fields and allowed values validated?
 
 **No.** API [validates fields](https://doc.gopay.com/#error) pretty extensively
 so there is no need to duplicate validation in SDK. It would only introduce new type of error.
 Or we would have to perfectly simulate API error messages. That's why SDK just calls API which
 behavior is well documented in [doc.gopay.com](https://doc.gopay.com).
 
@@ -185,15 +184,14 @@
 
 Your cache must implement template methods `get_token` and `set_token`.
 Be aware that there are two [scopes](https://doc.gopay.com/#access-token) (`TokenScope`) and
 SDK can be used for different clients (`clientId`, `gatewayUrl`). So `client` passed to
 methods is unique identifier (`string`) that is built for current environment.
 Below you can see example implementation of caching tokens in memory:
 
-
 ```python
 # register cache in optional service configuration
 payments = gopay.payments(
     {}, # your config
     {'cache': MyCache()}
 )
 ```
```

### Comparing `gopay-1.3.0/README.md` & `gopay-1.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 
 # GoPay's Python SDK for Payments REST API
 
 [![Build Status](https://travis-ci.org/gopaycommunity/gopay-python-api.svg?branch=master)](https://travis-ci.org/gopaycommunity/gopay-python-api)
 
 ## Requirements
 
-- Python >= 3.6
+- Python >= 3.7
 - dependencies:
-    - [`requests`](https://github.com/kennethreitz/requests)
-    - [`deprecated`](https://github.com/tantale/deprecated)
+  - [`requests`](https://github.com/kennethreitz/requests)
+  - [`deprecated`](https://github.com/tantale/deprecated)
 
 ## Installation
 
 The simplest way to install SDK is to use [PIP](https://docs.python.org/3/installing/):
 
 ```bash
 pip install gopay
@@ -46,48 +46,47 @@
 ### Configuration
 
 #### Required fields
 
 Required field | Data type | Documentation |
 -------------- | --------- | ----------- |
 `goid` | string | default GoPay account used in `createPayment` if `target` is not specified
-`clientId` | string | https://doc.gopay.com/#access-token |
-`clientSecret` | string | https://doc.gopay.com/#access-token |
+`clientId` | string | <https://doc.gopay.com/#access-token> |
+`clientSecret` | string | <https://doc.gopay.com/#access-token> |
 `gatewayUrl` | string | [test or production environment?](https://help.gopay.com/en/s/uY) |
 
 #### Optional fields
 
 Optional field | Data type | Default value | Documentation |
 -------------- | --------- | ------------- | ------------- |
-`scope` | string | [`GoPay\Definition\TokenScope::ALL`](src/Definition/TokenScope.php) | https://doc.gopay.com/#access-token |
+`scope` | string | [`GoPay\Definition\TokenScope::ALL`](src/Definition/TokenScope.php) | <https://doc.gopay.com/#access-token> |
 `language` | string | [`GoPay\Definition\Language::ENGLISH`](src/Definition/Language.php) | language used in `createPayment` if `lang` is not specified + used for [localization of errors](https://doc.gopay.com/#errors)
 `timeout` | int | 30 | Browser timeout in seconds |
 
-
 ### Available methods
 
 API | SDK method |
 --- | ---------- |
 [Create standard payment](https://doc.gopay.com/#payment-creation) | `$gopay->createPayment(array $payment)` |
 [Status of the payment](https://doc.gopay.com/#payment-status) | `$gopay->getStatus($id)` |
 [Refund of the payment](https://doc.gopay.com/#payment-refund) | `$gopay->refundPayment($id, $amount)` |
 [Create recurring payment](https://doc.gopay.com/#recurring-payments) | `$gopay->createPayment(array $payment)` |
 [Recurring payment on demand](https://doc.gopay.com/#recurring-on-demand) | `$gopay->createRecurrence($id, array $payment)` |
 [Cancellation of the recurring payment](https://doc.gopay.com/#recurring-payment-cancellation) | `$gopay->voidRecurrence($id)` |
 [Create pre-authorized payment](https://doc.gopay.com/#preauthorized-payments) | `$gopay->createPayment(array $payment)` |
 [Charge of pre-authorized payment](https://doc.gopay.com/#capturing-a-preauthorized-payment) | `$gopay->captureAuthorization($id)` |
 [Cancellation of the pre-authorized payment](https://doc.gopay.com/#cancelling-a-preauthorized-payment) | `$gopay->voidAuthorization($id)` |
+
 ### SDK response? Has my call succeed?
 
 SDK returns wrapped API response. Every method returns
 [`GoPay\Http\Response` object](src/Http/Response.php). Structure of `json/__toString`
 should be same as in [documentation](https://doc.gopay.com/en).
 SDK throws no exception. Please create an issue if you catch one.
 
-
 ```python
 response = payments.create_payment({...})
 if response.has_succeed():
     print("hooray, API returned " + str(response))
     return response.json['gw_url'] # url for initiation of gateway
 else:
     # errors format: https://doc.gopay.com/en/?shell#http-result-codes
@@ -97,15 +96,14 @@
 Method | Description |
 ------ | ---------- |
 `response.has_succeed()` | checks if API returns status code _200_ |
 `response.json` | decoded response, returned objects are converted into associative arrays |
 `response.status_code` | HTTP status code |
 `response.__str__()` | raw body from HTTP response |
 
-
 ### Are required fields and allowed values validated?
 
 **No.** API [validates fields](https://doc.gopay.com/#error) pretty extensively
 so there is no need to duplicate validation in SDK. It would only introduce new type of error.
 Or we would have to perfectly simulate API error messages. That's why SDK just calls API which
 behavior is well documented in [doc.gopay.com](https://doc.gopay.com).
 
@@ -165,15 +163,14 @@
 
 Your cache must implement template methods `get_token` and `set_token`.
 Be aware that there are two [scopes](https://doc.gopay.com/#access-token) (`TokenScope`) and
 SDK can be used for different clients (`clientId`, `gatewayUrl`). So `client` passed to
 methods is unique identifier (`string`) that is built for current environment.
 Below you can see example implementation of caching tokens in memory:
 
-
 ```python
 # register cache in optional service configuration
 payments = gopay.payments(
     {}, # your config
     {'cache': MyCache()}
 )
 ```
```

### Comparing `gopay-1.3.0/gopay/__init__.py` & `gopay-1.3.1/gopay/__init__.py`

 * *Files identical despite different names*

### Comparing `gopay-1.3.0/gopay/api.py` & `gopay-1.3.1/gopay/api.py`

 * *Files identical despite different names*

### Comparing `gopay-1.3.0/gopay/enums.py` & `gopay-1.3.1/gopay/enums.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,57 +80,75 @@
     XLS_A = "XLS_A"
     XLS_B = "XLS_B"
     XLS_C = "XLS_C"
     CSV_A = "CSV_A"
     CSV_B = "CSV_B"
     CSV_C = "CSV_C"
     CSV_D = "CSV_D"
+    CSV_E = "CSV_E"
     ABO_A = "ABO_A"
 
 
 class ItemType:
     ITEM = "ITEM"
     DISCOUNT = "DISCOUNT"
     DELIVERY = "DELIVERY"
     POSTAGE = "POSTAGE"
 
 
-class VatRate:
-    RATE_1 = 0
-    RATE_2 = 10
-    RATE_3 = 15
-    RATE_4 = 21
-
 
 class EETReceiptState:
     CREATED = "CREATED"
     DELIVERY_FAILED = "DELIVERY_FAILED"
     DELIVERED = "DELIVERED"
 
 
 class EETMode:
     AUTO = "AUTO"
     EET = "EET"
 
 
 class BankSwiftCode:
+    # CZ
     CESKA_SPORITELNA = "GIBACZPX"
     KOMERCNI_BANKA = "KOMBCZPP"
+    CSOB = "CEKOCZPP"
     RAIFFEISENBANK = "RZBCCZPP"
-    MBANK = "BREXCZPP"
+    UNICREDIT_BANK_CZ = "BACXCZPP"
+    MONETA_MONEY_BANK = "AGBACZPP"
     FIO_BANKA = "FIOBCZPP"
-    CSOB = "CEKOCZPP"
-    VSEOBECNA_VEROVA_BANKA_BANKA = "SUBASKBX"
+    MBANK = "BREXCZPP"
+    AIRBANK = "AIRACZPP"
+    ING_BANK = "INGBCZPP"
+    OBERBANK = "OBKLCZ2X"
+    VUB_PRAHA = "SUBACZPP"
+    HELLO_BANK = "BPPFCZP1"
+    CREDITAS = "CTASCZ22"
+    MAX_BANKA = "EXPNCZPP"
+    JT_BANKA = "JTBPCZPP"
+    # SK
     TATRA_BANKA = "TATRSKBX"
+    VSEOBECNA_VEROVA_BANKA_BANKA = "SUBASKBX"
     UNICREDIT_BANK_SK = "UNCRSKBX"
     SLOVENSKA_SPORITELNA = "GIBASKBX"
-    POSTOVA_BANKA = "POBNSKBA"
     CSOB_SK = "CEKOSKBX"
-    SBERBANK_SLOVENSKO = "LUBASKBX"
-    SPECIAL = "OTHERS"
+    POSTOVA_BANKA = "POBNSKBA"
+    OTP_BANKA_SLOVENSKO = "OTPVSKBX"
+    PRIMA_BANKA_SLOVENSKO = "KOMASK2X"
+    CITIBANK_EUROPE = "CITISKBA"
+    FIO_BANKA_SK = "FIOZSKBA"
+    MBANK_SK = "BREXSKBX"
+    ING_BANK_SK = "INGBSKBX"
+    JT_BANKA_SK = "JTBPSKBA"
+    OBERBANK_SK = "OBKLSKBA"
+    PRIVATBANKA = "BSLOSK22"
+    BKS_BANK = "BFKKSKBB"
+    RAIFFEISENBANK_SK = "TATRSKBXXXX"
+    KOMERCNI_BANKA_SK = "KOMBSKBA"
+    # PL
     MBANK1 = "BREXPLPW"
     CITI_HANDLOWY = "CITIPLPX"
     IKO = "BPKOPLPW-IKO"
     INTELIGO = "BPKOPLPW-INTELIGO"
     PLUS_BANK = "IVSEPLPP"
     BANK_BPH_SA = "BPHKPLPK"
     TOYOTA_BANK = "TOBAPLPW"
@@ -156,14 +174,16 @@
     BNP_PARIBAS_POLSKA = "PPABPLPK"
     CREDIT_AGRICOLE = "AGRIPLPR"
     DEUTSCHE_BANK_POLSKA_SA = "DEUTPLPX"
     DNB_NORD = "DNBANOKK"
     E_SKOK = "NBPLPLPW"
     EUROBANK = "SOGEPLPW"
     POLSKI_BANK_PRZEDSIEBIORCZOSCI_SPOLKA_AKCYJNA = "PBPBPLPW"
+    # Others
+    SPECIAL = "OTHERS"
 
 
 class RecurrenceState:
     REQUESTED = "REQUESTED"
     STARTED = "STARTED"
     STOPPED = "STOPPED"
```

### Comparing `gopay-1.3.0/gopay/http.py` & `gopay-1.3.1/gopay/http.py`

 * *Files identical despite different names*

### Comparing `gopay-1.3.0/gopay/oauth2.py` & `gopay-1.3.1/gopay/oauth2.py`

 * *Files identical despite different names*

### Comparing `gopay-1.3.0/gopay/payments.py` & `gopay-1.3.1/gopay/payments.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+from __future__ import annotations
 from typing import Dict, List, Union
 
+
 from gopay.api import JSON, FORM, add_defaults, Response, GoPay
 from gopay.oauth2 import OAuth2
 
 
 paymentSessionId = Union[List[str], str]
 
 
@@ -51,14 +53,17 @@
     ) -> Response:
         return self._api(
             f"payments/payment/{id_payment}/capture", JSON, capture_payment
         )
 
     def void_authorization(self, id_payment: Union[int, str]) -> Response:
         return self._api(f"payments/payment/{id_payment}/void-authorization", FORM, {})
+    
+    def get_card_details(self, card_id: int | str) -> Response:
+        return self._api(f"payments/cards/{card_id}", FORM, None)
 
     def get_payment_instruments(
         self, go_id: Union[int, str], currency: str
     ) -> Response:
         return self._api(
             f"eshops/eshop/{go_id}/payment-instruments/{currency}", "", None
         )
```

### Comparing `gopay-1.3.0/gopay.egg-info/PKG-INFO` & `gopay-1.3.1/gopay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 Metadata-Version: 2.1
 Name: gopay
-Version: 1.3.0
+Version: 1.3.1
 Home-page: https://github.com/gopaycommunity/gopay-python-sdk
 Author: GoPay
 Author-email: integrace@gopay.cz
 License: MIT
 Keywords: gopay payments sdk rest api
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # GoPay's Python SDK for Payments REST API
 
 [![Build Status](https://travis-ci.org/gopaycommunity/gopay-python-api.svg?branch=master)](https://travis-ci.org/gopaycommunity/gopay-python-api)
 
 ## Requirements
 
-- Python >= 3.6
+- Python >= 3.7
 - dependencies:
-    - [`requests`](https://github.com/kennethreitz/requests)
-    - [`deprecated`](https://github.com/tantale/deprecated)
+  - [`requests`](https://github.com/kennethreitz/requests)
+  - [`deprecated`](https://github.com/tantale/deprecated)
 
 ## Installation
 
 The simplest way to install SDK is to use [PIP](https://docs.python.org/3/installing/):
 
 ```bash
 pip install gopay
@@ -66,48 +67,47 @@
 ### Configuration
 
 #### Required fields
 
 Required field | Data type | Documentation |
 -------------- | --------- | ----------- |
 `goid` | string | default GoPay account used in `createPayment` if `target` is not specified
-`clientId` | string | https://doc.gopay.com/#access-token |
-`clientSecret` | string | https://doc.gopay.com/#access-token |
+`clientId` | string | <https://doc.gopay.com/#access-token> |
+`clientSecret` | string | <https://doc.gopay.com/#access-token> |
 `gatewayUrl` | string | [test or production environment?](https://help.gopay.com/en/s/uY) |
 
 #### Optional fields
 
 Optional field | Data type | Default value | Documentation |
 -------------- | --------- | ------------- | ------------- |
-`scope` | string | [`GoPay\Definition\TokenScope::ALL`](src/Definition/TokenScope.php) | https://doc.gopay.com/#access-token |
+`scope` | string | [`GoPay\Definition\TokenScope::ALL`](src/Definition/TokenScope.php) | <https://doc.gopay.com/#access-token> |
 `language` | string | [`GoPay\Definition\Language::ENGLISH`](src/Definition/Language.php) | language used in `createPayment` if `lang` is not specified + used for [localization of errors](https://doc.gopay.com/#errors)
 `timeout` | int | 30 | Browser timeout in seconds |
 
-
 ### Available methods
 
 API | SDK method |
 --- | ---------- |
 [Create standard payment](https://doc.gopay.com/#payment-creation) | `$gopay->createPayment(array $payment)` |
 [Status of the payment](https://doc.gopay.com/#payment-status) | `$gopay->getStatus($id)` |
 [Refund of the payment](https://doc.gopay.com/#payment-refund) | `$gopay->refundPayment($id, $amount)` |
 [Create recurring payment](https://doc.gopay.com/#recurring-payments) | `$gopay->createPayment(array $payment)` |
 [Recurring payment on demand](https://doc.gopay.com/#recurring-on-demand) | `$gopay->createRecurrence($id, array $payment)` |
 [Cancellation of the recurring payment](https://doc.gopay.com/#recurring-payment-cancellation) | `$gopay->voidRecurrence($id)` |
 [Create pre-authorized payment](https://doc.gopay.com/#preauthorized-payments) | `$gopay->createPayment(array $payment)` |
 [Charge of pre-authorized payment](https://doc.gopay.com/#capturing-a-preauthorized-payment) | `$gopay->captureAuthorization($id)` |
 [Cancellation of the pre-authorized payment](https://doc.gopay.com/#cancelling-a-preauthorized-payment) | `$gopay->voidAuthorization($id)` |
+
 ### SDK response? Has my call succeed?
 
 SDK returns wrapped API response. Every method returns
 [`GoPay\Http\Response` object](src/Http/Response.php). Structure of `json/__toString`
 should be same as in [documentation](https://doc.gopay.com/en).
 SDK throws no exception. Please create an issue if you catch one.
 
-
 ```python
 response = payments.create_payment({...})
 if response.has_succeed():
     print("hooray, API returned " + str(response))
     return response.json['gw_url'] # url for initiation of gateway
 else:
     # errors format: https://doc.gopay.com/en/?shell#http-result-codes
@@ -117,15 +117,14 @@
 Method | Description |
 ------ | ---------- |
 `response.has_succeed()` | checks if API returns status code _200_ |
 `response.json` | decoded response, returned objects are converted into associative arrays |
 `response.status_code` | HTTP status code |
 `response.__str__()` | raw body from HTTP response |
 
-
 ### Are required fields and allowed values validated?
 
 **No.** API [validates fields](https://doc.gopay.com/#error) pretty extensively
 so there is no need to duplicate validation in SDK. It would only introduce new type of error.
 Or we would have to perfectly simulate API error messages. That's why SDK just calls API which
 behavior is well documented in [doc.gopay.com](https://doc.gopay.com).
 
@@ -185,15 +184,14 @@
 
 Your cache must implement template methods `get_token` and `set_token`.
 Be aware that there are two [scopes](https://doc.gopay.com/#access-token) (`TokenScope`) and
 SDK can be used for different clients (`clientId`, `gatewayUrl`). So `client` passed to
 methods is unique identifier (`string`) that is built for current environment.
 Below you can see example implementation of caching tokens in memory:
 
-
 ```python
 # register cache in optional service configuration
 payments = gopay.payments(
     {}, # your config
     {'cache': MyCache()}
 )
 ```
```

### Comparing `gopay-1.3.0/setup.py` & `gopay-1.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="gopay",
-    version="1.3.0",
+    version="1.3.1",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/gopaycommunity/gopay-python-sdk",
     author="GoPay",
     author_email="integrace@gopay.cz",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     keywords="gopay payments sdk rest api",
     packages=["gopay"],
     install_requires=["requests", "deprecated>=1.2.0"],
 )
```

