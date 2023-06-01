# Comparing `tmp/server-roberta-0.0.1.tar.gz` & `tmp/server-roberta-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "server-roberta-0.0.1.tar", last modified: Thu Jun  1 03:56:09 2023, max compression
+gzip compressed data, was "server-roberta-0.0.2.tar", last modified: Thu Jun  1 04:17:16 2023, max compression
```

## Comparing `server-roberta-0.0.1.tar` & `server-roberta-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 03:56:09.279991 server-roberta-0.0.1/
--rw-rw-rw-   0        0        0    11404 2022-09-13 09:02:44.000000 server-roberta-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2479 2023-06-01 03:56:09.278994 server-roberta-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1873 2022-09-13 09:02:44.000000 server-roberta-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 03:56:09.240099 server-roberta-0.0.1/py/
-drwxrwxrwx   0        0        0        0 2023-06-01 03:56:09.263037 server-roberta-0.0.1/py/serverRoberta/
--rw-rw-rw-   0        0        0        0 2022-09-13 09:02:44.000000 server-roberta-0.0.1/py/serverRoberta/__init__.py
--rw-rw-rw-   0        0        0      108 2022-09-13 09:02:44.000000 server-roberta-0.0.1/py/serverRoberta/datos.py
--rw-rw-rw-   0        0        0     2987 2022-09-13 09:02:44.000000 server-roberta-0.0.1/py/serverRoberta/encrypt.py
--rw-rw-rw-   0        0        0     4021 2022-09-13 09:02:44.000000 server-roberta-0.0.1/py/serverRoberta/robertaModel.py
--rw-rw-rw-   0        0        0     3692 2022-09-13 09:02:44.000000 server-roberta-0.0.1/py/serverRoberta/server.py
--rw-rw-rw-   0        0        0      859 2023-06-01 03:55:51.000000 server-roberta-0.0.1/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-06-01 03:56:09.277995 server-roberta-0.0.1/server_roberta.egg-info/
--rw-rw-rw-   0        0        0     2479 2023-06-01 03:56:09.000000 server-roberta-0.0.1/server_roberta.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-06-01 03:56:09.000000 server-roberta-0.0.1/server_roberta.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 03:56:09.000000 server-roberta-0.0.1/server_roberta.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      148 2023-06-01 03:56:09.000000 server-roberta-0.0.1/server_roberta.egg-info/requires.txt
--rw-rw-rw-   0        0        0        3 2023-06-01 03:56:09.000000 server-roberta-0.0.1/server_roberta.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 03:56:09.280988 server-roberta-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-01 04:17:16.630994 server-roberta-0.0.2/
+-rw-rw-rw-   0        0        0    11404 2022-09-13 09:02:44.000000 server-roberta-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2479 2023-06-01 04:17:16.622016 server-roberta-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1873 2022-09-13 09:02:44.000000 server-roberta-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 04:17:16.459451 server-roberta-0.0.2/py/
+drwxrwxrwx   0        0        0        0 2023-06-01 04:17:16.604065 server-roberta-0.0.2/py/serverRoberta/
+-rw-rw-rw-   0        0        0        0 2022-09-13 09:02:44.000000 server-roberta-0.0.2/py/serverRoberta/__init__.py
+-rw-rw-rw-   0        0        0      108 2022-09-13 09:02:44.000000 server-roberta-0.0.2/py/serverRoberta/datos.py
+-rw-rw-rw-   0        0        0     2987 2022-09-13 09:02:44.000000 server-roberta-0.0.2/py/serverRoberta/encrypt.py
+-rw-rw-rw-   0        0        0     4021 2022-09-13 09:02:44.000000 server-roberta-0.0.2/py/serverRoberta/robertaModel.py
+-rw-rw-rw-   0        0        0     3692 2022-09-13 09:02:44.000000 server-roberta-0.0.2/py/serverRoberta/server.py
+-rw-rw-rw-   0        0        0      852 2023-06-01 04:14:44.000000 server-roberta-0.0.2/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-06-01 04:17:16.620024 server-roberta-0.0.2/server_roberta.egg-info/
+-rw-rw-rw-   0        0        0     2479 2023-06-01 04:17:16.000000 server-roberta-0.0.2/server_roberta.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-06-01 04:17:16.000000 server-roberta-0.0.2/server_roberta.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 04:17:16.000000 server-roberta-0.0.2/server_roberta.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      141 2023-06-01 04:17:16.000000 server-roberta-0.0.2/server_roberta.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        3 2023-06-01 04:17:16.000000 server-roberta-0.0.2/server_roberta.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 04:17:16.631991 server-roberta-0.0.2/setup.cfg
```

### Comparing `server-roberta-0.0.1/LICENSE` & `server-roberta-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.1/PKG-INFO` & `server-roberta-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: server-roberta
-Version: 0.0.1
+Version: 0.0.2
 Summary: To classify, BPE, ROBERTA and SVM are used
 Author-email: Tilsor <tilsor@tilsor.com.uy>
 Project-URL: Homepage, https://github.com/ariverolq/ModSecIntl_roberta_model
 Project-URL: Bug Tracker, https://github.com/ariverolq/ModSecIntl_roberta_model/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `server-roberta-0.0.1/README.md` & `server-roberta-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.1/py/serverRoberta/encrypt.py` & `server-roberta-0.0.2/py/serverRoberta/encrypt.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.1/py/serverRoberta/robertaModel.py` & `server-roberta-0.0.2/py/serverRoberta/robertaModel.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.1/py/serverRoberta/server.py` & `server-roberta-0.0.2/py/serverRoberta/server.py`

 * *Files identical despite different names*

### Comparing `server-roberta-0.0.1/pyproject.toml` & `server-roberta-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 requires = ["setuptools", "setuptools-scm","hatchling"]
 build-backend = ["setuptools.build_meta","hatchling.build"]
 [project]
 name = "server-roberta"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Tilsor", email="tilsor@tilsor.com.uy"},
 ]
 description = "To classify, BPE, ROBERTA and SVM are used"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ['fairseq==0.10.0', 'scipy==1.5.0', 'scikit-learn==0.23.1','pandas==1.3.4','pyparsing==3.0.6','torch==1.10.0','tqdm==4.62.3','wget==3.2','grpcio-tools==1.29.0','requests']
+dependencies = ['fairseq==0.10.0', 'scipy', 'scikit-learn==0.23.1','pandas==1.3.4','pyparsing==3.0.6','torch==1.10.0','tqdm==4.62.3','wget==3.2','grpcio-tools==1.29.0','requests']
 [project.urls]
 "Homepage" = "https://github.com/ariverolq/ModSecIntl_roberta_model"
 "Bug Tracker" = "https://github.com/ariverolq/ModSecIntl_roberta_model/issues"
```

### Comparing `server-roberta-0.0.1/server_roberta.egg-info/PKG-INFO` & `server-roberta-0.0.2/server_roberta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: server-roberta
-Version: 0.0.1
+Version: 0.0.2
 Summary: To classify, BPE, ROBERTA and SVM are used
 Author-email: Tilsor <tilsor@tilsor.com.uy>
 Project-URL: Homepage, https://github.com/ariverolq/ModSecIntl_roberta_model
 Project-URL: Bug Tracker, https://github.com/ariverolq/ModSecIntl_roberta_model/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

