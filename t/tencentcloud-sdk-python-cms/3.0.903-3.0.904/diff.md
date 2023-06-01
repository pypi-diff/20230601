# Comparing `tmp/tencentcloud-sdk-python-cms-3.0.903.tar.gz` & `tmp/tencentcloud-sdk-python-cms-3.0.904.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-cms-3.0.903.tar", last modified: Wed May 31 02:08:01 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-cms-3.0.904.tar", last modified: Thu Jun  1 02:31:01 2023, max compression
```

## Comparing `tencentcloud-sdk-python-cms-3.0.903.tar` & `tencentcloud-sdk-python-cms-3.0.904.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud/cms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud/cms/v20190321/
--rw-r--r--   0 root         (0) root         (0)     3664 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud/cms/v20190321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud/cms/v20190321/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63975 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud/cms/v20190321/models.py
--rw-r--r--   0 root         (0) root         (0)     9932 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud/cms/v20190321/cms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud/cms/__init__.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud_sdk_python_cms.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud_sdk_python_cms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      445 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud_sdk_python_cms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud_sdk_python_cms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/tencentcloud_sdk_python_cms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2023-05-31 02:08:01.000000 tencentcloud-sdk-python-cms-3.0.903/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/
+-rw-r--r--   0 root         (0) root         (0)      737 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud/cms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud/cms/v20190321/
+-rw-r--r--   0 root         (0) root         (0)     4152 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud/cms/v20190321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud/cms/v20190321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62863 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud/cms/v20190321/models.py
+-rw-r--r--   0 root         (0) root         (0)     6573 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud/cms/v20190321/cms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud/cms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud_sdk_python_cms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud_sdk_python_cms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      445 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud_sdk_python_cms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud_sdk_python_cms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       13 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/tencentcloud_sdk_python_cms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2023-06-01 02:31:01.000000 tencentcloud-sdk-python-cms-3.0.904/setup.cfg
```

### Comparing `tencentcloud-sdk-python-cms-3.0.903/README.rst` & `tencentcloud-sdk-python-cms-3.0.904/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-cms-3.0.903/tencentcloud/cms/v20190321/models.py` & `tencentcloud-sdk-python-cms-3.0.904/tencentcloud/cms/v20190321/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,37 +21,66 @@
 class CodeDetail(AbstractModel):
     """从图片中检测到的二维码，可能为多个
 
     """
 
     def __init__(self):
         r"""
-        :param CodePosition: 二维码在图片中的位置，由边界点的坐标表示
-        :type CodePosition: list of CodePosition
-        :param CodeCharset: 二维码文本的编码格式
+        :param StrCharset: 二维码文本的编码格式
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StrCharset: str
+        :param QrCodePosition: 二维码在图片中的位置，由边界点的坐标表示
+注意：此字段可能返回 null，表示取不到有效值。
+        :type QrCodePosition: list of CodePosition
+        :param StrQrCodeText: 二维码的文本内容
+注意：此字段可能返回 null，表示取不到有效值。
+        :type StrQrCodeText: str
+        :param Uint32QrCodeType: 二维码的类型：1:ONED_BARCODE，2:QRCOD，3:WXCODE，4:PDF417，5:DATAMATRIX
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Uint32QrCodeType: int
+        :param CodeCharset: 二维码文本的编码格式（已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
         :type CodeCharset: str
-        :param CodeText: 二维码的文本内容
+        :param CodePosition: 二维码在图片中的位置，由边界点的坐标表示（已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CodePosition: list of CodePosition
+        :param CodeText: 二维码的文本内容（已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
         :type CodeText: str
-        :param CodeType: 二维码的类型：1:ONED_BARCODE，2:QRCOD，3:WXCODE，4:PDF417，5:DATAMATRIX
+        :param CodeType: 二维码的类型：1:ONED_BARCODE，2:QRCOD，3:WXCODE，4:PDF417，5:DATAMATRIX（已废弃）
+注意：此字段可能返回 null，表示取不到有效值。
         :type CodeType: int
         """
-        self.CodePosition = None
+        self.StrCharset = None
+        self.QrCodePosition = None
+        self.StrQrCodeText = None
+        self.Uint32QrCodeType = None
         self.CodeCharset = None
+        self.CodePosition = None
         self.CodeText = None
         self.CodeType = None
 
 
     def _deserialize(self, params):
+        self.StrCharset = params.get("StrCharset")
+        if params.get("QrCodePosition") is not None:
+            self.QrCodePosition = []
+            for item in params.get("QrCodePosition"):
+                obj = CodePosition()
+                obj._deserialize(item)
+                self.QrCodePosition.append(obj)
+        self.StrQrCodeText = params.get("StrQrCodeText")
+        self.Uint32QrCodeType = params.get("Uint32QrCodeType")
+        self.CodeCharset = params.get("CodeCharset")
         if params.get("CodePosition") is not None:
             self.CodePosition = []
             for item in params.get("CodePosition"):
                 obj = CodePosition()
                 obj._deserialize(item)
                 self.CodePosition.append(obj)
-        self.CodeCharset = params.get("CodeCharset")
         self.CodeText = params.get("CodeText")
         self.CodeType = params.get("CodeType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
@@ -62,31 +91,33 @@
 class CodeDetect(AbstractModel):
     """图片二维码详情
 
     """
 
     def __init__(self):
         r"""
-        :param ModerationDetail: 从图片中检测到的二维码，可能为多个
-        :type ModerationDetail: list of CodeDetail
         :param ModerationCode: 检测是否成功，0：成功，-1：出错
+注意：此字段可能返回 null，表示取不到有效值。
         :type ModerationCode: int
+        :param ModerationDetail: 从图片中检测到的二维码，可能为多个
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ModerationDetail: list of CodeDetail
         """
-        self.ModerationDetail = None
         self.ModerationCode = None
+        self.ModerationDetail = None
 
 
     def _deserialize(self, params):
+        self.ModerationCode = params.get("ModerationCode")
         if params.get("ModerationDetail") is not None:
             self.ModerationDetail = []
             for item in params.get("ModerationDetail"):
                 obj = CodeDetail()
                 obj._deserialize(item)
                 self.ModerationDetail.append(obj)
-        self.ModerationCode = params.get("ModerationCode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -96,16 +127,18 @@
     """二维码在图片中的位置，由边界点的坐标表示
 
     """
 
     def __init__(self):
         r"""
         :param FloatX: 二维码边界点X轴坐标
+注意：此字段可能返回 null，表示取不到有效值。
         :type FloatX: float
         :param FloatY: 二维码边界点Y轴坐标
+注意：此字段可能返回 null，表示取不到有效值。
         :type FloatY: float
         """
         self.FloatX = None
         self.FloatY = None
 
 
     def _deserialize(self, params):
@@ -123,502 +156,423 @@
 class Coordinate(AbstractModel):
     """坐标
 
     """
 
     def __init__(self):
         r"""
-        :param Cx: 左上角横坐标
-        :type Cx: int
+        :param Width: 宽度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Width: int
         :param Cy: 左上角纵坐标
+注意：此字段可能返回 null，表示取不到有效值。
         :type Cy: int
+        :param Cx: 左上角横坐标
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Cx: int
         :param Height: 高度
+注意：此字段可能返回 null，表示取不到有效值。
         :type Height: int
-        :param Width: 宽度
-        :type Width: int
         """
-        self.Cx = None
+        self.Width = None
         self.Cy = None
+        self.Cx = None
         self.Height = None
-        self.Width = None
 
 
     def _deserialize(self, params):
-        self.Cx = params.get("Cx")
+        self.Width = params.get("Width")
         self.Cy = params.get("Cy")
+        self.Cx = params.get("Cx")
         self.Height = params.get("Height")
-        self.Width = params.get("Width")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class CreateFileSampleRequest(AbstractModel):
-    """CreateFileSample请求参数结构体
+class CreateKeywordsSamplesRequest(AbstractModel):
+    """CreateKeywordsSamples请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Contents: 文件类型结构数组
-        :type Contents: list of FileSample
-        :param EvilType: 恶意类型
-100：正常
-20001：政治
-20002：色情 
-20006：涉毒违法
-20007：谩骂 
-24001：暴恐
-20105：广告引流
-        :type EvilType: int
-        :param FileType: image：图片
-        :type FileType: str
-        :param Label: 样本类型
-1：黑库
-2：白库
-        :type Label: int
+        :param UserKeywords: 关键词库信息：单次限制写入2000个，词库总容量不可超过10000个。
+        :type UserKeywords: list of UserKeyword
+        :param LibID: 词库ID
+        :type LibID: str
         """
-        self.Contents = None
-        self.EvilType = None
-        self.FileType = None
-        self.Label = None
+        self.UserKeywords = None
+        self.LibID = None
 
 
     def _deserialize(self, params):
-        if params.get("Contents") is not None:
-            self.Contents = []
-            for item in params.get("Contents"):
-                obj = FileSample()
+        if params.get("UserKeywords") is not None:
+            self.UserKeywords = []
+            for item in params.get("UserKeywords"):
+                obj = UserKeyword()
                 obj._deserialize(item)
-                self.Contents.append(obj)
-        self.EvilType = params.get("EvilType")
-        self.FileType = params.get("FileType")
-        self.Label = params.get("Label")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class CreateFileSampleResponse(AbstractModel):
-    """CreateFileSample返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Progress: 任务状态
-1：已完成
-2：处理中
-        :type Progress: int
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.Progress = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.Progress = params.get("Progress")
-        self.RequestId = params.get("RequestId")
-
-
-class CreateTextSampleRequest(AbstractModel):
-    """CreateTextSample请求参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Contents: 关键词数组
-        :type Contents: list of str
-        :param EvilType: 恶意类型
-100：正常
-20001：政治
-20002：色情 
-20006：涉毒违法
-20007：谩骂 
-24001：暴恐
-20105：广告引流
-        :type EvilType: int
-        :param Label: 样本类型
-1：黑库
-2：白库
-        :type Label: int
-        :param Test: 测试修改参数
-        :type Test: str
-        """
-        self.Contents = None
-        self.EvilType = None
-        self.Label = None
-        self.Test = None
-
-
-    def _deserialize(self, params):
-        self.Contents = params.get("Contents")
-        self.EvilType = params.get("EvilType")
-        self.Label = params.get("Label")
-        self.Test = params.get("Test")
+                self.UserKeywords.append(obj)
+        self.LibID = params.get("LibID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class CreateTextSampleResponse(AbstractModel):
-    """CreateTextSample返回参数结构体
+class CreateKeywordsSamplesResponse(AbstractModel):
+    """CreateKeywordsSamples返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param ErrMsg: 操作样本失败时返回的错误信息示例：  "样本1":错误码，"样本2":错误码
-        :type ErrMsg: str
-        :param Progress: 任务状态
-1：已完成
-2：处理中
-        :type Progress: int
+        :param SampleIDs: 添加成功的关键词ID列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SampleIDs: list of str
+        :param DupInfos: 重复关键词列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type DupInfos: list of UserKeywordInfo
+        :param InvalidSamples: 无效关键词列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InvalidSamples: list of InvalidSample
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.ErrMsg = None
-        self.Progress = None
+        self.SampleIDs = None
+        self.DupInfos = None
+        self.InvalidSamples = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
-        self.ErrMsg = params.get("ErrMsg")
-        self.Progress = params.get("Progress")
+        self.SampleIDs = params.get("SampleIDs")
+        if params.get("DupInfos") is not None:
+            self.DupInfos = []
+            for item in params.get("DupInfos"):
+                obj = UserKeywordInfo()
+                obj._deserialize(item)
+                self.DupInfos.append(obj)
+        if params.get("InvalidSamples") is not None:
+            self.InvalidSamples = []
+            for item in params.get("InvalidSamples"):
+                obj = InvalidSample()
+                obj._deserialize(item)
+                self.InvalidSamples.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class CustomResult(AbstractModel):
     """文本返回的自定义词库结果
 
     """
 
     def __init__(self):
         r"""
         :param Keywords: 命中的自定义关键词
         :type Keywords: list of str
-        :param LibId: 自定义库id
-        :type LibId: str
         :param LibName: 自定义词库名称
         :type LibName: str
+        :param LibId: 自定义库id
+        :type LibId: str
         :param Type: 命中的自定义关键词的类型
         :type Type: str
         """
         self.Keywords = None
-        self.LibId = None
         self.LibName = None
+        self.LibId = None
         self.Type = None
 
 
     def _deserialize(self, params):
         self.Keywords = params.get("Keywords")
-        self.LibId = params.get("LibId")
         self.LibName = params.get("LibName")
+        self.LibId = params.get("LibId")
         self.Type = params.get("Type")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DeleteFileSampleRequest(AbstractModel):
-    """DeleteFileSample请求参数结构体
+class DeleteLibSamplesRequest(AbstractModel):
+    """DeleteLibSamples请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Ids: 唯一标识数组
-        :type Ids: list of str
+        :param SampleIDs: 关键词ID
+        :type SampleIDs: list of str
+        :param LibID: 词库ID
+        :type LibID: str
         """
-        self.Ids = None
+        self.SampleIDs = None
+        self.LibID = None
 
 
     def _deserialize(self, params):
-        self.Ids = params.get("Ids")
+        self.SampleIDs = params.get("SampleIDs")
+        self.LibID = params.get("LibID")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DeleteFileSampleResponse(AbstractModel):
-    """DeleteFileSample返回参数结构体
+class DeleteLibSamplesResponse(AbstractModel):
+    """DeleteLibSamples返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Progress: 任务状态
-1：已完成
-2：处理中
-        :type Progress: int
+        :param Count: 删除成功的数量
+        :type Count: int
+        :param Details: 每个关键词删除的结果
+        :type Details: list of DeleteSampleDetails
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.Progress = None
+        self.Count = None
+        self.Details = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
-        self.Progress = params.get("Progress")
+        self.Count = params.get("Count")
+        if params.get("Details") is not None:
+            self.Details = []
+            for item in params.get("Details"):
+                obj = DeleteSampleDetails()
+                obj._deserialize(item)
+                self.Details.append(obj)
         self.RequestId = params.get("RequestId")
 
 
-class DeleteTextSampleRequest(AbstractModel):
-    """DeleteTextSample请求参数结构体
+class DeleteSampleDetails(AbstractModel):
+    """词库关键词删除结果详情
 
     """
 
     def __init__(self):
         r"""
-        :param Ids: 唯一标识数组，目前暂时只支持单个删除
-        :type Ids: list of str
+        :param SampleID: 关键词ID
+        :type SampleID: str
+        :param Content: 关键词内容
+        :type Content: str
+        :param Deleted: 是否删除成功
+        :type Deleted: bool
+        :param ErrorInfo: 错误信息
+        :type ErrorInfo: str
         """
-        self.Ids = None
+        self.SampleID = None
+        self.Content = None
+        self.Deleted = None
+        self.ErrorInfo = None
 
 
     def _deserialize(self, params):
-        self.Ids = params.get("Ids")
+        self.SampleID = params.get("SampleID")
+        self.Content = params.get("Content")
+        self.Deleted = params.get("Deleted")
+        self.ErrorInfo = params.get("ErrorInfo")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DeleteTextSampleResponse(AbstractModel):
-    """DeleteTextSample返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Progress: 任务状态
-1：已完成
-2：处理中
-        :type Progress: int
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.Progress = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        self.Progress = params.get("Progress")
-        self.RequestId = params.get("RequestId")
-
-
-class DescribeFileSampleRequest(AbstractModel):
-    """DescribeFileSample请求参数结构体
+class DescribeKeywordsLibsRequest(AbstractModel):
+    """DescribeKeywordsLibs请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Filters: 支持通过标签值进行筛选
-        :type Filters: list of Filter
-        :param Limit: 数量限制，默认为20，最大值为100
+        :param Limit: 单页条数，最大为100条
         :type Limit: int
-        :param Offset: 偏移量，默认为0
+        :param Offset: 条数偏移量
         :type Offset: int
-        :param OrderDirection: 升序（asc）还是降序（desc），默认：desc
-        :type OrderDirection: str
-        :param OrderField: 按某个字段排序，目前仅支持CreatedAt排序
-        :type OrderField: str
+        :param Filters: 过滤器(支持LibName模糊查询,CustomLibIDs词库id列表过滤)
+        :type Filters: list of Filters
         """
-        self.Filters = None
         self.Limit = None
         self.Offset = None
-        self.OrderDirection = None
-        self.OrderField = None
+        self.Filters = None
 
 
     def _deserialize(self, params):
+        self.Limit = params.get("Limit")
+        self.Offset = params.get("Offset")
         if params.get("Filters") is not None:
             self.Filters = []
             for item in params.get("Filters"):
-                obj = Filter()
+                obj = Filters()
                 obj._deserialize(item)
                 self.Filters.append(obj)
-        self.Limit = params.get("Limit")
-        self.Offset = params.get("Offset")
-        self.OrderDirection = params.get("OrderDirection")
-        self.OrderField = params.get("OrderField")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DescribeFileSampleResponse(AbstractModel):
-    """DescribeFileSample返回参数结构体
+class DescribeKeywordsLibsResponse(AbstractModel):
+    """DescribeKeywordsLibs返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param FileSampleSet: 符合要求的样本的信息
-        :type FileSampleSet: list of FileSampleInfo
-        :param TotalCount: 符合要求的样本的数量
+        :param TotalCount: 词库记录数
         :type TotalCount: int
+        :param Infos: 词库详情
+        :type Infos: list of KeywordsLibInfo
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.FileSampleSet = None
         self.TotalCount = None
+        self.Infos = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
-        if params.get("FileSampleSet") is not None:
-            self.FileSampleSet = []
-            for item in params.get("FileSampleSet"):
-                obj = FileSampleInfo()
-                obj._deserialize(item)
-                self.FileSampleSet.append(obj)
         self.TotalCount = params.get("TotalCount")
+        if params.get("Infos") is not None:
+            self.Infos = []
+            for item in params.get("Infos"):
+                obj = KeywordsLibInfo()
+                obj._deserialize(item)
+                self.Infos.append(obj)
         self.RequestId = params.get("RequestId")
 
 
-class DescribeTextSampleRequest(AbstractModel):
-    """DescribeTextSample请求参数结构体
+class DescribeLibSamplesRequest(AbstractModel):
+    """DescribeLibSamples请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Filters: 支持通过标签值进行筛选
-        :type Filters: list of Filter
-        :param Limit: 数量限制，默认为20，最大值为100
+        :param Limit: 单页条数，最大为100条
         :type Limit: int
-        :param Offset: 偏移量，默认为0
+        :param Offset: 条数偏移量
         :type Offset: int
-        :param OrderDirection: 升序（asc）还是降序（desc），默认：desc
-        :type OrderDirection: str
-        :param OrderField: 按某个字段排序，目前仅支持CreatedAt排序
-        :type OrderField: str
+        :param LibID: 词库ID
+        :type LibID: str
+        :param Content: 词内容过滤
+        :type Content: str
+        :param EvilTypeList: 违规类型列表过滤
+        :type EvilTypeList: list of int
         """
-        self.Filters = None
         self.Limit = None
         self.Offset = None
-        self.OrderDirection = None
-        self.OrderField = None
+        self.LibID = None
+        self.Content = None
+        self.EvilTypeList = None
 
 
     def _deserialize(self, params):
-        if params.get("Filters") is not None:
-            self.Filters = []
-            for item in params.get("Filters"):
-                obj = Filter()
-                obj._deserialize(item)
-                self.Filters.append(obj)
         self.Limit = params.get("Limit")
         self.Offset = params.get("Offset")
-        self.OrderDirection = params.get("OrderDirection")
-        self.OrderField = params.get("OrderField")
+        self.LibID = params.get("LibID")
+        self.Content = params.get("Content")
+        self.EvilTypeList = params.get("EvilTypeList")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class DescribeTextSampleResponse(AbstractModel):
-    """DescribeTextSample返回参数结构体
+class DescribeLibSamplesResponse(AbstractModel):
+    """DescribeLibSamples返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param TextSampleSet: 符合要求的样本的信息
-        :type TextSampleSet: list of TextSample
-        :param TotalCount: 符合要求的样本的数量
+        :param TotalCount: 词记录数
         :type TotalCount: int
+        :param Infos: 词详情
+        :type Infos: list of UserKeywordInfo
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.TextSampleSet = None
         self.TotalCount = None
+        self.Infos = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
-        if params.get("TextSampleSet") is not None:
-            self.TextSampleSet = []
-            for item in params.get("TextSampleSet"):
-                obj = TextSample()
-                obj._deserialize(item)
-                self.TextSampleSet.append(obj)
         self.TotalCount = params.get("TotalCount")
+        if params.get("Infos") is not None:
+            self.Infos = []
+            for item in params.get("Infos"):
+                obj = UserKeywordInfo()
+                obj._deserialize(item)
+                self.Infos.append(obj)
         self.RequestId = params.get("RequestId")
 
 
 class DetailResult(AbstractModel):
     """文本返回的详细结果
 
     """
 
     def __init__(self):
         r"""
-        :param EvilLabel: 恶意标签，Normal：正常，Polity：涉政，Porn：色情，Illegal：违法，Abuse：谩骂，Terror：暴恐，Ad：广告，Custom：自定义关键词
-        :type EvilLabel: str
+        :param Keywords: 该标签下命中的关键词
+        :type Keywords: list of str
         :param EvilType: 恶意类型
 100：正常
 20001：政治
 20002：色情 
 20006：涉毒违法
 20007：谩骂
 20105：广告引流 
 24001：暴恐
         :type EvilType: int
-        :param Keywords: 该标签下命中的关键词
-        :type Keywords: list of str
         :param Score: 该标签模型命中的分值
         :type Score: int
+        :param EvilLabel: 恶意标签，Normal：正常，Polity：涉政，Porn：色情，Illegal：违法，Abuse：谩骂，Terror：暴恐，Ad：广告，Custom：自定义关键词
+        :type EvilLabel: str
         """
-        self.EvilLabel = None
-        self.EvilType = None
         self.Keywords = None
+        self.EvilType = None
         self.Score = None
+        self.EvilLabel = None
 
 
     def _deserialize(self, params):
-        self.EvilLabel = params.get("EvilLabel")
-        self.EvilType = params.get("EvilType")
         self.Keywords = params.get("Keywords")
+        self.EvilType = params.get("EvilType")
         self.Score = params.get("Score")
+        self.EvilLabel = params.get("EvilLabel")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -627,188 +581,74 @@
 class Device(AbstractModel):
     """设备信息
 
     """
 
     def __init__(self):
         r"""
-        :param DeviceId: 设备指纹ID
-        :type DeviceId: str
-        :param IDFA: IOS设备，Identifier For Advertising（广告标识符）
-        :type IDFA: str
         :param IDFV: IOS设备，IDFV - Identifier For Vendor（应用开发商标识符）
         :type IDFV: str
-        :param IMEI: 设备序列号
-        :type IMEI: str
+        :param TokenId: 设备指纹Token
+        :type TokenId: str
         :param IP: 用户IP
         :type IP: str
         :param Mac: Mac地址
         :type Mac: str
-        :param TokenId: 设备指纹Token
-        :type TokenId: str
+        :param IDFA: IOS设备，Identifier For Advertising（广告标识符）
+        :type IDFA: str
+        :param DeviceId: 设备指纹ID
+        :type DeviceId: str
+        :param IMEI: 设备序列号
+        :type IMEI: str
         """
-        self.DeviceId = None
-        self.IDFA = None
         self.IDFV = None
-        self.IMEI = None
+        self.TokenId = None
         self.IP = None
         self.Mac = None
-        self.TokenId = None
+        self.IDFA = None
+        self.DeviceId = None
+        self.IMEI = None
 
 
     def _deserialize(self, params):
-        self.DeviceId = params.get("DeviceId")
-        self.IDFA = params.get("IDFA")
         self.IDFV = params.get("IDFV")
-        self.IMEI = params.get("IMEI")
+        self.TokenId = params.get("TokenId")
         self.IP = params.get("IP")
         self.Mac = params.get("Mac")
-        self.TokenId = params.get("TokenId")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class FileSample(AbstractModel):
-    """文件类型样本
-
-    """
-
-    def __init__(self):
-        r"""
-        :param FileMd5: 文件md5
-        :type FileMd5: str
-        :param FileName: 文件名称
-        :type FileName: str
-        :param FileUrl: 文件url
-        :type FileUrl: str
-        :param CompressFileUrl: 文件压缩后云url
-        :type CompressFileUrl: str
-        """
-        self.FileMd5 = None
-        self.FileName = None
-        self.FileUrl = None
-        self.CompressFileUrl = None
-
-
-    def _deserialize(self, params):
-        self.FileMd5 = params.get("FileMd5")
-        self.FileName = params.get("FileName")
-        self.FileUrl = params.get("FileUrl")
-        self.CompressFileUrl = params.get("CompressFileUrl")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class FileSampleInfo(AbstractModel):
-    """文件样本返回信息
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Code: 处理错误码
-        :type Code: int
-        :param CreatedAt: 创建时间戳
-        :type CreatedAt: int
-        :param EvilType: 恶意类型
-100：正常
-20001：政治
-20002：色情 
-20006：涉毒违法
-20007：谩骂 
-24001：暴恐
-        :type EvilType: int
-        :param FileMd5: 文件的md5
-        :type FileMd5: str
-        :param FileName: 文件名称
-        :type FileName: str
-        :param FileType: 文件类型
-        :type FileType: str
-        :param Id: 唯一标识
-        :type Id: str
-        :param Label: 样本类型
-1：黑库
-2：白库
-        :type Label: int
-        :param Status: 任务状态
-1：添加完成
-2：添加处理中
-3：下载中
-4：下载完成
-5：上传完成
-6：步骤完成
-        :type Status: int
-        :param CompressFileUrl: 文件压缩后云url
-        :type CompressFileUrl: str
-        :param FileUrl: 文件的url
-        :type FileUrl: str
-        """
-        self.Code = None
-        self.CreatedAt = None
-        self.EvilType = None
-        self.FileMd5 = None
-        self.FileName = None
-        self.FileType = None
-        self.Id = None
-        self.Label = None
-        self.Status = None
-        self.CompressFileUrl = None
-        self.FileUrl = None
-
-
-    def _deserialize(self, params):
-        self.Code = params.get("Code")
-        self.CreatedAt = params.get("CreatedAt")
-        self.EvilType = params.get("EvilType")
-        self.FileMd5 = params.get("FileMd5")
-        self.FileName = params.get("FileName")
-        self.FileType = params.get("FileType")
-        self.Id = params.get("Id")
-        self.Label = params.get("Label")
-        self.Status = params.get("Status")
-        self.CompressFileUrl = params.get("CompressFileUrl")
-        self.FileUrl = params.get("FileUrl")
+        self.IDFA = params.get("IDFA")
+        self.DeviceId = params.get("DeviceId")
+        self.IMEI = params.get("IMEI")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class Filter(AbstractModel):
-    """筛选数据结构
+class Filters(AbstractModel):
+    """入参过滤条件
 
     """
 
     def __init__(self):
         r"""
-        :param Name: 需要过滤的字段
+        :param Name: 查询字段
         :type Name: str
-        :param Value: 需要过滤字段的值
-        :type Value: str
+        :param Values: 查询值
+        :type Values: list of str
         """
         self.Name = None
-        self.Value = None
+        self.Values = None
 
 
     def _deserialize(self, params):
         self.Name = params.get("Name")
-        self.Value = params.get("Value")
+        self.Values = params.get("Values")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -817,93 +657,103 @@
 class ImageData(AbstractModel):
     """图片识别结果详情
 
     """
 
     def __init__(self):
         r"""
-        :param EvilFlag: 是否恶意 0：正常 1：可疑
-        :type EvilFlag: int
         :param EvilType: 恶意类型
 100：正常 
 20001：政治
 20002：色情 
 20006：涉毒违法
 20007：谩骂 
 20103：性感
 24001：暴恐
         :type EvilType: int
-        :param CodeDetect: 图片二维码详情
-        :type CodeDetect: :class:`tencentcloud.cms.v20190321.models.CodeDetect`
         :param HotDetect: 图片性感详情
+注意：此字段可能返回 null，表示取不到有效值。
         :type HotDetect: :class:`tencentcloud.cms.v20190321.models.ImageHotDetect`
-        :param IllegalDetect: 图片违法详情
-        :type IllegalDetect: :class:`tencentcloud.cms.v20190321.models.ImageIllegalDetect`
-        :param LogoDetect: logo详情
-        :type LogoDetect: :class:`tencentcloud.cms.v20190321.models.LogoDetail`
-        :param OCRDetect: 图片OCR详情
-        :type OCRDetect: :class:`tencentcloud.cms.v20190321.models.OCRDetect`
-        :param PhoneDetect: 手机检测详情
-        :type PhoneDetect: :class:`tencentcloud.cms.v20190321.models.PhoneDetect`
+        :param EvilFlag: 是否恶意 0：正常 1：可疑
+        :type EvilFlag: int
+        :param CodeDetect: 图片二维码详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CodeDetect: :class:`tencentcloud.cms.v20190321.models.CodeDetect`
         :param PolityDetect: 图片涉政详情
+注意：此字段可能返回 null，表示取不到有效值。
         :type PolityDetect: :class:`tencentcloud.cms.v20190321.models.ImagePolityDetect`
+        :param IllegalDetect: 图片违法详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IllegalDetect: :class:`tencentcloud.cms.v20190321.models.ImageIllegalDetect`
         :param PornDetect: 图片涉黄详情
+注意：此字段可能返回 null，表示取不到有效值。
         :type PornDetect: :class:`tencentcloud.cms.v20190321.models.ImagePornDetect`
-        :param Similar: 图片相似度详情
-        :type Similar: :class:`tencentcloud.cms.v20190321.models.Similar`
         :param TerrorDetect: 图片暴恐详情
+注意：此字段可能返回 null，表示取不到有效值。
         :type TerrorDetect: :class:`tencentcloud.cms.v20190321.models.ImageTerrorDetect`
+        :param OCRDetect: 图片OCR详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type OCRDetect: :class:`tencentcloud.cms.v20190321.models.OCRDetect`
+        :param LogoDetect: logo详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LogoDetect: :class:`tencentcloud.cms.v20190321.models.LogoDetail`
+        :param Similar: 图片相似度详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Similar: :class:`tencentcloud.cms.v20190321.models.Similar`
+        :param PhoneDetect: 手机检测详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PhoneDetect: :class:`tencentcloud.cms.v20190321.models.PhoneDetect`
         """
-        self.EvilFlag = None
         self.EvilType = None
-        self.CodeDetect = None
         self.HotDetect = None
-        self.IllegalDetect = None
-        self.LogoDetect = None
-        self.OCRDetect = None
-        self.PhoneDetect = None
+        self.EvilFlag = None
+        self.CodeDetect = None
         self.PolityDetect = None
+        self.IllegalDetect = None
         self.PornDetect = None
-        self.Similar = None
         self.TerrorDetect = None
+        self.OCRDetect = None
+        self.LogoDetect = None
+        self.Similar = None
+        self.PhoneDetect = None
 
 
     def _deserialize(self, params):
-        self.EvilFlag = params.get("EvilFlag")
         self.EvilType = params.get("EvilType")
-        if params.get("CodeDetect") is not None:
-            self.CodeDetect = CodeDetect()
-            self.CodeDetect._deserialize(params.get("CodeDetect"))
         if params.get("HotDetect") is not None:
             self.HotDetect = ImageHotDetect()
             self.HotDetect._deserialize(params.get("HotDetect"))
-        if params.get("IllegalDetect") is not None:
-            self.IllegalDetect = ImageIllegalDetect()
-            self.IllegalDetect._deserialize(params.get("IllegalDetect"))
-        if params.get("LogoDetect") is not None:
-            self.LogoDetect = LogoDetail()
-            self.LogoDetect._deserialize(params.get("LogoDetect"))
-        if params.get("OCRDetect") is not None:
-            self.OCRDetect = OCRDetect()
-            self.OCRDetect._deserialize(params.get("OCRDetect"))
-        if params.get("PhoneDetect") is not None:
-            self.PhoneDetect = PhoneDetect()
-            self.PhoneDetect._deserialize(params.get("PhoneDetect"))
+        self.EvilFlag = params.get("EvilFlag")
+        if params.get("CodeDetect") is not None:
+            self.CodeDetect = CodeDetect()
+            self.CodeDetect._deserialize(params.get("CodeDetect"))
         if params.get("PolityDetect") is not None:
             self.PolityDetect = ImagePolityDetect()
             self.PolityDetect._deserialize(params.get("PolityDetect"))
+        if params.get("IllegalDetect") is not None:
+            self.IllegalDetect = ImageIllegalDetect()
+            self.IllegalDetect._deserialize(params.get("IllegalDetect"))
         if params.get("PornDetect") is not None:
             self.PornDetect = ImagePornDetect()
             self.PornDetect._deserialize(params.get("PornDetect"))
-        if params.get("Similar") is not None:
-            self.Similar = Similar()
-            self.Similar._deserialize(params.get("Similar"))
         if params.get("TerrorDetect") is not None:
             self.TerrorDetect = ImageTerrorDetect()
             self.TerrorDetect._deserialize(params.get("TerrorDetect"))
+        if params.get("OCRDetect") is not None:
+            self.OCRDetect = OCRDetect()
+            self.OCRDetect._deserialize(params.get("OCRDetect"))
+        if params.get("LogoDetect") is not None:
+            self.LogoDetect = LogoDetail()
+            self.LogoDetect._deserialize(params.get("LogoDetect"))
+        if params.get("Similar") is not None:
+            self.Similar = Similar()
+            self.Similar._deserialize(params.get("Similar"))
+        if params.get("PhoneDetect") is not None:
+            self.PhoneDetect = PhoneDetect()
+            self.PhoneDetect._deserialize(params.get("PhoneDetect"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -912,40 +762,40 @@
 class ImageHotDetect(AbstractModel):
     """图片性感详情
 
     """
 
     def __init__(self):
         r"""
+        :param Keywords: 关键词明细
+        :type Keywords: list of str
         :param EvilType: 恶意类型
 100：正常
 20103：性感
         :type EvilType: int
-        :param HitFlag: 处置判定 0：正常 1：可疑
-        :type HitFlag: int
-        :param Keywords: 关键词明细
-        :type Keywords: list of str
         :param Labels: 性感标签：性感特征中文描述
         :type Labels: list of str
         :param Score: 性感分：分值范围 0-100，分数越高性感倾向越明显
         :type Score: int
+        :param HitFlag: 处置判定 0：正常 1：可疑
+        :type HitFlag: int
         """
-        self.EvilType = None
-        self.HitFlag = None
         self.Keywords = None
+        self.EvilType = None
         self.Labels = None
         self.Score = None
+        self.HitFlag = None
 
 
     def _deserialize(self, params):
-        self.EvilType = params.get("EvilType")
-        self.HitFlag = params.get("HitFlag")
         self.Keywords = params.get("Keywords")
+        self.EvilType = params.get("EvilType")
         self.Labels = params.get("Labels")
         self.Score = params.get("Score")
+        self.HitFlag = params.get("HitFlag")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -996,30 +846,30 @@
 class ImageModerationRequest(AbstractModel):
     """ImageModeration请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param FileContent: 文件内容 Base64,与FileUrl必须二填一
-        :type FileContent: str
-        :param FileMD5: 文件MD5值
-        :type FileMD5: str
         :param FileUrl: 文件地址
         :type FileUrl: str
+        :param FileMD5: 文件MD5值
+        :type FileMD5: str
+        :param FileContent: 文件内容 Base64,与FileUrl必须二填一
+        :type FileContent: str
         """
-        self.FileContent = None
-        self.FileMD5 = None
         self.FileUrl = None
+        self.FileMD5 = None
+        self.FileContent = None
 
 
     def _deserialize(self, params):
-        self.FileContent = params.get("FileContent")
-        self.FileMD5 = params.get("FileMD5")
         self.FileUrl = params.get("FileUrl")
+        self.FileMD5 = params.get("FileMD5")
+        self.FileContent = params.get("FileContent")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1028,31 +878,31 @@
 class ImageModerationResponse(AbstractModel):
     """ImageModeration返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Data: 识别结果
-        :type Data: :class:`tencentcloud.cms.v20190321.models.ImageData`
         :param BusinessCode: 业务返回码
         :type BusinessCode: int
+        :param Data: 识别结果
+        :type Data: :class:`tencentcloud.cms.v20190321.models.ImageData`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.Data = None
         self.BusinessCode = None
+        self.Data = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
+        self.BusinessCode = params.get("BusinessCode")
         if params.get("Data") is not None:
             self.Data = ImageData()
             self.Data._deserialize(params.get("Data"))
-        self.BusinessCode = params.get("BusinessCode")
         self.RequestId = params.get("RequestId")
 
 
 class ImagePolityDetect(AbstractModel):
     """图片涉政详情
 
     """
@@ -1061,47 +911,49 @@
         r"""
         :param EvilType: 恶意类型
 100：正常 
 20001：政治
         :type EvilType: int
         :param HitFlag: 处置判定  0：正常 1：可疑
         :type HitFlag: int
-        :param PolityLogoDetail: 命中的logo标签信息
-        :type PolityLogoDetail: list of Logo
         :param FaceNames: 命中的人脸名称
         :type FaceNames: list of str
-        :param Keywords: 关键词明细
-        :type Keywords: list of str
+        :param PolityLogoDetail: 命中的logo标签信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type PolityLogoDetail: list of Logo
         :param PolityItems: 命中的政治物品名称
+注意：此字段可能返回 null，表示取不到有效值。
         :type PolityItems: list of str
         :param Score: 政治（人脸）分：分值范围 0-100，分数越高可疑程度越高
         :type Score: int
+        :param Keywords: 关键词明细
+        :type Keywords: list of str
         """
         self.EvilType = None
         self.HitFlag = None
-        self.PolityLogoDetail = None
         self.FaceNames = None
-        self.Keywords = None
+        self.PolityLogoDetail = None
         self.PolityItems = None
         self.Score = None
+        self.Keywords = None
 
 
     def _deserialize(self, params):
         self.EvilType = params.get("EvilType")
         self.HitFlag = params.get("HitFlag")
+        self.FaceNames = params.get("FaceNames")
         if params.get("PolityLogoDetail") is not None:
             self.PolityLogoDetail = []
             for item in params.get("PolityLogoDetail"):
                 obj = Logo()
                 obj._deserialize(item)
                 self.PolityLogoDetail.append(obj)
-        self.FaceNames = params.get("FaceNames")
-        self.Keywords = params.get("Keywords")
         self.PolityItems = params.get("PolityItems")
         self.Score = params.get("Score")
+        self.Keywords = params.get("Keywords")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1152,273 +1004,219 @@
 class ImageTerrorDetect(AbstractModel):
     """图片暴恐详情
 
     """
 
     def __init__(self):
         r"""
+        :param Keywords: 关键词明细
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Keywords: list of str
         :param EvilType: 恶意类型
 100：正常
 24001：暴恐
+注意：此字段可能返回 null，表示取不到有效值。
         :type EvilType: int
-        :param HitFlag: 处置判定 0：正常 1：可疑
-        :type HitFlag: int
-        :param Keywords: 关键词明细
-        :type Keywords: list of str
         :param Labels: 暴恐标签：返回暴恐特征中文描述
+注意：此字段可能返回 null，表示取不到有效值。
         :type Labels: list of str
         :param Score: 暴恐分：分值范围0--100，分数越高暴恐倾向越明显
+注意：此字段可能返回 null，表示取不到有效值。
         :type Score: int
+        :param HitFlag: 处置判定 0：正常 1：可疑
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HitFlag: int
         """
-        self.EvilType = None
-        self.HitFlag = None
         self.Keywords = None
+        self.EvilType = None
         self.Labels = None
         self.Score = None
+        self.HitFlag = None
 
 
     def _deserialize(self, params):
-        self.EvilType = params.get("EvilType")
-        self.HitFlag = params.get("HitFlag")
         self.Keywords = params.get("Keywords")
+        self.EvilType = params.get("EvilType")
         self.Labels = params.get("Labels")
         self.Score = params.get("Score")
+        self.HitFlag = params.get("HitFlag")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class Logo(AbstractModel):
-    """Logo
-
-    """
-
-    def __init__(self):
-        r"""
-        :param RrectF: logo图标坐标信息
-        :type RrectF: :class:`tencentcloud.cms.v20190321.models.RrectF`
-        :param Confidence: logo图标置信度
-        :type Confidence: float
-        :param Name: logo图标名称
-        :type Name: str
-        """
-        self.RrectF = None
-        self.Confidence = None
-        self.Name = None
-
-
-    def _deserialize(self, params):
-        if params.get("RrectF") is not None:
-            self.RrectF = RrectF()
-            self.RrectF._deserialize(params.get("RrectF"))
-        self.Confidence = params.get("Confidence")
-        self.Name = params.get("Name")
-        memeber_set = set(params.keys())
-        for name, value in vars(self).items():
-            if name in memeber_set:
-                memeber_set.remove(name)
-        if len(memeber_set) > 0:
-            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
-        
-
-
-class LogoDetail(AbstractModel):
-    """LogoDetail
+class InvalidSample(AbstractModel):
+    """无效关键词
 
     """
 
     def __init__(self):
         r"""
-        :param AppLogoDetail: 命中的Applogo详情
-        :type AppLogoDetail: list of Logo
+        :param Content: 关键词
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Content: str
+        :param InvalidCode: 无效代码:1-标签不存在;2-词过长;3-词类型不匹配;4-备注超长
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InvalidCode: int
+        :param InvalidMessage: 无效描述
+注意：此字段可能返回 null，表示取不到有效值。
+        :type InvalidMessage: str
         """
-        self.AppLogoDetail = None
+        self.Content = None
+        self.InvalidCode = None
+        self.InvalidMessage = None
 
 
     def _deserialize(self, params):
-        if params.get("AppLogoDetail") is not None:
-            self.AppLogoDetail = []
-            for item in params.get("AppLogoDetail"):
-                obj = Logo()
-                obj._deserialize(item)
-                self.AppLogoDetail.append(obj)
+        self.Content = params.get("Content")
+        self.InvalidCode = params.get("InvalidCode")
+        self.InvalidMessage = params.get("InvalidMessage")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ManualReviewContent(AbstractModel):
-    """人审审核数据相关信息
+class KeywordsLibInfo(AbstractModel):
+    """关键词库信息
 
     """
 
     def __init__(self):
         r"""
-        :param BatchId: 审核批次号
-        :type BatchId: str
-        :param Content: 审核内容
-        :type Content: str
-        :param ContentId: 消息Id
-        :type ContentId: str
-        :param ContentType: 审核内容类型 1 图片 2 视频 3 文本 4 音频
-        :type ContentType: int
-        :param UserInfo: 用户信息
-        :type UserInfo: :class:`tencentcloud.cms.v20190321.models.User`
-        :param AutoDetailCode: 机器审核类型，与腾讯机器审核定义一致
-100 正常
-20001 政治
-20002 色情
-20006 违法
-20007 谩骂
-24001 暴恐
-20105 广告
-20103 性感
-        :type AutoDetailCode: int
-        :param AutoResult: 机器审核结果 0 放过 1 拦截
-        :type AutoResult: int
-        :param CallBackInfo: 回调信息标识，回传数据时原样返回
-        :type CallBackInfo: str
-        :param CreateTime: 创建时间 格式“2020-01-01 00:00:12”
+        :param ID: 关键词库ID
+        :type ID: str
+        :param LibName: 关键词库名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type LibName: str
+        :param Describe: 关键词库描述信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Describe: str
+        :param CreateTime: 关键词库创建时间
         :type CreateTime: str
-        :param Priority: 审核优先级，可选值 [1,2,3,4]，其中 1 最高，4 最低
-        :type Priority: int
-        :param Title: 标题
-        :type Title: str
+        :param Suggestion: 审核建议(Review/Block)
+        :type Suggestion: str
+        :param MatchType: 匹配模式(ExactMatch/FuzzyMatch)
+        :type MatchType: str
+        :param BizTypes: 关联策略BizType列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type BizTypes: list of str
         """
-        self.BatchId = None
-        self.Content = None
-        self.ContentId = None
-        self.ContentType = None
-        self.UserInfo = None
-        self.AutoDetailCode = None
-        self.AutoResult = None
-        self.CallBackInfo = None
+        self.ID = None
+        self.LibName = None
+        self.Describe = None
         self.CreateTime = None
-        self.Priority = None
-        self.Title = None
+        self.Suggestion = None
+        self.MatchType = None
+        self.BizTypes = None
 
 
     def _deserialize(self, params):
-        self.BatchId = params.get("BatchId")
-        self.Content = params.get("Content")
-        self.ContentId = params.get("ContentId")
-        self.ContentType = params.get("ContentType")
-        if params.get("UserInfo") is not None:
-            self.UserInfo = User()
-            self.UserInfo._deserialize(params.get("UserInfo"))
-        self.AutoDetailCode = params.get("AutoDetailCode")
-        self.AutoResult = params.get("AutoResult")
-        self.CallBackInfo = params.get("CallBackInfo")
+        self.ID = params.get("ID")
+        self.LibName = params.get("LibName")
+        self.Describe = params.get("Describe")
         self.CreateTime = params.get("CreateTime")
-        self.Priority = params.get("Priority")
-        self.Title = params.get("Title")
+        self.Suggestion = params.get("Suggestion")
+        self.MatchType = params.get("MatchType")
+        self.BizTypes = params.get("BizTypes")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ManualReviewData(AbstractModel):
-    """人工审核接口返回结果，由ContentId和BatchId组成
+class Logo(AbstractModel):
+    """Logo审核结果
 
     """
 
     def __init__(self):
         r"""
-        :param BatchId: 人审内容批次号
-        :type BatchId: str
-        :param ContentId: 人审内容ID
-        :type ContentId: str
+        :param Confidence: logo图标置信度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Confidence: float
+        :param RrectF: logo图标坐标信息
+注意：此字段可能返回 null，表示取不到有效值。
+        :type RrectF: :class:`tencentcloud.cms.v20190321.models.RrectF`
+        :param Name: logo图标名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
         """
-        self.BatchId = None
-        self.ContentId = None
+        self.Confidence = None
+        self.RrectF = None
+        self.Name = None
 
 
     def _deserialize(self, params):
-        self.BatchId = params.get("BatchId")
-        self.ContentId = params.get("ContentId")
+        self.Confidence = params.get("Confidence")
+        if params.get("RrectF") is not None:
+            self.RrectF = RrectF()
+            self.RrectF._deserialize(params.get("RrectF"))
+        self.Name = params.get("Name")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ManualReviewRequest(AbstractModel):
-    """ManualReview请求参数结构体
+class LogoDetail(AbstractModel):
+    """Logo命中详情
 
     """
 
     def __init__(self):
         r"""
-        :param ReviewContent: 人工审核信息
-        :type ReviewContent: :class:`tencentcloud.cms.v20190321.models.ManualReviewContent`
+        :param AppLogoDetail: 命中的Applogo详情
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AppLogoDetail: list of Logo
         """
-        self.ReviewContent = None
+        self.AppLogoDetail = None
 
 
     def _deserialize(self, params):
-        if params.get("ReviewContent") is not None:
-            self.ReviewContent = ManualReviewContent()
-            self.ReviewContent._deserialize(params.get("ReviewContent"))
+        if params.get("AppLogoDetail") is not None:
+            self.AppLogoDetail = []
+            for item in params.get("AppLogoDetail"):
+                obj = Logo()
+                obj._deserialize(item)
+                self.AppLogoDetail.append(obj)
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class ManualReviewResponse(AbstractModel):
-    """ManualReview返回参数结构体
-
-    """
-
-    def __init__(self):
-        r"""
-        :param Data: 人审接口同步响应结果
-        :type Data: :class:`tencentcloud.cms.v20190321.models.ManualReviewData`
-        :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
-        :type RequestId: str
-        """
-        self.Data = None
-        self.RequestId = None
-
-
-    def _deserialize(self, params):
-        if params.get("Data") is not None:
-            self.Data = ManualReviewData()
-            self.Data._deserialize(params.get("Data"))
-        self.RequestId = params.get("RequestId")
-
-
 class OCRDetect(AbstractModel):
     """OCR识别结果详情
 
     """
 
     def __init__(self):
         r"""
         :param Item: 识别到的详细信息
+注意：此字段可能返回 null，表示取不到有效值。
         :type Item: list of OCRItem
         :param TextInfo: 识别到的文本信息
+注意：此字段可能返回 null，表示取不到有效值。
         :type TextInfo: str
         """
         self.Item = None
         self.TextInfo = None
 
 
     def _deserialize(self, params):
@@ -1442,43 +1240,49 @@
     """OCR详情
 
     """
 
     def __init__(self):
         r"""
         :param TextPosition: 检测到的文本坐标信息
+注意：此字段可能返回 null，表示取不到有效值。
         :type TextPosition: :class:`tencentcloud.cms.v20190321.models.Coordinate`
-        :param EvilLabel: 文本命中具体标签
-        :type EvilLabel: str
         :param EvilType: 文本命中恶意违规类型
+注意：此字段可能返回 null，表示取不到有效值。
         :type EvilType: int
-        :param Keywords: 文本命中违规的关键词
-        :type Keywords: list of str
-        :param Rate: 文本涉嫌违规分值
-        :type Rate: int
         :param TextContent: 检测到的文本信息
+注意：此字段可能返回 null，表示取不到有效值。
         :type TextContent: str
+        :param Rate: 文本涉嫌违规分值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Rate: int
+        :param EvilLabel: 文本命中具体标签
+注意：此字段可能返回 null，表示取不到有效值。
+        :type EvilLabel: str
+        :param Keywords: 文本命中违规的关键词
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Keywords: list of str
         """
         self.TextPosition = None
-        self.EvilLabel = None
         self.EvilType = None
-        self.Keywords = None
-        self.Rate = None
         self.TextContent = None
+        self.Rate = None
+        self.EvilLabel = None
+        self.Keywords = None
 
 
     def _deserialize(self, params):
         if params.get("TextPosition") is not None:
             self.TextPosition = Coordinate()
             self.TextPosition._deserialize(params.get("TextPosition"))
-        self.EvilLabel = params.get("EvilLabel")
         self.EvilType = params.get("EvilType")
-        self.Keywords = params.get("Keywords")
-        self.Rate = params.get("Rate")
         self.TextContent = params.get("TextContent")
+        self.Rate = params.get("Rate")
+        self.EvilLabel = params.get("EvilLabel")
+        self.Keywords = params.get("Keywords")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1490,33 +1294,37 @@
     """
 
     def __init__(self):
         r"""
         :param EvilType: 恶意类型
 100：正常
 21000：综合
+注意：此字段可能返回 null，表示取不到有效值。
         :type EvilType: int
-        :param HitFlag: 处置判定 0：正常 1：可疑
-        :type HitFlag: int
         :param Labels: 特征中文描述
+注意：此字段可能返回 null，表示取不到有效值。
         :type Labels: list of str
         :param Score: 分值范围 0-100，分数越高倾向越明显
+注意：此字段可能返回 null，表示取不到有效值。
         :type Score: int
+        :param HitFlag: 处置判定 0：正常 1：可疑
+注意：此字段可能返回 null，表示取不到有效值。
+        :type HitFlag: int
         """
         self.EvilType = None
-        self.HitFlag = None
         self.Labels = None
         self.Score = None
+        self.HitFlag = None
 
 
     def _deserialize(self, params):
         self.EvilType = params.get("EvilType")
-        self.HitFlag = params.get("HitFlag")
         self.Labels = params.get("Labels")
         self.Score = params.get("Score")
+        self.HitFlag = params.get("HitFlag")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1527,31 +1335,31 @@
 
     """
 
     def __init__(self):
         r"""
         :param Keywords: 预留字段，暂时不使用
         :type Keywords: list of str
-        :param Label: 风险类别，RiskAccount，RiskIP, RiskIMEI
-        :type Label: str
         :param Lable: 预留字段，暂时不用
         :type Lable: str
+        :param Label: 风险类别，RiskAccount，RiskIP, RiskIMEI
+        :type Label: str
         :param Level: 风险等级，1:疑似，2：恶意
         :type Level: int
         """
         self.Keywords = None
-        self.Label = None
         self.Lable = None
+        self.Label = None
         self.Level = None
 
 
     def _deserialize(self, params):
         self.Keywords = params.get("Keywords")
-        self.Label = params.get("Label")
         self.Lable = params.get("Lable")
+        self.Label = params.get("Label")
         self.Level = params.get("Level")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -1561,38 +1369,43 @@
 class RrectF(AbstractModel):
     """logo位置信息
 
     """
 
     def __init__(self):
         r"""
-        :param Cx: logo横坐标
-        :type Cx: float
+        :param Width: logo图标宽度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Width: float
         :param Cy: logo纵坐标
+注意：此字段可能返回 null，表示取不到有效值。
         :type Cy: float
-        :param Height: logo图标高度
-        :type Height: float
+        :param Cx: logo横坐标
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Cx: float
         :param Rotate: logo图标中心旋转度
+注意：此字段可能返回 null，表示取不到有效值。
         :type Rotate: float
-        :param Width: logo图标宽度
-        :type Width: float
+        :param Height: logo图标高度
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Height: float
         """
-        self.Cx = None
+        self.Width = None
         self.Cy = None
-        self.Height = None
+        self.Cx = None
         self.Rotate = None
-        self.Width = None
+        self.Height = None
 
 
     def _deserialize(self, params):
-        self.Cx = params.get("Cx")
+        self.Width = params.get("Width")
         self.Cy = params.get("Cy")
-        self.Height = params.get("Height")
+        self.Cx = params.get("Cx")
         self.Rotate = params.get("Rotate")
-        self.Width = params.get("Width")
+        self.Height = params.get("Height")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1612,14 +1425,15 @@
 20006：涉毒违法
 20007：谩骂 
 24001：暴恐
         :type EvilType: int
         :param HitFlag: 处置判定 0：未匹配到 1：恶意 2：白样本
         :type HitFlag: int
         :param SeedUrl: 返回的种子url
+注意：此字段可能返回 null，表示取不到有效值。
         :type SeedUrl: str
         """
         self.EvilType = None
         self.HitFlag = None
         self.SeedUrl = None
 
 
@@ -1639,106 +1453,106 @@
 class TextData(AbstractModel):
     """文本识别结果详情
 
     """
 
     def __init__(self):
         r"""
-        :param EvilFlag: 是否恶意 0：正常 1：可疑
-        :type EvilFlag: int
         :param EvilType: 恶意类型
 100：正常
 20001：政治
 20002：色情 
 20006：涉毒违法
 20007：谩骂
 20105：广告引流 
 24001：暴恐
         :type EvilType: int
-        :param Common: 消息类公共相关参数
-        :type Common: :class:`tencentcloud.cms.v20190321.models.TextOutputComm`
-        :param CustomResult: 返回的自定义词库结果
-        :type CustomResult: list of CustomResult
-        :param DetailResult: 返回的详细结果
-        :type DetailResult: list of DetailResult
-        :param ID: 消息类ID信息
-        :type ID: :class:`tencentcloud.cms.v20190321.models.TextOutputID`
-        :param Res: 消息类输出结果
-        :type Res: :class:`tencentcloud.cms.v20190321.models.TextOutputRes`
-        :param RiskDetails: 账号风险检测结果
-        :type RiskDetails: list of RiskDetails
-        :param BizType: 最终使用的BizType
-        :type BizType: int
+        :param EvilFlag: 是否恶意 0：正常 1：可疑
+        :type EvilFlag: int
         :param DataId: 和请求中的DataId一致，原样返回
         :type DataId: str
-        :param EvilLabel: 恶意标签，Normal：正常，Polity：涉政，Porn：色情，Illegal：违法，Abuse：谩骂，Terror：暴恐，Ad：广告，Custom：自定义关键词
-        :type EvilLabel: str
         :param Extra: 输出的其他信息，不同客户内容不同
         :type Extra: str
-        :param Keywords: 命中的关键词
-        :type Keywords: list of str
+        :param BizType: 最终使用的BizType
+        :type BizType: int
+        :param Res: 消息类输出结果
+        :type Res: :class:`tencentcloud.cms.v20190321.models.TextOutputRes`
+        :param RiskDetails: 账号风险检测结果
+        :type RiskDetails: list of RiskDetails
+        :param ID: 消息类ID信息
+        :type ID: :class:`tencentcloud.cms.v20190321.models.TextOutputID`
         :param Score: 命中的模型分值
         :type Score: int
+        :param Common: 消息类公共相关参数
+        :type Common: :class:`tencentcloud.cms.v20190321.models.TextOutputComm`
         :param Suggestion: 建议值,Block：打击,Review：待复审,Normal：正常
         :type Suggestion: str
+        :param Keywords: 命中的关键词
+        :type Keywords: list of str
+        :param DetailResult: 返回的详细结果
+        :type DetailResult: list of DetailResult
+        :param CustomResult: 返回的自定义词库结果
+        :type CustomResult: list of CustomResult
+        :param EvilLabel: 恶意标签，Normal：正常，Polity：涉政，Porn：色情，Illegal：违法，Abuse：谩骂，Terror：暴恐，Ad：广告，Custom：自定义关键词
+        :type EvilLabel: str
         """
-        self.EvilFlag = None
         self.EvilType = None
-        self.Common = None
-        self.CustomResult = None
-        self.DetailResult = None
-        self.ID = None
-        self.Res = None
-        self.RiskDetails = None
-        self.BizType = None
+        self.EvilFlag = None
         self.DataId = None
-        self.EvilLabel = None
         self.Extra = None
-        self.Keywords = None
+        self.BizType = None
+        self.Res = None
+        self.RiskDetails = None
+        self.ID = None
         self.Score = None
+        self.Common = None
         self.Suggestion = None
+        self.Keywords = None
+        self.DetailResult = None
+        self.CustomResult = None
+        self.EvilLabel = None
 
 
     def _deserialize(self, params):
-        self.EvilFlag = params.get("EvilFlag")
         self.EvilType = params.get("EvilType")
-        if params.get("Common") is not None:
-            self.Common = TextOutputComm()
-            self.Common._deserialize(params.get("Common"))
-        if params.get("CustomResult") is not None:
-            self.CustomResult = []
-            for item in params.get("CustomResult"):
-                obj = CustomResult()
-                obj._deserialize(item)
-                self.CustomResult.append(obj)
-        if params.get("DetailResult") is not None:
-            self.DetailResult = []
-            for item in params.get("DetailResult"):
-                obj = DetailResult()
-                obj._deserialize(item)
-                self.DetailResult.append(obj)
-        if params.get("ID") is not None:
-            self.ID = TextOutputID()
-            self.ID._deserialize(params.get("ID"))
+        self.EvilFlag = params.get("EvilFlag")
+        self.DataId = params.get("DataId")
+        self.Extra = params.get("Extra")
+        self.BizType = params.get("BizType")
         if params.get("Res") is not None:
             self.Res = TextOutputRes()
             self.Res._deserialize(params.get("Res"))
         if params.get("RiskDetails") is not None:
             self.RiskDetails = []
             for item in params.get("RiskDetails"):
                 obj = RiskDetails()
                 obj._deserialize(item)
                 self.RiskDetails.append(obj)
-        self.BizType = params.get("BizType")
-        self.DataId = params.get("DataId")
-        self.EvilLabel = params.get("EvilLabel")
-        self.Extra = params.get("Extra")
-        self.Keywords = params.get("Keywords")
+        if params.get("ID") is not None:
+            self.ID = TextOutputID()
+            self.ID._deserialize(params.get("ID"))
         self.Score = params.get("Score")
+        if params.get("Common") is not None:
+            self.Common = TextOutputComm()
+            self.Common._deserialize(params.get("Common"))
         self.Suggestion = params.get("Suggestion")
+        self.Keywords = params.get("Keywords")
+        if params.get("DetailResult") is not None:
+            self.DetailResult = []
+            for item in params.get("DetailResult"):
+                obj = DetailResult()
+                obj._deserialize(item)
+                self.DetailResult.append(obj)
+        if params.get("CustomResult") is not None:
+            self.CustomResult = []
+            for item in params.get("CustomResult"):
+                obj = CustomResult()
+                obj._deserialize(item)
+                self.CustomResult.append(obj)
+        self.EvilLabel = params.get("EvilLabel")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1749,44 +1563,44 @@
 
     """
 
     def __init__(self):
         r"""
         :param Content: 文本内容Base64编码。原文长度需小于15000字节，即5000个汉字以内。
         :type Content: str
-        :param Device: 设备相关信息
-        :type Device: :class:`tencentcloud.cms.v20190321.models.Device`
-        :param User: 用户相关信息
-        :type User: :class:`tencentcloud.cms.v20190321.models.User`
-        :param BizType: 该字段用于标识业务场景。您可以在内容安全控制台创建对应的ID，配置不同的内容审核策略，通过接口调用，默认不填为0，后端使用默认策略
-        :type BizType: int
         :param DataId: 数据ID，英文字母、下划线、-组成，不超过64个字符
         :type DataId: str
+        :param BizType: 该字段用于标识业务场景。您可以在内容安全控制台创建对应的ID，配置不同的内容审核策略，通过接口调用，默认不填为0，后端使用默认策略
+        :type BizType: int
+        :param User: 用户相关信息
+        :type User: :class:`tencentcloud.cms.v20190321.models.User`
         :param SdkAppId: 业务应用ID
         :type SdkAppId: int
+        :param Device: 设备相关信息
+        :type Device: :class:`tencentcloud.cms.v20190321.models.Device`
         """
         self.Content = None
-        self.Device = None
-        self.User = None
-        self.BizType = None
         self.DataId = None
+        self.BizType = None
+        self.User = None
         self.SdkAppId = None
+        self.Device = None
 
 
     def _deserialize(self, params):
         self.Content = params.get("Content")
-        if params.get("Device") is not None:
-            self.Device = Device()
-            self.Device._deserialize(params.get("Device"))
+        self.DataId = params.get("DataId")
+        self.BizType = params.get("BizType")
         if params.get("User") is not None:
             self.User = User()
             self.User._deserialize(params.get("User"))
-        self.BizType = params.get("BizType")
-        self.DataId = params.get("DataId")
         self.SdkAppId = params.get("SdkAppId")
+        if params.get("Device") is not None:
+            self.Device = Device()
+            self.Device._deserialize(params.get("Device"))
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
@@ -1795,60 +1609,61 @@
 class TextModerationResponse(AbstractModel):
     """TextModeration返回参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param Data: 识别结果
-        :type Data: :class:`tencentcloud.cms.v20190321.models.TextData`
         :param BusinessCode: 业务返回码
         :type BusinessCode: int
+        :param Data: 识别结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Data: :class:`tencentcloud.cms.v20190321.models.TextData`
         :param RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
         :type RequestId: str
         """
-        self.Data = None
         self.BusinessCode = None
+        self.Data = None
         self.RequestId = None
 
 
     def _deserialize(self, params):
+        self.BusinessCode = params.get("BusinessCode")
         if params.get("Data") is not None:
             self.Data = TextData()
             self.Data._deserialize(params.get("Data"))
-        self.BusinessCode = params.get("BusinessCode")
         self.RequestId = params.get("RequestId")
 
 
 class TextOutputComm(AbstractModel):
     """消息类输出公共参数
 
     """
 
     def __init__(self):
         r"""
-        :param AppID: 接入业务的唯一ID
-        :type AppID: int
         :param BUCtrlID: 接口唯一ID，旁路调用接口返回有该字段，标识唯一接口
         :type BUCtrlID: int
         :param SendTime: 消息发送时间
         :type SendTime: int
+        :param AppID: 接入业务的唯一ID
+        :type AppID: int
         :param Uin: 请求字段里的Common.Uin
         :type Uin: int
         """
-        self.AppID = None
         self.BUCtrlID = None
         self.SendTime = None
+        self.AppID = None
         self.Uin = None
 
 
     def _deserialize(self, params):
-        self.AppID = params.get("AppID")
         self.BUCtrlID = params.get("BUCtrlID")
         self.SendTime = params.get("SendTime")
+        self.AppID = params.get("AppID")
         self.Uin = params.get("Uin")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -1888,140 +1703,163 @@
 
     """
 
     def __init__(self):
         r"""
         :param Operator: 操作人,信安处理人企业微信ID
         :type Operator: str
+        :param ResultType: 恶意类型，广告（10001）， 政治（20001）， 色情（20002）， 社会事件（20004）， 暴力（20011）， 低俗（20012）， 违法犯罪（20006）， 欺诈（20008）， 版权（20013）， 谣言（20104）， 其他（21000）
+        :type ResultType: int
         :param ResultCode: 恶意操作码，
 删除（1）， 通过（2）， 先审后发（100012）
         :type ResultCode: int
         :param ResultMsg: 操作结果备注说明
         :type ResultMsg: str
-        :param ResultType: 恶意类型，广告（10001）， 政治（20001）， 色情（20002）， 社会事件（20004）， 暴力（20011）， 低俗（20012）， 违法犯罪（20006）， 欺诈（20008）， 版权（20013）， 谣言（20104）， 其他（21000）
-        :type ResultType: int
         """
         self.Operator = None
+        self.ResultType = None
         self.ResultCode = None
         self.ResultMsg = None
-        self.ResultType = None
 
 
     def _deserialize(self, params):
         self.Operator = params.get("Operator")
+        self.ResultType = params.get("ResultType")
         self.ResultCode = params.get("ResultCode")
         self.ResultMsg = params.get("ResultMsg")
-        self.ResultType = params.get("ResultType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class TextSample(AbstractModel):
-    """文字样本信息
+class User(AbstractModel):
+    """用户相关信息
 
     """
 
     def __init__(self):
         r"""
-        :param Code: 处理错误码
-        :type Code: int
-        :param Content: 关键词
+        :param Level: 用户等级，默认0 未知 1 低 2 中 3 高
+        :type Level: int
+        :param Gender: 性别 默认0 未知 1 男性 2 女性
+        :type Gender: int
+        :param Age: 年龄 默认0 未知
+        :type Age: int
+        :param UserId: 用户账号ID，如填写，会根据账号历史恶意情况，判定消息有害结果，特别是有利于可疑恶意情况下的辅助判断。账号可以填写微信uin、QQ号、微信openid、QQopenid、字符串等。该字段和账号类别确定唯一账号。
+        :type UserId: str
+        :param Phone: 手机号
+        :type Phone: str
+        :param AccountType: 账号类别，"1-微信uin 2-QQ号 3-微信群uin 4-qq群号 5-微信openid 6-QQopenid 7-其它string"
+        :type AccountType: int
+        :param Nickname: 用户昵称
+        :type Nickname: str
+        """
+        self.Level = None
+        self.Gender = None
+        self.Age = None
+        self.UserId = None
+        self.Phone = None
+        self.AccountType = None
+        self.Nickname = None
+
+
+    def _deserialize(self, params):
+        self.Level = params.get("Level")
+        self.Gender = params.get("Gender")
+        self.Age = params.get("Age")
+        self.UserId = params.get("UserId")
+        self.Phone = params.get("Phone")
+        self.AccountType = params.get("AccountType")
+        self.Nickname = params.get("Nickname")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            if name in memeber_set:
+                memeber_set.remove(name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class UserKeyword(AbstractModel):
+    """添加关键词。
+
+    """
+
+    def __init__(self):
+        r"""
+        :param Content: 关键词内容：最多40个字符，并且符合词类型的规则
         :type Content: str
-        :param CreatedAt: 创建时间戳
-        :type CreatedAt: int
-        :param EvilType: 恶意类型
-100：正常
-20001：政治
-20002：色情 
-20006：涉毒违法
-20007：谩骂 
-20105：广告引流 
-24001：暴恐
-        :type EvilType: int
-        :param Id: 唯一标识
-        :type Id: str
-        :param Label: 样本类型
-1：黑库
-2：白库
-        :type Label: int
-        :param Status: 任务状态
-1：已完成
-2：处理中
-        :type Status: int
+        :param Label: 关键词类型，取值范围为："Normal","Polity","Porn","Ad","Illegal","Abuse","Terror","Spam"
+        :type Label: str
+        :param Remark: 关键词备注：最多100个字符。
+        :type Remark: str
+        :param WordType: 词类型：Default,Pinyin,English,CompoundWord,ExclusionWord,AffixWord
+        :type WordType: str
         """
-        self.Code = None
         self.Content = None
-        self.CreatedAt = None
-        self.EvilType = None
-        self.Id = None
         self.Label = None
-        self.Status = None
+        self.Remark = None
+        self.WordType = None
 
 
     def _deserialize(self, params):
-        self.Code = params.get("Code")
         self.Content = params.get("Content")
-        self.CreatedAt = params.get("CreatedAt")
-        self.EvilType = params.get("EvilType")
-        self.Id = params.get("Id")
         self.Label = params.get("Label")
-        self.Status = params.get("Status")
+        self.Remark = params.get("Remark")
+        self.WordType = params.get("WordType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
-class User(AbstractModel):
-    """用户相关信息
+class UserKeywordInfo(AbstractModel):
+    """关键词信息
 
     """
 
     def __init__(self):
         r"""
-        :param AccountType: 账号类别，"1-微信uin 2-QQ号 3-微信群uin 4-qq群号 5-微信openid 6-QQopenid 7-其它string"
-        :type AccountType: int
-        :param Age: 年龄 默认0 未知
-        :type Age: int
-        :param Gender: 性别 默认0 未知 1 男性 2 女性
-        :type Gender: int
-        :param Level: 用户等级，默认0 未知 1 低 2 中 3 高
-        :type Level: int
-        :param Nickname: 用户昵称
-        :type Nickname: str
-        :param Phone: 手机号
-        :type Phone: str
-        :param UserId: 用户账号ID，如填写，会根据账号历史恶意情况，判定消息有害结果，特别是有利于可疑恶意情况下的辅助判断。账号可以填写微信uin、QQ号、微信openid、QQopenid、字符串等。该字段和账号类别确定唯一账号。
-        :type UserId: str
+        :param ID: 关键词条ID
+        :type ID: str
+        :param Content: 关键词内容
+        :type Content: str
+        :param Label: 关键词标签；取值范围为："Normal","Polity","Porn","Sexy","Ad","Illegal","Abuse","Terror","Spam","Moan"
+        :type Label: str
+        :param CreateTime: 创建时间
+        :type CreateTime: str
+        :param Remark: 备注
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Remark: str
+        :param WordType: 词类型：Default,Pinyin,English,CompoundWord,ExclusionWord,AffixWord
+注意：此字段可能返回 null，表示取不到有效值。
+        :type WordType: str
         """
-        self.AccountType = None
-        self.Age = None
-        self.Gender = None
-        self.Level = None
-        self.Nickname = None
-        self.Phone = None
-        self.UserId = None
+        self.ID = None
+        self.Content = None
+        self.Label = None
+        self.CreateTime = None
+        self.Remark = None
+        self.WordType = None
 
 
     def _deserialize(self, params):
-        self.AccountType = params.get("AccountType")
-        self.Age = params.get("Age")
-        self.Gender = params.get("Gender")
-        self.Level = params.get("Level")
-        self.Nickname = params.get("Nickname")
-        self.Phone = params.get("Phone")
-        self.UserId = params.get("UserId")
+        self.ID = params.get("ID")
+        self.Content = params.get("Content")
+        self.Label = params.get("Label")
+        self.CreateTime = params.get("CreateTime")
+        self.Remark = params.get("Remark")
+        self.WordType = params.get("WordType")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             if name in memeber_set:
                 memeber_set.remove(name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-cms-3.0.903/tencentcloud/__init__.py` & `tencentcloud-sdk-python-cms-3.0.904/tencentcloud/__init__.py`

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

### Comparing `tencentcloud-sdk-python-cms-3.0.903/tencentcloud_sdk_python_cms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-cms-3.0.904/tencentcloud_sdk_python_cms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cms
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Cms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cms-3.0.903/PKG-INFO` & `tencentcloud-sdk-python-cms-3.0.904/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-cms
-Version: 3.0.903
+Version: 3.0.904
 Summary: Tencent Cloud Cms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-cms-3.0.903/setup.py` & `tencentcloud-sdk-python-cms-3.0.904/setup.py`

 * *Files identical despite different names*

