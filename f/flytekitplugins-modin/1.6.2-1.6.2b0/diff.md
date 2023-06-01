# Comparing `tmp/flytekitplugins-modin-1.6.2.tar.gz` & `tmp/flytekitplugins-modin-1.6.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-modin-1.6.2.tar", last modified: Tue May 30 15:24:19 2023, max compression
+gzip compressed data, was "flytekitplugins-modin-1.6.2b0.tar", last modified: Thu Jun  1 20:41:57 2023, max compression
```

## Comparing `flytekitplugins-modin-1.6.2.tar` & `flytekitplugins-modin-1.6.2b0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:19.225503 flytekitplugins-modin-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-30 15:24:19.225503 flytekitplugins-modin-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-30 15:23:56.000000 flytekitplugins-modin-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:19.225503 flytekitplugins-modin-1.6.2/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:19.225503 flytekitplugins-modin-1.6.2/flytekitplugins/modin/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-30 15:23:56.000000 flytekitplugins-modin-1.6.2/flytekitplugins/modin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-05-30 15:23:56.000000 flytekitplugins-modin-1.6.2/flytekitplugins/modin/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:24:19.225503 flytekitplugins-modin-1.6.2/flytekitplugins_modin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-30 15:24:19.000000 flytekitplugins-modin-1.6.2/flytekitplugins_modin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-30 15:24:19.000000 flytekitplugins-modin-1.6.2/flytekitplugins_modin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:24:19.000000 flytekitplugins-modin-1.6.2/flytekitplugins_modin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:24:19.000000 flytekitplugins-modin-1.6.2/flytekitplugins_modin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-30 15:24:19.000000 flytekitplugins-modin-1.6.2/flytekitplugins_modin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 15:24:19.000000 flytekitplugins-modin-1.6.2/flytekitplugins_modin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:24:19.225503 flytekitplugins-modin-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-30 15:24:12.000000 flytekitplugins-modin-1.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:57.791866 flytekitplugins-modin-1.6.2b0/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-01 20:41:57.791866 flytekitplugins-modin-1.6.2b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-01 20:41:31.000000 flytekitplugins-modin-1.6.2b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:57.791866 flytekitplugins-modin-1.6.2b0/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:57.791866 flytekitplugins-modin-1.6.2b0/flytekitplugins/modin/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-01 20:41:31.000000 flytekitplugins-modin-1.6.2b0/flytekitplugins/modin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4074 2023-06-01 20:41:31.000000 flytekitplugins-modin-1.6.2b0/flytekitplugins/modin/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:41:57.791866 flytekitplugins-modin-1.6.2b0/flytekitplugins_modin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-01 20:41:57.000000 flytekitplugins-modin-1.6.2b0/flytekitplugins_modin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-01 20:41:57.000000 flytekitplugins-modin-1.6.2b0/flytekitplugins_modin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:41:57.000000 flytekitplugins-modin-1.6.2b0/flytekitplugins_modin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:57.000000 flytekitplugins-modin-1.6.2b0/flytekitplugins_modin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 20:41:57.000000 flytekitplugins-modin-1.6.2b0/flytekitplugins_modin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:41:57.000000 flytekitplugins-modin-1.6.2b0/flytekitplugins_modin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:41:57.791866 flytekitplugins-modin-1.6.2b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-06-01 20:41:50.000000 flytekitplugins-modin-1.6.2b0/setup.py
```

### Comparing `flytekitplugins-modin-1.6.2/PKG-INFO` & `flytekitplugins-modin-1.6.2b0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-modin
-Version: 1.6.2
+Version: 1.6.2b0
 Summary: Modin plugin for flytekit
 Author: Intel
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-modin-1.6.2/README.md` & `flytekitplugins-modin-1.6.2b0/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-modin-1.6.2/flytekitplugins/modin/schema.py` & `flytekitplugins-modin-1.6.2b0/flytekitplugins/modin/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-modin-1.6.2/flytekitplugins_modin.egg-info/PKG-INFO` & `flytekitplugins-modin-1.6.2b0/flytekitplugins_modin.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-modin
-Version: 1.6.2
+Version: 1.6.2b0
 Summary: Modin plugin for flytekit
 Author: Intel
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-modin-1.6.2/setup.py` & `flytekitplugins-modin-1.6.2b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plugin_requires = [
     "flytekit<1.3.0b2,<2.0.0",
     "modin>=0.13.0",
     "fsspec",
     "ray",
 ]
 
-__version__ = "1.6.2"
+__version__ = "1.6.2b0"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Intel",
     description="Modin plugin for flytekit",
     namespace_packages=["flytekitplugins"],
```

