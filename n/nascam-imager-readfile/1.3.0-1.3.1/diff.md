# Comparing `tmp/nascam_imager_readfile-1.3.0.tar.gz` & `tmp/nascam_imager_readfile-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nascam_imager_readfile-1.3.0.tar", max compression
+gzip compressed data, was "nascam_imager_readfile-1.3.1.tar", max compression
```

## Comparing `nascam_imager_readfile-1.3.0.tar` & `nascam_imager_readfile-1.3.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2022-05-07 17:20:12.000000 nascam_imager_readfile-1.3.0/LICENSE
--rw-r--r--   0        0        0     2801 2023-05-31 17:29:41.564429 nascam_imager_readfile-1.3.0/README.md
--rw-r--r--   0        0        0       49 2023-05-31 17:29:51.092622 nascam_imager_readfile-1.3.0/nascam_imager_readfile/__init__.py
--rw-r--r--   0        0        0     9089 2023-05-31 18:07:17.540970 nascam_imager_readfile-1.3.0/nascam_imager_readfile/_nascam.py
--rw-r--r--   0        0        0      687 2023-05-31 17:29:51.032621 nascam_imager_readfile-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-05-07 17:20:12.000000 nascam_imager_readfile-1.3.1/LICENSE
+-rw-r--r--   0        0        0     2801 2023-05-31 17:29:41.564429 nascam_imager_readfile-1.3.1/README.md
+-rw-r--r--   0        0        0       49 2023-06-01 19:18:41.798327 nascam_imager_readfile-1.3.1/nascam_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     9399 2023-06-01 19:21:15.106500 nascam_imager_readfile-1.3.1/nascam_imager_readfile/_nascam.py
+-rw-r--r--   0        0        0      687 2023-06-01 19:18:41.752326 nascam_imager_readfile-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3550 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.3.1/PKG-INFO
```

### Comparing `nascam_imager_readfile-1.3.0/LICENSE` & `nascam_imager_readfile-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nascam_imager_readfile-1.3.0/README.md` & `nascam_imager_readfile-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nascam_imager_readfile-1.3.0/nascam_imager_readfile/_nascam.py` & `nascam_imager_readfile-1.3.1/nascam_imager_readfile/_nascam.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     image_dtype = image_dtype.newbyteorder('>')
 
     # check file extension to know how to process
     try:
         if (file_obj["filename"].endswith("png") or file_obj["filename"].endswith("png.tar")):
             return __nascam_readfile_worker_png(file_obj)
         else:
-            print("Unrecognized file type: %s" % (file_obj["filename"]))
+            if (file_obj["quiet"] is False):
+                print("Unrecognized file type: %s" % (file_obj["filename"]))
     except Exception as e:
-        import traceback
-        traceback.print_exc()
-        print("Failed to process file '%s' " % (file_obj["filename"]))
+        if (file_obj["quiet"] is False):
+            print("Failed to process file '%s' " % (file_obj["filename"]))
         problematic = True
         error_message = "failed to process file: %s" % (str(e))
     return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
         image_width, image_height, image_dtype
 
 
 def __nascam_readfile_worker_png(file_obj):
@@ -67,15 +67,16 @@
             if ("file_list" in locals()):
                 # cleanup
                 for f in file_list:
                     try:
                         os.remove(f)
                     except Exception:
                         pass
-            print("Failed to open file '%s' " % (file_obj["filename"]))
+            if (file_obj["quiet"] is False):
+                print("Failed to open file '%s' " % (file_obj["filename"]))
             problematic = True
             error_message = "failed to open file: %s" % (str(e))
             return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
                 image_width, image_height, image_dtype
     else:
         # regular png
         file_list = [file_obj["filename"]]
@@ -99,15 +100,16 @@
                 "Imager unique ID": device_uid,
                 "Mode unique ID": mode_uid,
                 "Image request start": timestamp,
                 "Subframe requested exposure": exposure,
             }
             metadata_dict_list.append(metadata_dict)
         except Exception as e:
-            print("Failed to read metadata from file '%s' " % (f))
+            if (file_obj["quiet"] is False):
+                print("Failed to read metadata from file '%s' " % (f))
             problematic = True
             error_message = "failed to read metadata: %s" % (str(e))
             break
 
         # read png file
         try:
             # read file
@@ -119,15 +121,16 @@
             # initialize image stack
             if (first_frame is True):
                 images = image_matrix
                 first_frame = False
             else:
                 images = np.dstack([images, image_matrix])  # depth stack images (on last axis)
         except Exception as e:
-            print("Failed reading image data frame: %s" % (str(e)))
+            if (file_obj["quiet"] is False):
+                print("Failed reading image data frame: %s" % (str(e)))
             metadata_dict_list.pop()  # remove corresponding metadata entry
             problematic = True
             error_message = "image data read failure: %s" % (str(e))
             continue  # skip to next frame
 
     # remove untarred files
     if (is_tar_file is True):
@@ -135,25 +138,27 @@
             os.remove(f)
 
     # return
     return images, metadata_dict_list, problematic, file_obj["filename"], error_message, \
         image_width, image_height, image_dtype
 
 
-def read(file_list, workers=1, tar_tempdir=None):
+def read(file_list, workers=1, tar_tempdir=None, quiet=False):
     """
     Read in a single PNG.TAR file, or an array of them. All files
     must be the same type.
 
     :param file_list: filename or list of filenames
     :type file_list: str
     :param workers: number of worker processes to spawn, defaults to 1
     :type workers: int, optional
     :param tar_tempdir: path to untar to, defaults to '~/.nascam_imager_readfile'
     :type tar_tempdir: str, optional
+    :param quiet: reduce output while reading data
+    :type quiet: bool, optional
 
     :return: images, metadata dictionaries, and problematic files
     :rtype: numpy.ndarray, list[dict], list[dict]
     """
     # set tar path
     if (tar_tempdir is None):
         tar_tempdir = Path("%s/.nascam_imager_readfile" % (str(Path.home())))
@@ -166,14 +171,15 @@
 
     # convert to object, injecting other data we need for processing
     processing_list = []
     for f in file_list:
         processing_list.append({
             "filename": f,
             "tar_tempdir": tar_tempdir,
+            "quiet": quiet,
         })
 
     # check workers
     if (workers > 1):
         try:
             # set up process pool (ignore SIGINT before spawning pool so child processes inherit SIGINT handler)
             original_sigint_handler = signal.signal(signal.SIGINT, signal.SIG_IGN)
```

### Comparing `nascam_imager_readfile-1.3.0/pyproject.toml` & `nascam_imager_readfile-1.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nascam-imager-readfile"
-version = "1.3.0"
+version = "1.3.1"
 description = "Read functions for NASCAM ASI raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/nascam-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/nascam-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
```

### Comparing `nascam_imager_readfile-1.3.0/PKG-INFO` & `nascam_imager_readfile-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nascam-imager-readfile
-Version: 1.3.0
+Version: 1.3.1
 Summary: Read functions for NASCAM ASI raw files
 Home-page: https://github.com/ucalgary-aurora/nascam-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

