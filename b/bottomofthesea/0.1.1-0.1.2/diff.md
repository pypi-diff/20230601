# Comparing `tmp/bottomofthesea-0.1.1.tar.gz` & `tmp/bottomofthesea-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bottomofthesea-0.1.1.tar", max compression
+gzip compressed data, was "bottomofthesea-0.1.2.tar", max compression
```

## Comparing `bottomofthesea-0.1.1.tar` & `bottomofthesea-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-31 22:45:30.476356 bottomofthesea-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-31 22:45:30.476293 bottomofthesea-0.1.1/bottomofthesea/__init__.py
--rw-r--r--   0        0        0     7836 2023-05-31 23:29:45.720260 bottomofthesea-0.1.1/bottomofthesea/bottomofthesea.py
--rw-r--r--   0        0        0     1825 2023-05-31 23:29:45.720330 bottomofthesea-0.1.1/bottomofthesea/preprocess.py
--rw-r--r--   0        0        0      608 2023-05-31 23:25:16.537508 bottomofthesea-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 bottomofthesea-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-31 22:45:30.476356 bottomofthesea-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-31 22:45:30.476293 bottomofthesea-0.1.2/bottomofthesea/__init__.py
+-rw-r--r--   0        0        0     7891 2023-06-01 17:32:14.480642 bottomofthesea-0.1.2/bottomofthesea/bottomofthesea.py
+-rw-r--r--   0        0        0     1825 2023-05-31 23:29:45.720330 bottomofthesea-0.1.2/bottomofthesea/preprocess.py
+-rw-r--r--   0        0        0      608 2023-06-01 17:32:25.829987 bottomofthesea-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 bottomofthesea-0.1.2/PKG-INFO
```

### Comparing `bottomofthesea-0.1.1/bottomofthesea/bottomofthesea.py` & `bottomofthesea-0.1.2/bottomofthesea/bottomofthesea.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,16 +144,17 @@
         else:
             opener = "open" if sys.platform == "darwin" else "xdg-open"
             subprocess.call([opener, filepath])
 
     def get_input():
         video = input("which video do you want to decode?(e.g. 02ss.mov): ")
         seconds = input(
-            "You shall choose a second in video to see different contents(put one number 1~10): "
-        )
+            "Choose a second in the video to see different contents (e.g. 11 seconds into the video = 11; 1 minute 30 seconds = 90):"
+        ) 
+        
         return (video, seconds)
 
     def found_video(filename):
         # Try this folder
         file_path = os.path.join(os.getcwd(), filename)
         if os.path.exists(file_path):
             return True, file_path
@@ -220,11 +221,12 @@
         path = Steganography.found_video(video)[1]
         images = bottomofthesea.preprocess.prepareFrames(path, seconds)
         Steganography.RESOLUTION = bottomofthesea.preprocess.get_video_size(path)
         for i in images:
             img = Image.fromarray(i)
             # img.show()
             Steganography().decode(img).show()
+        
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `bottomofthesea-0.1.1/bottomofthesea/preprocess.py` & `bottomofthesea-0.1.2/bottomofthesea/preprocess.py`

 * *Files identical despite different names*

### Comparing `bottomofthesea-0.1.1/pyproject.toml` & `bottomofthesea-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bottomofthesea"
-version = "0.1.1"
+version = "0.1.2"
 description = "Decodes hidden materials in the video from the Land At The Bottom Of The Sea project"
 authors = ["doublescoop <backslash.share@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["decode", "decoding", "steganography", "steg", "thelandatthebottomofthesea"]
```

### Comparing `bottomofthesea-0.1.1/PKG-INFO` & `bottomofthesea-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bottomofthesea
-Version: 0.1.1
+Version: 0.1.2
 Summary: Decodes hidden materials in the video from the Land At The Bottom Of The Sea project
 License: MIT
 Keywords: decode,decoding,steganography,steg,thelandatthebottomofthesea
 Author: doublescoop
 Author-email: backslash.share@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

