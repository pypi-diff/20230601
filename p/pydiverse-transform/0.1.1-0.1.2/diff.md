# Comparing `tmp/pydiverse-transform-0.1.1.tar.gz` & `tmp/pydiverse_transform-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse-transform-0.1.1.tar", max compression
+gzip compressed data, was "pydiverse_transform-0.1.2.tar", max compression
```

## Comparing `pydiverse-transform-0.1.1.tar` & `pydiverse_transform-0.1.2.tar`

### file list

```diff
@@ -1,41 +1,40 @@
--rw-r--r--   0        0        0     1517 2022-08-30 10:14:23.006505 pydiverse-transform-0.1.1/LICENSE
--rw-r--r--   0        0        0     2325 2023-05-04 15:21:08.375883 pydiverse-transform-0.1.1/docs/package/README.md
--rw-r--r--   0        0        0     1806 2023-05-04 15:21:54.335822 pydiverse-transform-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       13 2022-09-15 12:24:32.275027 pydiverse-transform-0.1.1/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      387 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/__init__.py
--rw-r--r--   0        0        0      108 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/__init__.py
--rw-r--r--   0        0        0     3470 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/alignment.py
--rw-r--r--   0        0        0     2797 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/column.py
--rw-r--r--   0        0        0     5082 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/dispatchers.py
--rw-r--r--   0        0        0      191 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/__init__.py
--rw-r--r--   0        0        0     1078 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/expressions.py
--rw-r--r--   0        0        0      682 2022-09-15 12:24:32.275027 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/lambda_getter.py
--rw-r--r--   0        0        0     4871 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/symbolic_expressions.py
--rw-r--r--   0        0        0     4881 2023-05-04 13:58:19.766398 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/translator.py
--rw-r--r--   0        0        0     1708 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/util.py
--rw-r--r--   0        0        0      530 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/functions.py
--rw-r--r--   0        0        0      135 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/__init__.py
--rw-r--r--   0        0        0      903 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/aggregate.py
--rw-r--r--   0        0        0     3590 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/core.py
--rw-r--r--   0        0        0     1694 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/logical.py
--rw-r--r--   0        0        0     2341 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/numeric.py
--rw-r--r--   0        0        0    17847 2022-09-15 12:24:32.275027 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/registry.py
--rw-r--r--   0        0        0      518 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/string.py
--rw-r--r--   0        0        0      334 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/window.py
--rw-r--r--   0        0        0     3833 2023-05-04 13:58:19.758398 pydiverse-transform-0.1.1/src/pydiverse/transform/core/table.py
--rw-r--r--   0        0        0    16536 2023-05-04 13:58:19.802398 pydiverse-transform-0.1.1/src/pydiverse/transform/core/table_impl.py
--rw-r--r--   0        0        0       84 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/__init__.py
--rw-r--r--   0        0        0     2637 2023-05-04 13:58:24.130390 pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/bidict.py
--rw-r--r--   0        0        0     1161 2023-05-04 13:58:19.750398 pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/ordered_set.py
--rw-r--r--   0        0        0     1892 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/util.py
--rw-r--r--   0        0        0    14653 2023-05-04 13:58:19.790398 pydiverse-transform-0.1.1/src/pydiverse/transform/core/verbs.py
--rw-r--r--   0        0        0       42 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/eager/__init__.py
--rw-r--r--   0        0        0      265 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/eager/eager_table.py
--rw-r--r--   0        0        0    21007 2022-09-15 12:24:32.279027 pydiverse-transform-0.1.1/src/pydiverse/transform/eager/pandas_table.py
--rw-r--r--   0        0        0       36 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/lazy/__init__.py
--rw-r--r--   0        0        0      454 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/lazy/lazy_table.py
--rw-r--r--   0        0        0    26997 2023-05-04 14:24:43.368130 pydiverse-transform-0.1.1/src/pydiverse/transform/lazy/sql_table.py
--rw-r--r--   0        0        0        0 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/util/__init__.py
--rw-r--r--   0        0        0      730 2022-08-30 10:14:23.010505 pydiverse-transform-0.1.1/src/pydiverse/transform/util/testing.py
--rw-r--r--   0        0        0     3600 2023-05-04 15:24:47.800589 pydiverse-transform-0.1.1/setup.py
--rw-r--r--   0        0        0     3322 2023-05-04 15:24:47.800854 pydiverse-transform-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-05-22 14:59:50.867488 pydiverse_transform-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2325 2023-06-01 15:40:30.967225 pydiverse_transform-0.1.2/docs/package/README.md
+-rw-r--r--   0        0        0     1471 2023-06-01 15:44:26.899777 pydiverse_transform-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-05-22 14:59:50.868554 pydiverse_transform-0.1.2/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      387 2023-05-22 14:59:50.868629 pydiverse_transform-0.1.2/src/pydiverse/transform/__init__.py
+-rw-r--r--   0        0        0      108 2023-05-22 14:59:50.868774 pydiverse_transform-0.1.2/src/pydiverse/transform/core/__init__.py
+-rw-r--r--   0        0        0     3470 2023-05-22 14:59:50.868845 pydiverse_transform-0.1.2/src/pydiverse/transform/core/alignment.py
+-rw-r--r--   0        0        0     2797 2023-06-01 15:42:26.018480 pydiverse_transform-0.1.2/src/pydiverse/transform/core/column.py
+-rw-r--r--   0        0        0     5082 2023-05-22 14:59:50.868981 pydiverse_transform-0.1.2/src/pydiverse/transform/core/dispatchers.py
+-rw-r--r--   0        0        0      191 2023-05-22 14:59:50.869098 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/__init__.py
+-rw-r--r--   0        0        0     1078 2023-05-22 14:59:50.869154 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/expressions.py
+-rw-r--r--   0        0        0      682 2023-05-22 14:59:50.869206 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/lambda_getter.py
+-rw-r--r--   0        0        0     4871 2023-05-22 14:59:50.869290 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/symbolic_expressions.py
+-rw-r--r--   0        0        0     4881 2023-06-01 15:42:26.956127 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/translator.py
+-rw-r--r--   0        0        0     1708 2023-06-01 15:42:55.420078 pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/util.py
+-rw-r--r--   0        0        0      530 2023-05-22 14:59:50.869466 pydiverse_transform-0.1.2/src/pydiverse/transform/core/functions.py
+-rw-r--r--   0        0        0      135 2023-05-22 14:59:50.869536 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/__init__.py
+-rw-r--r--   0        0        0      903 2023-05-22 14:59:50.869588 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/aggregate.py
+-rw-r--r--   0        0        0     3590 2023-06-01 15:42:55.420238 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/core.py
+-rw-r--r--   0        0        0     1694 2023-05-22 14:59:50.869690 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/logical.py
+-rw-r--r--   0        0        0     2341 2023-05-22 14:59:50.869745 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/numeric.py
+-rw-r--r--   0        0        0    17847 2023-06-01 15:42:55.420630 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/registry.py
+-rw-r--r--   0        0        0      518 2023-05-22 14:59:50.869940 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/string.py
+-rw-r--r--   0        0        0      334 2023-05-22 14:59:50.870004 pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/window.py
+-rw-r--r--   0        0        0     3833 2023-06-01 15:42:55.420907 pydiverse_transform-0.1.2/src/pydiverse/transform/core/table.py
+-rw-r--r--   0        0        0    16536 2023-06-01 15:42:55.421102 pydiverse_transform-0.1.2/src/pydiverse/transform/core/table_impl.py
+-rw-r--r--   0        0        0       84 2023-05-22 14:59:50.870262 pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/__init__.py
+-rw-r--r--   0        0        0     2637 2023-06-01 15:42:55.421445 pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/bidict.py
+-rw-r--r--   0        0        0     1161 2023-06-01 15:42:55.421699 pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/ordered_set.py
+-rw-r--r--   0        0        0     1892 2023-05-22 14:59:50.870440 pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/util.py
+-rw-r--r--   0        0        0    14653 2023-06-01 15:42:55.421911 pydiverse_transform-0.1.2/src/pydiverse/transform/core/verbs.py
+-rw-r--r--   0        0        0       42 2023-05-22 14:59:50.870617 pydiverse_transform-0.1.2/src/pydiverse/transform/eager/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-22 14:59:50.870681 pydiverse_transform-0.1.2/src/pydiverse/transform/eager/eager_table.py
+-rw-r--r--   0        0        0    21007 2023-06-01 15:42:55.422346 pydiverse_transform-0.1.2/src/pydiverse/transform/eager/pandas_table.py
+-rw-r--r--   0        0        0       36 2023-05-22 14:59:50.870868 pydiverse_transform-0.1.2/src/pydiverse/transform/lazy/__init__.py
+-rw-r--r--   0        0        0      454 2023-05-22 14:59:50.870935 pydiverse_transform-0.1.2/src/pydiverse/transform/lazy/lazy_table.py
+-rw-r--r--   0        0        0    26997 2023-06-01 15:42:55.422749 pydiverse_transform-0.1.2/src/pydiverse/transform/lazy/sql_table.py
+-rw-r--r--   0        0        0        0 2023-05-22 14:59:50.871139 pydiverse_transform-0.1.2/src/pydiverse/transform/util/__init__.py
+-rw-r--r--   0        0        0      730 2023-06-01 15:32:07.608144 pydiverse_transform-0.1.2/src/pydiverse/transform/util/testing.py
+-rw-r--r--   0        0        0     3154 1970-01-01 00:00:00.000000 pydiverse_transform-0.1.2/PKG-INFO
```

### Comparing `pydiverse-transform-0.1.1/LICENSE` & `pydiverse_transform-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/docs/package/README.md` & `pydiverse_transform-0.1.2/docs/package/README.md`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/pyproject.toml` & `pydiverse_transform-0.1.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydiverse-transform"
-version = "0.1.1"
+version = "0.1.2"
 description = "Pipe based dataframe manipulation library that can also transform data on SQL databases"
 authors = [
   "QuantCo, Inc.",
   "Nicolas Camenisch <garnele007@gmail.com>",
   "Martin Trautmann <windiana@users.sf.net>",
 ]
 license = "BSD-3-Clause"
@@ -17,52 +17,47 @@
   "Intended Audience :: Developers",
   "Intended Audience :: Science/Research",
   "Programming Language :: SQL",
   "Topic :: Database",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.12"
+python = ">=3.9"
 numpy = ">=1.23.1"
 pandas = ">=1.4.3"
 SQLAlchemy = ">=1.4.27"
 
-Sphinx = { version = "^5.1.1", optional = true }
-sphinx-rtd-theme = { version = "^1.0.0", optional = true }
-sphinxcontrib-apidoc = { version="^0.3.0", optional = true }
-# bigquery currently does not support sqlalchemy 2.0
-#sqlalchemy-bigquery = { version=">=1.4.4", optional = true }
-#google-auth = { version=">=2.9.1", optional = true }
-
-[tool.poetry.extras]
-docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-apidoc"]
-#bigquery = ["sqlalchemy-bigquery", "google-auth"]
-
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = ">=7.1.2"
 pytest-xdist = ">=2.5.0"
 psycopg2 = ">=2.9.3"
-black = "^23.3.0"
+black = "23.3.0"
 isort = "^5.10.1"
-pre-commit = ">=2.20.0"
-pyodbc = ">=4.0.34"
+pre-commit = "^3.3.0"
+pyodbc = "^4.0.34"
+
+[tool.poetry.group.docs]
+optional = true
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = "^5.1.1"
+sphinx-rtd-theme = "^1.0.0"
+sphinxcontrib-apidoc = "^0.3.0"
 
 [tool.black]
 exclude = '''
 /(
     \.eggs
   | \.git
   | \.venv
   | build
   | dist
 )/
 '''
 
-preview = true
-
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
 ensure_newline_before_comments = true
 line_length = 88
 known_first_party = "pydiverse.transform"
 skip_glob = '\.eggs/*,\.git/*,\.venv/*,build/*,dist/*'
```

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/alignment.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/alignment.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/column.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/column.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/dispatchers.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/dispatchers.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/expressions.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/expressions.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/lambda_getter.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/lambda_getter.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/symbolic_expressions.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/symbolic_expressions.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/translator.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/translator.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/expressions/util.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/expressions/util.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/functions.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/functions.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/aggregate.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/aggregate.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/core.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/core.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/logical.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/logical.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/numeric.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/numeric.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/registry.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/registry.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/ops/string.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/ops/string.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/table.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/table.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/table_impl.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/table_impl.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/bidict.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/bidict.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/ordered_set.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/util/util.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/util/util.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/core/verbs.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/core/verbs.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/eager/pandas_table.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/eager/pandas_table.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/lazy/sql_table.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/lazy/sql_table.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/src/pydiverse/transform/util/testing.py` & `pydiverse_transform-0.1.2/src/pydiverse/transform/util/testing.py`

 * *Files identical despite different names*

### Comparing `pydiverse-transform-0.1.1/PKG-INFO` & `pydiverse_transform-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 Metadata-Version: 2.1
 Name: pydiverse-transform
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pipe based dataframe manipulation library that can also transform data on SQL databases
 License: BSD-3-Clause
 Author: QuantCo, Inc.
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
-Provides-Extra: docs
 Requires-Dist: SQLAlchemy (>=1.4.27)
-Requires-Dist: Sphinx (>=5.1.1,<6.0.0); extra == "docs"
 Requires-Dist: numpy (>=1.23.1)
 Requires-Dist: pandas (>=1.4.3)
-Requires-Dist: sphinx-rtd-theme (>=1.0.0,<2.0.0); extra == "docs"
-Requires-Dist: sphinxcontrib-apidoc (>=0.3.0,<0.4.0); extra == "docs"
 Description-Content-Type: text/markdown
 
 # pydiverse.transform
 
 [![CI](https://github.com/pydiverse/pydiverse.transform/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.transform/actions/workflows/ci.yml)
 
 Pipe based dataframe manipulation library that can also transform data on SQL databases
```

