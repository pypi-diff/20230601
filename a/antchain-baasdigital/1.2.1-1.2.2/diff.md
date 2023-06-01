# Comparing `tmp/antchain_baasdigital-1.2.1.tar.gz` & `tmp/antchain_baasdigital-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_baasdigital-1.2.1.tar", last modified: Fri Mar  3 05:26:02 2023, max compression
+gzip compressed data, was "dist/antchain_baasdigital-1.2.2.tar", last modified: Thu Jun  1 06:15:10 2023, max compression
```

## Comparing `antchain_baasdigital-1.2.1.tar` & `antchain_baasdigital-1.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/
--rw-r--r--   0 root         (0) root         (0)      600 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2210 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      828 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1014 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/antchain_baasdigital.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2210 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/antchain_baasdigital.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      387 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/antchain_baasdigital.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/antchain_baasdigital.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/antchain_baasdigital.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/antchain_baasdigital.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/antchain_sdk_baasdigital/
--rw-r--r--   0 root         (0) root         (0)       21 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/antchain_sdk_baasdigital/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93892 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/antchain_sdk_baasdigital/client.py
--rw-r--r--   0 root         (0) root         (0)   186315 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/antchain_sdk_baasdigital/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2528 2023-03-03 05:26:02.000000 antchain_baasdigital-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      828 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1014 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/antchain_baasdigital.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/antchain_baasdigital.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      387 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/antchain_baasdigital.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/antchain_baasdigital.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/antchain_baasdigital.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/antchain_baasdigital.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/antchain_sdk_baasdigital/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/antchain_sdk_baasdigital/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93892 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/antchain_sdk_baasdigital/client.py
+-rw-r--r--   0 root         (0) root         (0)   186857 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/antchain_sdk_baasdigital/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2528 2023-06-01 06:15:10.000000 antchain_baasdigital-1.2.2/setup.py
```

### Comparing `antchain_baasdigital-1.2.1/LICENSE` & `antchain_baasdigital-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_baasdigital-1.2.1/PKG-INFO` & `antchain_baasdigital-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_baasdigital
-Version: 1.2.1
+Version: 1.2.2
 Summary: Ant Chain BAASDIGITAL SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_baasdigital-1.2.1/README-CN.md` & `antchain_baasdigital-1.2.2/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_baasdigital-1.2.1/README.md` & `antchain_baasdigital-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `antchain_baasdigital-1.2.1/antchain_baasdigital.egg-info/PKG-INFO` & `antchain_baasdigital-1.2.2/antchain_baasdigital.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-baasdigital
-Version: 1.2.1
+Version: 1.2.2
 Summary: Ant Chain BAASDIGITAL SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_baasdigital-1.2.1/antchain_sdk_baasdigital/client.py` & `antchain_baasdigital-1.2.2/antchain_sdk_baasdigital/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.2.1',
+                    'sdk_version': '1.2.2',
                     '_prod_code': 'BAASDIGITAL',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -235,15 +235,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.2.1',
+                    'sdk_version': '1.2.2',
                     '_prod_code': 'BAASDIGITAL',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
```

### Comparing `antchain_baasdigital-1.2.1/antchain_sdk_baasdigital/models.py` & `antchain_baasdigital-1.2.2/antchain_sdk_baasdigital/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -386,14 +386,15 @@
         asset_uri: str = None,
         limited_amount: bool = None,
         write_offable: bool = None,
         burnable: bool = None,
         owner_account: str = None,
         issuer_list: List[str] = None,
         writeoff_list: List[str] = None,
+        address: str = None,
         create_time: int = None,
     ):
         # 数字权证项目id
         self.project_id = project_id
         # 模版类型
         # 1为共享型，2为独享型，3为高性能共享型，4为高性能独享型
         self.biz_type = biz_type
@@ -420,14 +421,16 @@
         self.burnable = burnable
         # 项目管理员账户地址
         self.owner_account = owner_account
         # 项目核销员账户地址列表
         self.issuer_list = issuer_list
         # 项目核销员账户地址列表
         self.writeoff_list = writeoff_list
+        # 项目部署的合约地址
+        self.address = address
         # 合约创建时间
         self.create_time = create_time
 
     def validate(self):
         self.validate_required(self.project_id, 'project_id')
         self.validate_required(self.biz_type, 'biz_type')
         self.validate_required(self.name, 'name')
@@ -471,14 +474,16 @@
             result['burnable'] = self.burnable
         if self.owner_account is not None:
             result['owner_account'] = self.owner_account
         if self.issuer_list is not None:
             result['issuer_list'] = self.issuer_list
         if self.writeoff_list is not None:
             result['writeoff_list'] = self.writeoff_list
+        if self.address is not None:
+            result['address'] = self.address
         if self.create_time is not None:
             result['create_time'] = self.create_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('project_id') is not None:
@@ -505,14 +510,16 @@
             self.burnable = m.get('burnable')
         if m.get('owner_account') is not None:
             self.owner_account = m.get('owner_account')
         if m.get('issuer_list') is not None:
             self.issuer_list = m.get('issuer_list')
         if m.get('writeoff_list') is not None:
             self.writeoff_list = m.get('writeoff_list')
+        if m.get('address') is not None:
+            self.address = m.get('address')
         if m.get('create_time') is not None:
             self.create_time = m.get('create_time')
         return self
 
 
 class AssetUriDefinition(TeaModel):
     def __init__(
@@ -2002,25 +2009,28 @@
     def __init__(
         self,
         req_msg_id: str = None,
         result_code: str = None,
         result_msg: str = None,
         project_id: str = None,
         hash: str = None,
+        address: str = None,
     ):
         # 请求唯一ID，用于链路跟踪和问题排查
         self.req_msg_id = req_msg_id
         # 结果码，一般OK表示调用成功
         self.result_code = result_code
         # 异常信息的文本描述
         self.result_msg = result_msg
         # 项目id
         self.project_id = project_id
         # 部署该项目到区块链的hash值
         self.hash = hash
+        # 该项目在链上部署的合约地址
+        self.address = address
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -2033,28 +2043,32 @@
             result['result_code'] = self.result_code
         if self.result_msg is not None:
             result['result_msg'] = self.result_msg
         if self.project_id is not None:
             result['project_id'] = self.project_id
         if self.hash is not None:
             result['hash'] = self.hash
+        if self.address is not None:
+            result['address'] = self.address
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('req_msg_id') is not None:
             self.req_msg_id = m.get('req_msg_id')
         if m.get('result_code') is not None:
             self.result_code = m.get('result_code')
         if m.get('result_msg') is not None:
             self.result_msg = m.get('result_msg')
         if m.get('project_id') is not None:
             self.project_id = m.get('project_id')
         if m.get('hash') is not None:
             self.hash = m.get('hash')
+        if m.get('address') is not None:
+            self.address = m.get('address')
         return self
 
 
 class UpdateProjectRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
```

### Comparing `antchain_baasdigital-1.2.1/setup.py` & `antchain_baasdigital-1.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_baasdigital.
 
-Created on 03/03/2023
+Created on 01/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_baasdigital"
 NAME = "antchain_baasdigital" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain BAASDIGITAL SDK Library for Python"
```

