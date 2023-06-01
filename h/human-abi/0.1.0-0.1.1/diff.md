# Comparing `tmp/human_abi-0.1.0.tar.gz` & `tmp/human_abi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "human_abi-0.1.0.tar", max compression
+gzip compressed data, was "human_abi-0.1.1.tar", max compression
```

## Comparing `human_abi-0.1.0.tar` & `human_abi-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      549 2023-06-01 09:26:27.543015 human_abi-0.1.0/LICENSE
--rw-r--r--   0        0        0     1120 2023-06-01 09:32:34.959988 human_abi-0.1.0/README.md
--rw-r--r--   0        0        0      314 2023-06-01 09:32:38.343861 human_abi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4163 2023-06-01 09:23:50.240071 human_abi-0.1.0/readable_abi/__init__.py
--rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 human_abi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      549 2023-06-01 09:26:27.543015 human_abi-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1120 2023-06-01 09:33:02.716638 human_abi-0.1.1/README.md
+-rw-r--r--   0        0        0     4163 2023-06-01 09:23:50.240071 human_abi-0.1.1/human_abi/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-01 09:37:12.999775 human_abi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1662 1970-01-01 00:00:00.000000 human_abi-0.1.1/PKG-INFO
```

### Comparing `human_abi-0.1.0/LICENSE` & `human_abi-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `human_abi-0.1.0/README.md` & `human_abi-0.1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Human ABI
 
 ## Summary
 
 This package provides a way to parse [Human Readable ABI](https://docs.ethers.org/v5/api/utils/abi/formats/#abi-formats--human-readable-abi) introduced by [ethers.js](https://ethers.org/) to the Python world. It's still pretty much a WIP. The goal is to be fully compatible with [ethers.js](https://ethers.org/) and [ethers-rs](https://github.com/gakonst/ethers-rs).
 
 ```bash
-$ pip install human_abi
+$ pip install human-abi
 ```
 
 ```py
 from human_abi import HumanReadableParser
 
 parser = HumanReadableParser('event TestEvent(uint indexed id, (string, uint16, (uint8, uint8)) value)')
 print(parser.take_event())
```

### Comparing `human_abi-0.1.0/readable_abi/__init__.py` & `human_abi-0.1.1/human_abi/__init__.py`

 * *Files identical despite different names*

### Comparing `human_abi-0.1.0/PKG-INFO` & `human_abi-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: human-abi
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Sorawit Suriyakarn
 Author-email: swit@blockpipe.io
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -17,15 +17,15 @@
 # Human ABI
 
 ## Summary
 
 This package provides a way to parse [Human Readable ABI](https://docs.ethers.org/v5/api/utils/abi/formats/#abi-formats--human-readable-abi) introduced by [ethers.js](https://ethers.org/) to the Python world. It's still pretty much a WIP. The goal is to be fully compatible with [ethers.js](https://ethers.org/) and [ethers-rs](https://github.com/gakonst/ethers-rs).
 
 ```bash
-$ pip install human_abi
+$ pip install human-abi
 ```
 
 ```py
 from human_abi import HumanReadableParser
 
 parser = HumanReadableParser('event TestEvent(uint indexed id, (string, uint16, (uint8, uint8)) value)')
 print(parser.take_event())
```

