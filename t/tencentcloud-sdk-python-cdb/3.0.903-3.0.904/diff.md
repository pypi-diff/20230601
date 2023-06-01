# Comparing `tmp/tencentcloud-sdk-python-cdb-3.0.903.tar.gz` & `tmp/tencentcloud-sdk-python-cdb-3.0.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.903.tar", last modified: Wed May 31 02:05:43 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cdb-3.0.904.tar", last modified: Thu Jun  1 02:28:38 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cdb-3.0.903.tar` & `tencentcloud-sdk-python-cdb-3.0.904.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/cdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)   150608 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/cdb/v20170320/cdb_client.py
--rw-r--r--   0 root         (0) root         (0)    18943 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   526224 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/cdb/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud_sdk_python_cdb.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:05:43.000000 tencentcloud-sdk-python-cdb-3.0.903/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/cdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)   150608 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/cdb/v20170320/cdb_client.py
+-rw-r--r--   0 root         (0) root         (0)    18943 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   526688 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/cdb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud_sdk_python_cdb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud_sdk_python_cdb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud_sdk_python_cdb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/tencentcloud_sdk_python_cdb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:28:38.000000 tencentcloud-sdk-python-cdb-3.0.904/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.903/README.rst` & `tencentcloud-sdk-python-cdb-3.0.904/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/cdb/v20170320/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -4975,24 +4975,32 @@
         r"""
         :param InstanceId: 实例 ID，格式如：cdb-c1nl9rpv。与云数据库控制台页面中显示的实例 ID 相同。
         :type InstanceId: str
         :param Offset: 偏移量，最小值为0。
         :type Offset: int
         :param Limit: 分页大小，默认值为20，最小值为1，最大值为100。
         :type Limit: int
+        :param MinStartTime: binlog开始时间，筛选大于等于此值，时间格式：2016-03-17 02:10:37
+        :type MinStartTime: str
+        :param MaxStartTime: binlog开始时间，筛选小于等于此值，时间格式：2016-03-17 02:10:37
+        :type MaxStartTime: str
         """
         self.InstanceId = None
         self.Offset = None
         self.Limit = None
+        self.MinStartTime = None
+        self.MaxStartTime = None
 
 
     def _deserialize(self, params):
         self.InstanceId = params.get("InstanceId")
         self.Offset = params.get("Offset")
         self.Limit = params.get("Limit")
+        self.MinStartTime = params.get("MinStartTime")
+        self.MaxStartTime = params.get("MaxStartTime")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.903/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cdb-3.0.904/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cdb-3.0.903/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.904/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.903/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cdb-3.0.904/tencentcloud_sdk_python_cdb.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cdb
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Cdb SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cdb-3.0.903/setup.py` & `tencentcloud-sdk-python-cdb-3.0.904/setup.py`

 * *Files identical despite different names*

