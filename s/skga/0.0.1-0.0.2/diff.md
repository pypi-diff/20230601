# Comparing `tmp/skga-0.0.1.tar.gz` & `tmp/skga-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skga-0.0.1.tar", last modified: Thu Jun  1 19:32:00 2023, max compression
+gzip compressed data, was "skga-0.0.2.tar", last modified: Thu Jun  1 19:44:22 2023, max compression
```

## Comparing `skga-0.0.1.tar` & `skga-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,28 @@
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:32:00.159832 skga-0.0.1/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.1/LICENSE
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-01 19:32:00.159648 skga-0.0.1/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.1/README.md
--rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.1/pyproject.toml
--rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-01 19:32:00.159916 skga-0.0.1/setup.cfg
--rw-r--r--   0 leosauberman   (501) staff       (20)     2382 2023-06-01 19:31:41.000000 skga-0.0.1/setup.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:32:00.158017 skga-0.0.1/skga/
--rw-r--r--   0 leosauberman   (501) staff       (20)       43 2023-06-01 19:21:11.000000 skga-0.0.1/skga/__init__.py
--rw-r--r--   0 leosauberman   (501) staff       (20)     8183 2023-05-07 22:04:48.000000 skga-0.0.1/skga/adaptee.py
--rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.1/skga/main.py
-drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:32:00.159350 skga-0.0.1/skga.egg-info/
--rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-01 19:32:00.000000 skga-0.0.1/skga.egg-info/PKG-INFO
--rw-r--r--   0 leosauberman   (501) staff       (20)      226 2023-06-01 19:32:00.000000 skga-0.0.1/skga.egg-info/SOURCES.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-01 19:32:00.000000 skga-0.0.1/skga.egg-info/dependency_links.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-01 19:32:00.000000 skga-0.0.1/skga.egg-info/requires.txt
--rw-r--r--   0 leosauberman   (501) staff       (20)        5 2023-06-01 19:32:00.000000 skga-0.0.1/skga.egg-info/top_level.txt
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:44:22.774374 skga-0.0.2/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1517 2023-05-07 22:28:59.000000 skga-0.0.2/LICENSE
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-01 19:44:22.774173 skga-0.0.2/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      623 2023-05-07 22:04:48.000000 skga-0.0.2/README.md
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:44:22.771528 skga-0.0.2/hbrkga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)       69 2023-06-01 19:42:30.000000 skga-0.0.2/hbrkga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2803 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/data_utils.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     7569 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/exploitation_method_BO.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     7803 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/exploitation_method_BO_only_elites.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     3929 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/exploitation_method_random_search.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2866 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/main-BO-only-elites.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2550 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/main-BO.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2560 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/main-randomwalk.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1306 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/nn_decoder_PT.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     5043 2023-05-07 22:04:48.000000 skga-0.0.2/hbrkga/nn_instance_PT.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2126 2023-06-01 19:08:45.000000 skga-0.0.2/pyproject.toml
+-rw-r--r--   0 leosauberman   (501) staff       (20)       38 2023-06-01 19:44:22.774454 skga-0.0.2/setup.cfg
+-rw-r--r--   0 leosauberman   (501) staff       (20)     2392 2023-06-01 19:44:16.000000 skga-0.0.2/setup.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:44:22.772549 skga-0.0.2/skga/
+-rw-r--r--   0 leosauberman   (501) staff       (20)       43 2023-06-01 19:21:11.000000 skga-0.0.2/skga/__init__.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)     8183 2023-05-07 22:04:48.000000 skga-0.0.2/skga/adaptee.py
+-rw-r--r--   0 leosauberman   (501) staff       (20)    10790 2023-05-07 22:04:48.000000 skga-0.0.2/skga/main.py
+drwxr-xr-x   0 leosauberman   (501) staff       (20)        0 2023-06-01 19:44:22.773812 skga-0.0.2/skga.egg-info/
+-rw-r--r--   0 leosauberman   (501) staff       (20)     1361 2023-06-01 19:44:22.000000 skga-0.0.2/skga.egg-info/PKG-INFO
+-rw-r--r--   0 leosauberman   (501) staff       (20)      511 2023-06-01 19:44:22.000000 skga-0.0.2/skga.egg-info/SOURCES.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)        1 2023-06-01 19:44:22.000000 skga-0.0.2/skga.egg-info/dependency_links.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)      850 2023-06-01 19:44:22.000000 skga-0.0.2/skga.egg-info/requires.txt
+-rw-r--r--   0 leosauberman   (501) staff       (20)       12 2023-06-01 19:44:22.000000 skga-0.0.2/skga.egg-info/top_level.txt
```

### Comparing `skga-0.0.1/LICENSE` & `skga-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `skga-0.0.1/PKG-INFO` & `skga-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.1
+Version: 0.0.2
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.1/README.md` & `skga-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `skga-0.0.1/pyproject.toml` & `skga-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skga-0.0.1/setup.py` & `skga-0.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="skga",
-    version="0.0.1",
+    version="0.0.2",
     description="The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/MLRG-CEFET-RJ/skga",
     author="Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra",
     author_email="leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br",
     license="BSD License",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
-    packages=["skga"],
+    packages=["skga", "hbrkga"],
     include_package_data=True,
     install_requires=[
         "bayesian-optimization==1.2.0",
         "bleach==6.0.0",
         "build==0.10.0",
         "certifi==2023.5.7",
         "charset-normalizer==3.1.0",
```

### Comparing `skga-0.0.1/skga/adaptee.py` & `skga-0.0.2/skga/adaptee.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.1/skga/main.py` & `skga-0.0.2/skga/main.py`

 * *Files identical despite different names*

### Comparing `skga-0.0.1/skga.egg-info/PKG-INFO` & `skga-0.0.2/skga.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skga
-Version: 0.0.1
+Version: 0.0.2
 Summary: The python package implementing the HyperBRKGA algorithm optimizes hyperparameters of machine learning algorithms through a hybrid approach based on genetic algorithms.
 Home-page: https://github.com/MLRG-CEFET-RJ/skga
 Author: Leonardo Sauberman, João Pedro Nogueira, Eduardo Bezerra
 Author-email: leonardo.moraes@aluno.cefet-rj.br, joao.carneiro@aluno.cefet-rj.br, ebezerra@cefet-rj.br
 License: BSD License
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `skga-0.0.1/skga.egg-info/requires.txt` & `skga-0.0.2/skga.egg-info/requires.txt`

 * *Files identical despite different names*

