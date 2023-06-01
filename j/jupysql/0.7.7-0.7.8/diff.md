# Comparing `tmp/jupysql-0.7.7.tar.gz` & `tmp/jupysql-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupysql-0.7.7.tar", last modified: Wed May 31 15:14:54 2023, max compression
+gzip compressed data, was "jupysql-0.7.8.tar", last modified: Thu Jun  1 17:36:52 2023, max compression
```

## Comparing `jupysql-0.7.7.tar` & `jupysql-0.7.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-05-31 15:14:33.000000 jupysql-0.7.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-31 15:14:33.000000 jupysql-0.7.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-31 15:14:54.096138 jupysql-0.7.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-31 15:14:33.000000 jupysql-0.7.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-31 15:14:33.000000 jupysql-0.7.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-31 15:14:54.096138 jupysql-0.7.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-31 15:14:33.000000 jupysql-0.7.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.080138 jupysql-0.7.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.088138 jupysql-0.7.7/src/jupysql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-31 15:14:53.000000 jupysql-0.7.7/src/jupysql.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.092138 jupysql-0.7.7/src/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/column_guesser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    21805 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/error_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.092138 jupysql-0.7.7/src/sql/ggplot/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/aes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/facet_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/src/sql/ggplot/geom/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/geom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/geom/geom.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/geom/geom_boxplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/geom/geom_histogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/ggplot/ggplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/magic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/magic_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/magic_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)    16139 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/store.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/src/sql/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/src/sql/widgets/table_widget/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/table_widget/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/src/sql/widgets/table_widget/css/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/table_widget/css/tableWidget.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 15:14:54.096138 jupysql-0.7.7/src/sql/widgets/table_widget/js/
--rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/table_widget/js/tableWidget.js
--rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/table_widget/table_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-31 15:14:33.000000 jupysql-0.7.7/src/sql/widgets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11820 2023-06-01 17:36:31.000000 jupysql-0.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-01 17:36:31.000000 jupysql-0.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-01 17:36:52.236551 jupysql-0.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-01 17:36:31.000000 jupysql-0.7.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-01 17:36:31.000000 jupysql-0.7.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-01 17:36:52.236551 jupysql-0.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-01 17:36:31.000000 jupysql-0.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.228551 jupysql-0.7.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.232551 jupysql-0.7.8/src/jupysql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-01 17:36:51.000000 jupysql-0.7.8/src/jupysql.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.232551 jupysql-0.7.8/src/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11971 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/column_guesser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21805 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/ggplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/aes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/facet_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/ggplot/geom/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/geom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/geom/geom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/geom/geom_boxplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/geom/geom_histogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/ggplot/ggplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10405 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18100 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/magic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9568 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/magic_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/magic_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24145 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18171 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5110 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/widgets/table_widget/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/table_widget/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/widgets/table_widget/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/table_widget/css/tableWidget.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 17:36:52.236551 jupysql-0.7.8/src/sql/widgets/table_widget/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    13523 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/table_widget/js/tableWidget.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5449 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/table_widget/table_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-01 17:36:31.000000 jupysql-0.7.8/src/sql/widgets/utils.py
```

### Comparing `jupysql-0.7.7/LICENSE` & `jupysql-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/PKG-INFO` & `jupysql-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.7
+Version: 0.7.8
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.7 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.8 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.7/README.md` & `jupysql-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/pyproject.toml` & `jupysql-0.7.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/setup.py` & `jupysql-0.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/jupysql.egg-info/PKG-INFO` & `jupysql-0.7.8/src/jupysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupysql
-Version: 0.7.7
+Version: 0.7.8
 Summary: Better SQL in Jupyter
 Home-page: https://github.com/ploomber/jupysql
 Author: Ploomber
 Author-email: contact@ploomber.io
 Project-URL: Source, https://github.com/ploomber/jupysql
 Keywords: database ipython postgresql mysql duckdb
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jupysql Version: 0.7.7 Summary: Better SQL in
+Metadata-Version: 2.1 Name: jupysql Version: 0.7.8 Summary: Better SQL in
 Jupyter Home-page: https://github.com/ploomber/jupysql Author: Ploomber Author-
 email: contact@ploomber.io Project-URL: Source, https://github.com/ploomber/
 jupysql Keywords: database ipython postgresql mysql duckdb Classifier:
 Development Status :: 3 - Alpha Classifier: Environment :: Console Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Topic ::
 Database Classifier: Topic :: Database :: Front-Ends Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `jupysql-0.7.7/src/jupysql.egg-info/SOURCES.txt` & `jupysql-0.7.8/src/jupysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/jupysql.egg-info/requires.txt` & `jupysql-0.7.8/src/jupysql.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/_patch.py` & `jupysql-0.7.8/src/sql/_patch.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/_testing.py` & `jupysql-0.7.8/src/sql/_testing.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/column_guesser.py` & `jupysql-0.7.8/src/sql/column_guesser.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/command.py` & `jupysql-0.7.8/src/sql/command.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/connection.py` & `jupysql-0.7.8/src/sql/connection.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/display.py` & `jupysql-0.7.8/src/sql/display.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/error_message.py` & `jupysql-0.7.8/src/sql/error_message.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/exceptions.py` & `jupysql-0.7.8/src/sql/exceptions.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/ggplot/facet_wrap.py` & `jupysql-0.7.8/src/sql/ggplot/facet_wrap.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/ggplot/geom/geom_histogram.py` & `jupysql-0.7.8/src/sql/ggplot/geom/geom_histogram.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/ggplot/ggplot.py` & `jupysql-0.7.8/src/sql/ggplot/ggplot.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/inspect.py` & `jupysql-0.7.8/src/sql/inspect.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/magic.py` & `jupysql-0.7.8/src/sql/magic.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/magic_cmd.py` & `jupysql-0.7.8/src/sql/magic_cmd.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/parse.py` & `jupysql-0.7.8/src/sql/parse.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/plot.py` & `jupysql-0.7.8/src/sql/plot.py`

 * *Files 24% similar despite different names*

```diff
@@ -601,7 +601,330 @@
         filter_query=filter_query,
         cases=cases,
     )
 
     data = conn.execute(query, with_).fetchall()
 
     return data
+
+
+@modify_exceptions
+def _bar(table, column, with_=None, conn=None):
+    """get x and height for bar plot"""
+    if not conn:
+        conn = sql.connection.Connection.current
+    use_backticks = conn.is_use_backtick_template()
+
+    if isinstance(column, list):
+        if len(column) > 2:
+            raise exceptions.UsageError(
+                f"Passed columns: {column}\n"
+                "Bar chart currently supports, either a single column"
+                " on which group by and count is applied or"
+                " two columns: labels and size"
+            )
+
+        x_ = column[0]
+        height_ = column[1]
+
+        print(f"Removing NULLs, if there exists any from {x_} and {height_}")
+        template_ = """
+            select "{{x_}}" as x,
+            "{{height_}}" as height
+            from "{{table}}"
+            where "{{x_}}" is not null
+            and "{{height_}}" is not null;
+            """
+
+        xlabel = x_
+        ylabel = height_
+
+        if use_backticks:
+            template_ = template_.replace('"', "`")
+
+        template = Template(template_)
+        query = template.render(table=table, x_=x_, height_=height_)
+
+    else:
+        print(f"Removing NULLs, if there exists any from {column}")
+        template_ = """
+                select "{{column}}" as x,
+                count("{{column}}") as height
+                from "{{table}}"
+                where "{{column}}" is not null
+                group by "{{column}}";
+                """
+
+        xlabel = column
+        ylabel = "Count"
+
+        if use_backticks:
+            template_ = template_.replace('"', "`")
+
+        template = Template(template_)
+        query = template.render(table=table, column=column)
+
+    data = conn.execute(query, with_).fetchall()
+
+    x, height = zip(*data)
+
+    if x[0] is None:
+        raise ValueError("Data contains NULLs")
+
+    return x, height, xlabel, ylabel
+
+
+@requires(["matplotlib"])
+@telemetry.log_call("bar", payload=True)
+def bar(
+    payload,
+    table,
+    column,
+    show_num=False,
+    orient="v",
+    with_=None,
+    conn=None,
+    cmap=None,
+    color=None,
+    edgecolor=None,
+    ax=None,
+):
+    """Plot Bar Chart
+
+    Parameters
+    ----------
+    table : str
+        Table name where the data is located
+
+    column : str
+        Column(s) to plot
+
+    show_num: bool
+        Show numbers on top of plot
+
+    orient : str, default='v'
+        Orientation of the plot. 'v' for vertical and 'h' for horizontal
+
+    conn : connection, default=None
+        Database connection. If None, it uses the current connection
+
+    Notes
+    -----
+
+    .. versionadded:: 0.7.6
+
+    Returns
+    -------
+    ax : matplotlib.Axes
+        Generated plot
+
+    """
+
+    if not conn:
+        conn = sql.connection.Connection.current
+
+    ax = ax or plt.gca()
+    payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
+
+    if column is None:
+        raise exceptions.UsageError("Column name has not been specified")
+
+    x, height_, xlabel, ylabel = _bar(table, column, with_=with_, conn=conn)
+
+    if color and cmap:
+        # raise a userwarning
+        warnings.warn(
+            "Both color and cmap are given. cmap will be ignored", UserWarning
+        )
+
+    if (not color) and cmap:
+        cmap = plt.get_cmap(cmap)
+        norm = Normalize(vmin=0, vmax=len(x))
+        color = [cmap(norm(i)) for i in range(len(x))]
+
+    if orient == "h":
+        ax.barh(
+            x,
+            height_,
+            align="center",
+            edgecolor=edgecolor,
+            color=color,
+        )
+        ax.set_xlabel(ylabel)
+        ax.set_ylabel(xlabel)
+    else:
+        ax.bar(
+            x,
+            height_,
+            align="center",
+            edgecolor=edgecolor,
+            color=color,
+        )
+        ax.set_ylabel(ylabel)
+        ax.set_xlabel(xlabel)
+
+    if show_num:
+        if orient == "v":
+            for i, v in enumerate(height_):
+                ax.text(
+                    i,
+                    v,
+                    str(v),
+                    color="black",
+                    fontweight="bold",
+                    ha="center",
+                    va="bottom",
+                )
+        else:
+            for i, v in enumerate(height_):
+                ax.text(
+                    v,
+                    i,
+                    str(v),
+                    color="black",
+                    fontweight="bold",
+                    ha="left",
+                    va="center",
+                )
+
+    ax.set_title(table)
+
+    return ax
+
+
+@modify_exceptions
+def _pie(table, column, with_=None, conn=None):
+    """get x and height for pie chart"""
+    if not conn:
+        conn = sql.connection.Connection.current
+    use_backticks = conn.is_use_backtick_template()
+
+    if isinstance(column, list):
+        if len(column) > 2:
+            raise exceptions.UsageError(
+                f"Passed columns: {column}\n"
+                "Pie chart currently supports, either a single column"
+                " on which group by and count is applied or"
+                " two columns: labels and size"
+            )
+
+        labels_ = column[0]
+        size_ = column[1]
+
+        print(f"Removing NULLs, if there exists any from {labels_} and {size_}")
+        template_ = """
+                select "{{labels_}}" as labels,
+                "{{size_}}" as size
+                from "{{table}}"
+                where "{{labels_}}" is not null
+                and "{{size_}}" is not null;
+                """
+        if use_backticks:
+            template_ = template_.replace('"', "`")
+
+        template = Template(template_)
+        query = template.render(table=table, labels_=labels_, size_=size_)
+
+    else:
+        print(f"Removing NULLs, if there exists any from {column}")
+        template_ = """
+                select "{{column}}" as x,
+                count("{{column}}") as height
+                from "{{table}}"
+                where "{{column}}" is not null
+                group by "{{column}}";
+                """
+        if use_backticks:
+            template_ = template_.replace('"', "`")
+
+        template = Template(template_)
+        query = template.render(table=table, column=column)
+
+    data = conn.execute(query, with_).fetchall()
+
+    labels, size = zip(*data)
+
+    if labels[0] is None:
+        raise ValueError("Data contains NULLs")
+
+    return labels, size
+
+
+@requires(["matplotlib"])
+@telemetry.log_call("bar", payload=True)
+def pie(
+    payload,
+    table,
+    column,
+    show_num=False,
+    with_=None,
+    conn=None,
+    cmap=None,
+    color=None,
+    ax=None,
+):
+    """Plot Pie Chart
+
+    Parameters
+    ----------
+    table : str
+        Table name where the data is located
+
+    column : str
+        Column(s) to plot
+
+    show_num: bool
+        Show numbers on top of plot
+
+    conn : connection, default=None
+        Database connection. If None, it uses the current connection
+
+    Notes
+    -----
+
+    .. versionadded:: 0.7.6
+
+    Returns
+    -------
+    ax : matplotlib.Axes
+        Generated plot
+    """
+
+    if not conn:
+        conn = sql.connection.Connection.current
+
+    ax = ax or plt.gca()
+    payload["connection_info"] = conn._get_curr_sqlalchemy_connection_info()
+
+    if column is None:
+        raise exceptions.UsageError("Column name has not been specified")
+
+    labels, size_ = _pie(table, column, with_=with_, conn=conn)
+
+    if color and cmap:
+        # raise a userwarning
+        warnings.warn(
+            "Both color and cmap are given. cmap will be ignored", UserWarning
+        )
+
+    if (not color) and cmap:
+        cmap = plt.get_cmap(cmap)
+        norm = Normalize(vmin=0, vmax=len(labels))
+        color = [cmap(norm(i)) for i in range(len(labels))]
+
+    if show_num:
+        ax.pie(
+            size_,
+            labels=labels,
+            colors=color,
+            autopct="%1.2f%%",
+        )
+    else:
+        ax.pie(
+            size_,
+            labels=labels,
+            colors=color,
+        )
+
+    ax.set_title(table)
+
+    return ax
```

### Comparing `jupysql-0.7.7/src/sql/run.py` & `jupysql-0.7.8/src/sql/run.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/store.py` & `jupysql-0.7.8/src/sql/store.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/util.py` & `jupysql-0.7.8/src/sql/util.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/widgets/table_widget/js/tableWidget.js` & `jupysql-0.7.8/src/sql/widgets/table_widget/js/tableWidget.js`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/widgets/table_widget/table_widget.py` & `jupysql-0.7.8/src/sql/widgets/table_widget/table_widget.py`

 * *Files identical despite different names*

### Comparing `jupysql-0.7.7/src/sql/widgets/utils.py` & `jupysql-0.7.8/src/sql/widgets/utils.py`

 * *Files identical despite different names*

