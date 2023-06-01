# Comparing `tmp/synphot-1.2.0.tar.gz` & `tmp/synphot-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synphot-1.2.0.tar", last modified: Mon Mar 20 20:31:46 2023, max compression
+gzip compressed data, was "synphot-1.2.1.tar", last modified: Thu Jun  1 21:19:06 2023, max compression
```

## Comparing `synphot-1.2.0.tar` & `synphot-1.2.1.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.596798 synphot-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-03-20 20:31:27.000000 synphot-1.2.0/.bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.584798 synphot-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.584798 synphot-1.2.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.584798 synphot-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/workflows/open_actions.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/workflows/predeps_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-03-20 20:31:27.000000 synphot-1.2.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-03-20 20:31:27.000000 synphot-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-20 20:31:27.000000 synphot-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-03-20 20:31:27.000000 synphot-1.2.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-20 20:31:27.000000 synphot-1.2.0/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-03-20 20:31:27.000000 synphot-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-03-20 20:31:27.000000 synphot-1.2.0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-03-20 20:31:27.000000 synphot-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-20 20:31:46.596798 synphot-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-20 20:31:27.000000 synphot-1.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-03-20 20:31:27.000000 synphot-1.2.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.588798 synphot-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.588798 synphot-1.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.580798 synphot-1.2.0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.588798 synphot-1.2.0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.588798 synphot-1.2.0/docs/synphot/
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/bandpass.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/c_ext.rst
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/config.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/filter_par.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/formulae.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/from_pysyn_iraf.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.588798 synphot-1.2.0/docs/synphot/images/
--rw-r--r--   0 runner    (1001) docker     (123)   142118 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/images/VegaPhotomSys.png
--rw-r--r--   0 runner    (1001) docker     (123)    49541 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/images/bb5000_lmcavg.png
--rw-r--r--   0 runner    (1001) docker     (123)    49043 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/images/bb5000_renorm.png
--rw-r--r--   0 runner    (1001) docker     (123)    32169 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/images/johnson_bi.png
--rw-r--r--   0 runner    (1001) docker     (123)    42702 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/images/tutorial_em_line.png
--rw-r--r--   0 runner    (1001) docker     (123)    58060 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/images/tutorial_fit_ab.png
--rw-r--r--   0 runner    (1001) docker     (123)    41626 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/images/vega_spec.png
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/observation.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28630 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/overview.rst
--rw-r--r--   0 runner    (1001) docker     (123)    18778 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/spectrum.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-03-20 20:31:27.000000 synphot-1.2.0/docs/synphot/units.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.588798 synphot-1.2.0/licenses/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-20 20:31:27.000000 synphot-1.2.0/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-03-20 20:31:27.000000 synphot-1.2.0/licenses/TYNT_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-03-20 20:31:27.000000 synphot-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-03-20 20:31:46.600798 synphot-1.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1546 2023-03-20 20:31:27.000000 synphot-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.592798 synphot-1.2.0/synphot/
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/binning.py
--rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/blackbody.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.592798 synphot-1.2.0/synphot/filter_parameterization/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/filter_parameterization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/filter_parameterization/filter_fft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.592798 synphot-1.2.0/synphot/filter_parameterization/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/filter_parameterization/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.592798 synphot-1.2.0/synphot/filter_parameterization/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/filter_parameterization/tests/data/fft_test_data.fits
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/filter_parameterization/tests/test_filter_fft.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.592798 synphot-1.2.0/synphot/include/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/include/synphot_utils.h
--rw-r--r--   0 runner    (1001) docker     (123)    27606 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/models.py
--rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/reddening.py
--rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/specio.py
--rw-r--r--   0 runner    (1001) docker     (123)    69390 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.592798 synphot-1.2.0/synphot/src/
--rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/src/synphot_utils.c
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.596798 synphot-1.2.0/synphot/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.596798 synphot-1.2.0/synphot/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   521280 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/cos_fuv_g130m_c1309_psa.fits
--rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/grw_70d5824_stisnic_005.fits
--rw-r--r--   0 runner    (1001) docker     (123)    86400 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/hst_acs_hrc_f555w.fits
--rw-r--r--   0 runner    (1001) docker     (123)    86400 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/hst_acs_hrc_f555w_x_grw70d5824.fits
--rw-r--r--   0 runner    (1001) docker     (123)   118080 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/hst_acs_hrc_f850lp.fits
--rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/k93_4500_0_5_rn_box.fits
--rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/milkyway_diffuse_001.fits
--rw-r--r--   0 runner    (1001) docker     (123)    61614 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/qso_template_001.dat
--rw-r--r--   0 runner    (1001) docker     (123)    88008 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/stis_fuv_f25ndq2_binset.bin
--rw-r--r--   0 runner    (1001) docker     (123)    46080 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/stis_fuv_f25ndq2_mjd58300_0822774.fits
--rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/us7.txt
--rw-r--r--   0 runner    (1001) docker     (123)    89280 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/data/wfc3_ir_g141_src_003_th.fits
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_blackbody.py
--rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_integrator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_reddening.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_specio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_spectrum_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_spectrum_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25824 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_spectrum_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/thermal.py
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    10429 2023-03-20 20:31:27.000000 synphot-1.2.0/synphot/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-20 20:31:46.000000 synphot-1.2.0/synphot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 20:31:46.592798 synphot-1.2.0/synphot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-20 20:31:46.000000 synphot-1.2.0/synphot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-03-20 20:31:46.000000 synphot-1.2.0/synphot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 20:31:46.000000 synphot-1.2.0/synphot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 20:31:46.000000 synphot-1.2.0/synphot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-20 20:31:46.000000 synphot-1.2.0/synphot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-20 20:31:46.000000 synphot-1.2.0/synphot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-03-20 20:31:27.000000 synphot-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.584549 synphot-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-01 21:18:44.000000 synphot-1.2.1/.bandit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.568548 synphot-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.572548 synphot-1.2.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.572548 synphot-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/workflows/open_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/workflows/predeps_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-06-01 21:18:44.000000 synphot-1.2.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-01 21:18:44.000000 synphot-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-01 21:18:44.000000 synphot-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-06-01 21:18:44.000000 synphot-1.2.1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-01 21:18:44.000000 synphot-1.2.1/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3207 2023-06-01 21:18:44.000000 synphot-1.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-06-01 21:18:44.000000 synphot-1.2.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-01 21:18:44.000000 synphot-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-01 21:19:06.584549 synphot-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-01 21:18:44.000000 synphot-1.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-01 21:18:44.000000 synphot-1.2.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.572548 synphot-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4724 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.572548 synphot-1.2.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    19012 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.568548 synphot-1.2.1/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.572548 synphot-1.2.1/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12585 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4513 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.572548 synphot-1.2.1/docs/synphot/
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/bandpass.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/c_ext.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/filter_par.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11039 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/formulae.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18230 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/from_pysyn_iraf.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.576549 synphot-1.2.1/docs/synphot/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   142118 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/images/VegaPhotomSys.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49541 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/images/bb5000_lmcavg.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49043 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/images/bb5000_renorm.png
+-rw-r--r--   0 runner    (1001) docker     (123)    32169 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/images/johnson_bi.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42702 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/images/tutorial_em_line.png
+-rw-r--r--   0 runner    (1001) docker     (123)    58060 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/images/tutorial_fit_ab.png
+-rw-r--r--   0 runner    (1001) docker     (123)    41626 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/images/vega_spec.png
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/observation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28630 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    18778 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/spectrum.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9992 2023-06-01 21:18:44.000000 synphot-1.2.1/docs/synphot/units.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.576549 synphot-1.2.1/licenses/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-01 21:18:44.000000 synphot-1.2.1/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-01 21:18:44.000000 synphot-1.2.1/licenses/TYNT_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-01 21:18:44.000000 synphot-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-06-01 21:19:06.588549 synphot-1.2.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1546 2023-06-01 21:18:44.000000 synphot-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.576549 synphot-1.2.1/synphot/
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16408 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9377 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/blackbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.580549 synphot-1.2.1/synphot/filter_parameterization/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/filter_parameterization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/filter_parameterization/filter_fft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.580549 synphot-1.2.1/synphot/filter_parameterization/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/filter_parameterization/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.580549 synphot-1.2.1/synphot/filter_parameterization/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    11520 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/filter_parameterization/tests/data/fft_test_data.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/filter_parameterization/tests/test_filter_fft.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.580549 synphot-1.2.1/synphot/include/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/include/synphot_utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27606 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/reddening.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12708 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/specio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69390 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.580549 synphot-1.2.1/synphot/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/src/synphot_utils.c
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.580549 synphot-1.2.1/synphot/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.584549 synphot-1.2.1/synphot/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   521280 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/cos_fuv_g130m_c1309_psa.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   120960 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/grw_70d5824_stisnic_005.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    86400 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/hst_acs_hrc_f555w.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    86400 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/hst_acs_hrc_f555w_x_grw70d5824.fits
+-rw-r--r--   0 runner    (1001) docker     (123)   118080 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/hst_acs_hrc_f850lp.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    25920 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/k93_4500_0_5_rn_box.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     8640 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/milkyway_diffuse_001.fits
+-rw-r--r--   0 runner    (1001) docker     (123)    61614 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/qso_template_001.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    88008 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/stis_fuv_f25ndq2_binset.bin
+-rw-r--r--   0 runner    (1001) docker     (123)    46080 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/stis_fuv_f25ndq2_mjd58300_0822774.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     8988 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/us7.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    89280 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/data/wfc3_ir_g141_src_003_th.fits
+-rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_blackbody.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7275 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18003 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_reddening.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_specio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_spectrum_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15792 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_spectrum_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25824 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_spectrum_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10421 2023-06-01 21:18:44.000000 synphot-1.2.1/synphot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-01 21:19:06.000000 synphot-1.2.1/synphot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 21:19:06.580549 synphot-1.2.1/synphot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-01 21:19:06.000000 synphot-1.2.1/synphot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-06-01 21:19:06.000000 synphot-1.2.1/synphot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:19:06.000000 synphot-1.2.1/synphot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 21:19:06.000000 synphot-1.2.1/synphot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-01 21:19:06.000000 synphot-1.2.1/synphot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 21:19:06.000000 synphot-1.2.1/synphot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-01 21:18:44.000000 synphot-1.2.1/tox.ini
```

### Comparing `synphot-1.2.0/.github/ISSUE_TEMPLATE/bug_report.md` & `synphot-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/.github/ISSUE_TEMPLATE/feature_request.md` & `synphot-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/.github/ISSUE_TEMPLATE/question.md` & `synphot-1.2.1/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/.github/PULL_REQUEST_TEMPLATE.md` & `synphot-1.2.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/.github/labeler.yml` & `synphot-1.2.1/.github/labeler.yml`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/.github/workflows/ci_workflows.yml` & `synphot-1.2.1/.github/workflows/ci_workflows.yml`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/.github/workflows/codeql-analysis.yml` & `synphot-1.2.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/.github/workflows/open_actions.yml` & `synphot-1.2.1/.github/workflows/open_actions.yml`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/.github/workflows/predeps_workflow.yml` & `synphot-1.2.1/.github/workflows/predeps_workflow.yml`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/.github/workflows/publish-to-pypi.yml` & `synphot-1.2.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/.gitignore` & `synphot-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/CHANGES.rst` & `synphot-1.2.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+1.2.1 (2023-06-01)
+==================
+
+- Compatibility with ``numpy`` 1.25. [#356]
+
 1.2.0 (2023-03-20)
 ==================
 
 - New ``filter_parameterization`` subpackage to handle filter parameterization,
   adapted from ``tynt`` package written by Brett Morris. [#257]
 
 - OBMAG and VEGAMAG are no longer interchangeable. [#331]
```

### Comparing `synphot-1.2.0/CODE_OF_CONDUCT.md` & `synphot-1.2.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/LICENSE.rst` & `synphot-1.2.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/PKG-INFO` & `synphot-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synphot
-Version: 1.2.0
+Version: 1.2.1
 Summary: Synthetic photometry
 Home-page: https://www.github.com/spacetelescope/synphot_refactor
 Author: STScI
 Author-email: help@stsci.edu
 License: BSD
 Keywords: astronomy,astrophysics,synthetic,photometry
 Classifier: Intended Audience :: Science/Research
```

### Comparing `synphot-1.2.0/README.rst` & `synphot-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/conftest.py` & `synphot-1.2.1/conftest.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/Makefile` & `synphot-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/_static/stsci_logo.png` & `synphot-1.2.1/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/conf.py` & `synphot-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/index.rst` & `synphot-1.2.1/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -245,15 +245,15 @@
     >>> bp = SpectralElement(Box1D, amplitude=1, x_0=4000, width=2000)
 
 Normalize the source spectrum to 1 Jy in a given box bandpass and
 integrate it::
 
     >>> sp_rn = sp.normalize(1 * u.Jy, band=bp)
     >>> sp_rn.integrate()  # doctest: +FLOAT_CMP
-    <Quantity 12540.4613615 ph / (cm2 s)>
+    <Quantity 12540.4613615 ph / (s cm2)>
 
 Create an observation by passing the redshifted and normalized source spectrum
 through the box bandpass::
 
     >>> from synphot import Observation
     >>> obs = Observation(sp_rn, bp)
```

### Comparing `synphot-1.2.0/docs/make.bat` & `synphot-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/bandpass.rst` & `synphot-1.2.1/docs/synphot/bandpass.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/filter_par.rst` & `synphot-1.2.1/docs/synphot/filter_par.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/formulae.rst` & `synphot-1.2.1/docs/synphot/formulae.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/from_pysyn_iraf.rst` & `synphot-1.2.1/docs/synphot/from_pysyn_iraf.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/images/VegaPhotomSys.png` & `synphot-1.2.1/docs/synphot/images/VegaPhotomSys.png`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/images/bb5000_lmcavg.png` & `synphot-1.2.1/docs/synphot/images/bb5000_lmcavg.png`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/images/bb5000_renorm.png` & `synphot-1.2.1/docs/synphot/images/bb5000_renorm.png`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/images/johnson_bi.png` & `synphot-1.2.1/docs/synphot/images/johnson_bi.png`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/images/tutorial_em_line.png` & `synphot-1.2.1/docs/synphot/images/tutorial_em_line.png`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/images/tutorial_fit_ab.png` & `synphot-1.2.1/docs/synphot/images/tutorial_fit_ab.png`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/images/vega_spec.png` & `synphot-1.2.1/docs/synphot/images/vega_spec.png`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/observation.rst` & `synphot-1.2.1/docs/synphot/observation.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/overview.rst` & `synphot-1.2.1/docs/synphot/overview.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/docs/synphot/spectrum.rst` & `synphot-1.2.1/docs/synphot/spectrum.rst`

 * *Files 2% similar despite different names*

```diff
@@ -195,24 +195,24 @@
 
     >>> from astropy import units as u
     >>> from synphot import SourceSpectrum, units, conf
     >>> from synphot.models import GaussianFlux1D
     >>> sp = SourceSpectrum(GaussianFlux1D, mean=6000*u.AA, fwhm=10*u.AA,
     ...                     total_flux=1*(u.erg/(u.cm**2 * u.s)))
     >>> sp.integrate()  # doctest: +FLOAT_CMP
-    <Quantity 3.02046758e+11 ph / (cm2 s)>
+    <Quantity 3.02046758e+11 ph / (s cm2)>
     >>> with conf.set_temp('default_integrator', 'analytical'):
     ...     print(f'{repr(sp.integrate())}')  # doctest: +FLOAT_CMP
-    <Quantity 3.02046994e+11 ph / (cm2 s)>
+    <Quantity 3.02046994e+11 ph / (s cm2)>
     >>> sp.integrate(integration_type='analytical')  # doctest: +FLOAT_CMP
-    <Quantity 3.02046994e+11 ph / (cm2 s)>
+    <Quantity 3.02046994e+11 ph / (s cm2)>
     >>> sp.integrate(flux_unit=units.FLAM)  # doctest: +FLOAT_CMP
-    <Quantity 0.99999972 erg / (cm2 s)>
+    <Quantity 0.99999972 erg / (s cm2)>
     >>> sp.integrate(flux_unit=units.FLAM, integration_type='analytical')  # doctest: +FLOAT_CMP
-    <Quantity 1. erg / (cm2 s)>
+    <Quantity 1. erg / (s cm2)>
 
 
 .. _synphot-empirical-source:
 
 Arrays
 ------
```

### Comparing `synphot-1.2.0/docs/synphot/tutorials.rst` & `synphot-1.2.1/docs/synphot/tutorials.rst`

 * *Files 2% similar despite different names*

```diff
@@ -117,18 +117,18 @@
     >>> ccm89_model = CCM89(Rv=3.1)
     >>> wav = np.arange(0.1, 3, 0.001) * u.micron
     >>> ebv = 0.1  # E(B-V)
     >>> redlaw = ReddeningLaw(ccm89_model)
     >>> extcurve = redlaw.extinction_curve(ebv, wavelengths=wav)
     >>> bb = SourceSpectrum(BlackBodyNorm1D, temperature=5000 * u.K)
     >>> bb.integrate()  # doctest: +FLOAT_CMP
-    <Quantity 9.31004974 ph / (cm2 s)>
+    <Quantity 9.31004028 ph / (s cm2)>
     >>> sp = bb * extcurve
     >>> sp.integrate()  # doctest: +FLOAT_CMP
-    <Quantity 8.27106961 ph / (cm2 s)>
+    <Quantity 8.27106961 ph / (s cm2)>
 
 
 .. _tutorial_fit_ew:
 
 Fitting, Equivalent Width
 -------------------------
```

### Comparing `synphot-1.2.0/docs/synphot/units.rst` & `synphot-1.2.1/docs/synphot/units.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/licenses/TYNT_LICENSE.txt` & `synphot-1.2.1/licenses/TYNT_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/setup.cfg` & `synphot-1.2.1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool:pytest]
 minversion = 5
 testpaths = "synphot" "docs"
 norecursedirs = build docs/_build synphot/src
 astropy_header = true
 doctest_plus = enabled
 doctest_subpackage_requires = 
-	docs/index.rst = astropy<5.3
-	docs/synphot/spectrum.rst = astropy<5.3
+	docs/index.rst = astropy>=5.3
+	docs/synphot/spectrum.rst = astropy>=5.3
+	docs/synphot/tutorials.rst = astropy>=5.3
 text_file_format = rst
 addopts = --doctest-rst --import-mode=append
 xfail_strict = true
 filterwarnings = 
 	error
 	ignore:can't resolve package from __spec__
 	ignore:numpy\.ndarray size changed:RuntimeWarning
```

### Comparing `synphot-1.2.0/setup.py` & `synphot-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/__init__.py` & `synphot-1.2.1/synphot/__init__.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/binning.py` & `synphot-1.2.1/synphot/binning.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/blackbody.py` & `synphot-1.2.1/synphot/blackbody.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/compat.py` & `synphot-1.2.1/synphot/compat.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/config.py` & `synphot-1.2.1/synphot/config.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/exceptions.py` & `synphot-1.2.1/synphot/exceptions.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/filter_parameterization/filter_fft.py` & `synphot-1.2.1/synphot/filter_parameterization/filter_fft.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/filter_parameterization/tests/data/fft_test_data.fits` & `synphot-1.2.1/synphot/filter_parameterization/tests/data/fft_test_data.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/filter_parameterization/tests/test_filter_fft.py` & `synphot-1.2.1/synphot/filter_parameterization/tests/test_filter_fft.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/include/synphot_utils.h` & `synphot-1.2.1/synphot/include/synphot_utils.h`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/models.py` & `synphot-1.2.1/synphot/models.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/observation.py` & `synphot-1.2.1/synphot/observation.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/reddening.py` & `synphot-1.2.1/synphot/reddening.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/specio.py` & `synphot-1.2.1/synphot/specio.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/spectrum.py` & `synphot-1.2.1/synphot/spectrum.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/src/synphot_utils.c` & `synphot-1.2.1/synphot/src/synphot_utils.c`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/cos_fuv_g130m_c1309_psa.fits` & `synphot-1.2.1/synphot/tests/data/cos_fuv_g130m_c1309_psa.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/grw_70d5824_stisnic_005.fits` & `synphot-1.2.1/synphot/tests/data/grw_70d5824_stisnic_005.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/hst_acs_hrc_f555w.fits` & `synphot-1.2.1/synphot/tests/data/hst_acs_hrc_f555w.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/hst_acs_hrc_f555w_x_grw70d5824.fits` & `synphot-1.2.1/synphot/tests/data/hst_acs_hrc_f555w_x_grw70d5824.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/hst_acs_hrc_f850lp.fits` & `synphot-1.2.1/synphot/tests/data/hst_acs_hrc_f850lp.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/k93_4500_0_5_rn_box.fits` & `synphot-1.2.1/synphot/tests/data/k93_4500_0_5_rn_box.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/milkyway_diffuse_001.fits` & `synphot-1.2.1/synphot/tests/data/milkyway_diffuse_001.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/qso_template_001.dat` & `synphot-1.2.1/synphot/tests/data/qso_template_001.dat`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/stis_fuv_f25ndq2_binset.bin` & `synphot-1.2.1/synphot/tests/data/stis_fuv_f25ndq2_binset.bin`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/stis_fuv_f25ndq2_mjd58300_0822774.fits` & `synphot-1.2.1/synphot/tests/data/stis_fuv_f25ndq2_mjd58300_0822774.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/us7.txt` & `synphot-1.2.1/synphot/tests/data/us7.txt`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/data/wfc3_ir_g141_src_003_th.fits` & `synphot-1.2.1/synphot/tests/data/wfc3_ir_g141_src_003_th.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_binning.py` & `synphot-1.2.1/synphot/tests/test_binning.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_blackbody.py` & `synphot-1.2.1/synphot/tests/test_blackbody.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_integrator.py` & `synphot-1.2.1/synphot/tests/test_integrator.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_models.py` & `synphot-1.2.1/synphot/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_observation.py` & `synphot-1.2.1/synphot/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_reddening.py` & `synphot-1.2.1/synphot/tests/test_reddening.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_specio.py` & `synphot-1.2.1/synphot/tests/test_specio.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_spectrum_bandpass.py` & `synphot-1.2.1/synphot/tests/test_spectrum_bandpass.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_spectrum_misc.py` & `synphot-1.2.1/synphot/tests/test_spectrum_misc.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_spectrum_source.py` & `synphot-1.2.1/synphot/tests/test_spectrum_source.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_thermal.py` & `synphot-1.2.1/synphot/tests/test_thermal.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_units.py` & `synphot-1.2.1/synphot/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/tests/test_utils.py` & `synphot-1.2.1/synphot/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/thermal.py` & `synphot-1.2.1/synphot/thermal.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/units.py` & `synphot-1.2.1/synphot/units.py`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/synphot/utils.py` & `synphot-1.2.1/synphot/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,16 +118,16 @@
     if np.any(wave <= 0):
         raise exceptions.ZeroWavelength(
             'Negative or zero wavelength occurs in wavelength array',
             rows=np.where(wave <= 0)[0])
 
     # Check for monotonicity
     sorted_wave = np.sort(wave)
-    if not np.alltrue(sorted_wave == wave):
-        if np.alltrue(sorted_wave[::-1] == wave):
+    if not np.all(sorted_wave == wave):
+        if np.all(sorted_wave[::-1] == wave):
             pass  # Monotonic descending is allowed
         else:
             raise exceptions.UnsortedWavelength(
                 'Wavelength array is not monotonic',
                 rows=np.where(sorted_wave != wave)[0])
 
     # Check for duplicate values
```

### Comparing `synphot-1.2.0/synphot.egg-info/PKG-INFO` & `synphot-1.2.1/synphot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synphot
-Version: 1.2.0
+Version: 1.2.1
 Summary: Synthetic photometry
 Home-page: https://www.github.com/spacetelescope/synphot_refactor
 Author: STScI
 Author-email: help@stsci.edu
 License: BSD
 Keywords: astronomy,astrophysics,synthetic,photometry
 Classifier: Intended Audience :: Science/Research
```

### Comparing `synphot-1.2.0/synphot.egg-info/SOURCES.txt` & `synphot-1.2.1/synphot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synphot-1.2.0/tox.ini` & `synphot-1.2.1/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,14 @@
     oldestdeps: astropy==4.3.*
 
     # The devdeps factor is intended to be used to install the latest developer version
     # or nightly wheel of key dependencies.
     devdeps: git+https://github.com/astropy/specutils.git@main#egg=specutils
 
     cov: pytest-cov
-    cov: codecov
 
 extras =
     test
     alldeps: all
 
 commands =
     devdeps: pip install -U -i https://pypi.anaconda.org/astropy/simple astropy --pre
```

