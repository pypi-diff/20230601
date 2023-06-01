# Comparing `tmp/ftsf-0.0.2.1.tar.gz` & `tmp/ftsf-0.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ftsf-0.0.2.1.tar", last modified: Thu Jun  1 20:02:18 2023, max compression
+gzip compressed data, was "ftsf-0.0.2.2.tar", last modified: Thu Jun  1 20:09:04 2023, max compression
```

## Comparing `ftsf-0.0.2.1.tar` & `ftsf-0.0.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:18.500089 ftsf-0.0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-01 20:02:18.500089 ftsf-0.0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:18.496089 ftsf-0.0.2.1/ftsf/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/backtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:18.496089 ftsf-0.0.2.1/ftsf/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/tests/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/tests/test_preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/tests/test_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/ftsf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:02:18.496089 ftsf-0.0.2.1/ftsf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-01 20:02:18.000000 ftsf-0.0.2.1/ftsf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-01 20:02:18.000000 ftsf-0.0.2.1/ftsf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:02:18.000000 ftsf-0.0.2.1/ftsf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 20:02:18.000000 ftsf-0.0.2.1/ftsf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 20:02:18.000000 ftsf-0.0.2.1/ftsf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-01 20:02:04.000000 ftsf-0.0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:02:18.500089 ftsf-0.0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:09:04.353506 ftsf-0.0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-01 20:09:04.353506 ftsf-0.0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:09:04.353506 ftsf-0.0.2.2/ftsf/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/ftsf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/ftsf/backtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7183 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/ftsf/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8442 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/ftsf/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4490 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/ftsf/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/ftsf/scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:09:04.353506 ftsf-0.0.2.2/ftsf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4927 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/ftsf/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/ftsf/tests/test_preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/ftsf/tests/test_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/ftsf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:09:04.353506 ftsf-0.0.2.2/ftsf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-01 20:09:04.000000 ftsf-0.0.2.2/ftsf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-01 20:09:04.000000 ftsf-0.0.2.2/ftsf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:09:04.000000 ftsf-0.0.2.2/ftsf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-01 20:09:04.000000 ftsf-0.0.2.2/ftsf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-01 20:09:04.000000 ftsf-0.0.2.2/ftsf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-01 20:08:43.000000 ftsf-0.0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 20:09:04.353506 ftsf-0.0.2.2/setup.cfg
```

### Comparing `ftsf-0.0.2.1/LICENSE` & `ftsf-0.0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/PKG-INFO` & `ftsf-0.0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftsf
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: Package for financial time series forecasting.
 Author-email: Nikita Safonov <sixxio@yandex.ru>
 Project-URL: Homepage, https://github.com/sixxio/ftsf
 Project-URL: Documentation, https://sixxio.github.io/ftsf/
 Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ftsf-0.0.2.1/README.md` & `ftsf-0.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/ftsf/__init__.py` & `ftsf-0.0.2.2/ftsf/__init__.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/ftsf/backtest.py` & `ftsf-0.0.2.2/ftsf/backtest.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/ftsf/evaluation.py` & `ftsf-0.0.2.2/ftsf/evaluation.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/ftsf/model.py` & `ftsf-0.0.2.2/ftsf/model.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/ftsf/preprocessing.py` & `ftsf-0.0.2.2/ftsf/preprocessing.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/ftsf/scaler.py` & `ftsf-0.0.2.2/ftsf/scaler.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/ftsf/tests/test_evaluation.py` & `ftsf-0.0.2.2/ftsf/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/ftsf/tests/test_preprocessing.py` & `ftsf-0.0.2.2/ftsf/tests/test_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/ftsf/utils.py` & `ftsf-0.0.2.2/ftsf/utils.py`

 * *Files identical despite different names*

### Comparing `ftsf-0.0.2.1/ftsf.egg-info/PKG-INFO` & `ftsf-0.0.2.2/ftsf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ftsf
-Version: 0.0.2.1
+Version: 0.0.2.2
 Summary: Package for financial time series forecasting.
 Author-email: Nikita Safonov <sixxio@yandex.ru>
 Project-URL: Homepage, https://github.com/sixxio/ftsf
 Project-URL: Documentation, https://sixxio.github.io/ftsf/
 Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ftsf-0.0.2.1/pyproject.toml` & `ftsf-0.0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ftsf"
-version = "0.0.2.1"
+version = "0.0.2.2"
 authors = [{ name="Nikita Safonov", email="sixxio@yandex.ru" }]
 description = "Package for financial time series forecasting."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
```

