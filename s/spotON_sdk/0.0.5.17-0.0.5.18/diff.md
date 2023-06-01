# Comparing `tmp/spotON_sdk-0.0.5.17.tar.gz` & `tmp/spotON_sdk-0.0.5.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.5.17.tar", last modified: Tue May 30 08:34:57 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.5.18.tar", last modified: Thu Jun  1 08:14:03 2023, max compression
```

## Comparing `spotON_sdk-0.0.5.17.tar` & `spotON_sdk-0.0.5.18.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.17/.gitignore
--rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.17/.gitmodules
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.17/LICENSE
--rw-r--r--   0        0        0      416 2023-05-29 06:36:38.819802 spotON_sdk-0.0.5.17/pyproject.toml
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0      394 2023-05-29 09:36:49.354599 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/API_Call.py
--rw-r--r--   0        0        0     2303 2023-05-28 16:41:31.459722 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      263 2023-05-28 19:44:31.805887 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/customBaseModel.py
--rw-r--r--   0        0        0     2914 2023-05-30 08:34:42.268090 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     8239 2023-05-29 07:59:04.654185 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/timeframes.py
--rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.5.17/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      460 2023-05-30 08:34:48.854877 spotON_sdk-0.0.5.17/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.17/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.5.17/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.17/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.17/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.17/PKG-INFO
+-rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.18/.gitignore
+-rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.18/.gitmodules
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.18/LICENSE
+-rw-r--r--   0        0        0      416 2023-05-29 06:36:38.819802 spotON_sdk-0.0.5.18/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0      394 2023-05-29 09:36:49.354599 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/API_Call.py
+-rw-r--r--   0        0        0     2303 2023-05-28 16:41:31.459722 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      263 2023-05-28 19:44:31.805887 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/customBaseModel.py
+-rw-r--r--   0        0        0     2914 2023-05-30 08:34:42.268090 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     8239 2023-05-29 07:59:04.654185 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/timeframes.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.5.18/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      460 2023-06-01 08:13:50.841346 spotON_sdk-0.0.5.18/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.18/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.5.18/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.18/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.18/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.18/PKG-INFO
```

### Comparing `spotON_sdk-0.0.5.17/.gitignore` & `spotON_sdk-0.0.5.18/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.17/LICENSE` & `spotON_sdk-0.0.5.18/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.17/spotON_sdk/Logic/Price/timeframes.py` & `spotON_sdk-0.0.5.18/spotON_sdk/Logic/Price/timeframes.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.17/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.5.18/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.17/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.5.18/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*

