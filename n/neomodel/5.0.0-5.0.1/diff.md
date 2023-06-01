# Comparing `tmp/neomodel-5.0.0.tar.gz` & `tmp/neomodel-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neomodel-5.0.0.tar", last modified: Tue Apr  4 13:17:51 2023, max compression
+gzip compressed data, was "neomodel-5.0.1.tar", last modified: Thu Jun  1 16:08:29 2023, max compression
```

## Comparing `neomodel-5.0.0.tar` & `neomodel-5.0.1.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.107010 neomodel-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 13:17:35.000000 neomodel-5.0.0/.env
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.099011 neomodel-5.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-04 13:17:35.000000 neomodel-5.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.099011 neomodel-5.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-04 13:17:35.000000 neomodel-5.0.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-04 13:17:35.000000 neomodel-5.0.0/.github/workflows/integration-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-04-04 13:17:35.000000 neomodel-5.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-04 13:17:35.000000 neomodel-5.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-04 13:17:35.000000 neomodel-5.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-04 13:17:35.000000 neomodel-5.0.0/AUTHORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15332 2023-04-04 13:17:35.000000 neomodel-5.0.0/Changelog
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-04 13:17:35.000000 neomodel-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-04 13:17:51.107010 neomodel-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-04-04 13:17:35.000000 neomodel-5.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-04 13:17:35.000000 neomodel-5.0.0/dev
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.099011 neomodel-5.0.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.099011 neomodel-5.0.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.099011 neomodel-5.0.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/_static/neomodel-148.png
--rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/_static/neomodel-300.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.095010 neomodel-5.0.0/doc/source/_themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.099011 neomodel-5.0.0/doc/source/_themes/alabaster/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/_themes/alabaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/_themes/alabaster/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/_themes/alabaster/about.html
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/_themes/alabaster/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/_themes/alabaster/navigation.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.099011 neomodel-5.0.0/doc/source/_themes/alabaster/static/
--rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/_themes/alabaster/static/alabaster.css_t
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/_themes/alabaster/support.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/_themes/alabaster/theme.conf
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/batch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9050 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/cypher.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/extending.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/hooks.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/module_documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/properties.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/queries.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11668 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/relationships.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/spatial_properties.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-04-04 13:17:35.000000 neomodel-5.0.0/doc/source/transactions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-04 13:17:35.000000 neomodel-5.0.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.103011 neomodel-5.0.0/neomodel/
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/cardinality.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.103011 neomodel-5.0.0/neomodel/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/contrib/semi_structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    16047 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/contrib/spatial_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)    23276 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9521 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    29926 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/match.py
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/match_q.py
--rw-r--r--   0 runner    (1001) docker     (123)    18947 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/relationship.py
--rw-r--r--   0 runner    (1001) docker     (123)    17588 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/relationship_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    14933 2023-04-04 13:17:35.000000 neomodel-5.0.0/neomodel/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.103011 neomodel-5.0.0/neomodel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4888 2023-04-04 13:17:51.000000 neomodel-5.0.0/neomodel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-04-04 13:17:51.000000 neomodel-5.0.0/neomodel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 13:17:51.000000 neomodel-5.0.0/neomodel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-04 13:17:51.000000 neomodel-5.0.0/neomodel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-04 13:17:51.000000 neomodel-5.0.0/neomodel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-04 13:17:51.000000 neomodel-5.0.0/neomodel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-04 13:17:35.000000 neomodel-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-04-04 13:17:35.000000 neomodel-5.0.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.103011 neomodel-5.0.0/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-04 13:17:35.000000 neomodel-5.0.0/scripts/docker-neo4j.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-04-04 13:17:35.000000 neomodel-5.0.0/scripts/neomodel_install_labels.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1044 2023-04-04 13:17:35.000000 neomodel-5.0.0/scripts/neomodel_remove_labels.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 13:17:51.107010 neomodel-5.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.107010 neomodel-5.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_cardinality.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:51.107010 neomodel-5.0.0/test/test_contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_contrib/test_semi_structured.py
--rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_contrib/test_spatial_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_contrib/test_spatial_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_cypher.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_indexing.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_issue112.py
--rw-r--r--   0 runner    (1001) docker     (123)    13730 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_issue283.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_issue600.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_label_drop.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_label_install.py
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_match_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_relationship_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_relative_relationships.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/test_transactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-04-04 13:17:35.000000 neomodel-5.0.0/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-04 13:17:35.000000 neomodel-5.0.0/tests-with-docker-compose.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:08:17.000000 neomodel-5.0.1/.env
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.489851 neomodel-5.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-01 16:08:17.000000 neomodel-5.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.489851 neomodel-5.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-01 16:08:17.000000 neomodel-5.0.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-01 16:08:17.000000 neomodel-5.0.1/.github/workflows/integration-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-01 16:08:17.000000 neomodel-5.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-01 16:08:17.000000 neomodel-5.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-01 16:08:17.000000 neomodel-5.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-01 16:08:17.000000 neomodel-5.0.1/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15896 2023-06-01 16:08:17.000000 neomodel-5.0.1/Changelog
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-01 16:08:17.000000 neomodel-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-01 16:08:29.497851 neomodel-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4040 2023-06-01 16:08:17.000000 neomodel-5.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 16:08:17.000000 neomodel-5.0.1/dev
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.489851 neomodel-5.0.1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.493851 neomodel-5.0.1/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.493851 neomodel-5.0.1/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_static/neomodel-148.png
+-rw-r--r--   0 runner    (1001) docker     (123)     9528 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_static/neomodel-300.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.489851 neomodel-5.0.1/doc/source/_themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.493851 neomodel-5.0.1/doc/source/_themes/alabaster/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/about.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/navigation.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.493851 neomodel-5.0.1/doc/source/_themes/alabaster/static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/static/alabaster.css_t
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/_themes/alabaster/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/batch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9076 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/cypher.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/extending.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/hooks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/module_documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8522 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/properties.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/queries.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11814 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/relationships.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8427 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/spatial_properties.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-06-01 16:08:17.000000 neomodel-5.0.1/doc/source/transactions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-01 16:08:17.000000 neomodel-5.0.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.493851 neomodel-5.0.1/neomodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/neomodel/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2218 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/contrib/semi_structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14800 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/contrib/spatial_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22464 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8706 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28792 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/match_q.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/relationship.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17147 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/relationship_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14887 2023-06-01 16:08:17.000000 neomodel-5.0.1/neomodel/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/neomodel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5124 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 16:08:29.000000 neomodel-5.0.1/neomodel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-06-01 16:08:17.000000 neomodel-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-01 16:08:17.000000 neomodel-5.0.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 16:08:17.000000 neomodel-5.0.1/scripts/docker-neo4j.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1959 2023-06-01 16:08:17.000000 neomodel-5.0.1/scripts/neomodel_install_labels.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1044 2023-06-01 16:08:17.000000 neomodel-5.0.1/scripts/neomodel_remove_labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:08:29.497851 neomodel-5.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5866 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4183 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_cardinality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:29.497851 neomodel-5.0.1/test/test_contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_contrib/test_semi_structured.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13020 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_contrib/test_spatial_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8997 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_contrib/test_spatial_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_cypher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_indexing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_issue112.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14083 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_issue283.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_issue600.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_label_drop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_label_install.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13365 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_match_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12384 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4272 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_relationship_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_relative_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/test_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-01 16:08:17.000000 neomodel-5.0.1/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-01 16:08:17.000000 neomodel-5.0.1/tests-with-docker-compose.sh
```

### Comparing `neomodel-5.0.0/.github/workflows/codeql-analysis.yml` & `neomodel-5.0.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/.github/workflows/python-publish.yml` & `neomodel-5.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/AUTHORS.txt` & `neomodel-5.0.1/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/Changelog` & `neomodel-5.0.1/Changelog`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Version 5.0.1 2023-06
+* Removed deprecated methods StructuredRel.delete and RelationshipManager.search
+* Extended test coverage, fixed some typos, improve linting
+* Upcoming breaking change notice : Version 5.1.0 will introduce a breaking change for users targeting a Neo4j database in version 5. This release will introduce Neo4j's new element_id, which replaces id. The breaking change will happen if you have custom Cypher queries that do things like "WHERE id(n)=$id" => you will have to use Cypher's elementId() function instead starting from neomodel 5.1.0
+
 Version 5.0.0 2023-03
 * Confirmed support of Neo4j versions 5.x and 4.4 (LTS)
 * Dropped support of EOL Neo4j versions (4.3 and below)
 * Confirmed support of Python 3.11
 * Migrated RelationshipTo/RelationshipFrom from a method to a class for consistency.
 * Add support for relationship indexes
 * Auto-generated indexes now have a deterministic name
```

### Comparing `neomodel-5.0.0/LICENSE` & `neomodel-5.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/PKG-INFO` & `neomodel-5.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neomodel
-Version: 5.0.0
+Version: 5.0.1
 Summary: An object mapper for the neo4j graph database.
 Author-email: Robin Edwards <robin.ge@gmail.com>
 Maintainer: Cristina Escalante
 Maintainer-email: Athanasios Anastasiou <athanastasiou@gmail.com>, Marius Conjeaud <marius.conjeaud@outlook.com>
 License: MIT
 Project-URL: documentation, https://neomodel.readthedocs.io/en/latest/
 Project-URL: repository, http://github.com/neo4j-contrib/neomodel
@@ -117,14 +117,20 @@
 
 Ensure ``dbms.security.auth_enabled=true`` in your database configuration file.
 Setup a virtual environment, install neomodel for development and run the test suite: ::
 
     $ pip install -e '.[dev]'
     $ pytest
 
+The tests in "test_connection.py" will fail locally if you don't specify the following environment variables::
+
+    $ export AURA_TEST_DB_USER=username
+    $ export AURA_TEST_DB_PASSWORD=password
+    $ export AURA_TEST_DB_HOSTNAME=url
+
 If you are running a neo4j database for the first time the test suite will set the password to 'test'.
 If the database is already populated, the test suite will abort with an error message and ask you to re-run it with the
 ``--resetdb`` switch. This is a safeguard to ensure that the test suite does not accidentally wipe out a database if you happen 
 to not have restarted your Neo4j server to point to a (usually named) ``debug.db`` database.
 
 If you have ``docker-compose`` installed, you can run the test suite against all supported Python
 interpreters and neo4j versions: ::
```

### Comparing `neomodel-5.0.0/README.rst` & `neomodel-5.0.1/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -91,14 +91,20 @@
 
 Ensure ``dbms.security.auth_enabled=true`` in your database configuration file.
 Setup a virtual environment, install neomodel for development and run the test suite: ::
 
     $ pip install -e '.[dev]'
     $ pytest
 
+The tests in "test_connection.py" will fail locally if you don't specify the following environment variables::
+
+    $ export AURA_TEST_DB_USER=username
+    $ export AURA_TEST_DB_PASSWORD=password
+    $ export AURA_TEST_DB_HOSTNAME=url
+
 If you are running a neo4j database for the first time the test suite will set the password to 'test'.
 If the database is already populated, the test suite will abort with an error message and ask you to re-run it with the
 ``--resetdb`` switch. This is a safeguard to ensure that the test suite does not accidentally wipe out a database if you happen 
 to not have restarted your Neo4j server to point to a (usually named) ``debug.db`` database.
 
 If you have ``docker-compose`` installed, you can run the test suite against all supported Python
 interpreters and neo4j versions: ::
```

### Comparing `neomodel-5.0.0/doc/Makefile` & `neomodel-5.0.1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/make.bat` & `neomodel-5.0.1/doc/make.bat`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/_static/neomodel-148.png` & `neomodel-5.0.1/doc/source/_static/neomodel-148.png`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/_static/neomodel-300.png` & `neomodel-5.0.1/doc/source/_static/neomodel-300.png`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/_themes/alabaster/about.html` & `neomodel-5.0.1/doc/source/_themes/alabaster/about.html`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/_themes/alabaster/layout.html` & `neomodel-5.0.1/doc/source/_themes/alabaster/layout.html`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/_themes/alabaster/static/alabaster.css_t` & `neomodel-5.0.1/doc/source/_themes/alabaster/static/alabaster.css_t`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/_themes/alabaster/support.py` & `neomodel-5.0.1/doc/source/_themes/alabaster/support.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/_themes/alabaster/theme.conf` & `neomodel-5.0.1/doc/source/_themes/alabaster/theme.conf`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/batch.rst` & `neomodel-5.0.1/doc/source/batch.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/conf.py` & `neomodel-5.0.1/doc/source/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "alabaster",
     "sphinx.ext.autodoc",
     "sphinx.ext.intersphinx",
+    "sphinx_copybutton",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # The suffix of source filenames.
 source_suffix = ".rst"
@@ -117,15 +118,15 @@
 # html_theme_options = {}
 html_theme_options = {
     "logo": "neomodel-148.png",
     #    'logo_align': 'left',
     "github_user": "neo4j-contrib",
     "github_repo": "neomodel",
     # 'github_branch': 'master',
-    "travis_button": True,
+    "travis_button": False,
 }
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 html_theme_path = [alabaster.get_path()]
```

### Comparing `neomodel-5.0.0/doc/source/configuration.rst` & `neomodel-5.0.1/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/cypher.rst` & `neomodel-5.0.1/doc/source/cypher.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/extending.rst` & `neomodel-5.0.1/doc/source/extending.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/getting_started.rst` & `neomodel-5.0.1/doc/source/getting_started.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/hooks.rst` & `neomodel-5.0.1/doc/source/hooks.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/index.rst` & `neomodel-5.0.1/doc/source/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,20 @@
 .. _neo4j_driver: https://github.com/neo4j/neo4j-python-driver
 .. _django_neomodel: https://github.com/neo4j-contrib/django-neomodel
 
 Requirements
 ============
 
 For releases 5.x :
+
 - Python 3.7+
 - neo4j 5.x, 4.4 (LTS)
 
 For releases 4.x :
+
 - Python 3.7 -> 3.10
 - Neo4j 4.x (including 4.4 LTS for neomodel version 4.0.10)
 
 Installation
 ============
 
 Install from pypi (recommended)::
```

### Comparing `neomodel-5.0.0/doc/source/module_documentation.rst` & `neomodel-5.0.1/doc/source/module_documentation.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/properties.rst` & `neomodel-5.0.1/doc/source/properties.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/queries.rst` & `neomodel-5.0.1/doc/source/queries.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/relationships.rst` & `neomodel-5.0.1/doc/source/relationships.rst`

 * *Files 1% similar despite different names*

```diff
@@ -247,16 +247,21 @@
 
     definition = dict(node_class=Person, direction=OUTGOING,
                       relation_type=None, model=None)
     relations_traversal = Traversal(jim, Person.__label__,
                                     definition)
     all_jims_relations = relations_traversal.all()
 
-The ``defintion`` argument is a :term:`py3:mapping` with these items:
+The ``definition`` argument is a :term:`py3:mapping` with these items:
 
 =================  ===============================================================
 ``node_class``     The class of the traversal target node.
 ``direction``      ``match.OUTGOING`` / ``match.INCOMING`` / ``match.EITHER``
 ``relation_type``  Can be ``None`` (for any direction), ``*`` for all paths
                    or an explicit name of a relation type (the edge's label).
 ``model``          The class of the relation model, ``None`` for such without one.
 =================  ===============================================================
+
+.. note::
+
+    The ``RelationshipTo`` and ``RelationshipFrom`` objects are simply a proxy
+    for defining Traversal objects at the class level.
```

### Comparing `neomodel-5.0.0/doc/source/spatial_properties.rst` & `neomodel-5.0.1/doc/source/spatial_properties.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/doc/source/transactions.rst` & `neomodel-5.0.1/doc/source/transactions.rst`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/docker-compose.yml` & `neomodel-5.0.1/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/neomodel/__init__.py` & `neomodel-5.0.1/neomodel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,8 +34,8 @@
 from .relationship import StructuredRel
 from .util import change_neo4j_password, clear_neo4j_database
 
 __author__ = "Robin Edwards"
 __email__ = "robin.ge@gmail.com"
 __license__ = "MIT"
 __package__ = "neomodel"
-__version__ = "5.0.0"
+__version__ = "5.0.1"
```

### Comparing `neomodel-5.0.0/neomodel/cardinality.py` & `neomodel-5.0.1/neomodel/cardinality.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/neomodel/contrib/semi_structured.py` & `neomodel-5.0.1/neomodel/contrib/semi_structured.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/neomodel/contrib/spatial_properties.py` & `neomodel-5.0.1/neomodel/contrib/spatial_properties.py`

 * *Files 9% similar despite different names*

```diff
@@ -98,33 +98,25 @@
         latitude = kwargs.pop("latitude", None)
         height = kwargs.pop("height", None)
 
         _x, _y, _z = None, None, None
 
         # CRS validity check is common to both types of constructors that follow
         if crs is not None and crs not in ACCEPTABLE_CRS:
-            raise ValueError(
-                "Invalid CRS({}). Expected one of {}".format(
-                    crs, ",".join(ACCEPTABLE_CRS)
-                )
-            )
+            raise ValueError(f"Invalid CRS({crs}). Expected one of {','.join(ACCEPTABLE_CRS)}")
         self._crs = crs
 
         # If positional arguments have been supplied, then this is a possible call to the copy constructor or
         # initialisation by a coordinate iterable as per ShapelyPoint constructor.
         if len(args) > 0:
             # If a coordinate iterable was passed, emulate a call with x,y[,z] parameters
             if isinstance(args[0], (tuple, list)):
                 # Check dimensionality of tuple
                 if len(args[0]) < 2 or len(args[0]) > 3:
-                    raise ValueError(
-                        "Invalid vector dimensions. Expected 2 or 3, received {}".format(
-                            len(args[0])
-                        )
-                    )
+                    raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0])}")
                 x = args[0][0]
                 y = args[0][1]
                 if len(args[0]) == 3:
                     z = args[0][2]
             # If another "Point" was passed, then this is a call to the copy constructor
             elif isinstance(args[0], ShapelyPoint):
                 super().__init__(args[0])
@@ -144,28 +136,18 @@
                     if len(args[0].coords[0]) == 2:
                         if crs is None:
                             self._crs = "cartesian"
                     elif len(args[0].coords[0]) == 3:
                         if crs is None:
                             self._crs = "cartesian-3d"
                     else:
-                        raise ValueError(
-                            "Invalid vector dimensions. "
-                            "Expected 2 or 3, received {}".format(
-                                len(args[0].coords[0])
-                            )
-                        )
+                        raise ValueError(f"Invalid vector dimensions. Expected 2 or 3, received {len(args[0].coords[0])}")
                 return
             else:
-                raise TypeError(
-                    "Invalid object passed to copy constructor. "
-                    "Expected NeomodelPoint or shapely Point, received {}".format(
-                        type(args[0])
-                    )
-                )
+                raise TypeError(f"Invalid object passed to copy constructor. Expected NeomodelPoint or shapely Point, received {type(args[0])}")
 
         # Initialisation is either via x,y[,z] XOR longitude,latitude[,height]. Specifying both leads to an error.
         if any(i is not None for i in [x, y, z]) and any(
             i is not None for i in [latitude, longitude, height]
         ):
             raise ValueError(
                 "Invalid instantiation via arguments. "
@@ -204,80 +186,70 @@
             _x = x
             _y = y
 
         if _z is None:
             if "-3d" not in self._crs:
                 super().__init__((float(_x), float(_y)), **kwargs)
             else:
-                raise ValueError(
-                    "Invalid vector dimensions(2) for given CRS({}).".format(self._crs)
-                )
+                raise ValueError(f"Invalid vector dimensions(2) for given CRS({self._crs}).")
         else:
             if "-3d" in self._crs:
                 super().__init__((float(_x), float(_y), float(_z)), **kwargs)
             else:
-                raise ValueError(
-                    "Invalid vector dimensions(3) for given CRS({}).".format(self._crs)
-                )
+                raise ValueError(f"Invalid vector dimensions(3) for given CRS({self._crs}).")
 
     @property
     def crs(self):
         return self._crs
 
     @property
     def x(self):
         if not self._crs.startswith("cartesian"):
             raise AttributeError(
-                'Invalid coordinate ("x") for points defined over {}'.format(self.crs)
+                f'Invalid coordinate ("x") for points defined over {self.crs}'
             )
         return super().x
 
     @property
     def y(self):
         if not self._crs.startswith("cartesian"):
             raise AttributeError(
-                'Invalid coordinate ("y") for points defined over {}'.format(self.crs)
+                f'Invalid coordinate ("y") for points defined over {self.crs}'
             )
         return super().y
 
     @property
     def z(self):
         if not self._crs == "cartesian-3d":
             raise AttributeError(
-                'Invalid coordinate ("z") for points defined over {}'.format(self.crs)
+                f'Invalid coordinate ("z") for points defined over {self.crs}'
             )
         return super().z
 
     @property
     def latitude(self):
         if not self._crs.startswith("wgs-84"):
             raise AttributeError(
-                'Invalid coordinate ("latitude") for points defined over {}'.format(
-                    self.crs
-                )
+                f'Invalid coordinate ("latitude") for points defined over {self.crs}'
             )
         return super().y
 
     @property
     def longitude(self):
         if not self._crs.startswith("wgs-84"):
             raise AttributeError(
-                'Invalid coordinate ("longitude") for points defined over {}'.format(
-                    self.crs
-                )
+                f'Invalid coordinate ("longitude") for points defined over {self.crs}'
             )
         return super().x
 
     @property
     def height(self):
         if not self._crs == "wgs-84-3d":
             raise AttributeError(
-                'Invalid coordinate ("height") for points defined over {}'.format(
-                    self.crs
-                )
+                f'Invalid coordinate ("height") for points defined over {self.crs}'
             )
         return super().z
 
     # The following operations are necessary here due to the way queries (and more importantly their parameters) get
     # combined and evaluated in neomodel. Specifically, query expressions get duplicated with deep copies and any valid
     # datatype values should also implement these operations.
     def __copy__(self):
@@ -308,30 +280,21 @@
         if "crs" in kwargs:
             crs = kwargs["crs"]
             del kwargs["crs"]
         else:
             crs = None
 
         if crs is None or (crs not in ACCEPTABLE_CRS):
-            raise ValueError(
-                "Invalid CRS({}). "
-                "Point properties require CRS to be one of {}".format(
-                    crs, ",".join(ACCEPTABLE_CRS)
-                )
-            )
+            raise ValueError(f"Invalid CRS({crs}). Point properties require CRS to be one of {','.join(ACCEPTABLE_CRS)}")
 
         # If a default value is passed and it is not a callable, then make sure it is in the right type
         if "default" in kwargs:
             if not hasattr(kwargs["default"], "__call__"):
                 if not isinstance(kwargs["default"], NeomodelPoint):
-                    raise TypeError(
-                        "Invalid default value. "
-                        "Expected NeomodelPoint, received {}".format(
-                            type(kwargs["default"])
-                        )
+                    raise TypeError(f"Invalid default value. Expected NeomodelPoint, received {type(kwargs['default'])}"
                     )
 
         super().__init__(*args, **kwargs)
         self._crs = crs
 
     @validator
     def inflate(self, value):
@@ -340,34 +303,24 @@
 
         :param value: Value returned from the database
         :type value: Neo4J POINT
         :return: NeomodelPoint
         """
         if not isinstance(value, neo4j.spatial.Point):
             raise TypeError(
-                "Invalid datatype to inflate. Expected POINT datatype, received {}".format(
-                    type(value)
-                )
+                f"Invalid datatype to inflate. Expected POINT datatype, received {type(value)}"
             )
 
         try:
             value_point_crs = SRID_TO_CRS[value.srid]
         except KeyError as e:
-            raise ValueError(
-                "Invalid SRID to inflate. "
-                "Expected one of {}, received {}".format(SRID_TO_CRS.keys(), value.srid)
-            ) from e
+            raise ValueError(f"Invalid SRID to inflate. Expected one of {SRID_TO_CRS.keys()}, received {value.srid}") from e
 
         if self._crs != value_point_crs:
-            raise ValueError(
-                "Invalid CRS. "
-                "Expected POINT defined over {}, received {}".format(
-                    self._crs, value_point_crs
-                )
-            )
+            raise ValueError(f"Invalid CRS. Expected POINT defined over {self._crs}, received {value_point_crs}")
         # cartesian
         if value.srid == 7203:
             return NeomodelPoint(x=value.x, y=value.y)
         # cartesian-3d
         if value.srid == 9157:
             return NeomodelPoint(x=value.x, y=value.y, z=value.z)
         # wgs-84
@@ -389,25 +342,19 @@
 
         :param value: The point that was assigned as value to a property in the model
         :type value: NeomodelPoint
         :return: Neo4J POINT
         """
         if not isinstance(value, NeomodelPoint):
             raise TypeError(
-                "Invalid datatype to deflate. Expected NeomodelPoint, received {}".format(
-                    type(value)
-                )
+                f"Invalid datatype to deflate. Expected NeomodelPoint, received {type(value)}"
             )
 
         if not value.crs == self._crs:
-            raise ValueError(
-                "Invalid CRS. "
-                "Expected NeomodelPoint defined over {}, "
-                "received NeomodelPoint defined over {}".format(self._crs, value.crs)
-            )
+            raise ValueError(f"Invalid CRS. Expected NeomodelPoint defined over {self._crs}, received NeomodelPoint defined over {value.crs}")
 
         if value.crs == "cartesian-3d":
             return neo4j.spatial.CartesianPoint((value.x, value.y, value.z))
         if value.crs == "cartesian":
             return neo4j.spatial.CartesianPoint((value.x, value.y))
         if value.crs == "wgs-84":
             return neo4j.spatial.WGS84Point((value.longitude, value.latitude))
```

### Comparing `neomodel-5.0.0/neomodel/core.py` & `neomodel-5.0.1/neomodel/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,25 +52,20 @@
 
     results, meta = db.cypher_query("SHOW INDEXES")
     results_as_dict = [dict(zip(meta, row)) for row in results]
     for index in results_as_dict:
         # Neo4j 4.3 introduced token lookup indexes
         # Two are created automatically so should not be dropped
         # They can be recognized because their labelsOrTypes and properties arrays are empty
-        if not index["labelsOrTypes"]:
-            if index["properties"]:
-                raise ValueError(
-                    f'Index {index["name"]} has no labels but has properties({",".join(index["properties"])}). Unknown index'
+        if index["labelsOrTypes"] and index["properties"]:
+            db.cypher_query("DROP INDEX " + index["name"])
+            if not quiet:
+                stdout.write(
+                    f' - Dropping index on labels {",".join(index["labelsOrTypes"])} with properties {",".join(index["properties"])}.\n'
                 )
-            continue
-        db.cypher_query("DROP INDEX " + index["name"])
-        if not quiet:
-            stdout.write(
-                f' - Dropping index on labels {",".join(index["labelsOrTypes"])} with properties {",".join(index["properties"])}.\n'
-            )
     if not quiet:
         stdout.write("\n")
 
 
 def remove_all_labels(stdout=None):
     """
     Calls functions for dropping constraints and indexes.
@@ -181,15 +176,15 @@
                         else:
                             raise
 
 
 def install_all_labels(stdout=None):
     """
     Discover all subclasses of StructuredNode in your application and execute install_labels on each.
-    Note: code most be loaded (imported) in order for a class to be discovered.
+    Note: code must be loaded (imported) in order for a class to be discovered.
 
     :param stdout: output stream
     :return: None
     """
 
     if not stdout or stdout is None:
         stdout = sys.stdout
@@ -317,26 +312,14 @@
         :return: NodeSet
         :rtype: NodeSet
         """
         from .match import NodeSet
 
         return NodeSet(cls)
 
-    @property
-    def _id(self, val):
-        warnings.warn(
-            "the _id property is deprecated please use .id",
-            category=DeprecationWarning,
-            stacklevel=1,
-        )
-        if val:
-            self.id = val
-
-        return self.id
-
     # methods
 
     @classmethod
     def _build_merge_query(
         cls, merge_params, update_existing=False, lazy=False, relationship=None
     ):
         """
@@ -345,44 +328,34 @@
         :param merge_params: The target node match parameters, each node must have a "create" key and optional "update".
         :type merge_params: list of dict
         :param update_existing: True to update properties of existing nodes, default False to keep existing values.
         :type update_existing: bool
         :rtype: tuple
         """
         query_params = dict(merge_params=merge_params)
-        n_merge = "n:{0} {{{1}}}".format(
-            ":".join(cls.inherited_labels()),
-            ", ".join(
-                "{0}: params.create.{0}".format(getattr(cls, p).db_property or p)
-                for p in cls.__required_properties__
-            ),
-        )
+        n_merge_labels = ":".join(cls.inherited_labels())
+        n_merge_prm = ", ".join((f"{getattr(cls, p).db_property or p}: params.create.{getattr(cls, p).db_property or p}" for p in cls.__required_properties__))
+        n_merge = f"n:{n_merge_labels} {{{n_merge_prm}}}"
         if relationship is None:
             # create "simple" unwind query
-            query = "UNWIND $merge_params as params\n MERGE ({0})\n ".format(n_merge)
+            query = f"UNWIND $merge_params as params\n MERGE ({n_merge})\n "
         else:
             # validate relationship
             if not isinstance(relationship.source, StructuredNode):
-                raise ValueError(
-                    "relationship source [{0}] is not a StructuredNode".format(
-                        repr(relationship.source)
-                    )
-                )
+                raise ValueError(f"relationship source [{repr(relationship.source)}] is not a StructuredNode")
             relation_type = relationship.definition.get("relation_type")
             if not relation_type:
                 raise ValueError(
                     "No relation_type is specified on provided relationship"
                 )
 
             from .match import _rel_helper
 
             query_params["source_id"] = relationship.source.id
-            query = "MATCH (source:{0}) WHERE ID(source) = $source_id\n ".format(
-                relationship.source.__label__
-            )
+            query = f"MATCH (source:{relationship.source.__label__}) WHERE ID(source) = $source_id\n "
             query += "WITH source\n UNWIND $merge_params as params \n "
             query += "MERGE "
             query += _rel_helper(
                 lhs="source",
                 rhs=n_merge,
                 ident=None,
                 relation_type=relation_type,
@@ -400,20 +373,15 @@
         else:
             query += "RETURN n"
 
         return query, query_params
 
     @classmethod
     def category(cls):
-        raise NotImplementedError(
-            "Category was deprecated and has now been removed, "
-            "the functionality is now achieved using the {0}.nodes attribute".format(
-                cls.__name__
-            )
-        )
+        raise NotImplementedError(f"Category was deprecated and has now been removed, the functionality is now achieved using the {cls.__name__}.nodes attribute")
 
     @classmethod
     def create(cls, *props, **kwargs):
         """
         Call to CREATE with parameters map. A new instance will be created and saved.
 
         :param props: dict of properties to create the nodes.
@@ -428,15 +396,15 @@
                 "streaming is not supported by bolt, please remove the kwarg",
                 category=DeprecationWarning,
                 stacklevel=1,
             )
 
         lazy = kwargs.get("lazy", False)
         # create mapped query
-        query = "CREATE (n:{0} $create_params)".format(":".join(cls.inherited_labels()))
+        query = f"CREATE (n:{':'.join(cls.inherited_labels())} $create_params)"
 
         # close query
         if lazy:
             query += " RETURN id(n)"
         else:
             query += " RETURN n"
 
@@ -626,23 +594,19 @@
         """
         self._pre_action_check("labels")
         return self.cypher("MATCH (n) WHERE id(n)=$self " "RETURN labels(n)")[0][0][0]
 
     def _pre_action_check(self, action):
         if hasattr(self, "deleted") and self.deleted:
             raise ValueError(
-                "{0}.{1}() attempted on deleted node".format(
-                    self.__class__.__name__, action
-                )
+                f"{self.__class__.__name__}.{action}() attempted on deleted node"
             )
         if not hasattr(self, "id"):
             raise ValueError(
-                "{0}.{1}() attempted on unsaved node".format(
-                    self.__class__.__name__, action
-                )
+                f"{self.__class__.__name__}.{action}() attempted on unsaved node"
             )
 
     def refresh(self):
         """
         Reload the node from neo4j
         """
         self._pre_action_check("refresh")
@@ -666,19 +630,19 @@
 
         # create or update instance node
         if hasattr(self, "id"):
             # update
             params = self.deflate(self.__properties__, self)
             query = "MATCH (n) WHERE id(n)=$self \n"
             query += "\n".join(
-                ["SET n.{0} = ${1}".format(key, key) + "\n" for key in params.keys()]
+                [f"SET n.{key} = ${key}" + "\n" for key in params.keys()]
             )
             for label in self.inherited_labels():
-                query += "SET n:`{0}`\n".format(label)
+                query += f"SET n:`{label}`\n"
             self.cypher(query, params)
         elif hasattr(self, "deleted") and self.deleted:
             raise ValueError(
-                "{0}.save() attempted on deleted node".format(self.__class__.__name__)
+                f"{self.__class__.__name__}.save() attempted on deleted node"
             )
         else:  # create
             self.id = self.create(self.__properties__)[0].id
         return self
```

### Comparing `neomodel-5.0.0/neomodel/exceptions.py` & `neomodel-5.0.1/neomodel/exceptions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 class NeomodelException(Exception):
     """
     A base class that identifies all exceptions raised by :mod:`neomodel`.
     """
+    pass
 
 
 class AttemptedCardinalityViolation(NeomodelException):
     """
     Attempted to alter the database state against the cardinality definitions.
 
     Example: a relationship of type `One` trying to connect a second node.
     """
+    pass
 
 
 class CardinalityViolation(NeomodelException):
     """
     The state of database doesn't match the nodes cardinality definition.
 
     For example a relationship type `OneOrMore` returns no nodes.
     """
 
     def __init__(self, rel_manager, actual):
         self.rel_manager = str(rel_manager)
         self.actual = str(actual)
 
     def __str__(self):
-        return "CardinalityViolation: Expected: {0}, got: {1}.".format(
-            self.rel_manager, self.actual
-        )
+        return f"CardinalityViolation: Expected: {self.rel_manager}, got: {self.actual}."
 
 
 class ModelDefinitionException(NeomodelException):
     """
     Abstract exception to handle error conditions related to the node-to-class registry.
     """
 
@@ -51,15 +51,15 @@
         Returns the current node class registry string formatted as a list of
         Labels --> <class to instantiate> entries.
 
         :return: str
         """
         ncr_items = list(
             map(
-                lambda x: "{} --> {}".format(",".join(x[0]), x[1]),
+                lambda x: f"{','.join(x[0])} --> {x[1]}",
                 self.current_node_class_registry.items(),
             )
         )
         return "\n".join(ncr_items)
 
 
 class NodeClassNotDefined(ModelDefinitionException):
@@ -69,36 +69,28 @@
     nodes for which class definitions do exist but have not been imported
     or because the retrieved nodes contain more labels for a known class.
 
     In either of these cases the mismatch must be reported
     """
 
     def __str__(self):
-        node_labels = ",".join(self.db_node_rel_class.labels())
+        node_labels = ",".join(self.db_node_rel_class.labels)
 
-        return "Node with labels {} does not resolve to any of the known objects\n{}\n".format(
-            node_labels, self._get_node_class_registry_formatted()
-        )
+        return f"Node with labels {node_labels} does not resolve to any of the known objects\n{self._get_node_class_registry_formatted()}\n"
 
 
 class RelationshipClassNotDefined(ModelDefinitionException):
     """
     Raised when it is impossible to resolve a Neo4j driver Relationship to
     a data model object.
     """
 
     def __str__(self):
         relationship_type = self.db_node_rel_class.type
-        return (
-            "Relationship of type {} does not resolve to any of the known "
-            "objects\n{}\n".format(
-                relationship_type, self._get_node_class_registry_formatted()
-            )
-        )
-
+        return f"Relationship of type {relationship_type} does not resolve to any of the known objects\n{self._get_node_class_registry_formatted()}\n"
 
 class RelationshipClassRedefined(ModelDefinitionException):
     """
     Raised when an attempt is made to re-map a relationship label to a relationship model of an entirely different type
     """
 
     def __init__(
@@ -118,60 +110,42 @@
         :type remapping_to_class: class
         """
         super().__init__(db_rel_class_type, current_node_class_registry)
         self.remapping_to_class = remapping_to_class
 
     def __str__(self):
         relationship_type = self.db_node_rel_class
-        return "Relationship of type {} redefined as {}.\n{}\n".format(
-            relationship_type,
-            self.remapping_to_class,
-            self._get_node_class_registry_formatted(),
-        )
+        return f"Relationship of type {relationship_type} redefined as {self.remapping_to_class}.\n{self._get_node_class_registry_formatted()}\n"
 
 
 class NodeClassAlreadyDefined(ModelDefinitionException):
     """
     Raised when an attempt is made to re-map a set of labels to a class
     that already has a mapping within the node-to-class registry.
     """
 
     def __str__(self):
         node_class_labels = ",".join(self.db_node_rel_class.inherited_labels())
 
-        return "Class {}.{} with labels {} already defined:\n{}\n".format(
-            self.db_node_rel_class.__module__,
-            self.db_node_rel_class.__name__,
-            node_class_labels,
-            self._get_node_class_registry_formatted(),
-        )
-
+        return f"Class {self.db_node_rel_class.__module__}.{self.db_node_rel_class.__name__} with labels {node_class_labels} already defined:\n{self._get_node_class_registry_formatted()}\n"
 
 class ConstraintValidationFailed(ValueError, NeomodelException):
     def __init__(self, msg):
         self.message = msg
 
 
 class DeflateError(ValueError, NeomodelException):
     def __init__(self, key, cls, msg, obj):
         self.property_name = key
         self.node_class = cls
         self.msg = msg
         self.obj = repr(obj)
 
     def __str__(self):
-        return (
-            "Attempting to deflate property '{0}' on {1} of class '{2}': "
-            "{3}".format(
-                self.property_name,
-                self.obj,
-                self.node_class.__name__,
-                self.msg,
-            )
-        )
+        return f"Attempting to deflate property '{self.property_name}' on {self.obj} of class '{self.node_class.__name__}': {self.msg}"
 
 
 class DoesNotExist(NeomodelException):
     _model_class = None
     """
     This class property refers the model class that a subclass of this class
     belongs to. It is set by :class:`~neomodel.core.NodeMeta`.
@@ -195,86 +169,58 @@
     def __init__(self, cls, key, value, nid):
         self.cls_name = cls.__name__
         self.property_name = key
         self.value = value
         self.nid = nid
 
     def __str__(self):
-        return """Found conflict with node {0}, has property '{1}' with value '{2}'
-            although class {3} already has a property '{1}'""".format(
-            self.nid, self.property_name, self.value, self.cls_name
-        )
+        return f"Found conflict with node {self.nid}, has property '{self.property_name}' with value '{self.value}' although class {self.cls_name} already has a property '{self.property_name}'"
 
 
 class InflateError(ValueError, NeomodelException):
     def __init__(self, key, cls, msg, obj=None):
         self.property_name = key
         self.node_class = cls
         self.msg = msg
         self.obj = repr(obj)
 
     def __str__(self):
-        return (
-            "Attempting to inflate property '{0}' on {1} of class '{2}': "
-            "{3}".format(
-                self.property_name,
-                self.obj,
-                self.node_class.__name__,
-                self.msg,
-            )
-        )
-
+        return f"Attempting to inflate property '{self.property_name}' on {self.obj} of class '{self.node_class.__name__}': {self.msg}"
 
 class DeflateConflict(InflateConflict):
     def __init__(self, cls, key, value, nid):
         self.cls_name = cls.__name__
         self.property_name = key
         self.value = value
         self.nid = nid if nid else "(unsaved)"
 
     def __str__(self):
-        return """Found trying to set property '{1}' with value '{2}' on node {0}
-            although class {3} already has a property '{1}'""".format(
-            self.nid, self.property_name, self.value, self.cls_name
-        )
-
+        return f"Found trying to set property '{self.property_name}' with value '{self.value}' on node {self.nid} although class {self.cls_name} already has a property '{self.property_name}'"
 
 class MultipleNodesReturned(ValueError, NeomodelException):
     def __init__(self, msg):
         self.message = msg
 
 
 class NotConnected(NeomodelException):
     def __init__(self, action, node1, node2):
         self.action = action
         self.node1 = node1
         self.node2 = node2
 
     def __str__(self):
-        return (
-            "Error performing '{0}' - Node {1} of type '{2}' is not "
-            "connected to {3} of type '{4}'.".format(
-                self.action,
-                self.node1.id,
-                self.node1.__class__.__name__,
-                self.node2.id,
-                self.node2.__class__.__name__,
-            )
-        )
-
+        return f"Error performing '{self.action}' - Node {self.node1.id} of type '{self.node1.__class__.__name__}' is not connected to {self.node2.id} of type '{self.node2.__class__.__name__}'."
 
 class RequiredProperty(NeomodelException):
     def __init__(self, key, cls):
         self.property_name = key
         self.node_class = cls
 
     def __str__(self):
-        return "property '{0}' on objects of class {1}".format(
-            self.property_name, self.node_class.__name__
-        )
+        return f"property '{self.property_name}' on objects of class {self.node_class.__name__}"
 
 
 class UniqueProperty(ConstraintValidationFailed):
     def __init__(self, msg):
         self.message = msg
```

### Comparing `neomodel-5.0.0/neomodel/match.py` & `neomodel-5.0.1/neomodel/match.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,48 +39,42 @@
     :param ident: A specific identity to name the relationship, or None.
     :type ident: str
     :param relation_type: None for all direct rels, * for all of any length, or a name of an explicit rel.
     :type relation_type: str
     :param direction: None or EITHER for all OUTGOING,INCOMING,EITHER. Otherwise OUTGOING or INCOMING.
     :param relation_properties: dictionary of relationship properties to match
     :returns: string
-    """
-
-    if direction == OUTGOING:
-        stmt = "-{0}->"
-    elif direction == INCOMING:
-        stmt = "<-{0}-"
-    else:
-        stmt = "-{0}-"
-
+    """ 
     rel_props = ""
 
     if relation_properties:
-        rel_props = " {{{0}}}".format(
-            ", ".join(
-                [
-                    "{0}: {1}".format(key, value)
-                    for key, value in relation_properties.items()
-                ]
-            )
-        )
+        rel_props_str = ', '.join((f"{key}: {value}" for key, value in relation_properties.items()))
+        rel_props = f" {{{rel_props_str}}}"
 
+    
+    rel_def = ""
     # direct, relation_type=None is unspecified, relation_type
     if relation_type is None:
-        stmt = stmt.format("")
+        rel_def = ""
     # all("*" wildcard) relation_type
     elif relation_type == "*":
-        stmt = stmt.format("[*]")
+        rel_def = "[*]"
     else:
         # explicit relation_type
-        stmt = stmt.format(
-            "[{0}:`{1}`{2}]".format(ident if ident else "", relation_type, rel_props)
-        )
+        rel_def = f"[{ident if ident else ''}:`{relation_type}`{rel_props}]"
 
-    return "({0}){1}({2})".format(lhs, stmt, rhs)
+    stmt = ""
+    if direction == OUTGOING:
+        stmt = f"-{rel_def}->"
+    elif direction == INCOMING:
+        stmt = f"<-{rel_def}-"
+    else:
+        stmt = f"-{rel_def}-"
+        
+    return f"({lhs}){stmt}({rhs})"
 
 
 def _rel_merge_helper(
     lhs,
     rhs,
     ident="neomodelident",
     relation_type=None,
@@ -115,44 +109,30 @@
     else:
         stmt = "-{0}-"
 
     rel_props = ""
     rel_none_props = ""
 
     if relation_properties:
-        rel_props = " {{{0}}}".format(
-            ", ".join(
-                [
-                    "{0}: {1}".format(key, value)
-                    for key, value in relation_properties.items()
-                    if value is not None
-                ]
-            )
-        )
+        rel_props_str = ", ".join((f"{key}: {value}" for key, value in relation_properties.items() if value is not None))
+        rel_props = f" {{{rel_props_str}}}"
         if None in relation_properties.values():
-            rel_none_props = " ON CREATE SET {0} ON MATCH SET {0}".format(
-                ", ".join(
-                    [
-                        "{0}.{1}={2}".format(ident, key, "${!s}".format(key))
-                        for key, value in relation_properties.items()
-                        if value is None
-                    ]
-                )
-            )
+            rel_prop_val_str = ", ".join((f"{ident}.{key}=${key!s}" for key, value in relation_properties.items() if value is None))
+            rel_none_props = f" ON CREATE SET {rel_prop_val_str} ON MATCH SET {rel_prop_val_str}"
     # direct, relation_type=None is unspecified, relation_type
     if relation_type is None:
         stmt = stmt.format("")
     # all("*" wildcard) relation_type
     elif relation_type == "*":
         stmt = stmt.format("[*]")
     else:
         # explicit relation_type
-        stmt = stmt.format("[{0}:`{1}`{2}]".format(ident, relation_type, rel_props))
+        stmt = stmt.format(f"[{ident}:`{relation_type}`{rel_props}]")
 
-    return "({0}){1}({2}){3}".format(lhs, stmt, rhs, rel_none_props)
+    return f"({lhs}){stmt}({rhs}){rel_none_props}"
 
 
 # special operators
 _SPECIAL_OPERATOR_IN = "IN"
 _SPECIAL_OPERATOR_INSENSITIVE = "(?i)"
 _SPECIAL_OPERATOR_ISNULL = "IS NULL"
 _SPECIAL_OPERATOR_ISNOTNULL = "IS NOT NULL"
@@ -204,15 +184,15 @@
     relationship definition on a NodeSet instance
     """
     rels = cls.defined_properties(rels=True, aliases=False, properties=False)
 
     for key in rels.keys():
         if hasattr(node_set, key):
             raise ValueError(
-                "Can't install traversal '{0}' exists on NodeSet".format(key)
+                f"Cannot install traversal '{key}' exists on NodeSet"
             )
 
         rel = getattr(cls, key)
         rel._lookup_node_class()
 
         traversal = Traversal(source=node_set, name=key, definition=rel.definition)
         setattr(node_set, key, traversal)
@@ -231,41 +211,39 @@
             prop, operator = key.rsplit("__")
             operator = OPERATOR_TABLE[operator]
         else:
             prop = key
             operator = "="
 
         if prop not in cls.defined_properties(rels=False):
-            raise ValueError("No such property {0} on {1}".format(prop, cls.__name__))
+            raise ValueError(f"No such property {prop} on {cls.__name__}")
 
         property_obj = getattr(cls, prop)
         if isinstance(property_obj, AliasProperty):
             prop = property_obj.aliased_to()
             deflated_value = getattr(cls, prop).deflate(value)
         else:
             # handle special operators
             if operator == _SPECIAL_OPERATOR_IN:
                 if not isinstance(value, tuple) and not isinstance(value, list):
                     raise ValueError(
-                        "Value must be a tuple or list for IN operation {0}={1}".format(
-                            key, value
-                        )
+                        f"Value must be a tuple or list for IN operation {key}={value}"
                     )
                 deflated_value = [property_obj.deflate(v) for v in value]
             elif operator == _SPECIAL_OPERATOR_ISNULL:
                 if not isinstance(value, bool):
                     raise ValueError(
-                        "Value must be a bool for isnull operation on {0}".format(key)
+                        f"Value must be a bool for isnull operation on {key}"
                     )
                 operator = "IS NULL" if value else "IS NOT NULL"
                 deflated_value = None
             elif operator in _REGEX_OPERATOR_TABLE.values():
                 deflated_value = property_obj.deflate(value)
                 if not isinstance(deflated_value, basestring):
-                    raise ValueError("Must be a string value for {0}".format(key))
+                    raise ValueError(f"Must be a string value for {key}")
                 if operator in _STRING_REGEX_OPERATOR_TABLE.values():
                     deflated_value = re.escape(deflated_value)
                 deflated_value = operator.format(deflated_value)
                 operator = _SPECIAL_OPERATOR_REGEX
             else:
                 deflated_value = property_obj.deflate(value)
 
@@ -284,15 +262,15 @@
     rel_definitions = cls.defined_properties(properties=False, rels=True, aliases=False)
 
     match, dont_match = {}, {}
 
     for key, value in kwargs.items():
         if key not in rel_definitions:
             raise ValueError(
-                "No such relation {0} defined on a {1}".format(key, cls.__name__)
+                f"No such relation {key} defined on a {cls.__name__}"
             )
 
         rhs_ident = key
 
         rel_definitions[key]._lookup_node_class()
 
         if value is True:
@@ -356,19 +334,19 @@
 
     def create_ident(self):
         self._ident_count += 1
         return "r" + str(self._ident_count)
 
     def build_order_by(self, ident, source):
         if "?" in source._order_by:
-            self._ast["with"] = "{0}, rand() as r".format(ident)
+            self._ast["with"] = f"{ident}, rand() as r"
             self._ast["order_by"] = "r"
         else:
             self._ast["order_by"] = [
-                "{0}.{1}".format(ident, p) for p in source._order_by
+                f"{ident}.{p}" for p in source._order_by
             ]
 
     def build_traversal(self, traversal):
         """
         traverse a relationship from a node to a set of nodes
         """
         # build source
@@ -395,31 +373,29 @@
         return traversal.name
 
     def build_node(self, node):
         ident = node.__class__.__name__.lower()
         place_holder = self._register_place_holder(ident)
 
         # Hack to emulate START to lookup a node by id
-        _node_lookup = "MATCH ({0}) WHERE id({0})=${1} WITH {0}".format(
-            ident, place_holder
-        )
+        _node_lookup = f"MATCH ({ident}) WHERE id({ident})=${place_holder} WITH {ident}"
         self._ast["lookup"] = _node_lookup
 
         self._query_params[place_holder] = node.id
 
         self._ast["return"] = ident
         self._ast["result_class"] = node.__class__
         return ident
 
     def build_label(self, ident, cls):
         """
         match nodes by a label
         """
         ident_w_label = ident + ":" + cls.__label__
-        self._ast["match"].append("({0})".format(ident_w_label))
+        self._ast["match"].append(f"({ident_w_label})")
         self._ast["return"] = ident
         self._ast["result_class"] = cls
         return ident
 
     def build_additional_match(self, ident, node_set):
         """
         handle additional matches supplied by 'has()' calls
@@ -460,25 +436,23 @@
             else:
                 kwargs = {child[0]: child[1]}
                 filters = process_filter_args(source_class, kwargs)
                 for prop, op_and_val in filters.items():
                     operator, val = op_and_val
                     if operator in _UNARY_OPERATORS:
                         # unary operators do not have a parameter
-                        statement = "{0}.{1} {2}".format(ident, prop, operator)
+                        statement = f"{ident}.{prop} {operator}"
                     else:
                         place_holder = self._register_place_holder(ident + "_" + prop)
-                        statement = "{0}.{1} {2} ${3}".format(
-                            ident, prop, operator, place_holder
-                        )
+                        statement = f"{ident}.{prop} {operator} ${place_holder}"
                         self._query_params[place_holder] = val
                     target.append(statement)
-        ret = " {0} ".format(q.connector).join(target)
+        ret = f" {q.connector} ".join(target)
         if q.negated:
-            ret = "NOT ({0})".format(ret)
+            ret = f"NOT ({ret})"
         return ret
 
     def build_where_stmt(self, ident, filters, q_filters=None, source_class=None):
         """
         construct a where statement from some filters
         """
         if q_filters is not None:
@@ -495,39 +469,31 @@
                     negate = True
                     row = row["__NOT__"]
 
                 for prop, operator_and_val in row.items():
                     operator, val = operator_and_val
                     if operator in _UNARY_OPERATORS:
                         # unary operators do not have a parameter
-                        statement = "{0} {1}.{2} {3}".format(
-                            "NOT" if negate else "", ident, prop, operator
-                        )
+                        statement = f"{'NOT' if negate else ''} {ident}.{prop} {operator}"
                     else:
                         place_holder = self._register_place_holder(ident + "_" + prop)
-                        statement = "{0} {1}.{2} {3} ${4}".format(
-                            "NOT" if negate else "",
-                            ident,
-                            prop,
-                            operator,
-                            place_holder,
-                        )
+                        statement = f"{'NOT' if negate else ''} {ident}.{prop} {operator} ${place_holder}"
                         self._query_params[place_holder] = val
                     stmts.append(statement)
 
             self._ast["where"].append(" AND ".join(stmts))
 
     def build_query(self):
         query = ""
 
         if "lookup" in self._ast:
             query += self._ast["lookup"]
 
         query += " MATCH "
-        query += ", ".join(["({0})".format(i) for i in self._ast["match"]])
+        query += ", ".join([f"({i})" for i in self._ast["match"]])
 
         if "where" in self._ast and self._ast["where"]:
             query += " WHERE "
             query += " AND ".join(self._ast["where"])
 
         if "with" in self._ast and self._ast["with"]:
             query += " WITH "
@@ -536,41 +502,41 @@
         query += " RETURN " + self._ast["return"]
 
         if "order_by" in self._ast and self._ast["order_by"]:
             query += " ORDER BY "
             query += ", ".join(self._ast["order_by"])
 
         if "skip" in self._ast:
-            query += " SKIP {0:d}".format(self._ast["skip"])
+            query += f" SKIP {self._ast['skip']:d}"
 
         if "limit" in self._ast:
-            query += " LIMIT {0:d}".format(self._ast["limit"])
+            query += f" LIMIT {self._ast['limit']:d}"
 
         return query
 
     def _count(self):
-        self._ast["return"] = "count({0})".format(self._ast["return"])
+        self._ast["return"] = f"count({self._ast['return']})"
         # drop order_by, results in an invalid query
         self._ast.pop("order_by", None)
         query = self.build_query()
         results, _ = db.cypher_query(query, self._query_params)
         return int(results[0][0])
 
     def _contains(self, node_id):
         # inject id = into ast
         ident = self._ast["return"]
         place_holder = self._register_place_holder(ident + "_contains")
-        self._ast["where"].append("id({0}) = ${1}".format(ident, place_holder))
+        self._ast["where"].append(f"id({ident}) = ${place_holder}")
         self._query_params[place_holder] = node_id
         return self._count() >= 1
 
     def _execute(self, lazy=False):
         if lazy:
             # inject id = into ast
-            self._ast["return"] = "id({})".format(self._ast["return"])
+            self._ast["return"] = f"id({self._ast['return']})"
         query = self.build_query()
         results, _ = db.cypher_query(query, self._query_params, resolve_objects=True)
         # The following is not as elegant as it could be but had to be copied from the
         # version prior to cypher_query with the resolve_objects capability.
         # It seems that certain calls are only supposed to be focusing to the first
         # result item returned (?)
         if results:
@@ -796,17 +762,15 @@
                     prop = prop[1:]
                     desc = True
                 else:
                     desc = False
 
                 if prop not in self.source_class.defined_properties(rels=False):
                     raise ValueError(
-                        "No such property {0} on {1}".format(
-                            prop, self.source_class.__name__
-                        )
+                        f"No such property {prop} on {self.source_class.__name__}"
                     )
 
                 property_obj = getattr(self.source_class, prop)
                 if isinstance(property_obj, AliasProperty):
                     prop = property_obj.aliased_to()
 
                 self._order_by.append(prop + (" DESC" if desc else ""))
@@ -841,27 +805,25 @@
         elif inspect.isclass(source) and issubclass(source, StructuredNode):
             self.source_class = source
         elif isinstance(source, StructuredNode):
             self.source_class = source.__class__
         elif isinstance(source, NodeSet):
             self.source_class = source.source_class
         else:
-            raise TypeError("Bad source for traversal: " "{0}".format(type(source)))
+            raise TypeError(f"Bad source for traversal: {type(source)}")
 
         invalid_keys = set(definition) - {
             "direction",
             "model",
             "node_class",
             "relation_type",
         }
         if invalid_keys:
             raise ValueError(
-                "Unallowed keys in Traversal definition: {invalid_keys}".format(
-                    invalid_keys=invalid_keys
-                )
+                f"Unallowed keys in Traversal definition: {invalid_keys}"
             )
 
         self.definition = definition
         self.target_class = definition["node_class"]
         self.name = name
         self.filters = []
```

### Comparing `neomodel-5.0.0/neomodel/match_q.py` & `neomodel-5.0.1/neomodel/match_q.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,18 @@
         setting up to do).
         """
         obj = QBase(children, connector, negated)
         obj.__class__ = cls
         return obj
 
     def __str__(self):
-        template = "(NOT ({0}: {1}))" if self.negated else "({0}: {1})"
-        return template.format(self.connector, ", ".join(str(c) for c in self.children))
+        return f"(NOT ({self.connector}: {', '.join(str(c) for c in self.children)}))" if self.negated else f"({self.connector}: {', '.join(str(c) for c in self.children)})"
 
     def __repr__(self):
-        return "<{0}: {1}>".format(self.__class__.__name__, self)
+        return f"<{self.__class__.__name__}: {self}>"
 
     def __deepcopy__(self, memodict):
         obj = QBase(connector=self.connector, negated=self.negated)
         obj.__class__ = self.__class__
         obj.children = copy.deepcopy(self.children, memodict)
         return obj
```

### Comparing `neomodel-5.0.0/neomodel/properties.py` & `neomodel-5.0.1/neomodel/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
                     setattr(self, name, None)
             else:
                 setattr(self, name, kwargs[name])
 
             if getattr(property, "choices", None):
                 setattr(
                     self,
-                    "get_{0}_display".format(name),
+                    f"get_{name}_display",
                     types.MethodType(display_for(name), self),
                 )
 
             if name in kwargs:
                 del kwargs[name]
 
         aliases = getattr(self, "__all_aliases__", None)
@@ -262,18 +262,15 @@
             raise ValueError("expression is undefined")
         self.expression = actual_re
 
     def normalize(self, value):
         normal = Unicode(value)
         if not re.match(self.expression, normal):
             raise ValueError(
-                "{0!r} does not matches {1!r}".format(
-                    value,
-                    self.expression,
-                )
+                f"{value!r} does not match {self.expression!r}"
             )
         return normal
 
 
 class EmailProperty(RegexProperty):
     """
     Store email addresses
@@ -321,21 +318,17 @@
     def normalize(self, value):
         # One thing to note here is that the following two checks can remain uncoupled
         # as long as it is guaranteed (by the constructor) that `choices` and `max_length`
         # are mutually exclusive. If that check in the constructor ever has to be removed,
         # these two validation checks here will have to be coupled so that having set
         # `choices` overrides having set the `max_length`.
         if self.choices is not None and value not in self.choices:
-            raise ValueError("Invalid choice: {}".format(value))
+            raise ValueError(f"Invalid choice: {value}")
         if self.max_length is not None and len(value) > self.max_length:
-            raise ValueError(
-                "Property max length exceeded. Expected {}, got {} == len('{}')".format(
-                    self.max_length, len(value), value
-                )
-            )
+            raise ValueError(f"Property max length exceeded. Expected {self.max_length}, got {len(value)} == len('{value}')")
         return Unicode(value)
 
     def default_value(self):
         return self.normalize(super().default_value())
 
 
 class IntegerProperty(Property):
@@ -382,17 +375,15 @@
                 "default",
                 "index",
                 "unique_index",
                 "required",
             ]:
                 if getattr(base_property, ilegal_attr, None):
                     raise ValueError(
-                        'ArrayProperty base_property cannot have "{0}" set'.format(
-                            ilegal_attr
-                        )
+                        f'ArrayProperty base_property cannot have "{ilegal_attr}" set'
                     )
 
         self.base_property = base_property
 
         super().__init__(**kwargs)
 
     @validator
@@ -466,15 +457,15 @@
             if "T" in value:
                 value = value[: value.find("T")]
         return datetime.strptime(Unicode(value), "%Y-%m-%d").date()
 
     @validator
     def deflate(self, value):
         if not isinstance(value, date):
-            msg = "datetime.date object expected, got {0}".format(repr(value))
+            msg = f"datetime.date object expected, got {repr(value)}"
             raise ValueError(msg)
         return value.isoformat()
 
 
 class DateTimeFormatProperty(Property):
     """
     Store a datetime by custome format
@@ -500,15 +491,15 @@
     @validator
     def inflate(self, value):
         return datetime.strptime(Unicode(value), self.format)
 
     @validator
     def deflate(self, value):
         if not isinstance(value, datetime):
-            raise ValueError("datetime object expected, got {0}.".format(type(value)))
+            raise ValueError(f"datetime object expected, got {type(value)}.")
         return datetime.strftime(value, self.format)
 
 
 class DateTimeProperty(Property):
     """A property representing a :class:`datetime.datetime` object as
     unix epoch.
 
@@ -528,35 +519,28 @@
         super().__init__(**kwargs)
 
     @validator
     def inflate(self, value):
         try:
             epoch = float(value)
         except ValueError as exc:
-            raise ValueError(
-                "Float or integer expected, got {0} can't inflate to "
-                "datetime.".format(type(value))
-            ) from exc
+            raise ValueError(f"Float or integer expected, got {type(value)} cannot inflate to datetime.") from exc
         except TypeError as exc:
-            raise TypeError(
-                "Float or integer expected. Can't inflate {0} to datetime.".format(
-                    type(value)
-                )
-            ) from exc
+            raise TypeError(f"Float or integer expected. Can't inflate {type(value)} to datetime.") from exc
         return datetime.utcfromtimestamp(epoch).replace(tzinfo=pytz.utc)
 
     @validator
     def deflate(self, value):
         if not isinstance(value, datetime):
-            raise ValueError("datetime object expected, got {0}.".format(type(value)))
+            raise ValueError(f"datetime object expected, got {type(value)}.")
         if value.tzinfo:
             value = value.astimezone(pytz.utc)
             epoch_date = datetime(1970, 1, 1, tzinfo=pytz.utc)
         elif config.FORCE_TIMEZONE:
-            raise ValueError("Error deflating {0}: No timezone provided.".format(value))
+            raise ValueError(f"Error deflating {value}: No timezone provided.")
         else:
             # No timezone specified on datetime object.. assuming UTC
             epoch_date = datetime(1970, 1, 1)
         return float((value - epoch_date).total_seconds())
 
 
 class JSONProperty(Property):
@@ -617,15 +601,15 @@
     A unique identifier, a randomly generated uid (uuid4) with a unique index
     """
 
     def __init__(self, **kwargs):
         for item in ["required", "unique_index", "index", "default"]:
             if item in kwargs:
                 raise ValueError(
-                    "{0} argument ignored by {1}".format(item, self.__class__.__name__)
+                    f"{item} argument ignored by {self.__class__.__name__}"
                 )
 
         kwargs["unique_index"] = True
         kwargs["default"] = lambda: uuid.uuid4().hex
         super().__init__(**kwargs)
 
     @validator
```

### Comparing `neomodel-5.0.0/neomodel/relationship_manager.py` & `neomodel-5.0.1/neomodel/relationship_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     OUTGOING,
     NodeSet,
     Traversal,
     _rel_helper,
     _rel_merge_helper,
 )
 from .relationship import StructuredRel
-from .util import _get_node_properties, deprecated, enumerate_traceback
+from .util import _get_node_properties, enumerate_traceback
 
 # basestring python 3.x fallback
 try:
     basestring
 except NameError:
     basestring = str
 
@@ -60,21 +60,15 @@
     def __str__(self):
         direction = "either"
         if self.definition["direction"] == OUTGOING:
             direction = "a outgoing"
         elif self.definition["direction"] == INCOMING:
             direction = "a incoming"
 
-        return "{0} in {1} direction of type {2} on node ({3}) of class '{4}'".format(
-            self.description,
-            direction,
-            self.definition["relation_type"],
-            self.source.id,
-            self.source_class.__name__,
-        )
+        return f"{self.description} in {direction} direction of type {self.definition['relation_type']} on node ({self.source.id}) of class '{self.source_class.__name__}'"
 
     def _check_node(self, obj):
         """check for valid node i.e correct class and is saved"""
         if not issubclass(type(obj), self.definition["node_class"]):
             raise ValueError(
                 "Expected node of class " + self.definition["node_class"].__name__
             )
@@ -302,24 +296,14 @@
         Retrieve a related node with the matching node properties or return None.
 
         :param kwargs: same syntax as `NodeSet.filter()`
         :return: node
         """
         return NodeSet(self._new_traversal()).get_or_none(**kwargs)
 
-    @deprecated("search() is now deprecated please use filter() and exclude()")
-    def search(self, **kwargs):
-        """
-        Retrieve related nodes matching the provided properties.
-
-        :param kwargs: same syntax as `NodeSet.filter()`
-        :return: NodeSet
-        """
-        return self.filter(**kwargs).all()
-
     def filter(self, *args, **kwargs):
         """
         Retrieve related nodes matching the provided properties.
 
         :param args: a Q object
         :param kwargs: same syntax as `NodeSet.filter()`
         :return: NodeSet
@@ -478,15 +462,15 @@
                 # __name__ is the namespace of the parent module for __init__.py files,
                 # and the namespace of the current module for other .py files,
                 # therefore there's a need to define the namespace differently for
                 # these two cases in order for . in relative imports to work correctly
                 # (i.e. to mean the same thing for both cases).
                 # For example in the comments below, namespace == myapp, always
                 if not hasattr(self, "module_file"):
-                    raise ImportError("Couldn't lookup '{0}'".format(name))
+                    raise ImportError(f"Couldn't lookup '{name}'")
 
                 if "__init__.py" in self.module_file:
                     # e.g. myapp/__init__.py -[__name__]-> myapp
                     namespace = self.module_name
                 else:
                     # e.g. myapp/models.py -[__name__]-> myapp.models
                     namespace = self.module_name.rpartition(".")[0]
```

### Comparing `neomodel-5.0.0/neomodel/util.py` & `neomodel-5.0.1/neomodel/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     def __init__(self):
         self.__dict__["_NODE_CLASS_REGISTRY"] = self._NODE_CLASS_REGISTRY
 
     def __str__(self):
         ncr_items = list(
             map(
-                lambda x: "{} --> {}".format(",".join(x[0]), x[1]),
+                lambda x: f"{','.join(x[0])} --> {x[1]}",
                 self._NODE_CLASS_REGISTRY.items(),
             )
         )
         return "\n".join(ncr_items)
 
 
 class Database(local, NodeClassRegistry):
@@ -113,16 +113,15 @@
         if parsed_url.netloc.find("@") > -1 and parsed_url.scheme in valid_schemas:
             credentials, hostname = parsed_url.netloc.rsplit("@", 1)
             username, password = credentials.split(":")
             password = unquote(password)
             database_name = parsed_url.path.strip("/")
         else:
             raise ValueError(
-                "Expecting url format: bolt://user:password@localhost:7687"
-                " got {0}".format(url)
+                f"Expecting url format: bolt://user:password@localhost:7687 got {url}"
             )
 
         options = {
             "auth": basic_auth(username, password),
             "connection_acquisition_timeout": config.CONNECTION_ACQUISITION_TIMEOUT,
             "connection_timeout": config.CONNECTION_TIMEOUT,
             "keep_alive": config.KEEP_ALIVE,
@@ -339,15 +338,15 @@
             os.environ.get("NEOMODEL_SLOW_QUERIES", 0)
         ):
             logger.debug(
                 "query: "
                 + query
                 + "\nparams: "
                 + repr(params)
-                + "\ntook: {:.2g}s\n".format(tte)
+                + f"\ntook: {tte:.2g}s\n"
             )
 
         return results, meta
 
 
 class TransactionProxy:
     bookmarks = None
```

### Comparing `neomodel-5.0.0/neomodel.egg-info/PKG-INFO` & `neomodel-5.0.1/neomodel.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neomodel
-Version: 5.0.0
+Version: 5.0.1
 Summary: An object mapper for the neo4j graph database.
 Author-email: Robin Edwards <robin.ge@gmail.com>
 Maintainer: Cristina Escalante
 Maintainer-email: Athanasios Anastasiou <athanastasiou@gmail.com>, Marius Conjeaud <marius.conjeaud@outlook.com>
 License: MIT
 Project-URL: documentation, https://neomodel.readthedocs.io/en/latest/
 Project-URL: repository, http://github.com/neo4j-contrib/neomodel
@@ -117,14 +117,20 @@
 
 Ensure ``dbms.security.auth_enabled=true`` in your database configuration file.
 Setup a virtual environment, install neomodel for development and run the test suite: ::
 
     $ pip install -e '.[dev]'
     $ pytest
 
+The tests in "test_connection.py" will fail locally if you don't specify the following environment variables::
+
+    $ export AURA_TEST_DB_USER=username
+    $ export AURA_TEST_DB_PASSWORD=password
+    $ export AURA_TEST_DB_HOSTNAME=url
+
 If you are running a neo4j database for the first time the test suite will set the password to 'test'.
 If the database is already populated, the test suite will abort with an error message and ask you to re-run it with the
 ``--resetdb`` switch. This is a safeguard to ensure that the test suite does not accidentally wipe out a database if you happen 
 to not have restarted your Neo4j server to point to a (usually named) ``debug.db`` database.
 
 If you have ``docker-compose`` installed, you can run the test suite against all supported Python
 interpreters and neo4j versions: ::
```

### Comparing `neomodel-5.0.0/neomodel.egg-info/SOURCES.txt` & `neomodel-5.0.1/neomodel.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 scripts/neomodel_install_labels.py
 scripts/neomodel_remove_labels.py
 test/__init__.py
 test/conftest.py
 test/test_alias.py
 test/test_batch.py
 test/test_cardinality.py
+test/test_connection.py
 test/test_cypher.py
 test/test_exceptions.py
 test/test_hooks.py
 test/test_indexing.py
 test/test_issue112.py
 test/test_issue283.py
 test/test_issue600.py
```

### Comparing `neomodel-5.0.0/pyproject.toml` & `neomodel-5.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 ]
 dependencies = [
     "neo4j-driver==4.4.10",
     "pytz>=2021.1",
     "neobolt==1.7.17",
     "six==1.16.0",
 ]
-version='5.0.0'
+version='5.0.1'
 
 [project.urls]
 documentation = "https://neomodel.readthedocs.io/en/latest/"
 repository = "http://github.com/neo4j-contrib/neomodel"
 changelog = "https://github.com/neo4j-contrib/neomodel/releases"
 
 [project.optional-dependencies]
@@ -52,15 +52,15 @@
     "pre-commit",
     "black",
     "isort",
     "Shapely>=1.8.1,<1.9"
 ]
 
 [tool.pytest.ini_options]
-addopts = "--resetdb --cov=neomodel --cov-report=html:coverage_report"
+addopts = "--resetdb"
 testpaths = "test"
 
 [tool.isort]
 profile = 'black'
 src_paths = ['neomodel']
 
 [tool.pylint.'MESSAGES CONTROL']
```

### Comparing `neomodel-5.0.0/scripts/neomodel_install_labels.py` & `neomodel-5.0.1/scripts/neomodel_install_labels.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/scripts/neomodel_remove_labels.py` & `neomodel-5.0.1/scripts/neomodel_remove_labels.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/conftest.py` & `neomodel-5.0.1/test/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import print_function
 
 import os
-import sys
 import warnings
 
 import pytest
 from neo4j.exceptions import ClientError as CypherError
 from neobolt.exceptions import ClientError
 
 from neomodel import change_neo4j_password, clear_neo4j_database, config, db
@@ -22,14 +21,35 @@
         "--resetdb",
         action="store_true",
         help="Ensures that the database is clear prior to running tests for neomodel",
         default=False,
     )
 
 
+def pytest_collection_modifyitems(items):
+    connect_to_aura_items = []
+    normal_items = []
+
+    # Separate all tests into two groups: those with "connect_to_aura" in their name, and all others
+    for item in items:
+        if "connect_to_aura" in item.name:
+            connect_to_aura_items.append(item)
+        else:
+            normal_items.append(item)
+
+    # Add all normal tests back to the front of the list
+    new_order = normal_items
+
+    # Add all connect_to_aura tests to the end of the list
+    new_order.extend(connect_to_aura_items)
+
+    # Replace the original items list with the new order
+    items[:] = new_order
+
+
 def pytest_sessionstart(session):
     """
     Provides initial connection to the database and sets up the rest of the test suite
 
     :param session: The session object. Please see <https://docs.pytest.org/en/latest/reference.html#_pytest.hookspec.pytest_sessionstart>`_
     :type Session object: For more information please see <https://docs.pytest.org/en/latest/reference.html#session>`_
     """
```

### Comparing `neomodel-5.0.0/test/test_alias.py` & `neomodel-5.0.1/test/test_alias.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_batch.py` & `neomodel-5.0.1/test/test_batch.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_cardinality.py` & `neomodel-5.0.1/test/test_cardinality.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,14 +7,15 @@
     One,
     OneOrMore,
     RelationshipTo,
     StringProperty,
     StructuredNode,
     ZeroOrMore,
     ZeroOrOne,
+    db,
 )
 
 
 class HairDryer(StructuredNode):
     version = IntegerProperty()
 
 
@@ -73,36 +74,65 @@
     j = ScrewDriver(version=2).save()
     with raises(AttemptedCardinalityViolation):
         m.driver.connect(j)
 
     m.driver.reconnect(h, j)
     assert m.driver.single().version == 2
 
+    # Forcing creation of a second ToothBrush to go around
+    # AttemptedCardinalityViolation
+    db.cypher_query(
+        """
+        MATCH (m:Monkey WHERE m.name="bob")
+        CREATE (s:ScrewDriver {version:3})
+        WITH m, s
+        CREATE (m)-[:HAS_SCREWDRIVER]->(s)
+    """
+    )
+    with raises(
+        CardinalityViolation, match=r"CardinalityViolation: Expected: .*, got: 2."
+    ):
+        m.driver.all()
+
 
 def test_cardinality_one_or_more():
     m = Monkey(name="jerry").save()
 
     with raises(CardinalityViolation):
         m.car.all()
 
     with raises(CardinalityViolation):
         m.car.single()
 
     c = Car(version=2).save()
     m.car.connect(c)
     assert m.car.single().version == 2
 
+    cars = m.car.all()
+    assert len(cars) == 1
+
     with raises(AttemptedCardinalityViolation):
         m.car.disconnect(c)
 
+    d = Car(version=3).save()
+    m.car.connect(d)
+    cars = m.car.all()
+    assert len(cars) == 2
+
+    m.car.disconnect(d)
+    cars = m.car.all()
+    assert len(cars) == 1
+
 
 def test_cardinality_one():
     m = Monkey(name="jerry").save()
 
-    with raises(CardinalityViolation):
+    with raises(
+        CardinalityViolation, match=r"CardinalityViolation: Expected: .*, got: none."
+    ):
         m.toothbrush.all()
 
     with raises(CardinalityViolation):
         m.toothbrush.single()
 
     b = ToothBrush(name="Jim").save()
     m.toothbrush.connect(b)
@@ -110,7 +140,29 @@
 
     x = ToothBrush(name="Jim").save
     with raises(AttemptedCardinalityViolation):
         m.toothbrush.connect(x)
 
     with raises(AttemptedCardinalityViolation):
         m.toothbrush.disconnect(b)
+
+    with raises(AttemptedCardinalityViolation):
+        m.toothbrush.disconnect_all()
+
+    # Forcing creation of a second ToothBrush to go around
+    # AttemptedCardinalityViolation
+    db.cypher_query(
+        """
+        MATCH (m:Monkey WHERE m.name="jerry")
+        CREATE (t:ToothBrush {name:"Jim"})
+        WITH m, t
+        CREATE (m)-[:HAS_TOOTHBRUSH]->(t)
+    """
+    )
+    with raises(
+        CardinalityViolation, match=r"CardinalityViolation: Expected: .*, got: 2."
+    ):
+        m.toothbrush.all()
+
+    jp = Monkey(name="Jean-Pierre")
+    with raises(ValueError, match="Node has not been saved cannot connect!"):
+        jp.toothbrush.connect(b)
```

### Comparing `neomodel-5.0.0/test/test_contrib/test_semi_structured.py` & `neomodel-5.0.1/test/test_contrib/test_semi_structured.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_contrib/test_spatial_datatypes.py` & `neomodel-5.0.1/test/test_contrib/test_spatial_datatypes.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_contrib/test_spatial_properties.py` & `neomodel-5.0.1/test/test_contrib/test_spatial_properties.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_cypher.py` & `neomodel-5.0.1/test/test_cypher.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_exceptions.py` & `neomodel-5.0.1/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_hooks.py` & `neomodel-5.0.1/test/test_hooks.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_indexing.py` & `neomodel-5.0.1/test/test_indexing.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 
 
 def test_unique_error():
     Human(name="j1m", age=13).save()
     try:
         Human(name="j1m", age=14).save()
     except UniqueProperty as e:
-        assert True
         assert str(e).find("j1m")
         assert str(e).find("name")
         assert str(e).find("FooBarr")
     else:
         assert False, "UniqueProperty not raised."
 
 
@@ -30,18 +29,19 @@
     Human(name="98", age=98).save()
     h = Human.nodes.get(age=98)
     assert h
     assert h.name == "98"
 
 
 def test_escaped_chars():
-    Human(name="sarah:test", age=3).save()
-    r = Human.nodes.filter(name="sarah:test")
+    _name = "sarah:test"
+    Human(name=_name, age=3).save()
+    r = Human.nodes.filter(name=_name)
     assert r
-    assert r[0].name == "sarah:test"
+    assert r[0].name == _name
 
 
 def test_does_not_exist():
     with raises(Human.DoesNotExist):
         Human.nodes.get(name="XXXX")
```

### Comparing `neomodel-5.0.0/test/test_issue283.py` & `neomodel-5.0.1/test/test_issue283.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,15 +261,18 @@
 
     # Simulate the condition where the definition of class RandomPerson is not
     # known yet.
     del neomodel.db._NODE_CLASS_REGISTRY[frozenset(["RandomPerson", "BasePerson"])]
 
     # Now try to instantiate a RandomPerson
     A = TechnicalPerson.get_or_create({"name": "Grumpy", "expertise": "Grumpiness"})[0]
-    with pytest.raises(neomodel.exceptions.NodeClassNotDefined):
+    with pytest.raises(
+        neomodel.exceptions.NodeClassNotDefined,
+        match=r"Node with labels .* does not resolve to any of the known objects.*",
+    ):
         for some_friend in A.friends_with:
             print(some_friend.name)
 
     A.delete()
     B.delete()
 
 
@@ -320,15 +323,18 @@
     def redefine_class_locally():
         # Since this test has already set up a class hierarchy in its global scope, we will try to redefine
         # SomePerson here.
         # The internal structure of the SomePerson entity does not matter at all here.
         class SomePerson(BaseOtherPerson):
             uid = neomodel.UniqueIdProperty()
 
-    with pytest.raises(neomodel.exceptions.NodeClassAlreadyDefined):
+    with pytest.raises(
+        neomodel.exceptions.NodeClassAlreadyDefined,
+        match=r"Class .* with labels .* already defined:.*",
+    ):
         redefine_class_locally()
 
 
 def test_relationship_object_resolution():
     """
     A query returning a "Relationship" object can now instantiate it to a data model class
     """
@@ -396,15 +402,18 @@
     Attempting to re-define an existing relationship with a completely unrelated class.
     :return:
     """
 
     class NewRelationship(neomodel.StructuredRel):
         profile_match_factor = neomodel.FloatProperty()
 
-    with pytest.raises(neomodel.RelationshipClassRedefined):
+    with pytest.raises(
+        neomodel.RelationshipClassRedefined,
+        match=r"Relationship of type .* redefined as .*",
+    ):
 
         class NewSomePerson(SomePerson):
             friends_with = neomodel.RelationshipTo(
                 "BaseOtherPerson", "FRIENDS_WITH", model=NewRelationship
             )
 
 
@@ -413,13 +422,16 @@
     Attempting to resolve an inexistent relationship should raise an exception
     :return:
     """
 
     # Forget about the FRIENDS_WITH Relationship.
     del neomodel.db._NODE_CLASS_REGISTRY[frozenset(["FRIENDS_WITH"])]
 
-    with pytest.raises(neomodel.RelationshipClassNotDefined):
+    with pytest.raises(
+        neomodel.RelationshipClassNotDefined,
+        match=r"Relationship of type .* does not resolve to any of the known objects.*",
+    ):
         query_data = neomodel.db.cypher_query(
             "MATCH (:ExtendedSomePerson)-[r:FRIENDS_WITH]->(:ExtendedSomePerson) "
             "RETURN DISTINCT r",
             resolve_objects=True,
         )
```

### Comparing `neomodel-5.0.0/test/test_issue600.py` & `neomodel-5.0.1/test/test_issue600.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_label_drop.py` & `neomodel-5.0.1/test/test_label_drop.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_label_install.py` & `neomodel-5.0.1/test/test_label_install.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,18 @@
     install_labels,
 )
 from neomodel.core import db, drop_constraints
 
 config.AUTO_INSTALL_LABELS = False
 
 
+class NodeWithIndex(StructuredNode):
+    name = StringProperty(index=True)
+
+
 class NodeWithConstraint(StructuredNode):
     name = StringProperty(unique_index=True)
 
 
 class NodeWithRelationship(StructuredNode):
     ...
 
@@ -72,18 +76,36 @@
     assert "constraint_unique_NodeWithConstraint_name" in constraint_names
     assert "constraint_unique_SomeNotUniqueNode_id" in constraint_names
 
     # remove constraint for above test
     _drop_constraints_for_label_and_property("NoConstraintsSetup", "name")
 
 
-def test_install_label_twice():
+def test_install_label_twice(capsys):
+    expected_std_out = (
+        "{code: Neo.ClientError.Schema.EquivalentSchemaRuleAlreadyExists}"
+    )
     install_labels(AbstractNode)
     install_labels(AbstractNode)
 
+    install_labels(NodeWithIndex)
+    install_labels(NodeWithIndex, quiet=False)
+    captured = capsys.readouterr()
+    assert expected_std_out in captured.out
+
+    install_labels(NodeWithConstraint)
+    install_labels(NodeWithConstraint, quiet=False)
+    captured = capsys.readouterr()
+    assert expected_std_out in captured.out
+
+    install_labels(OtherNodeWithRelationship)
+    install_labels(OtherNodeWithRelationship, quiet=False)
+    captured = capsys.readouterr()
+    assert expected_std_out in captured.out
+
 
 def test_install_labels_db_property():
     stdout = StringIO()
     drop_constraints()
     install_labels(SomeNotUniqueNode, quiet=False, stdout=stdout)
     assert "id" in stdout.getvalue()
     # make sure that the id_ constraint doesn't exist
```

### Comparing `neomodel-5.0.0/test/test_match_api.py` & `neomodel-5.0.1/test/test_match_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -313,14 +313,15 @@
     assert len(filter_empty_filter.all()) == 1, "unexpected number of results"
     assert (
         c1 in filter_empty_filter.all()
     ), "doesnt contain c1 in ``filter_empty_filter``"
 
 
 def test_q_filters():
+    # Test where no children and self.connector != conn ?
     for c in Coffee.nodes:
         c.delete()
 
     c1 = Coffee(name="Icelands finest", price=5, id_=1).save()
     c2 = Coffee(name="Britains finest", price=10, id_=2).save()
     c3 = Coffee(name="Japans finest", price=35, id_=3).save()
     c4 = Coffee(name="US extra-fine", price=None, id_=4).save()
@@ -368,14 +369,46 @@
     assert c6 in coffees_with_id_gte_3
 
     coffees_5_not_japans = Coffee.nodes.filter(
         Q(price__gt=5) & ~Q(name="Japans finest")
     ).all()
     assert c3 not in coffees_5_not_japans
 
+    empty_Q_condition = Coffee.nodes.filter(Q(price=5) | Q()).all()
+    assert (
+        len(empty_Q_condition) == 1
+    ), "undefined Q leading to unexpected number of results"
+    assert c1 in empty_Q_condition
+
+    combined_coffees = Coffee.nodes.filter(
+        Q(price=35), Q(name="Latte") | Q(name="Cappuccino")
+    )
+    assert len(combined_coffees) == 2
+    assert c5 in combined_coffees
+    assert c6 in combined_coffees
+    assert c3 not in combined_coffees
+
+    class QQ:
+        pass
+
+    with raises(TypeError):
+        wrong_Q = Coffee.nodes.filter(Q(price=5) | QQ()).all()
+
+
+def test_qbase():
+    test_print_out = str(Q(price=5) | Q(price=10))
+    test_repr = repr(Q(price=5) | Q(price=10))
+    assert test_print_out == "(OR: ('price', 5), ('price', 10))"
+    assert test_repr == "<Q: (OR: ('price', 5), ('price', 10))>"
+
+    assert ("price", 5) in (Q(price=5) | Q(price=10))
+
+    test_hash = set([Q(price_lt=30) | ~Q(price=5), Q(price_lt=30) | ~Q(price=5)])
+    assert len(test_hash) == 1
+
 
 def test_traversal_filter_left_hand_statement():
     nescafe = Coffee(name="Nescafe2", price=99).save()
     nescafe_gold = Coffee(name="Nescafe gold", price=11).save()
 
     tesco = Supplier(name="Sainsburys", delivery_cost=3).save()
     biedronka = Supplier(name="Biedronka", delivery_cost=5).save()
```

### Comparing `neomodel-5.0.0/test/test_models.py` & `neomodel-5.0.1/test/test_models.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_properties.py` & `neomodel-5.0.1/test/test_properties.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_relationship_models.py` & `neomodel-5.0.1/test/test_relationship_models.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_relationships.py` & `neomodel-5.0.1/test/test_relationships.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_relative_relationships.py` & `neomodel-5.0.1/test/test_relative_relationships.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/test_transactions.py` & `neomodel-5.0.1/test/test_transactions.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/test/utils.py` & `neomodel-5.0.1/test/utils.py`

 * *Files identical despite different names*

### Comparing `neomodel-5.0.0/tests-with-docker-compose.sh` & `neomodel-5.0.1/tests-with-docker-compose.sh`

 * *Files identical despite different names*

