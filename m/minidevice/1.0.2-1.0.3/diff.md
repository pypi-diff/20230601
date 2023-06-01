# Comparing `tmp/minidevice-1.0.2.tar.gz` & `tmp/minidevice-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-1.0.2.tar", last modified: Thu Jun  1 03:24:43 2023, max compression
+gzip compressed data, was "minidevice-1.0.3.tar", last modified: Thu Jun  1 04:19:08 2023, max compression
```

## Comparing `minidevice-1.0.2.tar` & `minidevice-1.0.3.tar`

### file list

```diff
@@ -1,19 +1,193 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 03:24:43.873790 minidevice-1.0.2/
--rw-rw-rw-   0        0        0     1205 2023-06-01 03:24:43.872809 minidevice-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      901 2023-06-01 01:33:14.000000 minidevice-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 03:24:43.842845 minidevice-1.0.2/minidevice/
--rw-rw-rw-   0        0        0       30 2023-06-01 03:24:16.000000 minidevice-1.0.2/minidevice/__init__.py
--rw-rw-rw-   0        0        0     2040 2023-06-01 01:14:31.000000 minidevice-1.0.2/minidevice/adb.py
--rw-rw-rw-   0        0        0      269 2023-05-31 10:26:49.000000 minidevice-1.0.2/minidevice/config.py
--rw-rw-rw-   0        0        0     2742 2023-06-01 01:29:57.000000 minidevice-1.0.2/minidevice/device.py
--rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.2/minidevice/minicap.py
--rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.2/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.2/minidevice/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-01 03:24:43.871810 minidevice-1.0.2/minidevice.egg-info/
--rw-rw-rw-   0        0        0     1205 2023-06-01 03:24:43.000000 minidevice-1.0.2/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-06-01 03:24:43.000000 minidevice-1.0.2/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 03:24:43.000000 minidevice-1.0.2/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2023-06-01 03:24:43.000000 minidevice-1.0.2/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-01 03:24:43.000000 minidevice-1.0.2/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 03:24:43.873790 minidevice-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      665 2023-06-01 03:24:08.000000 minidevice-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.346305 minidevice-1.0.3/
+-rw-rw-rw-   0        0        0       32 2023-06-01 04:17:59.000000 minidevice-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1394 2023-06-01 04:19:08.292128 minidevice-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1090 2023-06-01 04:04:50.000000 minidevice-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.790991 minidevice-1.0.3/minidevice/
+-rw-rw-rw-   0        0        0       30 2023-06-01 03:24:16.000000 minidevice-1.0.3/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     2040 2023-06-01 01:14:31.000000 minidevice-1.0.3/minidevice/adb.py
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.809808 minidevice-1.0.3/minidevice/bin/
+-rw-rw-rw-   0        0        0    97792 2023-03-12 01:13:21.000000 minidevice-1.0.3/minidevice/bin/AdbWinApi.dll
+-rw-rw-rw-   0        0        0    62976 2023-03-12 01:13:21.000000 minidevice-1.0.3/minidevice/bin/AdbWinUsbApi.dll
+-rwxrwxrwx   0        0        0  6021632 2023-03-12 01:13:21.000000 minidevice-1.0.3/minidevice/bin/adb.exe
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.764963 minidevice-1.0.3/minidevice/bin/minicap/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.763010 minidevice-1.0.3/minidevice/bin/minicap/jni/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.709643 minidevice-1.0.3/minidevice/bin/minicap/jni/android-10/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.823548 minidevice-1.0.3/minidevice/bin/minicap/jni/android-10/armeabi-v7a/
+-rw-rw-rw-   0        0        0     9688 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-10/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.711776 minidevice-1.0.3/minidevice/bin/minicap/jni/android-14/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.829452 minidevice-1.0.3/minidevice/bin/minicap/jni/android-14/armeabi-v7a/
+-rw-rw-rw-   0        0        0     5700 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-14/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.836283 minidevice-1.0.3/minidevice/bin/minicap/jni/android-14/x86/
+-rw-rw-rw-   0        0        0    11385 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-14/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.713727 minidevice-1.0.3/minidevice/bin/minicap/jni/android-15/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.841932 minidevice-1.0.3/minidevice/bin/minicap/jni/android-15/armeabi-v7a/
+-rw-rw-rw-   0        0        0     5700 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-15/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.848318 minidevice-1.0.3/minidevice/bin/minicap/jni/android-15/x86/
+-rw-rw-rw-   0        0        0    11385 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-15/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.714703 minidevice-1.0.3/minidevice/bin/minicap/jni/android-16/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.854349 minidevice-1.0.3/minidevice/bin/minicap/jni/android-16/armeabi-v7a/
+-rw-rw-rw-   0        0        0     9420 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-16/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.860768 minidevice-1.0.3/minidevice/bin/minicap/jni/android-16/x86/
+-rw-rw-rw-   0        0        0    11929 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-16/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.716656 minidevice-1.0.3/minidevice/bin/minicap/jni/android-17/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.866623 minidevice-1.0.3/minidevice/bin/minicap/jni/android-17/armeabi-v7a/
+-rw-rw-rw-   0        0        0    13472 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-17/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.873505 minidevice-1.0.3/minidevice/bin/minicap/jni/android-17/x86/
+-rw-rw-rw-   0        0        0    23907 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-17/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.717631 minidevice-1.0.3/minidevice/bin/minicap/jni/android-18/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.880385 minidevice-1.0.3/minidevice/bin/minicap/jni/android-18/armeabi-v7a/
+-rw-rw-rw-   0        0        0    13492 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-18/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.887219 minidevice-1.0.3/minidevice/bin/minicap/jni/android-18/x86/
+-rw-rw-rw-   0        0        0    23491 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-18/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.719631 minidevice-1.0.3/minidevice/bin/minicap/jni/android-19/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.893638 minidevice-1.0.3/minidevice/bin/minicap/jni/android-19/armeabi-v7a/
+-rw-rw-rw-   0        0        0    13488 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-19/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.900516 minidevice-1.0.3/minidevice/bin/minicap/jni/android-19/x86/
+-rw-rw-rw-   0        0        0    23725 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-19/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.722973 minidevice-1.0.3/minidevice/bin/minicap/jni/android-21/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.906374 minidevice-1.0.3/minidevice/bin/minicap/jni/android-21/arm64-v8a/
+-rw-rw-rw-   0        0        0    22000 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-21/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.912834 minidevice-1.0.3/minidevice/bin/minicap/jni/android-21/armeabi-v7a/
+-rw-rw-rw-   0        0        0    13492 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-21/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.918720 minidevice-1.0.3/minidevice/bin/minicap/jni/android-21/x86/
+-rw-rw-rw-   0        0        0    21676 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-21/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.924931 minidevice-1.0.3/minidevice/bin/minicap/jni/android-21/x86_64/
+-rw-rw-rw-   0        0        0    26328 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-21/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.725900 minidevice-1.0.3/minidevice/bin/minicap/jni/android-22/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.931696 minidevice-1.0.3/minidevice/bin/minicap/jni/android-22/arm64-v8a/
+-rw-rw-rw-   0        0        0    22000 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-22/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.937551 minidevice-1.0.3/minidevice/bin/minicap/jni/android-22/armeabi-v7a/
+-rw-rw-rw-   0        0        0    13492 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-22/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.944522 minidevice-1.0.3/minidevice/bin/minicap/jni/android-22/x86/
+-rw-rw-rw-   0        0        0    21676 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-22/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.951404 minidevice-1.0.3/minidevice/bin/minicap/jni/android-22/x86_64/
+-rw-rw-rw-   0        0        0    26328 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-22/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.729389 minidevice-1.0.3/minidevice/bin/minicap/jni/android-23/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.957259 minidevice-1.0.3/minidevice/bin/minicap/jni/android-23/arm64-v8a/
+-rw-rw-rw-   0        0        0    22328 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-23/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.963666 minidevice-1.0.3/minidevice/bin/minicap/jni/android-23/armeabi-v7a/
+-rw-rw-rw-   0        0        0    22128 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-23/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.969571 minidevice-1.0.3/minidevice/bin/minicap/jni/android-23/x86/
+-rw-rw-rw-   0        0        0    21932 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-23/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.977379 minidevice-1.0.3/minidevice/bin/minicap/jni/android-23/x86_64/
+-rw-rw-rw-   0        0        0    26688 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-23/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.732552 minidevice-1.0.3/minidevice/bin/minicap/jni/android-24/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.983744 minidevice-1.0.3/minidevice/bin/minicap/jni/android-24/arm64-v8a/
+-rw-rw-rw-   0        0        0    22576 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-24/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.989664 minidevice-1.0.3/minidevice/bin/minicap/jni/android-24/armeabi-v7a/
+-rw-rw-rw-   0        0        0    22100 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-24/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.996724 minidevice-1.0.3/minidevice/bin/minicap/jni/android-24/x86/
+-rw-rw-rw-   0        0        0    21944 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-24/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.002965 minidevice-1.0.3/minidevice/bin/minicap/jni/android-24/x86_64/
+-rw-rw-rw-   0        0        0    26672 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-24/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.736456 minidevice-1.0.3/minidevice/bin/minicap/jni/android-25/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.009912 minidevice-1.0.3/minidevice/bin/minicap/jni/android-25/arm64-v8a/
+-rw-rw-rw-   0        0        0    22576 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-25/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.015797 minidevice-1.0.3/minidevice/bin/minicap/jni/android-25/armeabi-v7a/
+-rw-rw-rw-   0        0        0    22100 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-25/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.021700 minidevice-1.0.3/minidevice/bin/minicap/jni/android-25/x86/
+-rw-rw-rw-   0        0        0    21944 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-25/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.028567 minidevice-1.0.3/minidevice/bin/minicap/jni/android-25/x86_64/
+-rw-rw-rw-   0        0        0    26672 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-25/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.740604 minidevice-1.0.3/minidevice/bin/minicap/jni/android-26/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.033789 minidevice-1.0.3/minidevice/bin/minicap/jni/android-26/arm64-v8a/
+-rw-rw-rw-   0        0        0    23592 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-26/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.040060 minidevice-1.0.3/minidevice/bin/minicap/jni/android-26/armeabi-v7a/
+-rw-rw-rw-   0        0        0    24760 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-26/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.045919 minidevice-1.0.3/minidevice/bin/minicap/jni/android-26/x86/
+-rw-rw-rw-   0        0        0    22588 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-26/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.052631 minidevice-1.0.3/minidevice/bin/minicap/jni/android-26/x86_64/
+-rw-rw-rw-   0        0        0    27280 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-26/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.744506 minidevice-1.0.3/minidevice/bin/minicap/jni/android-27/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.057513 minidevice-1.0.3/minidevice/bin/minicap/jni/android-27/arm64-v8a/
+-rw-rw-rw-   0        0        0    23592 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-27/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.063791 minidevice-1.0.3/minidevice/bin/minicap/jni/android-27/armeabi-v7a/
+-rw-rw-rw-   0        0        0    24784 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-27/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.070696 minidevice-1.0.3/minidevice/bin/minicap/jni/android-27/x86/
+-rw-rw-rw-   0        0        0    22564 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-27/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.076552 minidevice-1.0.3/minidevice/bin/minicap/jni/android-27/x86_64/
+-rw-rw-rw-   0        0        0    27280 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-27/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.746461 minidevice-1.0.3/minidevice/bin/minicap/jni/android-28/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.081485 minidevice-1.0.3/minidevice/bin/minicap/jni/android-28/arm64-v8a/
+-rw-rw-rw-   0        0        0    68736 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-28/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.087341 minidevice-1.0.3/minidevice/bin/minicap/jni/android-28/armeabi-v7a/
+-rw-rw-rw-   0        0        0    28900 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-28/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.094237 minidevice-1.0.3/minidevice/bin/minicap/jni/android-28/x86/
+-rw-rw-rw-   0        0        0    23032 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-28/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.099667 minidevice-1.0.3/minidevice/bin/minicap/jni/android-28/x86_64/
+-rw-rw-rw-   0        0        0    27776 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-28/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.751759 minidevice-1.0.3/minidevice/bin/minicap/jni/android-29/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.106514 minidevice-1.0.3/minidevice/bin/minicap/jni/android-29/arm64-v8a/
+-rw-rw-rw-   0        0        0    29088 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-29/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.112963 minidevice-1.0.3/minidevice/bin/minicap/jni/android-29/armeabi-v7a/
+-rw-rw-rw-   0        0        0    28888 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-29/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.121332 minidevice-1.0.3/minidevice/bin/minicap/jni/android-29/x86/
+-rw-rw-rw-   0        0        0    31868 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-29/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.128694 minidevice-1.0.3/minidevice/bin/minicap/jni/android-29/x86_64/
+-rw-rw-rw-   0        0        0    37272 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-29/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.754688 minidevice-1.0.3/minidevice/bin/minicap/jni/android-30/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.135549 minidevice-1.0.3/minidevice/bin/minicap/jni/android-30/arm64-v8a/
+-rw-rw-rw-   0        0        0    25136 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-30/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.143418 minidevice-1.0.3/minidevice/bin/minicap/jni/android-30/armeabi-v7a/
+-rw-rw-rw-   0        0        0    21360 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-30/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.154249 minidevice-1.0.3/minidevice/bin/minicap/jni/android-30/x86/
+-rw-rw-rw-   0        0        0    21272 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-30/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.161640 minidevice-1.0.3/minidevice/bin/minicap/jni/android-30/x86_64/
+-rw-rw-rw-   0        0        0    23448 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-30/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.758622 minidevice-1.0.3/minidevice/bin/minicap/jni/android-31/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.167497 minidevice-1.0.3/minidevice/bin/minicap/jni/android-31/arm64-v8a/
+-rw-rw-rw-   0        0        0    24488 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-31/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.174835 minidevice-1.0.3/minidevice/bin/minicap/jni/android-31/armeabi-v7a/
+-rw-rw-rw-   0        0        0    20956 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-31/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.181713 minidevice-1.0.3/minidevice/bin/minicap/jni/android-31/x86/
+-rw-rw-rw-   0        0        0    20532 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-31/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.190570 minidevice-1.0.3/minidevice/bin/minicap/jni/android-31/x86_64/
+-rw-rw-rw-   0        0        0    20136 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-31/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.762035 minidevice-1.0.3/minidevice/bin/minicap/jni/android-32/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.197402 minidevice-1.0.3/minidevice/bin/minicap/jni/android-32/arm64-v8a/
+-rw-rw-rw-   0        0        0    24488 2023-04-15 05:48:30.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-32/arm64-v8a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.204289 minidevice-1.0.3/minidevice/bin/minicap/jni/android-32/armeabi-v7a/
+-rw-rw-rw-   0        0        0    20956 2023-04-15 05:48:30.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-32/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.212234 minidevice-1.0.3/minidevice/bin/minicap/jni/android-32/x86/
+-rw-rw-rw-   0        0        0    20532 2023-04-15 05:48:30.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-32/x86/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.235293 minidevice-1.0.3/minidevice/bin/minicap/jni/android-32/x86_64/
+-rw-rw-rw-   0        0        0   176193 2023-05-31 05:40:13.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-32/x86_64/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.763987 minidevice-1.0.3/minidevice/bin/minicap/jni/android-9/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.240738 minidevice-1.0.3/minidevice/bin/minicap/jni/android-9/armeabi-v7a/
+-rw-rw-rw-   0        0        0     9688 2023-04-15 03:42:07.000000 minidevice-1.0.3/minidevice/bin/minicap/jni/android-9/armeabi-v7a/minicap.so
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.766914 minidevice-1.0.3/minidevice/bin/minicap/libs/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.248576 minidevice-1.0.3/minidevice/bin/minicap/libs/arm64-v8a/
+-rw-rw-rw-   0        0        0   537552 2023-04-15 05:39:49.000000 minidevice-1.0.3/minidevice/bin/minicap/libs/arm64-v8a/minicap
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.257386 minidevice-1.0.3/minidevice/bin/minicap/libs/armeabi-v7a/
+-rw-rw-rw-   0        0        0   298356 2023-04-15 05:39:37.000000 minidevice-1.0.3/minidevice/bin/minicap/libs/armeabi-v7a/minicap
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.266561 minidevice-1.0.3/minidevice/bin/minicap/libs/x86/
+-rw-rw-rw-   0        0        0   651488 2023-04-15 05:40:06.000000 minidevice-1.0.3/minidevice/bin/minicap/libs/x86/minicap
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.275827 minidevice-1.0.3/minidevice/bin/minicap/libs/x86_64/
+-rw-rw-rw-   0        0        0   665096 2023-04-15 05:40:18.000000 minidevice-1.0.3/minidevice/bin/minicap/libs/x86_64/minicap
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.766914 minidevice-1.0.3/minidevice/bin/minitouch/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:32.770709 minidevice-1.0.3/minidevice/bin/minitouch/libs/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.290786 minidevice-1.0.3/minidevice/bin/minitouch/libs/arm64-v8a/
+-rw-rw-rw-   0        0        0    25528 2023-04-27 11:32:08.000000 minidevice-1.0.3/minidevice/bin/minitouch/libs/arm64-v8a/minitouch
+-rw-rw-rw-   0        0        0    25528 2023-04-27 11:32:08.000000 minidevice-1.0.3/minidevice/bin/minitouch/libs/arm64-v8a/minitouch-nopie
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.303540 minidevice-1.0.3/minidevice/bin/minitouch/libs/armeabi-v7a/
+-rw-rw-rw-   0        0        0    17272 2023-04-27 11:32:08.000000 minidevice-1.0.3/minidevice/bin/minitouch/libs/armeabi-v7a/minitouch
+-rw-rw-rw-   0        0        0    17272 2023-04-27 11:32:08.000000 minidevice-1.0.3/minidevice/bin/minitouch/libs/armeabi-v7a/minitouch-nopie
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.321273 minidevice-1.0.3/minidevice/bin/minitouch/libs/x86/
+-rw-rw-rw-   0        0        0    25684 2023-04-27 11:32:08.000000 minidevice-1.0.3/minidevice/bin/minitouch/libs/x86/minitouch
+-rw-rw-rw-   0        0        0    25684 2023-04-27 11:32:08.000000 minidevice-1.0.3/minidevice/bin/minitouch/libs/x86/minitouch-nopie
+drwxrwxrwx   0        0        0        0 2023-06-01 04:18:33.336478 minidevice-1.0.3/minidevice/bin/minitouch/libs/x86_64/
+-rw-rw-rw-   0        0        0    27464 2023-04-27 11:32:08.000000 minidevice-1.0.3/minidevice/bin/minitouch/libs/x86_64/minitouch
+-rw-rw-rw-   0        0        0    27464 2023-04-27 11:32:08.000000 minidevice-1.0.3/minidevice/bin/minitouch/libs/x86_64/minitouch-nopie
+-rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.0.3/minidevice/config.py
+-rw-rw-rw-   0        0        0     2742 2023-06-01 01:29:57.000000 minidevice-1.0.3/minidevice/device.py
+-rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.3/minidevice/minicap.py
+-rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.3/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.3/minidevice/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-01 04:19:08.276959 minidevice-1.0.3/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     1394 2023-06-01 04:19:07.000000 minidevice-1.0.3/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4572 2023-06-01 04:19:08.000000 minidevice-1.0.3/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 04:19:07.000000 minidevice-1.0.3/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-06-01 04:19:08.000000 minidevice-1.0.3/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-01 04:19:08.000000 minidevice-1.0.3/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 04:19:08.294080 minidevice-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      829 2023-06-01 04:17:41.000000 minidevice-1.0.3/setup.py
```

### Comparing `minidevice-1.0.2/PKG-INFO` & `minidevice-1.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.2
+Version: 1.0.3
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Platform: UNKNOWN
@@ -38,8 +38,18 @@
 
 ### miniSwipe
 滑动
 - `pointArray` 滑动坐标列表 格式为`[(x,y),(x,y),(x,y),(x,y)]`
 - `duration`(可选) 持续时长 默认500ms
 - `pressure`(可选) 压力 默认100 仅使用minitouch时生效
 
+- `minidevice`
+    - `minicap/`
+    - `minitouch/`
+    - `adb.exe`
+    - `__init__.py`
+    - `adb.py`
+    - `AdbWinApi.dll`
+    - `AdbWinUsbApi.dll`
+    - `utils.py`
+项目结构
```

### Comparing `minidevice-1.0.2/README.md` & `minidevice-1.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -24,7 +24,18 @@
 - `pressure`(可选) 压力 默认100 仅使用minitouch时生效
 
 ### miniSwipe
 滑动
 - `pointArray` 滑动坐标列表 格式为`[(x,y),(x,y),(x,y),(x,y)]`
 - `duration`(可选) 持续时长 默认500ms
 - `pressure`(可选) 压力 默认100 仅使用minitouch时生效
+
+- `minidevice`
+    - `minicap/`
+    - `minitouch/`
+    - `adb.exe`
+    - `__init__.py`
+    - `adb.py`
+    - `AdbWinApi.dll`
+    - `AdbWinUsbApi.dll`
+    - `utils.py`
+项目结构
```

### Comparing `minidevice-1.0.2/minidevice/adb.py` & `minidevice-1.0.3/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.2/minidevice/device.py` & `minidevice-1.0.3/minidevice/device.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.2/minidevice/minicap.py` & `minidevice-1.0.3/minidevice/minicap.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.2/minidevice.egg-info/PKG-INFO` & `minidevice-1.0.3/minidevice.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.2
+Version: 1.0.3
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Platform: UNKNOWN
@@ -38,8 +38,18 @@
 
 ### miniSwipe
 滑动
 - `pointArray` 滑动坐标列表 格式为`[(x,y),(x,y),(x,y),(x,y)]`
 - `duration`(可选) 持续时长 默认500ms
 - `pressure`(可选) 压力 默认100 仅使用minitouch时生效
 
+- `minidevice`
+    - `minicap/`
+    - `minitouch/`
+    - `adb.exe`
+    - `__init__.py`
+    - `adb.py`
+    - `AdbWinApi.dll`
+    - `AdbWinUsbApi.dll`
+    - `utils.py`
+项目结构
```

### Comparing `minidevice-1.0.2/setup.py` & `minidevice-1.0.3/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from setuptools import setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='1.0.2',
+      version='1.0.3',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku',
       license='MIT',
       keywords='game',
       project_urls={},
       packages=['minidevice'],
-      install_requires=['opencv-python>=4.7.0.72', 'uiautomator2>=2.16.23','pyminitouch>=0.3.3'],
+      package_data={
+          "minidevice": ["bin/*","bin/minicap/*"]},
+      install_requires=['opencv-python>=4.7.0.72',
+                        'uiautomator2>=2.16.23',
+                        'pyminitouch>=0.3.3', 
+                        'urllib3'],
       python_requires='>=3'
-     )
+      )
```

