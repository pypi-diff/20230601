# Comparing `tmp/dariusVision-0.0.3.tar.gz` & `tmp/dariusVision-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dariusVision-0.0.3.tar", last modified: Sat Apr  8 08:43:33 2023, max compression
+gzip compressed data, was "dariusVision-0.0.4.tar", last modified: Thu Jun  1 07:54:15 2023, max compression
```

## Comparing `dariusVision-0.0.3.tar` & `dariusVision-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gbox3d    (1000) gbox3d    (1000)        0 2023-04-08 08:43:33.453952 dariusVision-0.0.3/
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)    35149 2023-04-07 04:46:45.000000 dariusVision-0.0.3/LICENSE
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      445 2023-04-08 08:43:33.453952 dariusVision-0.0.3/PKG-INFO
-drwxrwxr-x   0 gbox3d    (1000) gbox3d    (1000)        0 2023-04-08 08:43:33.453952 dariusVision-0.0.3/dariusVision/
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      175 2023-04-08 08:43:26.000000 dariusVision-0.0.3/dariusVision/__init__.py
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)     3265 2023-04-07 01:35:34.000000 dariusVision-0.0.3/dariusVision/cam.py
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)     9628 2023-04-08 08:39:34.000000 dariusVision-0.0.3/dariusVision/realsense2.py
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)     2011 2023-04-07 04:29:23.000000 dariusVision-0.0.3/dariusVision/utils.py
-drwxrwxr-x   0 gbox3d    (1000) gbox3d    (1000)        0 2023-04-08 08:43:33.453952 dariusVision-0.0.3/dariusVision.egg-info/
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      445 2023-04-08 08:43:33.000000 dariusVision-0.0.3/dariusVision.egg-info/PKG-INFO
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      289 2023-04-08 08:43:33.000000 dariusVision-0.0.3/dariusVision.egg-info/SOURCES.txt
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)        1 2023-04-08 08:43:33.000000 dariusVision-0.0.3/dariusVision.egg-info/dependency_links.txt
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)       33 2023-04-08 08:43:33.000000 dariusVision-0.0.3/dariusVision.egg-info/requires.txt
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)       13 2023-04-08 08:43:33.000000 dariusVision-0.0.3/dariusVision.egg-info/top_level.txt
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)       38 2023-04-08 08:43:33.453952 dariusVision-0.0.3/setup.cfg
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      644 2023-04-08 08:41:22.000000 dariusVision-0.0.3/setup.py
+drwxrwxr-x   0 gbox3d    (1000) gbox3d    (1000)        0 2023-06-01 07:54:15.981321 dariusVision-0.0.4/
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)    35149 2023-04-07 04:46:45.000000 dariusVision-0.0.4/LICENSE
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      445 2023-06-01 07:54:15.981321 dariusVision-0.0.4/PKG-INFO
+drwxrwxr-x   0 gbox3d    (1000) gbox3d    (1000)        0 2023-06-01 07:54:15.977321 dariusVision-0.0.4/dariusVision/
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      423 2023-06-01 07:48:43.000000 dariusVision-0.0.4/dariusVision/__init__.py
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)     3265 2023-04-07 01:35:34.000000 dariusVision-0.0.4/dariusVision/cam.py
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)    10315 2023-06-01 07:50:31.000000 dariusVision-0.0.4/dariusVision/realsense2.py
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)     2011 2023-04-07 04:29:23.000000 dariusVision-0.0.4/dariusVision/utils.py
+drwxrwxr-x   0 gbox3d    (1000) gbox3d    (1000)        0 2023-06-01 07:54:15.981321 dariusVision-0.0.4/dariusVision.egg-info/
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      445 2023-06-01 07:54:15.000000 dariusVision-0.0.4/dariusVision.egg-info/PKG-INFO
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      289 2023-06-01 07:54:15.000000 dariusVision-0.0.4/dariusVision.egg-info/SOURCES.txt
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)        1 2023-06-01 07:54:15.000000 dariusVision-0.0.4/dariusVision.egg-info/dependency_links.txt
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)       33 2023-06-01 07:54:15.000000 dariusVision-0.0.4/dariusVision.egg-info/requires.txt
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)       13 2023-06-01 07:54:15.000000 dariusVision-0.0.4/dariusVision.egg-info/top_level.txt
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)       38 2023-06-01 07:54:15.981321 dariusVision-0.0.4/setup.cfg
+-rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      644 2023-06-01 07:54:12.000000 dariusVision-0.0.4/setup.py
```

### Comparing `dariusVision-0.0.3/LICENSE` & `dariusVision-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dariusVision-0.0.3/dariusVision/cam.py` & `dariusVision-0.0.4/dariusVision/cam.py`

 * *Files identical despite different names*

### Comparing `dariusVision-0.0.3/dariusVision/realsense2.py` & `dariusVision-0.0.4/dariusVision/realsense2.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,39 +5,39 @@
 import numpy as np
 
 # from PIL import Image
 # from IPython.display import display
 
 #%%
 class rs2_AsyncCam : 
-    def __init__(self,vid_src=0,grab_delay=0.1,width=640,height=480) :
+    def __init__(self,vid_src=0,grab_delay=0.1) :
         self.frame_status = False
         self.running = False
         self.depth_frame = None
         self.color_frame = None
         self.grab_delay = grab_delay
-        self.width = width
-        self.height = height
         self.pipeline = None
         self._critical_Section = None 
+        self.video_source = vid_src
             
     def startCamera(self) :
         
         # RealSense context 생성
         context = rs.context()
 
         # 연결된 모든 RealSense 장치의 정보 얻기
         devices = context.query_devices()
 
         # 모든 장치의 이름 출력
         for dev in devices:
             print(dev.get_info(rs.camera_info.name))
 
-        self.camera_model = devices[0].get_info(rs.camera_info.name)
-        
+        self.camera_model = devices[self.video_source].get_info(rs.camera_info.name)
+        self.camera_name = self.camera_model.split(' ')[-1]
+                
         if self.pipeline is None :
             pipeline = rs.pipeline()
             config = rs.config()
 
             # Get device product line for setting a supporting resolution
             pipeline_wrapper = rs.pipeline_wrapper(pipeline)
             pipeline_profile = config.resolve(pipeline_wrapper)
@@ -48,22 +48,32 @@
             for s in device.sensors:
                 if s.get_info(rs.camera_info.name) == 'RGB Camera':
                     found_rgb = True
                     break
             if not found_rgb:
                 print("The demo requires Depth camera with Color sensor")
                 exit(0)
-
-            config.enable_stream(rs.stream.depth, self.width, self.height, rs.format.z16, 30)
-
-            if device_product_line == 'L500':
+                
+            if (self.camera_name == 'L515'):
+                config.enable_stream(rs.stream.depth, 1024, 768, rs.format.z16, 30)
                 config.enable_stream(rs.stream.color, 960, 540, rs.format.bgr8, 30)
-            else:
+            elif (self.camera_name == 'D435'):
+                config.enable_stream(rs.stream.depth, 640, 480, rs.format.z16, 30)
+                config.enable_stream(rs.stream.color, 640, 480, rs.format.bgr8, 30)                
+            else :
+                config.enable_stream(rs.stream.depth, 640, 480, rs.format.z16, 30)
                 config.enable_stream(rs.stream.color, 640, 480, rs.format.bgr8, 30)
 
+
+            # if device_product_line == 'L500':
+            #     config.enable_stream(rs.stream.color, 960, 540, rs.format.bgr8, 30)
+            # else:
+            #     config.enable_stream(rs.stream.depth, 640,480, rs.format.z16, 30)
+            #     config.enable_stream(rs.stream.color, 640, 480, rs.format.bgr8, 30)
+
             print("device_product_line: ", device_product_line)
             print("found_rgb: ", found_rgb)
             print("init ok")
             profile = pipeline.start(config)
             self.pipeline = pipeline
             
             depth_sensor = profile.get_device().first_depth_sensor()
```

### Comparing `dariusVision-0.0.3/dariusVision/utils.py` & `dariusVision-0.0.4/dariusVision/utils.py`

 * *Files identical despite different names*

### Comparing `dariusVision-0.0.3/setup.py` & `dariusVision-0.0.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dariusVision',
-    version='0.0.3',
+    version='0.0.4',
     description='camera utilities to get last frame',
     long_description='camera utilities to get last frame',
     packages=['dariusVision'],
     install_requires=[
         'numpy',
         'opencv-python',
         'pyrealsense2',
```

