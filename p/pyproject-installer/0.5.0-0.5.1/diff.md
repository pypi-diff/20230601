# Comparing `tmp/pyproject_installer-0.5.0.tar.gz` & `tmp/pyproject_installer-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject_installer-0.5.0.tar", last modified: Fri Apr 14 12:17:06 2023, max compression
+gzip compressed data, was "pyproject_installer-0.5.1.tar", last modified: Thu Jun  1 14:08:57 2023, max compression
```

## Comparing `pyproject_installer-0.5.0.tar` & `pyproject_installer-0.5.1.tar`

### file list

```diff
@@ -1,87 +1,90 @@
--rw-r--r--   0        0        0       78 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/__init__.py
--rw-r--r--   0        0        0    16053 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/__main__.py
--rw-r--r--   0        0        0      317 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/codes.py
--rw-r--r--   0        0        0      391 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/errors.py
--rw-r--r--   0        0        0       18 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/version.py
--rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/__init__.py
--rw-r--r--   0        0        0      501 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/__init__.py
--rw-r--r--   0        0        0     3266 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_elffile.py
--rw-r--r--   0        0        0     8813 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_manylinux.py
--rw-r--r--   0        0        0     2524 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_musllinux.py
--rw-r--r--   0        0        0     9399 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_parser.py
--rw-r--r--   0        0        0     1431 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_structures.py
--rw-r--r--   0        0        0     5148 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_tokenizer.py
--rw-r--r--   0        0        0     8161 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/markers.py
--rw-r--r--   0        0        0     3264 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/requirements.py
--rw-r--r--   0        0        0    39046 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/specifiers.py
--rw-r--r--   0        0        0    18065 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/tags.py
--rw-r--r--   0        0        0     4355 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/utils.py
--rw-r--r--   0        0        0    16295 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/version.py
--rw-r--r--   0        0        0      396 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/_types.py
--rw-r--r--   0        0        0      134 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/build_cmd/__init__.py
--rw-r--r--   0        0        0     1872 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/build_cmd/_build.py
--rw-r--r--   0        0        0      206 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/__init__.py
--rw-r--r--   0        0        0      181 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/_deps_command.py
--rw-r--r--   0        0        0     9067 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/deps_config.py
--rw-r--r--   0        0        0      618 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/__init__.py
--rw-r--r--   0        0        0      190 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/collector.py
--rw-r--r--   0        0        0     1653 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/metadata.py
--rw-r--r--   0        0        0      825 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/pep517.py
--rw-r--r--   0        0        0      679 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/pep518.py
--rw-r--r--   0        0        0     1062 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py
--rw-r--r--   0        0        0     2481 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/poetry.py
--rw-r--r--   0        0        0     2239 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/tox.py
--rw-r--r--   0        0        0       73 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/install_cmd/__init__.py
--rw-r--r--   0        0        0     6215 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/install_cmd/_install.py
--rw-r--r--   0        0        0      270 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/__init__.py
--rw-r--r--   0        0        0     9335 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/build_backend.py
--rw-r--r--   0        0        0      913 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/entry_points.py
--rw-r--r--   0        0        0      193 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/normalization.py
--rw-r--r--   0        0        0     1811 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/scripts.py
--rw-r--r--   0        0        0    10893 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/wheel.py
--rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/backend_helper/__init__.py
--rw-r--r--   0        0        0     5872 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/lib/backend_helper/backend_caller.py
--rw-r--r--   0        0        0       65 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/run_cmd/__init__.py
--rw-r--r--   0        0        0      430 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/run_cmd/_run_command.py
--rw-r--r--   0        0        0     7104 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/src/pyproject_installer/run_cmd/_run_env.py
--rw-r--r--   0        0        0      172 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/__init__.py
--rw-r--r--   0        0        0      367 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/common.py
--rw-r--r--   0        0        0     2092 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/config.py
--rw-r--r--   0        0        0     8581 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/metadata.py
--rw-r--r--   0        0        0     5559 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/sdist.py
--rw-r--r--   0        0        0     6922 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/wheel.py
--rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/_vendor/__init__.py
--rw-r--r--   0        0        0      396 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/_vendor/tomli/__init__.py
--rw-r--r--   0        0        0    22633 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/_vendor/tomli/_parser.py
--rw-r--r--   0        0        0     2943 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/_vendor/tomli/_re.py
--rw-r--r--   0        0        0      254 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/backend/_vendor/tomli/_types.py
--rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0     4612 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/integration/__init__.py
--rw-r--r--   0        0        0     5082 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/integration/conftest.py
--rw-r--r--   0        0        0     4144 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/integration/test_backends.py
--rw-r--r--   0        0        0     1719 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/integration/test_buildable.py
--rw-r--r--   0        0        0     2238 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/integration/test_config_settings.py
--rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/__init__.py
--rw-r--r--   0        0        0    31635 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_main.py
--rw-r--r--   0        0        0       92 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_version.py
--rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_build/__init__.py
--rw-r--r--   0        0        0      509 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_build/conftest.py
--rw-r--r--   0        0        0    15784 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_build/test_backend_caller.py
--rw-r--r--   0        0        0     8736 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_build/test_builder.py
--rw-r--r--   0        0        0     8179 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_build/test_pyproject_parser.py
--rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_deps/__init__.py
--rw-r--r--   0        0        0      495 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_deps/conftest.py
--rw-r--r--   0        0        0    22637 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_deps/test_collectors.py
--rw-r--r--   0        0        0    23966 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_deps/test_deps_config.py
--rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_install/__init__.py
--rw-r--r--   0        0        0    17931 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_install/test_installer.py
--rw-r--r--   0        0        0        0 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_run/__init__.py
--rw-r--r--   0        0        0    18875 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/tests/unit/test_run/test_env.py
--rw-r--r--   0        0        0    16949 2023-04-14 12:17:06.000000 pyproject_installer-0.5.0/PKG-INFO
--rw-r--r--   0        0        0     3464 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/pyproject.toml
--rw-r--r--   0        0        0    15997 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/README.md
--rw-r--r--   0        0        0     1024 2023-04-14 12:16:43.000000 pyproject_installer-0.5.0/LICENSE
+-rw-r--r--   0        0        0       78 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/__init__.py
+-rw-r--r--   0        0        0    16053 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/__main__.py
+-rw-r--r--   0        0        0      317 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/codes.py
+-rw-r--r--   0        0        0      391 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/errors.py
+-rw-r--r--   0        0        0       18 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/version.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/__init__.py
+-rw-r--r--   0        0        0      501 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/__init__.py
+-rw-r--r--   0        0        0     3266 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_elffile.py
+-rw-r--r--   0        0        0     8926 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_manylinux.py
+-rw-r--r--   0        0        0     2524 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_musllinux.py
+-rw-r--r--   0        0        0    10194 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_parser.py
+-rw-r--r--   0        0        0     1431 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_structures.py
+-rw-r--r--   0        0        0     5292 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_tokenizer.py
+-rw-r--r--   0        0        0     8208 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/markers.py
+-rw-r--r--   0        0        0    16397 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/metadata.py
+-rw-r--r--   0        0        0     3287 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/requirements.py
+-rw-r--r--   0        0        0    39206 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/specifiers.py
+-rw-r--r--   0        0        0    18106 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/tags.py
+-rw-r--r--   0        0        0     4355 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/utils.py
+-rw-r--r--   0        0        0    16326 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/version.py
+-rw-r--r--   0        0        0      396 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0      172 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/build_cmd/__init__.py
+-rw-r--r--   0        0        0     4477 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/build_cmd/_build.py
+-rw-r--r--   0        0        0      206 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/__init__.py
+-rw-r--r--   0        0        0      181 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/_deps_command.py
+-rw-r--r--   0        0        0     9067 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/deps_config.py
+-rw-r--r--   0        0        0      728 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/__init__.py
+-rw-r--r--   0        0        0      190 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/collector.py
+-rw-r--r--   0        0        0     2358 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/hatch.py
+-rw-r--r--   0        0        0     1306 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/metadata.py
+-rw-r--r--   0        0        0     1361 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pdm.py
+-rw-r--r--   0        0        0      825 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pep517.py
+-rw-r--r--   0        0        0      679 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pep518.py
+-rw-r--r--   0        0        0     1062 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py
+-rw-r--r--   0        0        0     2481 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/poetry.py
+-rw-r--r--   0        0        0     2239 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/tox.py
+-rw-r--r--   0        0        0       73 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/install_cmd/__init__.py
+-rw-r--r--   0        0        0     6215 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/install_cmd/_install.py
+-rw-r--r--   0        0        0      270 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/__init__.py
+-rw-r--r--   0        0        0     9335 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/build_backend.py
+-rw-r--r--   0        0        0      913 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/entry_points.py
+-rw-r--r--   0        0        0      193 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/normalization.py
+-rw-r--r--   0        0        0     1811 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/scripts.py
+-rw-r--r--   0        0        0    10893 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/wheel.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/backend_helper/__init__.py
+-rw-r--r--   0        0        0     5872 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/lib/backend_helper/backend_caller.py
+-rw-r--r--   0        0        0       65 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/run_cmd/__init__.py
+-rw-r--r--   0        0        0      430 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/run_cmd/_run_command.py
+-rw-r--r--   0        0        0     7104 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/src/pyproject_installer/run_cmd/_run_env.py
+-rw-r--r--   0        0        0      172 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/common.py
+-rw-r--r--   0        0        0     2092 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/config.py
+-rw-r--r--   0        0        0     8581 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/metadata.py
+-rw-r--r--   0        0        0     5559 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/sdist.py
+-rw-r--r--   0        0        0     6922 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/wheel.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/_vendor/__init__.py
+-rw-r--r--   0        0        0      396 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/_vendor/tomli/__init__.py
+-rw-r--r--   0        0        0    22633 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/_vendor/tomli/_parser.py
+-rw-r--r--   0        0        0     2943 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/_vendor/tomli/_re.py
+-rw-r--r--   0        0        0      254 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/backend/_vendor/tomli/_types.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     7856 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0     5082 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/integration/conftest.py
+-rw-r--r--   0        0        0     4144 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/integration/test_backends.py
+-rw-r--r--   0        0        0     1719 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/integration/test_buildable.py
+-rw-r--r--   0        0        0     2238 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/integration/test_config_settings.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0    31635 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_main.py
+-rw-r--r--   0        0        0       92 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_version.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_build/__init__.py
+-rw-r--r--   0        0        0      509 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_build/conftest.py
+-rw-r--r--   0        0        0    15784 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_build/test_backend_caller.py
+-rw-r--r--   0        0        0    12189 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_build/test_builder.py
+-rw-r--r--   0        0        0     8179 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_build/test_pyproject_parser.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_deps/__init__.py
+-rw-r--r--   0        0        0      495 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_deps/conftest.py
+-rw-r--r--   0        0        0    30305 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_deps/test_collectors.py
+-rw-r--r--   0        0        0    23966 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_deps/test_deps_config.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_install/__init__.py
+-rw-r--r--   0        0        0    17931 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_install/test_installer.py
+-rw-r--r--   0        0        0        0 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_run/__init__.py
+-rw-r--r--   0        0        0    18875 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/tests/unit/test_run/test_env.py
+-rw-r--r--   0        0        0    17234 2023-06-01 14:08:57.000000 pyproject_installer-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    16282 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/README.md
+-rw-r--r--   0        0        0     3464 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1024 2023-06-01 14:08:34.000000 pyproject_installer-0.5.1/LICENSE
```

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/__main__.py` & `pyproject_installer-0.5.1/src/pyproject_installer/__main__.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_elffile.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_manylinux.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_manylinux.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from ._elffile import EIClass, EIData, ELFFile, EMachine
 
 EF_ARM_ABIMASK = 0xFF000000
 EF_ARM_ABI_VER5 = 0x05000000
 EF_ARM_ABI_FLOAT_HARD = 0x00000400
 
 
+# `os.PathLike` not a generic type until Python 3.9, so sticking with `str`
+# as the type for `path` until then.
 @contextlib.contextmanager
 def _parse_elf(path: str) -> Generator[Optional[ELFFile], None, None]:
     try:
         with open(path, "rb") as f:
             yield ELFFile(f)
     except (OSError, TypeError, ValueError):
         yield None
```

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_musllinux.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_parser.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,15 +159,19 @@
 def _parse_extras(tokenizer: Tokenizer) -> List[str]:
     """
     extras = (LEFT_BRACKET wsp* extras_list? wsp* RIGHT_BRACKET)?
     """
     if not tokenizer.check("LEFT_BRACKET", peek=True):
         return []
 
-    with tokenizer.enclosing_tokens("LEFT_BRACKET", "RIGHT_BRACKET"):
+    with tokenizer.enclosing_tokens(
+        "LEFT_BRACKET",
+        "RIGHT_BRACKET",
+        around="extras",
+    ):
         tokenizer.consume("WS")
         extras = _parse_extras_list(tokenizer)
         tokenizer.consume("WS")
 
     return extras
 
 
@@ -199,29 +203,46 @@
 
 
 def _parse_specifier(tokenizer: Tokenizer) -> str:
     """
     specifier = LEFT_PARENTHESIS WS? version_many WS? RIGHT_PARENTHESIS
               | WS? version_many WS?
     """
-    with tokenizer.enclosing_tokens("LEFT_PARENTHESIS", "RIGHT_PARENTHESIS"):
+    with tokenizer.enclosing_tokens(
+        "LEFT_PARENTHESIS",
+        "RIGHT_PARENTHESIS",
+        around="version specifier",
+    ):
         tokenizer.consume("WS")
         parsed_specifiers = _parse_version_many(tokenizer)
         tokenizer.consume("WS")
 
     return parsed_specifiers
 
 
 def _parse_version_many(tokenizer: Tokenizer) -> str:
     """
     version_many = (SPECIFIER (WS? COMMA WS? SPECIFIER)*)?
     """
     parsed_specifiers = ""
     while tokenizer.check("SPECIFIER"):
+        span_start = tokenizer.position
         parsed_specifiers += tokenizer.read().text
+        if tokenizer.check("VERSION_PREFIX_TRAIL", peek=True):
+            tokenizer.raise_syntax_error(
+                ".* suffix can only be used with `==` or `!=` operators",
+                span_start=span_start,
+                span_end=tokenizer.position + 1,
+            )
+        if tokenizer.check("VERSION_LOCAL_LABEL_TRAIL", peek=True):
+            tokenizer.raise_syntax_error(
+                "Local version label can only be used with `==` or `!=` operators",
+                span_start=span_start,
+                span_end=tokenizer.position,
+            )
         tokenizer.consume("WS")
         if not tokenizer.check("COMMA"):
             break
         parsed_specifiers += tokenizer.read().text
         tokenizer.consume("WS")
 
     return parsed_specifiers
@@ -250,15 +271,19 @@
     """
     marker_atom = WS? LEFT_PARENTHESIS WS? marker WS? RIGHT_PARENTHESIS WS?
                 | WS? marker_item WS?
     """
 
     tokenizer.consume("WS")
     if tokenizer.check("LEFT_PARENTHESIS", peek=True):
-        with tokenizer.enclosing_tokens("LEFT_PARENTHESIS", "RIGHT_PARENTHESIS"):
+        with tokenizer.enclosing_tokens(
+            "LEFT_PARENTHESIS",
+            "RIGHT_PARENTHESIS",
+            around="marker expression",
+        ):
             tokenizer.consume("WS")
             marker: MarkerAtom = _parse_marker(tokenizer)
             tokenizer.consume("WS")
     else:
         marker = _parse_marker_item(tokenizer)
     tokenizer.consume("WS")
     return marker
```

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_structures.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/_tokenizer.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,16 @@
     "SPECIFIER": re.compile(
         Specifier._operator_regex_str + Specifier._version_regex_str,
         re.VERBOSE | re.IGNORECASE,
     ),
     "AT": r"\@",
     "URL": r"[^ \t]+",
     "IDENTIFIER": r"\b[a-zA-Z0-9][a-zA-Z0-9._-]*\b",
+    "VERSION_PREFIX_TRAIL": r"\.\*",
+    "VERSION_LOCAL_LABEL_TRAIL": r"\+[a-z0-9]+(?:[-_\.][a-z0-9]+)*",
     "WS": r"[ \t]+",
     "END": r"$",
 }
 
 
 class Tokenizer:
     """Context-sensitive token parsing.
@@ -163,26 +165,28 @@
         raise ParserSyntaxError(
             message,
             source=self.source,
             span=span,
         )
 
     @contextlib.contextmanager
-    def enclosing_tokens(self, open_token: str, close_token: str) -> Iterator[bool]:
+    def enclosing_tokens(
+        self, open_token: str, close_token: str, *, around: str
+    ) -> Iterator[None]:
         if self.check(open_token):
             open_position = self.position
             self.read()
         else:
             open_position = None
 
-        yield open_position is not None
+        yield
 
         if open_position is None:
             return
 
         if not self.check(close_token):
             self.raise_syntax_error(
-                f"Expected closing {close_token}",
+                f"Expected matching {close_token} for {open_token}, after {around}",
                 span_start=open_position,
             )
 
         self.read()
```

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/markers.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 
 import operator
 import os
 import platform
 import sys
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from ._parser import MarkerAtom, MarkerList, Op, Value, Variable, parse_marker
+from ._parser import (
+    MarkerAtom,
+    MarkerList,
+    Op,
+    Value,
+    Variable,
+    parse_marker as _parse_marker,
+)
 from ._tokenizer import ParserSyntaxError
 from .specifiers import InvalidSpecifier, Specifier
 from .utils import canonicalize_name
 
 __all__ = [
     "InvalidMarker",
     "UndefinedComparison",
@@ -185,15 +192,15 @@
 
 class Marker:
     def __init__(self, marker: str) -> None:
         # Note: We create a Marker object without calling this constructor in
         #       packaging.requirements.Requirement. If any additional logic is
         #       added here, make sure to mirror/adapt Requirement.
         try:
-            self._markers = _normalize_extra_values(parse_marker(marker))
+            self._markers = _normalize_extra_values(_parse_marker(marker))
             # The attribute `_markers` can be described in terms of a recursive type:
             # MarkerList = List[Union[Tuple[Node, ...], str, MarkerList]]
             #
             # For example, the following expression:
             # python_version > "3.6" or (python_version == "3.6" and os_name == "unix")
             #
             # is parsed into:
```

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/requirements.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/requirements.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 import urllib.parse
 from typing import Any, List, Optional, Set
 
-from ._parser import parse_requirement
+from ._parser import parse_requirement as _parse_requirement
 from ._tokenizer import ParserSyntaxError
 from .markers import Marker, _normalize_extra_values
 from .specifiers import SpecifierSet
 
 
 class InvalidRequirement(ValueError):
     """
@@ -28,15 +28,15 @@
     # TODO: Can we test whether something is contained within a requirement?
     #       If so how do we do that? Do we need to test against the _name_ of
     #       the thing as well as the version? What about the markers?
     # TODO: Can we normalize the name and extra name?
 
     def __init__(self, requirement_string: str) -> None:
         try:
-            parsed = parse_requirement(requirement_string)
+            parsed = _parse_requirement(requirement_string)
         except ParserSyntaxError as e:
             raise InvalidRequirement(str(e)) from e
 
         self.name: str = parsed.name
         if parsed.url:
             parsed_url = urllib.parse.urlparse(parsed.url)
             if parsed_url.scheme == "file":
```

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/specifiers.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/specifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,16 @@
             match.group("operator").strip(),
             match.group("version").strip(),
         )
 
         # Store whether or not this Specifier should accept prereleases
         self._prereleases = prereleases
 
-    @property
+    # https://github.com/python/mypy/pull/13475#pullrequestreview-1079784515
+    @property  # type: ignore[override]
     def prereleases(self) -> bool:
         # If there is an explicit prereleases set for this, then we'll just
         # blindly use that.
         if self._prereleases is not None:
             return self._prereleases
 
         # Look at all of our specifiers and determine if they are inclusive
@@ -394,15 +395,17 @@
         )
 
     def _compare_equal(self, prospective: Version, spec: str) -> bool:
 
         # We need special logic to handle prefix matching
         if spec.endswith(".*"):
             # In the case of prefix matching we want to ignore local segment.
-            normalized_prospective = canonicalize_version(prospective.public)
+            normalized_prospective = canonicalize_version(
+                prospective.public, strip_trailing_zero=False
+            )
             # Get the normalized version string ignoring the trailing .*
             normalized_spec = canonicalize_version(spec[:-2], strip_trailing_zero=False)
             # Split the spec out by dots, and pretend that there is an implicit
             # dot in between a release segment and a pre-release segment.
             split_spec = _version_split(normalized_spec)
 
             # Split the prospective version out by dots, and pretend that there
```

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/tags.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,24 +107,24 @@
         for abi in abis.split("."):
             for platform_ in platforms.split("."):
                 tags.add(Tag(interpreter, abi, platform_))
     return frozenset(tags)
 
 
 def _get_config_var(name: str, warn: bool = False) -> Union[int, str, None]:
-    value = sysconfig.get_config_var(name)
+    value: Union[int, str, None] = sysconfig.get_config_var(name)
     if value is None and warn:
         logger.debug(
             "Config variable '%s' is unset, Python ABI tag may be incorrect", name
         )
     return value
 
 
 def _normalize_string(string: str) -> str:
-    return string.replace(".", "_").replace("-", "_")
+    return string.replace(".", "_").replace("-", "_").replace(" ", "_")
 
 
 def _abi3_applies(python_version: PythonVersion) -> bool:
     """
     Determine if the Python version supports abi3.
 
     PEP 384 was first implemented in Python 3.2.
```

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/utils.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/packaging/version.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/packaging/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     from packaging.version import parse, Version
 """
 
 import collections
 import itertools
 import re
-from typing import Callable, Optional, SupportsInt, Tuple, Union
+from typing import Any, Callable, Optional, SupportsInt, Tuple, Union
 
 from ._structures import Infinity, InfinityType, NegativeInfinity, NegativeInfinityType
 
 __all__ = ["VERSION_PATTERN", "parse", "Version", "InvalidVersion"]
 
 InfiniteTypes = Union[InfinityType, NegativeInfinityType]
 PrePostDevType = Union[InfiniteTypes, Tuple[str, int]]
@@ -59,15 +59,15 @@
     Traceback (most recent call last):
         ...
     packaging.version.InvalidVersion: Invalid version: 'invalid'
     """
 
 
 class _BaseVersion:
-    _key: CmpKey
+    _key: Tuple[Any, ...]
 
     def __hash__(self) -> int:
         return hash(self._key)
 
     # Please keep the duplicated `isinstance` check
     # in the six comparisons hereunder
     # unless you find a way to avoid adding overhead function calls.
@@ -175,14 +175,15 @@
     >>> v1 >= v2
     False
     >>> v1 <= v2
     True
     """
 
     _regex = re.compile(r"^\s*" + VERSION_PATTERN + r"\s*$", re.VERBOSE | re.IGNORECASE)
+    _key: CmpKey
 
     def __init__(self, version: str) -> None:
         """Initialize a Version object.
 
         :param version:
             The string representation of a version which will be parsed and normalized
             before use.
```

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/_parser.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/_vendor/tomli/_re.py` & `pyproject_installer-0.5.1/src/pyproject_installer/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/deps_config.py` & `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/deps_config.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/__init__.py` & `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 from .pep517 import Pep517Collector
 from .pep518 import Pep518Collector
 from .pip_reqfile import PipReqFileCollector
 from .metadata import MetadataCollector
 from .poetry import PoetryCollector
 from .tox import ToxCollector
+from .hatch import HatchCollector
+from .pdm import PdmCollector
 
 
 __all__ = ["get_collector", "SUPPORTED_COLLECTORS"]
 
 SUPPORTED_COLLECTORS = {
     cls.name: cls
     for cls in [
         Pep517Collector,
         Pep518Collector,
         MetadataCollector,
         PipReqFileCollector,
         PoetryCollector,
         ToxCollector,
+        HatchCollector,
+        PdmCollector,
     ]
 }
 
 
 def get_collector(name):
     try:
         return SUPPORTED_COLLECTORS[name]
```

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/pep517.py` & `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pep517.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/pep518.py` & `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pep518.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py` & `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/pip_reqfile.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/poetry.py` & `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/poetry.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/deps_cmd/collectors/tox.py` & `pyproject_installer-0.5.1/src/pyproject_installer/deps_cmd/collectors/tox.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/install_cmd/_install.py` & `pyproject_installer-0.5.1/src/pyproject_installer/install_cmd/_install.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/lib/build_backend.py` & `pyproject_installer-0.5.1/src/pyproject_installer/lib/build_backend.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/lib/entry_points.py` & `pyproject_installer-0.5.1/src/pyproject_installer/lib/entry_points.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/lib/scripts.py` & `pyproject_installer-0.5.1/src/pyproject_installer/lib/scripts.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/lib/wheel.py` & `pyproject_installer-0.5.1/src/pyproject_installer/lib/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/lib/backend_helper/backend_caller.py` & `pyproject_installer-0.5.1/src/pyproject_installer/lib/backend_helper/backend_caller.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/src/pyproject_installer/run_cmd/_run_env.py` & `pyproject_installer-0.5.1/src/pyproject_installer/run_cmd/_run_env.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/backend/config.py` & `pyproject_installer-0.5.1/backend/config.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/backend/metadata.py` & `pyproject_installer-0.5.1/backend/metadata.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/backend/sdist.py` & `pyproject_installer-0.5.1/backend/sdist.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/backend/wheel.py` & `pyproject_installer-0.5.1/backend/wheel.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/backend/_vendor/tomli/_parser.py` & `pyproject_installer-0.5.1/backend/_vendor/tomli/_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/backend/_vendor/tomli/_re.py` & `pyproject_installer-0.5.1/backend/_vendor/tomli/_re.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/tests/integration/conftest.py` & `pyproject_installer-0.5.1/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/tests/integration/test_backends.py` & `pyproject_installer-0.5.1/tests/integration/test_backends.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/tests/integration/test_buildable.py` & `pyproject_installer-0.5.1/tests/integration/test_buildable.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/tests/integration/test_config_settings.py` & `pyproject_installer-0.5.1/tests/integration/test_config_settings.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/tests/unit/test_main.py` & `pyproject_installer-0.5.1/tests/unit/test_main.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/tests/unit/test_build/test_backend_caller.py` & `pyproject_installer-0.5.1/tests/unit/test_build/test_backend_caller.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/tests/unit/test_build/test_pyproject_parser.py` & `pyproject_installer-0.5.1/tests/unit/test_build/test_pyproject_parser.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/tests/unit/test_deps/test_collectors.py` & `pyproject_installer-0.5.1/tests/unit/test_deps/test_collectors.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,76 +27,14 @@
     assert isinstance(SUPPORTED_COLLECTORS, dict)
     for k, v in SUPPORTED_COLLECTORS.items():
         assert isinstance(k, str)
         assert issubclass(v, Collector)
 
 
 @pytest.fixture
-def pyproject_with_backend(pyproject, monkeypatch):
-    """Generates pyproject with self-hosted build backend"""
-
-    def _build_backend_src(be_content):
-        be_module = "be"
-        pyproject_toml_content = textwrap.dedent(
-            f"""\
-            [build-system]
-            requires=[]
-            build-backend="{be_module}"
-            backend-path=["."]
-            """
-        )
-        pyproject_path = pyproject(pyproject_toml_content)
-
-        backend_path = pyproject_path / be_module
-        backend_path.mkdir()
-        (backend_path / "__init__.py").write_text(be_content)
-
-        monkeypatch.chdir(pyproject_path)
-        return pyproject_path
-
-    return _build_backend_src
-
-
-@pytest.fixture
-def pyproject_metadata(pyproject_with_backend):
-    """Build backend with prepare_metadata_for_build_wheel"""
-
-    def _core_metadata(reqs):
-        content_fields = [
-            "Metadata-Version: 2.1",
-            "Name: foo",
-            "Version: 1.0",
-        ]
-        for req in reqs:
-            content_fields.append(f"Requires-Dist: {req}")
-
-        be_content = textwrap.dedent(
-            """\
-            def prepare_metadata_for_build_wheel(
-                metadata_directory, config_settings=None
-            ):
-                from pathlib import Path
-
-                distinfo = "foo-1.0.dist-info"
-                distinfo_path = Path(metadata_directory) / distinfo
-                distinfo_path.mkdir()
-                metadata_path = distinfo_path / "METADATA"
-                content = "{content}"
-
-                metadata_path.write_text(content, encoding="utf-8")
-
-                return distinfo
-            """
-        ).format(content="\\n".join(content_fields) + "\\n")
-        return pyproject_with_backend(be_content)
-
-    return _core_metadata
-
-
-@pytest.fixture
 def pyproject_pep517_wheel(pyproject_with_backend):
     """Build backend with get_requires_for_build_wheel"""
 
     def _pep517_wheel(reqs):
         be_content = textwrap.dedent(
             f"""\
             def get_requires_for_build_wheel(config_settings=None):
@@ -178,14 +116,59 @@
         config_path.write_text("\n".join(contents) + "\n", encoding="utf-8")
         monkeypatch.chdir(tmpdir)
         return config_path
 
     return _tox_deps
 
 
+@pytest.fixture
+def hatch_deps(tmpdir, monkeypatch):
+    """hatch's deps in specified config"""
+
+    def _hatch_deps(config, envname, deps, extra_deps=None):
+        if config == "pyproject.toml":
+            contents = [f"[tool.hatch.envs.{envname}]"]
+        else:
+            contents = [f"[envs.{envname}]"]
+        config_path = tmpdir / config
+        if deps is not None:
+            contents.append("dependencies = [")
+            contents.extend((f'"{x}",' for x in deps))
+            contents.append("]")
+        if extra_deps is not None:
+            contents.append("extra-dependencies = [")
+            contents.extend((f'"{x}",' for x in extra_deps))
+            contents.append("]")
+
+        config_path.write_text("\n".join(contents) + "\n", encoding="utf-8")
+        monkeypatch.chdir(tmpdir)
+        return config_path
+
+    return _hatch_deps
+
+
+@pytest.fixture
+def pdm_deps(tmpdir, monkeypatch):
+    """pdm deps"""
+
+    def _pdm_deps(group, deps):
+        contents = ["[tool.pdm.dev-dependencies]"]
+        if deps is not None:
+            contents.append(f"{group} = [")
+            contents.extend((f'"{x}",' for x in deps))
+            contents.append("]")
+
+        config_path = tmpdir / "pyproject.toml"
+        config_path.write_text("\n".join(contents) + "\n", encoding="utf-8")
+        monkeypatch.chdir(tmpdir)
+        return config_path
+
+    return _pdm_deps
+
+
 PEP508_DEPS_DATA = (
     ([], []),
     (["foo"], ["foo"]),
     (["foo == 1.0"], ["foo == 1.0"]),
     (
         ["foo @ https://example.com/foo.zip"],
         ["foo @ https://example.com/foo.zip"],
@@ -204,56 +187,59 @@
     (["_foo"], []),
     (["foo", "bar !> 1.0"], ["foo"]),
     (["foo", "bar > 1.0; invalid_marker == '1.0'"], ["foo"]),
 )
 
 
 @pytest.mark.parametrize("deps_data", PEP508_DEPS_DATA)
-def test_metadata_collector(deps_data, pyproject_metadata, depsconfig):
-    """Collection of core metadata"""
+def test_metadata_collector_metadata(deps_data, pyproject_metadata, depsconfig):
+    """Collection of core metadata via prepare_metadata_for_build_wheel"""
     # prepare source config
     srcname = "foo"
     collector = "metadata"
     input_conf = {"sources": {srcname: {"srctype": collector}}}
     depsconfig_path = depsconfig(json.dumps(input_conf))
 
     in_reqs, out_reqs = deps_data
 
     # configure pyproject with build backend
-    pyproject_metadata(in_reqs)
+    pyproject_metadata(reqs=in_reqs)
 
     deps_command("sync", depsconfig_path, srcnames=[])
 
     expected_conf = deepcopy(input_conf)
     if out_reqs:
         expected_conf["sources"][srcname]["deps"] = out_reqs
     actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
     assert actual_conf == expected_conf
 
 
-def test_metadata_collector_unsupported(pyproject_with_backend, depsconfig):
-    """Build backend doesn't support prepare_metadata_for_build_wheel"""
+@pytest.mark.parametrize("deps_data", PEP508_DEPS_DATA)
+def test_metadata_collector_wheel(
+    deps_data, pyproject_metadata_wheel, depsconfig
+):
+    """Collection of core metadata via build_wheel"""
     # prepare source config
     srcname = "foo"
     collector = "metadata"
     input_conf = {"sources": {srcname: {"srctype": collector}}}
     depsconfig_path = depsconfig(json.dumps(input_conf))
 
+    in_reqs, out_reqs = deps_data
+
     # configure pyproject with build backend
-    pyproject_with_backend("")
+    pyproject_metadata_wheel(reqs=in_reqs)
 
-    with pytest.raises(ValueError) as exc:
-        deps_command("sync", depsconfig_path, srcnames=[])
-    expected_err = (
-        "Backend doesn't support prepare_metadata_for_build_wheel hook"
-    )
-    assert expected_err in str(exc.value)
+    deps_command("sync", depsconfig_path, srcnames=[])
 
+    expected_conf = deepcopy(input_conf)
+    if out_reqs:
+        expected_conf["sources"][srcname]["deps"] = out_reqs
     actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
-    assert actual_conf == input_conf
+    assert actual_conf == expected_conf
 
 
 def test_pep518_collector_missing_pyproject_toml(
     tmpdir, depsconfig, monkeypatch
 ):
     """Collection of pep518 reqs with missing pyproject.toml"""
     # prepare source config
@@ -727,7 +713,268 @@
     expected_err = (
         f"Dependencies are not configured for {testenv}: missing {testenv}.deps"
     )
     assert expected_err in str(exc.value)
 
     actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
     assert actual_conf == input_conf
+
+
+@pytest.mark.parametrize("deps_data", PEP508_DEPS_DATA)
+@pytest.mark.parametrize("config", ("pyproject.toml", "hatch.toml"))
+def test_hatch_collector_deps(deps_data, config, hatch_deps, depsconfig):
+    """Collection of hatch dependencies"""
+    # prepare source config
+    srcname = "foo"
+    collector = "hatch"
+    envname = "test"
+
+    in_reqs, out_reqs = deps_data
+
+    hatch_config_path = hatch_deps(config, envname, in_reqs)
+    input_conf = {
+        "sources": {
+            srcname: {
+                "srctype": collector,
+                "srcargs": [str(hatch_config_path), envname],
+            },
+        }
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    deps_command("sync", depsconfig_path, srcnames=[])
+
+    expected_conf = deepcopy(input_conf)
+    if out_reqs:
+        expected_conf["sources"][srcname]["deps"] = out_reqs
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == expected_conf
+
+
+@pytest.mark.parametrize("deps_data", PEP508_DEPS_DATA)
+@pytest.mark.parametrize("config", ("pyproject.toml", "hatch.toml"))
+def test_hatch_collector_extra_deps(deps_data, config, hatch_deps, depsconfig):
+    """Collection of hatch extra-dependencies"""
+    # prepare source config
+    srcname = "foo"
+    collector = "hatch"
+    envname = "test"
+
+    in_reqs, out_reqs = deps_data
+
+    hatch_config_path = hatch_deps(
+        config, envname, deps=None, extra_deps=in_reqs
+    )
+    input_conf = {
+        "sources": {
+            srcname: {
+                "srctype": collector,
+                "srcargs": [str(hatch_config_path), envname],
+            },
+        }
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    deps_command("sync", depsconfig_path, srcnames=[])
+
+    expected_conf = deepcopy(input_conf)
+    if out_reqs:
+        expected_conf["sources"][srcname]["deps"] = out_reqs
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == expected_conf
+
+
+@pytest.mark.parametrize(
+    "hatch_config",
+    ("", "[tool]", "[tool.hatch]", "[tool.hatch.envs]", "[tool.hatch.envs.a]"),
+)
+def test_hatch_collector_missing_configuration_pyproject(
+    hatch_config, tmpdir, depsconfig, monkeypatch
+):
+    """Collection of hatch(pyproject.toml) with missing configuration"""
+    # prepare source config
+    srcname = "foo"
+    collector = "hatch"
+    hatchenv = "test"
+
+    hatch_config_path = tmpdir / "pyproject.toml"
+    hatch_config_path.write_text(hatch_config + "\n", encoding="utf-8")
+    input_conf = {
+        "sources": {
+            srcname: {
+                "srctype": collector,
+                "srcargs": [str(hatch_config_path), hatchenv],
+            },
+        }
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    monkeypatch.chdir(tmpdir)
+    with pytest.raises(ValueError) as exc:
+        deps_command("sync", depsconfig_path, srcnames=[])
+    expected_err = (
+        f"Hatch: missing tool.hatch.envs.{hatchenv} table in "
+        f"{hatch_config_path.name}"
+    )
+    assert str(exc.value) == expected_err
+
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == input_conf
+
+
+@pytest.mark.parametrize("hatch_config", ("", "[envs]", "[envs.a]"))
+def test_hatch_collector_missing_configuration_hatch(
+    hatch_config, tmpdir, depsconfig, monkeypatch
+):
+    """Collection of hatch(hatch.toml) with missing configuration"""
+    # prepare source config
+    srcname = "foo"
+    collector = "hatch"
+    hatchenv = "test"
+
+    hatch_config_path = tmpdir / "hatch.toml"
+    hatch_config_path.write_text(hatch_config + "\n", encoding="utf-8")
+    input_conf = {
+        "sources": {
+            srcname: {
+                "srctype": collector,
+                "srcargs": [str(hatch_config_path), hatchenv],
+            },
+        }
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    monkeypatch.chdir(tmpdir)
+    with pytest.raises(ValueError) as exc:
+        deps_command("sync", depsconfig_path, srcnames=[])
+    expected_err = (
+        f"Hatch: missing envs.{hatchenv} table in {hatch_config_path.name}"
+    )
+    assert str(exc.value) == expected_err
+
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == input_conf
+
+
+@pytest.mark.parametrize("config", ("pyproject.toml", "hatch.toml"))
+def test_hatch_collector_missing_deps(config, hatch_deps, depsconfig):
+    """Collection of missing hatch deps"""
+    # prepare source config
+    srcname = "foo"
+    collector = "hatch"
+    hatchenv = "test"
+
+    hatch_config_path = hatch_deps(config, hatchenv, deps=None, extra_deps=None)
+
+    input_conf = {
+        "sources": {
+            srcname: {
+                "srctype": collector,
+                "srcargs": [str(hatch_config_path), hatchenv],
+            },
+        }
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    with pytest.raises(ValueError) as exc:
+        deps_command("sync", depsconfig_path, srcnames=[])
+    expected_err = (
+        f"Hatch dependencies are not configured for {hatchenv}: "
+        f"missing {hatchenv}.dependencies and {hatchenv}.extra-dependencies"
+    )
+    assert str(exc.value) == expected_err
+
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == input_conf
+
+
+@pytest.mark.parametrize("deps_data", PEP508_DEPS_DATA)
+def test_pdm_collector_deps(deps_data, pdm_deps, depsconfig):
+    """Collection of pdm dependencies"""
+    # prepare source config
+    srcname = "foo"
+    collector = "pdm"
+    group = "test"
+
+    in_reqs, out_reqs = deps_data
+
+    pdm_deps(group, in_reqs)
+    input_conf = {
+        "sources": {
+            srcname: {
+                "srctype": collector,
+                "srcargs": [group],
+            },
+        }
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    deps_command("sync", depsconfig_path, srcnames=[])
+
+    expected_conf = deepcopy(input_conf)
+    if out_reqs:
+        expected_conf["sources"][srcname]["deps"] = out_reqs
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == expected_conf
+
+
+@pytest.mark.parametrize("pdm_config", ("", "[tool]", "[tool.pdm]"))
+def test_pdm_collector_missing_configuration(
+    pdm_config, tmpdir, depsconfig, monkeypatch
+):
+    """Collection of pdm with missing configuration"""
+    # prepare source config
+    srcname = "foo"
+    collector = "pdm"
+    group = "test"
+
+    pdm_config_path = tmpdir / "pyproject.toml"
+    pdm_config_path.write_text(pdm_config + "\n", encoding="utf-8")
+    input_conf = {
+        "sources": {
+            srcname: {
+                "srctype": collector,
+                "srcargs": [group],
+            },
+        }
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    monkeypatch.chdir(tmpdir)
+    with pytest.raises(ValueError) as exc:
+        deps_command("sync", depsconfig_path, srcnames=[])
+    expected_err = (
+        "Pdm: missing tool.pdm.dev-dependencies table in "
+        f"{pdm_config_path.name}"
+    )
+    assert str(exc.value) == expected_err
+
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == input_conf
+
+
+def test_pdm_collector_missing_deps(pdm_deps, depsconfig):
+    """Collection of missing pdm deps"""
+    # prepare source config
+    srcname = "foo"
+    collector = "pdm"
+    group = "test"
+
+    pdm_deps(group, deps=None)
+
+    input_conf = {
+        "sources": {
+            srcname: {
+                "srctype": collector,
+                "srcargs": [group],
+            },
+        }
+    }
+    depsconfig_path = depsconfig(json.dumps(input_conf))
+
+    with pytest.raises(ValueError) as exc:
+        deps_command("sync", depsconfig_path, srcnames=[])
+    expected_err = f"Pdm dependencies are not configured for group: {group}"
+    assert str(exc.value) == expected_err
+
+    actual_conf = json.loads(depsconfig_path.read_text(encoding="utf-8"))
+    assert actual_conf == input_conf
```

### Comparing `pyproject_installer-0.5.0/tests/unit/test_deps/test_deps_config.py` & `pyproject_installer-0.5.1/tests/unit/test_deps/test_deps_config.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/tests/unit/test_install/test_installer.py` & `pyproject_installer-0.5.1/tests/unit/test_install/test_installer.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/tests/unit/test_run/test_env.py` & `pyproject_installer-0.5.1/tests/unit/test_run/test_env.py`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/PKG-INFO` & `pyproject_installer-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-installer
-Version: 0.5.0
+Version: 0.5.1
 Summary: Pyproject installer
 Author-email: Stanislav Levin <slev@altlinux.org>
 License: MIT
 Project-URL: source,https://github.com/stanislavlevin/pyproject_installer
 Project-URL: tracker,https://github.com/stanislavlevin/pyproject_installer/issues
 Keywords: packaging,PEP517,build,install
 Classifier: Development Status :: 4 - Beta
@@ -62,18 +62,17 @@
   any Python project.<br>
   Current vendored packages:
   - `tomli` (used for parsing `pyproject.toml` configuration file).
      Note: `tomli` is the part of stdlib since Python 3.11.
   - `packaging` (used for parsing PEP508 dependencies)
 
 - Installation of build dependencies is up to the caller.<br>
-  Moreover, parsing of build requirements requires two additional external
-  packages: `packaging` and its dependency `pyparsing`. But since the validation
-  of build dependencies is optional (disabled by default) there is no point to
-  vendor them.
+  These dependencies of Python projects are managed externally with system
+  package managers like `apt` or `dnf`. [External source](#management-of-dependencies-sources) of upstream's
+  dependencies may be used for provision of formatted list of dependencies to external tools.
 
 - There is no post-installation bytecompilation.<br>
   PEP427 says that wheel installers should compile any installed .py to .pyc.
   External tools like RPM already provide Python bytecompilation means, which
   compile for multiple optimization levels at a time. No point to compile
   modules twice.
 
@@ -223,15 +222,15 @@
 {cwd}/dist/.wheeltracker
 <em><strong>example</strong></em>: python -m pyproject_installer run --wheel wheel.whl pytest
 </pre>
 
 Note: venv's directory name is `.run_venv`.
 
 
-### Management of dependencies' sources
+### Management of dependencies sources
 
 Collect PEP508 requirements from different sources, store and evaluate
 them in Python environment.
 
 ```
 python -m pyproject_installer deps --help
 ```
@@ -259,26 +258,26 @@
 <em><strong>example</strong></em>: python -m pyproject_installer deps show build
 </pre>
 
 ---
 
 <pre>
 <em><strong>name</strong></em>: add
-<em><strong>description</strong></em>: configure source of Python dependencies. Supported sources: standardized formats like PEP517, PEP518 or core metadata are fully supported, while tool-specific formats like pip, tox or poetry have limited support.
+<em><strong>description</strong></em>: configure source of Python dependencies. Supported sources: standardized formats like PEP517, PEP518 or core metadata are fully supported, while tool-specific formats like pip, tox, poetry, hatch or pdm have limited support.
 <em><strong>example</strong></em>: python -m pyproject_installer deps add --help
 </pre>
 
 Positional arguments:
 <pre>
 <em><strong>description</strong></em>: source name
 </pre>
 
 <pre>
 <em><strong>description</strong></em>: source type
-<em><strong>choice</strong></em>: pep517, pep518, metadata, pip_reqfile, poetry, tox
+<em><strong>choice</strong></em>: pep517, pep518, metadata, pip_reqfile, poetry, tox, hatch, pdm
 </pre>
 
 <pre>
 <em><strong>description</strong></em>: specific configuration options for source
 <em><strong>default</strong></em>: []
 </pre>
 
@@ -297,14 +296,20 @@
 python -m pyproject_installer deps add check pip_reqfile requirements.txt
 
 Configuration of source of <strong>tox</strong> requirements:
 python -m pyproject_installer deps add check tox tox.ini testenv
 
 Configuration of source of <strong>poetry</strong> requirements:
 python -m pyproject_installer deps add check poetry dev
+
+Configuration of source of <strong>hatch</strong> requirements:
+python -m pyproject_installer deps add check hatch hatch.toml test
+
+Configuration of source of <strong>pdm</strong> requirements:
+python -m pyproject_installer deps add check pdm test
 </pre>
 
 ---
 
 <pre>
 <em><strong>name</strong></em>: sync
 <em><strong>description</strong></em>: sync stored requirements to configured sources
@@ -392,16 +397,16 @@
 
 ### builder
 
 Functionally, today's builder is similar to [build](https://pypi.org/project/build).<br>
 The key differences are:
 - highly specialized defaults (see [description](#Description))
 - highly specialized features to drop extra runtime dependencies like
-  `pep517` or `packaging`. No point to vendor `pep517` to call only
-  `build_wheel` backend hook in subprocess.
+  `pep517`. No point to vendor `pep517` to call only `build_wheel` backend hook
+  in subprocess.
 
 ### installer
 
 Functionally, today's installer is similar to [installer](https://pypi.org/project/installer).<br>
 The key differences are:
 - highly specialized defaults and features (see [description](#Description))
```

### Comparing `pyproject_installer-0.5.0/pyproject.toml` & `pyproject_installer-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyproject_installer-0.5.0/README.md` & `pyproject_installer-0.5.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -39,18 +39,17 @@
   any Python project.<br>
   Current vendored packages:
   - `tomli` (used for parsing `pyproject.toml` configuration file).
      Note: `tomli` is the part of stdlib since Python 3.11.
   - `packaging` (used for parsing PEP508 dependencies)
 
 - Installation of build dependencies is up to the caller.<br>
-  Moreover, parsing of build requirements requires two additional external
-  packages: `packaging` and its dependency `pyparsing`. But since the validation
-  of build dependencies is optional (disabled by default) there is no point to
-  vendor them.
+  These dependencies of Python projects are managed externally with system
+  package managers like `apt` or `dnf`. [External source](#management-of-dependencies-sources) of upstream's
+  dependencies may be used for provision of formatted list of dependencies to external tools.
 
 - There is no post-installation bytecompilation.<br>
   PEP427 says that wheel installers should compile any installed .py to .pyc.
   External tools like RPM already provide Python bytecompilation means, which
   compile for multiple optimization levels at a time. No point to compile
   modules twice.
 
@@ -200,15 +199,15 @@
 {cwd}/dist/.wheeltracker
 <em><strong>example</strong></em>: python -m pyproject_installer run --wheel wheel.whl pytest
 </pre>
 
 Note: venv's directory name is `.run_venv`.
 
 
-### Management of dependencies' sources
+### Management of dependencies sources
 
 Collect PEP508 requirements from different sources, store and evaluate
 them in Python environment.
 
 ```
 python -m pyproject_installer deps --help
 ```
@@ -236,26 +235,26 @@
 <em><strong>example</strong></em>: python -m pyproject_installer deps show build
 </pre>
 
 ---
 
 <pre>
 <em><strong>name</strong></em>: add
-<em><strong>description</strong></em>: configure source of Python dependencies. Supported sources: standardized formats like PEP517, PEP518 or core metadata are fully supported, while tool-specific formats like pip, tox or poetry have limited support.
+<em><strong>description</strong></em>: configure source of Python dependencies. Supported sources: standardized formats like PEP517, PEP518 or core metadata are fully supported, while tool-specific formats like pip, tox, poetry, hatch or pdm have limited support.
 <em><strong>example</strong></em>: python -m pyproject_installer deps add --help
 </pre>
 
 Positional arguments:
 <pre>
 <em><strong>description</strong></em>: source name
 </pre>
 
 <pre>
 <em><strong>description</strong></em>: source type
-<em><strong>choice</strong></em>: pep517, pep518, metadata, pip_reqfile, poetry, tox
+<em><strong>choice</strong></em>: pep517, pep518, metadata, pip_reqfile, poetry, tox, hatch, pdm
 </pre>
 
 <pre>
 <em><strong>description</strong></em>: specific configuration options for source
 <em><strong>default</strong></em>: []
 </pre>
 
@@ -274,14 +273,20 @@
 python -m pyproject_installer deps add check pip_reqfile requirements.txt
 
 Configuration of source of <strong>tox</strong> requirements:
 python -m pyproject_installer deps add check tox tox.ini testenv
 
 Configuration of source of <strong>poetry</strong> requirements:
 python -m pyproject_installer deps add check poetry dev
+
+Configuration of source of <strong>hatch</strong> requirements:
+python -m pyproject_installer deps add check hatch hatch.toml test
+
+Configuration of source of <strong>pdm</strong> requirements:
+python -m pyproject_installer deps add check pdm test
 </pre>
 
 ---
 
 <pre>
 <em><strong>name</strong></em>: sync
 <em><strong>description</strong></em>: sync stored requirements to configured sources
@@ -369,16 +374,16 @@
 
 ### builder
 
 Functionally, today's builder is similar to [build](https://pypi.org/project/build).<br>
 The key differences are:
 - highly specialized defaults (see [description](#Description))
 - highly specialized features to drop extra runtime dependencies like
-  `pep517` or `packaging`. No point to vendor `pep517` to call only
-  `build_wheel` backend hook in subprocess.
+  `pep517`. No point to vendor `pep517` to call only `build_wheel` backend hook
+  in subprocess.
 
 ### installer
 
 Functionally, today's installer is similar to [installer](https://pypi.org/project/installer).<br>
 The key differences are:
 - highly specialized defaults and features (see [description](#Description))
```

### Comparing `pyproject_installer-0.5.0/LICENSE` & `pyproject_installer-0.5.1/LICENSE`

 * *Files identical despite different names*

