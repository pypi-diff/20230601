# Comparing `tmp/cad_to_dagmc-0.3.1.tar.gz` & `tmp/cad_to_dagmc-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cad_to_dagmc-0.3.1.tar", last modified: Tue May 30 21:42:46 2023, max compression
+gzip compressed data, was "cad_to_dagmc-0.3.2.tar", last modified: Thu Jun  1 21:41:48 2023, max compression
```

## Comparing `cad_to_dagmc-0.3.1.tar` & `cad_to_dagmc-0.3.2.tar`

### file list

```diff
@@ -1,75 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.108199 cad_to_dagmc-0.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.096199 cad_to_dagmc-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.096199 cad_to_dagmc-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/.github/workflows/anaconda-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/.github/workflows/ci_with_install.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-30 21:42:46.108199 cad_to_dagmc-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/environment.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.096199 cad_to_dagmc-0.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/cadquery_assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/cadquery_compound.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/cadquery_object_and_stp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/cadquery_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/create_stp_files_for_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/curved_cadquery_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/multiple_cadquery_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/multiple_stp_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/single_cadquery_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/single_stp_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/examples/single_stp_file_multiple_volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 21:42:46.108199 cad_to_dagmc-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.096199 cad_to_dagmc-0.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-30 21:42:45.000000 cad_to_dagmc-0.3.1/src/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.100199 cad_to_dagmc-0.3.1/src/cad_to_dagmc/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc/brep_part_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc/brep_to_h5m.py
--rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc/vertices_to_h5m.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.100199 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-05-30 21:42:46.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-05-30 21:42:46.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 21:42:46.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 21:42:46.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-30 21:42:46.000000 cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.104199 cad_to_dagmc-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/extrude_rectangle.stp
--rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/multi_volume_cylinders.stp
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/single_cube.stp
--rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/single_volume_thin.stp
--rw-r--r--   0 runner    (1001) docker     (123)  2013134 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/single_volume_thin.vtk
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.104199 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/
--rw-r--r--   0 runner    (1001) docker     (123)   267095 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/ball_reactor.brep
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_brep_part_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_matching_part_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_matching_part_id_with_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_matching_part_ids.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_loading_from_file_vs_shape_object.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.104199 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/create_brep_file_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/one_cube.brep
--rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_brep_file.brep
--rw-r--r--   0 runner    (1001) docker     (123)     8222 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_h5m_in_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_python_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_two_joined_cubes.brep
--rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_two_sep_cubes.brep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.108199 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/
--rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/extrude_rectangle.stp
--rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/multi_volume_cylinders.stp
--rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/single_cube.stp
--rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/single_volume_thin.stp
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_h5m_creation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_h5m_in_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/two_connected_cubes.stp
--rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/two_disconnected_cubes.stp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 21:42:46.108199 cad_to_dagmc-0.3.1/tests/test_vertices_to_h5m/
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/test_vertices_to_h5m/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/two_connected_cubes.stp
--rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-05-30 21:42:26.000000 cad_to_dagmc-0.3.1/tests/two_disconnected_cubes.stp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.270050 cad_to_dagmc-0.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.274050 cad_to_dagmc-0.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/.github/workflows/anaconda-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/.github/workflows/ci_with_install.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.274050 cad_to_dagmc-0.3.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/cadquery_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/cadquery_compound.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/cadquery_object_and_stp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/cadquery_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/create_stp_files_for_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/curved_cadquery_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/multiple_cadquery_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/multiple_stp_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/single_cadquery_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/single_stp_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/examples/single_stp_file_multiple_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.274050 cad_to_dagmc-0.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.274050 cad_to_dagmc-0.3.2/src/cad_to_dagmc/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc/brep_part_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc/brep_to_h5m.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5547 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc/vertices_to_h5m.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.274050 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 21:41:48.000000 cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.278050 cad_to_dagmc-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    71272 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/ENDFB-7.1-NNDC_H1.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/extrude_rectangle.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/multi_volume_cylinders.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/single_cube.stp
+-rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/single_volume_thin.stp
+-rw-r--r--   0 runner    (1001) docker     (123)  2013134 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/single_volume_thin.vtk
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.278050 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/
+-rw-r--r--   0 runner    (1001) docker     (123)   267095 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/ball_reactor.brep
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_brep_part_properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_matching_part_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_matching_part_id_with_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1417 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_matching_part_ids.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_loading_from_file_vs_shape_object.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/create_brep_file_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/one_cube.brep
+-rw-r--r--   0 runner    (1001) docker     (123)    11805 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_brep_file.brep
+-rw-r--r--   0 runner    (1001) docker     (123)     8798 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_h5m_in_transport.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_python_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_two_joined_cubes.brep
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_two_sep_cubes.brep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/
+-rw-r--r--   0 runner    (1001) docker     (123)    22142 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/extrude_rectangle.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    87541 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/multi_volume_cylinders.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    15945 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/single_cube.stp
+-rw-r--r--   0 runner    (1001) docker     (123)   212436 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/single_volume_thin.stp
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_h5m_creation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4587 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_h5m_in_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/two_connected_cubes.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/two_disconnected_cubes.stp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:41:48.282050 cad_to_dagmc-0.3.2/tests/test_vertices_to_h5m/
+-rw-r--r--   0 runner    (1001) docker     (123)    12432 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/test_vertices_to_h5m/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33452 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/two_connected_cubes.stp
+-rw-r--r--   0 runner    (1001) docker     (123)    33391 2023-06-01 21:41:31.000000 cad_to_dagmc-0.3.2/tests/two_disconnected_cubes.stp
```

### Comparing `cad_to_dagmc-0.3.1/.github/workflows/anaconda-publish.yml` & `cad_to_dagmc-0.3.2/.github/workflows/anaconda-publish.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/.github/workflows/black.yml` & `cad_to_dagmc-0.3.2/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/.github/workflows/ci_with_install.yml` & `cad_to_dagmc-0.3.2/.github/workflows/ci_with_install.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/.github/workflows/python-publish.yml` & `cad_to_dagmc-0.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/.gitignore` & `cad_to_dagmc-0.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/LICENSE` & `cad_to_dagmc-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/PKG-INFO` & `cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cad_to_dagmc
-Version: 0.3.1
+Name: cad-to-dagmc
+Version: 0.3.2
 Summary: Converts CAD files to a DAGMC h5m file
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/cad_to_dagmc
 Project-URL: Bug Tracker, https://github.com/fusion-energy/cad_to_dagmc/issues
 Keywords: dagmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,20 +18,19 @@
 [![N|Python](https://www.python.org/static/community_logos/python-powered-w-100x40.png)](https://www.python.org)
 
 [![CI with install](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/ci_with_install.yml/badge.svg)](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/ci_with_install.yml)
 
 [![Upload Python Package](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/python-publish.yml/badge.svg)](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/python-publish.yml)
 
 
-[![conda-publish](https://anaconda.org/fusion-energy/cad_to_dagmc/badges/version.svg)](https://anaconda.org/fusion-energy/cad_to_dagmc)
 [![PyPI](https://img.shields.io/pypi/v/cad_to_dagmc?color=brightgreen&label=pypi&logo=grebrightgreenen&logoColor=green)](https://pypi.org/project/cad_to_dagmc/)
 
 ___
 
-A minimal package that uses CadQuery functionality to convert Cad geometry to DAGMC h5m files
+A minimal package that uses CadQuery functionality to convert Cad geometry to [DAGMC](https://github.com/svalinn/DAGMC/) h5m files
 
 This particular method of producing DAGMC compatible h5m files from CAD geometry
 is intended to convert STP files or [CadQuery](https://cadquery.readthedocs.io) objects to h5m file.
 
 One unique feature of this package is the ability to combine STP files with CadQuery objects.
 This allows for the addition of parametric geometry to static geometry.
 
@@ -41,15 +40,15 @@
 ```bash
 conda create --name new_env python=3.9
 conda activate new_env
 ```
 
 Installs cad_to_dagmc and dependencies
 ```bash
-conda install -c fusion-energy -c cadquery -c conda-forge cad_to_dagmc
+conda install -c conda-forge cad_to_dagmc
 ```
 # Install (Mamba)
 
 Creates a new empty Conda environment and activate it
 ```bash
 conda create --name new_env python=3.9
 conda activate new_env
@@ -58,15 +57,15 @@
 Installs Mamba
 ```bash
 conda install -c conda-forge mamba
 ```
 
 Installs cad_to_dagmc and dependencies
 ```bash
-mamba install -c fusion-energy -c cadquery -c conda-forge cad_to_dagmc
+mamba install -c conda-forge cad_to_dagmc
 ```
 
 # Install (Conda + pip)
 
 You will need to install some dependencies that are not available via PyPi.
 This example uses Conda but Mamba could also be used.
 ```bash
```

### Comparing `cad_to_dagmc-0.3.1/README.md` & `cad_to_dagmc-0.3.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,20 +2,19 @@
 [![N|Python](https://www.python.org/static/community_logos/python-powered-w-100x40.png)](https://www.python.org)
 
 [![CI with install](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/ci_with_install.yml/badge.svg)](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/ci_with_install.yml)
 
 [![Upload Python Package](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/python-publish.yml/badge.svg)](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/python-publish.yml)
 
 
-[![conda-publish](https://anaconda.org/fusion-energy/cad_to_dagmc/badges/version.svg)](https://anaconda.org/fusion-energy/cad_to_dagmc)
 [![PyPI](https://img.shields.io/pypi/v/cad_to_dagmc?color=brightgreen&label=pypi&logo=grebrightgreenen&logoColor=green)](https://pypi.org/project/cad_to_dagmc/)
 
 ___
 
-A minimal package that uses CadQuery functionality to convert Cad geometry to DAGMC h5m files
+A minimal package that uses CadQuery functionality to convert Cad geometry to [DAGMC](https://github.com/svalinn/DAGMC/) h5m files
 
 This particular method of producing DAGMC compatible h5m files from CAD geometry
 is intended to convert STP files or [CadQuery](https://cadquery.readthedocs.io) objects to h5m file.
 
 One unique feature of this package is the ability to combine STP files with CadQuery objects.
 This allows for the addition of parametric geometry to static geometry.
 
@@ -25,15 +24,15 @@
 ```bash
 conda create --name new_env python=3.9
 conda activate new_env
 ```
 
 Installs cad_to_dagmc and dependencies
 ```bash
-conda install -c fusion-energy -c cadquery -c conda-forge cad_to_dagmc
+conda install -c conda-forge cad_to_dagmc
 ```
 # Install (Mamba)
 
 Creates a new empty Conda environment and activate it
 ```bash
 conda create --name new_env python=3.9
 conda activate new_env
@@ -42,15 +41,15 @@
 Installs Mamba
 ```bash
 conda install -c conda-forge mamba
 ```
 
 Installs cad_to_dagmc and dependencies
 ```bash
-mamba install -c fusion-energy -c cadquery -c conda-forge cad_to_dagmc
+mamba install -c conda-forge cad_to_dagmc
 ```
 
 # Install (Conda + pip)
 
 You will need to install some dependencies that are not available via PyPi.
 This example uses Conda but Mamba could also be used.
 ```bash
```

### Comparing `cad_to_dagmc-0.3.1/examples/cadquery_compound.py` & `cad_to_dagmc-0.3.2/examples/cadquery_compound.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/examples/create_stp_files_for_examples.py` & `cad_to_dagmc-0.3.2/examples/create_stp_files_for_examples.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/examples/curved_cadquery_object.py` & `cad_to_dagmc-0.3.2/examples/curved_cadquery_object.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/src/cad_to_dagmc/__init__.py` & `cad_to_dagmc-0.3.2/src/cad_to_dagmc/__init__.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/src/cad_to_dagmc/brep_part_finder.py` & `cad_to_dagmc-0.3.2/src/cad_to_dagmc/brep_part_finder.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/src/cad_to_dagmc/brep_to_h5m.py` & `cad_to_dagmc-0.3.2/src/cad_to_dagmc/brep_to_h5m.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/src/cad_to_dagmc/core.py` & `cad_to_dagmc-0.3.2/src/cad_to_dagmc/core.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/src/cad_to_dagmc/vertices_to_h5m.py` & `cad_to_dagmc-0.3.2/src/cad_to_dagmc/vertices_to_h5m.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/PKG-INFO` & `cad_to_dagmc-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cad-to-dagmc
-Version: 0.3.1
+Name: cad_to_dagmc
+Version: 0.3.2
 Summary: Converts CAD files to a DAGMC h5m file
 Author-email: Jonathan Shimwell <mail@jshimwell.com>
 Project-URL: Homepage, https://github.com/fusion-energy/cad_to_dagmc
 Project-URL: Bug Tracker, https://github.com/fusion-energy/cad_to_dagmc/issues
 Keywords: dagmc,geometry,plot,slice
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -18,20 +18,19 @@
 [![N|Python](https://www.python.org/static/community_logos/python-powered-w-100x40.png)](https://www.python.org)
 
 [![CI with install](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/ci_with_install.yml/badge.svg)](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/ci_with_install.yml)
 
 [![Upload Python Package](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/python-publish.yml/badge.svg)](https://github.com/fusion-energy/cad_to_dagmc/actions/workflows/python-publish.yml)
 
 
-[![conda-publish](https://anaconda.org/fusion-energy/cad_to_dagmc/badges/version.svg)](https://anaconda.org/fusion-energy/cad_to_dagmc)
 [![PyPI](https://img.shields.io/pypi/v/cad_to_dagmc?color=brightgreen&label=pypi&logo=grebrightgreenen&logoColor=green)](https://pypi.org/project/cad_to_dagmc/)
 
 ___
 
-A minimal package that uses CadQuery functionality to convert Cad geometry to DAGMC h5m files
+A minimal package that uses CadQuery functionality to convert Cad geometry to [DAGMC](https://github.com/svalinn/DAGMC/) h5m files
 
 This particular method of producing DAGMC compatible h5m files from CAD geometry
 is intended to convert STP files or [CadQuery](https://cadquery.readthedocs.io) objects to h5m file.
 
 One unique feature of this package is the ability to combine STP files with CadQuery objects.
 This allows for the addition of parametric geometry to static geometry.
 
@@ -41,15 +40,15 @@
 ```bash
 conda create --name new_env python=3.9
 conda activate new_env
 ```
 
 Installs cad_to_dagmc and dependencies
 ```bash
-conda install -c fusion-energy -c cadquery -c conda-forge cad_to_dagmc
+conda install -c conda-forge cad_to_dagmc
 ```
 # Install (Mamba)
 
 Creates a new empty Conda environment and activate it
 ```bash
 conda create --name new_env python=3.9
 conda activate new_env
@@ -58,15 +57,15 @@
 Installs Mamba
 ```bash
 conda install -c conda-forge mamba
 ```
 
 Installs cad_to_dagmc and dependencies
 ```bash
-mamba install -c fusion-energy -c cadquery -c conda-forge cad_to_dagmc
+mamba install -c conda-forge cad_to_dagmc
 ```
 
 # Install (Conda + pip)
 
 You will need to install some dependencies that are not available via PyPi.
 This example uses Conda but Mamba could also be used.
 ```bash
```

### Comparing `cad_to_dagmc-0.3.1/src/cad_to_dagmc.egg-info/SOURCES.txt` & `cad_to_dagmc-0.3.2/src/cad_to_dagmc.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 src/cad_to_dagmc/core.py
 src/cad_to_dagmc/vertices_to_h5m.py
 src/cad_to_dagmc.egg-info/PKG-INFO
 src/cad_to_dagmc.egg-info/SOURCES.txt
 src/cad_to_dagmc.egg-info/dependency_links.txt
 src/cad_to_dagmc.egg-info/requires.txt
 src/cad_to_dagmc.egg-info/top_level.txt
+tests/ENDFB-7.1-NNDC_H1.h5
 tests/extrude_rectangle.stp
 tests/multi_volume_cylinders.stp
 tests/single_cube.stp
 tests/single_volume_thin.stp
 tests/single_volume_thin.vtk
 tests/two_connected_cubes.stp
 tests/two_disconnected_cubes.stp
```

### Comparing `cad_to_dagmc-0.3.1/tests/extrude_rectangle.stp` & `cad_to_dagmc-0.3.2/tests/extrude_rectangle.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/multi_volume_cylinders.stp` & `cad_to_dagmc-0.3.2/tests/multi_volume_cylinders.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/single_cube.stp` & `cad_to_dagmc-0.3.2/tests/single_cube.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/single_volume_thin.stp` & `cad_to_dagmc-0.3.2/tests/single_volume_thin.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/single_volume_thin.vtk` & `cad_to_dagmc-0.3.2/tests/single_volume_thin.vtk`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_part_finder/ball_reactor.brep` & `cad_to_dagmc-0.3.2/tests/test_brep_part_finder/ball_reactor.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_brep_part_properties.py` & `cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_brep_part_properties.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_matching_part_id.py` & `cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_matching_part_id.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_matching_part_id_with_file.py` & `cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_matching_part_id_with_file.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_get_matching_part_ids.py` & `cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_get_matching_part_ids.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_part_finder/test_loading_from_file_vs_shape_object.py` & `cad_to_dagmc-0.3.2/tests/test_brep_part_finder/test_loading_from_file_vs_shape_object.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/create_brep_file_for_testing.py` & `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/create_brep_file_for_testing.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/one_cube.brep` & `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/one_cube.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_brep_file.brep` & `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_brep_file.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_h5m_in_transport.py` & `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_h5m_in_transport.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import openmc
-import openmc_data_downloader
 from cad_to_dagmc.brep_to_h5m import brep_to_h5m
 import math
 
 from cad_to_dagmc.brep_to_h5m import (
     mesh_brep,
     mesh_to_h5m_in_memory_method,
 )
@@ -21,16 +20,15 @@
     h5m_filename: str,
     material_tags: list,
     nuclides: list = None,
     cross_sections_xml: str = None,
 ):
     """A function for testing the geometry file with particle transport in
     DAGMC OpenMC. Requires openmc and either the cross_sections_xml to be
-    specified or openmc_data_downloader installed. Returns the flux on each
-    volume
+    specified. Returns the flux on each volume
 
     Arg:
         h5m_filename: The name of the DAGMC h5m file to test
         material_tags: The
         nuclides:
         cross_sections_xml:
 
@@ -43,27 +41,34 @@
         nuclides = list(NATURAL_ABUNDANCE.keys())
 
     materials = openmc.Materials()
     for i, material_tag in enumerate(material_tags):
         # simplified material definitions have been used to keen this example minimal
         mat_dag_material_tag = openmc.Material(name=material_tag)
         mat_dag_material_tag.add_nuclide(nuclides[i], 1, "ao")
-        mat_dag_material_tag.set_density("g/cm3", 0.1)
+        mat_dag_material_tag.set_density("g/cm3", 0.01)
 
         materials.append(mat_dag_material_tag)
 
     if cross_sections_xml:
-        materials.cross_sections = cross_sections_xml
+        openmc.config["cross_sections"] = cross_sections_xml
+
     else:
-        # downloads the nuclear data and sets the openmc_cross_sections environmental variable
-        materials.download_cross_section_data(
-            libraries=["ENDFB-7.1-NNDC"],
-            set_OPENMC_CROSS_SECTIONS=True,
-            particles=["neutron"],
-        )
+        with open("cross_sections.xml", "w") as file:
+            file.write(
+                """
+            <?xml version='1.0' encoding='UTF-8'?>
+            <cross_sections>
+            <library materials="H1" path="tests/ENDFB-7.1-NNDC_H1.h5" type="neutron"/>
+            <library materials="H2" path="ENDFB-7.1-NNDC_H2.h5" type="neutron"/>
+            </cross_sections>
+            """
+            )
+
+        openmc.config["cross_sections"] = "cross_sections.xml"
 
     dag_univ = openmc.DAGMCUniverse(filename=h5m_filename)
     bound_dag_univ = dag_univ.bounded_universe()
     geometry = openmc.Geometry(root=bound_dag_univ)
 
     # initializes a new source object
     my_source = openmc.Source()
@@ -129,15 +134,17 @@
         h5m_filename=h5m_filename,
         min_mesh_size=30,
         max_mesh_size=50,
         mesh_algorithm=1,
     )
 
     transport_particles_on_h5m_geometry(
-        h5m_filename=h5m_filename, material_tags=material_tags
+        h5m_filename=h5m_filename,
+        material_tags=material_tags,
+        nuclides=["H1"] * len(material_tags),
     )
 
 
 def test_transport_on_h5m_with_1_volumes():
     brep_filename = "tests/test_brep_to_h5m/one_cube.brep"
     h5m_filename = "one_cube.h5m"
     volumes = 1
@@ -149,15 +156,17 @@
         h5m_filename=h5m_filename,
         min_mesh_size=30,
         max_mesh_size=50,
         mesh_algorithm=1,
     )
 
     transport_particles_on_h5m_geometry(
-        h5m_filename=h5m_filename, material_tags=material_tags
+        h5m_filename=h5m_filename,
+        material_tags=material_tags,
+        nuclides=["H1"] * len(material_tags),
     )
 
 
 def test_transport_on_h5m_with_2_joined_volumes():
     brep_filename = "tests/test_brep_to_h5m/test_two_joined_cubes.brep"
     h5m_filename = "test_two_joined_cubes.h5m"
     volumes = 2
@@ -169,15 +178,17 @@
         h5m_filename=h5m_filename,
         min_mesh_size=30,
         max_mesh_size=50,
         mesh_algorithm=1,
     )
 
     transport_particles_on_h5m_geometry(
-        h5m_filename=h5m_filename, material_tags=material_tags
+        h5m_filename=h5m_filename,
+        material_tags=material_tags,
+        nuclides=["H1"] * len(material_tags),
     )
 
 
 def test_transport_on_h5m_with_2_sep_volumes():
     brep_filename = "tests/test_brep_to_h5m/test_two_sep_cubes.brep"
     h5m_filename = "test_two_sep_cubes.h5m"
     volumes = 2
@@ -189,15 +200,17 @@
         h5m_filename=h5m_filename,
         min_mesh_size=30,
         max_mesh_size=50,
         mesh_algorithm=1,
     )
 
     transport_particles_on_h5m_geometry(
-        h5m_filename=h5m_filename, material_tags=material_tags
+        h5m_filename=h5m_filename,
+        material_tags=material_tags,
+        nuclides=["H1"] * len(material_tags),
     )
 
 
 def test_transport_result_h5m_with_2_sep_volumes():
     brep_filename = "tests/test_brep_to_h5m/test_two_sep_cubes.brep"
     h5m_filename = "test_two_sep_cubes.h5m"
     volumes = 2
@@ -209,27 +222,31 @@
         h5m_filename=h5m_filename,
         min_mesh_size=30,
         max_mesh_size=50,
         mesh_algorithm=1,
     )
 
     new_tally = transport_particles_on_h5m_geometry(
-        h5m_filename=h5m_filename, material_tags=material_tags
+        h5m_filename=h5m_filename,
+        material_tags=material_tags,
+        nuclides=["H1"] * len(material_tags),
     )
 
     brep_to_h5m(
         brep_filename=brep_filename,
         material_tags=material_tags,
         h5m_filename=h5m_filename,
         min_mesh_size=30,
         max_mesh_size=50,
         mesh_algorithm=1,
     )
     stl_tally = transport_particles_on_h5m_geometry(
-        h5m_filename=h5m_filename, material_tags=material_tags
+        h5m_filename=h5m_filename,
+        material_tags=material_tags,
+        nuclides=["H1"] * len(material_tags),
     )
 
     assert math.isclose(new_tally, stl_tally)
 
 
 def test_stl_vs_in_memory_1_volume():
     brep_filename = "tests/test_brep_to_h5m/one_cube.brep"
@@ -246,15 +263,17 @@
     mesh_to_h5m_in_memory_method(
         volumes=volumes,
         material_tags=material_tags,
         h5m_filename="h5m_from_in_memory_method.h5m",
     )
 
     transport_particles_on_h5m_geometry(
-        h5m_filename="h5m_from_in_memory_method.h5m", material_tags=material_tags
+        h5m_filename="h5m_from_in_memory_method.h5m",
+        material_tags=material_tags,
+        nuclides=["H1"] * len(material_tags),
     )
 
 
 def test_stl_vs_in_memory_2_joined_volume():
     brep_filename = "tests/test_brep_to_h5m/test_two_joined_cubes.brep"
     volumes = 2
     material_tags = [f"material_{n}" for n in range(1, volumes + 1)]
@@ -269,9 +288,11 @@
     mesh_to_h5m_in_memory_method(
         volumes=volumes,
         material_tags=material_tags,
         h5m_filename="h5m_from_in_memory_method.h5m",
     )
 
     transport_particles_on_h5m_geometry(
-        h5m_filename="h5m_from_in_memory_method.h5m", material_tags=material_tags
+        h5m_filename="h5m_from_in_memory_method.h5m",
+        material_tags=material_tags,
+        nuclides=["H1"] * len(material_tags),
     )
```

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_python_api.py` & `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_python_api.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_two_joined_cubes.brep` & `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_two_joined_cubes.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_brep_to_h5m/test_two_sep_cubes.brep` & `cad_to_dagmc-0.3.2/tests/test_brep_to_h5m/test_two_sep_cubes.brep`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/extrude_rectangle.stp` & `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/extrude_rectangle.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/multi_volume_cylinders.stp` & `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/multi_volume_cylinders.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/single_cube.stp` & `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/single_cube.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/single_volume_thin.stp` & `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/single_volume_thin.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_h5m_creation.py` & `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_h5m_creation.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_h5m_in_simulation.py` & `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_h5m_in_simulation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import openmc
-import openmc_data_downloader
-
 
 """
     - h5m files can be used a transport geometry in DAGMC with OpenMC
 """
 
 
 def transport_particles_on_h5m_geometry(
     h5m_filename,
     material_tags,
 ):
     """A function for testing the geometry file with particle transport in DAGMC OpenMC"""
 
+    with open("cross_sections.xml", "w") as file:
+        file.write(
+            """
+        <?xml version='1.0' encoding='UTF-8'?>
+        <cross_sections>
+        <library materials="H1" path="tests/ENDFB-7.1-NNDC_H1.h5" type="neutron"/>
+        <library materials="H2" path="ENDFB-7.1-NNDC_H2.h5" type="neutron"/>
+        </cross_sections>
+        """
+        )
+
+    openmc.config["cross_sections"] = "cross_sections.xml"
+
     materials = openmc.Materials()
     for material_tag in material_tags:
         # simplified material definitions have been used to keen this example minimal
         mat_dag_material_tag = openmc.Material(name=material_tag)
         mat_dag_material_tag.add_nuclide("H1", 1, "ao")
-        mat_dag_material_tag.set_density("g/cm3", 2)
+        mat_dag_material_tag.set_density("g/cm3", 0.01)
 
         materials.append(mat_dag_material_tag)
 
-    materials.download_cross_section_data(
-        libraries=["ENDFB-7.1-NNDC"],
-        set_OPENMC_CROSS_SECTIONS=True,
-        particles=["neutron"],
-    )
-
     # makes use of the dagmc geometry
     dag_univ = openmc.DAGMCUniverse(h5m_filename)
 
     # creates an edge of universe boundary surface
     vac_surf = openmc.Sphere(r=10000, surface_id=9999, boundary_type="vacuum")
 
     # specifies the region as below the universe boundary
```

### Comparing `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/test_version.py` & `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/test_version.py`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/two_connected_cubes.stp` & `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/two_connected_cubes.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_cad_to_dagmc/two_disconnected_cubes.stp` & `cad_to_dagmc-0.3.2/tests/test_cad_to_dagmc/two_disconnected_cubes.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/test_vertices_to_h5m/test_package.py` & `cad_to_dagmc-0.3.2/tests/test_vertices_to_h5m/test_package.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from pathlib import Path
 
 import numpy as np
 import openmc
-import openmc_data_downloader
 import pymoab as mb
 from pymoab import core, types
 
 from cad_to_dagmc import vertices_to_h5m
 
 """
 Tests that check that:
@@ -54,28 +53,39 @@
 ):
     """A function for testing the geometry file with particle transport in DAGMC OpenMC"""
 
     materials = openmc.Materials()
     for material_tag in material_tags:
         # simplified material definitions have been used to keen this example minimal
         mat_dag_material_tag = openmc.Material(name=material_tag)
-        mat_dag_material_tag.add_element("H", 1, "ao")
-        mat_dag_material_tag.set_density("g/cm3", 2)
+        mat_dag_material_tag.add_nuclide("H1", 1, "ao")
+        mat_dag_material_tag.set_density("g/cm3", 0.01)
 
         materials.append(mat_dag_material_tag)
 
     if cross_sections_xml:
         materials.cross_sections = cross_sections_xml
     # downloads the nuclear data and sets the openmc_cross_sections environmental variable
 
-    materials.download_cross_section_data(
-        libraries=["ENDFB-7.1-NNDC"],
-        set_OPENMC_CROSS_SECTIONS=True,
-        particles=["neutron"],
-    )
+    if cross_sections_xml:
+        openmc.config["cross_sections"] = cross_sections_xml
+
+    else:
+        with open("cross_sections.xml", "w") as file:
+            file.write(
+                """
+            <?xml version='1.0' encoding='UTF-8'?>
+            <cross_sections>
+            <library materials="H1" path="tests/ENDFB-7.1-NNDC_H1.h5" type="neutron"/>
+            <library materials="H2" path="ENDFB-7.1-NNDC_H2.h5" type="neutron"/>
+            </cross_sections>
+            """
+            )
+
+        openmc.config["cross_sections"] = "cross_sections.xml"
 
     # makes use of the dagmc geometry
     dag_univ = openmc.DAGMCUniverse(h5m_filename)
 
     # creates an edge of universe boundary surface
     vac_surf = openmc.Sphere(r=10000, surface_id=9999, boundary_type="vacuum")
```

### Comparing `cad_to_dagmc-0.3.1/tests/two_connected_cubes.stp` & `cad_to_dagmc-0.3.2/tests/two_connected_cubes.stp`

 * *Files identical despite different names*

### Comparing `cad_to_dagmc-0.3.1/tests/two_disconnected_cubes.stp` & `cad_to_dagmc-0.3.2/tests/two_disconnected_cubes.stp`

 * *Files identical despite different names*

