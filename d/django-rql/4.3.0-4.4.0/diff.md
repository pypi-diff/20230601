# Comparing `tmp/django_rql-4.3.0.tar.gz` & `tmp/django_rql-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_rql-4.3.0.tar", max compression
+gzip compressed data, was "django_rql-4.4.0.tar", max compression
```

## Comparing `django_rql-4.3.0.tar` & `django_rql-4.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11348 2023-04-08 10:27:56.283624 django_rql-4.3.0/LICENSE
--rw-r--r--   0        0        0    10678 2023-04-08 10:27:56.287624 django_rql-4.3.0/README.md
--rw-r--r--   0        0        0       64 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/__init__.py
--rw-r--r--   0        0        0     1843 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/_dataclasses.py
--rw-r--r--   0        0        0     2746 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/constants.py
--rw-r--r--   0        0        0      384 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/drf/__init__.py
--rw-r--r--   0        0        0      190 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/drf/_utils.py
--rw-r--r--   0        0        0     4555 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/drf/backend.py
--rw-r--r--   0        0        0     9415 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/drf/compat.py
--rw-r--r--   0        0        0     3102 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/drf/paginations.py
--rw-r--r--   0        0        0     2854 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/drf/serializers.py
--rw-r--r--   0        0        0      137 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/fields.py
--rw-r--r--   0        0        0    45746 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/filter_cls.py
--rw-r--r--   0        0        0        0 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/management/commands/__init__.py
--rw-r--r--   0        0        0     3563 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/management/commands/generate_rql_class.py
--rw-r--r--   0        0        0     8109 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/openapi.py
--rw-r--r--   0        0        0     5613 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/qs.py
--rw-r--r--   0        0        0     6429 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/transformer.py
--rw-r--r--   0        0        0     1953 2023-04-08 10:27:56.287624 django_rql-4.3.0/dj_rql/utils.py
--rw-r--r--   0        0        0     2725 2023-04-08 10:30:13.023930 django_rql-4.3.0/pyproject.toml
--rw-r--r--   0        0        0    12059 1970-01-01 00:00:00.000000 django_rql-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11348 2023-06-01 06:49:12.127819 django_rql-4.4.0/LICENSE
+-rw-r--r--   0        0        0    10918 2023-06-01 06:49:12.127819 django_rql-4.4.0/README.md
+-rw-r--r--   0        0        0       64 2023-06-01 06:49:12.127819 django_rql-4.4.0/dj_rql/__init__.py
+-rw-r--r--   0        0        0     1843 2023-06-01 06:49:12.127819 django_rql-4.4.0/dj_rql/_dataclasses.py
+-rw-r--r--   0        0        0     2746 2023-06-01 06:49:12.127819 django_rql-4.4.0/dj_rql/constants.py
+-rw-r--r--   0        0        0      384 2023-06-01 06:49:12.127819 django_rql-4.4.0/dj_rql/drf/__init__.py
+-rw-r--r--   0        0        0      190 2023-06-01 06:49:12.127819 django_rql-4.4.0/dj_rql/drf/_utils.py
+-rw-r--r--   0        0        0     4555 2023-06-01 06:49:12.127819 django_rql-4.4.0/dj_rql/drf/backend.py
+-rw-r--r--   0        0        0     9415 2023-06-01 06:49:12.127819 django_rql-4.4.0/dj_rql/drf/compat.py
+-rw-r--r--   0        0        0     3102 2023-06-01 06:49:12.127819 django_rql-4.4.0/dj_rql/drf/paginations.py
+-rw-r--r--   0        0        0     2854 2023-06-01 06:49:12.127819 django_rql-4.4.0/dj_rql/drf/serializers.py
+-rw-r--r--   0        0        0      137 2023-06-01 06:49:12.127819 django_rql-4.4.0/dj_rql/fields.py
+-rw-r--r--   0        0        0    47930 2023-06-01 06:49:12.131819 django_rql-4.4.0/dj_rql/filter_cls.py
+-rw-r--r--   0        0        0        0 2023-06-01 06:49:12.131819 django_rql-4.4.0/dj_rql/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-01 06:49:12.131819 django_rql-4.4.0/dj_rql/management/commands/__init__.py
+-rw-r--r--   0        0        0     3563 2023-06-01 06:49:12.131819 django_rql-4.4.0/dj_rql/management/commands/generate_rql_class.py
+-rw-r--r--   0        0        0     8109 2023-06-01 06:49:12.131819 django_rql-4.4.0/dj_rql/openapi.py
+-rw-r--r--   0        0        0     5613 2023-06-01 06:49:12.131819 django_rql-4.4.0/dj_rql/qs.py
+-rw-r--r--   0        0        0     6429 2023-06-01 06:49:12.131819 django_rql-4.4.0/dj_rql/transformer.py
+-rw-r--r--   0        0        0     1953 2023-06-01 06:49:12.131819 django_rql-4.4.0/dj_rql/utils.py
+-rw-r--r--   0        0        0     2926 2023-06-01 06:51:09.761587 django_rql-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0    11993 1970-01-01 00:00:00.000000 django_rql-4.4.0/PKG-INFO
```

### Comparing `django_rql-4.3.0/LICENSE` & `django_rql-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/README.md` & `django_rql-4.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     """
     MODEL - Django ORM model
     FILTERS - List of filters
     EXTENDED_SEARCH_ORM_ROUTES - List of additional Django ORM fields for search
     DISTINCT - Boolean flag, that specifies if queryset must always be DISTINCT
     SELECT - Boolean flag, that specifies if Filter Class supports select operations and queryset optimizations
     OPENAPI_SPECIFICATION - Python class that renders OpenAPI specification
+    MAX_ORDERING_LENGTH_IN_QUERY - Integer max allowed number of provided ordering filters in query ordering expression
+    ALLOWED_ORDERING_PERMUTATIONS_IN_QUERY - Set of tuples of strings to specify a set of allowed ordering permutations
 
     Filters can be set in two ways:
         1) string (default settings are calculated from ORM)
         2) dict (overriding settings for specific cases)
 
     Filter Dict Structure
     {
@@ -266,25 +268,25 @@
     'field': CharField(null=True),
 },
 ```
 
 Development
 ===========
 
-1. Python 3.7+
+1. Python 3.8+
 2. Install poetry: `pip install poetry`
 3. Install dependencies: `poetry install`
 4. We use `isort` library to order and format our imports, and we check it using `flake8-isort` library (automatically on `flake8` run).  
 For convenience you may run `isort .` to order imports.
 5. Run flake8: `poetry run flake8`
 
 Testing
 =======
 
-1. Python 3.7+
+1. Python 3.8+
 2. Install poetry: `pip install poetry`
 3. Install dependencies: `poetry install`
 
 Check code style: `poetry run flake8`
 Run tests: `poetry run pytest`
 
 Tests reports are generated in `tests/reports`.
```

### Comparing `django_rql-4.3.0/dj_rql/_dataclasses.py` & `django_rql-4.4.0/dj_rql/_dataclasses.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/dj_rql/constants.py` & `django_rql-4.4.0/dj_rql/constants.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/dj_rql/drf/backend.py` & `django_rql-4.4.0/dj_rql/drf/backend.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/dj_rql/drf/compat.py` & `django_rql-4.4.0/dj_rql/drf/compat.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/dj_rql/drf/paginations.py` & `django_rql-4.4.0/dj_rql/drf/paginations.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/dj_rql/drf/serializers.py` & `django_rql-4.4.0/dj_rql/drf/serializers.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/dj_rql/filter_cls.py` & `django_rql-4.4.0/dj_rql/filter_cls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #
 #  Copyright © 2023 Ingram Micro Inc. All rights reserved.
 #
 import decimal
 import re
 from collections import defaultdict
 from datetime import datetime
+from itertools import chain
 from typing import Set
 from uuid import uuid4
 
 from django.db.models import (
     ForeignKey,
     ManyToManyField,
     Model,
@@ -54,14 +55,21 @@
     MODEL = None
     """The model this filter is for."""
 
     FILTERS = None
     """A list or tuple of filters definitions."""
 
     EXTENDED_SEARCH_ORM_ROUTES = ()
+    """List of additional Django ORM fields for search."""
+
+    MAX_ORDERING_LENGTH_IN_QUERY = 5
+    """Max allowed number of provided ordering filters in query ordering expression."""
+
+    ALLOWED_ORDERING_PERMUTATIONS_IN_QUERY = None
+    """Property to specify a set of allowed ordering permutations (default `None`)."""
 
     DISTINCT = False
     """If True, a `SELECT DISTINCT` will always be executed (default `False`)."""
 
     SELECT = False
     """If True, this FilterClass supports the `select` operator (default `False`)."""
 
@@ -103,39 +111,52 @@
 
         e = 'Wrong filter settings type for Filter Class.'
         assert (self.FILTERS is None) or isinstance(self.FILTERS, iterable_types), e
 
         e = 'Extended search ORM routes must be iterable.'
         assert isinstance(self.EXTENDED_SEARCH_ORM_ROUTES, iterable_types), e
 
+        e = 'Max ordering length must be integer.'
+        assert isinstance(self.MAX_ORDERING_LENGTH_IN_QUERY, int), e
+
+        perms = self.ALLOWED_ORDERING_PERMUTATIONS_IN_QUERY
+        if perms:
+            e = 'Allowed ordering permutations must be a set of tuples of string filter names.'
+            assert isinstance(perms, set), e
+            assert all(isinstance(t, tuple) for t in perms), e
+            assert all(isinstance(s, str) for s in chain.from_iterable(perms)), e
+
     def _get_init_filters(self):
         return self.FILTERS
 
     def _default_init(self, filters):
         e = 'At least one filter must be set for Filter Class.'
         assert filters, e
 
         self.filters = {}
         self.ordering_filters = set()
         self.search_filters = set()
         self.select_tree = {}
         self.default_exclusions = set()
         self.annotations = {}
+        self.allowed_ordering_permutations = None
 
         self._build_filters(filters)
+        self._validate_and_store_allowed_ordering_permutations()
         self._extend_annotations()
 
     def _init_from_class(self, instance):
         copied_attributes = (
             'filters',
             'ordering_filters',
             'search_filters',
             'select_tree',
             'default_exclusions',
             'annotations',
+            'allowed_ordering_permutations',
         )
         for attr in copied_attributes:
             setattr(self, attr, getattr(instance, attr))
 
     def build_q_for_custom_filter(self, data: FilterArgs) -> Q:
         """Django Q() builder for custom filter.
 
@@ -538,37 +559,53 @@
         return self.__apply_optimizations(
             OptimizationArgs(qs, select_data, node['fields']),
         )
 
     def _apply_ordering(self, qs, properties):
         if len(properties) == 0:
             return qs
-        elif len(properties) > 1:
+
+        if len(properties) > 1:
             raise RQLFilterParsingError(details={
                 'error': 'Bad ordering filter: query can contain only one ordering operation.',
             })
 
+        if len(properties[0]) > self.MAX_ORDERING_LENGTH_IN_QUERY:
+            raise RQLFilterParsingError(details={
+                'error': 'Bad ordering filter: max allowed number is {n}.'.format(
+                    n=self.MAX_ORDERING_LENGTH_IN_QUERY,
+                ),
+            })
+
         ordering_fields = []
+        perm = []
         for prop in properties[0]:
             filter_name, sign = self._get_filter_name_with_sign_for_ordering(prop)
             if filter_name not in self.ordering_filters:
                 raise RQLFilterParsingError(details={
                     'error': 'Bad ordering filter: {0}.'.format(filter_name),
                 })
 
+            perm.append('{0}{1}'.format(sign, filter_name))
             filters = self.filters[filter_name]
             if not isinstance(filters, list):
                 filters = [filters]
             for filter_item in filters:
                 if filter_item.get('distinct'):
                     self._is_distinct = True
 
                 ordering_name = self._get_filter_ordering_name(filter_item, filter_name)
                 ordering_fields.append('{0}{1}'.format(sign, ordering_name))
 
+        perms = self.allowed_ordering_permutations
+        if perms and tuple(perm) not in perms:
+            raise RQLFilterParsingError(details={
+                'error': 'Bad ordering filter: permutation not allowed.',
+            })
+
         return qs.order_by(*ordering_fields)
 
     @staticmethod
     def _get_filter_name_with_sign_for_ordering(prop):
         if RQL_MINUS == prop[0]:
             filter_name = prop[1:]
             sign = RQL_MINUS
@@ -762,14 +799,28 @@
 
                     own_annotation = self.annotations.get(filter_name)
                     if own_annotation:
                         extended_annotations[filter_name].append(own_annotation[0])
 
         self.annotations.update(dict(extended_annotations))
 
+    def _validate_and_store_allowed_ordering_permutations(self):
+        perms = self.ALLOWED_ORDERING_PERMUTATIONS_IN_QUERY
+        if perms:
+            for s in chain.from_iterable(perms):
+                filter_name = s[1:] if s and s[0] in ('+', '-') else s
+
+                e = 'Wrong configuration of allowed ordering permutations: {n}.'.format(n=s)
+                assert filter_name in self.ordering_filters, e
+
+            self.allowed_ordering_permutations = {
+                tuple(s[1:] if s[0] == '+' else s for s in t)
+                for t in perms
+            }
+
     @classmethod
     def _is_field_supported(cls, field):
         return isinstance(field, SUPPORTED_FIELD_TYPES)
 
     @classmethod
     def _get_field_related_model(cls, field):
         return field.related_model
```

### Comparing `django_rql-4.3.0/dj_rql/management/commands/generate_rql_class.py` & `django_rql-4.4.0/dj_rql/management/commands/generate_rql_class.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/dj_rql/openapi.py` & `django_rql-4.4.0/dj_rql/openapi.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/dj_rql/qs.py` & `django_rql-4.4.0/dj_rql/qs.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/dj_rql/transformer.py` & `django_rql-4.4.0/dj_rql/transformer.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/dj_rql/utils.py` & `django_rql-4.4.0/dj_rql/utils.py`

 * *Files identical despite different names*

### Comparing `django_rql-4.3.0/pyproject.toml` & `django_rql-4.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-rql"
-version = "4.3.0"
+version = "4.4.0"
 description = "Django RQL Filtering"
 authors = ["Ingram Micro"]
 license = "Apache-2.0"
 packages = [
     { include = "dj_rql" }
 ]
 readme = "./README.md"
@@ -15,15 +15,14 @@
     'Framework :: Django :: 3.2',
     'Framework :: Django :: 4.0',
     'Framework :: Django :: 4.1',
     'Framework :: Django :: 4.2',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: Apache Software License',
     'Operating System :: Unix',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Topic :: Text Processing :: Filters',
 ]
 keywords = [
@@ -31,30 +30,31 @@
     "rql",
     "filter",
     "rest",
     "api",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4"
-lib-rql = "^1.1.5"
+python = ">=3.8,<4"
 django = ">=3.2"
+lib-rql = "^2.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = ">=7.2.0,<8"
 pytest-cov = ">=2.10.1,<5"
 pytest-mock = "^3.3.1"
-coverage = {extras = ["toml"], version = ">=5.3,<7"}
+coverage = "^7"
 flake8 = ">=3.8,<6"
 flake8-bugbear = ">=20,<23"
 flake8-cognitive-complexity = "^0.1"
 flake8-commas = "~2.1"
 flake8-future-import = "~0.4"
 flake8-isort = "^5.0"
 flake8-broken-line = ">=0.3,<0.7"
+flake8-pyproject = "^1.2.3"
 pytest-django = ">=4.4.0"
 djangorestframework = ">=3.12"
 isort = "^5.10"
 importlib-metadata = "<5"
 django-fsm = ">=2.7.1"
 django-model-utils = ">=3.2.0"
 uritemplate = "^4.1.1"
@@ -98,7 +98,23 @@
 multi_line_output = 3
 force_grid_wrap = 4
 combine_as_imports = true
 use_parentheses = true
 include_trailing_comma = true
 line_length = 100
 lines_after_imports = 2
+
+[tool.flake8]
+exclude = [
+    ".idea",
+    ".vscode",
+    ".git",
+    "pg_data",
+    "venv",
+    "*.eggs",
+    "*.egg",
+    "_generated_filters*.py",
+]
+show-source = true
+max-line-length = 100
+max-cognitive-complexity = 20
+ignore = ["FI1", "W503", "W605"]
```

### Comparing `django_rql-4.3.0/PKG-INFO` & `django_rql-4.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 Metadata-Version: 2.1
 Name: django-rql
-Version: 4.3.0
+Version: 4.4.0
 Summary: Django RQL Filtering
 Home-page: https://connect.cloudblue.com/community/api/rql/
 License: Apache-2.0
 Keywords: django,rql,filter,rest,api
 Author: Ingram Micro
-Requires-Python: >=3.7,<4
+Requires-Python: >=3.8,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Text Processing :: Filters
 Requires-Dist: django (>=3.2)
-Requires-Dist: lib-rql (>=1.1.5,<2.0.0)
+Requires-Dist: lib-rql (>=2.0,<3.0)
 Project-URL: Repository, https://github.com/cloudblue/django-rql
 Description-Content-Type: text/markdown
 
 Django RQL
 ==========
 [![pyversions](https://img.shields.io/pypi/pyversions/django-rql.svg)](https://pypi.org/project/django-rql/)
 [![PyPi Status](https://img.shields.io/pypi/v/django-rql.svg)](https://pypi.org/project/django-rql/)
@@ -86,14 +80,16 @@
     """
     MODEL - Django ORM model
     FILTERS - List of filters
     EXTENDED_SEARCH_ORM_ROUTES - List of additional Django ORM fields for search
     DISTINCT - Boolean flag, that specifies if queryset must always be DISTINCT
     SELECT - Boolean flag, that specifies if Filter Class supports select operations and queryset optimizations
     OPENAPI_SPECIFICATION - Python class that renders OpenAPI specification
+    MAX_ORDERING_LENGTH_IN_QUERY - Integer max allowed number of provided ordering filters in query ordering expression
+    ALLOWED_ORDERING_PERMUTATIONS_IN_QUERY - Set of tuples of strings to specify a set of allowed ordering permutations
 
     Filters can be set in two ways:
         1) string (default settings are calculated from ORM)
         2) dict (overriding settings for specific cases)
 
     Filter Dict Structure
     {
@@ -300,25 +296,25 @@
     'field': CharField(null=True),
 },
 ```
 
 Development
 ===========
 
-1. Python 3.7+
+1. Python 3.8+
 2. Install poetry: `pip install poetry`
 3. Install dependencies: `poetry install`
 4. We use `isort` library to order and format our imports, and we check it using `flake8-isort` library (automatically on `flake8` run).  
 For convenience you may run `isort .` to order imports.
 5. Run flake8: `poetry run flake8`
 
 Testing
 =======
 
-1. Python 3.7+
+1. Python 3.8+
 2. Install poetry: `pip install poetry`
 3. Install dependencies: `poetry install`
 
 Check code style: `poetry run flake8`
 Run tests: `poetry run pytest`
 
 Tests reports are generated in `tests/reports`.
```

