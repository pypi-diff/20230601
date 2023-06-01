# Comparing `tmp/gmxapi-0.4.1.tar.gz` & `tmp/gmxapi-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/eric/develop/CLionProjects/gromacs2023/python_packaging/gmxapi/dist/.tmp-qsfur0sc/gmxapi-0.4.1.tar", last modified: Mon May 22 16:55:00 2023, max compression
+gzip compressed data, was "/Users/eric/develop/CLionProjects/gromacs2023/python_packaging/gmxapi/dist/.tmp-alqibrhq/gmxapi-0.4.2.tar", last modified: Thu Jun  1 17:44:02 2023, max compression
```

## Comparing `gmxapi-0.4.1.tar` & `gmxapi-0.4.2.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/
--rw-r--r--   0 eric       (501) staff       (20)    18861 2023-05-22 16:45:32.000000 gmxapi-0.4.1/CMakeLists.txt
--rw-r--r--   0 eric       (501) staff       (20)    24479 2023-05-15 03:20:39.000000 gmxapi-0.4.1/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      188 2023-05-22 16:45:32.000000 gmxapi-0.4.1/MANIFEST.in
--rw-r--r--   0 eric       (501) staff       (20)      742 2023-05-22 16:55:00.000000 gmxapi-0.4.1/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      498 2023-05-15 03:20:39.000000 gmxapi-0.4.1/README.rst
--rw-r--r--   0 eric       (501) staff       (20)      138 2023-05-22 16:45:32.000000 gmxapi-0.4.1/pyproject.toml
--rw-r--r--   0 eric       (501) staff       (20)      536 2023-05-22 16:55:00.000000 gmxapi-0.4.1/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)    17937 2023-05-22 16:45:32.000000 gmxapi-0.4.1/setup.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/cpp/
--rw-r--r--   0 eric       (501) staff       (20)    10101 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/cpp/export_context.cpp
--rw-r--r--   0 eric       (501) staff       (20)     3686 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/export_system.cpp
--rw-r--r--   0 eric       (501) staff       (20)     7541 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/export_tprfile.cpp
--rw-r--r--   0 eric       (501) staff       (20)     6083 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/gmxpy_exceptions.cpp
--rw-r--r--   0 eric       (501) staff       (20)     4745 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/gmxpy_exceptions.h
--rw-r--r--   0 eric       (501) staff       (20)     2066 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/launch_0_2_1.cpp
--rw-r--r--   0 eric       (501) staff       (20)     4744 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/module.cpp
--rw-r--r--   0 eric       (501) staff       (20)     4070 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/module.h
--rw-r--r--   0 eric       (501) staff       (20)     3040 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/mpi_bindings.cpp
--rw-r--r--   0 eric       (501) staff       (20)     3243 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/mpi_bindings.h
--rw-r--r--   0 eric       (501) staff       (20)     2097 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/mpi_gromacs_support.cpp
--rw-r--r--   0 eric       (501) staff       (20)     2827 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/mpi_no_gromacs_support.cpp
--rw-r--r--   0 eric       (501) staff       (20)     5054 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pycontext.cpp
--rw-r--r--   0 eric       (501) staff       (20)     3446 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pycontext.h
--rw-r--r--   0 eric       (501) staff       (20)     3048 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pycontext_create.cpp
--rw-r--r--   0 eric       (501) staff       (20)     2999 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pycontext_create_no_mpi.cpp
--rw-r--r--   0 eric       (501) staff       (20)     2034 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pysystem.cpp
--rw-r--r--   0 eric       (501) staff       (20)     2151 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/pysystem.h
--rw-r--r--   0 eric       (501) staff       (20)     3465 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/wrapped_exceptions.h
--rw-r--r--   0 eric       (501) staff       (20)     3529 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/wrapped_exceptions_0_1_0.cpp
--rw-r--r--   0 eric       (501) staff       (20)     4065 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/cpp/wrapped_exceptions_0_3_1.cpp
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi/
--rw-r--r--   0 eric       (501) staff       (20)     2814 2023-05-15 03:21:49.000000 gmxapi-0.4.1/src/gmxapi/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     3532 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/_logging.py
--rw-r--r--   0 eric       (501) staff       (20)     2300 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/_transform.py
--rw-r--r--   0 eric       (501) staff       (20)    31056 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/abc.py
--rw-r--r--   0 eric       (501) staff       (20)    22158 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/commandline.py
--rw-r--r--   0 eric       (501) staff       (20)     5362 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/datamodel.py
--rw-r--r--   0 eric       (501) staff       (20)     4315 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/exceptions.py
--rw-r--r--   0 eric       (501) staff       (20)      367 2023-05-22 16:45:32.000000 gmxapi-0.4.1/src/gmxapi/gmxconfig.json.in
--rw-r--r--   0 eric       (501) staff       (20)   244525 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/operation.py
--rw-r--r--   0 eric       (501) staff       (20)    31523 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/runtime.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi/simulation/
--rw-r--r--   0 eric       (501) staff       (20)     2787 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/__init__.py
--rw-r--r--   0 eric       (501) staff       (20)     2316 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/abc.py
--rw-r--r--   0 eric       (501) staff       (20)    57397 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/context.py
--rw-r--r--   0 eric       (501) staff       (20)     9778 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/fileio.py
--rw-r--r--   0 eric       (501) staff       (20)    50717 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/mdrun.py
--rw-r--r--   0 eric       (501) staff       (20)    18838 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/modify_input.py
--rw-r--r--   0 eric       (501) staff       (20)    19300 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/read_tpr.py
--rw-r--r--   0 eric       (501) staff       (20)    36791 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/simulation/workflow.py
--rw-r--r--   0 eric       (501) staff       (20)     7932 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/testsupport.py
--rw-r--r--   0 eric       (501) staff       (20)     6753 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/typing.py
--rw-r--r--   0 eric       (501) staff       (20)     2808 2023-05-15 03:20:39.000000 gmxapi-0.4.1/src/gmxapi/utility.py
--rw-r--r--   0 eric       (501) staff       (20)     8612 2023-05-22 16:38:39.000000 gmxapi-0.4.1/src/gmxapi/version.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      742 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)     1721 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-22 16:54:59.000000 gmxapi-0.4.1/src/gmxapi.egg-info/not-zip-safe
--rw-r--r--   0 eric       (501) staff       (20)       50 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)        7 2023-05-22 16:55:00.000000 gmxapi-0.4.1/src/gmxapi.egg-info/top_level.txt
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-05-22 16:55:00.000000 gmxapi-0.4.1/test/
--rw-r--r--   0 eric       (501) staff       (20)     5358 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/CMakeLists.txt
--rw-r--r--   0 eric       (501) staff       (20)     7010 2023-05-22 16:45:32.000000 gmxapi-0.4.1/test/conftest.py
--rw-r--r--   0 eric       (501) staff       (20)      113 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/pytest.ini
--rw-r--r--   0 eric       (501) staff       (20)    13256 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_commandline.py
--rw-r--r--   0 eric       (501) staff       (20)     2317 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_exceptions.py
--rw-r--r--   0 eric       (501) staff       (20)     5296 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_feature_check.py
--rw-r--r--   0 eric       (501) staff       (20)     4009 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_fileio.py
--rw-r--r--   0 eric       (501) staff       (20)     4689 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_fileio_low_level.py
--rw-r--r--   0 eric       (501) staff       (20)    12615 2023-05-22 16:38:39.000000 gmxapi-0.4.1/test/test_mdrun.py
--rw-r--r--   0 eric       (501) staff       (20)     6540 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_operation.py
--rw-r--r--   0 eric       (501) staff       (20)     8151 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_runtime.py
--rw-r--r--   0 eric       (501) staff       (20)     5584 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/test_subgraph.py
--rw-r--r--   0 eric       (501) staff       (20)    49825 2023-05-15 03:20:39.000000 gmxapi-0.4.1/test/testdata.json
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-06-01 17:44:02.000000 gmxapi-0.4.2/
+-rw-r--r--   0 eric       (501) staff       (20)    18861 2023-06-01 17:43:10.000000 gmxapi-0.4.2/CMakeLists.txt
+-rw-r--r--   0 eric       (501) staff       (20)    24479 2023-05-15 03:20:39.000000 gmxapi-0.4.2/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      188 2023-06-01 17:43:10.000000 gmxapi-0.4.2/MANIFEST.in
+-rw-r--r--   0 eric       (501) staff       (20)      742 2023-06-01 17:44:02.000000 gmxapi-0.4.2/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      498 2023-05-15 03:20:39.000000 gmxapi-0.4.2/README.rst
+-rw-r--r--   0 eric       (501) staff       (20)      138 2023-06-01 17:43:10.000000 gmxapi-0.4.2/pyproject.toml
+-rw-r--r--   0 eric       (501) staff       (20)      536 2023-06-01 17:44:02.000000 gmxapi-0.4.2/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)    17937 2023-06-01 17:43:10.000000 gmxapi-0.4.2/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-06-01 17:44:02.000000 gmxapi-0.4.2/src/
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-06-01 17:44:02.000000 gmxapi-0.4.2/src/cpp/
+-rw-r--r--   0 eric       (501) staff       (20)    10101 2023-05-22 16:38:39.000000 gmxapi-0.4.2/src/cpp/export_context.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     3686 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/export_system.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     7541 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/export_tprfile.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     6083 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/gmxpy_exceptions.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     4745 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/gmxpy_exceptions.h
+-rw-r--r--   0 eric       (501) staff       (20)     2066 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/launch_0_2_1.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     4744 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/module.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     4070 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/module.h
+-rw-r--r--   0 eric       (501) staff       (20)     3040 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/mpi_bindings.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     3243 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/mpi_bindings.h
+-rw-r--r--   0 eric       (501) staff       (20)     2097 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/mpi_gromacs_support.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     2827 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/mpi_no_gromacs_support.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     5054 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/pycontext.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     3446 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/pycontext.h
+-rw-r--r--   0 eric       (501) staff       (20)     3048 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/pycontext_create.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     2999 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/pycontext_create_no_mpi.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     2034 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/pysystem.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     2151 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/pysystem.h
+-rw-r--r--   0 eric       (501) staff       (20)     3465 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/wrapped_exceptions.h
+-rw-r--r--   0 eric       (501) staff       (20)     3529 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/wrapped_exceptions_0_1_0.cpp
+-rw-r--r--   0 eric       (501) staff       (20)     4065 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/cpp/wrapped_exceptions_0_3_1.cpp
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-06-01 17:44:02.000000 gmxapi-0.4.2/src/gmxapi/
+-rw-r--r--   0 eric       (501) staff       (20)     2814 2023-05-15 03:21:49.000000 gmxapi-0.4.2/src/gmxapi/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     3532 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/_logging.py
+-rw-r--r--   0 eric       (501) staff       (20)     2300 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/_transform.py
+-rw-r--r--   0 eric       (501) staff       (20)    31056 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/abc.py
+-rw-r--r--   0 eric       (501) staff       (20)    22158 2023-05-22 16:38:39.000000 gmxapi-0.4.2/src/gmxapi/commandline.py
+-rw-r--r--   0 eric       (501) staff       (20)     5362 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/datamodel.py
+-rw-r--r--   0 eric       (501) staff       (20)     4315 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/exceptions.py
+-rw-r--r--   0 eric       (501) staff       (20)      367 2023-06-01 17:43:10.000000 gmxapi-0.4.2/src/gmxapi/gmxconfig.json.in
+-rw-r--r--   0 eric       (501) staff       (20)   244525 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/operation.py
+-rw-r--r--   0 eric       (501) staff       (20)    31523 2023-05-22 16:38:39.000000 gmxapi-0.4.2/src/gmxapi/runtime.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-06-01 17:44:02.000000 gmxapi-0.4.2/src/gmxapi/simulation/
+-rw-r--r--   0 eric       (501) staff       (20)     2787 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/simulation/__init__.py
+-rw-r--r--   0 eric       (501) staff       (20)     2316 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/simulation/abc.py
+-rw-r--r--   0 eric       (501) staff       (20)    57397 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/simulation/context.py
+-rw-r--r--   0 eric       (501) staff       (20)     9778 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/simulation/fileio.py
+-rw-r--r--   0 eric       (501) staff       (20)    51117 2023-06-01 17:43:10.000000 gmxapi-0.4.2/src/gmxapi/simulation/mdrun.py
+-rw-r--r--   0 eric       (501) staff       (20)    18838 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/simulation/modify_input.py
+-rw-r--r--   0 eric       (501) staff       (20)    19300 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/simulation/read_tpr.py
+-rw-r--r--   0 eric       (501) staff       (20)    36791 2023-05-22 16:38:39.000000 gmxapi-0.4.2/src/gmxapi/simulation/workflow.py
+-rw-r--r--   0 eric       (501) staff       (20)     7932 2023-05-22 16:38:39.000000 gmxapi-0.4.2/src/gmxapi/testsupport.py
+-rw-r--r--   0 eric       (501) staff       (20)     6753 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/typing.py
+-rw-r--r--   0 eric       (501) staff       (20)     2808 2023-05-15 03:20:39.000000 gmxapi-0.4.2/src/gmxapi/utility.py
+-rw-r--r--   0 eric       (501) staff       (20)     8612 2023-06-01 17:43:10.000000 gmxapi-0.4.2/src/gmxapi/version.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-06-01 17:44:02.000000 gmxapi-0.4.2/src/gmxapi.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      742 2023-06-01 17:44:02.000000 gmxapi-0.4.2/src/gmxapi.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)     1721 2023-06-01 17:44:02.000000 gmxapi-0.4.2/src/gmxapi.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-06-01 17:44:02.000000 gmxapi-0.4.2/src/gmxapi.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2023-05-22 16:54:59.000000 gmxapi-0.4.2/src/gmxapi.egg-info/not-zip-safe
+-rw-r--r--   0 eric       (501) staff       (20)       50 2023-06-01 17:44:02.000000 gmxapi-0.4.2/src/gmxapi.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)        7 2023-06-01 17:44:02.000000 gmxapi-0.4.2/src/gmxapi.egg-info/top_level.txt
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2023-06-01 17:44:02.000000 gmxapi-0.4.2/test/
+-rw-r--r--   0 eric       (501) staff       (20)     5358 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/CMakeLists.txt
+-rw-r--r--   0 eric       (501) staff       (20)     7010 2023-06-01 17:43:10.000000 gmxapi-0.4.2/test/conftest.py
+-rw-r--r--   0 eric       (501) staff       (20)      113 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/pytest.ini
+-rw-r--r--   0 eric       (501) staff       (20)    13256 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/test_commandline.py
+-rw-r--r--   0 eric       (501) staff       (20)     2317 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/test_exceptions.py
+-rw-r--r--   0 eric       (501) staff       (20)     5296 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/test_feature_check.py
+-rw-r--r--   0 eric       (501) staff       (20)     4009 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/test_fileio.py
+-rw-r--r--   0 eric       (501) staff       (20)     4689 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/test_fileio_low_level.py
+-rw-r--r--   0 eric       (501) staff       (20)    12966 2023-06-01 17:43:10.000000 gmxapi-0.4.2/test/test_mdrun.py
+-rw-r--r--   0 eric       (501) staff       (20)     6540 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/test_operation.py
+-rw-r--r--   0 eric       (501) staff       (20)     8151 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/test_runtime.py
+-rw-r--r--   0 eric       (501) staff       (20)     5584 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/test_subgraph.py
+-rw-r--r--   0 eric       (501) staff       (20)    49825 2023-05-15 03:20:39.000000 gmxapi-0.4.2/test/testdata.json
```

### Comparing `gmxapi-0.4.1/CMakeLists.txt` & `gmxapi-0.4.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/LICENSE` & `gmxapi-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/PKG-INFO` & `gmxapi-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmxapi
-Version: 0.4.1
+Version: 0.4.2
 Summary: gmxapi Python interface for GROMACS.
 Home-page: http://gmxapi.org/
 Author: GROMACS gmxapi team
 Author-email: info@gmxapi.org
 License: LGPL
 Requires-Python: >=3.7
 License-File: LICENSE
```

### Comparing `gmxapi-0.4.1/setup.cfg` & `gmxapi-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/setup.py` & `gmxapi-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/export_context.cpp` & `gmxapi-0.4.2/src/cpp/export_context.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/export_system.cpp` & `gmxapi-0.4.2/src/cpp/export_system.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/export_tprfile.cpp` & `gmxapi-0.4.2/src/cpp/export_tprfile.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/gmxpy_exceptions.cpp` & `gmxapi-0.4.2/src/cpp/gmxpy_exceptions.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/gmxpy_exceptions.h` & `gmxapi-0.4.2/src/cpp/gmxpy_exceptions.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/launch_0_2_1.cpp` & `gmxapi-0.4.2/src/cpp/launch_0_2_1.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/module.cpp` & `gmxapi-0.4.2/src/cpp/module.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/module.h` & `gmxapi-0.4.2/src/cpp/module.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/mpi_bindings.cpp` & `gmxapi-0.4.2/src/cpp/mpi_bindings.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/mpi_bindings.h` & `gmxapi-0.4.2/src/cpp/mpi_bindings.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/mpi_gromacs_support.cpp` & `gmxapi-0.4.2/src/cpp/mpi_gromacs_support.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/mpi_no_gromacs_support.cpp` & `gmxapi-0.4.2/src/cpp/mpi_no_gromacs_support.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/pycontext.cpp` & `gmxapi-0.4.2/src/cpp/pycontext.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/pycontext.h` & `gmxapi-0.4.2/src/cpp/pycontext.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/pycontext_create.cpp` & `gmxapi-0.4.2/src/cpp/pycontext_create.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/pycontext_create_no_mpi.cpp` & `gmxapi-0.4.2/src/cpp/pycontext_create_no_mpi.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/pysystem.cpp` & `gmxapi-0.4.2/src/cpp/pysystem.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/pysystem.h` & `gmxapi-0.4.2/src/cpp/pysystem.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/wrapped_exceptions.h` & `gmxapi-0.4.2/src/cpp/wrapped_exceptions.h`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/wrapped_exceptions_0_1_0.cpp` & `gmxapi-0.4.2/src/cpp/wrapped_exceptions_0_1_0.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/cpp/wrapped_exceptions_0_3_1.cpp` & `gmxapi-0.4.2/src/cpp/wrapped_exceptions_0_3_1.cpp`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/__init__.py` & `gmxapi-0.4.2/src/gmxapi/__init__.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/_logging.py` & `gmxapi-0.4.2/src/gmxapi/_logging.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/_transform.py` & `gmxapi-0.4.2/src/gmxapi/_transform.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/abc.py` & `gmxapi-0.4.2/src/gmxapi/abc.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/commandline.py` & `gmxapi-0.4.2/src/gmxapi/commandline.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/datamodel.py` & `gmxapi-0.4.2/src/gmxapi/datamodel.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/exceptions.py` & `gmxapi-0.4.2/src/gmxapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/operation.py` & `gmxapi-0.4.2/src/gmxapi/operation.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/runtime.py` & `gmxapi-0.4.2/src/gmxapi/runtime.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/simulation/__init__.py` & `gmxapi-0.4.2/src/gmxapi/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/simulation/abc.py` & `gmxapi-0.4.2/src/gmxapi/simulation/abc.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/simulation/context.py` & `gmxapi-0.4.2/src/gmxapi/simulation/context.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/simulation/fileio.py` & `gmxapi-0.4.2/src/gmxapi/simulation/fileio.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/simulation/mdrun.py` & `gmxapi-0.4.2/src/gmxapi/simulation/mdrun.py`

 * *Files 1% similar despite different names*

```diff
@@ -783,19 +783,27 @@
     @classmethod
     def _make_uid(cls, input) -> str:
         # WARNING: The built-in hash will use memory locations, and so will not be consistent across
         # process ranks, even if the input should be the same.
         # Note also that that hash() has internal salt that is regenerated for every process.
         # TODO: Use input fingerprint for more useful identification.
         # 8 bytes is probably enough.
-        uid = hashlib.md5("mdrun{cls._number_issued}".encode("utf8")).digest()
         if input not in cls._uids:
+            uid = hashlib.md5(f"mdrun{cls._number_issued}".encode("utf8")).digest()
+            existing = [key for key, value in cls._uids.items() if uid == value]
+            if existing:
+                raise exceptions.ProtocolError(
+                    f"Calculated uid {uid.hex()} for input {input}, but uid is already used by "
+                    + ", ".join(repr(edge) for edge in existing)
+                    + "."
+                )
             cls._uids[input] = uid
             cls._number_issued += 1
         else:
+            uid = cls._uids[input]
             logger.debug(f"Reissuing uid for mdrun({input}): {uid.hex()}")
         new_uid = f"mdrun_{uid.hex()}"
         return new_uid
 
     def signature(self) -> _op.InputCollectionDescription:
         return _input
```

### Comparing `gmxapi-0.4.1/src/gmxapi/simulation/modify_input.py` & `gmxapi-0.4.2/src/gmxapi/simulation/modify_input.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/simulation/read_tpr.py` & `gmxapi-0.4.2/src/gmxapi/simulation/read_tpr.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/simulation/workflow.py` & `gmxapi-0.4.2/src/gmxapi/simulation/workflow.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/testsupport.py` & `gmxapi-0.4.2/src/gmxapi/testsupport.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/typing.py` & `gmxapi-0.4.2/src/gmxapi/typing.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/utility.py` & `gmxapi-0.4.2/src/gmxapi/utility.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/src/gmxapi/version.py` & `gmxapi-0.4.2/src/gmxapi/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 import warnings
 
 from .exceptions import FeatureNotAvailableError
 
 # TODO(#3851): Version management policy and procedures.
 _major = 0
 _minor = 4
-_micro = 1
+_micro = 2
 _suffix = ""
 
 # Reference https://www.python.org/dev/peps/pep-0440/ and
 # https://packaging.pypa.io/en/latest/version/ for
 # versioning semantics and rules.
 __version__ = "{major}.{minor}.{micro}{suffix}".format(
     major=_major, minor=_minor, micro=_micro, suffix=_suffix
```

### Comparing `gmxapi-0.4.1/src/gmxapi.egg-info/PKG-INFO` & `gmxapi-0.4.2/src/gmxapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gmxapi
-Version: 0.4.1
+Version: 0.4.2
 Summary: gmxapi Python interface for GROMACS.
 Home-page: http://gmxapi.org/
 Author: GROMACS gmxapi team
 Author-email: info@gmxapi.org
 License: LGPL
 Requires-Python: >=3.7
 License-File: LICENSE
```

### Comparing `gmxapi-0.4.1/src/gmxapi.egg-info/SOURCES.txt` & `gmxapi-0.4.2/src/gmxapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/CMakeLists.txt` & `gmxapi-0.4.2/test/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/conftest.py` & `gmxapi-0.4.2/test/conftest.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/test_commandline.py` & `gmxapi-0.4.2/test/test_commandline.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/test_exceptions.py` & `gmxapi-0.4.2/test/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/test_feature_check.py` & `gmxapi-0.4.2/test/test_feature_check.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/test_fileio.py` & `gmxapi-0.4.2/test/test_fileio.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/test_fileio_low_level.py` & `gmxapi-0.4.2/test/test_fileio_low_level.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/test_mdrun.py` & `gmxapi-0.4.2/test/test_mdrun.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,16 @@
 
 TODO: Factory accepts additional keyword input to indicate binding
  to the "potential" interface.
 """
 
 import logging
 import os
+import pathlib
+
 import pytest
 
 import gmxapi as gmx
 
 from gmxapi.utility import join_path
 from gmxapi.version import api_is_at_least
 
@@ -241,14 +243,22 @@
                 "-cpi": md1.output.checkpoint,
                 "-cpo": "state.cpt",
                 "-noappend": None,
             }
             runtime_args.update(mdrun_kwargs)
             md2 = gmx.mdrun(input2, runtime_args=runtime_args)
             md2.run()
+
+            # Check for issue #4795 regression
+            output_dir1 = pathlib.Path(md1.output.directory.result()).resolve()
+            output_dir2 = pathlib.Path(md2.output.directory.result()).resolve()
+            assert output_dir1.exists()
+            assert output_dir2.exists()
+            assert output_dir2 != output_dir1
+
             # By inspection of the output, we can see that the second trajectory has continued
             # from the checkpoint, but we cannot programmatically confirm it at this point.
             # TODO: Check more rigorously when we can read trajectory files.
 
 
 @pytest.mark.withmpi_only
 @pytest.mark.usefixtures("cleandir")
```

### Comparing `gmxapi-0.4.1/test/test_operation.py` & `gmxapi-0.4.2/test/test_operation.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/test_runtime.py` & `gmxapi-0.4.2/test/test_runtime.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/test_subgraph.py` & `gmxapi-0.4.2/test/test_subgraph.py`

 * *Files identical despite different names*

### Comparing `gmxapi-0.4.1/test/testdata.json` & `gmxapi-0.4.2/test/testdata.json`

 * *Files identical despite different names*

