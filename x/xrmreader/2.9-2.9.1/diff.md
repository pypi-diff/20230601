# Comparing `tmp/xrmreader-2.9.tar.gz` & `tmp/xrmreader-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrmreader-2.9.tar", last modified: Wed Jul 20 14:57:44 2022, max compression
+gzip compressed data, was "xrmreader-2.9.1.tar", last modified: Thu Jun  1 08:32:04 2023, max compression
```

## Comparing `xrmreader-2.9.tar` & `xrmreader-2.9.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxr-x   0 mareike   (1000) mareike   (1000)        0 2022-07-20 14:57:44.898222 xrmreader-2.9/
--rw-r--r--   0 mareike   (1000) mareike   (1000)     3505 2021-04-22 10:03:54.000000 xrmreader-2.9/LICENSE
--rw-rw-r--   0 mareike   (1000) mareike   (1000)     6028 2022-07-20 14:57:44.898222 xrmreader-2.9/PKG-INFO
--rw-r--r--   0 mareike   (1000) mareike   (1000)     2097 2021-04-22 10:03:03.000000 xrmreader-2.9/README.md
--rw-r--r--   0 mareike   (1000) mareike   (1000)      104 2021-02-22 09:53:59.000000 xrmreader-2.9/pyproject.toml
--rw-r--r--   0 mareike   (1000) mareike   (1000)      593 2022-07-20 14:57:44.898222 xrmreader-2.9/setup.cfg
-drwxrwxr-x   0 mareike   (1000) mareike   (1000)        0 2022-07-20 14:57:44.898222 xrmreader-2.9/xrmreader/
--rw-r--r--   0 mareike   (1000) mareike   (1000)      325 2021-03-17 09:38:26.000000 xrmreader-2.9/xrmreader/__init__.py
--rw-r--r--   0 mareike   (1000) mareike   (1000)    11182 2022-06-03 10:46:22.000000 xrmreader-2.9/xrmreader/preprocessor.py
--rw-r--r--   0 mareike   (1000) mareike   (1000)    30123 2022-07-20 14:53:23.000000 xrmreader-2.9/xrmreader/reader.py
-drwxrwxr-x   0 mareike   (1000) mareike   (1000)        0 2022-07-20 14:57:44.898222 xrmreader-2.9/xrmreader.egg-info/
--rw-r--r--   0 mareike   (1000) mareike   (1000)     6028 2022-07-20 14:57:44.000000 xrmreader-2.9/xrmreader.egg-info/PKG-INFO
--rw-r--r--   0 mareike   (1000) mareike   (1000)      274 2022-07-20 14:57:44.000000 xrmreader-2.9/xrmreader.egg-info/SOURCES.txt
--rw-r--r--   0 mareike   (1000) mareike   (1000)        1 2022-07-20 14:57:44.000000 xrmreader-2.9/xrmreader.egg-info/dependency_links.txt
--rw-r--r--   0 mareike   (1000) mareike   (1000)       38 2022-07-20 14:57:44.000000 xrmreader-2.9/xrmreader.egg-info/requires.txt
--rw-r--r--   0 mareike   (1000) mareike   (1000)       10 2022-07-20 14:57:44.000000 xrmreader-2.9/xrmreader.egg-info/top_level.txt
+drwxrwxr-x   0 mareike   (1000) mareike   (1000)        0 2023-06-01 08:32:04.530100 xrmreader-2.9.1/
+-rw-r--r--   0 mareike   (1000) mareike   (1000)     3505 2021-04-22 10:03:54.000000 xrmreader-2.9.1/LICENSE
+-rw-rw-r--   0 mareike   (1000) mareike   (1000)     6030 2023-06-01 08:32:04.530100 xrmreader-2.9.1/PKG-INFO
+-rw-r--r--   0 mareike   (1000) mareike   (1000)     2097 2021-04-22 10:03:03.000000 xrmreader-2.9.1/README.md
+-rw-r--r--   0 mareike   (1000) mareike   (1000)      104 2021-02-22 09:53:59.000000 xrmreader-2.9.1/pyproject.toml
+-rw-r--r--   0 mareike   (1000) mareike   (1000)      595 2023-06-01 08:32:04.530100 xrmreader-2.9.1/setup.cfg
+drwxrwxr-x   0 mareike   (1000) mareike   (1000)        0 2023-06-01 08:32:04.530100 xrmreader-2.9.1/tests/
+-rw-r--r--   0 mareike   (1000) mareike   (1000)     1332 2022-10-10 07:10:17.000000 xrmreader-2.9.1/tests/test.py
+drwxrwxr-x   0 mareike   (1000) mareike   (1000)        0 2023-06-01 08:32:04.530100 xrmreader-2.9.1/xrmreader/
+-rw-r--r--   0 mareike   (1000) mareike   (1000)      325 2021-03-17 09:38:26.000000 xrmreader-2.9.1/xrmreader/__init__.py
+-rw-r--r--   0 mareike   (1000) mareike   (1000)    11176 2023-06-01 08:30:05.000000 xrmreader-2.9.1/xrmreader/preprocessor.py
+-rw-r--r--   0 mareike   (1000) mareike   (1000)    30123 2022-07-20 14:53:23.000000 xrmreader-2.9.1/xrmreader/reader.py
+drwxrwxr-x   0 mareike   (1000) mareike   (1000)        0 2023-06-01 08:32:04.530100 xrmreader-2.9.1/xrmreader.egg-info/
+-rw-r--r--   0 mareike   (1000) mareike   (1000)     6030 2023-06-01 08:32:04.000000 xrmreader-2.9.1/xrmreader.egg-info/PKG-INFO
+-rw-r--r--   0 mareike   (1000) mareike   (1000)      288 2023-06-01 08:32:04.000000 xrmreader-2.9.1/xrmreader.egg-info/SOURCES.txt
+-rw-r--r--   0 mareike   (1000) mareike   (1000)        1 2023-06-01 08:32:04.000000 xrmreader-2.9.1/xrmreader.egg-info/dependency_links.txt
+-rw-r--r--   0 mareike   (1000) mareike   (1000)       38 2023-06-01 08:32:04.000000 xrmreader-2.9.1/xrmreader.egg-info/requires.txt
+-rw-r--r--   0 mareike   (1000) mareike   (1000)       10 2023-06-01 08:32:04.000000 xrmreader-2.9.1/xrmreader.egg-info/top_level.txt
```

### Comparing `xrmreader-2.9/LICENSE` & `xrmreader-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xrmreader-2.9/PKG-INFO` & `xrmreader-2.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrmreader
-Version: 2.9
+Version: 2.9.1
 Summary: A reader and preprocessor for txrm/xrm data acquired by Zeiss microscopes.
 Home-page: https://git5.cs.fau.de/mthies/xrm_reader
 Author: Mareike Thies
 Author-email: mareike.thies@fau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `xrmreader-2.9/README.md` & `xrmreader-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `xrmreader-2.9/setup.cfg` & `xrmreader-2.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xrmreader
-version = 2.9
+version = 2.9.1
 author = Mareike Thies
 author_email = mareike.thies@fau.de
 description = A reader and preprocessor for txrm/xrm data acquired by Zeiss microscopes.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://git5.cs.fau.de/mthies/xrm_reader
 license_files = LICENSE
```

### Comparing `xrmreader-2.9/xrmreader/preprocessor.py` & `xrmreader-2.9.1/xrmreader/preprocessor.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     num_images = metadata['number_of_images']
     x_shifts = metadata['x-shifts'][::angular_factor]
     y_shifts = metadata['y-shifts'][::angular_factor]
     reference = metadata['reference']
     if not dose_reduction == 1.:
         reference_smooth = smooth_reference(reference)
     if keep_rows is not None:
-        keep_rows = keep_rows.astype(np.bool)
+        keep_rows = keep_rows.astype(bool)
         projection_height = int(np.ceil(np.sum(keep_rows) / downsample_factor))
     else:
         projection_height = int(np.ceil(float(metadata['image_height']) / downsample_factor))
     if do_truncation_correction:
         projections = np.zeros((int(np.ceil(num_images / angular_factor)),
                                 projection_height,
                                 int(np.ceil(float(metadata['image_width']) / downsample_factor)) + 2 * int(
@@ -213,15 +213,15 @@
                              extension_fraction=0.1, dose_reduction=1., datatype=np.float32, keep_rows=None,
                              do_beam_hardening_correction=False, poly=None):
     metadata = read_metadata(str(projections_file))
     reference = metadata['reference']
     if not dose_reduction == 1.:
         reference_smooth = smooth_reference(reference)
     if keep_rows is not None:
-        keep_rows = keep_rows.astype(np.bool)
+        keep_rows = keep_rows.astype(bool)
     for projection in read_txrm_iterable(str(projections_file)):
         projection = np.expand_dims(projection, 0)
         projection = divide_by_reference(projection, reference)
         if keep_rows is not None:
             projection = projection[:, keep_rows, :]
         projection = negative_logarithm(projection)
         if not dose_reduction == 1.:
```

### Comparing `xrmreader-2.9/xrmreader/reader.py` & `xrmreader-2.9.1/xrmreader/reader.py`

 * *Files identical despite different names*

### Comparing `xrmreader-2.9/xrmreader.egg-info/PKG-INFO` & `xrmreader-2.9.1/xrmreader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrmreader
-Version: 2.9
+Version: 2.9.1
 Summary: A reader and preprocessor for txrm/xrm data acquired by Zeiss microscopes.
 Home-page: https://git5.cs.fau.de/mthies/xrm_reader
 Author: Mareike Thies
 Author-email: mareike.thies@fau.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

