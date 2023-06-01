# Comparing `tmp/pulsectl-asyncio-1.1.0.tar.gz` & `tmp/pulsectl-asyncio-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsectl-asyncio-1.1.0.tar", last modified: Sun May  7 20:25:20 2023, max compression
+gzip compressed data, was "pulsectl-asyncio-1.1.1.tar", last modified: Thu Jun  1 18:11:23 2023, max compression
```

## Comparing `pulsectl-asyncio-1.1.0.tar` & `pulsectl-asyncio-1.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:25:20.016627 pulsectl-asyncio-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-07 20:25:20.016627 pulsectl-asyncio-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:25:20.012627 pulsectl-asyncio-1.1.0/pulsectl_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio/pa_asyncio_mainloop.py
--rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio/pulsectl_async.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:25:20.012627 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-07 20:25:20.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-07 20:25:20.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 20:25:20.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-07 20:25:20.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-07 20:25:20.000000 pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-07 20:25:20.016627 pulsectl-asyncio-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 20:25:20.016627 pulsectl-asyncio-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/tests/test_async_with_dummy_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-07 20:25:06.000000 pulsectl-asyncio-1.1.0/tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7846 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/pulsectl_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio/pa_asyncio_mainloop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27164 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio/pulsectl_async.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-06-01 18:11:23.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-01 18:11:23.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:11:23.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 18:11:23.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-01 18:11:23.000000 pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:11:23.899489 pulsectl-asyncio-1.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    20261 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/tests/test_async_with_dummy_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-01 18:11:12.000000 pulsectl-asyncio-1.1.1/tests/test_examples.py
```

### Comparing `pulsectl-asyncio-1.1.0/LICENSE` & `pulsectl-asyncio-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.1.0/PKG-INFO` & `pulsectl-asyncio-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsectl-asyncio
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asyncio frontend for the pulsectl Python bindings of libpulse
 Home-page: https://github.com/mhthies/pulsectl-asyncio
 Author: Michael Thies
 Author-email: mail@mhthies.de
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pulsectl-asyncio-1.1.0/README.md` & `pulsectl-asyncio-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.1.0/pulsectl_asyncio/pa_asyncio_mainloop.py` & `pulsectl-asyncio-1.1.1/pulsectl_asyncio/pa_asyncio_mainloop.py`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.1.0/pulsectl_asyncio/pulsectl_async.py` & `pulsectl-asyncio-1.1.1/pulsectl_asyncio/pulsectl_async.py`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.1.0/pulsectl_asyncio.egg-info/PKG-INFO` & `pulsectl-asyncio-1.1.1/pulsectl_asyncio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsectl-asyncio
-Version: 1.1.0
+Version: 1.1.1
 Summary: Asyncio frontend for the pulsectl Python bindings of libpulse
 Home-page: https://github.com/mhthies/pulsectl-asyncio
 Author: Michael Thies
 Author-email: mail@mhthies.de
 License: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `pulsectl-asyncio-1.1.0/setup.cfg` & `pulsectl-asyncio-1.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pulsectl-asyncio
-version = 1.1.0
+version = 1.1.1
 url = https://github.com/mhthies/pulsectl-asyncio
 author = Michael Thies
 author_email = mail@mhthies.de
 description = Asyncio frontend for the pulsectl Python bindings of libpulse
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
@@ -23,14 +23,14 @@
 	Operating System :: POSIX
 	Development Status :: 5 - Production/Stable
 
 [options]
 packages = pulsectl_asyncio
 python_requires = >=3.6
 install_requires = 
-	pulsectl >=22.5.0,<=22.5.1
+	pulsectl >=23.5.0,<=23.5.2
 include_package_data = True
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `pulsectl-asyncio-1.1.0/tests/test_async_with_dummy_instance.py` & `pulsectl-asyncio-1.1.1/tests/test_async_with_dummy_instance.py`

 * *Files identical despite different names*

### Comparing `pulsectl-asyncio-1.1.0/tests/test_examples.py` & `pulsectl-asyncio-1.1.1/tests/test_examples.py`

 * *Files identical despite different names*

