# Comparing `tmp/salt-analytics-framework-0.4.0.tar.gz` & `tmp/salt-analytics-framework-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Thu May 18 16:29:43 2023, max compression
+gzip compressed data, last modified: Thu Jun  1 19:13:59 2023, max compression
```

## Comparing `salt-analytics-framework-0.4.0.tar` & `salt-analytics-framework-0.5.0.tar`

### file list

```diff
@@ -1,154 +1,172 @@
--rw-r--r--   0 root         (0) root         (0)       20 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.bandit
--rw-r--r--   0 root         (0) root         (0)      684 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.coveragerc
--rw-r--r--   0 root         (0) root         (0)        5 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.dockerignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/
--rw-r--r--   0 root         (0) root         (0)      229 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/actionlint.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/actions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/actions/setup-actionlint/
--rw-r--r--   0 root         (0) root         (0)      892 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/actions/setup-actionlint/action.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)    10391 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.github/workflows/ci.yml
--rw-r--r--   0 root         (0) root         (0)     1983 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     3674 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-config.yaml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/
--rw-r--r--   0 root         (0) root         (0)     4609 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/check-changelog-entries.py
--rw-r--r--   0 root         (0) root         (0)     2227 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/check-cli-examples.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/copyright-headers.py
--rw-r--r--   0 root         (0) root         (0)     2092 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/make-autodocs.py
--rw-r--r--   0 root         (0) root         (0)      579 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pre-commit-hooks/sort-pylint-spelling-words.py
--rw-r--r--   0 root         (0) root         (0)      650 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/.pylint-spelling-words
--rw-r--r--   0 root         (0) root         (0)     2665 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/CHANGELOG.rst
--rw-r--r--   0 root         (0) root         (0)     5256 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)     2487 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/CONTRIBUTING.md
--rw-r--r--   0 root         (0) root         (0)     9283 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      549 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/NOTICE
--rw-r--r--   0 root         (0) root         (0)     3046 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1861 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/changelog/
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/changelog/_template.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/
--rw-r--r--   0 root         (0) root         (0)      634 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/Makefile
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/_static/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/_static/.gitkeep
--rw-r--r--   0 root         (0) root         (0)      164 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/all.rst
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/changelog.rst
--rw-r--r--   0 root         (0) root         (0)     6553 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/conf.py
--rw-r--r--   0 root         (0) root         (0)      200 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/contents.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/index.rst
--rw-r--r--   0 root         (0) root         (0)      760 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/make.bat
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/
--rw-r--r--   0 root         (0) root         (0)       46 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/modules.rst
--rw-r--r--   0 root         (0) root         (0)      720 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.collect.rst
--rw-r--r--   0 root         (0) root         (0)      557 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.forward.rst
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.process.rst
--rw-r--r--   0 root         (0) root         (0)      861 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.rst
--rw-r--r--   0 root         (0) root         (0)      346 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.saltext.engines.rst
--rw-r--r--   0 root         (0) root         (0)      202 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.saltext.rst
--rw-r--r--   0 root         (0) root         (0)      408 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/ref/saf.utils.rst
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/docs/sitevars.rst
--rw-r--r--   0 root         (0) root         (0)    20016 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/noxfile.py
--rw-r--r--   0 root         (0) root         (0)     4837 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      428 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/pytest.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/
--rw-r--r--   0 root         (0) root         (0)      176 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/base.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/build.txt
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/changelog.txt
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/dev.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/docs-auto.txt
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/tests.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/requirements/tools.txt
--rw-r--r--   0 root         (0) root         (0)     3170 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      198 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/
--rw-r--r--   0 root         (0) root         (0)      914 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2618 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/beacons.py
--rw-r--r--   0 root         (0) root         (0)     3082 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/file.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/noop.py
--rw-r--r--   0 root         (0) root         (0)     1473 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/collect/salt_exec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/forward/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/forward/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/forward/disk.py
--rw-r--r--   0 root         (0) root         (0)      798 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/forward/noop.py
--rw-r--r--   0 root         (0) root         (0)     1825 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/forward/test.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/manager.py
--rw-r--r--   0 root         (0) root         (0)    10262 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/models.py
--rw-r--r--   0 root         (0) root         (0)     6800 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/pipeline.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/plugins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/noop.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/regex_mask.py
--rw-r--r--   0 root         (0) root         (0)      594 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/regex_mask.pyi
--rw-r--r--   0 root         (0) root         (0)     4490 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/process/shannon_mask.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/saltext/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/saltext/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/saltext/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/saltext/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2165 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/saltext/engines/analytics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/utils/dt.py
--rw-r--r--   0 root         (0) root         (0)     5542 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/utils/eventbus.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/saf/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3046 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3417 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      382 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      652 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/
--rw-r--r--   0 root         (0) root         (0)      738 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1207 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/forwarders/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/forwarders/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2303 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/forwarders/test_concurrency.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/manager/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/manager/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/manager/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/manager/test_disabled_pipeline.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/functional/manager/test_enabled_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_memusage.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_multiple.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_status.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/__init__.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/conftest.py
--rw-r--r--   0 root         (0) root         (0)     1734 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_arg.py
--rw-r--r--   0 root         (0) root         (0)     1563 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_collatz.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_config_get.py
--rw-r--r--   0 root         (0) root         (0)     1399 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/engines/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/integration/engines/test_engine.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/process/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/process/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3803 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/process/test_regex_mask.py
--rw-r--r--   0 root         (0) root         (0)     5436 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/process/test_shannon_mask.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/salt/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/salt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/salt/engines/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tests/unit/salt/engines/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/.ruff.toml
--rw-r--r--   0 root         (0) root         (0)      334 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5495 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/ci.py
--rw-r--r--   0 root         (0) root         (0)     1383 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/pre_commit.py
--rw-r--r--   0 root         (0) root         (0)     1382 2023-05-18 16:29:43.000000 salt-analytics-framework-0.4.0/tools/pre_commit.py~
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.bandit
+-rw-r--r--   0 root         (0) root         (0)      684 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.coveragerc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.github/
+-rw-r--r--   0 root         (0) root         (0)      229 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.github/actionlint.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.github/actions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.github/actions/setup-actionlint/
+-rw-r--r--   0 root         (0) root         (0)      892 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.github/actions/setup-actionlint/action.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.github/patches/
+-rw-r--r--   0 root         (0) root         (0)      362 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.github/patches/win_network.patch
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)    14266 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     3895 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     4609 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.pre-commit-hooks/check-changelog-entries.py
+-rw-r--r--   0 root         (0) root         (0)     2227 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.pre-commit-hooks/check-cli-examples.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.pre-commit-hooks/copyright-headers.py
+-rw-r--r--   0 root         (0) root         (0)     2092 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.pre-commit-hooks/make-autodocs.py
+-rw-r--r--   0 root         (0) root         (0)      579 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.pre-commit-hooks/sort-pylint-spelling-words.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/.pylint-spelling-words
+-rw-r--r--   0 root         (0) root         (0)     3867 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/CHANGELOG.rst
+-rw-r--r--   0 root         (0) root         (0)     5256 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)     2487 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)     9283 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      549 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/NOTICE
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2052 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/changelog/
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/changelog/_template.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/_static/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)      164 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/all.rst
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/changelog.rst
+-rw-r--r--   0 root         (0) root         (0)     6553 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      200 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/contents.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/ref/
+-rw-r--r--   0 root         (0) root         (0)       46 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/ref/modules.rst
+-rw-r--r--   0 root         (0) root         (0)      720 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/ref/saf.collect.rst
+-rw-r--r--   0 root         (0) root         (0)      557 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/ref/saf.forward.rst
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/ref/saf.process.rst
+-rw-r--r--   0 root         (0) root         (0)      861 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/ref/saf.rst
+-rw-r--r--   0 root         (0) root         (0)      346 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/ref/saf.saltext.engines.rst
+-rw-r--r--   0 root         (0) root         (0)      202 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/ref/saf.saltext.rst
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/ref/saf.utils.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/docs/sitevars.rst
+-rw-r--r--   0 root         (0) root         (0)    21298 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     6080 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      428 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/pytest.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/requirements/
+-rw-r--r--   0 root         (0) root         (0)      176 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/requirements/base.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/requirements/build.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/requirements/changelog.txt
+-rw-r--r--   0 root         (0) root         (0)      188 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/requirements/dev.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/requirements/docs-auto.txt
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/requirements/tests.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/requirements/tools.txt
+-rw-r--r--   0 root         (0) root         (0)     3249 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      198 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/
+-rw-r--r--   0 root         (0) root         (0)      914 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/collect/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/collect/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2618 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/collect/beacons.py
+-rw-r--r--   0 root         (0) root         (0)     3082 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/collect/file.py
+-rw-r--r--   0 root         (0) root         (0)     1473 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/collect/salt_exec.py
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/collect/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/forward/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/forward/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/forward/disk.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/forward/noop.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/forward/test.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/manager.py
+-rw-r--r--   0 root         (0) root         (0)    10331 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/models.py
+-rw-r--r--   0 root         (0) root         (0)     7792 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/plugins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/process/jupyter_notebook.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/process/regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)     4490 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/process/shannon_mask.py
+-rw-r--r--   0 root         (0) root         (0)     2931 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/process/test.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/saltext/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/saltext/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/saltext/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/saltext/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2165 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/saltext/engines/analytics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/utils/dt.py
+-rw-r--r--   0 root         (0) root         (0)     5542 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/utils/eventbus.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/saf/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3762 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      430 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      652 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      738 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/beacons/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/beacons/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/beacons/test_memusage.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/beacons/test_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/beacons/test_status.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/salt_exec/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/salt_exec/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/salt_exec/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1734 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/salt_exec/test_arg.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/salt_exec/test_collatz.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/collectors/salt_exec/test_config_get.py
+-rw-r--r--   0 root         (0) root         (0)     1399 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/engines/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/e2e/engines/test_engine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/functional/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/functional/collectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/functional/collectors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1236 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/functional/collectors/test_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/functional/processors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/functional/processors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1183 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/functional/processors/test_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/collectors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/collectors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/collectors/test_multiple.py
+-rw-r--r--   0 root         (0) root         (0)     1782 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/forwarders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/forwarders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/forwarders/test_concurrency.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/manager/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/manager/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      930 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/manager/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/manager/test_disabled_pipeline.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/manager/test_enabled_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/processors/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/processors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1796 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/integration/processors/test_chained.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/forwarders/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/forwarders/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/forwarders/test_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/process/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/process/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3803 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/process/test_regex_mask.py
+-rw-r--r--   0 root         (0) root         (0)     5436 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/process/test_shannon_mask.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/salt/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/salt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/salt/engines/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tests/unit/salt/engines/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tools/
+-rw-r--r--   0 root         (0) root         (0)       90 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tools/.ruff.toml
+-rw-r--r--   0 root         (0) root         (0)      334 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6780 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tools/ci.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-06-01 19:13:59.000000 salt-analytics-framework-0.5.0/tools/pre_commit.py
```

### Comparing `salt-analytics-framework-0.4.0/.coveragerc` & `salt-analytics-framework-0.5.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/.github/actions/setup-actionlint/action.yml` & `salt-analytics-framework-0.5.0/.github/actions/setup-actionlint/action.yml`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/.github/workflows/ci.yml` & `salt-analytics-framework-0.5.0/.github/workflows/ci.yml`

 * *Files 20% similar despite different names*

```diff
@@ -81,22 +81,30 @@
     timeout-minutes: 15
 
     strategy:
       fail-fast: false
       max-parallel: 10
       matrix:
         include:
-          - {"salt-version": "3005.0", "python-version": "3.7", "source": "pypi"}
-          - {"salt-version": "3005.0", "python-version": "3.8", "source": "pypi"}
-          - {"salt-version": "3005.0", "python-version": "3.9", "source": "pypi"}
-          - {"salt-version": "3006.0", "python-version": "3.7", "source": "pypi"}
-          - {"salt-version": "3006.0", "python-version": "3.8", "source": "pypi"}
-          - {"salt-version": "3006.0", "python-version": "3.9", "source": "pypi"}
-          - {"salt-version": "3006.0", "python-version": "3.10", "source": "pypi"}
-          - {"salt-version": "3006.x", "python-version": "3.10", "source": "onedir"}
+          - {"salt-version": "3005.0", "python-version": "3.7", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3005.0", "python-version": "3.7", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3005.0", "python-version": "3.8", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3005.0", "python-version": "3.8", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3005.0", "python-version": "3.9", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3005.0", "python-version": "3.9", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.7", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.7", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.8", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.8", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.9", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.9", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.10", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.10", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.x", "python-version": "3.10", "testsuite": "core", "source": "onedir"}
+          - {"salt-version": "3006.x", "python-version": "3.10", "testsuite": "examples", "source": "onedir"}
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
@@ -117,111 +125,152 @@
       run: |
         tools ci download-onedir --platform ${{ runner.os }} --arch ${{ runner.arch }} ${{ matrix.salt-version }}
 
     - name: Install Test Requirements
       env:
         SALT_REQUIREMENT: salt~=${{ matrix.salt-version }}
       run: |
-        nox --force-color -e tests-${{ matrix.source == 'onedir' && 'onedir' || '3' }} --install-only
+        nox --force-color -e tests${{ matrix.testsuite == 'examples' && '-examples' || '' }}-${{ matrix.source == 'onedir' && 'onedir' || '3' }} --install-only
 
     - name: Test
       env:
         SALT_REQUIREMENT: salt~=${{ matrix.salt-version }}
         SKIP_REQUIREMENTS_INSTALL: YES
       run: |
-        nox --force-color -e tests-${{ matrix.source == 'onedir' && 'onedir' || '3' }} -- -vv tests/
+        nox --force-color -e tests${{ matrix.testsuite == 'examples' && '-examples' || '' }}-${{ matrix.source == 'onedir' && 'onedir' || '3' }} -- -vv
 
     - name: Upload Logs
       if: always()
       uses: actions/upload-artifact@main
       with:
-        name: runtests-${{ runner.os }}-${{ matrix.python-version }}-salt-${{ matrix.salt-version }}-${{ matrix.source }}.log
+        name: runtests-${{ runner.os }}-${{ matrix.python-version }}-salt-${{ matrix.salt-version }}-${{ matrix.source }}${{ matrix.testsuite == 'examples' && '-examples' || '' }}.log
         path: artifacts/runtests-*.log
 
 
-#  windows:
-#    name: Windows
-#    runs-on: windows-latest
-#    needs: Pre-Commit
-#
-#    timeout-minutes: 40
-#
-#    strategy:
-#      fail-fast: false
-#      max-parallel: 3
-#      matrix:
-#        include:
-#          - {"salt-version": "3005.0", "python-version": "3.8", "source": "pypi"}
-#          - {"salt-version": "3005.0", "python-version": "3.9", "source": "pypi"}
-#          - {"salt-version": "3006.0", "python-version": "3.8", "source": "pypi"}
-#          - {"salt-version": "3006.0", "python-version": "3.9", "source": "pypi"}
-#          - {"salt-version": "3006.0", "python-version": "3.10", "source": "pypi"}
-#          - {"salt-version": "3006.x", "python-version": "3.10", "source": "onedir"}
-#
-#    steps:
-#    - uses: actions/checkout@v3
-#
-#    - name: Set up Python ${{ matrix.python-version }}
-#      uses: actions/setup-python@v4
-#      with:
-#        python-version: ${{ matrix.python-version }}
-#
-#    - name: Install Nox
-#      run: |
-#        python -m pip install --upgrade pip
-#        pip install nox
-#
-#    - name: Install `tools` command
-#      if: ${{ matrix.source == 'onedir' }}
-#      run: |
-#        python -m pip install -r requirements/tools.txt
-#
-#    - name: Download Salt Onedir
-#      if: ${{ matrix.source == 'onedir' }}
-#      run: |
-#        tools ci download-onedir --platform ${{ runner.os }} --arch ${{ runner.arch }} ${{ matrix.salt-version }}
-#
-#    - name: Install Test Requirements
-#      env:
-#        SALT_REQUIREMENT: salt~=${{ matrix.salt-version }}
-#        EXTRA_REQUIREMENTS_INSTALL: Cython
-#      run: |
-#        nox --force-color -e tests-${{ matrix.source == 'onedir' && 'onedir' || '3' }} --install-only
-#
-#    - name: Test
-#      env:
-#        SALT_REQUIREMENT: salt~=${{ matrix.salt-version }}
-#        SKIP_REQUIREMENTS_INSTALL: YES
-#      run: |
-#        nox --force-color -e tests-${{ matrix.source == 'onedir' && 'onedir' || '3' }} -- -vv tests/
-#
-#    - name: Upload Logs
-#      if: always()
-#      uses: actions/upload-artifact@main
-#      with:
-#        name: runtests-${{ runner.os }}-${{ matrix.python-version }}-salt-${{ matrix.salt-version }}-${{ matrix.source }}.log
-#        path: artifacts/runtests-*.log
+  windows:
+    name: Windows
+    runs-on: windows-latest
+    needs: Pre-Commit
+
+    timeout-minutes: 40
+
+    strategy:
+      fail-fast: false
+      max-parallel: 10
+      matrix:
+        include:
+          - {"salt-version": "3005.0", "python-version": "3.8", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3005.0", "python-version": "3.8", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.8", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.8", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.9", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.9", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.10", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.10", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.x", "python-version": "3.10", "testsuite": "core", "source": "onedir"}
+          - {"salt-version": "3006.x", "python-version": "3.10", "testsuite": "examples", "source": "onedir"}
+
+    steps:
+    - uses: actions/checkout@v3
+
+    - name: Set up Python ${{ matrix.python-version }}
+      uses: actions/setup-python@v4
+      with:
+        python-version: ${{ matrix.python-version }}
+
+    - name: Install Nox
+      run: |
+        python -m pip install --upgrade pip
+        pip install nox
+
+    - name: Install `tools` command
+      if: ${{ matrix.source == 'onedir' }}
+      shell: bash
+      run: |
+        python -m pip install -r requirements/tools.txt
+
+    - name: Download Salt Onedir
+      if: ${{ matrix.source == 'onedir' }}
+      shell: bash
+      run: |
+        tools ci download-onedir --platform ${{ runner.os }} --arch ${{ runner.arch }} ${{ matrix.salt-version }}
+
+    - name: Download libeay32.dll
+      shell: bash
+      if: ${{ matrix.python-version == '3.8' && startswith(matrix.salt-version, '3005') }}
+      run: |
+        export PY_LOC=$(which python.exe)
+        echo ${PY_LOC}
+        export PY_DIR=$(dirname ${PY_LOC})
+        echo ${PY_DIR}
+        curl https://repo.saltproject.io/windows/dependencies/64/libeay32.dll --output ${PY_DIR}/libeay32.dll
+        ls -l ${PY_DIR}
+
+    - name: Define test session
+      shell: bash
+      id: define-test-session
+      run: echo "test-session=tests${{ matrix.testsuite == 'examples' && '-examples' || '' }}-${{ matrix.source == 'onedir' && 'onedir' || '3' }}" >> "$GITHUB_OUTPUT"
+
+    - name: Install Test Requirements
+      shell: bash
+      env:
+        SALT_REQUIREMENT: salt~=${{ matrix.salt-version }}
+        EXTRA_REQUIREMENTS_INSTALL: Cython
+      run: |
+        export PATH="/C/Program Files (x86)/Windows Kits/10/bin/10.0.18362.0/x64;$PATH"
+        nox --force-color --envdir 'C:\.nox' -e ${{ steps.define-test-session.outputs.test-session }} --install-only
+
+    - name: Patch salt/utils/win_network.py
+      shell: bash
+      if: ${{ startswith(matrix.salt-version, '3006') }}
+      run: |
+        if [ "${{ matrix.source }}" == "pypi" ]; then
+          patch 'C:\.nox\${{ steps.define-test-session.outputs.test-session }}\lib\site-packages\salt\utils\win_network.py' ./.github/patches/win_network.patch
+        else
+          patch '.\artifacts\salt\lib\site-packages\salt\utils\win_network.py' ./.github/patches/win_network.patch
+        fi
+
+    - name: Test
+      shell: bash
+      env:
+        SALT_REQUIREMENT: salt~=${{ matrix.salt-version }}
+        SKIP_REQUIREMENTS_INSTALL: YES
+      run: |
+        export PATH="/C/Program Files (x86)/Windows Kits/10/bin/10.0.18362.0/x64;$PATH"
+        echo $PATH
+        nox --force-color --envdir 'C:\.nox' -e ${{ steps.define-test-session.outputs.test-session }}
+
+    - name: Upload Logs
+      if: always()
+      uses: actions/upload-artifact@main
+      with:
+        name: runtests-${{ runner.os }}-${{ matrix.python-version }}-salt-${{ matrix.salt-version }}-${{ matrix.source }}${{ matrix.testsuite == 'examples' && '-examples' || '' }}.log
+        path: artifacts/runtests-*.log
 
 
   macos:
     name: MacOS
     runs-on: macOS-latest
     needs: Pre-Commit
 
     timeout-minutes: 40
 
     strategy:
       fail-fast: false
       max-parallel: 6
       matrix:
         include:
-          - {"salt-version": "3005.0", "python-version": "3.9", "source": "pypi"}
-          - {"salt-version": "3006.0", "python-version": "3.9", "source": "pypi"}
-          - {"salt-version": "3006.0", "python-version": "3.10", "source": "pypi"}
-          - {"salt-version": "3006.x", "python-version": "3.10", "source": "onedir"}
+          - {"salt-version": "3005.0", "python-version": "3.9", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3005.0", "python-version": "3.9", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.9", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.9", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.10", "testsuite": "core", "source": "pypi"}
+          - {"salt-version": "3006.0", "python-version": "3.10", "testsuite": "examples", "source": "pypi"}
+          - {"salt-version": "3006.x", "python-version": "3.10", "testsuite": "core", "source": "onedir"}
+          - {"salt-version": "3006.x", "python-version": "3.10", "testsuite": "examples", "source": "onedir"}
 
     steps:
     - uses: actions/checkout@v3
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
@@ -242,37 +291,37 @@
       run: |
         tools ci download-onedir --platform ${{ runner.os }} --arch ${{ runner.arch }} ${{ matrix.salt-version }}
 
     - name: Install Test Requirements
       env:
         SALT_REQUIREMENT: salt~=${{ matrix.salt-version }}
       run: |
-        nox --force-color -e tests-${{ matrix.source == 'onedir' && 'onedir' || '3' }} --install-only
+        nox --force-color -e tests${{ matrix.testsuite == 'examples' && '-examples' || '' }}-${{ matrix.source == 'onedir' && 'onedir' || '3' }} --install-only
 
     - name: Test
       env:
         SALT_REQUIREMENT: salt~=${{ matrix.salt-version }}
         SKIP_REQUIREMENTS_INSTALL: YES
       run: |
-        nox --force-color -e tests-${{ matrix.source == 'onedir' && 'onedir' || '3' }} -- -vv tests/
+        nox --force-color -e tests${{ matrix.testsuite == 'examples' && '-examples' || '' }}-${{ matrix.source == 'onedir' && 'onedir' || '3' }} -- -vv
 
     - name: Upload Logs
       if: always()
       uses: actions/upload-artifact@main
       with:
-        name: runtests-${{ runner.os }}-${{ matrix.python-version }}-salt-${{ matrix.salt-version }}-${{ matrix.source }}.log
+        name: runtests-${{ runner.os }}-${{ matrix.python-version }}-salt-${{ matrix.salt-version }}-${{ matrix.source }}${{ matrix.testsuite == 'examples' && '-examples' || '' }}.log
         path: artifacts/runtests-*.log
 
   build:
     name: Build Package
     runs-on: ubuntu-latest
     needs:
       - docs
       - linux
-#      - windows
+      - windows
       - macos
     steps:
     - uses: actions/checkout@v3
       with:
         fetch-depth: 0
     - name: Set up Python
       uses: actions/setup-python@v4
```

### Comparing `salt-analytics-framework-0.4.0/.gitignore` & `salt-analytics-framework-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/.pre-commit-config.yaml` & `salt-analytics-framework-0.5.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -65,14 +65,21 @@
           - pre-commit
           - actionlint
         additional_dependencies:
           - boto3==1.21.46
           - pyyaml==6.0
           - jinja2==3.1.2
           - packaging==23.0
+      - id: tools
+        alias: examples-requirements
+        name: Collect examples requirements
+        files: "^examples/requirements/"
+        args:
+          - pre-commit
+          - examples-requirements
 
   # ----- Code Formatting and Analysis ---------------------------------------------------------->
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.265"
     hooks:
       - id: ruff
         args:
@@ -96,15 +103,15 @@
           - black==23.3.0
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.2.0
     hooks:
       - id: mypy
         name: Run mypy against the code base
-        files: ^(src/|tests/).*\.py$
+        files: ^(src/|tests/|examples/).*\.py$
         args: []
         additional_dependencies:
           - types-attrs
           - types-setuptools
           - pydantic
           - types-aiofiles
           - aiostream
```

### Comparing `salt-analytics-framework-0.4.0/.pre-commit-hooks/check-changelog-entries.py` & `salt-analytics-framework-0.5.0/.pre-commit-hooks/check-changelog-entries.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/.pre-commit-hooks/check-cli-examples.py` & `salt-analytics-framework-0.5.0/.pre-commit-hooks/check-cli-examples.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/.pre-commit-hooks/copyright-headers.py` & `salt-analytics-framework-0.5.0/.pre-commit-hooks/copyright-headers.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/.pre-commit-hooks/make-autodocs.py` & `salt-analytics-framework-0.5.0/.pre-commit-hooks/make-autodocs.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/.pre-commit-hooks/sort-pylint-spelling-words.py` & `salt-analytics-framework-0.5.0/.pre-commit-hooks/sort-pylint-spelling-words.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/.pylint-spelling-words` & `salt-analytics-framework-0.5.0/.pylint-spelling-words`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/CHANGELOG.rst` & `salt-analytics-framework-0.5.0/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,47 @@
 **Deprecations** section of releases.
 
 .. towncrier-draft-entries::
 
 .. towncrier release notes start
 
 
+0.5.0 (2023-06-01)
+==================
+
+Features
+--------
+
+- `#54 <https://github.com/saltstack/pytest-skip-markers/issues/54>`_: Add a Jupyter notebook processor that allows running parameterized notebooks using `papermill`
+
+
+
+Improvements
+------------
+
+- `#46 <https://github.com/saltstack/pytest-skip-markers/issues/46>`_: Allow multiple collectors to feed data into the processors chain
+
+- `#47 <https://github.com/saltstack/pytest-skip-markers/issues/47>`_: Forwarders always run concurrently now
+
+- `#48 <https://github.com/saltstack/pytest-skip-markers/issues/48>`_: Create a test event collector(generator)
+
+- `#49 <https://github.com/saltstack/pytest-skip-markers/issues/49>`_: Turn the `noop` processor into the `test` event processor(generator)
+
+- `#50 <https://github.com/saltstack/pytest-skip-markers/issues/50>`_: Allow defining if a pipeline should restart or not when it ends or when it fails during processing.
+
+- `#52 <https://github.com/saltstack/pytest-skip-markers/issues/52>`_: Chain processors asynchronously
+
+
+
+Trivial/Internal Changes
+------------------------
+
+- `#47 <https://github.com/saltstack/pytest-skip-markers/issues/47>`_: Add a timed test case to verify concurrency
+
+
 0.4.0 (2023-05-18)
 ==================
 
 Improvements
 ------------
 
 - `#41 <https://github.com/saltstack/pytest-skip-markers/issues/41>`_: AsyncIO cooperative file reads/writes. Support glob matching on paths.
```

### Comparing `salt-analytics-framework-0.4.0/CODE_OF_CONDUCT.md` & `salt-analytics-framework-0.5.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/CONTRIBUTING.md` & `salt-analytics-framework-0.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/LICENSE` & `salt-analytics-framework-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/NOTICE` & `salt-analytics-framework-0.5.0/NOTICE`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/PKG-INFO` & `salt-analytics-framework-0.5.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.4.0
+Version: 0.5.0
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
@@ -115,15 +115,22 @@
 
 The salt-analytics-framework project team welcomes contributions from the community.
 For more detailed information, refer to `CONTRIBUTING`_.
 
 .. _salt: https://github.com/saltstack/salt
 .. _engine: https://docs.saltproject.io/en/latest/topics/engines/index.html
 .. _CONTRIBUTING: https://github.com/saltstack/salt-analytics-framework/blob/main/CONTRIBUTING.md
+.. _examples: https://github.com/saltstack/salt-analytics-framework/blob/main/examples
 
 ..
    include-ends-here
 
 Documentation
 =============
 
 The full documentation can be seen `here <https://salt-analytics-framework.readthedocs.io>`_.
+
+
+Examples
+========
+
+Some examples of custom pipelines are provided.  You can find them at `examples`_.
```

### Comparing `salt-analytics-framework-0.4.0/README.rst` & `salt-analytics-framework-0.5.0/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -82,15 +82,22 @@
 
 The salt-analytics-framework project team welcomes contributions from the community.
 For more detailed information, refer to `CONTRIBUTING`_.
 
 .. _salt: https://github.com/saltstack/salt
 .. _engine: https://docs.saltproject.io/en/latest/topics/engines/index.html
 .. _CONTRIBUTING: https://github.com/saltstack/salt-analytics-framework/blob/main/CONTRIBUTING.md
+.. _examples: https://github.com/saltstack/salt-analytics-framework/blob/main/examples
 
 ..
    include-ends-here
 
 Documentation
 =============
 
 The full documentation can be seen `here <https://salt-analytics-framework.readthedocs.io>`_.
+
+
+Examples
+========
+
+Some examples of custom pipelines are provided.  You can find them at `examples`_.
```

### Comparing `salt-analytics-framework-0.4.0/changelog/_template.rst` & `salt-analytics-framework-0.5.0/changelog/_template.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/docs/Makefile` & `salt-analytics-framework-0.5.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/docs/conf.py` & `salt-analytics-framework-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/docs/index.rst` & `salt-analytics-framework-0.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/docs/make.bat` & `salt-analytics-framework-0.5.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/docs/ref/saf.collect.rst` & `salt-analytics-framework-0.5.0/docs/ref/saf.collect.rst`

 * *Files 15% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 -----------------------
 
 .. automodule:: saf.collect.file
    :members:
    :undoc-members:
    :show-inheritance:
 
-saf.collect.noop module
+saf.collect.test module
 -----------------------
 
-.. automodule:: saf.collect.noop
+.. automodule:: saf.collect.test
    :members:
    :undoc-members:
    :show-inheritance:
 
 saf.collect.salt\_exec module
 -----------------------------
```

### Comparing `salt-analytics-framework-0.4.0/docs/ref/saf.forward.rst` & `salt-analytics-framework-0.5.0/docs/ref/saf.forward.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/docs/ref/saf.process.rst` & `salt-analytics-framework-0.5.0/docs/ref/saf.process.rst`

 * *Files 20% similar despite different names*

```diff
@@ -5,18 +5,18 @@
    :members:
    :undoc-members:
    :show-inheritance:
 
 Submodules
 ----------
 
-saf.process.noop module
+saf.process.test module
 -----------------------
 
-.. automodule:: saf.process.noop
+.. automodule:: saf.process.test
    :members:
    :undoc-members:
    :show-inheritance:
 
 saf.process.regex\_mask module
 ------------------------------
```

### Comparing `salt-analytics-framework-0.4.0/docs/ref/saf.rst` & `salt-analytics-framework-0.5.0/docs/ref/saf.rst`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/noxfile.py` & `salt-analytics-framework-0.5.0/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,16 @@
 RUNTESTS_LOGFILE = ARTIFACTS_DIR / "runtests-{}.log".format(
     datetime.datetime.now().strftime("%Y%m%d%H%M%S.%f")
 )
 COVERAGE_REPORT_DB = REPO_ROOT / ".coverage"
 COVERAGE_REPORT_PROJECT = ARTIFACTS_DIR.relative_to(REPO_ROOT) / "coverage-project.xml"
 COVERAGE_REPORT_TESTS = ARTIFACTS_DIR.relative_to(REPO_ROOT) / "coverage-tests.xml"
 JUNIT_REPORT = ARTIFACTS_DIR.relative_to(REPO_ROOT) / "junit-report.xml"
+EXAMPLES_EXTENSION_DIR = REPO_ROOT / "examples"
+EXAMPLES_EXTENSION_TESTS_DIR = REPO_ROOT / "tests" / "examples"
 
 
 def _get_session_python_version_info(session):
     try:
         version_info = session._runner._real_python_version_info
     except AttributeError:
         session_py_version = session.run_always(
@@ -92,14 +94,15 @@
     session,
     *passed_requirements,
     install_coverage_requirements=True,
     install_test_requirements=True,
     install_source=False,
     install_salt=True,
     install_extras=None,
+    install_examples=True,
     onedir=False,
 ):
     install_extras = install_extras or []
     if SKIP_REQUIREMENTS_INSTALL is False:
         # Always have the wheel package installed
         session.install("--progress-bar=off", "setuptools>=65.6.3,<66", silent=PIP_INSTALL_SILENT)
         session.install("--progress-bar=off", "wheel", silent=PIP_INSTALL_SILENT)
@@ -124,30 +127,41 @@
 
         if install_test_requirements:
             install_extras.append("tests")
 
         if passed_requirements:
             session.install("--progress-bar=off", *passed_requirements, silent=PIP_INSTALL_SILENT)
 
+        if install_examples:
+            session.install(
+                "--progress-bar=off",
+                "-r",
+                f"{EXAMPLES_EXTENSION_DIR / 'requirements' / 'all.txt'}",
+                silent=PIP_INSTALL_SILENT,
+            )
+            session.install(
+                "--progress-bar=off", f"{EXAMPLES_EXTENSION_DIR}", silent=PIP_INSTALL_SILENT
+            )
+
         if install_source:
             pkg = "."
             if install_extras:
                 pkg += f"[{','.join(install_extras)}]"
             args = ["--progress-bar=off"]
             if onedir is False:
                 args.append("-e")
             args.append(pkg)
             session.install(*args, silent=PIP_INSTALL_SILENT)
         elif install_extras:
             pkg = f".[{','.join(install_extras)}]"
             session.install("--progress-bar=off", pkg, silent=PIP_INSTALL_SILENT)
 
 
-def _tests(session, onedir=False):
-    _install_requirements(session, install_source=True, onedir=onedir)
+def _tests(session, onedir=False, examples=False):
+    _install_requirements(session, install_source=True, onedir=onedir, install_examples=examples)
 
     sitecustomize_dir = session.run("salt-factories", "--coverage", silent=True, log=False)
     python_path_env_var = os.environ.get("PYTHONPATH") or None
     if python_path_env_var is None:
         python_path_env_var = sitecustomize_dir
     else:
         python_path_entries = python_path_env_var.split(os.pathsep)
@@ -178,40 +192,41 @@
         "--showlocals",
         "--strict-markers",
         "-ra",
         "-s",
     ]
     if session._runner.global_config.forcecolor:
         args.append("--color=yes")
+    tests_root = pathlib.Path("examples", "tests") if examples else pathlib.Path("tests")
     if not session.posargs:
-        args.append("tests/")
+        args.append(str(tests_root))
     else:
         for arg in session.posargs:
             if arg.startswith("--color") and args[0].startswith("--color"):
                 args.pop(0)
             args.append(arg)
         for arg in session.posargs:
             if arg.startswith("-"):
                 continue
-            if arg.startswith(f"tests{os.sep}"):
+            if arg.startswith(str(tests_root)):
                 break
             try:
-                pathlib.Path(arg).resolve().relative_to(REPO_ROOT / "tests")
+                pathlib.Path(arg).resolve().relative_to(REPO_ROOT / tests_root)
                 break
             except ValueError:
                 continue
         else:
-            args.append("tests/")
+            args.append(tests_root)
+
     try:
         session.run("coverage", "run", "-m", "pytest", *args, env=env)
     finally:
         # Always combine and generate the XML coverage report
         with contextlib.suppress(CommandFailed):
             session.run("coverage", "combine")
-
         try:
             # Generate report for salt code coverage
             session.run(
                 "coverage",
                 "xml",
                 "-o",
                 str(COVERAGE_REPORT_PROJECT),
@@ -239,15 +254,15 @@
                 # Move the coverage DB to artifacts/coverage in order for it to be archived by CI
                 if COVERAGE_REPORT_DB.exists():
                     shutil.move(
                         str(COVERAGE_REPORT_DB), str(ARTIFACTS_DIR / COVERAGE_REPORT_DB.name)
                     )
         except CommandFailed as exc:
             # Tracking code coverage is still not working that well
-            if onedir is False:
+            if onedir is False and examples is False:
                 raise exc from None
 
 
 @nox.session(python=PYTHON_VERSIONS)
 def tests(session):
     _tests(session, onedir=False)
 
@@ -264,14 +279,35 @@
                 ONEDIR_ARTIFACT_PATH.relative_to(REPO_ROOT)
             )
         )
 
     _tests(session, onedir=True)
 
 
+@nox.session(python=PYTHON_VERSIONS, name="tests-examples")
+def tests_examples(session):
+    _tests(session, onedir=False, examples=True)
+
+
+@nox.session(
+    python=str(ONEDIR_PYTHON_PATH),
+    name="tests-examples-onedir",
+    venv_params=["--system-site-packages"],
+)
+def test_onedir_examples(session):
+    if not ONEDIR_ARTIFACT_PATH.exists():
+        session.error(
+            "The salt onedir artifact, expected to be in '{}', was not found".format(
+                ONEDIR_ARTIFACT_PATH.relative_to(REPO_ROOT)
+            )
+        )
+
+    _tests(session, onedir=True, examples=True)
+
+
 class Tee:
     """
     Python class to mimic linux tee behavior.
     """
 
     def __init__(self, first, second) -> None:
         self._first = first
```

### Comparing `salt-analytics-framework-0.4.0/pyproject.toml` & `salt-analytics-framework-0.5.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -56,17 +56,19 @@
 show-source = true
 target-version = "py37"
 respect-gitignore = true
 src = [
   "src",
   "tests",
   "tools",
+  "examples",
 ]
 extend-exclude = [
   ".nox/**",
+  "examples/pipelines/**",
 ]
 extend-include = [
   "setup.py",
   "noxfile.py",
   "src/**/*.pyi",
 ]
 ignore = [
@@ -90,14 +92,18 @@
 format = "grouped"
 
 [tool.ruff.per-file-ignores]
 "src/**/*.py" = [
   "D104",   # Missing docstring in public package
   "D107",   # Missing docstring in `__init__`
 ]
+"examples/src/**/*.py" = [
+  "D104",   # Missing docstring in public package
+  "D107",   # Missing docstring in `__init__`
+]
 "src/**/*.pyi" = [
   "D100",   # Missing docstring in public module
 ]
 "src/saf/models.py" = [
   "D106",   # Missing docstring in public nested class
   "SLF001", # Private member accessed"
   "ARG003", # Unused class method argument: `kwargs`
@@ -138,14 +144,31 @@
   "ANN",      # Ignore missing type annotations in tests
   "ARG001",   # Unused function argument
   "D100",     # Missing docstring in public module
   "D103",     # Missing docstring in public function
   "D104",     # Missing docstring in public package
   "DTZ003",   # The use of `datetime.datetime.utcnow()` is not allowed, use `datetime.datetime.now(tz=)` instead
   "PLR2004",  # Magic value used in comparison, consider replacing 3 with a constant variable
+  "PT001",    # use @pytest.fixture() over @pytest.fixture
+  "PT023",    # use @pytest.mark.<blah>() over @pytest.mark.<blah>
+  "RET504",   # Unnecessary variable assignment before `return` statement"
+  "S101",     # Ignore the use of 'assert ...' in tests
+  "S603",     # `subprocess` call: check for execution of untrusted input
+  "SIM117",   # Use a single `with` statement with multiple contexts instead of nested `with` statements
+  "TCH002",   # Move third-party import into a type-checking block
+  "TCH003",   # Move standard library import `pathlib` into a type-checking block
+]
+"examples/tests/**/*.py" = [
+  "ANN",      # Ignore missing type annotations in tests
+  "ARG001",   # Unused function argument
+  "D100",     # Missing docstring in public module
+  "D103",     # Missing docstring in public function
+  "D104",     # Missing docstring in public package
+  "DTZ003",   # The use of `datetime.datetime.utcnow()` is not allowed, use `datetime.datetime.now(tz=)` instead
+  "PLR2004",  # Magic value used in comparison, consider replacing 3 with a constant variable
   "PT001",    # use @pytest.fixture() over @pytest.fixture
   "PT023",    # use @pytest.mark.<blah>() over @pytest.mark.<blah>
   "RET504",   # Unnecessary variable assignment before `return` statement"
   "S101",     # Ignore the use of 'assert ...' in tests
   "S603",     # `subprocess` call: check for execution of untrusted input
   "SIM117",   # Use a single `with` statement with multiple contexts instead of nested `with` statements
   "TCH002",   # Move third-party import into a type-checking block
```

### Comparing `salt-analytics-framework-0.4.0/setup.cfg` & `salt-analytics-framework-0.5.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,23 @@
 [options.package_data]
 saf = py.typed
 
 [options.entry_points]
 salt.loader = 
 	salt-analytics-framework = saf.saltext
 saf.collect = 
-	noop = saf.collect.noop
-	file = saf.collect.file
 	beacons = saf.collect.beacons
+	file = saf.collect.file
 	salt_exec = saf.collect.salt_exec
+	test = saf.collect.test
 saf.process = 
-	noop = saf.process.noop
 	regex_mask = saf.process.regex_mask
 	shannon_mask = saf.process.shannon_mask
+	jupyter_notebook = saf.process.jupyter_notebook
+	test = saf.process.test
 saf.forward = 
 	disk = saf.forward.disk
 	noop = saf.forward.noop
 	test = saf.forward.test
 
 [requirements-files]
 install_requires = requirements/base.txt
@@ -125,14 +126,15 @@
 warn_no_return = True
 warn_return_any = True
 warn_unused_configs = True
 warn_unused_ignores = True
 disallow_any_generics = True
 check_untyped_defs = True
 no_implicit_reexport = True
+explicit_package_bases = True
 plugins = pydantic.mypy
 
 [mypy-saf.*]
 disallow_untyped_defs = True
 
 [mypy-tests.*]
 disallow_untyped_defs = False
```

### Comparing `salt-analytics-framework-0.4.0/src/saf/__init__.py` & `salt-analytics-framework-0.5.0/src/saf/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/saf/collect/beacons.py` & `salt-analytics-framework-0.5.0/src/saf/collect/beacons.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/saf/collect/file.py` & `salt-analytics-framework-0.5.0/src/saf/collect/file.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/saf/collect/salt_exec.py` & `salt-analytics-framework-0.5.0/src/saf/collect/salt_exec.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/saf/forward/disk.py` & `salt-analytics-framework-0.5.0/src/saf/forward/disk.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/saf/forward/noop.py` & `salt-analytics-framework-0.5.0/src/saf/forward/noop.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/saf/forward/test.py` & `salt-analytics-framework-0.5.0/src/saf/forward/test.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 """
 from __future__ import annotations
 
 import asyncio
 import json
 import logging
 import pathlib
+from typing import Any
 from typing import Optional
 from typing import Type
 
+from pydantic import root_validator
+
 from saf.models import CollectedEvent
 from saf.models import ForwardConfigBase
 from saf.models import PipelineRunContext
 
 log = logging.getLogger(__name__)
 
 
@@ -29,14 +32,27 @@
     Test forwarder configuration.
     """
 
     sleep: float = 0.0
     path: Optional[pathlib.Path] = None
     message: Optional[str] = None
     dump_event: bool = False
+    add_event_to_shared_cache: bool = False
+
+    @root_validator
+    @classmethod
+    def _check_mutually_exclusive_parameters(
+        cls: Type[TestForwardConfig], values: dict[str, Any]
+    ) -> dict[str, Any]:
+        path = values.get("path")
+        add_event_to_shared_cache = values.get("add_event_to_shared_cache") or False
+        if path and add_event_to_shared_cache:
+            msg = "The 'path' and 'add_event_to_shared_cache' are mutually exclusive"
+            raise ValueError(msg)
+        return values
 
 
 def get_config_schema() -> Type[TestForwardConfig]:
     """
     Get the noop plugin configuration schema.
     """
     return TestForwardConfig
@@ -50,15 +66,23 @@
     """
     Method called to forward the event.
     """
     config = ctx.config
     log.info("Forwarding using %s: %s", config.name, event)
     if config.sleep > 0:
         await asyncio.sleep(config.sleep)
-    if config.path:
+    if config.add_event_to_shared_cache:
+        log.info(
+            "Storing collected events in `pipeline.shared_cache` under "
+            "the 'collected_events' key."
+        )
+        if "collected_events" not in ctx.shared_cache:
+            ctx.shared_cache["collected_events"] = []
+        ctx.shared_cache["collected_events"].append(event)
+    elif config.path:
         if config.message:
             if config.dump_event:
                 dump_text = json.dumps({config.message: event.dict()})
             else:
                 dump_text = config.message
         elif config.dump_event:
             dump_text = event.json()
```

### Comparing `salt-analytics-framework-0.4.0/src/saf/manager.py` & `salt-analytics-framework-0.5.0/src/saf/manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -82,22 +82,25 @@
         if name not in self.pipelines:
             return f"Cannot start unknown pipeline {name!r}"
         pipeline = self.pipelines[name]
         if pipeline.config.enabled is False:
             return f"Pipeline {name!r} is disabled, skipping start."
         if name in self.pipeline_tasks:
             return f"Pipeline {name!r} is already running"
+        pipeline.__enter__()
         self.pipeline_tasks[name] = self.loop.create_task(pipeline.run())
         return None
 
     async def stop_pipeline(self: MN, name: str) -> str | None:
         """
         Stop a pipeline by name.
         """
         log.info("Stopping pipeline %r", name)
         if name not in self.pipeline_tasks:
             return f"Pipeline {name!r} is not running. Not stopping it."
         task = self.pipeline_tasks.pop(name)
         if task.done() is not True:
             task.cancel()
             await task
+        pipeline = self.pipelines[name]
+        pipeline.__exit__()
         return None
```

### Comparing `salt-analytics-framework-0.4.0/src/saf/models.py` & `salt-analytics-framework-0.5.0/src/saf/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -225,19 +225,19 @@
 
 
 class PipelineConfig(NonMutableConfig):
     """
     Base config schema for pipeline configuration.
     """
 
-    collect: str
+    collect: List[str]
     process: List[str] = Field(default_factory=list)
     forward: List[str]
     enabled: bool = True
-    concurrent_forwarders: bool = True
+    restart: bool = True
 
     _name: str = PrivateAttr()
 
     @property
     def name(self: PC) -> str:
         """
         Return the pipeline name as defined in the configuration file.
@@ -262,14 +262,16 @@
     @validator("pipelines", pre=True)
     @classmethod
     def _validate_pipelines(
         cls: Type[AC], pipelines: Dict[str, Dict[str, Any]]
     ) -> Dict[str, Dict[str, Any]]:
         for name, data in pipelines.items():
             collect = data["collect"]
+            if isinstance(collect, str):
+                collect = [collect]
             process = data.get("process")
             forward = data["forward"]
             if process is None:
                 process = []
             elif isinstance(process, str):
                 process = [process]
             if isinstance(forward, str):
```

### Comparing `salt-analytics-framework-0.4.0/src/saf/pipeline.py` & `salt-analytics-framework-0.5.0/src/saf/pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,18 +3,21 @@
 """
 Salt Analytics Framework Pipeline.
 """
 from __future__ import annotations
 
 import asyncio
 import logging
+from functools import partial
 from typing import TYPE_CHECKING
 from typing import Any
+from typing import AsyncIterator
 from typing import TypeVar
 
+import aiostream.stream
 import backoff
 
 from saf.models import CollectConfigBase
 from saf.models import CollectedEvent
 from saf.models import ForwardConfigBase
 from saf.models import PipelineConfig
 from saf.models import PipelineRunContext
@@ -45,22 +48,29 @@
     """
     Salt Analytics Pipeline.
     """
 
     def __init__(self: P, name: str, config: PipelineConfig) -> None:
         self.name = name
         self.config = config
-        self.collect_config: CollectConfigBase = config.parent.collectors[config.collect]
+        self.collect_configs: list[CollectConfigBase] = []
+        for config_name in config.collect:
+            self.collect_configs.append(config.parent.collectors[config_name])
         self.process_configs: list[ProcessConfigBase] = []
         for config_name in config.process:
             self.process_configs.append(config.parent.processors[config_name])
         self.forward_configs: list[ForwardConfigBase] = []
         for config_name in config.forward:
             self.forward_configs.append(config.parent.forwarders[config_name])
 
+        self.shared_cache: dict[str, Any] = {}
+        self.collect_ctxs: dict[str, PipelineRunContext[CollectConfigBase]] = {}
+        self.process_ctxs: dict[str, PipelineRunContext[ProcessConfigBase]] = {}
+        self.forward_ctxs: dict[str, PipelineRunContext[ForwardConfigBase]] = {}
+
     async def run(self: P) -> None:
         """
         Run the pipeline.
         """
         log.info("Pipeline %r started", self.name)
         while True:
             try:
@@ -70,109 +80,141 @@
                 break
             except Exception:
                 log.exception(
                     "Failed to start the pipeline %s due to an error",
                     self.name,
                 )
                 break
+            if self.config.restart is False:
+                log.info(
+                    "The pipeline %r has the 'restart' config setting set to False. "
+                    "Not restarting it.",
+                    self.name,
+                )
+                break
 
     @backoff.on_exception(
         backoff.expo,
         Exception,
         jitter=backoff.full_jitter,
         max_tries=5,
         giveup=_check_backoff_exception,
         on_backoff=_log_backoff_exception,
     )
     async def _run(self: P) -> None:
-        shared_cache: dict[str, Any] = {}
-        process_ctxs: dict[str, PipelineRunContext[ProcessConfigBase]] = {}
-        forward_ctxs: dict[str, PipelineRunContext[ForwardConfigBase]] = {}
-        collect_ctx: PipelineRunContext[CollectConfigBase] = PipelineRunContext.construct(
-            config=self.collect_config,
-            shared_cache=shared_cache,
-        )
-        try:
-            collect_plugin = self.collect_config.loaded_plugin
-            async for event in collect_plugin.collect(ctx=collect_ctx):
-                events_to_process: list[CollectedEvent] = [event]
-                processed_events: list[CollectedEvent] = []
-                if not self.process_configs:
-                    # Consider all events to process as processed
-                    processed_events.extend(events_to_process)
-                    events_to_process.clear()
-                else:
-                    # Process the event
-                    stop_processing = False
-                    for process_config in self.process_configs:
-                        if stop_processing:
-                            break
-                        if not events_to_process:
-                            events_to_process.extend(processed_events)
-                            processed_events.clear()
-                        if process_config.name not in process_ctxs:
-                            process_ctxs[process_config.name] = PipelineRunContext.construct(
-                                config=process_config,
-                                shared_cache=shared_cache,
-                            )
-                        process_plugin = process_config.loaded_plugin
-                        while events_to_process:
-                            event_to_process = events_to_process.pop(0)
-                            try:
-                                async for processed_event in process_plugin.process(
-                                    ctx=process_ctxs[process_config.name],
-                                    event=event_to_process,
-                                ):
-                                    if processed_event is not None:
-                                        processed_events.append(processed_event)
-                            except Exception:
-                                log.exception(
-                                    "An exception occurred while processing the event. "
-                                    "Stopped processing this event."
-                                )
-                                stop_processing = True
-                                break
-
-                if not processed_events:
-                    # The processor(s) did not return any events to forward
-                    continue
-
-                # Forward the event
-                coros = []
-                for processed_event in processed_events:
-                    for forward_config in self.forward_configs:
-                        if forward_config.name not in forward_ctxs:
-                            forward_ctxs[forward_config.name] = PipelineRunContext.construct(
-                                config=forward_config,
-                                shared_cache=shared_cache,
-                            )
-                        forward_plugin = forward_config.loaded_plugin
-                        coros.append(
-                            self._wrap_forwarder_plugin_call(
-                                forward_plugin,
-                                forward_ctxs[forward_config.name],
-                                processed_event.copy(),
-                            ),
-                        )
-                if self.config.concurrent_forwarders:
-                    await asyncio.gather(*coros)
-                else:
-                    for coro in coros:
-                        await coro
-        finally:
-            shared_cache.clear()
-            process_ctxs.clear()
-            forward_ctxs.clear()
+        self._build_contexts()
+        async for event in self._collectors_stream():
+            async for processed_event in self._pipe_process_events(event):
+                await self._forward_event(processed_event)
+
+    def _build_contexts(self: P) -> None:
+        for collect_config in self.collect_configs:
+            if collect_config.name not in self.collect_ctxs:
+                self.collect_ctxs[collect_config.name] = PipelineRunContext.construct(
+                    config=collect_config,
+                    shared_cache=self.shared_cache,
+                )
+        for process_config in self.process_configs:
+            if process_config.name not in self.process_ctxs:
+                self.process_ctxs[process_config.name] = PipelineRunContext.construct(
+                    config=process_config,
+                    shared_cache=self.shared_cache,
+                )
+        for forward_config in self.forward_configs:
+            if forward_config.name not in self.forward_ctxs:
+                self.forward_ctxs[forward_config.name] = PipelineRunContext.construct(
+                    config=forward_config,
+                    shared_cache=self.shared_cache,
+                )
+
+    async def _collectors_stream(self: P) -> AsyncIterator[CollectedEvent]:
+        collectors = []
+        for collect_config in self.collect_configs:
+            collect_plugin = collect_config.loaded_plugin
+            collectors.append(
+                collect_plugin.collect(
+                    ctx=self.collect_ctxs[collect_config.name],
+                ),
+            )
+        combined = aiostream.stream.merge(*collectors)
+        async with combined.stream() as stream:
+            async for event in stream:
+                yield event
+
+    async def _pipe_process_event(
+        self: P,
+        process_config: ProcessConfigBase,
+        event: CollectedEvent,
+    ) -> AsyncIterator[CollectedEvent]:
+        process_plugin = process_config.loaded_plugin
+        async for processed_event in process_plugin.process(
+            ctx=self.process_ctxs[process_config.name], event=event
+        ):
+            # Allow other coroutines to run
+            await asyncio.sleep(0)
+            if processed_event is not None:
+                yield processed_event
+
+    async def _pipe_process_events(self: P, event: CollectedEvent) -> AsyncIterator[CollectedEvent]:
+        process_configs = list(self.process_configs)
+        process_config = process_configs.pop(0)
+        process = aiostream.stream.chain(self._pipe_process_event(process_config, event))
+        for process_config in process_configs:
+            process |= aiostream.pipe.flatmap(partial(self._pipe_process_event, process_config))
+        if TYPE_CHECKING:
+            assert process
+        async with process.stream() as stream:
+            async for processed_event in stream:
+                # Allow other coroutines to run
+                await asyncio.sleep(0)
+                if processed_event is not None:
+                    yield processed_event
+
+    async def _forward_event(self: P, event: CollectedEvent) -> None:
+        # Forward the event
+        coros = []
+        for forward_config in self.forward_configs:
+            forward_plugin = forward_config.loaded_plugin
+            coros.append(
+                self._wrap_forwarder_plugin_call(
+                    forward_plugin,
+                    self.forward_ctxs[forward_config.name],
+                    # We pass a copy of the event so that any forwarder get's the
+                    # same event and is free to modify it at will
+                    event.copy(),
+                ),
+            )
+        await asyncio.gather(*coros)
 
     async def _wrap_forwarder_plugin_call(
         self: P,
         plugin: ModuleType,
         ctx: PipelineRunContext[ForwardConfigBase],
         event: CollectedEvent,
     ) -> None:
         try:
+            # Allow other coroutines to run
+            await asyncio.sleep(0)
             await plugin.forward(ctx=ctx, event=event)
         except Exception:
             log.exception(
                 "An exception occurred while forwarding the event through config %r",
                 ctx.config,
             )
+
+    def _cleanup(self: P) -> None:
+        self.shared_cache.clear()
+        self.collect_ctxs.clear()
+        self.process_ctxs.clear()
+        self.forward_ctxs.clear()
+
+    def __enter__(self: P) -> P:
+        """
+        Enter pipeline context managert.
+        """
+        return self
+
+    def __exit__(self: P, *_: Any) -> None:  # noqa: ANN401
+        """
+        Exit pipeline context managert.
+        """
+        self._cleanup()
```

### Comparing `salt-analytics-framework-0.4.0/src/saf/plugins.py` & `salt-analytics-framework-0.5.0/src/saf/plugins.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/saf/process/regex_mask.py` & `salt-analytics-framework-0.5.0/src/saf/process/regex_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/saf/process/shannon_mask.py` & `salt-analytics-framework-0.5.0/src/saf/process/shannon_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/saf/saltext/engines/analytics.py` & `salt-analytics-framework-0.5.0/src/saf/saltext/engines/analytics.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/saf/utils/eventbus.py` & `salt-analytics-framework-0.5.0/src/saf/utils/eventbus.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/PKG-INFO` & `salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: salt-analytics-framework
-Version: 0.4.0
+Version: 0.5.0
 Summary: Salt Analytics Framework
 Home-page: https://github.com/saltstack/salt-analytics-framework
 Author: Pedro Algarvio
 Author-email: palgarvio@vmware.com
 License: Apache Software License
 Project-URL: Source, https://github.com/saltstack/salt-analytics-framework
 Project-URL: Tracker, https://github.com/saltstack/salt-analytics-framework/issues
@@ -115,15 +115,22 @@
 
 The salt-analytics-framework project team welcomes contributions from the community.
 For more detailed information, refer to `CONTRIBUTING`_.
 
 .. _salt: https://github.com/saltstack/salt
 .. _engine: https://docs.saltproject.io/en/latest/topics/engines/index.html
 .. _CONTRIBUTING: https://github.com/saltstack/salt-analytics-framework/blob/main/CONTRIBUTING.md
+.. _examples: https://github.com/saltstack/salt-analytics-framework/blob/main/examples
 
 ..
    include-ends-here
 
 Documentation
 =============
 
 The full documentation can be seen `here <https://salt-analytics-framework.readthedocs.io>`_.
+
+
+Examples
+========
+
+Some examples of custom pipelines are provided.  You can find them at `examples`_.
```

### Comparing `salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/SOURCES.txt` & `salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 .bandit
 .coveragerc
-.dockerignore
 .gitignore
 .pre-commit-config.yaml
 .pylint-spelling-words
 CHANGELOG.rst
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
 LICENSE
+MANIFEST.in
 NOTICE
 README.rst
 noxfile.py
 pyproject.toml
 pytest.ini
 setup.cfg
 setup.py
 .github/actionlint.yaml
 .github/actions/setup-actionlint/action.yml
+.github/patches/win_network.patch
 .github/workflows/ci.yml
 .pre-commit-hooks/check-changelog-entries.py
 .pre-commit-hooks/check-cli-examples.py
 .pre-commit-hooks/copyright-headers.py
 .pre-commit-hooks/make-autodocs.py
 .pre-commit-hooks/sort-pylint-spelling-words.py
 changelog/_template.rst
@@ -55,25 +56,25 @@
 src/saf/pipeline.py
 src/saf/plugins.py
 src/saf/py.typed
 src/saf/version.py
 src/saf/collect/__init__.py
 src/saf/collect/beacons.py
 src/saf/collect/file.py
-src/saf/collect/noop.py
 src/saf/collect/salt_exec.py
+src/saf/collect/test.py
 src/saf/forward/__init__.py
 src/saf/forward/disk.py
 src/saf/forward/noop.py
 src/saf/forward/test.py
 src/saf/process/__init__.py
-src/saf/process/noop.py
+src/saf/process/jupyter_notebook.py
 src/saf/process/regex_mask.py
-src/saf/process/regex_mask.pyi
 src/saf/process/shannon_mask.py
+src/saf/process/test.py
 src/saf/saltext/__init__.py
 src/saf/saltext/engines/__init__.py
 src/saf/saltext/engines/analytics.py
 src/saf/utils/__init__.py
 src/saf/utils/dt.py
 src/saf/utils/eventbus.py
 src/salt_analytics_framework.egg-info/PKG-INFO
@@ -81,40 +82,50 @@
 src/salt_analytics_framework.egg-info/dependency_links.txt
 src/salt_analytics_framework.egg-info/entry_points.txt
 src/salt_analytics_framework.egg-info/not-zip-safe
 src/salt_analytics_framework.egg-info/requires.txt
 src/salt_analytics_framework.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
+tests/e2e/__init__.py
+tests/e2e/conftest.py
+tests/e2e/collectors/__init__.py
+tests/e2e/collectors/beacons/__init__.py
+tests/e2e/collectors/beacons/test_memusage.py
+tests/e2e/collectors/beacons/test_multiple.py
+tests/e2e/collectors/beacons/test_status.py
+tests/e2e/collectors/salt_exec/__init__.py
+tests/e2e/collectors/salt_exec/conftest.py
+tests/e2e/collectors/salt_exec/test_arg.py
+tests/e2e/collectors/salt_exec/test_collatz.py
+tests/e2e/collectors/salt_exec/test_config_get.py
+tests/e2e/engines/__init__.py
+tests/e2e/engines/test_engine.py
 tests/functional/__init__.py
-tests/functional/conftest.py
-tests/functional/forwarders/__init__.py
-tests/functional/forwarders/test_concurrency.py
-tests/functional/manager/__init__.py
-tests/functional/manager/conftest.py
-tests/functional/manager/test_disabled_pipeline.py
-tests/functional/manager/test_enabled_pipeline.py
+tests/functional/collectors/__init__.py
+tests/functional/collectors/test_test.py
+tests/functional/processors/__init__.py
+tests/functional/processors/test_test.py
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/collectors/__init__.py
-tests/integration/collectors/beacons/__init__.py
-tests/integration/collectors/beacons/test_memusage.py
-tests/integration/collectors/beacons/test_multiple.py
-tests/integration/collectors/beacons/test_status.py
-tests/integration/collectors/salt_exec/__init__.py
-tests/integration/collectors/salt_exec/conftest.py
-tests/integration/collectors/salt_exec/test_arg.py
-tests/integration/collectors/salt_exec/test_collatz.py
-tests/integration/collectors/salt_exec/test_config_get.py
-tests/integration/engines/__init__.py
-tests/integration/engines/test_engine.py
+tests/integration/collectors/test_multiple.py
+tests/integration/forwarders/__init__.py
+tests/integration/forwarders/test_concurrency.py
+tests/integration/manager/__init__.py
+tests/integration/manager/conftest.py
+tests/integration/manager/test_disabled_pipeline.py
+tests/integration/manager/test_enabled_pipeline.py
+tests/integration/processors/__init__.py
+tests/integration/processors/test_chained.py
 tests/unit/__init__.py
+tests/unit/forwarders/__init__.py
+tests/unit/forwarders/test_test.py
 tests/unit/process/__init__.py
 tests/unit/process/test_regex_mask.py
 tests/unit/process/test_shannon_mask.py
 tests/unit/salt/__init__.py
 tests/unit/salt/engines/__init__.py
 tools/.ruff.toml
 tools/__init__.py
 tools/ci.py
-tools/pre_commit.py
-tools/pre_commit.py~
+tools/pre_commit.py
```

### Comparing `salt-analytics-framework-0.4.0/src/salt_analytics_framework.egg-info/requires.txt` & `salt-analytics-framework-0.5.0/src/salt_analytics_framework.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/tests/__init__.py` & `salt-analytics-framework-0.5.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/tests/conftest.py` & `salt-analytics-framework-0.5.0/tests/conftest.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,14 +21,25 @@
     COVERAGERC_FILE = str(CODE_DIR / ".coveragerc")
     MAYBE_RUN_COVERAGE = sys.argv[0].endswith("pytest.py") or "_COVERAGE_RCFILE" in os.environ
     if MAYBE_RUN_COVERAGE:
         # Flag coverage to track suprocesses by pointing it to the right .coveragerc file
         os.environ["COVERAGE_PROCESS_START"] = str(COVERAGERC_FILE)
 
 
+# ----- PyTest Tempdir Plugin Hooks -------------------------------------------------------------->
+def pytest_tempdir_basename() -> str:
+    """
+    Return the temporary directory basename for the salt test suite.
+    """
+    return "analytics"
+
+
+# <---- PyTest Tempdir Plugin Hooks ---------------------------------------------------------------
+
+
 @pytest.fixture(scope="session")
 def salt_factories_config() -> dict[str, Any]:
     """
     Return a dictionary with the keyword arguments for FactoriesManager.
     """
     if os.environ.get("CI"):
         start_timeout = 120
```

### Comparing `salt-analytics-framework-0.4.0/tests/functional/manager/test_disabled_pipeline.py` & `salt-analytics-framework-0.5.0/tests/integration/manager/test_enabled_pipeline.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,31 +2,36 @@
 # SPDX-License-Identifier: Apache-2.0
 #
 from __future__ import annotations
 
 import pytest
 
 
+@pytest.fixture
+def pipelines_config(pipelines_config, pipeline_name):
+    pipelines_config[pipeline_name]["enabled"] = True
+    return pipelines_config
+
+
 @pytest.mark.asyncio
-async def test_start_disabled_pipeline(manager):
-    pipeline = "my-pipeline"
+async def test_start_disabled_pipeline(manager, pipeline_name):
     # Make sure we have pipelines configured
     assert manager.pipelines
-    assert pipeline in manager.pipelines
-    # Make sure none of those pipelines are running
-    assert not manager.pipeline_tasks
-    result = await manager.start_pipeline("my-pipeline")
+    assert pipeline_name in manager.pipelines
+    # Make sure those pipelines are running
+    assert manager.pipeline_tasks
+    assert pipeline_name in manager.pipeline_tasks
+    result = await manager.start_pipeline(pipeline_name)
     assert result is not None
-    assert result == f"Pipeline '{pipeline}' is disabled, skipping start."
+    assert result == f"Pipeline '{pipeline_name}' is already running"
 
 
 @pytest.mark.asyncio
-async def test_stop_disabled_pipeline(manager):
-    pipeline = "my-pipeline"
+async def test_stop_disabled_pipeline(manager, pipeline_name):
     # Make sure we have pipelines configured
     assert manager.pipelines
-    assert pipeline in manager.pipelines
-    # Make sure none of those pipelines are running
-    assert not manager.pipeline_tasks
-    result = await manager.stop_pipeline("my-pipeline")
-    assert result is not None
-    assert result == f"Pipeline '{pipeline}' is not running. Not stopping it."
+    assert pipeline_name in manager.pipelines
+    # Make sure those pipelines are running
+    assert manager.pipeline_tasks
+    assert pipeline_name in manager.pipeline_tasks
+    result = await manager.stop_pipeline(pipeline_name)
+    assert result is None
```

### Comparing `salt-analytics-framework-0.4.0/tests/functional/manager/test_enabled_pipeline.py` & `salt-analytics-framework-0.5.0/tests/integration/manager/test_disabled_pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,37 +3,34 @@
 #
 from __future__ import annotations
 
 import pytest
 
 
 @pytest.fixture
-def analytics_config_dict(analytics_config_dict):
-    analytics_config_dict["pipelines"]["my-pipeline"]["enabled"] = True
-    return analytics_config_dict
+def pipelines_config(pipelines_config, pipeline_name):
+    pipelines_config[pipeline_name]["enabled"] = False
+    return pipelines_config
 
 
 @pytest.mark.asyncio
-async def test_start_disabled_pipeline(manager):
-    pipeline = "my-pipeline"
+async def test_start_disabled_pipeline(manager, pipeline_name):
     # Make sure we have pipelines configured
     assert manager.pipelines
-    assert pipeline in manager.pipelines
-    # Make sure those pipelines are running
-    assert manager.pipeline_tasks
-    assert pipeline in manager.pipeline_tasks
-    result = await manager.start_pipeline("my-pipeline")
+    assert pipeline_name in manager.pipelines
+    # Make sure none of those pipelines are running
+    assert not manager.pipeline_tasks
+    result = await manager.start_pipeline(pipeline_name)
     assert result is not None
-    assert result == f"Pipeline '{pipeline}' is already running"
+    assert result == f"Pipeline '{pipeline_name}' is disabled, skipping start."
 
 
 @pytest.mark.asyncio
-async def test_stop_disabled_pipeline(manager):
-    pipeline = "my-pipeline"
+async def test_stop_disabled_pipeline(manager, pipeline_name):
     # Make sure we have pipelines configured
     assert manager.pipelines
-    assert pipeline in manager.pipelines
-    # Make sure those pipelines are running
-    assert manager.pipeline_tasks
-    assert pipeline in manager.pipeline_tasks
-    result = await manager.stop_pipeline("my-pipeline")
-    assert result is None
+    assert pipeline_name in manager.pipelines
+    # Make sure none of those pipelines are running
+    assert not manager.pipeline_tasks
+    result = await manager.stop_pipeline(pipeline_name)
+    assert result is not None
+    assert result == f"Pipeline '{pipeline_name}' is not running. Not stopping it."
```

### Comparing `salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_memusage.py` & `salt-analytics-framework-0.5.0/tests/e2e/collectors/beacons/test_memusage.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,28 +29,28 @@
     collectors:
       beacons-collector:
         plugin: beacons
         beacons:
           - memusage
 
     processors:
-      noop-processor:
-        plugin: noop
+      test-processor:
+        plugin: test
 
 
     forwarders:
       disk-forwarder:
         plugin: disk
         path: {}
 
 
     pipelines:
       my-pipeline:
         collect: beacons-collector
-        process: noop-processor
+        process: test-processor
         forward: disk-forwarder
     """.format(
         analytics_events_dump_directory
     )
     with pytest.helpers.temp_file(
         "analytics", contents=analytics_config, directory=factory.config_dir
     ):
```

### Comparing `salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_multiple.py` & `salt-analytics-framework-0.5.0/tests/e2e/collectors/beacons/test_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,62 +14,58 @@
 
 
 @pytest.fixture(scope="module", autouse=True)
 def minion(master: SaltMaster, analytics_events_dump_directory) -> SaltMinion:
     default_config = {
         "engines": ["analytics"],
         "beacons": {
-            "memusage": [
-                {"interval": 0.1},
-                {"percent": "0.01%"},
-            ],
             "status": [
                 {"interval": 0.1},
                 {"time": ["all"]},
                 {"loadavg": ["all"]},
-            ],
+            ]
         },
     }
     factory = master.salt_minion_daemon(random_string("minion-"), defaults=default_config)
     analytics_config = """
     collectors:
       beacons-collector:
         plugin: beacons
         beacons:
-          - "*"
+          - status
 
     processors:
-      noop-processor:
-        plugin: noop
+      test-processor:
+        plugin: test
 
 
     forwarders:
       disk-forwarder:
         plugin: disk
         path: {}
 
 
     pipelines:
       my-pipeline:
         collect: beacons-collector
-        process: noop-processor
+        process: test-processor
         forward: disk-forwarder
     """.format(
         analytics_events_dump_directory
     )
     with pytest.helpers.temp_file(
         "analytics", contents=analytics_config, directory=factory.config_dir
     ):
-        with factory.started("-l", "trace"):
+        with factory.started():
             yield factory
 
 
 def test_pipeline(analytics_events_dump_directory: pathlib.Path):
     timeout = 10
-    missing_beacons = {"status", "memusage"}
+    missing_beacons = {"status"}
     while timeout:
         if not missing_beacons:
             break
         time.sleep(1)
         timeout -= 1
         for path in analytics_events_dump_directory.iterdir():
             event = json.loads(path.read_text())
```

### Comparing `salt-analytics-framework-0.4.0/tests/integration/collectors/beacons/test_status.py` & `salt-analytics-framework-0.5.0/tests/e2e/collectors/beacons/test_multiple.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,58 +14,62 @@
 
 
 @pytest.fixture(scope="module", autouse=True)
 def minion(master: SaltMaster, analytics_events_dump_directory) -> SaltMinion:
     default_config = {
         "engines": ["analytics"],
         "beacons": {
+            "memusage": [
+                {"interval": 0.1},
+                {"percent": "0.01%"},
+            ],
             "status": [
                 {"interval": 0.1},
                 {"time": ["all"]},
                 {"loadavg": ["all"]},
-            ]
+            ],
         },
     }
     factory = master.salt_minion_daemon(random_string("minion-"), defaults=default_config)
     analytics_config = """
     collectors:
       beacons-collector:
         plugin: beacons
         beacons:
-          - status
+          - "*"
 
     processors:
-      noop-processor:
-        plugin: noop
+      test-processor:
+        plugin: test
 
 
     forwarders:
       disk-forwarder:
         plugin: disk
         path: {}
 
 
     pipelines:
       my-pipeline:
         collect: beacons-collector
-        process: noop-processor
+        process: test-processor
         forward: disk-forwarder
     """.format(
         analytics_events_dump_directory
     )
     with pytest.helpers.temp_file(
         "analytics", contents=analytics_config, directory=factory.config_dir
     ):
-        with factory.started():
+        with factory.started("-l", "trace"):
             yield factory
 
 
 def test_pipeline(analytics_events_dump_directory: pathlib.Path):
     timeout = 10
-    missing_beacons = {"status"}
+    missing_beacons = {"status", "memusage"}
     while timeout:
         if not missing_beacons:
             break
         time.sleep(1)
         timeout -= 1
         for path in analytics_events_dump_directory.iterdir():
             event = json.loads(path.read_text())
```

### Comparing `salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/conftest.py` & `salt-analytics-framework-0.5.0/tests/e2e/collectors/salt_exec/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_arg.py` & `salt-analytics-framework-0.5.0/tests/e2e/collectors/salt_exec/test_arg.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,29 +29,29 @@
           - []
         kwargs:
           kwarg1: hello
           kwarg2: world
 
 
     processors:
-      noop-processor:
-        plugin: noop
+      test-processor:
+        plugin: test
 
 
     forwarders:
       disk-forwarder:
         plugin: disk
         filename: salt_exec_arg_dump
         path: {}
 
 
     pipelines:
       my-pipeline:
         collect: salt-collector
-        process: noop-processor
+        process: test-processor
         forward: disk-forwarder
     """.format(
         analytics_events_dump_directory
     )
 
 
 def test_pipeline(analytics_events_dump_directory: pathlib.Path):
```

### Comparing `salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_collatz.py` & `salt-analytics-framework-0.5.0/tests/e2e/collectors/salt_exec/test_config_get.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,54 +18,54 @@
 @pytest.fixture(scope="module")
 def analytics_config_contents(analytics_events_dump_directory) -> str:
     return """
     collectors:
       salt-collector:
         plugin: salt_exec
         interval: 1
-        fn: test.collatz
+        fn: config.get
         args:
-          - 5
+          - id
 
 
     processors:
-      noop-processor:
-        plugin: noop
+      test-processor:
+        plugin: test
 
 
     forwarders:
       disk-forwarder:
         plugin: disk
-        filename: salt_exec_collatz_dump
+        filename: salt_exec_config_dump
         path: {}
 
 
     pipelines:
       my-pipeline:
         collect: salt-collector
-        process: noop-processor
+        process: test-processor
         forward: disk-forwarder
     """.format(
         analytics_events_dump_directory
     )
 
 
-def test_pipeline(analytics_events_dump_directory: pathlib.Path):
+def test_pipeline(minion, analytics_events_dump_directory: pathlib.Path):
     """
-    Test output of test.collatz being dumped to disk.
+    Test output of config.get being dumped to disk.
     """
     timeout = 10
-    dumpfile = analytics_events_dump_directory / "salt_exec_collatz_dump"
+    dumpfile = analytics_events_dump_directory / "salt_exec_config_dump"
 
     while timeout:
         time.sleep(1)
         timeout -= 1
         if dumpfile.exists() and dumpfile.read_text().strip():
             break
     else:
         pytest.fail(f"Failed to find dumped events in {analytics_events_dump_directory}")
 
     contents = [
         CollectedEvent.parse_obj(json.loads(i)) for i in dumpfile.read_text().strip().split("\n")
     ]
     for event in contents:
-        assert event.data["ret"][0] == [5, 16, 8, 4, 2]
+        assert event.data["ret"] == minion.id
```

### Comparing `salt-analytics-framework-0.4.0/tests/integration/collectors/salt_exec/test_config_get.py` & `salt-analytics-framework-0.5.0/tests/e2e/collectors/salt_exec/test_collatz.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,54 +18,54 @@
 @pytest.fixture(scope="module")
 def analytics_config_contents(analytics_events_dump_directory) -> str:
     return """
     collectors:
       salt-collector:
         plugin: salt_exec
         interval: 1
-        fn: config.get
+        fn: test.collatz
         args:
-          - id
+          - 5
 
 
     processors:
-      noop-processor:
-        plugin: noop
+      test-processor:
+        plugin: test
 
 
     forwarders:
       disk-forwarder:
         plugin: disk
-        filename: salt_exec_config_dump
+        filename: salt_exec_collatz_dump
         path: {}
 
 
     pipelines:
       my-pipeline:
         collect: salt-collector
-        process: noop-processor
+        process: test-processor
         forward: disk-forwarder
     """.format(
         analytics_events_dump_directory
     )
 
 
-def test_pipeline(minion, analytics_events_dump_directory: pathlib.Path):
+def test_pipeline(analytics_events_dump_directory: pathlib.Path):
     """
-    Test output of config.get being dumped to disk.
+    Test output of test.collatz being dumped to disk.
     """
     timeout = 10
-    dumpfile = analytics_events_dump_directory / "salt_exec_config_dump"
+    dumpfile = analytics_events_dump_directory / "salt_exec_collatz_dump"
 
     while timeout:
         time.sleep(1)
         timeout -= 1
         if dumpfile.exists() and dumpfile.read_text().strip():
             break
     else:
         pytest.fail(f"Failed to find dumped events in {analytics_events_dump_directory}")
 
     contents = [
         CollectedEvent.parse_obj(json.loads(i)) for i in dumpfile.read_text().strip().split("\n")
     ]
     for event in contents:
-        assert event.data["ret"] == minion.id
+        assert event.data["ret"][0] == [5, 16, 8, 4, 2]
```

### Comparing `salt-analytics-framework-0.4.0/tests/integration/conftest.py` & `salt-analytics-framework-0.5.0/tests/e2e/conftest.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/tests/integration/engines/test_engine.py` & `salt-analytics-framework-0.5.0/tests/e2e/engines/test_engine.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,33 +15,33 @@
 def minion(master: SaltMaster, analytics_events_dump_directory) -> SaltMinion:
     default_config = {
         "engines": ["analytics"],
     }
     factory = master.salt_minion_daemon(random_string("minion-"), defaults=default_config)
     analytics_config = """
     collectors:
-      noop-collector:
-        plugin: noop
+      test-collector:
+        plugin: test
         interval: 1
 
     processors:
-      noop-processor:
-        plugin: noop
+      test-processor:
+        plugin: test
 
 
     forwarders:
       disk-forwarder:
         plugin: disk
         path: {}
 
 
     pipelines:
       my-pipeline:
-        collect: noop-collector
-        process: noop-processor
+        collect: test-collector
+        process: test-processor
         forward: disk-forwarder
     """.format(
         analytics_events_dump_directory
     )
     with pytest.helpers.temp_file(
         "analytics", contents=analytics_config, directory=factory.config_dir
     ):
```

### Comparing `salt-analytics-framework-0.4.0/tests/unit/process/test_regex_mask.py` & `salt-analytics-framework-0.5.0/tests/unit/process/test_regex_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/tests/unit/process/test_shannon_mask.py` & `salt-analytics-framework-0.5.0/tests/unit/process/test_shannon_mask.py`

 * *Files identical despite different names*

### Comparing `salt-analytics-framework-0.4.0/tools/ci.py` & `salt-analytics-framework-0.5.0/tools/ci.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 # Copyright 2023 VMware, Inc.
 # SPDX-License-Identifier: Apache-2.0
 """
 These commands are used in the CI pipeline.
 """
 from __future__ import annotations
 
+import contextlib
 import hashlib
 import json
 import logging
 import pathlib
+import shutil
+import sys
 import tempfile
 
 from ptscripts import CWD
 from ptscripts import Context
 from ptscripts import command_group
 
 log = logging.getLogger(__name__)
@@ -77,53 +80,88 @@
         repo_base_url += "/minor"
         ctx.info(f"Targgeting Salt version {salt_version}")
     else:
         salt_version = salt_version.replace(".x", "")
         ctx.info(f"Targetting the latest Salt minor version of {salt_version}")
 
     repo_json_url = f"{repo_base_url}/repo.json"
-    with ctx.web, tempfile.TemporaryDirectory(prefix=f"{salt_version}_release_") as tsd:
-        repo_json_file = _download_file(ctx, repo_json_url, pathlib.Path(tsd, "repo.json"))
+    tempdir_path = pathlib.Path(tempfile.gettempdir())
+    with ctx.web:
+        repo_json_file = _download_file(ctx, repo_json_url, tempdir_path / "repo.json")
         repo_json_data = json.loads(repo_json_file.read_text())
         ctx.info("Contents of the downloaded 'repo.json' file:")
         ctx.print(repo_json_data, soft_wrap=True)
         if salt_version not in repo_json_data:
             ctx.error(f"Could not find the '{salt_version}' key in the downloaded 'repo.json' file")
             ctx.exit(1)
         version_details = repo_json_data[salt_version]
         selected_fname_details: dict[str, str] | None = None
+        if platform == "windows":
+            file_extension = ".zip"
+        else:
+            file_extension = ".tar.xz"
         for _fname, details in version_details.items():
             if details["os"] != platform:
                 continue
             if details["arch"] != arch:
                 continue
+            if not details["name"].endswith(file_extension):
+                continue
             selected_fname_details = details
             break
         else:
             ctx.error(f"Could not find a onedir matching platform {platform!r} and arch {arch!r}")
             ctx.exit(1)
         ctx.info("Selected onedir archive details:")
         ctx.print(selected_fname_details, soft_wrap=True)
         onedir_url = f"{repo_base_url}/{salt_version}/{selected_fname_details['name']}"
         onedir_fpath = _download_file(
-            ctx, onedir_url, pathlib.Path(tsd, selected_fname_details["name"])
+            ctx, onedir_url, tempdir_path / selected_fname_details["name"]
         )
         onedir_checksum = _get_file_checksum(onedir_fpath, "sha512")
         if onedir_checksum != selected_fname_details["SHA512"]:
             ctx.error("The 'sha512' checksum does not match")
             ctx.error(f"{onedir_checksum!r} != {selected_fname_details['SHA512']!r}")
             ctx.exit(1)
 
         ctx.info("The downloaded file checksum matches")
         with ctx.chdir(artifacts_path):
-            ctx.info(f"Extracting {selected_fname_details['name']} to 'artifacts/' ...")
-            ctx.run("tar", "xf", onedir_fpath)
+            ctx.info(f"Extracting {onedir_fpath.name} to 'artifacts/' ...")
+            if platform == "windows":
+                ret = ctx.run(sys.executable, "-m", "zipfile", "-e", str(onedir_fpath), ".")
+                if ret.returncode:
+                    ctx.error(f"Failed to unzip {onedir_fpath.name}")
+                    ctx.exit(1)
+            else:
+                tar = shutil.which("tar")
+                if tar is None:
+                    ctx.error("Could not find the 'tar' binary in path")
+                    ctx.exit(1)
+                ctx.run("tar", "xf", onedir_fpath)
+
+        with contextlib.suppress(PermissionError):
+            onedir_fpath.unlink()
 
 
 def _download_file(ctx: Context, url: str, dest: str, auth: str | None = None) -> str:
+    curl = shutil.which("curl")
+    if curl is not None:
+        ret = ctx.run(curl, "-sS", "-o", str(dest), url)
+        if ret.returncode:
+            ctx.error(f"Failed to download {url}")
+            ctx.exit(1)
+        return dest
+    wget = shutil.which("wget")
+    if wget is not None:
+        with ctx.cwd(dest.parent):
+            ret = ctx.run(wget, "--no-verbose", url)
+            if ret.returncode:
+                ctx.error(f"Failed to download {url}")
+                ctx.exit(1)
+        return dest
     # NOTE the stream=True parameter below
     ctx.info(f"Downloading {url} ...")
     with ctx.web.get(url, stream=True, auth=auth) as r:
         r.raise_for_status()
         with dest.open("wb") as f:
             for chunk in r.iter_content(chunk_size=8192):
                 if chunk:
```

