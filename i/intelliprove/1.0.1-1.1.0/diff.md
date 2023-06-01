# Comparing `tmp/intelliprove-1.0.1.tar.gz` & `tmp/intelliprove-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intelliprove-1.0.1.tar", max compression
+gzip compressed data, was "intelliprove-1.1.0.tar", max compression
```

## Comparing `intelliprove-1.0.1.tar` & `intelliprove-1.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1686 2023-04-11 08:40:11.152223 intelliprove-1.0.1/README.md
--rw-r--r--   0        0        0      185 2023-04-11 08:40:11.152223 intelliprove-1.0.1/intelliprove/api/__init__.py
--rw-r--r--   0        0        0     5147 2023-04-11 08:40:11.152223 intelliprove-1.0.1/intelliprove/api/api_service.py
--rw-r--r--   0        0        0      141 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/exceptions/__init__.py
--rw-r--r--   0        0        0      891 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/exceptions/api.py
--rw-r--r--   0        0        0      790 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/exceptions/media.py
--rw-r--r--   0        0        0      261 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/exceptions/uuid.py
--rw-r--r--   0        0        0     3125 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/intelliprove_api.py
--rw-r--r--   0        0        0      214 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/__init__.py
--rw-r--r--   0        0        0      214 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/dataclasses/__init__.py
--rw-r--r--   0        0        0      642 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/dataclasses/biomarkers.py
--rw-r--r--   0        0        0      250 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/dataclasses/quality.py
--rw-r--r--   0        0        0      785 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/dataclasses/settings.py
--rw-r--r--   0        0        0      343 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/enums.py
--rw-r--r--   0        0        0      164 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/responses/__init__.py
--rw-r--r--   0        0        0     1199 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/responses/biomarkers_response.py
--rw-r--r--   0        0        0      754 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/models/responses/quality_response.py
--rw-r--r--   0        0        0       91 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/utils/__init__.py
--rw-r--r--   0        0        0      169 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/utils/identifiers.py
--rw-r--r--   0        0        0     2459 2023-04-11 08:40:11.156224 intelliprove-1.0.1/intelliprove/api/utils/media.py
--rw-r--r--   0        0        0      414 2023-04-11 08:40:11.156224 intelliprove-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 intelliprove-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1686 2023-06-01 13:49:57.540140 intelliprove-1.1.0/README.md
+-rw-r--r--   0        0        0      185 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/__init__.py
+-rw-r--r--   0        0        0     5513 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/api_service.py
+-rw-r--r--   0        0        0      141 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/exceptions/__init__.py
+-rw-r--r--   0        0        0      891 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/exceptions/api.py
+-rw-r--r--   0        0        0      790 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/exceptions/media.py
+-rw-r--r--   0        0        0      261 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/exceptions/uuid.py
+-rw-r--r--   0        0        0     3522 2023-06-01 13:49:57.540140 intelliprove-1.1.0/intelliprove/api/intelliprove_api.py
+-rw-r--r--   0        0        0      214 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/__init__.py
+-rw-r--r--   0        0        0      214 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/dataclasses/__init__.py
+-rw-r--r--   0        0        0      642 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/dataclasses/biomarkers.py
+-rw-r--r--   0        0        0      250 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/dataclasses/quality.py
+-rw-r--r--   0        0        0      785 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/dataclasses/settings.py
+-rw-r--r--   0        0        0      343 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/enums.py
+-rw-r--r--   0        0        0      164 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/responses/__init__.py
+-rw-r--r--   0        0        0     1199 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/responses/biomarkers_response.py
+-rw-r--r--   0        0        0      754 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/models/responses/quality_response.py
+-rw-r--r--   0        0        0       91 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/utils/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/utils/identifiers.py
+-rw-r--r--   0        0        0     2459 2023-06-01 13:49:57.544140 intelliprove-1.1.0/intelliprove/api/utils/media.py
+-rw-r--r--   0        0        0      426 2023-06-01 13:49:57.544140 intelliprove-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2223 1970-01-01 00:00:00.000000 intelliprove-1.1.0/PKG-INFO
```

### Comparing `intelliprove-1.0.1/README.md` & `intelliprove-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.1/intelliprove/api/api_service.py` & `intelliprove-1.1.0/intelliprove/api/api_service.py`

 * *Files 3% similar despite different names*

```diff
@@ -93,14 +93,25 @@
         uri = self.make_url(f"results/wait/{uuid}")
 
         resp = requests.get(uri, **self.request_kwargs)
         self._check_status_code(resp, (200, 204))
         result = resp.json()
         return BiomarkersResponse.from_json(result) if resp.status_code == 200 and isinstance(result, dict) and len(result.keys()) > 0 else None
 
+    def create_action_token(self, expires_in: int, metadata: dict) -> str:
+        uri = self.make_url(f"auth/action-token")
+
+        resp = requests.post(uri, data={
+            'expire_in': expires_in,
+            'meta': metadata
+        }, **self.request_kwargs)
+        self._check_status_code(resp)
+        result = resp.json()
+        return result['token']
+
     @property
     def headers(self) -> dict:
         return {
             'x-api-key': self.api_key,
             'Accept': 'application/json'
         }
```

### Comparing `intelliprove-1.0.1/intelliprove/api/exceptions/api.py` & `intelliprove-1.1.0/intelliprove/api/exceptions/api.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.1/intelliprove/api/exceptions/media.py` & `intelliprove-1.1.0/intelliprove/api/exceptions/media.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.1/intelliprove/api/intelliprove_api.py` & `intelliprove-1.1.0/intelliprove/api/intelliprove_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+from datetime import timedelta
 import logging
 
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 
 from intelliprove.api.api_service import ApiService
 from intelliprove.api.models import IntelliproveApiSettings, Biomarkers, Quality
 from intelliprove.api.models.responses import BiomarkersResponse
 from intelliprove.api.models.enums import QualityErrorType
 from intelliprove.api.utils import is_valid_video_path, is_valid_image_path, get_first_video_frame, check_file_size
 from intelliprove.api.exceptions import ImageQualityException, MediaException, ApiResultNotAvailable
@@ -73,7 +74,19 @@
             frame_path = get_first_video_frame(snapshot)
             return self.api.check_image(frame_path).to_dataclass()
 
         if is_valid_image_path(snapshot):
             return self.api.check_image(snapshot).to_dataclass()
 
         raise MediaException("Expected snapshot to be image or video file, invalid format or file not found.", snapshot)
+
+    def create_action_token(self, expires_in: Union[int, timedelta] = timedelta(hours=6), metadata: dict = {}) -> str:
+        """
+        Create a new action token
+        """
+
+        if isinstance(expires_in, timedelta):
+            expires_in = expires_in.seconds
+
+        token = self.api.create_action_token(expires_in, metadata)
+        return token
+
```

### Comparing `intelliprove-1.0.1/intelliprove/api/models/dataclasses/biomarkers.py` & `intelliprove-1.1.0/intelliprove/api/models/dataclasses/biomarkers.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.1/intelliprove/api/models/dataclasses/settings.py` & `intelliprove-1.1.0/intelliprove/api/models/dataclasses/settings.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.1/intelliprove/api/models/responses/biomarkers_response.py` & `intelliprove-1.1.0/intelliprove/api/models/responses/biomarkers_response.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.1/intelliprove/api/models/responses/quality_response.py` & `intelliprove-1.1.0/intelliprove/api/models/responses/quality_response.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.1/intelliprove/api/utils/media.py` & `intelliprove-1.1.0/intelliprove/api/utils/media.py`

 * *Files identical despite different names*

### Comparing `intelliprove-1.0.1/PKG-INFO` & `intelliprove-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: intelliprove
-Version: 1.0.1
+Version: 1.1.0
 Summary: The Python SDK for using IntelliProve.
 Author: Seppe De Langhe
 Author-email: seppe.delanghe@intelliprove.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

