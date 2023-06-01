# Comparing `tmp/swoop.db-0.1.0.tar.gz` & `tmp/swoop.db-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "swoop.db-0.1.0.tar", last modified: Wed May 31 22:41:57 2023, max compression
+gzip compressed data, was "swoop.db-0.1.1.tar", last modified: Thu Jun  1 19:55:43 2023, max compression
```

## Comparing `swoop.db-0.1.0.tar` & `swoop.db-0.1.1.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.980006 swoop.db-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-31 22:41:44.000000 swoop.db-0.1.0/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.972006 swoop.db-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.976006 swoop.db-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-31 22:41:44.000000 swoop.db-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-31 22:41:44.000000 swoop.db-0.1.0/.github/workflows/python-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-31 22:41:44.000000 swoop.db-0.1.0/.github/workflows/snyk-scan.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-31 22:41:44.000000 swoop.db-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-05-31 22:41:44.000000 swoop.db-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-31 22:41:44.000000 swoop.db-0.1.0/.snyk
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-31 22:41:44.000000 swoop.db-0.1.0/.sqlfluff
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-31 22:41:44.000000 swoop.db-0.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-05-31 22:41:44.000000 swoop.db-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-31 22:41:44.000000 swoop.db-0.1.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-05-31 22:41:44.000000 swoop.db-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-31 22:41:57.980006 swoop.db-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-31 22:41:44.000000 swoop.db-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-31 22:41:44.000000 swoop.db-0.1.0/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-31 22:41:44.000000 swoop.db-0.1.0/docker-compose.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-31 22:41:44.000000 swoop.db-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-31 22:41:44.000000 swoop.db-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 22:41:57.980006 swoop.db-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.972006 swoop.db-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.972006 swoop.db-0.1.0/src/swoop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.976006 swoop.db-0.1.0/src/swoop/db/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-31 22:41:44.000000 swoop.db-0.1.0/src/swoop/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-31 22:41:44.000000 swoop.db-0.1.0/src/swoop/db/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-31 22:41:44.000000 swoop.db-0.1.0/src/swoop/db/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.976006 swoop.db-0.1.0/src/swoop/db/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-05-31 22:41:44.000000 swoop.db-0.1.0/src/swoop/db/fixtures/base_01.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.976006 swoop.db-0.1.0/src/swoop/db/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-05-31 22:41:44.000000 swoop.db-0.1.0/src/swoop/db/migrations/00000_base_schema.up.sql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:44.000000 swoop.db-0.1.0/src/swoop/db/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-05-31 22:41:44.000000 swoop.db-0.1.0/src/swoop/db/schema.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.976006 swoop.db-0.1.0/src/swoop.db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-05-31 22:41:57.000000 swoop.db-0.1.0/src/swoop.db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-31 22:41:57.000000 swoop.db-0.1.0/src/swoop.db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 22:41:57.000000 swoop.db-0.1.0/src/swoop.db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-31 22:41:57.000000 swoop.db-0.1.0/src/swoop.db.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 22:41:57.000000 swoop.db-0.1.0/src/swoop.db.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-31 22:41:57.000000 swoop.db-0.1.0/src/swoop.db.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.980006 swoop.db-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-05-31 22:41:44.000000 swoop.db-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 22:41:57.980006 swoop.db-0.1.0/tests/pgtap/
--rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-31 22:41:44.000000 swoop.db-0.1.0/tests/pgtap/test_action.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-05-31 22:41:44.000000 swoop.db-0.1.0/tests/pgtap/test_item_inserts.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-31 22:41:44.000000 swoop.db-0.1.0/tests/pgtap/test_limit-locking.sql
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-31 22:41:44.000000 swoop.db-0.1.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-31 22:41:44.000000 swoop.db-0.1.0/tests/test_database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.197333 swoop.db-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.201333 swoop.db-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.github/workflows/publish-image.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.github/workflows/python-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.github/workflows/snyk-scan.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.snyk
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-01 19:55:28.000000 swoop.db-0.1.1/.sqlfluff
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-06-01 19:55:28.000000 swoop.db-0.1.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-06-01 19:55:28.000000 swoop.db-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-06-01 19:55:28.000000 swoop.db-0.1.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-06-01 19:55:28.000000 swoop.db-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-01 19:55:43.205333 swoop.db-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-01 19:55:28.000000 swoop.db-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-06-01 19:55:28.000000 swoop.db-0.1.1/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-01 19:55:28.000000 swoop.db-0.1.1/docker-compose.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-06-01 19:55:28.000000 swoop.db-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 19:55:28.000000 swoop.db-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:55:43.205333 swoop.db-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.201333 swoop.db-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.201333 swoop.db-0.1.1/src/swoop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/src/swoop/db/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/src/swoop/db/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/fixtures/base_01.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/src/swoop/db/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)    12955 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/migrations/00000_base_schema.up.sql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-06-01 19:55:28.000000 swoop.db-0.1.1/src/swoop/db/schema.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.201333 swoop.db-0.1.1/src/swoop.db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 19:55:43.000000 swoop.db-0.1.1/src/swoop.db.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:55:43.205333 swoop.db-0.1.1/tests/pgtap/
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/pgtap/test_action.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/pgtap/test_item_inserts.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/pgtap/test_limit-locking.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-01 19:55:28.000000 swoop.db-0.1.1/tests/test_database.py
```

### Comparing `swoop.db-0.1.0/.github/workflows/python-publish.yml` & `swoop.db-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/.github/workflows/python-test.yml` & `swoop.db-0.1.1/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/.github/workflows/snyk-scan.yml` & `swoop.db-0.1.1/.github/workflows/snyk-scan.yml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/.gitignore` & `swoop.db-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/.pre-commit-config.yaml` & `swoop.db-0.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/.snyk` & `swoop.db-0.1.1/.snyk`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/CONTRIBUTING.md` & `swoop.db-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/Dockerfile` & `swoop.db-0.1.1/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 RUN apt-get update && apt-get install -y git python3-venv
 WORKDIR /opt/swoop/db
 RUN python3 -m venv --copies swoop-db-venv
 COPY requirements.txt .
 RUN ls ./swoop-db-venv/bin/
 RUN ./swoop-db-venv/bin/pip install -r requirements.txt
 COPY ./src ./src
-COPY README.md pyproject.toml LICENSE .
+COPY README.md pyproject.toml LICENSE ./
 RUN --mount=source=.git,target=.git,type=bind ./swoop-db-venv/bin/pip install .
 
 
 FROM postgres:15-bullseye
 # install build deps and pg_partman
 RUN set -x && \
     apt-get update && \
```

### Comparing `swoop.db-0.1.0/LICENSE` & `swoop.db-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/PKG-INFO` & `swoop.db-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 0.1.0
+Version: 0.1.1
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-0.1.0/README.md` & `swoop.db-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/RELEASE.md` & `swoop.db-0.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/pyproject.toml` & `swoop.db-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/src/swoop/db/cli.py` & `swoop.db-0.1.1/src/swoop/db/cli.py`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/src/swoop/db/fixtures/base_01.sql` & `swoop.db-0.1.1/src/swoop/db/fixtures/base_01.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/src/swoop/db/migrations/00000_base_schema.up.sql` & `swoop.db-0.1.1/src/swoop/db/migrations/00000_base_schema.up.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/src/swoop/db/schema.sql` & `swoop.db-0.1.1/src/swoop/db/schema.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/src/swoop.db.egg-info/PKG-INFO` & `swoop.db-0.1.1/src/swoop.db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swoop.db
-Version: 0.1.0
+Version: 0.1.1
 Summary: Database for STAC Workflow Open Orchestration Framework
 Author-email: Jarrett Keifer <jkeifer@element84.com>
 License: Apache License 2.0
 Keywords: postgresql,sql,stac,workflow,geospatial
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `swoop.db-0.1.0/src/swoop.db.egg-info/SOURCES.txt` & `swoop.db-0.1.1/src/swoop.db.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 Dockerfile
 LICENSE
 README.md
 RELEASE.md
 docker-compose.yml
 pyproject.toml
 requirements.txt
+.github/workflows/publish-image.yml
 .github/workflows/python-publish.yml
 .github/workflows/python-test.yml
 .github/workflows/snyk-scan.yml
 src/swoop.db.egg-info/PKG-INFO
 src/swoop.db.egg-info/SOURCES.txt
 src/swoop.db.egg-info/dependency_links.txt
 src/swoop.db.egg-info/entry_points.txt
```

### Comparing `swoop.db-0.1.0/tests/conftest.py` & `swoop.db-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/tests/pgtap/test_action.sql` & `swoop.db-0.1.1/tests/pgtap/test_action.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/tests/pgtap/test_item_inserts.sql` & `swoop.db-0.1.1/tests/pgtap/test_item_inserts.sql`

 * *Files identical despite different names*

### Comparing `swoop.db-0.1.0/tests/pgtap/test_limit-locking.sql` & `swoop.db-0.1.1/tests/pgtap/test_limit-locking.sql`

 * *Files identical despite different names*

