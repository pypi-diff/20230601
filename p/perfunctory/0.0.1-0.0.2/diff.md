# Comparing `tmp/perfunctory-0.0.1.tar.gz` & `tmp/perfunctory-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perfunctory-0.0.1.tar", last modified: Wed May  4 10:18:19 2022, max compression
+gzip compressed data, was "perfunctory-0.0.2.tar", last modified: Thu Jun  1 17:46:52 2023, max compression
```

## Comparing `perfunctory-0.0.1.tar` & `perfunctory-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-05-04 10:18:19.388268 perfunctory-0.0.1/
--rw-rw-rw-   0        0        0     1066 2021-06-14 20:47:04.000000 perfunctory-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      641 2022-05-04 10:18:19.388268 perfunctory-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      143 2021-06-20 18:58:46.000000 perfunctory-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2022-05-04 10:18:19.380272 perfunctory-0.0.1/perfunctory/
--rw-rw-rw-   0        0        0     3914 2022-05-04 10:14:12.000000 perfunctory-0.0.1/perfunctory/Perfunctory.py
--rw-rw-rw-   0        0        0       37 2022-05-04 10:14:25.000000 perfunctory-0.0.1/perfunctory/__init__.py
-drwxrwxrwx   0        0        0        0 2022-05-04 10:18:19.386269 perfunctory-0.0.1/perfunctory.egg-info/
--rw-rw-rw-   0        0        0      641 2022-05-04 10:18:16.000000 perfunctory-0.0.1/perfunctory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2022-05-04 10:18:16.000000 perfunctory-0.0.1/perfunctory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-04 10:18:16.000000 perfunctory-0.0.1/perfunctory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2022-05-04 10:18:16.000000 perfunctory-0.0.1/perfunctory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-04 10:18:19.388268 perfunctory-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      889 2022-05-04 10:15:59.000000 perfunctory-0.0.1/setup.py
+drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:46:52.652437 perfunctory-0.0.2/
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)        4 2023-06-01 17:31:35.000000 perfunctory-0.0.2/LICENSE.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      542 2023-06-01 17:46:52.651824 perfunctory-0.0.2/PKG-INFO
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)       75 2023-06-01 17:32:16.000000 perfunctory-0.0.2/README.md
+drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:46:52.645839 perfunctory-0.0.2/perfunctory/
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:27:18.000000 perfunctory-0.0.2/perfunctory/__init__.py
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)     8204 2023-06-01 17:25:00.000000 perfunctory-0.0.2/perfunctory/rbaa.py
+drwxr-xr-x   0 harpreetsingh   (501) staff       (20)        0 2023-06-01 17:46:52.650824 perfunctory-0.0.2/perfunctory.egg-info/
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      542 2023-06-01 17:46:51.000000 perfunctory-0.0.2/perfunctory.egg-info/PKG-INFO
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      248 2023-06-01 17:46:51.000000 perfunctory-0.0.2/perfunctory.egg-info/SOURCES.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)        1 2023-06-01 17:46:51.000000 perfunctory-0.0.2/perfunctory.egg-info/dependency_links.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)      131 2023-06-01 17:46:51.000000 perfunctory-0.0.2/perfunctory.egg-info/requires.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)       12 2023-06-01 17:46:51.000000 perfunctory-0.0.2/perfunctory.egg-info/top_level.txt
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)       38 2023-06-01 17:46:52.652654 perfunctory-0.0.2/setup.cfg
+-rw-r--r--   0 harpreetsingh   (501) staff       (20)     1052 2023-06-01 17:45:50.000000 perfunctory-0.0.2/setup.py
```

### Comparing `perfunctory-0.0.1/setup.py` & `perfunctory-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
-
-VERSION = '0.0.1'
-DESCRIPTION = "Perfunctory"
-LONG_DESCRIPTION = """Nope"""
-
-# Setting up
-setup(
-    name="perfunctory",
-    version=VERSION,
-    author="(Hank Singh)",
-    author_email="<hanksingh07@gmail.com>",
-    description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    packages=find_packages(),
-    install_requires=[''],
-    keywords=['python'],
-    classifiers=[
-        "Development Status :: 1 - Planning",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: Microsoft :: Windows",
-    ]
-)
+from setuptools import setup, find_packages
+import codecs
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()
+
+VERSION = '0.0.2'
+DESCRIPTION = "perfunctory"
+LONG_DESCRIPTION = """Nope.
+                    """
+
+# Setting up
+setup(
+    name="perfunctory",
+    version=VERSION,
+    author="(Hank Singh)",
+    author_email="<harpreetsingh1811@gmail.com>",
+    description=DESCRIPTION,
+    long_description_content_type="text/markdown",
+    long_description=long_description,
+    packages=find_packages(),
+    install_requires=['numpy', 'pyttsx3', 'pyaudio', 'speedtest-cli', 'pynput', 'SpeechRecognition', 'geocoder', 'googlesearch-python', 'PyDictionary', 'psutil', 'calendar', 'wheel', 'twine' ],
+    keywords=['python'],
+    classifiers=[
+        "Development Status :: 1 - Planning",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: Microsoft :: Windows",
+    ]
+)
```

