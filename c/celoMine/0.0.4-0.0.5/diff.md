# Comparing `tmp/celoMine-0.0.4.tar.gz` & `tmp/celoMine-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\celoMine-0.0.4.tar", last modified: Thu Jun  1 09:39:03 2023, max compression
+gzip compressed data, was "dist\celoMine-0.0.5.tar", last modified: Thu Jun  1 14:12:06 2023, max compression
```

## Comparing `celoMine-0.0.4.tar` & `celoMine-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:39:03.978544 celoMine-0.0.4/
--rw-rw-rw-   0        0        0    35820 2023-05-31 18:08:15.000000 celoMine-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     2925 2023-06-01 09:39:03.978544 celoMine-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2362 2023-05-31 18:08:15.000000 celoMine-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-01 09:39:03.962551 celoMine-0.0.4/celoMine/
--rw-rw-rw-   0        0        0     5377 2023-05-31 18:08:15.000000 celoMine-0.0.4/celoMine/PredictivePR.py
--rw-rw-rw-   0        0        0       98 2023-05-31 18:08:15.000000 celoMine-0.0.4/celoMine/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:39:03.978544 celoMine-0.0.4/celoMine.egg-info/
--rw-rw-rw-   0        0        0     2925 2023-06-01 09:39:03.000000 celoMine-0.0.4/celoMine.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-06-01 09:39:03.000000 celoMine-0.0.4/celoMine.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:39:03.000000 celoMine-0.0.4/celoMine.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-01 09:39:03.000000 celoMine-0.0.4/celoMine.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-01 09:39:03.000000 celoMine-0.0.4/celoMine.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-01 09:39:03.978544 celoMine-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1008 2023-06-01 09:32:48.000000 celoMine-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:12:06.649458 celoMine-0.0.5/
+-rw-rw-rw-   0        0        0    35820 2023-05-31 18:08:15.000000 celoMine-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3733 2023-06-01 14:12:06.633834 celoMine-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3153 2023-06-01 14:11:04.000000 celoMine-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-01 14:12:06.618177 celoMine-0.0.5/celoMine/
+-rw-rw-rw-   0        0        0     5377 2023-05-31 18:08:15.000000 celoMine-0.0.5/celoMine/PredictivePR.py
+-rw-rw-rw-   0        0        0       98 2023-05-31 18:08:15.000000 celoMine-0.0.5/celoMine/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-01 14:12:06.633834 celoMine-0.0.5/celoMine.egg-info/
+-rw-rw-rw-   0        0        0     3733 2023-06-01 14:12:06.000000 celoMine-0.0.5/celoMine.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-01 14:12:06.000000 celoMine-0.0.5/celoMine.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-01 14:12:06.000000 celoMine-0.0.5/celoMine.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-01 14:12:06.000000 celoMine-0.0.5/celoMine.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-01 14:12:06.000000 celoMine-0.0.5/celoMine.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-01 14:12:06.649458 celoMine-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1029 2023-06-01 13:53:01.000000 celoMine-0.0.5/setup.py
```

### Comparing `celoMine-0.0.4/LICENSE` & `celoMine-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `celoMine-0.0.4/PKG-INFO` & `celoMine-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 Metadata-Version: 2.1
 Name: celoMine
-Version: 0.0.4
+Version: 0.0.5
 Summary: Predictive machine learning for Celonis
 Author: Jean BERTIN
 Author-email: <jeanbertin.ensam@gmail.com>
+License: GPL-v3
 Keywords: python,celonis,process mining
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # celoMine
 
+
+[![PyPI Downloads](https://img.shields.io/pypi/dm/celoMine.svg?label=PyPI%20downloads)](
+https://pypi.org/project/celoMine/)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-Ask%20questions-blue.svg)](
+https://stackoverflow.com/questions/tagged/celomine)
+[![Nature Paper](https://img.shields.io/badge/Article-Process-Mining--blue)](
+https://www.journals.elsevier.com/engineering-applications-of-artificial-intelligence/forthcoming-special-issues/artificial-intelligence-for-process-mining)
+
+
+
+
 celoMine brings predictive machine learning to your Celonis analyses to enable deep process insights and data-driven decision-making.
 This powerful python framework leverage machine learning algorithms and visualization techniques within your Celonis analyses to drive process optimization.
 
+- **Source code:** https://github.com/numpy/numpy
+- **Mailing list:** https://mail.python.org/mailman/listinfo/numpy-discussion
+- **Bug reports:** https://github.com/JeanBertinR/celoMine/issues
+- **Report a security vulnerability:** https://tidelift.com/docs/security
 
 <div align="center">
   <img src="./celoMine_logo.png" alt="Logo celoMine" width="50%">
 </div>
 
 ## Requirements
```

### Comparing `celoMine-0.0.4/README.md` & `celoMine-0.0.5/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 # celoMine
 
+
+[![PyPI Downloads](https://img.shields.io/pypi/dm/celoMine.svg?label=PyPI%20downloads)](
+https://pypi.org/project/celoMine/)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-Ask%20questions-blue.svg)](
+https://stackoverflow.com/questions/tagged/celomine)
+[![Nature Paper](https://img.shields.io/badge/Article-Process-Mining--blue)](
+https://www.journals.elsevier.com/engineering-applications-of-artificial-intelligence/forthcoming-special-issues/artificial-intelligence-for-process-mining)
+
+
+
+
 celoMine brings predictive machine learning to your Celonis analyses to enable deep process insights and data-driven decision-making.
 This powerful python framework leverage machine learning algorithms and visualization techniques within your Celonis analyses to drive process optimization.
 
+- **Source code:** https://github.com/numpy/numpy
+- **Mailing list:** https://mail.python.org/mailman/listinfo/numpy-discussion
+- **Bug reports:** https://github.com/JeanBertinR/celoMine/issues
+- **Report a security vulnerability:** https://tidelift.com/docs/security
 
 <div align="center">
   <img src="./celoMine_logo.png" alt="Logo celoMine" width="50%">
 </div>
 
 ## Requirements
```

### Comparing `celoMine-0.0.4/celoMine/PredictivePR.py` & `celoMine-0.0.5/celoMine/PredictivePR.py`

 * *Files identical despite different names*

### Comparing `celoMine-0.0.4/celoMine.egg-info/PKG-INFO` & `celoMine-0.0.5/celoMine.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,44 @@
 Metadata-Version: 2.1
 Name: celoMine
-Version: 0.0.4
+Version: 0.0.5
 Summary: Predictive machine learning for Celonis
 Author: Jean BERTIN
 Author-email: <jeanbertin.ensam@gmail.com>
+License: GPL-v3
 Keywords: python,celonis,process mining
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # celoMine
 
+
+[![PyPI Downloads](https://img.shields.io/pypi/dm/celoMine.svg?label=PyPI%20downloads)](
+https://pypi.org/project/celoMine/)
+[![Stack Overflow](https://img.shields.io/badge/stackoverflow-Ask%20questions-blue.svg)](
+https://stackoverflow.com/questions/tagged/celomine)
+[![Nature Paper](https://img.shields.io/badge/Article-Process-Mining--blue)](
+https://www.journals.elsevier.com/engineering-applications-of-artificial-intelligence/forthcoming-special-issues/artificial-intelligence-for-process-mining)
+
+
+
+
 celoMine brings predictive machine learning to your Celonis analyses to enable deep process insights and data-driven decision-making.
 This powerful python framework leverage machine learning algorithms and visualization techniques within your Celonis analyses to drive process optimization.
 
+- **Source code:** https://github.com/numpy/numpy
+- **Mailing list:** https://mail.python.org/mailman/listinfo/numpy-discussion
+- **Bug reports:** https://github.com/JeanBertinR/celoMine/issues
+- **Report a security vulnerability:** https://tidelift.com/docs/security
 
 <div align="center">
   <img src="./celoMine_logo.png" alt="Logo celoMine" width="50%">
 </div>
 
 ## Requirements
```

### Comparing `celoMine-0.0.4/setup.py` & `celoMine-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Predictive machine learning for Celonis'
 LONG_DESCRIPTION = 'Enrich Celonis process mining analyses using predictive machine learning and visualisation tools'
 
 # Setting up
 setup(
     name="celoMine",
     version=VERSION,
     author="Jean BERTIN",
     author_email="<jeanbertin.ensam@gmail.com>",
+    licence="GPL-v3",
     description=DESCRIPTION,
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=['pandas', 'numpy' ,'scikit-learn','matplotlib'],
     keywords=['python', 'celonis', 'process mining'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ]
-)
+)
```

