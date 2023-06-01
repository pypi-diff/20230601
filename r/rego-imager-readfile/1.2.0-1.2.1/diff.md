# Comparing `tmp/rego_imager_readfile-1.2.0.tar.gz` & `tmp/rego_imager_readfile-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rego_imager_readfile-1.2.0.tar", max compression
+gzip compressed data, was "rego_imager_readfile-1.2.1.tar", max compression
```

## Comparing `rego_imager_readfile-1.2.0.tar` & `rego_imager_readfile-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.2.0/LICENSE
--rw-r--r--   0        0        0     2688 2023-05-30 20:01:33.986595 rego_imager_readfile-1.2.0/README.md
--rw-r--r--   0        0        0      656 2023-05-30 21:50:02.012379 rego_imager_readfile-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-05-30 21:50:02.056681 rego_imager_readfile-1.2.0/rego_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8216 2023-05-31 15:31:57.803617 rego_imager_readfile-1.2.0/rego_imager_readfile/_rego.py
--rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 rego_imager_readfile-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2688 2023-05-30 20:01:33.986595 rego_imager_readfile-1.2.1/README.md
+-rw-r--r--   0        0        0      656 2023-06-01 19:14:18.280872 rego_imager_readfile-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-06-01 19:14:18.317873 rego_imager_readfile-1.2.1/rego_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8579 2023-06-01 19:15:57.945935 rego_imager_readfile-1.2.1/rego_imager_readfile/_rego.py
+-rw-r--r--   0        0        0     3387 1970-01-01 00:00:00.000000 rego_imager_readfile-1.2.1/PKG-INFO
```

### Comparing `rego_imager_readfile-1.2.0/LICENSE` & `rego_imager_readfile-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rego_imager_readfile-1.2.0/README.md` & `rego_imager_readfile-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `rego_imager_readfile-1.2.0/pyproject.toml` & `rego_imager_readfile-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rego-imager-readfile"
-version = "1.2.0"
+version = "1.2.1"
 description = "Read functions for REGO ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `rego_imager_readfile-1.2.0/rego_imager_readfile/_rego.py` & `rego_imager_readfile-1.2.1/rego_imager_readfile/_rego.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 import gzip
 import signal
 import numpy as np
 from multiprocessing import Pool
+from functools import partial
 
 # globals
 REGO_IMAGE_SIZE_BYTES = 512 * 512 * 2
 REGO_DT = np.dtype("uint16")
 REGO_DT = REGO_DT.newbyteorder('>')  # force big endian byte ordering
 
 
-def read(file_list, workers=1):
+def read(file_list, workers=1, quiet=False):
     """
     Read in a single PGM file or set of PGM files
 
     :param file_list: filename or list of filenames
     :type file_list: str
     :param workers: number of worker processes to spawn, defaults to 1
     :type workers: int, optional
+    :param quiet: reduce output while reading data
+    :type quiet: bool, optional
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
     # pre-allocate array sizes (optimization)
     predicted_num_frames = len(file_list) * 20
     images = np.empty([512, 512, predicted_num_frames], dtype=REGO_DT)
@@ -43,25 +46,25 @@
             # of signals in this way, proceed without it
             pool = Pool(processes=workers)
 
         # call readfile function, run each iteration with a single input file from file_list
         # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
         data = []
         try:
-            data = pool.map(__rego_readfile_worker, file_list)
+            data = pool.map(partial(__rego_readfile_worker, quiet=quiet), file_list)
         except KeyboardInterrupt:
             pool.terminate()  # gracefully kill children
             return np.empty((0, 0, 0), dtype=REGO_DT), [], []
         else:
             pool.close()
     else:
         # don't bother using multiprocessing with one worker, just call the worker function directly
         data = []
         for f in file_list:
-            data.append(__rego_readfile_worker(f))
+            data.append(__rego_readfile_worker(f, quiet=quiet))
 
     # reorganize data
     list_position = 0
     for i in range(0, len(data)):
         # check if file was problematic
         if (data[i][2] is True):
             problematic_file_list.append({
@@ -90,15 +93,15 @@
     images = images.astype(np.uint16)
 
     # return
     data = None
     return images, metadata_dict_list, problematic_file_list
 
 
-def __rego_readfile_worker(file):
+def __rego_readfile_worker(file, quiet=False):
     # init
     images = np.array([])
     metadata_dict_list = []
     first_frame = True
     metadata_dict = {}
     site_uid = ""
     device_uid = ""
@@ -108,29 +111,32 @@
     # check file extension to see if it's gzipped or not
     try:
         if file.endswith("pgm.gz"):
             unzipped = gzip.open(file, mode='rb')
         elif file.endswith("pgm"):
             unzipped = open(file, mode='rb')
         else:
-            print("Unrecognized file type: %s" % (file))
+            if (quiet is False):
+                print("Unrecognized file type: %s" % (file))
             return images, metadata_dict_list, problematic, file, error_message
     except Exception as e:
-        print("Failed to open file '%s' " % (file))
+        if (quiet is False):
+            print("Failed to open file '%s' " % (file))
         problematic = True
         error_message = "failed to open file: %s" % (str(e))
         return images, metadata_dict_list, problematic, file, error_message
 
     # read the file
     while True:
         # read a line
         try:
             line = unzipped.readline()
         except Exception as e:
-            print("Error reading before image data in file '%s'" % (file))
+            if (quiet is False):
+                print("Error reading before image data in file '%s'" % (file))
             problematic = True
             metadata_dict_list = []
             images = np.array([])
             error_message = "error reading before image data: %s" % (str(e))
             return images, metadata_dict_list, problematic, file, error_message
 
         # break loop at end of file
@@ -144,15 +150,16 @@
         # process line
         if (line.startswith(b'#"')):
             # metadata lines start with #"<key>"
             try:
                 line_decoded = line.decode("ascii")
             except Exception as e:
                 # skip metadata line if it can't be decoded, likely corrupt file
-                print("Error decoding metadata line: %s (line='%s', file='%s')" % (str(e), line, file))
+                if (quiet is False):
+                    print("Error decoding metadata line: %s (line='%s', file='%s')" % (str(e), line, file))
                 problematic = True
                 error_message = "error decoding metadata line: %s" % (str(e))
                 continue
 
             # split the key and value out of the metadata line
             line_decoded_split = line_decoded.split('"')
             key = line_decoded_split[1]
@@ -188,15 +195,16 @@
                 # format bytes into numpy array of unsigned shorts (2byte numbers, 0-65536),
                 # effectively an array of pixel values
                 image_np = np.frombuffer(image_bytes, dtype=REGO_DT)
 
                 # change 1d numpy array into 512x512 matrix with correctly located pixels
                 image_matrix = np.reshape(image_np, (512, 512, 1))
             except Exception as e:
-                print("Failed reading image data frame: %s" % (str(e)))
+                if (quiet is False):
+                    print("Failed reading image data frame: %s" % (str(e)))
                 metadata_dict_list.pop()  # remove corresponding metadata entry
                 problematic = True
                 error_message = "image data read failure: %s" % (str(e))
                 continue  # skip to next frame
 
             # initialize image stack
             if first_frame:
```

### Comparing `rego_imager_readfile-1.2.0/PKG-INFO` & `rego_imager_readfile-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rego-imager-readfile
-Version: 1.2.0
+Version: 1.2.1
 Summary: Read functions for REGO ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/rego-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

