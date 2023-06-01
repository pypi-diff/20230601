# Comparing `tmp/jaraco.collections-4.1.0.tar.gz` & `tmp/jaraco.collections-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.collections-4.1.0.tar", last modified: Thu Apr  6 10:18:56 2023, max compression
+gzip compressed data, was "jaraco.collections-4.2.0.tar", last modified: Thu Jun  1 14:09:51 2023, max compression
```

## Comparing `jaraco.collections-4.1.0.tar` & `jaraco.collections-4.2.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:18:56.609048 jaraco.collections-4.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:18:56.609048 jaraco.collections-4.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:18:56.609048 jaraco.collections-4.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-06 10:18:56.609048 jaraco.collections-4.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:18:56.609048 jaraco.collections-4.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:18:56.609048 jaraco.collections-4.1.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)    26507 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/jaraco/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:18:56.609048 jaraco.collections-4.1.0/jaraco.collections.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-04-06 10:18:56.000000 jaraco.collections-4.1.0/jaraco.collections.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-06 10:18:56.000000 jaraco.collections-4.1.0/jaraco.collections.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 10:18:56.000000 jaraco.collections-4.1.0/jaraco.collections.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-06 10:18:56.000000 jaraco.collections-4.1.0/jaraco.collections.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-06 10:18:56.000000 jaraco.collections-4.1.0/jaraco.collections.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-06 10:18:56.609048 jaraco.collections-4.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 10:18:56.609048 jaraco.collections-4.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-06 10:18:34.000000 jaraco.collections-4.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (123)    26928 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/jaraco/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/jaraco.collections.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-06-01 14:09:51.000000 jaraco.collections-4.2.0/jaraco.collections.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-01 14:09:51.000000 jaraco.collections-4.2.0/jaraco.collections.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 14:09:51.000000 jaraco.collections-4.2.0/jaraco.collections.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-01 14:09:51.000000 jaraco.collections-4.2.0/jaraco.collections.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 14:09:51.000000 jaraco.collections-4.2.0/jaraco.collections.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-06-01 14:09:51.867082 jaraco.collections-4.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 14:09:51.863082 jaraco.collections-4.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-01 14:09:29.000000 jaraco.collections-4.2.0/tox.ini
```

### Comparing `jaraco.collections-4.1.0/.github/workflows/main.yml` & `jaraco.collections-4.2.0/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: tests
 
 on: [push, pull_request]
 
+permissions:
+  contents: read
+
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
   # to a non-empty value is sufficient. For tox, it must be one of
   # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
@@ -100,14 +103,16 @@
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `jaraco.collections-4.1.0/CHANGES.rst` & `jaraco.collections-4.2.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v4.2.0
+======
+
+Added ``Mask``, the inverse of a ``Projection``.
+
 v4.1.0
 ======
 
 ``Projection`` now accepts an iterable or callable or pattern
 for matching keys.
 
 ``Projection`` now retains order of keys from the underlying
```

### Comparing `jaraco.collections-4.1.0/LICENSE` & `jaraco.collections-4.2.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.collections-4.1.0/PKG-INFO` & `jaraco.collections-4.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.collections
-Version: 4.1.0
+Version: 4.2.0
 Summary: Collection objects similar to those in stdlib by jaraco
 Home-page: https://github.com/jaraco/jaraco.collections
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,14 @@
 
 See the docs, linked above, for descriptions and usage examples.
 
 Highlights include:
 
 - RangeMap: A mapping that accepts a range of values for keys.
 - Projection: A subset over an existing mapping.
-- DictFilter: A different implementation of a projection.
 - KeyTransformingDict: Generalized mapping with keys transformed by a function.
 - FoldedCaseKeyedDict: A dict whose string keys are case-insensitive.
 - BijectiveMap: A map where keys map to values and values back to their keys.
 - ItemsAsAttributes: A mapping mix-in exposing items as attributes.
 - IdentityOverrideMap: A map whose keys map by default to themselves unless overridden.
 - FrozenDict: A hashable, immutable map.
 - Enumeration: An object whose keys are enumerated.
```

### Comparing `jaraco.collections-4.1.0/README.rst` & `jaraco.collections-4.2.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 See the docs, linked above, for descriptions and usage examples.
 
 Highlights include:
 
 - RangeMap: A mapping that accepts a range of values for keys.
 - Projection: A subset over an existing mapping.
-- DictFilter: A different implementation of a projection.
 - KeyTransformingDict: Generalized mapping with keys transformed by a function.
 - FoldedCaseKeyedDict: A dict whose string keys are case-insensitive.
 - BijectiveMap: A map where keys map to values and values back to their keys.
 - ItemsAsAttributes: A mapping mix-in exposing items as attributes.
 - IdentityOverrideMap: A map whose keys map by default to themselves unless overridden.
 - FrozenDict: A hashable, immutable map.
 - Enumeration: An object whose keys are enumerated.
```

### Comparing `jaraco.collections-4.1.0/docs/conf.py` & `jaraco.collections-4.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.collections-4.1.0/jaraco/collections.py` & `jaraco.collections-4.2.0/jaraco/collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,30 @@
     def __iter__(self):
         return self._keys_resolved()
 
     def __len__(self):
         return len(tuple(self._keys_resolved()))
 
 
+class Mask(Projection):
+    """
+    The inverse of a projection, masking out keys.
+
+    >>> sample = {'a': 1, 'b': 2, 'c': 3}
+    >>> msk = Mask(['a', 'c', 'd'], sample)
+    >>> dict(msk)
+    {'b': 2}
+    """
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        # self._match = compose(operator.not_, self._match)
+        self._match = lambda key, orig=self._match: not orig(key)
+
+
 class DictFilter(Projection):
     """
     *Deprecated*
 
     Takes a dict and simulates a sub-dict based on a pattern.
 
     >>> sample = dict(a=1, b=2, c=3, d=4, ef=5)
```

### Comparing `jaraco.collections-4.1.0/jaraco.collections.egg-info/PKG-INFO` & `jaraco.collections-4.2.0/jaraco.collections.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.collections
-Version: 4.1.0
+Version: 4.2.0
 Summary: Collection objects similar to those in stdlib by jaraco
 Home-page: https://github.com/jaraco/jaraco.collections
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -41,15 +41,14 @@
 
 See the docs, linked above, for descriptions and usage examples.
 
 Highlights include:
 
 - RangeMap: A mapping that accepts a range of values for keys.
 - Projection: A subset over an existing mapping.
-- DictFilter: A different implementation of a projection.
 - KeyTransformingDict: Generalized mapping with keys transformed by a function.
 - FoldedCaseKeyedDict: A dict whose string keys are case-insensitive.
 - BijectiveMap: A map where keys map to values and values back to their keys.
 - ItemsAsAttributes: A mapping mix-in exposing items as attributes.
 - IdentityOverrideMap: A map whose keys map by default to themselves unless overridden.
 - FrozenDict: A hashable, immutable map.
 - Enumeration: An object whose keys are enumerated.
```

### Comparing `jaraco.collections-4.1.0/jaraco.collections.egg-info/SOURCES.txt` & `jaraco.collections-4.2.0/jaraco.collections.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.rst
 LICENSE
 README.rst
 mypy.ini
 pyproject.toml
```

### Comparing `jaraco.collections-4.1.0/pytest.ini` & `jaraco.collections-4.2.0/pytest.ini`

 * *Files 26% similar despite different names*

```diff
@@ -3,32 +3,27 @@
 addopts=--doctest-modules --import-mode=importlib
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
-	# Suppress deprecation warning in flake8
-	ignore:SelectableGroups dict interface is deprecated::flake8
-
 	# shopkeep/pytest-black#55
 	ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
 	ignore:The \(fspath. py.path.local\) argument to BlackItem is deprecated.:pytest.PytestDeprecationWarning
 	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
 
-	# tholo/pytest-flake8#83
-	ignore:<class 'pytest_flake8.Flake8Item'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
-	ignore:The \(fspath. py.path.local\) argument to Flake8Item is deprecated.:pytest.PytestDeprecationWarning
-	ignore:Flake8Item is an Item subclass and should not be a collector:pytest.PytestWarning
-
 	# shopkeep/pytest-black#67
 	ignore:'encoding' argument not specified::pytest_black
 
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
+	# pypa/build#615
+	ignore:'encoding' argument not specified::build.env
+
 	## end upstream
 
 	ignore:DictFilter is deprecated
```

### Comparing `jaraco.collections-4.1.0/setup.cfg` & `jaraco.collections-4.2.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -26,23 +26,21 @@
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.3
+	pytest-ruff
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
```

### Comparing `jaraco.collections-4.1.0/tests/test_collections.py` & `jaraco.collections-4.2.0/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `jaraco.collections-4.1.0/tox.ini` & `jaraco.collections-4.2.0/tox.ini`

 * *Files identical despite different names*

