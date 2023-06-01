# Comparing `tmp/pyerrors-2.8.0.tar.gz` & `tmp/pyerrors-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyerrors-2.8.0.tar", last modified: Sun May 21 16:09:27 2023, max compression
+gzip compressed data, was "pyerrors-2.8.1.tar", last modified: Thu Jun  1 12:41:28 2023, max compression
```

## Comparing `pyerrors-2.8.0.tar` & `pyerrors-2.8.1.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.504111 pyerrors-2.8.0/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/.github/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      113 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/CODEOWNERS
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1051 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/ISSUE_TEMPLATE/bug-report.yml
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/.github/workflows/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      386 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/binder.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      737 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/codeql.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1012 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/docs.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1022 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/examples.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      547 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/flake8.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1043 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.github/workflows/pytest.yml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      211 2023-03-21 12:48:56.000000 pyerrors-2.8.0/.gitignore
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16537 2023-05-21 16:06:57.000000 pyerrors-2.8.0/CHANGELOG.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1278 2023-05-21 16:06:57.000000 pyerrors-2.8.0/CITATION.cff
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1842 2023-03-21 12:48:56.000000 pyerrors-2.8.0/CONTRIBUTING.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1070 2023-03-11 21:38:08.000000 pyerrors-2.8.0/LICENSE
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-05-21 16:09:27.504111 pyerrors-2.8.0/PKG-INFO
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1610 2023-05-21 16:06:57.000000 pyerrors-2.8.0/README.md
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        0 2023-03-11 21:38:08.000000 pyerrors-2.8.0/conftest.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.496111 pyerrors-2.8.0/examples/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87858 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/01_basic_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    62623 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/02_correlators.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    97653 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/03_pcac_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   129847 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/04_fit_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9053 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/05_matrix_operations.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30851 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/06_gevp.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10604 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/07_data_management.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    21826 2023-03-21 12:48:56.000000 pyerrors-2.8.0/examples/08_combined_fit_example.ipynb
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      757 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/base_style.mplstyle
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.496111 pyerrors-2.8.0/examples/data/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7407 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/correlator_test.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15009 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/f_A.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15072 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/f_P.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266539 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/matrix_correlator.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266778 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/matrix_correlator_V1V1.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266803 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/matrix_correlator_V2V2.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266702 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/data/matrix_correlator_V3V3.json.gz
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8575 2023-03-11 21:38:08.000000 pyerrors-2.8.0/examples/json_schema.json
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/pyerrors/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    29950 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/__init__.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    57481 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/correlators.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3609 2023-03-11 21:38:08.000000 pyerrors-2.8.0/pyerrors/covobs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2909 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/dirac.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30996 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/fits.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/pyerrors/input/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      579 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/__init__.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    25145 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/input/bdio.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30913 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/input/dobs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    19262 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/hadrons.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    26602 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/json.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8064 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/misc.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    49814 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/openQCD.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6509 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/pandas.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16290 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/input/sfcf.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2257 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/input/utils.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10177 2023-03-11 21:38:08.000000 pyerrors-2.8.0/pyerrors/linalg.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     5381 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/misc.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2273 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/mpm.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    67811 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/obs.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1466 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyerrors/roots.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       22 2023-05-21 16:06:57.000000 pyerrors-2.8.0/pyerrors/version.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/pyerrors.egg-info/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-05-21 16:09:27.000000 pyerrors-2.8.0/pyerrors.egg-info/PKG-INFO
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2700 2023-05-21 16:09:27.000000 pyerrors-2.8.0/pyerrors.egg-info/SOURCES.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        1 2023-05-21 16:09:27.000000 pyerrors-2.8.0/pyerrors.egg-info/dependency_links.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      196 2023-05-21 16:09:27.000000 pyerrors-2.8.0/pyerrors.egg-info/requires.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        9 2023-05-21 16:09:27.000000 pyerrors-2.8.0/pyerrors.egg-info/top_level.txt
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      100 2023-03-21 12:48:56.000000 pyerrors-2.8.0/pyproject.toml
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       38 2023-05-21 16:09:27.504111 pyerrors-2.8.0/setup.cfg
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1882 2023-03-21 12:48:56.000000 pyerrors-2.8.0/setup.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1159 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/benchmark_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    17752 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/correlators_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3470 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/covobs_test.py
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.488111 pyerrors-2.8.0/tests/data/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/data/openqcd_test/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87320 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/openqcd_test/openqcd2r1.ms.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2076 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/openqcd_test/openqcd2r1.ms1.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   157504 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/openqcd_test/sfqcdr1.gfms.dat
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      252 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/openqcd_test/sfqcdr1.rwms.dat
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/tests/data/sfcf_test/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.488111 pyerrors-2.8.0/tests/data/sfcf_test/broken_data_c/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/data/sfcf_test/broken_data_c/data_c_r0/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8712 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/data/sfcf_test/data_a/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    24665 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.F_V0
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14670 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.f_1
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9090 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.f_A
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.488111 pyerrors-2.8.0/tests/data/sfcf_test/data_c/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/data/sfcf_test/data_c/data_c_r0/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8918 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/tests/data/sfcf_test/data_o/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.492111 pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.500111 pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     4926 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2927 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1811 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A
-drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-05-21 16:09:27.504111 pyerrors-2.8.0/tests/data/sfcf_test/param/
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   142045 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/param/out.out
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_a
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_c
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_o
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1885 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/dirac_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    44785 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/fits_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15556 2023-05-21 16:06:57.000000 pyerrors-2.8.0/tests/json_io_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14226 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/linalg_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      543 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/misc_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      314 2023-03-11 21:38:08.000000 pyerrors-2.8.0/tests/mpm_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    45834 2023-05-21 16:06:57.000000 pyerrors-2.8.0/tests/obs_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7967 2023-05-21 16:06:57.000000 pyerrors-2.8.0/tests/openQCD_in_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10938 2023-05-21 16:06:57.000000 pyerrors-2.8.0/tests/pandas_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1262 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/roots_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6431 2023-03-21 12:48:56.000000 pyerrors-2.8.0/tests/sfcf_in_test.py
--rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1415 2023-05-21 16:06:57.000000 pyerrors-2.8.0/tests/utils_in_test.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.620364 pyerrors-2.8.1/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/.github/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      113 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/CODEOWNERS
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1051 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/ISSUE_TEMPLATE/bug-report.yml
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/.github/workflows/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      386 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/workflows/binder.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      737 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/workflows/codeql.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1012 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/workflows/docs.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1022 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/workflows/examples.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      547 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.github/workflows/flake8.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1043 2023-06-01 12:28:18.000000 pyerrors-2.8.1/.github/workflows/pytest.yml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      211 2023-03-21 12:48:56.000000 pyerrors-2.8.1/.gitignore
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16778 2023-06-01 12:32:58.000000 pyerrors-2.8.1/CHANGELOG.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1278 2023-05-21 16:06:57.000000 pyerrors-2.8.1/CITATION.cff
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1842 2023-03-21 12:48:56.000000 pyerrors-2.8.1/CONTRIBUTING.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1070 2023-03-11 21:38:08.000000 pyerrors-2.8.1/LICENSE
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-06-01 12:41:28.620364 pyerrors-2.8.1/PKG-INFO
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1610 2023-06-01 12:28:18.000000 pyerrors-2.8.1/README.md
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        0 2023-03-11 21:38:08.000000 pyerrors-2.8.1/conftest.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.608364 pyerrors-2.8.1/examples/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87858 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/01_basic_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    62623 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/02_correlators.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    97653 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/03_pcac_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   129847 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/04_fit_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9053 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/05_matrix_operations.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30851 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/06_gevp.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10604 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/07_data_management.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    21826 2023-03-21 12:48:56.000000 pyerrors-2.8.1/examples/08_combined_fit_example.ipynb
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      757 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/base_style.mplstyle
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.612364 pyerrors-2.8.1/examples/data/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     7407 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/correlator_test.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15009 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/f_A.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15072 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/f_P.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266539 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/matrix_correlator.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266778 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/matrix_correlator_V1V1.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266803 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/matrix_correlator_V2V2.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   266702 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/data/matrix_correlator_V3V3.json.gz
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8575 2023-03-11 21:38:08.000000 pyerrors-2.8.1/examples/json_schema.json
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.612364 pyerrors-2.8.1/pyerrors/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    29950 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/__init__.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    57481 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/correlators.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3609 2023-06-01 12:29:24.000000 pyerrors-2.8.1/pyerrors/covobs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2909 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/dirac.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30996 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/fits.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/pyerrors/input/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      579 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/input/__init__.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    25145 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/input/bdio.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    30920 2023-06-01 12:29:24.000000 pyerrors-2.8.1/pyerrors/input/dobs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    19262 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/input/hadrons.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    26602 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/input/json.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8064 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/input/misc.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    50595 2023-06-01 12:29:24.000000 pyerrors-2.8.1/pyerrors/input/openQCD.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6691 2023-06-01 12:29:24.000000 pyerrors-2.8.1/pyerrors/input/pandas.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    16290 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/input/sfcf.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2257 2023-05-21 16:06:57.000000 pyerrors-2.8.1/pyerrors/input/utils.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    10177 2023-03-11 21:38:08.000000 pyerrors-2.8.1/pyerrors/linalg.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     5381 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/misc.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2273 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/mpm.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    67930 2023-06-01 12:29:24.000000 pyerrors-2.8.1/pyerrors/obs.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1466 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyerrors/roots.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       22 2023-06-01 12:33:26.000000 pyerrors-2.8.1/pyerrors/version.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/pyerrors.egg-info/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2705 2023-06-01 12:41:28.000000 pyerrors-2.8.1/pyerrors.egg-info/PKG-INFO
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2700 2023-06-01 12:41:28.000000 pyerrors-2.8.1/pyerrors.egg-info/SOURCES.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        1 2023-06-01 12:41:28.000000 pyerrors-2.8.1/pyerrors.egg-info/dependency_links.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      202 2023-06-01 12:41:28.000000 pyerrors-2.8.1/pyerrors.egg-info/requires.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)        9 2023-06-01 12:41:28.000000 pyerrors-2.8.1/pyerrors.egg-info/top_level.txt
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      100 2023-03-21 12:48:56.000000 pyerrors-2.8.1/pyproject.toml
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)       38 2023-06-01 12:41:28.620364 pyerrors-2.8.1/setup.cfg
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1888 2023-06-01 12:34:43.000000 pyerrors-2.8.1/setup.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/tests/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1159 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/benchmark_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    17752 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/correlators_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     3470 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/covobs_test.py
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/tests/data/openqcd_test/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    38800 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    87320 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/openqcd_test/openqcd2r1.ms.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2076 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/openqcd_test/openqcd2r1.ms1.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   157504 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/openqcd_test/sfqcdr1.gfms.dat
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      252 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/openqcd_test/sfqcdr1.rwms.dat
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/sfcf_test/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/sfcf_test/broken_data_c/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/tests/data/sfcf_test/broken_data_c/data_c_r0/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8712 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/tests/data/sfcf_test/data_a/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    24665 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.F_V0
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14670 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.f_1
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9090 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.f_A
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/sfcf_test/data_c/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.616364 pyerrors-2.8.1/tests/data/sfcf_test/data_c/data_c_r0/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     8918 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/sfcf_test/data_o/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.604364 pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.620364 pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     4926 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     2927 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1811 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A
+drwxrwxr-x   0 fjosw     (1000) fjosw     (1000)        0 2023-06-01 12:41:28.620364 pyerrors-2.8.1/tests/data/sfcf_test/param/
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)   142045 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/param/out.out
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_a
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_c
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1661 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_o
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1885 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/dirac_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    44785 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/fits_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    15556 2023-05-21 16:06:57.000000 pyerrors-2.8.1/tests/json_io_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    14226 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/linalg_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      543 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/misc_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)      314 2023-03-11 21:38:08.000000 pyerrors-2.8.1/tests/mpm_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    46296 2023-06-01 12:29:24.000000 pyerrors-2.8.1/tests/obs_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     9253 2023-06-01 12:29:24.000000 pyerrors-2.8.1/tests/openQCD_in_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)    11768 2023-06-01 12:29:24.000000 pyerrors-2.8.1/tests/pandas_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1262 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/roots_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     6431 2023-03-21 12:48:56.000000 pyerrors-2.8.1/tests/sfcf_in_test.py
+-rw-rw-r--   0 fjosw     (1000) fjosw     (1000)     1415 2023-05-21 16:06:57.000000 pyerrors-2.8.1/tests/utils_in_test.py
```

### Comparing `pyerrors-2.8.0/.github/ISSUE_TEMPLATE/bug-report.yml` & `pyerrors-2.8.1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/.github/workflows/codeql.yml` & `pyerrors-2.8.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/.github/workflows/docs.yml` & `pyerrors-2.8.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/.github/workflows/examples.yml` & `pyerrors-2.8.1/.github/workflows/examples.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/.github/workflows/flake8.yml` & `pyerrors-2.8.1/.github/workflows/flake8.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/.github/workflows/pytest.yml` & `pyerrors-2.8.1/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/CHANGELOG.md` & `pyerrors-2.8.1/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [2.8.1] - 2023-06-01
+### Fixed
+- `input.pandas` can now deal with columns that only have `None` entries.
+- Bug in f-string conversion of `Obs` fixed.
+- Bug in edge case of `_compute_drho` fixed.
+- Several numpy 1.25 deprecations fixed.
+
+
 ## [2.8.0] - 2023-05-21
 ### Added
 - `pyerrors` can now deal with replica with different gapsizes.
 - String formatting method for `Obs` added.
 - `t0` can now be extracted from hadrons files.
 - `w0` can now be extracted from openQCD files.
 - `pandas` SQL export can now deal with `None` entries in columns with `pyerrors` datatypes.
```

### Comparing `pyerrors-2.8.0/CITATION.cff` & `pyerrors-2.8.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/CONTRIBUTING.md` & `pyerrors-2.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/LICENSE` & `pyerrors-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/PKG-INFO` & `pyerrors-2.8.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerrors
-Version: 2.8.0
+Version: 2.8.1
 Summary: Error propagation and statistical analysis for Monte Carlo simulations
 Home-page: https://github.com/fjosw/pyerrors
 Author: Fabian Joswig
 Author-email: fabian.joswig@ed.ac.uk
 License: MIT
 Project-URL: Documentation, https://fjosw.github.io/pyerrors/pyerrors.html
 Project-URL: Bug Tracker, https://github.com/fjosw/pyerrors/issues
```

### Comparing `pyerrors-2.8.0/README.md` & `pyerrors-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/01_basic_example.ipynb` & `pyerrors-2.8.1/examples/01_basic_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/02_correlators.ipynb` & `pyerrors-2.8.1/examples/02_correlators.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/03_pcac_example.ipynb` & `pyerrors-2.8.1/examples/03_pcac_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/04_fit_example.ipynb` & `pyerrors-2.8.1/examples/04_fit_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/05_matrix_operations.ipynb` & `pyerrors-2.8.1/examples/05_matrix_operations.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/06_gevp.ipynb` & `pyerrors-2.8.1/examples/06_gevp.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/07_data_management.ipynb` & `pyerrors-2.8.1/examples/07_data_management.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/08_combined_fit_example.ipynb` & `pyerrors-2.8.1/examples/08_combined_fit_example.ipynb`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/base_style.mplstyle` & `pyerrors-2.8.1/examples/base_style.mplstyle`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/data/correlator_test.json.gz` & `pyerrors-2.8.1/examples/data/correlator_test.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/data/f_A.json.gz` & `pyerrors-2.8.1/examples/data/f_A.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/data/f_P.json.gz` & `pyerrors-2.8.1/examples/data/f_P.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/data/matrix_correlator.json.gz` & `pyerrors-2.8.1/examples/data/matrix_correlator.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/data/matrix_correlator_V1V1.json.gz` & `pyerrors-2.8.1/examples/data/matrix_correlator_V1V1.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/data/matrix_correlator_V2V2.json.gz` & `pyerrors-2.8.1/examples/data/matrix_correlator_V2V2.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/data/matrix_correlator_V3V3.json.gz` & `pyerrors-2.8.1/examples/data/matrix_correlator_V3V3.json.gz`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/examples/json_schema.json` & `pyerrors-2.8.1/examples/json_schema.json`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/__init__.py` & `pyerrors-2.8.1/pyerrors/__init__.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/correlators.py` & `pyerrors-2.8.1/pyerrors/correlators.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/covobs.py` & `pyerrors-2.8.1/pyerrors/covobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         else:
             self._set_grad(grad)
         self.value = mean
 
     def errsq(self):
         """ Return the variance (= square of the error) of the Covobs
         """
-        return float(np.dot(np.transpose(self.grad), np.dot(self.cov, self.grad)))
+        return np.dot(np.transpose(self.grad), np.dot(self.cov, self.grad)).item()
 
     def _set_cov(self, cov):
         """ Set the covariance matrix of the covobs
 
         Parameters
         ----------
         cov : list or array
```

### Comparing `pyerrors-2.8.0/pyerrors/dirac.py` & `pyerrors-2.8.1/pyerrors/dirac.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/fits.py` & `pyerrors-2.8.1/pyerrors/fits.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/input/__init__.py` & `pyerrors-2.8.1/pyerrors/input/__init__.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/input/bdio.py` & `pyerrors-2.8.1/pyerrors/input/bdio.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/input/dobs.py` & `pyerrors-2.8.1/pyerrors/input/dobs.py`

 * *Files 1% similar despite different names*

```diff
@@ -846,15 +846,15 @@
 
             gradd = {'id': 'grad'}
             gradd['layout'] = '%d f%d' % (ncov, len(obsl))
             ds = ''
             for i in range(ncov):
                 for o in obsl:
                     if cname in o.covobs:
-                        val = o.covobs[cname].grad[i]
+                        val = o.covobs[cname].grad[i].item()
                         if val != 0:
                             ds += '%1.14e ' % (val)
                         else:
                             ds += '0 '
                     else:
                         ds += '0 '
             gradd['#data'] = ds
```

### Comparing `pyerrors-2.8.0/pyerrors/input/hadrons.py` & `pyerrors-2.8.1/pyerrors/input/hadrons.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/input/json.py` & `pyerrors-2.8.1/pyerrors/input/json.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/input/misc.py` & `pyerrors-2.8.1/pyerrors/input/misc.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/input/openQCD.py` & `pyerrors-2.8.1/pyerrors/input/openQCD.py`

 * *Files 2% similar despite different names*

```diff
@@ -1159,14 +1159,16 @@
         The correlator to extract data for.
     sep : str, optional
         The separator to use when parsing the replika names.
     **kwargs
         Additional keyword arguments. The following keyword arguments are recognized:
 
         - names (List[str]): A list of names to use for the replicas.
+        - files (List[str]): A list of files to read data from.
+        - idl (List[List[int]]): A list of idls per replicum, resticting data to the idls given.
 
     Returns
     -------
     Corr
         A complex valued `Corr` object containing the data read from the files. In case of boudary to bulk correlators.
     or
     CObs
@@ -1207,15 +1209,16 @@
             if not sep == "":
                 se = f.split(".")[0]
                 for s in f.split(".")[1:-2]:
                     se += "." + s
                 names.append(se.split(sep)[0] + "|r" + se.split(sep)[1])
             else:
                 names.append(prefix)
-
+    if 'idl' in kwargs:
+        expected_idl = kwargs.get('idl')
     names = sorted(names)
     files = sorted(files)
 
     cnfgs = []
     realsamples = []
     imagsamples = []
     repnum = 0
@@ -1250,41 +1253,49 @@
             packstr = '=i' + ('d' * 2 * tmax * 10) + ('d' * 2 * 2)
             cnfgs.append([])
             realsamples.append([])
             imagsamples.append([])
             for t in range(tmax):
                 realsamples[repnum].append([])
                 imagsamples[repnum].append([])
-
+            if 'idl' in kwargs:
+                left_idl = set(expected_idl[repnum])
             while True:
                 cnfgt = fp.read(chunksize)
                 if not cnfgt:
                     break
                 asascii = struct.unpack(packstr, cnfgt)
                 cnfg = asascii[0]
-                cnfgs[repnum].append(cnfg)
-
-                if corr not in placesBB:
-                    tmpcorr = asascii[1 + 2 * tmax * placesBI.index(corr):1 + 2 * tmax * placesBI.index(corr) + 2 * tmax]
-                else:
-                    tmpcorr = asascii[1 + 2 * tmax * len(placesBI) + 2 * placesBB.index(corr):1 + 2 * tmax * len(placesBI) + 2 * placesBB.index(corr) + 2]
-
-                corrres = [[], []]
-                for i in range(len(tmpcorr)):
-                    corrres[i % 2].append(tmpcorr[i])
-                for t in range(int(len(tmpcorr) / 2)):
-                    realsamples[repnum][t].append(corrres[0][t])
-                for t in range(int(len(tmpcorr) / 2)):
-                    imagsamples[repnum][t].append(corrres[1][t])
+                idl_wanted = True
+                if 'idl' in kwargs:
+                    idl_wanted = (cnfg in expected_idl[repnum])
+                    left_idl = left_idl - set([cnfg])
+                if idl_wanted:
+                    cnfgs[repnum].append(cnfg)
+
+                    if corr not in placesBB:
+                        tmpcorr = asascii[1 + 2 * tmax * placesBI.index(corr):1 + 2 * tmax * placesBI.index(corr) + 2 * tmax]
+                    else:
+                        tmpcorr = asascii[1 + 2 * tmax * len(placesBI) + 2 * placesBB.index(corr):1 + 2 * tmax * len(placesBI) + 2 * placesBB.index(corr) + 2]
+
+                    corrres = [[], []]
+                    for i in range(len(tmpcorr)):
+                        corrres[i % 2].append(tmpcorr[i])
+                    for t in range(int(len(tmpcorr) / 2)):
+                        realsamples[repnum][t].append(corrres[0][t])
+                    for t in range(int(len(tmpcorr) / 2)):
+                        imagsamples[repnum][t].append(corrres[1][t])
+            if 'idl' in kwargs:
+                left_idl = list(left_idl)
+                if len(left_idl) > 0:
+                    warnings.warn('Could not find idls ' + str(left_idl) + ' in replikum of file ' + file, UserWarning)
         repnum += 1
-
-    s = "Read correlator " + corr + " from " + str(repnum) + " replika with " + str(len(realsamples[0][t]))
+    s = "Read correlator " + corr + " from " + str(repnum) + " replika with idls" + str(realsamples[0][t])
     for rep in range(1, repnum):
-        s += ", " + str(len(realsamples[rep][t]))
-    s += " samples"
+        s += ", " + str(realsamples[rep][t])
     print(s)
     print("Asserted run parameters:\n T:", tmax, "kappa:", kappa, "csw:", csw, "dF:", dF, "zF:", zF, "bnd:", bnd)
 
     # we have the data now... but we need to re format the whole thing and put it into Corr objects.
 
     compObs = []
```

### Comparing `pyerrors-2.8.0/pyerrors/input/pandas.py` & `pyerrors-2.8.1/pyerrors/input/pandas.py`

 * *Files 4% similar despite different names*

```diff
@@ -167,33 +167,37 @@
     ------
     In case any column of the DataFrame is gzipped it is gunzipped in the process.
     """
     for column in df.select_dtypes(include="object"):
         if isinstance(df[column][0], bytes):
             if df[column][0].startswith(b"\x1f\x8b\x08\x00"):
                 df[column] = df[column].transform(lambda x: gzip.decompress(x).decode('utf-8'))
-        df = df.replace({r'^$': None}, regex=True)
-        i = 0
-        while df[column][i] is None:
-            i += 1
-        if isinstance(df[column][i], str):
-            if '"program":' in df[column][i][:20]:
-                df[column] = df[column].transform(lambda x: import_json_string(x, verbose=False) if x is not None else None)
-                if auto_gamma is True:
-                    if isinstance(df[column][i], list):
-                        df[column].apply(lambda x: [o.gm() if o is not None else x for o in x])
-                    else:
-                        df[column].apply(lambda x: x.gm() if x is not None else x)
+
+        if not all([e is None for e in df[column]]):
+            df[column] = df[column].replace({r'^$': None}, regex=True)
+            i = 0
+            while df[column][i] is None:
+                i += 1
+            if isinstance(df[column][i], str):
+                if '"program":' in df[column][i][:20]:
+                    df[column] = df[column].transform(lambda x: import_json_string(x, verbose=False) if x is not None else None)
+                    if auto_gamma is True:
+                        if isinstance(df[column][i], list):
+                            df[column].apply(lambda x: [o.gm() if o is not None else x for o in x])
+                        else:
+                            df[column].apply(lambda x: x.gm() if x is not None else x)
     return df
 
 
 def _need_to_serialize(col):
     serialize = False
     i = 0
-    while col[i] is None:
+    while i < len(col) and col[i] is None:
         i += 1
+    if i == len(col):
+        return serialize
     if isinstance(col[i], (Obs, Corr)):
         serialize = True
     elif isinstance(col[i], list):
         if all(isinstance(o, Obs) for o in col[i]):
             serialize = True
     return serialize
```

### Comparing `pyerrors-2.8.0/pyerrors/input/sfcf.py` & `pyerrors-2.8.1/pyerrors/input/sfcf.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/input/utils.py` & `pyerrors-2.8.1/pyerrors/input/utils.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/linalg.py` & `pyerrors-2.8.1/pyerrors/linalg.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/misc.py` & `pyerrors-2.8.1/pyerrors/misc.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/mpm.py` & `pyerrors-2.8.1/pyerrors/mpm.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors/obs.py` & `pyerrors-2.8.1/pyerrors/obs.py`

 * *Files 0% similar despite different names*

```diff
@@ -274,15 +274,15 @@
             self.e_n_tauint[e_name][self.e_n_tauint[e_name] <= 0.5] = 0.5 + np.finfo(np.float64).eps
             # hep-lat/0306017 eq. (42)
             self.e_n_dtauint[e_name] = self.e_n_tauint[e_name] * 2 * np.sqrt(np.abs(np.arange(w_max) + 0.5 - self.e_n_tauint[e_name]) / e_N)
             self.e_n_dtauint[e_name][0] = 0.0
 
             def _compute_drho(i):
                 tmp = (self.e_rho[e_name][i + 1:w_max]
-                       + np.concatenate([self.e_rho[e_name][i - 1:None if i - w_max // 2 <= 0 else 2 * (i - w_max // 2):-1],
+                       + np.concatenate([self.e_rho[e_name][i - 1:None if i - w_max // 2 <= 0 else (2 * i - (2 * w_max) // 2):-1],
                                          self.e_rho[e_name][1:max(1, w_max - 2 * i)]])
                        - 2 * self.e_rho[e_name][i] * self.e_rho[e_name][1:w_max - i])
                 self.e_drho[e_name][i] = np.sqrt(np.sum(tmp ** 2) / e_N)
 
             if self.tau_exp[e_name] > 0:
                 _compute_drho(1)
                 texp = self.tau_exp[e_name]
@@ -690,16 +690,20 @@
     def __repr__(self):
         return 'Obs[' + str(self) + ']'
 
     def __str__(self):
         return _format_uncertainty(self.value, self._dvalue)
 
     def __format__(self, format_type):
+        if format_type == "":
+            significance = 2
+        else:
+            significance = int(float(format_type.replace("+", "").replace("-", "")))
         my_str = _format_uncertainty(self.value, self._dvalue,
-                                     significance=int(float(format_type.replace("+", "").replace("-", ""))))
+                                     significance=significance)
         for char in ["+", " "]:
             if format_type.startswith(char):
                 if my_str[0] != "-":
                     my_str = char + my_str
         return my_str
 
     def __hash__(self):
@@ -1517,15 +1521,15 @@
         dvalue += gamma
 
     for e_name in obs1.cov_names:
 
         if e_name not in obs2.cov_names:
             continue
 
-        dvalue += float(np.dot(np.transpose(obs1.covobs[e_name].grad), np.dot(obs1.covobs[e_name].cov, obs2.covobs[e_name].grad)))
+        dvalue += np.dot(np.transpose(obs1.covobs[e_name].grad), np.dot(obs1.covobs[e_name].cov, obs2.covobs[e_name].grad)).item()
 
     return dvalue
 
 
 def import_jackknife(jacks, name, idl=None):
     """Imports jackknife samples and returns an Obs
```

### Comparing `pyerrors-2.8.0/pyerrors/roots.py` & `pyerrors-2.8.1/pyerrors/roots.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/pyerrors.egg-info/PKG-INFO` & `pyerrors-2.8.1/pyerrors.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyerrors
-Version: 2.8.0
+Version: 2.8.1
 Summary: Error propagation and statistical analysis for Monte Carlo simulations
 Home-page: https://github.com/fjosw/pyerrors
 Author: Fabian Joswig
 Author-email: fabian.joswig@ed.ac.uk
 License: MIT
 Project-URL: Documentation, https://fjosw.github.io/pyerrors/pyerrors.html
 Project-URL: Bug Tracker, https://github.com/fjosw/pyerrors/issues
```

### Comparing `pyerrors-2.8.0/pyerrors.egg-info/SOURCES.txt` & `pyerrors-2.8.1/pyerrors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/setup.py` & `pyerrors-2.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         'Changelog' :    'https://github.com/fjosw/pyerrors/blob/master/CHANGELOG.md'
       },
       author='Fabian Joswig',
       author_email='fabian.joswig@ed.ac.uk',
       license="MIT",
       packages=find_packages(),
       python_requires='>=3.7.0',
-      install_requires=['numpy>=1.21', 'autograd>=1.5', 'numdifftools>=0.9.41', 'matplotlib>=3.5', 'scipy>=1.7', 'iminuit>=2.17', 'h5py>=3.8', 'lxml>=4.9', 'python-rapidjson>=1.9', 'pandas>=1.1'],
+      install_requires=['numpy>=1.21,<1.25', 'autograd>=1.5', 'numdifftools>=0.9.41', 'matplotlib>=3.5', 'scipy>=1.7', 'iminuit>=2.17', 'h5py>=3.8', 'lxml>=4.9', 'python-rapidjson>=1.9', 'pandas>=1.1'],
       extras_require={'test': ['pytest', 'pytest-cov', 'pytest-benchmark', 'hypothesis']},
       classifiers=[
           'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: MIT License',
           'Programming Language :: Python :: 3',
           'Programming Language :: Python :: 3.7',
```

### Comparing `pyerrors-2.8.0/tests/benchmark_test.py` & `pyerrors-2.8.1/tests/benchmark_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/correlators_test.py` & `pyerrors-2.8.1/tests/correlators_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/covobs_test.py` & `pyerrors-2.8.1/tests/covobs_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat` & `pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r1.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat` & `pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r2.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat` & `pyerrors-2.8.1/tests/data/openqcd_test/ms5_xsf_T24L16r3.ms5_xsf_dd.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/openqcd_test/openqcd2r1.ms.dat` & `pyerrors-2.8.1/tests/data/openqcd_test/openqcd2r1.ms.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/openqcd_test/openqcd2r1.ms1.dat` & `pyerrors-2.8.1/tests/data/openqcd_test/openqcd2r1.ms1.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/openqcd_test/sfqcdr1.gfms.dat` & `pyerrors-2.8.1/tests/data/openqcd_test/sfqcdr1.gfms.dat`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1` & `pyerrors-2.8.1/tests/data/sfcf_test/broken_data_c/data_c_r0/data_c_r0_n1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.F_V0` & `pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.F_V0`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.f_1` & `pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.f_1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/data_a/data_a_r0.f_A` & `pyerrors-2.8.1/tests/data/sfcf_test/data_a/data_a_r0.f_A`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1` & `pyerrors-2.8.1/tests/data/sfcf_test/data_c/data_c_r0/data_c_r0_n1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0` & `pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/F_V0`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1` & `pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/f_1`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A` & `pyerrors-2.8.1/tests/data/sfcf_test/data_o/test_r0/cfg1/f_A`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/param/out.out` & `pyerrors-2.8.1/tests/data/sfcf_test/param/out.out`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_a` & `pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_a`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_c` & `pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_c`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/data/sfcf_test/param/parameters_o` & `pyerrors-2.8.1/tests/data/sfcf_test/param/parameters_o`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/dirac_test.py` & `pyerrors-2.8.1/tests/dirac_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/fits_test.py` & `pyerrors-2.8.1/tests/fits_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/json_io_test.py` & `pyerrors-2.8.1/tests/json_io_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/linalg_test.py` & `pyerrors-2.8.1/tests/linalg_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/misc_test.py` & `pyerrors-2.8.1/tests/misc_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/obs_test.py` & `pyerrors-2.8.1/tests/obs_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -758,19 +758,30 @@
     with pytest.raises(Exception):
         my_obs.gm()
 
     # check cases where tau is large compared to the chain length
     N = 15
     for i in range(10):
         arr = np.random.normal(1, .2, size=N)
-        for rho in .1 * np.arange(20):
+        for rho in .05 * np.arange(20):
             carr = gen_autocorrelated_array(arr, rho)
             a = pe.Obs([carr], ['a'])
             a.gm()
 
+    arr = np.random.normal(1, .2, size=999)
+    carr = gen_autocorrelated_array(arr, .8)
+    o = pe.Obs([carr], ['test'])
+    o.gamma_method()
+    no = np.NaN * o
+    no.gamma_method()
+    o.idl['test'] = range(1, 1998, 2)
+    o.gamma_method()
+    no = np.NaN * o
+    no.gamma_method()
+
 
 def test_irregular_gapped_dtauint():
     my_idl = list(range(0, 5010, 10))
     my_idl.remove(400)
     my_idl2 = list(range(0, 501, 1))
     my_idl2.remove(40)
 
@@ -1092,15 +1103,15 @@
         np.arange(1, 101),
         [1, 2, 3, 5, 6, 7, 9, 12],
         [7],
     ]
     for idx_new in idl:
         new = pe.obs._reduce_deltas(deltas, idx_old, idx_new)
         print(new)
-        assert(np.alltrue([float(i) for i in idx_new] == new))
+        assert(np.all([float(i) for i in idx_new] == new))
 
 
 def test_cobs_array():
     cobs = pe.Obs([np.random.normal(1.0, 0.1, 100)], ['t']) * (1 + 2j)
     np.identity(4) + cobs
     cobs + np.identity(4)
     np.identity(4) - cobs
@@ -1259,7 +1270,15 @@
     pe.obs._format_uncertainty(np.NaN, np.inf)
 
 def test_format():
     o1 = pe.pseudo_Obs(0.348, 0.0123, "test")
     assert o1.__format__("+3") == '+0.3480(123)'
     assert o1.__format__("+2") == '+0.348(12)'
     assert o1.__format__(" 2") == ' 0.348(12)'
+
+def test_f_string_obs():
+    o1 = pe.pseudo_Obs(0.348, 0.0123, "test")
+    print(f"{o1}")
+    print(f"{o1:3}")
+    print(f"{o1:+3}")
+    print(f"{o1:-1}")
+    print(f"{o1: 8}")
```

### Comparing `pyerrors-2.8.0/tests/openQCD_in_test.py` & `pyerrors-2.8.1/tests/openQCD_in_test.py`

 * *Files 26% similar despite different names*

```diff
@@ -117,15 +117,15 @@
     with pytest.raises(Exception):
         pe.input.openQCD.read_gf_coupling(path, prefix, c=0.35)
     with pytest.raises(Exception):
         pe.input.openQCD.read_gf_coupling(path, prefix, c=0.3, Zeuthen_flow=False)
 
 
 def test_read_ms5_xsf():
-    path = './tests//data/openqcd_test/'
+    path = './tests/data/openqcd_test/'
     prefix = "ms5_xsf_T24L16"
     corr = "gA"
     qc = 'dd'
 
     c = pe.input.openQCD.read_ms5_xsf(path, prefix, qc, corr)
 
     assert c.real[12].names == ['ms5_xsf_T24L16|r1', 'ms5_xsf_T24L16|r2', 'ms5_xsf_T24L16|r3']
@@ -141,14 +141,45 @@
         pe.input.openQCD.read_ms5_xsf(path, prefix, fqc, corr)
 
     fcorr = "gX"
     with pytest.raises(Exception):
         pe.input.openQCD.read_ms5_xsf(path, prefix, qc, fcorr)
 
 
+def test_read_ms5_xsf_idl():
+    path = './tests/data/openqcd_test/'
+    prefix = "ms5_xsf_T24L16"
+    corr = "gA"
+    qc = 'dd'
+
+    c = pe.input.openQCD.read_ms5_xsf(path, prefix, qc, corr, idl=[range(1, 6), range(1, 7), range(1, 8)])
+
+    assert c.real[12].names == ['ms5_xsf_T24L16|r1', 'ms5_xsf_T24L16|r2', 'ms5_xsf_T24L16|r3']
+
+    assert (c.real[12].shape['ms5_xsf_T24L16|r1'] == 5)
+    assert (c.real[12].shape['ms5_xsf_T24L16|r2'] == 6)
+    assert (c.real[12].shape['ms5_xsf_T24L16|r3'] == 7)
+
+    assert (c.real[12].idl['ms5_xsf_T24L16|r1'] == range(1, 6))
+    assert (c.real[12].idl['ms5_xsf_T24L16|r2'] == range(1, 7))
+    assert (c.real[12].idl['ms5_xsf_T24L16|r3'] == range(1, 8))
+
+    c = pe.input.openQCD.read_ms5_xsf(path, prefix, qc, corr, idl=[range(1, 11, 2), range(1, 11, 2), range(1, 11, 2)])
+
+    assert c.real[12].names == ['ms5_xsf_T24L16|r1', 'ms5_xsf_T24L16|r2', 'ms5_xsf_T24L16|r3']
+
+    assert (c.real[12].shape['ms5_xsf_T24L16|r1'] == 5)
+    assert (c.real[12].shape['ms5_xsf_T24L16|r2'] == 5)
+    assert (c.real[12].shape['ms5_xsf_T24L16|r3'] == 5)
+
+    assert (c.real[12].idl['ms5_xsf_T24L16|r1'] == range(1, 11, 2))
+    assert (c.real[12].idl['ms5_xsf_T24L16|r2'] == range(1, 11, 2))
+    assert (c.real[12].idl['ms5_xsf_T24L16|r3'] == range(1, 11, 2))
+
+
 def test_find_files():
     path = './tests/data/openqcd_test/'
     prefix = "ms5_xsf_T24L16"
     qc = 'dd'
 
     files = pe.input.openQCD._find_files(path, prefix, "ms5_xsf_" + qc, "dat")
     assert (len(files) == 3)
```

### Comparing `pyerrors-2.8.0/tests/pandas_test.py` & `pyerrors-2.8.1/tests/pandas_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -169,14 +169,30 @@
     pe.input.pandas.to_sql(my_df, 'test', (tmp_path / 'test.db').as_posix(), gz=gz)
     reconstructed_df = pe.input.pandas.read_sql('SELECT * FROM test', (tmp_path / 'test.db').as_posix(), auto_gamma=True)
     assert reconstructed_df.loc[1, "Obs1"] is None
     assert np.all(reconstructed_df.loc[0] == my_df.loc[0])
     assert np.all(reconstructed_df.loc[2:] == my_df.loc[2:])
 
 
+def test_null_col_df_gzsql_export_import(tmp_path):
+    my_dict = {"int": 1,
+               "float": -0.01,
+               "Noneval": None,
+               "Obs1": pe.pseudo_Obs(87, 21, "test_ensemble"),
+               "Obs2": pe.pseudo_Obs(-87, 21, "test_ensemble2")}
+    my_df = pd.DataFrame([my_dict] * 4)
+    pe.input.pandas.to_sql(my_df, 'test', (tmp_path / 'test.db').as_posix(), gz=True)
+    reconstructed_df = pe.input.pandas.read_sql('SELECT * FROM test', (tmp_path / 'test.db').as_posix(), auto_gamma=True)
+    assert np.all(reconstructed_df["int"] == my_df["int"])
+    assert np.all(reconstructed_df["float"] == my_df["float"])
+    assert np.all([e is None for e in reconstructed_df["Noneval"]])
+    assert np.all(reconstructed_df["Obs1"] == my_df["Obs1"])
+    assert np.all(reconstructed_df["Obs2"] == my_df["Obs2"])
+
+
 def test_df_Corr(tmp_path):
 
     my_corr = pe.Corr([pe.pseudo_Obs(-0.48, 0.04, "test"), pe.pseudo_Obs(-0.154, 0.03, "test")])
 
     my_dict = {"int": 1,
                "float": -0.01,
                "Corr": my_corr}
```

### Comparing `pyerrors-2.8.0/tests/roots_test.py` & `pyerrors-2.8.1/tests/roots_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/sfcf_in_test.py` & `pyerrors-2.8.1/tests/sfcf_in_test.py`

 * *Files identical despite different names*

### Comparing `pyerrors-2.8.0/tests/utils_in_test.py` & `pyerrors-2.8.1/tests/utils_in_test.py`

 * *Files identical despite different names*

