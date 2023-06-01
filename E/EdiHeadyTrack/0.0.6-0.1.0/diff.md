# Comparing `tmp/EdiHeadyTrack-0.0.6.tar.gz` & `tmp/EdiHeadyTrack-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thomas/Library/CloudStorage/OneDrive-UniversityofEdinburgh/PhD/1. Working/1. Computational/EdiHeadyTrack - PACKAGE SOURC", last modified: Thu Jun  1 13:04:20 2023, max compression
+gzip compressed data, was "/Users/thomas/Library/CloudStorage/OneDrive-UniversityofEdinburgh/PhD/1. Working/1. Computational/EdiHeadyTrack - PACKAGE SOURC", last modified: Thu Jun  1 13:13:05 2023, max compression
```

## Comparing `EdiHeadyTrack-0.0.6.tar` & `EdiHeadyTrack-0.1.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:04:20.162830 EdiHeadyTrack-0.0.6/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:04:20.157527 EdiHeadyTrack-0.0.6/EdiHeadyTrack/
--rwxr-xr-x   0 thomas     (501) staff       (20)      384 2023-05-16 14:34:30.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)    10545 2023-05-30 10:21:02.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/camera.py
--rwxr-xr-x   0 thomas     (501) staff       (20)     9787 2023-05-30 11:15:07.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/facedetector.py
--rw-r--r--   0 thomas     (501) staff       (20)     2763 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/filter.py
--rw-r--r--   0 thomas     (501) staff       (20)     1808 2023-05-30 14:02:35.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/imu.py
--rw-r--r--   0 thomas     (501) staff       (20)     9423 2023-06-01 12:47:57.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/plot.py
--rw-r--r--   0 thomas     (501) staff       (20)     7673 2023-05-30 13:13:46.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/sensordata.py
--rw-r--r--   0 thomas     (501) staff       (20)     3279 2023-05-30 09:09:03.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/video.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:04:20.158834 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)     4347 2023-06-01 13:04:20.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      598 2023-06-01 13:04:20.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-06-01 13:04:20.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       78 2023-06-01 13:04:20.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)       19 2023-06-01 13:04:20.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)       33 2023-05-16 08:07:20.000000 EdiHeadyTrack-0.0.6/MANIFEST.in
--rw-r--r--   0 thomas     (501) staff       (20)     4347 2023-06-01 13:04:20.162957 EdiHeadyTrack-0.0.6/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     3853 2023-05-30 15:20:09.000000 EdiHeadyTrack-0.0.6/README.md
--rw-r--r--   0 thomas     (501) staff       (20)       89 2023-05-12 09:37:25.000000 EdiHeadyTrack-0.0.6/pyproject.toml
--rw-r--r--   0 thomas     (501) staff       (20)      712 2023-06-01 13:04:20.163408 EdiHeadyTrack-0.0.6/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)       75 2023-05-16 08:58:57.000000 EdiHeadyTrack-0.0.6/setup.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:04:20.162539 EdiHeadyTrack-0.0.6/test/
--rw-r--r--   0 thomas     (501) staff       (20)        0 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.6/test/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)      578 2023-05-30 11:14:27.000000 EdiHeadyTrack-0.0.6/test/test_camera.py
--rw-r--r--   0 thomas     (501) staff       (20)      643 2023-05-30 11:27:51.000000 EdiHeadyTrack-0.0.6/test/test_facedetector.py
--rw-r--r--   0 thomas     (501) staff       (20)     1070 2023-05-30 13:48:57.000000 EdiHeadyTrack-0.0.6/test/test_filter.py
--rw-r--r--   0 thomas     (501) staff       (20)      260 2023-05-30 14:13:57.000000 EdiHeadyTrack-0.0.6/test/test_imu.py
--rw-r--r--   0 thomas     (501) staff       (20)     1650 2023-05-31 11:17:25.000000 EdiHeadyTrack-0.0.6/test/test_plot.py
--rw-r--r--   0 thomas     (501) staff       (20)     1258 2023-05-30 14:23:09.000000 EdiHeadyTrack-0.0.6/test/test_sensordata.py
--rw-r--r--   0 thomas     (501) staff       (20)      635 2023-05-30 11:14:03.000000 EdiHeadyTrack-0.0.6/test/test_video.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:13:05.897594 EdiHeadyTrack-0.1.0/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:13:05.893261 EdiHeadyTrack-0.1.0/EdiHeadyTrack/
+-rwxr-xr-x   0 thomas     (501) staff       (20)      384 2023-05-16 14:34:30.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)    10545 2023-05-30 10:21:02.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack/camera.py
+-rwxr-xr-x   0 thomas     (501) staff       (20)     9787 2023-05-30 11:15:07.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack/facedetector.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2763 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack/filter.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1808 2023-05-30 14:02:35.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack/imu.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9423 2023-06-01 12:47:57.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack/plot.py
+-rw-r--r--   0 thomas     (501) staff       (20)     7673 2023-05-30 13:13:46.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack/sensordata.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3279 2023-05-30 09:09:03.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack/video.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:13:05.894680 EdiHeadyTrack-0.1.0/EdiHeadyTrack.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)     4369 2023-06-01 13:13:05.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      606 2023-06-01 13:13:05.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-06-01 13:13:05.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       78 2023-06-01 13:13:05.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       19 2023-06-01 13:13:05.000000 EdiHeadyTrack-0.1.0/EdiHeadyTrack.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)    11357 2023-06-01 13:10:53.000000 EdiHeadyTrack-0.1.0/LICENSE
+-rw-r--r--   0 thomas     (501) staff       (20)       33 2023-05-16 08:07:20.000000 EdiHeadyTrack-0.1.0/MANIFEST.in
+-rw-r--r--   0 thomas     (501) staff       (20)     4369 2023-06-01 13:13:05.897729 EdiHeadyTrack-0.1.0/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     3853 2023-05-30 15:20:09.000000 EdiHeadyTrack-0.1.0/README.md
+-rw-r--r--   0 thomas     (501) staff       (20)       89 2023-05-12 09:37:25.000000 EdiHeadyTrack-0.1.0/pyproject.toml
+-rw-r--r--   0 thomas     (501) staff       (20)      712 2023-06-01 13:13:05.898246 EdiHeadyTrack-0.1.0/setup.cfg
+-rw-r--r--   0 thomas     (501) staff       (20)       75 2023-05-16 08:58:57.000000 EdiHeadyTrack-0.1.0/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:13:05.897301 EdiHeadyTrack-0.1.0/test/
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.1.0/test/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      578 2023-05-30 11:14:27.000000 EdiHeadyTrack-0.1.0/test/test_camera.py
+-rw-r--r--   0 thomas     (501) staff       (20)      643 2023-05-30 11:27:51.000000 EdiHeadyTrack-0.1.0/test/test_facedetector.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1070 2023-05-30 13:48:57.000000 EdiHeadyTrack-0.1.0/test/test_filter.py
+-rw-r--r--   0 thomas     (501) staff       (20)      260 2023-05-30 14:13:57.000000 EdiHeadyTrack-0.1.0/test/test_imu.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1650 2023-05-31 11:17:25.000000 EdiHeadyTrack-0.1.0/test/test_plot.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1258 2023-05-30 14:23:09.000000 EdiHeadyTrack-0.1.0/test/test_sensordata.py
+-rw-r--r--   0 thomas     (501) staff       (20)      635 2023-05-30 11:14:03.000000 EdiHeadyTrack-0.1.0/test/test_video.py
```

### Comparing `EdiHeadyTrack-0.0.6/EdiHeadyTrack/camera.py` & `EdiHeadyTrack-0.1.0/EdiHeadyTrack/camera.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/EdiHeadyTrack/facedetector.py` & `EdiHeadyTrack-0.1.0/EdiHeadyTrack/facedetector.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/EdiHeadyTrack/filter.py` & `EdiHeadyTrack-0.1.0/EdiHeadyTrack/filter.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/EdiHeadyTrack/imu.py` & `EdiHeadyTrack-0.1.0/EdiHeadyTrack/imu.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/EdiHeadyTrack/plot.py` & `EdiHeadyTrack-0.1.0/EdiHeadyTrack/plot.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/EdiHeadyTrack/sensordata.py` & `EdiHeadyTrack-0.1.0/EdiHeadyTrack/sensordata.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/EdiHeadyTrack/video.py` & `EdiHeadyTrack-0.1.0/EdiHeadyTrack/video.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/PKG-INFO` & `EdiHeadyTrack-0.1.0/EdiHeadyTrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: EdiHeadyTrack
-Version: 0.0.6
+Version: 0.1.0
 Summary: Automatic, markerless measurement of head kinematics using mediapipe and OpenCV
 Home-page: https://github.com/isDynamics/EdiHeadyTrack
 Author: Thomas Aston
 Author-email: thomas.aston@ed.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) 
 [![Build Status - GitHub](https://github.com/isDynamics/EdiHeadyTrack/workflows/pytesting/badge.svg)](https://github.com/isDynamics/EdiHeadyTrack/actions/workflows/pytesting.yml)
 [![codecov](https://codecov.io/gh/isDynamics/EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)](https://codecov.io/gh/isDynamics/EdiHeadyTrack)
 [![Documentation Status](https://readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https://ediheadytrack.readthedocs.io/en/latest/?badge=latest)
 # EdiHeadyTrack
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.6 Summary: Automatic,
+Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.1.0 Summary: Automatic,
 markerless measurement of head kinematics using mediapipe and OpenCV Home-page:
 https://github.com/isDynamics/EdiHeadyTrack Author: Thomas Aston Author-email:
 thomas.aston@ed.ac.uk Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
-Description-Content-Type: text/markdown [![License: GPL v3](https://
-img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
-3.0) [![Build Status - GitHub](https://github.com/isDynamics/EdiHeadyTrack/
-workflows/pytesting/badge.svg)](https://github.com/isDynamics/EdiHeadyTrack/
-actions/workflows/pytesting.yml) [![codecov](https://codecov.io/gh/isDynamics/
-EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)](https://
-codecov.io/gh/isDynamics/EdiHeadyTrack) [![Documentation Status](https://
-readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https://
-ediheadytrack.readthedocs.io/en/latest/?badge=latest) # EdiHeadyTrack ##
+Description-Content-Type: text/markdown License-File: LICENSE [![License: GPL
+v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
+licenses/gpl-3.0) [![Build Status - GitHub](https://github.com/isDynamics/
+EdiHeadyTrack/workflows/pytesting/badge.svg)](https://github.com/isDynamics/
+EdiHeadyTrack/actions/workflows/pytesting.yml) [![codecov](https://codecov.io/
+gh/isDynamics/EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)]
+(https://codecov.io/gh/isDynamics/EdiHeadyTrack) [![Documentation Status]
+(https://readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https:/
+/ediheadytrack.readthedocs.io/en/latest/?badge=latest) # EdiHeadyTrack ##
 Contributors [https://contrib.rocks/image?repo=isDynamics/EdiHeadyTrack] Made
 with [contrib.rocks](https://contrib.rocks).  ## About EdiHeadyTrack is a
 Python package for measuring head kinematics using markerless head pose
 detection methods. The current implementation primarily uses the FaceMesh
 module of MediaPipe's Python API for facial landmark detection alongside OpenCV
 for handling simple computer vision tasks. Full documentation for EdiHeadyTrack
 can be found [here](https://ediheadytrack.readthedocs.io). ## Technologies
```

### Comparing `EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/SOURCES.txt` & `EdiHeadyTrack-0.1.0/EdiHeadyTrack.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 EdiHeadyTrack/__init__.py
 EdiHeadyTrack/camera.py
```

### Comparing `EdiHeadyTrack-0.0.6/PKG-INFO` & `EdiHeadyTrack-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: EdiHeadyTrack
-Version: 0.0.6
+Version: 0.1.0
 Summary: Automatic, markerless measurement of head kinematics using mediapipe and OpenCV
 Home-page: https://github.com/isDynamics/EdiHeadyTrack
 Author: Thomas Aston
 Author-email: thomas.aston@ed.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) 
 [![Build Status - GitHub](https://github.com/isDynamics/EdiHeadyTrack/workflows/pytesting/badge.svg)](https://github.com/isDynamics/EdiHeadyTrack/actions/workflows/pytesting.yml)
 [![codecov](https://codecov.io/gh/isDynamics/EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)](https://codecov.io/gh/isDynamics/EdiHeadyTrack)
 [![Documentation Status](https://readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https://ediheadytrack.readthedocs.io/en/latest/?badge=latest)
 # EdiHeadyTrack
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.6 Summary: Automatic,
+Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.1.0 Summary: Automatic,
 markerless measurement of head kinematics using mediapipe and OpenCV Home-page:
 https://github.com/isDynamics/EdiHeadyTrack Author: Thomas Aston Author-email:
 thomas.aston@ed.ac.uk Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
-Description-Content-Type: text/markdown [![License: GPL v3](https://
-img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
-3.0) [![Build Status - GitHub](https://github.com/isDynamics/EdiHeadyTrack/
-workflows/pytesting/badge.svg)](https://github.com/isDynamics/EdiHeadyTrack/
-actions/workflows/pytesting.yml) [![codecov](https://codecov.io/gh/isDynamics/
-EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)](https://
-codecov.io/gh/isDynamics/EdiHeadyTrack) [![Documentation Status](https://
-readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https://
-ediheadytrack.readthedocs.io/en/latest/?badge=latest) # EdiHeadyTrack ##
+Description-Content-Type: text/markdown License-File: LICENSE [![License: GPL
+v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
+licenses/gpl-3.0) [![Build Status - GitHub](https://github.com/isDynamics/
+EdiHeadyTrack/workflows/pytesting/badge.svg)](https://github.com/isDynamics/
+EdiHeadyTrack/actions/workflows/pytesting.yml) [![codecov](https://codecov.io/
+gh/isDynamics/EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)]
+(https://codecov.io/gh/isDynamics/EdiHeadyTrack) [![Documentation Status]
+(https://readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https:/
+/ediheadytrack.readthedocs.io/en/latest/?badge=latest) # EdiHeadyTrack ##
 Contributors [https://contrib.rocks/image?repo=isDynamics/EdiHeadyTrack] Made
 with [contrib.rocks](https://contrib.rocks).  ## About EdiHeadyTrack is a
 Python package for measuring head kinematics using markerless head pose
 detection methods. The current implementation primarily uses the FaceMesh
 module of MediaPipe's Python API for facial landmark detection alongside OpenCV
 for handling simple computer vision tasks. Full documentation for EdiHeadyTrack
 can be found [here](https://ediheadytrack.readthedocs.io). ## Technologies
```

### Comparing `EdiHeadyTrack-0.0.6/README.md` & `EdiHeadyTrack-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/setup.cfg` & `EdiHeadyTrack-0.1.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EdiHeadyTrack
-version = 0.0.6
+version = 0.1.0
 author = Thomas Aston
 author_email = thomas.aston@ed.ac.uk
 description = Automatic, markerless measurement of head kinematics using mediapipe and OpenCV
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/isDynamics/EdiHeadyTrack
 classifiers =
```

### Comparing `EdiHeadyTrack-0.0.6/test/test_camera.py` & `EdiHeadyTrack-0.1.0/test/test_camera.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/test/test_facedetector.py` & `EdiHeadyTrack-0.1.0/test/test_facedetector.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/test/test_filter.py` & `EdiHeadyTrack-0.1.0/test/test_filter.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/test/test_plot.py` & `EdiHeadyTrack-0.1.0/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/test/test_sensordata.py` & `EdiHeadyTrack-0.1.0/test/test_sensordata.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.6/test/test_video.py` & `EdiHeadyTrack-0.1.0/test/test_video.py`

 * *Files identical despite different names*

