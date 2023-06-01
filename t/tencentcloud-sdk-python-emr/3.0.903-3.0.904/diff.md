# Comparing `tmp/tencentcloud-sdk-python-emr-3.0.903.tar.gz` & `tmp/tencentcloud-sdk-python-emr-3.0.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.903.tar", last modified: Wed May 31 02:11:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-emr-3.0.904.tar", last modified: Thu Jun  1 02:34:28 2023, max compression
```

## Comparing `tencentcloud-sdk-python-emr-3.0.903.tar` & `tencentcloud-sdk-python-emr-3.0.904.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud/emr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)    27330 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)    13881 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud/emr/v20190103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)   258513 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud_sdk_python_emr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/tencentcloud_sdk_python_emr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:11:15.000000 tencentcloud-sdk-python-emr-3.0.903/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)    27330 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)    13881 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud/emr/v20190103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260148 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud_sdk_python_emr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud_sdk_python_emr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud_sdk_python_emr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud_sdk_python_emr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/tencentcloud_sdk_python_emr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:34:28.000000 tencentcloud-sdk-python-emr-3.0.904/setup.cfg
```

### Comparing `tencentcloud-sdk-python-emr-3.0.903/README.rst` & `tencentcloud-sdk-python-emr-3.0.904/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.903/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-emr-3.0.904/tencentcloud/emr/v20190103/emr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.903/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-emr-3.0.904/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-emr-3.0.903/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-emr-3.0.904/tencentcloud/emr/v20190103/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1340,22 +1340,39 @@
 
     def __init__(self):
         r"""
         :param InstanceId: 集群实例ID
         :type InstanceId: str
         :param UserNameList: 集群用户名列表
         :type UserNameList: list of str
+        :param TkeClusterId: tke/eks集群id，容器集群传
+        :type TkeClusterId: str
+        :param DisplayStrategy: 默认空，容器版传"native"
+        :type DisplayStrategy: str
+        :param UserGroupList: 用户组
+        :type UserGroupList: list of UserAndGroup
         """
         self.InstanceId = None
         self.UserNameList = None
+        self.TkeClusterId = None
+        self.DisplayStrategy = None
+        self.UserGroupList = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.UserNameList = params.get("UserNameList")
+        self.TkeClusterId = params.get("TkeClusterId")
+        self.DisplayStrategy = params.get("DisplayStrategy")
+        if params.get("UserGroupList") is not None:
+            self.UserGroupList = []
+            for item in params.get("UserGroupList"):
+                obj = UserAndGroup()
+                obj._deserialize(item)
+                self.UserGroupList.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -6604,14 +6621,44 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
+
+
+class UserAndGroup(AbstractModel):
+    """容器集群用户组信息
+
+    """
+
+    def __init__(self):
+        r"""
+        :param UserName: 用户名
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserName: str
+        :param UserGroup: 用户组
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UserGroup: str
+        """
+        self.UserName = None
+        self.UserGroup = None
+
+
+    def _deserialize(self, params):
+        self.UserName = params.get("UserName")
+        self.UserGroup = params.get("UserGroup")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
 
 
 class UserInfoForUserManager(AbstractModel):
     """添加的用户信息列表
 
     """
```

### Comparing `tencentcloud-sdk-python-emr-3.0.903/tencentcloud/__init__.py` & `tencentcloud-sdk-python-emr-3.0.904/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-emr-3.0.903/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.904/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.903/tencentcloud_sdk_python_emr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-emr-3.0.904/tencentcloud_sdk_python_emr.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-emr
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Emr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-emr-3.0.903/setup.py` & `tencentcloud-sdk-python-emr-3.0.904/setup.py`

 * *Files identical despite different names*

