# Comparing `tmp/vivarium-1.1.0.tar.gz` & `tmp/vivarium-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium-1.1.0.tar", last modified: Wed May  3 21:39:46 2023, max compression
+gzip compressed data, was "vivarium-1.2.0.tar", last modified: Thu Jun  1 18:57:30 2023, max compression
```

## Comparing `vivarium-1.1.0.tar` & `vivarium-1.2.0.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.946247 vivarium-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-03 21:39:34.000000 vivarium-1.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-05-03 21:39:34.000000 vivarium-1.1.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-03 21:39:34.000000 vivarium-1.1.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-03 21:39:34.000000 vivarium-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-03 21:39:34.000000 vivarium-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-03 21:39:46.946247 vivarium-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-03 21:39:34.000000 vivarium-1.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/docs/source/api_reference/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/config_tree.rst
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/exceptions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/artifact/artifact.rst
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/artifact/hdf.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/artifact/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/artifact/manager.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/components/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/components/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/components/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/components/parser.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/engine.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/event.rst
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/lifecycle.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/logging/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/logging/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/logging/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/lookup.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/metrics.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/plugins.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/population/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/population/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/population/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/population/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/population/population_view.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/framework/randomness/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/randomness/exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/randomness/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/randomness/index_map.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/randomness/manager.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/randomness/stream.rst
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/resource.rst
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/state_machine.rst
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/time.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/framework/values.rst
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.922246 vivarium-1.1.0/docs/source/api_reference/interface/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/interface/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/interface/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/interface/interactive.rst
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/interface/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/interpolation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/api_reference/testing_utilities.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.926246 vivarium-1.1.0/docs/source/concepts/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/builder.rst
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/components.rst
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/crn.rst
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/entry_points.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/event.rst
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/interpolation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/lifecycle.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/logging.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/lookup.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.926246 vivarium-1.1.0/docs/source/concepts/model_specification/
--rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/model_specification/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/model_specification/yaml_basics.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/population.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/resource.rst
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/time.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/concepts/values.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.926246 vivarium-1.1.0/docs/source/images/
--rw-r--r--   0 runner    (1001) docker     (123)    32924 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/images/crn_compare_cubes.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   474719 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/images/crn_cube.jpg
--rw-r--r--   0 runner    (1001) docker     (123)   736204 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/images/crn_sim_alignment.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    12794 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/images/pipeline.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.926246 vivarium-1.1.0/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/artifact.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/boids.rst
--rw-r--r--   0 runner    (1001) docker     (123)    30080 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/disease_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11789 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/exploration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.926246 vivarium-1.1.0/docs/source/tutorials/running_a_simulation/
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/running_a_simulation/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/running_a_simulation/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-05-03 21:39:34.000000 vivarium-1.1.0/docs/source/tutorials/running_a_simulation/interactive.rst
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-03 21:39:34.000000 vivarium-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:39:46.946247 vivarium-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-05-03 21:39:34.000000 vivarium-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.918246 vivarium-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium/
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20046 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/config_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium/examples/boids/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/boids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/boids/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/boids/neighbors.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/boids/population.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/boids/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium/examples/disease_model/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/disease.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/disease_model.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/intervention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/mortality.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/observer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/population.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/examples/disease_model/risk.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/artifact/artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/artifact/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/artifact/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/components/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/components/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/components/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/event.py
--rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/lifecycle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/logging/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/logging/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/population/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/population/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/population/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/population/population_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/randomness/
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/randomness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/randomness/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9330 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/randomness/index_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/randomness/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/randomness/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/framework/results/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/results/stratification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17224 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    23704 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/framework/values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/src/vivarium/interface/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/interface/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/interface/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/interface/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14074 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-05-03 21:39:34.000000 vivarium-1.1.0/src/vivarium/testing_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.930246 vivarium-1.1.0/src/vivarium.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 21:39:46.000000 vivarium-1.1.0/src/vivarium.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.934247 vivarium-1.1.0/tests/config_tree/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/config_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/config_tree/test_basic_functionality.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/config_tree/test_ingestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/artifact/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/artifact/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/artifact/test_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/artifact/test_hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/artifact/test_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/components/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/components/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/components/test_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/population/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/population/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/population/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/population/test_population_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/randomness/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/test_crn.py
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/test_index_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/randomness/test_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.942247 vivarium-1.1.0/tests/framework/results/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6345 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/results/test_stratification.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_state_machine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/framework/test_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.946247 vivarium-1.1.0/tests/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/interface/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 21:39:46.946247 vivarium-1.1.0/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/test_data/bad_model_specification.txt
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/test_data/mock_model_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/test_data/mock_user_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-05-03 21:39:34.000000 vivarium-1.1.0/tests/test_interpolation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.537930 vivarium-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     9909 2023-06-01 18:57:20.000000 vivarium-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3267 2023-06-01 18:57:20.000000 vivarium-1.2.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-01 18:57:20.000000 vivarium-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-01 18:57:20.000000 vivarium-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 18:57:20.000000 vivarium-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-01 18:57:30.537930 vivarium-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-06-01 18:57:20.000000 vivarium-1.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.517930 vivarium-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.517930 vivarium-1.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.517930 vivarium-1.2.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.517930 vivarium-1.2.0/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.517930 vivarium-1.2.0/docs/source/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/config_tree.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/exceptions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.517930 vivarium-1.2.0/docs/source/api_reference/framework/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.521930 vivarium-1.2.0/docs/source/api_reference/framework/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/artifact/artifact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/artifact/hdf.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/artifact/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/artifact/manager.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.521930 vivarium-1.2.0/docs/source/api_reference/framework/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/components/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/components/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/components/parser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/engine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/event.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/lifecycle.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.521930 vivarium-1.2.0/docs/source/api_reference/framework/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/logging/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/logging/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/logging/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/lookup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/metrics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/plugins.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.521930 vivarium-1.2.0/docs/source/api_reference/framework/population/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/population/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/population/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/population/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/population/population_view.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.521930 vivarium-1.2.0/docs/source/api_reference/framework/randomness/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/randomness/exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/randomness/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/randomness/index_map.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/randomness/manager.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/randomness/stream.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/resource.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/state_machine.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/time.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/framework/values.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.521930 vivarium-1.2.0/docs/source/api_reference/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/interface/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/interface/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/interface/interactive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/interface/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/api_reference/testing_utilities.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.521930 vivarium-1.2.0/docs/source/concepts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/builder.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/components.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10758 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/crn.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/entry_points.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/event.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/interpolation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8511 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/lifecycle.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/logging.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9744 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/lookup.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.521930 vivarium-1.2.0/docs/source/concepts/model_specification/
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/model_specification/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/model_specification/yaml_basics.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/population.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/resource.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/time.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5624 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/concepts/values.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.525930 vivarium-1.2.0/docs/source/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    32924 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/images/crn_compare_cubes.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   474719 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/images/crn_cube.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)   736204 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/images/crn_sim_alignment.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    12794 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/images/pipeline.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.525930 vivarium-1.2.0/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/tutorials/artifact.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12496 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/tutorials/boids.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    30080 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/tutorials/disease_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/tutorials/exploration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/tutorials/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/tutorials/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.525930 vivarium-1.2.0/docs/source/tutorials/running_a_simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/tutorials/running_a_simulation/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/tutorials/running_a_simulation/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-06-01 18:57:20.000000 vivarium-1.2.0/docs/source/tutorials/running_a_simulation/interactive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-01 18:57:20.000000 vivarium-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:57:30.537930 vivarium-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3482 2023-06-01 18:57:20.000000 vivarium-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.513930 vivarium-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.525930 vivarium-1.2.0/src/vivarium/
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20046 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/config_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.525930 vivarium-1.2.0/src/vivarium/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.525930 vivarium-1.2.0/src/vivarium/examples/boids/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/boids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/boids/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/boids/neighbors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/boids/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/boids/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.529930 vivarium-1.2.0/src/vivarium/examples/disease_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/disease_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7405 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/disease_model/disease.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/disease_model/disease_model.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/disease_model/intervention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/disease_model/mortality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/disease_model/observer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/disease_model/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/examples/disease_model/risk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.529930 vivarium-1.2.0/src/vivarium/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.529930 vivarium-1.2.0/src/vivarium/framework/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10295 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/artifact/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/artifact/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/artifact/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.529930 vivarium-1.2.0/src/vivarium/framework/components/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11649 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/components/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9449 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/components/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15142 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22771 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/lifecycle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.529930 vivarium-1.2.0/src/vivarium/framework/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/logging/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/logging/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15012 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5924 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.529930 vivarium-1.2.0/src/vivarium/framework/population/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/population/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17485 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/population/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21337 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/population/population_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.529930 vivarium-1.2.0/src/vivarium/framework/randomness/
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/randomness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/randomness/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/randomness/index_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9250 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/randomness/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15022 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/randomness/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12195 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.533930 vivarium-1.2.0/src/vivarium/framework/results/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/results/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/results/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/results/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/results/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/results/stratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23704 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/framework/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.533930 vivarium-1.2.0/src/vivarium/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6673 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/interface/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/interface/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4512 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/interface/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12964 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-01 18:57:20.000000 vivarium-1.2.0/src/vivarium/testing_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.525930 vivarium-1.2.0/src/vivarium.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-06-01 18:57:30.000000 vivarium-1.2.0/src/vivarium.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-06-01 18:57:30.000000 vivarium-1.2.0/src/vivarium.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:57:30.000000 vivarium-1.2.0/src/vivarium.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 18:57:30.000000 vivarium-1.2.0/src/vivarium.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:57:30.000000 vivarium-1.2.0/src/vivarium.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-01 18:57:30.000000 vivarium-1.2.0/src/vivarium.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-01 18:57:30.000000 vivarium-1.2.0/src/vivarium.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.533930 vivarium-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.533930 vivarium-1.2.0/tests/config_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/config_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15651 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/config_tree/test_basic_functionality.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/config_tree/test_ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.533930 vivarium-1.2.0/tests/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.533930 vivarium-1.2.0/tests/framework/artifact/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/artifact/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/artifact/test_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11995 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/artifact/test_hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/artifact/test_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.533930 vivarium-1.2.0/tests/framework/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/components/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/components/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/components/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.533930 vivarium-1.2.0/tests/framework/population/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/population/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/population/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26165 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/population/test_population_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.533930 vivarium-1.2.0/tests/framework/randomness/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/randomness/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/randomness/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9924 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/randomness/test_crn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/randomness/test_index_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/randomness/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5267 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/randomness/test_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.537930 vivarium-1.2.0/tests/framework/results/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/results/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14210 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/results/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/results/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6830 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/results/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4091 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/results/test_stratification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8985 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/test_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9776 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4691 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/test_state_machine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/test_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/framework/test_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.537930 vivarium-1.2.0/tests/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/interface/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:57:30.537930 vivarium-1.2.0/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/test_data/bad_model_specification.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/test_data/mock_model_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/test_data/mock_user_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-06-01 18:57:20.000000 vivarium-1.2.0/tests/test_interpolation.py
```

### Comparing `vivarium-1.1.0/CHANGELOG.rst` & `vivarium-1.2.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+**1.2.0 - 06/01/23**
+
+ - Stop supporting Python 3.7 and start supporting 3.11
+ - Bugfix to allow for zero stratifications
+ - Removes ignore filters for known FutureWarnings
+ - Refactor location of default stratification definition
+ - Bugfix to stop shuffling simulants when drawing common random number
+
 **1.1.0 - 05/03/23**
 
  - Clean up randomness system
  - Fix a bug in stratification when a stratum is empty
  - Create a dedicated logging system
  - Fix bug in preventing passing an Iterable to `rate_to_probability`
```

### Comparing `vivarium-1.1.0/CODE_OF_CONDUCT.rst` & `vivarium-1.2.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/CONTRIBUTING.rst` & `vivarium-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/LICENSE.txt` & `vivarium-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/PKG-INFO` & `vivarium-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium
-Version: 1.1.0
+Version: 1.2.0
 Summary: vivarium is a microsimulation framework built on top of the standard scientific python stack.
 Home-page: https://github.com/ihmeuw/vivarium
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -48,15 +48,15 @@
 
 .. image:: https://zenodo.org/badge/96817805.svg
    :target: https://zenodo.org/badge/latestdoi/96817805
 
 Vivarium is a simulation framework written using standard scientific Python
 tools.
 
-**Vivarium requires Python 3.7-3.10 to run**
+**Vivarium requires Python 3.8-3.11 to run**
 
 You can install ``vivarium`` from PyPI with pip:
 
   ``> pip install vivarium``
 
 or build it from source with
```

### Comparing `vivarium-1.1.0/README.rst` & `vivarium-1.2.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 .. image:: https://zenodo.org/badge/96817805.svg
    :target: https://zenodo.org/badge/latestdoi/96817805
 
 Vivarium is a simulation framework written using standard scientific Python
 tools.
 
-**Vivarium requires Python 3.7-3.10 to run**
+**Vivarium requires Python 3.8-3.11 to run**
 
 You can install ``vivarium`` from PyPI with pip:
 
   ``> pip install vivarium``
 
 or build it from source with
```

### Comparing `vivarium-1.1.0/docs/Makefile` & `vivarium-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/nitpick-exceptions` & `vivarium-1.2.0/docs/nitpick-exceptions`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/concepts/builder.rst` & `vivarium-1.2.0/docs/source/concepts/builder.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/concepts/crn.rst` & `vivarium-1.2.0/docs/source/concepts/crn.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/concepts/entry_points.rst` & `vivarium-1.2.0/docs/source/concepts/entry_points.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/concepts/event.rst` & `vivarium-1.2.0/docs/source/concepts/event.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/concepts/lifecycle.rst` & `vivarium-1.2.0/docs/source/concepts/lifecycle.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/concepts/lookup.rst` & `vivarium-1.2.0/docs/source/concepts/lookup.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/concepts/model_specification/index.rst` & `vivarium-1.2.0/docs/source/concepts/model_specification/index.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/concepts/model_specification/yaml_basics.rst` & `vivarium-1.2.0/docs/source/concepts/model_specification/yaml_basics.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/concepts/population.rst` & `vivarium-1.2.0/docs/source/concepts/population.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/concepts/values.rst` & `vivarium-1.2.0/docs/source/concepts/values.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/conf.py` & `vivarium-1.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/glossary.rst` & `vivarium-1.2.0/docs/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/images/crn_compare_cubes.jpg` & `vivarium-1.2.0/docs/source/images/crn_compare_cubes.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/images/crn_cube.jpg` & `vivarium-1.2.0/docs/source/images/crn_cube.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/images/crn_sim_alignment.jpg` & `vivarium-1.2.0/docs/source/images/crn_sim_alignment.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/images/pipeline.jpg` & `vivarium-1.2.0/docs/source/images/pipeline.jpg`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/installation.rst` & `vivarium-1.2.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/tutorials/artifact.rst` & `vivarium-1.2.0/docs/source/tutorials/artifact.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/tutorials/boids.rst` & `vivarium-1.2.0/docs/source/tutorials/boids.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/tutorials/disease_model.rst` & `vivarium-1.2.0/docs/source/tutorials/disease_model.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/tutorials/exploration.rst` & `vivarium-1.2.0/docs/source/tutorials/exploration.rst`

 * *Files 2% similar despite different names*

```diff
@@ -159,14 +159,17 @@
     interpolation:
         order:
             component_configs: 0
         validate:
             component_configs: True
         extrapolate:
             component_configs: True
+    stratification:
+        default:
+            component_configs: []
 
 
 What do we see here?  The configuration is *hierarchical*.  There are a set of
 top level *keys* that define named subsets of configuration data. We can access
 just those subsets if we like.
 
 .. testcode::
@@ -296,28 +299,28 @@
     50%           2.506636
     75%           3.744090
     max           4.999967
     Name: age, dtype: float64
     alive    100000
     Name: alive, dtype: int64
     count    100000.000000
-    mean          0.500602
-    std           0.288434
-    min           0.000022
-    25%           0.251288
-    50%           0.499957
-    75%           0.749816
+    mean          0.499756
+    std           0.288412
+    min           0.000015
+    25%           0.251550
+    50%           0.497587
+    75%           0.749215
     max           0.999978
     Name: child_wasting_propensity, dtype: float64
     susceptible_to_lower_respiratory_infections    100000
     Name: lower_respiratory_infections, dtype: int64
     2021-12-31 12:00:00    100000
     Name: entrance_time, dtype: int64
-    Male      50162
-    Female    49838
+    Male      50185
+    Female    49815
     Name: sex, dtype: int64
     True    100000
     Name: tracked, dtype: int64
 
 
 
 Understanding the Simulation Data
```

### Comparing `vivarium-1.1.0/docs/source/tutorials/getting_started.rst` & `vivarium-1.2.0/docs/source/tutorials/getting_started.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/tutorials/running_a_simulation/cli.rst` & `vivarium-1.2.0/docs/source/tutorials/running_a_simulation/cli.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/docs/source/tutorials/running_a_simulation/interactive.rst` & `vivarium-1.2.0/docs/source/tutorials/running_a_simulation/interactive.rst`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/setup.py` & `vivarium-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import sys
 
-min_version, max_version = ((3, 6), "3.6"), ((3, 10), "3.10")
+min_version, max_version = ((3, 8), "3.8"), ((3, 11), "3.11")
 
 if not (min_version[0] <= sys.version_info[:2] <= max_version[0]):
     # Python 3.5 does not support f-strings
     py_version = ".".join([str(v) for v in sys.version_info[:3]])
     error = (
         "\n----------------------------------------\n"
         "Error: Vivarium runs under python {min_version}-{max_version}.\n"
```

### Comparing `vivarium-1.1.0/src/vivarium/__about__.py` & `vivarium-1.2.0/src/vivarium/__about__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,14 @@
     "__copyright__",
 ]
 
 __title__ = "vivarium"
 __summary__ = "vivarium is a microsimulation framework built on top of the standard scientific python stack."
 __uri__ = "https://github.com/ihmeuw/vivarium"
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 
 __author__ = "The vivarium developers"
 __email__ = "vivarium.dev@gmail.com"
 
 __license__ = "BSD-3-Clause"
 __copyright__ = f"Copyright 2016-2023 {__author__}"
```

### Comparing `vivarium-1.1.0/src/vivarium/config_tree.py` & `vivarium-1.2.0/src/vivarium/config_tree.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/boids/location.py` & `vivarium-1.2.0/src/vivarium/examples/boids/location.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/boids/neighbors.py` & `vivarium-1.2.0/src/vivarium/examples/boids/neighbors.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/boids/population.py` & `vivarium-1.2.0/src/vivarium/examples/boids/population.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/disease_model/__init__.py` & `vivarium-1.2.0/src/vivarium/examples/disease_model/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/disease_model/disease.py` & `vivarium-1.2.0/src/vivarium/examples/disease_model/disease.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/disease_model/disease_model.yaml` & `vivarium-1.2.0/src/vivarium/examples/disease_model/disease_model.yaml`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/disease_model/intervention.py` & `vivarium-1.2.0/src/vivarium/examples/disease_model/intervention.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/disease_model/mortality.py` & `vivarium-1.2.0/src/vivarium/examples/disease_model/mortality.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/disease_model/observer.py` & `vivarium-1.2.0/src/vivarium/examples/disease_model/observer.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/disease_model/population.py` & `vivarium-1.2.0/src/vivarium/examples/disease_model/population.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/examples/disease_model/risk.py` & `vivarium-1.2.0/src/vivarium/examples/disease_model/risk.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/artifact/artifact.py` & `vivarium-1.2.0/src/vivarium/framework/artifact/artifact.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/artifact/hdf.py` & `vivarium-1.2.0/src/vivarium/framework/artifact/hdf.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/artifact/manager.py` & `vivarium-1.2.0/src/vivarium/framework/artifact/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/components/manager.py` & `vivarium-1.2.0/src/vivarium/framework/components/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/components/parser.py` & `vivarium-1.2.0/src/vivarium/framework/components/parser.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/configuration.py` & `vivarium-1.2.0/src/vivarium/framework/configuration.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/engine.py` & `vivarium-1.2.0/src/vivarium/framework/engine.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/event.py` & `vivarium-1.2.0/src/vivarium/framework/event.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/lifecycle.py` & `vivarium-1.2.0/src/vivarium/framework/lifecycle.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/logging/manager.py` & `vivarium-1.2.0/src/vivarium/framework/logging/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/logging/utilities.py` & `vivarium-1.2.0/src/vivarium/framework/logging/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/lookup.py` & `vivarium-1.2.0/src/vivarium/framework/lookup.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/metrics.py` & `vivarium-1.2.0/src/vivarium/framework/metrics.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/plugins.py` & `vivarium-1.2.0/src/vivarium/framework/plugins.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/population/__init__.py` & `vivarium-1.2.0/src/vivarium/framework/population/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/population/manager.py` & `vivarium-1.2.0/src/vivarium/framework/population/manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/population/population_view.py` & `vivarium-1.2.0/src/vivarium/framework/population/population_view.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/randomness/__init__.py` & `vivarium-1.2.0/src/vivarium/framework/randomness/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/randomness/index_map.py` & `vivarium-1.2.0/src/vivarium/framework/randomness/index_map.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,37 +26,43 @@
 
     def __init__(self, key_columns: List[str] = None, size: int = 1_000_000):
         self._use_crn = bool(key_columns)
         self._key_columns = key_columns
         self._map = None
         self._size = size
 
-    def update(self, new_keys: pd.DataFrame) -> None:
+    def update(self, new_keys: pd.DataFrame, clock_time: pd.Timestamp) -> None:
         """Adds the new keys to the mapping.
 
         Parameters
         ----------
         new_keys
             A pandas DataFrame indexed by the simulant index and columns corresponding to
             the randomness system key columns.
+        clock_time
+            The simulation clock time. Used as the salt during hashing to
+            minimize inter-simulation collisions.
 
         """
         if new_keys.empty or not self._use_crn:
             return  # Nothing to do
 
         new_mapping_index, final_mapping_index = self._parse_new_keys(new_keys)
 
         final_keys = final_mapping_index.droplevel(self.SIM_INDEX_COLUMN)
         if len(final_keys) != len(final_keys.unique()):
             raise RandomnessError("Non-unique keys in index")
 
-        final_mapping = self._build_final_mapping(new_mapping_index)
+        final_mapping = self._build_final_mapping(new_mapping_index, clock_time)
 
         # Tack on the simulant index to the front of the map.
-        final_mapping.index = final_mapping_index
+        final_mapping.index = final_mapping.index.join(final_mapping_index).reorder_levels(
+            [self.SIM_INDEX_COLUMN] + self._key_columns
+        )
+        final_mapping = final_mapping.sort_index(level=self.SIM_INDEX_COLUMN)
         self._map = final_mapping
 
     def _parse_new_keys(self, new_keys: pd.DataFrame) -> Tuple[pd.MultiIndex, pd.MultiIndex]:
         """Parses raw new keys into the mapping index.
 
         Parameters
         ----------
@@ -80,33 +86,38 @@
 
         if self._map is None:
             final_mapping_index = new_mapping_index
         else:
             final_mapping_index = self._map.index.append(new_mapping_index)
         return new_mapping_index, final_mapping_index
 
-    def _build_final_mapping(self, new_mapping_index: pd.Index) -> pd.Series:
+    def _build_final_mapping(
+        self, new_mapping_index: pd.Index, clock_time: pd.Timestamp
+    ) -> pd.Series:
         """Builds a new mapping between key columns and the randomness index from the
         new mapping index and the existing map.
 
         Parameters
         ----------
         new_mapping_index
             An index with a level for the index assigned by the population system and
             additional levels for the key columns associated with the simulant index.
+        clock_time
+            The simulation clock time. Used as the salt during hashing to
+            minimize inter-simulation collisions.
 
         Returns
         -------
         pd.Series
             The new mapping incorporating the updates from the new mapping index and
             resolving collisions.
 
         """
         new_key_index = new_mapping_index.droplevel(self.SIM_INDEX_COLUMN)
-        mapping_update = self._hash(new_key_index)
+        mapping_update = self._hash(new_key_index, salt=clock_time)
         if self._map is None:
             current_map = mapping_update
         else:
             old_map = self._map.droplevel(self.SIM_INDEX_COLUMN)
             current_map = pd.concat([old_map, mapping_update])
 
         return self._resolve_collisions(new_key_index, current_map)
```

### Comparing `vivarium-1.1.0/src/vivarium/framework/randomness/manager.py` & `vivarium-1.2.0/src/vivarium/framework/randomness/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
             in the configuration.
 
         """
         if not all(k in simulants.columns for k in self._key_columns):
             raise RandomnessError(
                 "The simulants dataframe does not have all specified key_columns."
             )
-        self._key_mapping.update(simulants.loc[:, self._key_columns])
+        self._key_mapping.update(simulants.loc[:, self._key_columns], self._clock())
 
     def __str__(self):
         return "RandomnessManager()"
 
     def __repr__(self) -> str:
         return f"RandomnessManager(seed={self._seed}, key_columns={self._key_columns})"
```

### Comparing `vivarium-1.1.0/src/vivarium/framework/randomness/stream.py` & `vivarium-1.2.0/src/vivarium/framework/randomness/stream.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/resource.py` & `vivarium-1.2.0/src/vivarium/framework/resource.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/results/context.py` & `vivarium-1.2.0/src/vivarium/framework/results/context.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,19 +41,14 @@
     # noinspection PyAttributeOutsideInit
     def set_default_stratifications(self, default_grouping_columns: List[str]):
         if self.default_stratifications:
             raise ResultsConfigurationError(
                 "Multiple calls are being made to set default grouping columns "
                 "for results production."
             )
-        if not default_grouping_columns:
-            raise ResultsConfigurationError(
-                "Attempting to set an empty list as the default grouping columns "
-                "for results production."
-            )
         self.default_stratifications = default_grouping_columns
 
     def add_stratification(
         self,
         name: str,
         sources: List[str],
         categories: List[str],
@@ -121,15 +116,19 @@
             if pop_filter:
                 filtered_pop = population.query(pop_filter)
             else:
                 filtered_pop = population
             if filtered_pop.empty:
                 yield {}
             else:
-                pop_groups = filtered_pop.groupby(list(stratifications))
+                if not len(list(stratifications)):  # Handle situation of no stratifications
+                    pop_groups = filtered_pop.groupby(lambda _: True)
+                else:
+                    pop_groups = filtered_pop.groupby(list(stratifications))
+
                 for measure, aggregator_sources, aggregator, additional_keys in observations:
                     if aggregator_sources:
                         aggregates = (
                             pop_groups[aggregator_sources].apply(aggregator).fillna(0.0)
                         )
                     else:
                         aggregates = pop_groups.apply(aggregator)
@@ -140,15 +139,20 @@
                     if not isinstance(aggregates, pd.Series):
                         raise TypeError(
                             f"The aggregator return value is a {type(aggregates)} and could not be "
                             "made into a pandas.Series. This is probably not correct."
                         )
 
                     # Keep formatting all in one place.
-                    yield self._format_results(measure, aggregates, **additional_keys)
+                    yield self._format_results(
+                        measure,
+                        aggregates,
+                        bool(len(list(stratifications))),
+                        **additional_keys,
+                    )
 
     def _get_stratifications(
         self,
         additional_stratifications: List[str] = (),
         excluded_stratifications: List[str] = (),
     ) -> Tuple[str, ...]:
         stratifications = list(
@@ -158,17 +162,22 @@
         # Makes sure measure identifiers have fields in the same relative order.
         return tuple(sorted(stratifications))
 
     @staticmethod
     def _format_results(
         measure: str,
         aggregates: pd.Series,
+        has_stratifications: bool,
         **additional_keys: str,
     ) -> Dict[str, float]:
         results = {}
+        # Simpler formatting if we don't have stratifications
+        if not has_stratifications:
+            return {measure: aggregates.squeeze()}
+
         # First we expand the categorical index over unobserved pairs.
         # This ensures that the produced results are always the same length.
         if isinstance(aggregates.index, pd.MultiIndex):
             idx = pd.MultiIndex.from_product(
                 aggregates.index.levels, names=aggregates.index.names
             )
         else:
```

### Comparing `vivarium-1.1.0/src/vivarium/framework/results/interface.py` & `vivarium-1.2.0/src/vivarium/framework/results/interface.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/results/manager.py` & `vivarium-1.2.0/src/vivarium/framework/results/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,20 @@
     :class:`ResultsInterface` to register stratifications and observations,
     which provide it with lists of methods to apply in their respective areas.
     It is able to record observations at any of the time-step sub-steps
     (`time_step__prepare`, `time_step`, `time_step__cleanup`, and
     `collect_metrics`).
     """
 
+    configuration_defaults = {
+        "stratification": {
+            "default": [],
+        }
+    }
+
     def __init__(self):
         self._metrics = Counter()
         self._results_context = ResultsContext()
         self._required_columns = {"tracked"}
         self._required_values = set()
         self._name = "results_manager"
 
@@ -55,14 +61,16 @@
         builder.event.register_listener("time_step__prepare", self.on_time_step_prepare)
         builder.event.register_listener("time_step", self.on_time_step)
         builder.event.register_listener("time_step__cleanup", self.on_time_step_cleanup)
         builder.event.register_listener("collect_metrics", self.on_collect_metrics)
 
         self.get_value = builder.value.get_value
 
+        self.set_default_stratifications(builder)
+
         builder.value.register_value_modifier("metrics", self.get_results)
 
     def on_time_step_prepare(self, event: Event):
         self.gather_results("time_step__prepare", event)
 
     def on_time_step(self, event: Event):
         self.gather_results("time_step", event)
@@ -74,15 +82,16 @@
         self.gather_results("collect_metrics", event)
 
     def gather_results(self, event_name: str, event: Event):
         population = self._prepare_population(event)
         for results_group in self._results_context.gather_results(population, event_name):
             self._metrics.update(results_group)
 
-    def set_default_stratifications(self, default_stratifications: List[str]):
+    def set_default_stratifications(self, builder):
+        default_stratifications = builder.configuration.stratification.default
         self._results_context.set_default_stratifications(default_stratifications)
 
     def register_stratification(
         self,
         name: str,
         categories: List[str],
         mapper: Callable,
```

### Comparing `vivarium-1.1.0/src/vivarium/framework/results/stratification.py` & `vivarium-1.2.0/src/vivarium/framework/results/stratification.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/state_machine.py` & `vivarium-1.2.0/src/vivarium/framework/state_machine.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,18 +80,15 @@
     List[Tuple[str, pandas.Index]
         The first item in each tuple is the name of an output state and the
         second item is a `pandas.Index` representing the simulants to transition
         into that state.
 
     """
     output_map = {o: i for i, o in enumerate(outputs)}
-    # TODO: fix rather than suppress this FutureWarning
-    with warnings.catch_warnings():
-        warnings.simplefilter(action="ignore", category=FutureWarning)
-        groups = pd.Series(index).groupby([output_map[d] for d in decisions])
+    groups = pd.Series(index).groupby([output_map[d] for d in decisions])
     results = [(outputs[i], pd.Index(sub_group.values)) for i, sub_group in groups]
     selected_outputs = [o for o, _ in results]
     for output in outputs:
         if output not in selected_outputs:
             results.append((output, pd.Index([])))
     return results
 
@@ -208,14 +205,18 @@
     @property
     def sub_components(self) -> List:
         return self._sub_components
 
     def setup(self, builder: "Builder") -> None:
         pass
 
+    def set_model(self, model_name: str) -> None:
+        """Defines the column name for the model this state belongs to"""
+        self._model = model_name
+
     def next_state(
         self, index: pd.Index, event_time: "Time", population_view: "PopulationView"
     ) -> None:
         """Moves a population between different states.
 
         Parameters
         ----------
@@ -484,15 +485,15 @@
 
     def setup(self, builder: "Builder") -> None:
         self.population_view = builder.population.get_view([self.state_column])
 
     def add_states(self, states: Iterable[State]) -> None:
         for state in states:
             self.states.append(state)
-            state._model = self.state_column
+            state.set_model(self.state_column)
 
     def transition(self, index: pd.Index, event_time: "Time") -> None:
         """Finds the population in each state and moves them to the next state.
 
         Parameters
         ----------
         index
```

### Comparing `vivarium-1.1.0/src/vivarium/framework/time.py` & `vivarium-1.2.0/src/vivarium/framework/time.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/utilities.py` & `vivarium-1.2.0/src/vivarium/framework/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/framework/values.py` & `vivarium-1.2.0/src/vivarium/framework/values.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/interface/cli.py` & `vivarium-1.2.0/src/vivarium/interface/cli.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/interface/interactive.py` & `vivarium-1.2.0/src/vivarium/interface/interactive.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/interface/utilities.py` & `vivarium-1.2.0/src/vivarium/interface/utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium/interpolation.py` & `vivarium-1.2.0/src/vivarium/interpolation.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,28 +64,22 @@
         self.order = order
         self.extrapolate = extrapolate
         self.validate = validate
 
         if self.key_columns:
             # Since there are key_columns we need to group the table by those
             # columns to get the sub-tables to fit
-            # TODO: fix rather than suppress this FutureWarning
-            with warnings.catch_warnings():
-                warnings.simplefilter(action="ignore", category=FutureWarning)
-                sub_tables = self.data.groupby(list(self.key_columns))
+            sub_tables = self.data.groupby(list(self.key_columns))
         else:
             # There are no key columns so we will fit the whole table
             sub_tables = {None: self.data}.items()
 
         self.interpolations = {}
 
-        # TODO: fix rather than suppress this FutureWarning
-        with warnings.catch_warnings():
-            warnings.simplefilter(action="ignore", category=FutureWarning)
-            sub_tables = list(sub_tables)
+        sub_tables = list(sub_tables)
         for key, base_table in sub_tables:
             if (
                 base_table.empty
             ):  # if one of the key columns is a category and not all values are present in data
                 continue
             # since order 0, we can interpolate all values at once
             self.interpolations[key] = Order0Interp(
@@ -110,29 +104,23 @@
             A table with the interpolated values for the given interpolants.
         """
 
         if self.validate:
             validate_call_data(interpolants, self.key_columns, self.parameter_columns)
 
         if self.key_columns:
-            # TODO: fix rather than suppress this FutureWarning
-            with warnings.catch_warnings():
-                warnings.simplefilter(action="ignore", category=FutureWarning)
-                sub_tables = interpolants.groupby(list(self.key_columns))
+            sub_tables = interpolants.groupby(list(self.key_columns))
         else:
             sub_tables = [(None, interpolants)]
         # specify some numeric type for columns so they won't be objects but will updated with whatever
         # column type actually is
         result = pd.DataFrame(
             index=interpolants.index, columns=self.value_columns, dtype=np.float64
         )
-        # TODO: fix rather than suppress this FutureWarning
-        with warnings.catch_warnings():
-            warnings.simplefilter(action="ignore", category=FutureWarning)
-            sub_tables = list(sub_tables)
+        sub_tables = list(sub_tables)
         for key, sub_table in sub_tables:
             if sub_table.empty:
                 continue
             df = self.interpolations[key](sub_table)
             result.loc[sub_table.index, self.value_columns] = df.loc[
                 sub_table.index, self.value_columns
             ]
@@ -222,27 +210,21 @@
         p[1:] for p in parameter_columns if isinstance(p, (Tuple, List))
     ]  # strip out call column name
 
     # check no overlaps/gaps
     for p in param_edges:
         other_params = [p_ed[0] for p_ed in param_edges if p_ed != p]
         if other_params:
-            # TODO: fix rather than suppress this FutureWarning
-            with warnings.catch_warnings():
-                warnings.simplefilter(action="ignore", category=FutureWarning)
-                sub_tables = data.groupby(list(other_params))
+            sub_tables = data.groupby(list(other_params))
         else:
             sub_tables = {None: data}.items()
 
         n_p_total = len(set(data[p[0]]))
 
-        # TODO: fix rather than suppress this FutureWarning
-        with warnings.catch_warnings():
-            warnings.simplefilter(action="ignore", category=FutureWarning)
-            sub_tables = list(sub_tables)
+        sub_tables = list(sub_tables)
         for _, table in sub_tables:
             param_data = table[[p[0], p[1]]].copy().sort_values(by=p[0])
             start, end = param_data[p[0]].reset_index(drop=True), param_data[
                 p[1]
             ].reset_index(drop=True)
 
             if len(set(start)) < n_p_total:
```

### Comparing `vivarium-1.1.0/src/vivarium/testing_utilities.py` & `vivarium-1.2.0/src/vivarium/testing_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/src/vivarium.egg-info/PKG-INFO` & `vivarium-1.2.0/src/vivarium.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium
-Version: 1.1.0
+Version: 1.2.0
 Summary: vivarium is a microsimulation framework built on top of the standard scientific python stack.
 Home-page: https://github.com/ihmeuw/vivarium
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
@@ -48,15 +48,15 @@
 
 .. image:: https://zenodo.org/badge/96817805.svg
    :target: https://zenodo.org/badge/latestdoi/96817805
 
 Vivarium is a simulation framework written using standard scientific Python
 tools.
 
-**Vivarium requires Python 3.7-3.10 to run**
+**Vivarium requires Python 3.8-3.11 to run**
 
 You can install ``vivarium`` from PyPI with pip:
 
   ``> pip install vivarium``
 
 or build it from source with
```

### Comparing `vivarium-1.1.0/src/vivarium.egg-info/SOURCES.txt` & `vivarium-1.2.0/src/vivarium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/config_tree/test_basic_functionality.py` & `vivarium-1.2.0/tests/config_tree/test_basic_functionality.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/config_tree/test_ingestion.py` & `vivarium-1.2.0/tests/config_tree/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/conftest.py` & `vivarium-1.2.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/artifact/test_artifact.py` & `vivarium-1.2.0/tests/framework/artifact/test_artifact.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/artifact/test_hdf.py` & `vivarium-1.2.0/tests/framework/artifact/test_hdf.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/artifact/test_manager.py` & `vivarium-1.2.0/tests/framework/artifact/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/components/mocks.py` & `vivarium-1.2.0/tests/framework/components/mocks.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/components/test_manager.py` & `vivarium-1.2.0/tests/framework/components/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/components/test_parser.py` & `vivarium-1.2.0/tests/framework/components/test_parser.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/population/test_manager.py` & `vivarium-1.2.0/tests/framework/population/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/population/test_population_view.py` & `vivarium-1.2.0/tests/framework/population/test_population_view.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/randomness/conftest.py` & `vivarium-1.2.0/tests/framework/randomness/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/randomness/test_crn.py` & `vivarium-1.2.0/tests/framework/randomness/test_crn.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/randomness/test_index_map.py` & `vivarium-1.2.0/tests/framework/randomness/test_index_map.py`

 * *Files 11% similar despite different names*

```diff
@@ -165,58 +165,59 @@
     assert p > 0.05, "Data not uniform"
 
 
 @pytest.fixture(scope="function")
 def index_map(mocker):
     mock_index_map = IndexMap
 
-    def hash_mock(k, salt=0):
+    def hash_mock(k, salt):
         seed = 123456
+        salt = IndexMap()._convert_to_ten_digit_int(pd.Series(salt, index=k))
         rs = np.random.RandomState(seed=seed + salt)
         return pd.Series(rs.randint(0, len(k) * 10, size=len(k)), index=k)
 
     mocker.patch.object(mock_index_map, "_hash", side_effect=hash_mock)
 
     return mock_index_map
 
 
 def test_update_empty_bad_keys(index_map):
     keys = pd.DataFrame({"A": ["a"] * 10}, index=range(10))
     m = index_map(key_columns=list(keys.columns))
     with pytest.raises(RandomnessError):
-        m.update(keys)
+        m.update(keys, pd.to_datetime("2023-01-01"))
 
 
 def test_update_nonempty_bad_keys(index_map):
     keys = generate_keys(1000)
     m = index_map(key_columns=list(keys.columns))
-    m.update(keys)
+    m.update(keys, pd.to_datetime("2023-01-01"))
     with pytest.raises(RandomnessError):
-        m.update(keys)
+        m.update(keys, pd.to_datetime("2023-01-01"))
 
 
 def test_update_empty_good_keys(index_map):
     keys = generate_keys(1000)
     m = index_map(key_columns=list(keys.columns))
-    m.update(keys)
+    m.update(keys, pd.to_datetime("2023-01-01"))
     key_index = keys.set_index(list(keys.columns)).index
     assert len(m._map) == len(keys), "All keys not in mapping"
     assert (
         m._map.index.droplevel(m.SIM_INDEX_COLUMN).difference(key_index).empty
     ), "Extra keys in mapping"
     assert len(m._map.unique()) == len(keys), "Duplicate values in mapping"
 
 
 def test_update_nonempty_good_keys(index_map):
     keys = generate_keys(2000)
     m = index_map(key_columns=list(keys.columns))
     keys1, keys2 = keys[:1000], keys[1000:]
 
-    m.update(keys1)
-    m.update(keys2)
+    m.update(keys1, pd.to_datetime("2023-01-01"))
+    m.update(keys2, pd.to_datetime("2023-01-01"))
 
     key_index = keys.set_index(list(keys.columns)).index
     assert len(m._map) == len(keys), "All keys not in mapping"
     assert (
         m._map.index.droplevel(m.SIM_INDEX_COLUMN).difference(key_index).empty
     ), "Extra keys in mapping"
     assert len(m._map.unique()) == len(keys), "Duplicate values in mapping"
```

### Comparing `vivarium-1.1.0/tests/framework/randomness/test_manager.py` & `vivarium-1.2.0/tests/framework/randomness/test_manager.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/randomness/test_stream.py` & `vivarium-1.2.0/tests/framework/randomness/test_stream.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/results/mocks.py` & `vivarium-1.2.0/tests/framework/results/mocks.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/results/test_context.py` & `vivarium-1.2.0/tests/framework/results/test_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -362,20 +362,40 @@
         event_name=event_name,
     )
 
     for result in ctx.gather_results(population, event_name):
         assert len(result) == 0
 
 
+def test_gather_results_with_no_stratifications():
+    """Test case where we have no stratifications. gather_results should return one value."""
+    ctx = ResultsContext()
+
+    # Generate population DataFrame
+    population = BASE_POPULATION.copy()
+
+    event_name = "collect_metrics"
+    ctx.add_observation(
+        name="wizard_count",
+        pop_filter="",
+        aggregator_sources=None,
+        aggregator=len,
+        event_name=event_name,
+    )
+
+    assert len(ctx.stratifications) == 0
+    assert len(list(ctx.gather_results(population, event_name))) == 1
+
+
 def test__format_results():
     """Test that format results produces the expected number of keys and a specific expected key"""
     ctx = ResultsContext()
     aggregates = BASE_POPULATION.groupby(["house", "familiar"]).apply(len)
     measure = "wizard_count"
-    rv = ctx._format_results(measure, aggregates)
+    rv = ctx._format_results(measure, aggregates, has_stratifications=True)
 
     # Check that the number of expected data column names are there
     expected_keys_len = len(CATEGORIES) * len(FAMILIARS)
     assert len(rv.keys()) == expected_keys_len
 
     # Check that an example data column name is there
     expected_key = "MEASURE_wizard_count_HOUSE_slytherin_FAMILIAR_cat"
```

### Comparing `vivarium-1.1.0/tests/framework/results/test_interface.py` & `vivarium-1.2.0/tests/framework/results/test_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     additional_stratifications,
     excluded_stratifications,
     when,
 ):
     mgr = ResultsManager()
     interface = ResultsInterface(mgr)
     builder = mocker.Mock()
+    builder.configuration.stratification.default = []
     # Set up mock builder with mocked get_value call for Pipelines
     mocker.patch.object(builder, "value.get_value")
     builder.value.get_value = MethodType(mock_get_value, builder)
     mgr.setup(builder)
     assert len(interface._manager._results_context.observations) == 0
     interface.register_observation(
         name,
```

### Comparing `vivarium-1.1.0/tests/framework/results/test_manager.py` & `vivarium-1.2.0/tests/framework/results/test_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -220,7 +220,21 @@
         lambda: None,
         additional_stratifications=additional,
         excluded_stratifications=excluded,
         when="collect_metrics",
     )
     for m in match:
         assert m in caplog.text
+
+
+def test_setting_default_stratifications_at_setup(mocker):
+    """Test that set default stratifications happens at setup"""
+    mgr = ResultsManager()
+    builder = mocker.Mock()
+    mgr._results_context.set_default_stratifications = mocker.Mock()
+    mgr._results_context.set_default_stratifications.assert_not_called()
+
+    mgr.setup(builder)
+
+    mgr._results_context.set_default_stratifications.assert_called_once_with(
+        builder.configuration.stratification.default
+    )
```

### Comparing `vivarium-1.1.0/tests/framework/results/test_stratification.py` & `vivarium-1.2.0/tests/framework/results/test_stratification.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pandas as pd
 import pytest
 
+from vivarium.framework.results.manager import ResultsManager
 from vivarium.framework.results.stratification import Stratification
 
 from .mocks import (
     CATEGORIES,
     NAME,
     SOURCES,
     STUDENT_HOUSES,
@@ -136,7 +137,19 @@
 )
 def test_stratification_call_raises(
     name, sources, categories, mapper, is_vectorized, expected_exception
 ):
     my_stratification = Stratification(name, sources, categories, mapper, is_vectorized)
     with pytest.raises(expected_exception):
         raise my_stratification(STUDENT_TABLE)
+
+
+@pytest.mark.parametrize("default_stratifications", [["age", "sex"], ["age"], []])
+def test_setting_default_stratifications(default_stratifications, mocker):
+    """Test that default stratifications are set as expected."""
+    mgr = ResultsManager()
+    builder = mocker.Mock()
+    builder.configuration.stratification.default = default_stratifications
+
+    mgr.setup(builder)
+
+    assert mgr._results_context.default_stratifications == default_stratifications
```

### Comparing `vivarium-1.1.0/tests/framework/test_configuration.py` & `vivarium-1.2.0/tests/framework/test_configuration.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/test_engine.py` & `vivarium-1.2.0/tests/framework/test_engine.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/test_event.py` & `vivarium-1.2.0/tests/framework/test_event.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/test_lifecycle.py` & `vivarium-1.2.0/tests/framework/test_lifecycle.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/test_lookup.py` & `vivarium-1.2.0/tests/framework/test_lookup.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/test_plugins.py` & `vivarium-1.2.0/tests/framework/test_plugins.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/test_resource.py` & `vivarium-1.2.0/tests/framework/test_resource.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/test_state_machine.py` & `vivarium-1.2.0/tests/framework/test_state_machine.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/test_utilities.py` & `vivarium-1.2.0/tests/framework/test_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/framework/test_values.py` & `vivarium-1.2.0/tests/framework/test_values.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/interface/test_utilities.py` & `vivarium-1.2.0/tests/interface/test_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium-1.1.0/tests/test_interpolation.py` & `vivarium-1.2.0/tests/test_interpolation.py`

 * *Files identical despite different names*

