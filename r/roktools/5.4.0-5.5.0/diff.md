# Comparing `tmp/roktools-5.4.0-py2.py3-none-any.whl.zip` & `tmp/roktools-5.5.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 20472 bytes, number of entries: 17
--rw-r--r--  2.0 unx        0 b- defN 23-May-29 14:15 roktools/__init__.py
+Zip file size: 20872 bytes, number of entries: 17
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 14:25 roktools/__init__.py
 -rw-r--r--  2.0 unx     4641 b- defN 23-May-29 14:14 roktools/cl.py
 -rw-r--r--  2.0 unx      400 b- defN 23-May-29 14:14 roktools/file.py
 -rw-r--r--  2.0 unx    33542 b- defN 23-May-29 14:14 roktools/geodetic.py
 -rw-r--r--  2.0 unx     1479 b- defN 23-May-29 14:14 roktools/logger.py
 -rw-r--r--  2.0 unx     3613 b- defN 23-May-29 14:14 roktools/rinex.py
 -rw-r--r--  2.0 unx      861 b- defN 23-May-29 14:14 roktools/stats.py
 -rw-r--r--  2.0 unx     1580 b- defN 23-May-29 14:14 roktools/tensorial.py
--rw-r--r--  2.0 unx     7182 b- defN 23-May-29 14:14 roktools/time.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-29 14:15 roktools/gnss/__init__.py
+-rw-r--r--  2.0 unx     9044 b- defN 23-Jun-01 14:23 roktools/time.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-01 14:25 roktools/gnss/__init__.py
 -rw-r--r--  2.0 unx     1722 b- defN 23-May-29 14:14 roktools/gnss/types.py
--rw-rw-rw-  2.0 unx     1067 b- defN 23-May-29 14:15 roktools-5.4.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     2604 b- defN 23-May-29 14:15 roktools-5.4.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-29 14:15 roktools-5.4.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      127 b- defN 23-May-29 14:15 roktools-5.4.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 23-May-29 14:15 roktools-5.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1314 b- defN 23-May-29 14:15 roktools-5.4.0.dist-info/RECORD
-17 files, 60251 bytes uncompressed, 18336 bytes compressed:  69.6%
+-rw-rw-rw-  2.0 unx     1067 b- defN 23-Jun-01 14:25 roktools-5.5.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2604 b- defN 23-Jun-01 14:25 roktools-5.5.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Jun-01 14:25 roktools-5.5.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      127 b- defN 23-Jun-01 14:25 roktools-5.5.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 23-Jun-01 14:25 roktools-5.5.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1314 b- defN 23-Jun-01 14:25 roktools-5.5.0.dist-info/RECORD
+17 files, 62113 bytes uncompressed, 18736 bytes compressed:  69.8%
```

## zipnote {}

```diff
@@ -27,26 +27,26 @@
 
 Filename: roktools/gnss/__init__.py
 Comment: 
 
 Filename: roktools/gnss/types.py
 Comment: 
 
-Filename: roktools-5.4.0.dist-info/LICENSE
+Filename: roktools-5.5.0.dist-info/LICENSE
 Comment: 
 
-Filename: roktools-5.4.0.dist-info/METADATA
+Filename: roktools-5.5.0.dist-info/METADATA
 Comment: 
 
-Filename: roktools-5.4.0.dist-info/WHEEL
+Filename: roktools-5.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: roktools-5.4.0.dist-info/entry_points.txt
+Filename: roktools-5.5.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: roktools-5.4.0.dist-info/top_level.txt
+Filename: roktools-5.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: roktools-5.4.0.dist-info/RECORD
+Filename: roktools-5.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## roktools/time.py

```diff
@@ -1,11 +1,13 @@
 from collections import namedtuple
 import datetime
 import math
 import enum
+from typing import List, Tuple
+import numpy as np
 WeekTow = namedtuple('WeekTow', 'week tow day_of_week')
 
 
 class TimeScale(enum.Enum):
     GPS = enum.auto()
     UTC = enum.auto()
 
@@ -201,8 +203,52 @@
         
         >>> interval = 0.01
         >>> round_to_interval(dt, interval)
         datetime.datetime(2023, 4, 20, 10, 48, 52, 790000)
     """
     timestamp = epoch.timestamp()
     rounded_timestamp = round(timestamp / interval) * interval
-    return datetime.datetime.fromtimestamp(rounded_timestamp)
+    return datetime.datetime.fromtimestamp(rounded_timestamp)
+
+
+def get_interval(epochs: List[datetime.datetime], target_intervals: Tuple[float] = (2.0, 1.0, 0.5, 0.1, 0.05, 0.01)) -> float:
+        """
+        Finds the closest possible interval from a predefined set of intervals to the computed inteval
+        from the pvt.
+
+        Args:
+            epochs: List of datetimes 
+            interval: The target intervals for which the closest possible interval is to be found.
+
+        Returns:
+            The closest possible interval from the predefined set.
+
+        >>> epochs = [datetime.datetime(2023, 6, 1, 12, 0, 0), datetime.datetime(2023, 6, 1, 12, 0, 2), datetime.datetime(2023, 6, 1, 12, 0, 3)]
+        >>> get_interval(epochs)
+        2.0
+
+        >>> epochs = [datetime.datetime(2023, 6, 1, 12, 0, 0), datetime.datetime(2023, 6, 1, 12, 0, 1), datetime.datetime(2023, 6, 1, 12, 0, 2)]
+        >>> get_interval(epochs)
+        1.0
+
+        >>> epochs = [datetime.datetime(2023, 6, 1, 12, 0, 0), datetime.datetime(2023, 6, 1, 12, 0, 0, 500000), datetime.datetime(2023, 6, 1, 12, 0, 1)]
+        >>> get_interval(epochs)
+        0.5
+
+        >>> epochs = [datetime.datetime(2023, 6, 1, 12, 0, 0), datetime.datetime(2023, 6, 1, 12, 0, 0, 100000), datetime.datetime(2023, 6, 1, 12, 0, 0, 200000)]
+        >>> get_interval(epochs)
+        0.1
+
+        >>> epochs = [datetime.datetime(2023, 6, 1, 12, 0, 0), datetime.datetime(2023, 6, 1, 12, 0, 0, 10000), datetime.datetime(2023, 6, 1, 12, 0, 0, 11000)]
+        >>> get_interval(epochs)
+        0.01
+
+        """
+        interval = np.median(np.ediff1d(epochs))
+        differences = [abs(interval.total_seconds() - target_interval) for target_interval in target_intervals]
+        return target_intervals[differences.index(min(differences))]
+
+
+
+if __name__ == "__main__":
+    import doctest
+    doctest.testmod()
```

## Comparing `roktools-5.4.0.dist-info/LICENSE` & `roktools-5.5.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `roktools-5.4.0.dist-info/METADATA` & `roktools-5.5.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roktools
-Version: 5.4.0
+Version: 5.5.0
 Summary: Set of tools used in internal Rokubun projects
 Home-page: https://www.rokubun.cat
 Author: Àlex López, Miquel García
 Author-email: alex.lopez@rokubun.cat, miquel.garcia@rokubun.cat
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

## Comparing `roktools-5.4.0.dist-info/RECORD` & `roktools-5.5.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 roktools/cl.py,sha256=LuRhDicv8eJAxvI7gbnG7RnOiRmEtyuUKg-nNcJlL1U,4641
 roktools/file.py,sha256=hJuPUBGz7MC600sfvOgwa2Md4uSHr10iChrW36sAeRQ,400
 roktools/geodetic.py,sha256=dxSoPxxooEyeKyEQqGfcb1WYmH9-Hl-kREtQu9kHpE4,33542
 roktools/logger.py,sha256=4kvcTWXPoiG-MlyP6B330l4Fu7MfCuDjuIlIiLA8f1Y,1479
 roktools/rinex.py,sha256=74IU4Nw-KKiAW1mTJd3UZYPH83oFQHppsfBejE8RH_Q,3613
 roktools/stats.py,sha256=I-XJdwktJIZgO7BIaEZYyGXQOpWBRLQCMStzRfmLvJk,861
 roktools/tensorial.py,sha256=RZ8-9Z926mQigYX9S0tjAa068jUMu5JkBElXLSLbYDY,1580
-roktools/time.py,sha256=1e4Ll0uAI7iNViWo5sOwmDdUZAeMa3GczvwAOMTT3Ww,7182
+roktools/time.py,sha256=I_LGNDy-xsVkj0E2C8elLk_vB9X9c3uyTq-MMnwWtUI,9044
 roktools/gnss/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 roktools/gnss/types.py,sha256=6g-Hp2HcGGwbhP-tlGoZlah0sJkcMQ3y7e-j9NKAa3I,1722
-roktools-5.4.0.dist-info/LICENSE,sha256=Wwany6RAAZ9vVHjFLA9KBJ0HE77d52s2NOUA1CPAEug,1067
-roktools-5.4.0.dist-info/METADATA,sha256=t29KvktTI7vOCfLdPxQ0lstg0iKQM189oRmM1Ys9gfw,2604
-roktools-5.4.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
-roktools-5.4.0.dist-info/entry_points.txt,sha256=tqrJvPDvOGCSWlRebEVLccLeFL5t-VHWC2aIoBNaZLA,127
-roktools-5.4.0.dist-info/top_level.txt,sha256=0RQjCH-RrFWM5YvdqifHlQ9EqtA2tdgtUb7tVuWzFDE,9
-roktools-5.4.0.dist-info/RECORD,,
+roktools-5.5.0.dist-info/LICENSE,sha256=Wwany6RAAZ9vVHjFLA9KBJ0HE77d52s2NOUA1CPAEug,1067
+roktools-5.5.0.dist-info/METADATA,sha256=XwRA8HHjK1P87XNhpEVIkz5ViOe8kfcjYfJO7nm0_Yw,2604
+roktools-5.5.0.dist-info/WHEEL,sha256=a-zpFRIJzOq5QfuhBzbhiA1eHTzNCJn8OdRvhdNX0Rk,110
+roktools-5.5.0.dist-info/entry_points.txt,sha256=tqrJvPDvOGCSWlRebEVLccLeFL5t-VHWC2aIoBNaZLA,127
+roktools-5.5.0.dist-info/top_level.txt,sha256=0RQjCH-RrFWM5YvdqifHlQ9EqtA2tdgtUb7tVuWzFDE,9
+roktools-5.5.0.dist-info/RECORD,,
```

