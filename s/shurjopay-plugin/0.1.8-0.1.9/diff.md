# Comparing `tmp/shurjopay-plugin-0.1.8.tar.gz` & `tmp/shurjopay-plugin-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shurjopay-plugin-0.1.8.tar", last modified: Thu Jun  1 09:18:34 2023, max compression
+gzip compressed data, was "shurjopay-plugin-0.1.9.tar", last modified: Thu Jun  1 10:23:48 2023, max compression
```

## Comparing `shurjopay-plugin-0.1.8.tar` & `shurjopay-plugin-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-06-01 09:18:34.123985 shurjopay-plugin-0.1.8/
--rw-r--r--   0 imtiaz     (501) staff       (20)     1097 2022-12-27 06:57:09.000000 shurjopay-plugin-0.1.8/LICENSE
--rw-r--r--   0 imtiaz     (501) staff       (20)       52 2022-11-03 05:39:41.000000 shurjopay-plugin-0.1.8/MANIFEST.in
--rw-r--r--   0 imtiaz     (501) staff       (20)     4581 2023-06-01 09:18:34.123828 shurjopay-plugin-0.1.8/PKG-INFO
--rw-r--r--   0 imtiaz     (501) staff       (20)     3982 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.8/README.md
--rw-r--r--   0 imtiaz     (501) staff       (20)      103 2022-11-03 05:39:41.000000 shurjopay-plugin-0.1.8/pyproject.toml
--rw-r--r--   0 imtiaz     (501) staff       (20)       38 2023-06-01 09:18:34.124035 shurjopay-plugin-0.1.8/setup.cfg
--rw-r--r--   0 imtiaz     (501) staff       (20)      933 2023-06-01 09:16:25.000000 shurjopay-plugin-0.1.8/setup.py
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-06-01 09:18:34.119939 shurjopay-plugin-0.1.8/src/
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-06-01 09:18:34.121938 shurjopay-plugin-0.1.8/src/shurjopay_plugin/
--rw-r--r--   0 imtiaz     (501) staff       (20)       75 2022-12-27 06:57:09.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin/__init__.py
--rw-r--r--   0 imtiaz     (501) staff       (20)     1531 2023-03-23 09:34:12.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin/logger_config.py
--rw-r--r--   0 imtiaz     (501) staff       (20)     5454 2023-06-01 09:16:25.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin/models.py
--rw-r--r--   0 imtiaz     (501) staff       (20)    11432 2023-06-01 09:16:25.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin/shurjopay_plugin.py
--rw-r--r--   0 imtiaz     (501) staff       (20)     2305 2023-05-29 11:58:35.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin/utils.py
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-06-01 09:18:34.123201 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/
--rw-r--r--   0 imtiaz     (501) staff       (20)     4581 2023-06-01 09:18:34.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/PKG-INFO
--rw-r--r--   0 imtiaz     (501) staff       (20)      497 2023-06-01 09:18:34.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 imtiaz     (501) staff       (20)        1 2023-06-01 09:18:34.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 imtiaz     (501) staff       (20)        9 2023-06-01 09:18:34.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/requires.txt
--rw-r--r--   0 imtiaz     (501) staff       (20)       17 2023-06-01 09:18:34.000000 shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/top_level.txt
-drwxr-xr-x   0 imtiaz     (501) staff       (20)        0 2023-06-01 09:18:34.123591 shurjopay-plugin-0.1.8/tests/
--rw-r--r--   0 imtiaz     (501) staff       (20)     2125 2023-06-01 09:16:25.000000 shurjopay-plugin-0.1.8/tests/test_models.py
--rw-r--r--   0 imtiaz     (501) staff       (20)     3110 2023-06-01 09:16:25.000000 shurjopay-plugin-0.1.8/tests/test_shurjopay_plugin.py
+drwxr-xr-x   0 axiom     (1000) axiom     (1000)        0 2023-06-01 10:23:48.260732 shurjopay-plugin-0.1.9/
+-rw-r--r--   0 axiom     (1000) axiom     (1000)     1097 2023-05-28 12:15:36.000000 shurjopay-plugin-0.1.9/LICENSE
+-rw-r--r--   0 axiom     (1000) axiom     (1000)       52 2023-05-28 12:15:36.000000 shurjopay-plugin-0.1.9/MANIFEST.in
+-rw-r--r--   0 axiom     (1000) axiom     (1000)     4581 2023-06-01 10:23:48.260732 shurjopay-plugin-0.1.9/PKG-INFO
+-rw-r--r--   0 axiom     (1000) axiom     (1000)     3982 2023-05-31 09:49:53.000000 shurjopay-plugin-0.1.9/README.md
+-rw-r--r--   0 axiom     (1000) axiom     (1000)      103 2023-05-28 12:15:36.000000 shurjopay-plugin-0.1.9/pyproject.toml
+-rw-r--r--   0 axiom     (1000) axiom     (1000)       38 2023-06-01 10:23:48.260732 shurjopay-plugin-0.1.9/setup.cfg
+-rw-r--r--   0 axiom     (1000) axiom     (1000)      933 2023-06-01 10:19:08.000000 shurjopay-plugin-0.1.9/setup.py
+drwxr-xr-x   0 axiom     (1000) axiom     (1000)        0 2023-06-01 10:23:48.254065 shurjopay-plugin-0.1.9/src/
+drwxr-xr-x   0 axiom     (1000) axiom     (1000)        0 2023-06-01 10:23:48.257398 shurjopay-plugin-0.1.9/src/shurjopay_plugin/
+-rw-r--r--   0 axiom     (1000) axiom     (1000)       75 2023-05-28 12:15:36.000000 shurjopay-plugin-0.1.9/src/shurjopay_plugin/__init__.py
+-rw-r--r--   0 axiom     (1000) axiom     (1000)     1531 2023-05-28 12:15:36.000000 shurjopay-plugin-0.1.9/src/shurjopay_plugin/logger_config.py
+-rw-r--r--   0 axiom     (1000) axiom     (1000)     5518 2023-06-01 10:19:34.000000 shurjopay-plugin-0.1.9/src/shurjopay_plugin/models.py
+-rw-r--r--   0 axiom     (1000) axiom     (1000)    11432 2023-06-01 07:42:42.000000 shurjopay-plugin-0.1.9/src/shurjopay_plugin/shurjopay_plugin.py
+-rw-r--r--   0 axiom     (1000) axiom     (1000)     2305 2023-05-31 07:08:36.000000 shurjopay-plugin-0.1.9/src/shurjopay_plugin/utils.py
+drwxr-xr-x   0 axiom     (1000) axiom     (1000)        0 2023-06-01 10:23:48.257398 shurjopay-plugin-0.1.9/src/shurjopay_plugin.egg-info/
+-rw-r--r--   0 axiom     (1000) axiom     (1000)     4581 2023-06-01 10:23:48.000000 shurjopay-plugin-0.1.9/src/shurjopay_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 axiom     (1000) axiom     (1000)      497 2023-06-01 10:23:48.000000 shurjopay-plugin-0.1.9/src/shurjopay_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 axiom     (1000) axiom     (1000)        1 2023-06-01 10:23:48.000000 shurjopay-plugin-0.1.9/src/shurjopay_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 axiom     (1000) axiom     (1000)        9 2023-06-01 10:23:48.000000 shurjopay-plugin-0.1.9/src/shurjopay_plugin.egg-info/requires.txt
+-rw-r--r--   0 axiom     (1000) axiom     (1000)       17 2023-06-01 10:23:48.000000 shurjopay-plugin-0.1.9/src/shurjopay_plugin.egg-info/top_level.txt
+drwxr-xr-x   0 axiom     (1000) axiom     (1000)        0 2023-06-01 10:23:48.257398 shurjopay-plugin-0.1.9/tests/
+-rw-r--r--   0 axiom     (1000) axiom     (1000)     2125 2023-05-31 09:44:20.000000 shurjopay-plugin-0.1.9/tests/test_models.py
+-rw-r--r--   0 axiom     (1000) axiom     (1000)     3110 2023-05-31 09:44:30.000000 shurjopay-plugin-0.1.9/tests/test_shurjopay_plugin.py
```

### Comparing `shurjopay-plugin-0.1.8/LICENSE` & `shurjopay-plugin-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.8/PKG-INFO` & `shurjopay-plugin-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shurjopay-plugin
-Version: 0.1.8
+Version: 0.1.9
 Summary: Shurjopay version 2.1 payment gateway integration package for python users
 Home-page: https://github.com/shurjopay-plugins/sp-plugin-python.git
 Author: Mahabubul Hasan
 Author-email: plugindev@shurjomukhi.com.bd
 Project-URL: Bug Tracker, https://github.com/shurjopay-plugins/sp-plugin-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shurjopay-plugin-0.1.8/README.md` & `shurjopay-plugin-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.8/setup.py` & `shurjopay-plugin-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="shurjopay-plugin",
-    version="0.1.8",
+    version="0.1.9",
     author="Mahabubul Hasan",
     author_email="plugindev@shurjomukhi.com.bd",
     description="Shurjopay version 2.1 payment gateway integration package for python users",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/shurjopay-plugins/sp-plugin-python.git",
     project_urls={
```

### Comparing `shurjopay-plugin-0.1.8/src/shurjopay_plugin/logger_config.py` & `shurjopay-plugin-0.1.9/src/shurjopay_plugin/logger_config.py`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.8/src/shurjopay_plugin/models.py` & `shurjopay-plugin-0.1.9/src/shurjopay_plugin/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     '''This class is used to store verified payment details'''
 
     def __init__(self, **kwargs):
 
         self.payment_id = int(kwargs.get('id'))
         self.shurjopay_order_id = str(kwargs.get('order_id'))
         self.merchant_invoice_no = str(kwargs.get('invoice_no'))
+        self.bank_trx_id = str(kwargs.get('bank_trx_id') or '')
 
         self.currency = str(kwargs.get('currency'))  # payment currency
         self.amount = float(kwargs.get('amount'))  # payment amount
         self.payable_amount = float(kwargs.get('payable_amount'))
         self.received_amount = float(kwargs.get('recived_amount'))
         self.discount_amount = float(kwargs.get('discount_amount'))
         self.discount_percent = int(kwargs.get('disc_percent'))
```

### Comparing `shurjopay-plugin-0.1.8/src/shurjopay_plugin/shurjopay_plugin.py` & `shurjopay-plugin-0.1.9/src/shurjopay_plugin/shurjopay_plugin.py`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.8/src/shurjopay_plugin/utils.py` & `shurjopay-plugin-0.1.9/src/shurjopay_plugin/utils.py`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.8/src/shurjopay_plugin.egg-info/PKG-INFO` & `shurjopay-plugin-0.1.9/src/shurjopay_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shurjopay-plugin
-Version: 0.1.8
+Version: 0.1.9
 Summary: Shurjopay version 2.1 payment gateway integration package for python users
 Home-page: https://github.com/shurjopay-plugins/sp-plugin-python.git
 Author: Mahabubul Hasan
 Author-email: plugindev@shurjomukhi.com.bd
 Project-URL: Bug Tracker, https://github.com/shurjopay-plugins/sp-plugin-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shurjopay-plugin-0.1.8/tests/test_models.py` & `shurjopay-plugin-0.1.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `shurjopay-plugin-0.1.8/tests/test_shurjopay_plugin.py` & `shurjopay-plugin-0.1.9/tests/test_shurjopay_plugin.py`

 * *Files identical despite different names*

