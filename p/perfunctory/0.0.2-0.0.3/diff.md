# Comparing `tmp/perfunctory-0.0.2.tar.gz` & `tmp/perfunctory-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfunctory-0.0.2.tar", last modified: Thu Jun  1 17:46:52 2023, max compression
+gzip compressed data, was "perfunctory-0.0.3.tar", last modified: Thu Jun  1 17:56:00 2023, max compression
```

## Comparing `perfunctory-0.0.2.tar` & `perfunctory-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:46:52.652437 perfunctory-0.0.2/
--rw-r--r--   0 harpreetsingh   (501) staff       (20)        4 2023-06-01 17:31:35.000000 perfunctory-0.0.2/LICENSE.txt
--rw-r--r--   0 harpreetsingh   (501) staff       (20)      542 2023-06-01 17:46:52.651824 perfunctory-0.0.2/PKG-INFO
--rw-r--r--   0 harpreetsingh   (501) staff       (20)       75 2023-06-01 17:32:16.000000 perfunctory-0.0.2/README.md
-drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:46:52.645839 perfunctory-0.0.2/perfunctory/
--rw-r--r--   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:27:18.000000 perfunctory-0.0.2/perfunctory/__init__.py
--rw-r--r--   0 harpreetsingh   (501) staff       (20)     8204 2023-06-01 17:25:00.000000 perfunctory-0.0.2/perfunctory/rbaa.py
-drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:46:52.650824 perfunctory-0.0.2/perfunctory.egg-info/
--rw-r--r--   0 harpreetsingh   (501) staff       (20)      542 2023-06-01 17:46:51.000000 perfunctory-0.0.2/perfunctory.egg-info/PKG-INFO
--rw-r--r--   0 harpreetsingh   (501) staff       (20)      248 2023-06-01 17:46:51.000000 perfunctory-0.0.2/perfunctory.egg-info/SOURCES.txt
--rw-r--r--   0 harpreetsingh   (501) staff       (20)        1 2023-06-01 17:46:51.000000 perfunctory-0.0.2/perfunctory.egg-info/dependency_links.txt
--rw-r--r--   0 harpreetsingh   (501) staff       (20)      131 2023-06-01 17:46:51.000000 perfunctory-0.0.2/perfunctory.egg-info/requires.txt
--rw-r--r--   0 harpreetsingh   (501) staff       (20)       12 2023-06-01 17:46:51.000000 perfunctory-0.0.2/perfunctory.egg-info/top_level.txt
--rw-r--r--   0 harpreetsingh   (501) staff       (20)       38 2023-06-01 17:46:52.652654 perfunctory-0.0.2/setup.cfg
--rw-r--r--   0 harpreetsingh   (501) staff       (20)     1052 2023-06-01 17:45:50.000000 perfunctory-0.0.2/setup.py
+drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:56:00.544544 perfunctory-0.0.3/
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)        4 2023-06-01 17:31:35.000000 perfunctory-0.0.3/LICENSE.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      542 2023-06-01 17:56:00.544048 perfunctory-0.0.3/PKG-INFO
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)       75 2023-06-01 17:32:16.000000 perfunctory-0.0.3/README.md
+drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:56:00.539790 perfunctory-0.0.3/perfunctory/
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:27:18.000000 perfunctory-0.0.3/perfunctory/__init__.py
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)     8204 2023-06-01 17:25:00.000000 perfunctory-0.0.3/perfunctory/rbaa.py
+drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:56:00.543170 perfunctory-0.0.3/perfunctory.egg-info/
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      542 2023-06-01 17:56:00.000000 perfunctory-0.0.3/perfunctory.egg-info/PKG-INFO
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      248 2023-06-01 17:56:00.000000 perfunctory-0.0.3/perfunctory.egg-info/SOURCES.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)        1 2023-06-01 17:56:00.000000 perfunctory-0.0.3/perfunctory.egg-info/dependency_links.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      122 2023-06-01 17:56:00.000000 perfunctory-0.0.3/perfunctory.egg-info/requires.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)       12 2023-06-01 17:56:00.000000 perfunctory-0.0.3/perfunctory.egg-info/top_level.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)       38 2023-06-01 17:56:00.544791 perfunctory-0.0.3/setup.cfg
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)     1040 2023-06-01 17:55:36.000000 perfunctory-0.0.3/setup.py
```

### Comparing `perfunctory-0.0.2/PKG-INFO` & `perfunctory-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfunctory
-Version: 0.0.2
+Version: 0.0.3
 Summary: perfunctory
 Home-page: UNKNOWN
 Author: (Hank Singh)
 Author-email: <harpreetsingh1811@gmail.com>
 License: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `perfunctory-0.0.2/perfunctory/rbaa.py` & `perfunctory-0.0.3/perfunctory/rbaa.py`

 * *Files identical despite different names*

### Comparing `perfunctory-0.0.2/perfunctory.egg-info/PKG-INFO` & `perfunctory-0.0.3/perfunctory.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perfunctory
-Version: 0.0.2
+Version: 0.0.3
 Summary: perfunctory
 Home-page: UNKNOWN
 Author: (Hank Singh)
 Author-email: <harpreetsingh1811@gmail.com>
 License: UNKNOWN
 Keywords: python
 Platform: UNKNOWN
```

### Comparing `perfunctory-0.0.2/setup.py` & `perfunctory-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = "perfunctory"
 LONG_DESCRIPTION = """Nope.
                     """
 
 # Setting up
 setup(
     name="perfunctory",
     version=VERSION,
     author="(Hank Singh)",
     author_email="<harpreetsingh1811@gmail.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['numpy', 'pyttsx3', 'pyaudio', 'speedtest-cli', 'pynput', 'SpeechRecognition', 'geocoder', 'googlesearch-python', 'PyDictionary', 'psutil', 'calendar', 'wheel', 'twine' ],
+    install_requires=['numpy', 'pyttsx3', 'pyaudio', 'speedtest-cli', 'pynput', 'SpeechRecognition', 'geocoder', 'googlesearch-python', 'PyDictionary', 'psutil', 'wheel', 'twine' ],
     keywords=['python'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: Microsoft :: Windows",
     ]
```

