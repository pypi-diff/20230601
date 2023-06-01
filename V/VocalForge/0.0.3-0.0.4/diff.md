# Comparing `tmp/VocalForge-0.0.3.tar.gz` & `tmp/VocalForge-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VocalForge-0.0.3.tar", last modified: Thu Jun  1 02:30:15 2023, max compression
+gzip compressed data, was "VocalForge-0.0.4.tar", last modified: Thu Jun  1 02:33:44 2023, max compression
```

## Comparing `VocalForge-0.0.3.tar` & `VocalForge-0.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:30:15.296374 VocalForge-0.0.3/
--rw-rw-r--   0 rio       (1000) rio       (1000)     1067 2023-05-21 03:39:13.000000 VocalForge-0.0.3/LICENSE.md
--rw-rw-r--   0 rio       (1000) rio       (1000)     6310 2023-06-01 02:30:15.296374 VocalForge-0.0.3/PKG-INFO
--rw-rw-r--   0 rio       (1000) rio       (1000)     5774 2023-05-21 03:39:13.000000 VocalForge-0.0.3/README.md
--rw-rw-r--   0 rio       (1000) rio       (1000)      706 2023-06-01 02:30:09.000000 VocalForge-0.0.3/pyproject.toml
--rw-rw-r--   0 rio       (1000) rio       (1000)      302 2023-06-01 02:27:56.000000 VocalForge-0.0.3/requirements.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)       38 2023-06-01 02:30:15.296374 VocalForge-0.0.3/setup.cfg
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:30:15.296374 VocalForge-0.0.3/src/
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:30:15.296374 VocalForge-0.0.3/src/VocalForge/
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:30:15.296374 VocalForge-0.0.3/src/VocalForge/audio/
--rw-rw-r--   0 rio       (1000) rio       (1000)      204 2023-05-31 00:06:05.000000 VocalForge-0.0.3/src/VocalForge/audio/__init__.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    10276 2023-05-30 05:30:07.000000 VocalForge-0.0.3/src/VocalForge/audio/audio_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     4708 2023-05-31 03:13:49.000000 VocalForge-0.0.3/src/VocalForge/audio/export_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     5777 2023-05-31 03:15:02.000000 VocalForge-0.0.3/src/VocalForge/audio/isolate.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2068 2023-05-30 05:32:42.000000 VocalForge-0.0.3/src/VocalForge/audio/overlap.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2386 2023-05-31 00:06:30.000000 VocalForge-0.0.3/src/VocalForge/audio/refine_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     3002 2023-05-30 05:31:11.000000 VocalForge-0.0.3/src/VocalForge/audio/voice_detection.py
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:30:15.296374 VocalForge-0.0.3/src/VocalForge/text/
--rw-rw-r--   0 rio       (1000) rio       (1000)      250 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/__init__.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     3555 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/create_dataset.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2211 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/ctc.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    26284 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/ctc_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     1666 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/normalization_helpers.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     4247 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/normalize_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)    10460 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/process_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2442 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/refine_text.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2277 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/segment.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     1759 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/split_audio.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     5407 2023-05-31 04:31:49.000000 VocalForge-0.0.3/src/VocalForge/text/text_utils.py
--rw-rw-r--   0 rio       (1000) rio       (1000)     2330 2023-05-21 03:39:13.000000 VocalForge-0.0.3/src/VocalForge/text/transcribe.py
-drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:30:15.296374 VocalForge-0.0.3/src/VocalForge.egg-info/
--rw-rw-r--   0 rio       (1000) rio       (1000)     6310 2023-06-01 02:30:15.000000 VocalForge-0.0.3/src/VocalForge.egg-info/PKG-INFO
--rw-rw-r--   0 rio       (1000) rio       (1000)      906 2023-06-01 02:30:15.000000 VocalForge-0.0.3/src/VocalForge.egg-info/SOURCES.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)        1 2023-06-01 02:30:15.000000 VocalForge-0.0.3/src/VocalForge.egg-info/dependency_links.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)      302 2023-06-01 02:30:15.000000 VocalForge-0.0.3/src/VocalForge.egg-info/requires.txt
--rw-rw-r--   0 rio       (1000) rio       (1000)       11 2023-06-01 02:30:15.000000 VocalForge-0.0.3/src/VocalForge.egg-info/top_level.txt
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1067 2023-05-21 03:39:13.000000 VocalForge-0.0.4/LICENSE.md
+-rw-rw-r--   0 rio       (1000) rio       (1000)     6310 2023-06-01 02:33:44.242594 VocalForge-0.0.4/PKG-INFO
+-rw-rw-r--   0 rio       (1000) rio       (1000)     5774 2023-05-21 03:39:13.000000 VocalForge-0.0.4/README.md
+-rw-rw-r--   0 rio       (1000) rio       (1000)      706 2023-06-01 02:33:01.000000 VocalForge-0.0.4/pyproject.toml
+-rw-rw-r--   0 rio       (1000) rio       (1000)      312 2023-06-01 02:32:29.000000 VocalForge-0.0.4/requirements.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)       38 2023-06-01 02:33:44.242594 VocalForge-0.0.4/setup.cfg
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/src/
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/src/VocalForge/
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/src/VocalForge/audio/
+-rw-rw-r--   0 rio       (1000) rio       (1000)      204 2023-05-31 00:06:05.000000 VocalForge-0.0.4/src/VocalForge/audio/__init__.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    10276 2023-05-30 05:30:07.000000 VocalForge-0.0.4/src/VocalForge/audio/audio_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4708 2023-05-31 03:13:49.000000 VocalForge-0.0.4/src/VocalForge/audio/export_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     5777 2023-05-31 03:15:02.000000 VocalForge-0.0.4/src/VocalForge/audio/isolate.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2068 2023-05-30 05:32:42.000000 VocalForge-0.0.4/src/VocalForge/audio/overlap.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2386 2023-05-31 00:06:30.000000 VocalForge-0.0.4/src/VocalForge/audio/refine_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     3002 2023-05-30 05:31:11.000000 VocalForge-0.0.4/src/VocalForge/audio/voice_detection.py
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/src/VocalForge/text/
+-rw-rw-r--   0 rio       (1000) rio       (1000)      250 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/__init__.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     3555 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/create_dataset.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2211 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/ctc.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    26284 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/ctc_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1666 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/normalization_helpers.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     4247 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/normalize_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)    10460 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/process_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2442 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/refine_text.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2277 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/segment.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     1759 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/split_audio.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     5407 2023-05-31 04:31:49.000000 VocalForge-0.0.4/src/VocalForge/text/text_utils.py
+-rw-rw-r--   0 rio       (1000) rio       (1000)     2330 2023-05-21 03:39:13.000000 VocalForge-0.0.4/src/VocalForge/text/transcribe.py
+drwxrwxr-x   0 rio       (1000) rio       (1000)        0 2023-06-01 02:33:44.242594 VocalForge-0.0.4/src/VocalForge.egg-info/
+-rw-rw-r--   0 rio       (1000) rio       (1000)     6310 2023-06-01 02:33:44.000000 VocalForge-0.0.4/src/VocalForge.egg-info/PKG-INFO
+-rw-rw-r--   0 rio       (1000) rio       (1000)      906 2023-06-01 02:33:44.000000 VocalForge-0.0.4/src/VocalForge.egg-info/SOURCES.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)        1 2023-06-01 02:33:44.000000 VocalForge-0.0.4/src/VocalForge.egg-info/dependency_links.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)      312 2023-06-01 02:33:44.000000 VocalForge-0.0.4/src/VocalForge.egg-info/requires.txt
+-rw-rw-r--   0 rio       (1000) rio       (1000)       11 2023-06-01 02:33:44.000000 VocalForge-0.0.4/src/VocalForge.egg-info/top_level.txt
```

### Comparing `VocalForge-0.0.3/LICENSE.md` & `VocalForge-0.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/PKG-INFO` & `VocalForge-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VocalForge
-Version: 0.0.3
+Version: 0.0.4
 Summary: Your one-stop solution for voice dataset creation
 Author-email: Rio Harper <rio@rioharper.com>
 Project-URL: Homepage, https://github.com/rioharper/VocalForge/
 Project-URL: Bug Tracker, https://github.com/rioharper/VocalForge/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
```

### Comparing `VocalForge-0.0.3/README.md` & `VocalForge-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/pyproject.toml` & `VocalForge-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 dynamic = ["dependencies"]
 name = "VocalForge"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Rio Harper", email="rio@rioharper.com" },
 ]
 description = "Your one-stop solution for voice dataset creation"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `VocalForge-0.0.3/src/VocalForge/audio/audio_utils.py` & `VocalForge-0.0.4/src/VocalForge/audio/audio_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/audio/export_audio.py` & `VocalForge-0.0.4/src/VocalForge/audio/export_audio.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/audio/isolate.py` & `VocalForge-0.0.4/src/VocalForge/audio/isolate.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/audio/overlap.py` & `VocalForge-0.0.4/src/VocalForge/audio/overlap.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/audio/refine_audio.py` & `VocalForge-0.0.4/src/VocalForge/audio/refine_audio.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/audio/voice_detection.py` & `VocalForge-0.0.4/src/VocalForge/audio/voice_detection.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/create_dataset.py` & `VocalForge-0.0.4/src/VocalForge/text/create_dataset.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/ctc.py` & `VocalForge-0.0.4/src/VocalForge/text/ctc.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/ctc_utils.py` & `VocalForge-0.0.4/src/VocalForge/text/ctc_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/normalization_helpers.py` & `VocalForge-0.0.4/src/VocalForge/text/normalization_helpers.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/normalize_text.py` & `VocalForge-0.0.4/src/VocalForge/text/normalize_text.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/process_text.py` & `VocalForge-0.0.4/src/VocalForge/text/process_text.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/refine_text.py` & `VocalForge-0.0.4/src/VocalForge/text/refine_text.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/segment.py` & `VocalForge-0.0.4/src/VocalForge/text/segment.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/split_audio.py` & `VocalForge-0.0.4/src/VocalForge/text/split_audio.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/text_utils.py` & `VocalForge-0.0.4/src/VocalForge/text/text_utils.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge/text/transcribe.py` & `VocalForge-0.0.4/src/VocalForge/text/transcribe.py`

 * *Files identical despite different names*

### Comparing `VocalForge-0.0.3/src/VocalForge.egg-info/PKG-INFO` & `VocalForge-0.0.4/src/VocalForge.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VocalForge
-Version: 0.0.3
+Version: 0.0.4
 Summary: Your one-stop solution for voice dataset creation
 Author-email: Rio Harper <rio@rioharper.com>
 Project-URL: Homepage, https://github.com/rioharper/VocalForge/
 Project-URL: Bug Tracker, https://github.com/rioharper/VocalForge/issues
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.3
```

### Comparing `VocalForge-0.0.3/src/VocalForge.egg-info/SOURCES.txt` & `VocalForge-0.0.4/src/VocalForge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

