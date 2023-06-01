# Comparing `tmp/atpublic-3.1.1.tar.gz` & `tmp/atpublic-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atpublic-3.1.1.tar", last modified: Sat Sep  3 00:43:54 2022, max compression
+gzip compressed data, was "atpublic-3.1.2.tar", last modified: Thu Jun  1 05:03:42 2023, max compression
```

## Comparing `atpublic-3.1.1.tar` & `atpublic-3.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-rw-rw-   0 root         (0) root         (0)      556 2022-09-03 00:43:18.056890 atpublic-3.1.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      721 2022-09-03 00:43:18.056890 atpublic-3.1.1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     3304 2022-09-03 00:43:18.056890 atpublic-3.1.1/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     3009 2022-09-03 00:43:18.056890 atpublic-3.1.1/docs/NEWS.rst
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-03 00:43:18.056890 atpublic-3.1.1/docs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      175 2022-09-03 00:43:18.056890 atpublic-3.1.1/docs/apiref.rst
--rw-rw-rw-   0 root         (0) root         (0)     7326 2022-09-03 00:43:18.056890 atpublic-3.1.1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2022-09-03 00:43:18.056890 atpublic-3.1.1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     8020 2022-09-03 00:43:18.056890 atpublic-3.1.1/docs/using.rst
--rw-rw-rw-   0 root         (0) root         (0)     2838 2022-09-03 00:43:18.057891 atpublic-3.1.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      509 2022-09-03 00:43:18.057891 atpublic-3.1.1/src/public/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      759 2022-09-03 00:43:18.057891 atpublic-3.1.1/src/public/private.py
--rw-rw-rw-   0 root         (0) root         (0)     3057 2022-09-03 00:43:18.057891 atpublic-3.1.1/src/public/public.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-03 00:43:18.057891 atpublic-3.1.1/src/public/py.typed
--rw-rw-rw-   0 root         (0) root         (0)      107 2022-09-03 00:43:18.057891 atpublic-3.1.1/src/public/types.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-09-03 00:43:18.057891 atpublic-3.1.1/test/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      204 2022-09-03 00:43:18.057891 atpublic-3.1.1/test/test_mypy.py
--rw-rw-rw-   0 root         (0) root         (0)      923 2022-09-03 00:43:18.057891 atpublic-3.1.1/test/test_private.py
--rw-rw-rw-   0 root         (0) root         (0)     3104 2022-09-03 00:43:18.057891 atpublic-3.1.1/test/test_public.py
--rw-rw-rw-   0 root         (0) root         (0)      925 2022-09-03 00:43:18.057891 atpublic-3.1.1/tox.ini
--rw-------   0 runner    (1000) runner    (1000)     1812 2022-09-03 00:43:54.018859 atpublic-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0      556 2023-06-01 05:03:16.165251 atpublic-3.1.2/LICENSE
+-rw-r--r--   0        0        0      721 2023-06-01 05:03:16.165251 atpublic-3.1.2/README.rst
+-rw-r--r--   0        0        0     3304 2023-06-01 05:03:16.166251 atpublic-3.1.2/conftest.py
+-rw-r--r--   0        0        0     3148 2023-06-01 05:03:16.166251 atpublic-3.1.2/docs/NEWS.rst
+-rw-r--r--   0        0        0        0 2023-06-01 05:03:16.189250 atpublic-3.1.2/docs/__init__.py
+-rw-r--r--   0        0        0      175 2023-06-01 05:03:16.166251 atpublic-3.1.2/docs/apiref.rst
+-rw-r--r--   0        0        0     7326 2023-06-01 05:03:16.166251 atpublic-3.1.2/docs/conf.py
+-rw-r--r--   0        0        0     2250 2023-06-01 05:03:16.166251 atpublic-3.1.2/docs/index.rst
+-rw-r--r--   0        0        0     8020 2023-06-01 05:03:16.166251 atpublic-3.1.2/docs/using.rst
+-rw-r--r--   0        0        0     2852 2023-06-01 05:03:42.619331 atpublic-3.1.2/pyproject.toml
+-rw-r--r--   0        0        0      509 2023-06-01 05:03:16.167251 atpublic-3.1.2/src/public/__init__.py
+-rw-r--r--   0        0        0      759 2023-06-01 05:03:16.167251 atpublic-3.1.2/src/public/private.py
+-rw-r--r--   0        0        0     3057 2023-06-01 05:03:16.167251 atpublic-3.1.2/src/public/public.py
+-rw-r--r--   0        0        0        0 2023-06-01 05:03:16.189250 atpublic-3.1.2/src/public/py.typed
+-rw-r--r--   0        0        0      107 2023-06-01 05:03:16.167251 atpublic-3.1.2/src/public/types.py
+-rw-r--r--   0        0        0        0 2023-06-01 05:03:16.189250 atpublic-3.1.2/test/__init__.py
+-rw-r--r--   0        0        0      204 2023-06-01 05:03:16.167251 atpublic-3.1.2/test/test_mypy.py
+-rw-r--r--   0        0        0      923 2023-06-01 05:03:16.167251 atpublic-3.1.2/test/test_private.py
+-rw-r--r--   0        0        0     3104 2023-06-01 05:03:16.167251 atpublic-3.1.2/test/test_public.py
+-rw-r--r--   0        0        0      780 2023-06-01 05:03:16.167251 atpublic-3.1.2/tox.ini
+-rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 atpublic-3.1.2/PKG-INFO
```

### Comparing `atpublic-3.1.1/LICENSE` & `atpublic-3.1.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2016-2022 Barry Warsaw
+Copyright 2016-2023 Barry Warsaw
 
 Licensed under the Apache License, Version 2.0 (the "License"); you may not
 use this file except in compliance with the License.  You may obtain a copy of
 the License at
 
 http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `atpublic-3.1.1/README.rst` & `atpublic-3.1.2/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 *publicness* of the names in your module.  They keep your module's ``__all__``
 in sync so you don't have to.
 
 
 Author
 ======
 
-``public`` is Copyright (C) 2016-2022 Barry Warsaw <barry@python.org>
+``public`` is Copyright (C) 2016-2023 Barry Warsaw <barry@python.org>
 
 Licensed under the terms of the Apache License Version 2.0.  See the LICENSE
 file for details.
 
 
 Project details
 ===============
```

### Comparing `atpublic-3.1.1/conftest.py` & `atpublic-3.1.2/conftest.py`

 * *Files identical despite different names*

### Comparing `atpublic-3.1.1/docs/NEWS.rst` & `atpublic-3.1.2/docs/NEWS.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 ==================
 @public change log
 ==================
 
+3.1.2 (2023-05-31)
+==================
+* Switch to ``pdm-backend`` (GL#15)
+* Bump dependencies.
+* More GitLab CI integration improvements.
+
 3.1.1 (2022-09-02)
 ==================
 * Improvements to the GitLab CI integration.
 
 3.1 (2022-08-27)
 ================
 * Fix a typo in pyproject.toml file.
```

### Comparing `atpublic-3.1.1/docs/conf.py` & `atpublic-3.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `atpublic-3.1.1/docs/index.rst` & `atpublic-3.1.2/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
 You can contact the author via barry@python.org.
 
 
 Copyright
 =========
 
-Copyright (C) 2016-2022 Barry A. Warsaw
+Copyright (C) 2016-2023 Barry A. Warsaw
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `atpublic-3.1.1/docs/using.rst` & `atpublic-3.1.2/docs/using.rst`

 * *Files identical despite different names*

### Comparing `atpublic-3.1.1/pyproject.toml` & `atpublic-3.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,29 +23,30 @@
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
 ]
 dependencies = []
 dynamic = []
-version = "3.1.1"
+version = "3.1.2"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.urls]
 "Home Page" = "https://public.readthedocs.io"
 Documentation = "https://public.readthedocs.io"
 Source = "https://gitlab.com/warsaw/public.git"
 "Bug Tracker" = "https://gitlab.com/warsaw/public/issues"
 
 [project.optional-dependencies]
 
 [tool.pdm.version]
-from = "src/public/__init__.py"
+source = "file"
+path = "src/public/__init__.py"
 
 [tool.pdm.build]
 source-includes = [
     "docs/",
     "test/",
     "tox.ini",
     "conftest.py",
@@ -128,10 +129,10 @@
     "pytest",
     "sybil.*",
 ]
 ignore_missing_imports = true
 
 [build-system]
 requires = [
-    "pdm-pep517",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `atpublic-3.1.1/src/public/private.py` & `atpublic-3.1.2/src/public/private.py`

 * *Files identical despite different names*

### Comparing `atpublic-3.1.1/src/public/public.py` & `atpublic-3.1.2/src/public/public.py`

 * *Files identical despite different names*

### Comparing `atpublic-3.1.1/test/test_private.py` & `atpublic-3.1.2/test/test_private.py`

 * *Files identical despite different names*

### Comparing `atpublic-3.1.1/test/test_public.py` & `atpublic-3.1.2/test/test_public.py`

 * *Files identical despite different names*

### Comparing `atpublic-3.1.1/PKG-INFO` & `atpublic-3.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 Metadata-Version: 2.1
 Name: atpublic
-Version: 3.1.1
+Version: 3.1.2
 Summary: Keep all y'all's __all__'s in sync
+Keywords: __all__ public private
+Author-Email: Barry Warsaw <barry@python.org>
 License: Apache-2.0
-Keywords: __all__,public,private
-Author-email: Barry Warsaw <barry@python.org>
-Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Development Status :: 6 - Mature
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Project-URL: Bug Tracker, https://gitlab.com/warsaw/public/issues
+Project-URL: Home page, https://public.readthedocs.io
 Project-URL: Documentation, https://public.readthedocs.io
-Project-URL: Home Page, https://public.readthedocs.io
 Project-URL: Source, https://gitlab.com/warsaw/public.git
+Project-URL: Bug tracker, https://gitlab.com/warsaw/public/issues
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 
 ======================
  @public and @private
 ======================
 
 This library provides two very simple decorators that document the
 *publicness* of the names in your module.  They keep your module's ``__all__``
 in sync so you don't have to.
 
 
 Author
 ======
 
-``public`` is Copyright (C) 2016-2022 Barry Warsaw <barry@python.org>
+``public`` is Copyright (C) 2016-2023 Barry Warsaw <barry@python.org>
 
 Licensed under the terms of the Apache License Version 2.0.  See the LICENSE
 file for details.
 
 
 Project details
 ===============
 
  * Project home: https://gitlab.com/warsaw/public
  * Report bugs at: https://gitlab.com/warsaw/public/issues
  * Code hosting: https://gitlab.com/warsaw/public.git
  * Documentation: https://public.readthedocs.io
  * PyPI: https://pypi.python.org/pypi/atpublic
-
```

