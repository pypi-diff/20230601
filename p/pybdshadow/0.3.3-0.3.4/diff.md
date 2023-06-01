# Comparing `tmp/pybdshadow-0.3.3.tar.gz` & `tmp/pybdshadow-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybdshadow-0.3.3.tar", last modified: Sun May  8 02:01:12 2022, max compression
+gzip compressed data, was "pybdshadow-0.3.4.tar", last modified: Thu Jun  1 02:05:30 2023, max compression
```

## Comparing `pybdshadow-0.3.3.tar` & `pybdshadow-0.3.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 02:01:12.893692 pybdshadow-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     7694 2022-05-08 02:01:12.893692 pybdshadow-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6847 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 02:01:12.893692 pybdshadow-0.3.3/pybdshadow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7694 2022-05-08 02:01:12.000000 pybdshadow-0.3.3/pybdshadow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-05-08 02:01:12.000000 pybdshadow-0.3.3/pybdshadow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-08 02:01:12.000000 pybdshadow-0.3.3/pybdshadow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-05-08 02:01:12.000000 pybdshadow-0.3.3/pybdshadow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-05-08 02:01:12.000000 pybdshadow-0.3.3/pybdshadow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-08 02:01:12.893692 pybdshadow-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 02:01:12.893692 pybdshadow-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-08 02:01:12.893692 pybdshadow-0.3.3/src/pybdshadow/
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/src/pybdshadow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8846 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/src/pybdshadow/analysis.py
--rw-r--r--   0 runner    (1001) docker     (121)     4811 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/src/pybdshadow/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (121)    12899 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/src/pybdshadow/pybdshadow.py
--rw-r--r--   0 runner    (1001) docker     (121)     2835 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/src/pybdshadow/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11005 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/src/pybdshadow/visiblearea.py
--rw-r--r--   0 runner    (1001) docker     (121)    19361 2022-05-08 02:00:57.000000 pybdshadow-0.3.3/src/pybdshadow/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:05:30.491593 pybdshadow-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-06-01 02:05:30.491593 pybdshadow-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6800 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:05:30.487594 pybdshadow-0.3.4/pybdshadow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7627 2023-06-01 02:05:30.000000 pybdshadow-0.3.4/pybdshadow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-01 02:05:30.000000 pybdshadow-0.3.4/pybdshadow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 02:05:30.000000 pybdshadow-0.3.4/pybdshadow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-06-01 02:05:30.000000 pybdshadow-0.3.4/pybdshadow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-01 02:05:30.000000 pybdshadow-0.3.4/pybdshadow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 02:05:30.491593 pybdshadow-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:05:30.487594 pybdshadow-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 02:05:30.487594 pybdshadow-0.3.4/src/pybdshadow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/src/pybdshadow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9460 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/src/pybdshadow/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/src/pybdshadow/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14016 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/src/pybdshadow/pybdshadow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/src/pybdshadow/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/src/pybdshadow/visiblearea.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19403 2023-06-01 02:05:19.000000 pybdshadow-0.3.4/src/pybdshadow/visualization.py
```

### Comparing `pybdshadow-0.3.3/LICENSE` & `pybdshadow-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pybdshadow-0.3.3/PKG-INFO` & `pybdshadow-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pybdshadow
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python package to generate building shadow geometry
 Home-page: https://github.com/ni1o1/pybdshadow
 Author: Qing Yu
 Author-email: qingyu0815@foxmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/ni1o1/pybdshadow/issues
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -127,19 +126,19 @@
 
 ### Shadow coverage analysis
 
 `pybdshadow` provides the functionality to analysis sunshine time on the roof and on the ground.
 
 Result of shadow coverage on the roof:
 
-![1651645524782.png](image/README/1651645524782.png)
+![1651645524782.png](image/README/1651645524782.png)![1651975815798.png](image/README/1651975815798.png)
 
 Result of sunshine time on the ground:
 
-![1651645530892.png](image/README/1651645530892.png)
+![1651645530892.png](image/README/1651645530892.png)![1651975824187.png](image/README/1651975824187.png)
 
 ## Dependency
 
 `pybdshadow` depends on the following packages
 
 * `numpy`
 * `pandas`
@@ -147,16 +146,14 @@
 * `rtree`
 * `geopandas`
 * `matplotlib`
 * [`suncalc`](https://github.com/kylebarron/suncalc-py)
 * [`keplergl`](https://kepler.gl/)
 * [`TransBigData`](https://github.com/ni1o1/transbigdata)
 
-## Citation information [![status](https://joss.theoj.org/papers/9d4c2bf5285cffed1be3065ad7da94dd/status.svg)](https://joss.theoj.org/papers/9d4c2bf5285cffed1be3065ad7da94dd)
+## Citation information
 
 Citation information can be found at [CITATION.cff](https://github.com/ni1o1/pybdshadow/blob/main/CITATION.cff).
 
 ## Contributing to pybdshadow [![GitHub contributors](https://img.shields.io/github/contributors/ni1o1/pybdshadow.svg)](https://github.com/ni1o1/pybdshadow/graphs/contributors) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ni1o1/pybdshadow)
 
 All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome. A detailed overview on how to contribute can be found in the [contributing guide](https://github.com/ni1o1/pybdshadow/blob/master/CONTRIBUTING.md) on GitHub.
-
-
```

### Comparing `pybdshadow-0.3.3/README.md` & `pybdshadow-0.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -104,19 +104,19 @@
 
 ### Shadow coverage analysis
 
 `pybdshadow` provides the functionality to analysis sunshine time on the roof and on the ground.
 
 Result of shadow coverage on the roof:
 
-![1651645524782.png](image/README/1651645524782.png)
+![1651645524782.png](image/README/1651645524782.png)![1651975815798.png](image/README/1651975815798.png)
 
 Result of sunshine time on the ground:
 
-![1651645530892.png](image/README/1651645530892.png)
+![1651645530892.png](image/README/1651645530892.png)![1651975824187.png](image/README/1651975824187.png)
 
 ## Dependency
 
 `pybdshadow` depends on the following packages
 
 * `numpy`
 * `pandas`
@@ -124,14 +124,14 @@
 * `rtree`
 * `geopandas`
 * `matplotlib`
 * [`suncalc`](https://github.com/kylebarron/suncalc-py)
 * [`keplergl`](https://kepler.gl/)
 * [`TransBigData`](https://github.com/ni1o1/transbigdata)
 
-## Citation information [![status](https://joss.theoj.org/papers/9d4c2bf5285cffed1be3065ad7da94dd/status.svg)](https://joss.theoj.org/papers/9d4c2bf5285cffed1be3065ad7da94dd)
+## Citation information
 
 Citation information can be found at [CITATION.cff](https://github.com/ni1o1/pybdshadow/blob/main/CITATION.cff).
 
 ## Contributing to pybdshadow [![GitHub contributors](https://img.shields.io/github/contributors/ni1o1/pybdshadow.svg)](https://github.com/ni1o1/pybdshadow/graphs/contributors) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ni1o1/pybdshadow)
 
 All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome. A detailed overview on how to contribute can be found in the [contributing guide](https://github.com/ni1o1/pybdshadow/blob/master/CONTRIBUTING.md) on GitHub.
```

### Comparing `pybdshadow-0.3.3/pybdshadow.egg-info/PKG-INFO` & `pybdshadow-0.3.4/pybdshadow.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pybdshadow
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python package to generate building shadow geometry
 Home-page: https://github.com/ni1o1/pybdshadow
 Author: Qing Yu
 Author-email: qingyu0815@foxmail.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/ni1o1/pybdshadow/issues
-Platform: UNKNOWN
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Text Processing :: Indexing
 Classifier: Topic :: Utilities
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
@@ -127,19 +126,19 @@
 
 ### Shadow coverage analysis
 
 `pybdshadow` provides the functionality to analysis sunshine time on the roof and on the ground.
 
 Result of shadow coverage on the roof:
 
-![1651645524782.png](image/README/1651645524782.png)
+![1651645524782.png](image/README/1651645524782.png)![1651975815798.png](image/README/1651975815798.png)
 
 Result of sunshine time on the ground:
 
-![1651645530892.png](image/README/1651645530892.png)
+![1651645530892.png](image/README/1651645530892.png)![1651975824187.png](image/README/1651975824187.png)
 
 ## Dependency
 
 `pybdshadow` depends on the following packages
 
 * `numpy`
 * `pandas`
@@ -147,16 +146,14 @@
 * `rtree`
 * `geopandas`
 * `matplotlib`
 * [`suncalc`](https://github.com/kylebarron/suncalc-py)
 * [`keplergl`](https://kepler.gl/)
 * [`TransBigData`](https://github.com/ni1o1/transbigdata)
 
-## Citation information [![status](https://joss.theoj.org/papers/9d4c2bf5285cffed1be3065ad7da94dd/status.svg)](https://joss.theoj.org/papers/9d4c2bf5285cffed1be3065ad7da94dd)
+## Citation information
 
 Citation information can be found at [CITATION.cff](https://github.com/ni1o1/pybdshadow/blob/main/CITATION.cff).
 
 ## Contributing to pybdshadow [![GitHub contributors](https://img.shields.io/github/contributors/ni1o1/pybdshadow.svg)](https://github.com/ni1o1/pybdshadow/graphs/contributors) ![GitHub commit activity](https://img.shields.io/github/commit-activity/m/ni1o1/pybdshadow)
 
 All contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome. A detailed overview on how to contribute can be found in the [contributing guide](https://github.com/ni1o1/pybdshadow/blob/master/CONTRIBUTING.md) on GitHub.
-
-
```

### Comparing `pybdshadow-0.3.3/setup.py` & `pybdshadow-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pybdshadow",
-    version="0.3.3",
+    version="0.3.4",
     author="Qing Yu",
     author_email="qingyu0815@foxmail.com",
     description="Python package to generate building shadow geometry",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="BSD",
     url="https://github.com/ni1o1/pybdshadow",
```

### Comparing `pybdshadow-0.3.3/src/pybdshadow/__init__.py` & `pybdshadow-0.3.4/src/pybdshadow/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 __author__ = 'Qing Yu <qingyu0815@foxmail.com>'
 
 # module level doc-string
 __doc__ = """
 `pybdshadow` - Python package to generate building shadow geometry.
 """
 from .pybdshadow import *
@@ -49,18 +49,20 @@
 )
 from .visualization import (
     show_bdshadow,
 )
 from .analysis import (
     cal_sunshine,
     cal_sunshadows,
-    cal_shadowcoverage
+    cal_shadowcoverage,
+    get_timetable
 )
 
 __all__ = ['bdshadow_sunlight',
            'bdshadow_pointlight',
            'bd_preprocess',
            'show_bdshadow',
            'cal_sunshine',
            'cal_sunshadows',
            'cal_shadowcoverage',
+           'get_timetable'
            ]
```

### Comparing `pybdshadow-0.3.3/src/pybdshadow/analysis.py` & `pybdshadow-0.3.4/src/pybdshadow/analysis.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,228 +6,233 @@
 from .pybdshadow import (
     bdshadow_sunlight,
 )
 from .preprocess import bd_preprocess
 
 
 def get_timetable(lon, lat, dates=['2022-01-01'], precision=3600, padding=1800):
-    # generate timetable
+    # generate timetable with given interval
     def get_timeSeries(day, lon, lat, precision=3600, padding=1800):
         date = pd.to_datetime(day+' 12:45:33.959797119')
         times = get_times(date, lon, lat)
         date_sunrise = times['sunrise']
         data_sunset = times['sunset']
         timestamp_sunrise = pd.Series(date_sunrise).astype('int')
         timestamp_sunset = pd.Series(data_sunset).astype('int')
         times = pd.to_datetime(pd.Series(range(
             timestamp_sunrise.iloc[0]+padding*1000000000,
             timestamp_sunset.iloc[0]-padding*1000000000,
             precision*1000000000)))
         return times
     dates = pd.DataFrame(pd.concat(
-        [get_timeSeries(date, lon, lat, precision,padding) for date in dates]), columns=['datetime'])
+        [get_timeSeries(date, lon, lat, precision, padding) for date in dates]), columns=['datetime'])
     dates['date'] = dates['datetime'].apply(lambda r: str(r)[:19])
     return dates
 
-def cal_sunshine(buildings, day='2022-01-01', roof=False,grids =  gpd.GeoDataFrame(), accuracy=1, precision=3600, padding=0):
+
+def cal_sunshine(buildings, day='2022-01-01', roof=False, grids=gpd.GeoDataFrame(), accuracy=1, precision=3600, padding=1800):
     '''
     Calculate the sunshine time in given date.
 
-    **Parameters**
-
+    Parameters
+    --------------------
     buildings : GeoDataFrame
         Buildings. coordinate system should be WGS84
     day : str
         the day to calculate the sunshine
     roof : bool
         whether to calculate roof shadow.
     grids : GeoDataFrame
         grids generated by TransBigData in study area
     precision : number
         time precision(s)
     padding : number
         padding time before and after sunrise and sunset
     accuracy : number
         size of grids. Produce vector polygons if set as `vector` 
-        
-    **Return**
 
+    Return
+    ----------
     grids : GeoDataFrame
         grids generated by TransBigData in study area, each grids have a `time` column store the sunshine time
 
     '''
-    # 计算白天时间
+    # calculate day time duration
     lon, lat = buildings['geometry'].iloc[0].bounds[:2]
     date = pd.to_datetime(day+' 12:45:33.959797119')
     times = get_times(date, lon, lat)
     date_sunrise = times['sunrise']
     data_sunset = times['sunset']
     timestamp_sunrise = pd.Series(date_sunrise).astype('int')
     timestamp_sunset = pd.Series(data_sunset).astype('int')
     sunlighthour = (
         timestamp_sunset.iloc[0]-timestamp_sunrise.iloc[0])/(1000000000*3600)
 
-    # Generate shadow every 1800 s
-    shadows = cal_sunshadows(buildings, dates=[day], precision=precision, padding=padding)
+    # Generate shadow every time interval
+    shadows = cal_sunshadows(
+        buildings, dates=[day], precision=precision, padding=padding)
     if accuracy == 'vector':
         if roof:
-            shadows = shadows[shadows['type'] == 'roof'] 
+            shadows = shadows[shadows['type'] == 'roof']
             shadows = bd_preprocess(shadows)
-            shadows = shadows.groupby(['date','type'])['geometry'].apply(
-                        lambda df: MultiPolygon(list(df)).buffer(0)).reset_index()
+            shadows = shadows.groupby(['date', 'type'])['geometry'].apply(
+                lambda df: MultiPolygon(list(df)).buffer(0)).reset_index()
             shadows = bd_preprocess(shadows)
             shadows = count_overlapping_features(shadows)
         else:
-            shadows = shadows[shadows['type'] == 'ground'] 
+            shadows = shadows[shadows['type'] == 'ground']
             shadows = bd_preprocess(shadows)
-            shadows = shadows.groupby(['date','type'])['geometry'].apply(
-                        lambda df: MultiPolygon(list(df)).buffer(0)).reset_index()
+            shadows = shadows.groupby(['date', 'type'])['geometry'].apply(
+                lambda df: MultiPolygon(list(df)).buffer(0)).reset_index()
             shadows = bd_preprocess(shadows)
             shadows = count_overlapping_features(shadows)
 
         shadows['time'] = shadows['count']*precision
         shadows['Hour'] = sunlighthour-shadows['time']/3600
-        shadows.loc[shadows['Hour']<=0,'Hour']=0
+        shadows.loc[shadows['Hour'] <= 0, 'Hour'] = 0
         return shadows
     else:
         # Grid analysis of shadow cover duration(ground).
         grids = cal_shadowcoverage(
-            shadows, buildings, grids = grids,roof=roof, precision=precision, accuracy=accuracy)
+            shadows, buildings, grids=grids, roof=roof, precision=precision, accuracy=accuracy)
 
         grids['Hour'] = sunlighthour-grids['time']/3600
         return grids
 
-    
-
 
-def cal_sunshadows(buildings, cityname='somecity', dates=['2022-01-01'], precision=3600, padding=0,
+def cal_sunshadows(buildings, cityname='somecity', dates=['2022-01-01'], precision=3600, padding=1800,
                    roof=True, include_building=True, save_shadows=False, printlog=False):
     '''
     Calculate the sunlight shadow in different date with given time precision.
 
-    **Parameters**
-
+    Parameters
+    --------------------
     buildings : GeoDataFrame
         Buildings. coordinate system should be WGS84
     cityname : string
         Cityname. If save_shadows, this function will create `result/cityname` folder to save the shadows
     dates : list
-        list of dates
+        List of dates
     precision : number
-        time precision(s)
+        Time precision(s)
     padding : number
-        padding time before and after sunrise and sunset
+        Padding time (second) before and after sunrise and sunset. Should be over 1800s to avoid sun altitude under 0
     roof : bool
         whether to calculate roof shadow.
     include_building : bool
         whether the shadow include building outline
     save_shadows : bool
         whether to save calculated shadows
     printlog : bool
         whether to print log
 
-    **Return**
-
+    Return
+    ----------
     allshadow : GeoDataFrame
         All building shadows calculated
     '''
-    # 获取城市位置
+    if (padding < 1800):
+        raise ValueError(
+            'Padding time should be over 1800s to avoid sun altitude under 0')  # pragma: no cover
+    # obtain city location
     lon, lat = buildings['geometry'].iloc[0].bounds[:2]
     timetable = get_timetable(lon, lat, dates, precision, padding)
     import os
     if save_shadows:
-        if not os.path.exists('result'):
-            os.mkdir('result')
-        if not os.path.exists('result/'+cityname):
-            os.mkdir('result/'+cityname)
+        if not os.path.exists('result'):             # pragma: no cover
+            os.mkdir('result')                       # pragma: no cover
+        if not os.path.exists('result/'+cityname):   # pragma: no cover
+            os.mkdir('result/'+cityname)             # pragma: no cover
     allshadow = []
     for i in range(len(timetable)):
         date = timetable['datetime'].iloc[i]
         name = timetable['date'].iloc[i]
         if not os.path.exists('result/'+cityname+'/roof_'+name+'.json'):
             if printlog:
-                print('Calculating', cityname, ':', name)
+                print('Calculating', cityname, ':', name)    # pragma: no cover
             # Calculate shadows
             shadows = bdshadow_sunlight(
                 buildings, date, roof=roof, include_building=include_building)
             shadows['date'] = date
             roof_shaodws = shadows[shadows['type'] == 'roof']
             ground_shaodws = shadows[shadows['type'] == 'ground']
 
             if save_shadows:
-                if len(roof_shaodws) > 0:
-                    roof_shaodws.to_file(
-                        'result/'+cityname+'/roof_'+name+'.json', driver='GeoJSON')
-                if len(ground_shaodws) > 0:
-                    ground_shaodws.to_file(
-                        'result/'+cityname+'/ground_'+name+'.json', driver='GeoJSON')
+                if len(roof_shaodws) > 0:    # pragma: no cover
+                    roof_shaodws.to_file(    # pragma: no cover
+                        'result/'+cityname+'/roof_'+name+'.json', driver='GeoJSON')  # pragma: no cover
+                if len(ground_shaodws) > 0:  # pragma: no cover
+                    ground_shaodws.to_file(  # pragma: no cover
+                        'result/'+cityname+'/ground_'+name+'.json', driver='GeoJSON')  # pragma: no cover
             allshadow.append(shadows)
     allshadow = pd.concat(allshadow)
     return allshadow
 
 
-def cal_shadowcoverage(shadows_input, buildings, grids = gpd.GeoDataFrame(),roof=True, precision=3600, accuracy=1):
+def cal_shadowcoverage(shadows_input, buildings, grids=gpd.GeoDataFrame(), roof=True, precision=3600, accuracy=1):
     '''
     Calculate the sunlight shadow coverage time for given area.
 
-    **Parameters**
-
+    Parameters
+    --------------------
     shadows_input : GeoDataFrame
         All building shadows calculated
     buildings : GeoDataFrame
         Buildings. coordinate system should be WGS84
     grids : GeoDataFrame
         grids generated by TransBigData in study area
     roof : bool
         If true roof shadow, false then ground shadow
     precision : number
         time precision(s), which is for calculation of coverage time
     accuracy : number
         size of grids.
 
-    **Return**
-
+    Return
+    --------------------
     grids : GeoDataFrame
         grids generated by TransBigData in study area, each grids have a `time` column store the shadow coverage time
 
     '''
     shadows = bd_preprocess(shadows_input)
 
-    # 研究区域
+    # study area
     bounds = buildings.unary_union.bounds
-    if len(grids)==0:
+    if len(grids) == 0:
         grids, params = tbd.area_to_grid(bounds, accuracy)
-    
+
     if roof:
         ground_shadows = shadows[shadows['type'] == 'roof'].groupby(['date'])['geometry'].apply(
             lambda df: MultiPolygon(list(df)).buffer(0)).reset_index()
 
         buildings.crs = None
         grids = gpd.sjoin(grids, buildings)
     else:
         ground_shadows = shadows[shadows['type'] == 'ground'].groupby(['date'])['geometry'].apply(
             lambda df: MultiPolygon(list(df)).buffer(0)).reset_index()
 
         buildings.crs = None
         grids = gpd.sjoin(grids, buildings, how='left')
         grids = grids[grids['index_right'].isnull()]
 
-    gridcount = gpd.sjoin(grids[['LONCOL', 'LATCOL', 'geometry']], ground_shadows[['geometry','date']]).\
-        drop_duplicates(subset=['LONCOL', 'LATCOL','date']).groupby(['LONCOL', 'LATCOL'])['geometry'].\
-            count().rename('count').reset_index()
+    gridcount = gpd.sjoin(grids[['LONCOL', 'LATCOL', 'geometry']], ground_shadows[['geometry', 'date']]).\
+        drop_duplicates(subset=['LONCOL', 'LATCOL', 'date']).groupby(['LONCOL', 'LATCOL'])['geometry'].\
+        count().rename('count').reset_index()
     grids = pd.merge(grids, gridcount, how='left')
     grids['time'] = grids['count'].fillna(0)*precision
 
     return grids
 
+
 def count_overlapping_features(gdf):
     import shapely
     bounds = gdf.geometry.exterior.unary_union
     new_polys = list(shapely.ops.polygonize(bounds))
     new_gdf = gpd.GeoDataFrame(geometry=new_polys)
     new_gdf['id'] = range(len(new_gdf))
     new_gdf_centroid = new_gdf.copy()
     new_gdf_centroid['geometry'] = new_gdf.centroid
-    overlapcount = gpd.sjoin(new_gdf_centroid,gdf)
-    overlapcount = overlapcount.groupby(['id'])['index_right'].count().rename('count').reset_index()
-    out_gdf = pd.merge(new_gdf,overlapcount)
-    return out_gdf
+    overlapcount = gpd.sjoin(new_gdf_centroid, gdf)
+    overlapcount = overlapcount.groupby(
+        ['id'])['index_right'].count().rename('count').reset_index()
+    out_gdf = pd.merge(new_gdf, overlapcount)
+    return out_gdf
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pybdshadow-0.3.3/src/pybdshadow/preprocess.py` & `pybdshadow-0.3.4/src/pybdshadow/preprocess.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,24 +35,27 @@
 
 
 def bd_preprocess(buildings, height=''):
     '''
     Preprocess building data, so that we can perform shadow calculation.
     Remove empty polygons and convert multipolygons into polygons.
 
-    **Parameters**
+    Parameters
+    --------------
     buildings : GeoDataFrame
         Buildings.
     height : string
-        Column name of building height
+        Column name of building height(meter).
 
-    **Return**
+    Return
+    ----------
     allbds : GeoDataFrame
         Polygon buildings
     '''
+    buildings['geometry'] = buildings.buffer(0)
     buildings = buildings[buildings.is_valid].copy()
     if height!='':
         # 建筑高度筛选
         buildings[height] = pd.to_numeric(buildings[height], errors='coerce')
         buildings = buildings[buildings[height]>0].copy()
 
     polygon_buildings = buildings[buildings['geometry'].apply(
@@ -66,16 +69,20 @@
         singlebd['geometry'] = list(r['geometry'].geoms)
         for i in r.index:
             if i != 'geometry':
                 singlebd[i] = r[i]
         allbds.append(singlebd)
     allbds.append(polygon_buildings)
     allbds = pd.concat(allbds)
-    allbds['building_id'] = range(len(allbds))
-    allbds['geometry'] = allbds.buffer(0)
+    if len(allbds) > 0:
+        allbds = gpd.GeoDataFrame(allbds)
+        allbds['building_id'] = range(len(allbds))
+        allbds['geometry'] = allbds.buffer(0)
+    else:
+        allbds = gpd.GeoDataFrame()
     return allbds
 
 def gdf_difference(gdf_a,gdf_b,col = 'building_id'):
     '''
     difference gdf_b from gdf_a
     '''
     gdfa = gdf_a.copy()
```

### Comparing `pybdshadow-0.3.3/src/pybdshadow/pybdshadow.py` & `pybdshadow-0.3.4/src/pybdshadow/pybdshadow.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,76 +32,89 @@
 import pandas as pd
 import geopandas as gpd
 from suncalc import get_position
 from shapely.geometry import Polygon,LineString, MultiPolygon
 import math
 import numpy as np
 from .utils import (
-    lonlat_mercator_vector,
-    mercator_lonlat_vector
+    lonlat2aeqd,
+    aeqd2lonlat
 )
 from .preprocess import gdf_difference,gdf_intersect
 
 
 def calSunShadow_vector(shape, shapeHeight, sunPosition):
-    # 多维数据类型：numpy
-    # 输入的shape是一个矩阵（n*2*2) n个建筑物面，每个建筑有2个点，每个点有三个维度
-    # shapeHeight(n) 每一栋建筑的高度都是一样的
+    '''
+    Calculate the shadow of a building on the ground.
 
-    # 坐标系转换transform coordinate system
-    shape = lonlat_mercator_vector(shape)
-    # print(shape,np.shape(shape))
+    Parameters
+    ----------
+    shape : numpy.ndarray
+        The shape of the building. The shape of the array is (n,2,2), where n the number of walls, 2 is that each wall has two points, and the last dimension is for longitude and latitude.
+    shapeHeight : float
+        The height of the building.
+    sunPosition : dict
+        The position of the sun. The keys are 'azimuth' and 'altitude'.
+
+    Returns
+    -------
+    shadow : numpy.ndarray
+        The shadow of the building on the ground. shape = [n,5,2]
+    '''
+    # transform coordinate system
+    meanlon = shape[:,:,0].mean()
+    meanlat = shape[:,:,1].mean()
+    shape = lonlat2aeqd(shape)
 
     azimuth = sunPosition['azimuth']
     altitude = sunPosition['altitude']
 
     n = np.shape(shape)[0]
     distance = shapeHeight/math.tan(altitude)
 
-    # 计算投影位置偏移
-    lonDistance = distance*math.sin(azimuth)  # n个偏移量[n]
+    # calculate the offset of the projection position
+    lonDistance = distance*math.sin(azimuth) 
     lonDistance = lonDistance.reshape((n, 1))
     latDistance = distance*math.cos(azimuth)
     latDistance = latDistance.reshape((n, 1))
 
-    shadowShape = np.zeros((n, 5, 2))  # n个建筑物面，每个面都有5个点，每个点都有个维数
+    shadowShape = np.zeros((n, 5, 2)) # n buildings, each building has 5 points, each point has 2 dimensions
 
-    shadowShape[:, 0:2, :] += shape  # 前两个点不变
+    shadowShape[:, 0:2, :] += shape  
     shadowShape[:, 2:4, 0] = shape[:, :, 0] + lonDistance
     shadowShape[:, 2:4, 1] = shape[:, :, 1] + latDistance
 
     shadowShape[:, [2, 3], :] = shadowShape[:, [3, 2], :]
     shadowShape[:, 4, :] = shadowShape[:, 0, :]
 
-    shadowShape = mercator_lonlat_vector(shadowShape)
-    # print(shadowShape,np.shape(shadowShape))
+    shadowShape = aeqd2lonlat(shadowShape,meanlon,meanlat)
     return shadowShape
 
 
 def bdshadow_sunlight(buildings, date,  height='height', roof=False,include_building = True,ground=0):
     '''
     Calculate the sunlight shadow of the buildings.
 
-    **Parameters**
-
+    Parameters
+    ----------
     buildings : GeoDataFrame
         Buildings. coordinate system should be WGS84
     date : datetime
         Datetime
     height : string
-        Column name of building height
+        Column name of building height(meter).
     roof : bool
-        whether to calculate the roof shadows
+        Whether to calculate the roof shadows.
     include_building : bool
-        whether the shadow include building outline
+        Whether the shadow include building outline.
     ground : number
-        Height of the ground
-
-    **Return**
+        Height of the ground(meter).
 
+    Returns
+    ----------
     shadows : GeoDataFrame
         Building shadow
     '''
 
     building = buildings.copy()
 
     building[height] -= ground
@@ -110,14 +123,16 @@
     # calculate position
     lon1, lat1, lon2, lat2 = list(building.bounds.mean())
     lon = (lon1+lon2)/2
     lat = (lat1+lat2)/2
 
     # obtain sun position
     sunPosition = get_position(date, lon, lat)
+    if ( sunPosition['altitude']<0):
+        raise ValueError("Given time before sunrise or after sunset")   # pragma: no cover
     buildingshadow = building.copy()
 
     a = buildingshadow['geometry'].apply(lambda r: list(r.exterior.coords))
     buildingshadow['wall'] = a
     buildingshadow = buildingshadow.set_index(['building_id'])
     a = buildingshadow.apply(lambda x: pd.Series(x['wall']), axis=1).unstack()
     walls = a[- a.isnull()].reset_index().sort_values(
@@ -223,14 +238,31 @@
         shadows = pd.concat([roof_shadow, ground_shadow])
         shadows.crs = None
         shadows['geometry'] = shadows.buffer(0.000001).buffer(-0.000001)
         return shadows
 
 
 def calPointLightShadow_vector(shape, shapeHeight, pointLight):
+    '''
+    calculate shadow for a point light
+    
+    Parameters
+    ----------
+    shape : numpy.array
+        The shape of the building. The shape of the array is (n,2,2), where n the number of walls, 2 is that each wall has two points, and the last dimension is for longitude and latitude.
+    shapeHeight : numpy.array
+        height of building, shape = [n,1], n is the number of buildings
+    pointLight : dict
+        point light, pointLight = {'position':[lon,lat,height]}
+    
+    Returns
+    -------
+    shadowShape : numpy.array
+        shape of shadow, shape = [n,5,2]
+    '''
     # 多维数据类型：numpy
     # 输入的shape是一个矩阵（n*2*2) n个建筑物面，每个建筑有2个点，每个点有三个维度
     # shapeHeight(n) 每一栋建筑的高度都是一样的
     n = np.shape(shape)[0]
     pointLightPosition = pointLight['position']  # [lon,lat,height]
 
     # 高度比
@@ -260,29 +292,31 @@
                         pointheight,
                         merge=True,
                         height='height',
                         ground=0):
     '''
     Calculate the sunlight shadow of the buildings.
 
-    **Parameters**
+    Parameters
+    --------------------
     buildings : GeoDataFrame
         Buildings. coordinate system should be WGS84
     pointlon,pointlat,pointheight : float
-        Point light coordinates and height
+        Point light coordinates and height(meter).
     date : datetime
         Datetime
     merge : bool
-        whether to merge the wall shadows into the building shadows
+        Whether to merge the wall shadows into the building shadows
     height : string
-        Column name of building height
+        Column name of building height(meter).
     ground : number
         Height of the ground
-
-    **Return**
+    
+    Returns
+    ----------
     shadows : GeoDataFrame
         Building shadow
     '''
 
     building = buildings.copy()
 
     building[height] -= ground
```

### Comparing `pybdshadow-0.3.3/src/pybdshadow/visiblearea.py` & `pybdshadow-0.3.4/src/pybdshadow/visiblearea.py`

 * *Files identical despite different names*

### Comparing `pybdshadow-0.3.3/src/pybdshadow/visualization.py` & `pybdshadow-0.3.4/src/pybdshadow/visualization.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,29 +38,31 @@
                   ad=gpd.GeoDataFrame(),
                   ad_visualArea=gpd.GeoDataFrame(),
                   height='height',
                   zoom='auto'):
     '''
     Visualize the building and shadow with keplergl.
 
-    **Parameters**
+    Parameters
+    --------------------
     buildings : GeoDataFrame
         Buildings. coordinate system should be WGS84
     shadows : GeoDataFrame
         Building shadows. coordinate system should be WGS84
     ad : GeoDataFrame
         Advertisment. coordinate system should be WGS84
     ad_visualArea : GeoDataFrame
         Visualarea of Advertisment. coordinate system should be WGS84
     height : string
         Column name of building height
     zoom : number
         Zoom level of the map
 
-    **Return**
+    Return
+    --------------------
     vmap : keplergl.keplergl.KeplerGl
         Visualizations provided by keplergl
     '''
     displaybuilding = buildings.copy()
     displaybuildingshadow = shadows.copy()
     displayad = ad.copy()
     displayad_visualArea = ad_visualArea.copy()
```

