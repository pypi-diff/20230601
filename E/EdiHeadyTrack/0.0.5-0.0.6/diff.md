# Comparing `tmp/EdiHeadyTrack-0.0.5.tar.gz` & `tmp/EdiHeadyTrack-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/thomas/Library/CloudStorage/OneDrive-UniversityofEdinburgh/PhD/1. Working/1. Computational/EdiHeadyTrack - PACKAGE SOURC", last modified: Tue May 16 08:50:06 2023, max compression
+gzip compressed data, was "/Users/thomas/Library/CloudStorage/OneDrive-UniversityofEdinburgh/PhD/1. Working/1. Computational/EdiHeadyTrack - PACKAGE SOURC", last modified: Thu Jun  1 13:04:20 2023, max compression
```

## Comparing `EdiHeadyTrack-0.0.5.tar` & `EdiHeadyTrack-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:50:06.138376 EdiHeadyTrack-0.0.5/
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:50:06.136115 EdiHeadyTrack-0.0.5/EdiHeadyTrack/
--rwxr-xr-x   0 thomas     (501) staff       (20)      475 2023-05-16 08:36:57.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/__init__.py
--rwxr-xr-x   0 thomas     (501) staff       (20)     8554 2023-05-12 13:09:34.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/calibration.py
--rw-r--r--   0 thomas     (501) staff       (20)     2883 2023-05-12 13:12:59.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/camera.py
--rwxr-xr-x   0 thomas     (501) staff       (20)    15161 2023-05-16 08:42:22.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/facedetector.py
--rw-r--r--   0 thomas     (501) staff       (20)     2763 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/filter.py
--rw-r--r--   0 thomas     (501) staff       (20)     5891 2023-05-12 13:40:15.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/head.py
--rw-r--r--   0 thomas     (501) staff       (20)     3370 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/imu.py
--rw-r--r--   0 thomas     (501) staff       (20)     1029 2023-05-16 07:56:28.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/load_sample.py
--rw-r--r--   0 thomas     (501) staff       (20)     9604 2023-05-16 08:43:03.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/plot.py
--rw-r--r--   0 thomas     (501) staff       (20)     1492 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/sensordata.py
--rw-r--r--   0 thomas     (501) staff       (20)     3278 2023-05-12 13:26:00.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack/video.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:50:06.137314 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/
--rw-r--r--   0 thomas     (501) staff       (20)     4383 2023-05-16 08:50:06.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)      588 2023-05-16 08:50:06.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/SOURCES.txt
--rw-r--r--   0 thomas     (501) staff       (20)        1 2023-05-16 08:50:06.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/dependency_links.txt
--rw-r--r--   0 thomas     (501) staff       (20)       78 2023-05-16 08:50:06.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/requires.txt
--rw-r--r--   0 thomas     (501) staff       (20)       19 2023-05-16 08:50:06.000000 EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/top_level.txt
--rw-r--r--   0 thomas     (501) staff       (20)    35149 2023-05-12 10:53:25.000000 EdiHeadyTrack-0.0.5/LICENSE
--rw-r--r--   0 thomas     (501) staff       (20)       33 2023-05-16 08:07:20.000000 EdiHeadyTrack-0.0.5/MANIFEST.in
--rw-r--r--   0 thomas     (501) staff       (20)     4383 2023-05-16 08:50:06.138482 EdiHeadyTrack-0.0.5/PKG-INFO
--rw-r--r--   0 thomas     (501) staff       (20)     3867 2023-05-12 14:52:31.000000 EdiHeadyTrack-0.0.5/README.md
--rw-r--r--   0 thomas     (501) staff       (20)       89 2023-05-12 09:37:25.000000 EdiHeadyTrack-0.0.5/pyproject.toml
--rw-r--r--   0 thomas     (501) staff       (20)      712 2023-05-16 08:50:06.138933 EdiHeadyTrack-0.0.5/setup.cfg
--rw-r--r--   0 thomas     (501) staff       (20)       76 2023-05-16 08:44:42.000000 EdiHeadyTrack-0.0.5/setup.py
-drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-05-16 08:50:06.138094 EdiHeadyTrack-0.0.5/test/
--rw-r--r--   0 thomas     (501) staff       (20)        0 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.5/test/__init__.py
--rw-r--r--   0 thomas     (501) staff       (20)     1274 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.5/test/test_calibrating.py
--rw-r--r--   0 thomas     (501) staff       (20)      230 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.5/test/test_logging.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:04:20.162830 EdiHeadyTrack-0.0.6/
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:04:20.157527 EdiHeadyTrack-0.0.6/EdiHeadyTrack/
+-rwxr-xr-x   0 thomas     (501) staff       (20)      384 2023-05-16 14:34:30.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)    10545 2023-05-30 10:21:02.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/camera.py
+-rwxr-xr-x   0 thomas     (501) staff       (20)     9787 2023-05-30 11:15:07.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/facedetector.py
+-rw-r--r--   0 thomas     (501) staff       (20)     2763 2023-05-10 12:57:57.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/filter.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1808 2023-05-30 14:02:35.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/imu.py
+-rw-r--r--   0 thomas     (501) staff       (20)     9423 2023-06-01 12:47:57.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/plot.py
+-rw-r--r--   0 thomas     (501) staff       (20)     7673 2023-05-30 13:13:46.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/sensordata.py
+-rw-r--r--   0 thomas     (501) staff       (20)     3279 2023-05-30 09:09:03.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack/video.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:04:20.158834 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/
+-rw-r--r--   0 thomas     (501) staff       (20)     4347 2023-06-01 13:04:20.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)      598 2023-06-01 13:04:20.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/SOURCES.txt
+-rw-r--r--   0 thomas     (501) staff       (20)        1 2023-06-01 13:04:20.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/dependency_links.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       78 2023-06-01 13:04:20.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/requires.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       19 2023-06-01 13:04:20.000000 EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/top_level.txt
+-rw-r--r--   0 thomas     (501) staff       (20)       33 2023-05-16 08:07:20.000000 EdiHeadyTrack-0.0.6/MANIFEST.in
+-rw-r--r--   0 thomas     (501) staff       (20)     4347 2023-06-01 13:04:20.162957 EdiHeadyTrack-0.0.6/PKG-INFO
+-rw-r--r--   0 thomas     (501) staff       (20)     3853 2023-05-30 15:20:09.000000 EdiHeadyTrack-0.0.6/README.md
+-rw-r--r--   0 thomas     (501) staff       (20)       89 2023-05-12 09:37:25.000000 EdiHeadyTrack-0.0.6/pyproject.toml
+-rw-r--r--   0 thomas     (501) staff       (20)      712 2023-06-01 13:04:20.163408 EdiHeadyTrack-0.0.6/setup.cfg
+-rw-r--r--   0 thomas     (501) staff       (20)       75 2023-05-16 08:58:57.000000 EdiHeadyTrack-0.0.6/setup.py
+drwxr-xr-x   0 thomas     (501) staff       (20)        0 2023-06-01 13:04:20.162539 EdiHeadyTrack-0.0.6/test/
+-rw-r--r--   0 thomas     (501) staff       (20)        0 2023-04-20 09:19:02.000000 EdiHeadyTrack-0.0.6/test/__init__.py
+-rw-r--r--   0 thomas     (501) staff       (20)      578 2023-05-30 11:14:27.000000 EdiHeadyTrack-0.0.6/test/test_camera.py
+-rw-r--r--   0 thomas     (501) staff       (20)      643 2023-05-30 11:27:51.000000 EdiHeadyTrack-0.0.6/test/test_facedetector.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1070 2023-05-30 13:48:57.000000 EdiHeadyTrack-0.0.6/test/test_filter.py
+-rw-r--r--   0 thomas     (501) staff       (20)      260 2023-05-30 14:13:57.000000 EdiHeadyTrack-0.0.6/test/test_imu.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1650 2023-05-31 11:17:25.000000 EdiHeadyTrack-0.0.6/test/test_plot.py
+-rw-r--r--   0 thomas     (501) staff       (20)     1258 2023-05-30 14:23:09.000000 EdiHeadyTrack-0.0.6/test/test_sensordata.py
+-rw-r--r--   0 thomas     (501) staff       (20)      635 2023-05-30 11:14:03.000000 EdiHeadyTrack-0.0.6/test/test_video.py
```

### Comparing `EdiHeadyTrack-0.0.5/EdiHeadyTrack/calibration.py` & `EdiHeadyTrack-0.0.6/EdiHeadyTrack/camera.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,88 @@
 # **************************************************************************** #
 #                                                                              #
 #                                                         :::      ::::::::    #
-#    calibration.py                                     :+:      :+:    :+:    #
+#    camera.py                                          :+:      :+:    :+:    #
 #                                                     +:+ +:+         +:+      #
 #    By: taston <thomas.aston@ed.ac.uk>             +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
-#    Created: 2023/04/25 10:20:08 by taston            #+#    #+#              #
-#    Updated: 2023/05/12 14:09:34 by taston           ###   ########.fr        #
+#    Created: 2023/04/25 15:41:23 by taston            #+#    #+#              #
+#    Updated: 2023/05/30 11:21:02 by taston           ###   ########.fr        #
 #                                                                              #
 # **************************************************************************** #
 
-import cv2 
 import numpy as np
+import cv2 
 from datetime import datetime
 from .video import Video
 
+class Camera:
+    """
+    A class used to represent a Camera.
+
+    ...
+
+    Attributes
+    ----------
+    focal_length : float
+        float representing the focal length of the Camera in mm
+    internal_matrix : ndarray
+        array representing the Camera's intrinsic parameters
+    distortion_matrix : ndarray
+        array representing the Camera's lens distortion parameters
+    calibrator : Calibrator
+        Calibrator object used for camera calibration
+    calibrated : bool
+        bool for quick checking if camera has been calibrated
+    video : Video
+        Video object where the footage has been shot using this Camera
+        
+    Methods
+    -------
+    calibrate(checkerboard=(9,6), video=Video()):
+        Performs calibration on the camera
+    """
+    def __init__(self):
+        """
+        Parameters
+        ----------
+        ...
+        """
+        
+        width = 1920
+        height = 1080
+        self.focal_length = height * 1.28
+        self.internal_matrix = np.array([[self.focal_length, 0, width/2],
+                                          [0, self.focal_length, height/2],
+                                          [0, 0, 1]])
+        self.distortion_matrix = np.zeros((4, 1), dtype=np.float64)
+        self.calibrated = False
+
+    
+    def calibrate(self, checkerboard=(9,6), video=Video(), show=True):
+        """Creates a calibrator object and calibrates the Camera.
+
+        If arguments checkerboard and video aren't passed in, the
+        default checkerboard pattern and an empty video are used.
+
+        Parameters
+        ----------
+        checkerboard : tuple, optional
+            Checkerboard pattern used in camera calibration (default is 9x6)
+        video : Video, optional
+            Video used to calibrate camera
+        """
+        
+        self.video = video
+        self.calibrator = Calibrator(checkerboard, self.video, show)
+        self.calibrated = True
+
+        return self
+    
+
 class Checkerboard:
     """
     A class used to represent a calibration Checkerboard
 
     ...
     
     Attributes
@@ -83,14 +147,15 @@
                             gray_frame, self.dimensions,
                             cv2.CALIB_CB_ADAPTIVE_THRESH
                             + cv2.CALIB_CB_FAST_CHECK +
                             cv2.CALIB_CB_NORMALIZE_IMAGE)
 
         return ret, corners
 
+
 class Calibrator:
     """
     A class used to represent a camera Calibrator
 
     ...
     
     Attributes
@@ -118,25 +183,26 @@
         Perform camera calibration process
     draw_corners(corners)
         Draw checkerboard corners on video frame
     save_outputs()
         Save camera parameters to csv files
     """
 
-    def __init__(self, checkerboard, video=Video()):
+    def __init__(self, checkerboard, video=Video(), show=True):
         """
         Parameters
         ----------
         checkerboard : tuple
             tuple representing Checkerboard pattern
         video : Video, optional
             Video used for camera calibration. If no video specified
             an empty video will be attempted.
         """
         timestamp = datetime.now().strftime("%H:%M:%S")
+        self.show = show
         self.video = video
         print('-'*120)
         print('{:<100} {:>19}'.format(f'Creating Calibrator object for video {self.video.filename}:', timestamp))
         print('-'*120)
         print(self.video)
         self.checkerboard = Checkerboard(checkerboard)
         print(f'Checkerboard dimensions: {self.checkerboard.dimensions[0]} x {self.checkerboard.dimensions[1]}')
@@ -162,15 +228,17 @@
             ret, self.frame = self.video.cap.read()
             frame_number = int(self.video.cap.get(cv2.CAP_PROP_POS_FRAMES))
             self.gray_frame = cv2.cvtColor(self.frame, cv2.COLOR_BGR2GRAY)
             ret, corners = self.checkerboard.get_corners(self.gray_frame)
             if ret:
                 complete, image = self.draw_corners(corners)
             if complete: break
-            cv2.imshow('Calibrating...', self.frame)
+
+            if self.show == True:
+                cv2.imshow('Calibrating...', self.frame)
             self.video.writer.write(self.frame)
             k = cv2.waitKey(1)
             if k == 27:
                 self.video.cap.release()
                 self.video.writer.release()
                 cv2.destroyAllWindows()
                 break
@@ -224,9 +292,11 @@
     def save_outputs(self):
         """
         Saves matrices to csv
         """
         timestamp = datetime.now().strftime("%H:%M:%S")
         print('Saving outputs...')
         from numpy import savetxt
-        savetxt('EdiHeadyTrack/resources/camera_matrix.csv', self.matrix, delimiter=',')
-        savetxt('EdiHeadyTrack/resources/camera_distortion.csv', self.distortion, delimiter=',')
+        savetxt('camera_matrix.csv', self.matrix, delimiter=',')
+        savetxt('camera_distortion.csv', self.distortion, delimiter=',')
+
+        return
```

### Comparing `EdiHeadyTrack-0.0.5/EdiHeadyTrack/facedetector.py` & `EdiHeadyTrack-0.0.6/EdiHeadyTrack/facedetector.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #                                                                              #
 #                                                         :::      ::::::::    #
 #    facedetector.py                                    :+:      :+:    :+:    #
 #                                                     +:+ +:+         +:+      #
 #    By: taston <thomas.aston@ed.ac.uk>             +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2023/02/10 16:43:13 by taston            #+#    #+#              #
-#    Updated: 2023/05/16 09:42:22 by taston           ###   ########.fr        #
+#    Updated: 2023/05/30 12:15:07 by taston           ###   ########.fr        #
 #                                                                              #
 # **************************************************************************** #
 
 import cv2
 import mediapipe as mp
 import numpy as np
 from numpy import genfromtxt
@@ -31,22 +31,23 @@
     camera : Camera, optional
         Camera object to be used with FaceDetector
     face2d : dict
         dict of detected face points in 2d
     face3d : list
         list of known 3d face points (from mesh model)
     """
-    def __init__(self, video=Video(), camera=Camera()):
+    def __init__(self, video=Video(), camera=Camera(), show=True):
         self.camera = camera
         self.video = video
         self.face2d = {'time': [],
                        'frame': [],
                        'key landmark positions':    [],
                        'all landmark positions':    []}
         self.face3d = []
+        self.show = show
 
 class MediaPipe(FaceDetector):
     """
     A class for representing a MediaPipe FaceDetector
 
     ...
     
@@ -81,15 +82,15 @@
     Methods
     -------
     find_faces(img)
         search for faces in a given frame
     run()
         run through the tracking procedure using MediaPipe face mesh
     """
-    def __init__(self, video=Video(), camera=Camera(),
+    def __init__(self, video=Video(), camera=Camera(), show=True,
                  staticMode=False, maxFaces=1, refineLandmarks=False, minDetectionCon=0.5, minTrackCon=0.5):
         """
         Parameters
         ----------
         video : Video, optional
             video to perform head pose estimation on (default is empty Video)
         camera : Camera, optional
@@ -101,28 +102,27 @@
         refineLandmarks : bool, optional
             flag setting if landmarks should be refined or not (default False)
         minDetectionCon : float, optional
             minimum detection confidence (default 0.5)
         minTrackCon : float, optional
             minimum tracking confidence (default 0.5)
         """
-        super().__init__(video, camera)
+        super().__init__(video, camera, show)
         timestamp = datetime.now().strftime("%H:%M:%S")
         print('-'*120)
         print('{:<100} {:>19}'.format(f'Creating MediaPipe object for video {self.video.filename}:', timestamp))
         print('-'*120)
         print(self.video)
         self.staticMode = staticMode
         self.refineLandmarks = refineLandmarks
         self.maxFaces = maxFaces
         self.minDetectionCon = minDetectionCon
         self.minTrackCon = minTrackCon
         self.mpDraw = mp.solutions.drawing_utils
         self.mpFaceMesh = mp.solutions.face_mesh
-        print(type(self.mpDraw), type(self.mpFaceMesh))
         self.faceMesh = self.mpFaceMesh.FaceMesh(self.staticMode,
                                                  self.maxFaces,
                                                  self.refineLandmarks,
                                                  self.minDetectionCon,
                                                  self.minTrackCon)
         self.drawSpec = self.mpDraw.DrawingSpec(thickness=1, circle_radius=2)
         self.key_landmarks = [33, 263, 1, 61, 291, 199]
@@ -145,35 +145,50 @@
                        [-4.445859, 2.663991, 3.173422], # 33
                        [-2.456206,	-4.342621, 4.283884], # 61
                        [0, -9.403378, 4.264492], # 199
                        [4.445859, 2.663991, 3.173422], # 263
                        [2.456206, -4.342621, 4.283884]] # 291
         
         progress_bar = tqdm(range(self.video.total_frames))
+        out = cv2.VideoWriter('tracking.mp4',
+                              cv2.VideoWriter_fourcc(*'mp4v'),
+                              self.video.fps,
+                              (self.video.width,self.video.height))
+        # self.video.create_writer('tracking.mp4')
         self.tracking_frames = []
         while True:
             success, img = self.video.cap.read()
             if success:
                 progress_bar.update(1)
                 # current_frame = int(self.video.cap.get(1))
                 self.find_faces(img)
-                cv2.namedWindow("EdiHeadyTrack", cv2.WINDOW_NORMAL)
-                cv2.resizeWindow("EdiHeadyTrack", int(self.video.width/2), int(self.video.height/2))
-                cv2.imshow("EdiHeadyTrack", img)
+                if self.show == True:
+                    cv2.namedWindow("EdiHeadyTrack", cv2.WINDOW_NORMAL)
+                    cv2.resizeWindow("EdiHeadyTrack", int(self.video.width/2), int(self.video.height/2))
+                    cv2.imshow("EdiHeadyTrack", img)
                 # cv2.imwrite(f'tracking frames/{current_frame}.png', img)
-                
+                # self.video.writer.write(img)
+                out.write(img)
                 if cv2.waitKey(5) & 0xFF == ord('q'):
+                    self.video.cap.release()
+                    out.release()
+                    cv2.destroyAllWindows()
                     progress_bar.close()
                     print('Face tracking interuppted...')
                     break     
             else:
+                self.video.cap.release()
+                out.release()
+                cv2.destroyAllWindows()
                 progress_bar.close()
                 print('Face tracking complete...')
                 break
 
+        return
+
     def find_faces(self, img):
         """Finds faces in a supplied image
 
         Parameters
         ----------
         img : ndarray
             ndarray representing the image in which faces should be found
@@ -201,162 +216,22 @@
                     y = int(lm.y * self.video.height)
 
                     landmark_position = [x,y]
                     landmark_positions.append(landmark_position)
                     
                     if idx in self.key_landmarks:
                         if idx == 1:
-                            nose2d = (lm.x * self.video.width, lm.y * self.video.height)
+                            self.nose2d = (lm.x * self.video.width, lm.y * self.video.height)
                             nose3d = (lm.x * self.video.width, lm.y * self.video.height, lm.z * 3000)
 
+                            
                         key_landmark_positions.append(landmark_position)
-                
+
                 self.face2d['all landmark positions'].append(landmark_positions)
                 self.face2d['key landmark positions'].append(key_landmark_positions)
 
         self.tracking_frames.append(cv2.cvtColor(img, cv2.COLOR_BGR2RGB))
+        
         return
     
     def __str__(self):
-        return f'MediaPipe Face Detector with video {self.video.filename}'
-
-
-# class OpenPose(FaceDetector):
-#     def __init__(self):
-#         ...
-
-# class FaceMeshDetector():
-#     def __init__(self, staticMode=False, maxFaces=2, refineLandmarks=False, minDetectionCon=0.5, minTrackCon=0.5):
-#         '''
-#         Initialise object
-#         '''
-#         self.staticMode = staticMode
-#         self.maxFaces = maxFaces
-#         self.refineLandmarks = refineLandmarks
-#         self.minDetectionCon = minDetectionCon
-#         self.minTrackCon = minTrackCon
-
-#         self.mpDraw = mp.solutions.drawing_utils
-#         self.mpFaceMesh = mp.solutions.face_mesh
-#         self.faceMesh = self.mpFaceMesh.FaceMesh(self.staticMode,
-#                                                  self.maxFaces,
-#                                                  self.refineLandmarks,
-#                                                  self.minDetectionCon,
-#                                                  self.minTrackCon)
-#         self.drawSpec = self.mpDraw.DrawingSpec(thickness=1, circle_radius=2)
-
-#     def findFaceMesh(self, img, draw=True):
-#         '''
-#         Finds face mesh and draws it
-#         '''
-#         img.flags.writeable = False
-#         self.imgRGB = cv2.cvtColor(img, cv2.COLOR_BGR2RGB)
-#         ih, iw, ic = img.shape
-#         self.results = self.faceMesh.process(self.imgRGB)
-#         face = {
-#                     "x": [],
-#                     "y": [],
-#                     "z": [],
-#                     "x_av": None,
-#                     "y_av": None,
-#                     "yaw": None,
-#                     "pitch": None,
-#                     "roll": None
-#                 }
-#         p1 = (0, 0)
-#         p2 = (0, 0)
-#         face_2d = []
-#         face_3d = [[0, -1.126865, 7.475604], # 1
-#                    [-4.445859, 2.663991, 3.173422], # 33
-#                    [-2.456206,	-4.342621, 4.283884], # 61
-#                    [0, -9.403378, 4.264492], # 199
-#                    [4.445859, 2.663991, 3.173422], # 263
-#                    [2.456206, -4.342621, 4.283884]] # 291
-
-#         key_landmarks = [33, 263, 1, 61, 291, 199]
-#         # If something detected
-#         if self.results.multi_face_landmarks:
-#             faces = []
-#             for faceLandmarks in self.results.multi_face_landmarks:
-#                 # self.mpDraw.draw_landmarks(img, faceLandmarks, self.mpFaceMesh.FACEMESH_TESSELATION,
-#                 #                             self.drawSpec,self.drawSpec)
-#                 self.mpDraw.draw_landmarks(img, 
-#                                            faceLandmarks, 
-#                                            self.mpFaceMesh.FACEMESH_TESSELATION,
-#                                            None,
-#                                            mp.solutions.drawing_styles
-#                                            .get_default_face_mesh_tesselation_style())
-
-                
-#                 # Get landmarks
-#                 for idx, lm in enumerate(faceLandmarks.landmark):
-                    
-#                     face["x"].append(int(lm.x*iw))
-#                     face["y"].append(int(lm.y*ih))  
-#                     face["z"].append(lm.z)
-#                     if idx in key_landmarks:
-#                         if idx == 1:
-#                             nose_2d = (lm.x * iw, lm.y * ih)
-#                             nose_3d = (lm.x * iw, lm.y*ih, lm.z * 3000)
-
-#                         x, y = int(lm.x * iw), int(lm.y * ih)
-#                         face_2d.append([x, y])
-#                         # face_3d.append([x, y, lm.z])
-
-#                 faces.append(face)
-#                 # face_2d = [face["x"], face["y"]]
-#                 # face_3d = [face["x"], face["y"], face["z"]]
-#                 face_2d = np.array(face_2d, dtype=np.float64)
-#                 face_3d = np.array(face_3d, dtype=np.float64)
-#                 # print(face_2d)
-#                 # print(face_3d)
-#                 # Camera properties
-#                 # camera_matrix = genfromtxt('camera_matrix.csv', delimiter=',')
-#                 # print(camera_matrix)
-#                 # distortion_matrix = genfromtxt('camera_distortion.csv', delimiter=',')
-                
-#                 focal_length = ih * 1.28
-#                 camera_matrix = np.array([[focal_length, 0, iw/2],
-#                                           [0, focal_length, ih/2],
-#                                           [0, 0, 1]])
-#                 distortion_matrix = np.zeros((4, 1), dtype=np.float64)
-    
-#                 # Solve PnP
-#                 success, rot_vec, trans_vec = cv2.solvePnP(face_3d, face_2d, camera_matrix, distortion_matrix, flags=cv2.SOLVEPNP_ITERATIVE)
-                    
-#                 # Rotational matrix
-#                 rmat = cv2.Rodrigues(rot_vec)[0]
-
-#                 # Get angles
-#                 P = np.hstack((rmat, np.zeros((3, 1), dtype=np.float64)))
-#                 eulerAngles =  cv2.decomposeProjectionMatrix(P)[6]
-#                 yaw   = eulerAngles[1, 0]
-#                 pitch = eulerAngles[0, 0]
-#                 roll  = eulerAngles[2, 0] 
-                
-#                 # Angle correction performed to centre around zero
-#                 if pitch < 0:
-#                     pitch = - 180 - pitch
-#                 elif pitch >= 0: 
-#                     pitch = 180 - pitch
-
-#                 # Define points for direction line drawn on face
-#                 if nose_2d:
-#                     p1 = (int(nose_2d[0]), int(nose_2d[1]))
-#                     p2 = (int(nose_2d[0] - yaw * 2), int(nose_2d[1] - pitch * 2))
-
-        
-#         else:
-#             faces = None 
-            
-#         if faces:
-#             for face in faces:
-#                 if face["x"]:
-#                     face["x_av"] = np.average(face["x"])
-#                     face["y_av"] = np.average(face["y"])
-#                     face["yaw"] = yaw
-#                     face["pitch"] = pitch
-#                     face["roll"] = roll
-        
-        
-#         return img, face, faces, p1, p2
-    
+        return f'MediaPipe Face Detector with video {self.video.filename}'
```

### Comparing `EdiHeadyTrack-0.0.5/EdiHeadyTrack/filter.py` & `EdiHeadyTrack-0.0.6/EdiHeadyTrack/filter.py`

 * *Files identical despite different names*

### Comparing `EdiHeadyTrack-0.0.5/EdiHeadyTrack/head.py` & `EdiHeadyTrack-0.0.6/EdiHeadyTrack/sensordata.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,47 @@
 # **************************************************************************** #
 #                                                                              #
 #                                                         :::      ::::::::    #
-#    head.py                                            :+:      :+:    :+:    #
+#    sensordata.py                                      :+:      :+:    :+:    #
 #                                                     +:+ +:+         +:+      #
 #    By: taston <thomas.aston@ed.ac.uk>             +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
-#    Created: 2023/04/26 11:14:49 by taston            #+#    #+#              #
-#    Updated: 2023/05/12 14:40:15 by taston           ###   ########.fr        #
+#    Created: 2023/04/25 15:35:24 by taston            #+#    #+#              #
+#    Updated: 2023/05/30 14:13:46 by taston           ###   ########.fr        #
 #                                                                              #
 # **************************************************************************** #
 
 import cv2
 import numpy as np
 from datetime import datetime
 import pandas as pd
 from .facedetector import FaceDetector
 from .filter import Filter
-from .sensordata import SensorData
+
+class SensorData:
+    """
+    A class representing SensorData
+
+    Attributes
+    ----------
+    velocity : dict
+        time history of rotational velocities
+    acceleration : dict
+        time history of rotational accelerations
+    """
+    def __init__(self):
+        self.velocity = {'time':    [],
+                         'yaw':     [],
+                         'pitch':   [],
+                         'roll':    []}
+        self.acceleration = {'time':    [],
+                             'yaw':     [],
+                             'pitch':   [],
+                             'roll':    []}
+        
 
 class Head(SensorData):
     """
     A class used to represent a Head obtained using head pose estimation
     techniques
 
     ...
@@ -41,35 +62,36 @@
     apply_filter(filter)
         applies filter to head pose data
     calculate_kinematics()
         calculates kinematic data from pose time history
     calculate_pose()
         computes HeadPose from detected facial landmarks
     """
-    counter = 0
-    def __init__(self, facedetector=FaceDetector(), id=counter):
+    _counter = 0
+    
+    def __init__(self, facedetector=FaceDetector(), id=_counter):
         """
         Parameters
         ----------
         facedetector : FaceDetector, optional
             the FaceDetector object used to find the Head (default FaceDetector())
         id : str, int, float, optional
             unique identifier for each Head object (defaults to count of existing heads)
         """
         timestamp = datetime.now().strftime("%H:%M:%S")
         print('-'*120)
         print('{:<100} {:>19}'.format(f'Creating Head object for {facedetector}:', timestamp))
         print('-'*120)
         super().__init__()
-        Head.counter += 1
+        Head._counter += 1
         self.facedetector = facedetector
-        # if id:
-        self.id = id
-        # # else:
-        #     self.id = id
+        if id:
+            self.id = id
+        else:
+            self.id = Head._counter
         self.pose = {'time':    [],
                      'yaw':     [],
                      'pitch':   [],
                      'roll':    []}
         
         self.calculate_pose()
         self.calculate_kinematics()
@@ -135,26 +157,65 @@
             elif pitch >= 0: 
                 pitch = 180 - pitch
             
             self.pose['yaw'].append(yaw)
             self.pose['pitch'].append(pitch)
             self.pose['roll'].append(roll)
 
+            if self.facedetector.nose2d:
+                    nose2d = self.facedetector.nose2d
+                    p1 = (int(nose2d[0]), int(nose2d[1]))
+                    p2 = (int(nose2d[0] - yaw * 2), int(nose2d[1] - pitch * 2))
+
+        return
+
     def calculate_kinematics(self):
         """
         Calculates kinematic data from pose time history
         """
         # print('Calculating kinematic data from head pose...')
 
         self.velocity['time'] = self.pose['time'][1:]
         self.acceleration['time'] = self.pose['time'][2:]
 
         for key in list(self.pose.keys())[1:]:
             self.velocity[key] = np.diff(np.array(self.pose[key])) / np.diff(np.array(self.pose['time']))
             self.acceleration[key] = np.diff(np.array(self.velocity[key])) / np.diff(np.array(self.velocity['time']))
 
+        return self
 
 
+class IMU(SensorData):
+    """
+    A class used to represent an IMU
 
-
+    ...
     
-    
+    Attributes
+    ----------
+    filename : str
+        file containing IMU sensor data
+    id : int, float, str
+        unique identifier given to IMU
+    time_offset : float
+        time offset applied to IMU data to sync with head pose data
+    """
+    _counter = 0
+    def __init__(self, filename=None, time_offset=0, id=_counter):
+        """
+        Parameters
+        ----------
+        filename : str
+            file containing IMU sensor data
+        id : int, float, str
+            unique identifier given to IMU
+        time_offset : float
+            time offset applied to IMU data to sync with head pose data
+        """
+        super().__init__()
+        IMU._counter += 1
+        self.filename = filename
+        self.time_offset = time_offset
+        if id:
+            self.id = id
+        else:
+            self.id = IMU._counter
```

### Comparing `EdiHeadyTrack-0.0.5/EdiHeadyTrack/plot.py` & `EdiHeadyTrack-0.0.6/EdiHeadyTrack/plot.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,130 +2,58 @@
 #                                                                              #
 #                                                         :::      ::::::::    #
 #    plot.py                                            :+:      :+:    :+:    #
 #                                                     +:+ +:+         +:+      #
 #    By: taston <thomas.aston@ed.ac.uk>             +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2023/04/27 10:18:49 by taston            #+#    #+#              #
-#    Updated: 2023/05/16 09:43:03 by taston           ###   ########.fr        #
+#    Updated: 2023/06/01 13:47:57 by taston           ###   ########.fr        #
 #                                                                              #
 # **************************************************************************** #
 
 
-from .head import Head
-from .imu import IMU
-from .sensordata import SensorData
+from .imu import Wax9
+from .sensordata import *
 import matplotlib.pyplot as plt
 from matplotlib.offsetbox import (TextArea, DrawingArea, OffsetImage,
                                   AnnotationBbox)
 
 class Plot:
     """
     A class representing a Plot
 
     ...
     
     Attributes
     ----------
     colors : list
         list of colors used in plots
+    sensors : list, SensorData
+        list of SensorData objects to be plotted
+    lines : list, dict 
+        list of dicts containing data of each line being plotted 
 
     Methods
     -------
-    plot_comparison(property, xlim, ylim, key_times, *sensors)
+    plot_propertyplot_property(self, property='velocity', xlim=None, ylim=None, key_times=[], show=True):
         plots a time comparison between sensor data
-    plot_head(property, *heads)
-        plots head pose estimation data only
-    plot_imu(property, time_range, *imus)
-        plots IMU data only
     """
-    def __init__(self):
+    def __init__(self, *sensors):
         self.colors = []
-
-    def plot_head(self, property, *heads):
-        """Plots head pose estimation data only
-        
-        Parameters
-        ----------
-        property : str
-            specifies which property to be plotted (from ('pose', 'velocity', 'acceleration')
-        *heads : Head
-            head objects to be plotted
-        """
-        plt.rcParams.update({'font.size': 14})
-        fig = plt.figure('EdiHeadyTrack - Head Data Plotting') #,figsize=[7,7])    
-        
-        for head in heads:
-            if not isinstance(head, Head):
-                raise TypeError(f'Attempted to plot type {type(head)}. Only Head objects may be plotted here!')
-            
-            if hasattr(head, property):
-                property_dict = getattr(head, property)
-                for idx, key in enumerate(list(property_dict.keys())[1:]):
-                    ax = plt.subplot(len(list(property_dict.keys()))-1, 1, idx+1)
-                    ax.grid(color='0.95')
-                    if property == 'pose':
-                        ax.set_ylabel(r'$\theta$ (deg)')
-                    elif property == 'velocity':
-                        ax.set_ylabel(r'$\omega$ (deg/s)')
-                    elif property =='acceleration':
-                        ax.set_ylabel(r'$\alpha$ (deg/s$^2$)')
-
-                    ax.plot(property_dict['time'], property_dict[key], label=f'{head.id} {key}')
-                    ax.legend(loc='best')
-
-        plt.xlabel(r'Time (s)')
-        plt.tight_layout()
-
-        plt.show()
-
-    def plot_imu(self, property, time_range, *imus):
-        """Plots head pose estimation data only
-        
-        Parameters
-        ----------
-        property : str
-            specifies which property to be plotted (from ('pose', 'velocity', 'acceleration')
-        time_range : tuple, float
-            range of times to be plotted over (lower limit, upper limit)
-        *imus : IMU
-            IMU objects to be plotted
-        """
-        plt.rcParams.update({'font.size': 14})
-        fig = plt.figure('EdiHeadyTrack - Head Data Plotting',figsize=[7,7])    
-
-        for imu in imus:
-            if not isinstance(imu, IMU):
-                raise TypeError(f'Attempted to plot type {type(imu)}. Only IMU objects may be plotted here!')
-
-            if hasattr(imu, property):
-                property_dict = getattr(imu, property)
-                for idx, key in enumerate(list(property_dict.keys())[1:]):
-                    ax = plt.subplot(len(list(property_dict.keys()))-1, 1, idx+1)
-                    ax.grid(color='0.95')
-                    if property == 'pose':
-                        ax.set_ylabel(r'$\theta$ (deg)')
-                    elif property == 'velocity':
-                        ax.set_ylabel(r'$\omega$ (deg/s)')
-                    elif property =='acceleration':
-                        ax.set_ylabel(r'$\alpha$ (deg/s$^2$)')
-
-                    if time_range:
-                        ax.set_xlim(time_range)
-
-                    ax.plot(property_dict['time'], property_dict[key], label=f'{imu.id} {key}')
-                    ax.legend(loc='best')
-
-        plt.xlabel(r'Time (s)')
-        plt.tight_layout()
-
-        plt.show()
+        self.sensors = []
+        self.lines = []
+        for sensor in sensors:
+            if not isinstance(sensor, SensorData):
+                raise TypeError(f'Attempted to plot type {type(sensor)}. Only SensorData objects may be plotted here!')
+            else:
+                self.sensors.append(sensor)
 
 
-    def plot_comparison(self, property, xlim, ylim, key_times=[], *sensors):
+    def plot_property(self, property='velocity', 
+                      xlim=None, ylim=None, key_times=[], show=True):
         """Plots comparison between sensor data
         
         Parameters
         ----------
         property : str
             specifies which property to be plotted (from ('pose', 'velocity', 'acceleration')
         xlim : tuple, float
@@ -136,48 +64,81 @@
             key time points to display frame images for 
         *sensors : SensorData
             sensor data objects to be added to plot
         """
         plt.rcParams.update({'font.size': 14})
         fig = plt.figure('EdiHeadyTrack - Head Data Plotting',figsize=[6,8])    
 
-        key_frames = [int(240*time) for time in key_times]
-
-        for sensor in sensors:
-            if not isinstance(sensor, SensorData):
-                raise TypeError(f'Attempted to plot type {type(sensor)}. Only SensorData objects may be plotted here!')
+        # if key_times:
+        #     key_frames = [int(240*time) for time in key_times]
 
+        for sensor in self.sensors:
             if hasattr(sensor, property):
                 property_dict = getattr(sensor, property)
                 for idx, key in enumerate(list(property_dict.keys())[1:]):
+                    
                     ax = plt.subplot(len(list(property_dict.keys())), 1, idx+2)
                     ax.grid(color='0.95')
                     if property == 'pose':
                         ax.set_ylabel(fr'$\theta_{{{key}}}$ (deg)')
                     elif property == 'velocity':
                         ax.set_ylabel(fr'$\omega_{{{key}}}$ (deg/s)')
                     elif property =='acceleration':
                         ax.set_ylabel(fr'$\alpha_{{{key}}}$ (deg/s$^2$)')
 
                     if xlim:
                         ax.set_xlim(xlim)
-                    if ylim:
-                        ax.set_ylim(ylim)
 
-                    for time in key_times:
-                        ax.axvline(x=time, color='green', ls=':')
-                    
+                    # TODO: improve method of using different colors.
+                    #       Maybe use 
+                    lims = []
                     if isinstance(sensor, Head):
-                        ax.plot(property_dict['time'], property_dict[key], label=f'{sensor.id}', color='c', ls='dashed')
+                        x_data = property_dict['time']
+                        y_data = property_dict[key]
+                        if xlim:
+                            for lim in xlim:
+                                for idx, time in enumerate(x_data):
+                                    if time > lim:
+                                        lims.append(idx)
+                                        break
+                            x_data = x_data[lims[0]:lims[1]]
+                            y_data = y_data[lims[0]:lims[1]]
+                        line, = ax.plot(x_data, 
+                                        y_data, 
+                                        label=f'{sensor.id}', 
+                                        color='c', ls='dashed')
+        
+                        self.lines.append({'sensor':    sensor.id,
+                                           'property':  f'{key}, {property}',
+                                           'values':    y_data})
+                        if key_times:
+                            key_frames = [int(sensor.facedetector.video.fps*time) for time in key_times]
+                            
                     elif isinstance(sensor, IMU):
-                        ax.plot(property_dict['time'], property_dict[key], label=f'{sensor.id}', color='k')
-
-                    # ax.set_ylim(min(property_dict[key] - abs(min(property_dict[key])/10)) , max(property_dict[key] + abs(max(property_dict[key])/10)))
-                    ax.set_ylim(-220, 220)
-
+                        x_data = property_dict['time']
+                        y_data = property_dict[key]
+                        if xlim:
+                            for lim in xlim:
+                                for idx, time in enumerate(x_data):
+                                    if time > lim:
+                                        lims.append(idx)
+                                        break
+                            x_data = x_data[lims[0]:lims[1]]
+                            y_data = y_data[lims[0]:lims[1]]
+                        line, = ax.plot(x_data, 
+                                        y_data, 
+                                        label=f'{sensor.id}', 
+                                        color='k')
+                        self.lines.append({'sensor':    sensor.id,
+                                           'property':  f'{key}, {property}',
+                                           'values':    y_data})
+            
+                    for time in key_times:
+                        ax.axvline(x=time, color='green', ls=':')
+                        
                     if idx + 2 != len(list(property_dict.keys())):
                         plt.setp(ax.get_xticklabels(), visible=False)
                     else:
                         ax.set_xlabel(r'Time (s)')
                     
                     if idx + 2 == 3: 
                         handles, labels = ax.get_legend_handles_labels()
@@ -185,38 +146,65 @@
 
         ax1 = plt.subplot(411, sharex=ax)
         for time in key_times:
             ax1.axvline(x=time, color='green', ls=':')
         plt.setp(ax1.get_xticklabels(), visible=False)
         plt.setp(ax1.get_yticklabels(), visible=False)
 
-        for sensor in sensors:
-            if isinstance(sensor, Head):
-                for idx, frame in enumerate(key_frames):
-                    img = sensor.facedetector.tracking_frames[frame]
-
-                    frame_index = sensor.facedetector.face2d['frame'].index(frame)
-                    x_list = [pos[0] for pos in sensor.facedetector.face2d['all landmark positions'][frame_index]]
-                    y_list = [pos[1] for pos in sensor.facedetector.face2d['all landmark positions'][frame_index]]
-                    
-                    top_bound = max(0, min(y_list[:]) - 200)
-                    bottom_bound = min(sensor.facedetector.video.height, max(y_list[:]) + 200)
-                    left_bound = max(0, min(x_list[:]) - 200)
-                    right_bound = min(sensor.facedetector.video.width, max(x_list[:]) + 200)
-                    
-                    img = img[top_bound:bottom_bound, left_bound:right_bound, :]
-
-                    imagebox = OffsetImage(img, zoom=0.08)
-                    imagebox.image.axes = ax1
-
-                    ab = AnnotationBbox(imagebox, [key_times[idx],0.5],
-                                        xybox=(1, 1),
-                                        xycoords='data',
-                                        boxcoords="offset points",
-                                        pad=0.01,
-                                        bboxprops =dict(edgecolor='white')
-                                        )
+        if key_times:
+            for sensor in self.sensors:
+                if isinstance(sensor, Head):
+                    for idx, frame in enumerate(key_frames):
+                        img = sensor.facedetector.tracking_frames[frame]
+
+                        frame_index = sensor.facedetector.face2d['frame'].index(frame)
+                        x_list = [pos[0] for pos in sensor.facedetector.face2d['all landmark positions'][frame_index]]
+                        y_list = [pos[1] for pos in sensor.facedetector.face2d['all landmark positions'][frame_index]]
+                        
+                        top_bound = max(0, min(y_list[:]) - 200)
+                        bottom_bound = min(sensor.facedetector.video.height, max(y_list[:]) + 200)
+                        left_bound = max(0, min(x_list[:]) - 200)
+                        right_bound = min(sensor.facedetector.video.width, max(x_list[:]) + 200)
+                        
+                        img = img[top_bound:bottom_bound, left_bound:right_bound, :]
+
+                        imagebox = OffsetImage(img, zoom=0.08)
+                        imagebox.image.axes = ax1
+
+                        ab = AnnotationBbox(imagebox, [key_times[idx],0.5],
+                                            xybox=(1, 1),
+                                            xycoords='data',
+                                            boxcoords="offset points",
+                                            pad=0.01,
+                                            bboxprops =dict(edgecolor='white')
+                                            )
 
-                    ax1.add_artist(ab)
+                        ax1.add_artist(ab)
         
         # plt.savefig('resources/comparison.png', bbox_inches='tight')
-        plt.show()
+        if show == True:
+            plt.show()
+        
+        return self
+
+    def summarise(self):
+        '''
+        Produces a summary of the maximum values of each line in a 
+        Plot object.
+        '''
+        sensor_prev = None
+        for line in self.lines:
+            sensor = line['sensor']
+
+            if sensor != sensor_prev:
+                print('-'*46)
+                print(f'{sensor} plot summary')
+                print('-'*46)
+                print('{:<30} {:>15}'.format(line['property'], 
+                                             round(max(abs(line['values'])), 2)))
+            else:
+                print('{:<30} {:>15}'.format(line['property'], 
+                                             round(max(abs(line['values'])), 2)))
+            
+            sensor_prev = sensor
+        
+        print('-'*46)
```

### Comparing `EdiHeadyTrack-0.0.5/EdiHeadyTrack/video.py` & `EdiHeadyTrack-0.0.6/EdiHeadyTrack/video.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #                                                                              #
 #                                                         :::      ::::::::    #
 #    video.py                                           :+:      :+:    :+:    #
 #                                                     +:+ +:+         +:+      #
 #    By: taston <thomas.aston@ed.ac.uk>             +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2023/04/25 10:00:46 by taston            #+#    #+#              #
-#    Updated: 2023/05/12 14:26:00 by taston           ###   ########.fr        #
+#    Updated: 2023/05/30 10:09:03 by taston           ###   ########.fr        #
 #                                                                              #
 # **************************************************************************** #
 
 import cv2
 
 class Video:
     """
@@ -65,15 +65,15 @@
         '''
         Create writer object for recording videos based on chosen video.
         '''
         self.writer = cv2.VideoWriter('calibration.mp4',
                             cv2.VideoWriter_fourcc(*'mp4v'),
                             self.fps,
                             (self.width, self.height))
-
+ 
     def get_dim(self):
         '''
         Get video resolution
         '''
         width = int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
         height = int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
         return width, height
```

### Comparing `EdiHeadyTrack-0.0.5/EdiHeadyTrack.egg-info/PKG-INFO` & `EdiHeadyTrack-0.0.6/EdiHeadyTrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: EdiHeadyTrack
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automatic, markerless measurement of head kinematics using mediapipe and OpenCV
 Home-page: https://github.com/isDynamics/EdiHeadyTrack
 Author: Thomas Aston
 Author-email: thomas.aston@ed.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) 
 [![Build Status - GitHub](https://github.com/isDynamics/EdiHeadyTrack/workflows/pytesting/badge.svg)](https://github.com/isDynamics/EdiHeadyTrack/actions/workflows/pytesting.yml)
 [![codecov](https://codecov.io/gh/isDynamics/EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)](https://codecov.io/gh/isDynamics/EdiHeadyTrack)
 [![Documentation Status](https://readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https://ediheadytrack.readthedocs.io/en/latest/?badge=latest)
 # EdiHeadyTrack
@@ -53,15 +52,15 @@
 ```bash
 pip install EdiHeadyTrack
 ```
 For further installation instructions, consult the [documentation](https://ediheadytrack.readthedocs.io/en/latest/installation.html).
 
 ## Example
 An example output from EdiHeadyTrack is shown below. A full worked example detailing how this can be achieved is provided [here](https://ediheadytrack.readthedocs.io/en/latest/example.html). 
-![Example image](https://raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/EdiHeadyTrack/resources/comparison.png)
+![Example image](https://raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/resources/comparison.png)
 
 
 <!-- ## Change log
 See [CHANGELOG.md](https://github.com/isDynamics/EdiHeadyTrack/blob/master/CHANGELOG.md).
 
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.5 Summary: Automatic,
+Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.6 Summary: Automatic,
 markerless measurement of head kinematics using mediapipe and OpenCV Home-page:
 https://github.com/isDynamics/EdiHeadyTrack Author: Thomas Aston Author-email:
 thomas.aston@ed.ac.uk Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
-Description-Content-Type: text/markdown License-File: LICENSE [![License: GPL
-v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
-licenses/gpl-3.0) [![Build Status - GitHub](https://github.com/isDynamics/
-EdiHeadyTrack/workflows/pytesting/badge.svg)](https://github.com/isDynamics/
-EdiHeadyTrack/actions/workflows/pytesting.yml) [![codecov](https://codecov.io/
-gh/isDynamics/EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)]
-(https://codecov.io/gh/isDynamics/EdiHeadyTrack) [![Documentation Status]
-(https://readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https:/
-/ediheadytrack.readthedocs.io/en/latest/?badge=latest) # EdiHeadyTrack ##
+Description-Content-Type: text/markdown [![License: GPL v3](https://
+img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
+3.0) [![Build Status - GitHub](https://github.com/isDynamics/EdiHeadyTrack/
+workflows/pytesting/badge.svg)](https://github.com/isDynamics/EdiHeadyTrack/
+actions/workflows/pytesting.yml) [![codecov](https://codecov.io/gh/isDynamics/
+EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)](https://
+codecov.io/gh/isDynamics/EdiHeadyTrack) [![Documentation Status](https://
+readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https://
+ediheadytrack.readthedocs.io/en/latest/?badge=latest) # EdiHeadyTrack ##
 Contributors [https://contrib.rocks/image?repo=isDynamics/EdiHeadyTrack] Made
 with [contrib.rocks](https://contrib.rocks).  ## About EdiHeadyTrack is a
 Python package for measuring head kinematics using markerless head pose
 detection methods. The current implementation primarily uses the FaceMesh
 module of MediaPipe's Python API for facial landmark detection alongside OpenCV
 for handling simple computer vision tasks. Full documentation for EdiHeadyTrack
 can be found [here](https://ediheadytrack.readthedocs.io). ## Technologies
 Project is created with: * Python 3.9.0 ## Setup EdiHeadyTrack is available on
 PyPI! Install using: ```bash pip install EdiHeadyTrack ``` For further
 installation instructions, consult the [documentation](https://
 ediheadytrack.readthedocs.io/en/latest/installation.html). ## Example An
 example output from EdiHeadyTrack is shown below. A full worked example
 detailing how this can be achieved is provided [here](https://
 ediheadytrack.readthedocs.io/en/latest/example.html). ![Example image](https://
-raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/EdiHeadyTrack/
-resources/comparison.png)  ## Citation If you use `EdiHeadyTrack` in you work,
-please cite the following publication:  As BibTeX:  ## Getting Involved For any
+raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/resources/
+comparison.png)  ## Citation If you use `EdiHeadyTrack` in you work, please
+cite the following publication:  As BibTeX:  ## Getting Involved For any
 suggestions, please [create a new issue](https://github.com/isDynamics/
 EdiHeadyTrack/issues).
```

### Comparing `EdiHeadyTrack-0.0.5/PKG-INFO` & `EdiHeadyTrack-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: EdiHeadyTrack
-Version: 0.0.5
+Version: 0.0.6
 Summary: Automatic, markerless measurement of head kinematics using mediapipe and OpenCV
 Home-page: https://github.com/isDynamics/EdiHeadyTrack
 Author: Thomas Aston
 Author-email: thomas.aston@ed.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) 
 [![Build Status - GitHub](https://github.com/isDynamics/EdiHeadyTrack/workflows/pytesting/badge.svg)](https://github.com/isDynamics/EdiHeadyTrack/actions/workflows/pytesting.yml)
 [![codecov](https://codecov.io/gh/isDynamics/EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)](https://codecov.io/gh/isDynamics/EdiHeadyTrack)
 [![Documentation Status](https://readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https://ediheadytrack.readthedocs.io/en/latest/?badge=latest)
 # EdiHeadyTrack
@@ -53,15 +52,15 @@
 ```bash
 pip install EdiHeadyTrack
 ```
 For further installation instructions, consult the [documentation](https://ediheadytrack.readthedocs.io/en/latest/installation.html).
 
 ## Example
 An example output from EdiHeadyTrack is shown below. A full worked example detailing how this can be achieved is provided [here](https://ediheadytrack.readthedocs.io/en/latest/example.html). 
-![Example image](https://raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/EdiHeadyTrack/resources/comparison.png)
+![Example image](https://raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/resources/comparison.png)
 
 
 <!-- ## Change log
 See [CHANGELOG.md](https://github.com/isDynamics/EdiHeadyTrack/blob/master/CHANGELOG.md).
 
 
 ## Contributing
```

#### html2text {}

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.5 Summary: Automatic,
+Metadata-Version: 2.1 Name: EdiHeadyTrack Version: 0.0.6 Summary: Automatic,
 markerless measurement of head kinematics using mediapipe and OpenCV Home-page:
 https://github.com/isDynamics/EdiHeadyTrack Author: Thomas Aston Author-email:
 thomas.aston@ed.ac.uk Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.9
-Description-Content-Type: text/markdown License-File: LICENSE [![License: GPL
-v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/
-licenses/gpl-3.0) [![Build Status - GitHub](https://github.com/isDynamics/
-EdiHeadyTrack/workflows/pytesting/badge.svg)](https://github.com/isDynamics/
-EdiHeadyTrack/actions/workflows/pytesting.yml) [![codecov](https://codecov.io/
-gh/isDynamics/EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)]
-(https://codecov.io/gh/isDynamics/EdiHeadyTrack) [![Documentation Status]
-(https://readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https:/
-/ediheadytrack.readthedocs.io/en/latest/?badge=latest) # EdiHeadyTrack ##
+Description-Content-Type: text/markdown [![License: GPL v3](https://
+img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-
+3.0) [![Build Status - GitHub](https://github.com/isDynamics/EdiHeadyTrack/
+workflows/pytesting/badge.svg)](https://github.com/isDynamics/EdiHeadyTrack/
+actions/workflows/pytesting.yml) [![codecov](https://codecov.io/gh/isDynamics/
+EdiHeadyTrack/branch/master/graph/badge.svg?token=FOE3NBS07X)](https://
+codecov.io/gh/isDynamics/EdiHeadyTrack) [![Documentation Status](https://
+readthedocs.org/projects/ediheadytrack/badge/?version=latest)](https://
+ediheadytrack.readthedocs.io/en/latest/?badge=latest) # EdiHeadyTrack ##
 Contributors [https://contrib.rocks/image?repo=isDynamics/EdiHeadyTrack] Made
 with [contrib.rocks](https://contrib.rocks).  ## About EdiHeadyTrack is a
 Python package for measuring head kinematics using markerless head pose
 detection methods. The current implementation primarily uses the FaceMesh
 module of MediaPipe's Python API for facial landmark detection alongside OpenCV
 for handling simple computer vision tasks. Full documentation for EdiHeadyTrack
 can be found [here](https://ediheadytrack.readthedocs.io). ## Technologies
 Project is created with: * Python 3.9.0 ## Setup EdiHeadyTrack is available on
 PyPI! Install using: ```bash pip install EdiHeadyTrack ``` For further
 installation instructions, consult the [documentation](https://
 ediheadytrack.readthedocs.io/en/latest/installation.html). ## Example An
 example output from EdiHeadyTrack is shown below. A full worked example
 detailing how this can be achieved is provided [here](https://
 ediheadytrack.readthedocs.io/en/latest/example.html). ![Example image](https://
-raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/EdiHeadyTrack/
-resources/comparison.png)  ## Citation If you use `EdiHeadyTrack` in you work,
-please cite the following publication:  As BibTeX:  ## Getting Involved For any
+raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/resources/
+comparison.png)  ## Citation If you use `EdiHeadyTrack` in you work, please
+cite the following publication:  As BibTeX:  ## Getting Involved For any
 suggestions, please [create a new issue](https://github.com/isDynamics/
 EdiHeadyTrack/issues).
```

### Comparing `EdiHeadyTrack-0.0.5/README.md` & `EdiHeadyTrack-0.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 ```bash
 pip install EdiHeadyTrack
 ```
 For further installation instructions, consult the [documentation](https://ediheadytrack.readthedocs.io/en/latest/installation.html).
 
 ## Example
 An example output from EdiHeadyTrack is shown below. A full worked example detailing how this can be achieved is provided [here](https://ediheadytrack.readthedocs.io/en/latest/example.html). 
-![Example image](https://raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/EdiHeadyTrack/resources/comparison.png)
+![Example image](https://raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/resources/comparison.png)
 
 
 <!-- ## Change log
 See [CHANGELOG.md](https://github.com/isDynamics/EdiHeadyTrack/blob/master/CHANGELOG.md).
 
 
 ## Contributing
```

#### html2text {}

```diff
@@ -17,11 +17,11 @@
 Python 3.9.0 ## Setup EdiHeadyTrack is available on PyPI! Install using:
 ```bash pip install EdiHeadyTrack ``` For further installation instructions,
 consult the [documentation](https://ediheadytrack.readthedocs.io/en/latest/
 installation.html). ## Example An example output from EdiHeadyTrack is shown
 below. A full worked example detailing how this can be achieved is provided
 [here](https://ediheadytrack.readthedocs.io/en/latest/example.html). ![Example
 image](https://raw.githubusercontent.com/isDynamics/EdiHeadyTrack/master/
-EdiHeadyTrack/resources/comparison.png)  ## Citation If you use `EdiHeadyTrack`
-in you work, please cite the following publication:  As BibTeX:  ## Getting
-Involved For any suggestions, please [create a new issue](https://github.com/
-isDynamics/EdiHeadyTrack/issues).
+resources/comparison.png)  ## Citation If you use `EdiHeadyTrack` in you work,
+please cite the following publication:  As BibTeX:  ## Getting Involved For any
+suggestions, please [create a new issue](https://github.com/isDynamics/
+EdiHeadyTrack/issues).
```

### Comparing `EdiHeadyTrack-0.0.5/setup.cfg` & `EdiHeadyTrack-0.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = EdiHeadyTrack
-version = 0.0.5
+version = 0.0.6
 author = Thomas Aston
 author_email = thomas.aston@ed.ac.uk
 description = Automatic, markerless measurement of head kinematics using mediapipe and OpenCV
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/isDynamics/EdiHeadyTrack
 classifiers =
```

