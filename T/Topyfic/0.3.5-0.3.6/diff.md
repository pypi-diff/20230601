# Comparing `tmp/Topyfic-0.3.5.tar.gz` & `tmp/Topyfic-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Topyfic-0.3.5.tar", last modified: Thu Jun  1 17:41:08 2023, max compression
+gzip compressed data, was "Topyfic-0.3.6.tar", last modified: Thu Jun  1 17:45:36 2023, max compression
```

## Comparing `Topyfic-0.3.5.tar` & `Topyfic-0.3.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-06-01 17:41:08.443459 Topyfic-0.3.5/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.3.5/LICENSE.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-06-01 17:41:08.443534 Topyfic-0.3.5/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.3.5/README.md
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-06-01 17:41:08.442407 Topyfic-0.3.5/Topyfic/
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)      199 2023-05-31 23:13:17.000000 Topyfic-0.3.5/Topyfic/__init__.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    44516 2023-05-31 23:01:59.000000 Topyfic-0.3.5/Topyfic/analysis.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     4128 2023-05-31 23:11:38.000000 Topyfic-0.3.5/Topyfic/main.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    13297 2023-05-31 23:11:38.000000 Topyfic-0.3.5/Topyfic/topModel.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     8983 2023-05-31 23:11:38.000000 Topyfic-0.3.5/Topyfic/topic.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10440 2023-05-31 22:59:19.000000 Topyfic-0.3.5/Topyfic/train.py
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-06-01 17:41:08.443326 Topyfic-0.3.5/Topyfic.egg-info/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-06-01 17:41:08.000000 Topyfic-0.3.5/Topyfic.egg-info/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      304 2023-06-01 17:41:08.000000 Topyfic-0.3.5/Topyfic.egg-info/SOURCES.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-06-01 17:41:08.000000 Topyfic-0.3.5/Topyfic.egg-info/dependency_links.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-06-01 17:41:08.000000 Topyfic-0.3.5/Topyfic.egg-info/requires.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-06-01 17:41:08.000000 Topyfic-0.3.5/Topyfic.egg-info/top_level.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-06-01 17:41:08.443805 Topyfic-0.3.5/setup.cfg
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1997 2023-06-01 17:40:16.000000 Topyfic-0.3.5/setup.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-06-01 17:45:36.333154 Topyfic-0.3.6/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.3.6/LICENSE.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-06-01 17:45:36.333241 Topyfic-0.3.6/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.3.6/README.md
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-06-01 17:45:36.331980 Topyfic-0.3.6/Topyfic/
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)      199 2023-06-01 17:44:41.000000 Topyfic-0.3.6/Topyfic/__init__.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    44516 2023-05-31 23:01:59.000000 Topyfic-0.3.6/Topyfic/analysis.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     4128 2023-05-31 23:11:38.000000 Topyfic-0.3.6/Topyfic/main.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    13297 2023-05-31 23:11:38.000000 Topyfic-0.3.6/Topyfic/topModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     8983 2023-05-31 23:11:38.000000 Topyfic-0.3.6/Topyfic/topic.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    10440 2023-05-31 22:59:19.000000 Topyfic-0.3.6/Topyfic/train.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-06-01 17:45:36.332999 Topyfic-0.3.6/Topyfic.egg-info/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-06-01 17:45:36.000000 Topyfic-0.3.6/Topyfic.egg-info/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      304 2023-06-01 17:45:36.000000 Topyfic-0.3.6/Topyfic.egg-info/SOURCES.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-06-01 17:45:36.000000 Topyfic-0.3.6/Topyfic.egg-info/dependency_links.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-06-01 17:45:36.000000 Topyfic-0.3.6/Topyfic.egg-info/requires.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-06-01 17:45:36.000000 Topyfic-0.3.6/Topyfic.egg-info/top_level.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-06-01 17:45:36.333543 Topyfic-0.3.6/setup.cfg
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1997 2023-06-01 17:45:07.000000 Topyfic-0.3.6/setup.py
```

### Comparing `Topyfic-0.3.5/LICENSE.txt` & `Topyfic-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.5/PKG-INFO` & `Topyfic-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.3.5
+Version: 0.3.6
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.5.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.6.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.3.5/README.md` & `Topyfic-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.5/Topyfic/analysis.py` & `Topyfic-0.3.6/Topyfic/analysis.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.5/Topyfic/main.py` & `Topyfic-0.3.6/Topyfic/main.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.5/Topyfic/topModel.py` & `Topyfic-0.3.6/Topyfic/topModel.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.5/Topyfic/topic.py` & `Topyfic-0.3.6/Topyfic/topic.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.5/Topyfic/train.py` & `Topyfic-0.3.6/Topyfic/train.py`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.5/Topyfic.egg-info/PKG-INFO` & `Topyfic-0.3.6/Topyfic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.3.5
+Version: 0.3.6
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.5.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.6.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.3.5/setup.py` & `Topyfic-0.3.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='Topyfic',  # the name of your package
     packages=['Topyfic'],  # same as above
-    version='v0.3.5',  # version number
+    version='v0.3.6',  # version number
     license='MIT',  # license type
     description='Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) '
                 'using leiden clustering and harmony for single cell epigenomics data',
     # short description
     author='Narges Rezaie',  # your name
     author_email='nargesrezaie80@gmail.com',  # your email
     url='https://github.com/mortazavilab/Topyfic',  # url to your git repo
-    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.5.tar.gz',  # link to the tar.gz file associated with this release
+    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.6.tar.gz',  # link to the tar.gz file associated with this release
     keywords=['Cellular Programs', 'Latent Dirichlet allocation', 'single-cell multiome', 'single-cell RNA-seq',
               'gene regulatory network', 'Topic Modeling', 'single-nucleus RNA-seq'],  #
     python_requires='>=3.8',
     install_requires=[  # these can also include >, <, == to enforce version compatibility
         'pandas>=1.4.4',  # make sure the packages you put here are those NOT included in the base python distribution
         'scikit-learn>=0.24.2',
         'pytest',
```

