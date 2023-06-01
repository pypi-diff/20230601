# Comparing `tmp/beancount_cc_importers-0.1.0-2-py3-none-any.whl.zip` & `tmp/beancount_cc_importers-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,14 @@
-Zip file size: 18834 bytes, number of entries: 10
+Zip file size: 20900 bytes, number of entries: 12
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-03 02:09 beancount_cc_importers/__init__.py
 -rw-rw-rw-  2.0 fat     3139 b- defN 23-Jun-01 05:12 beancount_cc_importers/alipay.py
 -rw-rw-rw-  2.0 fat     1980 b- defN 23-Jan-11 05:17 beancount_cc_importers/cmb.py
 -rw-rw-rw-  2.0 fat     2046 b- defN 23-Jan-11 05:18 beancount_cc_importers/eml.py
 -rw-rw-rw-  2.0 fat     3568 b- defN 23-Mar-03 06:11 beancount_cc_importers/lingqian.py
--rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-01 06:32 beancount_cc_importers-0.1.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      777 b- defN 23-Jun-01 06:32 beancount_cc_importers-0.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 06:32 beancount_cc_importers-0.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-01 06:32 beancount_cc_importers-0.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      901 b- defN 23-Jun-01 06:32 beancount_cc_importers-0.1.0.dist-info/RECORD
-10 files, 48349 bytes uncompressed, 17268 bytes compressed:  64.3%
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Jun-01 06:31 beancount_cc_importers/util/__init__.py
+-rw-rw-rw-  2.0 fat     6269 b- defN 23-Mar-03 08:05 beancount_cc_importers/util/eml2csv.py
+-rw-rw-rw-  2.0 fat    35823 b- defN 23-Jun-01 06:42 beancount_cc_importers-0.1.1.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      777 b- defN 23-Jun-01 06:42 beancount_cc_importers-0.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-01 06:42 beancount_cc_importers-0.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       23 b- defN 23-Jun-01 06:42 beancount_cc_importers-0.1.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1089 b- defN 23-Jun-01 06:42 beancount_cc_importers-0.1.1.dist-info/RECORD
+12 files, 54806 bytes uncompressed, 19028 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -9,23 +9,29 @@
 
 Filename: beancount_cc_importers/eml.py
 Comment: 
 
 Filename: beancount_cc_importers/lingqian.py
 Comment: 
 
-Filename: beancount_cc_importers-0.1.0.dist-info/LICENSE
+Filename: beancount_cc_importers/util/__init__.py
 Comment: 
 
-Filename: beancount_cc_importers-0.1.0.dist-info/METADATA
+Filename: beancount_cc_importers/util/eml2csv.py
 Comment: 
 
-Filename: beancount_cc_importers-0.1.0.dist-info/WHEEL
+Filename: beancount_cc_importers-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: beancount_cc_importers-0.1.0.dist-info/top_level.txt
+Filename: beancount_cc_importers-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: beancount_cc_importers-0.1.0.dist-info/RECORD
+Filename: beancount_cc_importers-0.1.1.dist-info/WHEEL
+Comment: 
+
+Filename: beancount_cc_importers-0.1.1.dist-info/top_level.txt
+Comment: 
+
+Filename: beancount_cc_importers-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `beancount_cc_importers-0.1.0.dist-info/LICENSE` & `beancount_cc_importers-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `beancount_cc_importers-0.1.0.dist-info/METADATA` & `beancount_cc_importers-0.1.1.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beancount-cc-importers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Beancount plugins to import bank debts
 Home-page: https://github.com/chen-chao/beancount_cc_importers
 Author: Chao Chen
 Author-email: Chao Chen <wenbushi@gmail.com>
 License: GPL-3.0
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

