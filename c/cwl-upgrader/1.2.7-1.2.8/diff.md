# Comparing `tmp/cwl-upgrader-1.2.7.tar.gz` & `tmp/cwl-upgrader-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cwl-upgrader-1.2.7.tar", last modified: Thu May 11 11:23:32 2023, max compression
+gzip compressed data, was "cwl-upgrader-1.2.8.tar", last modified: Thu Jun  1 10:40:08 2023, max compression
```

## Comparing `cwl-upgrader-1.2.7.tar` & `cwl-upgrader-1.2.8.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       91 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     6361 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)     2484 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      992 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/README.rst
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.441087 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     2484 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     1086 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       56 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      228 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       12 2023-05-11 11:23:32.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-05-11 11:23:29.000000 cwl-upgrader-1.2.7/cwl_upgrader.egg-info/zip-safe
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.441087 cwl-upgrader-1.2.7/cwlupgrader/
--rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/cwlupgrader/__init__.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)    34460 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/cwlupgrader/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/cwlupgrader/py.typed
--rw-r--r--   0 michael   (1000) michael   (1000)      395 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2305 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.441087 cwl-upgrader-1.2.7/testdata/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.441087 cwl-upgrader-1.2.7/testdata/draft-3/
--rw-r--r--   0 michael   (1000) michael   (1000)    11102 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/draft-3/attributor-prok-cheetah.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      625 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/draft-3/wf.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/testdata/v1.0/
--rw-r--r--   0 michael   (1000) michael   (1000)      433 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/1st-workflow.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      385 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/arguments.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8843 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/attributor-prok-cheetah.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1157 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/conflict-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      312 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/listing_deep1-arr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      307 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/listing_deep1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/networkaccess.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/tar-param.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      489 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.0/wf.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/testdata/v1.1/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1425 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.1/conflict-wf.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      425 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.1/listing_deep1-arr.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.1/listing_deep1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.1/networkaccess.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/testdata/v1.2/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      432 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.2/1st-workflow.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      495 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.2/arguments.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.2/listing_deep1.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.2/networkaccess.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      443 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/testdata/v1.2/tar-param.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:32.445087 cwl-upgrader-1.2.7/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4202 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/tests/test_complete.py
--rw-r--r--   0 michael   (1000) michael   (1000)      537 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/tests/test_output_dir.py
--rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-05-11 11:23:25.000000 cwl-upgrader-1.2.7/tests/util.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:40:08.493110 cwl-upgrader-1.2.8/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       91 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     6612 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)     2223 2023-06-01 10:40:08.493110 cwl-upgrader-1.2.8/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      992 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/README.rst
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:40:08.489110 cwl-upgrader-1.2.8/cwl_upgrader.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2223 2023-06-01 10:40:08.000000 cwl-upgrader-1.2.8/cwl_upgrader.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     1896 2023-06-01 10:40:08.000000 cwl-upgrader-1.2.8/cwl_upgrader.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-01 10:40:08.000000 cwl-upgrader-1.2.8/cwl_upgrader.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       55 2023-06-01 10:40:08.000000 cwl-upgrader-1.2.8/cwl_upgrader.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      216 2023-06-01 10:40:08.000000 cwl-upgrader-1.2.8/cwl_upgrader.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       12 2023-06-01 10:40:08.000000 cwl-upgrader-1.2.8/cwl_upgrader.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-06-01 10:39:45.000000 cwl-upgrader-1.2.8/cwl_upgrader.egg-info/zip-safe
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:40:08.489110 cwl-upgrader-1.2.8/cwlupgrader/
+-rw-r--r--   0 michael   (1000) michael   (1000)       79 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/cwlupgrader/__init__.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    34444 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/cwlupgrader/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/cwlupgrader/py.typed
+-rw-r--r--   0 michael   (1000) michael   (1000)      396 2023-06-01 10:40:08.493110 cwl-upgrader-1.2.8/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2293 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:40:08.489110 cwl-upgrader-1.2.8/testdata/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:40:08.489110 cwl-upgrader-1.2.8/testdata/draft-3/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11102 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/draft-3/attributor-prok-cheetah.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      625 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/draft-3/wf.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:40:08.493110 cwl-upgrader-1.2.8/testdata/v1.0/
+-rw-r--r--   0 michael   (1000) michael   (1000)      433 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.0/1st-workflow.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      385 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.0/arguments.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8843 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.0/attributor-prok-cheetah.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1157 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.0/conflict-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      312 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.0/listing_deep1-arr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      307 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.0/listing_deep1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.0/networkaccess.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.0/tar-param.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      489 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.0/wf.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:40:08.493110 cwl-upgrader-1.2.8/testdata/v1.1/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1425 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.1/conflict-wf.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      425 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.1/listing_deep1-arr.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.1/listing_deep1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.1/networkaccess.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:40:08.493110 cwl-upgrader-1.2.8/testdata/v1.2/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      432 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.2/1st-workflow.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      495 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.2/arguments.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      404 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.2/listing_deep1.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      330 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.2/networkaccess.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      443 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/testdata/v1.2/tar-param.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-06-01 10:40:08.493110 cwl-upgrader-1.2.8/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4202 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/tests/test_complete.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      537 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/tests/test_output_dir.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      787 2023-06-01 10:39:39.000000 cwl-upgrader-1.2.8/tests/util.py
```

### Comparing `cwl-upgrader-1.2.7/LICENSE.txt` & `cwl-upgrader-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.7/Makefile` & `cwl-upgrader-1.2.8/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 PACKAGE=cwlupgrader
 EXTRAS=
 
 # `SHELL=bash` doesn't work for some, so don't use BASH-isms like
 # `[[` conditional expressions.
 PYSOURCES=$(wildcard cwlupgrader/**.py tests/*.py) setup.py
 DEVPKGS=diff_cover black pylint pep257 pydocstyle flake8 tox tox-pyenv \
-	isort wheel autoflake flake8-bugbear pyupgrade bandit \
+	isort wheel autoflake flake8-bugbear pyupgrade bandit build\
 	-rtest-requirements.txt -rmypy-requirements.txt
 DEBDEVPKGS=pylint python3-coverage sloccount \
 	   python3-flake8 shellcheck
-VERSION=1.2.7  # please also update setup.py
+VERSION=1.2.8  # please also update setup.py
 
 ## all                    : default task (install cwl-upgrader in dev mode)
 all: dev
 
 ## help                   : print this help message and exit
 help: Makefile
 	@sed -n 's/^##//p' $<
@@ -53,32 +53,33 @@
 
 ## install                : install the cwlupgrader package and scripts
 install: FORCE
 	pip install .$(EXTRAS)
 
 ## dev                    : install the cwlupgrader package in dev mode
 dev: install-dep
+	pip install -U pip setuptools wheel
 	pip install -e .$(EXTRAS)
 
 ## dist                   : create a module package for distribution
 dist: dist/${MODULE}-$(VERSION).tar.gz
 
 dist/${MODULE}-$(VERSION).tar.gz: $(SOURCES)
-	python setup.py sdist bdist_wheel
+	python -m build
 
 ## clean                  : clean up all temporary / machine-generated files
 clean: FORCE
 	rm -f ${MODILE}/*.pyc tests/*.pyc
 	python setup.py clean --all || true
 	rm -Rf .coverage
 	rm -f diff-cover.html
 
 # Linting and code style related targets
 ## sort_import            : sorting imports using isort: https://github.com/timothycrosley/isort
-sort_imports: $(PYSOURCES)
+sort_imports: $(PYSOURCES) mypy-stubs
 	isort $^
 
 remove_unused_imports: $(PYSOURCES)
 	autoflake --in-place --remove-all-unused-imports $^
 
 pep257: pydocstyle
 ## pydocstyle             : check Python docstring style
@@ -94,18 +95,18 @@
 
 ## codespell              : check for common misspellings
 codespell:
 	codespell -w $(shell git ls-files | grep -v mypy-stubs | grep -v gitignore | grep -v EDAM.owl | grep -v pre.yml | grep -v test_schema)
 
 ## format                 : check/fix all code indentation and formatting (runs black)
 format:
-	black setup.py cwlupgrader tests
+	black setup.py cwlupgrader tests mypy-stubs
 
 format-check:
-	black --diff --check cwlupgrader setup.py
+	black --diff --check cwlupgrader setup.py mypy-stubs
 
 ## pylint                 : run static code analysis on Python code
 pylint: $(PYSOURCES)
 	pylint --msg-template="{path}:{line}: [{msg_id}({symbol}), {obj}] {msg}" \
                 $^ -j0|| true
 
 pylint_report.txt: $(PYSOURCES)
@@ -132,19 +133,19 @@
 coverage-report: .coverage
 	coverage report
 
 diff-cover: coverage.xml
 	diff-cover --compare-branch=main $^
 
 diff-cover.html: coverage.xml
-	diff-cover --compare-branch main $^ --html-report $@
+	diff-cover --compare-branch=main $^ --html-report $@
 
 ## test                   : run the cwlupgrader test suite
 test: $(PYSOURCES)
-	python -m pytest -rs
+	python -m pytest -rs ${PYTEST_EXTRA}
 
 ## testcov                : run the cwlupgrader test suite and collect coverage
 testcov: $(PYSOURCES)
 	python setup.py test --addopts "--cov" ${PYTEST_EXTRA}
 
 sloccount.sc: $(PYSOURCES) Makefile
 	sloccount --duplicates --wide --details $^ > $@
@@ -163,30 +164,36 @@
 	then \
 		rm -Rf mypy-stubs/ruamel/yaml ; \
 		ln -s $(shell python3 -c 'import ruamel.yaml; import os.path; print(os.path.dirname(ruamel.yaml.__file__))') \
 			mypy-stubs/ruamel/ ; \
 	fi  # if minimally required ruamel.yaml version is 0.15.99 or greater, than the above can be removed
 	MYPYPATH=$$MYPYPATH:mypy-stubs mypy $^
 
+mypy_3.6: $(filter-out setup.py,$(PYSOURCES))
+	MYPYPATH=$$MYPYPATH:mypy-stubs mypy --python-version 3.6 $^
+
+shellcheck: FORCE
+	shellcheck conformance-test.sh release-test.sh
+
 pyupgrade: $(PYSOURCES)
 	pyupgrade --exit-zero-even-if-changed --py36-plus $^
 
 release-test: FORCE
 	git diff-index --quiet HEAD -- || ( echo You have uncommitted changes, please commit them and try again; false )
 	./release-test.sh
 
 release: release-test
 	. testenv2/bin/activate && \
 		python testenv2/src/${MODULE}/setup.py sdist bdist_wheel && \
 		pip install twine && \
 		twine upload testenv2/src/${MODULE}/dist/* && \
 		git tag v${VERSION} && git push --tags
 
-flake8: $(PYSOURCES)
-	flake8 $^
+flake8: FORCE
+	flake8 $(PYSOURCES)
 
 FORCE:
 
 # Use this to print the value of a Makefile variable
 # Example `make print-VERSION`
 # From https://www.cmcrossroads.com/article/printing-value-makefile-variable
 print-%  : ; @echo $* = $($*)
```

### Comparing `cwl-upgrader-1.2.7/PKG-INFO` & `cwl-upgrader-1.2.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,16 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: cwl-upgrader
-Version: 1.2.7
+Version: 1.2.8
 Summary: Common Workflow Language standalone document upgrader
 Home-page: https://github.com/common-workflow-language/cwl-upgrader
+Download-URL: https://github.com/common-workflow-language/cwl-upgrader
 Author: Common Workflow Language contributors
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
-Download-URL: https://github.com/common-workflow-language/cwl-upgrader
-Description: =====================================================
-        Common workflow language standalone document upgrader
-        =====================================================
-        
-        This is a standalone upgrader for Common Workflow Language documents from
-        version ``draft-3``, ``v1.0``, and ``v1.1`` to ``v1.2``.
-        
-        See https://github.com/sbg/sevenbridges-cwl-draft2-upgrader for upgrading from ``sbg:draft-2``.
-        
-        It does not check for correctness of the input document, for that one can use
-        `the CWL reference implementation <https://github.com/common-workflow-language/cwltool>`_ (``cwltool --validate``).
-        
-        This is written and tested for Python 3.6, 3.7, 3.8, 3.9, and 3.10.
-        
-        Install
-        -------
-        
-        Installing the official package from PyPI::
-        
-          pip install cwl-upgrader
-        
-        Or from source::
-        
-          git clone https://github.com/common-workflow-language/cwl-upgrader.git
-          pip install ./cwl-upgrader/
-        
-        Run on the command line
-        -----------------------
-        
-        ::
-        
-          cwl-upgrader path-to-cwl-document [another-path-to-cwl-document ...]
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -54,7 +20,41 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6, <4
+License-File: LICENSE.txt
+
+=====================================================
+Common workflow language standalone document upgrader
+=====================================================
+
+This is a standalone upgrader for Common Workflow Language documents from
+version ``draft-3``, ``v1.0``, and ``v1.1`` to ``v1.2``.
+
+See https://github.com/sbg/sevenbridges-cwl-draft2-upgrader for upgrading from ``sbg:draft-2``.
+
+It does not check for correctness of the input document, for that one can use
+`the CWL reference implementation <https://github.com/common-workflow-language/cwltool>`_ (``cwltool --validate``).
+
+This is written and tested for Python 3.6, 3.7, 3.8, 3.9, and 3.10.
+
+Install
+-------
+
+Installing the official package from PyPI::
+
+  pip install cwl-upgrader
+
+Or from source::
+
+  git clone https://github.com/common-workflow-language/cwl-upgrader.git
+  pip install ./cwl-upgrader/
+
+Run on the command line
+-----------------------
+
+::
+
+  cwl-upgrader path-to-cwl-document [another-path-to-cwl-document ...]
```

### Comparing `cwl-upgrader-1.2.7/README.rst` & `cwl-upgrader-1.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.7/cwl_upgrader.egg-info/PKG-INFO` & `cwl-upgrader-1.2.8/cwl_upgrader.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,50 +1,16 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: cwl-upgrader
-Version: 1.2.7
+Version: 1.2.8
 Summary: Common Workflow Language standalone document upgrader
 Home-page: https://github.com/common-workflow-language/cwl-upgrader
+Download-URL: https://github.com/common-workflow-language/cwl-upgrader
 Author: Common Workflow Language contributors
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
-Download-URL: https://github.com/common-workflow-language/cwl-upgrader
-Description: =====================================================
-        Common workflow language standalone document upgrader
-        =====================================================
-        
-        This is a standalone upgrader for Common Workflow Language documents from
-        version ``draft-3``, ``v1.0``, and ``v1.1`` to ``v1.2``.
-        
-        See https://github.com/sbg/sevenbridges-cwl-draft2-upgrader for upgrading from ``sbg:draft-2``.
-        
-        It does not check for correctness of the input document, for that one can use
-        `the CWL reference implementation <https://github.com/common-workflow-language/cwltool>`_ (``cwltool --validate``).
-        
-        This is written and tested for Python 3.6, 3.7, 3.8, 3.9, and 3.10.
-        
-        Install
-        -------
-        
-        Installing the official package from PyPI::
-        
-          pip install cwl-upgrader
-        
-        Or from source::
-        
-          git clone https://github.com/common-workflow-language/cwl-upgrader.git
-          pip install ./cwl-upgrader/
-        
-        Run on the command line
-        -----------------------
-        
-        ::
-        
-          cwl-upgrader path-to-cwl-document [another-path-to-cwl-document ...]
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -54,7 +20,41 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.6, <4
+License-File: LICENSE.txt
+
+=====================================================
+Common workflow language standalone document upgrader
+=====================================================
+
+This is a standalone upgrader for Common Workflow Language documents from
+version ``draft-3``, ``v1.0``, and ``v1.1`` to ``v1.2``.
+
+See https://github.com/sbg/sevenbridges-cwl-draft2-upgrader for upgrading from ``sbg:draft-2``.
+
+It does not check for correctness of the input document, for that one can use
+`the CWL reference implementation <https://github.com/common-workflow-language/cwltool>`_ (``cwltool --validate``).
+
+This is written and tested for Python 3.6, 3.7, 3.8, 3.9, and 3.10.
+
+Install
+-------
+
+Installing the official package from PyPI::
+
+  pip install cwl-upgrader
+
+Or from source::
+
+  git clone https://github.com/common-workflow-language/cwl-upgrader.git
+  pip install ./cwl-upgrader/
+
+Run on the command line
+-----------------------
+
+::
+
+  cwl-upgrader path-to-cwl-document [another-path-to-cwl-document ...]
```

### Comparing `cwl-upgrader-1.2.7/cwlupgrader/main.py` & `cwl-upgrader-1.2.8/cwlupgrader/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 _logger = logging.getLogger("cwl-upgrader")  # pylint: disable=invalid-name
 defaultStreamHandler = logging.StreamHandler()  # pylint: disable=invalid-name
 _logger.addHandler(defaultStreamHandler)
 _logger.setLevel(logging.INFO)
 
 yaml = ruamel.yaml.main.YAML(typ="rt")
 yaml.allow_duplicate_keys = True
-yaml.preserve_quotes = True  # type: ignore
+yaml.preserve_quotes = True
 yaml.default_flow_style = False
 
 
 def parse_args(args: List[str]) -> argparse.Namespace:
     """Argument parser."""
     parser = argparse.ArgumentParser(
         description="Tool to upgrade CWL documents from one version to another. "
```

### Comparing `cwl-upgrader-1.2.7/setup.py` & `cwl-upgrader-1.2.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,32 +9,32 @@
 README = os.path.join(SETUP_DIR, "README.rst")
 
 NEEDS_PYTEST = {"pytest", "test", "ptr"}.intersection(sys.argv)
 PYTEST_RUNNER = ["pytest-runner", "pytest-cov"] if NEEDS_PYTEST else []
 
 setup(
     name="cwl-upgrader",
-    version="1.2.7",
+    version="1.2.8",
     description="Common Workflow Language standalone document upgrader",
     long_description=open(README).read(),
     author="Common Workflow Language contributors",
     author_email="common-workflow-language@googlegroups.com",
     url="https://github.com/common-workflow-language/cwl-upgrader",
     download_url="https://github.com/common-workflow-language/cwl-upgrader",
     license="Apache 2.0",
     packages=["cwlupgrader", "cwlupgrader.tests"],
     include_package_data=True,
     package_dir={"cwlupgrader.tests": "tests"},
     package_data={"cwlupgrader.tests": ["../testdata/**/*.cwl"]},
     install_requires=[
         "setuptools",
-        "ruamel.yaml >= 0.16.0, < 0.17.27;python_version>='3.10'",
-        "ruamel.yaml >= 0.15.98, < 0.17.27;python_version>='3.9'",
-        "ruamel.yaml >= 0.15.78, < 0.17.27;python_version>='3.8'",
-        "ruamel.yaml >= 0.15.71, < 0.17.27",
+        "ruamel.yaml >= 0.16.0, < 0.18;python_version>='3.10'",
+        "ruamel.yaml >= 0.15.98, < 0.18;python_version>='3.9'",
+        "ruamel.yaml >= 0.15.78, < 0.18;python_version>='3.8'",
+        "ruamel.yaml >= 0.15.71, < 0.18",
         "schema_salad",
     ],
     entry_points={"console_scripts": ["cwl-upgrader = cwlupgrader.main:main"]},
     python_requires=">=3.6, <4",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Console",
```

### Comparing `cwl-upgrader-1.2.7/testdata/draft-3/attributor-prok-cheetah.cwl` & `cwl-upgrader-1.2.8/testdata/draft-3/attributor-prok-cheetah.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.7/testdata/draft-3/wf.cwl` & `cwl-upgrader-1.2.8/testdata/draft-3/wf.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.7/testdata/v1.0/attributor-prok-cheetah.cwl` & `cwl-upgrader-1.2.8/testdata/v1.0/attributor-prok-cheetah.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.7/testdata/v1.0/conflict-wf.cwl` & `cwl-upgrader-1.2.8/testdata/v1.0/conflict-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.7/testdata/v1.1/conflict-wf.cwl` & `cwl-upgrader-1.2.8/testdata/v1.1/conflict-wf.cwl`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.7/tests/test_complete.py` & `cwl-upgrader-1.2.8/tests/test_complete.py`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.7/tests/test_output_dir.py` & `cwl-upgrader-1.2.8/tests/test_output_dir.py`

 * *Files identical despite different names*

### Comparing `cwl-upgrader-1.2.7/tests/util.py` & `cwl-upgrader-1.2.8/tests/util.py`

 * *Files identical despite different names*

