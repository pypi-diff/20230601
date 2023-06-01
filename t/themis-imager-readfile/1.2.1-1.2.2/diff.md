# Comparing `tmp/themis_imager_readfile-1.2.1.tar.gz` & `tmp/themis_imager_readfile-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themis_imager_readfile-1.2.1.tar", max compression
+gzip compressed data, was "themis_imager_readfile-1.2.2.tar", max compression
```

## Comparing `themis_imager_readfile-1.2.1.tar` & `themis_imager_readfile-1.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.2.1/LICENSE
--rw-r--r--   0        0        0     2763 2023-05-15 18:17:56.997619 themis_imager_readfile-1.2.1/README.md
--rw-r--r--   0        0        0      666 2023-05-31 15:56:15.011026 themis_imager_readfile-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       49 2023-05-31 15:56:15.045027 themis_imager_readfile-1.2.1/themis_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8971 2023-05-31 15:54:47.371259 themis_imager_readfile-1.2.1/themis_imager_readfile/_themis.py
--rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 themis_imager_readfile-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2763 2023-05-15 18:17:56.997619 themis_imager_readfile-1.2.2/README.md
+-rw-r--r--   0        0        0      666 2023-06-01 19:09:36.235074 themis_imager_readfile-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-06-01 19:09:36.268075 themis_imager_readfile-1.2.2/themis_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     9408 2023-06-01 19:13:29.828869 themis_imager_readfile-1.2.2/themis_imager_readfile/_themis.py
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 themis_imager_readfile-1.2.2/PKG-INFO
```

### Comparing `themis_imager_readfile-1.2.1/LICENSE` & `themis_imager_readfile-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.2.1/README.md` & `themis_imager_readfile-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.2.1/pyproject.toml` & `themis_imager_readfile-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "themis-imager-readfile"
-version = "1.2.1"
+version = "1.2.2"
 description = "Read functions for THEMIS ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `themis_imager_readfile-1.2.1/themis_imager_readfile/_themis.py` & `themis_imager_readfile-1.2.2/themis_imager_readfile/_themis.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import gzip
 import bz2
 import signal
 import numpy as np
 from multiprocessing import Pool
+from functools import partial
 
 # globals
 THEMIS_IMAGE_SIZE_BYTES = 131072
 THEMIS_DT = np.dtype("uint16")
 THEMIS_DT = THEMIS_DT.newbyteorder('>')  # force big endian byte ordering
 THEMIS_EXPECTED_MINUTE_NUM_FRAMES = 20
 
 
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
     # if input is just a single file name in a string, convert to a list to be fed to the workers
     if isinstance(file_list, str):
         file_list = [file_list]
@@ -39,25 +42,25 @@
             # of signals in this way, proceed without it
             pool = Pool(processes=workers)
 
         # call readfile function, run each iteration with a single input file from file_list
         # NOTE: structure of data - data[file][metadata dictionary lists = 1, images = 0][frame]
         data = []
         try:
-            data = pool.map(__themis_readfile_worker, file_list)
+            data = pool.map(partial(__themis_readfile_worker, quiet=quiet), file_list)
         except KeyboardInterrupt:
             pool.terminate()  # gracefully kill children
             return np.empty((0, 0, 0), dtype=THEMIS_DT), [], []
         else:
             pool.close()
     else:
         # don't bother using multiprocessing with one worker, just call the worker function directly
         data = []
         for f in file_list:
-            data.append(__themis_readfile_worker(f))
+            data.append(__themis_readfile_worker(f, quiet=quiet))
 
     # derive number of frames to prepare for
     total_num_frames = 0
     for i in range(0, len(data)):
         if (data[i][2] is True):
             continue
         total_num_frames += data[i][0].shape[2]
@@ -99,15 +102,15 @@
     images = images.astype(np.uint16)
 
     # return
     data = None
     return images, metadata_dict_list, problematic_file_list
 
 
-def __themis_readfile_worker(file):
+def __themis_readfile_worker(file, quiet=False):
     # init
     images = np.array([])
     metadata_dict_list = []
     first_frame = True
     metadata_dict = {}
     site_uid = ""
     device_uid = ""
@@ -119,31 +122,34 @@
         if file.endswith("pgm.gz"):
             unzipped = gzip.open(file, mode='rb')
         elif file.endswith("pgm"):
             unzipped = open(file, mode='rb')
         elif file.endswith("pgm.bz2"):
             unzipped = bz2.open(file, mode='rb')
         else:
-            print("Unrecognized file type: %s" % (file))
+            if (quiet is False):
+                print("Unrecognized file type: %s" % (file))
             problematic = True
             error_message = "Unrecognized file type"
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
@@ -157,21 +163,23 @@
         # process line
         if (line.startswith(b'#"')):
             # metadata lines start with #"<key>"
             try:
                 line_decoded = line.decode("ascii")
             except Exception as e:
                 # skip metadata line if it can't be decoded, likely corrupt file but don't mark it as one yet
-                print("Warning: issue decoding metadata line: %s (line='%s', file='%s')" % (str(e), line, file))
+                if (quiet is False):
+                    print("Warning: issue decoding metadata line: %s (line='%s', file='%s')" % (str(e), line, file))
                 continue
 
             # split the key and value out of the metadata line
             line_decoded_split = line_decoded.split('"')
             if (len(line_decoded_split) != 3):
-                print("Warning: issue splitting metadata line (line='%s', file='%s')" % (line_decoded, file))
+                if (quiet is False):
+                    print("Warning: issue splitting metadata line (line='%s', file='%s')" % (line_decoded, file))
                 continue
             key = line_decoded_split[1]
             value = line_decoded_split[2].strip()
 
             # add entry to dictionary
             metadata_dict[key] = value
 
@@ -202,15 +210,16 @@
                 # format bytes into numpy array of unsigned shorts (2byte numbers, 0-65536),
                 # effectively an array of pixel values
                 image_np = np.frombuffer(image_bytes, dtype=THEMIS_DT)
 
                 # change 1d numpy array into 256x256 matrix with correctly located pixels
                 image_matrix = np.reshape(image_np, (256, 256, 1))
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
@@ -220,13 +229,14 @@
                 images = np.dstack([images, image_matrix])  # depth stack images (on 3rd axis)
 
     # close gzip file
     unzipped.close()
 
     # check to see if the image is empty
     if (images.size == 0):
-        print("Error reading image file: found no image data")
+        if (quiet is False):
+            print("Error reading image file: found no image data")
         problematic = True
         error_message = "no image data"
 
     # return
     return images, metadata_dict_list, problematic, file, error_message
```

### Comparing `themis_imager_readfile-1.2.1/PKG-INFO` & `themis_imager_readfile-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: themis-imager-readfile
-Version: 1.2.1
+Version: 1.2.2
 Summary: Read functions for THEMIS ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/themis-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

