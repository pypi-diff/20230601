# Comparing `tmp/privateai_client-1.1.0.tar.gz` & `tmp/privateai_client-1.2.0.tar.gz`

## Comparing `privateai_client-1.1.0.tar` & `privateai_client-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.1.0/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 privateai_client-1.1.0/.github/pull-request-template.md
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 privateai_client-1.1.0/.vscode/settings.json
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/__init__.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/objects.py
--rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/pai_client.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/components/__init__.py
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/components/pai_requests.py
--rw-r--r--   0        0        0     3483 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/components/pai_responses.py
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/components/pai_uris.py
--rw-r--r--   0        0        0    17874 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/components/request_objects.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/tests/__init__.py
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/tests/test_client.py
--rw-r--r--   0        0        0    32963 2020-02-02 00:00:00.000000 privateai_client-1.1.0/src/privateai_client/tests/test_request_objects.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 privateai_client-1.1.0/.gitignore
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-1.1.0/LICENSE
--rw-r--r--   0        0        0    11926 2020-02-02 00:00:00.000000 privateai_client-1.1.0/README.md
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 privateai_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    12557 2020-02-02 00:00:00.000000 privateai_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 privateai_client-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.2.0/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 privateai_client-1.2.0/.github/pull-request-template.md
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 privateai_client-1.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/__init__.py
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/objects.py
+-rw-r--r--   0        0        0     5058 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/pai_client.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/components/__init__.py
+-rw-r--r--   0        0        0     2055 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/components/pai_requests.py
+-rw-r--r--   0        0        0     3733 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/components/pai_responses.py
+-rw-r--r--   0        0        0     1644 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/components/pai_uris.py
+-rw-r--r--   0        0        0    23503 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/components/request_objects.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/tests/__init__.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/tests/test_client.py
+-rw-r--r--   0        0        0    39761 2020-02-02 00:00:00.000000 privateai_client-1.2.0/src/privateai_client/tests/test_request_objects.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 privateai_client-1.2.0/.gitignore
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 privateai_client-1.2.0/LICENSE
+-rw-r--r--   0        0        0    12896 2020-02-02 00:00:00.000000 privateai_client-1.2.0/README.md
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 privateai_client-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    13527 2020-02-02 00:00:00.000000 privateai_client-1.2.0/PKG-INFO
```

### Comparing `privateai_client-1.1.0/src/privateai_client/objects.py` & `privateai_client-1.2.0/src/privateai_client/objects.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from .components import request_objects as req_objects
 
-class request_objects:
 
+class request_objects:
     bleep_obj = req_objects.BleepRequest
     file_uri_obj = req_objects.ProcessFileUriRequest
     file_base64_obj = req_objects.ProcessFileBase64Request
     process_text_obj = req_objects.ProcessTextRequest
     audio_options_obj = req_objects.AudioOptions
+    entity = req_objects.Entity
     entity_type_selector_obj = req_objects.EntityTypeSelector
     entity_detection_obj = req_objects.EntityDetection
     file_obj = req_objects.File
     filter_selector_obj = req_objects.FilterSelector
     pdf_options_obj = req_objects.PDFOptions
     processed_text_obj = req_objects.ProcessedText
+    reidentify_text_obj = req_objects.ReidentifyTextRequest
     timestamp_obj = req_objects.Timestamp
-
```

### Comparing `privateai_client-1.1.0/src/privateai_client/pai_client.py` & `privateai_client-1.2.0/src/privateai_client/pai_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,118 +2,141 @@
 from typing import Union
 
 from .components import *
 
 
 class PAIClient:
     """
-    Client used to connect to private-ai's deidentication service   
+    Client used to connect to private-ai's deidentication service
     """
-    def __init__(self, scheme:str, host: str, port:str = None, **kwargs):
+
+    def __init__(self, scheme: str, host: str, port: str = None, **kwargs):
         # Add source url
         self.uris = PAIURIs(scheme, host, port)
         self.get = PAIGetRequests(self.uris)
         self.post = PAIPostRequests(self.uris)
         if "api_key" in kwargs.keys():
-            self.add_api_key(kwargs['api_key'])
+            self.add_api_key(kwargs["api_key"])
         elif "bearer_token" in kwargs.keys():
-            self.add_bearer_token(kwargs['bearer_token'])
-        
+            self.add_bearer_token(kwargs["bearer_token"])
+
     def _add_auth(self, auth_type, auth_val):
         auth_header = {}
-        if auth_type == 'api_key':
-            auth_header = {'x-api-key': auth_val}
-        elif auth_type == 'bearer_token':
-            auth_header = {'Authorization': f"Bearer {auth_val}"}
+        if auth_type == "api_key":
+            auth_header = {"x-api-key": auth_val}
+        elif auth_type == "bearer_token":
+            auth_header = {"Authorization": f"Bearer {auth_val}"}
         else:
-            raise ValueError(f"{auth_type} is not currently a supported method of authorization")
+            raise ValueError(
+                f"{auth_type} is not currently a supported method of authorization"
+            )
         for subclass in [self.get, self.post]:
             subclass.headers = {**auth_header, **subclass.base_header}
 
     def add_api_key(self, api_key):
         self._add_auth("api_key", api_key)
 
     def add_bearer_token(self, token):
-        self._add_auth('bearer_token', token)
+        self._add_auth("bearer_token", token)
 
     def ping(self):
         """
-        Makes a call to the Private-AI service's health endpoint. 
+        Makes a call to the Private-AI service's health endpoint.
         Can be used as a validator to ensure the service is running.
         """
         response = self.get.health()
         if response.status_code != 200:
             logging.warning(f"The Private AI server cannot be reached")
             return False
         return True
 
     def get_metrics(self):
         """
         Returns information about the Private-AI's server
         """
         return MetricsResponse(self.get.metrics())
-    
+
     def get_version(self):
         """
         Returns the version of the container application code
         """
         return VersionResponse(self.get.version)
-    
+
     def process_text(self, request_object: Union[dict, ProcessTextRequest]):
         """
-        Used to deidentify text 
+        Used to deidentify text
         """
         if type(request_object) is ProcessTextRequest:
             response = TextResponse(self.post.process_text(request_object.to_dict()))
         elif type(request_object) is dict:
             response = TextResponse(self.post.process_text(request_object))
         else:
-            raise ValueError("request_object can only be a dictionary or a ProcessTextRequest object")
+            raise ValueError(
+                "request_object can only be a dictionary or a ProcessTextRequest object"
+            )
         return response
-    
+
+    def reidentify_text(self, request_object: Union[dict, ReidentifyTextRequest]):
+        """
+        Used to reidentify text
+        """
+        if type(request_object) is ReidentifyTextRequest:
+            response = ReidentifyTextResponse(
+                self.post.reidentify_text(request_object.to_dict())
+            )
+        elif type(request_object) is dict:
+            response = ReidentifyTextRequest(self.post.process_text(request_object))
+        else:
+            raise ValueError(
+                "request_object can only be a dictionary or a ReidentifyTextRequest object"
+            )
+        return response
+
     def process_files_uri(self, request_object: Union[dict, ProcessFileUriRequest]):
         """
         Used to deidentify files by uri
         """
         if type(request_object) is ProcessFileUriRequest:
-            response = FilesUriResponse(self.post.process_files_uri(request_object.to_dict()))
+            response = FilesUriResponse(
+                self.post.process_files_uri(request_object.to_dict())
+            )
         elif type(request_object) is dict:
             response = FilesUriResponse(self.post.process_files_uri(request_object))
         else:
-            raise ValueError("request_object can only be a dictionary or a ProcessFileUriRequest object")
+            raise ValueError(
+                "request_object can only be a dictionary or a ProcessFileUriRequest object"
+            )
         return response
 
-    def process_files_base64(self, request_object: Union[dict, ProcessFileBase64Request]):
+    def process_files_base64(
+        self, request_object: Union[dict, ProcessFileBase64Request]
+    ):
         """
         Used to deidentify base64 files
         """
         if type(request_object) is ProcessFileBase64Request:
-            response = FilesBase64Response(self.post.process_files_base64(request_object.to_dict()))
+            response = FilesBase64Response(
+                self.post.process_files_base64(request_object.to_dict())
+            )
         elif type(request_object) is dict:
-            response = FilesBase64Response(self.post.process_files_base64(request_object))
+            response = FilesBase64Response(
+                self.post.process_files_base64(request_object)
+            )
         else:
-            raise ValueError("request_object can only be a dictionary or a ProcessFileBase64Request object")
+            raise ValueError(
+                "request_object can only be a dictionary or a ProcessFileBase64Request object"
+            )
         return response
-    
+
     def bleep(self, request_object: Union[dict, BleepRequest]):
         """
         Used to deidentify files by uri
         """
         if type(request_object) is BleepRequest:
             response = BleepResponse(self.post.bleep(request_object.to_dict()))
         elif type(request_object) is dict:
             response = BleepResponse(self.post.bleep(request_object))
         else:
-            raise ValueError("request_object can only be a dictionary or a BleepRequest object")
+            raise ValueError(
+                "request_object can only be a dictionary or a BleepRequest object"
+            )
         return response
-
-    
-
-    
-
-
-
-
-
-
-
-
```

### Comparing `privateai_client-1.1.0/src/privateai_client/components/pai_responses.py` & `privateai_client-1.2.0/src/privateai_client/components/pai_responses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from requests import Response
 
 
-
 class BaseResponse:
-
-    def __init__(self, response_object: Response, json_response:bool =True):
+    def __init__(self, response_object: Response, json_response: bool = True):
         self._response = response_object
         # Should be json or text
         self._json_response = json_response
 
     def __call__(self):
         return self.response
 
@@ -23,103 +21,110 @@
     @property
     def ok(self):
         return self().ok
 
     @property
     def status_code(self):
         return self().status_code
-    
+
     @property
     def body(self):
         if self._json_response:
-            return self().json() 
+            return self().json()
         else:
             return self().text
 
     @response.setter
     def response(self, new_response):
         if type(new_response) is not Response:
             raise ValueError("response must be a Response object")
         self._response = new_response
 
     def get_attribute_entries(self, name):
         # Used for any nested data in the response body
-        if not self._json_response: 
+        if not self._json_response:
             raise ValueError("get_attribute_entries needs a response of type json")
         body = self.body
         if type(body) is list:
-            return [row.get(name) for row in self().json()]
+            return (
+                self.body[0].get(name)
+                if len(body) == 1
+                else [row.get(name) for row in self().json()]
+            )
         elif type(body) is dict:
             return body.get(name)
 
 
 class MetricsResponse(BaseResponse):
-
-    def __init__(self, response_object: Response=None):
+    def __init__(self, response_object: Response = None):
         super(MetricsResponse, self).__init__(response_object, False)
 
-class VersionResponse(BaseResponse):
 
-    def __init__(self, response_object: Response=None):
+class VersionResponse(BaseResponse):
+    def __init__(self, response_object: Response = None):
         super(VersionResponse, self).__init__(response_object, True)
 
     @property
     def app_version(self):
-        return self.get_attribute_entries('app_version')
+        return self.get_attribute_entries("app_version")
 
-class DemiTextResponse(BaseResponse):
 
-    def __init__(self, response_object: Response=None):
+class DemiTextResponse(BaseResponse):
+    def __init__(self, response_object: Response = None):
         super(DemiTextResponse, self).__init__(response_object, True)
 
     @property
     def processed_text(self):
         return self.get_attribute_entries("processed_text")
-    
+
     @property
     def entities(self):
         return self.get_attribute_entries("entities")
-    
+
     @property
     def entities_present(self):
         return self.get_attribute_entries("entities_present")
 
-class TextResponse(DemiTextResponse):
 
-    def __init__(self, response_object: Response=None):
+class TextResponse(DemiTextResponse):
+    def __init__(self, response_object: Response = None):
         super(TextResponse, self).__init__(response_object)
-    
+
     @property
     def characters_processed(self):
         return self.get_attribute_entries("characters_processed")
-    
+
     @property
     def languages_detected(self):
         return self.get_attribute_entries("languages_detected")
-    
-class FilesUriResponse(DemiTextResponse):
 
+
+class FilesUriResponse(DemiTextResponse):
     def __init__(self, response_object: Response = None):
         super(FilesUriResponse, self).__init__(response_object)
 
     @property
     def result_uri(self):
         return self.get_attribute_entries("result_uri")
-    
-class FilesBase64Response(DemiTextResponse):
 
+
+class FilesBase64Response(DemiTextResponse):
     def __init__(self, response_object: Response = None):
         super(FilesBase64Response, self).__init__(response_object)
 
     @property
     def processed_file(self):
         return self.get_attribute_entries("processed_file")
-    
-class BleepResponse(BaseResponse):
 
+
+class BleepResponse(BaseResponse):
     def __init__(self, response_object: Response = None):
         super(BleepResponse, self).__init__(response_object, True)
-    
+
     @property
     def bleeped_file(self):
         return self.get_attribute_entries("bleeped_file")
-        
+
+
+class ReidentifyTextResponse(BaseResponse):
+    def __init__(self, response_object: Response = None):
+        super(ReidentifyTextResponse, self).__init__(response_object, True)
```

### Comparing `privateai_client-1.1.0/src/privateai_client/components/pai_uris.py` & `privateai_client-1.2.0/src/privateai_client/components/pai_uris.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,51 +1,59 @@
-
-
 class PAIURIs:
-
     def __init__(self, scheme, host, port=None):
-        self.valid_schemes = ['http', 'https']
-        scheme = scheme.split('://')[0]
+        self.valid_schemes = ["http", "https"]
+        scheme = scheme.split("://")[0]
         if scheme not in self.valid_schemes:
-            raise ValueError(f"Scheme must be one of the following: {', '.join(self.valid_schemes)}")
+            raise ValueError(
+                f"Scheme must be one of the following: {', '.join(self.valid_schemes)}"
+            )
         port = f":{port}" if port else ""
         self._pai_uri = f"{scheme}://{host}{port}"
 
     @property
     def pai_uri(self):
         return self._pai_uri
-    
+
     @property
     def api_version(self):
         return "v3"
 
     @property
     def bleep(self):
         return self._create_uri(self.pai_uri, self.api_version, "bleep")
 
     @property
     def health(self):
         return self._create_uri(self.pai_uri, "healthz")
-    
+
     @property
     def metrics(self):
         return self._create_uri(self.pai_uri, "metrics")
-    
+
     @property
     def process_text(self):
         return self._create_uri(self.pai_uri, self.api_version, "process", "text")
-    
+
     @property
     def process_files_uri(self):
-        return self._create_uri(self.pai_uri, self.api_version, "process", "files", "uri")
-    
+        return self._create_uri(
+            self.pai_uri, self.api_version, "process", "files", "uri"
+        )
+
+    @property
+    def reidentify_text(self):
+        return self._create_uri(
+            self.pai_uri, self.api_version, "process", "text", "reidentify"
+        )
+
     @property
     def process_files_base64(self):
-        return self._create_uri(self.pai_uri, self.api_version, "process", "files", "base64")
+        return self._create_uri(
+            self.pai_uri, self.api_version, "process", "files", "base64"
+        )
 
     @property
     def version(self):
         return self._create_uri(self.pai_uri, "")
 
     def _create_uri(self, *args):
         return "/".join([x.strip("/") for x in args])
-
```

### Comparing `privateai_client-1.1.0/src/privateai_client/tests/test_request_objects.py` & `privateai_client-1.2.0/src/privateai_client/tests/test_request_objects.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,644 +5,1086 @@
 
 # File Tests
 def test_file_initializer():
     file = File(data="test", content_type="application/pdf")
     assert file.data == "test"
     assert file.content_type == "application/pdf"
 
+
 def test_file_initializer_fromdict():
-    file = File.fromdict({"data":"test", "content_type":"application/pdf"})
+    file = File.fromdict({"data": "test", "content_type": "application/pdf"})
     assert file.data == "test"
     assert file.content_type == "application/pdf"
 
+
 def test_file_invalid_initialize_fromdict():
     error_msg = "File can only accept the values 'data' and 'content_type'"
     with pytest.raises(TypeError) as excinfo:
-        File.fromdict({"data":"test", "content_type":"application/pdf", "garbage":"value"})
+        File.fromdict(
+            {"data": "test", "content_type": "application/pdf", "garbage": "value"}
+        )
     assert error_msg in str(excinfo.value)
 
+
 def test_file_data_validator():
     error_msg = "data must be string-type"
     with pytest.raises(TypeError) as excinfo:
         file = File(data=12, content_type="application/pdf")
     assert error_msg in str(excinfo.value)
 
+
 def test_file_content_type_validator():
     error_msg = "strawberry/filling is not valid. File.content_type can only be one of the following:"
     with pytest.raises(ValueError) as excinfo:
         file = File(data="test", content_type="strawberry/filling")
     assert error_msg in str(excinfo.value)
 
+
 def test_file_setters():
     file = File(data="test", content_type="application/pdf")
     file.data = "new test"
     file.content_type = "application/xml"
     assert file.data == "new test"
     assert file.content_type == "application/xml"
 
+
 # Filter Selector Tests
 def test_filter_selector_initializer():
     test_type = "ALLOW"
     test_pattern = "[A-Z]"
     filter_selector = FilterSelector(type=test_type, pattern=test_pattern)
     assert filter_selector.type == test_type
     assert filter_selector.pattern == test_pattern
 
+
 def test_filter_selector_initialize_fromdict():
     test_type = "ALLOW"
     test_pattern = "[A-Z]"
     test_dict = {"type": test_type, "pattern": test_pattern}
     filter_selector = FilterSelector.fromdict(test_dict)
     assert filter_selector.type == test_type
     assert filter_selector.pattern == test_pattern
 
+
 def test_filter_selector_invalid_initialize_fromdict():
     with pytest.raises(TypeError) as excinfo:
-        FilterSelector.fromdict({"type": "ALLOW", "pattern": "[A-Z]", "fake_key": "fake_value"})
-    assert "FilterSelector can only accept the values 'type' and 'pattern'" in str(excinfo.value)
+        FilterSelector.fromdict(
+            {"type": "ALLOW", "pattern": "[A-Z]", "fake_key": "fake_value"}
+        )
+    assert "FilterSelector can only accept the values 'type' and 'pattern'" in str(
+        excinfo.value
+    )
+
 
 def test_filter_selector_setters():
     test_type = "ALLOW"
     test_pattern = "[A-Z]"
     filter_selector = FilterSelector(type=test_type, pattern=test_pattern)
     filter_selector.type = "BLOCK"
     filter_selector.pattern = "*1"
-    
+
     assert filter_selector.type == "BLOCK"
     assert filter_selector.pattern == "*1"
 
+
 def test_filter_selector_type_validator():
     test_type = "JUNK"
     test_pattern = "[A-Z]"
     with pytest.raises(ValueError) as excinfo:
         FilterSelector(type=test_type, pattern=test_pattern)
-    assert " is not valid. FilterSelector.type can only be one of the following: " in str(excinfo.value)
+    assert (
+        " is not valid. FilterSelector.type can only be one of the following: "
+        in str(excinfo.value)
+    )
+
 
 def test_filter_selector_pattern_validator():
     test_type = "ALLOW"
     test_pattern = 12
     with pytest.raises(TypeError) as excinfo:
         FilterSelector(type=test_type, pattern=test_pattern)
     assert "FilterSelector.pattern must be of type string" in str(excinfo.value)
 
+
 def test_filter_to_dict():
     test_type = "ALLOW"
     test_pattern = "[A-Z]"
     filter_selector = FilterSelector(type=test_type, pattern=test_pattern)
     filter_dict = filter_selector.to_dict()
-    assert filter_dict["type"]== test_type
+    assert filter_dict["type"] == test_type
     assert filter_dict["pattern"] == test_pattern
 
+
+# Entity Tests
+def test_entity_initializer():
+    entity = Entity(processed_text="NAME_1", text="this is a test")
+    assert entity.processed_text == "NAME_1"
+    assert entity.text == "this is a test"
+
+
+def test_entity_initializer_fromdict():
+    entity = Entity.fromdict({"processed_text": "NAME_1", "text": "this is a test"})
+    assert entity.processed_text == "NAME_1"
+    assert entity.text == "this is a test"
+
+
+def test_entity_invalid_initialize_fromdict():
+    error_msg = "Entity can only accept the values 'processed_text' and 'text'"
+    with pytest.raises(TypeError) as excinfo:
+        Entity.fromdict(
+            {"processed_text": "NAME_1", "text": "this is a test", "garbage": "value"}
+        )
+    assert error_msg in str(excinfo.value)
+
+
+def test_entity_processed_text_validator():
+    error_msg = "Entity.processed_text must be of type string"
+    with pytest.raises(TypeError) as excinfo:
+        Entity(processed_text=12, text="ayy")
+    assert error_msg in str(excinfo.value)
+
+
+def test_entity_text_validator():
+    error_msg = "Entity.text must be of type string"
+    with pytest.raises(TypeError) as excinfo:
+        entity = Entity(processed_text="ORGANIZATION_60", text=45.2)
+    assert error_msg in str(excinfo.value)
+
+
+def test_entity_setters():
+    entity = Entity(processed_text="NAME_1", text="Jerry Stevens")
+    entity.processed_text = "CONDITION_20"
+    entity.text = "Broken leg"
+    assert entity.processed_text == "CONDITION_20"
+    assert entity.text == "Broken leg"
+
+
 # Entity Type Selector Tests
 def test_entity_type_selector_initializer():
     test_type = "DISABLE"
 
     entity_type_selector = EntityTypeSelector(type=test_type)
     assert entity_type_selector.type == test_type
     assert entity_type_selector.value == []
 
+
 def test_entity_type_selector_initialize_fromdict():
-    entity_type_obj = EntityTypeSelector.fromdict({"type":"ENABLE", "value":["NAME"]})
+    entity_type_obj = EntityTypeSelector.fromdict({"type": "ENABLE", "value": ["NAME"]})
     assert entity_type_obj.type == "ENABLE"
     assert entity_type_obj.value == ["NAME"]
 
+
 def test_entity_type_selector_invalid_initialize_fromdict():
     error_msg = "EntityTypeSelector can only accept the values 'type' and 'value'"
     with pytest.raises(TypeError) as excinfo:
-        EntityTypeSelector.fromdict({"type":"ENABLE", "value":["NAME"], "garbage":"value"})
+        EntityTypeSelector.fromdict(
+            {"type": "ENABLE", "value": ["NAME"], "garbage": "value"}
+        )
     assert error_msg in str(excinfo.value)
 
+
 def test_entity_type_selector_setters():
-    entity_type_obj = EntityTypeSelector(type="ENABLE", value=['LOCATION'])
+    entity_type_obj = EntityTypeSelector(type="ENABLE", value=["LOCATION"])
     entity_type_obj.type = "DISABLE"
     assert entity_type_obj.type == "DISABLE"
 
+
 def test_entity_type_selector_type_validator():
-    error_msg = "'JUNK' is not valid. EntityTypeSelector.type can only be one of the following: " 
-    entity_type_obj = EntityTypeSelector(type="ENABLE", value=['LOCATION'])
+    error_msg = "'JUNK' is not valid. EntityTypeSelector.type can only be one of the following: "
+    entity_type_obj = EntityTypeSelector(type="ENABLE", value=["LOCATION"])
     with pytest.raises(ValueError) as excinfo:
-        entity_type_obj.type = 'JUNK'
+        entity_type_obj.type = "JUNK"
     assert error_msg in str(excinfo.value)
 
+
 def test_entity_type_selector_value_validator():
     error_msg = "EntityTypeSelector.value must be of type list"
     with pytest.raises(TypeError) as excinfo:
         EntityTypeSelector(type="ENABLE", value={})
     assert error_msg in str(excinfo.value)
 
+
 def test_entity_type_selector_to_dict():
-    entity_type_obj = EntityTypeSelector.fromdict({"type":"ENABLE", "value":["NAME"]}).to_dict()
+    entity_type_obj = EntityTypeSelector.fromdict(
+        {"type": "ENABLE", "value": ["NAME"]}
+    ).to_dict()
     assert entity_type_obj["type"] == "ENABLE"
     assert entity_type_obj["value"] == ["NAME"]
 
+
 # Entity Detection Tests
 def test_entity_detection_default_initializer():
     entity_detection = EntityDetection()
     assert entity_detection.accuracy == "high"
     assert entity_detection.entity_types == []
     assert entity_detection.filter == []
     assert entity_detection.return_entity == True
 
+
 def test_entity_detection_initializer():
-    entity_detection_obj = EntityDetection(accuracy="high",
-                                           entity_types=[EntityTypeSelector(type="ENABLE")],
-                                           filter=[FilterSelector(type="ALLOW", pattern="hey")],
-                                           return_entity=False
+    entity_detection_obj = EntityDetection(
+        accuracy="high",
+        entity_types=[EntityTypeSelector(type="ENABLE")],
+        filter=[FilterSelector(type="ALLOW", pattern="hey")],
+        return_entity=False,
     )
     assert entity_detection_obj.accuracy == "high"
     assert type(entity_detection_obj.entity_types[0]) is EntityTypeSelector
     assert type(entity_detection_obj.filter[0]) is FilterSelector
     assert entity_detection_obj.return_entity is False
 
 
 def test_entity_detection_initialize_fromdict():
-    entity_detection = EntityDetection.fromdict({"accuracy":"high", 
-                                                 "entity_types":[EntityTypeSelector(type="ENABLE").to_dict()],
-                                                 "filter": [FilterSelector(type="ALLOW", pattern="hey").to_dict()],
-                                                 "return_entity": False
-                        })
+    entity_detection = EntityDetection.fromdict(
+        {
+            "accuracy": "high",
+            "entity_types": [EntityTypeSelector(type="ENABLE").to_dict()],
+            "filter": [FilterSelector(type="ALLOW", pattern="hey").to_dict()],
+            "return_entity": False,
+        }
+    )
     assert entity_detection.accuracy == "high"
     assert type(entity_detection.entity_types[0]) is EntityTypeSelector
     assert type(entity_detection.filter[0]) is FilterSelector
     assert entity_detection.return_entity is False
 
+
 def test_entity_detection_invalid_initialize_fromdict():
     error_msg = "EntityDetection can only accept the values 'accuracy', 'entity_types', 'filter' and 'return_entity'"
     with pytest.raises(TypeError) as excinfo:
-        EntityDetection.fromdict({"accuracy":"high", 
-                                  "entity_types":[EntityTypeSelector(type="ENABLE").to_dict()],
-                                  "filter": [FilterSelector(type="ALLOW", pattern="hey").to_dict()],
-                                  "return_entity": False,
-                                  "garbage": "value"
-        })
+        EntityDetection.fromdict(
+            {
+                "accuracy": "high",
+                "entity_types": [EntityTypeSelector(type="ENABLE").to_dict()],
+                "filter": [FilterSelector(type="ALLOW", pattern="hey").to_dict()],
+                "return_entity": False,
+                "garbage": "value",
+            }
+        )
     assert error_msg in str(excinfo.value)
 
+
 def test_entity_detection_setters():
-    entity_detection_obj = EntityDetection.fromdict({"accuracy":"high", 
-                                                 "entity_types":[EntityTypeSelector(type="ENABLE").to_dict()],
-                                                 "filter": [FilterSelector(type="ALLOW", pattern="hey").to_dict()],
-                                                 "return_entity": False
-    })
-    entity_detection_obj.accuracy = 'standard'
+    entity_detection_obj = EntityDetection.fromdict(
+        {
+            "accuracy": "high",
+            "entity_types": [EntityTypeSelector(type="ENABLE").to_dict()],
+            "filter": [FilterSelector(type="ALLOW", pattern="hey").to_dict()],
+            "return_entity": False,
+        }
+    )
+    entity_detection_obj.accuracy = "standard"
     entity_detection_obj.return_entity = True
-    assert entity_detection_obj.accuracy == 'standard'
+    assert entity_detection_obj.accuracy == "standard"
     assert entity_detection_obj.return_entity == True
 
+
 def test_entity_detection_accuracy_validator():
-    error_msg = "junk is not valid. EntityDetection.accuracy can only be one of the following: "
-    entity_detection_obj = EntityDetection.fromdict({"accuracy":"high", 
-                                                 "entity_types":[EntityTypeSelector(type="ENABLE").to_dict()],
-                                                 "filter": [FilterSelector(type="ALLOW", pattern="hey").to_dict()],
-                                                 "return_entity": False
-    })
+    error_msg = (
+        "junk is not valid. EntityDetection.accuracy can only be one of the following: "
+    )
+    entity_detection_obj = EntityDetection.fromdict(
+        {
+            "accuracy": "high",
+            "entity_types": [EntityTypeSelector(type="ENABLE").to_dict()],
+            "filter": [FilterSelector(type="ALLOW", pattern="hey").to_dict()],
+            "return_entity": False,
+        }
+    )
     with pytest.raises(ValueError) as excinfo:
         entity_detection_obj.accuracy = "junk"
     assert error_msg in str(excinfo.value)
 
+
 def test_entity_detection_entity_types_validator():
-    error_msg = "EntityDetection.entity_types can only contain EntityTypeSelector objects"
+    error_msg = (
+        "EntityDetection.entity_types can only contain EntityTypeSelector objects"
+    )
     with pytest.raises(ValueError) as excinfo:
-        EntityDetection(accuracy="high",
+        EntityDetection(
+            accuracy="high",
             entity_types=["junk"],
             filter=[FilterSelector(type="ALLOW", pattern="hey")],
-            return_entity=False
+            return_entity=False,
         )
     assert error_msg in str(excinfo.value)
 
+
 def test_entity_detection_entity_types_validator():
     error_msg = "EntityDetection.filter can only contain FilterSelector objects"
     with pytest.raises(ValueError) as excinfo:
-        EntityDetection(accuracy="high",
+        EntityDetection(
+            accuracy="high",
             entity_types=[EntityTypeSelector(type="ENABLE")],
             filter=["junk"],
-            return_entity=False
+            return_entity=False,
         )
     assert error_msg in str(excinfo.value)
 
+
 def test_entity_detection_return_entity_validator():
     error_msg = "EntityDetection.return_entity must be of type bool"
-    entity_detection_obj = EntityDetection.fromdict({"accuracy":"high", 
-                                                 "entity_types":[EntityTypeSelector(type="ENABLE").to_dict()],
-                                                 "filter": [FilterSelector(type="ALLOW", pattern="hey").to_dict()],
-                                                 "return_entity": False
-    })
+    entity_detection_obj = EntityDetection.fromdict(
+        {
+            "accuracy": "high",
+            "entity_types": [EntityTypeSelector(type="ENABLE").to_dict()],
+            "filter": [FilterSelector(type="ALLOW", pattern="hey").to_dict()],
+            "return_entity": False,
+        }
+    )
     with pytest.raises(ValueError) as excinfo:
         entity_detection_obj.return_entity = "junk"
     assert error_msg in str(excinfo.value)
 
+
 def test_entity_detection_to_dict():
-    entity_detection_obj = EntityDetection(accuracy="high",
-                                           entity_types=[EntityTypeSelector(type="ENABLE")],
-                                           filter=[FilterSelector(type="ALLOW", pattern="hey")],
-                                           return_entity=False
+    entity_detection_obj = EntityDetection(
+        accuracy="high",
+        entity_types=[EntityTypeSelector(type="ENABLE")],
+        filter=[FilterSelector(type="ALLOW", pattern="hey")],
+        return_entity=False,
     ).to_dict()
     assert entity_detection_obj["accuracy"] == "high"
     assert type(entity_detection_obj["entity_types"][0]) is dict
     assert type(entity_detection_obj["filter"][0]) is dict
     assert entity_detection_obj["return_entity"] is False
 
+
 # Processed Text Tests
 def test_processed_text_default_initializer():
     processed_text = ProcessedText()
     assert processed_text.type == "MARKER"
     assert processed_text.pattern == "[UNIQUE_NUMBERED_ENTITY_TYPE]"
 
+
 def test_processed_text_initializer():
-    processed_text = ProcessedText(type="MASK", pattern= "*ALL_ENTITY_TYPES*")
+    processed_text = ProcessedText(type="MASK", mask_character="*")
     assert processed_text.type == "MASK"
-    assert processed_text.pattern == "*ALL_ENTITY_TYPES*"
+    assert processed_text.mask_character == "*"
+
 
 def test_processed_text_initialize_fromdict():
-    processed_text = ProcessedText.fromdict({"type":"MARKER","pattern":"[UNIQUE_NUMBERED_ENTITY_TYPE]"})
+    processed_text = ProcessedText.fromdict(
+        {"type": "MARKER", "pattern": "[UNIQUE_NUMBERED_ENTITY_TYPE]"}
+    )
     assert processed_text.type == "MARKER"
     assert processed_text.pattern == "[UNIQUE_NUMBERED_ENTITY_TYPE]"
 
+
 def test_processed_text_invalid_initialize_fromdict():
     error_msg = "ProcessedText can only accept the values 'type' and 'pattern'"
     with pytest.raises(TypeError) as excinfo:
-        ProcessedText.fromdict({"type":"MARKER","pattern":"[UNIQUE_NUMBERED_ENTITY_TYPE]", "junk":"value"})
+        ProcessedText.fromdict(
+            {
+                "type": "MARKER",
+                "pattern": "[UNIQUE_NUMBERED_ENTITY_TYPE]",
+                "junk": "value",
+            }
+        )
     assert error_msg in str(excinfo.value)
 
+
 def test_processed_text_setters():
     processed_text = ProcessedText()
     processed_text.type = "MASK"
     processed_text.pattern = "*ALL_ENTITY_TYPES*"
     assert processed_text.type == "MASK"
     assert processed_text.pattern == "*ALL_ENTITY_TYPES*"
 
+
 def test_processed_text_type_validator():
-    error_msg = "junk is not valid. ProcessedText.type can only be one of the following: "
+    error_msg = (
+        "junk is not valid. ProcessedText.type can only be one of the following: "
+    )
     with pytest.raises(ValueError) as excinfo:
-        ProcessedText.fromdict({"type":"junk","pattern":"[UNIQUE_NUMBERED_ENTITY_TYPE]"})
+        ProcessedText.fromdict(
+            {"type": "junk", "pattern": "[UNIQUE_NUMBERED_ENTITY_TYPE]"}
+        )
     assert error_msg in str(excinfo.value)
 
+
 def test_processed_text_pattern_validator():
-    error_msg = "junk is not valid. ProcessedText.pattern can only be one of the following: "
+    error_msg = (
+        "junk is not valid. ProcessedText.pattern can only be one of the following: "
+    )
     with pytest.raises(ValueError) as excinfo:
-        ProcessedText.fromdict({"type":"MASK","pattern":"junk"})
+        ProcessedText.fromdict({"type": "MARKER", "pattern": "junk"})
     assert error_msg in str(excinfo.value)
 
+
 def test_processed_text_to_dict():
-    processed_text = ProcessedText(type="MASK", pattern= "*ALL_ENTITY_TYPES*").to_dict()
+    processed_text = ProcessedText(type="MASK", mask_character="*").to_dict()
     assert processed_text["type"] == "MASK"
-    assert processed_text["pattern"] == "*ALL_ENTITY_TYPES*"
+    assert processed_text["mask_character"] == "*"
+
 
 # PDF Options Tests
 def test_pdf_options_default_initializer():
     pdf_options = PDFOptions()
     assert pdf_options.density == 150
 
+
 def test_pdf_options_initializer():
     pdf_options = PDFOptions(density=300)
     assert pdf_options.density == 300
 
+
 def test_pdf_options_initialize_fromdict():
     pdf_options = PDFOptions.fromdict({"density": 300})
     assert pdf_options.density == 300
 
+
 def test_pdf_options_invalid_initialize_fromdict():
     error_msg = "PDFOptions can only accept 'density'"
     with pytest.raises(TypeError) as excinfo:
         PDFOptions.fromdict({"density": 300, "junk": "value"})
     assert error_msg in str(excinfo.value)
 
+
 def test_pdf_options_setters():
     pdf_options = PDFOptions(density=300)
     pdf_options.density = 10
     assert pdf_options.density == 10
 
+
 def test_pdf_options_density_validator():
     error_msg = "PDFOptions.density must be of type int"
     pdf_options = PDFOptions()
     with pytest.raises(ValueError) as excinfo:
         pdf_options.density = "junk"
     assert error_msg in str(excinfo.value)
 
+
 def test_pdf_options_to_dict():
     pdf_options = PDFOptions().to_dict()
-    assert pdf_options['density'] == 150
+    assert pdf_options["density"] == 150
+
 
 # Audio Options Tests
 def test_audio_options_default_initializer():
     audio_options = AudioOptions()
     assert audio_options.bleep_end_padding == 0
     assert audio_options.bleep_start_padding == 0
 
+
 def test_audio_options_initializer():
     audio_options = AudioOptions(bleep_start_padding=200, bleep_end_padding=300)
     assert audio_options.bleep_end_padding == 300
     assert audio_options.bleep_start_padding == 200
 
+
 def test_audio_options_initialize_fromdict():
-    audio_options = AudioOptions.fromdict({"bleep_start_padding":200, "bleep_end_padding":300})
+    audio_options = AudioOptions.fromdict(
+        {"bleep_start_padding": 200, "bleep_end_padding": 300}
+    )
     assert audio_options.bleep_end_padding == 300
     assert audio_options.bleep_start_padding == 200
 
+
 def test_audio_options_invalid_initialize_fromdict():
-    error_msg = "ProcessedText can only accept the values 'bleep_start_padding' and 'bleep_end_padding'" 
+    error_msg = "ProcessedText can only accept the values 'bleep_start_padding' and 'bleep_end_padding'"
     with pytest.raises(TypeError) as excinfo:
-        AudioOptions.fromdict({"bleep_start_padding":200, "bleep_end_padding":300, "junk": "value"})
+        AudioOptions.fromdict(
+            {"bleep_start_padding": 200, "bleep_end_padding": 300, "junk": "value"}
+        )
     assert error_msg in str(excinfo.value)
 
+
 def test_audio_options_setters():
     audio_options = AudioOptions()
     audio_options.bleep_end_padding = 1
     audio_options.bleep_start_padding = 2
 
     assert audio_options.bleep_end_padding == 1
     assert audio_options.bleep_start_padding == 2
 
+
 def test_audio_options_bleep_start_padding_validator():
-    error_msg = "AudioOptions.bleep_start_padding must be of type int" 
+    error_msg = "AudioOptions.bleep_start_padding must be of type int"
     with pytest.raises(ValueError) as excinfo:
         AudioOptions().bleep_start_padding = "junk"
     assert error_msg in str(excinfo.value)
 
+
 def test_audio_options_bleep_end_padding_validator():
-    error_msg = "AudioOptions.bleep_end_padding must be of type int" 
+    error_msg = "AudioOptions.bleep_end_padding must be of type int"
     with pytest.raises(ValueError) as excinfo:
         AudioOptions().bleep_end_padding = "junk"
     assert error_msg in str(excinfo.value)
 
+
 def test_audio_options_to_dict():
     audio_options = AudioOptions().to_dict()
     assert audio_options["bleep_end_padding"] == 0
     assert audio_options["bleep_start_padding"] == 0
 
+
 # Timestamp Tests
 def test_timestamp_initializer():
     timestamp = Timestamp(start=2.0, end=3.0)
     assert timestamp.start == 2.0
     assert timestamp.end == 3.0
 
+
 def test_timestamp_initialize_fromdict():
-    timestamp = Timestamp.fromdict({"start":2.0, "end":3.0})
+    timestamp = Timestamp.fromdict({"start": 2.0, "end": 3.0})
     assert timestamp.start == 2.0
-    assert timestamp.end == 3.0    
+    assert timestamp.end == 3.0
+
 
 def test_timestamp_invalid_initialize_fromdict():
-    error_msg = "Timestamp can only accept the values 'start' and 'end'" 
+    error_msg = "Timestamp can only accept the values 'start' and 'end'"
     with pytest.raises(TypeError) as excinfo:
-        Timestamp.fromdict({"start":2.0, "end":3.0, "junk": "value"})
+        Timestamp.fromdict({"start": 2.0, "end": 3.0, "junk": "value"})
     assert error_msg in str(excinfo.value)
 
+
 def test_timestamp_setters():
     timestamp = Timestamp(start=2.0, end=3.0)
     timestamp.start = 0.0
     timestamp.end = 5.0
     assert timestamp.start == 0.0
     assert timestamp.end == 5.0
 
+
 def test_timestamp_start_validator():
-    error_msg = "Timestamp.start must be of type float" 
+    error_msg = "Timestamp.start must be of type float"
     with pytest.raises(ValueError) as excinfo:
-        Timestamp.fromdict({"start":"test", "end":3.0})
+        Timestamp.fromdict({"start": "test", "end": 3.0})
     assert error_msg in str(excinfo.value)
 
+
 def test_timestamp_end_validator():
     error_msg = "Timestamp.end must be of type float"
     with pytest.raises(ValueError) as excinfo:
-        Timestamp.fromdict({"start":2.0, "end":"test"})
+        Timestamp.fromdict({"start": 2.0, "end": "test"})
     assert error_msg in str(excinfo.value)
 
+
 def test_timestamp_to_dict():
     timestamp = Timestamp(start=2.0, end=3.0).to_dict()
-    assert timestamp['start'] == 2.0
-    assert timestamp['end'] == 3.0
+    assert timestamp["start"] == 2.0
+    assert timestamp["end"] == 3.0
+
 
 # Process Text Request Tests
 def test_process_text_request_default_initializer():
-    process_text_request = ProcessTextRequest(text = ['hey'])
-    assert process_text_request.text == ['hey']
+    process_text_request = ProcessTextRequest(text=["hey"])
+    assert process_text_request.text == ["hey"]
     assert process_text_request.link_batch == False
     assert type(process_text_request.entity_detection) == EntityDetection
     assert type(process_text_request.processed_text) == ProcessedText
 
+
 def test_process_text_request_initializer():
-    text = ['hey!']
+    text = ["hey!"]
     link_batch = True
-    entity_type = EntityTypeSelector(type="ENABLE", value=['NAME'])
-    filter = FilterSelector(type='ALLOW', pattern='hey')
-    entity_detection = EntityDetection(accuracy='standard', entity_types=[entity_type], filter=[filter], return_entity=False)
-    processed_text = ProcessedText(type='MARKER', pattern='BEST_ENTITY_TYPE')
-    
-    process_text_request = ProcessTextRequest(text=text, link_batch=link_batch, entity_detection=entity_detection, processed_text=processed_text)
+    entity_type = EntityTypeSelector(type="ENABLE", value=["NAME"])
+    filter = FilterSelector(type="ALLOW", pattern="hey")
+    entity_detection = EntityDetection(
+        accuracy="standard",
+        entity_types=[entity_type],
+        filter=[filter],
+        return_entity=False,
+    )
+    processed_text = ProcessedText(type="MARKER", pattern="BEST_ENTITY_TYPE")
+
+    process_text_request = ProcessTextRequest(
+        text=text,
+        link_batch=link_batch,
+        entity_detection=entity_detection,
+        processed_text=processed_text,
+    )
 
     assert process_text_request.text == text
     assert process_text_request.link_batch == link_batch
     assert process_text_request.entity_detection.accuracy == entity_detection.accuracy
-    assert process_text_request.entity_detection.entity_types[0].type == entity_type.type
-    assert process_text_request.entity_detection.entity_types[0].value == entity_type.value
+    assert (
+        process_text_request.entity_detection.entity_types[0].type == entity_type.type
+    )
+    assert (
+        process_text_request.entity_detection.entity_types[0].value == entity_type.value
+    )
     assert process_text_request.entity_detection.filter[0].type == filter.type
     assert process_text_request.entity_detection.filter[0].pattern == filter.pattern
     assert process_text_request.processed_text.type == processed_text.type
     assert process_text_request.processed_text.pattern == processed_text.pattern
 
+
 def test_process_text_request_initialize_fromdict():
     request_obj = {
         "text": ["hey!"],
         "link_batch": False,
-        "entity_detection": {"accuracy":"standard",
-                             "entity_types": [{"type": "DISABLE", "value":["LOCATION"]}],
-                             "filter": [{"type": "BLOCK", "pattern": "Roger"}],
-                             "return_entity": False
+        "entity_detection": {
+            "accuracy": "standard",
+            "entity_types": [{"type": "DISABLE", "value": ["LOCATION"]}],
+            "filter": [{"type": "BLOCK", "pattern": "Roger"}],
+            "return_entity": False,
         },
-        "processed_text": {
-            "type": "MARKER",
-            "pattern": "ALL_ENTITY_TYPES"
-        }
+        "processed_text": {"type": "MARKER", "pattern": "ALL_ENTITY_TYPES"},
     }
     process_text_request = ProcessTextRequest.fromdict(request_obj)
     assert process_text_request.text == request_obj["text"]
     assert process_text_request.link_batch == request_obj["link_batch"]
-    assert process_text_request.entity_detection.accuracy == request_obj["entity_detection"]["accuracy"]
-    assert process_text_request.entity_detection.entity_types[0].type == request_obj["entity_detection"]["entity_types"][0]["type"]
-    assert process_text_request.entity_detection.entity_types[0].value == request_obj["entity_detection"]["entity_types"][0]["value"]
-    assert process_text_request.entity_detection.filter[0].type == request_obj["entity_detection"]["filter"][0]["type"]
-    assert process_text_request.entity_detection.filter[0].pattern == request_obj["entity_detection"]["filter"][0]["pattern"]
-    assert process_text_request.processed_text.type == request_obj["processed_text"]["type"]
-    assert process_text_request.processed_text.pattern == request_obj["processed_text"]["pattern"]
+    assert (
+        process_text_request.entity_detection.accuracy
+        == request_obj["entity_detection"]["accuracy"]
+    )
+    assert (
+        process_text_request.entity_detection.entity_types[0].type
+        == request_obj["entity_detection"]["entity_types"][0]["type"]
+    )
+    assert (
+        process_text_request.entity_detection.entity_types[0].value
+        == request_obj["entity_detection"]["entity_types"][0]["value"]
+    )
+    assert (
+        process_text_request.entity_detection.filter[0].type
+        == request_obj["entity_detection"]["filter"][0]["type"]
+    )
+    assert (
+        process_text_request.entity_detection.filter[0].pattern
+        == request_obj["entity_detection"]["filter"][0]["pattern"]
+    )
+    assert (
+        process_text_request.processed_text.type
+        == request_obj["processed_text"]["type"]
+    )
+    assert (
+        process_text_request.processed_text.pattern
+        == request_obj["processed_text"]["pattern"]
+    )
+
 
 def test_process_text_request_invalid_initialize_fromdict():
     error_msg = "ProcessTextRequest can only accept the values 'text', 'link_batch', 'entity_detection' and 'process_text'"
     request_obj = {
         "text": ["hey!"],
         "link_batch": False,
-        "entity_detection": {"accuracy":"standard",
-                             "entity_types": [{"type": "DISABLE", "value":["LOCATION"]}],
-                             "filter": [{"type": "BLOCK", "pattern": "Roger"}],
-                             "return_entity": False
-        },
-        "processed_text": {
-            "type": "MARKER",
-            "pattern": "ALL_ENTITY_TYPES"
+        "entity_detection": {
+            "accuracy": "standard",
+            "entity_types": [{"type": "DISABLE", "value": ["LOCATION"]}],
+            "filter": [{"type": "BLOCK", "pattern": "Roger"}],
+            "return_entity": False,
         },
-        "junk": "value"
+        "processed_text": {"type": "MARKER", "pattern": "ALL_ENTITY_TYPES"},
+        "junk": "value",
     }
     with pytest.raises(TypeError) as excinfo:
         ProcessTextRequest.fromdict(request_obj)
     assert error_msg in str(excinfo.value)
 
+
 def test_process_text_request_to_dict():
-    text = ['hey!']
+    text = ["hey!"]
     link_batch = True
-    entity_type = EntityTypeSelector(type="ENABLE", value=['NAME'])
-    filter = FilterSelector(type='ALLOW', pattern='hey')
-    entity_detection = EntityDetection(accuracy='standard', entity_types=[entity_type], filter=[filter], return_entity=False)
-    processed_text = ProcessedText(type='MARKER', pattern='BEST_ENTITY_TYPE')
-    
-    process_text_request = ProcessTextRequest(text=text, link_batch=link_batch, entity_detection=entity_detection, processed_text=processed_text).to_dict()
+    entity_type = EntityTypeSelector(type="ENABLE", value=["NAME"])
+    filter = FilterSelector(type="ALLOW", pattern="hey")
+    entity_detection = EntityDetection(
+        accuracy="standard",
+        entity_types=[entity_type],
+        filter=[filter],
+        return_entity=False,
+    )
+    processed_text = ProcessedText(type="MARKER", pattern="BEST_ENTITY_TYPE")
+
+    process_text_request = ProcessTextRequest(
+        text=text,
+        link_batch=link_batch,
+        entity_detection=entity_detection,
+        processed_text=processed_text,
+    ).to_dict()
     print(process_text_request)
     assert process_text_request["text"] == text
     assert process_text_request["link_batch"] == link_batch
-    assert process_text_request["entity_detection"]["accuracy"] == entity_detection.accuracy
-    assert process_text_request["entity_detection"]["entity_types"][0]["type"] == entity_type.type
-    assert process_text_request["entity_detection"]["entity_types"][0]["value"] == entity_type.value
+    assert (
+        process_text_request["entity_detection"]["accuracy"]
+        == entity_detection.accuracy
+    )
+    assert (
+        process_text_request["entity_detection"]["entity_types"][0]["type"]
+        == entity_type.type
+    )
+    assert (
+        process_text_request["entity_detection"]["entity_types"][0]["value"]
+        == entity_type.value
+    )
     assert process_text_request["entity_detection"]["filter"][0]["type"] == filter.type
-    assert process_text_request["entity_detection"]["filter"][0]["pattern"] == filter.pattern
+    assert (
+        process_text_request["entity_detection"]["filter"][0]["pattern"]
+        == filter.pattern
+    )
     assert process_text_request["processed_text"]["type"] == processed_text.type
     assert process_text_request["processed_text"]["pattern"] == processed_text.pattern
 
+
 # Process File URI Request Tests
 def test_process_file_uri_request_default_initializer():
     process_file_uri_obj = ProcessFileUriRequest(uri="this/location/right/here.png")
     assert process_file_uri_obj.uri == "this/location/right/here.png"
     assert type(process_file_uri_obj.entity_detection) is EntityDetection
     assert type(process_file_uri_obj.pdf_options) is PDFOptions
     assert type(process_file_uri_obj.audio_options) is AudioOptions
 
+
 def test_process_file_uri_request_initializer():
-    entity_type = EntityTypeSelector(type="ENABLE", value=['NAME'])
-    filter = FilterSelector(type='ALLOW', pattern='hey')
-    entity_detection = EntityDetection(accuracy='standard', entity_types=[entity_type], filter=[filter], return_entity=False)
+    entity_type = EntityTypeSelector(type="ENABLE", value=["NAME"])
+    filter = FilterSelector(type="ALLOW", pattern="hey")
+    entity_detection = EntityDetection(
+        accuracy="standard",
+        entity_types=[entity_type],
+        filter=[filter],
+        return_entity=False,
+    )
     pdf_options = PDFOptions(density=100)
     audio_options = AudioOptions(bleep_start_padding=1, bleep_end_padding=2)
-    process_file_uri_obj = ProcessFileUriRequest(uri="this/location/right/here.png", entity_detection=entity_detection, pdf_options=pdf_options, audio_options=audio_options)
+    process_file_uri_obj = ProcessFileUriRequest(
+        uri="this/location/right/here.png",
+        entity_detection=entity_detection,
+        pdf_options=pdf_options,
+        audio_options=audio_options,
+    )
     assert process_file_uri_obj.uri == "this/location/right/here.png"
-    assert process_file_uri_obj.entity_detection.accuracy == 'standard'
+    assert process_file_uri_obj.entity_detection.accuracy == "standard"
     assert process_file_uri_obj.pdf_options.density == 100
     assert process_file_uri_obj.audio_options.bleep_end_padding == 2
 
+
 def test_process_file_uri_request_initialize_fromdict():
-    entity_type = EntityTypeSelector(type="ENABLE", value=['NAME'])
-    filter = FilterSelector(type='ALLOW', pattern='hey')
-    entity_detection = EntityDetection(accuracy='standard', entity_types=[entity_type], filter=[filter], return_entity=False)
+    entity_type = EntityTypeSelector(type="ENABLE", value=["NAME"])
+    filter = FilterSelector(type="ALLOW", pattern="hey")
+    entity_detection = EntityDetection(
+        accuracy="standard",
+        entity_types=[entity_type],
+        filter=[filter],
+        return_entity=False,
+    )
     pdf_options = PDFOptions(density=100)
     audio_options = AudioOptions(bleep_start_padding=1, bleep_end_padding=2)
-    process_file_uri_obj = ProcessFileUriRequest.fromdict({"uri":"this/location/right/here.png", "entity_detection":entity_detection.to_dict(), "pdf_options":pdf_options.to_dict(), "audio_options":audio_options.to_dict()})
+    process_file_uri_obj = ProcessFileUriRequest.fromdict(
+        {
+            "uri": "this/location/right/here.png",
+            "entity_detection": entity_detection.to_dict(),
+            "pdf_options": pdf_options.to_dict(),
+            "audio_options": audio_options.to_dict(),
+        }
+    )
     assert process_file_uri_obj.uri == "this/location/right/here.png"
-    assert process_file_uri_obj.entity_detection.accuracy == 'standard'
+    assert process_file_uri_obj.entity_detection.accuracy == "standard"
     assert process_file_uri_obj.pdf_options.density == 100
     assert process_file_uri_obj.audio_options.bleep_end_padding == 2
 
+
 def test_process_file_uri_request_invalid_initialize_fromdict():
     error_msg = "ProcessFileUriRequest can only accept the values 'uri', 'entity_detection', 'pdf_options and 'audio_options'"
-    entity_type = EntityTypeSelector(type="ENABLE", value=['NAME'])
-    filter = FilterSelector(type='ALLOW', pattern='hey')
-    entity_detection = EntityDetection(accuracy='standard', entity_types=[entity_type], filter=[filter], return_entity=False)
+    entity_type = EntityTypeSelector(type="ENABLE", value=["NAME"])
+    filter = FilterSelector(type="ALLOW", pattern="hey")
+    entity_detection = EntityDetection(
+        accuracy="standard",
+        entity_types=[entity_type],
+        filter=[filter],
+        return_entity=False,
+    )
     pdf_options = PDFOptions(density=100)
     audio_options = AudioOptions(bleep_start_padding=1, bleep_end_padding=2)
     with pytest.raises(TypeError) as excinfo:
-        ProcessFileUriRequest.fromdict({"uri":"this/location/right/here.png", "entity_detection":entity_detection.to_dict(), "pdf_options":pdf_options.to_dict(), "audio_options":audio_options.to_dict(), "junk": "value"})
+        ProcessFileUriRequest.fromdict(
+            {
+                "uri": "this/location/right/here.png",
+                "entity_detection": entity_detection.to_dict(),
+                "pdf_options": pdf_options.to_dict(),
+                "audio_options": audio_options.to_dict(),
+                "junk": "value",
+            }
+        )
     assert error_msg in str(excinfo.value)
 
 
 def test_process_file_uri_request_to_dict():
-    entity_type = EntityTypeSelector(type="ENABLE", value=['NAME'])
-    filter = FilterSelector(type='ALLOW', pattern='hey')
-    entity_detection = EntityDetection(accuracy='standard', entity_types=[entity_type], filter=[filter], return_entity=False)
+    entity_type = EntityTypeSelector(type="ENABLE", value=["NAME"])
+    filter = FilterSelector(type="ALLOW", pattern="hey")
+    entity_detection = EntityDetection(
+        accuracy="standard",
+        entity_types=[entity_type],
+        filter=[filter],
+        return_entity=False,
+    )
     pdf_options = PDFOptions(density=100)
     audio_options = AudioOptions(bleep_start_padding=1, bleep_end_padding=2)
-    process_file_uri_obj = ProcessFileUriRequest(uri="this/location/right/here.png", entity_detection=entity_detection, pdf_options=pdf_options, audio_options=audio_options).to_dict()
+    process_file_uri_obj = ProcessFileUriRequest(
+        uri="this/location/right/here.png",
+        entity_detection=entity_detection,
+        pdf_options=pdf_options,
+        audio_options=audio_options,
+    ).to_dict()
     assert process_file_uri_obj["uri"] == "this/location/right/here.png"
-    assert process_file_uri_obj["entity_detection"]["accuracy"] == 'standard'
+    assert process_file_uri_obj["entity_detection"]["accuracy"] == "standard"
     assert process_file_uri_obj["pdf_options"]["density"] == 100
     assert process_file_uri_obj["audio_options"]["bleep_end_padding"] == 2
 
+
 # Process File Base64 Request Tests
 def test_process_file_base64_request_default_initializer():
-    process_file_base64_request_obj = ProcessFileBase64Request(file="sfsfxe234jkjsdlkfnDATA!!!!!!")
+    process_file_base64_request_obj = ProcessFileBase64Request(
+        file="sfsfxe234jkjsdlkfnDATA!!!!!!"
+    )
     assert process_file_base64_request_obj.file == "sfsfxe234jkjsdlkfnDATA!!!!!!"
     assert type(process_file_base64_request_obj.entity_detection) is EntityDetection
     assert type(process_file_base64_request_obj.pdf_options) is PDFOptions
     assert type(process_file_base64_request_obj.audio_options) is AudioOptions
 
+
 def test_process_file_base64_request_initializer():
-    entity_type = EntityTypeSelector(type="ENABLE", value=['NAME'])
-    filter = FilterSelector(type='ALLOW', pattern='hey')
-    entity_detection = EntityDetection(accuracy='standard', entity_types=[entity_type], filter=[filter], return_entity=False)
+    entity_type = EntityTypeSelector(type="ENABLE", value=["NAME"])
+    filter = FilterSelector(type="ALLOW", pattern="hey")
+    entity_detection = EntityDetection(
+        accuracy="standard",
+        entity_types=[entity_type],
+        filter=[filter],
+        return_entity=False,
+    )
     pdf_options = PDFOptions(density=100)
     audio_options = AudioOptions(bleep_start_padding=1, bleep_end_padding=2)
-    process_file_base64_request_obj = ProcessFileBase64Request(file="sfsfxe234jkjsdlkfnDATA", entity_detection=entity_detection, pdf_options=pdf_options, audio_options=audio_options)
+    process_file_base64_request_obj = ProcessFileBase64Request(
+        file="sfsfxe234jkjsdlkfnDATA",
+        entity_detection=entity_detection,
+        pdf_options=pdf_options,
+        audio_options=audio_options,
+    )
     assert process_file_base64_request_obj.file == "sfsfxe234jkjsdlkfnDATA"
-    assert process_file_base64_request_obj.entity_detection.accuracy == 'standard'
+    assert process_file_base64_request_obj.entity_detection.accuracy == "standard"
     assert process_file_base64_request_obj.pdf_options.density == 100
     assert process_file_base64_request_obj.audio_options.bleep_end_padding == 2
 
+
 def test_process_file_base64_request_initialize_fromdict():
     file = File(data="sfsfxe234jkjsdlkfnDATA", content_type="application/pdf")
-    entity_type = EntityTypeSelector(type="ENABLE", value=['NAME'])
-    filter = FilterSelector(type='ALLOW', pattern='hey')
-    entity_detection = EntityDetection(accuracy='standard', entity_types=[entity_type], filter=[filter], return_entity=False)
+    entity_type = EntityTypeSelector(type="ENABLE", value=["NAME"])
+    filter = FilterSelector(type="ALLOW", pattern="hey")
+    entity_detection = EntityDetection(
+        accuracy="standard",
+        entity_types=[entity_type],
+        filter=[filter],
+        return_entity=False,
+    )
     pdf_options = PDFOptions(density=100)
     audio_options = AudioOptions(bleep_start_padding=1, bleep_end_padding=2)
-    process_file_base64_request_obj = ProcessFileBase64Request.fromdict({"file":file.to_dict(), "entity_detection":entity_detection.to_dict(), "pdf_options":pdf_options.to_dict(), "audio_options":audio_options.to_dict()})
+    process_file_base64_request_obj = ProcessFileBase64Request.fromdict(
+        {
+            "file": file.to_dict(),
+            "entity_detection": entity_detection.to_dict(),
+            "pdf_options": pdf_options.to_dict(),
+            "audio_options": audio_options.to_dict(),
+        }
+    )
     assert process_file_base64_request_obj.file.data == "sfsfxe234jkjsdlkfnDATA"
-    assert process_file_base64_request_obj.entity_detection.accuracy == 'standard'
+    assert process_file_base64_request_obj.entity_detection.accuracy == "standard"
     assert process_file_base64_request_obj.pdf_options.density == 100
     assert process_file_base64_request_obj.audio_options.bleep_end_padding == 2
 
+
 def test_process_file_base64_request_invalid_initialize_fromdict():
     error_msg = "ProcessFileBase64Request can only accept the values 'file', 'entity_detection', 'pdf_options and 'audio_options'"
     file = File(data="sfsfxe234jkjsdlkfnDATA", content_type="application/pdf")
-    entity_type = EntityTypeSelector(type="ENABLE", value=['NAME'])
-    filter = FilterSelector(type='ALLOW', pattern='hey')
-    entity_detection = EntityDetection(accuracy='standard', entity_types=[entity_type], filter=[filter], return_entity=False)
+    entity_type = EntityTypeSelector(type="ENABLE", value=["NAME"])
+    filter = FilterSelector(type="ALLOW", pattern="hey")
+    entity_detection = EntityDetection(
+        accuracy="standard",
+        entity_types=[entity_type],
+        filter=[filter],
+        return_entity=False,
+    )
     pdf_options = PDFOptions(density=100)
     audio_options = AudioOptions(bleep_start_padding=1, bleep_end_padding=2)
     with pytest.raises(TypeError) as excinfo:
-        ProcessFileBase64Request.fromdict({"file":file.to_dict(), "entity_detection":entity_detection.to_dict(), "pdf_options":pdf_options.to_dict(), "audio_options":audio_options.to_dict(), "junk":"value"})    
+        ProcessFileBase64Request.fromdict(
+            {
+                "file": file.to_dict(),
+                "entity_detection": entity_detection.to_dict(),
+                "pdf_options": pdf_options.to_dict(),
+                "audio_options": audio_options.to_dict(),
+                "junk": "value",
+            }
+        )
     assert error_msg in str(excinfo.value)
 
 
 def test_process_file_base64_request_to_dict():
-    entity_type = EntityTypeSelector(type="ENABLE", value=['NAME'])
-    filter = FilterSelector(type='ALLOW', pattern='hey')
-    entity_detection = EntityDetection(accuracy='standard', entity_types=[entity_type], filter=[filter], return_entity=False)
+    entity_type = EntityTypeSelector(type="ENABLE", value=["NAME"])
+    filter = FilterSelector(type="ALLOW", pattern="hey")
+    entity_detection = EntityDetection(
+        accuracy="standard",
+        entity_types=[entity_type],
+        filter=[filter],
+        return_entity=False,
+    )
     pdf_options = PDFOptions(density=100)
     audio_options = AudioOptions(bleep_start_padding=1, bleep_end_padding=2)
-    process_file_base64_request_obj = ProcessFileBase64Request(file="sfsfxe234jkjsdlkfnDATA", entity_detection=entity_detection, pdf_options=pdf_options, audio_options=audio_options).to_dict()
+    process_file_base64_request_obj = ProcessFileBase64Request(
+        file="sfsfxe234jkjsdlkfnDATA",
+        entity_detection=entity_detection,
+        pdf_options=pdf_options,
+        audio_options=audio_options,
+    ).to_dict()
     assert process_file_base64_request_obj["file"] == "sfsfxe234jkjsdlkfnDATA"
-    assert process_file_base64_request_obj["entity_detection"]["accuracy"] == 'standard'
+    assert process_file_base64_request_obj["entity_detection"]["accuracy"] == "standard"
     assert process_file_base64_request_obj["pdf_options"]["density"] == 100
     assert process_file_base64_request_obj["audio_options"]["bleep_end_padding"] == 2
 
+
 # Bleep Request Tests
 def test_bleep_request_initializer():
-    file=File(data="test", content_type="image/jpg")
-    timestamps=[Timestamp(start=0.0, end=1.0)]
+    file = File(data="test", content_type="image/jpg")
+    timestamps = [Timestamp(start=0.0, end=1.0)]
     bleep_request = BleepRequest(file=file, timestamps=timestamps)
-    assert bleep_request.file.data == 'test'
+    assert bleep_request.file.data == "test"
     assert bleep_request.timestamps[0].start == 0
 
+
 def test_bleep_request_initialize_fromdict():
-    file=File(data="test", content_type="image/jpg")
-    timestamps=[Timestamp(start=0.0, end=1.0)]
-    bleep_request = BleepRequest.fromdict({"file":file.to_dict(), "timestamps":[row.to_dict() for row in timestamps]})
-    assert bleep_request.file.data == 'test'
+    file = File(data="test", content_type="image/jpg")
+    timestamps = [Timestamp(start=0.0, end=1.0)]
+    bleep_request = BleepRequest.fromdict(
+        {"file": file.to_dict(), "timestamps": [row.to_dict() for row in timestamps]}
+    )
+    assert bleep_request.file.data == "test"
     assert bleep_request.timestamps[0].start == 0
 
+
 def test_bleep_request_invalid_initialize_fromdict():
     error_msg = "BleepRequest can only accept the values 'file'and 'timestamps'"
-    file=File(data="test", content_type="image/jpg")
-    timestamps=[Timestamp(start=0.0, end=1.0)]
+    file = File(data="test", content_type="image/jpg")
+    timestamps = [Timestamp(start=0.0, end=1.0)]
     with pytest.raises(TypeError) as excinfo:
-        BleepRequest.fromdict({"file":file.to_dict(), "timestamps":[row.to_dict() for row in timestamps], "junk": "value"})
+        BleepRequest.fromdict(
+            {
+                "file": file.to_dict(),
+                "timestamps": [row.to_dict() for row in timestamps],
+                "junk": "value",
+            }
+        )
     assert error_msg in str(excinfo.value)
 
+
 def test_bleep_request_to_dict():
-    file=File(data="test", content_type="image/jpg")
-    timestamps=[Timestamp(start=0.0, end=1.0)]
+    file = File(data="test", content_type="image/jpg")
+    timestamps = [Timestamp(start=0.0, end=1.0)]
     bleep_request = BleepRequest(file=file, timestamps=timestamps).to_dict()
-    assert bleep_request["file"]["data"] == 'test'
+    assert bleep_request["file"]["data"] == "test"
     assert bleep_request["timestamps"][0]["start"] == 0
-    
+
+
+# Reidentify Text Request Tests
+def test_reidentify_text_request_initializer():
+    processed_text = ["this is a test"]
+    entities = [Entity(processed_text="NAME", text="Hola")]
+    model = "gpt-700.2-ultra-turbo"
+    reid = ReidentifyTextRequest(
+        processed_text=processed_text, entities=entities, model=model
+    )
+    assert reid.processed_text == ["this is a test"]
+    assert reid.entities[0].text == "Hola"
+    assert reid.model == "gpt-700.2-ultra-turbo"
+
+
+def test_reidentify_text_request_initialize_fromdict():
+    processed_text = ["this is a test"]
+    entities = [Entity(processed_text="NAME", text="Hola")]
+    model = "gpt-700.2-ultra-turbo"
+    reid = ReidentifyTextRequest.fromdict(
+        {
+            "processed_text": processed_text,
+            "entities": [row.to_dict() for row in entities],
+            "model": model,
+        }
+    )
+    assert reid.processed_text == ["this is a test"]
+    assert reid.entities[0].text == "Hola"
+    assert reid.model == "gpt-700.2-ultra-turbo"
+
+
+def test_reidentify_text_request_invalid_initialize_fromdict():
+    error_msg = "ReidentifyTextRequest can only accept the values 'processed_text', 'entities' and 'model"
+    processed_text = ["this is a test"]
+    entities = [Entity(processed_text="NAME", text="Hola")]
+    model = "gpt-700.2-ultra-turbo"
+    with pytest.raises(TypeError) as excinfo:
+        ReidentifyTextRequest.fromdict(
+            {
+                "processed_text": processed_text,
+                "entities": [row.to_dict() for row in entities],
+                "model": model,
+                "junk": "value",
+            }
+        )
+        assert error_msg in str(excinfo.value)
+
+
+def test_reidentify_text_request_to_dict():
+    processed_text = ["this is a test"]
+    entities = [Entity(processed_text="NAME", text="Hola")]
+    model = "gpt-700.2-ultra-turbo"
+    reid = ReidentifyTextRequest(
+        processed_text=processed_text, entities=entities, model=model
+    ).to_dict()
+    assert reid["processed_text"][0] == "this is a test"
+    assert reid["entities"][0]["text"] == "Hola"
+    assert reid["model"] == "gpt-700.2-ultra-turbo"
+
+
+def test_synthetic_text():
+    processed_text = ProcessedText(
+        type="SYNTHETIC",
+        synthetic_entity_accuracy="standard",
+        preserve_relationships=True,
+    )
+    assert processed_text.type == "SYNTHETIC"
+    assert hasattr(processed_text, "pattern") == False
+
+
+def test_change_type():
+    processed_text = ProcessedText(
+        type="MARKER", pattern="UNIQUE_NUMBERED_ENTITY_TYPE"
+    )  # Marker
+    processed_text.type = "MASK"
+    assert processed_text.type == "MASK"
+    assert hasattr(processed_text, "pattern") == False
+    assert processed_text.mask_character == "#"
+
+
+def test_mask_invalid_mask_character_initialize():
+    error_msg = "mask_character must have only one character."
+    with pytest.raises(ValueError) as excinfo:
+        processed_text = ProcessedText(type="MASK", mask_character="invalid")
+    assert error_msg in str(excinfo.value)
+
+
+def test_mask_invalid_mask_character():
+    error_msg = "mask_character must have only one character."
+    processed_text = ProcessedText()
+    processed_text.type = "MASK"
+    assert processed_text.type == "MASK"
+    with pytest.raises(ValueError) as excinfo:
+        processed_text.mask_character = "invalid"
+    assert error_msg in str(excinfo.value)
+
+
+def test_synthetic_invalid_accuracy_initialize():
+    error_msg = "Synthetic Entity Accuracy can only accept values"
+    with pytest.raises(ValueError) as excinfo:
+        processed_text = ProcessedText(
+            type="SYNTHETIC",
+            synthetic_entity_accuracy="invalid",
+            preserve_relationships=True,
+        )
+    assert error_msg in str(excinfo.value)
+
+
+def test_synthetic_invalid_accuracy():
+    error_msg = "Synthetic Entity Accuracy can only accept values"
+    processed_text = ProcessedText(
+        type="SYNTHETIC",
+        preserve_relationships=True,
+    )
+    with pytest.raises(ValueError) as excinfo:
+        processed_text.synthetic_entity_accuracy = "invalid"
+    assert error_msg in str(excinfo.value)
```

### Comparing `privateai_client-1.1.0/LICENSE` & `privateai_client-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `privateai_client-1.1.0/README.md` & `privateai_client-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -182,15 +182,15 @@
 
 ```
 ["This is John Smith's sample process text object request where names won't be removed"]
 ```
 
 #### Building Request Objects
 
-Request objects can initialized by passing in all the required values needed for the request as arguments or from a dictionary, using the object's `fromdict` function:
+Request objects can initialized by passing in all the required values needed for the request as arguments or from a dictionary, using the object's `fromdict` function. Any object can be created as per the [Private AI documentation][1].
 
 ```python
 # Passing arguments
 sample_data = "JVBERi0xLjQKJdPr6eEKMSAwIG9iago8PC9UaXRsZSAoc2FtcGxlKQovUHJvZHVj..."
 sample_content_type = "application/pdf"
 
 sample_file_obj = request_objects.file_obj(data=sample_data, content_type=sample_content_type)
@@ -204,31 +204,37 @@
 
 Request objects also can be formatted as dictionaries, using the request object's `to_dict()` function:
 
 ```python
 from privateai_client import request_objects
 
 sample_text = "Sample text."
+sample_accuracy = "standard"
+
 # Create the nested request objects
 sample_entity_type_selector = request_objects.entity_type_selector_obj(type="DISABLE", value=['HIPAA'])
-sample_entity_detection = request_objects.entity_detection_obj(entity_types=[sample_entity_type_selector])
+sample_entity_detection = request_objects.entity_detection_obj(
+    entity_types=[sample_entity_type_selector],
+    accuracy=sample_accuracy
+)
+
 # Create the request object
 sample_request = request_objects.process_text_obj(text=[sample_text], entity_detection=sample_entity_detection)
 
 # All nested request objects are also formatted
 print(sample_request.to_dict())
 ```
 
 Output:
 
 ```
 {
  'text': ['Sample text.'],
  'link_batch': False,
- 'entity_detection': {'accuracy': 'high', 'entity_types': [{'type': 'DISABLE', 'value': ['HIPAA']}], 'filter': [], 'return_entity': True},
+ 'entity_detection': {'accuracy': 'standard', 'entity_types': [{'type': 'DISABLE', 'value': ['HIPAA']}], 'filter': [], 'return_entity': True},
  'processed_text': {'type': 'MARKER', 'pattern': '[UNIQUE_NUMBERED_ENTITY_TYPE]'}
 }
 ```
 
 ### Sample Use <a name=sample-use></a>
 
 #### Processing a directory of files
@@ -384,8 +390,32 @@
     }
 )
 obj = request_objects.process_text_obj
 func = client.process_text
 data_frame['text'] = [(lambda x: func(obj(text=[x])).processed_text[0])(row) for row in data_frame['text']]
 ```
 
+Reidentifying Text
+```python
+from privateai_client import PAIClient
+from privateai_client import request_objects
+
+client = PAIClient("http", "localhost", "8080")
+
+# Deidentify the text
+initial_text = 'My name is John. I work for Private AI'
+request_obj = request_objects.process_text_obj(text=[initial_text])
+response_obj = client.process_text(request_obj)
+
+# Store the response data
+deidentified_text = response_obj.processed_text
+print(deidentified_text)
+entity_list = [request_objects.entity(row['processed_text'], row['text']) for row in response_obj.entities]
+print([row.to_dict() for row in entity_list])
+
+# # Call the reidentify Route
+request_obj = request_objects.reidentify_text_obj(processed_text=[deidentified_text], entities=entity_list)
+response_obj = client.reidentify_text(request_obj)
+print(response_obj.body)
+```
+
 [1]: https://docs.private-ai.com/reference/latest/operation/process_text_v3_process_text_post/
```

### Comparing `privateai_client-1.1.0/pyproject.toml` & `privateai_client-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "privateai_client"
-version = "1.1.0"
+version = "1.2.0"
 authors = [
   { name="Adam Guiducci", email="adam.guiducci@private-ai.com" },
   { name="Bryan Bell-Smith", email="bryan.bellsmith@private-ai.com" },
 ]
 description = "A thin client for communicating with the Private AI de-identication API."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -17,7 +17,8 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/privateai/pai-thin-client/"
 "Bug Tracker" = "https://github.com/privateai/pai-thin-client/issues"
+
```

### Comparing `privateai_client-1.1.0/PKG-INFO` & `privateai_client-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: privateai_client
-Version: 1.1.0
+Version: 1.2.0
 Summary: A thin client for communicating with the Private AI de-identication API.
 Project-URL: Homepage, https://github.com/privateai/pai-thin-client/
 Project-URL: Bug Tracker, https://github.com/privateai/pai-thin-client/issues
 Author-email: Adam Guiducci <adam.guiducci@private-ai.com>, Bryan Bell-Smith <bryan.bellsmith@private-ai.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -196,15 +196,15 @@
 
 ```
 ["This is John Smith's sample process text object request where names won't be removed"]
 ```
 
 #### Building Request Objects
 
-Request objects can initialized by passing in all the required values needed for the request as arguments or from a dictionary, using the object's `fromdict` function:
+Request objects can initialized by passing in all the required values needed for the request as arguments or from a dictionary, using the object's `fromdict` function. Any object can be created as per the [Private AI documentation][1].
 
 ```python
 # Passing arguments
 sample_data = "JVBERi0xLjQKJdPr6eEKMSAwIG9iago8PC9UaXRsZSAoc2FtcGxlKQovUHJvZHVj..."
 sample_content_type = "application/pdf"
 
 sample_file_obj = request_objects.file_obj(data=sample_data, content_type=sample_content_type)
@@ -218,31 +218,37 @@
 
 Request objects also can be formatted as dictionaries, using the request object's `to_dict()` function:
 
 ```python
 from privateai_client import request_objects
 
 sample_text = "Sample text."
+sample_accuracy = "standard"
+
 # Create the nested request objects
 sample_entity_type_selector = request_objects.entity_type_selector_obj(type="DISABLE", value=['HIPAA'])
-sample_entity_detection = request_objects.entity_detection_obj(entity_types=[sample_entity_type_selector])
+sample_entity_detection = request_objects.entity_detection_obj(
+    entity_types=[sample_entity_type_selector],
+    accuracy=sample_accuracy
+)
+
 # Create the request object
 sample_request = request_objects.process_text_obj(text=[sample_text], entity_detection=sample_entity_detection)
 
 # All nested request objects are also formatted
 print(sample_request.to_dict())
 ```
 
 Output:
 
 ```
 {
  'text': ['Sample text.'],
  'link_batch': False,
- 'entity_detection': {'accuracy': 'high', 'entity_types': [{'type': 'DISABLE', 'value': ['HIPAA']}], 'filter': [], 'return_entity': True},
+ 'entity_detection': {'accuracy': 'standard', 'entity_types': [{'type': 'DISABLE', 'value': ['HIPAA']}], 'filter': [], 'return_entity': True},
  'processed_text': {'type': 'MARKER', 'pattern': '[UNIQUE_NUMBERED_ENTITY_TYPE]'}
 }
 ```
 
 ### Sample Use <a name=sample-use></a>
 
 #### Processing a directory of files
@@ -398,8 +404,32 @@
     }
 )
 obj = request_objects.process_text_obj
 func = client.process_text
 data_frame['text'] = [(lambda x: func(obj(text=[x])).processed_text[0])(row) for row in data_frame['text']]
 ```
 
+Reidentifying Text
+```python
+from privateai_client import PAIClient
+from privateai_client import request_objects
+
+client = PAIClient("http", "localhost", "8080")
+
+# Deidentify the text
+initial_text = 'My name is John. I work for Private AI'
+request_obj = request_objects.process_text_obj(text=[initial_text])
+response_obj = client.process_text(request_obj)
+
+# Store the response data
+deidentified_text = response_obj.processed_text
+print(deidentified_text)
+entity_list = [request_objects.entity(row['processed_text'], row['text']) for row in response_obj.entities]
+print([row.to_dict() for row in entity_list])
+
+# # Call the reidentify Route
+request_obj = request_objects.reidentify_text_obj(processed_text=[deidentified_text], entities=entity_list)
+response_obj = client.reidentify_text(request_obj)
+print(response_obj.body)
+```
+
 [1]: https://docs.private-ai.com/reference/latest/operation/process_text_v3_process_text_post/
```

