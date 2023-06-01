# Comparing `tmp/trex_imager_readfile-1.4.0.tar.gz` & `tmp/trex_imager_readfile-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trex_imager_readfile-1.4.0.tar", max compression
+gzip compressed data, was "trex_imager_readfile-1.4.1.tar", max compression
```

## Comparing `trex_imager_readfile-1.4.0.tar` & `trex_imager_readfile-1.4.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      186 2023-04-25 13:48:57.783144 trex_imager_readfile-1.4.0/README.md
--rw-r--r--   0        0        0      699 2023-05-31 18:09:31.438669 trex_imager_readfile-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      397 2023-05-31 18:09:31.471670 trex_imager_readfile-1.4.0/trex_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8497 2023-05-03 20:42:44.563933 trex_imager_readfile-1.4.0/trex_imager_readfile/blueline.py
--rw-r--r--   0        0        0     8447 2023-05-03 20:42:40.512856 trex_imager_readfile-1.4.0/trex_imager_readfile/nir.py
--rw-r--r--   0        0        0    20625 2023-05-31 18:11:41.895299 trex_imager_readfile-1.4.0/trex_imager_readfile/rgb.py
--rw-r--r--   0        0        0     8541 2023-05-03 20:42:47.366986 trex_imager_readfile-1.4.0/trex_imager_readfile/spectrograph.py
--rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 trex_imager_readfile-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      186 2023-04-25 13:48:57.783144 trex_imager_readfile-1.4.1/README.md
+-rw-r--r--   0        0        0      699 2023-06-01 18:43:30.748107 trex_imager_readfile-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      397 2023-06-01 18:43:30.787107 trex_imager_readfile-1.4.1/trex_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     9073 2023-06-01 18:59:35.187783 trex_imager_readfile-1.4.1/trex_imager_readfile/blueline.py
+-rw-r--r--   0        0        0     9018 2023-06-01 19:04:02.929246 trex_imager_readfile-1.4.1/trex_imager_readfile/nir.py
+-rw-r--r--   0        0        0    20625 2023-06-01 19:06:54.748765 trex_imager_readfile-1.4.1/trex_imager_readfile/rgb.py
+-rw-r--r--   0        0        0     9121 2023-06-01 18:59:34.177762 trex_imager_readfile-1.4.1/trex_imager_readfile/spectrograph.py
+-rw-r--r--   0        0        0      970 1970-01-01 00:00:00.000000 trex_imager_readfile-1.4.1/PKG-INFO
```

### Comparing `trex_imager_readfile-1.4.0/pyproject.toml` & `trex_imager_readfile-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "trex-imager-readfile"
-version = "1.4.0"
+version = "1.4.1"
 description = "Read functions for TREx ASI raw image files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/trex-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/trex-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `trex_imager_readfile-1.4.0/trex_imager_readfile/blueline.py` & `trex_imager_readfile-1.4.1/trex_imager_readfile/blueline.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,33 +161,45 @@
     """
     # pre-allocate array sizes (optimization)
     predicted_num_frames = len(file_list) * 20
     images = np.empty([270, 320, predicted_num_frames], dtype=__BLUELINE_DT)
     metadata_dict_list = [{}] * predicted_num_frames
     problematic_file_list = []
 
-    # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    pool = Pool(processes=workers)
-    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
-
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
-    # call readfile function, run each iteration with a single input file from file_list
-    # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
-    data = []
-    try:
-        data = pool.map(partial(__blueline_readfile_worker, quiet=quiet), file_list)
-    except KeyboardInterrupt:
-        pool.terminate()  # gracefully kill children
-        return np.empty((0, 0, 0), dtype=__BLUELINE_DT), [], []
+    # check workers
+    if (workers > 1):
+        try:
+            # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
+            original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+            pool = Pool(processes=workers)
+            signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+        except ValueError:
+            # likely the read call is being used within a context that doesn't support the usage
+            # of signals in this way, proceed without it
+            pool = Pool(processes=workers)
+
+        # call readfile function, run each iteration with a single input file from file_list
+        # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
+        data = []
+        try:
+            data = pool.map(partial(__blueline_readfile_worker, quiet=quiet), file_list)
+        except KeyboardInterrupt:
+            pool.terminate()  # gracefully kill children
+            return np.empty((0, 0, 0), dtype=__BLUELINE_DT), [], []
+        else:
+            pool.close()
     else:
-        pool.close()
+        # don't bother using multiprocessing with one worker, just call the worker function directly
+        data = []
+        for f in file_list:
+            data.append(__blueline_readfile_worker(f, quiet=quiet))
 
     # reorganize data
     list_position = 0
     for i in range(0, len(data)):
         # check if file was problematic
         if (data[i][2] is True):
             problematic_file_list.append({
```

### Comparing `trex_imager_readfile-1.4.0/trex_imager_readfile/nir.py` & `trex_imager_readfile-1.4.1/trex_imager_readfile/nir.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,33 +161,45 @@
     """
     # pre-allocate array sizes (optimization)
     predicted_num_frames = len(file_list) * 10
     images = np.empty([256, 256, predicted_num_frames], dtype=__NIR_DT)
     metadata_dict_list = [{}] * predicted_num_frames
     problematic_file_list = []
 
-    # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    pool = Pool(processes=workers)
-    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
-
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
-    # call readfile function, run each iteration with a single input file from file_list
-    # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
-    data = []
-    try:
-        data = pool.map(partial(__nir_readfile_worker, quiet=quiet), file_list)
-    except KeyboardInterrupt:
-        pool.terminate()  # gracefully kill children
-        return np.empty((0, 0, 0), dtype=__NIR_DT), [], []
+    # check workers
+    if (workers > 1):
+        try:
+            # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
+            original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+            pool = Pool(processes=workers)
+            signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+        except ValueError:
+            # likely the read call is being used within a context that doesn't support the usage
+            # of signals in this way, proceed without it
+            pool = Pool(processes=workers)
+
+        # call readfile function, run each iteration with a single input file from file_list
+        # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
+        data = []
+        try:
+            data = pool.map(partial(__nir_readfile_worker, quiet=quiet), file_list)
+        except KeyboardInterrupt:
+            pool.terminate()  # gracefully kill children
+            return np.empty((0, 0, 0), dtype=__NIR_DT), [], []
+        else:
+            pool.close()
     else:
-        pool.close()
+        # don't bother using multiprocessing with one worker, just call the worker function directly
+        data = []
+        for f in file_list:
+            data.append(__nir_readfile_worker(f, quiet=quiet))
 
     # reorganize data
     list_position = 0
     for i in range(0, len(data)):
         # check if file was problematic
         if (data[i][2] is True):
             problematic_file_list.append({
```

### Comparing `trex_imager_readfile-1.4.0/trex_imager_readfile/rgb.py` & `trex_imager_readfile-1.4.1/trex_imager_readfile/rgb.py`

 * *Files identical despite different names*

### Comparing `trex_imager_readfile-1.4.0/trex_imager_readfile/spectrograph.py` & `trex_imager_readfile-1.4.1/trex_imager_readfile/spectrograph.py`

 * *Files 3% similar despite different names*

```diff
@@ -161,33 +161,45 @@
     """
     # pre-allocate array sizes (optimization)
     predicted_num_frames = len(file_list) * 4
     images = np.empty([1024, 256, predicted_num_frames], dtype=__SPECTROGRAPH_DT)
     metadata_dict_list = [{}] * predicted_num_frames
     problematic_file_list = []
 
-    # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
-    original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
-    pool = Pool(processes=workers)
-    signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
-
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
 
-    # call readfile function, run each iteration with a single input file from file_list
-    # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
-    data = []
-    try:
-        data = pool.map(partial(__spectrograph_readfile_worker, quiet=quiet), file_list)
-    except KeyboardInterrupt:
-        pool.terminate()  # gracefully kill children
-        return np.empty((0, 0, 0), dtype=__SPECTROGRAPH_DT), [], []
+    # check workers
+    if (workers > 1):
+        try:
+            # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
+            original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
+            pool = Pool(processes=workers)
+            signal.signal(signal.SIGINT, original_sigint_handler)  # restore SIGINT handler
+        except ValueError:
+            # likely the read call is being used within a context that doesn't support the usage
+            # of signals in this way, proceed without it
+            pool = Pool(processes=workers)
+
+        # call readfile function, run each iteration with a single input file from file_list
+        # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
+        data = []
+        try:
+            data = pool.map(partial(__spectrograph_readfile_worker, quiet=quiet), file_list)
+        except KeyboardInterrupt:
+            pool.terminate()  # gracefully kill children
+            return np.empty((0, 0, 0), dtype=__SPECTROGRAPH_DT), [], []
+        else:
+            pool.close()
     else:
-        pool.close()
+        # don't bother using multiprocessing with one worker, just call the worker function directly
+        data = []
+        for f in file_list:
+            data.append(__spectrograph_readfile_worker(f, quiet=quiet))
 
     # reorganize data
     list_position = 0
     for i in range(0, len(data)):
         # check if file was problematic
         if (data[i][2] is True):
             problematic_file_list.append({
```

### Comparing `trex_imager_readfile-1.4.0/PKG-INFO` & `trex_imager_readfile-1.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trex-imager-readfile
-Version: 1.4.0
+Version: 1.4.1
 Summary: Read functions for TREx ASI raw image files
 Home-page: https://github.com/ucalgary-aurora/trex-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

