# Comparing `tmp/tencentcloud-sdk-python-dcdb-3.0.903.tar.gz` & `tmp/tencentcloud-sdk-python-dcdb-3.0.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.903.tar", last modified: Wed May 31 02:09:47 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-dcdb-3.0.904.tar", last modified: Thu Jun  1 02:32:54 2023, max compression
```

## Comparing `tencentcloud-sdk-python-dcdb-3.0.903.tar` & `tencentcloud-sdk-python-dcdb-3.0.904.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud_sdk_python_dcdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/dcdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/dcdb/v20180411/
--rw-r--r--   0 root         (0) root         (0)    13609 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/dcdb/v20180411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/dcdb/v20180411/__init__.py
--rw-r--r--   0 root         (0) root         (0)   238676 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/dcdb/v20180411/models.py
--rw-r--r--   0 root         (0) root         (0)    69104 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/dcdb/v20180411/dcdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/dcdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1664 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1008 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:09:47.000000 tencentcloud-sdk-python-dcdb-3.0.903/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud_sdk_python_dcdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud_sdk_python_dcdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud_sdk_python_dcdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud_sdk_python_dcdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/dcdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/dcdb/v20180411/
+-rw-r--r--   0 root         (0) root         (0)    13722 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/dcdb/v20180411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/dcdb/v20180411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   241269 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/dcdb/v20180411/models.py
+-rw-r--r--   0 root         (0) root         (0)    70022 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/dcdb/v20180411/dcdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/dcdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1664 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:32:54.000000 tencentcloud-sdk-python-dcdb-3.0.904/setup.cfg
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud_sdk_python_dcdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.903/README.rst` & `tencentcloud-sdk-python-dcdb-3.0.904/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/dcdb/v20180411/errorcodes.py` & `tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/dcdb/v20180411/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,17 @@
 
 # 拉取安全组详情失败。
 FAILEDOPERATION_GETSECURITYGROUPDETAILFAILED = 'FailedOperation.GetSecurityGroupDetailFailed'
 
 # 修改账号权限失败。
 FAILEDOPERATION_MODIFYRIGHTFAILED = 'FailedOperation.ModifyRightFailed'
 
+# 修改账号配置失败。
+FAILEDOPERATION_MODIFYUSERCONFIGFAILED = 'FailedOperation.ModifyUserConfigFailed'
+
 # 消息队列操作失败。
 FAILEDOPERATION_MSGQUEUEOPERATIONFAILED = 'FailedOperation.MsgQueueOperationFailed'
 
 # 隔离实例失败。
 FAILEDOPERATION_OSSISOLATEINSTANCEFAILED = 'FailedOperation.OssIsolateInstanceFailed'
 
 # 请求后端接口失败。
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/dcdb/v20180411/models.py` & `tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/dcdb/v20180411/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -399,14 +399,42 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ConfigValue(AbstractModel):
+    """配置信息。包含配置项Config，配置值Value
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Config: 配置项的名称，支持填写max_user_connections
+        :type Config: str
+        :param Value: 配置值
+        :type Value: str
+        """
+        self.Config = None
+        self.Value = None
+
+
+    def _deserialize(self, params):
+        self.Config = params.get("Config")
+        self.Value = params.get("Value")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ConstraintRange(AbstractModel):
     """约束类型值的范围
 
     """
 
     def __init__(self):
         r"""
@@ -4616,14 +4644,72 @@
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class ModifyAccountConfigRequest(AbstractModel):
+    """ModifyAccountConfig请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param InstanceId: 实例 ID，格式如：tdsqlshard-kpkvq5oj，与云数据库控制台页面中显示的实例 ID 相同。
+        :type InstanceId: str
+        :param UserName: 账号的名称
+        :type UserName: str
+        :param Host: 账号的域名
+        :type Host: str
+        :param Configs: 配置列表，每一个元素是Config和Value的组合
+        :type Configs: list of ConfigValue
+        """
+        self.InstanceId = None
+        self.UserName = None
+        self.Host = None
+        self.Configs = None
+
+
+    def _deserialize(self, params):
+        self.InstanceId = params.get("InstanceId")
+        self.UserName = params.get("UserName")
+        self.Host = params.get("Host")
+        if params.get("Configs") is not None:
+            self.Configs = []
+            for item in params.get("Configs"):
+                obj = ConfigValue()
+                obj._deserialize(item)
+                self.Configs.append(obj)
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyAccountConfigResponse(AbstractModel):
+    """ModifyAccountConfig返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        self.RequestId = params.get("RequestId")
+
+
 class ModifyAccountDescriptionRequest(AbstractModel):
     """ModifyAccountDescription请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/dcdb/v20180411/dcdb_client.py` & `tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/dcdb/v20180411/dcdb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1178,14 +1178,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def ModifyAccountConfig(self, request):
+        """修改账号的一些配置，比如 max_user_connections
+
+        :param request: Request instance for ModifyAccountConfig.
+        :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyAccountConfigRequest`
+        :rtype: :class:`tencentcloud.dcdb.v20180411.models.ModifyAccountConfigResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyAccountConfig", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyAccountConfigResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def ModifyAccountDescription(self, request):
         """本接口（ModifyAccountDescription）用于修改云数据库账号备注。
         注意：相同用户名，不同Host是不同的账号。
 
         :param request: Request instance for ModifyAccountDescription.
         :type request: :class:`tencentcloud.dcdb.v20180411.models.ModifyAccountDescriptionRequest`
         :rtype: :class:`tencentcloud.dcdb.v20180411.models.ModifyAccountDescriptionResponse`
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.903/tencentcloud/__init__.py` & `tencentcloud-sdk-python-dcdb-3.0.904/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.903'
+__version__ = '3.0.904'
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.903/PKG-INFO` & `tencentcloud-sdk-python-dcdb-3.0.904/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-dcdb
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Dcdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-dcdb-3.0.903/setup.py` & `tencentcloud-sdk-python-dcdb-3.0.904/setup.py`

 * *Files identical despite different names*

