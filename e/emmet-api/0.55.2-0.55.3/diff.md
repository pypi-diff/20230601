# Comparing `tmp/emmet-api-0.55.2.tar.gz` & `tmp/emmet-api-0.55.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emmet-api-0.55.2.tar", last modified: Tue May 16 21:41:50 2023, max compression
+gzip compressed data, was "emmet-api-0.55.3.tar", last modified: Thu Jun  1 18:07:11 2023, max compression
```

## Comparing `emmet-api-0.55.2.tar` & `emmet-api-0.55.3.tar`

### file list

```diff
@@ -1,346 +1,346 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-05-16 21:41:40.000000 emmet-api-0.55.2/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 21:41:50.237911 emmet-api-0.55.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-16 21:41:40.000000 emmet-api-0.55.2/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.205911 emmet-api-0.55.2/emmet/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/core/assets/
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/assets/mp_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/assets/mp_logo_small.png
--rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/documentation.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/global_header.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/core/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_consumer/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_consumer/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_general_store/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/_general_store/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/dois/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/dois/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/dois/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/materials/absorption/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/absorption/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/absorption/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/materials/alloys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/alloys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/alloys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/alloys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.213911 emmet-api-0.55.2/emmet/api/routes/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/charge_density/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/charge_density/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/chemenv/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/chemenv/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/dielectric/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/dielectric/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/elasticity/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/elasticity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electrodes/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electrodes/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electrodes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/eos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/eos/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/fermi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/fermi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/fermi/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.217911 emmet-api-0.55.2/emmet/api/routes/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/magnetism/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/magnetism/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/materials/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/materials/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/materials/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/materials/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/query_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/phonon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/phonon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/phonon/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/phonon/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/piezo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/piezo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/provenance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/provenance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/provenance/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/robocrys/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/robocrys/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/similarity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/similarity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/similarity/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/substrates/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/substrates/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/data_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/synthesis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.221911 emmet-api-0.55.2/emmet/api/routes/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/tasks/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/tasks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/thermo/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/xas/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/materials/xas/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/association/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/association/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/association/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/bonds/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/bonds/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/molecules/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/molecules/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/molecules/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/partial_charges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/partial_charges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/partial_charges/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/partial_spins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/partial_spins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/partial_spins/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/redox/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/redox/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/summary/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/summary/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/summary/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/tasks/hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/tasks/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/tasks/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/thermo/query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/thermo/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.225911 emmet-api-0.55.2/emmet/api/routes/molecules/vibrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/vibrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-16 21:41:40.000000 emmet-api-0.55.2/emmet/api/routes/molecules/vibrations/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/emmet_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-16 21:41:49.000000 emmet-api-0.55.2/emmet_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-05-16 21:41:50.000000 emmet-api-0.55.2/emmet_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:41:49.000000 emmet-api-0.55.2/emmet_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 21:41:49.000000 emmet-api-0.55.2/emmet_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-16 21:41:49.000000 emmet-api-0.55.2/emmet_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-16 21:41:49.000000 emmet-api-0.55.2/emmet_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-16 21:41:40.000000 emmet-api-0.55.2/legacy_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-05-16 21:41:40.000000 emmet-api-0.55.2/material_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-05-16 21:41:40.000000 emmet-api-0.55.2/molecule_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/deployment.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8979 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9323 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/macos-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5890 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.10.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9110 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.10_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.11.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.11_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6128 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.8.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.8_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6051 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.9.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9324 2023-05-16 21:41:40.000000 emmet-api-0.55.2/requirements/ubuntu-latest_py3.9_extras.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 21:41:50.237911 emmet-api-0.55.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-16 21:41:40.000000 emmet-api-0.55.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-16 21:41:40.000000 emmet-api-0.55.2/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/_consumer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/_consumer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/_consumer/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/_general_store/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/_general_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/_general_store/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/core/test_mapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.209911 emmet-api-0.55.2/tests/legacy/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/legacy/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/legacy/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/legacy/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.209911 emmet-api-0.55.2/tests/materials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/charge_density/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/charge_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/charge_density/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/chemenv/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/chemenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/chemenv/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/dielectric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/dielectric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/dielectric/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/elasticity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/elasticity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/elasticity/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.229911 emmet-api-0.55.2/tests/materials/electrodes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/electrodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/electrodes/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/electrodes/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/electronic_structure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/electronic_structure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/electronic_structure/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/eos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/eos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/grain_boundary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/grain_boundary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/grain_boundary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/magnetism/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/magnetism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/magnetism/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/materials/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/materials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/materials/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/materials/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/materials/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/mpcomplete/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/mpcomplete/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/mpcomplete/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/oxidation_states/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/oxidation_states/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/oxidation_states/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/piezo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/piezo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/piezo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/robocrys/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/robocrys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/robocrys/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/substrates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/substrates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/substrates/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/surface_properties/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/surface_properties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/surface_properties/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/synthesis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/synthesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/synthesis/test_adaptor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/synthesis/test_adaptor_synpro.py
--rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/synthesis/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/synthesis/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/tasks/test_query_operators.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/tasks/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/thermo/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/materials/xas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/xas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/materials/xas/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.233911 emmet-api-0.55.2/tests/molecules/bonds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/bonds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/bonds/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/molecules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/molecules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/molecules/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/molecules/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/orbitals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/orbitals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/orbitals/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/redox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/redox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/redox/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/summary/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/summary/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/summary/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/tasks/test_hint_scheme.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/tasks/test_query_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:50.237911 emmet-api-0.55.2/tests/molecules/thermo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/thermo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-16 21:41:40.000000 emmet-api-0.55.2/tests/molecules/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1837 2023-06-01 18:07:05.000000 emmet-api-0.55.3/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-01 18:07:11.300487 emmet-api-0.55.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-01 18:07:05.000000 emmet-api-0.55.3/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.272487 emmet-api-0.55.3/emmet/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.276487 emmet-api-0.55.3/emmet/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/core/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/assets/mp_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11087 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/assets/mp_logo_small.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/global_header.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/core/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_consumer/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_consumer/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_general_store/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/_general_store/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/dois/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/dois/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/dois/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5111 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/absorption/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/absorption/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/absorption/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/alloys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/alloys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/alloys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/alloys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3441 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/charge_density/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/charge_density/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/chemenv/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/chemenv/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2291 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/dielectric/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/dielectric/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/elasticity/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/elasticity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12780 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electrodes/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electrodes/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electrodes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.280487 emmet-api-0.55.3/emmet/api/routes/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/eos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/eos/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/fermi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/fermi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/fermi/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/magnetism/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/magnetism/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/materials/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/materials/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/materials/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4780 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/materials/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/query_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/phonon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/phonon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/phonon/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/phonon/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/piezo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/piezo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/provenance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/provenance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/provenance/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/robocrys/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/robocrys/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/similarity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/similarity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/similarity/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/substrates/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/substrates/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.284487 emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/data_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/synthesis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/tasks/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/tasks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/thermo/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/xas/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/materials/xas/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/association/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/association/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/association/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/bonds/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/bonds/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/molecules/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14682 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/molecules/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/molecules/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/partial_charges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/partial_charges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/partial_charges/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/partial_spins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/partial_spins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/partial_spins/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/redox/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/redox/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/summary/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/summary/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/summary/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/tasks/hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/tasks/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/tasks/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.288487 emmet-api-0.55.3/emmet/api/routes/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/thermo/query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/thermo/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/emmet/api/routes/molecules/vibrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/vibrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-06-01 18:07:05.000000 emmet-api-0.55.3/emmet/api/routes/molecules/vibrations/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/emmet_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-01 18:07:10.000000 emmet-api-0.55.3/emmet_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-06-01 18:07:11.000000 emmet-api-0.55.3/emmet_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:07:10.000000 emmet-api-0.55.3/emmet_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 18:07:10.000000 emmet-api-0.55.3/emmet_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-06-01 18:07:10.000000 emmet-api-0.55.3/emmet_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-01 18:07:10.000000 emmet-api-0.55.3/emmet_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-06-01 18:07:05.000000 emmet-api-0.55.3/legacy_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13027 2023-06-01 18:07:05.000000 emmet-api-0.55.3/material_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-06-01 18:07:05.000000 emmet-api-0.55.3/molecule_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     6259 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/deployment.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5911 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5850 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8981 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9437 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9360 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/macos-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.10.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9126 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.10_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5851 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.11.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.11_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9438 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.8_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.9.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 2023-06-01 18:07:05.000000 emmet-api-0.55.3/requirements/ubuntu-latest_py3.9_extras.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 18:07:11.300487 emmet-api-0.55.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-06-01 18:07:05.000000 emmet-api-0.55.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-06-01 18:07:05.000000 emmet-api-0.55.3/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/_consumer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/_consumer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/_consumer/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/_general_store/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/_general_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/_general_store/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/core/test_mapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.276487 emmet-api-0.55.3/tests/legacy/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/legacy/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/legacy/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/legacy/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.276487 emmet-api-0.55.3/tests/materials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/materials/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/materials/charge_density/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/charge_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/charge_density/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/materials/chemenv/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/chemenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/chemenv/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.292487 emmet-api-0.55.3/tests/materials/dielectric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/dielectric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/dielectric/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/elasticity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/elasticity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/elasticity/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/electrodes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/electrodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/electrodes/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/electrodes/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/electronic_structure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/electronic_structure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5055 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/electronic_structure/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/eos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/grain_boundary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/grain_boundary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/grain_boundary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/magnetism/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/magnetism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/magnetism/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/materials/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/materials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/materials/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6514 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/materials/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/materials/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/mpcomplete/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/mpcomplete/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/mpcomplete/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/oxidation_states/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/oxidation_states/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/oxidation_states/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/piezo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/piezo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/piezo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/robocrys/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/robocrys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/robocrys/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/substrates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/substrates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/substrates/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/surface_properties/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/surface_properties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/surface_properties/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/synthesis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/synthesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/synthesis/test_adaptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3170 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/synthesis/test_adaptor_synpro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7067 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/synthesis/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/synthesis/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/tasks/test_query_operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/tasks/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/thermo/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/materials/xas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/xas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/materials/xas/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.296487 emmet-api-0.55.3/tests/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/bonds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/bonds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/bonds/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/molecules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/molecules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/molecules/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7121 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/molecules/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/orbitals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/orbitals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/orbitals/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/redox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/redox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/redox/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/summary/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/summary/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/summary/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/tasks/test_hint_scheme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/tasks/test_query_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:11.300487 emmet-api-0.55.3/tests/molecules/thermo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/thermo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-01 18:07:05.000000 emmet-api-0.55.3/tests/molecules/thermo/test_query_operators.py
```

### Comparing `emmet-api-0.55.2/Dockerfile` & `emmet-api-0.55.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/app.py` & `emmet-api-0.55.3/app.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/core/api.py` & `emmet-api-0.55.3/emmet/api/core/api.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/core/assets/mp_logo.svg` & `emmet-api-0.55.3/emmet/api/core/assets/mp_logo.svg`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/core/assets/mp_logo_small.png` & `emmet-api-0.55.3/emmet/api/core/assets/mp_logo_small.png`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/core/documentation.py` & `emmet-api-0.55.3/emmet/api/core/documentation.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/core/global_header.py` & `emmet-api-0.55.3/emmet/api/core/global_header.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/core/settings.py` & `emmet-api-0.55.3/emmet/api/core/settings.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/_consumer/query_operator.py` & `emmet-api-0.55.3/emmet/api/routes/_consumer/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/_consumer/resources.py` & `emmet-api-0.55.3/emmet/api/routes/_consumer/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/_general_store/query_operator.py` & `emmet-api-0.55.3/emmet/api/routes/_general_store/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/_general_store/resources.py` & `emmet-api-0.55.3/emmet/api/routes/_general_store/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/dois/resources.py` & `emmet-api-0.55.3/emmet/api/routes/dois/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/legacy/jcesr/resources.py` & `emmet-api-0.55.3/emmet/api/routes/legacy/jcesr/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/absorption/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/absorption/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/alloys/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/alloys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/alloys/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/alloys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/bonds/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/bonds/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/charge_density/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/charge_density/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/charge_density/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/charge_density/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/chemenv/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/chemenv/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/chemenv/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/chemenv/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/dielectric/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/dielectric/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/dielectric/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/dielectric/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/elasticity/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/elasticity/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/elasticity/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/elasticity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/electrodes/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/electrodes/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/electrodes/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/electrodes/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/electrodes/utils.py` & `emmet-api-0.55.3/emmet/api/routes/materials/electrodes/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/electronic_structure/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/electronic_structure/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/eos/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/eos/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/fermi/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/fermi/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/grain_boundary/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/grain_boundary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/magnetism/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/magnetism/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/magnetism/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/magnetism/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/materials/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/materials/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/materials/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/materials/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/materials/utils.py` & `emmet-api-0.55.3/emmet/api/routes/materials/materials/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/query_operator.py` & `emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/query_operator.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/mpcomplete/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/mpcomplete/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/oxidation_states/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/oxidation_states/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/phonon/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/phonon/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/phonon/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/phonon/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/piezo/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/piezo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/piezo/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/piezo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/provenance/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/provenance/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/robocrys/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/robocrys/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/robocrys/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/robocrys/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/similarity/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/similarity/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/substrates/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/substrates/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/substrates/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/substrates/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/summary/hint_scheme.py` & `emmet-api-0.55.3/emmet/api/routes/materials/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/summary/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/summary/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/surface_properties/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/surface_properties/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/synthesis/data_adaptor.py` & `emmet-api-0.55.3/emmet/api/routes/materials/synthesis/data_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py` & `emmet-api-0.55.3/emmet/api/routes/materials/synthesis/data_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/synthesis/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/synthesis/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/synthesis/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/synthesis/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/synthesis/utils.py` & `emmet-api-0.55.3/emmet/api/routes/materials/synthesis/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/tasks/hint_scheme.py` & `emmet-api-0.55.3/emmet/api/routes/materials/tasks/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/tasks/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/tasks/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/tasks/utils.py` & `emmet-api-0.55.3/emmet/api/routes/materials/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/thermo/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/thermo/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/xas/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/materials/xas/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/materials/xas/resources.py` & `emmet-api-0.55.3/emmet/api/routes/materials/xas/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/association/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/association/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/bonds/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/bonds/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/bonds/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/bonds/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/molecules/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/molecules/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/molecules/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/molecules/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/orbitals/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/orbitals/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/partial_charges/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/partial_charges/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/partial_spins/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/partial_spins/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/redox/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/redox/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/redox/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/redox/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/summary/hint_scheme.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/summary/hint_scheme.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/summary/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/summary/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/summary/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/summary/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/tasks/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/tasks/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/tasks/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/tasks/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/thermo/query_operators.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/thermo/query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/thermo/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/thermo/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/utils.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet/api/routes/molecules/vibrations/resources.py` & `emmet-api-0.55.3/emmet/api/routes/molecules/vibrations/resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/emmet_api.egg-info/SOURCES.txt` & `emmet-api-0.55.3/emmet_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/legacy_resources.py` & `emmet-api-0.55.3/legacy_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/material_resources.py` & `emmet-api-0.55.3/material_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/molecule_resources.py` & `emmet-api-0.55.3/molecule_resources.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/requirements/deployment.txt` & `emmet-api-0.55.3/requirements/deployment.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=emmet/emmet-api/requirements/deployment.txt --resolver=backtracking emmet/emmet-api/setup.py python/requirements.txt
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -46,31 +46,33 @@
     # via matplotlib
 cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.2
+ddtrace==1.13.4
     # via emmet-api (emmet/emmet-api/setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
-    # via cattrs
-fastapi==0.95.1
+    # via
+    #   anyio
+    #   cattrs
+fastapi==0.95.2
     # via
     #   emmet-api (emmet/emmet-api/setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -106,15 +108,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.50.4
+maggma==0.51.3
     # via emmet-api (emmet/emmet-api/setup.py)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -130,15 +132,15 @@
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -157,51 +159,51 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   -r python/requirements.txt
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.14.1
     # via pymatgen
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -236,23 +238,23 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
@@ -260,15 +262,15 @@
     # via matminer
 scipy==1.10.1
     # via
     #   -r python/requirements.txt
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (emmet/emmet-api/setup.py)
 shapely==2.0.1
     # via
@@ -287,15 +289,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -306,26 +308,26 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (emmet/emmet-api/setup.py)
 werkzeug==2.3.4
     # via flask
```

### Comparing `emmet-api-0.55.2/requirements/macos-latest_py3.10.txt` & `emmet-api-0.55.3/requirements/macos-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
 #    pip-compile --output-file=requirements/macos-latest_py3.10.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -46,31 +46,33 @@
     # via matplotlib
 cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
-    # via cattrs
-fastapi==0.95.1
+    # via
+    #   anyio
+    #   cattrs
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -106,15 +108,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -128,15 +130,15 @@
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -154,50 +156,50 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.14.1
     # via pymatgen
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -232,38 +234,38 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -282,15 +284,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -301,26 +303,26 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.4
     # via flask
```

### Comparing `emmet-api-0.55.2/requirements/macos-latest_py3.10_extras.txt` & `emmet-api-0.55.3/requirements/ubuntu-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
 # This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -47,45 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.6
     # via pytest-cov
 cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
+    #   anyio
     #   cattrs
     #   pytest
-fastapi==0.95.1
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -95,15 +96,15 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.27.5
+griffe==0.29.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
@@ -144,15 +145,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -189,33 +190,33 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.21.2
+mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.0.0
+mkdocstrings-python==1.1.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -243,45 +244,45 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 platformdirs==3.5.1
     # via virtualenv
 plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.1
+pre-commit==3.3.2
     # via emmet-api (setup.py)
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -290,15 +291,15 @@
     #   robocrys
 pycodestyle==2.10.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -316,15 +317,15 @@
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.11
+pymdown-extensions==10.0.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -335,15 +336,15 @@
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
@@ -358,38 +359,38 @@
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -411,15 +412,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -437,33 +438,33 @@
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.30.0.0
+types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==67.7.0.2
+types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 virtualenv==20.23.0
     # via pre-commit
```

### Comparing `emmet-api-0.55.2/requirements/macos-latest_py3.11.txt` & `emmet-api-0.55.3/requirements/macos-latest_py3.11.txt`

 * *Files 1% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
 #    pip-compile --output-file=requirements/macos-latest_py3.11.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -46,29 +46,29 @@
     # via matplotlib
 cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.1
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -104,15 +104,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -126,15 +126,15 @@
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -152,50 +152,50 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.14.1
     # via pymatgen
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -230,38 +230,38 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -280,15 +280,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -299,26 +299,26 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.4
     # via flask
```

### Comparing `emmet-api-0.55.2/requirements/macos-latest_py3.11_extras.txt` & `emmet-api-0.55.3/requirements/ubuntu-latest_py3.11_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
 # This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.11_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -47,41 +47,41 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.6
     # via pytest-cov
 cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.1
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -91,15 +91,15 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.27.5
+griffe==0.29.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
@@ -140,15 +140,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -185,33 +185,33 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.21.2
+mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.0.0
+mkdocstrings-python==1.1.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -239,45 +239,45 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 platformdirs==3.5.1
     # via virtualenv
 plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.1
+pre-commit==3.3.2
     # via emmet-api (setup.py)
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -286,15 +286,15 @@
     #   robocrys
 pycodestyle==2.10.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -312,15 +312,15 @@
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.11
+pymdown-extensions==10.0.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -331,15 +331,15 @@
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
@@ -354,38 +354,38 @@
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -407,15 +407,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -428,33 +428,33 @@
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.30.0.0
+types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==67.7.0.2
+types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 virtualenv==20.23.0
     # via pre-commit
```

### Comparing `emmet-api-0.55.2/requirements/macos-latest_py3.8.txt` & `emmet-api-0.55.3/requirements/ubuntu-latest_py3.10.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -46,31 +46,33 @@
     # via matplotlib
 cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
-    # via cattrs
-fastapi==0.95.1
+    # via
+    #   anyio
+    #   cattrs
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -83,21 +85,15 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+    # via opentelemetry-api
 inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -112,15 +108,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -134,15 +130,15 @@
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -160,52 +156,50 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 plotly==5.14.1
     # via pymatgen
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -240,38 +234,38 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -290,15 +284,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -309,40 +303,35 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
-    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.4
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.2/requirements/macos-latest_py3.8_extras.txt` & `emmet-api-0.55.3/requirements/macos-latest_py3.10_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.10
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.10_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -47,45 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.6
     # via pytest-cov
 cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
+    #   anyio
     #   cattrs
     #   pytest
-fastapi==0.95.1
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -95,38 +96,30 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.27.5
+griffe==0.29.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+    # via opentelemetry-api
 inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -152,15 +145,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -197,33 +190,33 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.21.2
+mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.0.0
+mkdocstrings-python==1.1.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -251,47 +244,45 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 platformdirs==3.5.1
     # via virtualenv
 plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.1
+pre-commit==3.3.2
     # via emmet-api (setup.py)
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -300,15 +291,15 @@
     #   robocrys
 pycodestyle==2.10.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -326,15 +317,15 @@
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.11
+pymdown-extensions==10.0.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -345,15 +336,15 @@
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
@@ -368,38 +359,38 @@
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -421,15 +412,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -447,37 +438,33 @@
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.30.0.0
+types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==67.7.0.2
+types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
-    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
-    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 virtualenv==20.23.0
     # via pre-commit
@@ -490,13 +477,11 @@
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.2/requirements/macos-latest_py3.9.txt` & `emmet-api-0.55.3/requirements/ubuntu-latest_py3.11.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -46,31 +46,29 @@
     # via matplotlib
 cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.1
-    # via cattrs
-fastapi==0.95.1
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -83,19 +81,15 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via matplotlib
+    # via opentelemetry-api
 inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -110,15 +104,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -132,15 +126,15 @@
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -158,50 +152,50 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.14.1
     # via pymatgen
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -236,38 +230,38 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -286,15 +280,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -305,40 +299,35 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
-    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.4
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.2/requirements/macos-latest_py3.9_extras.txt` & `emmet-api-0.55.3/requirements/ubuntu-latest_py3.9_extras.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -47,45 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.6
     # via pytest-cov
 cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
+    #   anyio
     #   cattrs
     #   pytest
-fastapi==0.95.1
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -95,15 +96,15 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.27.5
+griffe==0.29.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
@@ -114,14 +115,15 @@
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via
     #   flask
     #   markdown
     #   mkdocs
+    #   mkdocstrings
     #   opentelemetry-api
 importlib-resources==5.12.0
     # via matplotlib
 inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
@@ -150,15 +152,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -195,33 +197,33 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.21.2
+mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.0.0
+mkdocstrings-python==1.1.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -249,45 +251,45 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 platformdirs==3.5.1
     # via virtualenv
 plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.1
+pre-commit==3.3.2
     # via emmet-api (setup.py)
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -296,15 +298,15 @@
     #   robocrys
 pycodestyle==2.10.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -322,15 +324,15 @@
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.11
+pymdown-extensions==10.0.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -341,15 +343,15 @@
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
@@ -364,38 +366,38 @@
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -417,15 +419,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -443,21 +445,21 @@
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.30.0.0
+types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==67.7.0.2
+types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mkdocstrings
     #   mp-api
@@ -465,15 +467,15 @@
     #   pydantic
     #   pydash
     #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 virtualenv==20.23.0
     # via pre-commit
```

### Comparing `emmet-api-0.55.2/requirements/ubuntu-latest_py3.10.txt` & `emmet-api-0.55.3/requirements/macos-latest_py3.9.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.10.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -46,31 +46,33 @@
     # via matplotlib
 cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
-    # via cattrs
-fastapi==0.95.1
+    # via
+    #   anyio
+    #   cattrs
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -83,15 +85,19 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via matplotlib
 inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -106,15 +112,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -128,15 +134,15 @@
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -154,50 +160,50 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.14.1
     # via pymatgen
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -232,38 +238,38 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -282,15 +288,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -301,35 +307,40 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
+    #   aioitertools
+    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
+    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.4
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.2/requirements/ubuntu-latest_py3.10_extras.txt` & `emmet-api-0.55.3/requirements/macos-latest_py3.8_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.10
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.10_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.8_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -47,45 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.6
     # via pytest-cov
 cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
+    #   anyio
     #   cattrs
     #   pytest
-fastapi==0.95.1
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -95,30 +96,39 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.27.5
+griffe==0.29.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   mkdocstrings
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
 inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -144,15 +154,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -189,33 +199,33 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.21.2
+mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.0.0
+mkdocstrings-python==1.1.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -243,45 +253,47 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 platformdirs==3.5.1
     # via virtualenv
 plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.1
+pre-commit==3.3.2
     # via emmet-api (setup.py)
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -290,15 +302,15 @@
     #   robocrys
 pycodestyle==2.10.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -316,15 +328,15 @@
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.11
+pymdown-extensions==10.0.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -335,15 +347,15 @@
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
@@ -358,38 +370,38 @@
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -411,15 +423,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -437,33 +449,37 @@
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.30.0.0
+types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==67.7.0.2
+types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
+    #   aioitertools
+    #   bytecode
     #   ddtrace
     #   emmet-core
+    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
+    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 virtualenv==20.23.0
     # via pre-commit
@@ -476,11 +492,13 @@
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.2/requirements/ubuntu-latest_py3.11.txt` & `emmet-api-0.55.3/requirements/ubuntu-latest_py3.8.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.11.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -46,29 +46,33 @@
     # via matplotlib
 cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.1
+exceptiongroup==1.1.1
+    # via
+    #   anyio
+    #   cattrs
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -81,15 +85,21 @@
 h11==0.14.0
     # via uvicorn-tschaume
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
 inflect==6.0.4
     # via robocrys
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
     # via flask
 jmespath==1.0.1
@@ -104,15 +114,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -126,15 +136,15 @@
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -152,50 +162,52 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 plotly==5.14.1
     # via pymatgen
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -230,38 +242,38 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -280,15 +292,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -299,35 +311,40 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
+    #   aioitertools
+    #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
+    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.4
     # via flask
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.2/requirements/ubuntu-latest_py3.11_extras.txt` & `emmet-api-0.55.3/requirements/ubuntu-latest_py3.8_extras.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.11
+# This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.11_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -47,41 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.6
     # via pytest-cov
 cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-fastapi==0.95.1
+exceptiongroup==1.1.1
+    # via
+    #   anyio
+    #   cattrs
+    #   pytest
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -91,30 +96,39 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.27.5
+griffe==0.29.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via opentelemetry-api
+    # via
+    #   flask
+    #   markdown
+    #   mkdocs
+    #   mkdocstrings
+    #   opentelemetry-api
+importlib-resources==5.12.0
+    # via
+    #   jsonschema
+    #   matplotlib
 inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -140,15 +154,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -185,33 +199,33 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.21.2
+mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.0.0
+mkdocstrings-python==1.1.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -239,45 +253,47 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
+pkgutil-resolve-name==1.3.10
+    # via jsonschema
 platformdirs==3.5.1
     # via virtualenv
 plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.1
+pre-commit==3.3.2
     # via emmet-api (setup.py)
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -286,15 +302,15 @@
     #   robocrys
 pycodestyle==2.10.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -312,15 +328,15 @@
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.11
+pymdown-extensions==10.0.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -331,15 +347,15 @@
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
@@ -354,38 +370,38 @@
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -407,54 +423,63 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via
     #   ddtrace
     #   plotly
 threadpoolctl==3.1.0
     # via scikit-learn
+tomli==2.0.1
+    # via
+    #   coverage
+    #   mypy
+    #   pytest
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.30.0.0
+types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==67.7.0.2
+types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
+    #   aioitertools
+    #   bytecode
     #   ddtrace
     #   emmet-core
+    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
+    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 virtualenv==20.23.0
     # via pre-commit
@@ -467,11 +492,13 @@
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via importlib-metadata
+    # via
+    #   importlib-metadata
+    #   importlib-resources
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.2/requirements/ubuntu-latest_py3.8.txt` & `emmet-api-0.55.3/requirements/macos-latest_py3.8.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #
 # This file is autogenerated by pip-compile with Python 3.8
 # by the following command:
 #
-#    pip-compile --output-file=requirements/ubuntu-latest_py3.8.txt --resolver=backtracking
+#    pip-compile --output-file=requirements/macos-latest_py3.8.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -46,31 +46,33 @@
     # via matplotlib
 cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
-    # via cattrs
-fastapi==0.95.1
+    # via
+    #   anyio
+    #   cattrs
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -112,15 +114,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -134,15 +136,15 @@
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -160,52 +162,52 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 pkgutil-resolve-name==1.3.10
     # via jsonschema
 plotly==5.14.1
     # via pymatgen
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -240,38 +242,38 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -290,15 +292,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -309,29 +311,29 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
     #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.4
     # via flask
```

### Comparing `emmet-api-0.55.2/requirements/ubuntu-latest_py3.8_extras.txt` & `emmet-api-0.55.3/requirements/macos-latest_py3.9_extras.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.8
+# This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.8_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.9_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -47,45 +47,46 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.6
     # via pytest-cov
 cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
     # via
+    #   anyio
     #   cattrs
     #   pytest
-fastapi==0.95.1
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -95,15 +96,15 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.27.5
+griffe==0.29.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
@@ -114,19 +115,18 @@
     #   anyio
     #   requests
 importlib-metadata==6.0.1
     # via
     #   flask
     #   markdown
     #   mkdocs
+    #   mkdocstrings
     #   opentelemetry-api
 importlib-resources==5.12.0
-    # via
-    #   jsonschema
-    #   matplotlib
+    # via matplotlib
 inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -152,15 +152,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -197,33 +197,33 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.21.2
+mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.0.0
+mkdocstrings-python==1.1.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -251,47 +251,45 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
-pkgutil-resolve-name==1.3.10
-    # via jsonschema
 platformdirs==3.5.1
     # via virtualenv
 plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.1
+pre-commit==3.3.2
     # via emmet-api (setup.py)
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -300,15 +298,15 @@
     #   robocrys
 pycodestyle==2.10.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -326,15 +324,15 @@
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.11
+pymdown-extensions==10.0.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -345,15 +343,15 @@
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
@@ -368,38 +366,38 @@
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -421,15 +419,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -447,21 +445,21 @@
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.30.0.0
+types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==67.7.0.2
+types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mkdocstrings
     #   mp-api
@@ -469,15 +467,15 @@
     #   pydantic
     #   pydash
     #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 virtualenv==20.23.0
     # via pre-commit
```

### Comparing `emmet-api-0.55.2/requirements/ubuntu-latest_py3.9.txt` & `emmet-api-0.55.3/requirements/ubuntu-latest_py3.9.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 # This file is autogenerated by pip-compile with Python 3.9
 # by the following command:
 #
 #    pip-compile --output-file=requirements/ubuntu-latest_py3.9.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -46,31 +46,33 @@
     # via matplotlib
 cryptography==40.0.2
     # via paramiko
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
 exceptiongroup==1.1.1
-    # via cattrs
-fastapi==0.95.1
+    # via
+    #   anyio
+    #   cattrs
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 flask==2.3.2
     # via mongogrant
 fonttools==4.39.4
     # via matplotlib
@@ -110,15 +112,15 @@
     # via
     #   ddtrace
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markupsafe==2.1.2
     # via
     #   jinja2
     #   werkzeug
 matminer==0.8.0
     # via robocrys
@@ -132,15 +134,15 @@
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -158,50 +160,50 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mongomock
     #   plotly
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 plotly==5.14.1
     # via pymatgen
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -236,38 +238,38 @@
     #   pandas
 pytz==2023.3
     # via pandas
 pyyaml==6.0
     # via pybtex
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -286,15 +288,15 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
@@ -305,29 +307,29 @@
 threadpoolctl==3.1.0
     # via scikit-learn
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
     #   aioitertools
     #   bytecode
     #   ddtrace
     #   emmet-core
     #   mp-api
     #   pydantic
     #   pydash
     #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 werkzeug==2.3.4
     # via flask
```

### Comparing `emmet-api-0.55.2/requirements/ubuntu-latest_py3.9_extras.txt` & `emmet-api-0.55.3/requirements/macos-latest_py3.11_extras.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #
-# This file is autogenerated by pip-compile with Python 3.9
+# This file is autogenerated by pip-compile with Python 3.11
 # by the following command:
 #
-#    pip-compile --all-extras --output-file=requirements/ubuntu-latest_py3.9_extras.txt --resolver=backtracking
+#    pip-compile --all-extras --output-file=requirements/macos-latest_py3.11_extras.txt --resolver=backtracking
 #
 aioitertools==0.11.0
     # via maggma
-anyio==3.6.2
+anyio==3.7.0
     # via starlette
 attrs==23.1.0
     # via
     #   cattrs
     #   ddtrace
     #   jsonschema
 bcrypt==4.0.1
     # via paramiko
 blinker==1.6.2
     # via flask
-boto3==1.26.133
+boto3==1.26.142
     # via
     #   emmet-api (setup.py)
     #   maggma
-botocore==1.29.133
+botocore==1.29.142
     # via
     #   boto3
     #   s3transfer
 bracex==2.3.post1
     # via wcmatch
-bytecode==0.14.1
+bytecode==0.14.2
     # via ddtrace
 cattrs==22.2.0
     # via ddtrace
 certifi==2023.5.7
     # via requests
 cffi==1.15.1
     # via
@@ -47,45 +47,41 @@
     #   mkdocs
     #   mongogrant
     #   uvicorn-tschaume
 colorama==0.4.6
     # via griffe
 contourpy==1.0.7
     # via matplotlib
-coverage[toml]==7.2.5
+coverage[toml]==7.2.6
     # via pytest-cov
 cryptography==40.0.2
     # via paramiko
 csscompressor==0.9.5
     # via mkdocs-minify-plugin
 cycler==0.11.0
     # via matplotlib
 ddsketch==2.0.4
     # via ddtrace
-ddtrace==1.13.1
+ddtrace==1.13.4
     # via emmet-api (setup.py)
-deprecated==1.2.13
+deprecated==1.2.14
     # via opentelemetry-api
 distlib==0.3.6
     # via virtualenv
 dnspython==2.3.0
     # via
     #   maggma
     #   pymongo
-emmet-core[all]==0.55.0
+emmet-core[all]==0.55.2
     # via
     #   emmet-api (setup.py)
     #   mp-api
 envier==0.4.0
     # via ddtrace
-exceptiongroup==1.1.1
-    # via
-    #   cattrs
-    #   pytest
-fastapi==0.95.1
+fastapi==0.95.2
     # via
     #   emmet-api (setup.py)
     #   maggma
 filelock==3.12.0
     # via virtualenv
 flake8==6.0.0
     # via emmet-api (setup.py)
@@ -95,36 +91,30 @@
     # via matplotlib
 future==0.18.3
     # via
     #   matminer
     #   uncertainties
 ghp-import==2.1.0
     # via mkdocs
-griffe==0.27.5
+griffe==0.29.0
     # via mkdocstrings-python
 gunicorn==20.1.0
     # via emmet-api (setup.py)
 h11==0.14.0
     # via uvicorn-tschaume
 htmlmin2==0.1.13
     # via mkdocs-minify-plugin
 identify==2.5.24
     # via pre-commit
 idna==3.4
     # via
     #   anyio
     #   requests
 importlib-metadata==6.0.1
-    # via
-    #   flask
-    #   markdown
-    #   mkdocs
-    #   opentelemetry-api
-importlib-resources==5.12.0
-    # via matplotlib
+    # via opentelemetry-api
 inflect==6.0.4
     # via robocrys
 iniconfig==2.0.0
     # via pytest
 itsdangerous==2.1.2
     # via flask
 jinja2==3.1.2
@@ -150,15 +140,15 @@
     #   maggma
 kiwisolver==1.4.4
     # via matplotlib
 latexcodec==2.0.1
     # via pybtex
 livereload==2.6.3
     # via emmet-api (setup.py)
-maggma==0.50.4
+maggma==0.51.1
     # via emmet-api (setup.py)
 markdown==3.3.7
     # via
     #   mkdocs
     #   mkdocs-autorefs
     #   mkdocs-material
     #   mkdocstrings
@@ -195,33 +185,33 @@
     # via emmet-api (setup.py)
 mkdocs-material-extensions==1.1.1
     # via
     #   emmet-api (setup.py)
     #   mkdocs-material
 mkdocs-minify-plugin==0.6.4
     # via emmet-api (setup.py)
-mkdocstrings[python]==0.21.2
+mkdocstrings[python]==0.22.0
     # via
     #   emmet-api (setup.py)
     #   mkdocstrings-python
-mkdocstrings-python==1.0.0
+mkdocstrings-python==1.1.0
     # via mkdocstrings
 mongogrant==0.3.3
     # via maggma
 mongomock==4.1.2
     # via maggma
 monty==2023.5.8
     # via
     #   emmet-core
     #   maggma
     #   matminer
     #   mp-api
     #   pymatgen
     #   robocrys
-mp-api==0.33.2
+mp-api==0.33.3
     # via pymatgen
 mpmath==1.3.0
     # via sympy
 msgpack==1.0.5
     # via
     #   maggma
     #   mp-api
@@ -249,45 +239,45 @@
     #   pymatgen
     #   robocrys
     #   scikit-learn
     #   scipy
     #   seekpath
     #   shapely
     #   spglib
-opentelemetry-api==1.17.0
+opentelemetry-api==1.18.0
     # via ddtrace
-orjson==3.8.12
+orjson==3.8.14
     # via maggma
 packaging==23.1
     # via
     #   ddtrace
     #   matplotlib
     #   mkdocs
     #   mongomock
     #   plotly
     #   pytest
 palettable==3.3.3
     # via pymatgen
-pandas==2.0.1
+pandas==2.0.2
     # via
     #   matminer
     #   pymatgen
-paramiko==3.1.0
+paramiko==3.2.0
     # via sshtunnel
 pillow==9.5.0
     # via matplotlib
 platformdirs==3.5.1
     # via virtualenv
 plotly==5.14.1
     # via pymatgen
 pluggy==1.0.0
     # via pytest
-pre-commit==3.3.1
+pre-commit==3.3.2
     # via emmet-api (setup.py)
-protobuf==4.23.0
+protobuf==4.23.2
     # via
     #   ddsketch
     #   ddtrace
 pubchempy==1.0.4
     # via robocrys
 pybtex==0.24.0
     # via
@@ -296,15 +286,15 @@
     #   robocrys
 pycodestyle==2.10.0
     # via
     #   emmet-api (setup.py)
     #   flake8
 pycparser==2.21
     # via cffi
-pydantic==1.10.7
+pydantic==1.10.8
     # via
     #   emmet-core
     #   fastapi
     #   inflect
     #   maggma
 pydash==7.0.3
     # via maggma
@@ -322,15 +312,15 @@
     #   pymatgen-analysis-alloys
     #   pymatgen-analysis-diffusion
     #   robocrys
 pymatgen-analysis-alloys==0.0.6
     # via emmet-core
 pymatgen-analysis-diffusion==2022.7.21
     # via emmet-core
-pymdown-extensions==9.11
+pymdown-extensions==10.0.1
     # via
     #   mkdocs-material
     #   mkdocstrings
 pymongo==4.3.3
     # via
     #   maggma
     #   matminer
@@ -341,15 +331,15 @@
     # via matplotlib
 pyrsistent==0.19.3
     # via jsonschema
 pytest==7.3.1
     # via
     #   emmet-api (setup.py)
     #   pytest-cov
-pytest-cov==4.0.0
+pytest-cov==4.1.0
     # via emmet-api (setup.py)
 python-dateutil==2.8.2
     # via
     #   botocore
     #   ghp-import
     #   maggma
     #   matplotlib
@@ -364,38 +354,38 @@
     #   pybtex
     #   pymdown-extensions
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 pyzmq==24.0.1
     # via maggma
-requests==2.30.0
+requests==2.31.0
     # via
     #   matminer
     #   mongogrant
     #   mp-api
     #   pymatgen
 robocrys==0.2.7
     # via emmet-core
-ruamel-yaml==0.17.26
+ruamel-yaml==0.17.28
     # via
     #   pymatgen
     #   robocrys
 ruamel-yaml-clib==0.2.7
     # via ruamel-yaml
 s3transfer==0.6.1
     # via boto3
 scikit-learn==1.2.2
     # via matminer
 scipy==1.10.1
     # via
     #   pymatgen
     #   robocrys
     #   scikit-learn
-seekpath==2.0.1
+seekpath==2.1.0
     # via emmet-core
 sentinels==1.0.0
     # via mongomock
 setproctitle==1.3.2
     # via emmet-api (setup.py)
 shapely==2.0.1
     # via
@@ -417,63 +407,54 @@
     # via
     #   emmet-core
     #   pymatgen
     #   robocrys
     #   seekpath
 sshtunnel==0.4.0
     # via maggma
-starlette==0.26.1
+starlette==0.27.0
     # via fastapi
 sympy==1.12
     # via
     #   matminer
     #   pymatgen
 tabulate==0.9.0
     # via pymatgen
 tenacity==8.2.2
     # via
     #   ddtrace
     #   plotly
 threadpoolctl==3.1.0
     # via scikit-learn
-tomli==2.0.1
-    # via
-    #   coverage
-    #   mypy
-    #   pytest
 tornado==6.3.2
     # via livereload
 tqdm==4.65.0
     # via
     #   maggma
     #   matminer
     #   pymatgen
-types-requests==2.30.0.0
+types-requests==2.31.0.1
     # via emmet-api (setup.py)
-types-setuptools==67.7.0.2
+types-setuptools==67.8.0.0
     # via emmet-api (setup.py)
 types-urllib3==1.26.25.13
     # via types-requests
-typing-extensions==4.5.0
+typing-extensions==4.6.2
     # via
-    #   aioitertools
-    #   bytecode
     #   ddtrace
     #   emmet-core
-    #   mkdocstrings
     #   mp-api
     #   mypy
     #   pydantic
     #   pydash
-    #   starlette
 tzdata==2023.3
     # via pandas
 uncertainties==3.1.7
     # via pymatgen
-urllib3==1.26.15
+urllib3==1.26.16
     # via
     #   botocore
     #   requests
 uvicorn-tschaume==0.19.1
     # via emmet-api (setup.py)
 virtualenv==20.23.0
     # via pre-commit
@@ -486,13 +467,11 @@
 wincertstore==0.2
     # via emmet-api (setup.py)
 wrapt==1.15.0
     # via deprecated
 xmltodict==0.13.0
     # via ddtrace
 zipp==3.15.0
-    # via
-    #   importlib-metadata
-    #   importlib-resources
+    # via importlib-metadata
 
 # The following packages are considered to be unsafe in a requirements file:
 # setuptools
```

### Comparing `emmet-api-0.55.2/setup.py` & `emmet-api-0.55.3/setup.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/_consumer/test_query_operators.py` & `emmet-api-0.55.3/tests/_consumer/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/_general_store/test_query_operators.py` & `emmet-api-0.55.3/tests/_general_store/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/core/test_mapi.py` & `emmet-api-0.55.3/tests/core/test_mapi.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/legacy/molecules/test_query_operators.py` & `emmet-api-0.55.3/tests/legacy/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/bonds/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/charge_density/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/charge_density/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/chemenv/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/chemenv/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/dielectric/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/dielectric/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/elasticity/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/elasticity/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/electrodes/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/electrodes/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/electrodes/test_utils.py` & `emmet-api-0.55.3/tests/materials/electrodes/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/electronic_structure/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/electronic_structure/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/grain_boundary/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/grain_boundary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/magnetism/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/magnetism/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/materials/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/materials/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/materials/test_utils.py` & `emmet-api-0.55.3/tests/materials/materials/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/mpcomplete/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/mpcomplete/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/oxidation_states/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/oxidation_states/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/piezo/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/piezo/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/robocrys/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/robocrys/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/substrates/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/substrates/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/summary/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/surface_properties/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/surface_properties/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/synthesis/test_adaptor.py` & `emmet-api-0.55.3/tests/materials/synthesis/test_adaptor.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/synthesis/test_adaptor_synpro.py` & `emmet-api-0.55.3/tests/materials/synthesis/test_adaptor_synpro.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/synthesis/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/synthesis/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/synthesis/test_utils.py` & `emmet-api-0.55.3/tests/materials/synthesis/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/tasks/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/tasks/test_utils.py` & `emmet-api-0.55.3/tests/materials/tasks/test_utils.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/materials/xas/test_query_operators.py` & `emmet-api-0.55.3/tests/materials/xas/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/molecules/bonds/test_query_operators.py` & `emmet-api-0.55.3/tests/molecules/bonds/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/molecules/molecules/test_query_operators.py` & `emmet-api-0.55.3/tests/molecules/molecules/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/molecules/orbitals/test_query_operators.py` & `emmet-api-0.55.3/tests/molecules/orbitals/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/molecules/redox/test_query_operators.py` & `emmet-api-0.55.3/tests/molecules/redox/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/molecules/summary/test_query_operators.py` & `emmet-api-0.55.3/tests/molecules/summary/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/molecules/tasks/test_query_operators.py` & `emmet-api-0.55.3/tests/molecules/tasks/test_query_operators.py`

 * *Files identical despite different names*

### Comparing `emmet-api-0.55.2/tests/molecules/thermo/test_query_operators.py` & `emmet-api-0.55.3/tests/molecules/thermo/test_query_operators.py`

 * *Files identical despite different names*

