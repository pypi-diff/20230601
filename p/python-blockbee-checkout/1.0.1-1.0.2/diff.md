# Comparing `tmp/python-blockbee-checkout-1.0.1.tar.gz` & `tmp/python-blockbee-checkout-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-blockbee-checkout-1.0.1.tar", last modified: Thu Apr 20 14:22:35 2023, max compression
+gzip compressed data, was "python-blockbee-checkout-1.0.2.tar", last modified: Thu Jun  1 11:42:39 2023, max compression
```

## Comparing `python-blockbee-checkout-1.0.1.tar` & `python-blockbee-checkout-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-04-20 14:22:35.008952 python-blockbee-checkout-1.0.1/
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-04-20 14:22:35.007983 python-blockbee-checkout-1.0.1/BlockBee/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     2570 2023-04-20 14:20:52.000000 python-blockbee-checkout-1.0.1/BlockBee/BlockBeeCheckout.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)       52 2023-04-20 14:20:52.000000 python-blockbee-checkout-1.0.1/BlockBee/__init__.py
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1075 2023-01-30 18:34:25.000000 python-blockbee-checkout-1.0.1/LICENSE
--rw-r--r--   0 arianoangelo   (501) staff       (20)     3453 2023-04-20 14:22:35.008853 python-blockbee-checkout-1.0.1/PKG-INFO
-drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-04-20 14:22:35.008688 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/
--rw-r--r--   0 arianoangelo   (501) staff       (20)     3453 2023-04-20 14:22:34.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/PKG-INFO
--rw-r--r--   0 arianoangelo   (501) staff       (20)      352 2023-04-20 14:22:34.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/SOURCES.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-04-20 14:22:34.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/dependency_links.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-01-31 09:40:46.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/not-zip-safe
--rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2023-04-20 14:22:34.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/requires.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2023-04-20 14:22:34.000000 python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/top_level.txt
--rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2023-04-20 14:22:35.008988 python-blockbee-checkout-1.0.1/setup.cfg
--rw-r--r--   0 arianoangelo   (501) staff       (20)     1037 2023-04-20 14:20:52.000000 python-blockbee-checkout-1.0.1/setup.py
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-06-01 11:42:39.909345 python-blockbee-checkout-1.0.2/
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-06-01 11:42:39.908265 python-blockbee-checkout-1.0.2/BlockBee/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     2570 2023-04-20 14:20:52.000000 python-blockbee-checkout-1.0.2/BlockBee/BlockBeeCheckout.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       52 2023-04-20 14:20:52.000000 python-blockbee-checkout-1.0.2/BlockBee/__init__.py
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1075 2023-01-30 18:34:25.000000 python-blockbee-checkout-1.0.2/LICENSE
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     3482 2023-06-01 11:42:39.909239 python-blockbee-checkout-1.0.2/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     2815 2023-06-01 11:41:47.000000 python-blockbee-checkout-1.0.2/README.md
+drwxr-xr-x   0 arianoangelo   (501) staff       (20)        0 2023-06-01 11:42:39.909074 python-blockbee-checkout-1.0.2/python_blockbee_checkout.egg-info/
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     3482 2023-06-01 11:42:39.000000 python-blockbee-checkout-1.0.2/python_blockbee_checkout.egg-info/PKG-INFO
+-rw-r--r--   0 arianoangelo   (501) staff       (20)      362 2023-06-01 11:42:39.000000 python-blockbee-checkout-1.0.2/python_blockbee_checkout.egg-info/SOURCES.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-06-01 11:42:39.000000 python-blockbee-checkout-1.0.2/python_blockbee_checkout.egg-info/dependency_links.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        1 2023-06-01 11:42:39.000000 python-blockbee-checkout-1.0.2/python_blockbee_checkout.egg-info/not-zip-safe
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2023-06-01 11:42:39.000000 python-blockbee-checkout-1.0.2/python_blockbee_checkout.egg-info/requires.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)        9 2023-06-01 11:42:39.000000 python-blockbee-checkout-1.0.2/python_blockbee_checkout.egg-info/top_level.txt
+-rw-r--r--   0 arianoangelo   (501) staff       (20)       38 2023-06-01 11:42:39.909383 python-blockbee-checkout-1.0.2/setup.cfg
+-rw-r--r--   0 arianoangelo   (501) staff       (20)     1037 2023-06-01 11:41:47.000000 python-blockbee-checkout-1.0.2/setup.py
```

### Comparing `python-blockbee-checkout-1.0.1/BlockBee/BlockBeeCheckout.py` & `python-blockbee-checkout-1.0.2/BlockBee/BlockBeeCheckout.py`

 * *Files identical despite different names*

### Comparing `python-blockbee-checkout-1.0.1/LICENSE` & `python-blockbee-checkout-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-blockbee-checkout-1.0.1/PKG-INFO` & `python-blockbee-checkout-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-blockbee-checkout
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python Library for BlockBee Checkout
 Home-page: https://github.com/blockbee-io/python-blockbee-checkout
 Author: BlockBee
 Author-email: info@blockbee.io
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -94,7 +94,10 @@
 ### Changelog
 
 #### 1.0.0
 * Initial Release
 
 #### 1.0.1
 * Minor bugfixes
+
+#### 1.0.2
+* Minor bugfixes
```

### Comparing `python-blockbee-checkout-1.0.1/python_blockbee_checkout.egg-info/PKG-INFO` & `python-blockbee-checkout-1.0.2/python_blockbee_checkout.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-blockbee-checkout
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python Library for BlockBee Checkout
 Home-page: https://github.com/blockbee-io/python-blockbee-checkout
 Author: BlockBee
 Author-email: info@blockbee.io
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -94,7 +94,10 @@
 ### Changelog
 
 #### 1.0.0
 * Initial Release
 
 #### 1.0.1
 * Minor bugfixes
+
+#### 1.0.2
+* Minor bugfixes
```

### Comparing `python-blockbee-checkout-1.0.1/setup.py` & `python-blockbee-checkout-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
 
     name='python-blockbee-checkout',
 
-    version='1.0.1',
+    version='1.0.2',
 
     packages=find_packages(),
 
     author="BlockBee",
 
     author_email="info@blockbee.io",
     install_requires=[
```

