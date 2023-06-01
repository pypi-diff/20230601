# Comparing `tmp/elvia-datascience-forecasting-2.3.2.tar.gz` & `tmp/elvia-datascience-forecasting-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elvia-datascience-forecasting-2.3.2.tar", last modified: Mon Jan 23 21:10:02 2023, max compression
+gzip compressed data, was "elvia-datascience-forecasting-2.3.3.tar", last modified: Thu Jun  1 14:34:53 2023, max compression
```

## Comparing `elvia-datascience-forecasting-2.3.2.tar` & `elvia-datascience-forecasting-2.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-01-23 21:10:02.304983 elvia-datascience-forecasting-2.3.2/
--rw-rw-rw-   0        0        0      146 2023-01-23 21:10:02.302981 elvia-datascience-forecasting-2.3.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-01-23 21:10:02.247981 elvia-datascience-forecasting-2.3.2/elvia_datascience_forecasting.egg-info/
--rw-rw-rw-   0        0        0      146 2023-01-23 21:10:02.000000 elvia-datascience-forecasting-2.3.2/elvia_datascience_forecasting.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1422 2023-01-23 21:10:02.000000 elvia-datascience-forecasting-2.3.2/elvia_datascience_forecasting.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-23 21:10:02.000000 elvia-datascience-forecasting-2.3.2/elvia_datascience_forecasting.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-01-23 21:10:02.000000 elvia-datascience-forecasting-2.3.2/elvia_datascience_forecasting.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-01-23 21:10:02.000000 elvia-datascience-forecasting-2.3.2/elvia_datascience_forecasting.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-23 21:10:02.253991 elvia-datascience-forecasting-2.3.2/forecast_dataprep/
--rw-rw-rw-   0        0        0       71 2023-01-23 21:09:06.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-23 21:10:02.275982 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/
--rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/__init__.py
--rw-rw-rw-   0        0        0     2037 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/cyclical_features.py
--rw-rw-rw-   0        0        0     1246 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/delayed_features.py
--rw-rw-rw-   0        0        0     2926 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/national_holiday.py
--rw-rw-rw-   0        0        0      845 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/prices.py
--rw-rw-rw-   0        0        0     4397 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/school_holiday.py
--rw-rw-rw-   0        0        0     1757 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/temperature.py
--rw-rw-rw-   0        0        0      180 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/time_constants.py
--rw-rw-rw-   0        0        0     1290 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/weekly_average.py
-drwxrwxrwx   0        0        0        0 2023-01-23 21:10:02.288982 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/
--rw-rw-rw-   0        0        0     2745 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/__init__.py
--rw-rw-rw-   0        0        0      259 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/bq_auth.py
--rw-rw-rw-   0        0        0     4940 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/common.py
--rw-rw-rw-   0        0        0      577 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/data_models.py
--rw-rw-rw-   0        0        0     3196 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/meteringpoints.py
--rw-rw-rw-   0        0        0     3277 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/substations.py
-drwxrwxrwx   0        0        0        0 2023-01-23 21:10:02.295004 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_ingestion/
--rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_ingestion/__init__.py
--rw-rw-rw-   0        0        0     2034 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_ingestion/prediction.py
--rw-rw-rw-   0        0        0     3083 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_ingestion/shared.py
--rw-rw-rw-   0        0        0     7296 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_ingestion/training.py
--rw-rw-rw-   0        0        0     3363 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_models.py
--rw-rw-rw-   0        0        0     8506 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/functions.py
-drwxrwxrwx   0        0        0        0 2023-01-23 21:10:02.301995 elvia-datascience-forecasting-2.3.2/forecast_dataprep/weather_api/
--rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/weather_api/__init__.py
--rw-rw-rw-   0        0        0     1193 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/weather_api/data_models.py
--rw-rw-rw-   0        0        0     8404 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.2/forecast_dataprep/weather_api/wrapper.py
--rw-rw-rw-   0        0        0      230 2023-01-18 21:23:05.000000 elvia-datascience-forecasting-2.3.2/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-23 21:10:02.304983 elvia-datascience-forecasting-2.3.2/setup.cfg
--rw-rw-rw-   0        0        0     1402 2023-01-23 21:07:35.000000 elvia-datascience-forecasting-2.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.277194 elvia-datascience-forecasting-2.3.3/
+-rw-rw-rw-   0        0        0      146 2023-06-01 14:34:53.276191 elvia-datascience-forecasting-2.3.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.193653 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/
+-rw-rw-rw-   0        0        0      146 2023-06-01 14:34:53.000000 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1422 2023-06-01 14:34:53.000000 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 14:34:53.000000 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      220 2023-06-01 14:34:53.000000 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-06-01 14:34:53.000000 elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.201647 elvia-datascience-forecasting-2.3.3/forecast_dataprep/
+-rw-rw-rw-   0        0        0       71 2023-06-01 14:33:20.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.231664 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/
+-rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/__init__.py
+-rw-rw-rw-   0        0        0     2037 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/cyclical_features.py
+-rw-rw-rw-   0        0        0     1246 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/delayed_features.py
+-rw-rw-rw-   0        0        0     2926 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/national_holiday.py
+-rw-rw-rw-   0        0        0      845 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/prices.py
+-rw-rw-rw-   0        0        0     4397 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/school_holiday.py
+-rw-rw-rw-   0        0        0     1757 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/temperature.py
+-rw-rw-rw-   0        0        0      180 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/time_constants.py
+-rw-rw-rw-   0        0        0     1290 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/weekly_average.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.252192 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/
+-rw-rw-rw-   0        0        0     2745 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/__init__.py
+-rw-rw-rw-   0        0        0      259 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/bq_auth.py
+-rw-rw-rw-   0        0        0     4940 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/common.py
+-rw-rw-rw-   0        0        0      577 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/data_models.py
+-rw-rw-rw-   0        0        0     3196 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/meteringpoints.py
+-rw-rw-rw-   0        0        0     3277 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/substations.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.264199 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/
+-rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/__init__.py
+-rw-rw-rw-   0        0        0     2034 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/prediction.py
+-rw-rw-rw-   0        0        0     3083 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/shared.py
+-rw-rw-rw-   0        0        0     7296 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/training.py
+-rw-rw-rw-   0        0        0     3367 2023-05-30 13:30:49.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_models.py
+-rw-rw-rw-   0        0        0     8506 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/functions.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:34:53.273196 elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/
+-rw-rw-rw-   0        0        0        0 2023-01-18 21:20:19.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/__init__.py
+-rw-rw-rw-   0        0        0     1193 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/data_models.py
+-rw-rw-rw-   0        0        0     8404 2023-01-23 21:07:36.000000 elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/wrapper.py
+-rw-rw-rw-   0        0        0      230 2023-01-18 21:23:05.000000 elvia-datascience-forecasting-2.3.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 14:34:53.278195 elvia-datascience-forecasting-2.3.3/setup.cfg
+-rw-rw-rw-   0        0        0     1402 2023-01-23 21:07:35.000000 elvia-datascience-forecasting-2.3.3/setup.py
```

### Comparing `elvia-datascience-forecasting-2.3.2/elvia_datascience_forecasting.egg-info/SOURCES.txt` & `elvia-datascience-forecasting-2.3.3/elvia_datascience_forecasting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/cyclical_features.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/cyclical_features.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/delayed_features.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/delayed_features.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/national_holiday.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/national_holiday.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/prices.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/prices.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/school_holiday.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/school_holiday.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/temperature.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/temperature.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_enrichment/weekly_average.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_enrichment/weekly_average.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/__init__.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/__init__.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/common.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/common.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/data_models.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/data_models.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/meteringpoints.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/meteringpoints.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_fetching/substations.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_fetching/substations.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_ingestion/prediction.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/prediction.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_ingestion/shared.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/shared.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_ingestion/training.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_ingestion/training.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/data_models.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/data_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                 identifier, int
         ) and identifier > 707057500014300000 and identifier < 707057500087400700:
             return ModelTargetLevel.METERING_POINT
         elif isinstance(identifier, str) and re.fullmatch(
                 r"7070575000[\d]{8}", identifier):
             return ModelTargetLevel.METERING_POINT
         elif isinstance(identifier, str) and re.fullmatch(
-                r"T[0-9A-Z\-]+", identifier.upper()):
+                r"[A-ZÆØÅ\d\-]+", identifier.upper()):
             return ModelTargetLevel.SUBSTATION
         return None
 
     @property
     def level(self) -> Optional[ModelTargetLevel]:
         return self.get_type(self.identifiers[0]) if self.identifiers else None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/functions.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/functions.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/weather_api/data_models.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/data_models.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/forecast_dataprep/weather_api/wrapper.py` & `elvia-datascience-forecasting-2.3.3/forecast_dataprep/weather_api/wrapper.py`

 * *Files identical despite different names*

### Comparing `elvia-datascience-forecasting-2.3.2/setup.py` & `elvia-datascience-forecasting-2.3.3/setup.py`

 * *Files identical despite different names*

