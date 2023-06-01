# Comparing `tmp/prisma_pynext-0.8.8.tar.gz` & `tmp/prisma_pynext-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prisma_pynext-0.8.8.tar", last modified: Thu Jun  1 08:40:05 2023, max compression
+gzip compressed data, was "prisma_pynext-0.8.9.tar", last modified: Thu Jun  1 08:44:42 2023, max compression
```

## Comparing `prisma_pynext-0.8.8.tar` & `prisma_pynext-0.8.9.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.391117 prisma_pynext-0.8.8/
--rw-r--r--   0 filipesommer   (501) staff       (20)    11357 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/LICENSE
--rw-r--r--   0 filipesommer   (501) staff       (20)      294 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/MANIFEST.in
--rw-r--r--   0 filipesommer   (501) staff       (20)    16595 2023-06-01 08:40:05.390882 prisma_pynext-0.8.8/PKG-INFO
--rw-r--r--   0 filipesommer   (501) staff       (20)    15103 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/README.md
--rw-r--r--   0 filipesommer   (501) staff       (20)     1123 2023-05-29 23:47:48.000000 prisma_pynext-0.8.8/pyproject.toml
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.377039 prisma_pynext-0.8.8/requirements/
--rw-r--r--   0 filipesommer   (501) staff       (20)      159 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/requirements/base.txt
--rw-r--r--   0 filipesommer   (501) staff       (20)       11 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/requirements/node.txt
--rw-r--r--   0 filipesommer   (501) staff       (20)       38 2023-06-01 08:40:05.391169 prisma_pynext-0.8.8/setup.cfg
--rw-r--r--   0 filipesommer   (501) staff       (20)     3036 2023-05-29 23:49:29.000000 prisma_pynext-0.8.8/setup.py
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.375881 prisma_pynext-0.8.8/src/
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.379465 prisma_pynext-0.8.8/src/prisma/
--rw-r--r--   0 filipesommer   (501) staff       (20)     1815 2023-06-01 08:40:00.000000 prisma_pynext-0.8.8/src/prisma/__init__.py
--rw-r--r--   0 filipesommer   (501) staff       (20)       86 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/__main__.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1669 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/_async_http.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1804 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/_compat.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     3996 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/_config.py
--rw-r--r--   0 filipesommer   (501) staff       (20)      356 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/_constants.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1199 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/_proxy.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     4073 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/_raw_query.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1361 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/_sync_http.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1120 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/_types.py
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.379918 prisma_pynext-0.8.8/src/prisma/binaries/
--rw-r--r--   0 filipesommer   (501) staff       (20)       50 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/binaries/__init__.py
--rw-r--r--   0 filipesommer   (501) staff       (20)      293 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/binaries/constants.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1915 2023-06-01 08:13:38.000000 prisma_pynext-0.8.8/src/prisma/binaries/platform.py
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.380897 prisma_pynext-0.8.8/src/prisma/cli/
--rw-r--r--   0 filipesommer   (501) staff       (20)       79 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/__init__.py
--rw-r--r--   0 filipesommer   (501) staff       (20)    11850 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/_node.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     2616 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/cli.py
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.381610 prisma_pynext-0.8.8/src/prisma/cli/commands/
--rw-r--r--   0 filipesommer   (501) staff       (20)        0 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/commands/__init__.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1679 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/commands/dev.py
--rw-r--r--   0 filipesommer   (501) staff       (20)      587 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/commands/fetch.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1919 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/commands/generate.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1430 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/commands/version.py
--rw-r--r--   0 filipesommer   (501) staff       (20)      292 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/custom.py
--rw-r--r--   0 filipesommer   (501) staff       (20)      608 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/options.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     3608 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/prisma.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     4174 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/cli/utils.py
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.382032 prisma_pynext-0.8.8/src/prisma/engine/
--rw-r--r--   0 filipesommer   (501) staff       (20)      156 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/engine/__init__.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1768 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/engine/errors.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     7404 2023-06-01 08:39:22.000000 prisma_pynext-0.8.8/src/prisma/engine/utils.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     4968 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/errors.py
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.383342 prisma_pynext-0.8.8/src/prisma/generator/
--rw-r--r--   0 filipesommer   (501) staff       (20)       91 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/__init__.py
--rw-r--r--   0 filipesommer   (501) staff       (20)      135 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/errors.py
--rw-r--r--   0 filipesommer   (501) staff       (20)      245 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/filters.py
--rw-r--r--   0 filipesommer   (501) staff       (20)    10586 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/generator.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     2267 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/jsonrpc.py
--rw-r--r--   0 filipesommer   (501) staff       (20)    32409 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/models.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     4131 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/schema.py
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.386402 prisma_pynext-0.8.8/src/prisma/generator/templates/
--rw-r--r--   0 filipesommer   (501) staff       (20)      936 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/_header.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)      807 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/_utils.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)    35089 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/actions.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)     1133 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/bases.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)    24388 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/builder.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)    17878 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/client.py.jinja
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.386878 prisma_pynext-0.8.8/src/prisma/generator/templates/engine/
--rw-r--r--   0 filipesommer   (501) staff       (20)     1935 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/engine/abstract.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)     2754 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/engine/http.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)     5814 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/engine/query.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)      270 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/enums.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)     4804 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/fields.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)      385 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/http.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)     9044 2023-05-31 09:44:28.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/models.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)     1420 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/partials.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)    21757 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/templates/types.py.jinja
--rw-r--r--   0 filipesommer   (501) staff       (20)      400 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/types.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     3453 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/generator/utils.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     2943 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/http_abstract.py
--rw-r--r--   0 filipesommer   (501) staff       (20)    13272 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/mypy.py
--rw-r--r--   0 filipesommer   (501) staff       (20)       65 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/py.typed
--rw-r--r--   0 filipesommer   (501) staff       (20)      880 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/testing.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     3581 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/utils.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     2752 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma/validator.py
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.387424 prisma_pynext-0.8.8/src/prisma_cleanup/
--rw-r--r--   0 filipesommer   (501) staff       (20)       41 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma_cleanup/__init__.py
--rw-r--r--   0 filipesommer   (501) staff       (20)       59 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma_cleanup/__main__.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     2305 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma_cleanup/_cleanup.py
--rw-r--r--   0 filipesommer   (501) staff       (20)        0 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/src/prisma_cleanup/py.typed
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.388392 prisma_pynext-0.8.8/src/prisma_pynext.egg-info/
--rw-r--r--   0 filipesommer   (501) staff       (20)    16595 2023-06-01 08:40:05.000000 prisma_pynext-0.8.8/src/prisma_pynext.egg-info/PKG-INFO
--rw-r--r--   0 filipesommer   (501) staff       (20)     2722 2023-06-01 08:40:05.000000 prisma_pynext-0.8.8/src/prisma_pynext.egg-info/SOURCES.txt
--rw-r--r--   0 filipesommer   (501) staff       (20)        1 2023-06-01 08:40:05.000000 prisma_pynext-0.8.8/src/prisma_pynext.egg-info/dependency_links.txt
--rw-r--r--   0 filipesommer   (501) staff       (20)       78 2023-06-01 08:40:05.000000 prisma_pynext-0.8.8/src/prisma_pynext.egg-info/entry_points.txt
--rw-r--r--   0 filipesommer   (501) staff       (20)        1 2023-05-29 23:49:05.000000 prisma_pynext-0.8.8/src/prisma_pynext.egg-info/not-zip-safe
--rw-r--r--   0 filipesommer   (501) staff       (20)      199 2023-06-01 08:40:05.000000 prisma_pynext-0.8.8/src/prisma_pynext.egg-info/requires.txt
--rw-r--r--   0 filipesommer   (501) staff       (20)       22 2023-06-01 08:40:05.000000 prisma_pynext-0.8.8/src/prisma_pynext.egg-info/top_level.txt
-drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:40:05.390623 prisma_pynext-0.8.8/tests/
--rw-r--r--   0 filipesommer   (501) staff       (20)     1493 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_actions.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1215 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_batch.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     8660 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_builder.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     6622 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_client.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     2679 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_config.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1779 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_dotenv.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     5807 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_engine.py
--rw-r--r--   0 filipesommer   (501) staff       (20)      281 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_fields.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     2327 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_http.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     2093 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_misc.py
--rw-r--r--   0 filipesommer   (501) staff       (20)      980 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_models.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1169 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_proxy.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     1292 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_testing.py
--rw-r--r--   0 filipesommer   (501) staff       (20)     2517 2023-05-29 23:26:03.000000 prisma_pynext-0.8.8/tests/test_validator.py
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.033643 prisma_pynext-0.8.9/
+-rw-r--r--   0 filipesommer   (501) staff       (20)    11357 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/LICENSE
+-rw-r--r--   0 filipesommer   (501) staff       (20)      294 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/MANIFEST.in
+-rw-r--r--   0 filipesommer   (501) staff       (20)    16595 2023-06-01 08:44:42.033436 prisma_pynext-0.8.9/PKG-INFO
+-rw-r--r--   0 filipesommer   (501) staff       (20)    15103 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/README.md
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1123 2023-05-29 23:47:48.000000 prisma_pynext-0.8.9/pyproject.toml
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.013401 prisma_pynext-0.8.9/requirements/
+-rw-r--r--   0 filipesommer   (501) staff       (20)      159 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/requirements/base.txt
+-rw-r--r--   0 filipesommer   (501) staff       (20)       11 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/requirements/node.txt
+-rw-r--r--   0 filipesommer   (501) staff       (20)       38 2023-06-01 08:44:42.033696 prisma_pynext-0.8.9/setup.cfg
+-rw-r--r--   0 filipesommer   (501) staff       (20)     3036 2023-05-29 23:49:29.000000 prisma_pynext-0.8.9/setup.py
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.011801 prisma_pynext-0.8.9/src/
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.017505 prisma_pynext-0.8.9/src/prisma/
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1815 2023-06-01 08:44:32.000000 prisma_pynext-0.8.9/src/prisma/__init__.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)       86 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/__main__.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1669 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/_async_http.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1804 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/_compat.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     3996 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/_config.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)      356 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/_constants.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1199 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/_proxy.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     4073 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/_raw_query.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1361 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/_sync_http.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1120 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/_types.py
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.018120 prisma_pynext-0.8.9/src/prisma/binaries/
+-rw-r--r--   0 filipesommer   (501) staff       (20)       50 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/binaries/__init__.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)      293 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/binaries/constants.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1915 2023-06-01 08:13:38.000000 prisma_pynext-0.8.9/src/prisma/binaries/platform.py
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.019609 prisma_pynext-0.8.9/src/prisma/cli/
+-rw-r--r--   0 filipesommer   (501) staff       (20)       79 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/__init__.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)    11850 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/_node.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2616 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/cli.py
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.020486 prisma_pynext-0.8.9/src/prisma/cli/commands/
+-rw-r--r--   0 filipesommer   (501) staff       (20)        0 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/commands/__init__.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1679 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/commands/dev.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)      587 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/commands/fetch.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1919 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/commands/generate.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1430 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/commands/version.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)      292 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/custom.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)      608 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/options.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     3608 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/prisma.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     4174 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/cli/utils.py
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.021009 prisma_pynext-0.8.9/src/prisma/engine/
+-rw-r--r--   0 filipesommer   (501) staff       (20)      156 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/engine/__init__.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1768 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/engine/errors.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     7565 2023-06-01 08:44:28.000000 prisma_pynext-0.8.9/src/prisma/engine/utils.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     4968 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/errors.py
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.023875 prisma_pynext-0.8.9/src/prisma/generator/
+-rw-r--r--   0 filipesommer   (501) staff       (20)       91 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/__init__.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)      135 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/errors.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)      245 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/filters.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)    10586 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/generator.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2267 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/jsonrpc.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)    32409 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/models.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     4131 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/schema.py
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.027302 prisma_pynext-0.8.9/src/prisma/generator/templates/
+-rw-r--r--   0 filipesommer   (501) staff       (20)      936 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/_header.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)      807 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/_utils.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)    35089 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/actions.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1133 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/bases.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)    24388 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/builder.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)    17878 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/client.py.jinja
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.028053 prisma_pynext-0.8.9/src/prisma/generator/templates/engine/
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1935 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/engine/abstract.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2754 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/engine/http.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)     5814 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/engine/query.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)      270 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/enums.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)     4804 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/fields.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)      385 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/http.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)     9044 2023-05-31 09:44:28.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/models.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1420 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/partials.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)    21757 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/templates/types.py.jinja
+-rw-r--r--   0 filipesommer   (501) staff       (20)      400 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/types.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     3453 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/generator/utils.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2943 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/http_abstract.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)    13272 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/mypy.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)       65 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/py.typed
+-rw-r--r--   0 filipesommer   (501) staff       (20)      880 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/testing.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     3581 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/utils.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2752 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma/validator.py
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.028865 prisma_pynext-0.8.9/src/prisma_cleanup/
+-rw-r--r--   0 filipesommer   (501) staff       (20)       41 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma_cleanup/__init__.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)       59 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma_cleanup/__main__.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2305 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma_cleanup/_cleanup.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)        0 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/src/prisma_cleanup/py.typed
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.030078 prisma_pynext-0.8.9/src/prisma_pynext.egg-info/
+-rw-r--r--   0 filipesommer   (501) staff       (20)    16595 2023-06-01 08:44:41.000000 prisma_pynext-0.8.9/src/prisma_pynext.egg-info/PKG-INFO
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2722 2023-06-01 08:44:42.000000 prisma_pynext-0.8.9/src/prisma_pynext.egg-info/SOURCES.txt
+-rw-r--r--   0 filipesommer   (501) staff       (20)        1 2023-06-01 08:44:42.000000 prisma_pynext-0.8.9/src/prisma_pynext.egg-info/dependency_links.txt
+-rw-r--r--   0 filipesommer   (501) staff       (20)       78 2023-06-01 08:44:42.000000 prisma_pynext-0.8.9/src/prisma_pynext.egg-info/entry_points.txt
+-rw-r--r--   0 filipesommer   (501) staff       (20)        1 2023-05-29 23:49:05.000000 prisma_pynext-0.8.9/src/prisma_pynext.egg-info/not-zip-safe
+-rw-r--r--   0 filipesommer   (501) staff       (20)      199 2023-06-01 08:44:42.000000 prisma_pynext-0.8.9/src/prisma_pynext.egg-info/requires.txt
+-rw-r--r--   0 filipesommer   (501) staff       (20)       22 2023-06-01 08:44:42.000000 prisma_pynext-0.8.9/src/prisma_pynext.egg-info/top_level.txt
+drwxr-xr-x   0 filipesommer   (501) staff       (20)        0 2023-06-01 08:44:42.033120 prisma_pynext-0.8.9/tests/
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1493 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_actions.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1215 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_batch.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     8660 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_builder.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     6622 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_client.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2679 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_config.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1779 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_dotenv.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     5807 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_engine.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)      281 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_fields.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2327 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_http.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2093 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_misc.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)      980 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_models.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1169 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_proxy.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     1292 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_testing.py
+-rw-r--r--   0 filipesommer   (501) staff       (20)     2517 2023-05-29 23:26:03.000000 prisma_pynext-0.8.9/tests/test_validator.py
```

### Comparing `prisma_pynext-0.8.8/LICENSE` & `prisma_pynext-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/PKG-INFO` & `prisma_pynext-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisma_pynext
-Version: 0.8.8
+Version: 0.8.9
 Summary: Prisma Client Python is an auto-generated and fully type-safe database client
 Home-page: https://github.com/RobertCraigie/prisma-client-py
 Author: Robert Craigie
 Author-email: robert@craigie.dev
 Maintainer: Filipe Sommer
 License: APACHE
 Project-URL: Documentation, https://prisma-client-py.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prisma_pynext Version: 0.8.8 Summary: Prisma Client
+Metadata-Version: 2.1 Name: prisma_pynext Version: 0.8.9 Summary: Prisma Client
 Python is an auto-generated and fully type-safe database client Home-page:
 https://github.com/RobertCraigie/prisma-client-py Author: Robert Craigie
 Author-email: robert@craigie.dev Maintainer: Filipe Sommer License: APACHE
 Project-URL: Documentation, https://prisma-client-py.readthedocs.io Project-
 URL: Source, https://github.com/RobertCraigie/prisma-client-py Project-URL:
 Tracker, https://github.com/RobertCraigie/prisma-client-py/issues Keywords:
 orm,mysql,typing,prisma,sqlite,database,postgresql Classifier: Development
```

### Comparing `prisma_pynext-0.8.8/README.md` & `prisma_pynext-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/pyproject.toml` & `prisma_pynext-0.8.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/setup.py` & `prisma_pynext-0.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/__init__.py` & `prisma_pynext-0.8.9/src/prisma/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 
 __title__ = 'prisma_pynext'
 __author__ = 'RobertCraigie'
 __license__ = 'APACHE'
 __copyright__ = 'Copyright 2020-2023 RobertCraigie'
-__version__ = '0.8.8'
+__version__ = '0.8.9'
 
 from typing import TYPE_CHECKING
 
 from ._config import config as config
 from .utils import setup_logging
 from . import errors as errors
 from .validator import *
```

### Comparing `prisma_pynext-0.8.8/src/prisma/_async_http.py` & `prisma_pynext-0.8.9/src/prisma/_async_http.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/_compat.py` & `prisma_pynext-0.8.9/src/prisma/_compat.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/_config.py` & `prisma_pynext-0.8.9/src/prisma/_config.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/_proxy.py` & `prisma_pynext-0.8.9/src/prisma/_proxy.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/_raw_query.py` & `prisma_pynext-0.8.9/src/prisma/_raw_query.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/_sync_http.py` & `prisma_pynext-0.8.9/src/prisma/_sync_http.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/_types.py` & `prisma_pynext-0.8.9/src/prisma/_types.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/binaries/platform.py` & `prisma_pynext-0.8.9/src/prisma/binaries/platform.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/cli/_node.py` & `prisma_pynext-0.8.9/src/prisma/cli/_node.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/cli/cli.py` & `prisma_pynext-0.8.9/src/prisma/cli/cli.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/cli/commands/dev.py` & `prisma_pynext-0.8.9/src/prisma/cli/commands/dev.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/cli/commands/fetch.py` & `prisma_pynext-0.8.9/src/prisma/cli/commands/fetch.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/cli/commands/generate.py` & `prisma_pynext-0.8.9/src/prisma/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/cli/commands/version.py` & `prisma_pynext-0.8.9/src/prisma/cli/commands/version.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/cli/options.py` & `prisma_pynext-0.8.9/src/prisma/cli/options.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/cli/prisma.py` & `prisma_pynext-0.8.9/src/prisma/cli/prisma.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/cli/utils.py` & `prisma_pynext-0.8.9/src/prisma/cli/utils.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/engine/errors.py` & `prisma_pynext-0.8.9/src/prisma/engine/errors.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/engine/utils.py` & `prisma_pynext-0.8.9/src/prisma/engine/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,17 +105,24 @@
             file_from_paths,
         )
     elif global_path.exists():
         file = global_path
         log.debug('Query engine found in the global path')
 
 
-    os.listdir("/vercel/.cache/prisma-python/binaries/4.14.0/d9a4c5988f480fa576d43970d5a23641aa77bc9c/node_modules")
-    os.listdir("/vercel/.cache/prisma-python/binaries/4.14.0/")
-    os.listdir("/vercel/.cache/prisma-python/")
+    #os.listdir("/vercel/.cache/prisma-python/binaries/4.14.0/d9a4c5988f480fa576d43970d5a23641aa77bc9c/node_modules")
+    #os.listdir("/vercel/.cache/prisma-python/binaries/4.14.0/")
+    try:
+        os.listdir("vercel/.cache/prisma-python/")
+    except FileNotFoundError:
+        pass
+    try:
+        os.listdir("/vercel/.cache/prisma-python/")
+    except FileNotFoundError:
+        pass
     raise errors.BinaryNotFoundError(
         f'Only files ' + str(os.listdir("/vercel/.cache"))
     )
     os.listdir("/vercel")
     onlyfiles = [f for f in os.listdir("/vercel/.cache/prisma-python/binaries/4.14.0/d9a4c5988f480fa576d43970d5a23641aa77bc9c/node_modules/prisma/") if os.path.isfile(os.path.join("/vercel/.cache/prisma-python/binaries/4.14.0/d9a4c5988f480fa576d43970d5a23641aa77bc9c/node_modules/prisma/", f))]
     # raise errors.BinaryNotFoundError(
     #         f'Only files ' + str(onlyfiles)
```

### Comparing `prisma_pynext-0.8.8/src/prisma/errors.py` & `prisma_pynext-0.8.9/src/prisma/errors.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/generator.py` & `prisma_pynext-0.8.9/src/prisma/generator/generator.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/jsonrpc.py` & `prisma_pynext-0.8.9/src/prisma/generator/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/models.py` & `prisma_pynext-0.8.9/src/prisma/generator/models.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/schema.py` & `prisma_pynext-0.8.9/src/prisma/generator/schema.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/_header.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/_header.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/_utils.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/_utils.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/actions.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/actions.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/bases.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/bases.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/builder.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/builder.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/client.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/client.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/engine/abstract.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/engine/abstract.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/engine/http.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/engine/http.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/engine/query.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/engine/query.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/fields.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/fields.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/models.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/models.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/partials.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/partials.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/templates/types.py.jinja` & `prisma_pynext-0.8.9/src/prisma/generator/templates/types.py.jinja`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/generator/utils.py` & `prisma_pynext-0.8.9/src/prisma/generator/utils.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/http_abstract.py` & `prisma_pynext-0.8.9/src/prisma/http_abstract.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/mypy.py` & `prisma_pynext-0.8.9/src/prisma/mypy.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/testing.py` & `prisma_pynext-0.8.9/src/prisma/testing.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/utils.py` & `prisma_pynext-0.8.9/src/prisma/utils.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma/validator.py` & `prisma_pynext-0.8.9/src/prisma/validator.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma_cleanup/_cleanup.py` & `prisma_pynext-0.8.9/src/prisma_cleanup/_cleanup.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/src/prisma_pynext.egg-info/PKG-INFO` & `prisma_pynext-0.8.9/src/prisma_pynext.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prisma-pynext
-Version: 0.8.8
+Version: 0.8.9
 Summary: Prisma Client Python is an auto-generated and fully type-safe database client
 Home-page: https://github.com/RobertCraigie/prisma-client-py
 Author: Robert Craigie
 Author-email: robert@craigie.dev
 Maintainer: Filipe Sommer
 License: APACHE
 Project-URL: Documentation, https://prisma-client-py.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: prisma-pynext Version: 0.8.8 Summary: Prisma Client
+Metadata-Version: 2.1 Name: prisma-pynext Version: 0.8.9 Summary: Prisma Client
 Python is an auto-generated and fully type-safe database client Home-page:
 https://github.com/RobertCraigie/prisma-client-py Author: Robert Craigie
 Author-email: robert@craigie.dev Maintainer: Filipe Sommer License: APACHE
 Project-URL: Documentation, https://prisma-client-py.readthedocs.io Project-
 URL: Source, https://github.com/RobertCraigie/prisma-client-py Project-URL:
 Tracker, https://github.com/RobertCraigie/prisma-client-py/issues Keywords:
 orm,mysql,typing,prisma,sqlite,database,postgresql Classifier: Development
```

### Comparing `prisma_pynext-0.8.8/src/prisma_pynext.egg-info/SOURCES.txt` & `prisma_pynext-0.8.9/src/prisma_pynext.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_actions.py` & `prisma_pynext-0.8.9/tests/test_actions.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_batch.py` & `prisma_pynext-0.8.9/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_builder.py` & `prisma_pynext-0.8.9/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_client.py` & `prisma_pynext-0.8.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_config.py` & `prisma_pynext-0.8.9/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_dotenv.py` & `prisma_pynext-0.8.9/tests/test_dotenv.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_engine.py` & `prisma_pynext-0.8.9/tests/test_engine.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_http.py` & `prisma_pynext-0.8.9/tests/test_http.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_misc.py` & `prisma_pynext-0.8.9/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_models.py` & `prisma_pynext-0.8.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_proxy.py` & `prisma_pynext-0.8.9/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_testing.py` & `prisma_pynext-0.8.9/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `prisma_pynext-0.8.8/tests/test_validator.py` & `prisma_pynext-0.8.9/tests/test_validator.py`

 * *Files identical despite different names*

