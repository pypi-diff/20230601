# Comparing `tmp/shurjopay-plugin-0.1.7.tar.gz` & `tmp/shurjopay-plugin-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shurjopay-plugin-0.1.7.tar", last modified: Mon May 29 11:58:57 2023, max compression
+gzip compressed data, was "shurjopay-plugin-0.1.8.tar", last modified: Thu Jun  1 09:18:34 2023, max compression
```

## Comparing `shurjopay-plugin-0.1.7.tar` & `shurjopay-plugin-0.1.8.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-05-29 11:58:57.890639 shurjopay-plugin-0.1.7/
--rw-r--r--   0 imtiaz     (501) staff       (20)     1097 2022-12-27 06:57:09.000000 shurjopay-plugin-0.1.7/LICENSE
--rw-r--r--   0 imtiaz     (501) staff       (20)       52 2022-11-03 05:39:41.000000 shurjopay-plugin-0.1.7/MANIFEST.in
--rw-r--r--   0 imtiaz     (501) staff       (20)     4581 2023-05-29 11:58:57.890501 shurjopay-plugin-0.1.7/PKG-INFO
--rw-r--r--   0 imtiaz     (501) staff       (20)     3982 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.7/README.md
--rw-r--r--   0 imtiaz     (501) staff       (20)      103 2022-11-03 05:39:41.000000 shurjopay-plugin-0.1.7/pyproject.toml
--rw-r--r--   0 imtiaz     (501) staff       (20)       38 2023-05-29 11:58:57.890686 shurjopay-plugin-0.1.7/setup.cfg
--rw-r--r--   0 imtiaz     (501) staff       (20)      933 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.7/setup.py
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-05-29 11:58:57.887037 shurjopay-plugin-0.1.7/src/
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-05-29 11:58:57.889341 shurjopay-plugin-0.1.7/src/shurjopay_plugin/
--rw-r--r--   0 imtiaz     (501) staff       (20)       75 2022-12-27 06:57:09.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin/__init__.py
--rw-r--r--   0 imtiaz     (501) staff       (20)     1531 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin/logger_config.py
--rw-r--r--   0 imtiaz     (501) staff       (20)     5182 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin/models.py
--rw-r--r--   0 imtiaz     (501) staff       (20)    11381 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin/shurjopay_plugin.py
--rw-r--r--   0 imtiaz     (501) staff       (20)     2305 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin/utils.py
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-05-29 11:58:57.890128 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/
--rw-r--r--   0 imtiaz     (501) staff       (20)     4581 2023-05-29 11:58:57.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/PKG-INFO
--rw-r--r--   0 imtiaz     (501) staff       (20)      476 2023-05-29 11:58:57.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 imtiaz     (501) staff       (20)        1 2023-05-29 11:58:57.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 imtiaz     (501) staff       (20)        9 2023-05-29 11:58:57.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/requires.txt
--rw-r--r--   0 imtiaz     (501) staff       (20)       17 2023-05-29 11:58:57.000000 shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-05-29 11:58:57.890285 shurjopay-plugin-0.1.7/tests/
--rw-r--r--   0 imtiaz     (501) staff       (20)     2752 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.7/tests/test_shurjopay_plugin.py
+drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-06-01 09:18:34.123985 shurjopay-plugin-0.1.8/
+-rw-r--r--   0 imtiaz     (501) staff       (20)     1097 2022-12-27 06:57:09.000000 shurjopay-plugin-0.1.8/LICENSE
+-rw-r--r--   0 imtiaz     (501) staff       (20)       52 2022-11-03 05:39:41.000000 shurjopay-plugin-0.1.8/MANIFEST.in
+-rw-r--r--   0 imtiaz     (501) staff       (20)     4581 2023-06-01 09:18:34.123828 shurjopay-plugin-0.1.8/PKG-INFO
+-rw-r--r--   0 imtiaz     (501) staff       (20)     3982 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.8/README.md
+-rw-r--r--   0 imtiaz     (501) staff       (20)      103 2022-11-03 05:39:41.000000 shurjopay-plugin-0.1.8/pyproject.toml
+-rw-r--r--   0 imtiaz     (501) staff       (20)       38 2023-06-01 09:18:34.124035 shurjopay-plugin-0.1.8/setup.cfg
+-rw-r--r--   0 imtiaz     (501) staff       (20)      933 2023-06-01 09:16:25.000000 shurjopay-plugin-0.1.8/setup.py
+drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-06-01 09:18:34.119939 shurjopay-plugin-0.1.8/src/
+drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-06-01 09:18:34.121938 shurjopay-plugin-0.1.8/src/shurjopay_plugin/
+-rw-r--r--   0 imtiaz     (501) staff       (20)       75 2022-12-27 06:57:09.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin/__init__.py
+-rw-r--r--   0 imtiaz     (501) staff       (20)     1531 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin/logger_config.py
+-rw-r--r--   0 imtiaz     (501) staff       (20)     5454 2023-06-01 09:16:25.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin/models.py
+-rw-r--r--   0 imtiaz     (501) staff       (20)    11432 2023-06-01 09:16:25.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin/shurjopay_plugin.py
+-rw-r--r--   0 imtiaz     (501) staff       (20)     2305 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin/utils.py
+drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-06-01 09:18:34.123201 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/
+-rw-r--r--   0 imtiaz     (501) staff       (20)     4581 2023-06-01 09:18:34.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 imtiaz     (501) staff       (20)      497 2023-06-01 09:18:34.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 imtiaz     (501) staff       (20)        1 2023-06-01 09:18:34.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 imtiaz     (501) staff       (20)        9 2023-06-01 09:18:34.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/requires.txt
+-rw-r--r--   0 imtiaz     (501) staff       (20)       17 2023-06-01 09:18:34.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-06-01 09:18:34.123591 shurjopay-plugin-0.1.8/tests/
+-rw-r--r--   0 imtiaz     (501) staff       (20)     2125 2023-06-01 09:16:25.000000 shurjopay-plugin-0.1.8/tests/test_models.py
+-rw-r--r--   0 imtiaz     (501) staff       (20)     3110 2023-06-01 09:16:25.000000 shurjopay-plugin-0.1.8/tests/test_shurjopay_plugin.py
```

### Comparing `shurjopay-plugin-0.1.7/LICENSE` & `shurjopay-plugin-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.7/PKG-INFO` & `shurjopay-plugin-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shurjopay-plugin
-Version: 0.1.7
+Version: 0.1.8
 Summary: Shurjopay version 2.1 payment gateway integration package for python users
 Home-page: https://github.com/shurjopay-plugins/sp-plugin-python.git
 Author: Mahabubul Hasan
 Author-email: plugindev@shurjomukhi.com.bd
 Project-URL: Bug Tracker, https://github.com/shurjopay-plugins/sp-plugin-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shurjopay-plugin-0.1.7/README.md` & `shurjopay-plugin-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.7/setup.py` & `shurjopay-plugin-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="shurjopay-plugin",
-    version="0.1.7",
+    version="0.1.8",
     author="Mahabubul Hasan",
     author_email="plugindev@shurjomukhi.com.bd",
     description="Shurjopay version 2.1 payment gateway integration package for python users",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shurjopay-plugins/sp-plugin-python.git",
     project_urls={
```

### Comparing `shurjopay-plugin-0.1.7/src/shurjopay_plugin/logger_config.py` & `shurjopay-plugin-0.1.8/src/shurjopay_plugin/logger_config.py`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.7/src/shurjopay_plugin/shurjopay_plugin.py` & `shurjopay-plugin-0.1.8/src/shurjopay_plugin/shurjopay_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,48 +12,51 @@
     VerifiedPaymentDetailsModel
 )
 from .utils import (
     get_client_ip,
     Endpoints,
     ShurjopayStatus,
     ShurjopayException,
-    ShurjopayAuthException)
+    ShurjopayAuthException
+)
 from .logger_config import ShurjopayLoggerConfig
 
 
 class ShurjopayPlugin(object):
-    '''
-        shurjoPay Online payment gateway has several API's which need to be integrated by merchants for accessing different services. The available services are:
+    """
+        shurjoPay Online payment gateway has several API's
+        which need to be integrated by merchants for
+        accessing different services. The available services are:
         - Authenticating
         - Making payment
-        - Verifying payment 
+        - Verifying payment
         - Checking payment status
-        For more details view the shurjoPay version-2.1 integration documentation : https://docs.google.com/document/d/19J4HE0j873nBJqcN-uRBYYAa_qBA3p1XSY-jy2fwvEE/edit .    
-    '''
+        For more details view the shurjoPay version-2.1 integration documentation :
+        https://docs.google.com/document/d/19J4HE0j873nBJqcN-uRBYYAa_qBA3p1XSY-jy2fwvEE/edit .
+    """
     # shurjopay Token attributes
     # token(str),
     # token_type,
     # expires_in,
     # sp_code,
     # message
     AUTH_TOKEN = None
 
     # Status Message
     AUTHENTICATION_SUCCESS = 'Merchant Authentication Successful!'
     AUTHENTICATION_FAILED = 'Merchant Authentication Failed!'
     AUTHENTICATION_SUCCESS = 'Merchant Authentication Successful!'
     AUTHENTICATION_FAILED = 'Merchant Authentication Failed!'
     AUTHENTICATION_TOKEN_EXPIRED = 'Shurjopay Token Expired!'
-    WRONG_CREDENTIALS = 'Please check your credentials'
+    WRONG_CREDENTIALS = 'Please Check Your Credentials!'
     PAYMENT_REQUEST_SUCCESS = 'Shurjopay Payment Request Successful!'
     PAYMENT_REQUEST_FAILED = 'Shurjopay Payment Request Failed!'
     PAYMENT_VERIFICATION_FAILED = 'Shurjopay Payment Verification Failed!'
     PAYMENT_CHECK_FAILED = 'Shurjopay Payment Checking Failed!'
 
-
     def __init__(self, sp_config) -> None:
         # Initialize the configuration keys for plugin configuration
         self.SP_USERNAME = sp_config.SP_USERNAME
         self.SP_PASSWORD = sp_config.SP_PASSWORD
         self.SP_ENDPOINT = requests.compat.urljoin(
             sp_config.SP_ENDPOINT, Endpoints.API.value)
         self.SP_RETURN = sp_config.SP_RETURN
@@ -62,29 +65,30 @@
 
         if sp_config.SP_LOGDIR is None or sp_config.SP_LOGDIR == '':
             self.logger = ShurjopayLoggerConfig().get_logger()
             return
         self.logger = ShurjopayLoggerConfig().get_file_logger(sp_config.SP_LOGDIR)
 
     def authenticate(self):
-        ''' Authenticate with shurjoPay Payment Gateway using Merchant credectials.
+        """ Authenticate with shurjoPay Payment Gateway using Merchant credectials.
 
         Returns
         -------
-        AUTH_TOKEN (ShurjoPayTokenModel): token details from "get-token" api response which contains
+        AUTH_TOKEN (ShurjoPayTokenModel): token details from shurjopay
             - token(str), 
             - token_type(str),
             - expires_in(int),(in seconds)
             - sp_code(int),
             - message(str)
 
         Raises
         -----
-        ShurjopayAuthException: If authentication fails due to invalid credentials or any other reason. 
-        '''
+        ShurjopayAuthException: If authentication fails due to 
+        invalid credentials or any other reason. 
+        """
         # Create token endpoint url
         url = requests.compat.urljoin(self.SP_ENDPOINT, Endpoints.TOKEN.value)
         self.logger.info(self.SP_ENDPOINT)
         self.logger.info(url)
         payloads = {
             "username": self.SP_USERNAME,
             "password": self.SP_PASSWORD,
@@ -106,41 +110,45 @@
         except ShurjopayAuthException as ex:
             # Log authentication expception error
             self.logger.error(f'{self.WRONG_CREDENTIALS}, {ex}')
             # Raise exception if authentication fails
             raise ShurjopayAuthException(self.WRONG_CREDENTIALS, ex)
 
     def is_token_valid(self):
-        '''Checks if token is valid or not by comparing token expiry time with current time
+        """Checks if token is valid or not by comparing
+        token expiry time with current time
 
         Returns
         -------
         True: if token is valid 
         None: if token is invalid
-        '''
+        """
         return True if (datetime.datetime.strptime(
-                       self.AUTH_TOKEN.token_create_time, "%Y-%m-%d %I:%M:%S%p") + datetime.timedelta(seconds=self.AUTH_TOKEN.expires_in)) > datetime.datetime.now() else False
+                       self.AUTH_TOKEN.token_create_time, "%Y-%m-%d %I:%M:%S%p") +
+            datetime.timedelta(seconds=self.AUTH_TOKEN.expires_in)) > datetime.datetime.now() else False
 
     def make_payment(self, payment_req):
-        '''Make payment request to shurjoPay Gateway using a payment request object containing payment details.
+        """Make payment request to shurjoPay Gateway 
+        using a payment request object containing payment details.
 
         Args
         ----
-        payment_req (PaymentRequestModel): PaymentRequest object containing payment details.
+        payment_req (PaymentRequestModel): PaymentRequestModel object containing payment details.
 
         Returns
         -------
-        payment_details (PaymentDetailsModel): PaymentDetails object containing redirect URL to reach payment page, order id to verify order in shurjoPay.
+        payment_details (PaymentDetailsModel): PaymentDetailsModel object containing redirect URL 
+        to reach payment page, order id to verify order in shurjoPay.
         None: if response dosenot contains callback url.
 
         Raises
         ------
         ShurjopayAuthException if payment fails due to token expired or invalid token.
         ShurjopayException if payment fails due to any other reason.
-        '''
+        """
         try:
             # Check if token is valid or expired
             if self.AUTH_TOKEN is None or self.is_token_valid() is False:
                 # Authenticate with shurjoPay
                 self.AUTH_TOKEN = self.authenticate()
         except ShurjopayAuthException as ex:
             self.logger.error(f'{self.AUTHENTICATION_FAILED}: {ex}')
@@ -174,29 +182,28 @@
         else:
             self.logger.warning(
                 f'{self.AUTHENTICATION_FAILED}: {self.AUTHENTICATION_TOKEN_EXPIRED}')
             raise ShurjopayAuthException(
                 self.AUTHENTICATION_FAILED, self.AUTHENTICATION_TOKEN_EXPIRED)
 
     def verify_payment(self, order_id):
-        ''' Complete the payment process ushig the order id in the the IPN.
-
+        """ Complete the payment process ushig the order id in the the IPN.
         Args
         -----
         order_id (str): Order id of the payment.
 
         Returns
         -------
-        VerifiedPaymentModel: VerifiedPayment object containing payment details.
+        VerifiedPaymentModel: VerifiedPaymentModel object containing payment details.
 
         Raises
         -------
         ShurjopayAuthException if payment fails due to token expired or invalid token.
         ShurjopayException if payment fails due to any other reason.
-        '''
+        """
         try:
             # Check if token is valid or expired
             if self.AUTH_TOKEN is None or self.is_token_valid() is False:
                 # Authenticate with shurjoPay
                 self.AUTH_TOKEN = self.authenticate()
         except ShurjopayAuthException as ex:
             self.logger.error(self.AUTHENTICATION_FAILED, ex)
@@ -233,23 +240,23 @@
         else:
             self.logger.error(
                 f'{self.AUTHENTICATION_FAILED}: {self.AUTHENTICATION_TOKEN_EXPIRED}')
             raise ShurjopayAuthException(
                 self.AUTHENTICATION_FAILED, self.AUTHENTICATION_TOKEN_EXPIRED)
 
     def _map_payment_request(self, payment_req):
-        ''' This method is used to map additional parameters to payment request details.
+        """ This method is used to map additional parameters to payment request details.
         Args
         ----
         payment_req (PaymentRequestModel): Payment request object
 
         Returns
         -------
         payment_req (dict) : a dictionary containing complete payment request details.
-        '''
+        """
         return {
             'token': self.AUTH_TOKEN.token,
             'return_url': self.SP_RETURN,
             'cancel_url': self.SP_CANCEL,
             'store_id': self.AUTH_TOKEN.store_id,
             'prefix': self.SP_PREFIX,
             'amount': payment_req.amount,
```

### Comparing `shurjopay-plugin-0.1.7/src/shurjopay_plugin/utils.py` & `shurjopay-plugin-0.1.8/src/shurjopay_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.7/src/shurjopay_plugin.egg-info/PKG-INFO` & `shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shurjopay-plugin
-Version: 0.1.7
+Version: 0.1.8
 Summary: Shurjopay version 2.1 payment gateway integration package for python users
 Home-page: https://github.com/shurjopay-plugins/sp-plugin-python.git
 Author: Mahabubul Hasan
 Author-email: plugindev@shurjomukhi.com.bd
 Project-URL: Bug Tracker, https://github.com/shurjopay-plugins/sp-plugin-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shurjopay-plugin-0.1.7/tests/test_shurjopay_plugin.py` & `shurjopay-plugin-0.1.8/tests/test_shurjopay_plugin.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,40 +40,51 @@
         # unit testing for make payment
         self._payment_request_details = self._plugin.make_payment(
             self._payment_request)
 
         print(json.dumps(self._payment_request_details.__dict__, indent=4))
 
         self.assertEqual(
-            5, self._payment_request_details.amount, 'amount is not equal')
+            5, self._payment_request_details.amount,
+            'amount is not equal')
 
         self.assertEqual(
-            'BDT', self._payment_request_details.currency, 'Currency  is not equal')
+            'BDT', self._payment_request_details.currency,
+            'Currency  is not equal')
 
         self.assertEqual(
-            'MD. ABDUL KARIM', self._payment_request_details.customer_name, 'Customer Name is not equal')
+            'MD. ABDUL KARIM', self._payment_request_details.customer_name,
+            'Customer Name is not equal')
 
         self.assertEqual(
-            '01111111111', self._payment_request_details.customer_phone, 'Customer Phone is not equal')
+            '01111111111', self._payment_request_details.customer_phone,
+            'Customer Phone is not equal')
 
         self.assertEqual(
-            'mohakhali', self._payment_request_details.customer_address, "Customer Address is not equal")
+            'mohakhali', self._payment_request_details.customer_address,
+            "Customer Address is not equal")
 
         self.assertEqual(
-            'Dhaka', self._payment_request_details.customer_city, 'Customer City is not equal')
+            'Dhaka', self._payment_request_details.customer_city,
+            'Customer City is not equal')
 
     def test_verify_payment(self):
         # unit testing for verify payment
         try:
-            verified_payment_details = self._plugin.verify_payment(
+            self.verified_payment_details = self._plugin.verify_payment(
                 'SP_PLUGIN_PYTHON64744291a63de')
-            self.assertEqual(2382747, verified_payment_details.id,
+            print(json.dumps(
+                self.verified_payment_details.__dict__, indent=4))
+            self.assertEqual(2382747, self.verified_payment_details.payment_id,
                              "ID is not equal")
             self.assertEqual(
-                "SP_PLUGIN_PYTHON64744291a63de", verified_payment_details.order_id,
+                "SP_PLUGIN_PYTHON64744291a63de", self.verified_payment_details.shurjopay_order_id,
                 "Order ID is not equal")
+            self.assertEqual(
+                'MD. ABDUL KARIM', self.verified_payment_details.customer_name,
+                'Customer Name is not equal')
         except ShurjopayException as e:
             LOGGER.info(e)
 
 
 if __name__ == '__main__':
     unittest.main()
```

