# Comparing `tmp/pandas-gpt-0.0.2.tar.gz` & `tmp/pandas-gpt-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandas-gpt-0.0.2.tar", last modified: Thu Jun  1 03:28:07 2023, max compression
+gzip compressed data, was "pandas-gpt-0.1.0.tar", last modified: Thu Jun  1 03:30:04 2023, max compression
```

## Comparing `pandas-gpt-0.0.2.tar` & `pandas-gpt-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:28:07.447489 pandas-gpt-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1073 2023-06-01 02:58:30.000000 pandas-gpt-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1902 2023-06-01 03:28:07.447489 pandas-gpt-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1702 2023-06-01 02:58:30.000000 pandas-gpt-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:28:07.445489 pandas-gpt-0.0.2/pandas_gpt/
--rw-r--r--   0 root         (0) root         (0)     2874 2023-06-01 02:58:30.000000 pandas-gpt-0.0.2/pandas_gpt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:28:07.446489 pandas-gpt-0.0.2/pandas_gpt.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1902 2023-06-01 03:28:07.000000 pandas-gpt-0.0.2/pandas_gpt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      224 2023-06-01 03:28:07.000000 pandas-gpt-0.0.2/pandas_gpt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 03:28:07.000000 pandas-gpt-0.0.2/pandas_gpt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-01 03:28:07.000000 pandas-gpt-0.0.2/pandas_gpt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-01 03:28:07.000000 pandas-gpt-0.0.2/pandas_gpt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      273 2023-06-01 03:27:59.000000 pandas-gpt-0.0.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 03:28:07.447489 pandas-gpt-0.0.2/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:30:04.113900 pandas-gpt-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-06-01 02:58:30.000000 pandas-gpt-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-06-01 03:30:04.112900 pandas-gpt-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-06-01 02:58:30.000000 pandas-gpt-0.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:30:04.111900 pandas-gpt-0.1.0/pandas_gpt/
+-rw-r--r--   0 root         (0) root         (0)     2874 2023-06-01 02:58:30.000000 pandas-gpt-0.1.0/pandas_gpt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 03:30:04.112900 pandas-gpt-0.1.0/pandas_gpt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-06-01 03:30:04.000000 pandas-gpt-0.1.0/pandas_gpt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-01 03:30:04.000000 pandas-gpt-0.1.0/pandas_gpt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 03:30:04.000000 pandas-gpt-0.1.0/pandas_gpt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-01 03:30:04.000000 pandas-gpt-0.1.0/pandas_gpt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-01 03:30:04.000000 pandas-gpt-0.1.0/pandas_gpt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      273 2023-06-01 03:29:56.000000 pandas-gpt-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 03:30:04.113900 pandas-gpt-0.1.0/setup.cfg
```

### Comparing `pandas-gpt-0.0.2/LICENSE` & `pandas-gpt-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pandas-gpt-0.0.2/PKG-INFO` & `pandas-gpt-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-gpt
-Version: 0.0.2
+Version: 0.1.0
 Summary: Power up your data science workflow with ChatGPT
 Author: Ryan Vandersmith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `pandas-gpt` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)
```

### Comparing `pandas-gpt-0.0.2/README.md` & `pandas-gpt-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `pandas-gpt-0.0.2/pandas_gpt/__init__.py` & `pandas-gpt-0.1.0/pandas_gpt/__init__.py`

 * *Files identical despite different names*

### Comparing `pandas-gpt-0.0.2/pandas_gpt.egg-info/PKG-INFO` & `pandas-gpt-0.1.0/pandas_gpt.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandas-gpt
-Version: 0.0.2
+Version: 0.1.0
 Summary: Power up your data science workflow with ChatGPT
 Author: Ryan Vandersmith
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `pandas-gpt` [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/rvanasa/pandas-gpt/blob/main/notebooks/pandas_gpt_demo.ipynb)
```

