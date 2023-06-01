# Comparing `tmp/chunked-uploads-attentive-0.0.6.tar.gz` & `tmp/chunked-uploads-attentive-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chunked-uploads-attentive-0.0.6.tar", last modified: Thu May 25 05:43:48 2023, max compression
+gzip compressed data, was "chunked-uploads-attentive-0.0.7.tar", last modified: Thu Jun  1 18:43:50 2023, max compression
```

## Comparing `chunked-uploads-attentive-0.0.6.tar` & `chunked-uploads-attentive-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 05:43:48.476237 chunked-uploads-attentive-0.0.6/
--rw-rw-rw-   0        0        0      478 2023-05-25 05:43:48.476237 chunked-uploads-attentive-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-25 05:43:48.476237 chunked-uploads-attentive-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      925 2023-05-25 05:43:44.000000 chunked-uploads-attentive-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 05:43:48.439888 chunked-uploads-attentive-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 05:43:48.460600 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/
--rw-rw-rw-   0        0        0      478 2023-05-25 05:43:48.000000 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      527 2023-05-25 05:43:48.000000 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 05:43:48.000000 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-25 05:43:48.000000 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-25 05:43:48.000000 chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 05:43:48.476237 chunked-uploads-attentive-0.0.6/src/uploads/
--rw-rw-rw-   0        0        0        0 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.6/src/uploads/__init__.py
--rw-rw-rw-   0        0        0      325 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.6/src/uploads/admin.py
--rw-rw-rw-   0        0        0      152 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.6/src/uploads/apps.py
--rw-rw-rw-   0        0        0      300 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.6/src/uploads/constants.py
--rw-rw-rw-   0        0        0      262 2023-02-13 12:36:18.000000 chunked-uploads-attentive-0.0.6/src/uploads/exceptions.py
--rw-rw-rw-   0        0        0     3853 2023-05-07 19:41:00.000000 chunked-uploads-attentive-0.0.6/src/uploads/models.py
--rw-rw-rw-   0        0        0      384 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.6/src/uploads/response.py
--rw-rw-rw-   0        0        0      578 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.6/src/uploads/serializers.py
--rw-rw-rw-   0        0        0     2417 2023-05-07 19:40:59.000000 chunked-uploads-attentive-0.0.6/src/uploads/settings.py
--rw-rw-rw-   0        0        0       63 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.6/src/uploads/tests.py
--rw-rw-rw-   0        0        0    12227 2023-05-12 19:57:30.000000 chunked-uploads-attentive-0.0.6/src/uploads/views.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:43:50.370589 chunked-uploads-attentive-0.0.7/
+-rw-rw-rw-   0        0        0      478 2023-06-01 18:43:50.367601 chunked-uploads-attentive-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-01 18:43:50.370589 chunked-uploads-attentive-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      925 2023-06-01 18:42:49.000000 chunked-uploads-attentive-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 18:43:50.323598 chunked-uploads-attentive-0.0.7/src/
+drwxrwxrwx   0        0        0        0 2023-06-01 18:43:50.333603 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/
+-rw-rw-rw-   0        0        0      478 2023-06-01 18:43:50.000000 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      527 2023-06-01 18:43:50.000000 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 18:43:50.000000 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-06-01 18:43:50.000000 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-01 18:43:50.000000 chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 18:43:50.363594 chunked-uploads-attentive-0.0.7/src/uploads/
+-rw-rw-rw-   0        0        0        0 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.7/src/uploads/__init__.py
+-rw-rw-rw-   0        0        0      325 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.7/src/uploads/admin.py
+-rw-rw-rw-   0        0        0      152 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.7/src/uploads/apps.py
+-rw-rw-rw-   0        0        0      300 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.7/src/uploads/constants.py
+-rw-rw-rw-   0        0        0      262 2023-02-13 12:36:18.000000 chunked-uploads-attentive-0.0.7/src/uploads/exceptions.py
+-rw-rw-rw-   0        0        0     3853 2023-05-07 19:41:00.000000 chunked-uploads-attentive-0.0.7/src/uploads/models.py
+-rw-rw-rw-   0        0        0      384 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.7/src/uploads/response.py
+-rw-rw-rw-   0        0        0      578 2023-04-20 11:41:44.000000 chunked-uploads-attentive-0.0.7/src/uploads/serializers.py
+-rw-rw-rw-   0        0        0     2750 2023-05-31 05:22:56.000000 chunked-uploads-attentive-0.0.7/src/uploads/settings.py
+-rw-rw-rw-   0        0        0       63 2023-03-21 15:09:06.000000 chunked-uploads-attentive-0.0.7/src/uploads/tests.py
+-rw-rw-rw-   0        0        0    12316 2023-05-31 05:23:58.000000 chunked-uploads-attentive-0.0.7/src/uploads/views.py
```

### Comparing `chunked-uploads-attentive-0.0.6/setup.py` & `chunked-uploads-attentive-0.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Chunked Upload of files on gcs using Django'
 LONG_DESCRIPTION = 'A package that allows to transfer files and resume in case of data failure'
 
 # Setting up
 setup(
     name="chunked-uploads-attentive",
     version=VERSION,
```

### Comparing `chunked-uploads-attentive-0.0.6/src/chunked_uploads_attentive.egg-info/SOURCES.txt` & `chunked-uploads-attentive-0.0.7/src/chunked_uploads_attentive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chunked-uploads-attentive-0.0.6/src/uploads/models.py` & `chunked-uploads-attentive-0.0.7/src/uploads/models.py`

 * *Files identical despite different names*

### Comparing `chunked-uploads-attentive-0.0.6/src/uploads/serializers.py` & `chunked-uploads-attentive-0.0.7/src/uploads/serializers.py`

 * *Files identical despite different names*

### Comparing `chunked-uploads-attentive-0.0.6/src/uploads/settings.py` & `chunked-uploads-attentive-0.0.7/src/uploads/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,14 +12,20 @@
         # Deprecated class name (for backwards compatibility purposes)
         from django.core.serializers.json import (
             DateTimeAwareJSONEncoder as DjangoJSONEncoder,
         )
     except ImportError:
         raise ImportError("Dude! what version of Django are you using?")
 
+def read_env(key, default=None):
+    try:
+        return os.environ[key]
+    except KeyError:
+        return default
+    
 # How long after creation the upload will expire
 DEFAULT_EXPIRATION_DELTA = timedelta(days=1)
 EXPIRATION_DELTA = getattr(
     settings, "CHUNKED_UPLOAD_EXPIRATION_DELTA", DEFAULT_EXPIRATION_DELTA
 )
 
 # Path where uploading files will be stored until completion
@@ -61,7 +67,10 @@
 # determine the "null" and "blank" properties of "user" field in the "ChunkedUpload" model
 DEFAULT_MODEL_USER_FIELD_NULL = getattr(
     settings, "CHUNKED_UPLOAD_MODEL_USER_FIELD_NULL", True
 )
 DEFAULT_MODEL_USER_FIELD_BLANK = getattr(
     settings, "CHUNKED_UPLOAD_MODEL_USER_FIELD_BLANK", True
 )
+
+GS_BUCKET_NAME = read_env('GOOGLE_CLOUD_BUCKET_NAME', 'cos-dev-filestore')
+os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = read_env('GOOGLE_APPLICATION_CREDENTIALS', "C:\\raven-356806-4358641d2512.json")
```

### Comparing `chunked-uploads-attentive-0.0.6/src/uploads/views.py` & `chunked-uploads-attentive-0.0.7/src/uploads/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import os
 from django.views.generic import View
 from django.shortcuts import get_object_or_404
 from django.core.files.base import ContentFile
 from django.utils import timezone
 import datetime
 
-from .settings import MAX_BYTES
+
+from .settings import MAX_BYTES,GS_BUCKET_NAME
 from .models import ChunkedUpload, MyChunkedUpload
 from .response import Response
 from .constants import http_status, COMPLETE
 from .exceptions import ChunkedUploadError
 
 from django.views.generic.base import TemplateView
 from uploads.serializers import ChunkedUploadSerializer
@@ -189,15 +190,15 @@
             status=http_status.HTTP_200_OK,
         )
 
 class ChunkedUploadApiViewSet(viewsets.ModelViewSet):
 
     today = timezone.localtime(timezone.now()).date()
     client = storage.Client()
-    bucket = client.get_bucket("cos-dev-filestore")
+    bucket = client.get_bucket(GS_BUCKET_NAME)
     queryset = MyChunkedUpload.objects.all()
     model = MyChunkedUpload
     serializer_class = ChunkedUploadSerializer
     CHUNK_SIZE = 262144
 
     def md5(self, file):
         """
@@ -214,14 +215,16 @@
         Takes in various chunks and stores them in a file. Also updates the database.
         """
         filename = request.data["filename"] 
         chunk_num = request.data["chunk_num"]
         chunk = request.data["chunk"]
         file_md5 = request.data['file_md5'] 
         chunk_md5 = request.data['chunk_md5']
+        self.CHUNK_SIZE = request.data.get('chunk_size', self.CHUNK_SIZE)
+
         #file_size = request.data["size"]
         if(chunk_md5 != self.md5(chunk)):
             return Response({"chunk_num" : chunk_num,"message" :"File Corrupt","status" : 2})
 
         if self.queryset.filter(file_md5=file_md5).exists():
             resume_upload = self.queryset.get(file_md5=file_md5)
             resume_serializer = ChunkedUploadSerializer(resume_upload)
```

