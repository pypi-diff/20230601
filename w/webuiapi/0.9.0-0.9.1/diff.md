# Comparing `tmp/webuiapi-0.9.0-py3-none-any.whl.zip` & `tmp/webuiapi-0.9.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 12425 bytes, number of entries: 7
--rw-r--r--  2.0 unx      532 b- defN 23-May-26 01:18 webuiapi/__init__.py
--rw-r--r--  2.0 unx    34359 b- defN 23-May-26 01:18 webuiapi/webuiapi.py
--rw-r--r--  2.0 unx     1079 b- defN 23-May-26 01:18 webuiapi-0.9.0.dist-info/LICENSE
--rw-r--r--  2.0 unx    12995 b- defN 23-May-26 01:18 webuiapi-0.9.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 01:18 webuiapi-0.9.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-26 01:18 webuiapi-0.9.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      545 b- defN 23-May-26 01:18 webuiapi-0.9.0.dist-info/RECORD
-7 files, 49611 bytes uncompressed, 11463 bytes compressed:  76.9%
+Zip file size: 12615 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      532 b- defN 23-Jun-01 06:03 webuiapi/__init__.py
+-rw-r--r--  2.0 unx    34535 b- defN 23-Jun-01 06:03 webuiapi/webuiapi.py
+-rw-r--r--  2.0 unx     1079 b- defN 23-Jun-01 06:03 webuiapi-0.9.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13529 b- defN 23-Jun-01 06:03 webuiapi-0.9.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-01 06:03 webuiapi-0.9.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-01 06:03 webuiapi-0.9.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      545 b- defN 23-Jun-01 06:03 webuiapi-0.9.1.dist-info/RECORD
+7 files, 50321 bytes uncompressed, 11653 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: webuiapi/__init__.py
 Comment: 
 
 Filename: webuiapi/webuiapi.py
 Comment: 
 
-Filename: webuiapi-0.9.0.dist-info/LICENSE
+Filename: webuiapi-0.9.1.dist-info/LICENSE
 Comment: 
 
-Filename: webuiapi-0.9.0.dist-info/METADATA
+Filename: webuiapi-0.9.1.dist-info/METADATA
 Comment: 
 
-Filename: webuiapi-0.9.0.dist-info/WHEEL
+Filename: webuiapi-0.9.1.dist-info/WHEEL
 Comment: 
 
-Filename: webuiapi-0.9.0.dist-info/top_level.txt
+Filename: webuiapi-0.9.1.dist-info/top_level.txt
 Comment: 
 
-Filename: webuiapi-0.9.0.dist-info/RECORD
+Filename: webuiapi-0.9.1.dist-info/RECORD
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
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 __all__ = [
     "__version__",
     "WebUIApi",
     "WebUIApiResult",
     "Upscaler",
     "HiResUpscaler",
```

## webuiapi/webuiapi.py

```diff
@@ -134,38 +134,44 @@
         self,
         host="127.0.0.1",
         port=7860,
         baseurl=None,
         sampler="Euler a",
         steps=20,
         use_https=False,
+        username=None,
+        password=None,
     ):
         if baseurl is None:
             if use_https:
                 baseurl = f"https://{host}:{port}/sdapi/v1"
             else:
                 baseurl = f"http://{host}:{port}/sdapi/v1"
 
         self.baseurl = baseurl
         self.default_sampler = sampler
         self.default_steps = steps
 
         self.session = requests.Session()
 
-        self.check_controlnet()
+        if username and password:
+            self.set_auth(username, password)
+        else:
+            self.check_controlnet()
 
     def check_controlnet(self):
         try:
             scripts = self.get_scripts()
             self.has_controlnet = "controlnet m2m" in scripts["txt2img"]
         except:
             pass
 
     def set_auth(self, username, password):
         self.session.auth = (username, password)
+        self.check_controlnet()
 
     def _to_api_result(self, response):
         if response.status_code != 200:
             raise RuntimeError(response.status_code, response.text)
 
         r = response.json()
         images = []
```

## Comparing `webuiapi-0.9.0.dist-info/LICENSE` & `webuiapi-0.9.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `webuiapi-0.9.0.dist-info/METADATA` & `webuiapi-0.9.1.dist-info/METADATA`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: webuiapi
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python API client for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/mix1009/sdwebuiapi
 Author: ChunKoo Park
 Author-email: mix1009@gmail.com
 License: MIT
 Keywords: stable-diffuion-webui,AUTOMATIC1111,stable-diffusion,api
+Platform: UNKNOWN
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
-License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: Pillow
 
 # sdwebuiapi
 API client for AUTOMATIC1111/stable-diffusion-webui
 
 Supports txt2img, img2img, extra-single-image, extra-batch-images API calls.
@@ -48,15 +48,17 @@
 
 # create API client with custom host, port and https
 #api = webuiapi.WebUIApi(host='webui.example.com', port=443, use_https=True)
 
 # create API client with default sampler, steps.
 #api = webuiapi.WebUIApi(sampler='Euler a', steps=20)
 
-# optionally set username, password when --api-auth is set on webui.
+# optionally set username, password when --api-auth=username:password is set on webui.
+# username, password are not protected and can be derived easily if the communication channel is not encrypted.
+# you can also pass username, password to the WebUIApi constructor.
 api.set_auth('username', 'password')
 ```
 
 ## txt2img
 ```
 result1 = api.txt2img(prompt="cute squirrel",
                     negative_prompt="ugly, out of frame",
@@ -145,14 +147,24 @@
 ```
 ![extra_batch_images_1](https://user-images.githubusercontent.com/1288793/200459540-b0bd2931-93db-4d03-9cc1-a9f5e5c89745.jpg)
 ```
 result4.images[1]
 ```
 ![extra_batch_images_2](https://user-images.githubusercontent.com/1288793/200459542-aa8547a0-f6db-436b-bec1-031a93a7b1d4.jpg)
 
+### Async API support
+txt2img, img2img, extra_single_image, extra_batch_images support async api call with use_async=True parameter. You need asyncio, aiohttp packages installed.
+```
+result = await api.txt2img(prompt="cute kitten",
+                    seed=1001,
+                    use_async=True
+                    )
+result.image
+```
+
 ### Scripts support
 Scripts from AUTOMATIC1111's Web UI are supported, but there aren't official models that define a script's interface.
 
 To find out the list of arguments that are accepted by a particular script look up the associated python file from
 AUTOMATIC1111's repo `scripts/[script_name].py`. Search for its `run(p, **args)` function and the arguments that come
 after 'p' is the list of accepted arguments
 
@@ -380,26 +392,26 @@
 r = api.txt2img(prompt="photo of a beautiful girl with blonde hair", height=512, seed=100)
 img = r.image
 img
 ```
 ![cn1](https://user-images.githubusercontent.com/1288793/222315754-43c6dc8c-2a62-4a31-b51a-f68523118e0d.png)
 
 ```
-# txt2img with ControlNet (used 1.0 but also supports 2.0)
+# txt2img with ControlNet (used 1.0 but also supports 1.1)
 unit1 = webuiapi.ControlNetUnit(input_image=img, module='canny', model='control_canny-fp16 [e3fe7712]')
 
 r = api.txt2img(prompt="photo of a beautiful girl", controlnet_units=[unit1])
 r.image
 ```
 
 ![cn2](https://user-images.githubusercontent.com/1288793/222315791-c6c480eb-2987-4044-b673-5f2cb6135f87.png)
 
 
 ```
-# img2img with multiple ControlNets (used 1.0 but also supports 2.0)
+# img2img with multiple ControlNets (used 1.0 but also supports 1.1)
 unit1 = webuiapi.ControlNetUnit(input_image=img, module='canny', model='control_canny-fp16 [e3fe7712]')
 unit2 = webuiapi.ControlNetUnit(input_image=img, module='depth', model='control_depth-fp16 [400750f6]', weight=0.5)
 
 r2 = api.img2img(prompt="girl",
             images=[img], 
             width=512,
             height=512,
@@ -422,7 +434,9 @@
 ![cn5](https://user-images.githubusercontent.com/1288793/222315859-e6b6286e-854d-40c1-a516-5a08c827c49a.png)
 
 
 ```
 r = api.controlnet_detect(images=[img], module='canny')
 r.image
 ```
+
+
```

## Comparing `webuiapi-0.9.0.dist-info/RECORD` & `webuiapi-0.9.1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-webuiapi/__init__.py,sha256=sO9Tlyij7K8StG1E_8uPYO5If--hjsieDP7SDmEcGtY,532
-webuiapi/webuiapi.py,sha256=aJVb0q2Tai5bgfHfjRU2mGdRS063wA3m6cGYoRKgbhk,34359
-webuiapi-0.9.0.dist-info/LICENSE,sha256=Zl3ztitjIWviypQXfHYvUR099Y5IUOh15IVxAOw9XV8,1079
-webuiapi-0.9.0.dist-info/METADATA,sha256=2rFI5IOfn9aPF4dCtMgM5UKj2c1N2bDOVEH_f30MUrc,12995
-webuiapi-0.9.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-webuiapi-0.9.0.dist-info/top_level.txt,sha256=84RprjAaGWFS3oujg2AE1dTHp6o4yGT9isvN6frk5p4,9
-webuiapi-0.9.0.dist-info/RECORD,,
+webuiapi/__init__.py,sha256=OF4mr8dzZjSTkJxCJnyuSYz0GuoOcN3S69_5c9sUJfU,532
+webuiapi/webuiapi.py,sha256=iqlWYOLw1nSAh_D9qPH4inzujnBKZXxF0yFuD54mQOc,34535
+webuiapi-0.9.1.dist-info/LICENSE,sha256=Zl3ztitjIWviypQXfHYvUR099Y5IUOh15IVxAOw9XV8,1079
+webuiapi-0.9.1.dist-info/METADATA,sha256=cY45dg8mtpAa5dKuou05VhAJ3cDS7yOTwv_iEGIpaSA,13529
+webuiapi-0.9.1.dist-info/WHEEL,sha256=_NOXIqFgOaYmlm9RJLPQZ13BJuEIrp5jx5ptRD5uh3Y,92
+webuiapi-0.9.1.dist-info/top_level.txt,sha256=84RprjAaGWFS3oujg2AE1dTHp6o4yGT9isvN6frk5p4,9
+webuiapi-0.9.1.dist-info/RECORD,,
```

