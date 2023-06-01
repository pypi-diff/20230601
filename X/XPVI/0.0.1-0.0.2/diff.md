# Comparing `tmp/XPVI-0.0.1.tar.gz` & `tmp/XPVI-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\XPVI-0.0.1.tar", last modified: Thu Jun  1 03:03:23 2023, max compression
+gzip compressed data, was "dist\XPVI-0.0.2.tar", last modified: Thu Jun  1 03:07:24 2023, max compression
```

## Comparing `XPVI-0.0.1.tar` & `XPVI-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 03:03:23.038203 XPVI-0.0.1/
--rw-rw-rw-   0        0        0     3345 2023-06-01 03:03:23.037203 XPVI-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1807 2023-06-01 01:38:41.000000 XPVI-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 03:03:23.036205 XPVI-0.0.1/XPVI.egg-info/
--rw-rw-rw-   0        0        0     3345 2023-06-01 03:03:22.000000 XPVI-0.0.1/XPVI.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      130 2023-06-01 03:03:22.000000 XPVI-0.0.1/XPVI.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 03:03:22.000000 XPVI-0.0.1/XPVI.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 03:03:22.000000 XPVI-0.0.1/XPVI.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 03:03:23.038203 XPVI-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0    10189 2023-06-01 03:03:22.000000 XPVI-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 03:07:24.496989 XPVI-0.0.2/
+-rw-rw-rw-   0        0        0     3985 2023-06-01 03:07:24.496989 XPVI-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1871 2023-06-01 03:06:55.000000 XPVI-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 03:07:24.494990 XPVI-0.0.2/XPVI.egg-info/
+-rw-rw-rw-   0        0        0     3985 2023-06-01 03:07:24.000000 XPVI-0.0.2/XPVI.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      130 2023-06-01 03:07:24.000000 XPVI-0.0.2/XPVI.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 03:07:24.000000 XPVI-0.0.2/XPVI.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 03:07:24.000000 XPVI-0.0.2/XPVI.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 03:07:24.498100 XPVI-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0    10189 2023-06-01 03:07:24.000000 XPVI-0.0.2/setup.py
```

### Comparing `XPVI-0.0.1/PKG-INFO` & `XPVI-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,121 +1,185 @@
 Metadata-Version: 2.1
 Name: XPVI
-Version: 0.0.1
+Version: 0.0.2
 Summary: Get and save custom variables "to" a usb video device
 Home-page: UNKNOWN
 Author: Karrson Heumann
 Author-email: <mail@example.com>
 License: UNKNOWN
 Description: 
         # XPVI
         
          Cross Platform Video Info
+        
+        
         Get and save custom system-wide variables "to" a usb video device or filepath.
+        
+        
         Also works with audio devices, very useful for saving calibration data.
+        
+        
         Can also get a device index from it's name and vice-versa.
         
         
         
         # Install
         
         You will get an error if not admin,
         
+        
+        
         but assuming you are an admin...
         
+        
+        
          => pip install XPVI
         
         
         
         # Docs
         
          => XPVI(.bat or .sh)
         
+        
+        
         ...
         
+        
+        
         syntax:
+        
+        
         v* (get_all_video_devices)
+        
+        
         a* (get_all_audio_devices)
+        
+        
         v2i name (get_id_from_video_device)
+        
+        
         a2i name (get_id_from_audio_device)
+        
+        
         i2v id (get_video_device_from_id)
+        
+        
         i2a id (get_audio_device_from_id)
+        
+        
         set name key value (set_value)
+        
+        
         set name key "NULL" (delete_key)
+        
+        
         get name key (get_value)
+        
+        
         get name "ALL" (get_values)
         
         
         
         # Error Handling
         
          Not everyone has FFMPEG, but it's required for this to work.
         
+        
+        
         So in every app that calls the XPVI cli (which is the only official way to interface with it),
         
+        
+        
         it should first call XPVI itself and check if the word "syntax" is contained 
         
+        
+        
         (case may change in the future, so check should be case-insensitive)...
         
+        
+        
         If it contains it, there were no errors.
         
+        
+        
         Otherwise, there was an error in the installation 
         
+        
+        
         (maybe FFMPEG is missing for example, but we can't be sure)
         
+        
+        
         and so we need to show a message box with the XPVI command's output.
         
         
         
         # Example
         
          => XPVI.bat v*
         
+        
+        
         ...
         
+        
+        
         [(0, 'c922 Pro Stream Webcam'), (1, 'OBS Virtual Camera')]
         
         
         
         Now we know that 'c922 Pro Stream Webcam' is our video device...
         
         
         
         => XPVI.bat v2i "c922 Pro Stream Webcam"
         
+        
+        
         ...
         
+        
+        
         0
         
         
         
         INDEX = XPVI command output
         
         
         
         #Great! We finally have a way to use a specific camera with opencv!
         
+        
+        
         cap = cv2.VideoCapture(INDEX) 
         
         
         
         ... (INSERT CAMERA CALIBRATION CODE) ...
         
         
         
         => XPVI.bat set "c922 Pro Stream Webcam" fx (INSERT FOCAL X DATA)
         
+        
+        
         ...
         
         
         
         => XPVI.bat get "c922 Pro Stream Webcam" fx
         
+        
+        
         ...
         
+        
+        
         (INSERT FOCAL X DATA)
         
 Keywords: python,video,audio,camera,microphone,data
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `XPVI-0.0.1/README.md` & `XPVI-0.0.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,106 +1,170 @@
 # XPVI
 
  Cross Platform Video Info
+
+
 Get and save custom system-wide variables "to" a usb video device or filepath.
+
+
 Also works with audio devices, very useful for saving calibration data.
+
+
 Can also get a device index from it's name and vice-versa.
 
 
 
 # Install
 
 You will get an error if not admin,
 
+
+
 but assuming you are an admin...
 
+
+
  => pip install XPVI
 
 
 
 # Docs
 
  => XPVI(.bat or .sh)
 
+
+
 ...
 
+
+
 syntax:
+
+
 v* (get_all_video_devices)
+
+
 a* (get_all_audio_devices)
+
+
 v2i name (get_id_from_video_device)
+
+
 a2i name (get_id_from_audio_device)
+
+
 i2v id (get_video_device_from_id)
+
+
 i2a id (get_audio_device_from_id)
+
+
 set name key value (set_value)
+
+
 set name key "NULL" (delete_key)
+
+
 get name key (get_value)
+
+
 get name "ALL" (get_values)
 
 
 
 # Error Handling
 
  Not everyone has FFMPEG, but it's required for this to work.
 
+
+
 So in every app that calls the XPVI cli (which is the only official way to interface with it),
 
+
+
 it should first call XPVI itself and check if the word "syntax" is contained 
 
+
+
 (case may change in the future, so check should be case-insensitive)...
 
+
+
 If it contains it, there were no errors.
 
+
+
 Otherwise, there was an error in the installation 
 
+
+
 (maybe FFMPEG is missing for example, but we can't be sure)
 
+
+
 and so we need to show a message box with the XPVI command's output.
 
 
 
 # Example
 
  => XPVI.bat v*
 
+
+
 ...
 
+
+
 [(0, 'c922 Pro Stream Webcam'), (1, 'OBS Virtual Camera')]
 
 
 
 Now we know that 'c922 Pro Stream Webcam' is our video device...
 
 
 
 => XPVI.bat v2i "c922 Pro Stream Webcam"
 
+
+
 ...
 
+
+
 0
 
 
 
 INDEX = XPVI command output
 
 
 
 #Great! We finally have a way to use a specific camera with opencv!
 
+
+
 cap = cv2.VideoCapture(INDEX) 
 
 
 
 ... (INSERT CAMERA CALIBRATION CODE) ...
 
 
 
 => XPVI.bat set "c922 Pro Stream Webcam" fx (INSERT FOCAL X DATA)
 
+
+
 ...
 
 
 
 => XPVI.bat get "c922 Pro Stream Webcam" fx
 
+
+
 ...
 
+
+
 (INSERT FOCAL X DATA)
```

### Comparing `XPVI-0.0.1/XPVI.egg-info/PKG-INFO` & `XPVI-0.0.2/XPVI.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,121 +1,185 @@
 Metadata-Version: 2.1
 Name: XPVI
-Version: 0.0.1
+Version: 0.0.2
 Summary: Get and save custom variables "to" a usb video device
 Home-page: UNKNOWN
 Author: Karrson Heumann
 Author-email: <mail@example.com>
 License: UNKNOWN
 Description: 
         # XPVI
         
          Cross Platform Video Info
+        
+        
         Get and save custom system-wide variables "to" a usb video device or filepath.
+        
+        
         Also works with audio devices, very useful for saving calibration data.
+        
+        
         Can also get a device index from it's name and vice-versa.
         
         
         
         # Install
         
         You will get an error if not admin,
         
+        
+        
         but assuming you are an admin...
         
+        
+        
          => pip install XPVI
         
         
         
         # Docs
         
          => XPVI(.bat or .sh)
         
+        
+        
         ...
         
+        
+        
         syntax:
+        
+        
         v* (get_all_video_devices)
+        
+        
         a* (get_all_audio_devices)
+        
+        
         v2i name (get_id_from_video_device)
+        
+        
         a2i name (get_id_from_audio_device)
+        
+        
         i2v id (get_video_device_from_id)
+        
+        
         i2a id (get_audio_device_from_id)
+        
+        
         set name key value (set_value)
+        
+        
         set name key "NULL" (delete_key)
+        
+        
         get name key (get_value)
+        
+        
         get name "ALL" (get_values)
         
         
         
         # Error Handling
         
          Not everyone has FFMPEG, but it's required for this to work.
         
+        
+        
         So in every app that calls the XPVI cli (which is the only official way to interface with it),
         
+        
+        
         it should first call XPVI itself and check if the word "syntax" is contained 
         
+        
+        
         (case may change in the future, so check should be case-insensitive)...
         
+        
+        
         If it contains it, there were no errors.
         
+        
+        
         Otherwise, there was an error in the installation 
         
+        
+        
         (maybe FFMPEG is missing for example, but we can't be sure)
         
+        
+        
         and so we need to show a message box with the XPVI command's output.
         
         
         
         # Example
         
          => XPVI.bat v*
         
+        
+        
         ...
         
+        
+        
         [(0, 'c922 Pro Stream Webcam'), (1, 'OBS Virtual Camera')]
         
         
         
         Now we know that 'c922 Pro Stream Webcam' is our video device...
         
         
         
         => XPVI.bat v2i "c922 Pro Stream Webcam"
         
+        
+        
         ...
         
+        
+        
         0
         
         
         
         INDEX = XPVI command output
         
         
         
         #Great! We finally have a way to use a specific camera with opencv!
         
+        
+        
         cap = cv2.VideoCapture(INDEX) 
         
         
         
         ... (INSERT CAMERA CALIBRATION CODE) ...
         
         
         
         => XPVI.bat set "c922 Pro Stream Webcam" fx (INSERT FOCAL X DATA)
         
+        
+        
         ...
         
         
         
         => XPVI.bat get "c922 Pro Stream Webcam" fx
         
+        
+        
         ...
         
+        
+        
         (INSERT FOCAL X DATA)
         
 Keywords: python,video,audio,camera,microphone,data
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `XPVI-0.0.1/setup.py` & `XPVI-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Get and save custom variables "to" a usb video device'
 LONG_DESCRIPTION = 'Cross Platform Video Info, \n' + \
 'Get and save custom system-wide variables "to" a usb video device or filepath, \n' + \
 'Also works with audio devices, very useful for saving calibration data, \n' + \
 'Can also get a device index from it\'s name and vice-versa'
 
 def install_package():
```

