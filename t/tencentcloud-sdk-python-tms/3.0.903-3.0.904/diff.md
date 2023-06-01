# Comparing `tmp/tencentcloud-sdk-python-tms-3.0.903.tar.gz` & `tmp/tencentcloud-sdk-python-tms-3.0.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-tms-3.0.903.tar", last modified: Wed May 31 02:24:15 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-tms-3.0.904.tar", last modified: Thu Jun  1 02:49:19 2023, max compression
```

## Comparing `tencentcloud-sdk-python-tms-3.0.903.tar` & `tencentcloud-sdk-python-tms-3.0.904.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud_sdk_python_tms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud_sdk_python_tms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud_sdk_python_tms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud_sdk_python_tms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud_sdk_python_tms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20200713/
--rw-r--r--   0 root         (0) root         (0)     3027 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20200713/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4658 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20200713/tms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20200713/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26183 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20200713/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20201229/
--rw-r--r--   0 root         (0) root         (0)     1723 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20201229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3547 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20201229/tms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20804 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:24:15.000000 tencentcloud-sdk-python-tms-3.0.903/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud_sdk_python_tms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud_sdk_python_tms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud_sdk_python_tms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud_sdk_python_tms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud_sdk_python_tms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20200713/
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20200713/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4658 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20200713/tms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20200713/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26183 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20200713/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20201229/
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20201229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3547 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20201229/tms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20804 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:49:19.000000 tencentcloud-sdk-python-tms-3.0.904/setup.cfg
```

### Comparing `tencentcloud-sdk-python-tms-3.0.903/tencentcloud_sdk_python_tms.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-tms-3.0.904/tencentcloud_sdk_python_tms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.903/tencentcloud_sdk_python_tms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-tms-3.0.904/tencentcloud_sdk_python_tms.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tms
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Tms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tms-3.0.903/README.rst` & `tencentcloud-sdk-python-tms-3.0.904/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20200713/errorcodes.py` & `tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20200713/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20200713/tms_client.py` & `tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20200713/tms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20200713/models.py` & `tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20200713/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20201229/errorcodes.py` & `tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20201229/tms_client.py` & `tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20201229/tms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.903/tencentcloud/tms/v20201229/models.py` & `tencentcloud-sdk-python-tms-3.0.904/tencentcloud/tms/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-tms-3.0.903/tencentcloud/__init__.py` & `tencentcloud-sdk-python-tms-3.0.904/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-tms-3.0.903/PKG-INFO` & `tencentcloud-sdk-python-tms-3.0.904/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-tms
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Tms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-tms-3.0.903/setup.py` & `tencentcloud-sdk-python-tms-3.0.904/setup.py`

 * *Files identical despite different names*

