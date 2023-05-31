# Comparing `tmp/pdlpy-0.4.0.tar.gz` & `tmp/pdlpy-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdlpy-0.4.0.tar", last modified: Sat Apr  1 07:35:18 2023, max compression
+gzip compressed data, was "pdlpy-0.4.1.tar", last modified: Wed May 31 22:33:13 2023, max compression
```

## Comparing `pdlpy-0.4.0.tar` & `pdlpy-0.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 07:35:18.273676 pdlpy-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-03-26 11:27:10.000000 pdlpy-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2948 2023-04-01 07:35:18.273676 pdlpy-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2180 2023-03-26 22:21:06.000000 pdlpy-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 07:35:18.273676 pdlpy-0.4.0/pdlpy/
--rw-r--r--   0 root         (0) root         (0)      339 2023-04-01 06:54:01.000000 pdlpy-0.4.0/pdlpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1905 2023-04-01 07:04:30.000000 pdlpy-0.4.0/pdlpy/bernoulli.py
--rw-r--r--   0 root         (0) root         (0)     2152 2023-04-01 07:04:43.000000 pdlpy-0.4.0/pdlpy/binomial.py
--rw-r--r--   0 root         (0) root         (0)      471 2023-04-01 07:29:00.000000 pdlpy-0.4.0/pdlpy/decorators.py
--rw-r--r--   0 root         (0) root         (0)      473 2023-04-01 05:29:24.000000 pdlpy-0.4.0/pdlpy/distribution.py
--rw-r--r--   0 root         (0) root         (0)     1806 2023-04-01 07:05:08.000000 pdlpy-0.4.0/pdlpy/exponential.py
--rw-r--r--   0 root         (0) root         (0)     1948 2023-04-01 07:05:18.000000 pdlpy-0.4.0/pdlpy/geometric.py
--rw-r--r--   0 root         (0) root         (0)     2400 2023-04-01 07:05:27.000000 pdlpy-0.4.0/pdlpy/hypergeometric.py
--rw-r--r--   0 root         (0) root         (0)      164 2022-12-02 04:21:44.000000 pdlpy-0.4.0/pdlpy/math.py
--rw-r--r--   0 root         (0) root         (0)     1723 2023-04-01 07:05:34.000000 pdlpy-0.4.0/pdlpy/normal.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-04-01 07:05:51.000000 pdlpy-0.4.0/pdlpy/poisson.py
--rw-r--r--   0 root         (0) root         (0)     1911 2023-04-01 07:06:00.000000 pdlpy-0.4.0/pdlpy/uniform.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-01 07:35:18.273676 pdlpy-0.4.0/pdlpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2948 2023-04-01 07:35:18.000000 pdlpy-0.4.0/pdlpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      395 2023-04-01 07:35:18.000000 pdlpy-0.4.0/pdlpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-01 07:35:18.000000 pdlpy-0.4.0/pdlpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-04-01 07:35:18.000000 pdlpy-0.4.0/pdlpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-01 07:35:18.000000 pdlpy-0.4.0/pdlpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-01 07:35:18.273676 pdlpy-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1033 2023-03-26 21:27:52.000000 pdlpy-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 22:33:13.438468 pdlpy-0.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-28 05:14:58.000000 pdlpy-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-05-31 22:33:13.438468 pdlpy-0.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-05-28 05:14:58.000000 pdlpy-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 22:33:13.438468 pdlpy-0.4.1/pdlpy/
+-rw-r--r--   0 root         (0) root         (0)      339 2023-05-31 06:38:13.000000 pdlpy-0.4.1/pdlpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-05-28 05:14:56.000000 pdlpy-0.4.1/pdlpy/bernoulli.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2023-05-28 05:14:56.000000 pdlpy-0.4.1/pdlpy/binomial.py
+-rw-r--r--   0 root         (0) root         (0)      471 2023-05-28 05:14:56.000000 pdlpy-0.4.1/pdlpy/decorators.py
+-rw-r--r--   0 root         (0) root         (0)      473 2023-05-28 05:14:57.000000 pdlpy-0.4.1/pdlpy/distribution.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2023-05-28 05:14:57.000000 pdlpy-0.4.1/pdlpy/exponential.py
+-rw-r--r--   0 root         (0) root         (0)     1948 2023-05-28 05:14:57.000000 pdlpy-0.4.1/pdlpy/geometric.py
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-05-31 05:59:33.000000 pdlpy-0.4.1/pdlpy/hypergeometric.py
+-rw-r--r--   0 root         (0) root         (0)      164 2023-05-28 05:14:57.000000 pdlpy-0.4.1/pdlpy/math.py
+-rw-r--r--   0 root         (0) root         (0)     1747 2023-05-31 03:53:49.000000 pdlpy-0.4.1/pdlpy/normal.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-05-28 05:14:57.000000 pdlpy-0.4.1/pdlpy/poisson.py
+-rw-r--r--   0 root         (0) root         (0)     1911 2023-05-28 05:14:57.000000 pdlpy-0.4.1/pdlpy/uniform.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-31 22:33:13.438468 pdlpy-0.4.1/pdlpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2911 2023-05-31 22:33:13.000000 pdlpy-0.4.1/pdlpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      395 2023-05-31 22:33:13.000000 pdlpy-0.4.1/pdlpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-31 22:33:13.000000 pdlpy-0.4.1/pdlpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       92 2023-05-31 22:33:13.000000 pdlpy-0.4.1/pdlpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-31 22:33:13.000000 pdlpy-0.4.1/pdlpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-31 22:33:13.438468 pdlpy-0.4.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-31 06:38:05.000000 pdlpy-0.4.1/setup.py
```

### Comparing `pdlpy-0.4.0/LICENSE` & `pdlpy-0.4.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 André Bienemann
+Copyright (c) 2023 André Bienemann
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pdlpy-0.4.0/PKG-INFO` & `pdlpy-0.4.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pdlpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Probability Distribution Library for Python
 Home-page: https://github.com/andrebienemann/pdlpy
 Author: André Bienemann
 Author-email: andre.bienemann@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -63,9 +61,7 @@
 
 ## Links
 
 - [Documentation](https://andrebienemann.github.io/pdlpy/)
 - [PyPI Releases](https://pypi.org/project/pdlpy/)
 - [Source Code](https://github.com/andrebienemann/pdlpy/)
 - [Issue Tracker](https://github.com/andrebienemann/pdlpy/issues/)
-
-
```

### Comparing `pdlpy-0.4.0/README.md` & `pdlpy-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pdlpy-0.4.0/pdlpy/bernoulli.py` & `pdlpy-0.4.1/pdlpy/bernoulli.py`

 * *Files identical despite different names*

### Comparing `pdlpy-0.4.0/pdlpy/binomial.py` & `pdlpy-0.4.1/pdlpy/binomial.py`

 * *Files identical despite different names*

### Comparing `pdlpy-0.4.0/pdlpy/exponential.py` & `pdlpy-0.4.1/pdlpy/exponential.py`

 * *Files identical despite different names*

### Comparing `pdlpy-0.4.0/pdlpy/geometric.py` & `pdlpy-0.4.1/pdlpy/geometric.py`

 * *Files identical despite different names*

### Comparing `pdlpy-0.4.0/pdlpy/hypergeometric.py` & `pdlpy-0.4.1/pdlpy/hypergeometric.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,16 +58,16 @@
         Parameters
         x: the value of the random variable X
 
         Returns
         The probability that X will take a value exactly equal to x
         """
 
-        if x < 0 or x > self._n:
-            raise ValueError("x must be in the range [0, n]")
+        if x < max(0, self._n + self._M - self._N) or x > min(self._n, self._M):
+            raise ValueError("x must be in the range [max(0, n + M - N), min(n, M)]")
 
         return (
             ncr(self._M, x)
             * ncr(self._N - self._M, self._n - x)
             / ncr(self._N, self._n)
         )
 
@@ -79,14 +79,14 @@
         Parameters
         x: the value of the random variable X
 
         Returns
         The probability that X will take a value less than or equal to x
         """
 
-        if x < 0 or x > self._n:
-            raise ValueError("x must be in the range [0, n]")
+        if x < max(0, self._n + self._M - self._N) or x > min(self._n, self._M):
+            raise ValueError("x must be in the range [max(0, n + M - N), min(n, M)]")
 
-        if x == 0:
-            return self.pmf(0)
+        if x == max(0, self._n + self._M - self._N):
+            return self.pmf(max(0, self._n + self._M - self._N))
         else:
             return self.pmf(x) + self.cdf(x - 1)
```

### Comparing `pdlpy-0.4.0/pdlpy/normal.py` & `pdlpy-0.4.1/pdlpy/normal.py`

 * *Files 9% similar despite different names*

```diff
@@ -43,15 +43,17 @@
 
         Parameters
         x: the value of random variable X
 
         Returns
         The relative likelihood that X will lie in the sample space of x
         """
-        return (1 / sqrt(2 * pi * self._v)) * e ** (-((x - self._e) ** 2 / 2 * self._v))
+        return (1 / sqrt(2 * pi * self._v)) * e ** (
+            -((x - self._e) ** 2 / (2 * self._v))
+        )
 
     @iterable
     def cdf(self, x: Union[list, tuple, float]) -> Union[list, tuple, float]:
         """
         Cumulative Distribution Function
 
         Parameters
```

### Comparing `pdlpy-0.4.0/pdlpy/poisson.py` & `pdlpy-0.4.1/pdlpy/poisson.py`

 * *Files identical despite different names*

### Comparing `pdlpy-0.4.0/pdlpy/uniform.py` & `pdlpy-0.4.1/pdlpy/uniform.py`

 * *Files identical despite different names*

### Comparing `pdlpy-0.4.0/pdlpy.egg-info/PKG-INFO` & `pdlpy-0.4.1/pdlpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pdlpy
-Version: 0.4.0
+Version: 0.4.1
 Summary: Probability Distribution Library for Python
 Home-page: https://github.com/andrebienemann/pdlpy
 Author: André Bienemann
 Author-email: andre.bienemann@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -63,9 +61,7 @@
 
 ## Links
 
 - [Documentation](https://andrebienemann.github.io/pdlpy/)
 - [PyPI Releases](https://pypi.org/project/pdlpy/)
 - [Source Code](https://github.com/andrebienemann/pdlpy/)
 - [Issue Tracker](https://github.com/andrebienemann/pdlpy/issues/)
-
-
```

### Comparing `pdlpy-0.4.0/setup.py` & `pdlpy-0.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="pdlpy",
-    version="0.4.0",
+    version="0.4.1",
     author="André Bienemann",
     author_email="andre.bienemann@gmail.com",
     description="Probability Distribution Library for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/andrebienemann/pdlpy",
     extras_require={
         "dev": ["black", "coverage", "isort", "twine", "wheel"],
-        "docs": ["mkdocs", "mkdocs-material"],
+        "docs": ["mkdocs", "mkdocs-material", "plotly", "dash", "gunicorn"],
     },
     packages=setuptools.find_packages(),
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

