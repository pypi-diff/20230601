# Comparing `tmp/cdp-scrapers-0.6.1.tar.gz` & `tmp/cdp-scrapers-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdp-scrapers-0.6.1.tar", last modified: Tue Feb 21 22:12:54 2023, max compression
+gzip compressed data, was "cdp-scrapers-0.7.0.tar", last modified: Thu Jun  1 18:38:07 2023, max compression
```

## Comparing `cdp-scrapers-0.6.1.tar` & `cdp-scrapers-0.7.0.tar`

### file list

```diff
@@ -1,45 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:12:54.062260 cdp-scrapers-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-02-21 22:12:54.062260 cdp-scrapers-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4645 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:12:54.058260 cdp-scrapers-0.6.1/cdp_scrapers/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:12:54.062260 cdp-scrapers-0.6.1/cdp_scrapers/instances/
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28137 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/atlanta.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/houston.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/kingcounty-static.json
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/kingcounty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/lacity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/portland-static.json
--rw-r--r--   0 runner    (1001) docker     (123)    25070 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/portland.py
--rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/seattle-static.json
--rw-r--r--   0 runner    (1001) docker     (123)    21997 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/instances/seattle.py
--rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/legistar_content_parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)    58592 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/legistar_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    23453 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/prime_gov_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20610 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/scraper_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/cdp_scrapers/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:12:54.058260 cdp-scrapers-0.6.1/cdp_scrapers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-02-21 22:12:54.000000 cdp-scrapers-0.6.1/cdp_scrapers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-02-21 22:12:54.000000 cdp-scrapers-0.6.1/cdp_scrapers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 22:12:54.000000 cdp-scrapers-0.6.1/cdp_scrapers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-21 22:12:54.000000 cdp-scrapers-0.6.1/cdp_scrapers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 22:12:54.000000 cdp-scrapers-0.6.1/cdp_scrapers.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-02-21 22:12:54.000000 cdp-scrapers-0.6.1/cdp_scrapers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-02-21 22:12:54.000000 cdp-scrapers-0.6.1/cdp_scrapers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 22:12:54.062260 cdp-scrapers-0.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     5422 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/docs/finding_legistar_id.rst
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/docs/legistar_scraper.rst
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-02-21 22:12:54.062260 cdp-scrapers-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-02-21 22:12:49.000000 cdp-scrapers-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.719034 cdp-scrapers-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.cookiecutter.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.707034 cdp-scrapers-0.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.707034 cdp-scrapers-0.7.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.707034 cdp-scrapers-0.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.github/workflows/docs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.707034 cdp-scrapers-0.7.0/.github/workflows/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.github/workflows/scripts/run-scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.github/workflows/test-scraper.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3127 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/Justfile
+-rw-r--r--   0 runner    (1001) docker     (123)    16018 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-01 18:38:07.719034 cdp-scrapers-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4756 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.711034 cdp-scrapers-0.7.0/cdp_scrapers/
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/finding_legistar_id.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.715034 cdp-scrapers-0.7.0/cdp_scrapers/instances/
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28100 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/atlanta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/houston.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/kingcounty-static.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/kingcounty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/lacity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12830 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/portland-static.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25152 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/portland.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/seattle-static.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21950 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/instances/seattle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5899 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/legistar_content_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59260 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/legistar_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23466 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/prime_gov_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    25365 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/scraper_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/static_data.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.715034 cdp-scrapers-0.7.0/cdp_scrapers/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/tests/legistar_content_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/tests/test_prime_gov_agenda_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/tests/test_prime_gov_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13141 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/tests/test_scraper_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9379 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/tests/test_scrapers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/tests/test_youtube_scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/cdp_scrapers/youtube_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.715034 cdp-scrapers-0.7.0/cdp_scrapers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-01 18:38:07.000000 cdp-scrapers-0.7.0/cdp_scrapers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-06-01 18:38:07.000000 cdp-scrapers-0.7.0/cdp_scrapers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:38:07.000000 cdp-scrapers-0.7.0/cdp_scrapers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:38:07.000000 cdp-scrapers-0.7.0/cdp_scrapers.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-01 18:38:07.000000 cdp-scrapers-0.7.0/cdp_scrapers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-01 18:38:07.000000 cdp-scrapers-0.7.0/cdp_scrapers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.719034 cdp-scrapers-0.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5458 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/docs/finding_legistar_id.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/docs/legistar_scraper.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:38:07.719034 cdp-scrapers-0.7.0/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/images/get_events.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15098 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/images/seattle_legistar_url.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:38:07.719034 cdp-scrapers-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 18:37:56.000000 cdp-scrapers-0.7.0/setup.py
```

### Comparing `cdp-scrapers-0.6.1/PKG-INFO` & `cdp-scrapers-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: cdp-scrapers
-Version: 0.6.1
+Version: 0.7.0
 Summary: Scratchpad for scraper development and general utilities.
-Home-page: https://github.com/CouncilDataProject/cdp-scrapers
-Author: Eva Maxfield Brown, Sung Cho, Shak Ragoler
-Author-email: evamaxfieldbrown@gmail.com
-License: MIT license
-Keywords: cdp-scrapers
-Platform: UNKNOWN
+Author: Sung Cho, Shak Ragoler
+Author-email: Eva Maxfield Brown <evamaxfieldbrown@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/CouncilDataProject/cdp-scrapers
+Project-URL: Bug Tracker, https://github.com/CouncilDataProject/cdp-scrapers/issues
+Project-URL: Documentation, https://CouncilDataProject.github.io/cdp-scrapers
+Project-URL: User Support, https://github.com/CouncilDataProject/cdp-scrapers/issues
 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: atlanta
+Provides-Extra: all
+Provides-Extra: lint
 Provides-Extra: test
+Provides-Extra: docs
 Provides-Extra: dev
-Provides-Extra: all
 License-File: LICENSE
 
 # cdp-scrapers
 
-[![Build Status](https://github.com/CouncilDataProject/cdp-scrapers/workflows/Build%20Main/badge.svg)](https://github.com/CouncilDataProject/cdp-scrapers/actions)
-[![Documentation](https://github.com/CouncilDataProject/cdp-scrapers/workflows/Documentation/badge.svg)](https://CouncilDataProject.github.io/cdp-scrapers/)
+[![Build Status](https://github.com/CouncilDataProject/cdp-scrapers/workflows/CI/badge.svg)](https://github.com/CouncilDataProject/cdp-scrapers/actions)
+[![Documentation](https://github.com/CouncilDataProject/cdp-scrapers/workflows/Documentation/badge.svg)](https://CouncilDataProject.github.io/cdp-scrapers)
 
 Scratchpad for scraper development and general utilities.
 
 ---
 
+## Installation
+
+**Stable Release:** `pip install cdp-scrapers`<br>
+**Development Head:** `pip install git+https://github.com/CouncilDataProject/cdp-scrapers.git`
+
 ## Council Data Project
 
 Council Data Project is an open-source project dedicated to providing journalists,
 activists, researchers, and all members of each community we serve with the tools they
 need to stay informed and hold their Council Members accountable.
 
 For more information about Council Data Project, please visit
@@ -76,17 +83,15 @@
 )
 ```
 
 ### Scrapers
 
 #### Event Scraper Structure
 
-![get_events](./images/get_events.png)
-
-Our current event scraper structure is as shown above. The main function `get_events` 
+Our current event scraper structure is as follows. The main function `get_events` 
 gets all the required data and it calls the `get_content_uris` function to return the 
 required video data.
 
 If your city uses Legistar and the Legistar data is publicly available.
 - You may be able to reuse our scraper with minimal modifications, such as providing the 
 correct Legistar client ID for your municipality.
 - If the Legistar data returned only does not include the EventVideoPath field for the 
@@ -135,10 +140,8 @@
 
 For full package documentation please visit [councildataproject.org/cdp-scrapers](https://councildataproject.org/cdp-scrapers).
 
 ## Development
 
 Refer to [CONTRIBUTING.md](CONTRIBUTING.md) for information related to developing the code.
 
-**MIT license**
-
-
+**MPLv2 License**
```

### Comparing `cdp-scrapers-0.6.1/README.md` & `cdp-scrapers-0.7.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 # cdp-scrapers
 
-[![Build Status](https://github.com/CouncilDataProject/cdp-scrapers/workflows/Build%20Main/badge.svg)](https://github.com/CouncilDataProject/cdp-scrapers/actions)
-[![Documentation](https://github.com/CouncilDataProject/cdp-scrapers/workflows/Documentation/badge.svg)](https://CouncilDataProject.github.io/cdp-scrapers/)
+[![Build Status](https://github.com/CouncilDataProject/cdp-scrapers/workflows/CI/badge.svg)](https://github.com/CouncilDataProject/cdp-scrapers/actions)
+[![Documentation](https://github.com/CouncilDataProject/cdp-scrapers/workflows/Documentation/badge.svg)](https://CouncilDataProject.github.io/cdp-scrapers)
 
 Scratchpad for scraper development and general utilities.
 
 ---
 
+## Installation
+
+**Stable Release:** `pip install cdp-scrapers`<br>
+**Development Head:** `pip install git+https://github.com/CouncilDataProject/cdp-scrapers.git`
+
 ## Council Data Project
 
 Council Data Project is an open-source project dedicated to providing journalists,
 activists, researchers, and all members of each community we serve with the tools they
 need to stay informed and hold their Council Members accountable.
 
 For more information about Council Data Project, please visit
@@ -51,17 +56,15 @@
 )
 ```
 
 ### Scrapers
 
 #### Event Scraper Structure
 
-![get_events](./images/get_events.png)
-
-Our current event scraper structure is as shown above. The main function `get_events` 
+Our current event scraper structure is as follows. The main function `get_events` 
 gets all the required data and it calls the `get_content_uris` function to return the 
 required video data.
 
 If your city uses Legistar and the Legistar data is publicly available.
 - You may be able to reuse our scraper with minimal modifications, such as providing the 
 correct Legistar client ID for your municipality.
 - If the Legistar data returned only does not include the EventVideoPath field for the 
@@ -110,8 +113,8 @@
 
 For full package documentation please visit [councildataproject.org/cdp-scrapers](https://councildataproject.org/cdp-scrapers).
 
 ## Development
 
 Refer to [CONTRIBUTING.md](CONTRIBUTING.md) for information related to developing the code.
 
-**MIT license**
+**MPLv2 License**
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/__init__.py` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,24 @@
-# -*- coding: utf-8 -*-
-
-"""
-Individual scratchpad and maybe up-to-date CDP instance scrapers.
-"""
+"""Individual scratchpad and maybe up-to-date CDP instance scrapers."""
 
 import importlib
 import inspect
 import sys
 from datetime import datetime
 from functools import partial
 from pkgutil import iter_modules
 from typing import Any, Callable, Dict, List, Type
 
 from cdp_backend.pipeline.ingestion_models import EventIngestionModel
 from cdp_backend.pipeline.mock_get_events import (
     get_events as get_test_deployment_events,
 )
 
-from cdp_scrapers.instances.houston import get_houston_events
 from cdp_scrapers.instances.atlanta import get_events as get_atlanta_events
+from cdp_scrapers.instances.houston import get_houston_events
 from cdp_scrapers.instances.lacity import LosAngelesScraper, get_lacity_events
 from cdp_scrapers.instances.portland import get_portland_events
 from cdp_scrapers.legistar_utils import LegistarScraper
 
 ###############################################################################
 
 
@@ -38,15 +34,15 @@
 
 SCRAPER_FUNCTIONS: Dict[str, Callable] = {}
 for submodule in iter_modules(__path__):
     # Import the submodule
     mod = importlib.import_module(f"{__name__}.{submodule.name}")
 
     # Get the scraper from the module
-    for a, member_cls in inspect.getmembers(mod, inspect.isclass):
+    for _a, member_cls in inspect.getmembers(mod, inspect.isclass):
         if (
             issubclass(member_cls, LegistarScraper)
             and member_cls is not LegistarScraper
         ):
             scraper_get_events = partial(
                 _init_and_run_get_events,
                 legistar_scraper=member_cls,
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/atlanta.py` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/atlanta.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 
 log = logging.getLogger(__name__)
 
 
 def get_single_person(driver: "WebDriver", member_name: str) -> ingestion_models.Person:
     """
     Get all the information fot one person
-    Includes: role, seat, picture, phone, email
+    Includes: role, seat, picture, phone, email.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     driver:
         webdriver calling the people's dictionary page
     member_name:
         person's name
 
-    Returns:
-    --------------
+    Returns
+    -------
     ingestion_models
         the ingestion model for the person's part
     """
     import selenium
     from selenium.webdriver.common.by import By
 
     log.info("start get active person ingestion model")
@@ -79,18 +79,18 @@
             roles=[ingestion_models.Role(title=member_role)],
         ),
     )
 
 
 def get_person() -> dict:
     """
-    Put the informtion get by get_single_person() to dictionary
+    Put the informtion get by get_single_person() to dictionary.
 
-    Returns:
-    --------------
+    Returns
+    -------
     dictionary
         key: person's name
         value: person's ingestion model
     """
     from selenium import webdriver
     from selenium.webdriver.chrome.options import Options
     from selenium.webdriver.chrome.service import Service
@@ -130,41 +130,41 @@
         person_dict[member_name] = member_model
     driver.quit()
     return person_dict
 
 
 def get_new_person(name: str) -> ingestion_models.Person:
     """
-    Creates the person ingestion model for the people that are not recored
+    Creates the person ingestion model for the people that are not recored.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     name:str
         the name of the person
 
-    Returns:
-    --------------
+    Returns
+    -------
     ingestion model
         the person ingestion model for the newly appeared person
     """
     log.info("start get inactive person ingestion model")
     return ingestion_models.Person(name=name, is_active=False)
 
 
 def convert_status_constant(decision: str) -> str:
     """
-    Converts the matter result status to the exsiting constants
+    Converts the matter result status to the exsiting constants.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     decision: str
         decision of the matter
 
-    Returns:
-    --------------
+    Returns
+    -------
     db_constants
         result status constants
     """
     log.info("start convert result status for vote ingestion model")
     d_constant = decision
     if ("FAVORABLE" in decision) or ("ADOPTED" in decision) or ("ACCEPTED" in decision):
         d_constant = db_constants.MatterStatusDecision.ADOPTED
@@ -184,34 +184,34 @@
 def assign_constant(
     driver: "WebDriver",
     i: int,
     j: int,
     vote_decision: str,
     voting_list: list,
     body_name: str,
-    PERSONS: dict,
+    persons: dict,
 ):
     """
-    Assign constants and add Vote to the ingestion models based on the vote decision
+    Assign constants and add Vote to the ingestion models based on the vote decision.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     driver:webdriver
         webdriver of the matter page
     i: int
         tr[i] is the matter we are looking at
     j: int
         the row number of the information in a matter that we are looking at
     vote_decision: str
         the vote decision constant of the vote decision
     voting_list: list
         the list that contains vote ingestion models
     body_name: str
         the body name of the current meeting
-    PERSONS: dict
+    persons: dict
         Dict[str, ingestion_models.Person]
     """
     from selenium.webdriver.common.by import By
 
     log.info("start get vote ingestion model for one type of decision")
     v_res = driver.find_element(
         By.XPATH,
@@ -231,16 +231,16 @@
                 r"([a-zA-Z]+)((\ {0,1}[a-zA-Z]+\.{0,1}\ )|(\ ))([a-zA-Z]+)", p
             )
             if n_temp is not None:
                 n = f"{n_temp.group(1)} {n_temp.group(5)}"
             else:
                 raise ValueError("Person name could not be constructed.")
         person = get_new_person(n)
-        if n in PERSONS:
-            person = PERSONS[n]
+        if n in persons:
+            person = persons[n]
             if person.seat is not None:
                 if person.seat.roles is not None:
                     person.seat.roles[0].body = ingestion_models.Body(
                         body_name, is_active=True
                     )
                     if body_name == "City Council":
                         if (
@@ -260,34 +260,34 @@
 
 
 def get_voting_result(
     driver: "WebDriver",
     sub_sections_len: int,
     i: int,
     body_name: str,
-    PERSONS: dict,
+    persons: dict,
 ) -> list:
     """
-    Scrapes and converts the voting decisions to the exsiting constants
+    Scrapes and converts the voting decisions to the exsiting constants.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     driver:webdriver
         webdriver of the matter page
     sub_sections_len: int
         the row number in the block under the matter for the current date
     i: int
         tr[i] is the matter we are looking at
     body_name: str
         the body name of the current meeting
-    PERSONS: dict
+    persons: dict
         Dict[str, ingestion_models.Person]
 
-    Returns:
-    --------------
+    Returns
+    -------
     list
         contains the Vote ingestion model for each person
     """
     from selenium.webdriver.common.by import By
 
     log.info("start get the vote ingestion model for a matter")
     voting_list: list[ingestion_models.Vote] = []
@@ -300,51 +300,51 @@
             + str(j)
             + "]",
         )
         sub_content_role = sub_content.find_element(By.CLASS_NAME, "Role").text
         if "AYES" in sub_content_role:
             vote_decision = db_constants.VoteDecision.APPROVE
             assign_constant(
-                driver, i, j, vote_decision, voting_list, body_name, PERSONS
+                driver, i, j, vote_decision, voting_list, body_name, persons
             )
         if "NAYS" in sub_content_role:
             vote_decision = db_constants.VoteDecision.REJECT
             assign_constant(
-                driver, i, j, vote_decision, voting_list, body_name, PERSONS
+                driver, i, j, vote_decision, voting_list, body_name, persons
             )
         if (
             "ABSENT" in sub_content_role
             or "AWAY" in sub_content_role
             or "EXCUSED" in sub_content_role
         ):
             vote_decision = db_constants.VoteDecision.ABSENT_NON_VOTING
             assign_constant(
-                driver, i, j, vote_decision, voting_list, body_name, PERSONS
+                driver, i, j, vote_decision, voting_list, body_name, persons
             )
         if "ABSTAIN" in sub_content_role:
             vote_decision = db_constants.VoteDecision.ABSTAIN_NON_VOTING
             assign_constant(
-                driver, i, j, vote_decision, voting_list, body_name, PERSONS
+                driver, i, j, vote_decision, voting_list, body_name, persons
             )
     return voting_list
 
 
 def get_matter_status(driver: "WebDriver", i: int) -> Tuple[list, str]:
     """
-    Find the matter result status
+    Find the matter result status.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     driver:webdriver
         webdriver of the matter page
     i: int
         tracker used to loop the rows in the matter page
 
-    Returns:
-    --------------
+    Returns
+    -------
     sub_sections: element
         the block under the matter for the current date
     decision_constant: element
         the matter decision constant
     """
     from selenium.webdriver.common.by import By
 
@@ -362,45 +362,45 @@
         + str(i + 1)
         + "]/td/table/tbody/tr",
     )
     status_constant = convert_status_constant(decision)
     return sub_sections, status_constant
 
 
-def parse_single_matter(
+def parse_single_matter(  # noqa: C901 D417
     driver: "WebDriver",
     test: str,
     item: str,
     body_name: str,
     s_word_formated: datetime,
-    PERSONS: dict,
+    persons: dict,
 ) -> ingestion_models.EventMinutesItem:
     """
-    Get the minute items that contains a matter
+    Get the minute items that contains a matter.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     driver:webdriver
         webdriver of the matter page
     matter:element
         the matter we are looking at
     body_name: str
         the body name of the current meeting
     s_word_formated: datetime
         the date of the current meeting
-    PERSONS: dict
+    persons: dict
         Dict[str, ingestion_models.Person]
 
-    Returns:
-    --------------
+    Returns
+    -------
     ingestion model
         minutes ingestion model with the matters information
     """
     from selenium.webdriver.common.by import By
-    from selenium.webdriver.support import expected_conditions as EC
+    from selenium.webdriver.support import expected_conditions as ec
     from selenium.webdriver.support.ui import WebDriverWait
 
     log.info("start get ingestion model for a matter")
     voting_list = []
     matter_name = item[0:9]  # name of the matter eg. "22-C-5024", "22-R-3404"
     matter_title = item[
         12:
@@ -412,15 +412,15 @@
     matter_type_list = re.split("A |AN ", matter_type_temp)
     if len(matter_type_list) > 1:
         matter_type = matter_type_list[1]
     link = driver.find_element("link text", item)
     link.click()
     # get to the specific page for each matter
     s_matter = WebDriverWait(driver, 10).until(
-        EC.presence_of_all_elements_located(
+        ec.presence_of_all_elements_located(
             (
                 By.XPATH,
                 '//*[@id="ContentPlaceHolder1_divHistory"]/div/table/tbody/tr',
             )
         )
     )
     sponsor_raw = driver.find_element(
@@ -440,44 +440,44 @@
                     r"([a-zA-Z]+)((\ {0,1}[a-zA-Z]+\.{0,1}\ )|(\ ))([a-zA-Z]+)",
                     current_temp2,
                 )
                 if current_name is not None:
                     current = f"{current_name.group(1)} {current_name.group(5)}"
                 else:
                     raise ValueError("Person name could not be constructed.")
-                if current in PERSONS:
-                    sponsors.append(PERSONS[current])
+                if current in persons:
+                    sponsors.append(persons[current])
                 else:
                     sponsors.append(get_new_person(current))
             elif "Post" in s:
                 current_temp3 = s.split("Large ")[1]
                 current_name = re.match(
                     r"([a-zA-Z]+)((\ {0,1}[a-zA-Z]+\.{0,1}\ )|(\ ))([a-zA-Z]+)",
                     current_temp3,
                 )
                 if current_name is not None:
                     current = f"{current_name.group(1)} {current_name.group(5)}"
                 else:
                     raise ValueError("Person name could not be constructed.")
-                if current in PERSONS:
-                    sponsors.append(PERSONS[current])
+                if current in persons:
+                    sponsors.append(persons[current])
                 else:
                     sponsors.append(get_new_person(current))
             elif "President" in s:
                 current_temp4 = s.split("President ")[1]
                 current_name = re.match(
                     r"([a-zA-Z]+)((\ {0,1}[a-zA-Z]+\.{0,1}\ )|(\ ))([a-zA-Z]+)",
                     current_temp4,
                 )
                 if current_name is not None:
                     current = f"{current_name.group(1)} {current_name.group(5)}"
                 else:
                     raise ValueError("Person name could not be constructed.")
-                if current in PERSONS:
-                    sponsors.append(PERSONS[current])
+                if current in persons:
+                    sponsors.append(persons[current])
                 else:
                     sponsors.append(get_new_person(current))
         s_rows = len(s_matter)
         for i in range(1, s_rows + 1, 2):
             header = driver.find_element(
                 By.XPATH,
                 '//*[@id="ContentPlaceHolder1_divHistory"]/div/table/tbody/tr['
@@ -495,15 +495,15 @@
                     db_constants.MatterStatusDecision.ADOPTED,
                 ):
                     decision = db_constants.EventMinutesItemDecision.PASSED
                 else:
                     decision = db_constants.EventMinutesItemDecision.FAILED
                 if "[" in test:
                     voting_list = get_voting_result(
-                        driver, len(sub_sections), i, body_name, PERSONS
+                        driver, len(sub_sections), i, body_name, persons
                     )
 
         if len(sponsors) != 0:
             return ingestion_models.EventMinutesItem(
                 minutes_item=ingestion_models.MinutesItem(
                     name=matter_name.title(), description=matter_title
                 ),
@@ -529,55 +529,55 @@
             result_status=status,
         ),
         decision=decision,
         votes=voting_list,
     )
 
 
-def parse_event(
+def parse_event(  # noqa: C901
     url: str,
 ) -> ingestion_models.EventIngestionModel:
     """
-    Scrapes all the information for a meeting
+    Scrapes all the information for a meeting.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     url:str
         the url of the meeting that we want to scrape
 
-    Returns:
-    --------------
+    Returns
+    -------
     ingestion model
         the ingestion model for the meeting
     """
     import selenium
     from selenium import webdriver
     from selenium.webdriver.chrome.options import Options
     from selenium.webdriver.chrome.service import Service
     from selenium.webdriver.common.by import By
-    from selenium.webdriver.support import expected_conditions as EC
+    from selenium.webdriver.support import expected_conditions as ec
     from selenium.webdriver.support.ui import WebDriverWait
     from webdriver_manager.chrome import ChromeDriverManager
 
     log.info("start get ingestion model for a event")
 
-    MINUTE_INDEX = [chr(i) for i in range(ord("A"), ord("Z") + 1)]
-    PERSONS = get_person()
+    minute_index = [chr(i) for i in range(ord("A"), ord("Z") + 1)]
+    persons = get_person()
 
     chrome_options = Options()
     chrome_options.add_argument("--headless")
 
     driver = webdriver.Chrome(
         options=chrome_options, service=Service(ChromeDriverManager().install())
     )
 
     driver.get(url)
 
     WebDriverWait(driver, 10).until(
-        EC.presence_of_all_elements_located(
+        ec.presence_of_all_elements_located(
             (By.XPATH, '//*[@id="MeetingDetail"]/tbody/tr')
         )
     )
 
     body_name = driver.find_element(
         By.ID, "ContentPlaceHolder1_lblMeetingGroup"
     ).text  # body name
@@ -623,15 +623,15 @@
                 if (
                     driver.find_element(
                         By.XPATH,
                         '//*[@id="MeetingDetail"]/tbody/tr['
                         + str(i)
                         + "]/td[1]/strong",
                     ).text
-                )[0] in MINUTE_INDEX:
+                )[0] in minute_index:
                     if (
                         len(
                             driver.find_elements(
                                 By.XPATH,
                                 '//*[@id="MeetingDetail"]/tbody/tr['
                                 + str(i + 1)
                                 + "]/td[3]/span",
@@ -660,15 +660,15 @@
                 matter = driver.find_element(
                     By.XPATH, '//*[@id="MeetingDetail"]/tbody/tr[' + str(i) + "]/td[3]"
                 )
                 test = matter.find_element(By.CLASS_NAME, "ItemVoteResult").text
                 item = matter.find_element(By.CLASS_NAME, "AgendaOutlineLink").text
                 if len(item) != 0:
                     matter_model = parse_single_matter(
-                        driver, test, item, body_name, s_word_formated, PERSONS
+                        driver, test, item, body_name, s_word_formated, persons
                     )
                     event_minutes_items.append(matter_model)
             elif (
                 len(
                     driver.find_elements(
                         By.XPATH,
                         '//*[@id="MeetingDetail"]/tbody/tr[' + str(i) + "]/td[6]/span",
@@ -678,15 +678,15 @@
                 matter = driver.find_element(
                     By.XPATH, '//*[@id="MeetingDetail"]/tbody/tr[' + str(i) + "]/td[6]"
                 )
                 test = matter.find_element(By.CLASS_NAME, "ItemVoteResult").text
                 item = matter.find_element(By.CLASS_NAME, "AgendaOutlineLink").text
                 if len(item) != 0:
                     matter_model = parse_single_matter(
-                        driver, test, item, body_name, s_word_formated, PERSONS
+                        driver, test, item, body_name, s_word_formated, persons
                     )
                     event_minutes_items.append(matter_model)
             i += 1
         except (
             selenium.common.exceptions.NoSuchElementException,
             selenium.common.exceptions.TimeoutException,
         ):
@@ -721,25 +721,27 @@
         agenda_uri=agenda_uri,
         minutes_uri=minutes_uri,
     )
 
 
 def get_year(driver: "WebDriver", url: str, from_dt: datetime) -> str:
     """
-    Navigate to the year that we are looking for
+    Navigate to the year that we are looking for.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     driver:webdriver
         empty webdriver
     url:str
         the url of the calender page
+    from_dt:datetime
+        the datetime object for the search target year
 
-    Returns:
-    --------------
+    Returns
+    -------
     link:str
         the link to the calender of the year that we are looking for
     """
     from selenium.webdriver.common.by import By
 
     log.info("start get the current year's calender page")
     driver.get(url)
@@ -754,29 +756,29 @@
 def get_date(
     driver: "WebDriver",
     url: str,
     from_dt: datetime,
     to_dt: datetime,
 ) -> list:
     """
-    Get a list of ingestion models for the meetings hold during the selected time range
+    Get a list of ingestion models for the meetings hold during the selected time range.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     driver:webdriver
         empty webdriver
     url:str
         the url of the calender page
     from_dt:
         the begin date
-    to_date:
+    to_dt:
         the end date
 
-    Returns:
-    --------------
+    Returns
+    -------
     list
         all the ingestion models for the selected date range
     """
     from selenium.webdriver.common.by import By
 
     log.info("start calling parse_event for a signle meeting")
     driver.get(url)
@@ -799,25 +801,25 @@
     driver.quit()
     return events
 
 
 def get_events(from_dt: datetime, to_dt: datetime) -> list:
     """
     gets the right calender link
-    feed it to the function that get a list of ingestion models
+    feed it to the function that get a list of ingestion models.
 
-    Parameter:
-    ----------------
+    Parameters
+    ----------
     from_dt:
         the begin date
-    to_date:
+    to_dt:
         the end date
 
-    Returns:
-    --------------
+    Returns
+    -------
     list
         all the ingestion models for the selected date range
     """
     from selenium import webdriver
     from selenium.webdriver.chrome.options import Options
     from selenium.webdriver.chrome.service import Service
     from webdriver_manager.chrome import ChromeDriverManager
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/empty.py` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/empty.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 from datetime import datetime
-from typing import List
+from typing import Any, List
 
 from cdp_backend.pipeline.ingestion_models import EventIngestionModel
 
 ###############################################################################
 
 
 def get_events(
     from_dt: datetime,
     to_dt: datetime,
-    **kwargs,
+    **kwargs: Any,
 ) -> List[EventIngestionModel]:
     """
     Get all events for the provided timespan.
 
     Parameters
     ----------
     from_dt: datetime
         Datetime to start event gather from.
     to_dt: datetime
         Datetime to end event gather at.
+    kwargs: Any
+        Any keyword arguments to provide to downstream functions.
 
     Returns
     -------
     events: List[EventIngestionModel]
         All events gathered that occured in the provided time range.
 
     Notes
     -----
     As the implimenter of the get_events function, you can choose to ignore the from_dt
     and to_dt parameters. However, they are useful for manually kicking off pipelines
     from GitHub Actions UI.
     """
-
     # Your implementation here
     return []
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/houston.py` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/houston.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,66 +14,66 @@
 
 class HoustonScraper(IngestionModelScraper):
     def __init__(self):
         super().__init__(timezone="America/Chicago")
 
     def remove_extra_type(self, element: Union[Tag, NavigableString, None]) -> Tag:
         """
-        Remove types that are not useful
+        Remove types that are not useful.
 
-        Parameter:
-        ----------------
+        Parameters
+        ----------
         element: Union[Tag, NavigableString, None]
             The element in the page that we want to scrape
 
-        Returns:
-        ----------------
+        Returns
+        -------
         Tag
             Same elements as received, assuming the elements are not null
         """
         if isinstance(element, NavigableString) or element is None:
             raise ValueError(f"Wrong Type {type(element)}")
         return element
 
     def get_body_name(self, event: Union[Tag, NavigableString, None]) -> str:
         """
-        Get the body name for an event
+        Get the body name for an event.
 
-        Parameter:
-        ----------------
+        Parameters
+        ----------
         event: Union[Tag, NavigableString, None]
             All elements in the page that we want to scrape
 
-        Returns:
-        ----------------
+        Returns
+        -------
         str
             The body name
         """
         log.info("start get body name")
         event = self.remove_extra_type(event)
-        bodyTable = event.find_all("table")[1].find("table")
-        if "CITY COUNCIL" in bodyTable.text:
+        body_table = event.find_all("table")[1].find("table")
+        if "CITY COUNCIL" in body_table.text:
             return "City Council"
         else:
-            return bodyTable.find_all("span")[3].text.title()
+            return body_table.find_all("span")[3].text.title()
 
     def get_event_minutes_item(
         self,
         event: Union[Tag, NavigableString, None],
     ) -> List[ingestion_models.EventMinutesItem]:
         """
-        Parse the page and gather the event minute items
+        Parse the page and gather the event minute items.
 
-        Parameter:
-        ----------------
+        Parameters
+        ----------
         event: Union[Tag, NavigableString, None]
             All elements in the page that we want to scrape
 
-        Returns:
-        ----------------
+        Returns
+        -------
         List[ingestion_models.EventMinutesItem]
             All the event minute items gathered from the event on the page
         """
         log.info("start get items")
         event_minutes_items = []
         all_items = self.remove_extra_type(event).find_all("td", {"class": "style4"})
         for item in all_items:
@@ -97,57 +97,57 @@
 
     def get_diff_yearid(self, event_date: datetime) -> str:
         """
         Get the events in different years as the events for different
         years are stored in different tabs. Can get multiple events
         across years.
 
-        Parameters:
-        ---------------
+        Parameters
+        ----------
         event_date: datetime
             The date of the event we are trying to parse
 
-        Returns:
-        ---------------
+        Returns
+        -------
         str
             The year id that can locate the year tab where the event is stored
         """
         year = str(event_date.year)
         year_id = "city-council-" + year
         return year_id
 
     def get_date_mainlink(self, element: Tag) -> str:
         """
         Find the main link for one event.
 
-        Parameters:
-        --------------
+        Parameters
+        ----------
         element: Tag
             The element of one event
 
-        Returns:
-        --------------
+        Returns
+        -------
         str
             The main link for this event
         """
         link_post = element.find("a")["href"]
         link = f"https://houstontx.new.swagit.com/{link_post}"
         return link
 
     def get_agenda(self, element: Tag) -> Union[Tag, NavigableString, None]:
         """
-        Get event agenda for a specific details page
+        Get event agenda for a specific details page.
 
-        Parameters:
-        ----------------
+        Parameters
+        ----------
         element: Tag
             The element from which we want to get agenda
 
-        Returns:
-        ----------------
+        Returns
+        -------
         Tag
             The agenda web page we want parse
         """
         link = self.get_date_mainlink(element)
         agenda_link = link + "/agenda"
         page = requests.get(agenda_link)
         event = BeautifulSoup(page.content, "html.parser")
@@ -155,23 +155,25 @@
         return form1
 
     def get_event(
         self, date: str, element: Tag
     ) -> ingestion_models.EventIngestionModel:
         """
         Parse one event at a specific date. City council meeting information for
-        a specific date
+        a specific date.
 
-        Parameters:
-        --------------
-        date: the date of this meeting
-        element: the meeting Tag element
+        Parameters
+        ----------
+        date: str
+            the date of this meeting
+        element: Tag
+            the meeting Tag element
 
-        Returns:
-        --------------
+        Returns
+        -------
         ingestion_models.EventIngestionModel
             EventIngestionModel for one meeting date
         """
         log.info("start get one event")
         main_uri = self.get_date_mainlink(element)
         agenda = self.get_agenda(element)
         event = ingestion_models.EventIngestionModel(
@@ -188,34 +190,34 @@
         )
         return event
 
     def get_all_elements_in_range(
         self, time_from: datetime, time_to: datetime
     ) -> Dict[str, Tag]:
         """
-        Get all the meetings in a range of dates
+        Get all the meetings in a range of dates.
 
-        Parameters:
-        --------------
+        Parameters
+        ----------
         time_from: datetime
             Earliest meeting date to look at
         time_to: datetime
             Latest meeting date to look at
 
-        Returns:
-        --------------
+        Returns
+        -------
         Dict[str, Tag]
             Dictionary of mapping between the date of the meeting and the element for
             the meeting in that date
         """
         if time_from.year != time_to.year:
             raise ValueError(
                 "time_from and time_to are in different years, which is not supported"
             )
-        date_years = dict()
+        date_years = {}
         main_url = "https://houstontx.new.swagit.com/views/408"
         main_page = requests.get(main_url)
         main = BeautifulSoup(main_page.content, "html.parser")
         main_div = self.remove_extra_type(
             main.find("div", id=self.get_diff_yearid(time_from))
         )
         main_table = self.remove_extra_type(main_div.find("table", id="video-table"))
@@ -231,32 +233,32 @@
                 date_years[date] = year_elem
         return date_years
 
     def get_events(
         self, from_dt: datetime, to_dt: datetime
     ) -> List[ingestion_models.EventIngestionModel]:
         """
-        Get all city council meetings information within a specific time range
+        Get all city council meetings information within a specific time range.
 
-        Parameters:
-        --------------
+        Parameters
+        ----------
         from_dt: datetime
             The start date of the time range
         to_dt: datetime
             The end date of the time range
 
-        Returns:
-        --------------
+        Returns
+        -------
         list[ingestion_models.EventIngestionModel]
             A list of EventIngestionModel that contains all city council
             meetings information within a specific time range
         """
         events = []
         d = self.get_all_elements_in_range(from_dt, to_dt)
-        for date, element in d.items():
+        for date, _element in d.items():
             events.append(self.get_event(date, d[date]))
         return events
 
 
 def get_houston_events(
     from_dt: Optional[datetime] = None,
     to_dt: Optional[datetime] = None,
@@ -272,14 +274,16 @@
     ----------
     from_dt: datetime, optional
         The timespan beginning datetime to query for events after.
         Default is 2 days from UTC now
     to_dt: datetime, optional
         The timespan end datetime to query for events before.
         Default is UTC now
+    kwargs: Any
+        Any extra keyword arguments to pass to the get_events function.
 
     Returns
     -------
     events: List[EventIngestionModel]
 
     See Also
     --------
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/kingcounty-static.json` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/kingcounty-static.json`

 * *Files identical despite different names*

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/kingcounty.py` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/kingcounty.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import json
 import logging
 import re
 from pathlib import Path
 from typing import Dict
 from urllib.request import urlopen
@@ -27,17 +26,15 @@
 ###############################################################################
 
 
 class KingCountyScraper(LegistarScraper):
     PYTHON_MUNICIPALITY_SLUG: str = "king_county"
 
     def __init__(self):
-        """
-        King County specific implementation of LegistarScraper.
-        """
+        """King County specific implementation of LegistarScraper."""
         super().__init__(
             client="kingcounty",
             timezone="America/Los_Angeles",
             ignore_minutes_item_patterns=[
                 "This meeting also constitutes a meeting of the City Council",
                 "In-person attendance is currently prohibited",
                 "Times listed are estimated",
@@ -52,29 +49,31 @@
                 "SUBJECT TO A MOTION TO SUSPEND THE RULES TO TAKE ACTION WITHOUT REFERRAL TO COMMITTEE PURSUANT",  # noqa: E501
                 "If you do not have access to the ZOOM application",
                 "Executive Session: For 15 minutes, with action to follow",
                 "on the agenda for procedural matters",
                 "This is a mandatory referral to the",
                 "Watch King County TV Channel 22",
             ],
-            static_data=parse_static_file(STATIC_FILE_DEFAULT_PATH),
+            static_data=parse_static_file(
+                STATIC_FILE_DEFAULT_PATH, "America/Los_Angeles"
+            ),
             role_replacements={
                 "Boardmember": RoleTitle.MEMBER,
                 "Mr.": RoleTitle.MEMBER,
                 "Councilmemeber DELETE": RoleTitle.COUNCILMEMBER,
                 "Vice-Chair": RoleTitle.VICE_CHAIR,
                 "Council Member": RoleTitle.COUNCILMEMBER,
                 "Policy Chair": RoleTitle.CHAIR,
             },
         )
 
     @staticmethod
     def get_static_person_info() -> Dict[str, Person]:
         """
-        Scrape current council members information from kingcounty.gov
+        Scrape current council members information from kingcounty.gov.
 
         Returns
         -------
         persons: Dict[str, Person]
             keyed by name
 
         Notes
@@ -157,9 +156,9 @@
         """
         static_info_json = {STATIC_FILE_KEY_PERSONS: {}}
         for [name, person] in KingCountyScraper.get_static_person_info().items():
             # to allow for easy future addition of info other than Persons
             # save under top-level key "persons" in the file
             static_info_json[STATIC_FILE_KEY_PERSONS][name] = person.to_dict()
 
-        with open(file_path, "wt") as dump:
+        with open(file_path, "w") as dump:
             dump.write(json.dumps(static_info_json, indent=4))
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/lacity.py` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/lacity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import logging
 from datetime import datetime
 from typing import Any, List, Optional
 
 from cdp_backend.pipeline.ingestion_models import EventIngestionModel
 
@@ -16,17 +15,15 @@
 ###############################################################################
 
 
 class LosAngelesScraper(PrimeGovScraper):
     PYTHON_MUNICIPALITY_SLUG: str = "lacity"
 
     def __init__(self):
-        """
-        LA, CA specific implementation of PrimeGovScraper.
-        """
+        """LA, CA specific implementation of PrimeGovScraper."""
         super().__init__(
             client_id="lacity",
             timezone="America/Los_Angeles",
         )
 
 
 def get_lacity_events(
@@ -44,14 +41,16 @@
     ----------
     from_dt: datetime, optional
         The timespan beginning datetime to query for events after.
         Default is 2 days from UTC now
     to_dt: datetime, optional
         The timespan end datetime to query for events before.
         Default is UTC now
+    kwargs: Any
+        Any extra keyword arguments to pass to the get events function.
 
     Returns
     -------
     events: List[EventIngestionModel]
 
     See Also
     --------
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/portland-static.json` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/portland-static.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9759141156462586%*

 * *Differences: {"'persons'": "{'Dan Ryan': {'roles': {0: {'end_datetime': 1798704000}, 3: {'end_datetime': "*

 * *              "1798704000}, insert: [(4, OrderedDict([('title', 'Member'), ('start_datetime', "*

 * *              "1672560000), ('end_datetime', 1798704000), ('body', OrderedDict([('name', "*

 * *              "'Community and Civic Life')]))])), (5, OrderedDict([('title', 'Member'), "*

 * *              "('start_datetime', 1672560000), ('end_datetime', 1798704000), ('body', "*

 * *              "OrderedDict([('name', 'Equity and Huma […]*

```diff
@@ -57,15 +57,15 @@
             "is_active": true,
             "name": "Dan Ryan",
             "phone": "503-823-3589",
             "picture_uri": "https://www.portland.gov/sites/default/files/styles/4x5_320w/public/2021/katalina-berbari-2_0.jpg",
             "roles": [
                 {
                     "body": "City Council",
-                    "end_datetime": 1672473600,
+                    "end_datetime": 1798704000,
                     "start_datetime": 1599721200,
                     "title": "Councilmember"
                 },
                 {
                     "body": {
                         "name": "Development Services (BDS)"
                     },
@@ -81,17 +81,41 @@
                     "start_datetime": 1599721200,
                     "title": "Member"
                 },
                 {
                     "body": {
                         "name": "Children's Levy"
                     },
-                    "end_datetime": 1672473600,
+                    "end_datetime": 1798704000,
                     "start_datetime": 1599721200,
                     "title": "Member"
+                },
+                {
+                    "body": {
+                        "name": "Community and Civic Life"
+                    },
+                    "end_datetime": 1798704000,
+                    "start_datetime": 1672560000,
+                    "title": "Member"
+                },
+                {
+                    "body": {
+                        "name": "Equity and Human Rights"
+                    },
+                    "end_datetime": 1798704000,
+                    "start_datetime": 1672560000,
+                    "title": "Member"
+                },
+                {
+                    "body": {
+                        "name": "Parks & Recreation"
+                    },
+                    "end_datetime": 1798704000,
+                    "start_datetime": 1672560000,
+                    "title": "Member"
                 }
             ],
             "router_string": null,
             "seat": "Position 2",
             "website": "https://www.portland.gov/ryan"
         },
         "Jo Ann Hardesty": {
@@ -203,14 +227,31 @@
                     "title": "Member"
                 }
             ],
             "router_string": null,
             "seat": "Position 4",
             "website": "https://www.portland.gov/mapps"
         },
+        "Rene Gonzalez": {
+            "email": "gonzalezoffice@portlandoregon.gov",
+            "is_active": true,
+            "name": "Rene Gonzalez",
+            "phone": "503-823-4151",
+            "picture_uri": "https://www.portland.gov/sites/default/files/styles/4x5_320w/public/2022/rene-headshot-1cropped_0.jpg?itok=fIOTpP8t",
+            "roles": [
+                {
+                    "body": "City Council",
+                    "end_datetime": 1798704000,
+                    "start_datetime": 1672560000,
+                    "title": "Councilmember"
+                }
+            ],
+            "seat": "Position 3",
+            "website": "https://www.portland.gov/gonzalez"
+        },
         "Ted Wheeler": {
             "email": "wheelermediarequests@portlandoregon.gov",
             "external_source_id": null,
             "is_active": true,
             "name": "Ted Wheeler",
             "phone": "503-823-4120",
             "picture_uri": "https://www.portland.gov/sites/default/files/styles/4x5_320w/public/2020-03/mayor-wheeler-headshot-4x5-3-5-2020.jpg",
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/portland.py` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/portland.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+from __future__ import annotations
+
 import logging
 import re
 from datetime import datetime, timedelta
 from pathlib import Path
-from typing import Any, List, NamedTuple, Optional, Union
+from typing import Any, NamedTuple
 from urllib.error import HTTPError, URLError
 from urllib.request import Request, urlopen
 
 from bs4 import BeautifulSoup, Tag
 from cdp_backend.database.constants import (
     EventMinutesItemDecision,
     MatterStatusDecision,
@@ -33,15 +35,17 @@
 
 ###############################################################################
 
 log = logging.getLogger(__name__)
 
 ###############################################################################
 
-SCRAPER_STATIC_DATA = parse_static_file(Path(__file__).parent / "portland-static.json")
+SCRAPER_STATIC_DATA = parse_static_file(
+    Path(__file__).parent / "portland-static.json", "America/Los_Angeles"
+)
 
 ###############################################################################
 
 MATTER_ADOPTED_PATTERNS = [
     "accepted",
     "passed",
     "adopted",
@@ -65,20 +69,20 @@
 ]
 
 ###############################################################################
 
 
 class WebPageSoup(NamedTuple):
     status: bool
-    soup: Optional[BeautifulSoup] = None
+    soup: BeautifulSoup | None = None
 
 
-def load_web_page(url: Union[str, Request]) -> WebPageSoup:
+def load_web_page(url: str | Request) -> WebPageSoup:
     """
-    Load web page at url and return content soupified
+    Load web page at url and return content soupified.
 
     Parameters
     ----------
     url: str | urllib.request.Request
         Web page to load
 
     Returns
@@ -95,15 +99,15 @@
 
     return WebPageSoup(False)
 
 
 def make_efile_url(efile_page_url: str) -> str:
     """
     Helper function to get file download link
-    on a Portland EFile hosting web page
+    on a Portland EFile hosting web page.
 
     Parameters
     ----------
     efile_page_url: str
         URL to Portland efile hosting web page
         e.g. https://efiles.portlandoregon.gov/record/14803529
 
@@ -117,15 +121,15 @@
         efile_page_url += "/"
     return f"{efile_page_url}File/Document"
 
 
 def get_disposition(minute_section: Tag) -> str:
     """
     Return disposition string given within minute_section <div>
-    on the event web page
+    on the event web page.
 
     Parameters
     ----------
     minute_section: Tag
         <div> within event web page for a given event minute item
 
     Returns
@@ -139,17 +143,17 @@
     )
     result_status_element = result_status_element_sibling.next_sibling
     return result_status_element.text
 
 
 def disposition_to_minute_decision(
     disposition: str,
-) -> Optional[EventMinutesItemDecision]:
+) -> EventMinutesItemDecision | None:
     """
-    Decide EventMinutesItemDecision constant from event minute item disposition
+    Decide EventMinutesItemDecision constant from event minute item disposition.
 
     Parameters
     ----------
     disposition: str
         Disposition event web page for a given item
         e.g. Passed, Continued
 
@@ -165,15 +169,15 @@
         if re.search(pattern, disposition, re.I):
             return EventMinutesItemDecision.PASSED
     return None
 
 
 def separate_name_from_title(title_and_name: str) -> str:
     """
-    Return just name
+    Return just name.
 
     Parameters
     ----------
     title_and_name: str
         e.g. Mayor Ted Wheeler
 
     Returns
@@ -201,15 +205,15 @@
 
 class PortlandScraper(IngestionModelScraper):
     def __init__(self):
         super().__init__(timezone="America/Los_Angeles")
 
     def get_person(self, name: str) -> Person:
         """
-        Return matching Person from portland-static.json
+        Return matching Person from portland-static.json.
 
         Parameters
         ----------
         name: str
             Person full name
 
         Returns
@@ -287,31 +291,30 @@
                 + "-"
                 + agenda_name[agenda_name.index(",") + 2 : agenda_name.index(",") + 6]
             )
         return base_minute_section
 
     def get_matter(
         self, minute_section: Tag, event_page: BeautifulSoup
-    ) -> Optional[Matter]:
+    ) -> Matter | None:
         """
-        Make Matter from information in minute_section
+        Make Matter from information in minute_section.
 
         Parameters
         ----------
         minute_section: Tag
             <div> within event web page for a given event minute item
         event_page: BeautifulSoup
             The entire page where the event is found
 
         Returns
         -------
         matter: Optional[Matter]
             Matter if required information could be parsed from minute_section
         """
-
         # Find title
         title_div = minute_section.find("div", class_="council-document__title")
 
         matter_type = None
         matter_title = None
 
         if title_div is not None:
@@ -375,19 +378,17 @@
                 name=self.get_doc_number(minute_section, event_page),
                 sponsors=sponsor_list,
                 title=matter_title,
                 result_status=result_status,
             ),
         )
 
-    def get_supporting_files(
-        self, minute_section: Tag
-    ) -> Optional[List[SupportingFile]]:
+    def get_supporting_files(self, minute_section: Tag) -> list[SupportingFile] | None:
         """
-        Return SupportingFiles for a given EventMinutesItem
+        Return SupportingFiles for a given EventMinutesItem.
 
         Parameters
         ----------
         minute_section: Tag
             <div> within event web page for a given event minute item
 
         Returns
@@ -398,15 +399,15 @@
         -----
         Follow hyperlink to go to minutes item details page.
         On the details page look for directly-linked files
         and externally-hosted efiles.
 
         See Also
         --------
-        make_efile_url()
+        make_efile_url
         """
         try:
             # on the event page, event minute item titles are listed
             # in <div> with a particular class attribute.
             # so look for the minute_item_index-th such <div> on the event page
             div = minute_section.find(
                 "div", class_="field--label-hidden council-document__title"
@@ -418,15 +419,15 @@
             return None
 
         # load the mintues item details page that may have links to supporting files
         details_soup = load_web_page(details_url)
         if not details_soup.status:
             return None
 
-        supporting_files: List[SupportingFile] = []
+        supporting_files: list[SupportingFile] = []
         # first, try to get Documents and Exhibits and Impact Statement
         # these will contain links to files
         for div in details_soup.soup.find_all(
             "div",
             class_=re.compile(
                 "field field--label-above field--name-field-"
                 "((documents-and-exhibits)|(file-impact-statement)) field--type-file"
@@ -468,18 +469,18 @@
                 )
             ]
         )
 
         # remove any Nones
         return reduced_list(supporting_files)
 
-    def get_votes(self, minute_section: Tag) -> Optional[List[Vote]]:
+    def get_votes(self, minute_section: Tag) -> list[Vote] | None:
         """
         Look for 'Votes:' in minute_section and
-        create a Vote object for each line
+        create a Vote object for each line.
 
         Parameters
         ----------
         minute_section: Tag
             <div> within event web page for a given event minute item
 
         Returns
@@ -526,18 +527,18 @@
                 )
             )
 
         return reduced_list(vote_list)
 
     def get_event_minutes(
         self, event_page: BeautifulSoup
-    ) -> Optional[List[EventMinutesItem]]:
+    ) -> list[EventMinutesItem] | None:
         """
         Make EventMinutesItem from each relation--type-agenda-item <div>
-        on event_page
+        on event_page.
 
         Parameters
         ----------
         event_page: BeautifulSoup
             Web page for the meeting loaded as a bs4 object
 
         Returns
@@ -572,15 +573,15 @@
                         votes=self.get_votes(minute_section),
                     )
                 )
             )
 
         return reduced_list(event_minute_items)
 
-    def get_sessions(self, event_page: BeautifulSoup) -> Optional[List[Session]]:
+    def get_sessions(self, event_page: BeautifulSoup) -> list[Session] | None:
         """
         Parse meeting video URIs from event_page,
         return Session for each video found.
 
         Parameters
         ----------
         event_page: BeautifulSoup
@@ -595,15 +596,15 @@
         # including youtube video url for the session, if available
         # <div class="session-meta">
         # ...
         # <time class="datetime">Wednesday, December 15, 2021 9:30 am</time>
         # ...
         # <iframe src="https://www.youtube.com/...">
 
-        sessions: List[Session] = []
+        sessions: list[Session] = []
         session_index = 0
 
         for session_div in event_page.find_all("div", class_="session-meta"):
             session_time = session_div.find("time", class_="datetime")
             # plenty of sessions have no video listed so must check.
             # recall we require video_uri for a valid Session.
             video_iframe = session_div.find("iframe", src=re.compile(".*youtube.*"))
@@ -624,18 +625,18 @@
                     )
                 )
 
             session_index += 1
 
         return reduced_list(sessions)
 
-    def get_agenda_uri(self, event_page: BeautifulSoup) -> Optional[str]:
+    def get_agenda_uri(self, event_page: BeautifulSoup) -> str | None:
         """
         Find the uri for the file containing the agenda for a Portland, OR city
-        council meeting
+        council meeting.
 
         Parameters
         ----------
         event_page: BeautifulSoup
             Web page for the meeting loaded as a bs4 object
 
         Returns
@@ -653,17 +654,17 @@
             agenda_uri_element = parent_agenda_uri_element.find("a")
         else:
             return None
         if agenda_uri_element is not None:
             return f"https://www.portland.gov{agenda_uri_element['href']}"
         return None
 
-    def get_event(self, event_time: datetime) -> Optional[EventIngestionModel]:
+    def get_event(self, event_time: datetime) -> EventIngestionModel | None:
         """
-        Portland, OR city council meeting information for a specific date
+        Portland, OR city council meeting information for a specific date.
 
         Parameters
         ----------
         event_time: datetime
             Meeting date
 
         Returns
@@ -692,20 +693,20 @@
                 minutes_uri=None,
                 sessions=self.get_sessions(event_page.soup),
             ),
         )
 
     def get_events(
         self,
-        begin: Optional[datetime] = None,
-        end: Optional[datetime] = None,
-    ) -> List[EventIngestionModel]:
+        begin: datetime | None = None,
+        end: datetime | None = None,
+    ) -> list[EventIngestionModel]:
         """
         Portland, OR city council meeting information over given time span
-        as List[EventIngestionModel]
+        as List[EventIngestionModel].
 
         Parameters
         ----------
         begin: datetime, optional
             The timespan beginning datetime to query for events after.
             Default is 2 days from UTC now
         end: datetime, optional
@@ -733,32 +734,34 @@
             # prefer to return [] over None to backend pipeline
             # for easier iterate there
             collapse=False,
         )
 
 
 def get_portland_events(
-    from_dt: Optional[datetime] = None,
-    to_dt: Optional[datetime] = None,
+    from_dt: datetime | None = None,
+    to_dt: datetime | None = None,
     **kwargs: Any,
-) -> List[EventIngestionModel]:
+) -> list[EventIngestionModel]:
     """
     Public API for use in instances.__init__ so that this func can be attached
     as an attribute to cdp_scrapers.instances module.
     Thus the outside world like cdp-backend can get at this by asking for
     "get_portland_events".
 
     Parameters
     ----------
     from_dt: datetime, optional
         The timespan beginning datetime to query for events after.
         Default is 2 days from UTC now
     to_dt: datetime, optional
         The timespan end datetime to query for events before.
         Default is UTC now
+    kwargs: Any
+        Any extra keywords arguments to pass to the get events function.
 
     Returns
     -------
     events: List[EventIngestionModel]
 
     See Also
     --------
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/seattle-static.json` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/seattle-static.json`

 * *Files identical despite different names*

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/instances/seattle.py` & `cdp-scrapers-0.7.0/cdp_scrapers/instances/seattle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
+
+from __future__ import annotations
 
 import json
 import logging
 import re
 import warnings
 from datetime import datetime
 from pathlib import Path
-from typing import Dict, List, Optional
 from urllib.error import HTTPError, URLError
 from urllib.parse import parse_qs, quote_plus, urlsplit
 from urllib.request import urlopen
 
 import requests
 import urllib3
 from bs4 import BeautifulSoup
@@ -32,26 +32,24 @@
 ###############################################################################
 
 STATIC_FILE_KEY_PERSONS = "persons"
 STATIC_FILE_DEFAULT_PATH = Path(__file__).parent / "seattle-static.json"
 
 # we have discovered the city clerk accidentally entered Daniel Strauss
 # instead of the correct Dan Strauss for a few events
-PERSON_ALIASES = {"Dan Strauss": set(["Daniel Strauss"])}
+PERSON_ALIASES = {"Dan Strauss": {"Daniel Strauss"}}
 
 ###############################################################################
 
 
 class SeattleScraper(LegistarScraper):
     PYTHON_MUNICIPALITY_SLUG: str = "seattle"
 
     def __init__(self):
-        """
-        Seattle specific implementation of LegistarScraper.
-        """
+        """Seattle specific implementation of LegistarScraper."""
         super().__init__(
             client="seattle",
             timezone="America/Los_Angeles",
             ignore_minutes_item_patterns=[
                 "This meeting also constitutes a meeting of the City Council",
                 "In-person attendance is currently prohibited",
                 "Times listed are estimated",
@@ -63,15 +61,17 @@
                 "Items of Business",
                 # Common to see "CITY COUNCIL:",
                 # Or more generally "{body name}:"
                 # Check for last char ":"
                 r".+:$",
                 "Pursuant to Washington State",
             ],
-            static_data=parse_static_file(STATIC_FILE_DEFAULT_PATH),
+            static_data=parse_static_file(
+                STATIC_FILE_DEFAULT_PATH, "America/Los_Angeles"
+            ),
             person_aliases=PERSON_ALIASES,
         )
 
         # TODO: larger fix later
         #
         # try:
         #     urlopen("https://seattlechannel.org/")
@@ -81,17 +81,17 @@
         #     raise Exception(
         #         "seattlechannel.org may have fixed their SSL cert. "
         #         "Check and fix 'requests.get(*, verify=False)' calls"
         #     )
 
     def parse_content_uris(
         self, video_page_url: str, event_short_date: str
-    ) -> List[ContentURIs]:
+    ) -> list[ContentURIs]:
         """
-        Return URLs for videos and captions parsed from seattlechannel.org web page
+        Return URLs for videos and captions parsed from seattlechannel.org web page.
 
         Parameters
         ----------
         video_page_url: str
             URL to a web page for a particular meeting video
 
         event_short_date: str
@@ -100,15 +100,15 @@
         Returns
         -------
         content_uris: List[ContentURIs]
             List of ContentURIs objects for each session found.
 
         See Also
         --------
-        get_content_uris()
+        get_content_uris
         """
         with warnings.catch_warnings():
             warnings.simplefilter(
                 "ignore",
                 category=urllib3.exceptions.InsecureRequestWarning,
             )
             # now load the page to get the actual video url
@@ -196,18 +196,16 @@
                 r"file\:\s*\"([^\"]+)",
                 video_json_blob[captions_start:captions_end],
             )
         ]
 
         # use max count between videos and captions
         # so we don't lose any (e.g. caption = None if < # videos)
-        iter = range(max(len(video_uris), len(caption_uris)))
         list_uri = []
-
-        for i in iter:
+        for i in range(max(len(video_uris), len(caption_uris))):
             # just in case # videos != # captions
             try:
                 video_uri = video_uris[i]
             except IndexError:
                 video_uri = None
 
             try:
@@ -220,15 +218,15 @@
         if len(list_uri) == 0:
             log.debug(f"No video URI found on {video_page_url}")
         return list_uri
 
     @staticmethod
     def roman_to_int(roman: str):
         """
-        Roman numeral to an integer
+        Roman numeral to an integer.
 
         Parameters
         ----------
         roman: str
             Roman numeral string
 
         Returns
@@ -248,17 +246,17 @@
                 int_val += rom_val[roman[i]] - 2 * rom_val[roman[i - 1]]
             else:
                 int_val += rom_val[roman[i]]
         return int_val
 
     def get_video_page_urls(
         self, video_list_page_url: str, event_short_date: str
-    ) -> List[str]:
+    ) -> list[str]:
         """
-        Return URLs to web pages hosting videos for meetings from event_short_date
+        Return URLs to web pages hosting videos for meetings from event_short_date.
 
         Parameters
         ----------
         video_list_page_url: str
             URL to web page listing videos featuring the responsible group/body
             for the event described in legistar_ev.
             e.g. http://www.seattlechannel.org/BudgetCommittee?Mode2=Video
@@ -269,15 +267,15 @@
         Returns
         -------
         video_page_urls: List[str]
             web page URL per video
 
         See Also
         --------
-        get_content_uris()
+        get_content_uris
         """
         with warnings.catch_warnings():
             warnings.simplefilter(
                 "ignore",
                 category=urllib3.exceptions.InsecureRequestWarning,
             )
             # request list of videos for this group on this event's date
@@ -301,26 +299,23 @@
         #                     <div class="videoDate">10/14/2021</div>
         #         </div>
         #         <div class="titleExcerptText"><p><em>Pursuant to Washington ... </div>
         #     </div>
         # </div>
         #    <div class="row borderBottomNone paginationItem">
 
-        session_video_page_urls: Dict[int, str] = {}
+        session_video_page_urls: dict[int, str] = {}
 
         # want <a> tag in the <div> with
         # title attribute that contains the event date,
         # onclick attribute that calls loadJWPlayer,
         # href attribute that contains videoid
 
         soup = BeautifulSoup(response, "html.parser")
-        for link in soup.find(
-            "div",
-            class_="paginationContainer",
-        ).find_all(
+        for link in soup.find("div", class_="paginationContainer",).find_all(
             "a",
             href=re.compile("videoid"),
             onclick=re.compile("loadJWPlayer"),
             title=re.compile(event_short_date),
         ):
             # e.g. "Session I m/d/yy"
             match = re.search(
@@ -344,31 +339,31 @@
 
         # ordered by session number
         return [
             session_video_page_urls[session]
             for session in sorted(session_video_page_urls.keys())
         ]
 
-    def get_content_uris(self, legistar_ev: Dict) -> List[ContentURIs]:
+    def get_content_uris(self, legistar_ev: dict) -> list[ContentURIs]:
         """
-        Return URLs for videos and captions parsed from seattlechannel.org web page
+        Return URLs for videos and captions parsed from seattlechannel.org web page.
 
         Parameters
         ----------
         legistar_ev: Dict
             Data for one Legistar Event.
 
         Returns
         -------
         content_uris: List[ContentURIs]
             List of ContentURIs objects for each session found.
 
         See Also
         --------
-        parse_content_uris()
+        parse_content_uris
 
         Notes
         -----
         get_events() calls get_content_uris() to get video and caption URIs.
         get_content_uris() gets video page URL from EventInSiteURL.
         If "videoid" in video page URL, calls parse_content_uris().
         Else, calls get_video_page_urls() to get proper video page URL with "videoid",
@@ -432,17 +427,17 @@
             # 1 web page per session video for this multi-session event
             for page_url in self.get_video_page_urls(video_page_url, event_short_date)
             # video and caption urls on the session video web page
             for uris in self.parse_content_uris(page_url, event_short_date)
         ]
 
     @staticmethod
-    def get_person_picture_url(person_www: str) -> Optional[str]:
+    def get_person_picture_url(person_www: str) -> str | None:
         """
-        Parse person_www and return banner image used on the web page
+        Parse person_www and return banner image used on the web page.
 
         Parameters
         ----------
         person_www: str
             e.g. http://www.seattle.gov/council/pedersen
 
         Returns
@@ -473,31 +468,31 @@
             ).group(1)
         except AttributeError:
             pass
 
         return None
 
     @staticmethod
-    def get_static_person_info() -> Optional[List[Person]]:
+    def get_static_person_info() -> list[Person] | None:  # noqa: C901
         """
-        Return partial Persons with static long-term information
+        Return partial Persons with static long-term information.
 
         Returns
         -------
         persons: Optional[List[Person]]
         """
         try:
             # has table with all council members
             with urlopen("https://seattle.legistar.com/MainBody.aspx") as resp:
                 soup = BeautifulSoup(resp.read(), "html.parser")
         except URLError or HTTPError:
             log.debug("Failed to open https://seattle.legistar.com/MainBody.aspx")
             return None
 
-        static_person_info: List[Person] = []
+        static_person_info: list[Person] = []
 
         # <tr id="ctl00_ContentPlaceHolder1_gridPeople_ctl00__0" ...>
         #     <td class="rgSorted" style="white-space:nowrap;">
         #         <a ...>Alex Pedersen</a>
         #     </td>
         #     <td>Councilmember<br /><em>Council Position No. 4</em></td>
         #     <td>1/1/2020</td>
@@ -589,36 +584,36 @@
             )
 
         return static_person_info
 
     @staticmethod
     def dump_static_info(file_path: str) -> bool:
         """
-        Save static data in json format
+        Save static data in json format.
 
         Parameters
         ----------
         file_path: str
             Static data dump file path
 
         Returns
         -------
         bool
             True if some data was saved in file_path
 
         See Also
         --------
-        LegistarScraper.inject_known_data()
+        LegistarScraper.inject_known_data
         """
         static_person_info = {}
         for person in SeattleScraper.get_static_person_info():
             # save this Person in json keyed by the name
             static_person_info[person.name] = json.loads(person.to_json())
 
         if not static_person_info:
             return False
 
-        with open(file_path, "wt") as dump:
+        with open(file_path, "w") as dump:
             dump.write(
                 json.dumps({STATIC_FILE_KEY_PERSONS: static_person_info}, indent=4)
             )
         return True
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/legistar_content_parsers.py` & `cdp-scrapers-0.7.0/cdp_scrapers/legistar_content_parsers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import re
 from typing import List, Optional
 from urllib.parse import unquote
 from urllib.request import urlopen
 
 from bs4 import BeautifulSoup
@@ -11,21 +10,21 @@
 
 from .scraper_utils import str_simplified
 from .types import ContentURIs, LegistarContentParser
 
 
 def _parse_format_1(client: str, soup: BeautifulSoup) -> Optional[List[ContentURIs]]:
     """
-    Works for milwaukee, kingcounty, phoenix
+    Works for milwaukee, kingcounty, phoenix.
 
     Parameters
     ----------
     client: str
         Which legistar client to target. Ex: "seattle"
-    video web page: BeautifulSoup
+    soup: BeautifulSoup
         Video web page loaded into bs4
 
     Returns
     -------
     uris: Optional[List[ContentURIs]]
         URIs for video and optional caption
 
@@ -48,34 +47,34 @@
     if video_script_text is None:
         return None
 
     video_script_text = video_script_text.string
     # Below two lines of code tries to extract video url from downLoadLinks variable
     # "http:\/\/archive-media.granicus.com:443\/OnDemand\/king\/king_e560cf63-5570-416e-a47d-0e1e13652224.mp4"
     try:
-        downloadLinks = video_script_text.split("[[")[1]
-        video_url = downloadLinks.split('",')[1].strip('"')
+        download_links = video_script_text.split("[[")[1]
+        video_url = download_links.split('",')[1].strip('"')
     except IndexError:
         # split() did not yield expected # items
         return None
     # Cleans up the video url to remove backward slash(\)
     video_uri = video_url.replace("\\", "")
     # caption URIs are not found for kingcounty events.
     return [ContentURIs(video_uri=video_uri, caption_uri=None)]
 
 
 def _parse_format_2(client: str, soup: BeautifulSoup) -> Optional[List[ContentURIs]]:
     """
-    Works for denver
+    Works for denver.
 
     Parameters
     ----------
     client: str
         Which legistar client to target. Ex: "seattle"
-    video web page: BeautifulSoup
+    soup: BeautifulSoup
         Video web page loaded into bs4
 
     Returns
     -------
     uris: Optional[List[ContentURIs]]
         URIs for video and optional caption
 
@@ -90,21 +89,21 @@
     if video_url is None:
         return None
     return [ContentURIs(str_simplified(video_url.a["href"]))]
 
 
 def _parse_format_3(client: str, soup: BeautifulSoup) -> Optional[List[ContentURIs]]:
     """
-    Works for boston, corpuschristi, elpasotexas
+    Works for boston, corpuschristi, elpasotexas.
 
     Parameters
     ----------
     client: str
         Which legistar client to target. Ex: "seattle"
-    video web page: BeautifulSoup
+    soup: BeautifulSoup
         Video web page loaded into bs4
 
     Returns
     -------
     uris: Optional[List[ContentURIs]]
         URIs for video and optional caption
 
@@ -139,21 +138,21 @@
             ),
         )
     ]
 
 
 def _parse_format_4(client: str, soup: BeautifulSoup) -> Optional[List[ContentURIs]]:
     """
-    Works for longbeach, richmondva
+    Works for longbeach, richmondva.
 
     Parameters
     ----------
     client: str
         Which legistar client to target. Ex: "seattle"
-    video web page: BeautifulSoup
+    soup: BeautifulSoup
         Video web page loaded into bs4
 
     Returns
     -------
     uris: Optional[List[ContentURIs]]
         URIs for video and optional caption
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/legistar_utils.py` & `cdp-scrapers-0.7.0/cdp_scrapers/legistar_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
+
+from __future__ import annotations
 
 import enum
 import logging
 import re
 from copy import deepcopy
 from datetime import datetime, timedelta
 from json import JSONDecodeError
-from typing import Any, Dict, List, NamedTuple, Optional, Set
+from typing import Any, NamedTuple
 from urllib.error import HTTPError, URLError
-from urllib.parse import quote_plus
+from urllib.parse import quote_plus, urlsplit
 from urllib.request import urlopen
 
 import requests
 from bs4 import BeautifulSoup
 from cdp_backend.database.constants import (
     EventMinutesItemDecision,
     MatterStatusDecision,
@@ -108,25 +109,25 @@
 LEGISTAR_EV_EXT_ID = "EventId"
 LEGISTAR_EV_BODY = "EventBodyInfo"
 
 LEGISTAR_DATETIME_FORMAT = "%Y-%m-%dT%H:%M:%S"
 ###############################################################################
 
 
-known_legistar_persons: Dict[int, Dict[str, Any]] = {}
-known_legistar_bodies: Dict[int, Dict[str, Any]] = {}
+known_legistar_persons: dict[int, dict[str, Any]] = {}
+known_legistar_bodies: dict[int, dict[str, Any]] = {}
 # video web page parser type per municipality
-video_page_parser: Dict[str, LegistarContentParser] = {}
+video_page_parser: dict[str, LegistarContentParser] = {}
 
 
 def get_legistar_body(
     client: str,
     body_id: int,
     use_cache: bool = False,
-) -> Optional[Dict[str, Any]]:
+) -> dict[str, Any] | None:
     """
     Return information for a single legistar body in JSON.
 
     Parameters
     ----------
     client: str
         Which legistar client to target. Ex: "seattle"
@@ -171,15 +172,15 @@
     return body
 
 
 def get_legistar_person(
     client: str,
     person_id: int,
     use_cache: bool = False,
-) -> Optional[Dict[str, Any]]:
+) -> dict[str, Any] | None:
     """
     Return information for a single legistar person in JSON.
 
     Parameters
     ----------
     client: str
         Which legistar client to target. Ex: "seattle"
@@ -231,32 +232,32 @@
 
     if response.status_code != 200:
         person[LEGISTAR_PERSON_ROLES] = None
         if use_cache:
             known_legistar_persons[person_id] = person
         return person
 
-    office_records: List[Dict[str, Any]] = response.json()
+    office_records: list[dict[str, Any]] = response.json()
     for record in office_records:
         # body for this role
         record[LEGISTAR_ROLE_BODY] = get_legistar_body(
             client=client, body_id=record["OfficeRecordBodyId"], use_cache=use_cache
         )
 
     person[LEGISTAR_PERSON_ROLES] = office_records
     if use_cache:
         known_legistar_persons[person_id] = person
     return person
 
 
 def get_legistar_events_for_timespan(
     client: str,
-    begin: Optional[datetime] = None,
-    end: Optional[datetime] = None,
-) -> List[Dict]:
+    begin: datetime | None = None,
+    end: datetime | None = None,
+) -> list[dict]:
     """
     Get all legistar events and each events minutes items, people, and votes, for a
     client for a given timespan.
 
     Parameters
     ----------
     client: str
@@ -378,30 +379,32 @@
 
     log.debug(f"Collected {len(response)} Legistar events")
     return response
 
 
 class ContentUriScrapeResult(NamedTuple):
     class Status(enum.IntEnum):
+        """Status of content parsing."""
+
         # Web page(s) are in unrecognized structure
         UnrecognizedPatternError = -1
         # Error in accessing some resource
         ResourceAccessError = -2
         # Video was not provided for the event
         ContentNotProvidedError = -3
         # Found URIs to video and optional caption
         Ok = 0
 
     status: Status
-    uris: Optional[List[ContentURIs]] = None
+    uris: list[ContentURIs] | None = None
 
 
-def parse_video_page_url(video_page_url: str, client: str) -> List[ContentURIs]:
+def parse_video_page_url(video_page_url: str, client: str) -> list[ContentURIs]:
     """
-    Return URLs for videos and captions from a Legistar/Granicus-hosted video web page
+    Return URLs for videos and captions from a Legistar/Granicus-hosted video web page.
 
     Parameters
     ----------
     video_page_url: str
         The URL for the page of the legistar video
     client: str
         Which legistar client to target. Ex: "seattle"
@@ -428,17 +431,17 @@
                     break
             else:
                 uris = None
 
     return uris
 
 
-def get_legistar_content_uris(client: str, legistar_ev: Dict) -> ContentUriScrapeResult:
+def get_legistar_content_uris(client: str, legistar_ev: dict) -> ContentUriScrapeResult:
     """
-    Return URLs for videos and captions from a Legistar/Granicus-hosted video web page
+    Return URLs for videos and captions from a Legistar/Granicus-hosted video web page.
 
     Parameters
     ----------
     client: str
         Which legistar client to target. Ex: "seattle"
     legistar_ev: Dict
         Data for one Legistar Event.
@@ -452,18 +455,20 @@
             URIs for video and optional caption
 
     Raises
     ------
     NotImplementedError
         Means the content structure of the web page hosting session video has changed.
         We need explicit review and update the scraping code.
+    ConnectionError
+        When the Legistar site (e.g. *.legistar.com) itself may be down.
 
     See Also
     --------
-    LegistarScraper.get_content_uris()
+    LegistarScraper.get_content_uris
     cdp_scrapers.legistar_content_parsers
     """
     global video_page_parser
 
     # prefer video file path in legistar Event.EventVideoPath
     if legistar_ev[LEGISTAR_SESSION_VIDEO_URI]:
         return (
@@ -482,14 +487,24 @@
         # a td tag with a certain id pattern.
         # this is usually something like
         # https://somewhere.legistar.com/MeetingDetail.aspx...
         # that is a summary-like page for a meeting
         with urlopen(legistar_ev[LEGISTAR_EV_SITE_URL]) as resp:
             soup = BeautifulSoup(resp.read(), "html.parser")
 
+            if "server error" in soup.text.lower():
+                try:
+                    url_attrs = urlsplit(legistar_ev[LEGISTAR_EV_SITE_URL])
+                    netloc = url_attrs.netloc
+                except ValueError:
+                    netloc = legistar_ev[LEGISTAR_EV_SITE_URL]
+                raise ConnectionError(
+                    f"{netloc} appears to be down: {str_simplified(soup.text)}"
+                )
+
     except (URLError, HTTPError) as e:
         log.debug(f"{legistar_ev[LEGISTAR_EV_SITE_URL]}: {str(e)}")
         return (ContentUriScrapeResult.Status.ResourceAccessError, None)
 
     # this gets us the url for the web PAGE containing the video
     # video link is provided in the window.open()command inside onclick event
     # <a id="ctl00_ContentPlaceHolder1_hypVideo"
@@ -530,15 +545,15 @@
             "get_legistar_content_uris() needs attention. "
             f"Unrecognized video web page HTML structure: {video_page_url}"
         )
     return (ContentUriScrapeResult.Status.Ok, uris)
 
 
 class LegistarScraper(IngestionModelScraper):
-    """
+    r"""
     Base class for transforming Legistar API data to CDP IngestionModel.
 
     If get_events() naively fails and raises an error, a given installation must define
     a derived class and implement the get_content_uris() function.
 
     Parameters
     ----------
@@ -609,41 +624,44 @@
         CDP standard role.
         Default: None
 
     See Also
     --------
     cdp_scrapers.legistar_utils.LegistarScraper.get_content_uris
     cdp_scrapers.instances.seattle.SeattleScraper
-    """  # noqa: W605
+    """
 
     def __init__(
         self,
         client: str,
         timezone: str,
-        ignore_minutes_item_patterns: List[str] = [],
+        ignore_minutes_item_patterns: list[str] | None = None,
         vote_approve_pattern: str = r"approve|favor|yes",
         vote_abstain_pattern: str = r"abstain|refuse|refrain",
         vote_reject_pattern: str = r"reject|oppose|no",
         vote_absent_pattern: str = r"absent",
         vote_nonvoting_pattern: str = r"nv|(?:non.*voting)",
         matter_adopted_pattern: str = (
             r"approved|confirmed|passed|adopted|consent|(?:voted.*com+it+ee)"
         ),
         matter_in_progress_pattern: str = r"heard|read|filed|held|(?:in.*com+it+ee)",
         matter_rejected_pattern: str = r"rejected|dropped",
         minutes_item_decision_passed_pattern: str = r"pass",
         minutes_item_decision_failed_pattern: str = r"not|fail",
-        static_data: Optional[ScraperStaticData] = None,
-        person_aliases: Optional[Dict[str, Set[str]]] = None,
-        role_replacements: Optional[Dict[str, str]] = None,
+        static_data: ScraperStaticData | None = None,
+        person_aliases: dict[str, set[str]] | None = None,
+        role_replacements: dict[str, str] | None = None,
     ):
         super().__init__(timezone=timezone, person_aliases=person_aliases)
 
+        if ignore_minutes_item_patterns is None:
+            ignore_minutes_item_patterns = []
+
         self.client_name: str = client
-        self.ignore_minutes_item_patterns: List[str] = ignore_minutes_item_patterns
+        self.ignore_minutes_item_patterns: list[str] = ignore_minutes_item_patterns
 
         # regex patterns used to infer cdp_backend.database.constants
         # from Legistar string fields
         self.vote_approve_pattern: str = vote_approve_pattern
         self.vote_abstain_pattern: str = vote_abstain_pattern
         self.vote_reject_pattern: str = vote_reject_pattern
         # TODO: need to debug these using real examples
@@ -660,15 +678,15 @@
         self.minutes_item_decision_failed_pattern: str = (
             minutes_item_decision_failed_pattern
         )
 
         self.static_data = static_data
         self.role_replacements = role_replacements or {}
 
-    def get_matter_status(self, legistar_matter_status: str) -> Optional[str]:
+    def get_matter_status(self, legistar_matter_status: str) -> str | None:
         """
         Return appropriate MatterStatusDecision constant from EventItemMatterStatus.
 
         Parameters
         ----------
         legistar_matter_status: str
             Legistar API EventItemMatterStatus.
@@ -720,15 +738,15 @@
 
         log.debug(f"no MatterStatusDecision filter for {legistar_matter_status}")
         return None
 
     def get_minutes_item_decision(
         self,
         legistar_item_passed_name: str,
-    ) -> Optional[str]:
+    ) -> str | None:
         """
         Return appropriate EventMinutesItemDecision constant from
         EventItemPassedFlagName.
 
         Parameters
         ----------
         legistar_item_passed_name: str
@@ -767,15 +785,15 @@
             is not None
         ):
             return EventMinutesItemDecision.FAILED
 
         log.debug(f"no EventMinutesItemDecision filter for {legistar_item_passed_name}")
         return None
 
-    def get_vote_decision(self, legistar_vote: Dict) -> Optional[str]:
+    def get_vote_decision(self, legistar_vote: dict) -> str | None:  # noqa: C901
         """
         Return appropriate VoteDecision constant based on Legistar Vote.
 
         Parameters
         ----------
         legistar_vote: Dict
             Legistar API Vote
@@ -861,15 +879,15 @@
             elif nonvoting:
                 return VoteDecision.ABSTAIN_NON_VOTING
 
         if not decision:
             log.debug(f"no VoteDecision filter for {vote_value}")
         return decision
 
-    def get_body(self, legistar_body: Dict[str, Any]) -> Optional[Body]:
+    def get_body(self, legistar_body: dict[str, Any]) -> Body | None:
         """
         Return CDP Body for Legistar body.
 
         Parameters
         ----------
         legistar_body: Dict
             Legistar API body
@@ -878,15 +896,15 @@
         -------
         body: Optional[body]
             The Legistar body converted to a CDP body ingestion model.
             None if missing required information.
 
         See Also
         --------
-        get_legistar_body()
+        get_legistar_body
         """
         if not legistar_body:
             return None
 
         return self.get_none_if_empty(
             Body(
                 external_source_id=str(legistar_body[LEGISTAR_BODY_EXT_ID]),
@@ -915,18 +933,18 @@
         """
         if role_title in self.role_replacements:
             return self.role_replacements[role_title]
 
         return role_title
 
     def get_roles(
-        self, legistar_office_records: List[Dict[str, Any]]
-    ) -> Optional[List[Role]]:
+        self, legistar_office_records: list[dict[str, Any]]
+    ) -> list[Role] | None:
         """
-        Return list of CDP Role from list of legistar OfficeRecord
+        Return list of CDP Role from list of legistar OfficeRecord.
 
         Parameters
         ----------
         legistar_office_records: List[Dict]
             Legistar API OfficeRecords
 
         Returns
@@ -968,15 +986,15 @@
                         ),
                     )
                 )
                 for record in legistar_office_records
             ]
         )
 
-    def resolve_person_alias(self, person: Person) -> Optional[Person]:
+    def resolve_person_alias(self, person: Person) -> Person | None:
         """
         If input person is in fact an alias of a reference known person,
         return the reference person instead.
         Else return person as-is.
 
         Parameters
         ----------
@@ -1002,21 +1020,21 @@
 
         for name, aliases in self.person_aliases.items():
             if person.name in aliases:
                 # found the reference person with input person.name as an alias
                 try:
                     # query to get PersonId for the reference person we want to use
                     # in place of the input person
-                    response: List[Dict[str, Any]] = requests.get(
+                    response: list[dict[str, Any]] = requests.get(
                         request_format.format(
                             client=self.client_name, name=quote_plus(name)
                         ),
                     ).json()
                 except JSONDecodeError:
-                    response: List[Dict[str, Any]] = []
+                    response: list[dict[str, Any]] = []
 
                 if len(response) == 0 or LEGISTAR_PERSON_EXT_ID not in response[0]:
                     log.error(
                         f"Found {person.name}, an alias of {name} "
                         f"but failed get valid JSON for {name} from Legistar API. "
                         f"Keeping this alias {person.name} without resolving."
                     )
@@ -1029,15 +1047,15 @@
                         use_cache=True,
                     )
                 )
 
         # input person is not an alias of a reference Person
         return person
 
-    def get_person(self, legistar_person: Dict) -> Optional[Person]:
+    def get_person(self, legistar_person: dict) -> Person | None:
         """
         Return CDP Person for Legistar Person.
 
         Parameters
         ----------
         legistar_person: Dict
             Legistar API Person
@@ -1046,15 +1064,15 @@
         -------
         person: Optional[Person]
             The Legistar Person converted to a CDP person ingestion model.
             None if missing information.
 
         See Also
         --------
-        get_legistar_person()
+        get_legistar_person
         """
         if (
             not legistar_person
             or not legistar_person[LEGISTAR_PERSON_NAME]
             # have seen PersonFullName with something like "no sponsor required"
             or re.search("no.*required", legistar_person[LEGISTAR_PERSON_NAME], re.I)
         ):
@@ -1076,15 +1094,15 @@
                     phone=phone,
                     website=str_simplified(legistar_person[LEGISTAR_PERSON_WEBSITE]),
                     is_active=bool(legistar_person[LEGISTAR_PERSON_ACTIVE]),
                 )
             )
         )
 
-    def get_votes(self, legistar_votes: List[Dict]) -> Optional[List[Vote]]:
+    def get_votes(self, legistar_votes: list[dict]) -> list[Vote] | None:
         """
         Return List[Vote] for Legistar API Votes.
 
         Parameters
         ----------
         legistar_votes: List[Dict]
             Legistar votes as CDP Vote ingestion models.
@@ -1106,16 +1124,16 @@
                 )
                 for vote in legistar_votes
             ]
         )
 
     def get_event_supporting_files(
         self,
-        legistar_ev_attachments: List[Dict],
-    ) -> Optional[List[SupportingFile]]:
+        legistar_ev_attachments: list[dict],
+    ) -> list[SupportingFile] | None:
         """
         Return List[SupportingFile] for Legistar API MatterAttachments.
 
         Parameters
         ----------
         legistar_ev_attachments: List[Dict]
             Legistar API MatterAttachments
@@ -1135,26 +1153,27 @@
                         uri=str_simplified(attachment[LEGISTAR_FILE_URI]),
                     )
                 )
                 for attachment in legistar_ev_attachments
             ]
         )
 
-    def get_sponsors(self, legistar_sponsors: List[Dict]) -> Optional[List[Person]]:
+    def get_sponsors(self, legistar_sponsors: list[dict]) -> list[Person] | None:
+        """Get legislation sponsors."""
         if not legistar_sponsors:
             return None
 
         return reduced_list(
             [
                 self.get_person(sponsor["SponsorPersonInfo"])
                 for sponsor in legistar_sponsors
             ]
         )
 
-    def get_matter(self, legistar_ev: Dict) -> Optional[Matter]:
+    def get_matter(self, legistar_ev: dict) -> Matter | None:
         """
         Return Matter from Legistar API EventItem.
 
         Parameters
         ----------
         legistar_ev: Dict
             Legistar API EventItem
@@ -1177,39 +1196,38 @@
                 title=str_simplified(legistar_ev[LEGISTAR_MATTER_TITLE]),
                 result_status=self.get_matter_status(
                     legistar_ev[LEGISTAR_MATTER_STATUS]
                 ),
             )
         )
 
-    def get_minutes_item(self, legistar_ev_item: Dict) -> Optional[MinutesItem]:
+    def get_minutes_item(self, legistar_ev_item: dict) -> MinutesItem | None:
         """
         Return MinutesItem from parts of Legistar API EventItem.
 
         Parameters
         ----------
         legistar_ev_item: Dict
             Legistar API EventItem
 
         Returns
         -------
         minutes_item: Optional[MinutesItem]
             None if could not get nonempty MinutesItem.name from EventItem.
         """
-
         return self.get_none_if_empty(
             MinutesItem(
                 external_source_id=str(legistar_ev_item[LEGISTAR_MINUTE_EXT_ID]),
                 name=str_simplified(legistar_ev_item[LEGISTAR_MINUTE_NAME]),
             )
         )
 
     def fix_event_minutes(
-        self, ev_minutes_item: Optional[EventMinutesItem], legistar_ev_item: Dict
-    ) -> Optional[EventMinutesItem]:
+        self, ev_minutes_item: EventMinutesItem | None, legistar_ev_item: dict
+    ) -> EventMinutesItem | None:
         """
         Inspect the MinutesItem and Matter in ev_minutes_item.
         - Move some fields between them to make the information more meaningful.
         - Enforce matter.result_status when appropriate.
 
         Parameters
         ----------
@@ -1248,38 +1266,39 @@
                 #       is incomplete or malformed
                 ev_minutes_item.matter.result_status = MatterStatusDecision.IN_PROGRESS
 
         return ev_minutes_item
 
     def filter_event_minutes(
         self, ev_minutes_item: EventMinutesItem
-    ) -> Optional[EventMinutesItem]:
+    ) -> EventMinutesItem | None:
         """
         Return None if minutes_item.name contains unimportant text
-        that we want to ignore
+        that we want to ignore.
 
         Parameters
         ----------
         ev_minutes_item: EventMinutesItem
+            The minutes item to filter.
 
         Returns
         -------
         filtered_event_minutes_items: Optional[EventMinutesItem]
             The allowed minutes item or None is filtered out.
         """
         if not ev_minutes_item.minutes_item or not ev_minutes_item.minutes_item.name:
             return ev_minutes_item
-        for filter in self.ignore_minutes_item_patterns:
-            if re.search(filter, ev_minutes_item.minutes_item.name, re.IGNORECASE):
+        for filter_ in self.ignore_minutes_item_patterns:
+            if re.search(filter_, ev_minutes_item.minutes_item.name, re.IGNORECASE):
                 return None
         return ev_minutes_item
 
     def get_event_minutes(
-        self, legistar_ev_items: List[Dict]
-    ) -> Optional[List[EventMinutesItem]]:
+        self, legistar_ev_items: list[dict]
+    ) -> list[EventMinutesItem] | None:
         """
         Return List[EventMinutesItem] for Legistar API EventItems.
 
         Parameters
         ----------
         legistar_ev_items: List[Dict]
             Legistar API EventItems
@@ -1314,17 +1333,17 @@
                 )
                 # EventMinutesItem object per member in EventItems
                 for item in legistar_ev_items
             ]
         )
 
     @staticmethod
-    def date_and_time_to_datetime(ev_date: str, ev_time: Optional[str]) -> datetime:
+    def date_and_time_to_datetime(ev_date: str, ev_time: str | None) -> datetime:
         """
-        Return datetime from ev_date and ev_time
+        Return datetime from ev_date and ev_time.
 
         Parameters
         ----------
         ev_date: str
             Formatted as "%Y-%m-%dT%H:%M:%S"
         ev_time: Optional[str]
             Formatted as "%I:%M %p"
@@ -1355,15 +1374,15 @@
                 month=d.month,
                 day=d.day,
                 hour=0,
                 minute=0,
                 second=0,
             )
 
-    def get_content_uris(self, legistar_ev: Dict) -> List[ContentURIs]:
+    def get_content_uris(self, legistar_ev: dict) -> list[ContentURIs]:
         """
         Must implement in class derived from LegistarScraper.
         If Legistar Event.EventVideoPath is used, return an empty list in the override.
 
         Parameters
         ----------
         legistar_ev: Dict
@@ -1390,30 +1409,30 @@
 
         raise NotImplementedError(
             f"Please provide get_content_uris() for {self.client_name}"
         )
 
     def inject_known_person(self, person: Person) -> Person:
         """
-        Inject information if person exists in static_data.persons
+        Inject information if person exists in static_data.persons.
 
         Parameters
         ----------
         person: Person
             Person into which to inject data from static_data
 
         Returns
         -------
         Person
             Input person updated with information from static_data,
             and seat.roles sanitized.
 
         See Also
         --------
-        scraper_utils.sanitize_roles()
+        scraper_utils.sanitize_roles
         """
         try:
             known_person = self.static_data.persons[person.name]
         except (AttributeError, KeyError):
             return person
 
         for attr in person.__dataclass_fields__.keys():
@@ -1436,19 +1455,19 @@
                 ),
                 static_data=self.static_data,
             )
 
         return person
 
     def inject_known_data(
-        self, events: List[EventIngestionModel]
-    ) -> List[EventIngestionModel]:
+        self, events: list[EventIngestionModel]
+    ) -> list[EventIngestionModel]:
         """
         Augment with long-term static data that changes very infrequently.
-        e.e. self.static_data which includes Person.picture_uri, Person.seat
+        e.e. self.static_data which includes Person.picture_uri, Person.seat.
 
         Parameters
         ----------
         events:
             Returned events from get_events()
 
         Returns
@@ -1474,16 +1493,16 @@
                 if minute_item.votes:
                     for vote in minute_item.votes:
                         vote.person = self.inject_known_person(vote.person)
 
         return events
 
     def post_process_ingestion_models(
-        self, events: List[EventIngestionModel]
-    ) -> List[EventIngestionModel]:
+        self, events: list[EventIngestionModel]
+    ) -> list[EventIngestionModel]:
         """
         Called at the end of get_events() for fully custom site-specific prcessing.
         inject_known_data() already operated on input events.
 
         Parameters
         ----------
         events:
@@ -1494,20 +1513,20 @@
         events: List[EventIngestionModel]
             Base implementation simply returns input events as-is
         """
         return events
 
     def get_events(
         self,
-        begin: Optional[datetime] = None,
-        end: Optional[datetime] = None,
-    ) -> List[EventIngestionModel]:
+        begin: datetime | None = None,
+        end: datetime | None = None,
+    ) -> list[EventIngestionModel]:
         """
         Calls get_legistar_events_for_timespan to retrieve Legistar API data
-        and return as List[EventIngestionModel]
+        and return as List[EventIngestionModel].
 
         Parameters
         ----------
         begin: datetime, optional
             The timespan beginning datetime to query for events after.
             Default is 2 days from UTC now
         end: datetime, optional
@@ -1597,15 +1616,15 @@
             resp = urlopen(f"http://webapi.legistar.com/v1/{self.client_name}/bodies")
             return resp.status == 200
         except URLError or HTTPError:
             return False
 
     def check_for_cdp_min_ingestion(self, check_days: int = 7) -> bool:
         """
-        Test if can obtain at least one minimally defined EventIngestionModel
+        Test if can obtain at least one minimally defined EventIngestionModel.
 
         Parameters
         ----------
         check_days: int, default=7
             Test duration is the past check_days days from now
 
         Returns
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/prime_gov_utils.py` & `cdp-scrapers-0.7.0/cdp_scrapers/prime_gov_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import re
 from datetime import datetime, timedelta
 from logging import getLogger
 from pathlib import Path
 from typing import Any, Dict, Iterator, List, Optional, Pattern, Set, Tuple
 
@@ -44,36 +43,36 @@
 
 Meeting = Dict[str, Any]
 Agenda = BeautifulSoup
 
 
 def primegov_strftime(dt: datetime) -> str:
     """
-    strftime() in format expected for search by primegov api
+    strftime() in format expected for search by primegov api.
 
     Parameters
     ----------
     dt: datetime
         datetime to convert
 
     Returns
     -------
     str
         Input datetime in string
 
     See Also
     --------
-    civic_scraper.platforms.primegov.site.PrimeGovSite.scrape()
+    civic_scraper.platforms.primegov.site.PrimeGovSite.scrape
     """
     return dt.strftime(DATE_FORMAT)
 
 
 def primegov_strptime(meeting: Meeting) -> Optional[datetime]:
     """
-    strptime() on meeting_date_time using expected format commonly used in primegov api
+    strptime() on meeting_date_time using expected format commonly used in primegov api.
 
     Parameters
     ----------
     meeting: Meeting
         Target meeting
 
     Returns
@@ -140,15 +139,15 @@
     Returns
     -------
     Iterator[Tag]
         List of <table> for minutes items
     """
     # look for <div> with certain class then get the <table> inside the <div>
     divs = agenda.find_all("div", class_="agenda-item")
-    return map(lambda d: d.find("table"), divs)
+    return [d.find("table") for d in divs]
 
 
 def get_minutes_item(minutes_table: Tag) -> MinutesItem:
     """
     Extract minutes item name and description.
 
     Parameters
@@ -164,34 +163,34 @@
     Raises
     ------
     ValueError
         If the <table> HTML structure is not as expected
 
     See Also
     --------
-    get_minutes_tables()
+    get_minutes_tables
     """
     rows = minutes_table.find_all("tr")
 
     try:
         # minutes item name in the first row, description in the second row
         name = rows[0].find("td").string
         desc = rows[1].find("div").string
-    except (IndexError, AttributeError):
+    except (IndexError, AttributeError) as e:
         # rows is empty; find*() returned None
         raise ValueError(
             f"Minutes item <table> is no longer recognized: {minutes_table}"
-        )
+        ) from e
 
     return MinutesItem(name=str_simplified(name), description=str_simplified(desc))
 
 
 def get_support_files_div(minutes_table: Tag) -> Tag:
     """
-    Find the <div> containing a minutes item's support document URLs
+    Find the <div> containing a minutes item's support document URLs.
 
     Parameters
     ----------
     minutes_table: Tag
         <table> for a minutes item on agenda web page
 
     Returns
@@ -202,15 +201,15 @@
     # go up from the <table> for this minutes item
     # then find the next <div> that contains the associated support files.
     return minutes_table.parent.find_next_sibling("div", class_="item_contents")
 
 
 def get_support_files(minutes_table: Tag) -> Iterator[SupportingFile]:
     """
-    Extract the minutes item's support file URLs
+    Extract the minutes item's support file URLs.
 
     Parameters
     ----------
     minutes_table: Tag
         <table> for a minutes item on agenda web page
 
     Returns
@@ -221,55 +220,57 @@
     Raises
     ------
     ValueError
         If the <table> HTML structure is not as expected
 
     See Also
     --------
-    get_minutes_tables()
+    get_minutes_tables
     """
 
     def extract_file(file_div: Tag) -> SupportingFile:
         try:
             # the second <a> tag in each file <div> has the file url.
             url_tag = file_div.find_all("a")[1]
-        except IndexError:
+        except IndexError as e:
             # if here, we found <div> with correct class
             # so if we didn't find expected <a>, probably means HTML changed
-            raise ValueError(f"Support file <div> is no longer recognized: {file_div}")
+            raise ValueError(
+                f"Support file <div> is no longer recognized: {file_div}"
+            ) from e
 
         # they sometimes include file suffix in the document title
         # e.g. Budget Recommendation dated 5-18-22.pdf
         # get rid of the suffix .pdf from the descriptive name for the file
         name = re.sub(r"\.\S{2,4}\s*$", "", url_tag.text)
 
         url: str = url_tag["href"]
         # don't need all the query after the file suffix
         # e.g. ...pdf?name=...
         url = url[: url.find("?")]
 
         # use as id if file name is just a number
-        id = Path(url).stem
-        if re.match(r"\d+", id) is None:
-            id = None
+        id_ = Path(url).stem
+        if re.match(r"\d+", id_) is None:
+            id_ = None
 
         return SupportingFile(
-            external_source_id=id, name=str_simplified(name), uri=str_simplified(url)
+            external_source_id=id_, name=str_simplified(name), uri=str_simplified(url)
         )
 
     contents_div = get_support_files_div(minutes_table)
     file_divs = contents_div.find_all("div", class_="attachment-holder")
-    return map(extract_file, file_divs)
+    return [extract_file(file_div) for file_div in file_divs]
 
 
-def get_matter(
+def get_matter(  # noqa: C901
     minutes_table: Tag, minutes_item: Optional[MinutesItem] = None
 ) -> Optional[Matter]:
     """
-    Extract matter info from a minutes item <table>
+    Extract matter info from a minutes item <table>.
 
     Parameters
     ----------
     minutes_table: Tag
         <table> for a minutes item on agenda web page
     minutes_item: Optional[MinutesItem] = None
         Associated minutes item that will be used to fill in some info.
@@ -283,64 +284,58 @@
     Notes
     -----
     Only basic string clean-up is applied, e.g. simplify whitespace.
     Caller is expect to clean up the data as appropriate.
 
     See Also
     --------
-    get_minutes_tables()
+    get_minutes_tables
     """
     # ex 1. APPROVED Information Technology Agency report dated July 26, 2022
     #       - (3) Yes; (0) No
     # ex 2. APPROVED Motion (Buscaino - Lee) - (3) Yes; (0) No
 
     def _get_matter_text(minutes_table: Tag) -> Optional[str]:
-        """
-        Matter text blob from minutes item <table>
-        """
+        """Matter text blob from minutes item <table>."""
         this_div = minutes_table.parent
         matter_div = this_div.next_sibling
         files_div = get_support_files_div(minutes_table)
 
         # If there is a <div> between current <table>
         # and the <div> with the support documents,
         # that <div> will contain matter information
         if matter_div == files_div:
             return None
         return str_simplified(matter_div.text)
 
     def _extract_status(text: str) -> Tuple[str, Optional[str]]:
-        """
-        (matter text blob, result status)
-        """
+        """(matter text blob, result status)."""
         uppercase_word = re.search(r"^\s*([A-Z]+)", text)
         if uppercase_word is None:
             return text, None
 
         result_status = uppercase_word.group(1)
         return str_simplified(text[uppercase_word.end() :]), str_simplified(
             result_status
         )
 
     def _get_name(text: str) -> str:
-        """
-        Keep just the name in the matter text blob
-        """
+        """Keep just the name in the matter text blob."""
         name_end = text.rfind(" dated")
         if name_end < 0:
             name_end = text.rfind(" - (")
 
         if name_end < 0:
             return text
         return str_simplified(text[:name_end])
 
     def _get_type(matter_name: str) -> Optional[str]:
         """
         Last word seems to be appropriate to use as type
-        e.g. report, motion
+        e.g. report, motion.
         """
         type_end = matter_name.rfind("(")
         if type_end < 0:
             type_end = None
 
         type_start = matter_name.rfind(" ", None, type_end)
         if type_start < 0:
@@ -362,15 +357,15 @@
         result_status=result_status,
         title=matter_title,
     )
 
 
 class PrimeGovScraper(PrimeGovSite, IngestionModelScraper):
     """
-    Adapter for civic_scraper PrimeGovSite in cdp-scrapers
+    Adapter for civic_scraper PrimeGovSite in cdp-scrapers.
 
     See Also
     --------
     civic_scraper.platforms.primegov.site.PrimeGoveSite
     cdp_screapers.scraper_utils.IngestionModelScraper
     """
 
@@ -381,25 +376,25 @@
         matter_adopted_pattern: str = (
             r"approved|confirmed|passed|adopted|consent|(?:voted.*com+it+ee)"
         ),
         matter_in_progress_pattern: str = r"heard|read|filed|held|(?:in.*com+it+ee)",
         matter_rejected_pattern: str = r"rejected|dropped",
         person_aliases: Optional[Dict[str, Set[str]]] = None,
     ):
-        """
+        r"""
         Parameters
         ----------
         client_id: str
             primegov api instance id, e.g. lacity for Los Angeles, CA
         timezone: str
             Local time zone
         matter_adopted_pattern: str
             Regex pattern used to convert matter was adopted to CDP constant value.
             Default: "approved|confirmed|passed|adopted"
-        matter_in_progess_pattern: str
+        matter_in_progress_pattern: str
             Regex pattern used to convert matter is in-progress to CDP constant value.
             Default: "heard|ready|filed|held|(?:in\\s*committee)"
         matter_rejected_pattern: str
             Regex pattern used to convert matter was rejected to CDP constant value.
             Default: "rejected|dropped"
         person_aliases: Optional[Dict[str, Set[str]]] = None
             Dictionary used to catch name aliases
@@ -435,15 +430,15 @@
             f"for primegov_instance: {self.primegov_instance}, "
             f"in timezone: {self.timezone}, "
             f"at url: {self.url}"
         )
 
     def get_session(self, meeting: Meeting) -> Optional[Session]:
         """
-        Extract a Session from a primegov meeting dictionary
+        Extract a Session from a primegov meeting dictionary.
 
         Parameters
         ----------
         meeting: Meeting
             Target meeting
 
         Returns
@@ -457,15 +452,15 @@
                 video_uri=str_simplified(meeting[VIDEO_URL]),
                 session_index=0,
             )
         )
 
     def get_body(self, meeting: Meeting) -> Optional[Body]:
         """
-        Extract a Body from a primegov meeting dictionary
+        Extract a Body from a primegov meeting dictionary.
 
         Parameters
         ----------
         meeting: Meeting
             Target meeting
 
         Returns
@@ -473,37 +468,37 @@
         Optional[Body]
             Body extracted from the meeting
         """
         return self.get_none_if_empty(Body(name=str_simplified(meeting[BODY_NAME])))
 
     def get_minutes_item(self, minutes_table: Tag) -> Optional[MinutesItem]:
         """
-        Extract a minutes item from a <table> on agenda web page
+        Extract a minutes item from a <table> on agenda web page.
 
         Parameters
         ----------
         minutes_table: Tag
             <table> tag on agenda web page for a minutes item.
 
         Returns
         -------
         Optional[MinutesItem]
             MinutesItem from given <table>
 
         See Also
         --------
-        get_minutes_item()
+        get_minutes_item
         """
         return self.get_none_if_empty(get_minutes_item(minutes_table))
 
     def get_matter(
         self, minutes_table: Tag, minutes_item: Optional[MinutesItem] = None
     ) -> Optional[Matter]:
         """
-        Extract matter info from a minutes item <table> on agenda web page
+        Extract matter info from a minutes item <table> on agenda web page.
 
         Parameters
         ----------
         minutes_table: Tag
             <table> tag on agenda web page for a minutes item.
         minutes_item: Optional[MinutesItem] = None
             Associated minutes item that will be used to fill in some info.
@@ -517,15 +512,15 @@
         -----
         self.matter_status_pattern_map is used to standardize result_status
         to one of the CDP ingetion model constants.
 
         See Also
         --------
         matter_status_pattern_map
-        get_matter()
+        get_matter
         """
 
         def _standardize_type(matter: Matter) -> Matter:
             if matter.matter_type is not None:
                 # First letter uppercased
                 matter.matter_type = re.sub(
                     r"^\s*([a-z])", lambda m: m.group(1).upper(), matter.matter_type
@@ -546,31 +541,31 @@
 
         matter = _standardize_type(matter)
         matter = _standarize_status(matter)
         return self.get_none_if_empty(matter)
 
     def get_event_minutes_item(self, minutes_table: Tag) -> Optional[EventMinutesItem]:
         """
-        Extract event minutes item info from a minutes item <table> on agenda web page
+        Extract event minutes item info from a minutes item <table> on agenda web page.
 
         Parameters
         ----------
         minutes_table: Tag
             <table> tag on agenda web page for a minutes item.
 
         Returns
         -------
         EventMinutesItem
             Container object with matter, minutes item
 
         See Also
         --------
-        get_matter()
-        get_minutes_item()
-        get_support_files()
+        get_matter
+        get_minutes_item
+        get_support_files
         """
 
         def _get_index(minutes_table: Tag) -> Optional[int]:
             # Parent <table> of this minutes item contains a <span> tag
             # with this minutes item's 1-baesd number
             # <span ...>(1)</span>
             index_pattern: Pattern = re.compile(r"\s*\(\s*(\d+)\s*\)\s*")
@@ -593,15 +588,15 @@
             index=index,
             matter=matter,
             minutes_item=minutes_item,
             supporting_files=support_files,
         )
         return self.get_none_if_empty(event_minutes_item)
 
-    def get_event_minutes_items(
+    def get_event_minutes_items(  # noqa: C901
         self, meeting: Meeting
     ) -> Optional[List[EventMinutesItem]]:
         """
         First find a web page for the given meeting's agenda.
         Then scrape minutes items.
 
         Parameters
@@ -612,35 +607,35 @@
         Returns
         -------
         Optional[List[EventMinutesItem]]
             Event minutes items scraped from the meeting agenda web page.
 
         See Also
         --------
-        get_event_minutes_item()
+        get_event_minutes_item
         """
 
         def _get_output_id(output_docs: List[Dict]) -> int:
             """
             Extract an agenda output document id
-            "compiledMeetingDocumentFiles": [{"id": 41005, ...}, ...]
+            "compiledMeetingDocumentFiles": [{"id": 41005, ...}, ...].
             """
-            WEB_PAGE_TYPE = 3
+            web_page_type = 3
             web_pages = list(
-                filter(lambda d: d["compileOutputType"] == WEB_PAGE_TYPE, output_docs)
+                filter(lambda d: d["compileOutputType"] == web_page_type, output_docs)
             )
             # it appears that, when there are multiple, we want output type 3
             if any(web_pages):
                 document = web_pages[0]
             else:
                 document = output_docs[0]
             return document["id"]
 
         def _find_agenda_urls() -> Iterator[str]:
-            output_templates = meeting.get("templates", list())
+            output_templates = meeting.get("templates", [])
             # These 2 output file templates refer to potential agenda web pages
             # meeting["templates"] = [
             #     {"title": "Journal", ...},
             #     {"title": "Agenda", "compileOutputType": 3, ...},
             #     ...,
             # ]
             for journal in filter(
@@ -674,30 +669,30 @@
         if not agenda or not minutes_tables:
             return None
 
         return reduced_list(map(self.get_event_minutes_item, minutes_tables))
 
     def get_event(self, meeting: Meeting) -> Optional[EventIngestionModel]:
         """
-        Extract a EventIngestionModel from a primegov meeting dictionary
+        Extract a EventIngestionModel from a primegov meeting dictionary.
 
         Parameters
         ----------
         meeting: Meeting
             Target meeting
 
         Returns
         -------
         Optional[EventIngestionModel]
             EventIngestionModel extracted from the meeting
 
         See Also
         --------
-        get_body()
-        get_session()
+        get_body
+        get_session
         """
         return self.get_none_if_empty(
             EventIngestionModel(
                 body=self.get_body(meeting),
                 sessions=reduced_list([self.get_session(meeting)]),
                 external_source_id=str_simplified(str(meeting[MEETING_ID])),
                 event_minutes_items=self.get_event_minutes_items(meeting),
@@ -706,15 +701,15 @@
 
     def get_meetings(
         self,
         begin: datetime,
         end: datetime,
     ) -> Iterator[Meeting]:
         """
-        Query meetings from primegov api endpoint
+        Query meetings from primegov api endpoint.
 
         Parameters
         ----------
         begin: datetime
             The timespan beginning datetime to query for events after.
         end: datetime
             The timespan end datetime to query for events before.
@@ -727,15 +722,15 @@
         Notes
         -----
         Because of CDP's preference for videos,
         meetings without video URL are filtered out.
 
         See Also
         --------
-        get_events()
+        get_events
         """
         resp = self.session.get(
             API_URL.format(
                 base_url=self.base_url,
                 begin=primegov_strftime(begin),
                 end=primegov_strftime(end),
             )
@@ -760,15 +755,15 @@
         Returns
         -------
         events: List[EventIngestionModel]
             One instance of EventIngestionModel per primegov api meeting
 
         See Also
         --------
-        get_meetings()
+        get_meetings
         """
         if end is None:
             end = datetime.utcnow()
         if begin is None:
             begin = end - timedelta(days=2)
 
         meetings = self.get_meetings(begin, end)
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/scraper_utils.py` & `cdp-scrapers-0.7.0/cdp_scrapers/scraper_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,41 @@
+from __future__ import annotations
+
 import json
 import re
+import sys
 from copy import deepcopy
 from datetime import datetime, timedelta
-from itertools import filterfalse, groupby
+from itertools import chain, filterfalse, groupby
 from logging import getLogger
 from pathlib import Path
-from typing import Any, Dict, List, NamedTuple, Optional, Set
+from typing import Any, NamedTuple
 
 import cleantext
 import pytz
 from cdp_backend.database.constants import RoleTitle
 from cdp_backend.pipeline.ingestion_models import (
     Body,
     IngestionModel,
     Person,
     Role,
     Seat,
 )
 from cdp_backend.utils.constants_utils import get_all_class_attr_values
 
-from .types import ScraperStaticData
+from .types import PersonsComparison, ScraperStaticData
 
 ###############################################################################
 
 log = getLogger(__name__)
 
 ###############################################################################
 
 
-def reduced_list(input_list: List[Any], collapse: bool = True) -> Optional[List]:
+def reduced_list(input_list: list[Any], collapse: bool = True) -> list | None:
     """
     Remove all None items from input_list.
 
     Parameters
     ----------
     input_list: List[Any]
         Input list from which to filter out items that are None
@@ -56,14 +59,15 @@
     """
     Remove leading and trailing whitespaces, simplify multiple whitespaces, unify
     newline characters.
 
     Parameters
     ----------
     input_str: str
+        The string to be cleaned.
 
     Returns
     -------
     cleaned: str
         input_str stripped if it is a string
     """
     if not isinstance(input_str, str):
@@ -75,18 +79,19 @@
 
     # Replace utf-8 char encodings with single utf-8 chars themselves
     input_str = input_str.encode("utf-8").decode("utf-8")
 
     return input_str
 
 
-def parse_static_person(
-    person_json: Dict[str, Any],
-    all_seats: Dict[str, Seat],
-    primary_bodies: Dict[str, Body],
+def parse_static_person(  # noqa: C901
+    person_json: dict[str, Any],
+    all_seats: dict[str, Seat],
+    primary_bodies: dict[str, Body],
+    timezone: pytz.timezone,
 ) -> Person:
     """
     Parse Dict[str, Any] for a person in static data file to a Person instance.
     person_json["seat"] and person_json["roles"] are validated against
     all_seats and primary_bodies in static data file.
 
     Parameters
@@ -96,26 +101,30 @@
 
     all_seats: Dict[str, Seat]
         Seats defined as top-level in static data file
 
     primary_bodies: Dict[str, Body]
         Bodies defined as top-level in static data file.
 
+    timezone: str
+        The timezone for the target client.
+        i.e. "America/Los_Angeles" or "America/New_York"
+        See https://en.wikipedia.org/wiki/List_of_tz_database_time_zones for canonical
+        timezones.
 
     See Also
     --------
-    parse_static_file()
-    sanitize_roles()
+    parse_static_file
+    sanitize_roles
     """
     log.debug(f"Begin parsing static data for {person_json['name']}")
 
-    person: Person = Person.from_dict(
-        # "seat" and "roles" are not direct serializations of Seat/Role
-        {k: v for k, v in person_json.items() if k != "seat" and k != "roles"}
-    )
+    # "seat" and "roles" are not direct serializations of Seat/Role
+    kwargs = {k: v for k, v in person_json.items() if k != "seat" and k != "roles"}
+    person: Person = Person(**kwargs)
     if "seat" not in person_json:
         log.debug("Seat name not given")
         return person
 
     seat_name: str = person_json["seat"]
     if seat_name not in all_seats:
         log.error(f"{seat_name} is not defined in top-level 'seats'")
@@ -124,15 +133,15 @@
     # Keep all_seats unmodified; we will append Roles to this person.seat below
     person.seat = deepcopy(all_seats[seat_name])
     if "roles" not in person_json:
         log.debug("Roles not given")
         return person
 
     # Role.title must be a RoleTitle constant so get all allowed values
-    role_titles: List[str] = get_all_class_attr_values(RoleTitle)
+    role_titles: list[str] = get_all_class_attr_values(RoleTitle)
     for role_json in person_json["roles"]:
         if (
             # if str, it is looked-up in primary_bodies
             isinstance(role_json["body"], str)
             and role_json["body"] not in primary_bodies
         ):
             log.error(
@@ -141,104 +150,133 @@
             )
         elif role_json["title"] not in role_titles:
             log.error(
                 f"{role_json} is ignored. "
                 f"{role_json['title']} is not a RoleTitle constant."
             )
         else:
-            role: Role = Role.from_dict(
-                {k: v for k, v in role_json.items() if k != "body"}
+            kwargs = {k: v for k, v in role_json.items() if k != "body"}
+            try:
+                log.debug(f"{kwargs} -> {Role.from_dict(kwargs)}")
+            except Exception:
+                pass
+            else:
+                log.info(f"We can resume using from_dict ({sys.version_info})")
+
+            dt_val = kwargs.get("start_datetime")
+            kwargs["start_datetime"] = (
+                dt_val
+                if dt_val is None
+                else timezone.localize(datetime.fromtimestamp(dt_val))
+            )
+            dt_val = kwargs.get("end_datetime")
+            kwargs["end_datetime"] = (
+                dt_val
+                if dt_val is None
+                else timezone.localize(datetime.fromtimestamp(dt_val))
             )
+
+            role: Role = Role(**kwargs)
             if isinstance(role_json["body"], str):
                 role.body = primary_bodies[role_json["body"]]
             else:
                 # This role.body is a dictionary and defines a non-primary one
                 # e.g. like a committee such as Transportation
                 # that is not the main/full council
-                role.body = Body.from_dict(role_json["body"])
+                kwargs = role_json["body"]
+                role.body = Body(**kwargs)
 
             if person.seat.roles is None:
                 person.seat.roles = [role]
             else:
                 person.seat.roles.append(role)
 
     return person
 
 
-def parse_static_file(file_path: Path) -> ScraperStaticData:
+def parse_static_file(file_path: Path, timezone: str) -> ScraperStaticData:
     """
-    Parse Seats, Bodies and Persons from static data JSON
+    Parse Seats, Bodies and Persons from static data JSON.
 
     Parameters
     ----------
     file_path: Path
         Path to file containing static data in JSON
 
+    timezone: str
+        The timezone for the target client.
+        i.e. "America/Los_Angeles" or "America/New_York"
+        See https://en.wikipedia.org/wiki/List_of_tz_database_time_zones for canonical
+        timezones.
+
     Returns
     -------
     ScraperStaticData:
         Tuple[Dict[str, Seat], Dict[str, Body], Dict[str, Person]]
 
     See Also
-    -----
-    parse_static_person()
-    sanitize_roles()
+    --------
+    parse_static_person
+    sanitize_roles
 
     Notes
     -----
     Function looks for "seats", "primary_bodies", "persons" top-level keys
     """
     with open(file_path) as static_file:
-        static_json: Dict[str, Dict[str, Any]] = json.load(static_file)
+        static_json: dict[str, dict[str, Any]] = json.load(static_file)
 
         if "seats" not in static_json:
-            seats: Dict[str, Seat] = {}
+            seats: dict[str, Seat] = {}
         else:
-            seats: Dict[str, Seat] = {
-                seat_name: Seat.from_dict(seat)
+            seats: dict[str, Seat] = {
+                seat_name: Seat(**seat)
                 for seat_name, seat in static_json["seats"].items()
             }
 
         if "primary_bodies" not in static_json:
-            primary_bodies: Dict[str, Body] = {}
+            primary_bodies: dict[str, Body] = {}
         else:
-            primary_bodies: Dict[str, Body] = {
-                body_name: Body.from_dict(body)
+            primary_bodies: dict[str, Body] = {
+                body_name: Body(**body)
                 for body_name, body in static_json["primary_bodies"].items()
             }
 
         if "persons" not in static_json:
-            known_persons: Dict[str, Person] = {}
+            known_persons: dict[str, Person] = {}
         else:
-            known_persons: Dict[str, Person] = {
-                person_name: parse_static_person(person, seats, primary_bodies)
+            timezone = pytz.timezone(timezone)
+            known_persons: dict[str, Person] = {
+                person_name: parse_static_person(
+                    person, seats, primary_bodies, timezone
+                )
                 for person_name, person in static_json["persons"].items()
             }
 
         log.debug(
             f"ScraperStaticData parsed from {file_path}:\n"
             f"    seats: {list(seats.keys())}\n"
             f"    primary_bodies: {list(primary_bodies.keys())}\n"
             f"    persons: {list(known_persons.keys())}\n"
         )
         return ScraperStaticData(
             seats=seats, primary_bodies=primary_bodies, persons=known_persons
         )
 
 
-def sanitize_roles(
+def sanitize_roles(  # noqa: C901
     person_name: str,
-    roles: Optional[List[Role]] = None,
-    static_data: Optional[ScraperStaticData] = None,
-    council_pres_patterns: List[str] = ["chair", "pres", "super"],
-    chair_patterns: List[str] = ["chair", "pres"],
-) -> Optional[List[Role]]:
+    roles: list[Role] | None = None,
+    static_data: ScraperStaticData | None = None,
+    council_pres_patterns: list[str] | None = None,
+    chair_patterns: list[str] | None = None,
+) -> list[Role] | None:
     """
     1. Standardize roles[i].title to RoleTitle constants
-    2. Ensure only 1 councilmember Role per term
+    2. Ensure only 1 councilmember Role per term.
 
     Parameters
     ----------
     person_name: str
         Sanitization target Person.name
 
     roles: Optional[List[Role]] = None
@@ -264,14 +302,18 @@
     roles[i].title cannot be "Councilmember" or "Council President".
 
     Use "City Council" and "Council Briefing"
     if static_data.primary_bodies is empty.
     """
     if roles is None:
         roles = []
+    if council_pres_patterns is None:
+        council_pres_patterns = ["chair", "pres", "super"]
+    if chair_patterns is None:
+        chair_patterns = ["chair", "pres"]
 
     if not static_data or not static_data.primary_bodies:
         # Primary/full council not defined in static data file.
         # these are reasonably good defaults for most municipalities.
         primary_body_names = ["city council", "council briefing"]
     else:
         primary_body_names = [
@@ -280,17 +322,15 @@
 
     try:
         have_primary_roles = len(static_data.persons[person_name].seat.roles) > 0
     except (KeyError, AttributeError, TypeError):
         have_primary_roles = False
 
     def _is_role_period_ok(role: Role) -> bool:
-        """
-        Test that role.[start | end]_datetime is acceptable
-        """
+        """Test that role.[start | end]_datetime is acceptable."""
         if role.start_datetime is None or role.end_datetime is None:
             return False
         if not have_primary_roles:
             # no roles in static data; accept if this this role is current
             return role.start_datetime.astimezone(
                 pytz.utc
             ) <= datetime.today().astimezone(pytz.utc) and datetime.today().astimezone(
@@ -304,41 +344,35 @@
                 static_role.start_datetime <= role.start_datetime
                 and role.end_datetime <= static_role.end_datetime
             ):
                 return True
         return False
 
     def _is_primary_body(role: Role) -> bool:
-        """
-        Is role.body one of primary_bodies in static data file
-        """
+        """Is role.body one of primary_bodies in static data file."""
         return (
             role.body is not None
             and role.body.name is not None
             and str_simplified(role.body.name).lower() in primary_body_names
         )
 
     def _fix_primary_title(role: Role) -> str:
-        """
-        Council president or Councilmember
-        """
+        """Council president or Councilmember."""
         if (
             role.title is None
             or re.search(
                 "|".join(council_pres_patterns), str_simplified(role.title), re.I
             )
             is None
         ):
             return RoleTitle.COUNCILMEMBER
         return RoleTitle.COUNCILPRESIDENT
 
     def _fix_nonprimary_title(role: Role) -> str:
-        """
-        Not council president or councilmember
-        """
+        """Not council president or councilmember."""
         if role.title is None:
             return RoleTitle.MEMBER
 
         role_title = str_simplified(role.title).lower()
         # Role is not for a primary/full council
         # Role.title cannot be Councilmember or Council President
         if "vice" in role_title:
@@ -378,15 +412,15 @@
         end_datetime: datetime
         index_in_roles: int
 
     # when checking for overlapping terms, we should do so per body.
     # e.g. simultaneous councilmember roles in city council and in council briefing
     # are completely acceptable and common.
 
-    scraped_member_roles_by_body: List[List[Role]] = [
+    scraped_member_roles_by_body: list[list[Role]] = [
         list(roles_for_body)
         for body_name, roles_for_body in groupby(
             sorted(
                 filter(
                     # get all dynamically scraped councilmember terms
                     lambda role: not have_primary_roles
                     and _is_councilmember_term(role),
@@ -421,17 +455,104 @@
                 roles[
                     roles.index(prev_role)
                 ].end_datetime = this_role.start_datetime - timedelta(days=1)
 
     return roles
 
 
+def extract_persons(events):
+    """
+    Get all sponsors and voters across all events.
+
+    Parameters
+    ----------
+    events: list[EventIngestionModel]
+        Scraped events
+
+    Returns
+    -------
+    list[Person]
+        Unique list of all sponsors and voters found
+    """
+
+    def extract_sponsors(event_item):
+        sponsors = event_item.matter.sponsors if event_item.matter else []
+        sponsors = sponsors or []
+        sponsors = reduced_list(sponsors, collapse=False)
+        return sponsors
+
+    def extract_voters(event_item):
+        votes = event_item.votes or []
+        voters = [v.person for v in votes]
+        voters = reduced_list(voters, collapse=False)
+        return voters
+
+    events = reduced_list(events, collapse=False)
+    items = [e.event_minutes_items or [] for e in events]
+    items = chain.from_iterable(items)
+    items = reduced_list(items, collapse=False)
+
+    sponsors = map(extract_sponsors, items)
+    sponsors = chain.from_iterable(sponsors)
+    voters = map(extract_voters, items)
+    voters = chain.from_iterable(voters)
+
+    persons = chain(sponsors, voters)
+    persons = {p.name: p for p in persons}
+    persons = list(persons.values())
+    return persons
+
+
+def compare_persons(
+    scraped_persons, known_persons, primary_bodies
+) -> PersonsComparison:
+    """
+    Look for old and new councilmembers.
+
+    Parameters
+    ----------
+    scraped_persons: list[Person]
+        e.g. from extract_persons
+    known_persons: list[Person]
+        e.g. from ScraperStaticData
+    primary_bodies: list[Body]
+        e.g. from ScraperStaticData
+
+    Returns
+    -------
+    PersonsComparison
+        Old and new councilmember names
+    """
+
+    def holds_primary_role(person):
+        roles = person.seat.roles if person.seat and person.seat.roles else []
+        active_roles = filter(
+            lambda r: r.end_datetime is None
+            or datetime.today().date() <= r.end_datetime.date(),
+            roles,
+        )
+
+        body_names = [r.body.name if r.body else None for r in active_roles]
+        body_names = reduced_list(body_names, collapse=False)
+        primary_body_names = filter(lambda b: b.name in body_names, primary_bodies)
+        return any(primary_body_names)
+
+    active_persons = list(filter(lambda p: p and p.is_active, scraped_persons))
+    primary_persons = list(filter(holds_primary_role, active_persons))
+    names = {p.name for p in primary_persons}
+
+    known_names = {p.name for p in known_persons}
+    old_names = list(known_names - names)
+    new_names = list(names - known_names)
+    return PersonsComparison(old_names, new_names)
+
+
 class IngestionModelScraper:
     """
-    Base class for events scrapers providing IngestionModels for cdp-backend pipeline
+    Base class for events scrapers providing IngestionModels for cdp-backend pipeline.
 
     Parameters
     ----------
     timezone: str
         The timezone for the target client.
         i.e. "America/Los_Angeles" or "America/New_York"
         See https://en.wikipedia.org/wiki/List_of_tz_database_time_zones for canonical
@@ -441,23 +562,24 @@
         and resolve improperly different Persons to the one correct Person.
         Default: None
     """
 
     def __init__(
         self,
         timezone: str,
-        person_aliases: Optional[Dict[str, Set[str]]] = None,
+        person_aliases: dict[str, set[str]] | None = None,
     ):
         self.timezone: pytz.timezone = pytz.timezone(timezone)
         self.person_aliases = person_aliases
 
     @staticmethod
     def find_time_zone() -> str:
         """
-        Return name for a US time zone matching UTC offset calculated from OS clock.
+        Return name for a US time zone matching UTC
+        offset calculated from OS clock.
         """
         utc_now = pytz.utc.localize(datetime.utcnow())
         local_now = datetime.now()
 
         for zone_name in pytz.country_timezones("us"):
             zone = pytz.timezone(zone_name)
             # if this is my time zone
@@ -494,15 +616,15 @@
             return self.timezone.localize(local_time)
         except (AttributeError, ValueError):
             # AttributeError: time_zone or local_time is None
             # ValueError: local_time is not navie (has time zone info)
             return local_time
 
     @staticmethod
-    def get_required_attrs(model: IngestionModel) -> List[str]:
+    def get_required_attrs(model: IngestionModel) -> list[str]:
         """
         Return list of keys required in model as specified in IngestionModel class
         definition.
 
         Parameters
         ----------
         model: IngestionModel
@@ -550,15 +672,15 @@
         ).split(",")
 
         if num_keys != len(keys):
             log.debug(f"{model.__class__} has {num_keys} required keys but got {keys}")
 
         return keys
 
-    def get_none_if_empty(self, model: IngestionModel) -> Optional[IngestionModel]:
+    def get_none_if_empty(self, model: IngestionModel) -> IngestionModel | None:
         """
         Check required keys in model, return None if any such key has no value.
         i.e. If all required keys have valid value, return as-is.
 
         Parameters
         ----------
         model: IngestionModel
@@ -624,7 +746,29 @@
             This base implementation always returns person as-is.
 
         See Also
         --------
         instances.seattle.person_aliases
         """
         return person
+
+    def handle_old_new_council(
+        self, old_names: list[str], new_names: list[str]
+    ) -> None:
+        """
+        Override to handle old and new councilmember information.
+
+        Parameters
+        ----------
+        old_names: list[str]
+            e.g. from scraper_utils.compare_persons
+        new_names: list[str]
+            e.g. from scraper_utils.compare_persons
+
+        Notes
+        -----
+        Base implementation simply logs
+        """
+        if any(old_names):
+            log.info(f"{old_names} are no longer found in scraped data")
+        if any(new_names):
+            log.warning(f"{new_names} are new. Update self.static_data.persons.")
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers/types.py` & `cdp-scrapers-0.7.0/cdp_scrapers/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 from typing import Callable, Dict, List, NamedTuple, Optional
 
 from bs4 import BeautifulSoup
 from cdp_backend.pipeline.ingestion_models import Body, Person, Seat
 
 ###############################################################################
@@ -16,14 +15,19 @@
 
 class ScraperStaticData(NamedTuple):
     seats: Dict[str, Seat] = None
     primary_bodies: Dict[str, Body] = None
     persons: Dict[str, Person] = None
 
 
+class PersonsComparison(NamedTuple):
+    old_names: List[str] = []
+    new_names: List[str] = []
+
+
 LegistarContentParser = Callable[[str, BeautifulSoup], Optional[List[ContentURIs]]]
 """
 Function that returns URLs for videos and captions
 from a Legistar/Granicus-hosted video web page
 
 Parameters
 ----------
@@ -36,9 +40,9 @@
 -------
 uris: Optional[List[ContentURIs]]
     URIs for video and optional caption
 
 See Also
 --------
 cdp_scrapers.legistar_content_parsers
-cdp_scrapers.legistar_utils.get_legistar_content_uris()
+cdp_scrapers.legistar_utils.get_legistar_content_uris
 """
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers.egg-info/PKG-INFO` & `cdp-scrapers-0.7.0/cdp_scrapers.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 Metadata-Version: 2.1
 Name: cdp-scrapers
-Version: 0.6.1
+Version: 0.7.0
 Summary: Scratchpad for scraper development and general utilities.
-Home-page: https://github.com/CouncilDataProject/cdp-scrapers
-Author: Eva Maxfield Brown, Sung Cho, Shak Ragoler
-Author-email: evamaxfieldbrown@gmail.com
-License: MIT license
-Keywords: cdp-scrapers
-Platform: UNKNOWN
+Author: Sung Cho, Shak Ragoler
+Author-email: Eva Maxfield Brown <evamaxfieldbrown@gmail.com>
+License: MIT License
+Project-URL: Homepage, https://github.com/CouncilDataProject/cdp-scrapers
+Project-URL: Bug Tracker, https://github.com/CouncilDataProject/cdp-scrapers/issues
+Project-URL: Documentation, https://CouncilDataProject.github.io/cdp-scrapers
+Project-URL: User Support, https://github.com/CouncilDataProject/cdp-scrapers/issues
 Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: atlanta
+Provides-Extra: all
+Provides-Extra: lint
 Provides-Extra: test
+Provides-Extra: docs
 Provides-Extra: dev
-Provides-Extra: all
 License-File: LICENSE
 
 # cdp-scrapers
 
-[![Build Status](https://github.com/CouncilDataProject/cdp-scrapers/workflows/Build%20Main/badge.svg)](https://github.com/CouncilDataProject/cdp-scrapers/actions)
-[![Documentation](https://github.com/CouncilDataProject/cdp-scrapers/workflows/Documentation/badge.svg)](https://CouncilDataProject.github.io/cdp-scrapers/)
+[![Build Status](https://github.com/CouncilDataProject/cdp-scrapers/workflows/CI/badge.svg)](https://github.com/CouncilDataProject/cdp-scrapers/actions)
+[![Documentation](https://github.com/CouncilDataProject/cdp-scrapers/workflows/Documentation/badge.svg)](https://CouncilDataProject.github.io/cdp-scrapers)
 
 Scratchpad for scraper development and general utilities.
 
 ---
 
+## Installation
+
+**Stable Release:** `pip install cdp-scrapers`<br>
+**Development Head:** `pip install git+https://github.com/CouncilDataProject/cdp-scrapers.git`
+
 ## Council Data Project
 
 Council Data Project is an open-source project dedicated to providing journalists,
 activists, researchers, and all members of each community we serve with the tools they
 need to stay informed and hold their Council Members accountable.
 
 For more information about Council Data Project, please visit
@@ -76,17 +83,15 @@
 )
 ```
 
 ### Scrapers
 
 #### Event Scraper Structure
 
-![get_events](./images/get_events.png)
-
-Our current event scraper structure is as shown above. The main function `get_events` 
+Our current event scraper structure is as follows. The main function `get_events` 
 gets all the required data and it calls the `get_content_uris` function to return the 
 required video data.
 
 If your city uses Legistar and the Legistar data is publicly available.
 - You may be able to reuse our scraper with minimal modifications, such as providing the 
 correct Legistar client ID for your municipality.
 - If the Legistar data returned only does not include the EventVideoPath field for the 
@@ -135,10 +140,8 @@
 
 For full package documentation please visit [councildataproject.org/cdp-scrapers](https://councildataproject.org/cdp-scrapers).
 
 ## Development
 
 Refer to [CONTRIBUTING.md](CONTRIBUTING.md) for information related to developing the code.
 
-**MIT license**
-
-
+**MPLv2 License**
```

### Comparing `cdp-scrapers-0.6.1/cdp_scrapers.egg-info/requires.txt` & `cdp-scrapers-0.7.0/cdp_scrapers.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,41 @@
 beautifulsoup4~=4.9
 cdp-backend>=3.2.4
 defusedxml~=0.7.1
 pytz~=2021.1
 requests~=2.25
 clean-text~=0.6.0
 civic-scraper~=0.2.5
+yt-dlp>=2023.2.17
 
 [all]
-beautifulsoup4~=4.9
-cdp-backend>=3.2.4
-defusedxml~=0.7.1
-pytz~=2021.1
-requests~=2.25
-clean-text~=0.6.0
-civic-scraper~=0.2.5
 selenium~=4.3
 webdriver-manager~=3.8
-black>=19.10b0
-flake8>=3.8.3
-flake8-debugger>=3.2.1
-pytest>=5.4.3
-pytest-cov>=2.9.0
-pytest-raises>=0.11
-tox>=3.15.2
-bump2version>=1.0.1
-ipython>=7.15.0
-m2r2>=0.2.7
-Sphinx>=3.4.3
-sphinx_rtd_theme>=0.5.1
-tox>=3.15.2
-twine>=3.1.1
-wheel>=0.34.2
 
 [atlanta]
 selenium~=4.3
 webdriver-manager~=3.8
 
 [dev]
-selenium~=4.3
-webdriver-manager~=3.8
-black>=19.10b0
-flake8>=3.8.3
-flake8-debugger>=3.2.1
-pytest>=5.4.3
-pytest-cov>=2.9.0
-pytest-raises>=0.11
-tox>=3.15.2
-bump2version>=1.0.1
-ipython>=7.15.0
+ipython>=8.4.0
+
+[docs]
 m2r2>=0.2.7
-Sphinx>=3.4.3
-sphinx_rtd_theme>=0.5.1
-tox>=3.15.2
-twine>=3.1.1
-wheel>=0.34.2
+Sphinx>=4.0.0
+furo>=2022.4.7
+numpydoc
+sphinx-copybutton
+docutils<0.19,>=0.18
+
+[lint]
+black>=22.3.0
+check-manifest>=0.48
+ruff>=0.0.216
+mypy>=0.790
+pre-commit>=2.20.0
 
 [test]
-selenium~=4.3
-webdriver-manager~=3.8
-black>=19.10b0
-flake8>=3.8.3
-flake8-debugger>=3.2.1
+coverage>=5.1
 pytest>=5.4.3
 pytest-cov>=2.9.0
 pytest-raises>=0.11
-tox>=3.15.2
+pytest-rerunfailures>=11.1.2
```

### Comparing `cdp-scrapers-0.6.1/docs/Makefile` & `cdp-scrapers-0.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cdp-scrapers-0.6.1/docs/conf.py` & `cdp-scrapers-0.7.0/docs/conf.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,43 +17,47 @@
 # directory, add these directories to sys.path here. If the directory is
 # relative to the documentation root, use os.path.abspath to make it
 # absolute, like shown here.
 #
 import os
 import sys
 
-import sphinx_rtd_theme
-
 import cdp_scrapers
 
 sys.path.insert(0, os.path.abspath(".."))
 
 
+
 # -- General configuration ---------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = "1.0"
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named "sphinx.ext.*") or your custom ones.
 extensions = [
+    # Sphinx lib ext
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
+    "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
-    "sphinx.ext.napoleon",
-    "sphinx.ext.mathjax",
+    # Installed Sphinx ext
+    "sphinx_copybutton",
+    # Doc installs
     "m2r2",
+    "numpydoc", 
 ]
 
-# Control napoleon
-napoleon_google_docstring = False
-napolean_include_init_with_doc = True
-napoleon_use_ivar = True
-napoleon_use_param = False
+copybutton_prompt_text = r">>> |\.\.\. |\$ |In \[\d*\]: | {2,5}\.\.\.: | {5,8}: "
+copybutton_prompt_is_regexp = True
+
+numpydoc_show_class_members = False
+
+sphinx_tabs_disable_tab_closing = True
 
 # Control autodoc
 autoclass_content = "both"  # include init doc with class
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
@@ -62,21 +66,21 @@
 #
 source_suffix = {
     ".rst": "restructuredtext",
     ".txt": "markdown",
     ".md": "markdown",
 }
 
-# The master toctree document.
-master_doc = "index"
+# The main toctree document.
+main_doc = "index"
 
 # General information about the project.
-project = u"cdp-scrapers"
-copyright = u"2021, Eva Maxfield Brown"
-author = u"Eva Maxfield Brown"
+project = "cdp-scrapers"
+copyright = "2023"
+author = "Eva Maxfield Brown, Sung Cho, Shak Ragoler"
 
 # The version info for the project you"re documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
 version = cdp_scrapers.__version__
@@ -103,24 +107,21 @@
 
 
 # -- Options for HTML output -------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = "sphinx_rtd_theme"
+html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a
 # theme further.  For a list of options available for each theme, see the
 # documentation.
 #
-html_theme_options = {
-    "collapse_navigation": False,
-    "prev_next_buttons_location": "top",
-}
+html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 
@@ -148,39 +149,38 @@
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass
 # [howto, manual, or own class]).
 latex_documents = [
     (
-        master_doc,
+        main_doc,
         "cdp_scrapers.tex",
-        u"cdp-scrapers Documentation",
-        u"Eva Maxfield Brown",
+        "cdp-scrapers Documentation",
+        "Eva Maxfield Brown, Sung Cho, Shak Ragoler",
         "manual",
     ),
 ]
 
 
 # -- Options for manual page output ------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [(master_doc, "cdp_scrapers", u"cdp-scrapers Documentation", [author], 1)]
+man_pages = [(main_doc, "cdp_scrapers", "cdp-scrapers Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output ----------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
     (
-        master_doc,
+        main_doc,
         "cdp_scrapers",
-        u"cdp-scrapers Documentation",
+        "cdp-scrapers Documentation",
         author,
         "cdp_scrapers",
-        "One line description of project.",
-        "Miscellaneous",
+        "Scratchpad for scraper development and general utilities.",
     ),
 ]
```

### Comparing `cdp-scrapers-0.6.1/docs/index.rst` & `cdp-scrapers-0.7.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
    :maxdepth: 1
    :caption: Contents:
 
    Overview <self>
    installation
    Searching for your Municipality's Legistar ID <finding_legistar_id.rst>
    LegistarScraper <legistar_scraper.rst>
-   Package Modules <modules>
+   Package modules <modules>
    contributing
 
 .. mdinclude:: ../README.md
 
 Specific Doc Pages
 ==================
```

### Comparing `cdp-scrapers-0.6.1/docs/installation.rst` & `cdp-scrapers-0.7.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cdp-scrapers-0.6.1/docs/make.bat` & `cdp-scrapers-0.7.0/docs/make.bat`

 * *Files identical despite different names*

