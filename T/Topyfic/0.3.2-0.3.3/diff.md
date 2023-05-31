# Comparing `tmp/Topyfic-0.3.2.tar.gz` & `tmp/Topyfic-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Topyfic-0.3.2.tar", last modified: Wed May 31 22:42:22 2023, max compression
+gzip compressed data, was "Topyfic-0.3.3.tar", last modified: Wed May 31 23:14:43 2023, max compression
```

## Comparing `Topyfic-0.3.2.tar` & `Topyfic-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-31 22:42:22.640323 Topyfic-0.3.2/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.3.2/LICENSE.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-05-31 22:42:22.640396 Topyfic-0.3.2/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.3.2/README.md
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-31 22:42:22.638986 Topyfic-0.3.2/Topyfic/
--rw-rw-r--   0 nargesrezaie   (501) staff       (20)      148 2023-05-31 22:39:08.000000 Topyfic-0.3.2/Topyfic/__init__.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    44549 2023-04-26 18:27:24.000000 Topyfic-0.3.2/Topyfic/analysis.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     4115 2022-12-08 00:57:41.000000 Topyfic-0.3.2/Topyfic/main.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    13356 2023-05-31 22:19:13.000000 Topyfic-0.3.2/Topyfic/topModel.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     9141 2023-05-31 22:19:13.000000 Topyfic-0.3.2/Topyfic/topic.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    10433 2023-05-31 22:40:14.000000 Topyfic-0.3.2/Topyfic/train.py
--rw-r--r--   0 nargesrezaie   (501) staff       (20)    37663 2023-05-31 22:40:14.000000 Topyfic-0.3.2/Topyfic/utils.py
-drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-31 22:42:22.640188 Topyfic-0.3.2/Topyfic.egg-info/
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-05-31 22:42:22.000000 Topyfic-0.3.2/Topyfic.egg-info/PKG-INFO
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      321 2023-05-31 22:42:22.000000 Topyfic-0.3.2/Topyfic.egg-info/SOURCES.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-05-31 22:42:22.000000 Topyfic-0.3.2/Topyfic.egg-info/dependency_links.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-05-31 22:42:22.000000 Topyfic-0.3.2/Topyfic.egg-info/requires.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-05-31 22:42:22.000000 Topyfic-0.3.2/Topyfic.egg-info/top_level.txt
--rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-05-31 22:42:22.640677 Topyfic-0.3.2/setup.cfg
--rw-r--r--   0 nargesrezaie   (501) staff       (20)     1997 2023-05-31 22:41:46.000000 Topyfic-0.3.2/setup.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-31 23:14:43.803700 Topyfic-0.3.3/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1067 2022-01-27 20:57:46.000000 Topyfic-0.3.3/LICENSE.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-05-31 23:14:43.803768 Topyfic-0.3.3/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     3280 2023-04-27 22:47:11.000000 Topyfic-0.3.3/README.md
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-31 23:14:43.802534 Topyfic-0.3.3/Topyfic/
+-rw-rw-r--   0 nargesrezaie   (501) staff       (20)      199 2023-05-31 23:13:17.000000 Topyfic-0.3.3/Topyfic/__init__.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    44516 2023-05-31 23:01:59.000000 Topyfic-0.3.3/Topyfic/analysis.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     4128 2023-05-31 23:11:38.000000 Topyfic-0.3.3/Topyfic/main.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    13297 2023-05-31 23:11:38.000000 Topyfic-0.3.3/Topyfic/topModel.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     8983 2023-05-31 23:11:38.000000 Topyfic-0.3.3/Topyfic/topic.py
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)    10440 2023-05-31 22:59:19.000000 Topyfic-0.3.3/Topyfic/train.py
+drwxr-xr-x   0 nargesrezaie   (501) staff       (20)        0 2023-05-31 23:14:43.803560 Topyfic-0.3.3/Topyfic.egg-info/
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      903 2023-05-31 23:14:43.000000 Topyfic-0.3.3/Topyfic.egg-info/PKG-INFO
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      304 2023-05-31 23:14:43.000000 Topyfic-0.3.3/Topyfic.egg-info/SOURCES.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        1 2023-05-31 23:14:43.000000 Topyfic-0.3.3/Topyfic.egg-info/dependency_links.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)      269 2023-05-31 23:14:43.000000 Topyfic-0.3.3/Topyfic.egg-info/requires.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)        8 2023-05-31 23:14:43.000000 Topyfic-0.3.3/Topyfic.egg-info/top_level.txt
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)       79 2023-05-31 23:14:43.804045 Topyfic-0.3.3/setup.cfg
+-rw-r--r--   0 nargesrezaie   (501) staff       (20)     1997 2023-05-31 23:14:12.000000 Topyfic-0.3.3/setup.py
```

### Comparing `Topyfic-0.3.2/LICENSE.txt` & `Topyfic-0.3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.2/PKG-INFO` & `Topyfic-0.3.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.3.2
+Version: 0.3.3
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.2.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.3.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.3.2/README.md` & `Topyfic-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `Topyfic-0.3.2/Topyfic/analysis.py` & `Topyfic-0.3.3/Topyfic/analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import pandas as pd
 import numpy as np
 import anndata
 import sys
 from scipy import stats
 import warnings
 import random
-from statsmodels.stats.multitest import fdrcorrection
+import pickle
 from scipy.cluster.hierarchy import ward, dendrogram, leaves_list
 
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpatches
 import seaborn as sns
 
-from Topyfic.topModel import *
+from Topyfic.topModel import TopModel
 
 sns.set_context('paper')
 warnings.filterwarnings('ignore')
 
 
 class Analysis:
     """
```

### Comparing `Topyfic-0.3.2/Topyfic/main.py` & `Topyfic-0.3.3/Topyfic/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import click
-from Topyfic.utils import *
+from Topyfic.utils.analyseModel import *
 
 
 @click.group()
 def cli():
     pass
```

### Comparing `Topyfic-0.3.2/Topyfic/topModel.py` & `Topyfic-0.3.3/Topyfic/topModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import sys
 import warnings
 import joblib
 import pickle
 import numpy as np
 import pandas as pd
-from sklearn.decomposition import LatentDirichletAllocation
 import matplotlib.pyplot as plt
 import seaborn as sns
-from scipy import stats
 
 sns.set_context('paper')
 warnings.filterwarnings('ignore')
 
-from Topyfic.topic import *
-from utils import MA_plot
+from Topyfic.topic import Topic
+from Topyfic.utils.analyseModel import MA_plot
 
 
 class TopModel:
     """
     A class that saved a model
 
     :param name: name of class
```

### Comparing `Topyfic-0.3.2/Topyfic/topic.py` & `Topyfic-0.3.3/Topyfic/topic.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,20 @@
 import sys
 import warnings
-import joblib
 import pandas as pd
-import numpy as np
 import yaml
 from yaml.loader import SafeLoader
 
-import gseapy as gp
-from gseapy.plot import dotplot
-from gseapy import gseaplot
-from reactome2py import analysis
-
-import matplotlib.pyplot as plt
 import seaborn as sns
 
 sns.set_context('paper')
 
 warnings.filterwarnings('ignore')
 
-from utils import GSEA, functional_enrichment_analysis
+from Topyfic.utils.analyseModel import GSEA, functional_enrichment_analysis
 
 
 class Topic:
     """
     A class saved topic along with other useful information
 
     :param topic_id: ID of topic which is unique
```

### Comparing `Topyfic-0.3.2/Topyfic/train.py` & `Topyfic-0.3.3/Topyfic/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import joblib
 import os
 from multiprocessing import Pool
 from itertools import repeat
 import pickle
 from sklearn.decomposition import LatentDirichletAllocation
 
-from Topyfic.topModel import *
+from Topyfic.topModel import TopModel
 
 warnings.filterwarnings("ignore")
 
 
 class Train:
     """
     A class used to train reproducible latent dirichlet allocation (rLDA) model
```

### Comparing `Topyfic-0.3.2/Topyfic.egg-info/PKG-INFO` & `Topyfic-0.3.3/Topyfic.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Topyfic
-Version: 0.3.2
+Version: 0.3.3
 Summary: Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) using leiden clustering and harmony for single cell epigenomics data
 Home-page: https://github.com/mortazavilab/Topyfic
-Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.2.tar.gz
+Download-URL: https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.3.tar.gz
 Author: Narges Rezaie
 Author-email: nargesrezaie80@gmail.com
 License: MIT
 Keywords: Cellular Programs,Latent Dirichlet allocation,single-cell multiome,single-cell RNA-seq,gene regulatory network,Topic Modeling,single-nucleus RNA-seq
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research 
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
```

### Comparing `Topyfic-0.3.2/setup.py` & `Topyfic-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup
 
 setup(
     name='Topyfic',  # the name of your package
     packages=['Topyfic'],  # same as above
-    version='v0.3.2',  # version number
+    version='v0.3.3',  # version number
     license='MIT',  # license type
     description='Topyfic is a Python package designed to identify reproducible latent dirichlet allocation (LDA) '
                 'using leiden clustering and harmony for single cell epigenomics data',
     # short description
     author='Narges Rezaie',  # your name
     author_email='nargesrezaie80@gmail.com',  # your email
     url='https://github.com/mortazavilab/Topyfic',  # url to your git repo
-    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.2.tar.gz',  # link to the tar.gz file associated with this release
+    download_url='https://github.com/mortazavilab/Topyfic/archive/refs/tags/v0.3.3.tar.gz',  # link to the tar.gz file associated with this release
     keywords=['Cellular Programs', 'Latent Dirichlet allocation', 'single-cell multiome', 'single-cell RNA-seq',
               'gene regulatory network', 'Topic Modeling', 'single-nucleus RNA-seq'],  #
     python_requires='>=3.8',
     install_requires=[  # these can also include >, <, == to enforce version compatibility
         'pandas>=1.4.4',  # make sure the packages you put here are those NOT included in the base python distribution
         'scikit-learn>=0.24.2',
         'pytest',
```

