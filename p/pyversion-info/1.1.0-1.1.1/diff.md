# Comparing `tmp/pyversion-info-1.1.0.tar.gz` & `tmp/pyversion-info-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyversion-info-1.1.0.tar", last modified: Mon Nov  8 21:11:52 2021, max compression
+gzip compressed data, was "pyversion-info-1.1.1.tar", last modified: Thu Jun  1 18:48:27 2023, max compression
```

## Comparing `pyversion-info-1.1.0.tar` & `pyversion-info-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2021-11-08 21:11:52.048414 pyversion-info-1.1.0/
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     2423 2021-11-08 21:11:46.000000 pyversion-info-1.1.0/CHANGELOG.md
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     1095 2021-11-08 21:11:46.000000 pyversion-info-1.1.0/LICENSE
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      126 2021-10-01 23:18:30.000000 pyversion-info-1.1.0/MANIFEST.in
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     4719 2021-11-08 21:11:52.048414 pyversion-info-1.1.0/PKG-INFO
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     3352 2021-11-04 14:33:41.000000 pyversion-info-1.1.0/README.rst
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2021-11-08 21:11:52.044413 pyversion-info-1.1.0/docs/
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      766 2021-11-04 14:28:25.000000 pyversion-info-1.1.0/docs/api.rst
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     2627 2021-11-08 21:11:46.000000 pyversion-info-1.1.0/docs/changelog.rst
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     3614 2021-11-08 21:02:55.000000 pyversion-info-1.1.0/docs/command.rst
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      968 2021-11-08 21:11:46.000000 pyversion-info-1.1.0/docs/conf.py
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     2729 2021-11-04 14:28:25.000000 pyversion-info-1.1.0/docs/index.rst
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)       59 2021-11-04 14:28:25.000000 pyversion-info-1.1.0/docs/requirements.txt
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      118 2020-11-25 18:56:18.000000 pyversion-info-1.1.0/pyproject.toml
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     2022 2021-11-08 21:11:52.048414 pyversion-info-1.1.0/setup.cfg
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2021-11-08 21:11:52.040413 pyversion-info-1.1.0/src/
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2021-11-08 21:11:52.044413 pyversion-info-1.1.0/src/pyversion_info/
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)    18554 2021-11-08 21:11:46.000000 pyversion-info-1.1.0/src/pyversion_info/__init__.py
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     7214 2021-11-08 20:59:10.000000 pyversion-info-1.1.0/src/pyversion_info/__main__.py
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)        0 2021-10-01 02:20:20.000000 pyversion-info-1.1.0/src/pyversion_info/py.typed
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     4217 2021-11-05 15:02:02.000000 pyversion-info-1.1.0/src/pyversion_info/util.py
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2021-11-08 21:11:52.048414 pyversion-info-1.1.0/src/pyversion_info.egg-info/
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     4719 2021-11-08 21:11:52.000000 pyversion-info-1.1.0/src/pyversion_info.egg-info/PKG-INFO
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      712 2021-11-08 21:11:52.000000 pyversion-info-1.1.0/src/pyversion_info.egg-info/SOURCES.txt
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)        1 2021-11-08 21:11:52.000000 pyversion-info-1.1.0/src/pyversion_info.egg-info/dependency_links.txt
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)       65 2021-11-08 21:11:52.000000 pyversion-info-1.1.0/src/pyversion_info.egg-info/entry_points.txt
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)       90 2021-11-08 21:11:52.000000 pyversion-info-1.1.0/src/pyversion_info.egg-info/requires.txt
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)       15 2021-11-08 21:11:52.000000 pyversion-info-1.1.0/src/pyversion_info.egg-info/top_level.txt
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2021-11-08 21:11:52.048414 pyversion-info-1.1.0/test/
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)      284 2021-11-04 14:28:25.000000 pyversion-info-1.1.0/test/conftest.py
-drwxr-xr-x   0 jwodder   (1001) jwodder   (1002)        0 2021-11-08 21:11:52.048414 pyversion-info-1.1.0/test/data/
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)    11392 2021-11-04 14:28:25.000000 pyversion-info-1.1.0/test/data/pyversion-info-data.json
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)    37153 2021-11-08 20:59:51.000000 pyversion-info-1.1.0/test/test_cmd_cpython.py
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)    12868 2021-11-04 14:28:25.000000 pyversion-info-1.1.0/test/test_cmd_pypy.py
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)    25938 2021-11-05 18:14:27.000000 pyversion-info-1.1.0/test/test_cpython_info.py
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     4908 2021-11-04 14:28:25.000000 pyversion-info-1.1.0/test/test_pypy_info.py
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     3086 2021-11-05 15:02:02.000000 pyversion-info-1.1.0/test/test_util.py
--rw-r--r--   0 jwodder   (1001) jwodder   (1002)     1479 2021-11-05 15:02:02.000000 pyversion-info-1.1.0/tox.ini
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-06-01 18:48:27.653154 pyversion-info-1.1.1/
+-rw-r--r--   0 jwodder    (501) staff       (20)     2514 2023-06-01 18:48:21.000000 pyversion-info-1.1.1/CHANGELOG.md
+-rw-r--r--   0 jwodder    (501) staff       (20)     1095 2023-06-01 18:48:21.000000 pyversion-info-1.1.1/LICENSE
+-rw-r--r--   0 jwodder    (501) staff       (20)      126 2021-10-04 00:33:13.000000 pyversion-info-1.1.1/MANIFEST.in
+-rw-r--r--   0 jwodder    (501) staff       (20)     4707 2023-06-01 18:48:27.653297 pyversion-info-1.1.1/PKG-INFO
+-rw-r--r--   0 jwodder    (501) staff       (20)     3352 2021-11-06 02:16:59.000000 pyversion-info-1.1.1/README.rst
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-06-01 18:48:27.642444 pyversion-info-1.1.1/docs/
+-rw-r--r--   0 jwodder    (501) staff       (20)      766 2021-11-06 02:16:59.000000 pyversion-info-1.1.1/docs/api.rst
+-rw-r--r--   0 jwodder    (501) staff       (20)     2719 2023-06-01 18:48:21.000000 pyversion-info-1.1.1/docs/changelog.rst
+-rw-r--r--   0 jwodder    (501) staff       (20)     3614 2021-11-19 14:52:13.000000 pyversion-info-1.1.1/docs/command.rst
+-rw-r--r--   0 jwodder    (501) staff       (20)      982 2023-06-01 18:48:21.000000 pyversion-info-1.1.1/docs/conf.py
+-rw-r--r--   0 jwodder    (501) staff       (20)     2729 2021-11-06 02:16:59.000000 pyversion-info-1.1.1/docs/index.rst
+-rw-r--r--   0 jwodder    (501) staff       (20)       59 2022-05-30 18:44:26.000000 pyversion-info-1.1.1/docs/requirements.txt
+-rw-r--r--   0 jwodder    (501) staff       (20)       91 2022-07-07 12:48:58.000000 pyversion-info-1.1.1/pyproject.toml
+-rw-r--r--   0 jwodder    (501) staff       (20)     2036 2023-06-01 18:48:27.654100 pyversion-info-1.1.1/setup.cfg
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-06-01 18:48:27.636210 pyversion-info-1.1.1/src/
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-06-01 18:48:27.644374 pyversion-info-1.1.1/src/pyversion_info/
+-rw-r--r--   0 jwodder    (501) staff       (20)    18559 2023-06-01 18:48:21.000000 pyversion-info-1.1.1/src/pyversion_info/__init__.py
+-rw-r--r--   0 jwodder    (501) staff       (20)     7214 2021-11-19 14:52:13.000000 pyversion-info-1.1.1/src/pyversion_info/__main__.py
+-rw-r--r--   0 jwodder    (501) staff       (20)        0 2021-10-04 00:33:13.000000 pyversion-info-1.1.1/src/pyversion_info/py.typed
+-rw-r--r--   0 jwodder    (501) staff       (20)     4217 2021-11-06 02:16:59.000000 pyversion-info-1.1.1/src/pyversion_info/util.py
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-06-01 18:48:27.646310 pyversion-info-1.1.1/src/pyversion_info.egg-info/
+-rw-r--r--   0 jwodder    (501) staff       (20)     4707 2023-06-01 18:48:27.000000 pyversion-info-1.1.1/src/pyversion_info.egg-info/PKG-INFO
+-rw-r--r--   0 jwodder    (501) staff       (20)      712 2023-06-01 18:48:27.000000 pyversion-info-1.1.1/src/pyversion_info.egg-info/SOURCES.txt
+-rw-r--r--   0 jwodder    (501) staff       (20)        1 2023-06-01 18:48:27.000000 pyversion-info-1.1.1/src/pyversion_info.egg-info/dependency_links.txt
+-rw-r--r--   0 jwodder    (501) staff       (20)       64 2023-06-01 18:48:27.000000 pyversion-info-1.1.1/src/pyversion_info.egg-info/entry_points.txt
+-rw-r--r--   0 jwodder    (501) staff       (20)       94 2023-06-01 18:48:27.000000 pyversion-info-1.1.1/src/pyversion_info.egg-info/requires.txt
+-rw-r--r--   0 jwodder    (501) staff       (20)       15 2023-06-01 18:48:27.000000 pyversion-info-1.1.1/src/pyversion_info.egg-info/top_level.txt
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-06-01 18:48:27.651924 pyversion-info-1.1.1/test/
+-rw-r--r--   0 jwodder    (501) staff       (20)      284 2021-11-06 02:16:59.000000 pyversion-info-1.1.1/test/conftest.py
+drwxr-xr-x   0 jwodder    (501) staff       (20)        0 2023-06-01 18:48:27.652310 pyversion-info-1.1.1/test/data/
+-rw-r--r--   0 jwodder    (501) staff       (20)    11392 2021-11-06 02:16:59.000000 pyversion-info-1.1.1/test/data/pyversion-info-data.json
+-rw-r--r--   0 jwodder    (501) staff       (20)    37153 2021-11-19 14:52:13.000000 pyversion-info-1.1.1/test/test_cmd_cpython.py
+-rw-r--r--   0 jwodder    (501) staff       (20)    12868 2021-11-06 02:16:59.000000 pyversion-info-1.1.1/test/test_cmd_pypy.py
+-rw-r--r--   0 jwodder    (501) staff       (20)    25938 2021-11-06 02:16:59.000000 pyversion-info-1.1.1/test/test_cpython_info.py
+-rw-r--r--   0 jwodder    (501) staff       (20)     4908 2021-11-06 02:16:59.000000 pyversion-info-1.1.1/test/test_pypy_info.py
+-rw-r--r--   0 jwodder    (501) staff       (20)     3086 2021-11-06 02:16:59.000000 pyversion-info-1.1.1/test/test_util.py
+-rw-r--r--   0 jwodder    (501) staff       (20)     1442 2022-12-26 21:57:18.000000 pyversion-info-1.1.1/tox.ini
```

### Comparing `pyversion-info-1.1.0/CHANGELOG.md` & `pyversion-info-1.1.1/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v1.1.1 (2023-06-01)
+-------------------
+- Support Python 3.11
+- Support cachecontrol 0.13
+
 v1.1.0 (2021-11-08)
 -------------------
 - Use pydantic internally for parsing & validating version databases
 - `eol_date()` and `is_eol()` now accept major and micro versions
 - The `show` command now outputs the EOL date and EOL state for all CPython
   version levels
```

### Comparing `pyversion-info-1.1.0/LICENSE` & `pyversion-info-1.1.1/LICENSE`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2019-2021 John Thorvald Wodder II
+Copyright (c) 2019-2023 John Thorvald Wodder II
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pyversion-info-1.1.0/PKG-INFO` & `pyversion-info-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: pyversion-info
-Version: 1.1.0
+Version: 1.1.1
 Summary: Get information about released & unreleased CPython and PyPy versions
 Home-page: https://github.com/jwodder/pyversion-info
 Author: John Thorvald Wodder II
 Author-email: pyversion-info@varonathe.org
 License: MIT
 Project-URL: Source Code, https://github.com/jwodder/pyversion-info
 Project-URL: Bug Tracker, https://github.com/jwodder/pyversion-info/issues
 Project-URL: Documentation, https://pyversion-info.readthedocs.io
 Keywords: CPython,PyPy,history,python,python versions
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Typing :: Typed
-Requires-Python: ~=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: http://www.repostatus.org/badges/latest/active.svg
     :target: http://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
@@ -123,9 +122,7 @@
 Caveats
 =======
 
 The CPython database is generally only updated when an edit is made to a
 release schedule PEP.  Occasionally, a deadline listed in a PEP is missed, but
 the PEP is not updated for a couple days, and so for a brief period this
 library will falsely report the given version as released.
-
-
```

### Comparing `pyversion-info-1.1.0/README.rst` & `pyversion-info-1.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/docs/api.rst` & `pyversion-info-1.1.1/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/docs/changelog.rst` & `pyversion-info-1.1.1/docs/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 .. currentmodule:: pyversion_info
 
 Changelog
 =========
 
+v1.1.1 (2023-06-01)
+-------------------
+- Support Python 3.11
+- Support cachecontrol 0.13
+
+
 v1.1.0 (2021-11-08)
 -------------------
 - Use pydantic internally for parsing & validating version databases
 - `~CPythonVersionInfo.eol_date()` and `~CPythonVersionInfo.is_eol()` now
   accept major and micro versions
```

### Comparing `pyversion-info-1.1.0/docs/command.rst` & `pyversion-info-1.1.1/docs/command.rst`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/docs/conf.py` & `pyversion-info-1.1.1/docs/conf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pyversion_info import __version__
 
 project = "pyversion-info"
 author = "John T. Wodder II"
-copyright = "2019-2021 John T. Wodder II"
+copyright = "2019-2023 John T. Wodder II"  # noqa: A001
 
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "sphinx_copybutton",
 ]
```

### Comparing `pyversion-info-1.1.0/docs/index.rst` & `pyversion-info-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/setup.cfg` & `pyversion-info-1.1.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 keywords = 
 	CPython
 	PyPy
 	history
 	python
 	python versions
 classifiers = 
-	Development Status :: 4 - Beta
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Programming Language :: Python :: Implementation :: CPython
 	Programming Language :: Python :: Implementation :: PyPy
 	License :: OSI Approved :: MIT License
 	Intended Audience :: Developers
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	Typing :: Typed
@@ -36,17 +36,17 @@
 	Documentation = https://pyversion-info.readthedocs.io
 
 [options]
 packages = find:
 package_dir = 
 	=src
 include_package_data = True
-python_requires = ~=3.7
+python_requires = >=3.7
 install_requires = 
-	cachecontrol[filecache] ~= 0.12.0
+	cachecontrol[filecache] >= 0.12, < 0.14
 	click                   >= 8.0
 	platformdirs            ~= 2.1
 	pydantic                ~= 1.7
 	requests                ~= 2.20
 
 [options.packages.find]
 where = src
```

### Comparing `pyversion-info-1.1.0/src/pyversion_info/__init__.py` & `pyversion-info-1.1.1/src/pyversion_info/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 Visit <https://github.com/jwodder/pyversion-info> or
 <https://pyversion-info.rtfd.io> for more information.
 """
 
 from __future__ import annotations
 
-__version__ = "1.1.0"
+__version__ = "1.1.1"
 __author__ = "John Thorvald Wodder II"
 __author_email__ = "pyversion-info@varonathe.org"
 __license__ = "MIT"
 __url__ = "https://github.com/jwodder/pyversion-info"
 
 from collections import OrderedDict
 from dataclasses import dataclass
@@ -88,15 +88,15 @@
         :param str url: The URL from which to fetch the data
         :param Union[str,Path,None] cache_dir: The directory to use for caching
             HTTP requests.  May be `None` to disable caching.
         :rtype: VersionDatabase
         """
         s = requests.Session()
         if cache_dir is not None:
-            s = CacheControl(s, cache=FileCache(cache_dir))
+            s = CacheControl(s, cache=FileCache(str(cache_dir)))
         with s:
             r = s.get(url)
             r.raise_for_status()
             return cls.parse_obj(r.json())
 
     @classmethod
     def parse_file(cls, filepath: Union[str, Path]) -> VersionDatabase:
```

### Comparing `pyversion-info-1.1.0/src/pyversion_info/__main__.py` & `pyversion-info-1.1.1/src/pyversion_info/__main__.py`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/src/pyversion_info/util.py` & `pyversion-info-1.1.1/src/pyversion_info/util.py`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/src/pyversion_info.egg-info/PKG-INFO` & `pyversion-info-1.1.1/src/pyversion_info.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: pyversion-info
-Version: 1.1.0
+Version: 1.1.1
 Summary: Get information about released & unreleased CPython and PyPy versions
 Home-page: https://github.com/jwodder/pyversion-info
 Author: John Thorvald Wodder II
 Author-email: pyversion-info@varonathe.org
 License: MIT
 Project-URL: Source Code, https://github.com/jwodder/pyversion-info
 Project-URL: Bug Tracker, https://github.com/jwodder/pyversion-info/issues
 Project-URL: Documentation, https://pyversion-info.readthedocs.io
 Keywords: CPython,PyPy,history,python,python versions
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Typing :: Typed
-Requires-Python: ~=3.7
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 .. image:: http://www.repostatus.org/badges/latest/active.svg
     :target: http://www.repostatus.org/#active
     :alt: Project Status: Active — The project has reached a stable, usable
           state and is being actively developed.
@@ -123,9 +122,7 @@
 Caveats
 =======
 
 The CPython database is generally only updated when an edit is made to a
 release schedule PEP.  Occasionally, a deadline listed in a PEP is missed, but
 the PEP is not updated for a couple days, and so for a brief period this
 library will falsely report the given version as released.
-
-
```

### Comparing `pyversion-info-1.1.0/src/pyversion_info.egg-info/SOURCES.txt` & `pyversion-info-1.1.1/src/pyversion_info.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/test/data/pyversion-info-data.json` & `pyversion-info-1.1.1/test/data/pyversion-info-data.json`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/test/test_cmd_cpython.py` & `pyversion-info-1.1.1/test/test_cmd_cpython.py`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/test/test_cmd_pypy.py` & `pyversion-info-1.1.1/test/test_cmd_pypy.py`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/test/test_cpython_info.py` & `pyversion-info-1.1.1/test/test_cpython_info.py`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/test/test_pypy_info.py` & `pyversion-info-1.1.1/test/test_pypy_info.py`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/test/test_util.py` & `pyversion-info-1.1.1/test/test_util.py`

 * *Files identical despite different names*

### Comparing `pyversion-info-1.1.0/tox.ini` & `pyversion-info-1.1.1/tox.ini`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 [tox]
-envlist = lint,typing,py36,py37,py38,py39,py310,pypy3
+envlist = lint,typing,py36,py37,py38,py39,py310,py311,pypy3
 skip_missing_interpreters = True
 isolated_build = True
 minversion = 3.3.0
 
 [testenv]
 setenv =
     TZ=EST5EDT,M3.2.0,M11.1.0
 deps =
-    pytest~=6.0
-    pytest-cov~=2.0
-    pytest-mock~=3.0
+    pytest
+    pytest-cov
+    pytest-mock
 commands =
     pytest {posargs} test
 
 [testenv:lint]
 skip_install = True
 deps =
-    flake8~=3.7
+    flake8
     flake8-bugbear
-    flake8-builtins~=1.4
+    flake8-builtins
     flake8-unused-arguments
 commands =
-    flake8 --config=tox.ini src test
+    flake8 src test
 
 [testenv:typing]
 deps =
-    mypy~=0.900
+    mypy
     types-requests
     {[testenv]deps}
 commands =
     mypy src test
 
 [pytest]
 addopts = --cov=pyversion_info --no-cov-on-fail
@@ -39,33 +39,33 @@
 [coverage:run]
 branch = True
 parallel = True
 
 [coverage:paths]
 source =
     src
-    .tox/*/site-packages
+    .tox/**/site-packages
 
 [coverage:report]
 precision = 2
 show_missing = True
 exclude_lines =
     pragma: no cover
     if TYPE_CHECKING:
     \.\.\.
 
 [flake8]
 doctests = False
-exclude = .*/,build/,dist/,venv/
+exclude = .*/,build/,dist/,test/data,venv/
 hang-closing = False
 max-doc-length = 120
 max-line-length = 120
 unused-arguments-ignore-stub-functions = True
-select = C,B,B902,B950,E,E242,F,I,U100,W
-ignore = B005,E203,E262,E266,E501,I201,W503
+select = A,B,B902,B950,C,E,E242,F,U100,W
+ignore = B005,E203,E262,E266,E501,W503
 
 [isort]
 atomic = True
 force_sort_within_sections = True
 honor_noqa = True
 lines_between_sections = 0
 profile = black
```

