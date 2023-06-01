# Comparing `tmp/alibabacloud_airticketopen20230117-1.0.6.tar.gz` & `tmp/alibabacloud_airticketopen20230117-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_airticketopen20230117-1.0.6.tar", last modified: Thu May 18 09:10:15 2023, max compression
+gzip compressed data, was "dist/alibabacloud_airticketopen20230117-2.0.0.tar", last modified: Thu Jun  1 04:11:37 2023, max compression
```

## Comparing `alibabacloud_airticketopen20230117-1.0.6.tar` & `alibabacloud_airticketopen20230117-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/
--rw-r--r--   0 root         (0) root         (0)       76 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2388 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1052 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1137 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104846 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117/client.py
--rw-r--r--   0 root         (0) root         (0)   506629 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2388 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      500 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2660 2023-05-18 09:10:15.000000 alibabacloud_airticketopen20230117-1.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1137 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104846 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/client.py
+-rw-r--r--   0 root         (0) root         (0)   506226 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2388 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      156 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2660 2023-06-01 04:11:37.000000 alibabacloud_airticketopen20230117-2.0.0/setup.py
```

### Comparing `alibabacloud_airticketopen20230117-1.0.6/LICENSE` & `alibabacloud_airticketopen20230117-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-1.0.6/PKG-INFO` & `alibabacloud_airticketopen20230117-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_airticketopen20230117
-Version: 1.0.6
+Version: 2.0.0
 Summary: Alibaba Cloud airticketOpen (20230117) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_airticketopen20230117-1.0.6/README-CN.md` & `alibabacloud_airticketopen20230117-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-1.0.6/README.md` & `alibabacloud_airticketopen20230117-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117/client.py` & `alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117/models.py` & `alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1990,48 +1990,42 @@
         if m.get('mobile_country_code') is not None:
             self.mobile_country_code = m.get('mobile_country_code')
         if m.get('mobile_phone_num') is not None:
             self.mobile_phone_num = m.get('mobile_phone_num')
         return self
 
 
-class BookRequestPassengerAncillaryPurchaseMapListAncillaryList(TeaModel):
+class BookRequestPassengerAncillaryPurchaseMapListBookAncillaryReqItem(TeaModel):
     def __init__(
         self,
         ancillary_id: str = None,
-        ancillary_info: Dict[str, Any] = None,
         ancillary_type: int = None,
     ):
         self.ancillary_id = ancillary_id
-        self.ancillary_info = ancillary_info
         self.ancillary_type = ancillary_type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         if self.ancillary_id is not None:
             result['ancillary_id'] = self.ancillary_id
-        if self.ancillary_info is not None:
-            result['ancillary_info'] = self.ancillary_info
         if self.ancillary_type is not None:
             result['ancillary_type'] = self.ancillary_type
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('ancillary_id') is not None:
             self.ancillary_id = m.get('ancillary_id')
-        if m.get('ancillary_info') is not None:
-            self.ancillary_info = m.get('ancillary_info')
         if m.get('ancillary_type') is not None:
             self.ancillary_type = m.get('ancillary_type')
         return self
 
 
 class BookRequestPassengerAncillaryPurchaseMapListPassengerListCredential(TeaModel):
     def __init__(
@@ -2154,53 +2148,47 @@
             self.type = m.get('type')
         return self
 
 
 class BookRequestPassengerAncillaryPurchaseMapList(TeaModel):
     def __init__(
         self,
-        ancillary_list: List[BookRequestPassengerAncillaryPurchaseMapListAncillaryList] = None,
+        book_ancillary_req_item: BookRequestPassengerAncillaryPurchaseMapListBookAncillaryReqItem = None,
         passenger_list: List[BookRequestPassengerAncillaryPurchaseMapListPassengerList] = None,
     ):
-        self.ancillary_list = ancillary_list
+        self.book_ancillary_req_item = book_ancillary_req_item
         self.passenger_list = passenger_list
 
     def validate(self):
-        if self.ancillary_list:
-            for k in self.ancillary_list:
-                if k:
-                    k.validate()
+        if self.book_ancillary_req_item:
+            self.book_ancillary_req_item.validate()
         if self.passenger_list:
             for k in self.passenger_list:
                 if k:
                     k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
-        result['ancillary_list'] = []
-        if self.ancillary_list is not None:
-            for k in self.ancillary_list:
-                result['ancillary_list'].append(k.to_map() if k else None)
+        if self.book_ancillary_req_item is not None:
+            result['book_ancillary_req_item'] = self.book_ancillary_req_item.to_map()
         result['passenger_list'] = []
         if self.passenger_list is not None:
             for k in self.passenger_list:
                 result['passenger_list'].append(k.to_map() if k else None)
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
-        self.ancillary_list = []
-        if m.get('ancillary_list') is not None:
-            for k in m.get('ancillary_list'):
-                temp_model = BookRequestPassengerAncillaryPurchaseMapListAncillaryList()
-                self.ancillary_list.append(temp_model.from_map(k))
+        if m.get('book_ancillary_req_item') is not None:
+            temp_model = BookRequestPassengerAncillaryPurchaseMapListBookAncillaryReqItem()
+            self.book_ancillary_req_item = temp_model.from_map(m['book_ancillary_req_item'])
         self.passenger_list = []
         if m.get('passenger_list') is not None:
             for k in m.get('passenger_list'):
                 temp_model = BookRequestPassengerAncillaryPurchaseMapListPassengerList()
                 self.passenger_list.append(temp_model.from_map(k))
         return self
```

### Comparing `alibabacloud_airticketopen20230117-1.0.6/alibabacloud_airticketopen20230117.egg-info/PKG-INFO` & `alibabacloud_airticketopen20230117-2.0.0/alibabacloud_airticketopen20230117.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-airticketopen20230117
-Version: 1.0.6
+Version: 2.0.0
 Summary: Alibaba Cloud airticketOpen (20230117) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_airticketopen20230117-1.0.6/setup.py` & `alibabacloud_airticketopen20230117-2.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_airticketopen20230117.
 
-Created on 18/05/2023
+Created on 01/06/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_airticketopen20230117"
 NAME = "alibabacloud_airticketopen20230117" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud airticketOpen (20230117) SDK Library for Python"
```

