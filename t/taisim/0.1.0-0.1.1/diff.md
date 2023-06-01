# Comparing `tmp/taisim-0.1.0.tar.gz` & `tmp/taisim-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taisim-0.1.0.tar", last modified: Wed May 31 19:43:12 2023, max compression
+gzip compressed data, was "taisim-0.1.1.tar", last modified: Thu Jun  1 00:14:31 2023, max compression
```

## Comparing `taisim-0.1.0.tar` & `taisim-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:43:12.274929 taisim-0.1.0/
--rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-30 21:36:27.000000 taisim-0.1.0/LICENSE
--rw-r--r--   0 root         (0) staff       (20)       37 2023-05-30 21:36:27.000000 taisim-0.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      423 2023-05-30 21:36:27.000000 taisim-0.1.0/NEWS.txt
--rw-r--r--   0 root         (0) staff       (20)      678 2023-05-31 19:43:12.274126 taisim-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3613 2023-05-30 21:36:27.000000 taisim-0.1.0/README.rst
--rw-r--r--   0 root         (0) staff       (20)       38 2023-05-31 19:43:12.275214 taisim-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) staff       (20)     1619 2023-05-31 19:42:35.000000 taisim-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:43:12.248455 taisim-0.1.0/src/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:43:12.259225 taisim-0.1.0/src/taisim/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.1.0/src/taisim/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:43:12.267789 taisim-0.1.0/src/taisim/components/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.1.0/src/taisim/components/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-30 21:36:27.000000 taisim-0.1.0/src/taisim/components/log.py
--rw-r--r--   0 root         (0) staff       (20)     1230 2023-05-30 21:36:27.000000 taisim-0.1.0/src/taisim/components/video.py
--rw-r--r--   0 root         (0) staff       (20)     1439 2023-05-31 19:43:03.000000 taisim-0.1.0/src/taisim/external_data.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:43:12.271085 taisim-0.1.0/src/taisim/gui/
--rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.1.0/src/taisim/gui/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     8155 2023-05-30 21:36:27.000000 taisim-0.1.0/src/taisim/gui/help_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3895 2023-05-30 21:36:27.000000 taisim-0.1.0/src/taisim/gui/sensor_bar.py
--rw-r--r--   0 root         (0) staff       (20)     3837 2023-05-31 19:42:03.000000 taisim-0.1.0/src/taisim/player.py
--rw-r--r--   0 root         (0) staff       (20)    17862 2023-05-30 21:36:27.000000 taisim-0.1.0/src/taisim/sensor.py
--rw-r--r--   0 root         (0) staff       (20)     3454 2023-05-31 19:42:51.000000 taisim-0.1.0/src/taisim/simulator.py
--rw-r--r--   0 root         (0) staff       (20)     9889 2023-05-30 21:36:27.000000 taisim-0.1.0/src/taisim/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-05-31 19:43:12.265332 taisim-0.1.0/src/taisim.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      678 2023-05-31 19:43:12.000000 taisim-0.1.0/src/taisim.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)      601 2023-05-31 19:43:12.000000 taisim-0.1.0/src/taisim.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-31 19:43:12.000000 taisim-0.1.0/src/taisim.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       40 2023-05-31 19:43:12.000000 taisim-0.1.0/src/taisim.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 21:36:48.000000 taisim-0.1.0/src/taisim.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) staff       (20)       21 2023-05-31 19:43:12.000000 taisim-0.1.0/src/taisim.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        7 2023-05-31 19:43:12.000000 taisim-0.1.0/src/taisim.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-01 00:14:31.690901 taisim-0.1.1/
+-rw-r--r--   0 root         (0) staff       (20)     1070 2023-05-30 21:36:27.000000 taisim-0.1.1/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)       37 2023-05-30 21:36:27.000000 taisim-0.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      423 2023-05-30 21:36:27.000000 taisim-0.1.1/NEWS.txt
+-rw-r--r--   0 root         (0) staff       (20)      678 2023-06-01 00:14:31.690380 taisim-0.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3613 2023-05-30 21:36:27.000000 taisim-0.1.1/README.rst
+-rw-r--r--   0 root         (0) staff       (20)       38 2023-06-01 00:14:31.691089 taisim-0.1.1/setup.cfg
+-rw-r--r--   0 root         (0) staff       (20)     1619 2023-06-01 00:14:00.000000 taisim-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-01 00:14:31.662552 taisim-0.1.1/src/
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-01 00:14:31.674480 taisim-0.1.1/src/taisim/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.1.1/src/taisim/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-01 00:14:31.686478 taisim-0.1.1/src/taisim/components/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.1.1/src/taisim/components/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     1577 2023-05-30 21:36:27.000000 taisim-0.1.1/src/taisim/components/log.py
+-rw-r--r--   0 root         (0) staff       (20)     1230 2023-05-30 21:36:27.000000 taisim-0.1.1/src/taisim/components/video.py
+-rw-r--r--   0 root         (0) staff       (20)     1439 2023-06-01 00:14:14.000000 taisim-0.1.1/src/taisim/external_data.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-01 00:14:31.689059 taisim-0.1.1/src/taisim/gui/
+-rw-r--r--   0 root         (0) staff       (20)        0 2023-05-30 21:36:27.000000 taisim-0.1.1/src/taisim/gui/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     8155 2023-05-30 21:36:27.000000 taisim-0.1.1/src/taisim/gui/help_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3895 2023-05-30 21:36:27.000000 taisim-0.1.1/src/taisim/gui/sensor_bar.py
+-rw-r--r--   0 root         (0) staff       (20)     3837 2023-05-31 19:42:03.000000 taisim-0.1.1/src/taisim/player.py
+-rw-r--r--   0 root         (0) staff       (20)    17862 2023-06-01 00:13:51.000000 taisim-0.1.1/src/taisim/sensor.py
+-rw-r--r--   0 root         (0) staff       (20)     3454 2023-05-31 19:42:51.000000 taisim-0.1.1/src/taisim/simulator.py
+-rw-r--r--   0 root         (0) staff       (20)     9889 2023-05-30 21:36:27.000000 taisim-0.1.1/src/taisim/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-06-01 00:14:31.684158 taisim-0.1.1/src/taisim.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      678 2023-06-01 00:14:31.000000 taisim-0.1.1/src/taisim.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)      601 2023-06-01 00:14:31.000000 taisim-0.1.1/src/taisim.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-06-01 00:14:31.000000 taisim-0.1.1/src/taisim.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)       40 2023-06-01 00:14:31.000000 taisim-0.1.1/src/taisim.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-05-30 21:36:48.000000 taisim-0.1.1/src/taisim.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) staff       (20)       21 2023-06-01 00:14:31.000000 taisim-0.1.1/src/taisim.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        7 2023-06-01 00:14:31.000000 taisim-0.1.1/src/taisim.egg-info/top_level.txt
```

### Comparing `taisim-0.1.0/LICENSE` & `taisim-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taisim-0.1.0/PKG-INFO` & `taisim-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taisim
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple python3 simulator for advanced driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut@outlook.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Platform: UNKNOWN
```

### Comparing `taisim-0.1.0/README.rst` & `taisim-0.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `taisim-0.1.0/setup.py` & `taisim-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     # For more details, see:
     # http://packages.python.org/distribute/setuptools.html#declaring-dependencies
     'requests'	
 ]
 
 
 setup(name='taisim',
-    version='0.1.0',
+    version='0.1.1',
     description="Simple python3 simulator for advanced driving systems",
     long_description="simple python simulator for advanced driving systems",
     
     keywords='Simulator computer vision Advanced Driving',
     author='Tucudean Adrian-Ionut',
     author_email='Tucudean.Adrian.Ionut@outlook.com',
     url='https://github.com/Amporu/SparkVerse',
```

### Comparing `taisim-0.1.0/src/taisim/components/log.py` & `taisim-0.1.1/src/taisim/components/log.py`

 * *Files identical despite different names*

### Comparing `taisim-0.1.0/src/taisim/components/video.py` & `taisim-0.1.1/src/taisim/components/video.py`

 * *Files identical despite different names*

### Comparing `taisim-0.1.0/src/taisim/external_data.py` & `taisim-0.1.1/src/taisim/external_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 autor: Tucudean Adrian-Ionut
 date: 22.05.2023
 email: Tucudean.Adrian.Ionut@outlook.com
 license: MIT
 """
 import os
 from taisim.components.log import logger
-VERSION='0.1.0'
+VERSION='0.1.1'
 logger.info("VERSION : \033[92m%s\033[0m",VERSION)
 CAR    = os.path.join(os.path.dirname(__file__), 'data/player.png')
 LEVEL1 = os.path.join(os.path.dirname(__file__), 'data/LineFollower1.png')
 LEVEL2 = os.path.join(os.path.dirname(__file__), 'data/LineFollower2.png')
 LEVEL3 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper1.png')
 LEVEL4 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper2.png')
 LEVEL5 = os.path.join(os.path.dirname(__file__), 'data/LaneKeeper3.png')
```

### Comparing `taisim-0.1.0/src/taisim/gui/help_bar.py` & `taisim-0.1.1/src/taisim/gui/help_bar.py`

 * *Files identical despite different names*

### Comparing `taisim-0.1.0/src/taisim/gui/sensor_bar.py` & `taisim-0.1.1/src/taisim/gui/sensor_bar.py`

 * *Files identical despite different names*

### Comparing `taisim-0.1.0/src/taisim/player.py` & `taisim-0.1.1/src/taisim/player.py`

 * *Files identical despite different names*

### Comparing `taisim-0.1.0/src/taisim/sensor.py` & `taisim-0.1.1/src/taisim/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -358,15 +358,15 @@
                 lines.append(lines[i-1]-step)
         #print(lines)
         lidar_distance=[]
         x_p=[]
         y_p=[]
         x_lidar=[]
         y_lidar=[]
-        space=20
+        space=25
         mask_gray=cv2.cvtColor(frame,cv2.COLOR_BGR2GRAY)
         for i in range(self.angular_resolution):
 
             x_p1 = self.player.x_value + space * math.cos(math.radians(lines[i]))
             y_p1= self.player.y_value + space * math.sin(math.radians(lines[i]))
             x_p.append(int(x_p1))
             y_p.append(int(y_p1))
```

### Comparing `taisim-0.1.0/src/taisim/simulator.py` & `taisim-0.1.1/src/taisim/simulator.py`

 * *Files identical despite different names*

### Comparing `taisim-0.1.0/src/taisim/utils.py` & `taisim-0.1.1/src/taisim/utils.py`

 * *Files identical despite different names*

### Comparing `taisim-0.1.0/src/taisim.egg-info/PKG-INFO` & `taisim-0.1.1/src/taisim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taisim
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple python3 simulator for advanced driving systems
 Home-page: https://github.com/Amporu/SparkVerse
 Author: Tucudean Adrian-Ionut
 Author-email: Tucudean.Adrian.Ionut@outlook.com
 License: MIT
 Keywords: Simulator computer vision Advanced Driving
 Platform: UNKNOWN
```

### Comparing `taisim-0.1.0/src/taisim.egg-info/SOURCES.txt` & `taisim-0.1.1/src/taisim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

