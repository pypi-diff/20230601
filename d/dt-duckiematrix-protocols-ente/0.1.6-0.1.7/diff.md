# Comparing `tmp/dt-duckiematrix-protocols-ente-0.1.6.tar.gz` & `tmp/dt-duckiematrix-protocols-ente-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dt-duckiematrix-protocols-ente-0.1.6.tar", last modified: Mon Dec 20 23:59:34 2021, max compression
+gzip compressed data, was "dt-duckiematrix-protocols-ente-0.1.7.tar", last modified: Thu Jun  1 20:44:57 2023, max compression
```

## Comparing `dt-duckiematrix-protocols-ente-0.1.6.tar` & `dt-duckiematrix-protocols-ente-0.1.7.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.111372 dt-duckiematrix-protocols-ente-0.1.6/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2021-09-21 17:06:15.000000 dt-duckiematrix-protocols-ente-0.1.6/MANIFEST.in
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      593 2021-12-20 23:59:34.111372 dt-duckiematrix-protocols-ente-0.1.6/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6310 2021-09-21 17:06:15.000000 dt-duckiematrix-protocols-ente-0.1.6/README.md
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2021-12-20 23:59:34.111372 dt-duckiematrix-protocols-ente-0.1.6/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2166 2021-10-14 18:45:09.000000 dt-duckiematrix-protocols-ente-0.1.6/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.103372 dt-duckiematrix-protocols-ente-0.1.6/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.103372 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      331 2021-09-21 17:16:42.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/CBorMessage.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      418 2021-12-20 20:01:37.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/CameraFrame.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      151 2021-10-14 18:46:39.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/EmptyMessage.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      666 2021-10-14 18:46:39.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/LEDsCommand.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      184 2021-10-14 22:51:56.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/LayerMessage.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      740 2021-10-18 20:40:40.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/NetworkEndpoint.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      224 2021-10-20 21:42:59.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/NetworkJoin.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      872 2021-10-21 20:25:07.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/NetworkJoined.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      139 2021-10-15 21:18:03.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/NetworkLeave.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      166 2021-10-15 21:18:03.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/NetworkReady.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      143 2021-10-15 21:58:53.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/StringMessage.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      149 2021-10-14 18:46:39.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/TimeOfFlightRange.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      147 2021-10-14 18:46:39.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/WheelEncoderTicks.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      182 2021-10-14 18:46:39.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/WheelsCommand.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       37 2021-10-14 18:43:58.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.107372 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       50 2021-12-20 23:59:32.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.107372 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/commons/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1456 2021-12-20 21:23:32.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/commons/CBORProtocol.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2208 2021-11-05 17:55:43.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/commons/LayerProtocol.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4683 2021-12-20 21:23:47.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/commons/ProtocolAbs.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2021-10-14 18:59:46.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/commons/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     8319 2021-12-20 20:01:37.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/commons/socket.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1436 2021-12-20 21:25:18.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/matrix.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.107372 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      950 2021-10-21 20:25:07.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/RobotProtocols.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6432 2021-12-20 23:59:07.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/RobotsManager.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       93 2021-12-20 20:53:43.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/__init__.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.107372 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/features/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2021-10-18 21:33:30.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/features/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1727 2021-10-21 20:02:44.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/features/motion.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3965 2021-12-20 22:00:52.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/features/sensors.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6454 2021-12-20 23:20:46.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/robots.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.107372 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/types/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2021-11-04 16:54:03.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/types/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1850 2021-11-05 17:14:00.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/types/colors.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4630 2021-11-05 17:14:11.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/types/geometry.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1896 2021-11-04 23:36:43.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/types/markers.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.107372 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1153 2021-11-04 22:40:53.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/Color.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      812 2021-10-05 23:15:03.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/MonitoredCondition.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1500 2021-10-19 20:23:55.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/MonitoredObject.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2946 2021-11-05 16:42:02.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/Pose3D.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1200 2021-11-04 22:40:39.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/Vector3.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2021-10-14 19:24:00.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      235 2021-10-15 22:13:11.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/communication.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1393 2021-11-04 17:42:56.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/types.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.111372 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/viewer/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7008 2021-11-05 21:58:16.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/viewer/MarkersManager.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      177 2021-11-04 23:35:44.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/viewer/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    15616 2021-11-05 21:57:13.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/viewer/markers.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.111372 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols_ente.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      593 2021-12-20 23:59:33.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols_ente.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2432 2021-12-20 23:59:33.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols_ente.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2021-12-20 23:59:33.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols_ente.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       73 2021-12-20 23:59:33.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols_ente.egg-info/top_level.txt
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2021-12-20 23:59:34.111372 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_types/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      145 2021-10-21 20:24:22.000000 dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_types/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       42 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/MANIFEST.in
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      526 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6310 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/README.md
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2166 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.557155 dt-duckiematrix-protocols-ente-0.1.7/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.557155 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      331 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/CBorMessage.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      418 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/CameraFrame.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      151 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/EmptyMessage.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      666 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/LEDsCommand.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      184 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/LayerMessage.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      740 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/NetworkEndpoint.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      224 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/NetworkJoin.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      872 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/NetworkJoined.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      139 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/NetworkLeave.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      166 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/NetworkReady.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      143 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/StringMessage.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      149 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/TimeOfFlightRange.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      147 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/WheelEncoderTicks.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      182 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/WheelsCommand.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       37 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.557155 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       50 2023-06-01 20:44:55.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/commons/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1456 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/commons/CBORProtocol.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2208 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/commons/LayerProtocol.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4683 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/commons/ProtocolAbs.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/commons/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     8319 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/commons/socket.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1436 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/matrix.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      950 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/RobotProtocols.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6610 2023-04-28 12:36:04.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/RobotsManager.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       93 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/__init__.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/features/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/features/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4033 2023-04-28 12:36:04.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/features/lights.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1727 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/features/motion.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     3965 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/features/sensors.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6721 2023-04-28 12:36:04.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/robots.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/types/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/types/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1850 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/types/colors.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     4630 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/types/geometry.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1896 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/types/markers.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1153 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/Color.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      812 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/MonitoredCondition.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1500 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/MonitoredObject.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2946 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/Pose3D.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1200 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/Vector3.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      235 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/communication.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1393 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/types.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/viewer/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     7008 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/viewer/MarkersManager.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      177 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/viewer/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    15616 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/viewer/markers.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols_ente.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      526 2023-06-01 20:44:57.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols_ente.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     2487 2023-06-01 20:44:57.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols_ente.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-06-01 20:44:57.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols_ente.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       73 2023-06-01 20:44:57.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols_ente.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-06-01 20:44:57.561155 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_types/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      145 2023-04-19 19:49:19.000000 dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_types/__init__.py
```

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/README.md` & `dt-duckiematrix-protocols-ente-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/setup.py` & `dt-duckiematrix-protocols-ente-0.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/LEDsCommand.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/LEDsCommand.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/NetworkEndpoint.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/NetworkEndpoint.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_messages/NetworkJoined.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_messages/NetworkJoined.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/commons/CBORProtocol.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/commons/CBORProtocol.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/commons/LayerProtocol.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/commons/LayerProtocol.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/commons/ProtocolAbs.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/commons/ProtocolAbs.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/commons/socket.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/commons/socket.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/matrix.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/matrix.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/RobotProtocols.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/RobotProtocols.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/RobotsManager.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/RobotsManager.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,51 +74,56 @@
 
     def DB21M(self, key: str, **kwargs) -> DB21M:
         features: Set[RobotFeature] = {
             RobotFeature.DIFFERENTIAL_DRIVE,
             RobotFeature.CAMERA_0,
             RobotFeature.ENCODER_LEFT,
             RobotFeature.ENCODER_RIGHT,
-            RobotFeature.TOF_FRONT_CENTER
+            RobotFeature.TOF_FRONT_CENTER,
+            RobotFeature.LIGHTS_5,
         }
         return self._make_robot(key, DB21M, features, **kwargs)
 
     def DB21J(self, key: str, **kwargs) -> DB21J:
         features: Set[RobotFeature] = {
             RobotFeature.DIFFERENTIAL_DRIVE,
             RobotFeature.CAMERA_0,
             RobotFeature.ENCODER_LEFT,
             RobotFeature.ENCODER_RIGHT,
-            RobotFeature.TOF_FRONT_CENTER
+            RobotFeature.TOF_FRONT_CENTER,
+            RobotFeature.LIGHTS_5,
         }
         return self._make_robot(key, DB21J, features, **kwargs)
 
     def DB21R(self, key: str, **kwargs) -> DB21R:
         features: Set[RobotFeature] = {
             RobotFeature.DIFFERENTIAL_DRIVE,
             RobotFeature.CAMERA_0,
             RobotFeature.ENCODER_LEFT,
             RobotFeature.ENCODER_RIGHT,
-            RobotFeature.TOF_FRONT_CENTER
+            RobotFeature.TOF_FRONT_CENTER,
+            RobotFeature.LIGHTS_5,
         }
         return self._make_robot(key, DB21R, features, **kwargs)
 
     def DB19(self, key: str, **kwargs) -> DB19:
         features: Set[RobotFeature] = {
             RobotFeature.DIFFERENTIAL_DRIVE,
             RobotFeature.CAMERA_0,
             RobotFeature.ENCODER_LEFT,
             RobotFeature.ENCODER_RIGHT,
+            RobotFeature.LIGHTS_5,
         }
         return self._make_robot(key, DB19, features, **kwargs)
 
     def DB18(self, key: str, **kwargs) -> DB18:
         features: Set[RobotFeature] = {
             RobotFeature.DIFFERENTIAL_DRIVE,
             RobotFeature.CAMERA_0,
+            RobotFeature.LIGHTS_5,
         }
         return self._make_robot(key, DB18, features, **kwargs)
 
     def WT21A(self, key: str, **kwargs) -> WT21A:
         features: Set[RobotFeature] = {
             RobotFeature.CAMERA_0
         }
```

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/features/motion.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/features/motion.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/features/sensors.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/features/sensors.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/robot/robots.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/robot/robots.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from enum import Enum
 from typing import Optional, Dict, Set, Union, List
 
 from dt_duckiematrix_protocols.commons.LayerProtocol import LayerProtocol
 from dt_duckiematrix_protocols.commons.ProtocolAbs import ProtocolAbs
 from dt_duckiematrix_protocols.robot.RobotProtocols import RobotProtocolAbs
+from dt_duckiematrix_protocols.robot.features.lights import Lights
 from dt_duckiematrix_protocols.robot.features.sensors import Camera, TimeOfFlight
 from dt_duckiematrix_protocols.robot.features.motion import DifferentialDrive, \
     DifferentialDriveWheels
 from dt_duckiematrix_protocols.types.geometry import IPose3D
 from dt_duckiematrix_protocols.utils.Pose3D import Pose3D
 
 
@@ -15,15 +16,15 @@
 #
 # # Duckiebot
 # DB18 = 10
 # DB19 = 11
 # DB20 = 12
 # DB21M = 13
 # DB21J = 14
-# DB21R = 15
+# DBR4 = 15
 # # Watchtower
 # WT18 = 20
 # WT19A = 21
 # WT19B = 22
 # WT21A = 23
 # WT21B = 24
 # # Traffic Light
@@ -48,19 +49,15 @@
 class RobotFeature(Enum):
     # motion
     FRAME = "frame"
     DIFFERENTIAL_DRIVE = "wheels"
     # cameras
     CAMERA_0 = "camera_0"
     # lights
-    LIGHT_0 = "light_0"
-    LIGHT_1 = "light_1"
-    LIGHT_2 = "light_2"
-    LIGHT_3 = "light_3"
-    LIGHT_4 = "light_4"
+    LIGHTS_5 = "lights_5"
     # encoders
     ENCODER_LEFT = "encoder_left"
     ENCODER_RIGHT = "encoder_right"
     # ToFs
     TOF_FRONT_CENTER = "tof_front_center"
     TOF_FRONT_LEFT = "tof_front_left"
     TOF_FRONT_RIGHT = "tof_front_right"
@@ -105,14 +102,18 @@
             self._camera_0 = Camera(self._protocol("robot"), camera_0_key)
         # - wheels
         self._wheels: Optional[DifferentialDriveWheels] = None
         if RobotFeature.DIFFERENTIAL_DRIVE in features:
             encoder_left: bool = RobotFeature.ENCODER_LEFT in features
             encoder_right: bool = RobotFeature.ENCODER_RIGHT in features
             self._wheels = DifferentialDriveWheels(robot_proto, key, encoder_left, encoder_right)
+        # - lights
+        self._lights: Optional[Lights] = None
+        if RobotFeature.LIGHTS_5 in features:
+            self._lights = Lights(layer_proto, key)
 
     def session(self) -> ProtocolAbs.SessionProtocolContext:
         return self._protocol("robot").session()
 
     @property
     def pose(self) -> IPose3D:
         return self._pose
@@ -163,17 +164,24 @@
 class DifferentialDriveRobot(RobotAbs):
 
     @property
     def drive(self) -> DifferentialDrive:
         return self._drive
 
 
+class LightsEnabledRobot(RobotAbs):
+
+    @property
+    def lights(self) -> Lights:
+        return self._lights
+
+
 # DB - Duckiebots
 
-class DBRobot(CameraEnabledRobot, WheeledRobot, DifferentialDriveRobot):
+class DBRobot(CameraEnabledRobot, WheeledRobot, DifferentialDriveRobot, LightsEnabledRobot):
     pass
 
 
 class DB2XRobot(DBRobot):
     pass
 
 
@@ -268,9 +276,9 @@
     "WT18",
     # Duckiecams
     "DCRobot",
     "DC21",
     # Generic Robots
     "CameraEnabledRobot",
     "WheeledRobot",
-    "DifferentialDriveWheels"
+    "DifferentialDriveRobot"
 ]
```

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/types/colors.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/types/colors.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/types/geometry.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/types/geometry.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/types/markers.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/types/markers.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/Color.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/Color.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/MonitoredCondition.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/MonitoredCondition.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/MonitoredObject.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/MonitoredObject.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/Pose3D.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/Pose3D.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/Vector3.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/Vector3.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/utils/types.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/utils/types.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/viewer/MarkersManager.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/viewer/MarkersManager.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols/viewer/markers.py` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols/viewer/markers.py`

 * *Files identical despite different names*

### Comparing `dt-duckiematrix-protocols-ente-0.1.6/src/dt_duckiematrix_protocols_ente.egg-info/SOURCES.txt` & `dt-duckiematrix-protocols-ente-0.1.7/src/dt_duckiematrix_protocols_ente.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 src/dt_duckiematrix_protocols/commons/__init__.py
 src/dt_duckiematrix_protocols/commons/socket.py
 src/dt_duckiematrix_protocols/robot/RobotProtocols.py
 src/dt_duckiematrix_protocols/robot/RobotsManager.py
 src/dt_duckiematrix_protocols/robot/__init__.py
 src/dt_duckiematrix_protocols/robot/robots.py
 src/dt_duckiematrix_protocols/robot/features/__init__.py
+src/dt_duckiematrix_protocols/robot/features/lights.py
 src/dt_duckiematrix_protocols/robot/features/motion.py
 src/dt_duckiematrix_protocols/robot/features/sensors.py
 src/dt_duckiematrix_protocols/types/__init__.py
 src/dt_duckiematrix_protocols/types/colors.py
 src/dt_duckiematrix_protocols/types/geometry.py
 src/dt_duckiematrix_protocols/types/markers.py
 src/dt_duckiematrix_protocols/utils/Color.py
```

