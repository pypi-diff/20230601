# Comparing `tmp/impact-stack-auth-wsgi-middleware-0.2.0.tar.gz` & `tmp/impact-stack-auth-wsgi-middleware-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impact-stack-auth-wsgi-middleware-0.2.0.tar", last modified: Tue Jun 21 14:34:50 2022, max compression
+gzip compressed data, was "impact-stack-auth-wsgi-middleware-0.3.0.tar", last modified: Thu Jun  1 13:42:02 2023, max compression
```

## Comparing `impact-stack-auth-wsgi-middleware-0.2.0.tar` & `impact-stack-auth-wsgi-middleware-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 roman     (1000) users      (100)        0 2022-06-21 14:34:50.497219 impact-stack-auth-wsgi-middleware-0.2.0/
--rw-r--r--   0 roman     (1000) users      (100)      394 2022-06-21 14:27:07.000000 impact-stack-auth-wsgi-middleware-0.2.0/.editorconfig
--rw-r--r--   0 roman     (1000) users      (100)      115 2022-06-21 14:27:07.000000 impact-stack-auth-wsgi-middleware-0.2.0/.gitignore
--rw-r--r--   0 roman     (1000) users      (100)      162 2022-06-21 14:27:07.000000 impact-stack-auth-wsgi-middleware-0.2.0/.gitlab-ci.yml
--rw-r--r--   0 roman     (1000) users      (100)      872 2022-06-21 14:27:07.000000 impact-stack-auth-wsgi-middleware-0.2.0/.pre-commit-config.yaml
--rw-r--r--   0 roman     (1000) users      (100)    14866 2020-05-25 10:17:19.000000 impact-stack-auth-wsgi-middleware-0.2.0/.pylintrc
--rw-r--r--   0 roman     (1000) users      (100)    35149 2019-05-17 15:12:07.000000 impact-stack-auth-wsgi-middleware-0.2.0/LICENSE
--rw-r--r--   0 roman     (1000) users      (100)     1740 2022-06-21 14:30:28.000000 impact-stack-auth-wsgi-middleware-0.2.0/Makefile
--rw-r--r--   0 roman     (1000) users      (100)     2848 2022-06-21 14:34:50.497219 impact-stack-auth-wsgi-middleware-0.2.0/PKG-INFO
--rw-r--r--   0 roman     (1000) users      (100)     2654 2022-01-24 11:23:19.000000 impact-stack-auth-wsgi-middleware-0.2.0/README.md
-drwxr-xr-x   0 roman     (1000) users      (100)        0 2022-06-21 14:34:50.493219 impact-stack-auth-wsgi-middleware-0.2.0/impact_stack/
-drwxr-xr-x   0 roman     (1000) users      (100)        0 2022-06-21 14:34:50.497219 impact-stack-auth-wsgi-middleware-0.2.0/impact_stack/auth_wsgi_middleware/
--rw-r--r--   0 roman     (1000) users      (100)     2734 2022-06-21 14:27:07.000000 impact-stack-auth-wsgi-middleware-0.2.0/impact_stack/auth_wsgi_middleware/__init__.py
-drwxr-xr-x   0 roman     (1000) users      (100)        0 2022-06-21 14:34:50.497219 impact-stack-auth-wsgi-middleware-0.2.0/impact_stack_auth_wsgi_middleware.egg-info/
--rw-r--r--   0 roman     (1000) users      (100)     2848 2022-06-21 14:34:50.000000 impact-stack-auth-wsgi-middleware-0.2.0/impact_stack_auth_wsgi_middleware.egg-info/PKG-INFO
--rw-r--r--   0 roman     (1000) users      (100)      554 2022-06-21 14:34:50.000000 impact-stack-auth-wsgi-middleware-0.2.0/impact_stack_auth_wsgi_middleware.egg-info/SOURCES.txt
--rw-r--r--   0 roman     (1000) users      (100)        1 2022-06-21 14:34:50.000000 impact-stack-auth-wsgi-middleware-0.2.0/impact_stack_auth_wsgi_middleware.egg-info/dependency_links.txt
--rw-r--r--   0 roman     (1000) users      (100)       37 2022-06-21 14:34:50.000000 impact-stack-auth-wsgi-middleware-0.2.0/impact_stack_auth_wsgi_middleware.egg-info/requires.txt
--rw-r--r--   0 roman     (1000) users      (100)       13 2022-06-21 14:34:50.000000 impact-stack-auth-wsgi-middleware-0.2.0/impact_stack_auth_wsgi_middleware.egg-info/top_level.txt
--rw-r--r--   0 roman     (1000) users      (100)      967 2022-06-21 14:33:20.000000 impact-stack-auth-wsgi-middleware-0.2.0/pyproject.toml
--rw-r--r--   0 roman     (1000) users      (100)      174 2022-06-21 14:31:48.000000 impact-stack-auth-wsgi-middleware-0.2.0/requirements-dev.in
--rw-r--r--   0 roman     (1000) users      (100)     3164 2022-06-21 14:32:04.000000 impact-stack-auth-wsgi-middleware-0.2.0/requirements-dev.txt
--rw-r--r--   0 roman     (1000) users      (100)      449 2022-06-21 14:30:37.000000 impact-stack-auth-wsgi-middleware-0.2.0/requirements.txt
--rw-r--r--   0 roman     (1000) users      (100)       38 2022-06-21 14:34:50.497219 impact-stack-auth-wsgi-middleware-0.2.0/setup.cfg
--rw-r--r--   0 roman     (1000) users      (100)      104 2022-06-21 14:27:07.000000 impact-stack-auth-wsgi-middleware-0.2.0/setup.py
-drwxr-xr-x   0 roman     (1000) users      (100)        0 2022-06-21 14:34:50.497219 impact-stack-auth-wsgi-middleware-0.2.0/tests/
--rw-r--r--   0 roman     (1000) users      (100)       30 2020-05-25 10:17:19.000000 impact-stack-auth-wsgi-middleware-0.2.0/tests/__init__.py
--rw-r--r--   0 roman     (1000) users      (100)     3014 2022-06-21 14:27:07.000000 impact-stack-auth-wsgi-middleware-0.2.0/tests/flask_jwt_test.py
+drwxr-xr-x   0 roman     (1000) users      (100)        0 2023-06-01 13:42:02.207314 impact-stack-auth-wsgi-middleware-0.3.0/
+-rw-r--r--   0 roman     (1000) users      (100)      394 2022-06-21 14:27:07.000000 impact-stack-auth-wsgi-middleware-0.3.0/.editorconfig
+-rw-r--r--   0 roman     (1000) users      (100)      115 2022-06-21 14:27:07.000000 impact-stack-auth-wsgi-middleware-0.3.0/.gitignore
+-rw-r--r--   0 roman     (1000) users      (100)      134 2023-06-01 13:34:02.000000 impact-stack-auth-wsgi-middleware-0.3.0/.gitlab-ci.yml
+-rw-r--r--   0 roman     (1000) users      (100)      714 2023-02-23 11:16:46.000000 impact-stack-auth-wsgi-middleware-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 roman     (1000) users      (100)    35149 2019-05-17 15:12:07.000000 impact-stack-auth-wsgi-middleware-0.3.0/LICENSE
+-rw-r--r--   0 roman     (1000) users      (100)     1570 2023-02-23 11:16:46.000000 impact-stack-auth-wsgi-middleware-0.3.0/Makefile
+-rw-r--r--   0 roman     (1000) users      (100)     2868 2023-06-01 13:42:02.207314 impact-stack-auth-wsgi-middleware-0.3.0/PKG-INFO
+-rw-r--r--   0 roman     (1000) users      (100)     2654 2022-01-24 11:23:19.000000 impact-stack-auth-wsgi-middleware-0.3.0/README.md
+drwxr-xr-x   0 roman     (1000) users      (100)        0 2023-06-01 13:42:02.203314 impact-stack-auth-wsgi-middleware-0.3.0/impact_stack/
+drwxr-xr-x   0 roman     (1000) users      (100)        0 2023-06-01 13:42:02.203314 impact-stack-auth-wsgi-middleware-0.3.0/impact_stack/auth_wsgi_middleware/
+-rw-r--r--   0 roman     (1000) users      (100)     2734 2023-06-01 13:34:02.000000 impact-stack-auth-wsgi-middleware-0.3.0/impact_stack/auth_wsgi_middleware/__init__.py
+drwxr-xr-x   0 roman     (1000) users      (100)        0 2023-06-01 13:42:02.207314 impact-stack-auth-wsgi-middleware-0.3.0/impact_stack_auth_wsgi_middleware.egg-info/
+-rw-r--r--   0 roman     (1000) users      (100)     2868 2023-06-01 13:42:02.000000 impact-stack-auth-wsgi-middleware-0.3.0/impact_stack_auth_wsgi_middleware.egg-info/PKG-INFO
+-rw-r--r--   0 roman     (1000) users      (100)      524 2023-06-01 13:42:02.000000 impact-stack-auth-wsgi-middleware-0.3.0/impact_stack_auth_wsgi_middleware.egg-info/SOURCES.txt
+-rw-r--r--   0 roman     (1000) users      (100)        1 2023-06-01 13:42:02.000000 impact-stack-auth-wsgi-middleware-0.3.0/impact_stack_auth_wsgi_middleware.egg-info/dependency_links.txt
+-rw-r--r--   0 roman     (1000) users      (100)      157 2023-06-01 13:42:02.000000 impact-stack-auth-wsgi-middleware-0.3.0/impact_stack_auth_wsgi_middleware.egg-info/requires.txt
+-rw-r--r--   0 roman     (1000) users      (100)       13 2023-06-01 13:42:02.000000 impact-stack-auth-wsgi-middleware-0.3.0/impact_stack_auth_wsgi_middleware.egg-info/top_level.txt
+-rw-r--r--   0 roman     (1000) users      (100)     1181 2023-06-01 13:41:15.000000 impact-stack-auth-wsgi-middleware-0.3.0/pyproject.toml
+-rw-r--r--   0 roman     (1000) users      (100)     3139 2023-06-01 13:34:05.000000 impact-stack-auth-wsgi-middleware-0.3.0/requirements-dev.txt
+-rw-r--r--   0 roman     (1000) users      (100)      496 2023-06-01 13:34:05.000000 impact-stack-auth-wsgi-middleware-0.3.0/requirements.txt
+-rw-r--r--   0 roman     (1000) users      (100)       38 2023-06-01 13:42:02.207314 impact-stack-auth-wsgi-middleware-0.3.0/setup.cfg
+-rw-r--r--   0 roman     (1000) users      (100)      104 2022-06-21 14:27:07.000000 impact-stack-auth-wsgi-middleware-0.3.0/setup.py
+drwxr-xr-x   0 roman     (1000) users      (100)        0 2023-06-01 13:42:02.207314 impact-stack-auth-wsgi-middleware-0.3.0/tests/
+-rw-r--r--   0 roman     (1000) users      (100)       30 2020-05-25 10:17:19.000000 impact-stack-auth-wsgi-middleware-0.3.0/tests/__init__.py
+-rw-r--r--   0 roman     (1000) users      (100)     3035 2023-06-01 13:34:05.000000 impact-stack-auth-wsgi-middleware-0.3.0/tests/flask_jwt_test.py
```

### Comparing `impact-stack-auth-wsgi-middleware-0.2.0/.pre-commit-config.yaml` & `impact-stack-auth-wsgi-middleware-0.3.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,14 @@
     hooks:
     -   id: trailing-whitespace
     -   id: end-of-file-fixer
     -   id: debug-statements
     -   id: check-added-large-files
 -   repo: local
     hooks:
-    -   id: safety
-        name: safety
-        entry: safety check -r
-        language: system
-        files: requirements.txt
     -   id: isort
         name: isort
         entry: isort
         language: system
         types:
         - python
     -   id: black
@@ -24,15 +19,14 @@
         entry: black
         language: system
         files: \.py$
     -   id: pylint
         name: pylint
         entry: pylint --jobs=2
         language: system
-        exclude: ^migrations/
         types:
         - python
     -   id: pydocstyle
         name: pydocstyle
         entry: pydocstyle
         language: python
         files: \.py$
```

### Comparing `impact-stack-auth-wsgi-middleware-0.2.0/LICENSE` & `impact-stack-auth-wsgi-middleware-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `impact-stack-auth-wsgi-middleware-0.2.0/Makefile` & `impact-stack-auth-wsgi-middleware-0.3.0/Makefile`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-.PHONY: help bootstrap lint test safety requirements
+.PHONY: help bootstrap lint test requirements
 
 VENV?=.venv
 PYTHON?=python3
 
 help:
 	@echo
 	@echo "make install         -- setup production environment"
 	@echo
 	@echo "make development     -- setup development environment"
 	@echo "make test            -- run full test suite"
 	@echo "make lint            -- run all linters on the code base"
-	@echo "make safety          -- run safety check on packages"
 	@echo
 	@echo "make requirements    -- only compile the requirements*.txt files"
 	@echo "make .venv           -- bootstrap the virtualenv."
 	@echo
 
 install: $(VENV)/.pip-installed-production
 
@@ -22,26 +21,21 @@
 
 lint: development
 	$(VENV)/bin/pre-commit run -a
 
 test: development
 	$(VENV)/bin/pytest
 
-safety: requirements.txt development
-	$(VENV)/bin/safety check -r $<
-
 requirements: requirements.txt requirements-dev.txt
 
-%.txt: %.in
-	$(VENV)/bin/pip-compile -v --output-file $@ $<
-
-requirements-dev.txt: requirements-dev.in requirements.in setup.py
-
 requirements.txt: pyproject.toml
-	$(VENV)/bin/pip-compile -v --output-file $@ $<
+	$(VENV)/bin/pip-compile -v --output-file=$@ $<
+
+requirements-dev.txt: pyproject.toml
+	$(VENV)/bin/pip-compile -v --output-file=$@ --extra=dev $<
 
 # Actual files/directories
 ################################################################################
 
 # Create this directory as a symbolic link to an existing virtualenv, if you want to use that.
 $(VENV):
 	$(PYTHON) -m venv --system-site-packages $(VENV)
```

### Comparing `impact-stack-auth-wsgi-middleware-0.2.0/PKG-INFO` & `impact-stack-auth-wsgi-middleware-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: impact-stack-auth-wsgi-middleware
-Version: 0.2.0
+Version: 0.3.0
 Author-email: Roman Zimmermann <roman@more-onion.com>
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # WSGI authentication middleware
 
 This app is just one piece in our bigger [authorization scheme for microservices](https://docs.google.com/document/d/1wbdSyAU0OV0e2rH-nh_IiJkgNDWyKXhptsJwIff64A0/edit?usp=sharing).
 Its purpose is make migrating to session cookies simpler by ensuring that backend microservices only need to deal with JWTs that contain all the needed claims.
```

### Comparing `impact-stack-auth-wsgi-middleware-0.2.0/README.md` & `impact-stack-auth-wsgi-middleware-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `impact-stack-auth-wsgi-middleware-0.2.0/impact_stack/auth_wsgi_middleware/__init__.py` & `impact-stack-auth-wsgi-middleware-0.3.0/impact_stack/auth_wsgi_middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `impact-stack-auth-wsgi-middleware-0.2.0/impact_stack_auth_wsgi_middleware.egg-info/PKG-INFO` & `impact-stack-auth-wsgi-middleware-0.3.0/impact_stack_auth_wsgi_middleware.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: impact-stack-auth-wsgi-middleware
-Version: 0.2.0
+Version: 0.3.0
 Author-email: Roman Zimmermann <roman@more-onion.com>
 Description-Content-Type: text/markdown
+Provides-Extra: dev
 License-File: LICENSE
 
 # WSGI authentication middleware
 
 This app is just one piece in our bigger [authorization scheme for microservices](https://docs.google.com/document/d/1wbdSyAU0OV0e2rH-nh_IiJkgNDWyKXhptsJwIff64A0/edit?usp=sharing).
 Its purpose is make migrating to session cookies simpler by ensuring that backend microservices only need to deal with JWTs that contain all the needed claims.
```

### Comparing `impact-stack-auth-wsgi-middleware-0.2.0/impact_stack_auth_wsgi_middleware.egg-info/SOURCES.txt` & `impact-stack-auth-wsgi-middleware-0.3.0/impact_stack_auth_wsgi_middleware.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 .editorconfig
 .gitignore
 .gitlab-ci.yml
 .pre-commit-config.yaml
-.pylintrc
 LICENSE
 Makefile
 README.md
 pyproject.toml
-requirements-dev.in
 requirements-dev.txt
 requirements.txt
 setup.py
 impact_stack/auth_wsgi_middleware/__init__.py
 impact_stack_auth_wsgi_middleware.egg-info/PKG-INFO
 impact_stack_auth_wsgi_middleware.egg-info/SOURCES.txt
 impact_stack_auth_wsgi_middleware.egg-info/dependency_links.txt
```

### Comparing `impact-stack-auth-wsgi-middleware-0.2.0/pyproject.toml` & `impact-stack-auth-wsgi-middleware-0.3.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,43 @@
 [build-system]
-requires = ["setuptools", "setuptools-scm"]
+requires = [
+  "setuptools>=45",
+  "setuptools-scm[toml]>=6.2",
+  "wheel",
+]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "impact-stack-auth-wsgi-middleware"
-version = "0.2.0"
+dynamic = ["version"]
 dependencies = [
     "itsdangerous",
     "redis<4.1",
     "werkzeug>=2.1",
 ]
 authors = [
   {name = "Roman Zimmermann", email = "roman@more-onion.com"},
 ]
 readme = "README.md"
 
+[project.optional-dependencies]
+dev = [
+  "black",
+  "fakeredis",
+  "flask",
+  "flask-jwt-extended",
+  "isort",
+  "pip-tools",
+  "pre-commit",
+  "pydocstyle[toml]>=6",
+  "pylint",
+  "pytest",
+  "pytest-cov",
+]
+
 [tool.black]
 line-length = 100
 
 [tool.coverage.run]
 source = ["impact_stack"]
 relative_files = true
 
@@ -32,22 +51,21 @@
 
 [tool.pydocstyle]
 convention = "google"
 
 [tool.pylint.basic]
 good-names = ["db"]
 
-[tool.pylint.messages_control]
-disable = "C0330, C0326"
-
 [tool.pylint.format]
 max-line-length = "100"
 
 [tool.pytest.ini_options]
 addopts = "--cov --cov-report=term --cov-report=xml --junitxml=pytest-junit.xml"
 python_classes = [
   "*Test",
   "Test*",
 ]
 
 [tool.setuptools]
 packages = ["impact_stack.auth_wsgi_middleware"]
+
+[tool.setuptools_scm]
```

### Comparing `impact-stack-auth-wsgi-middleware-0.2.0/tests/flask_jwt_test.py` & `impact-stack-auth-wsgi-middleware-0.3.0/tests/flask_jwt_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Test the middleware by wrapping a Flask app that accepts JWT tokens."""
 
-# pylint: disable=redefined-outer-name
+# pylint: disable=redefined-outer-name,unused-argument
 
 import json
 
 import fakeredis
 import flask_jwt_extended
 import pytest
 from flask import Flask, jsonify
@@ -40,25 +40,26 @@
     with app.app_context():
         yield app
 
 
 @pytest.fixture(scope="class")
 def auth_middleware(app, jwt):
     """Initialize the auth middleware."""
-    # pylint: disable=protected-access,unused-argument
-    m = AuthMiddleware.init_app(app)
-    m.token_store._client.set("user1-uuid", flask_jwt_extended.create_access_token("user1"))
-    return m
+    # pylint: disable=protected-access
+    middleware = AuthMiddleware.init_app(app)
+    middleware.token_store._client.set(
+        "user1-uuid", flask_jwt_extended.create_access_token("user1")
+    )
+    return middleware
 
 
 @pytest.fixture
 def client(app):
     """Define a test client instance and context."""
-    with app.test_client() as c:
-        yield c
+    return app.test_client()
 
 
 @pytest.mark.usefixtures("auth_middleware")
 class TestMiddleware:
     """Test the middleware."""
 
     @staticmethod
```

