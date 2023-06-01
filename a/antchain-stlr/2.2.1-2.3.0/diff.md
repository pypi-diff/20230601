# Comparing `tmp/antchain_stlr-2.2.1.tar.gz` & `tmp/antchain_stlr-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_stlr-2.2.1.tar", last modified: Mon May 22 06:02:56 2023, max compression
+gzip compressed data, was "dist/antchain_stlr-2.3.0.tar", last modified: Thu Jun  1 06:07:09 2023, max compression
```

## Comparing `antchain_stlr-2.2.1.tar` & `antchain_stlr-2.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/
--rw-r--r--   0 root         (0) root         (0)      600 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/README-CN.md
--rw-r--r--   0 root         (0) root         (0)      993 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_sdk_stlr/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_sdk_stlr/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96687 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_sdk_stlr/client.py
--rw-r--r--   0 root         (0) root         (0)   229440 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_sdk_stlr/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2168 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/antchain_stlr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2493 2023-05-22 06:02:56.000000 antchain_stlr-2.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:07:09.000000 antchain_stlr-2.3.0/
+-rw-r--r--   0 root         (0) root         (0)      600 2023-06-01 06:07:08.000000 antchain_stlr-2.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-01 06:07:08.000000 antchain_stlr-2.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-01 06:07:09.000000 antchain_stlr-2.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      807 2023-06-01 06:07:08.000000 antchain_stlr-2.3.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)      993 2023-06-01 06:07:08.000000 antchain_stlr-2.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:07:09.000000 antchain_stlr-2.3.0/antchain_sdk_stlr/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-01 06:07:08.000000 antchain_stlr-2.3.0/antchain_sdk_stlr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101739 2023-06-01 06:07:08.000000 antchain_stlr-2.3.0/antchain_sdk_stlr/client.py
+-rw-r--r--   0 root         (0) root         (0)   239571 2023-06-01 06:07:08.000000 antchain_stlr-2.3.0/antchain_sdk_stlr/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 06:07:09.000000 antchain_stlr-2.3.0/antchain_stlr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2168 2023-06-01 06:07:09.000000 antchain_stlr-2.3.0/antchain_stlr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      331 2023-06-01 06:07:09.000000 antchain_stlr-2.3.0/antchain_stlr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 06:07:09.000000 antchain_stlr-2.3.0/antchain_stlr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2023-06-01 06:07:09.000000 antchain_stlr-2.3.0/antchain_stlr.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-01 06:07:09.000000 antchain_stlr-2.3.0/antchain_stlr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-06-01 06:07:09.000000 antchain_stlr-2.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-06-01 06:07:08.000000 antchain_stlr-2.3.0/setup.py
```

### Comparing `antchain_stlr-2.2.1/LICENSE` & `antchain_stlr-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.2.1/PKG-INFO` & `antchain_stlr-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_stlr
-Version: 2.2.1
+Version: 2.3.0
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.2.1/README-CN.md` & `antchain_stlr-2.3.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.2.1/README.md` & `antchain_stlr-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `antchain_stlr-2.2.1/antchain_sdk_stlr/client.py` & `antchain_stlr-2.3.0/antchain_sdk_stlr/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '2.2.1',
+                    'sdk_version': '2.3.0',
                     '_prod_code': 'STLR',
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
-                    'sdk_version': '2.2.1',
+                    'sdk_version': '2.3.0',
                     '_prod_code': 'STLR',
                     '_prod_channel': 'undefined'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
@@ -2209,14 +2209,126 @@
         """
         UtilClient.validate_model(request)
         return TeaCore.from_map(
             stlr_models.ListEcarOffsetdatumResponse(),
             await self.do_request_async('1.0', 'antchain.carbon.ecar.offsetdatum.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def list_ecar_enterprisemember(
+        self,
+        request: stlr_models.ListEcarEnterprisememberRequest,
+    ) -> stlr_models.ListEcarEnterprisememberResponse:
+        """
+        Description: 机构会员列表查询，支持分页查询指定时间范围内的会员列表，返回结果按照会员注册时间降序排列
+        Summary: 机构会员列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.list_ecar_enterprisemember_ex(request, headers, runtime)
+
+    async def list_ecar_enterprisemember_async(
+        self,
+        request: stlr_models.ListEcarEnterprisememberRequest,
+    ) -> stlr_models.ListEcarEnterprisememberResponse:
+        """
+        Description: 机构会员列表查询，支持分页查询指定时间范围内的会员列表，返回结果按照会员注册时间降序排列
+        Summary: 机构会员列表查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.list_ecar_enterprisemember_ex_async(request, headers, runtime)
+
+    def list_ecar_enterprisemember_ex(
+        self,
+        request: stlr_models.ListEcarEnterprisememberRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.ListEcarEnterprisememberResponse:
+        """
+        Description: 机构会员列表查询，支持分页查询指定时间范围内的会员列表，返回结果按照会员注册时间降序排列
+        Summary: 机构会员列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.ListEcarEnterprisememberResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.enterprisemember.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def list_ecar_enterprisemember_ex_async(
+        self,
+        request: stlr_models.ListEcarEnterprisememberRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.ListEcarEnterprisememberResponse:
+        """
+        Description: 机构会员列表查询，支持分页查询指定时间范围内的会员列表，返回结果按照会员注册时间降序排列
+        Summary: 机构会员列表查询
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.ListEcarEnterprisememberResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.enterprisemember.list', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def preview_ecar_offsetdatum(
+        self,
+        request: stlr_models.PreviewEcarOffsetdatumRequest,
+    ) -> stlr_models.PreviewEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠项目数据预览，包括注册会员数和累积碳能量值
+        Summary: 碳普惠项目数据预览
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.preview_ecar_offsetdatum_ex(request, headers, runtime)
+
+    async def preview_ecar_offsetdatum_async(
+        self,
+        request: stlr_models.PreviewEcarOffsetdatumRequest,
+    ) -> stlr_models.PreviewEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠项目数据预览，包括注册会员数和累积碳能量值
+        Summary: 碳普惠项目数据预览
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.preview_ecar_offsetdatum_ex_async(request, headers, runtime)
+
+    def preview_ecar_offsetdatum_ex(
+        self,
+        request: stlr_models.PreviewEcarOffsetdatumRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.PreviewEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠项目数据预览，包括注册会员数和累积碳能量值
+        Summary: 碳普惠项目数据预览
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.PreviewEcarOffsetdatumResponse(),
+            self.do_request('1.0', 'antchain.carbon.ecar.offsetdatum.preview', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def preview_ecar_offsetdatum_ex_async(
+        self,
+        request: stlr_models.PreviewEcarOffsetdatumRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> stlr_models.PreviewEcarOffsetdatumResponse:
+        """
+        Description: 碳普惠项目数据预览，包括注册会员数和累积碳能量值
+        Summary: 碳普惠项目数据预览
+        """
+        UtilClient.validate_model(request)
+        return TeaCore.from_map(
+            stlr_models.PreviewEcarOffsetdatumResponse(),
+            await self.do_request_async('1.0', 'antchain.carbon.ecar.offsetdatum.preview', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_third_cert(
         self,
         request: stlr_models.QueryThirdCertRequest,
     ) -> stlr_models.QueryThirdCertResponse:
         """
         Description: 三方平台调用此接口，查询用户的证书信息
         Summary: 证书查询
```

### Comparing `antchain_stlr-2.2.1/antchain_sdk_stlr/models.py` & `antchain_stlr-2.3.0/antchain_sdk_stlr/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -661,14 +661,64 @@
         if m.get('counteraction_amount') is not None:
             self.counteraction_amount = m.get('counteraction_amount')
         if m.get('data_unit') is not None:
             self.data_unit = m.get('data_unit')
         return self
 
 
+class EnterpriseMemberSummary(TeaModel):
+    def __init__(
+        self,
+        account_did: str = None,
+        name: str = None,
+        mobile: str = None,
+        register_time: str = None,
+    ):
+        # 机构会员DID
+        self.account_did = account_did
+        # 会员姓名，数据脱敏处理返回
+        self.name = name
+        # 会员手机号码，数据脱敏处理返回
+        self.mobile = mobile
+        # 会员注册时间
+        self.register_time = register_time
+
+    def validate(self):
+        self.validate_required(self.account_did, 'account_did')
+        self.validate_required(self.register_time, 'register_time')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.account_did is not None:
+            result['account_did'] = self.account_did
+        if self.name is not None:
+            result['name'] = self.name
+        if self.mobile is not None:
+            result['mobile'] = self.mobile
+        if self.register_time is not None:
+            result['register_time'] = self.register_time
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('account_did') is not None:
+            self.account_did = m.get('account_did')
+        if m.get('name') is not None:
+            self.name = m.get('name')
+        if m.get('mobile') is not None:
+            self.mobile = m.get('mobile')
+        if m.get('register_time') is not None:
+            self.register_time = m.get('register_time')
+        return self
+
+
 class AnyStatisticalItem(TeaModel):
     def __init__(
         self,
         item_code: str = None,
         amount: str = None,
         unit: str = None,
         unit_label: str = None,
@@ -5132,24 +5182,27 @@
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         account_did: str = None,
         name: str = None,
         identity_card_code: str = None,
+        mobile: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 注册会员在蚂蚁DIS服务的DID账号
         self.account_did = account_did
         # 注册会员姓名
         self.name = name
         # 注册会员身份证号码
         self.identity_card_code = identity_card_code
+        # 手机号码
+        self.mobile = mobile
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
@@ -5162,28 +5215,32 @@
             result['product_instance_id'] = self.product_instance_id
         if self.account_did is not None:
             result['account_did'] = self.account_did
         if self.name is not None:
             result['name'] = self.name
         if self.identity_card_code is not None:
             result['identity_card_code'] = self.identity_card_code
+        if self.mobile is not None:
+            result['mobile'] = self.mobile
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('account_did') is not None:
             self.account_did = m.get('account_did')
         if m.get('name') is not None:
             self.name = m.get('name')
         if m.get('identity_card_code') is not None:
             self.identity_card_code = m.get('identity_card_code')
+        if m.get('mobile') is not None:
+            self.mobile = m.get('mobile')
         return self
 
 
 class RegisterEcarEnterprisememberResponse(TeaModel):
     def __init__(
         self,
         req_msg_id: str = None,
@@ -5651,15 +5708,15 @@
         self.occurrent_end_time = occurrent_end_time
         # 碳普惠平台编码
         self.carbon_offset_platform_no = carbon_offset_platform_no
         # 发生场景编码，需指定相关碳普惠平台的场景编码，可以指定多个场景
         self.scenario_code = scenario_code
         # 分页查询数据时的页码，从1开始，不传入时默认值为1
         self.current = current
-        # 每页数据量，默认值为20，取值范围为[10,100]
+        # 每页数据量，默认值为20，取值范围为[10,200]
         self.page_size = page_size
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -5788,14 +5845,251 @@
         if m.get('list') is not None:
             for k in m.get('list'):
                 temp_model = CarbonOffsetAcquisitionItem()
                 self.list.append(temp_model.from_map(k))
         return self
 
 
+class ListEcarEnterprisememberRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        register_start_time: str = None,
+        register_end_time: str = None,
+        current: int = None,
+        page_size: int = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 会员注册开始时间
+        self.register_start_time = register_start_time
+        # 会员注册结束时间
+        self.register_end_time = register_end_time
+        # 当前查询页码，默认值为1
+        self.current = current
+        # 每页记录条数，默认为20，取值范围为[10,200]
+        self.page_size = page_size
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.register_start_time is not None:
+            result['register_start_time'] = self.register_start_time
+        if self.register_end_time is not None:
+            result['register_end_time'] = self.register_end_time
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('register_start_time') is not None:
+            self.register_start_time = m.get('register_start_time')
+        if m.get('register_end_time') is not None:
+            self.register_end_time = m.get('register_end_time')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        return self
+
+
+class ListEcarEnterprisememberResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        current: int = None,
+        page_size: int = None,
+        total: int = None,
+        list: List[EnterpriseMemberSummary] = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 当前查询的页码
+        self.current = current
+        # 每页记录条数
+        self.page_size = page_size
+        # 记录总条数
+        self.total = total
+        # 会员资料列表
+        self.list = list
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.current is not None:
+            result['current'] = self.current
+        if self.page_size is not None:
+            result['page_size'] = self.page_size
+        if self.total is not None:
+            result['total'] = self.total
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('current') is not None:
+            self.current = m.get('current')
+        if m.get('page_size') is not None:
+            self.page_size = m.get('page_size')
+        if m.get('total') is not None:
+            self.total = m.get('total')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = EnterpriseMemberSummary()
+                self.list.append(temp_model.from_map(k))
+        return self
+
+
+class PreviewEcarOffsetdatumRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        project_no: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 碳普惠项目编码
+        self.project_no = project_no
+
+    def validate(self):
+        self.validate_required(self.project_no, 'project_no')
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.project_no is not None:
+            result['project_no'] = self.project_no
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('project_no') is not None:
+            self.project_no = m.get('project_no')
+        return self
+
+
+class PreviewEcarOffsetdatumResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        register_member_total: int = None,
+        carbon_energy_total: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 注册会员总数
+        self.register_member_total = register_member_total
+        # 碳总能量值
+        self.carbon_energy_total = carbon_energy_total
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.register_member_total is not None:
+            result['register_member_total'] = self.register_member_total
+        if self.carbon_energy_total is not None:
+            result['carbon_energy_total'] = self.carbon_energy_total
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('register_member_total') is not None:
+            self.register_member_total = m.get('register_member_total')
+        if m.get('carbon_energy_total') is not None:
+            self.carbon_energy_total = m.get('carbon_energy_total')
+        return self
+
+
 class QueryThirdCertRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         product_id: str = None,
         certification_type: str = None,
```

### Comparing `antchain_stlr-2.2.1/antchain_stlr.egg-info/PKG-INFO` & `antchain_stlr-2.3.0/antchain_stlr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-stlr
-Version: 2.2.1
+Version: 2.3.0
 Summary: Ant Chain STLR SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_stlr-2.2.1/setup.py` & `antchain_stlr-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_stlr.
 
-Created on 22/05/2023
+Created on 01/06/2023
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_stlr"
 NAME = "antchain_stlr" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain STLR SDK Library for Python"
```

