# Comparing `tmp/m9s_nereid-6.0.8.tar.gz` & `tmp/m9s_nereid-6.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m9s_nereid-6.0.8.tar", last modified: Sun Nov 13 17:15:39 2022, max compression
+gzip compressed data, was "m9s_nereid-6.0.9.tar", last modified: Sat Nov 26 16:05:57 2022, max compression
```

## Comparing `m9s_nereid-6.0.8.tar` & `m9s_nereid-6.0.9.tar`

### file list

```diff
@@ -1,189 +1,193 @@
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.615316 m9s_nereid-6.0.8/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       72 2022-02-15 08:26:40.000000 m9s_nereid-6.0.8/.coveragerc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       12 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/.gitignore
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1794 2022-11-13 14:32:56.000000 m9s_nereid-6.0.8/.gitlab-ci.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      105 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/.gitmodules
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      283 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/.travis.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1871 2021-05-14 10:34:06.000000 m9s_nereid-6.0.8/CHANGELOG
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      832 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1577 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/LICENSE.BSD
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/LICENSE.GPL3
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      519 2022-02-15 08:26:40.000000 m9s_nereid-6.0.8/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1599 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/MIGRATION
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      644 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/Makefile
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3213 2022-11-13 17:15:39.615316 m9s_nereid-6.0.8/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1291 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1938 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      248 2022-09-14 14:34:20.000000 m9s_nereid-6.0.8/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.603316 m9s_nereid-6.0.8/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.603316 m9s_nereid-6.0.8/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       27 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3498 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/doc/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.607317 m9s_nereid-6.0.8/docs/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5564 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/Makefile
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.607317 m9s_nereid-6.0.8/docs/_static/
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     3593 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/_static/favicon.png
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    71979 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/_static/logo.png
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.607317 m9s_nereid-6.0.8/docs/_templates/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      872 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/_templates/sidebarintro.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      667 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/api.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10180 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/docs/conf.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10187 2016-10-03 10:42:45.000000 m9s_nereid-6.0.8/docs/conf.py.bak
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      727 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/contents.rst.inc
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2362 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/foreword.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1938 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4551 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/installation.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    33942 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/license.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3188 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/locale.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5096 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/make.bat
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5612 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/quickstart.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/tryton_module_api.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       40 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/tutorial.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2652 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/docs/versionmanagement.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.607317 m9s_nereid-6.0.8/m9s_nereid.egg-info/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3213 2022-11-13 17:15:39.000000 m9s_nereid-6.0.8/m9s_nereid.egg-info/PKG-INFO
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4485 2022-11-13 17:15:39.000000 m9s_nereid-6.0.8/m9s_nereid.egg-info/SOURCES.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2022-11-13 17:15:39.000000 m9s_nereid-6.0.8/m9s_nereid.egg-info/dependency_links.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       50 2022-11-13 17:15:39.000000 m9s_nereid-6.0.8/m9s_nereid.egg-info/entry_points.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-01-22 10:03:37.000000 m9s_nereid-6.0.8/m9s_nereid.egg-info/not-zip-safe
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      155 2022-11-13 17:15:39.000000 m9s_nereid-6.0.8/m9s_nereid.egg-info/requires.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       15 2022-11-13 17:15:39.000000 m9s_nereid-6.0.8/m9s_nereid.egg-info/top_level.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.607317 m9s_nereid-6.0.8/nereid/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      883 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    21603 2022-02-17 09:41:22.000000 m9s_nereid-6.0.8/nereid/application.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6146 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/nereid/caching.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1135 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid/config.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.607317 m9s_nereid-6.0.8/nereid/contrib/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/nereid/contrib/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6815 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/nereid/contrib/locale.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    11470 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid/contrib/pagination.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    11178 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/nereid/contrib/sitemap.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2157 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid/csrf.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1026 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/nereid/ctx.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      261 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/nereid/exceptions.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1464 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid/globals.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    21442 2022-04-30 13:24:27.000000 m9s_nereid-6.0.8/nereid/helpers.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      170 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/nereid/logging.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3044 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid/routing.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3589 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid/sessions.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      936 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid/signals.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14287 2022-11-10 15:09:44.000000 m9s_nereid-6.0.8/nereid/templating.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5459 2022-02-15 09:58:02.000000 m9s_nereid-6.0.8/nereid/testing.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.611317 m9s_nereid-6.0.8/nereid/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      934 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid/tests/__init__.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.611317 m9s_nereid-6.0.8/nereid/tests/templates/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       18 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/nereid/tests/templates/from-local.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        6 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/nereid/tests/templates/home.jinja
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.611317 m9s_nereid-6.0.8/nereid/tests/templates/localhost/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/nereid/tests/templates/localhost/site-specific-template.html
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.611317 m9s_nereid-6.0.8/nereid/tests/templates/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       19 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/nereid/tests/templates/tests/exists-both.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3536 2022-02-17 09:45:00.000000 m9s_nereid-6.0.8/nereid/tests/test_dispatch.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3094 2022-04-30 13:25:26.000000 m9s_nereid-6.0.8/nereid/tests/test_helpers.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5262 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/nereid/tests/test_pagination.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6280 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/nereid/tests/test_signals.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    17372 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/nereid/tests/test_templates.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4801 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid/wrappers.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.611317 m9s_nereid-6.0.8/nereid_test_module/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      840 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/nereid_test_module/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      346 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/nereid_test_module/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2071 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/nereid_test_module/model.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.611317 m9s_nereid-6.0.8/nereid_test_module/templates/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       73 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/nereid_test_module/templates/registration.jinja
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.611317 m9s_nereid-6.0.8/nereid_test_module/templates/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       24 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/nereid_test_module/templates/tests/from-module.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       15 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/nereid_test_module/templates/tests/test-changing-context.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      904 2021-02-12 20:10:26.000000 m9s_nereid-6.0.8/nereid_test_module/templates/tests/translation-test.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      157 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/nereid_test_module/tryton.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      221 2022-03-25 09:26:04.000000 m9s_nereid-6.0.8/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      448 2022-11-13 17:15:39.619316 m9s_nereid-6.0.8/setup.cfg
--rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     5376 2022-02-19 08:35:09.000000 m9s_nereid-6.0.8/setup.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.611317 m9s_nereid-6.0.8/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      468 2022-04-30 15:18:52.000000 m9s_nereid-6.0.8/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      738 2022-04-30 07:53:53.000000 m9s_nereid-6.0.8/tox.ini
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.611317 m9s_nereid-6.0.8/trytond_nereid/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/trytond_nereid/.drone.yml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/trytond_nereid/.flake8
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/trytond_nereid/.isort.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      862 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/COPYRIGHT
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/INSTALL
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/LICENSE
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/trytond_nereid/MANIFEST.in
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      910 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/README.md
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       28 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/README.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1078 2022-02-18 09:17:23.000000 m9s_nereid-6.0.8/trytond_nereid/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       16 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/trytond_nereid/babel.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4861 2022-03-25 09:26:04.000000 m9s_nereid-6.0.8/trytond_nereid/configuration.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1458 2022-02-18 09:17:23.000000 m9s_nereid-6.0.8/trytond_nereid/country.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      986 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/trytond_nereid/currency.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/trytond_nereid/dev_requirements.txt
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.611317 m9s_nereid-6.0.8/trytond_nereid/doc/
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.615316 m9s_nereid-6.0.8/trytond_nereid/doc/de/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       27 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/doc/de/index.rst
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       28 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/doc/index.rst
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.615316 m9s_nereid-6.0.8/trytond_nereid/icons/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2021-02-14 10:44:50.000000 m9s_nereid-6.0.8/trytond_nereid/icons/tryton-media.svg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      989 2021-02-14 10:44:50.000000 m9s_nereid-6.0.8/trytond_nereid/icons/tryton-web.svg
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.615316 m9s_nereid-6.0.8/trytond_nereid/locale/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12688 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/locale/ca.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14142 2022-04-12 07:18:45.000000 m9s_nereid-6.0.8/trytond_nereid/locale/de.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13174 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/locale/es.po
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1311 2022-04-08 10:03:51.000000 m9s_nereid-6.0.8/trytond_nereid/message.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      646 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/trytond_nereid/model.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12355 2022-04-29 14:20:23.000000 m9s_nereid-6.0.8/trytond_nereid/party.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3509 2022-03-29 15:04:46.000000 m9s_nereid-6.0.8/trytond_nereid/party.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/trytond_nereid/requirements.txt
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4565 2022-02-15 11:09:33.000000 m9s_nereid-6.0.8/trytond_nereid/setup.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8087 2022-02-18 09:17:23.000000 m9s_nereid-6.0.8/trytond_nereid/static_file.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3259 2022-03-25 09:26:04.000000 m9s_nereid-6.0.8/trytond_nereid/static_file.xml
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.615316 m9s_nereid-6.0.8/trytond_nereid/templates/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/trytond_nereid/templates/home.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/templates/new-password.jinja
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.615316 m9s_nereid-6.0.8/trytond_nereid/templates/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      129 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/trytond_nereid/templates/tests/exists-both.html
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       12 2020-03-16 09:24:45.000000 m9s_nereid-6.0.8/trytond_nereid/templates/tests/from-module.html
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.615316 m9s_nereid-6.0.8/trytond_nereid/tests/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      260 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/tests/__init__.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    15574 2022-03-25 09:50:34.000000 m9s_nereid-6.0.8/trytond_nereid/tests/debug_test_translation.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14973 2022-04-30 15:14:52.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_address.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    46739 2022-05-05 08:26:46.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_auth.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3649 2021-12-11 18:21:20.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_common.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5168 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_country.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5638 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_currency.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10376 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_i18n.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1846 2022-03-29 10:02:56.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_nereid.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10084 2022-04-30 15:12:48.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_routing.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4716 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_static_file.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14867 2022-03-29 15:04:46.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_translation.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4671 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_user.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2281 2021-12-16 10:44:45.000000 m9s_nereid-6.0.8/trytond_nereid/tests/test_website.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      611 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/tox.ini
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    28367 2022-02-18 09:17:23.000000 m9s_nereid-6.0.8/trytond_nereid/translation.py
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      442 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/translation.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      156 2022-11-10 15:09:44.000000 m9s_nereid-6.0.8/trytond_nereid/tryton.cfg
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    36639 2022-09-14 13:59:59.000000 m9s_nereid-6.0.8/trytond_nereid/user.py
-drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-13 17:15:39.615316 m9s_nereid-6.0.8/trytond_nereid/view/
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      366 2022-03-29 15:04:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/contact_mechanism_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/contact_mechanism_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/contact_mechanism_tree_sequence.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      765 2021-05-14 10:34:06.000000 m9s_nereid-6.0.8/trytond_nereid/view/nereid_user_form2.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      265 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/nereid_user_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      338 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/party_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      631 2021-03-16 09:13:55.000000 m9s_nereid-6.0.8/trytond_nereid/view/static_file_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/static_file_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      459 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/static_folder_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      182 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/static_folder_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      367 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/translation_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      796 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/url_map_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      278 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/url_map_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      252 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/url_rule_defaults_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      431 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/url_rule_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1007 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/website_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      322 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/website_locale_form.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      239 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/website_locale_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid-6.0.8/trytond_nereid/view/website_tree.xml
--rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    15451 2022-02-18 09:17:23.000000 m9s_nereid-6.0.8/trytond_nereid/website.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.393809 m9s_nereid-6.0.9/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       72 2022-02-15 08:26:40.000000 m9s_nereid-6.0.9/.coveragerc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       12 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/.gitignore
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1794 2022-11-13 14:32:56.000000 m9s_nereid-6.0.9/.gitlab-ci.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      104 2022-11-26 15:16:29.000000 m9s_nereid-6.0.9/.gitmodules
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/.isort.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      283 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/.travis.yml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.381809 m9s_nereid-6.0.9/.woodpecker/
+-rwxrwxr-x   0 mathiasb  (1000) mathiasb  (1000)     1367 2022-11-23 17:28:52.000000 m9s_nereid-6.0.9/.woodpecker/mail_curl.sh
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      645 2022-11-23 20:42:33.000000 m9s_nereid-6.0.9/.woodpecker/report.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1471 2022-11-24 16:32:28.000000 m9s_nereid-6.0.9/.woodpecker/test.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1871 2021-05-14 10:34:06.000000 m9s_nereid-6.0.9/CHANGELOG
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      832 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1577 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/LICENSE.BSD
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/LICENSE.GPL3
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      519 2022-02-15 08:26:40.000000 m9s_nereid-6.0.9/MANIFEST.in
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1599 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/MIGRATION
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      638 2022-11-26 15:16:47.000000 m9s_nereid-6.0.9/Makefile
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3213 2022-11-26 16:05:57.393809 m9s_nereid-6.0.9/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1291 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1687 2022-11-26 15:16:47.000000 m9s_nereid-6.0.9/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      248 2022-09-14 14:34:20.000000 m9s_nereid-6.0.9/dev_requirements.txt
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.381809 m9s_nereid-6.0.9/doc/
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.381809 m9s_nereid-6.0.9/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       27 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3498 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/doc/index.rst
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.385809 m9s_nereid-6.0.9/docs/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5564 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/docs/Makefile
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.385809 m9s_nereid-6.0.9/docs/_static/
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     3593 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/docs/_static/favicon.png
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    71979 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/docs/_static/logo.png
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.385809 m9s_nereid-6.0.9/docs/_templates/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      768 2022-11-26 15:16:47.000000 m9s_nereid-6.0.9/docs/_templates/sidebarintro.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      667 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/docs/api.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10389 2022-11-26 15:16:29.000000 m9s_nereid-6.0.9/docs/conf.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10187 2016-10-03 10:42:45.000000 m9s_nereid-6.0.9/docs/conf.py.bak
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      739 2022-11-26 15:16:47.000000 m9s_nereid-6.0.9/docs/contents.rst.inc
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2278 2022-11-26 15:16:47.000000 m9s_nereid-6.0.9/docs/foreword.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1687 2022-11-26 15:16:47.000000 m9s_nereid-6.0.9/docs/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3688 2022-11-26 15:16:47.000000 m9s_nereid-6.0.9/docs/installation.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1789 2022-11-26 15:16:47.000000 m9s_nereid-6.0.9/docs/installation_windows.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    33942 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/docs/license.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3173 2022-11-26 15:16:47.000000 m9s_nereid-6.0.9/docs/locale.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5096 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/docs/make.bat
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5908 2022-11-26 15:16:47.000000 m9s_nereid-6.0.9/docs/quickstart.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/docs/tryton_module_api.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2652 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/docs/versionmanagement.rst
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.385809 m9s_nereid-6.0.9/m9s_nereid.egg-info/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3213 2022-11-26 16:05:57.000000 m9s_nereid-6.0.9/m9s_nereid.egg-info/PKG-INFO
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4566 2022-11-26 16:05:57.000000 m9s_nereid-6.0.9/m9s_nereid.egg-info/SOURCES.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2022-11-26 16:05:57.000000 m9s_nereid-6.0.9/m9s_nereid.egg-info/dependency_links.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       50 2022-11-26 16:05:57.000000 m9s_nereid-6.0.9/m9s_nereid.egg-info/entry_points.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        1 2020-01-22 10:03:37.000000 m9s_nereid-6.0.9/m9s_nereid.egg-info/not-zip-safe
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      155 2022-11-26 16:05:57.000000 m9s_nereid-6.0.9/m9s_nereid.egg-info/requires.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       15 2022-11-26 16:05:57.000000 m9s_nereid-6.0.9/m9s_nereid.egg-info/top_level.txt
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.385809 m9s_nereid-6.0.9/nereid/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      883 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    21603 2022-02-17 09:41:22.000000 m9s_nereid-6.0.9/nereid/application.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6146 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/nereid/caching.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1135 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid/config.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.385809 m9s_nereid-6.0.9/nereid/contrib/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/nereid/contrib/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6815 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/nereid/contrib/locale.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    11470 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid/contrib/pagination.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    11178 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/nereid/contrib/sitemap.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2157 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid/csrf.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1026 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/nereid/ctx.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      261 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/nereid/exceptions.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1464 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid/globals.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    21256 2022-11-26 16:02:53.000000 m9s_nereid-6.0.9/nereid/helpers.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      170 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/nereid/logging.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3044 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid/routing.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3589 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid/sessions.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      936 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid/signals.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14287 2022-11-10 15:09:44.000000 m9s_nereid-6.0.9/nereid/templating.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5459 2022-02-15 09:58:02.000000 m9s_nereid-6.0.9/nereid/testing.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.385809 m9s_nereid-6.0.9/nereid/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      934 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid/tests/__init__.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.385809 m9s_nereid-6.0.9/nereid/tests/templates/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       18 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/nereid/tests/templates/from-local.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        6 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/nereid/tests/templates/home.jinja
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.385809 m9s_nereid-6.0.9/nereid/tests/templates/localhost/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/nereid/tests/templates/localhost/site-specific-template.html
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.385809 m9s_nereid-6.0.9/nereid/tests/templates/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       19 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/nereid/tests/templates/tests/exists-both.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3536 2022-02-17 09:45:00.000000 m9s_nereid-6.0.9/nereid/tests/test_dispatch.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3526 2022-11-26 16:00:09.000000 m9s_nereid-6.0.9/nereid/tests/test_helpers.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5262 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/nereid/tests/test_pagination.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     6280 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/nereid/tests/test_signals.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    17372 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/nereid/tests/test_templates.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4801 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid/wrappers.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/nereid_test_module/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      840 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/nereid_test_module/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      346 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/nereid_test_module/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2071 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/nereid_test_module/model.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/nereid_test_module/templates/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       73 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/nereid_test_module/templates/registration.jinja
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/nereid_test_module/templates/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       24 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/nereid_test_module/templates/tests/from-module.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       15 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/nereid_test_module/templates/tests/test-changing-context.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      904 2021-02-12 20:10:26.000000 m9s_nereid-6.0.9/nereid_test_module/templates/tests/translation-test.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      157 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/nereid_test_module/tryton.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      221 2022-03-25 09:26:04.000000 m9s_nereid-6.0.9/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      448 2022-11-26 16:05:57.393809 m9s_nereid-6.0.9/setup.cfg
+-rwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)     5376 2022-02-19 08:35:09.000000 m9s_nereid-6.0.9/setup.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      468 2022-04-30 15:18:52.000000 m9s_nereid-6.0.9/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      843 2022-11-24 16:59:38.000000 m9s_nereid-6.0.9/tox.ini
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/trytond_nereid/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1875 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/trytond_nereid/.drone.yml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       46 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/trytond_nereid/.flake8
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      173 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/trytond_nereid/.isort.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      862 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/COPYRIGHT
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      700 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/INSTALL
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    35147 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/LICENSE
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      125 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/trytond_nereid/MANIFEST.in
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      910 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/README.md
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       28 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/README.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1078 2022-02-18 09:17:23.000000 m9s_nereid-6.0.9/trytond_nereid/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       16 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/trytond_nereid/babel.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4861 2022-03-25 09:26:04.000000 m9s_nereid-6.0.9/trytond_nereid/configuration.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1458 2022-02-18 09:17:23.000000 m9s_nereid-6.0.9/trytond_nereid/country.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      986 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/trytond_nereid/currency.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       77 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/trytond_nereid/dev_requirements.txt
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/trytond_nereid/doc/
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/trytond_nereid/doc/de/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       27 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/doc/de/index.rst
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       28 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/doc/index.rst
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/trytond_nereid/icons/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      296 2021-02-14 10:44:50.000000 m9s_nereid-6.0.9/trytond_nereid/icons/tryton-media.svg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      989 2021-02-14 10:44:50.000000 m9s_nereid-6.0.9/trytond_nereid/icons/tryton-web.svg
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/trytond_nereid/locale/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12688 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/locale/ca.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14142 2022-04-12 07:18:45.000000 m9s_nereid-6.0.9/trytond_nereid/locale/de.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    13174 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/locale/es.po
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1311 2022-04-08 10:03:51.000000 m9s_nereid-6.0.9/trytond_nereid/message.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      646 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/trytond_nereid/model.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    12355 2022-04-29 14:20:23.000000 m9s_nereid-6.0.9/trytond_nereid/party.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3509 2022-03-29 15:04:46.000000 m9s_nereid-6.0.9/trytond_nereid/party.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      106 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/trytond_nereid/requirements.txt
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4565 2022-02-15 11:09:33.000000 m9s_nereid-6.0.9/trytond_nereid/setup.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     8087 2022-02-18 09:17:23.000000 m9s_nereid-6.0.9/trytond_nereid/static_file.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3259 2022-03-25 09:26:04.000000 m9s_nereid-6.0.9/trytond_nereid/static_file.xml
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/trytond_nereid/templates/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/trytond_nereid/templates/home.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)        0 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/templates/new-password.jinja
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.389809 m9s_nereid-6.0.9/trytond_nereid/templates/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      129 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/trytond_nereid/templates/tests/exists-both.html
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)       12 2020-03-16 09:24:45.000000 m9s_nereid-6.0.9/trytond_nereid/templates/tests/from-module.html
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.393809 m9s_nereid-6.0.9/trytond_nereid/tests/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      260 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/tests/__init__.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    15574 2022-03-25 09:50:34.000000 m9s_nereid-6.0.9/trytond_nereid/tests/debug_test_translation.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14973 2022-04-30 15:14:52.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_address.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    46739 2022-05-05 08:26:46.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_auth.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     3649 2021-12-11 18:21:20.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_common.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5168 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_country.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     5638 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_currency.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10376 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_i18n.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1846 2022-03-29 10:02:56.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_nereid.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    10084 2022-04-30 15:12:48.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_routing.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4716 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_static_file.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    14867 2022-03-29 15:04:46.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_translation.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     4671 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_user.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     2281 2021-12-16 10:44:45.000000 m9s_nereid-6.0.9/trytond_nereid/tests/test_website.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      611 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/tox.ini
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    28367 2022-02-18 09:17:23.000000 m9s_nereid-6.0.9/trytond_nereid/translation.py
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      442 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/translation.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      156 2022-11-13 17:15:48.000000 m9s_nereid-6.0.9/trytond_nereid/tryton.cfg
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    36639 2022-09-14 13:59:59.000000 m9s_nereid-6.0.9/trytond_nereid/user.py
+drwxr-xr-x   0 mathiasb  (1000) mathiasb  (1000)        0 2022-11-26 16:05:57.393809 m9s_nereid-6.0.9/trytond_nereid/view/
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      366 2022-03-29 15:04:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/contact_mechanism_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/contact_mechanism_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      290 2022-03-29 15:04:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/contact_mechanism_tree_sequence.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      765 2021-05-14 10:34:06.000000 m9s_nereid-6.0.9/trytond_nereid/view/nereid_user_form2.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      265 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/nereid_user_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      338 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/party_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      631 2021-03-16 09:13:55.000000 m9s_nereid-6.0.9/trytond_nereid/view/static_file_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/static_file_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      459 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/static_folder_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      182 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/static_folder_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      367 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/translation_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      796 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/url_map_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      278 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/url_map_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      252 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/url_rule_defaults_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      431 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/url_rule_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)     1007 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/website_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      322 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/website_locale_form.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      239 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/website_locale_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)      210 2020-03-16 09:24:46.000000 m9s_nereid-6.0.9/trytond_nereid/view/website_tree.xml
+-rw-r--r--   0 mathiasb  (1000) mathiasb  (1000)    15451 2022-02-18 09:17:23.000000 m9s_nereid-6.0.9/trytond_nereid/website.py
```

### Comparing `m9s_nereid-6.0.8/.drone.yml` & `m9s_nereid-6.0.9/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/.gitlab-ci.yml` & `m9s_nereid-6.0.9/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/CHANGELOG` & `m9s_nereid-6.0.9/CHANGELOG`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/COPYRIGHT` & `m9s_nereid-6.0.9/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/INSTALL` & `m9s_nereid-6.0.9/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/LICENSE.BSD` & `m9s_nereid-6.0.9/LICENSE.BSD`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/LICENSE.GPL3` & `m9s_nereid-6.0.9/LICENSE.GPL3`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/MANIFEST.in` & `m9s_nereid-6.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/MIGRATION` & `m9s_nereid-6.0.9/MIGRATION`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/Makefile` & `m9s_nereid-6.0.9/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -6,13 +6,13 @@
 	find . -name '*.pyc' -exec rm -f {} +
 	find . -name '*.pyo' -exec rm -f {} +
 	find . -name '*~' -exec rm -f {} +
 
 upload-docs:
 	$(MAKE) -C docs html dirhtml epub
 	cd docs/_build/; mv html nereid-docs; zip -r nereid-docs.zip nereid-docs; mv nereid-docs html
-	scp -r docs/_build/dirhtml/* openlabs.co.in:/var/www/nereid.openlabs.co.in/docs/
-	scp docs/_build/nereid-docs.zip openlabs.co.in:/var/www/nereid.openlabs.co.in/docs/nereid-docs.zip
-	scp docs/_build/epub/Nereid.epub openlabs.co.in:/var/www/nereid.openlabs.co.in/docs/nereid-docs.epub
+	scp -r docs/_build/dirhtml/* root@web:/srv/www/sites/nereid.m9s.biz/public
+	scp docs/_build/nereid-docs.zip root@web:/srv/www/sites/nereid.m9s.biz/public/docs/nereid-docs.zip
+	scp docs/_build/epub/Nereid.epub root@web:/srv/www/sites/nereid.m9s.biz/public/docs/nereid-docs.epub
 
 docs:
 	$(MAKE) -C docs html
```

### Comparing `m9s_nereid-6.0.8/PKG-INFO` & `m9s_nereid-6.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s_nereid
-Version: 6.0.8
+Version: 6.0.9
 Summary: Tryton Nereid Module
 Home-page: http://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_nereid-6.0.8/README.md` & `m9s_nereid-6.0.9/README.md`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/README.rst` & `m9s_nereid-6.0.9/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -2,42 +2,39 @@
 
 Welcome to Nereid
 ==================
 
 Welcome to Nereid's documentation.  This documentation is divided into
 different parts.  We recommend that you get started with
 :ref:`installation` and then head over to :ref:`quickstart`.
-Besides quickstart, there is also a more detailed :ref:`tutorial` that
-shows how to create a complete (albeit small) application with Nereid.  If
-you'd rather dive into the internals of Nereid, check out
+If you'd rather dive into the internals of Nereid, check out
 the :ref:`api` documentation.
  
 The main dependencies of Nereid are `Flask`_ and `Tryton`_. In addition,
 Nereid uses `Babel`_ for internationalisation, `Speak Later`_ for lazy
-strings, `WTForms`_ for form building and `ccy`_ for currency mapping. 
+strings and `WTForms`_ for form building.
 
 The template engine used is `Jinja2`_ and `Flask`_ is built over `Werkzeug`_ 
 a WSGI toolkit.These libraries are not documented here.  If you want to dive 
 into their documentation, check out the following links:
 
--   `Flask Documentation <http://flask.pocoo.org/docs/>`_
--   `Tryton Documentation <http://doc.tryton.org/2.4/>`_
--   `Babel Documentation <http://babel.edgewall.org/wiki/Documentation>`_
--   `Speaklater Documentation <http://pypi.python.org/pypi/speaklater>`_
--   `WTForms Documentation <http://wtforms.simplecodes.com/docs/dev/>`_
--   `CCY documentation <http://pypi.python.org/pypi/ccy>`_
--   `Jinja2 Documentation <http://jinja.pocoo.org/2/documentation/>`_
+-   `Flask Documentation <https://flask.palletsprojects.com/>`_
+-   `Tryton Documentation <https://docs.tryton.org/>`_
+-   `Babel Documentation <https://babel.pocoo.org/>`_
+-   `Speaklater Documentation <https://pypi.python.org/pypi/speaklater>`_
+-   `WTForms Documentation <https://wtforms.readthedocs.io/>`_
+-   `Jinja2 Documentation <https://jinja.palletsprojects.com/>`_
 
 If this documentation reminds you of `Flask`_ documentation, it is not a
 coincidence, it has been designed so to ease up the learning curve for
 anyone who knows both `Flask`_ and `Tryton`_.
 
-.. _Flask: http://flask.pocoo.org/
-.. _Tryton: http://www.tryton.org/index.html
-.. _WTForms: http://wtforms.simplecodes.com/docs/dev/
-.. _Babel: http://babel.edgewall.org/
-.. _Speak Later: http://pypi.python.org/pypi/speaklater
+.. _Flask: https://flask.palletsprojects.com/
+.. _Tryton: https://www.tryton.org
+.. _WTForms: https://wtforms.readthedocs.io
+.. _Babel: https://babel.pocoo.org/
+.. _Speak Later: https://pypi.python.org/pypi/speaklater
 .. _ccy: http://pypi.python.org/pypi/ccy
-.. _Jinja2: http://jinja.pocoo.org/2/
-.. _Werkzeug: http://werkzeug.pocoo.org/
+.. _Jinja2: https://jinja.palletsprojects.com/
+.. _Werkzeug: https://werkzeug.palletsprojects.com/
 
 .. include:: contents.rst.inc
```

### Comparing `m9s_nereid-6.0.8/doc/index.rst` & `m9s_nereid-6.0.9/doc/index.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/docs/Makefile` & `m9s_nereid-6.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/docs/_static/favicon.png` & `m9s_nereid-6.0.9/docs/_static/favicon.png`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/docs/_static/logo.png` & `m9s_nereid-6.0.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/docs/api.rst` & `m9s_nereid-6.0.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/docs/conf.py` & `m9s_nereid-6.0.9/docs/conf.py.bak`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import os
 import sys
+import os
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('..'))
 sys.path.append(os.path.abspath('_themes'))
 
@@ -41,31 +41,30 @@
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = 'Nereid'
-copyright = '2012-2015, Openlabs Technologies & Consulting (P) Limited'
+project = u'Nereid'
+copyright = u'2012-2015, Openlabs Technologies & Consulting (P) Limited'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
 import pkg_resources
-
 try:
     release = pkg_resources.get_distribution('trytond_nereid').version
 except pkg_resources.DistributionNotFound:
-    print('To build the documentation, The distribution information of Nereid')
-    print('Has to be available.  Either install the package into your')
-    print('development environment or run "setup.py develop" to setup the')
-    print('metadata.  A virtualenv is recommended!')
+    print 'To build the documentation, The distribution information of Nereid'
+    print 'Has to be available.  Either install the package into your'
+    print 'development environment or run "setup.py develop" to setup the'
+    print 'metadata.  A virtualenv is recommended!'
     sys.exit(1)
 del pkg_resources
 
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
@@ -197,16 +196,16 @@
 # Additional stuff for the LaTeX preamble.
 #'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass[howto/manual]).
 latex_documents = [
-    ('index', 'Nereid.tex', 'Nereid Documentation',
-        'Openlabs Technologies \\& Consulting (P) Limited', 'manual'),
+    ('index', 'Nereid.tex', u'Nereid Documentation',
+        u'Openlabs Technologies \\& Consulting (P) Limited', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -227,30 +226,30 @@
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'nereid', 'Nereid Documentation',
-     ['Openlabs Technologies & Consulting (P) Limited'], 1)
+    ('index', 'nereid', u'Nereid Documentation',
+     [u'Openlabs Technologies & Consulting (P) Limited'], 1)
 ]
 
 # If true, show URL addresses after external links.
 #man_show_urls = False
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    ('index', 'Nereid', 'Nereid Documentation',
-        'Openlabs Technologies & Consulting (P) Limited', 'Nereid',
+    ('index', 'Nereid', u'Nereid Documentation',
+        u'Openlabs Technologies & Consulting (P) Limited', 'Nereid',
         'One line description of project.', 'Miscellaneous'),
 ]
 
 # Documents to append as an appendix to all manuals.
 #texinfo_appendices = []
 
 # If false, no module index is generated.
@@ -259,18 +258,18 @@
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
 
 # -- Options for Epub output -------------------------------------------------
 
 # Bibliographic Dublin Core info.
-epub_title = 'Nereid'
-epub_author = 'Openlabs Technologies & Consulting (P) Limited'
-epub_publisher = 'Openlabs Technologies & Consulting (P) Limited'
-epub_copyright = '2012-2015, Openlabs Technologies & Consulting (P) Limited'
+epub_title = u'Nereid'
+epub_author = u'Openlabs Technologies & Consulting (P) Limited'
+epub_publisher = u'Openlabs Technologies & Consulting (P) Limited'
+epub_copyright = u'2012-2015, Openlabs Technologies & Consulting (P) Limited'
 
 # The language of the text. It defaults to the language option
 # or en if the language is not set.
 #epub_language = ''
 
 # The scheme of the identifier. Typical schemes are ISBN or URL.
 #epub_scheme = ''
```

### Comparing `m9s_nereid-6.0.8/docs/conf.py.bak` & `m9s_nereid-6.0.9/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Note that not all possible configuration values are present in this
 # autogenerated file.
 #
 # All configuration values have a default; values that are commented out
 # serve to show the default.
 
-import sys
 import os
+import sys
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 sys.path.insert(0, os.path.abspath('..'))
 sys.path.append(os.path.abspath('_themes'))
 
@@ -41,32 +41,42 @@
 # The encoding of source files.
 #source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'Nereid'
-copyright = u'2012-2015, Openlabs Technologies & Consulting (P) Limited'
-
+project = 'Nereid'
+copyright = '2014-2023, MBSolutions,  ' \
+    '2012-2015, Openlabs Technologies & Consulting (P) Limited'
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The full version, including alpha/beta/rc tags.
 import pkg_resources
+import subprocess
+
+release = ''
 try:
     release = pkg_resources.get_distribution('trytond_nereid').version
 except pkg_resources.DistributionNotFound:
-    print 'To build the documentation, The distribution information of Nereid'
-    print 'Has to be available.  Either install the package into your'
-    print 'development environment or run "setup.py develop" to setup the'
-    print 'metadata.  A virtualenv is recommended!'
+    packages = subprocess.check_output(
+        'pip freeze', shell=True, encoding='utf-8').split('\n')
+    for package in packages:
+        if 'nereid==' in package:
+            release = package.split('==')[1]
+            break
+if not release:
+    print('To build the documentation the distribution information of Nereid')
+    print('has to be available.  Either install the package into your')
+    print('development environment or run "setup.py develop" to setup the')
+    print('metadata.  A virtualenv is recommended!')
     sys.exit(1)
-del pkg_resources
+del pkg_resources, subprocess
 
 # The short X.Y version.
 version = '.'.join(release.split('.')[:2])
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
@@ -75,15 +85,15 @@
 # non-false value, then it is used:
 #today = ''
 # Else, today_fmt is used as the format for a strftime call.
 #today_fmt = '%B %d, %Y'
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
-exclude_patterns = ['_build']
+exclude_patterns = ['_build', '_themes']
 
 # The reST default role(used for this markup: `text`) to use for all documents.
 #default_role = None
 
 # If true, '()' will be appended to :func: etc. cross-reference text.
 #add_function_parentheses = True
 
@@ -110,15 +120,15 @@
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #html_theme_options = {}
 
 # Add any paths that contain custom themes here, relative to this directory.
-html_theme_path = ['_themes']
+html_theme_path = ['_themes/src/pallets_sphinx_themes/themes']
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 #html_title = None
 
 # A shorter title for the navigation bar.  Default is the same as html_title.
 #html_short_title = None
@@ -196,16 +206,16 @@
 # Additional stuff for the LaTeX preamble.
 #'preamble': '',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass[howto/manual]).
 latex_documents = [
-    ('index', 'Nereid.tex', u'Nereid Documentation',
-        u'Openlabs Technologies \\& Consulting (P) Limited', 'manual'),
+    ('index', 'Nereid.tex', 'Nereid Documentation',
+        'Openlabs Technologies \\& Consulting (P) Limited', 'manual'),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 #latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -226,30 +236,30 @@
 
 
 # -- Options for manual page output ------------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'nereid', u'Nereid Documentation',
-     [u'Openlabs Technologies & Consulting (P) Limited'], 1)
+    ('index', 'nereid', 'Nereid Documentation',
+     ['MBSolutions'], 1)
 ]
 
 # If true, show URL addresses after external links.
 #man_show_urls = False
 
 
 # -- Options for Texinfo output ----------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    ('index', 'Nereid', u'Nereid Documentation',
-        u'Openlabs Technologies & Consulting (P) Limited', 'Nereid',
+    ('index', 'Nereid', 'Nereid Documentation',
+        'MBSolutions', 'Nereid',
         'One line description of project.', 'Miscellaneous'),
 ]
 
 # Documents to append as an appendix to all manuals.
 #texinfo_appendices = []
 
 # If false, no module index is generated.
@@ -258,19 +268,18 @@
 # How to display URL addresses: 'footnote', 'no', or 'inline'.
 #texinfo_show_urls = 'footnote'
 
 
 # -- Options for Epub output -------------------------------------------------
 
 # Bibliographic Dublin Core info.
-epub_title = u'Nereid'
-epub_author = u'Openlabs Technologies & Consulting (P) Limited'
-epub_publisher = u'Openlabs Technologies & Consulting (P) Limited'
-epub_copyright = u'2012-2015, Openlabs Technologies & Consulting (P) Limited'
-
+epub_title = 'Nereid'
+epub_author = 'MBSolutions'
+epub_publisher = 'MBSolutions'
+epub_copyright = copyright
 # The language of the text. It defaults to the language option
 # or en if the language is not set.
 #epub_language = ''
 
 # The scheme of the identifier. Typical schemes are ISBN or URL.
 #epub_scheme = ''
 
@@ -308,7 +317,8 @@
     'flask': ('http://flask.pocoo.org/docs/', None),
 
 }
 
 
 # --- Tryton specific configuration ----
 os.environ['TRYTOND_DATABASE_URI'] = 'sqlite://'
+os.environ['DB_NAME'] = ':memory:'
```

### Comparing `m9s_nereid-6.0.8/docs/contents.rst.inc` & `m9s_nereid-6.0.9/docs/contents.rst.inc`

 * *Files 15% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 Familiarity with Tryton is assumed.
 
 .. toctree::
    :maxdepth: 2
 
    foreword
    installation
+   installation_windows
    quickstart
-   tutorial
 
 
 API Reference
 -------------
 
 If you are looking for information on a specific function, class or
 method, this part of the documentation is for you.
```

### Comparing `m9s_nereid-6.0.8/docs/foreword.rst` & `m9s_nereid-6.0.9/docs/foreword.rst`

 * *Files 9% similar despite different names*

```diff
@@ -19,25 +19,25 @@
 decision that we made while building nereid itself is tailored to build 
 applications which extend the functionality of the ERP system, like 
 e-commerce systems, EDI systems, Customer/Supplier Portals etc.
 
 Why Tryton as a backend ?
 -------------------------
 
-Well, why not, would be our question to you ? It's scalable, it's flexible 
+It's scalable, it's flexible 
 and offers the best approach we have seen so far into a declarative coding 
 pattern for model design in any ORM. The unique way Tryton handles 
 inheritance also makes it an excellent choice. In addition to the above, 
 Tryton by default has several modules which make designing business 
 applications faster in comparison to other frameworks.
 
 Let's say that you want to build a customer portal, (which is our example 
 application), all that you need to do from your end is create a module 
 which exposes the information that you want to, and leave other stuff like 
-order management, account management etc to the existing Tryton modules.
+order management, account management etc. to existing Tryton modules.
 
 Configuration and Conventions
 -----------------------------
 
 Flask has many configuration values, with sensible defaults, and a few
 conventions when getting started.  Nereid follows the same pattern of
 configuration values where it makes sense to use them. For configurations
@@ -45,9 +45,8 @@
 configuration is done from Tryton on the company or in website settings.
  
 Each website that you plan to have, needs to have a subdirectory within the
 application's python source tree. By convention a `static` subdirectory with
 the static content like CSS and JS is also created within it. While this 
 can be changed you usually don't have to, especially when getting started.
 
-Continue to :ref:`installation`, the :ref:`quickstart`, or the
-:ref:`advanced_foreword`.
+Continue to :ref:`installation` or :ref:`quickstart`.
```

### Comparing `m9s_nereid-6.0.8/docs/index.rst` & `m9s_nereid-6.0.9/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -2,42 +2,39 @@
 
 Welcome to Nereid
 ==================
 
 Welcome to Nereid's documentation.  This documentation is divided into
 different parts.  We recommend that you get started with
 :ref:`installation` and then head over to :ref:`quickstart`.
-Besides quickstart, there is also a more detailed :ref:`tutorial` that
-shows how to create a complete (albeit small) application with Nereid.  If
-you'd rather dive into the internals of Nereid, check out
+If you'd rather dive into the internals of Nereid, check out
 the :ref:`api` documentation.
  
 The main dependencies of Nereid are `Flask`_ and `Tryton`_. In addition,
 Nereid uses `Babel`_ for internationalisation, `Speak Later`_ for lazy
-strings, `WTForms`_ for form building and `ccy`_ for currency mapping. 
+strings and `WTForms`_ for form building.
 
 The template engine used is `Jinja2`_ and `Flask`_ is built over `Werkzeug`_ 
 a WSGI toolkit.These libraries are not documented here.  If you want to dive 
 into their documentation, check out the following links:
 
--   `Flask Documentation <http://flask.pocoo.org/docs/>`_
--   `Tryton Documentation <http://doc.tryton.org/2.4/>`_
--   `Babel Documentation <http://babel.edgewall.org/wiki/Documentation>`_
--   `Speaklater Documentation <http://pypi.python.org/pypi/speaklater>`_
--   `WTForms Documentation <http://wtforms.simplecodes.com/docs/dev/>`_
--   `CCY documentation <http://pypi.python.org/pypi/ccy>`_
--   `Jinja2 Documentation <http://jinja.pocoo.org/2/documentation/>`_
+-   `Flask Documentation <https://flask.palletsprojects.com/>`_
+-   `Tryton Documentation <https://docs.tryton.org/>`_
+-   `Babel Documentation <https://babel.pocoo.org/>`_
+-   `Speaklater Documentation <https://pypi.python.org/pypi/speaklater>`_
+-   `WTForms Documentation <https://wtforms.readthedocs.io/>`_
+-   `Jinja2 Documentation <https://jinja.palletsprojects.com/>`_
 
 If this documentation reminds you of `Flask`_ documentation, it is not a
 coincidence, it has been designed so to ease up the learning curve for
 anyone who knows both `Flask`_ and `Tryton`_.
 
-.. _Flask: http://flask.pocoo.org/
-.. _Tryton: http://www.tryton.org/index.html
-.. _WTForms: http://wtforms.simplecodes.com/docs/dev/
-.. _Babel: http://babel.edgewall.org/
-.. _Speak Later: http://pypi.python.org/pypi/speaklater
+.. _Flask: https://flask.palletsprojects.com/
+.. _Tryton: https://www.tryton.org
+.. _WTForms: https://wtforms.readthedocs.io
+.. _Babel: https://babel.pocoo.org/
+.. _Speak Later: https://pypi.python.org/pypi/speaklater
 .. _ccy: http://pypi.python.org/pypi/ccy
-.. _Jinja2: http://jinja.pocoo.org/2/
-.. _Werkzeug: http://werkzeug.pocoo.org/
+.. _Jinja2: https://jinja.palletsprojects.com/
+.. _Werkzeug: https://werkzeug.palletsprojects.com/
 
 .. include:: contents.rst.inc
```

### Comparing `m9s_nereid-6.0.8/docs/installation.rst` & `m9s_nereid-6.0.9/docs/installation.rst`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 Installation
 ============
 
 Nereid depends on a handful of Python libraries including Tryton.
 
 So how do you get all that on your system quickly?  There are many ways you
-could do that, but the most kick-ass method is `virtualenv`_. The `Flask
+could do that, but the most advanced method is `virtualenv`_. The `Flask
 Documentation`_ has a detailed `section on using virtualenv`_ to install
 Flask. You could refer to the same and then follow the instructions below.
 
 .. _virtualenv:
 
 virtualenv
 ----------
@@ -26,134 +26,115 @@
 
 or even better
 
 .. code-block:: sh
 
     $ sudo pip install virtualenv
 
-One of these will probably install virtualenv on your system.  Maybe it's even
-in your package manager.  If you use Ubuntu, try
+One of these will probably install virtualenv on your system.
+
+**The preferred way is to use
+your package manager. On Debian or Ubuntu systems use**
+
+.. code-block:: sh
+
+    $ sudo apt-get install virtualenv
+
+A very comfortable extension for managing multiple environments is virtualenvwrapper.
 
 .. code-block:: sh
 
-    $ sudo apt-get install python-virtualenv
+    $ sudo apt-get install virtualenvwrapper
 
-If you are on Windows and don't have the `easy_install` command, you must
-install it first.  Check :ref:`windows-easy-install` section for more
-information about how to do that.  Once you have it installed, run the same
-commands as above, but without the `sudo` prefix.
+.. note::
+    While developing and running on Windows is not recommended there are some
+    detailed instructions for Windows in :ref:`installation_windows`.
 
-Once you have virtualenv installed, just fire up a shell and create
-your own environment.  I usually create a project folder and a `venv`
-folder within
+Once you have virtualenvwrapper installed, it is able to manage separate directories
+for your project files and the virtualenv libraries thus keeping your project directory clean.
 
+Just add the following line to your ~/.bashrc
 
 .. code-block:: sh
 
-    $ mkdir myproject
-    $ cd myproject
-    $ virtualenv venv
-    New python executable in venv/bin/python
-    Installing distribute............done.
+    export PROJECT_HOME=<your_project_home>
 
-Now, whenever you want to work on a project, you only have to activate the
-corresponding environment.  On OS X and Linux, do the following:
+and you are ready to fire up a shell and create your own environment. 
+
+With virtualenvwrapper creating a new a project is as simple as 
 
 .. code-block:: sh
 
-    $ . venv/bin/activate
+    $ mkproject myproject
 
-If you are a Windows user, the following command is for you:
+Now, whenever you want to work on a project, you only have to activate the
+corresponding environment.  On OS X and Linux, do the following:
 
 .. code-block:: sh
 
-    $ venv\scripts\activate
+    $ workon myproject
 
 Either way, you should now be using your virtualenv (notice how the prompt of
 your shell has changed to show the active environment).
 
 Now you can just enter the following command to get Nereid activated in your
 virtualenv:
 
 
 .. code-block:: sh
 
-    $ pip install Nereid 
+    $ pip install m9s-nereid
 
 A few seconds, and you are good to go.
 
 
 System-Wide Installation
 ------------------------
 
-This is possible as well, though I do not recommend it.  Just run
-`pip` with root privileges
+This is possible as well, though usually not recommended. Could be a way to go in
+isolated containers. You have been warned! Just run `pip` with root privileges
 
 .. code-block:: sh
 
-    $ sudo pip install Nereid 
-
-(On Windows systems, run it in a command-prompt window with administrator
-privileges, and leave out `sudo`.)
+    $ sudo pip install m9s-nereid
 
 
 Living on the Edge
 ------------------
 
 If you want to work with the latest version of Nereid, you can tell
-it to operate on a git checkout.  Either way, virtualenv is recommended.
+it to operate on a git checkout.  Either way, virtualenv is strongly recommended.
 
 Get the git checkout in a new virtualenv and run in development mode
 
 .. code-block:: sh
 
-    $ git clone http://github.com/openlabs/nereid.git
-    Initialized empty Git repository in ~/dev/nereid/.git/
-    $ cd nereid 
-    $ virtualenv venv --distribute
-    New python executable in venv/bin/python
-    Installing distribute............done.
-    $ . venv/bin/activate
-    $ python setup.py develop
-    ...
-    Finished processing dependencies for Nereid 
+    $ git clone https://gitlab.com/m9s/nereid
+    $ pip install -e nereid
 
 This will pull in the dependencies and activate the git head as the current
 version inside the virtualenv.  Then all you have to do is run ``git pull
 origin`` to update to the latest version.
 
 
-.. _windows-easy-install:
-
-`pip` and `distribute` on Windows
------------------------------------
-
-On Windows, installation of `easy_install` is a bit tricky, but still
-achievable.  Read the section on `pip and distribute on Windows`_ on the
-Flask documentation for a better understanding.
-
-
 .. _cloning_for_dev:
 
 Cloning for Development
 -----------------------
 
 If you are cloning the repository for development or updating the
 documentation, you also need to initialise the git submodules for the
 theme used in the documentation.
 
 .. code-block:: sh
-    :emphasize-lines: 4,6 
+    :emphasize-lines: 3,4 
 
-    $ git clone http://github.com/openlabs/nereid.git
-    Initialized empty Git repository in ~/dev/nereid/.git/
+    $ git clone https://gitlab.com/m9s/nereid
     $ cd nereid
     $ git submodule init
-    Submodule 'docs/_themes' (git://github.com/openlabs/flask-sphinx-themes.git) registered for path 'docs/_themes'
     $ git submodule update
-    Submodule path 'docs/_themes': checked out 'revision #'
 
 
-.. _pip and distribute on Windows: http://flask.pocoo.org/docs/installation/#pip-and-distribute-on-windows
-.. _virtualenvs: http://www.virtualenv.org/en/latest/index.html
-.. _section on using virtualenv: http://flask.pocoo.org/docs/installation/#virtualenv
-.. _Flask Documentation: http://flask.pocoo.org/docs/
+.. _virtualenvs: https://virtualenv.pypa.io
+.. _section on using virtualenv: https://flask.palletsprojects.com/installation/#virtual-environments
+.. _Flask Documentation: https://flask.palletsprojects.com/
+
```

### Comparing `m9s_nereid-6.0.8/docs/license.rst` & `m9s_nereid-6.0.9/docs/license.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/docs/locale.rst` & `m9s_nereid-6.0.9/docs/locale.rst`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 This design allows your application to adapt to most requirements of
 localisation. For example if your web application has to be available to
 users in Spain, France and Belgium and has content in English, French and 
 Spanish, a good way to use locales would be:
 
 ============== ======================== ======================
- Code           Langauge                 Currency               
+ Code           Language                 Currency
 ============== ======================== ======================
  en             en_GB                    EUR                    
  fr             fr_FR                    EUR                    
  es             es_ES                    EUR                    
 ============== ======================== ======================
 
 URLs
```

### Comparing `m9s_nereid-6.0.8/docs/make.bat` & `m9s_nereid-6.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/docs/quickstart.rst` & `m9s_nereid-6.0.9/docs/quickstart.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,21 @@
 A minimal Nereid application first requries a Tryton database with the
 Nereid module installed. If you already have a database with Nereid
 installed, head over to `creating website`_.
 
 Setting up a database
 `````````````````````
 
-TODO
+Set up your database like any other `Tryton database <https://docs.tryton.org/projects/server/en/latest/topics/setup_database.html#topics-setup-database>`_
+
+.. code-block:: sh
+
+    $ trytond-admin -c <config file> -d <database name> -u nereid
+
+
 
 .. _creating website:
 
 Creating a new website
 ``````````````````````
 
 Once the nereid module is installed in a Tryton database, open the
@@ -63,15 +69,15 @@
 
 Creating the application and template
 `````````````````````````````````````
 
 Once the website is created, a python script which loads nereid and runs
 the application needs to be written. This script is used to load Nereid,
 configure your application settings and also serves as an APP_MODULE if
-you plan to use WSGI HTTP servers like `Gunicorn`_ 
+you plan to use WSGI HTTP servers like `Gunicorn`_ or `uWSGI`_
 
 .. code-block:: python
 
     #!/usr/bin/env python
     from nereid import Nereid
 
     CONFIG = dict(
@@ -170,7 +176,8 @@
     </html>
 
 Run the application again and you should be able to see the rendered HTML
 on your browser at `localhost:5000 <http://localhost:5000/>`_
 
 
 .. _Gunicorn: http://gunicorn.org/
+.. _uWSGI: https://uwsgi-docs.readthedocs.io
```

### Comparing `m9s_nereid-6.0.8/docs/versionmanagement.rst` & `m9s_nereid-6.0.9/docs/versionmanagement.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/m9s_nereid.egg-info/PKG-INFO` & `m9s_nereid-6.0.9/m9s_nereid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m9s-nereid
-Version: 6.0.8
+Version: 6.0.9
 Summary: Tryton Nereid Module
 Home-page: http://www.m9s.biz/
 Download-URL: https://gitlab.com/m9s/nereid.git
 Author: MBSolutions
 Author-email: info@m9s.biz
 License: GPL-3
 Project-URL: Bug Tracker, https://support.m9s.biz/
```

### Comparing `m9s_nereid-6.0.8/m9s_nereid.egg-info/SOURCES.txt` & `m9s_nereid-6.0.9/m9s_nereid.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,30 +17,33 @@
 README.md
 README.rst
 dev_requirements.txt
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
+.woodpecker/mail_curl.sh
+.woodpecker/report.yml
+.woodpecker/test.yml
 doc/index.rst
 doc/de/index.rst
 docs/Makefile
 docs/api.rst
 docs/conf.py
 docs/conf.py.bak
 docs/contents.rst.inc
 docs/foreword.rst
 docs/index.rst
 docs/installation.rst
+docs/installation_windows.rst
 docs/license.rst
 docs/locale.rst
 docs/make.bat
 docs/quickstart.rst
 docs/tryton_module_api.rst
-docs/tutorial.rst
 docs/versionmanagement.rst
 docs/_static/favicon.png
 docs/_static/logo.png
 docs/_templates/sidebarintro.html
 m9s_nereid.egg-info/PKG-INFO
 m9s_nereid.egg-info/SOURCES.txt
 m9s_nereid.egg-info/dependency_links.txt
```

### Comparing `m9s_nereid-6.0.8/nereid/__init__.py` & `m9s_nereid-6.0.9/nereid/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/application.py` & `m9s_nereid-6.0.9/nereid/application.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/caching.py` & `m9s_nereid-6.0.9/nereid/caching.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/config.py` & `m9s_nereid-6.0.9/nereid/config.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/contrib/locale.py` & `m9s_nereid-6.0.9/nereid/contrib/locale.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/contrib/pagination.py` & `m9s_nereid-6.0.9/nereid/contrib/pagination.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/contrib/sitemap.py` & `m9s_nereid-6.0.9/nereid/contrib/sitemap.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/csrf.py` & `m9s_nereid-6.0.9/nereid/csrf.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/ctx.py` & `m9s_nereid-6.0.9/nereid/ctx.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/globals.py` & `m9s_nereid-6.0.9/nereid/globals.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/helpers.py` & `m9s_nereid-6.0.9/nereid/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 from werkzeug.exceptions import (
     BadRequest, NotFound, RequestedRangeNotSatisfiable, abort)
 from werkzeug.urls import url_quote
 from werkzeug.utils import redirect
 from werkzeug.wsgi import wrap_file
 
 import trytond.modules
+from trytond.tools.misc import slugify as _slugify
 
 from trytond.config import config
 from trytond.transaction import Transaction
 
 from .globals import (  # noqa
     current_app, current_locale, current_user, current_website, request)
 
@@ -185,14 +186,19 @@
 
     .. versionchanged:: 1.1
         Filename may be a :class:`~os.PathLike` object.
 
     .. versionadded:: 1.1
         Partial content supports :class:`~io.BytesIO`.
 
+    .. versionchanged:: 6.0.8
+        The slugify method from nereid went partly into Tryton 5.4
+        Nereid now uses this method and extends it to return lower
+        case on slugs.
+
     :param filename_or_fp: the filename of the file to send.
                            This is relative to the :attr:`~nereid.root_path`
                            if a relative path is specified.
                            Alternatively a file object might be provided in
                            which case ``X-Sendfile`` might not work and fall
                            back to the traditional method.  Make sure that the
                            file pointer is positioned at the start of data to
@@ -346,27 +352,16 @@
         # make sure we don't send x-sendfile for servers that
         # ignore the 304 status code for x-sendfile.
         if rv.status_code == 304:
             rv.headers.pop("x-sendfile", None)
     return rv
 
 
-# The slugify method from nereid went upstream into 5.4
-# Only difference: we want lower case on slugs
-# TODO: Extend on 5.4 to that from trytond/tools/misc
-_slugify_strip_re = re.compile(r'[^\w\s-]')
-_slugify_hyphenate_re = re.compile(r'[-\s]+')
-
-
 def slugify(value, hyphenate='-'):
-    if not isinstance(value, str):
-        value = str(value)
-    value = unicodedata.normalize('NFKD', value)
-    value = str(_slugify_strip_re.sub('', value).strip())
-    return _slugify_hyphenate_re.sub(hyphenate, value).lower()
+    return _slugify(value, hyphenate=hyphenate).lower()
 
 
 def _rst_to_html_filter(value):
     """
     Converts RST text to HTML
     ~~~~~~~~~~~~~~~~~~~~~~~~~
     This uses docutils, if the library is missing, then the
```

### Comparing `m9s_nereid-6.0.8/nereid/routing.py` & `m9s_nereid-6.0.9/nereid/routing.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/sessions.py` & `m9s_nereid-6.0.9/nereid/sessions.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/signals.py` & `m9s_nereid-6.0.9/nereid/signals.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/templating.py` & `m9s_nereid-6.0.9/nereid/templating.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/testing.py` & `m9s_nereid-6.0.9/nereid/testing.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/tests/__init__.py` & `m9s_nereid-6.0.9/nereid/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/tests/test_dispatch.py` & `m9s_nereid-6.0.9/nereid/tests/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/tests/test_helpers.py` & `m9s_nereid-6.0.9/nereid/tests/test_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import jinja2
 
 from trytond.pool import PoolMeta
 from trytond.tests.test_tryton import with_transaction
 
 from nereid import template_filter, url_for
+from nereid.helpers import slugify
 from nereid.testing import POOL as Pool
 
 from .test_templates import BaseTestCase
 
 
 class TestURLfor(BaseTestCase):
     """
@@ -96,14 +97,27 @@
         app.jinja_loader.loaders
         app.jinja_loader._loaders.insert(0, jinja2.DictLoader(templates))
 
         with app.test_client() as c:
             response = c.get('/')
             self.assertEqual(response.data, b'cba')
 
+    def test_slugify(self):
+        "Test slugify"
+        self.assertEqual(slugify('unicode ♥ is ☢'), 'unicode-is')
+
+    def test_slugify_hyphenate(self):
+        "Test hyphenate in slugify"
+        self.assertEqual(slugify('foo bar', hyphenate='_'), 'foo_bar')
+
+    def test_slugify_lower(self):
+        "Test lower case in slugify"
+        self.assertEqual(slugify('Foo BaR'), 'foo-bar')
+
+
 
 def suite():
     "Nereid Helpers test suite"
     test_suite = unittest.TestSuite()
     test_suite.addTests([
         unittest.TestLoader().loadTestsFromTestCase(TestURLfor),
         unittest.TestLoader().loadTestsFromTestCase(TestHelperFunctions),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `m9s_nereid-6.0.8/nereid/tests/test_pagination.py` & `m9s_nereid-6.0.9/nereid/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/tests/test_signals.py` & `m9s_nereid-6.0.9/nereid/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/tests/test_templates.py` & `m9s_nereid-6.0.9/nereid/tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid/wrappers.py` & `m9s_nereid-6.0.9/nereid/wrappers.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid_test_module/README.rst` & `m9s_nereid-6.0.9/nereid_test_module/README.rst`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid_test_module/model.py` & `m9s_nereid-6.0.9/nereid_test_module/model.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/nereid_test_module/templates/tests/translation-test.html` & `m9s_nereid-6.0.9/nereid_test_module/templates/tests/translation-test.html`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/setup.py` & `m9s_nereid-6.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/tox.ini` & `m9s_nereid-6.0.9/trytond_nereid/tox.ini`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,15 @@
 [tox]
-envlist = {py310}-{sqlite}
+envlist = {py35,py36,py37}-{sqlite,postgresql},pypy3-{sqlite,postgresql}
 
 [testenv]
+commands = {envpython} setup.py test
 deps =
-    coverage
-    -rdev_requirements.txt
-    {py310}-postgresql: psycopg2-binary
+    {py35,py36,py37}-postgresql: psycopg2 >= 2.5
     pypy3-postgresql: psycopg2cffi >= 2.5
-
+    {py35,py36}-sqlite: sqlitebck
 setenv =
     sqlite: TRYTOND_DATABASE_URI={env:SQLITE_URI:sqlite://}
-    postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://test:test@postgres}
+    postgresql: TRYTOND_DATABASE_URI={env:POSTGRESQL_URI:postgresql://}
     sqlite: DB_NAME={env:SQLITE_NAME::memory:}
     postgresql: DB_NAME={env:POSTGRESQL_NAME:test}
-
-[testenv:py310-sqlite]
-commands = coverage run setup.py test
-
-[testenv:py310-postgresql]
-commands = python setup.py test
-
-install_command = pip install --pre --find-links https://trydevpi.tryton.org/?local_version={env:CI_JOB_ID:{env:CI_BUILD_NUMBER:}.{env:CI_JOB_NUMBER:}}&mirror=github {opts} {packages}
+install_command = pip install --pre --find-links https://trydevpi.tryton.org/?mirror=bitbucket {opts} {packages}
```

### Comparing `m9s_nereid-6.0.8/trytond_nereid/.drone.yml` & `m9s_nereid-6.0.9/trytond_nereid/.drone.yml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/COPYRIGHT` & `m9s_nereid-6.0.9/trytond_nereid/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/INSTALL` & `m9s_nereid-6.0.9/trytond_nereid/INSTALL`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/LICENSE` & `m9s_nereid-6.0.9/trytond_nereid/LICENSE`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/README.md` & `m9s_nereid-6.0.9/trytond_nereid/README.md`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/__init__.py` & `m9s_nereid-6.0.9/trytond_nereid/__init__.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/configuration.xml` & `m9s_nereid-6.0.9/trytond_nereid/configuration.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/country.py` & `m9s_nereid-6.0.9/trytond_nereid/country.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/currency.py` & `m9s_nereid-6.0.9/trytond_nereid/currency.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/icons/tryton-web.svg` & `m9s_nereid-6.0.9/trytond_nereid/icons/tryton-web.svg`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/locale/ca.po` & `m9s_nereid-6.0.9/trytond_nereid/locale/ca.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/locale/de.po` & `m9s_nereid-6.0.9/trytond_nereid/locale/de.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/locale/es.po` & `m9s_nereid-6.0.9/trytond_nereid/locale/es.po`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/message.xml` & `m9s_nereid-6.0.9/trytond_nereid/message.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/model.py` & `m9s_nereid-6.0.9/trytond_nereid/model.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/party.py` & `m9s_nereid-6.0.9/trytond_nereid/party.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/party.xml` & `m9s_nereid-6.0.9/trytond_nereid/party.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/setup.py` & `m9s_nereid-6.0.9/trytond_nereid/setup.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/static_file.py` & `m9s_nereid-6.0.9/trytond_nereid/static_file.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/static_file.xml` & `m9s_nereid-6.0.9/trytond_nereid/static_file.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/debug_test_translation.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/debug_test_translation.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_address.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_address.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_auth.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_common.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_country.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_country.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_currency.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_currency.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_i18n.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_i18n.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_nereid.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_nereid.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_routing.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_static_file.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_static_file.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_translation.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_translation.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_user.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/tests/test_website.py` & `m9s_nereid-6.0.9/trytond_nereid/tests/test_website.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/translation.py` & `m9s_nereid-6.0.9/trytond_nereid/translation.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/user.py` & `m9s_nereid-6.0.9/trytond_nereid/user.py`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/view/nereid_user_form2.xml` & `m9s_nereid-6.0.9/trytond_nereid/view/nereid_user_form2.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/view/static_file_form.xml` & `m9s_nereid-6.0.9/trytond_nereid/view/static_file_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/view/url_map_form.xml` & `m9s_nereid-6.0.9/trytond_nereid/view/url_map_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/view/website_form.xml` & `m9s_nereid-6.0.9/trytond_nereid/view/website_form.xml`

 * *Files identical despite different names*

### Comparing `m9s_nereid-6.0.8/trytond_nereid/website.py` & `m9s_nereid-6.0.9/trytond_nereid/website.py`

 * *Files identical despite different names*

