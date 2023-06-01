# Comparing `tmp/rapidexec-0.0.2.tar.gz` & `tmp/rapidexec-0.0.3.tar.gz`

## Comparing `rapidexec-0.0.2.tar` & `rapidexec-0.0.3.tar`

### file list

```diff
@@ -1,108 +1,108 @@
--rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 rapidexec-0.0.2/Makefile
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/10c3b8cef2d7cc80
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/1818bfa1bd179e59
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/22bd47409fd7c69f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/268c03884f402466
--rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/2694e4d07d4109e2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/299b2767d156295c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/2c1eebf9a18bad9a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/2fc86cefd31dfc3d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/2fd0e1d766833c3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/34fc3c104f4fa7c4
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/3df319264a556f22
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/3f79e6b5d1330dec
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/45a3f94c0f96a385
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/46db4ba82b77ddb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/4bf325b2fef8f024
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/4ea703b46434a417
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/57e4496688fdf27
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/5808bfa06e5c87da
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/5aec382a2ad3bf0d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/5c3fb0a2903f833c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/5f9a3c21723df053
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/621ec582d38dee3b
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/72f5b0e04bce5c05
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/77cd20fcf489855f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/7ed4f9d6fbad82a2
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/822cee63a41955b1
--rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/85b57e0f3fdec51f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/89224bad46317d3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/8c29a49c31719ef6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/8c76579657306f9d
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/8ebaa362ef45b2b3
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/9300205a76b4aba
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/95e2b56816649143
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/967f421e7cc51659
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/96c6041d9c501a75
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/975be10cef2289d6
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/9f1cf7874e23f1bb
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/9f9c0b549716099f
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/a447b23329cec11e
--rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/a58518bcb4877be7
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/a73cc6f84f800e44
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/abf704f425e1f84e
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/ae1e858bf6e288a2
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/aefaa4ecf7e8aa47
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/b065fb4879956e13
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/b0e5e7b31566508e
--rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/b315eacd1e21a82f
--rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/b42cd2e611ba9966
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/b548815ba1b7fad5
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/b67523c5567ff181
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/c270507c69b766ff
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/d13d4f1be7bddc28
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/d3c7ef085d7b4ce
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/d7e96ecf62fcc658
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/d86fb3ba2a66e2ef
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/d8db62e0c33e5b94
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/da09c6a4090af3bb
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/e3e818b6081c745c
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/e494090f5c592773
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/e88b60ad46034cfa
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/eaabf6a2b525aad4
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/ecf4ef3e9da00bc9
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/ef698edbbbf8d700
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/f599e3ccbd3d841a
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/f831cba8155d6cdb
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/fe44785dea20b873
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.ruff_cache/content/fef8b13e54ebe4a8
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 rapidexec-0.0.2/docs/images/docker-ps.png
--rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 rapidexec-0.0.2/docs/images/export-exclude.png
--rw-r--r--   0        0        0    12961 2020-02-02 00:00:00.000000 rapidexec-0.0.2/docs/images/export-include.png
--rw-r--r--   0        0        0    18784 2020-02-02 00:00:00.000000 rapidexec-0.0.2/docs/images/export.png
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/__init__.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/cli.py
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/commands/__init__.py
--rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/commands/base.py
--rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/commands/command.py
--rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/commands/filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/config/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/console/__init__.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/console/progress_manager.py
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/console/singleton.py
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/console/test_2.py
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/console/wrapper.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/services/__init__.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/services/export.py
--rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/services/live.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/services/compose/__init__.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/services/compose/logs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/services/docker/__init__.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/services/docker/logs.py
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 rapidexec-0.0.2/rapidexec/services/docker/ps.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 rapidexec-0.0.2/requirements/base.txt
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rapidexec-0.0.2/requirements/dev.txt
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 rapidexec-0.0.2/scripts/format.sh
--rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 rapidexec-0.0.2/scripts/lint.sh
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 rapidexec-0.0.2/scripts/test.sh
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 rapidexec-0.0.2/tests/test_version.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 rapidexec-0.0.2/tests/test_data/invalid_format_pyproject.toml
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 rapidexec-0.0.2/tests/test_data/missing_required_field_pyproject.toml
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 rapidexec-0.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 rapidexec-0.0.2/LICENSE
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 rapidexec-0.0.2/README.md
--rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 rapidexec-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3807 2020-02-02 00:00:00.000000 rapidexec-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 rapidexec-0.0.3/Makefile
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/10c3b8cef2d7cc80
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/1818bfa1bd179e59
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/22bd47409fd7c69f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/268c03884f402466
+-rw-r--r--   0        0        0     3009 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/2694e4d07d4109e2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/299b2767d156295c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/2c1eebf9a18bad9a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/2fc86cefd31dfc3d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/2fd0e1d766833c3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/34fc3c104f4fa7c4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/3df319264a556f22
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/3f79e6b5d1330dec
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/45a3f94c0f96a385
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/46db4ba82b77ddb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/4bf325b2fef8f024
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/4ea703b46434a417
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/57e4496688fdf27
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/5808bfa06e5c87da
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/5aec382a2ad3bf0d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/5c3fb0a2903f833c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/5f9a3c21723df053
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/621ec582d38dee3b
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/72f5b0e04bce5c05
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/77cd20fcf489855f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/7ed4f9d6fbad82a2
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/822cee63a41955b1
+-rw-r--r--   0        0        0     3995 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/85b57e0f3fdec51f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/89224bad46317d3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/8c29a49c31719ef6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/8c76579657306f9d
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/8ebaa362ef45b2b3
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/9300205a76b4aba
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/95e2b56816649143
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/967f421e7cc51659
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/96c6041d9c501a75
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/975be10cef2289d6
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/9f1cf7874e23f1bb
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/9f9c0b549716099f
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/a447b23329cec11e
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/a58518bcb4877be7
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/a73cc6f84f800e44
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/abf704f425e1f84e
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/ae1e858bf6e288a2
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/aefaa4ecf7e8aa47
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/b065fb4879956e13
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/b0e5e7b31566508e
+-rw-r--r--   0        0        0     3093 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/b315eacd1e21a82f
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/b42cd2e611ba9966
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/b548815ba1b7fad5
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/b67523c5567ff181
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/c270507c69b766ff
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/d13d4f1be7bddc28
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/d3c7ef085d7b4ce
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/d7e96ecf62fcc658
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/d86fb3ba2a66e2ef
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/d8db62e0c33e5b94
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/da09c6a4090af3bb
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/e3e818b6081c745c
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/e494090f5c592773
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/e88b60ad46034cfa
+-rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/eaabf6a2b525aad4
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/ecf4ef3e9da00bc9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/ef698edbbbf8d700
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/f599e3ccbd3d841a
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/f831cba8155d6cdb
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/fe44785dea20b873
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.ruff_cache/content/fef8b13e54ebe4a8
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 rapidexec-0.0.3/docs/images/docker-ps.png
+-rw-r--r--   0        0        0     6499 2020-02-02 00:00:00.000000 rapidexec-0.0.3/docs/images/export-exclude.png
+-rw-r--r--   0        0        0    12961 2020-02-02 00:00:00.000000 rapidexec-0.0.3/docs/images/export-include.png
+-rw-r--r--   0        0        0    18784 2020-02-02 00:00:00.000000 rapidexec-0.0.3/docs/images/export.png
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/__init__.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/cli.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/commands/__init__.py
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/commands/base.py
+-rw-r--r--   0        0        0     2786 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/commands/command.py
+-rw-r--r--   0        0        0     2718 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/commands/filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/config/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/console/__init__.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/console/progress_manager.py
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/console/singleton.py
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/console/test_2.py
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/console/wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/services/__init__.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/services/export.py
+-rw-r--r--   0        0        0     3541 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/services/live.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/services/compose/__init__.py
+-rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/services/compose/logs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/services/docker/__init__.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/services/docker/logs.py
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 rapidexec-0.0.3/rapidexec/services/docker/ps.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 rapidexec-0.0.3/requirements/base.txt
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 rapidexec-0.0.3/requirements/dev.txt
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 rapidexec-0.0.3/scripts/format.sh
+-rwxr-xr-x   0        0        0       81 2020-02-02 00:00:00.000000 rapidexec-0.0.3/scripts/lint.sh
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 rapidexec-0.0.3/scripts/test.sh
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 rapidexec-0.0.3/tests/test_version.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 rapidexec-0.0.3/tests/test_data/invalid_format_pyproject.toml
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 rapidexec-0.0.3/tests/test_data/missing_required_field_pyproject.toml
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 rapidexec-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 rapidexec-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 rapidexec-0.0.3/README.md
+-rw-r--r--   0        0        0     1975 2020-02-02 00:00:00.000000 rapidexec-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 rapidexec-0.0.3/PKG-INFO
```

### Comparing `rapidexec-0.0.2/.ruff_cache/content/10c3b8cef2d7cc80` & `rapidexec-0.0.3/.ruff_cache/content/10c3b8cef2d7cc80`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/22bd47409fd7c69f` & `rapidexec-0.0.3/.ruff_cache/content/22bd47409fd7c69f`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/2694e4d07d4109e2` & `rapidexec-0.0.3/.ruff_cache/content/2694e4d07d4109e2`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/77cd20fcf489855f` & `rapidexec-0.0.3/.ruff_cache/content/77cd20fcf489855f`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/822cee63a41955b1` & `rapidexec-0.0.3/.ruff_cache/content/822cee63a41955b1`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/85b57e0f3fdec51f` & `rapidexec-0.0.3/.ruff_cache/content/85b57e0f3fdec51f`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/a58518bcb4877be7` & `rapidexec-0.0.3/.ruff_cache/content/a58518bcb4877be7`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/b0e5e7b31566508e` & `rapidexec-0.0.3/.ruff_cache/content/b0e5e7b31566508e`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/b315eacd1e21a82f` & `rapidexec-0.0.3/.ruff_cache/content/b315eacd1e21a82f`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/b42cd2e611ba9966` & `rapidexec-0.0.3/.ruff_cache/content/b42cd2e611ba9966`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/e3e818b6081c745c` & `rapidexec-0.0.3/.ruff_cache/content/e3e818b6081c745c`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/eaabf6a2b525aad4` & `rapidexec-0.0.3/.ruff_cache/content/eaabf6a2b525aad4`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/ecf4ef3e9da00bc9` & `rapidexec-0.0.3/.ruff_cache/content/ecf4ef3e9da00bc9`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.ruff_cache/content/fe44785dea20b873` & `rapidexec-0.0.3/.ruff_cache/content/fe44785dea20b873`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/docs/images/docker-ps.png` & `rapidexec-0.0.3/docs/images/docker-ps.png`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/docs/images/export-exclude.png` & `rapidexec-0.0.3/docs/images/export-exclude.png`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/docs/images/export-include.png` & `rapidexec-0.0.3/docs/images/export-include.png`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/docs/images/export.png` & `rapidexec-0.0.3/docs/images/export.png`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/cli.py` & `rapidexec-0.0.3/rapidexec/cli.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/commands/base.py` & `rapidexec-0.0.3/rapidexec/commands/base.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/commands/command.py` & `rapidexec-0.0.3/rapidexec/commands/command.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/commands/filters.py` & `rapidexec-0.0.3/rapidexec/commands/filters.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/console/progress_manager.py` & `rapidexec-0.0.3/rapidexec/console/progress_manager.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/console/wrapper.py` & `rapidexec-0.0.3/rapidexec/console/wrapper.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/services/export.py` & `rapidexec-0.0.3/rapidexec/services/export.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/services/live.py` & `rapidexec-0.0.3/rapidexec/services/live.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/services/compose/logs.py` & `rapidexec-0.0.3/rapidexec/services/compose/logs.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/services/docker/logs.py` & `rapidexec-0.0.3/rapidexec/services/docker/logs.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/rapidexec/services/docker/ps.py` & `rapidexec-0.0.3/rapidexec/services/docker/ps.py`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/.gitignore` & `rapidexec-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/LICENSE` & `rapidexec-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/README.md` & `rapidexec-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
 ### Example output
 
 #### docker-ps
 ```bash
 $ rapidexec docker-ps
 ```
-![image](./docs/images/docker-ps.png)
+![image](https://raw.githubusercontent.com/godd0t/rapidexec/main/docs/images/docker-ps.png)
 
 #### export
 
 1. Scenario: toml file pyproject.toml and output file requirements.txt
     ```bash
     $ rapidexec export -f pyproject.toml -o requirements.txt
     ```
@@ -75,13 +75,13 @@
     $ rapidexec export --include dev
     ```
     ![image](https://raw.githubusercontent.com/godd0t/rapidexec/main/docs/images/export-include.png)
 
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](https://github.com/godd0t/rapidexec/blob/main/LICENSE) file for details.
 
 
 ## Contributing
 
 If you want to contribute to this project, you can create a pull request on GitHub.
```

### Comparing `rapidexec-0.0.2/pyproject.toml` & `rapidexec-0.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapidexec-0.0.2/PKG-INFO` & `rapidexec-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapidexec
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple, fast, and flexible way to execute commands in a Docker container.
 Project-URL: Homepage, https://github.com/godd0t/rapidexec
 License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django :: 4.2
@@ -85,15 +85,15 @@
 
 ### Example output
 
 #### docker-ps
 ```bash
 $ rapidexec docker-ps
 ```
-![image](./docs/images/docker-ps.png)
+![image](https://raw.githubusercontent.com/godd0t/rapidexec/main/docs/images/docker-ps.png)
 
 #### export
 
 1. Scenario: toml file pyproject.toml and output file requirements.txt
     ```bash
     $ rapidexec export -f pyproject.toml -o requirements.txt
     ```
@@ -109,13 +109,13 @@
     $ rapidexec export --include dev
     ```
     ![image](https://raw.githubusercontent.com/godd0t/rapidexec/main/docs/images/export-include.png)
 
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the MIT License - see the [LICENSE](https://github.com/godd0t/rapidexec/blob/main/LICENSE) file for details.
 
 
 ## Contributing
 
 If you want to contribute to this project, you can create a pull request on GitHub.
```

