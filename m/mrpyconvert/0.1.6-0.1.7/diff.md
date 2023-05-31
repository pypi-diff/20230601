# Comparing `tmp/mrpyconvert-0.1.6.tar.gz` & `tmp/mrpyconvert-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrpyconvert-0.1.6.tar", max compression
+gzip compressed data, was "mrpyconvert-0.1.7.tar", max compression
```

## Comparing `mrpyconvert-0.1.6.tar` & `mrpyconvert-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1064 2022-04-19 22:33:27.705840 mrpyconvert-0.1.6/LICENSE
--rw-r--r--   0        0        0       94 2023-03-23 20:24:49.074668 mrpyconvert-0.1.6/README.md
--rw-r--r--   0        0        0       46 2023-05-31 23:07:30.786223 mrpyconvert-0.1.6/mrpyconvert/__init__.py
--rw-r--r--   0        0        0     1798 2023-03-23 20:24:49.121983 mrpyconvert-0.1.6/mrpyconvert/dicom_sorter.py
--rw-r--r--   0        0        0    16227 2023-05-31 23:26:39.979382 mrpyconvert-0.1.6/mrpyconvert/mrpyconvert.py
--rw-r--r--   0        0        0      426 2023-05-31 23:27:07.686911 mrpyconvert-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 mrpyconvert-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-04-19 22:33:27.705840 mrpyconvert-0.1.7/LICENSE
+-rw-r--r--   0        0        0       94 2023-03-23 20:24:49.074668 mrpyconvert-0.1.7/README.md
+-rw-r--r--   0        0        0       46 2023-05-31 23:07:30.786223 mrpyconvert-0.1.7/mrpyconvert/__init__.py
+-rw-r--r--   0        0        0     1798 2023-03-23 20:24:49.121983 mrpyconvert-0.1.7/mrpyconvert/dicom_sorter.py
+-rw-r--r--   0        0        0    16365 2023-05-31 23:32:00.902474 mrpyconvert-0.1.7/mrpyconvert/mrpyconvert.py
+-rw-r--r--   0        0        0      426 2023-05-31 23:33:59.089949 mrpyconvert-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      736 1970-01-01 00:00:00.000000 mrpyconvert-0.1.7/PKG-INFO
```

### Comparing `mrpyconvert-0.1.6/LICENSE` & `mrpyconvert-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `mrpyconvert-0.1.6/mrpyconvert/dicom_sorter.py` & `mrpyconvert-0.1.7/mrpyconvert/dicom_sorter.py`

 * *Files identical despite different names*

### Comparing `mrpyconvert-0.1.6/mrpyconvert/mrpyconvert.py` & `mrpyconvert-0.1.7/mrpyconvert/mrpyconvert.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,17 +140,22 @@
                 print(f'More than one copy of {description} for at least one study')
 
     def set_names(self, bids_names: dict):
         for series in self.series:
             if series.orig_subject in bids_names:
                 series.subject = bids_names[series.orig_subject]
 
-    def generate_scripts(self, bids_path, script_ext='.sh', script_path=os.getcwd(), slurm=False,
+    def generate_scripts(self, bids_path, script_ext=None, script_path=os.getcwd(), slurm=False,
                          additional_commands=None, script_prefix=None):
 
+        if not script_ext:
+            if slurm:
+                script_ext = '.srun'
+            else:
+                script_ext = '.sh'
         # assign session numbers to series objects using dates
         if self.autosession:
             all_subjects = {x.subject for x in self.series}
             for subject in all_subjects:
                 s_series = [s for s in self.series if s.subject == subject]
                 s_series.sort(key = lambda x: (x.date, x.study_uid))
                 # get unique values, preserving order
```

### Comparing `mrpyconvert-0.1.6/PKG-INFO` & `mrpyconvert-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mrpyconvert
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tool to create scripts to convert dicom to bids
 License: MIT
 Author: Jolinda Smith
 Author-email: jolinda@uoregon.edu
 Requires-Python: >=3.6.8,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

