# Comparing `tmp/mrpyconvert-0.1.5.tar.gz` & `tmp/mrpyconvert-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrpyconvert-0.1.5.tar", max compression
+gzip compressed data, was "mrpyconvert-0.1.6.tar", max compression
```

## Comparing `mrpyconvert-0.1.5.tar` & `mrpyconvert-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2022-04-19 22:33:27.705840 mrpyconvert-0.1.5/LICENSE
--rw-r--r--   0        0        0       94 2023-03-23 20:24:49.074668 mrpyconvert-0.1.5/README.md
--rw-r--r--   0        0        0       46 2023-05-31 23:07:30.786223 mrpyconvert-0.1.5/mrpyconvert/__init__.py
--rw-r--r--   0        0        0     1798 2023-03-23 20:24:49.121983 mrpyconvert-0.1.5/mrpyconvert/dicom_sorter.py
--rw-r--r--   0        0        0    15813 2023-03-23 20:24:49.191366 mrpyconvert-0.1.5/mrpyconvert/mrpyconvert.py
--rw-r--r--   0        0        0      426 2023-05-31 23:17:35.955261 mrpyconvert-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 mrpyconvert-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-04-19 22:33:27.705840 mrpyconvert-0.1.6/LICENSE
+-rw-r--r--   0        0        0       94 2023-03-23 20:24:49.074668 mrpyconvert-0.1.6/README.md
+-rw-r--r--   0        0        0       46 2023-05-31 23:07:30.786223 mrpyconvert-0.1.6/mrpyconvert/__init__.py
+-rw-r--r--   0        0        0     1798 2023-03-23 20:24:49.121983 mrpyconvert-0.1.6/mrpyconvert/dicom_sorter.py
+-rw-r--r--   0        0        0    16227 2023-05-31 23:26:39.979382 mrpyconvert-0.1.6/mrpyconvert/mrpyconvert.py
+-rw-r--r--   0        0        0      426 2023-05-31 23:27:07.686911 mrpyconvert-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 mrpyconvert-0.1.6/PKG-INFO
```

### Comparing `mrpyconvert-0.1.5/LICENSE` & `mrpyconvert-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mrpyconvert-0.1.5/mrpyconvert/dicom_sorter.py` & `mrpyconvert-0.1.6/mrpyconvert/dicom_sorter.py`

 * *Files identical despite different names*

### Comparing `mrpyconvert-0.1.5/mrpyconvert/mrpyconvert.py` & `mrpyconvert-0.1.6/mrpyconvert/mrpyconvert.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,30 +89,34 @@
     def __init__(self, autosession=False):
         self.autosession = autosession
         self.series = []
         self.entities = []
 
     def add_dicoms(self, dicom_path, subject=None, session=None):
         series_paths = [pathlib.Path(root) for root, dirs, files in os.walk(dicom_path, followlinks=True) if not dirs]
-        found_series = [series for s in series_paths if (series := Series(s, subject, session)).has_dicoms]
+        # sadly I need to support python < 3.8, no walruses allowed
+        #found_series = [series for s in series_paths if (series := Series(s, subject, session)).has_dicoms]
+        found_series = [Series(s, subject, session) for s in series_paths if Series(s, subject, session).has_dicoms]
 
         if not found_series:
             print('No dicoms found')
             return
         else:
             self.series.extend(found_series)
 
 
     def inspect(self, dicom_path=None):
         if not dicom_path:
             all_series = self.series
         else:
             series_paths = [pathlib.Path(root) for root, dirs, files in os.walk(dicom_path, followlinks=True) if
                             not dirs]
-            all_series = [series for s in series_paths if (series := Series(s)).has_dicoms]
+            #all_series = [series for s in series_paths if (series := Series(s)).has_dicoms]
+            all_series = [Series(s) for s in series_paths if Series(s).has_dicoms]
+
 
         if not all_series:
             print(f'No dicoms found in {dicom_path}')
             return
 
         all_subjects = {x.subject for x in all_series}
         all_studies = {x.study_uid for x in all_series}
@@ -171,15 +175,17 @@
 
             series_to_consider = [s for s in self.series if re.fullmatch(entity.search, s.series_description)]
             series_to_consider = sorted(series_to_consider, key=lambda x: (x.subject, x.study_uid, x.series_number))
 
             series_to_convert = []
             if entity.index:
                 for k, g in itertools.groupby(series_to_consider, key=lambda x: x.study_uid):
-                    if m := next((x for i, x in enumerate(g) if i+1 == entity.index), None): series_to_convert.append(m)
+                    #if m := next((x for i, x in enumerate(g) if i+1 == entity.index), None): series_to_convert.append(m)
+                    m = next((x for i, x in enumerate(g) if i+1 == entity.index), None)
+                    if m: series_to_convert.append(m)
             else:
                 series_to_convert = series_to_consider
 
             runs = []
             if entity.autorun:
                 for k, g in itertools.groupby(series_to_consider, key=lambda x: x.study_uid):
                     runs.extend([i + 1 for i, s in enumerate(g)])
```

### Comparing `mrpyconvert-0.1.5/PKG-INFO` & `mrpyconvert-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrpyconvert
-Version: 0.1.5
+Version: 0.1.6
 Summary: Tool to create scripts to convert dicom to bids
 License: MIT
 Author: Jolinda Smith
 Author-email: jolinda@uoregon.edu
 Requires-Python: >=3.6.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

