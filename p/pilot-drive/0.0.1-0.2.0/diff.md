# Comparing `tmp/pilot-drive-0.0.1.tar.gz` & `tmp/pilot-drive-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilot-drive-0.0.1.tar", last modified: Tue Mar 22 19:54:33 2022, max compression
+gzip compressed data, was "pilot-drive-0.2.0.tar", last modified: Thu Jun  1 02:42:01 2023, max compression
```

## Comparing `pilot-drive-0.0.1.tar` & `pilot-drive-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,113 @@
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.321618 pilot-drive-0.0.1/
--rw-rw-r--   0 lame      (1000) lame      (1000)     3466 2022-03-22 19:44:24.000000 pilot-drive-0.0.1/.gitignore
--rw-rw-r--   0 lame      (1000) lame      (1000)    35149 2022-01-28 17:57:54.000000 pilot-drive-0.0.1/LICENSE
--rw-rw-r--   0 lame      (1000) lame      (1000)      133 2022-03-22 19:47:21.000000 pilot-drive-0.0.1/MANIFEST.in
--rw-rw-r--   0 lame      (1000) lame      (1000)      921 2022-03-22 19:54:33.321618 pilot-drive-0.0.1/PKG-INFO
--rw-rw-r--   0 lame      (1000) lame      (1000)      336 2021-05-03 14:37:42.000000 pilot-drive-0.0.1/README.md
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.317618 pilot-drive-0.0.1/pilot_drive.egg-info/
--rw-rw-r--   0 lame      (1000) lame      (1000)      921 2022-03-22 19:54:32.000000 pilot-drive-0.0.1/pilot_drive.egg-info/PKG-INFO
--rw-rw-r--   0 lame      (1000) lame      (1000)     1411 2022-03-22 19:54:33.000000 pilot-drive-0.0.1/pilot_drive.egg-info/SOURCES.txt
--rw-rw-r--   0 lame      (1000) lame      (1000)        1 2022-03-22 19:54:32.000000 pilot-drive-0.0.1/pilot_drive.egg-info/dependency_links.txt
--rw-rw-r--   0 lame      (1000) lame      (1000)       10 2022-03-22 19:54:33.000000 pilot-drive-0.0.1/pilot_drive.egg-info/requires.txt
--rw-rw-r--   0 lame      (1000) lame      (1000)        4 2022-03-22 19:54:33.000000 pilot-drive-0.0.1/pilot_drive.egg-info/top_level.txt
--rw-rw-r--   0 lame      (1000) lame      (1000)       38 2022-03-22 19:54:33.321618 pilot-drive-0.0.1/setup.cfg
--rw-rw-r--   0 lame      (1000) lame      (1000)      995 2022-03-22 19:08:32.000000 pilot-drive-0.0.1/setup.py
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.317618 pilot-drive-0.0.1/src/
--rw-rw-r--   0 lame      (1000) lame      (1000)        0 2022-01-28 01:27:54.000000 pilot-drive-0.0.1/src/__init__.py
--rw-rw-r--   0 lame      (1000) lame      (1000)     5741 2022-03-22 18:55:33.000000 pilot-drive-0.0.1/src/main.py
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.321618 pilot-drive-0.0.1/src/utils/
--rw-rw-r--   0 lame      (1000) lame      (1000)        0 2022-01-28 01:23:38.000000 pilot-drive-0.0.1/src/utils/__init__.py
--rw-rw-r--   0 lame      (1000) lame      (1000)     3950 2022-03-21 23:31:21.000000 pilot-drive-0.0.1/src/utils/adb_manager.py
--rw-rw-r--   0 lame      (1000) lame      (1000)     3224 2022-03-21 23:31:21.000000 pilot-drive-0.0.1/src/utils/adb_notification.py
--rw-rw-r--   0 lame      (1000) lame      (1000)     2052 2022-03-21 23:31:21.000000 pilot-drive-0.0.1/src/utils/adb_read_icon_db.py
--rw-rw-r--   0 lame      (1000) lame      (1000)     7327 2022-03-21 23:31:21.000000 pilot-drive-0.0.1/src/utils/bt_ctl.py
--rw-rw-r--   0 lame      (1000) lame      (1000)     4252 2022-03-21 23:31:21.000000 pilot-drive-0.0.1/src/utils/bt_track.py
--rw-rw-r--   0 lame      (1000) lame      (1000)     4405 2022-03-21 23:31:21.000000 pilot-drive-0.0.1/src/utils/obd_info.py
--rw-rw-r--   0 lame      (1000) lame      (1000)      180 2022-03-05 21:05:13.000000 pilot-drive-0.0.1/src/utils/sys_utils.py
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.317618 pilot-drive-0.0.1/src/web/
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.317618 pilot-drive-0.0.1/src/web/static/
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.321618 pilot-drive-0.0.1/src/web/static/css/
--rw-rw-rw-   0 lame      (1000) lame      (1000)    43280 2019-03-21 20:51:52.000000 pilot-drive-0.0.1/src/web/static/css/Futura.ttf
--rw-rw-r--   0 lame      (1000) lame      (1000)     3402 2022-03-22 01:26:54.000000 pilot-drive-0.0.1/src/web/static/css/pilot_style.css
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.321618 pilot-drive-0.0.1/src/web/static/icons/
--rw-rw-r--   0 lame      (1000) lame      (1000)    11651 2022-03-01 20:58:59.000000 pilot-drive-0.0.1/src/web/static/icons/adb_button.png
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.321618 pilot-drive-0.0.1/src/web/static/icons/adb_icons/
--rw-rw-r--   0 lame      (1000) lame      (1000)     5563 2022-03-18 02:19:27.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/Add alarm.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     8721 2022-03-16 00:16:09.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/Aurora Store.png
--rw-rw-r--   0 lame      (1000) lame      (1000)    13413 2022-03-12 02:43:03.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/Car Scanner.png
--rw-rw-r--   0 lame      (1000) lame      (1000)    13653 2022-03-22 01:10:52.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/Messaging.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     5972 2022-03-13 14:44:24.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/New alarm.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     8655 2022-03-13 14:44:24.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/NewPipe.png
--rw-rw-r--   0 lame      (1000) lame      (1000)    10557 2022-03-22 01:10:52.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/NordVPN.png
--rw-rw-r--   0 lame      (1000) lame      (1000)    15048 2022-03-18 02:19:27.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/Phone.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     7482 2022-03-11 18:21:38.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/ProtonMail.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     7253 2022-03-22 01:10:52.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/Pulse Music.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     7358 2022-03-21 23:52:37.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/Spotify.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     6782 2022-03-16 00:16:09.000000 pilot-drive-0.0.1/src/web/static/icons/adb_icons/Venmo.png
--rw-rw-r--   0 lame      (1000) lame      (1000)    11367 2022-03-01 20:46:56.000000 pilot-drive-0.0.1/src/web/static/icons/car_button.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     8919 2022-03-01 20:54:07.000000 pilot-drive-0.0.1/src/web/static/icons/home_button.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     7796 2022-02-19 15:29:24.000000 pilot-drive-0.0.1/src/web/static/icons/next_button.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     6373 2022-02-19 15:29:24.000000 pilot-drive-0.0.1/src/web/static/icons/pause_button.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     8090 2022-02-19 15:29:24.000000 pilot-drive-0.0.1/src/web/static/icons/play_button.png
--rw-rw-r--   0 lame      (1000) lame      (1000)     8107 2022-02-19 15:29:24.000000 pilot-drive-0.0.1/src/web/static/icons/prev_button.png
--rw-rw-r--   0 lame      (1000) lame      (1000)    15794 2022-03-02 22:07:16.000000 pilot-drive-0.0.1/src/web/static/icons/settings_button.png
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.321618 pilot-drive-0.0.1/src/web/static/js/
--rw-rw-r--   0 lame      (1000) lame      (1000)    13454 2022-03-21 23:31:21.000000 pilot-drive-0.0.1/src/web/static/js/pilot-drive_script.js
-drwxrwxr-x   0 lame      (1000) lame      (1000)        0 2022-03-22 19:54:33.321618 pilot-drive-0.0.1/src/web/templates/
--rw-rw-r--   0 lame      (1000) lame      (1000)     4857 2022-03-22 01:26:54.000000 pilot-drive-0.0.1/src/web/templates/home.html
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.634342 pilot-drive-0.2.0/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       48 2023-04-12 00:54:49.000000 pilot-drive-0.2.0/MANIFEST.in
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      920 2023-06-01 02:42:01.633342 pilot-drive-0.2.0/PKG-INFO
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      203 2023-04-12 00:54:49.000000 pilot-drive-0.2.0/README.md
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.629342 pilot-drive-0.2.0/pilot_drive/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       64 2023-05-27 05:15:25.000000 pilot-drive-0.2.0/pilot_drive/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     2035 2023-05-28 00:12:45.000000 pilot-drive-0.2.0/pilot_drive/__main__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     2369 2023-05-31 01:56:57.000000 pilot-drive-0.2.0/pilot_drive/constants.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)    36338 2023-06-01 02:40:03.000000 pilot-drive-0.2.0/pilot_drive/installer.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.629342 pilot-drive-0.2.0/pilot_drive/master_logging/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       83 2023-04-12 00:54:49.000000 pilot-drive-0.2.0/pilot_drive/master_logging/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     6592 2023-04-12 00:54:49.000000 pilot-drive-0.2.0/pilot_drive/master_logging/master_logger.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.629342 pilot-drive-0.2.0/pilot_drive/master_queue/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      103 2023-04-12 00:54:49.000000 pilot-drive-0.2.0/pilot_drive/master_queue/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     2239 2023-05-30 23:49:46.000000 pilot-drive-0.2.0/pilot_drive/master_queue/master_event_queue.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     9313 2023-05-28 00:12:45.000000 pilot-drive-0.2.0/pilot_drive/pd_manager.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.629342 pilot-drive-0.2.0/pilot_drive/services/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      282 2023-05-26 19:58:14.000000 pilot-drive-0.2.0/pilot_drive/services/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1884 2023-04-26 11:26:53.000000 pilot-drive-0.2.0/pilot_drive/services/abstract_service.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.629342 pilot-drive-0.2.0/pilot_drive/services/bluetooth/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      171 2023-05-05 20:20:01.000000 pilot-drive-0.2.0/pilot_drive/services/bluetooth/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)    12174 2023-05-31 02:13:27.000000 pilot-drive-0.2.0/pilot_drive/services/bluetooth/bluetooth.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1482 2023-05-24 11:39:57.000000 pilot-drive-0.2.0/pilot_drive/services/bluetooth/constants.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      270 2023-04-28 04:39:57.000000 pilot-drive-0.2.0/pilot_drive/services/bluetooth/exceptions.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.629342 pilot-drive-0.2.0/pilot_drive/services/camera/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       80 2023-04-19 11:43:45.000000 pilot-drive-0.2.0/pilot_drive/services/camera/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     2515 2023-04-28 04:24:02.000000 pilot-drive-0.2.0/pilot_drive/services/camera/camera.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      144 2023-04-28 04:39:57.000000 pilot-drive-0.2.0/pilot_drive/services/camera/exceptions.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.630342 pilot-drive-0.2.0/pilot_drive/services/media/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      101 2023-04-28 04:09:35.000000 pilot-drive-0.2.0/pilot_drive/services/media/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     2157 2023-04-28 04:54:19.000000 pilot-drive-0.2.0/pilot_drive/services/media/abstract_media_source.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     8855 2023-05-31 02:14:12.000000 pilot-drive-0.2.0/pilot_drive/services/media/bluetooth_media.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1210 2023-04-28 04:09:35.000000 pilot-drive-0.2.0/pilot_drive/services/media/constants.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     3736 2023-05-31 02:13:27.000000 pilot-drive-0.2.0/pilot_drive/services/media/media.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.630342 pilot-drive-0.2.0/pilot_drive/services/phone/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      102 2023-05-17 00:44:33.000000 pilot-drive-0.2.0/pilot_drive/services/phone/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      958 2023-05-05 20:20:01.000000 pilot-drive-0.2.0/pilot_drive/services/phone/abstract_manager.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1223 2023-05-06 16:29:14.000000 pilot-drive-0.2.0/pilot_drive/services/phone/ancs_api.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)    12022 2023-05-08 20:24:52.000000 pilot-drive-0.2.0/pilot_drive/services/phone/android_manager.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     3202 2023-05-08 10:35:08.000000 pilot-drive-0.2.0/pilot_drive/services/phone/constants.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      188 2023-05-05 20:20:01.000000 pilot-drive-0.2.0/pilot_drive/services/phone/exceptions.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     6653 2023-05-06 16:29:14.000000 pilot-drive-0.2.0/pilot_drive/services/phone/ios_manager.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)    12462 2023-05-06 16:29:14.000000 pilot-drive-0.2.0/pilot_drive/services/phone/phone.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.630342 pilot-drive-0.2.0/pilot_drive/services/settings/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      123 2023-05-27 04:03:51.000000 pilot-drive-0.2.0/pilot_drive/services/settings/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      305 2023-04-19 11:43:45.000000 pilot-drive-0.2.0/pilot_drive/services/settings/exceptions.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     8702 2023-04-19 11:43:45.000000 pilot-drive-0.2.0/pilot_drive/services/settings/settings.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.630342 pilot-drive-0.2.0/pilot_drive/services/shared/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       68 2023-04-28 04:09:35.000000 pilot-drive-0.2.0/pilot_drive/services/shared/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)    15077 2023-05-12 03:13:38.000000 pilot-drive-0.2.0/pilot_drive/services/shared/bluez_api.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     3057 2023-04-28 04:52:24.000000 pilot-drive-0.2.0/pilot_drive/services/shared/dbus_api.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.630342 pilot-drive-0.2.0/pilot_drive/services/updater/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      104 2023-05-26 19:57:40.000000 pilot-drive-0.2.0/pilot_drive/services/updater/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      874 2023-05-29 19:06:37.000000 pilot-drive-0.2.0/pilot_drive/services/updater/constants.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     9228 2023-05-29 19:06:37.000000 pilot-drive-0.2.0/pilot_drive/services/updater/updater.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.630342 pilot-drive-0.2.0/pilot_drive/services/vehicle/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       84 2023-04-19 11:43:45.000000 pilot-drive-0.2.0/pilot_drive/services/vehicle/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      859 2023-05-24 11:39:57.000000 pilot-drive-0.2.0/pilot_drive/services/vehicle/constants.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     7622 2023-05-28 00:12:45.000000 pilot-drive-0.2.0/pilot_drive/services/vehicle/vehicle.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.631342 pilot-drive-0.2.0/pilot_drive/web/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       64 2023-04-12 00:54:49.000000 pilot-drive-0.2.0/pilot_drive/web/__init__.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.631342 pilot-drive-0.2.0/pilot_drive/web/files/
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.633342 pilot-drive-0.2.0/pilot_drive/web/files/assets/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      327 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/DataGauge-000ca041.css
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      549 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/DataGauge-6847a0de.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)    43280 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Futura-0b7756bb.ttf
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1399 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Media-e6afad0b.css
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     4868 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Media-f5f7947b.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      620 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Phone-53254b1a.css
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     2814 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Phone-d3ecf529.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      780 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/PhoneNotification-4e1dec3c.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      480 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/PhoneNotification-63fbfbc5.css
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1050 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Settings-165234ab.css
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     2191 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Settings-84838880.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      300 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/TextButton-1d08b82b.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      645 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/ThemePicker-4dd479f5.css
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1003 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/ThemePicker-82c99768.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     2212 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Updater-38554013.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      842 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Updater-7477c411.css
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1773 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Vehicle-2d37e6ff.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      558 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/Vehicle-709fe5c7.css
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      350 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/bluetooth_disabled-375e461d.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       66 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/bluetooth_disabled-b2ae7768.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      735 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/car_issue-bff3f380.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)    83395 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/index-b1308428.js
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      930 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/index-de5890b0.css
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      361 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/media-760b8c2a.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      351 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/mobile_disabled-f3ad3577.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      501 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/notifications_off-751622c7.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      190 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/pause-cc951caf.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      360 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/phone-024e2f62.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      447 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/phone_lock-b885e81c.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      170 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/play-8bea5786.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1058 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/settings-342fb430.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      192 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/skip_next-1e2bfc6a.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      184 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/skip_prev-e81c8432.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      574 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/usb_disabled-467dd84d.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      496 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/assets/vehicle-8e6324e3.svg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      486 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/index.html
+-rw-r--r--   0 lameo     (1000) lameo     (1000)    10184 2023-06-01 02:41:58.000000 pilot-drive-0.2.0/pilot_drive/web/files/pilot_icon.png
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1604 2023-04-12 00:54:49.000000 pilot-drive-0.2.0/pilot_drive/web/web.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.629342 pilot-drive-0.2.0/pilot_drive.egg-info/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)      920 2023-06-01 02:42:01.000000 pilot-drive-0.2.0/pilot_drive.egg-info/PKG-INFO
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     3911 2023-06-01 02:42:01.000000 pilot-drive-0.2.0/pilot_drive.egg-info/SOURCES.txt
+-rw-r--r--   0 lameo     (1000) lameo     (1000)        1 2023-06-01 02:42:01.000000 pilot-drive-0.2.0/pilot_drive.egg-info/dependency_links.txt
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       57 2023-06-01 02:42:01.000000 pilot-drive-0.2.0/pilot_drive.egg-info/entry_points.txt
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       37 2023-06-01 02:42:01.000000 pilot-drive-0.2.0/pilot_drive.egg-info/requires.txt
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       17 2023-06-01 02:42:01.000000 pilot-drive-0.2.0/pilot_drive.egg-info/top_level.txt
+-rw-r--r--   0 lameo     (1000) lameo     (1000)       38 2023-06-01 02:42:01.634342 pilot-drive-0.2.0/setup.cfg
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     1303 2023-05-27 03:42:01.000000 pilot-drive-0.2.0/setup.py
+drwxr-xr-x   0 lameo     (1000) lameo     (1000)        0 2023-06-01 02:42:01.633342 pilot-drive-0.2.0/test/
+-rw-r--r--   0 lameo     (1000) lameo     (1000)        0 2023-04-12 00:54:49.000000 pilot-drive-0.2.0/test/__init__.py
+-rw-r--r--   0 lameo     (1000) lameo     (1000)     4042 2023-05-13 18:20:24.000000 pilot-drive-0.2.0/test/test_installer.py
```

### Comparing `pilot-drive-0.0.1/PKG-INFO` & `pilot-drive-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: pilot-drive
-Version: 0.0.1
-Summary: PILOT Auto is a modular vehicle head unit built in Python
-Home-page: https://github.com/lamemakes/pilot-auto
-Author: Wesley Appler
+Version: 0.2.0
+Summary: PILOT Drive is a modular vehicle head unit built in Python
+Home-page: https://github.com/lamemakes/pilot-drive
+Author: lamemakes
 Author-email: wes@lamemakes.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/lamemakes/pilot-auto/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+License: GNU GPL v3
+Project-URL: Documentation, https://pilot-drive.readthedocs.org
+Project-URL: Bug Tracker, https://github.com/lamemakes/pilot-drive/issues
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Unix
-Requires-Python: >=3.6
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PILOT
-An open source carPC operating system for Raspberry Pi written using Python 3.
-
-Full documentation is on the way along with a more detailed README, but in the 
-meantime feel free to ask questions, contribute, and give contrusctive criticism! 
-I'm new to the open source community, & absolutely taking any feedback I can get. 
-
-
 
+# The PILOT Drive Backend
 
+Built in Python 3.11, the backend utilizes a WebSocket to communicate with the UI along with multiple multiprocessing processes running simultaneously to allow for asynchrony.
```

### Comparing `pilot-drive-0.0.1/pilot_drive.egg-info/PKG-INFO` & `pilot-drive-0.2.0/pilot_drive.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 Metadata-Version: 2.1
 Name: pilot-drive
-Version: 0.0.1
-Summary: PILOT Auto is a modular vehicle head unit built in Python
-Home-page: https://github.com/lamemakes/pilot-auto
-Author: Wesley Appler
+Version: 0.2.0
+Summary: PILOT Drive is a modular vehicle head unit built in Python
+Home-page: https://github.com/lamemakes/pilot-drive
+Author: lamemakes
 Author-email: wes@lamemakes.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/lamemakes/pilot-auto/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+License: GNU GPL v3
+Project-URL: Documentation, https://pilot-drive.readthedocs.org
+Project-URL: Bug Tracker, https://github.com/lamemakes/pilot-drive/issues
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: Unix
-Requires-Python: >=3.6
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PILOT
-An open source carPC operating system for Raspberry Pi written using Python 3.
-
-Full documentation is on the way along with a more detailed README, but in the 
-meantime feel free to ask questions, contribute, and give contrusctive criticism! 
-I'm new to the open source community, & absolutely taking any feedback I can get. 
-
-
 
+# The PILOT Drive Backend
 
+Built in Python 3.11, the backend utilizes a WebSocket to communicate with the UI along with multiple multiprocessing processes running simultaneously to allow for asynchrony.
```

### Comparing `pilot-drive-0.0.1/setup.py` & `pilot-drive-0.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from setuptools import setup, find_packages
+from pilot_drive import __version__ as pilot_version
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="pilot-drive",
-    version="0.0.1",
-    author="Wesley Appler",
+    version=pilot_version,
+    author="lamemakes",
     author_email="wes@lamemakes.com",
-    description="PILOT Auto is a modular vehicle head unit built in Python",
+    description="PILOT Drive is a modular vehicle head unit built in Python",
+    license="GNU GPL v3",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/lamemakes/pilot-auto",
+    url="https://github.com/lamemakes/pilot-drive",
     project_urls={
-        "Bug Tracker": "https://github.com/lamemakes/pilot-auto/issues",
+        "Documentation": "https://pilot-drive.readthedocs.org",
+        "Bug Tracker": "https://github.com/lamemakes/pilot-drive/issues",
     },
+    install_requires=["websockets", "requests", "dasbus", "PyGObject"],
+    entry_points={"console_scripts": [
+        "pilot-drive = pilot_drive.__main__:run"]},
+    packages=find_packages(
+        exclude=["*.tests", "*.tests.*", "tests.*", "tests"]),
+    include_package_data=True,
+    python_requires=">=3.11",
     classifiers=[
-        "Programming Language :: Python :: 3",
+        "Environment :: Web Environment",
+        "Intended Audience :: End Users/Desktop",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-        "Operating System :: Unix",
+        "Operating System :: POSIX :: Linux",
     ],
-    install_requires=["flask", "obd"],
-    package_data={"pilot-drive": ["src/web/*", "tests/*"]},
-    packages=find_packages(include=["src", "src.*"]),
-    #entry_points={'console_scripts' : ["pilot-drive=pilot-drive.main:main"]},
-    python_requires=">=3.6",
-)
+)
```

### Comparing `pilot-drive-0.0.1/src/web/static/css/Futura.ttf` & `pilot-drive-0.2.0/pilot_drive/web/files/assets/Futura-0b7756bb.ttf`

 * *Files identical despite different names*

