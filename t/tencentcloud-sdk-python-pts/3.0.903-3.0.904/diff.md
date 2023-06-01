# Comparing `tmp/tencentcloud-sdk-python-pts-3.0.903.tar.gz` & `tmp/tencentcloud-sdk-python-pts-3.0.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-pts-3.0.903.tar", last modified: Wed May 31 02:17:49 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-pts-3.0.904.tar", last modified: Thu Jun  1 02:43:31 2023, max compression
```

## Comparing `tencentcloud-sdk-python-pts-3.0.903.tar` & `tencentcloud-sdk-python-pts-3.0.904.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud/pts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud/pts/v20210728/
--rw-r--r--   0 root         (0) root         (0)    39209 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud/pts/v20210728/pts_client.py
--rw-r--r--   0 root         (0) root         (0)     1942 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud/pts/v20210728/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud/pts/v20210728/__init__.py
--rw-r--r--   0 root         (0) root         (0)   193898 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud/pts/v20210728/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud/pts/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud_sdk_python_pts.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud_sdk_python_pts.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud_sdk_python_pts.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud_sdk_python_pts.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/tencentcloud_sdk_python_pts.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:17:49.000000 tencentcloud-sdk-python-pts-3.0.903/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud/pts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud/pts/v20210728/
+-rw-r--r--   0 root         (0) root         (0)    39209 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud/pts/v20210728/pts_client.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud/pts/v20210728/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud/pts/v20210728/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   193898 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud/pts/v20210728/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud/pts/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud_sdk_python_pts.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud_sdk_python_pts.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud_sdk_python_pts.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud_sdk_python_pts.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/tencentcloud_sdk_python_pts.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:43:31.000000 tencentcloud-sdk-python-pts-3.0.904/setup.cfg
```

### Comparing `tencentcloud-sdk-python-pts-3.0.903/README.rst` & `tencentcloud-sdk-python-pts-3.0.904/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.903/tencentcloud/pts/v20210728/pts_client.py` & `tencentcloud-sdk-python-pts-3.0.904/tencentcloud/pts/v20210728/pts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.903/tencentcloud/pts/v20210728/errorcodes.py` & `tencentcloud-sdk-python-pts-3.0.904/tencentcloud/pts/v20210728/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.903/tencentcloud/pts/v20210728/models.py` & `tencentcloud-sdk-python-pts-3.0.904/tencentcloud/pts/v20210728/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-pts-3.0.903/tencentcloud/__init__.py` & `tencentcloud-sdk-python-pts-3.0.904/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-pts-3.0.903/PKG-INFO` & `tencentcloud-sdk-python-pts-3.0.904/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-pts
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Pts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-pts-3.0.903/tencentcloud_sdk_python_pts.egg-info/PKG-INFO` & `tencentcloud-sdk-python-pts-3.0.904/tencentcloud_sdk_python_pts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-pts
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Pts SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-pts-3.0.903/setup.py` & `tencentcloud-sdk-python-pts-3.0.904/setup.py`

 * *Files identical despite different names*

