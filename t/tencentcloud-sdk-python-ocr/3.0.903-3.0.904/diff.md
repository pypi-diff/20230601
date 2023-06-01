# Comparing `tmp/tencentcloud-sdk-python-ocr-3.0.903.tar.gz` & `tmp/tencentcloud-sdk-python-ocr-3.0.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.903.tar", last modified: Wed May 31 02:17:04 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-ocr-3.0.904.tar", last modified: Thu Jun  1 02:42:44 2023, max compression
```

## Comparing `tencentcloud-sdk-python-ocr-3.0.903.tar` & `tencentcloud-sdk-python-ocr-3.0.904.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud_sdk_python_ocr.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/ocr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)   113899 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/ocr/v20181119/ocr_client.py
--rw-r--r--   0 root         (0) root         (0)     5894 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   508075 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/ocr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:17:04.000000 tencentcloud-sdk-python-ocr-3.0.903/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud_sdk_python_ocr.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud_sdk_python_ocr.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud_sdk_python_ocr.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud_sdk_python_ocr.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/ocr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)   114877 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/ocr/v20181119/ocr_client.py
+-rw-r--r--   0 root         (0) root         (0)     5894 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   512616 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/ocr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:42:44.000000 tencentcloud-sdk-python-ocr-3.0.904/setup.cfg
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.903/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.904/tencentcloud_sdk_python_ocr.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.903/README.rst` & `tencentcloud-sdk-python-ocr-3.0.904/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1747,14 +1747,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(e.message, e.message)
 
 
+    def RecognizePhilippinesUMIDOCR(self, request):
+        """菲律宾UMID识别
+
+        :param request: Request instance for RecognizePhilippinesUMIDOCR.
+        :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesUMIDOCRRequest`
+        :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesUMIDOCRResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RecognizePhilippinesUMIDOCR", params, headers=headers)
+            response = json.loads(body)
+            model = models.RecognizePhilippinesUMIDOCRResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(e.message, e.message)
+
+
     def RecognizePhilippinesVoteIDOCR(self, request):
         """本接口支持菲律宾VoteID识别，识别字段包括姓名、姓氏、出生日期、婚姻状况、国籍、地址、地区、菲律宾VoteID的VIN等。
 
         默认接口请求频率限制：20次/秒。
 
         :param request: Request instance for RecognizePhilippinesVoteIDOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizePhilippinesVoteIDOCRRequest`
@@ -1826,14 +1849,16 @@
                 raise TencentCloudSDKException(e.message, e.message)
 
 
     def RecognizeThaiIDCardOCR(self, request):
         """本接口支持泰国身份证识别，识别字段包括泰文姓名、英文姓名、地址、出生日期、身份证号码、首次领用日期、签发日期等字段。
         本接口暂未完全对外开放，如需咨询，请[联系商务](https://cloud.tencent.com/about/connect)
 
+        默认接口请求频率限制：10次/秒
+
         :param request: Request instance for RecognizeThaiIDCardOCR.
         :type request: :class:`tencentcloud.ocr.v20181119.models.RecognizeThaiIDCardOCRRequest`
         :rtype: :class:`tencentcloud.ocr.v20181119.models.RecognizeThaiIDCardOCRResponse`
 
         """
         try:
             params = request._serialize()
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/ocr/v20181119/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7312,14 +7312,111 @@
             self.Birthday._deserialize(params.get("Birthday"))
         if params.get("IssueDate") is not None:
             self.IssueDate = TextDetectionResult()
             self.IssueDate._deserialize(params.get("IssueDate"))
         self.RequestId = params.get("RequestId")
 
 
+class RecognizePhilippinesUMIDOCRRequest(AbstractModel):
+    """RecognizePhilippinesUMIDOCR请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param ImageBase64: 图片的 Base64 值。 支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。 支持的图片大小：所下载图片经Base64编码后不超过 7M。图片下载时间不超过 3 秒。 图片的 ImageUrl、ImageBase64 必须提供一个，如果都提供，只使用 ImageUrl。
+        :type ImageBase64: str
+        :param ImageUrl: 图片的 Url 地址。 支持的图片格式：PNG、JPG、JPEG，暂不支持 GIF 格式。 支持的图片大小：所下载图片经 Base64 编码后不超过 7M。图片下载时间不超过 3 秒。 图片存储于腾讯云的 Url 可保障更高的下载速度和稳定性，建议图片存储于腾讯云。 非腾讯云存储的 Url 速度和稳定性可能受一定影响。
+        :type ImageUrl: str
+        :param ReturnHeadImage: 是否返回人像照片。
+        :type ReturnHeadImage: bool
+        """
+        self.ImageBase64 = None
+        self.ImageUrl = None
+        self.ReturnHeadImage = None
+
+
+    def _deserialize(self, params):
+        self.ImageBase64 = params.get("ImageBase64")
+        self.ImageUrl = params.get("ImageUrl")
+        self.ReturnHeadImage = params.get("ReturnHeadImage")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RecognizePhilippinesUMIDOCRResponse(AbstractModel):
+    """RecognizePhilippinesUMIDOCR返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Surname: 姓
+        :type Surname: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param MiddleName: 中间名
+        :type MiddleName: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param GivenName: 名
+        :type GivenName: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param Address: 地址
+        :type Address: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param Birthday: 生日
+        :type Birthday: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param CRN: crn码
+        :type CRN: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param Sex: 性别
+        :type Sex: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param HeadPortrait: 人像照片Base64后的结果
+        :type HeadPortrait: :class:`tencentcloud.ocr.v20181119.models.TextDetectionResult`
+        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self.Surname = None
+        self.MiddleName = None
+        self.GivenName = None
+        self.Address = None
+        self.Birthday = None
+        self.CRN = None
+        self.Sex = None
+        self.HeadPortrait = None
+        self.RequestId = None
+
+
+    def _deserialize(self, params):
+        if params.get("Surname") is not None:
+            self.Surname = TextDetectionResult()
+            self.Surname._deserialize(params.get("Surname"))
+        if params.get("MiddleName") is not None:
+            self.MiddleName = TextDetectionResult()
+            self.MiddleName._deserialize(params.get("MiddleName"))
+        if params.get("GivenName") is not None:
+            self.GivenName = TextDetectionResult()
+            self.GivenName._deserialize(params.get("GivenName"))
+        if params.get("Address") is not None:
+            self.Address = TextDetectionResult()
+            self.Address._deserialize(params.get("Address"))
+        if params.get("Birthday") is not None:
+            self.Birthday = TextDetectionResult()
+            self.Birthday._deserialize(params.get("Birthday"))
+        if params.get("CRN") is not None:
+            self.CRN = TextDetectionResult()
+            self.CRN._deserialize(params.get("CRN"))
+        if params.get("Sex") is not None:
+            self.Sex = TextDetectionResult()
+            self.Sex._deserialize(params.get("Sex"))
+        if params.get("HeadPortrait") is not None:
+            self.HeadPortrait = TextDetectionResult()
+            self.HeadPortrait._deserialize(params.get("HeadPortrait"))
+        self.RequestId = params.get("RequestId")
+
+
 class RecognizePhilippinesVoteIDOCRRequest(AbstractModel):
     """RecognizePhilippinesVoteIDOCR请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.903/tencentcloud/__init__.py` & `tencentcloud-sdk-python-ocr-3.0.904/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-ocr-3.0.903/PKG-INFO` & `tencentcloud-sdk-python-ocr-3.0.904/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-ocr
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Ocr SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-ocr-3.0.903/setup.py` & `tencentcloud-sdk-python-ocr-3.0.904/setup.py`

 * *Files identical despite different names*

