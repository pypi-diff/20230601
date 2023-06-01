# Comparing `tmp/server-roberta-0.0.3.tar.gz` & `tmp/server-roberta-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server-roberta-0.0.3.tar", last modified: Thu Jun  1 04:21:57 2023, max compression
+gzip compressed data, was "server-roberta-0.0.4.tar", last modified: Thu Jun  1 01:46:35 2023, max compression
```

## Comparing `server-roberta-0.0.3.tar` & `server-roberta-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 04:21:57.099240 server-roberta-0.0.3/
--rw-rw-rw-   0        0        0    11404 2022-09-13 09:02:44.000000 server-roberta-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     2479 2023-06-01 04:21:57.098242 server-roberta-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1873 2022-09-13 09:02:44.000000 server-roberta-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 04:21:57.035383 server-roberta-0.0.3/py/
-drwxrwxrwx   0        0        0        0 2023-06-01 04:21:57.081287 server-roberta-0.0.3/py/serverRoberta/
--rw-rw-rw-   0        0        0        0 2022-09-13 09:02:44.000000 server-roberta-0.0.3/py/serverRoberta/__init__.py
--rw-rw-rw-   0        0        0      108 2022-09-13 09:02:44.000000 server-roberta-0.0.3/py/serverRoberta/datos.py
--rw-rw-rw-   0        0        0     2987 2022-09-13 09:02:44.000000 server-roberta-0.0.3/py/serverRoberta/encrypt.py
--rw-rw-rw-   0        0        0     4021 2022-09-13 09:02:44.000000 server-roberta-0.0.3/py/serverRoberta/robertaModel.py
--rw-rw-rw-   0        0        0     3692 2022-09-13 09:02:44.000000 server-roberta-0.0.3/py/serverRoberta/server.py
--rw-rw-rw-   0        0        0      801 2023-06-01 04:21:35.000000 server-roberta-0.0.3/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-01 04:21:57.097245 server-roberta-0.0.3/server_roberta.egg-info/
--rw-rw-rw-   0        0        0     2479 2023-06-01 04:21:57.000000 server-roberta-0.0.3/server_roberta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-06-01 04:21:57.000000 server-roberta-0.0.3/server_roberta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 04:21:57.000000 server-roberta-0.0.3/server_roberta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-01 04:21:57.000000 server-roberta-0.0.3/server_roberta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-06-01 04:21:57.000000 server-roberta-0.0.3/server_roberta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 04:21:57.099240 server-roberta-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 01:46:35.909309 server-roberta-0.0.4/
+-rw-rw-rw-   0        0        0    11404 2022-09-13 09:02:44.000000 server-roberta-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     2479 2023-06-01 01:46:35.898034 server-roberta-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1873 2022-09-13 09:02:44.000000 server-roberta-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 01:46:35.877088 server-roberta-0.0.4/py/
+drwxrwxrwx   0        0        0        0 2023-06-01 01:46:35.888068 server-roberta-0.0.4/py/serverRoberta/
+-rw-rw-rw-   0        0        0      112 2023-06-01 01:41:50.000000 server-roberta-0.0.4/py/serverRoberta/__init__.py
+-rw-rw-rw-   0        0        0      108 2022-09-13 09:02:44.000000 server-roberta-0.0.4/py/serverRoberta/datos.py
+-rw-rw-rw-   0        0        0     2987 2022-09-13 09:02:44.000000 server-roberta-0.0.4/py/serverRoberta/encrypt.py
+-rw-rw-rw-   0        0        0     4021 2022-09-13 09:02:44.000000 server-roberta-0.0.4/py/serverRoberta/robertaModel.py
+-rw-rw-rw-   0        0        0     3692 2022-09-13 09:02:44.000000 server-roberta-0.0.4/py/serverRoberta/server.py
+-rw-rw-rw-   0        0        0      801 2023-06-01 01:45:40.000000 server-roberta-0.0.4/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-01 01:46:35.897037 server-roberta-0.0.4/server_roberta.egg-info/
+-rw-rw-rw-   0        0        0     2479 2023-06-01 01:46:35.000000 server-roberta-0.0.4/server_roberta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-06-01 01:46:35.000000 server-roberta-0.0.4/server_roberta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 01:46:35.000000 server-roberta-0.0.4/server_roberta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-01 01:46:35.000000 server-roberta-0.0.4/server_roberta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-06-01 01:46:35.000000 server-roberta-0.0.4/server_roberta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 01:46:35.909309 server-roberta-0.0.4/setup.cfg
```

### Comparing `server-roberta-0.0.3/LICENSE` & `server-roberta-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.3/PKG-INFO` & `server-roberta-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: server-roberta
-Version: 0.0.3
+Version: 0.0.4
 Summary: To classify, BPE, ROBERTA and SVM are used
 Author-email: Tilsor <tilsor@tilsor.com.uy>
 Project-URL: Homepage, https://github.com/ariverolq/ModSecIntl_roberta_model
 Project-URL: Bug Tracker, https://github.com/ariverolq/ModSecIntl_roberta_model/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `server-roberta-0.0.3/README.md` & `server-roberta-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.3/py/serverRoberta/encrypt.py` & `server-roberta-0.0.4/py/serverRoberta/encrypt.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.3/py/serverRoberta/robertaModel.py` & `server-roberta-0.0.4/py/serverRoberta/robertaModel.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.3/py/serverRoberta/server.py` & `server-roberta-0.0.4/py/serverRoberta/server.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.3/pyproject.toml` & `server-roberta-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 requires = ["setuptools", "setuptools-scm","hatchling"]
 build-backend = ["setuptools.build_meta","hatchling.build"]
 [project]
 name = "server-roberta"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Tilsor", email="tilsor@tilsor.com.uy"},
 ]
 description = "To classify, BPE, ROBERTA and SVM are used"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `server-roberta-0.0.3/server_roberta.egg-info/PKG-INFO` & `server-roberta-0.0.4/server_roberta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: server-roberta
-Version: 0.0.3
+Version: 0.0.4
 Summary: To classify, BPE, ROBERTA and SVM are used
 Author-email: Tilsor <tilsor@tilsor.com.uy>
 Project-URL: Homepage, https://github.com/ariverolq/ModSecIntl_roberta_model
 Project-URL: Bug Tracker, https://github.com/ariverolq/ModSecIntl_roberta_model/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

