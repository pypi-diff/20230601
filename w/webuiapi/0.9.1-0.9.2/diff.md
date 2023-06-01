# Comparing `tmp/webuiapi-0.9.1-py3-none-any.whl.zip` & `tmp/webuiapi-0.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12615 bytes, number of entries: 7
--rw-r--r--  2.0 unx      532 b- defN 23-Jun-01 06:03 webuiapi/__init__.py
--rw-r--r--  2.0 unx    34535 b- defN 23-Jun-01 06:03 webuiapi/webuiapi.py
--rw-r--r--  2.0 unx     1079 b- defN 23-Jun-01 06:03 webuiapi-0.9.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    13529 b- defN 23-Jun-01 06:03 webuiapi-0.9.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 06:03 webuiapi-0.9.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-Jun-01 06:03 webuiapi-0.9.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      545 b- defN 23-Jun-01 06:03 webuiapi-0.9.1.dist-info/RECORD
-7 files, 50321 bytes uncompressed, 11653 bytes compressed:  76.8%
+Zip file size: 12658 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      532 b- defN 23-Jun-01 06:33 webuiapi/__init__.py
+-rw-r--r--  2.0 unx    34658 b- defN 23-Jun-01 06:33 webuiapi/webuiapi.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jun-01 06:33 webuiapi-0.9.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13529 b- defN 23-Jun-01 06:33 webuiapi-0.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 06:33 webuiapi-0.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-01 06:33 webuiapi-0.9.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      545 b- defN 23-Jun-01 06:33 webuiapi-0.9.2.dist-info/RECORD
+7 files, 50444 bytes uncompressed, 11696 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webuiapi/__init__.py
 Comment: 
 
 Filename: webuiapi/webuiapi.py
 Comment: 
 
-Filename: webuiapi-0.9.1.dist-info/LICENSE
+Filename: webuiapi-0.9.2.dist-info/LICENSE
 Comment: 
 
-Filename: webuiapi-0.9.1.dist-info/METADATA
+Filename: webuiapi-0.9.2.dist-info/METADATA
 Comment: 
 
-Filename: webuiapi-0.9.1.dist-info/WHEEL
+Filename: webuiapi-0.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: webuiapi-0.9.1.dist-info/top_level.txt
+Filename: webuiapi-0.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: webuiapi-0.9.1.dist-info/RECORD
+Filename: webuiapi-0.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## webuiapi/__init__.py

```diff
@@ -8,15 +8,15 @@
     ModelKeywordResult,
     ModelKeywordInterface,
     InstructPix2PixInterface,
     ControlNetInterface,
     ControlNetUnit,
 )
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 
 __all__ = [
     "__version__",
     "WebUIApi",
     "WebUIApiResult",
     "Upscaler",
     "HiResUpscaler",
```

## webuiapi/webuiapi.py

```diff
@@ -351,15 +351,16 @@
             response = self.session.post(url=url, json=json)
             return self._to_api_result(response)
 
     async def async_post(self, url, json):
         import aiohttp
 
         async with aiohttp.ClientSession() as session:
-            async with session.post(url, json=json) as response:
+            auth = aiohttp.BasicAuth(self.session.auth[0], self.session.auth[1]) if self.session.auth else None
+            async with session.post(url, json=json, auth=auth) as response:
                 return await self._to_api_result_async(response)
 
     def img2img(
         self,
         images=[],  # list of PIL Image
         resize_mode=0,
         denoising_strength=0.75,
```

## Comparing `webuiapi-0.9.1.dist-info/LICENSE` & `webuiapi-0.9.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webuiapi-0.9.1.dist-info/METADATA` & `webuiapi-0.9.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webuiapi
-Version: 0.9.1
+Version: 0.9.2
 Summary: Python API client for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/mix1009/sdwebuiapi
 Author: ChunKoo Park
 Author-email: mix1009@gmail.com
 License: MIT
 Keywords: stable-diffuion-webui,AUTOMATIC1111,stable-diffusion,api
 Platform: UNKNOWN
```

## Comparing `webuiapi-0.9.1.dist-info/RECORD` & `webuiapi-0.9.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-webuiapi/__init__.py,sha256=OF4mr8dzZjSTkJxCJnyuSYz0GuoOcN3S69_5c9sUJfU,532
-webuiapi/webuiapi.py,sha256=iqlWYOLw1nSAh_D9qPH4inzujnBKZXxF0yFuD54mQOc,34535
-webuiapi-0.9.1.dist-info/LICENSE,sha256=Zl3ztitjIWviypQXfHYvUR099Y5IUOh15IVxAOw9XV8,1079
-webuiapi-0.9.1.dist-info/METADATA,sha256=cY45dg8mtpAa5dKuou05VhAJ3cDS7yOTwv_iEGIpaSA,13529
-webuiapi-0.9.1.dist-info/WHEEL,sha256=_NOXIqFgOaYmlm9RJLPQZ13BJuEIrp5jx5ptRD5uh3Y,92
-webuiapi-0.9.1.dist-info/top_level.txt,sha256=84RprjAaGWFS3oujg2AE1dTHp6o4yGT9isvN6frk5p4,9
-webuiapi-0.9.1.dist-info/RECORD,,
+webuiapi/__init__.py,sha256=C_Q4u40RWL9yf3gYnSz8OynKGKq9Cvw09iPoZ0BV0Fg,532
+webuiapi/webuiapi.py,sha256=1xGdpbYCvK804MwDoBnZ3cRxqrIOPlsKYZnV-0k_aJM,34658
+webuiapi-0.9.2.dist-info/LICENSE,sha256=Zl3ztitjIWviypQXfHYvUR099Y5IUOh15IVxAOw9XV8,1079
+webuiapi-0.9.2.dist-info/METADATA,sha256=klRamkeHvizZzF8wWww2RV9BPBHEvwOpzxGNP5KFoBM,13529
+webuiapi-0.9.2.dist-info/WHEEL,sha256=_NOXIqFgOaYmlm9RJLPQZ13BJuEIrp5jx5ptRD5uh3Y,92
+webuiapi-0.9.2.dist-info/top_level.txt,sha256=84RprjAaGWFS3oujg2AE1dTHp6o4yGT9isvN6frk5p4,9
+webuiapi-0.9.2.dist-info/RECORD,,
```

