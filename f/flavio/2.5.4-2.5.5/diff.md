# Comparing `tmp/flavio-2.5.4.tar.gz` & `tmp/flavio-2.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flavio-2.5.4.tar", last modified: Mon Apr 24 15:13:52 2023, max compression
+gzip compressed data, was "flavio-2.5.5.tar", last modified: Thu Jun  1 13:34:12 2023, max compression
```

## Comparing `flavio-2.5.4.tar` & `flavio-2.5.5.tar`

### file list

```diff
@@ -1,379 +1,379 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.332509 flavio-2.5.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-04-24 15:07:11.000000 flavio-2.5.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:07:11.000000 flavio-2.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-24 15:13:52.332509 flavio-2.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-04-24 15:07:11.000000 flavio-2.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.264509 flavio-2.5.4/flavio/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/_parse_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/citations.py
--rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.268509 flavio-2.5.4/flavio/data/
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/citations.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)   984881 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/measurements.yml
--rw-r--r--   0 runner    (1001) docker     (123)    26734 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/parameters_correlated.yml
--rw-r--r--   0 runner    (1001) docker     (123)    87280 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/parameters_metadata.yml
--rw-r--r--   0 runner    (1001) docker     (123)    20166 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/parameters_uncorrelated.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.268509 flavio-2.5.4/flavio/data/test/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/test/1.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/test/2.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/test/2009.09313_digitized.npz
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/test/3.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/test/4.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    72365 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/test/SPheno-2.spc.MSSM
--rw-r--r--   0 runner    (1001) docker     (123)    72151 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/test/SPheno.spc.MSSM
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/data/test/wcxf-flavio-example.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.268509 flavio-2.5.4/flavio/io/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/io/instanceio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/io/test_yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/io/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.272509 flavio-2.5.4/flavio/math/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/math/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/math/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/math/integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/math/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/math/test_integrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/math/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/math/test_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.272509 flavio-2.5.4/flavio/physics/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.280509 flavio-2.5.4/flavio/physics/bdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/angular.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bc_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bll.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/blnu.py
--rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bpll.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bpll_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bpll_subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bpnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.284509 flavio-2.5.4/flavio/physics/bdecays/bvll/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/amplitudes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/nonfactorizable.py
--rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/observables_bs.py
--rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/qcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/qcdf_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/test_bvll.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/test_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/test_qcdf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py
--rw-r--r--   0 runner    (1001) docker     (123)    24633 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bvnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bxgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bxll.py
--rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bxll_qed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/bxlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.284509 flavio-2.5.4/flavio/physics/bdecays/formfactors/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.284509 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_gamma/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_gamma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.284509 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/btop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/cln.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/isgurwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/test_btop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.288509 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/btov.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/cln.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/clnexp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/isgurwise.py
--rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/test_btov.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/hqet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.288509 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_12/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_12/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      910 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_12/sse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.288509 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_32/
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_32/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/formfactors/test_cln.py
--rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/lambdablambda1520ll.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/lambdablambdagamma.py
--rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/lambdablambdall.py
--rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/lambdablambdall_subleading.py
--rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/matrixelements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_angular.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bc_lifetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bll.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_blnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bpll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bpll_lfv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bpnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bvgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bvlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bvnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bxgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bxll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_bxlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_lambdablambda1520ll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_lambdablambdall.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_matrixelements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/test_wc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/bdecays/wilsoncoefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.288509 flavio-2.5.4/flavio/physics/betadecays/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/betadecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/betadecays/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/betadecays/ft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/betadecays/test_betadecays.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ckm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.256509 flavio-2.5.4/flavio/physics/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.288509 flavio-2.5.4/flavio/physics/data/arXiv-0810-4077v3/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-0810-4077v3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   520886 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.296509 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/README
--rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_ls_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_sl_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_ss_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_ls_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_sl_results.d
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_ss_results.d
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.300509 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/
--rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31665 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31759 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31660 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31733 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.300509 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/
--rw-r--r--   0 runner    (1001) docker     (123)    31533 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31652 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31801 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    31903 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    31646 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.300509 flavio-2.5.4/flavio/physics/data/arXiv-1602-01399v1/
--rw-r--r--   0 runner    (1001) docker     (123)    30161 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d
--rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_results.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.304509 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json
--rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.304509 flavio-2.5.4/flavio/physics/data/arXiv-2102.07233v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.304509 flavio-2.5.4/flavio/physics/data/qcdf_interpolate/
--rw-r--r--   0 runner    (1001) docker     (123)   146774 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.308509 flavio-2.5.4/flavio/physics/data/wcsm/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.308509 flavio-2.5.4/flavio/physics/ddecays/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ddecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ddecays/dlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ddecays/dplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.308509 flavio-2.5.4/flavio/physics/ddecays/formfactors/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ddecays/formfactors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ddecays/formfactors/bcl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ddecays/formfactors/bsz.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ddecays/formfactors/test_formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ddecays/rge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ddecays/test_dlnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/ddecays/test_dplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.308509 flavio-2.5.4/flavio/physics/dileptons/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/dileptons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/dileptons/partondist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/dileptons/ppll.py
--rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/dileptons/pplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/dileptons/test_ppll.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/dileptons/test_pplnu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.312509 flavio-2.5.4/flavio/physics/edms/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/edms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/edms/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/edms/neutronedm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/edms/paraedm.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/edms/slcouplings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/edms/test_neutronedm.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/edms/test_paraedm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/eft.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.312509 flavio-2.5.4/flavio/physics/higgs/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/higgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/higgs/decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/higgs/production.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/higgs/signalstrength.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/higgs/test_higgs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/higgs/width.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.316509 flavio-2.5.4/flavio/physics/kdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/kll.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/klnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/kpilnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/kpinunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/kpipi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/lambdaplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/test_formfactors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/test_kll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/test_klnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/test_kpilnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/test_kpinunu.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/test_kpipi.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/test_lambdaplnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/kdecays/wilsoncoefficients.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.316509 flavio-2.5.4/flavio/physics/mdms/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mdms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mdms/al.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mdms/test_al.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.320509 flavio-2.5.4/flavio/physics/mesonmixing/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mesonmixing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mesonmixing/amplitude.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mesonmixing/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mesonmixing/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mesonmixing/test_mesonmixing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mesonmixing/wilsoncoefficient.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.320509 flavio-2.5.4/flavio/physics/mudecays/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mudecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mudecays/mu3e.py
--rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mudecays/mueconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mudecays/muegamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mudecays/test_mu3e.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mudecays/test_mueconversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/mudecays/test_muegamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.320509 flavio-2.5.4/flavio/physics/neutrinos/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/neutrinos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/neutrinos/test_trident.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/neutrinos/trident.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.324509 flavio-2.5.4/flavio/physics/quarkonium/
--rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/quarkonium/Pll.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/quarkonium/Sll.py
--rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/quarkonium/Vll.py
--rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/quarkonium/Vllgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/quarkonium/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/quarkonium/test_Pll.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/quarkonium/test_Sll.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/quarkonium/test_Vll.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/quarkonium/test_Vllgamma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.324509 flavio-2.5.4/flavio/physics/running/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/running/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/running/betafunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/running/masses.py
--rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/running/running.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/running/test_running.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.324509 flavio-2.5.4/flavio/physics/scattering/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/scattering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/scattering/ee_ww.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/scattering/test_ee_ww.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.328509 flavio-2.5.4/flavio/physics/taudecays/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/tau3l.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/taulgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/taulnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/taupl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/taupnu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/tauvl.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/test_tau3l.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/test_taulgamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/test_taulnunu.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/test_taupl.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/test_taupnu.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/taudecays/test_tauvl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/test_ckm.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/test_eft.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.328509 flavio-2.5.4/flavio/physics/wdecays/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/wdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/wdecays/gammaw.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/wdecays/mw.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/wdecays/test_mW.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/wdecays/test_wdecays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.332509 flavio-2.5.4/flavio/physics/zdecays/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/zdecays/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/zdecays/afbz.py
--rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/zdecays/gammaz.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/zdecays/gammazsm.py
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/zdecays/smeftew.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/zdecays/test_smeftew.py
--rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/physics/zdecays/test_zdecays.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.332509 flavio-2.5.4/flavio/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/plots/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/plots/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    39693 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/plots/plotfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/plots/test_plotfunctions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.332509 flavio-2.5.4/flavio/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/statistics/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/statistics/likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    88695 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/statistics/probability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/statistics/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/statistics/test_likelihood.py
--rw-r--r--   0 runner    (1001) docker     (123)    37591 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/statistics/test_probability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/test_citations.py
--rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/test_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/test_parseerrors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-24 15:07:11.000000 flavio-2.5.4/flavio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:13:52.264509 flavio-2.5.4/flavio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-24 15:13:52.000000 flavio-2.5.4/flavio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-04-24 15:13:52.000000 flavio-2.5.4/flavio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:13:52.000000 flavio-2.5.4/flavio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-24 15:13:52.000000 flavio-2.5.4/flavio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-24 15:13:52.000000 flavio-2.5.4/flavio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:13:52.332509 flavio-2.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-04-24 15:07:11.000000 flavio-2.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.794995 flavio-2.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-06-01 13:27:50.000000 flavio-2.5.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:27:50.000000 flavio-2.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-01 13:34:12.794995 flavio-2.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-06-01 13:27:50.000000 flavio-2.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.742995 flavio-2.5.5/flavio/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7808 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/_parse_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34349 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.746995 flavio-2.5.5/flavio/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/citations.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)   985205 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/measurements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    26734 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/parameters_correlated.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    87280 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/parameters_metadata.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20166 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/parameters_uncorrelated.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.750995 flavio-2.5.5/flavio/data/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/test/1.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/test/2.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20880 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/test/2009.09313_digitized.npz
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/test/3.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/test/4.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    72365 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/test/SPheno-2.spc.MSSM
+-rw-r--r--   0 runner    (1001) docker     (123)    72151 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/test/SPheno.spc.MSSM
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/data/test/wcxf-flavio-example.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.750995 flavio-2.5.5/flavio/io/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/io/instanceio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/io/test_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/io/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.750995 flavio-2.5.5/flavio/math/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/math/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/math/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/math/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/math/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/math/test_integrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/math/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/math/test_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8615 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10071 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.750995 flavio-2.5.5/flavio/physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.758995 flavio-2.5.5/flavio/physics/bdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23063 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/angular.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bc_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/blnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13932 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bpll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bpll_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5997 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bpll_subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8935 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bpnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.762995 flavio-2.5.5/flavio/physics/bdecays/bvll/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/amplitudes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4329 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/nonfactorizable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26541 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10380 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/observables_bs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/qcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/qcdf_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/test_bvll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/test_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/test_qcdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24633 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bvnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bxgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21779 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bxll.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19644 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bxll_qed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13458 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/bxlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.762995 flavio-2.5.5/flavio/physics/bdecays/formfactors/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.762995 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_gamma/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_gamma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.762995 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3118 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/btop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2094 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/isgurwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/test_btop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.766995 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/btov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/clnexp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/isgurwise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7690 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/test_btov.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5830 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/hqet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.766995 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_12/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_12/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      910 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_12/sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.766995 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_32/
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_32/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/formfactors/test_cln.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15733 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/lambdablambda1520ll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/lambdablambdagamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/lambdablambdall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5534 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/lambdablambdall_subleading.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10988 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/matrixelements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_angular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bc_lifetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8491 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_blnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2425 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bpll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bpll_lfv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bpnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bvgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5923 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bvlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bvnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bxgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bxll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_bxlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9563 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_lambdablambda1520ll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_lambdablambdall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_matrixelements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/test_wc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/bdecays/wilsoncoefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.766995 flavio-2.5.5/flavio/physics/betadecays/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/betadecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/betadecays/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14672 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/betadecays/ft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/betadecays/test_betadecays.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ckm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.738994 flavio-2.5.5/flavio/physics/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.766995 flavio-2.5.5/flavio/physics/data/arXiv-0810-4077v3/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-0810-4077v3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   520886 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.770995 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/README
+-rw-r--r--   0 runner    (1001) docker     (123)     4077 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_ls_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_sl_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     4391 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_ss_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_ls_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_sl_results.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_ss_results.d
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.770995 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    31696 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31665 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31724 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31759 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31660 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31733 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31559 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.774995 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/
+-rw-r--r--   0 runner    (1001) docker     (123)    31533 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31749 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31652 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31801 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31888 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31741 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31903 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    31646 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.774995 flavio-2.5.5/flavio/physics/data/arXiv-1602-01399v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    30161 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_results.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.774995 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18049 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18073 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17991 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17969 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.774995 flavio-2.5.5/flavio/physics/data/arXiv-2102.07233v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.774995 flavio-2.5.5/flavio/physics/data/qcdf_interpolate/
+-rw-r--r--   0 runner    (1001) docker     (123)   146774 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.774995 flavio-2.5.5/flavio/physics/data/wcsm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.774995 flavio-2.5.5/flavio/physics/ddecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ddecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ddecays/dlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ddecays/dplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.778995 flavio-2.5.5/flavio/physics/ddecays/formfactors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ddecays/formfactors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ddecays/formfactors/bcl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ddecays/formfactors/bsz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ddecays/formfactors/test_formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ddecays/rge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ddecays/test_dlnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/ddecays/test_dplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.778995 flavio-2.5.5/flavio/physics/dileptons/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/dileptons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/dileptons/partondist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8624 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/dileptons/ppll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7770 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/dileptons/pplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/dileptons/test_ppll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/dileptons/test_pplnu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.778995 flavio-2.5.5/flavio/physics/edms/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/edms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2574 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/edms/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/edms/neutronedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/edms/paraedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/edms/slcouplings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/edms/test_neutronedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/edms/test_paraedm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/eft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.778995 flavio-2.5.5/flavio/physics/higgs/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/higgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3885 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/higgs/decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/higgs/production.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/higgs/signalstrength.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/higgs/test_higgs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/higgs/width.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.782995 flavio-2.5.5/flavio/physics/kdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/kll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/klnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5591 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/kpilnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/kpinunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/kpipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/lambdaplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/test_formfactors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/test_kll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/test_klnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/test_kpilnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/test_kpinunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/test_kpipi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/test_lambdaplnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/kdecays/wilsoncoefficients.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.782995 flavio-2.5.5/flavio/physics/mdms/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mdms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2070 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mdms/al.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mdms/test_al.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.782995 flavio-2.5.5/flavio/physics/mesonmixing/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mesonmixing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4621 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mesonmixing/amplitude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mesonmixing/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9676 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mesonmixing/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9895 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mesonmixing/test_mesonmixing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mesonmixing/wilsoncoefficient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.782995 flavio-2.5.5/flavio/physics/mudecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mudecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mudecays/mu3e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4173 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mudecays/mueconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mudecays/muegamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mudecays/test_mu3e.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mudecays/test_mueconversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/mudecays/test_muegamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.782995 flavio-2.5.5/flavio/physics/neutrinos/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/neutrinos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/neutrinos/test_trident.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/neutrinos/trident.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.786995 flavio-2.5.5/flavio/physics/quarkonium/
+-rw-r--r--   0 runner    (1001) docker     (123)     4210 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/quarkonium/Pll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/quarkonium/Sll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7287 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/quarkonium/Vll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9262 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/quarkonium/Vllgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/quarkonium/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/quarkonium/test_Pll.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/quarkonium/test_Sll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/quarkonium/test_Vll.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/quarkonium/test_Vllgamma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.786995 flavio-2.5.5/flavio/physics/running/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/running/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/running/betafunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/running/masses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12998 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/running/running.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/running/test_running.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.786995 flavio-2.5.5/flavio/physics/scattering/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/scattering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17615 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/scattering/ee_ww.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/scattering/test_ee_ww.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.790995 flavio-2.5.5/flavio/physics/taudecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/tau3l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/taulgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2969 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/taulnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/taupl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/taupnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/tauvl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/test_tau3l.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/test_taulgamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/test_taulnunu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/test_taupl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/test_taupnu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/taudecays/test_tauvl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/test_ckm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/test_eft.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.790995 flavio-2.5.5/flavio/physics/wdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/wdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/wdecays/gammaw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/wdecays/mw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/wdecays/test_mW.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/wdecays/test_wdecays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.790995 flavio-2.5.5/flavio/physics/zdecays/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/zdecays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/zdecays/afbz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7028 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/zdecays/gammaz.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/zdecays/gammazsm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/zdecays/smeftew.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/zdecays/test_smeftew.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6563 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/physics/zdecays/test_zdecays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.794995 flavio-2.5.5/flavio/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/plots/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/plots/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40493 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/plots/plotfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/plots/test_plotfunctions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.794995 flavio-2.5.5/flavio/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/statistics/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31480 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/statistics/likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88695 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/statistics/probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/statistics/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13195 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/statistics/test_likelihood.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37591 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/statistics/test_probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/test_citations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18339 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/test_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/test_parseerrors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-01 13:27:50.000000 flavio-2.5.5/flavio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 13:34:12.746995 flavio-2.5.5/flavio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-06-01 13:34:12.000000 flavio-2.5.5/flavio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13325 2023-06-01 13:34:12.000000 flavio-2.5.5/flavio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 13:34:12.000000 flavio-2.5.5/flavio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-06-01 13:34:12.000000 flavio-2.5.5/flavio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 13:34:12.000000 flavio-2.5.5/flavio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 13:34:12.794995 flavio-2.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-01 13:27:50.000000 flavio-2.5.5/setup.py
```

### Comparing `flavio-2.5.4/LICENSE.txt` & `flavio-2.5.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/PKG-INFO` & `flavio-2.5.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavio
-Version: 2.5.4
+Version: 2.5.5
 Summary: A Python package for flavour physics phenomenology in the Standard Model and beyond
 Home-page: https://flav-io.github.io
 Author: David M. Straub
 Author-email: straub@protonmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flavio Version: 2.5.4 Summary: A Python package for
+Metadata-Version: 2.1 Name: flavio Version: 2.5.5 Summary: A Python package for
 flavour physics phenomenology in the Standard Model and beyond Home-page:
 https://flav-io.github.io Author: David M. Straub Author-email:
 straub@protonmail.com License: MIT Platform: UNKNOWN Description-Content-Type:
 text/markdown Provides-Extra: plotting Provides-Extra: sampling Provides-Extra:
 testing License-File: LICENSE.txt ![Build_Status](https://travis-ci.org/flav-
 io/flavio.svg?branch=master) [![Coverage Status](https://coveralls.io/repos/
 github/flav-io/flavio/badge.svg)](https://coveralls.io/github/flav-io/flavio)
```

### Comparing `flavio-2.5.4/README.md` & `flavio-2.5.5/README.md`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/__init__.py` & `flavio-2.5.5/flavio/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/_parse_errors.py` & `flavio-2.5.5/flavio/_parse_errors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/citations.py` & `flavio-2.5.5/flavio/citations.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/classes.py` & `flavio-2.5.5/flavio/classes.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/data/citations.yml` & `flavio-2.5.5/flavio/data/citations.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/data/config.yml` & `flavio-2.5.5/flavio/data/config.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/data/measurements.yml` & `flavio-2.5.5/flavio/data/measurements.yml`

 * *Files identical despite different names*

```diff
@@ -4505,14 +4505,28 @@
 
 LHCb RD* 2017:
   experiment: LHCb
   inspire: Aaij:2017uff
   values:
     Rtaumu(B->D*lnu): 0.291 ± 0.019 ± 0.026 ± 0.013
 
+LHCb RD* 2023:
+  experiment: LHCb
+  inspire: LHCb:2023cjr
+  values:
+    Rtaumu(B->D*lnu): 0.247 ± 0.015 ± 0.015 ± 0.012
+
+LHCb RD RD* 2022:
+    experiment: LHCb
+    inspire: LHCb:2023zxo
+    values:
+        Rtaumu(B->Dlnu): 0.441 +- 0.060 +- 0.066
+        Rtaumu(B->D*lnu): 0.281 +- 0.018 +- 0.024
+    correlation: -0.43
+
 CMS Bs->mumu 2013:
   experiment: CMS
   inspire: Chatrchyan:2013bka
   observables:
     - BR(Bs->mumu)
     - BR(B0->mumu)
   values:
```

### Comparing `flavio-2.5.4/flavio/data/parameters_correlated.yml` & `flavio-2.5.5/flavio/data/parameters_correlated.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/data/parameters_metadata.yml` & `flavio-2.5.5/flavio/data/parameters_metadata.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/data/parameters_uncorrelated.yml` & `flavio-2.5.5/flavio/data/parameters_uncorrelated.yml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/data/test/2009.09313_digitized.npz` & `flavio-2.5.5/flavio/data/test/2009.09313_digitized.npz`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/data/test/SPheno-2.spc.MSSM` & `flavio-2.5.5/flavio/data/test/SPheno-2.spc.MSSM`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/data/test/SPheno.spc.MSSM` & `flavio-2.5.5/flavio/data/test/SPheno.spc.MSSM`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/functions.py` & `flavio-2.5.5/flavio/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/io/instanceio.py` & `flavio-2.5.5/flavio/io/instanceio.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/io/test_yaml.py` & `flavio-2.5.5/flavio/io/test_yaml.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/io/yaml.py` & `flavio-2.5.5/flavio/io/yaml.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/math/functions.py` & `flavio-2.5.5/flavio/math/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/math/integrate.py` & `flavio-2.5.5/flavio/math/integrate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/math/optimize.py` & `flavio-2.5.5/flavio/math/optimize.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/math/test_math.py` & `flavio-2.5.5/flavio/math/test_math.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/math/test_optimize.py` & `flavio-2.5.5/flavio/math/test_optimize.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/measurements.py` & `flavio-2.5.5/flavio/measurements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/parameters.py` & `flavio-2.5.5/flavio/parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/__init__.py` & `flavio-2.5.5/flavio/physics/bdecays/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/angular.py` & `flavio-2.5.5/flavio/physics/bdecays/angular.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bc_lifetime.py` & `flavio-2.5.5/flavio/physics/bdecays/bc_lifetime.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bll.py` & `flavio-2.5.5/flavio/physics/bdecays/bll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bllgamma.py` & `flavio-2.5.5/flavio/physics/bdecays/bllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/blnu.py` & `flavio-2.5.5/flavio/physics/bdecays/blnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bpll.py` & `flavio-2.5.5/flavio/physics/bdecays/bpll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bpll_lfv.py` & `flavio-2.5.5/flavio/physics/bdecays/bpll_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bpll_subleading.py` & `flavio-2.5.5/flavio/physics/bdecays/bpll_subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bplnu.py` & `flavio-2.5.5/flavio/physics/bdecays/bplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bpnunu.py` & `flavio-2.5.5/flavio/physics/bdecays/bpnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvgamma.py` & `flavio-2.5.5/flavio/physics/bdecays/bvgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/_qcdf_interpolate_write.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/amplitudes.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/amplitudes.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/lfv.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/nonfactorizable.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/nonfactorizable.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/observables.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/observables.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/observables_bs.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/observables_bs.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/qcdf.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/qcdf.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/qcdf_interpolate.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/qcdf_interpolate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/subleading.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/test_bvll.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/test_bvll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/test_lfv.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/test_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/test_qcdf.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/test_qcdf.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py` & `flavio-2.5.5/flavio/physics/bdecays/bvll/test_qcdf_interpolate.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvlnu.py` & `flavio-2.5.5/flavio/physics/bdecays/bvlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bvnunu.py` & `flavio-2.5.5/flavio/physics/bdecays/bvnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bxgamma.py` & `flavio-2.5.5/flavio/physics/bdecays/bxgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bxll.py` & `flavio-2.5.5/flavio/physics/bdecays/bxll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bxll_qed.py` & `flavio-2.5.5/flavio/physics/bdecays/bxll_qed.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/bxlnu.py` & `flavio-2.5.5/flavio/physics/bdecays/bxlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/common.py` & `flavio-2.5.5/flavio/physics/bdecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_gamma/bgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bcl.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bcl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bcl_lmvd.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bcl_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bcl_parameters_lmvd.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bsz.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/bsz_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/btop.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/btop.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/cln.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/cln.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_p/test_btop.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_p/test_btop.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/bsz.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/bsz_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/btov.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/btov.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/cln.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/cln.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,28 +9,32 @@
 process_dict = {}
 process_dict['B->D*'] = {'B': 'B0', 'V': 'D*+', 'q': 'b->c'}
 
 
 def h_to_A(mB, mV, h, q2):
     """Convert HQET form factors to the standard basis.
 
-    See e.g. arXiv:1309.0301, eqs. (38), (39)"""
+    See e.g. arXiv:1309.0301, eqs. (38), (39) but notice that we use the
+    convention of arXiv:1703.05330 for h_T3, which differs by a factor -2
+    from the one in arXiv:1309.0301 (see Eq. (11e) in arXiv:1703.05330 and
+    Eq. (46b) in arXiv:1309.0301).
+    """
     ff = {}
     pre = 1 / 2 / sqrt(mB * mV)
     ff['V'] = pre * (mB + mV) * h['V']
     ff['A1'] = pre * ((mB + mV)**2 - q2) / (mB + mV) * h['A1']
     ff['A2'] = pre * (mB + mV) * (h['A3'] + mV / mB * h['A2'])
     ff['A0'] = pre * (((mB + mV)**2 - q2) / (2 * mV) * h['A1']
                       - (mB**2 - mV**2 + q2) / (2 * mB) * h['A2']
                       - (mB**2 - mV**2 - q2) / (2 * mV) * h['A3'])
     ff['T1'] = pre * ((mB + mV) * h['T1'] - (mB - mV) * h['T2'])
     ff['T2'] = pre * (((mB + mV)**2 - q2) / (mB + mV) * h['T1']
                       - ((mB - mV)**2 - q2) / (mB - mV) * h['T2'])
     ff['T3'] = pre * ((mB - mV) * h['T1'] - (mB + mV) * h['T2']
-                      - 2 * (mB**2 - mV**2) / mB * h['T3'])
+                      + (mB**2 - mV**2) / mB * h['T3']) # h_T3 as in arXiv:1703.05330
     # conversion from A_1, A_2 to A_12
     ff['A12'] = ((ff['A1'] * (mB + mV)**2 * (mB**2 - mV**2 - q2)
                  - ff['A2'] * (mB**4 + (mV**2 - q2)**2
                  - 2 * mB**2 * (mV**2 + q2)))
                  / (16. * mB * mV**2 * (mB + mV)))
     del ff['A2']
     # conversion from T_2, T_3 to T_23
```

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/clnexp.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/clnexp.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/isgurwise.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/isgurwise.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/lattice_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/sse.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/sse.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/b_v/test_btov.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/b_v/test_btov.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/common.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/hqet.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/hqet.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_12/lambdab.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_12/lattice_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_12/sse.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_12/sse.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_12/test_lambda.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_32/LatticeQCD.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_32/QuarkModel_MCN.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/lambdab_32/lambdab.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/formfactors/test_cln.py` & `flavio-2.5.5/flavio/physics/bdecays/formfactors/test_cln.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/lambdablambda1520ll.py` & `flavio-2.5.5/flavio/physics/bdecays/lambdablambda1520ll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/lambdablambdall.py` & `flavio-2.5.5/flavio/physics/bdecays/lambdablambdall.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/lambdablambdall_subleading.py` & `flavio-2.5.5/flavio/physics/bdecays/lambdablambdall_subleading.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/matrixelements.py` & `flavio-2.5.5/flavio/physics/bdecays/matrixelements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_angular.py` & `flavio-2.5.5/flavio/physics/bdecays/test_angular.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bc_lifetime.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bc_lifetime.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bll.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bllgamma.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_blnu.py` & `flavio-2.5.5/flavio/physics/bdecays/test_blnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bpll.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bpll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bpll_lfv.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bpll_lfv.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bplnu.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bpnunu.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bpnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bvgamma.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bvgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bvlnu.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bvlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bvnunu.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bvnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bxgamma.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bxgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bxll.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bxll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_bxlnu.py` & `flavio-2.5.5/flavio/physics/bdecays/test_bxlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_lambdablambda1520ll.py` & `flavio-2.5.5/flavio/physics/bdecays/test_lambdablambda1520ll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_lambdablambdall.py` & `flavio-2.5.5/flavio/physics/bdecays/test_lambdablambdall.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_matrixelements.py` & `flavio-2.5.5/flavio/physics/bdecays/test_matrixelements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/test_wc.py` & `flavio-2.5.5/flavio/physics/bdecays/test_wc.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/bdecays/wilsoncoefficients.py` & `flavio-2.5.5/flavio/physics/bdecays/wilsoncoefficients.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/betadecays/common.py` & `flavio-2.5.5/flavio/physics/betadecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/betadecays/ft.py` & `flavio-2.5.5/flavio/physics/betadecays/ft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/betadecays/test_betadecays.py` & `flavio-2.5.5/flavio/physics/betadecays/test_betadecays.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/ckm.py` & `flavio-2.5.5/flavio/physics/ckm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/common.py` & `flavio-2.5.5/flavio/physics/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat` & `flavio-2.5.5/flavio/physics/data/arXiv-0810-4077v3/f_12_79.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/README` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/README`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_ls_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_ls_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_sl_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_sl_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_ss_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/av_ss_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_ls_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_ls_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_sl_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_sl_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_ss_corrmat.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1501-00367v2/t_ss_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/Bomega_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/BsKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v1/Bsphi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/Bomega_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/BsKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1503-05534v2/Bsphi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat` & `flavio-2.5.5/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_covariance.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat` & `flavio-2.5.5/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_HO_results.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d` & `flavio-2.5.5/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.d`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat` & `flavio-2.5.5/flavio/physics/data/arXiv-1602-01399v1/LambdabLambda_covariance.dat`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BD_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BDstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BK_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/BKstar_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR-Lattice.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/Bpi_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json` & `flavio-2.5.5/flavio/physics/data/arXiv-1811-00983v1/Brho_LCSR.json`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml` & `flavio-2.5.5/flavio/physics/data/arXiv-2102.07233v2/LCSR-LQCD_mod_BCL_params_K=4.yaml`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz` & `flavio-2.5.5/flavio/physics/data/qcdf_interpolate/qcdf_interpolate.npz`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy` & `flavio-2.5.5/flavio/physics/data/wcsm/wc_sm_dB1_2_55.npy`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/ddecays/dlnu.py` & `flavio-2.5.5/flavio/physics/ddecays/dlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/ddecays/dplnu.py` & `flavio-2.5.5/flavio/physics/ddecays/dplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/ddecays/formfactors/__init__.py` & `flavio-2.5.5/flavio/physics/ddecays/formfactors/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/ddecays/formfactors/bcl.py` & `flavio-2.5.5/flavio/physics/ddecays/formfactors/bcl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/ddecays/formfactors/bsz.py` & `flavio-2.5.5/flavio/physics/ddecays/formfactors/bsz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/ddecays/formfactors/test_formfactors.py` & `flavio-2.5.5/flavio/physics/ddecays/formfactors/test_formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/ddecays/test_dlnu.py` & `flavio-2.5.5/flavio/physics/ddecays/test_dlnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/ddecays/test_dplnu.py` & `flavio-2.5.5/flavio/physics/ddecays/test_dplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/dileptons/partondist.py` & `flavio-2.5.5/flavio/physics/dileptons/partondist.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/dileptons/ppll.py` & `flavio-2.5.5/flavio/physics/dileptons/ppll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/dileptons/pplnu.py` & `flavio-2.5.5/flavio/physics/dileptons/pplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/dileptons/test_ppll.py` & `flavio-2.5.5/flavio/physics/dileptons/test_ppll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/dileptons/test_pplnu.py` & `flavio-2.5.5/flavio/physics/dileptons/test_pplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/edms/common.py` & `flavio-2.5.5/flavio/physics/edms/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/edms/neutronedm.py` & `flavio-2.5.5/flavio/physics/edms/neutronedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/edms/paraedm.py` & `flavio-2.5.5/flavio/physics/edms/paraedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/edms/test_neutronedm.py` & `flavio-2.5.5/flavio/physics/edms/test_neutronedm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/eft.py` & `flavio-2.5.5/flavio/physics/eft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/elements.py` & `flavio-2.5.5/flavio/physics/elements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/higgs/decay.py` & `flavio-2.5.5/flavio/physics/higgs/decay.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/higgs/production.py` & `flavio-2.5.5/flavio/physics/higgs/production.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/higgs/signalstrength.py` & `flavio-2.5.5/flavio/physics/higgs/signalstrength.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/higgs/test_higgs.py` & `flavio-2.5.5/flavio/physics/higgs/test_higgs.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/higgs/width.py` & `flavio-2.5.5/flavio/physics/higgs/width.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/formfactors.py` & `flavio-2.5.5/flavio/physics/kdecays/formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/kll.py` & `flavio-2.5.5/flavio/physics/kdecays/kll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/klnu.py` & `flavio-2.5.5/flavio/physics/kdecays/klnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/kpilnu.py` & `flavio-2.5.5/flavio/physics/kdecays/kpilnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/kpinunu.py` & `flavio-2.5.5/flavio/physics/kdecays/kpinunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/kpipi.py` & `flavio-2.5.5/flavio/physics/kdecays/kpipi.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/lambdaplnu.py` & `flavio-2.5.5/flavio/physics/kdecays/lambdaplnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/test_formfactors.py` & `flavio-2.5.5/flavio/physics/kdecays/test_formfactors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/test_kll.py` & `flavio-2.5.5/flavio/physics/kdecays/test_kll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/test_klnu.py` & `flavio-2.5.5/flavio/physics/kdecays/test_klnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/test_kpilnu.py` & `flavio-2.5.5/flavio/physics/kdecays/test_kpilnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/test_kpinunu.py` & `flavio-2.5.5/flavio/physics/kdecays/test_kpinunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/kdecays/wilsoncoefficients.py` & `flavio-2.5.5/flavio/physics/kdecays/wilsoncoefficients.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mdms/al.py` & `flavio-2.5.5/flavio/physics/mdms/al.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mdms/test_al.py` & `flavio-2.5.5/flavio/physics/mdms/test_al.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mesonmixing/amplitude.py` & `flavio-2.5.5/flavio/physics/mesonmixing/amplitude.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mesonmixing/common.py` & `flavio-2.5.5/flavio/physics/mesonmixing/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mesonmixing/observables.py` & `flavio-2.5.5/flavio/physics/mesonmixing/observables.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mesonmixing/test_mesonmixing.py` & `flavio-2.5.5/flavio/physics/mesonmixing/test_mesonmixing.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mesonmixing/wilsoncoefficient.py` & `flavio-2.5.5/flavio/physics/mesonmixing/wilsoncoefficient.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mudecays/mu3e.py` & `flavio-2.5.5/flavio/physics/mudecays/mu3e.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mudecays/mueconversion.py` & `flavio-2.5.5/flavio/physics/mudecays/mueconversion.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mudecays/muegamma.py` & `flavio-2.5.5/flavio/physics/mudecays/muegamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/mudecays/test_muegamma.py` & `flavio-2.5.5/flavio/physics/mudecays/test_muegamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/neutrinos/test_trident.py` & `flavio-2.5.5/flavio/physics/neutrinos/test_trident.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/neutrinos/trident.py` & `flavio-2.5.5/flavio/physics/neutrinos/trident.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/quarkonium/Pll.py` & `flavio-2.5.5/flavio/physics/quarkonium/Pll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/quarkonium/Sll.py` & `flavio-2.5.5/flavio/physics/quarkonium/Sll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/quarkonium/Vll.py` & `flavio-2.5.5/flavio/physics/quarkonium/Vll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/quarkonium/Vllgamma.py` & `flavio-2.5.5/flavio/physics/quarkonium/Vllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/quarkonium/test_Pll.py` & `flavio-2.5.5/flavio/physics/quarkonium/test_Pll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/quarkonium/test_Sll.py` & `flavio-2.5.5/flavio/physics/quarkonium/test_Sll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/quarkonium/test_Vll.py` & `flavio-2.5.5/flavio/physics/quarkonium/test_Vll.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/quarkonium/test_Vllgamma.py` & `flavio-2.5.5/flavio/physics/quarkonium/test_Vllgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/running/betafunctions.py` & `flavio-2.5.5/flavio/physics/running/betafunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/running/masses.py` & `flavio-2.5.5/flavio/physics/running/masses.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/running/running.py` & `flavio-2.5.5/flavio/physics/running/running.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/running/test_running.py` & `flavio-2.5.5/flavio/physics/running/test_running.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/scattering/ee_ww.py` & `flavio-2.5.5/flavio/physics/scattering/ee_ww.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/scattering/test_ee_ww.py` & `flavio-2.5.5/flavio/physics/scattering/test_ee_ww.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/taudecays/common.py` & `flavio-2.5.5/flavio/physics/taudecays/common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/taudecays/tau3l.py` & `flavio-2.5.5/flavio/physics/taudecays/tau3l.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/taudecays/taulgamma.py` & `flavio-2.5.5/flavio/physics/taudecays/taulgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/taudecays/taulnunu.py` & `flavio-2.5.5/flavio/physics/taudecays/taulnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/taudecays/taupl.py` & `flavio-2.5.5/flavio/physics/taudecays/taupl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/taudecays/taupnu.py` & `flavio-2.5.5/flavio/physics/taudecays/taupnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/taudecays/tauvl.py` & `flavio-2.5.5/flavio/physics/taudecays/tauvl.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/taudecays/test_taulgamma.py` & `flavio-2.5.5/flavio/physics/taudecays/test_taulgamma.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/taudecays/test_taulnunu.py` & `flavio-2.5.5/flavio/physics/taudecays/test_taulnunu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/taudecays/test_taupnu.py` & `flavio-2.5.5/flavio/physics/taudecays/test_taupnu.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/test_ckm.py` & `flavio-2.5.5/flavio/physics/test_ckm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/test_common.py` & `flavio-2.5.5/flavio/physics/test_common.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/test_eft.py` & `flavio-2.5.5/flavio/physics/test_eft.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/units.py` & `flavio-2.5.5/flavio/physics/units.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/wdecays/gammaw.py` & `flavio-2.5.5/flavio/physics/wdecays/gammaw.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/wdecays/mw.py` & `flavio-2.5.5/flavio/physics/wdecays/mw.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/wdecays/test_mW.py` & `flavio-2.5.5/flavio/physics/wdecays/test_mW.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/wdecays/test_wdecays.py` & `flavio-2.5.5/flavio/physics/wdecays/test_wdecays.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/zdecays/afbz.py` & `flavio-2.5.5/flavio/physics/zdecays/afbz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/zdecays/gammaz.py` & `flavio-2.5.5/flavio/physics/zdecays/gammaz.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/zdecays/gammazsm.py` & `flavio-2.5.5/flavio/physics/zdecays/gammazsm.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/zdecays/smeftew.py` & `flavio-2.5.5/flavio/physics/zdecays/smeftew.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/physics/zdecays/test_zdecays.py` & `flavio-2.5.5/flavio/physics/zdecays/test_zdecays.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/plots/__init__.py` & `flavio-2.5.5/flavio/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/plots/colors.py` & `flavio-2.5.5/flavio/plots/colors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/plots/plotfunctions.py` & `flavio-2.5.5/flavio/plots/plotfunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -504,37 +504,55 @@
     data = density_contour_data(x=x, y=y, covariance_factor=covariance_factor,
                                 n_bins=n_bins, n_sigma=n_sigma)
     data['z_min'] = np.min(data['z']) # set minimum to prevent warning
     data.update(kwargs) #  since we cannot do **data, **kwargs in Python <3.5
     return contour(**data)
 
 
-def likelihood_contour_data(log_likelihood, x_min, x_max, y_min, y_max,
-              n_sigma=1, steps=20, threads=1, pool=None):
+def likelihood_contour_data(
+        log_likelihood,
+        x_min, x_max, y_min, y_max, *,
+        xscale='linear', yscale='linear',
+        n_sigma=1, steps=20, threads=1, pool=None):
     r"""Generate data required to plot coloured confidence contours (or bands)
     given a log likelihood function.
 
     Parameters:
 
     - `log_likelihood`: function returning the logarithm of the likelihood.
       Can e.g. be the method of the same name of a FastFit instance.
     - `x_min`, `x_max`, `y_min`, `y_max`: data boundaries
+    - `xscale`, `yscale`: `linear` (default) or `log` scale
     - `n_sigma`: plot confidence level corresponding to this number of standard
       deviations. Either a number (defaults to 1) or a tuple to plot several
       contours.
     - `steps`: number of grid steps in each dimension (total computing time is
       this number squared times the computing time of one `log_likelihood` call!)
     - `threads`: number of threads, defaults to 1. If greater than one,
       computation of z values will be done in parallel.
     - `pool`: an instance of `multiprocessing.Pool` (or a compatible
     implementation, e.g. from `multiprocess` or `schwimmbad`). Overrides the
     `threads` argument.
     """
-    _x = np.linspace(x_min, x_max, steps)
-    _y = np.linspace(y_min, y_max, steps)
+    if xscale == 'linear':
+        _x = np.linspace(x_min, x_max, steps)
+    elif xscale == 'log':
+        if x_min <= 0 or x_max <= 0:
+            raise ValueError("`x_min` and `x_max` have to be positive if `xscale` is set to `log`.")
+        _x = np.logspace(np.log10(x_min), np.log10(x_max), steps)
+    else:
+        raise ValueError("`xscale` must be 'linear' or 'log'.")
+    if yscale == 'linear':
+        _y = np.linspace(y_min, y_max, steps)
+    elif yscale == 'log':
+        if y_min <= 0 or y_max <= 0:
+            raise ValueError("`y_min` and `y_max` have to be positive if `yscale` is set to `log`.")
+        _y = np.logspace(np.log10(y_min), np.log10(y_max), steps)
+    else:
+        raise ValueError("`yscale` must be 'linear' or 'log'.")
     x, y = np.meshgrid(_x, _y)
     if threads == 1:
         @np.vectorize
         def chi2_vect(x, y): # needed for evaluation on meshgrid
             return -2*log_likelihood([x,y])
         z = chi2_vect(x, y)
     else:
@@ -597,15 +615,15 @@
                   "and might be removed in the future. "
                   "Please update your code.", FutureWarning)
     valid_args = inspect.signature(likelihood_contour_data).parameters.keys()
     data_kwargs = {k:v for k,v in kwargs.items() if k in valid_args}
     if 'pre_calculated_z' not in kwargs:
         contour_kwargs = likelihood_contour_data(log_likelihood,
                       x_min, x_max, y_min, y_max,
-                      n_sigma, steps, **data_kwargs)
+                      n_sigma=n_sigma, steps=steps, **data_kwargs)
     else:
         contour_kwargs = {}
         nx, ny = kwargs['pre_calculated_z'].shape
         _x = np.linspace(x_min, x_max, nx)
         _y = np.linspace(y_min, y_max, ny)
         x, y = np.meshgrid(_x, _y)
         contour_kwargs['x'] = x
```

### Comparing `flavio-2.5.4/flavio/plots/test_plotfunctions.py` & `flavio-2.5.5/flavio/plots/test_plotfunctions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/statistics/functions.py` & `flavio-2.5.5/flavio/statistics/functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/statistics/likelihood.py` & `flavio-2.5.5/flavio/statistics/likelihood.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/statistics/probability.py` & `flavio-2.5.5/flavio/statistics/probability.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/statistics/test_functions.py` & `flavio-2.5.5/flavio/statistics/test_functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/statistics/test_likelihood.py` & `flavio-2.5.5/flavio/statistics/test_likelihood.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/statistics/test_probability.py` & `flavio-2.5.5/flavio/statistics/test_probability.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/test_citations.py` & `flavio-2.5.5/flavio/test_citations.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/test_classes.py` & `flavio-2.5.5/flavio/test_classes.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/test_functions.py` & `flavio-2.5.5/flavio/test_functions.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/test_measurements.py` & `flavio-2.5.5/flavio/test_measurements.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/test_parameters.py` & `flavio-2.5.5/flavio/test_parameters.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/test_parseerrors.py` & `flavio-2.5.5/flavio/test_parseerrors.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio/util.py` & `flavio-2.5.5/flavio/util.py`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/flavio.egg-info/PKG-INFO` & `flavio-2.5.5/flavio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flavio
-Version: 2.5.4
+Version: 2.5.5
 Summary: A Python package for flavour physics phenomenology in the Standard Model and beyond
 Home-page: https://flav-io.github.io
 Author: David M. Straub
 Author-email: straub@protonmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flavio Version: 2.5.4 Summary: A Python package for
+Metadata-Version: 2.1 Name: flavio Version: 2.5.5 Summary: A Python package for
 flavour physics phenomenology in the Standard Model and beyond Home-page:
 https://flav-io.github.io Author: David M. Straub Author-email:
 straub@protonmail.com License: MIT Platform: UNKNOWN Description-Content-Type:
 text/markdown Provides-Extra: plotting Provides-Extra: sampling Provides-Extra:
 testing License-File: LICENSE.txt ![Build_Status](https://travis-ci.org/flav-
 io/flavio.svg?branch=master) [![Coverage Status](https://coveralls.io/repos/
 github/flav-io/flavio/badge.svg)](https://coveralls.io/github/flav-io/flavio)
```

### Comparing `flavio-2.5.4/flavio.egg-info/SOURCES.txt` & `flavio-2.5.5/flavio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flavio-2.5.4/setup.py` & `flavio-2.5.5/setup.py`

 * *Files identical despite different names*

