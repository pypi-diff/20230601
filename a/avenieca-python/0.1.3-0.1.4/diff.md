# Comparing `tmp/avenieca-python-0.1.3.tar.gz` & `tmp/avenieca-python-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avenieca-python-0.1.3.tar", last modified: Thu Jun  1 16:50:35 2023, max compression
+gzip compressed data, was "avenieca-python-0.1.4.tar", last modified: Thu Jun  1 17:06:09 2023, max compression
```

## Comparing `avenieca-python-0.1.3.tar` & `avenieca-python-0.1.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:35.000709 avenieca-python-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-01 16:50:35.000709 avenieca-python-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.992709 avenieca-python-0.1.3/avenieca/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.992709 avenieca-python-0.1.3/avenieca/api/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/cortex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/eca.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/ecaresponse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/ess.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/sequence.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.992709 avenieca-python-0.1.3/avenieca/api/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/api/utils/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.996709 avenieca-python-0.1.3/avenieca/config/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/broker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/cortex.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/document.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/ras.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/retrieval.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/twin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/config/vse.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.996709 avenieca-python-0.1.3/avenieca/producers/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/producers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/producers/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/producers/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.996709 avenieca-python-0.1.3/avenieca/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/utils/hash.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/avenieca/utils/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:34.996709 avenieca-python-0.1.3/avenieca_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-01 16:50:34.000000 avenieca-python-0.1.3/avenieca_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 16:50:34.000000 avenieca-python-0.1.3/avenieca_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:50:34.000000 avenieca-python-0.1.3/avenieca_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 16:50:34.000000 avenieca-python-0.1.3/avenieca_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 16:50:34.000000 avenieca-python-0.1.3/avenieca_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:50:35.000709 avenieca-python-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:50:35.000709 avenieca-python-0.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/test/test_producers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-01 16:50:22.000000 avenieca-python-0.1.3/test/test_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:09.101991 avenieca-python-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-01 17:06:09.097991 avenieca-python-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8632 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:09.093991 avenieca-python-0.1.4/avenieca/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:09.097991 avenieca-python-0.1.4/avenieca/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/cortex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/eca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/ecaresponse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3319 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/ess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/sequence.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:09.097991 avenieca-python-0.1.4/avenieca/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/api/utils/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:09.097991 avenieca-python-0.1.4/avenieca/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/broker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/cortex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/ras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/retrieval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/twin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/config/vse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:09.097991 avenieca-python-0.1.4/avenieca/producers/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/producers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/producers/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/producers/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:09.097991 avenieca-python-0.1.4/avenieca/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/utils/hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/avenieca/utils/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:09.097991 avenieca-python-0.1.4/avenieca_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-06-01 17:06:09.000000 avenieca-python-0.1.4/avenieca_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 17:06:09.000000 avenieca-python-0.1.4/avenieca_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:06:09.000000 avenieca-python-0.1.4/avenieca_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 17:06:09.000000 avenieca-python-0.1.4/avenieca_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-01 17:06:09.000000 avenieca-python-0.1.4/avenieca_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 17:06:09.101991 avenieca-python-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:06:09.097991 avenieca-python-0.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/test/test_producers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-01 17:05:56.000000 avenieca-python-0.1.4/test/test_signal.py
```

### Comparing `avenieca-python-0.1.3/LICENSE` & `avenieca-python-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/PKG-INFO` & `avenieca-python-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avenieca-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python SDK for AveniECA
 Home-page: https://github.com/aveni-hub/avenieca-python
 Author: Ogban Ugot
 Author-email: ogbanugot@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `avenieca-python-0.1.3/README.md` & `avenieca-python-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/auth.py` & `avenieca-python-0.1.4/avenieca/api/auth.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/client.py` & `avenieca-python-0.1.4/avenieca/api/client.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/cortex.py` & `avenieca-python-0.1.4/avenieca/api/cortex.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/document.py` & `avenieca-python-0.1.4/avenieca/api/document.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/eca.py` & `avenieca-python-0.1.4/avenieca/api/eca.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/ecaresponse.py` & `avenieca-python-0.1.4/avenieca/api/ecaresponse.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/embedding.py` & `avenieca-python-0.1.4/avenieca/api/embedding.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/ess.py` & `avenieca-python-0.1.4/avenieca/api/ess.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/model.py` & `avenieca-python-0.1.4/avenieca/api/model.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/retrieval.py` & `avenieca-python-0.1.4/avenieca/api/retrieval.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/api/sequence.py` & `avenieca-python-0.1.4/avenieca/api/sequence.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/config/cortex.py` & `avenieca-python-0.1.4/avenieca/config/cortex.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/config/document.py` & `avenieca-python-0.1.4/avenieca/config/document.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/config/retrieval.py` & `avenieca-python-0.1.4/avenieca/config/retrieval.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/config/server.py` & `avenieca-python-0.1.4/avenieca/config/server.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/config/twin.py` & `avenieca-python-0.1.4/avenieca/config/twin.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/config/vse.py` & `avenieca-python-0.1.4/avenieca/config/vse.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/consumer.py` & `avenieca-python-0.1.4/avenieca/consumer.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/data.py` & `avenieca-python-0.1.4/avenieca/data.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/producer.py` & `avenieca-python-0.1.4/avenieca/producer.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/producers/event.py` & `avenieca-python-0.1.4/avenieca/producers/event.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/producers/stream.py` & `avenieca-python-0.1.4/avenieca/producers/stream.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/utils/hash.py` & `avenieca-python-0.1.4/avenieca/utils/hash.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca/utils/signal.py` & `avenieca-python-0.1.4/avenieca/utils/signal.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/avenieca_python.egg-info/PKG-INFO` & `avenieca-python-0.1.4/avenieca_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avenieca-python
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python SDK for AveniECA
 Home-page: https://github.com/aveni-hub/avenieca-python
 Author: Ogban Ugot
 Author-email: ogbanugot@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python
```

### Comparing `avenieca-python-0.1.3/avenieca_python.egg-info/SOURCES.txt` & `avenieca-python-0.1.4/avenieca_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/setup.py` & `avenieca-python-0.1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # The text of the README file is used as a description
 README = (HERE / "README.md").read_text()
 
 # This call to set up() does all the work
 setup(
     name="avenieca-python",
-    version="0.1.3",
+    version="0.1.4",
     description="Python SDK for AveniECA",
     url="https://github.com/aveni-hub/avenieca-python",
     long_description=README,
     long_description_content_type="text/markdown",
     author="Ogban Ugot",
     author_email="ogbanugot@gmail.com",
     license="MIT",
```

### Comparing `avenieca-python-0.1.3/test/test_producers.py` & `avenieca-python-0.1.4/test/test_producers.py`

 * *Files identical despite different names*

### Comparing `avenieca-python-0.1.3/test/test_signal.py` & `avenieca-python-0.1.4/test/test_signal.py`

 * *Files identical despite different names*

