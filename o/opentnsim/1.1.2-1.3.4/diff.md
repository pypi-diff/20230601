# Comparing `tmp/opentnsim-1.1.2.tar.gz` & `tmp/opentnsim-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentnsim-1.1.2.tar", last modified: Sat May 27 12:33:59 2023, max compression
+gzip compressed data, was "opentnsim-1.3.4.tar", last modified: Thu Jun  1 07:49:15 2023, max compression
```

## Comparing `opentnsim-1.1.2.tar` & `opentnsim-1.3.4.tar`

### file list

```diff
@@ -1,98 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.273583 opentnsim-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-27 12:33:41.000000 opentnsim-1.1.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-27 12:33:41.000000 opentnsim-1.1.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-27 12:33:41.000000 opentnsim-1.1.2/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-27 12:33:41.000000 opentnsim-1.1.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-27 12:33:41.000000 opentnsim-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-27 12:33:59.273583 opentnsim-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-27 12:33:41.000000 opentnsim-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.261583 opentnsim-1.1.2/data/
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-27 12:33:41.000000 opentnsim-1.1.2/data/Correctionfactors.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-05-27 12:33:41.000000 opentnsim-1.1.2/data/KarpovSmoothCurves.csv
--rw-r--r--   0 runner    (1001) docker     (123)   212529 2023-05-27 12:33:41.000000 opentnsim-1.1.2/data/ais.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.261583 opentnsim-1.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/OpenTNSim.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.261583 opentnsim-1.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   785084 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/_static/book.png
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/opentnsim.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-27 12:33:41.000000 opentnsim-1.1.2/docs/version-conventions.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.265583 opentnsim-1.1.2/opentnsim/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20866 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    80195 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/energy.py
--rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/graph_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    69590 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-05-27 12:33:42.000000 opentnsim-1.1.2/opentnsim/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.265583 opentnsim-1.1.2/opentnsim.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-27 12:33:59.000000 opentnsim-1.1.2/opentnsim.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-27 12:33:42.000000 opentnsim-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-27 12:33:59.273583 opentnsim-1.1.2/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2642 2023-05-27 12:33:42.000000 opentnsim-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.269583 opentnsim-1.1.2/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.269583 opentnsim-1.1.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  2888448 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/data/ect-bctn.json
--rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips.py
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_limiting_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_limiting_depth_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_uniform_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_uniform_depth_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_varying_depth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_varying_depth_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_resistance_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_resistance_components_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_squat.py
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_squat_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_total_power.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_total_power_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_Van_Dorsser_et_al_2020_draught_payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_Van_Dorsser_et_al_2020_draught_payload_expected.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_basic_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_single_vessel_with_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_single_vessel_without_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_without_pre-conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 12:33:59.273583 opentnsim-1.1.2/tests/vessels/
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-27 12:33:42.000000 opentnsim-1.1.2/tests/vessels/vessels.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.607651 opentnsim-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-01 07:49:02.000000 opentnsim-1.3.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-01 07:49:02.000000 opentnsim-1.3.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-06-01 07:49:02.000000 opentnsim-1.3.4/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-01 07:49:02.000000 opentnsim-1.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-01 07:49:02.000000 opentnsim-1.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-01 07:49:15.607651 opentnsim-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-06-01 07:49:02.000000 opentnsim-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.591651 opentnsim-1.3.4/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-06-01 07:49:02.000000 opentnsim-1.3.4/data/Correctionfactors.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-01 07:49:02.000000 opentnsim-1.3.4/data/KarpovSmoothCurves.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   212529 2023-06-01 07:49:02.000000 opentnsim-1.3.4/data/ais.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.595651 opentnsim-1.3.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     7598 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     6810 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/OpenTNSim.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.595651 opentnsim-1.3.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   785084 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/_static/book.png
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4894 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/opentnsim.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-01 07:49:02.000000 opentnsim-1.3.4/docs/version-conventions.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.595651 opentnsim-1.3.4/opentnsim/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20866 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80195 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/energy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/fis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9524 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/graph_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69590 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6434 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13353 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14357 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-06-01 07:49:03.000000 opentnsim-1.3.4/opentnsim/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.595651 opentnsim-1.3.4/opentnsim.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 07:49:15.000000 opentnsim-1.3.4/opentnsim.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-01 07:49:03.000000 opentnsim-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-06-01 07:49:15.607651 opentnsim-1.3.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2716 2023-06-01 07:49:03.000000 opentnsim-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.603651 opentnsim-1.3.4/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.603651 opentnsim-1.3.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  2888448 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/data/ect-bctn.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7603 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7661 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7498 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3672 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7862 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7740 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_limiting_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_limiting_depth_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6801 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_uniform_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_uniform_depth_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     6866 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_varying_depth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_varying_depth_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_resistance_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_resistance_components_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_squat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_squat_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3944 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_total_power.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_total_power_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7166 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3146 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_Van_Dorsser_et_al_2020_draught_payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_Van_Dorsser_et_al_2020_draught_payload_expected.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4229 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_basic_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_fis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8211 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_single_vessel_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6652 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_single_vessel_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10023 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9022 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9678 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_without_pre-conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 07:49:15.607651 opentnsim-1.3.4/tests/vessels/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-01 07:49:03.000000 opentnsim-1.3.4/tests/vessels/vessels.csv
```

### Comparing `opentnsim-1.1.2/AUTHORS.rst` & `opentnsim-1.3.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/CONTRIBUTING.rst` & `opentnsim-1.3.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/HISTORY.rst` & `opentnsim-1.3.4/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/LICENSE.txt` & `opentnsim-1.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/PKG-INFO` & `opentnsim-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentnsim
-Version: 1.1.2
+Version: 1.3.4
 Summary: The OpenTNSim package aims to facilitate the analysis of network performance for different network configurations, fleet compositions and traffic rules.
 Home-page: https://github.com/TUDelft-CITG/OpenTNSim
 Author: Mark van Koningsveld
 Author-email: m.vankoningsveld@tudelft.nl
 License: mit
 Keywords: OpenTNSim
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opentnsim Version: 1.1.2 Summary: The OpenTNSim
+Metadata-Version: 2.1 Name: opentnsim Version: 1.3.4 Summary: The OpenTNSim
 package aims to facilitate the analysis of network performance for different
 network configurations, fleet compositions and traffic rules. Home-page: https:
 //github.com/TUDelft-CITG/OpenTNSim Author: Mark van Koningsveld Author-email:
 m.vankoningsveld@tudelft.nl License: mit Keywords: OpenTNSim Platform: any
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `opentnsim-1.1.2/README.md` & `opentnsim-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/data/Correctionfactors.csv` & `opentnsim-1.3.4/data/Correctionfactors.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/data/KarpovSmoothCurves.csv` & `opentnsim-1.3.4/data/KarpovSmoothCurves.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/data/ais.csv` & `opentnsim-1.3.4/data/ais.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/docs/Makefile` & `opentnsim-1.3.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/docs/OpenTNSim.png` & `opentnsim-1.3.4/docs/OpenTNSim.png`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/docs/_static/book.png` & `opentnsim-1.3.4/docs/_static/book.png`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/docs/conf.py` & `opentnsim-1.3.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/docs/index.rst` & `opentnsim-1.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/docs/installation.rst` & `opentnsim-1.3.4/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/docs/opentnsim.rst` & `opentnsim-1.3.4/docs/opentnsim.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/docs/version-conventions.rst` & `opentnsim-1.3.4/docs/version-conventions.rst`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/opentnsim/cli.py` & `opentnsim-1.3.4/opentnsim/cli.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/opentnsim/core.py` & `opentnsim-1.3.4/opentnsim/core.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/opentnsim/energy.py` & `opentnsim-1.3.4/opentnsim/energy.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/opentnsim/graph_module.py` & `opentnsim-1.3.4/opentnsim/graph_module.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/opentnsim/lock.py` & `opentnsim-1.3.4/opentnsim/lock.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/opentnsim/model.py` & `opentnsim-1.3.4/opentnsim/model.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/opentnsim/plot.py` & `opentnsim-1.3.4/opentnsim/plot.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/opentnsim/strategy.py` & `opentnsim-1.3.4/opentnsim/strategy.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/opentnsim/utils.py` & `opentnsim-1.3.4/opentnsim/utils.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/opentnsim.egg-info/PKG-INFO` & `opentnsim-1.3.4/opentnsim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentnsim
-Version: 1.1.2
+Version: 1.3.4
 Summary: The OpenTNSim package aims to facilitate the analysis of network performance for different network configurations, fleet compositions and traffic rules.
 Home-page: https://github.com/TUDelft-CITG/OpenTNSim
 Author: Mark van Koningsveld
 Author-email: m.vankoningsveld@tudelft.nl
 License: mit
 Keywords: OpenTNSim
 Platform: any
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: opentnsim Version: 1.1.2 Summary: The OpenTNSim
+Metadata-Version: 2.1 Name: opentnsim Version: 1.3.4 Summary: The OpenTNSim
 package aims to facilitate the analysis of network performance for different
 network configurations, fleet compositions and traffic rules. Home-page: https:
 //github.com/TUDelft-CITG/OpenTNSim Author: Mark van Koningsveld Author-email:
 m.vankoningsveld@tudelft.nl License: mit Keywords: OpenTNSim Platform: any
 Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
 :: Developers Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3 Description-Content-Type: text/markdown Provides-Extra:
```

### Comparing `opentnsim-1.1.2/opentnsim.egg-info/SOURCES.txt` & `opentnsim-1.3.4/opentnsim.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 docs/opentnsim.rst
 docs/version-conventions.rst
 docs/_static/book.png
 opentnsim/__init__.py
 opentnsim/cli.py
 opentnsim/core.py
 opentnsim/energy.py
+opentnsim/fis.py
 opentnsim/graph_module.py
 opentnsim/lock.py
 opentnsim/model.py
 opentnsim/plot.py
 opentnsim/strategy.py
 opentnsim/utils.py
 opentnsim.egg-info/PKG-INFO
@@ -70,14 +71,15 @@
 tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route.py
 tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv
 tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py
 tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv
 tests/test_Van_Dorsser_et_al_2020_draught_payload.py
 tests/test_Van_Dorsser_et_al_2020_draught_payload_expected.csv
 tests/test_basic_simulation.py
+tests/test_fis.py
 tests/test_single_vessel_with_pre-conversion.py
 tests/test_single_vessel_without_pre-conversion.py
 tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py
 tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py
 tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py
 tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py
 tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py
```

### Comparing `opentnsim-1.1.2/setup.cfg` & `opentnsim-1.3.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -14,30 +14,14 @@
 	Programming Language :: Python
 
 [options]
 zip_safe = False
 packages = find:
 include_package_data = True
 setup_requires = pyscaffold>=3.1a0,<3.2a0
-install_requires = 
-	Deprecated
-	simpy
-	networkx
-	halem
-	shapely>=2
-	scipy
-	plotly
-	pyscaffold
-	simplekml
-	matplotlib
-	click
-	nose
-	flask
-	flask_cors
-	tqdm
 
 [options.packages.find]
 where = Transport-Network-Analysis
 
 [options.extras_require]
 testing = 
 	geopandas
```

### Comparing `opentnsim-1.1.2/setup.py` & `opentnsim-1.3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,33 +20,38 @@
     sys.exit(1)
 
 requires = [
     "pandas>=0.24.0",
     "openclsim>=0.16",
     "numpy",
     "simpy",
-    "networkx<3",
+    "networkx>=3",
+    "geopandas",
     "shapely>=2",
     "scipy",
     "click",
     "matplotlib",
     # read shapefiles
     "pyproj",
     # unit conversions
     "pint",
     "plotly",
     "simplekml",
     "nose",
+    # downloading
+    "requests",
+    "requests-cache",
     # web mode
     "Flask>=1.0",
     "Flask-cors",
     "sphinx_rtd_theme",
     "Dill",
     # deprecate old functions
     "Deprecated",
+    "tqdm",
 ]
 
 setup_requirements = [
     "pytest-runner",
 ]
 
 tests_require = [
@@ -70,15 +75,14 @@
     "notebook==6.4",
     "nbconvert==6.4",
     "jupyter",
     "jupyter-book==0.13.1",
     "ipywidgets==7.7",
     "jsonschema==3.0",
     "jupyterlab_widgets==3",
-    "tqdm",
 ]
 
 with open("README.md", "r") as des:
     long_description = des.read()
 
 setup(
     author="Mark van Koningsveld",
@@ -103,10 +107,10 @@
     name="opentnsim",
     packages=find_packages(include=["opentnsim"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=tests_require,
     extras_require={"testing": tests_require},
     url="https://github.com/TUDelft-CITG/OpenTNSim",
-    version="1.1.2",
+    version="1.3.4",
     zip_safe=False,
 )
```

### Comparing `opentnsim-1.1.2/tests/data/ect-bctn.json` & `opentnsim-1.3.4/tests/data/ect-bctn.json`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_current_influence_limiting_depth_single_and_round_trips_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_emission_rates_v_depth_engine_age.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_limiting_depth_route_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_uniform_depth_route_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_along_varying_depth_route_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_fuel_use_and_emissions_given_engine_age_round_trip_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_limiting_depth.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_limiting_depth.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_limiting_depth_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_limiting_depth_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_uniform_depth.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_uniform_depth.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_uniform_depth_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_uniform_depth_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_varying_depth.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_varying_depth.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_power2v_varying_depth_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_power2v_varying_depth_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_resistance_components.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_resistance_components.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_resistance_components_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_resistance_components_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_squat.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_squat.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_total_power.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_total_power.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_diesel_use_along_validation_route_with_C_year_without_C_year_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_emissions_along_validation_route_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv` & `opentnsim-1.3.4/tests/test_ManJiang_et_al_2022_v113_renewable_energy_sources_use_along_validation_route_expected.csv`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_Van_Dorsser_et_al_2020_draught_payload.py` & `opentnsim-1.3.4/tests/test_Van_Dorsser_et_al_2020_draught_payload.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_basic_simulation.py` & `opentnsim-1.3.4/tests/test_basic_simulation.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_single_vessel_with_pre-conversion.py` & `opentnsim-1.3.4/tests/test_single_vessel_with_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_single_vessel_without_pre-conversion.py` & `opentnsim-1.3.4/tests/test_single_vessel_without_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py` & `opentnsim-1.3.4/tests/test_two_vessels_bidirectional_simultaneous_arrival_with_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py` & `opentnsim-1.3.4/tests/test_two_vessels_bidirectional_simultaneous_arrival_without_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py` & `opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_with_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py` & `opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_separate_locking_without_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py` & `opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_with_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_without_pre-conversion.py` & `opentnsim-1.3.4/tests/test_two_vessels_unidirectional_simultaneous_arrival_simultaneous_locking_without_pre-conversion.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/test_utils.py` & `opentnsim-1.3.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/utils.py` & `opentnsim-1.3.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `opentnsim-1.1.2/tests/vessels/vessels.csv` & `opentnsim-1.3.4/tests/vessels/vessels.csv`

 * *Files identical despite different names*

