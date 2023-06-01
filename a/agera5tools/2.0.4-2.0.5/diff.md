# Comparing `tmp/agera5tools-2.0.4.tar.gz` & `tmp/agera5tools-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agera5tools-2.0.4.tar", last modified: Thu Mar 16 16:14:47 2023, max compression
+gzip compressed data, was "agera5tools-2.0.5.tar", last modified: Thu Jun  1 09:43:45 2023, max compression
```

## Comparing `agera5tools-2.0.4.tar` & `agera5tools-2.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 wit015    (1000) wit015    (1000)        0 2023-03-16 16:14:47.472046 agera5tools-2.0.4/
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     1070 2021-04-23 11:28:38.000000 agera5tools-2.0.4/LICENSE
--rw-rw-r--   0 wit015    (1000) wit015    (1000)      116 2023-01-13 16:22:24.000000 agera5tools-2.0.4/MANIFEST.in
--rw-rw-r--   0 wit015    (1000) wit015    (1000)    10359 2023-03-16 16:14:47.472046 agera5tools-2.0.4/PKG-INFO
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     9805 2023-01-13 16:22:24.000000 agera5tools-2.0.4/README.md
-drwxrwxr-x   0 wit015    (1000) wit015    (1000)        0 2023-03-16 16:14:47.468046 agera5tools-2.0.4/agera5tools/
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     4925 2023-03-16 16:13:06.000000 agera5tools-2.0.4/agera5tools/__init__.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     3383 2023-03-16 16:11:30.000000 agera5tools-2.0.4/agera5tools/agera5tools.yaml
--rw-rw-r--   0 wit015    (1000) wit015    (1000)    11251 2023-02-02 12:54:57.000000 agera5tools-2.0.4/agera5tools/build.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     1427 2023-01-13 16:22:24.000000 agera5tools-2.0.4/agera5tools/check.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     7844 2023-02-02 12:54:57.000000 agera5tools-2.0.4/agera5tools/cmd.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     3233 2023-03-01 14:21:37.000000 agera5tools-2.0.4/agera5tools/db_data_provider.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     2484 2023-01-13 16:22:24.000000 agera5tools-2.0.4/agera5tools/dump_clip.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)      871 2023-01-13 16:22:24.000000 agera5tools-2.0.4/agera5tools/dump_grid.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     1996 2023-01-13 16:22:24.000000 agera5tools-2.0.4/agera5tools/extract_point.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000) 12522296 2021-04-27 09:04:22.000000 agera5tools-2.0.4/agera5tools/grid_elevation_landfraction.nc
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     2682 2023-01-13 16:22:24.000000 agera5tools-2.0.4/agera5tools/help.html
--rwxrwxr-x   0 wit015    (1000) wit015    (1000)     2388 2023-01-13 16:22:24.000000 agera5tools-2.0.4/agera5tools/help.md
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     4039 2023-03-16 16:13:06.000000 agera5tools-2.0.4/agera5tools/init.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     5275 2023-02-02 12:54:57.000000 agera5tools-2.0.4/agera5tools/mirror.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     2437 2023-03-01 14:21:37.000000 agera5tools-2.0.4/agera5tools/server.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)    11375 2023-03-01 14:21:37.000000 agera5tools-2.0.4/agera5tools/util.py
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     4490 2023-03-16 16:11:30.000000 agera5tools-2.0.4/agera5tools/wdp.py
-drwxrwxr-x   0 wit015    (1000) wit015    (1000)        0 2023-03-16 16:14:47.472046 agera5tools-2.0.4/agera5tools.egg-info/
--rw-rw-r--   0 wit015    (1000) wit015    (1000)    10359 2023-03-16 16:14:47.000000 agera5tools-2.0.4/agera5tools.egg-info/PKG-INFO
--rw-rw-r--   0 wit015    (1000) wit015    (1000)      635 2023-03-16 16:14:47.000000 agera5tools-2.0.4/agera5tools.egg-info/SOURCES.txt
--rw-rw-r--   0 wit015    (1000) wit015    (1000)        1 2023-03-16 16:14:47.000000 agera5tools-2.0.4/agera5tools.egg-info/dependency_links.txt
--rw-rw-r--   0 wit015    (1000) wit015    (1000)       52 2023-03-16 16:14:47.000000 agera5tools-2.0.4/agera5tools.egg-info/entry_points.txt
--rw-rw-r--   0 wit015    (1000) wit015    (1000)       12 2023-03-16 16:14:47.000000 agera5tools-2.0.4/agera5tools.egg-info/top_level.txt
--rw-rw-r--   0 wit015    (1000) wit015    (1000)     1049 2023-03-16 16:13:06.000000 agera5tools-2.0.4/pyproject.toml
--rw-rw-r--   0 wit015    (1000) wit015    (1000)       38 2023-03-16 16:14:47.472046 agera5tools-2.0.4/setup.cfg
+drwxrwxr-x   0 wit015    (1000) wit015    (1000)        0 2023-06-01 09:43:45.411119 agera5tools-2.0.5/
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     1070 2021-04-23 11:28:38.000000 agera5tools-2.0.5/LICENSE
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)      116 2023-01-13 16:22:24.000000 agera5tools-2.0.5/MANIFEST.in
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)    10359 2023-06-01 09:43:45.407119 agera5tools-2.0.5/PKG-INFO
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     9805 2023-01-13 16:22:24.000000 agera5tools-2.0.5/README.md
+drwxrwxr-x   0 wit015    (1000) wit015    (1000)        0 2023-06-01 09:43:45.407119 agera5tools-2.0.5/agera5tools/
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     4925 2023-06-01 09:35:41.000000 agera5tools-2.0.5/agera5tools/__init__.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     3403 2023-06-01 09:34:05.000000 agera5tools-2.0.5/agera5tools/agera5tools.yaml
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)    11907 2023-06-01 09:34:05.000000 agera5tools-2.0.5/agera5tools/build.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     1427 2023-01-13 16:22:24.000000 agera5tools-2.0.5/agera5tools/check.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     7842 2023-06-01 09:34:05.000000 agera5tools-2.0.5/agera5tools/cmd.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     3233 2023-03-01 14:21:37.000000 agera5tools-2.0.5/agera5tools/db_data_provider.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     2484 2023-01-13 16:22:24.000000 agera5tools-2.0.5/agera5tools/dump_clip.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)      871 2023-01-13 16:22:24.000000 agera5tools-2.0.5/agera5tools/dump_grid.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     1996 2023-01-13 16:22:24.000000 agera5tools-2.0.5/agera5tools/extract_point.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000) 12522296 2021-04-27 09:04:22.000000 agera5tools-2.0.5/agera5tools/grid_elevation_landfraction.nc
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     2682 2023-01-13 16:22:24.000000 agera5tools-2.0.5/agera5tools/help.html
+-rwxrwxr-x   0 wit015    (1000) wit015    (1000)     2388 2023-01-13 16:22:24.000000 agera5tools-2.0.5/agera5tools/help.md
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     4039 2023-03-16 16:13:06.000000 agera5tools-2.0.5/agera5tools/init.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     5429 2023-06-01 09:34:05.000000 agera5tools-2.0.5/agera5tools/mirror.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     2437 2023-03-01 14:21:37.000000 agera5tools-2.0.5/agera5tools/server.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)    11743 2023-06-01 09:34:05.000000 agera5tools-2.0.5/agera5tools/util.py
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     4490 2023-03-16 16:11:30.000000 agera5tools-2.0.5/agera5tools/wdp.py
+drwxrwxr-x   0 wit015    (1000) wit015    (1000)        0 2023-06-01 09:43:45.407119 agera5tools-2.0.5/agera5tools.egg-info/
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)    10359 2023-06-01 09:43:45.000000 agera5tools-2.0.5/agera5tools.egg-info/PKG-INFO
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)      635 2023-06-01 09:43:45.000000 agera5tools-2.0.5/agera5tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)        1 2023-06-01 09:43:45.000000 agera5tools-2.0.5/agera5tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)       52 2023-06-01 09:43:45.000000 agera5tools-2.0.5/agera5tools.egg-info/entry_points.txt
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)       12 2023-06-01 09:43:45.000000 agera5tools-2.0.5/agera5tools.egg-info/top_level.txt
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)     1049 2023-06-01 09:35:41.000000 agera5tools-2.0.5/pyproject.toml
+-rw-rw-r--   0 wit015    (1000) wit015    (1000)       38 2023-06-01 09:43:45.411119 agera5tools-2.0.5/setup.cfg
```

### Comparing `agera5tools-2.0.4/LICENSE` & `agera5tools-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/PKG-INFO` & `agera5tools-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agera5tools
-Version: 2.0.4
+Version: 2.0.5
 Summary: AgERA5 is a tool for handling AgERA5 data from the Copernicus Climate Data Store.
 Author-email: Allard de Wit <allard.dewit@wur.nl>
 Project-URL: Homepage, https://github.com/ajwdewit/agera5tools
 Project-URL: documentation, https://agera5tools.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `agera5tools-2.0.4/README.md` & `agera5tools-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/__init__.py` & `agera5tools-2.0.5/agera5tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import yaml
 from dotmap import DotMap
 import click
 
 from . import util
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 
 def setup_logging(config, has_filesystem):
     """sets up the logging system for both logging to file and to console.
 
     file logging is based on a rotating file handler to avoid log files becoming very large.
 
     :param config: a configuration object.
```

### Comparing `agera5tools-2.0.4/agera5tools/agera5tools.yaml` & `agera5tools-2.0.5/agera5tools/agera5tools.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,15 @@
   # The data source name (dsn) points to the database and should have the form of an
   # SQLAlchemy database URL: https://docs.sqlalchemy.org/en/20/core/engines.html
   # Note that the URL may contain the database password in plain text which is a security
   # risk.
   dsn: sqlite:////tmp/agera5/agera5.db
   agera5_table_name: weather_grid_agera5
   grid_table_name: grid_agera5
+  chunk_size: 10000
 data_storage:
   # Storage path for NetCDF files, CSV files and temporary storage.
   netcdf_path: /tmp/agera5/ncfiles/
   keep_netcdf: yes
   tmp_path: /tmp/agera5/tmp
   csv_path: /tmp/agera5/csv
 variables:
```

### Comparing `agera5tools-2.0.4/agera5tools/build.py` & `agera5tools-2.0.5/agera5tools/build.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- coding: utf-8 -*-
 # Copyright (c) December 2022, Wageningen Environmental Research
 # Allard de Wit (allard.dewit@wur.nl)
 import logging
 import shutil
+import time
 from uuid import uuid4
 import datetime as dt
 from zipfile import ZipFile
 import concurrent.futures
 import copy
 from itertools import product
 
 import cdsapi
-import sqlalchemy as sa
 import xarray as xr
+import sqlalchemy as sa
 
-from .util import days_in_month, variable_names, create_target_fname, last_day_in_month, add_grid, convert_to_celsius
+from .util import days_in_month, variable_names, create_target_fname, last_day_in_month, \
+    add_grid, convert_to_celsius, chunker
 from . import config
 
 
 def parse_date_from_zipfname(zipfname):
     """Parse the date from the filename and returns a date object.
     """
     d = zipfname.filename.split("_")[3]
@@ -117,14 +119,15 @@
 
 def modify_dataframe(df):
     """Modifies the dataframe to have it properly formatted. Such as:
      - Renaming columns and forcing them into lower case
      - Make the 'day' column a proper date object
      - reset the index and remove lat/lon columns
      - removing rows with N/A values
+     - removing rows with idgrid == -999
      - convert Kelvin to Celsius if configured so.
 
     :param df: a dataframe with AgERA5 data
     :return: a modified dataframe
     """
     # Rename columns
     rename_cols = {c:c.lower() for c in df.columns}
@@ -143,14 +146,19 @@
     # Convert day to a proper date object
     df["day"] = df["day"].dt.date
 
     # Remove any rows with N/A values
     ix = df.isna().any(axis=1)
     df = df[~ix]
 
+    # Remove rows with idgrid == -999
+    # this represents grids at the lowest row
+    ix = df.idgrid == -999
+    df = df[~ix]
+
     # Convert Kelvin to Celsius if configured
     if config.misc.kelvin_to_celsius:
         df = convert_to_celsius(df)
 
     # Solar radiation flux can be integer for more compact output
     if "solar_radiation_flux" in df.columns:
         df["solar_radiation_flux"] = df.solar_radiation_flux.astype(int)
@@ -175,18 +183,29 @@
     """Insert dataframe rows into the database.
 
     :param df: a dataframe with AgERA5 data
     :param descriptor: a descriptor for this set of data, usually year-month ("2000-01") or a date ("2000-01-01")
     """
     logger = logging.getLogger(__name__)
     engine = sa.create_engine(config.database.dsn)
+    meta = sa.MetaData(engine)
+    tbl = sa.Table(config.database.agera5_table_name, meta, autoload=True)
     try:
+        recs = df.to_dict(orient="records")
+        nrecs_written = 0
+        t1 = time.time()
         with engine.begin() as DBconn:
-            df.to_sql(config.database.agera5_table_name, DBconn, if_exists="append", index=False)
-            logger.info(f"Written AgERA5 data for {descriptor} to database.")
+            ins = tbl.insert()
+            for chunk in chunker(recs, config.database.chunk_size):
+                DBconn.execute(ins, chunk)
+                nrecs_written += len(chunk)
+                msg = f"Written {nrecs_written} from total {len(recs)} records to database."
+                logger.info(msg)
+        msg = f"Written AgERA5 data for {descriptor} to database in {time.time() - t1} seconds."
+        logger.info(msg)
     except sa.exc.IntegrityError as e:
         logger.error(f"Failed inserting AgERA5 data for {descriptor}: duplicate rows!")
 
 
 def df_to_csv(df, descriptor):
     """Write dataframe to a compressed CSV file
```

### Comparing `agera5tools-2.0.4/agera5tools/check.py` & `agera5tools-2.0.5/agera5tools/check.py`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/cmd.py` & `agera5tools-2.0.5/agera5tools/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,15 +161,15 @@
 @click.command("mirror")
 @click.option("-c", "--to_csv", is_flag=True,
               help="Write AgERA5 data to compressed CSV files.")
 def cmd_mirror(to_csv=False):
     """Incrementally updates the AgERA5 database by daily downloads from the CDS.
     """
     days, days_failed = mirror(to_csv)
-    days_done = days.difference((days_failed))
+    days_done = days.difference(days_failed)
     if not days:
         click.echo("Found no days to update the AgERA5 database for.")
     else:
 
         msg = "Mirror found the following:\n" \
               f" - Days found for mirroring: {day_fmt(days)}\n" \
               f" - Days successfully updated: {day_fmt(days_done)}\n"
```

### Comparing `agera5tools-2.0.4/agera5tools/db_data_provider.py` & `agera5tools-2.0.5/agera5tools/db_data_provider.py`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/dump_clip.py` & `agera5tools-2.0.5/agera5tools/dump_clip.py`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/dump_grid.py` & `agera5tools-2.0.5/agera5tools/dump_grid.py`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/extract_point.py` & `agera5tools-2.0.5/agera5tools/extract_point.py`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/grid_elevation_landfraction.nc` & `agera5tools-2.0.5/agera5tools/grid_elevation_landfraction.nc`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/help.html` & `agera5tools-2.0.5/agera5tools/help.html`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/help.md` & `agera5tools-2.0.5/agera5tools/help.md`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/init.py` & `agera5tools-2.0.5/agera5tools/init.py`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/mirror.py` & `agera5tools-2.0.5/agera5tools/mirror.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,14 +101,18 @@
     procedure should be run daily to update the local database with the remote AgERA5 data at
     the CDS.
 
     :param to_csv: Flag indicating if a compressed CSV file should be written.
     """
     logger = logging.getLogger(__name__)
     days = find_days_to_update()
+    if days:
+        logger.info(f"Found following days for updating AgERA5: {days}")
+    else:
+        logger.info(f"Found no days for updating AgERA5")
     days_failed = set()
     for day in sorted(days):
         logger.info(f"Starting AgERA5 download for {day}")
         to_download = []
         for varname in selected_variables:
             to_download.append((varname, day))
```

### Comparing `agera5tools-2.0.4/agera5tools/server.py` & `agera5tools-2.0.5/agera5tools/server.py`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools/util.py` & `agera5tools-2.0.5/agera5tools/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -310,8 +310,20 @@
     for d in days:
         s += f"{d.strftime('%Y-%m-%d')}, "
     if s:
         s = s[:-2]
     else:
         s = "N/A"
 
-    return s
+    return s
+
+
+def chunker(seq, size):
+    """Returns a generator that divides seq in chunks of given size.
+
+    The last chunk can have less than size entities.
+
+    :param seq: The sequence to be chunked
+    :param size: The chunk size, should be > 0
+    :return: a generator that chunks the sequence
+    """
+    return (seq[pos:pos + size] for pos in range(0, len(seq), size))
```

### Comparing `agera5tools-2.0.4/agera5tools/wdp.py` & `agera5tools-2.0.5/agera5tools/wdp.py`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/agera5tools.egg-info/PKG-INFO` & `agera5tools-2.0.5/agera5tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agera5tools
-Version: 2.0.4
+Version: 2.0.5
 Summary: AgERA5 is a tool for handling AgERA5 data from the Copernicus Climate Data Store.
 Author-email: Allard de Wit <allard.dewit@wur.nl>
 Project-URL: Homepage, https://github.com/ajwdewit/agera5tools
 Project-URL: documentation, https://agera5tools.readthedocs.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `agera5tools-2.0.4/agera5tools.egg-info/SOURCES.txt` & `agera5tools-2.0.5/agera5tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `agera5tools-2.0.4/pyproject.toml` & `agera5tools-2.0.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "agera5tools"
-version = "2.0.4"
+version = "2.0.5"
 authors = [
   { name="Allard de Wit", email="allard.dewit@wur.nl" },
 ]
 description = "AgERA5 is a tool for handling AgERA5 data from the Copernicus Climate Data Store."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

