# Comparing `tmp/pyikarus-0.3.3.dev20230601114417.tar.gz` & `tmp/pyikarus-0.3.3.dev20230601194812.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.3.dev20230601114417.tar", last modified: Thu Jun  1 11:44:17 2023, max compression
+gzip compressed data, was "pyikarus-0.3.3.dev20230601194812.tar", last modified: Thu Jun  1 19:48:13 2023, max compression
```

## Comparing `pyikarus-0.3.3.dev20230601114417.tar` & `pyikarus-0.3.3.dev20230601194812.tar`

### file list

```diff
@@ -1,331 +1,331 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.967877 pyikarus-0.3.3.dev20230601114417/
--rw-r--r--   0 root         (0) root         (0)      312 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.bettercodehub.yml
--rw-r--r--   0 root         (0) root         (0)     1300 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.clang-format
--rw-r--r--   0 root         (0) root         (0)     1017 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.cmake-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.911876 pyikarus-0.3.3.dev20230601114417/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.919876 pyikarus-0.3.3.dev20230601114417/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      460 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      615 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/codespell.yml
--rw-r--r--   0 root         (0) root         (0)     1034 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/createDockerContainer.yml
--rw-r--r--   0 root         (0) root         (0)     5615 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/createRelease.yml
--rw-r--r--   0 root         (0) root         (0)     1834 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/debian-coverage.yml
--rw-r--r--   0 root         (0) root         (0)     2612 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/debian.yml
--rw-r--r--   0 root         (0) root         (0)     2042 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/ghpages.yml
--rw-r--r--   0 root         (0) root         (0)     1712 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/releasePythonPackage.yml
--rw-r--r--   0 root         (0) root         (0)      314 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/reuseLint.yml
--rw-r--r--   0 root         (0) root         (0)     3335 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/runExamples.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/.github/workflows/scripts/
--rw-r--r--   0 root         (0) root         (0)     3071 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/scripts/release.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/style.yml
--rw-r--r--   0 root         (0) root         (0)      482 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/.reuse/
--rw-r--r--   0 root         (0) root         (0)      661 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.reuse/dep5
--rw-r--r--   0 root         (0) root         (0)     3707 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1251 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5335 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)      784 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/LICENSES/
--rw-r--r--   0 root         (0) root         (0)    18375 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 root         (0) root         (0)     7048 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)    42098 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 root         (0) root         (0)     1078 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSES/MIT.txt
--rw-r--r--   0 root         (0) root         (0)    16727 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSES/MPL-2.0.txt
--rw-r--r--   0 root         (0) root         (0)     3732 2023-06-01 11:44:17.967877 pyikarus-0.3.3.dev20230601114417/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3321 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/cmake/
--rw-r--r--   0 root         (0) root         (0)      184 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      973 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/cmake/FormatTarget/
--rw-r--r--   0 root         (0) root         (0)     1807 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      683 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/AddMatplotppFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      691 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/AddSpdlogFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      325 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      379 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/IkarusMacros.cmake
--rw-r--r--   0 root         (0) root         (0)     2040 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/tools.cmake
--rw-r--r--   0 root         (0) root         (0)      148 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/codecov.yml
--rw-r--r--   0 root         (0) root         (0)      121 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/codespellignore
--rw-r--r--   0 root         (0) root         (0)     1588 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/docs/BuildLocally/
--rw-r--r--   0 root         (0) root         (0)      439 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/BuildLocally/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      333 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/docs/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     1136 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rw-r--r--   0 root         (0) root         (0)     6961 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/literature.bib
--rw-r--r--   0 root         (0) root         (0)      117 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/literature.bib.license
--rw-r--r--   0 root         (0) root         (0)     1271 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/mkdocs-macros.py
--rw-r--r--   0 root         (0) root         (0)      398 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/mkdocs.insiders.yml
--rw-r--r--   0 root         (0) root         (0)     5042 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.911876 pyikarus-0.3.3.dev20230601114417/docs/overrides/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/docs/overrides/partials/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/overrides/partials/comments.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/docs/website/
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/.meta.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/
--rw-r--r--   0 root         (0) root         (0)     4710 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/assembler.md
--rw-r--r--   0 root         (0) root         (0)     6387 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/controlRoutines.md
--rw-r--r--   0 root         (0) root         (0)     2024 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/dirichletBCs.md
--rw-r--r--   0 root         (0) root         (0)     3237 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/feRequirements.md
--rw-r--r--   0 root         (0) root         (0)    12894 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/finiteElements.md
--rw-r--r--   0 root         (0) root         (0)     2745 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/grids.md
--rw-r--r--   0 root         (0) root         (0)     4121 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/index.md
--rw-r--r--   0 root         (0) root         (0)     4932 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/localBasis.md
--rw-r--r--   0 root         (0) root         (0)    44213 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/localFunctions.md
--rw-r--r--   0 root         (0) root         (0)     3978 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/manifolds.md
--rw-r--r--   0 root         (0) root         (0)     2590 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/nonlinearOperator.md
--rw-r--r--   0 root         (0) root         (0)     3086 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/observer.md
--rw-r--r--   0 root         (0) root         (0)     5211 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/
--rw-r--r--   0 root         (0) root         (0)     6655 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/cantileverBeam.md
--rw-r--r--   0 root         (0) root         (0)     7251 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/computePi.md
--rw-r--r--   0 root         (0) root         (0)     5439 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/cooksMembrane.md
--rw-r--r--   0 root         (0) root         (0)     7323 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/incompressibleRubberBlock.md
--rw-r--r--   0 root         (0) root         (0)     2164 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/index.md
--rw-r--r--   0 root         (0) root         (0)     7774 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/kirchhoffPlate.md
--rw-r--r--   0 root         (0) root         (0)     5114 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/newtonRaphsonMethod.md
--rw-r--r--   0 root         (0) root         (0)     6177 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/nonLinearElasticity.md
--rw-r--r--   0 root         (0) root         (0)     4179 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/
--rw-r--r--   0 root         (0) root         (0)     2439 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/buildDocumentationLocally.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/codeStyle.md
--rw-r--r--   0 root         (0) root         (0)     2415 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/howToEdit.md
--rw-r--r--   0 root         (0) root         (0)     1736 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/
--rw-r--r--   0 root         (0) root         (0)      274 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/.authors.yml
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/posts/
--rw-r--r--   0 root         (0) root         (0)     7731 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/05_cppReferences/
--rw-r--r--   0 root         (0) root         (0)     2324 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/99_Literature/
--rw-r--r--   0 root         (0) root         (0)      169 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.935876 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.935876 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/
--rw-r--r--   0 root         (0) root         (0)    52795 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rw-r--r--   0 root         (0) root         (0)    46250 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rw-r--r--   0 root         (0) root         (0)     2852 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rw-r--r--   0 root         (0) root         (0)    17924 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rw-r--r--   0 root         (0) root         (0)     9455 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/
--rw-r--r--   0 root         (0) root         (0)    35234 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rw-r--r--   0 root         (0) root         (0)    62184 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rw-r--r--   0 root         (0) root         (0)     2281 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rw-r--r--   0 root         (0) root         (0)    40033 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rw-r--r--   0 root         (0) root         (0)    25505 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rw-r--r--   0 root         (0) root         (0)     8101 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_blue.svg
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_blue.svg.license
--rw-r--r--   0 root         (0) root         (0)     8255 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_white.svg
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_white.svg.license
--rw-r--r--   0 root         (0) root         (0)     4364 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/download.md
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/gallery.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/docs/website/javascripts/
--rw-r--r--   0 root         (0) root         (0)      486 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/docs/website/stylesheets/
--rw-r--r--   0 root         (0) root         (0)      302 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/stylesheets/extra.css
--rw-r--r--   0 root         (0) root         (0)      504 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/dune.module
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/ikarus/
--rw-r--r--   0 root         (0) root         (0)      743 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    12924 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/assembler/simpleAssemblers.hh
--rw-r--r--   0 root         (0) root         (0)    10714 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/
--rw-r--r--   0 root         (0) root         (0)      239 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2575 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/loadControl.hh
--rw-r--r--   0 root         (0) root         (0)     2970 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      185 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/
--rw-r--r--   0 root         (0) root         (0)      282 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5311 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/autodiffFE.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/powerBasisFE.hh
--rw-r--r--   0 root         (0) root         (0)     1827 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/scalarFE.hh
--rw-r--r--   0 root         (0) root         (0)     9346 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feRequirements.hh
--rw-r--r--   0 root         (0) root         (0)     1338 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/
--rw-r--r--   0 root         (0) root         (0)      345 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    21360 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rw-r--r--   0 root         (0) root         (0)    13674 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/
--rw-r--r--   0 root         (0) root         (0)      397 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5699 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/interface.hh
--rw-r--r--   0 root         (0) root         (0)     2718 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)     4635 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rw-r--r--   0 root         (0) root         (0)     3809 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rw-r--r--   0 root         (0) root         (0)     5734 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/svk.hh
--rw-r--r--   0 root         (0) root         (0)      473 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/tags.hh
--rw-r--r--   0 root         (0) root         (0)     8008 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rw-r--r--   0 root         (0) root         (0)     1196 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials.hh
--rw-r--r--   0 root         (0) root         (0)    15536 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rw-r--r--   0 root         (0) root         (0)    12678 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/io/
--rw-r--r--   0 root         (0) root         (0)      258 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/io/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2350 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/io/resultEvaluators.hh
--rw-r--r--   0 root         (0) root         (0)     3829 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/io/resultFunction.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6735 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/dirichletValues.hh
--rw-r--r--   0 root         (0) root         (0)     7789 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/nonLinearOperator.hh
--rw-r--r--   0 root         (0) root         (0)    12303 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/python/
--rw-r--r--   0 root         (0) root         (0)      294 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/python/assembler/
--rw-r--r--   0 root         (0) root         (0)      249 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6752 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/python/basis/
--rw-r--r--   0 root         (0) root         (0)      237 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/basis/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/python/dirichletValues/
--rw-r--r--   0 root         (0) root         (0)      257 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/dirichletValues/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4169 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      303 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5220 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/materials/
--rw-r--r--   0 root         (0) root         (0)      268 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     9949 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/materials/material.hh
--rw-r--r--   0 root         (0) root         (0)     5207 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/python/test/
--rw-r--r--   0 root         (0) root         (0)      511 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3830 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/test/linearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)     4340 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/test/nonLinearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/python/utils/
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1185 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/solver/
--rw-r--r--   0 root         (0) root         (0)      211 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/solver/linearSolver/
--rw-r--r--   0 root         (0) root         (0)      244 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/linearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     8891 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/
--rw-r--r--   0 root         (0) root         (0)      272 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5406 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rw-r--r--   0 root         (0) root         (0)     8297 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rw-r--r--   0 root         (0) root         (0)    18574 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.951877 pyikarus-0.3.3.dev20230601114417/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      712 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/algorithms.hh
--rw-r--r--   0 root         (0) root         (0)      878 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/autodiffHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1469 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/basis.hh
--rw-r--r--   0 root         (0) root         (0)     6930 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/concepts.hh
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.955877 pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/
--rw-r--r--   0 root         (0) root         (0)      262 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/griddrawer.hh
--rw-r--r--   0 root         (0) root         (0)      544 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/matplotHelper.cpp
--rw-r--r--   0 root         (0) root         (0)      703 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/matplotHelper.hh
--rw-r--r--   0 root         (0) root         (0)     2484 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/duneUtilities.hh
--rw-r--r--   0 root         (0) root         (0)     2347 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/eigenDuneTransformations.hh
--rw-r--r--   0 root         (0) root         (0)      682 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/eigenSparseAddon.hh
--rw-r--r--   0 root         (0) root         (0)     1367 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/findLineSegment.cpp
--rw-r--r--   0 root         (0) root         (0)      724 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/findLineSegment.hh
--rw-r--r--   0 root         (0) root         (0)     3611 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/flatPreBasis.hh
--rw-r--r--   0 root         (0) root         (0)     2171 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/functionSanityChecks.cpp
--rw-r--r--   0 root         (0) root         (0)     6359 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/functionSanityChecks.hh
--rw-r--r--   0 root         (0) root         (0)     3152 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/init.hh
--rw-r--r--   0 root         (0) root         (0)    15244 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/linearAlgebraHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1711 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.955877 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/
--rw-r--r--   0 root         (0) root         (0)      450 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1554 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/controlLogger.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/controlVTKWriter.hh
--rw-r--r--   0 root         (0) root         (0)      905 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/genericControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1053 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/gridDrawerObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1132 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/loadControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1985 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/nonLinearSolverLogger.hh
--rw-r--r--   0 root         (0) root         (0)     5497 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/observer.hh
--rw-r--r--   0 root         (0) root         (0)      489 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/observerMessages.hh
--rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/pathFollowingFunctions.hh
--rw-r--r--   0 root         (0) root         (0)     1131 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/polyfit.cpp
--rw-r--r--   0 root         (0) root         (0)      570 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/polyfit.hh
--rw-r--r--   0 root         (0) root         (0)    10054 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/tensorUtils.hh
--rw-r--r--   0 root         (0) root         (0)    15149 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/traits.hh
--rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus.pc.in
--rw-r--r--   0 root         (0) root         (0)      196 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/iwyu.imp
--rw-r--r--   0 root         (0) root         (0)      422 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.955877 pyikarus-0.3.3.dev20230601114417/python/
--rw-r--r--   0 root         (0) root         (0)      423 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/python/ikarus/
--rw-r--r--   0 root         (0) root         (0)      500 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/python/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      167 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1628 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/assembler/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/basis.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/python/ikarus/finite_elements/
--rw-r--r--   0 root         (0) root         (0)      173 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/finite_elements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/finite_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/generator.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/materials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/python/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      163 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      768 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3732 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10030 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/setup.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/sandbox/
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/sandbox/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/sandbox/src/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/sandbox/src/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)   674469 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/sandbox/src/auxiliaryFiles/circle.msh
--rw-r--r--   0 root         (0) root         (0)      320 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/sandbox/src/sandbox.cpp
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 11:44:17.967877 pyikarus-0.3.3.dev20230601114417/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1080 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/tests/
--rw-r--r--   0 root         (0) root         (0)      150 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.963877 pyikarus-0.3.3.dev20230601114417/tests/src/
--rw-r--r--   0 root         (0) root         (0)     1408 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3907 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testAssembler.cpp
--rw-r--r--   0 root         (0) root         (0)     1292 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testAutodiffHelper.cpp
--rw-r--r--   0 root         (0) root         (0)    14291 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testCommon.hh
--rw-r--r--   0 root         (0) root         (0)     2639 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testDependencies.cpp
--rw-r--r--   0 root         (0) root         (0)     6520 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testDirichletValue.cpp
--rw-r--r--   0 root         (0) root         (0)     4795 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testEAS.hh
--rw-r--r--   0 root         (0) root         (0)     1600 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testEnhancedAssumedStrains.cpp
--rw-r--r--   0 root         (0) root         (0)     5818 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFEElement.hh
--rw-r--r--   0 root         (0) root         (0)      571 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFactories.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.967877 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/
--rw-r--r--   0 root         (0) root         (0)     9028 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredQuadscoarse.msh
--rw-r--r--   0 root         (0) root         (0)      395 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTest.geo
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTest.msh
--rw-r--r--   0 root         (0) root         (0)      546 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTest2.geo
--rw-r--r--   0 root         (0) root         (0)    11431 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTrianglesfine.msh
--rw-r--r--   0 root         (0) root         (0)     1870 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFunctionTraits.cpp
--rw-r--r--   0 root         (0) root         (0)     1114 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testHelpers.hh
--rw-r--r--   0 root         (0) root         (0)     3190 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testLinearElasticity.cpp
--rw-r--r--   0 root         (0) root         (0)     2278 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testManifolds.cpp
--rw-r--r--   0 root         (0) root         (0)     7962 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testMaterial.cpp
--rw-r--r--   0 root         (0) root         (0)    15896 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)      669 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearElasticityNeoHooke.cpp
--rw-r--r--   0 root         (0) root         (0)     1121 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearElasticitySVK.cpp
--rw-r--r--   0 root         (0) root         (0)     9937 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearOperator.cpp
--rw-r--r--   0 root         (0) root         (0)     6327 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testPathFollowing.cpp
--rw-r--r--   0 root         (0) root         (0)     1651 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testPolyFit.cpp
--rw-r--r--   0 root         (0) root         (0)      696 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testPythonConversion.cpp
--rw-r--r--   0 root         (0) root         (0)    17596 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testTrustRegion.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.584395 pyikarus-0.3.3.dev20230601194812/
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.bettercodehub.yml
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.clang-format
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.cmake-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.524395 pyikarus-0.3.3.dev20230601194812/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.536395 pyikarus-0.3.3.dev20230601194812/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.540395 pyikarus-0.3.3.dev20230601194812/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/createDockerContainer.yml
+-rw-r--r--   0 root         (0) root         (0)     5615 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/createRelease.yml
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/ghpages.yml
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/reuseLint.yml
+-rw-r--r--   0 root         (0) root         (0)     3335 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/runExamples.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.540395 pyikarus-0.3.3.dev20230601194812/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      482 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.540395 pyikarus-0.3.3.dev20230601194812/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.540395 pyikarus-0.3.3.dev20230601194812/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)    18375 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/LICENSES/MIT.txt
+-rw-r--r--   0 root         (0) root         (0)    16727 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-06-01 19:48:13.584395 pyikarus-0.3.3.dev20230601194812/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.540395 pyikarus-0.3.3.dev20230601194812/cmake/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/cmake/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      973 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/cmake/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.544395 pyikarus-0.3.3.dev20230601194812/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.544395 pyikarus-0.3.3.dev20230601194812/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/cmake/modules/AddMatplotppFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/cmake/modules/AddSpdlogFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      325 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/cmake/modules/IkarusMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/cmake/tools.cmake
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.544395 pyikarus-0.3.3.dev20230601194812/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.544395 pyikarus-0.3.3.dev20230601194812/docs/BuildLocally/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/BuildLocally/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.544395 pyikarus-0.3.3.dev20230601194812/docs/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/literature.bib
+-rw-r--r--   0 root         (0) root         (0)      117 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/literature.bib.license
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/mkdocs-macros.py
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/mkdocs.insiders.yml
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.528395 pyikarus-0.3.3.dev20230601194812/docs/overrides/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.544395 pyikarus-0.3.3.dev20230601194812/docs/overrides/partials/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/overrides/partials/comments.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.548395 pyikarus-0.3.3.dev20230601194812/docs/website/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/.meta.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.548395 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/
+-rw-r--r--   0 root         (0) root         (0)     4710 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/assembler.md
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/controlRoutines.md
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/dirichletBCs.md
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/feRequirements.md
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/finiteElements.md
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/grids.md
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/index.md
+-rw-r--r--   0 root         (0) root         (0)     4932 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/localBasis.md
+-rw-r--r--   0 root         (0) root         (0)    44213 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/localFunctions.md
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/manifolds.md
+-rw-r--r--   0 root         (0) root         (0)     2551 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/nonlinearOperator.md
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/observer.md
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.552395 pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/cantileverBeam.md
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/computePi.md
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/cooksMembrane.md
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/incompressibleRubberBlock.md
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/index.md
+-rw-r--r--   0 root         (0) root         (0)     7774 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/kirchhoffPlate.md
+-rw-r--r--   0 root         (0) root         (0)     5088 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/newtonRaphsonMethod.md
+-rw-r--r--   0 root         (0) root         (0)     6164 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/nonLinearElasticity.md
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.552395 pyikarus-0.3.3.dev20230601194812/docs/website/03_contribution/
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/03_contribution/buildDocumentationLocally.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/03_contribution/codeStyle.md
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/03_contribution/howToEdit.md
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.552395 pyikarus-0.3.3.dev20230601194812/docs/website/04_blog/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/04_blog/.authors.yml
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/04_blog/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.552395 pyikarus-0.3.3.dev20230601194812/docs/website/04_blog/posts/
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.552395 pyikarus-0.3.3.dev20230601194812/docs/website/05_cppReferences/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.552395 pyikarus-0.3.3.dev20230601194812/docs/website/99_Literature/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.552395 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.556395 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/
+-rw-r--r--   0 root         (0) root         (0)    52795 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)    46250 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rw-r--r--   0 root         (0) root         (0)    17924 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.556395 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/
+-rw-r--r--   0 root         (0) root         (0)    35234 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rw-r--r--   0 root         (0) root         (0)    62184 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rw-r--r--   0 root         (0) root         (0)    40033 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rw-r--r--   0 root         (0) root         (0)    25505 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rw-r--r--   0 root         (0) root         (0)     8101 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/logo_blue.svg
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/logo_blue.svg.license
+-rw-r--r--   0 root         (0) root         (0)     8255 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/logo_white.svg
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/logo_white.svg.license
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/download.md
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/gallery.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.556395 pyikarus-0.3.3.dev20230601194812/docs/website/javascripts/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.556395 pyikarus-0.3.3.dev20230601194812/docs/website/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/docs/website/stylesheets/extra.css
+-rw-r--r--   0 root         (0) root         (0)      504 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/dune.module
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.556395 pyikarus-0.3.3.dev20230601194812/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.556395 pyikarus-0.3.3.dev20230601194812/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/assembler/simpleAssemblers.hh
+-rw-r--r--   0 root         (0) root         (0)    10714 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.560395 pyikarus-0.3.3.dev20230601194812/ikarus/controlRoutines/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/controlRoutines/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/controlRoutines/loadControl.hh
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.560395 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.560395 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feBases/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feBases/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feBases/autodiffFE.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feBases/scalarFE.hh
+-rw-r--r--   0 root         (0) root         (0)     9346 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feRequirements.hh
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.560395 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    21360 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rw-r--r--   0 root         (0) root         (0)    13674 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.564395 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/interface.hh
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/svk.hh
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/tags.hh
+-rw-r--r--   0 root         (0) root         (0)     7995 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials.hh
+-rw-r--r--   0 root         (0) root         (0)    15536 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rw-r--r--   0 root         (0) root         (0)    12678 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.564395 pyikarus-0.3.3.dev20230601194812/ikarus/io/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/io/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/io/resultEvaluators.hh
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/io/resultFunction.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.564395 pyikarus-0.3.3.dev20230601194812/ikarus/linearAlgebra/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/linearAlgebra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6735 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/linearAlgebra/dirichletValues.hh
+-rw-r--r--   0 root         (0) root         (0)     7698 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/linearAlgebra/nonLinearOperator.hh
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.564395 pyikarus-0.3.3.dev20230601194812/ikarus/python/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.564395 pyikarus-0.3.3.dev20230601194812/ikarus/python/assembler/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.564395 pyikarus-0.3.3.dev20230601194812/ikarus/python/basis/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.564395 pyikarus-0.3.3.dev20230601194812/ikarus/python/dirichletValues/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/dirichletValues/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4169 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.564395 pyikarus-0.3.3.dev20230601194812/ikarus/python/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5220 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.564395 pyikarus-0.3.3.dev20230601194812/ikarus/python/finiteElements/materials/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9949 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/finiteElements/materials/material.hh
+-rw-r--r--   0 root         (0) root         (0)     5207 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.568395 pyikarus-0.3.3.dev20230601194812/ikarus/python/test/
+-rw-r--r--   0 root         (0) root         (0)      511 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/test/linearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)     4340 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/test/nonLinearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.568395 pyikarus-0.3.3.dev20230601194812/ikarus/python/utils/
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.568395 pyikarus-0.3.3.dev20230601194812/ikarus/solver/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.568395 pyikarus-0.3.3.dev20230601194812/ikarus/solver/linearSolver/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/solver/linearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     8891 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.568395 pyikarus-0.3.3.dev20230601194812/ikarus/solver/nonLinearSolver/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rw-r--r--   0 root         (0) root         (0)     8297 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rw-r--r--   0 root         (0) root         (0)    18574 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.572395 pyikarus-0.3.3.dev20230601194812/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/algorithms.hh
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/autodiffHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/basis.hh
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.572395 pyikarus-0.3.3.dev20230601194812/ikarus/utils/drawing/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/drawing/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/drawing/griddrawer.hh
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/drawing/matplotHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/drawing/matplotHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/duneUtilities.hh
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/eigenDuneTransformations.hh
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/eigenSparseAddon.hh
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/findLineSegment.cpp
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/findLineSegment.hh
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/flatPreBasis.hh
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/functionSanityChecks.cpp
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/functionSanityChecks.hh
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/init.hh
+-rw-r--r--   0 root         (0) root         (0)    15244 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/linearAlgebraHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.576395 pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/controlLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/controlVTKWriter.hh
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/genericControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/gridDrawerObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/loadControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/observer.hh
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/observerMessages.hh
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/pathFollowingFunctions.hh
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/polyfit.cpp
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/polyfit.hh
+-rw-r--r--   0 root         (0) root         (0)    10054 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/tensorUtils.hh
+-rw-r--r--   0 root         (0) root         (0)    15149 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus/utils/traits.hh
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/ikarus.pc.in
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/iwyu.imp
+-rw-r--r--   0 root         (0) root         (0)      422 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.576395 pyikarus-0.3.3.dev20230601194812/python/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.576395 pyikarus-0.3.3.dev20230601194812/python/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.576395 pyikarus-0.3.3.dev20230601194812/python/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/assembler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/basis.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.576395 pyikarus-0.3.3.dev20230601194812/python/ikarus/finite_elements/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/finite_elements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/finite_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/materials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.576395 pyikarus-0.3.3.dev20230601194812/python/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      768 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.580395 pyikarus-0.3.3.dev20230601194812/python/pyikarus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-06-01 19:48:13.000000 pyikarus-0.3.3.dev20230601194812/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10030 2023-06-01 19:48:13.000000 pyikarus-0.3.3.dev20230601194812/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 19:48:13.000000 pyikarus-0.3.3.dev20230601194812/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 19:48:13.000000 pyikarus-0.3.3.dev20230601194812/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 19:48:13.000000 pyikarus-0.3.3.dev20230601194812/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/python/setup.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.580395 pyikarus-0.3.3.dev20230601194812/sandbox/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/sandbox/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.580395 pyikarus-0.3.3.dev20230601194812/sandbox/src/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.580395 pyikarus-0.3.3.dev20230601194812/sandbox/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)   674469 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/sandbox/src/auxiliaryFiles/circle.msh
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/sandbox/src/sandbox.cpp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 19:48:13.584395 pyikarus-0.3.3.dev20230601194812/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-06-01 19:48:12.000000 pyikarus-0.3.3.dev20230601194812/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.580395 pyikarus-0.3.3.dev20230601194812/tests/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.584395 pyikarus-0.3.3.dev20230601194812/tests/src/
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testAssembler.cpp
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testAutodiffHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)    14291 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testCommon.hh
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testDependencies.cpp
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testDirichletValue.cpp
+-rw-r--r--   0 root         (0) root         (0)     4795 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testEAS.hh
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testEnhancedAssumedStrains.cpp
+-rw-r--r--   0 root         (0) root         (0)     5805 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testFEElement.hh
+-rw-r--r--   0 root         (0) root         (0)      571 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testFactories.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 19:48:13.584395 pyikarus-0.3.3.dev20230601194812/tests/src/testFiles/
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rw-r--r--   0 root         (0) root         (0)      395 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testFiles/unstructuredTest.geo
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testFiles/unstructuredTest.msh
+-rw-r--r--   0 root         (0) root         (0)      546 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testFiles/unstructuredTest2.geo
+-rw-r--r--   0 root         (0) root         (0)    11431 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testFunctionTraits.cpp
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testHelpers.hh
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testLinearElasticity.cpp
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testManifolds.cpp
+-rw-r--r--   0 root         (0) root         (0)     7949 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testMaterial.cpp
+-rw-r--r--   0 root         (0) root         (0)    15845 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testNonLinearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testNonLinearElasticityNeoHooke.cpp
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testNonLinearElasticitySVK.cpp
+-rw-r--r--   0 root         (0) root         (0)     9846 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testNonLinearOperator.cpp
+-rw-r--r--   0 root         (0) root         (0)     6251 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testPathFollowing.cpp
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testPolyFit.cpp
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testPythonConversion.cpp
+-rw-r--r--   0 root         (0) root         (0)    17531 2023-06-01 19:48:04.000000 pyikarus-0.3.3.dev20230601194812/tests/src/testTrustRegion.cpp
```

### Comparing `pyikarus-0.3.3.dev20230601114417/.clang-format` & `pyikarus-0.3.3.dev20230601194812/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.cmake-format` & `pyikarus-0.3.3.dev20230601194812/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.3.dev20230601194812/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.3.dev20230601194812/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.github/workflows/createRelease.yml` & `pyikarus-0.3.3.dev20230601194812/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.3.dev20230601194812/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.github/workflows/debian.yml` & `pyikarus-0.3.3.dev20230601194812/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.github/workflows/ghpages.yml` & `pyikarus-0.3.3.dev20230601194812/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.github/workflows/releasePythonPackage.yml` & `pyikarus-0.3.3.dev20230601194812/.github/workflows/releasePythonPackage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.github/workflows/runExamples.yml` & `pyikarus-0.3.3.dev20230601194812/.github/workflows/runExamples.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.github/workflows/scripts/release.py` & `pyikarus-0.3.3.dev20230601194812/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.github/workflows/style.yml` & `pyikarus-0.3.3.dev20230601194812/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/.reuse/dep5` & `pyikarus-0.3.3.dev20230601194812/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/CHANGELOG.md` & `pyikarus-0.3.3.dev20230601194812/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 - Added computation of Cauchy stress in linear elasticity ([#137](https://github.com/ikarus-project/ikarus/pull/137))
 - Added greeting and init function for a reasonable default, e.g., log also to file ([#147](https://github.com/ikarus-project/ikarus/pull/147))
 - Added an interface for the material library ([#154](https://github.com/ikarus-project/ikarus/pull/154))
 - Added a wrapper for flat and blocked basis ([#157](https://github.com/ikarus-project/ikarus/pull/157))
 - Added basic python bindings and infrastructure. Ikarus can now be downloaded via `pip install pyikarus` ([#157](https://github.com/ikarus-project/ikarus/pull/152))
 - Added result evaluators to post-process desired results ([#165](https://github.com/ikarus-project/ikarus/pull/165))
 - Added explicit calculation of scalars, vectors, and matrices for `NonLinearElastic` ([#160](https://github.com/ikarus-project/ikarus/pull/160))
+- Renamed Ikarus::linearAlgebraFunctions to Ikarus::functions ([#171](https://github.com/ikarus-project/ikarus/pull/171))
 
 ## Release v0.3 (Prometheus)
 
 - Added codespell workflow (CI checks now for grammar and typos in comments and variable names) [#70](https://github.com/ikarus-project/ikarus/pull/70)
 - Added `EnhancedAssumedStrains` to decorate a linear-elastic element with various EAS methods [#74](https://github.com/ikarus-project/ikarus/pull/74)
 - Added the ability for the linear solver to accept matrix-valued rhs [#76](https://github.com/ikarus-project/ikarus/pull/76)
 - Added a path-following technique, such that a scalar subsidiary equation, for example, for `Arc length method`,  can be implemented independently [#80](https://github.com/ikarus-project/ikarus/pull/80)
```

### Comparing `pyikarus-0.3.3.dev20230601114417/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601194812/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/CODE_OF_CONDUCT.md` & `pyikarus-0.3.3.dev20230601194812/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/LICENSE.md` & `pyikarus-0.3.3.dev20230601194812/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.3.dev20230601194812/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.3.dev20230601194812/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.3.dev20230601194812/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/LICENSES/MIT.txt` & `pyikarus-0.3.3.dev20230601194812/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.3.dev20230601194812/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/PKG-INFO` & `pyikarus-0.3.3.dev20230601194812/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230601114417
+Version: 0.3.3.dev20230601194812
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230601114417 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230601194812 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [![Debian](https://github.com/
 ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://
 github.com/ikarus-project/ikarus/actions/workflows/debian.yml) [![codecov]
```

### Comparing `pyikarus-0.3.3.dev20230601114417/README.md` & `pyikarus-0.3.3.dev20230601194812/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/cmake/CPM.cmake` & `pyikarus-0.3.3.dev20230601194812/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601194812/cmake/FormatTarget/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.3.dev20230601194812/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.3.dev20230601194812/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.3.dev20230601194812/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.3.dev20230601194812/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/cmake/tools.cmake` & `pyikarus-0.3.3.dev20230601194812/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/config.h.cmake` & `pyikarus-0.3.3.dev20230601194812/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.3.dev20230601194812/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/literature.bib` & `pyikarus-0.3.3.dev20230601194812/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/mkdocs-macros.py` & `pyikarus-0.3.3.dev20230601194812/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/mkdocs.yml` & `pyikarus-0.3.3.dev20230601194812/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/overrides/partials/comments.html` & `pyikarus-0.3.3.dev20230601194812/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/assembler.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/finiteElements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/grids.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/index.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/nonlinearOperator.md`

 * *Files 4% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 Then, a ``NonLinearOperator`` can be constructed as follows:
 
 ```cpp
 double x               = 13;
 auto fvLambda  = [&](auto&& x) { return f(x); };
 auto dfvLambda = [&](auto&& x) { return df(x); };
 
-auto nonLinOp = Ikarus::NonLinearOperator(linearAlgebraFunctions(fvLambda, dfvLambda), parameter(x));
+auto nonLinOp = Ikarus::NonLinearOperator(functions(fvLambda, dfvLambda), parameter(x));
 ```
 !!! note 
     It is assumed that the second function is the derivative of the first function, the third function is the derivative of the second function (2nd derivative of the first function), and so on.
 
-``linearAlgebraFunctions(...)`` and ``parameter(...)`` are helper functions. They are necessary to distinguish which argument is a function and which argument is a parameter.
+``functions(...)`` and ``parameter(...)`` are helper functions. They are necessary to distinguish which argument is a function and which argument is a parameter.
 
 ``nonLinOp`` provides the following features:
 ```cpp
 void updateAll() // (1)!
 void update<n>() // (2)!
 auto& value() // (3)!
 auto& derivative() // (4)!
@@ -35,15 +35,15 @@
 auto& secondParameter() // (8)!
 auto& nthParameter<n>() // (9)!
 auto& lastParameter() // (10)!
 auto subOperator<n,m,...>() // (11)!
 ```
 
 1. Evaluates all functions.
-2. Evaluates the n-th function in ``linearAlgebraFunctions(...)`` . Counting starts from 0, as always in C++.
+2. Evaluates the n-th function in ``functions(...)`` . Counting starts from 0, as always in C++.
 3. Returns the result of the function evaluation.
 4. Returns the result of the evaluation of the first derivative (if the function for the first derivative is passed to the nonlinear operator during construction).
 5. Returns the result of the evaluation of the second derivative (if the function for the second derivative is passed to the nonlinear operator during construction).
 6. Returns the result of the evaluation of the n-th derivative (if the function for the n-th derivative is passed to the nonlinear operator during construction).
 7. Returns the value of the first parameter.
 8. Returns the value of the second parameter (if available).
 9. Returns the value of the n-th parameter (if available).
```

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/observer.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/solvers.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/computePi.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/index.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/kirchhoffPlate.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 3. Maximum number of iterations
 4. Expected value (analytical solution)
 
 Functors are created then to evaluate the function to be solved for and its derivative. These are then passed to the non-linear operator as shown below:
 ```cpp
 auto fvLambda  = [&](auto &&x) { return f(x); };
 auto dfvLambda = [&](auto &&x) { return df(x); };
-Ikarus::NonLinearOperator nonLinOp(Ikarus::linearAlgebraFunctions(fvLambda, dfvLambda), Ikarus::parameter(x));
+Ikarus::NonLinearOperator nonLinOp(Ikarus::functions(fvLambda, dfvLambda), Ikarus::parameter(x));
 ```
 The standard implementation of the Newton-Raphson method is illustrated in this function, which also uses `nonLinOp`.
 ```cpp
 int iterCount = 1;
 while (abs(nonLinOp.value()) > eps and iterCount <= maxIter) {
   x -= nonLinOp.value() / nonLinOp.derivative();
   nonLinOp.updateAll();
@@ -85,15 +85,15 @@
   double x               = 13;
   const double eps       = 1e-10;
   const int maxIter      = 20;
   const double xExpected = std::sqrt(5.0) - 1.0;
 
   auto fvLambda  = [&](auto &&x) { return f(x); };
   auto dfvLambda = [&](auto &&x) { return df(x); };
-  Ikarus::NonLinearOperator nonLinOp(Ikarus::linearAlgebraFunctions(fvLambda, dfvLambda), Ikarus::parameter(x));
+  Ikarus::NonLinearOperator nonLinOp(Ikarus::functions(fvLambda, dfvLambda), Ikarus::parameter(x));
 
   Ikarus::NewtonRaphson nr(nonLinOp);
   nr.setup({eps, maxIter});
   
   auto ourSimpleObserver = std::make_shared<OurFirstObserver>();
   nr.subscribe(NonLinearSolverMessages::ITERATION_STARTED, ourSimpleObserver);
```

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/nonLinearElasticity.md`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
   if (std::abs(intersection.geometry().center()[1]) < 1e-8) dirichletFlags[localView.index(localIndex)] = true;
 });
 ```
 The finite element requirements are defined by using the affordance `#!cpp Ikarus::AffordanceCollections::elastoStatics`.
 This is then used to create functors to get the stiffness matrix, residual vector, and energy value using a sparse assembler.
 A non-linear operator and the linear solver used by the `solverType` are defined as:
 ```cpp
-auto nonLinOp = Ikarus::NonLinearOperator(linearAlgebraFunctions(energyFunction, residualFunction, KFunction), parameter(d, lambda));
+auto nonLinOp = Ikarus::NonLinearOperator(functions(energyFunction, residualFunction, KFunction), parameter(d, lambda));
 auto linSolver = Ikarus::ILinearSolver<double>(Ikarus::SolverTypeTag::sd_UmfPackLU);
 ```
 An object for the Newton-Raphson method or the trust region method can then be defined as
 ```cpp
 #if solverType == 0
   auto nr = Ikarus::makeNewtonRaphson(nonLinOp.subOperator<1, 2>(), std::move(linSolver));
 #endif
```

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/02_examples/vonMisesTruss.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/03_contribution/openTask.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_blue.svg` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/logo_blue.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_white.svg` & `pyikarus-0.3.3.dev20230601194812/docs/website/auxiliaryImages/logo_white.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/download.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/docs/website/index.md` & `pyikarus-0.3.3.dev20230601194812/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601194812/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.3.dev20230601194812/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/autodiffFE.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feBases/autodiffFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
       };
       auto df = [&](auto &) {
         auto moduli = (matImpl.template tangentModuli<MaterialImpl::strainTag, true>(E)).eval();
         return (moduli(fixedDiagonalVoigtIndices, fixedDiagonalVoigtIndices) / MaterialImpl::derivativeFactor).eval();
       };
 
       auto Er    = E(fixedDiagonalVoigtIndices, fixedDiagonalVoigtIndices).eval().template cast<ScalarType>();
-      auto nonOp = Ikarus::NonLinearOperator(linearAlgebraFunctions(f, df), parameter(Er));
+      auto nonOp = Ikarus::NonLinearOperator(functions(f, df), parameter(Er));
       auto nr    = Ikarus::makeNewtonRaphson(
              nonOp, [](auto &r, auto &A) { return (A.inverse() * r).eval(); },
              [&](auto &Ex33, auto &Ecomps) {
             for (int ri = 0; auto i : fixedDiagonalVoigtIndices) {
               auto indexPair = fromVoigt(i);
               E(indexPair[0], indexPair[1]) += Ecomps(ri++);
             }
```

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/mechanics/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/finiteElements/physicsHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/io/resultEvaluators.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/io/resultEvaluators.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/io/resultFunction.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/io/resultFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     template <class Pars, class Tuple, std::size_t... I>
     constexpr decltype(auto) makeTupleOfValuesAndReferences(Tuple&& t, Pars&& p, std::index_sequence<I...>) {
       return std::make_tuple(
           forwardasReferenceWrapperIfIsReference(applyAndRemoveReferenceWrapper(std::get<I>(t), p.args))...);
     }
 
     template <typename... Args>
-    struct LinearAlgebraFunctions {
+    struct Functions {
       std::tuple<std::reference_wrapper<std::remove_reference_t<Args>>...> args;
     };
 
     template <typename... Args>
     struct Parameter {
       std::tuple<std::reference_wrapper<std::remove_reference_t<Args>>...> args;
     };
@@ -53,20 +53,20 @@
 
   template <typename... Args>
   auto parameter(Args&&... args) {
     return Impl::Parameter<Args&&...>{std::forward_as_tuple(std::forward<Args>(args)...)};
   }
 
   template <typename... Args>
-  auto linearAlgebraFunctions(Args&&... args) {
-    return Impl::LinearAlgebraFunctions<Args&&...>{std::forward_as_tuple(std::forward<Args>(args)...)};
+  auto functions(Args&&... args) {
+    return Impl::Functions<Args&&...>{std::forward_as_tuple(std::forward<Args>(args)...)};
   }
 
   template <typename... DerivativeArgs, typename... ParameterArgs>
-  auto initResults(const Impl::LinearAlgebraFunctions<DerivativeArgs...>& derivativesFunctions,
+  auto initResults(const Impl::Functions<DerivativeArgs...>& derivativesFunctions,
                    const Impl::Parameter<ParameterArgs...>& parameterI) {
     return Impl::makeTupleOfValuesAndReferences(
         derivativesFunctions.args, parameterI,
         std::make_index_sequence<std::tuple_size_v<std::remove_reference_t<decltype(derivativesFunctions.args)>>>{});
   }
 
   template <typename TypeListOne, typename TypeListTwo>
@@ -78,29 +78,29 @@
                     "This type should not be instantiated. check that your arguments satisfies the template below");
     }
   };
 
   /* NonLinearOperator is a class taking linear algebra function and their arguments.
    * The fcuntion are assumed to be derivatvies of each other. */
   template <typename... DerivativeArgs, typename... ParameterArgs>
-  class NonLinearOperator<Impl::LinearAlgebraFunctions<DerivativeArgs...>, Impl::Parameter<ParameterArgs...>> {
+  class NonLinearOperator<Impl::Functions<DerivativeArgs...>, Impl::Parameter<ParameterArgs...>> {
     using FunctionReturnValues = std::tuple<Ikarus::Std::ReturnType<DerivativeArgs, ParameterArgs&...>...>;
     using ParameterValues      = std::tuple<ParameterArgs...>;
 
   public:
     template <int n>
     using FunctionReturnType = std::tuple_element_t<n, FunctionReturnValues>;
 
     template <int n>
     using ParameterValue = std::remove_cvref_t<std::tuple_element_t<n, ParameterValues>>;
 
     using ValueType      = std::remove_cvref_t<std::tuple_element_t<0, FunctionReturnValues>>;
     using DerivativeType = std::remove_cvref_t<std::tuple_element_t<1, FunctionReturnValues>>;
 
-    explicit NonLinearOperator(const Impl::LinearAlgebraFunctions<DerivativeArgs...>& derivativesFunctions,
+    explicit NonLinearOperator(const Impl::Functions<DerivativeArgs...>& derivativesFunctions,
                                const Impl::Parameter<ParameterArgs...>& parameterI)
         : derivatives_{derivativesFunctions.args},
           args_{parameterI.args},
           derivativesEvaluated_(initResults(derivativesFunctions, parameterI)) {}
 
     /* Evaluates all functions. Usually called if the parameters changes */
     void updateAll() {
@@ -145,15 +145,15 @@
     auto& nthParameter() requires(sizeof...(ParameterArgs) >= n) {
       return std::get<n>(args_).get();
     }
 
     /* Returns a new NonLinearOperator from the given indices */
     template <int... Derivatives>
     auto subOperator() {
-      return Ikarus::NonLinearOperator(linearAlgebraFunctions(std::get<Derivatives>(derivatives_)...),
+      return Ikarus::NonLinearOperator(functions(std::get<Derivatives>(derivatives_)...),
                                        Impl::applyAndRemoveReferenceWrapper(parameter<ParameterArgs...>, args_));
     }
 
   private:
     using FunctionReturnValuesWrapper = std::tuple<std::conditional_t<
         std::is_reference_v<Ikarus::Std::ReturnType<DerivativeArgs, ParameterArgs&...>>,
         std::reference_wrapper<std::remove_cvref_t<Ikarus::Std::ReturnType<DerivativeArgs, ParameterArgs&...>>>,
```

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/python/basis/basis.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/python/basis/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.3.dev20230601194812/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.3.dev20230601194812/ikarus/python/test/nonLinearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.3.dev20230601194812/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/algorithms.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/basis.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/concepts.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/init.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/polyfit.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/ikarus/utils/traits.hh` & `pyikarus-0.3.3.dev20230601194812/ikarus/utils/traits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/ikarus/__init__.py` & `pyikarus-0.3.3.dev20230601194812/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/ikarus/_ikarus.cc` & `pyikarus-0.3.3.dev20230601194812/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.3.dev20230601194812/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/ikarus/basis.py` & `pyikarus-0.3.3.dev20230601194812/python/ikarus/basis.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/ikarus/dirichletValues.py` & `pyikarus-0.3.3.dev20230601194812/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/ikarus/finite_elements/__init__.py` & `pyikarus-0.3.3.dev20230601194812/python/ikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/ikarus/generator.py` & `pyikarus-0.3.3.dev20230601194812/python/ikarus/generator.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/ikarus/materials.py` & `pyikarus-0.3.3.dev20230601194812/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/ikarus/utils/__init__.py` & `pyikarus-0.3.3.dev20230601194812/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.3.dev20230601194812/python/pyikarus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230601114417
+Version: 0.3.3.dev20230601194812
 Home-page: 
 Author: mueller@ibb.uni-stuttgart.de
 Author-email: mueller@ibb.uni-stuttgart.de
 Classifier: Programming Language :: C++
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Requires-Python: >=3.4
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230601114417 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230601194812 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [![Debian](https://github.com/
 ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://
 github.com/ikarus-project/ikarus/actions/workflows/debian.yml) [![codecov]
```

### Comparing `pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.3.dev20230601194812/python/pyikarus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/python/setup.py.in` & `pyikarus-0.3.3.dev20230601194812/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601194812/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.3.dev20230601194812/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/setup.py` & `pyikarus-0.3.3.dev20230601194812/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # build _ikarus
 # cd /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-ikarusVersion = "0.3.3.dev20230601114417"
+ikarusVersion = "0.3.3.dev20230601194812"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor since ikarus pypi package already exists
 metadata["name"] = "pyikarus"
```

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601194812/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testAssembler.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testAssembler.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testCommon.hh` & `pyikarus-0.3.3.dev20230601194812/tests/src/testCommon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testDependencies.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testDependencies.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testDirichletValue.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testDirichletValue.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testEAS.hh` & `pyikarus-0.3.3.dev20230601194812/tests/src/testEAS.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testEnhancedAssumedStrains.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testEnhancedAssumedStrains.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testFEElement.hh` & `pyikarus-0.3.3.dev20230601194812/tests/src/testFEElement.hh`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     requirements.insertGlobalSolution(Ikarus::FESolutions::displacement, d_);
     return sparseAssembler.getVector(requirements);
   };
   auto ddfvLambda = [&](auto&& d_) -> auto& {
     requirements.insertGlobalSolution(Ikarus::FESolutions::displacement, d_);
     return sparseAssembler.getMatrix(requirements);
   };
-  auto nonLinOp = Ikarus::NonLinearOperator(linearAlgebraFunctions(fvLambda, dfvLambda, ddfvLambda), parameter(d));
+  auto nonLinOp = Ikarus::NonLinearOperator(functions(fvLambda, dfvLambda, ddfvLambda), parameter(d));
 
   // execute all passed functions
   nonLinOp.updateAll();
   Dune::Hybrid::forEach(Dune::Hybrid::integralRange(Dune::index_constant<sizeof...(F)>()),
                         [&](auto i) { t.subTest(std::get<i.value>(fTuple)(nonLinOp, fe, requirements)); });
 
   // check if element has a test functor, if yes we execute it
```

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testFactories.hh` & `pyikarus-0.3.3.dev20230601194812/tests/src/testFactories.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.3.dev20230601194812/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.3.dev20230601194812/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.3.dev20230601194812/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testFunctionTraits.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testFunctionTraits.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testHelpers.hh` & `pyikarus-0.3.3.dev20230601194812/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testLinearElasticity.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testLinearElasticity.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testManifolds.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testManifolds.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testMaterial.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testMaterial.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     return (mat.template tangentModuli<strainTag>(xv) * strainDerivativeFactor * strainDerivativeFactor).eval();
   };
 
   using ReturnTypeDerivative = Ikarus::Std::ReturnType<decltype(df), decltype(ev)&>;
 
   using ReturnTypeSecondDerivative = Ikarus::Std::ReturnType<decltype(ddf), decltype(ev)&>;
 
-  auto nonLinOp    = Ikarus::NonLinearOperator(linearAlgebraFunctions(f, df, ddf), parameter(ev));
+  auto nonLinOp    = Ikarus::NonLinearOperator(functions(f, df, ddf), parameter(ev));
   auto subNonLinOp = nonLinOp.template subOperator<1, 2>();
 
   t.check(checkGradient(nonLinOp, {.draw = false, .writeSlopeStatementIfFailed = true})) << "checkGradient Failed";
   t.check(checkHessian(nonLinOp, {.draw = false, .writeSlopeStatementIfFailed = true})) << "checkHessian Failed";
   t.check(checkJacobian(subNonLinOp, {.draw = false, .writeSlopeStatementIfFailed = true})) << "checkJacobian Failed";
 
   return t;
```

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearElasticity.hh` & `pyikarus-0.3.3.dev20230601194812/tests/src/testNonLinearElasticity.hh`

 * *Files 0% similar despite different names*

```diff
@@ -99,16 +99,16 @@
 
   auto energyFunction = [&](auto&& disp_, auto&& lambdaLocal) -> auto& {
     req.insertGlobalSolution(Ikarus::FESolutions::displacement, disp_)
         .insertParameter(Ikarus::FEParameter::loadfactor, lambdaLocal);
     return sparseAssembler.getScalar(req);
   };
 
-  auto nonLinOp = Ikarus::NonLinearOperator(linearAlgebraFunctions(energyFunction, residualFunction, KFunction),
-                                            parameter(d, lambda));
+  auto nonLinOp
+      = Ikarus::NonLinearOperator(functions(energyFunction, residualFunction, KFunction), parameter(d, lambda));
 
   const double gradTol = 1e-8;
 
   auto tr = Ikarus::makeTrustRegion(nonLinOp);
   tr->setup({.verbosity = 1,
              .maxiter   = 1000,
              .grad_tol  = gradTol,
```

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearElasticityNeoHooke.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testNonLinearElasticityNeoHooke.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearElasticitySVK.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testNonLinearElasticitySVK.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearOperator.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testNonLinearOperator.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 auto simple1DOperatorNewtonRhapsonTest() {
   TestSuite t("simple1DOperatorNewtonRhapsonTest");
 
   double x = 13;
 
   auto fvLambda  = [&](auto&& x_) { return f(x_); };
   auto dfvLambda = [&](auto&& x_) { return df(x_); };
-  Ikarus::NonLinearOperator nonLinOp(linearAlgebraFunctions(fvLambda, dfvLambda), parameter(x));
+  Ikarus::NonLinearOperator nonLinOp(functions(fvLambda, dfvLambda), parameter(x));
 
   // Newton method test
   const double eps       = 1e-14;
   const int maxIter      = 20;
   const double xExpected = std::sqrt(5.0) - 1.0;
 
   Ikarus::NewtonRaphson nr(nonLinOp);
@@ -64,15 +64,15 @@
 
 auto simple1DOperatorNewtonRhapsonCheckThatThePerfectPredictorWorksTest() {
   TestSuite t("simple1DOperatorNewtonRhapsonCheckThatThePerfectPredictorWorksTest");
   double x = 0;
 
   auto fvLambda  = [](auto&& x_) { return f(x_); };
   auto dfvLambda = [](auto&& x_) { return df(x_); };
-  Ikarus::NonLinearOperator nonLinOp(linearAlgebraFunctions(fvLambda, dfvLambda), parameter(x));
+  Ikarus::NonLinearOperator nonLinOp(functions(fvLambda, dfvLambda), parameter(x));
 
   const double eps       = 1e-14;
   const int maxIter      = 20;
   const double xExpected = std::sqrt(5.0) - 1.0;
 
   Ikarus::NewtonRaphson nr(nonLinOp);
 
@@ -83,15 +83,15 @@
 auto dfFail(double x) { return x + 1000000; }
 
 auto simple1DOperatorNewtonRhapsonWithWrongDerivativeTest() {
   double x = 13;
 
   auto fvLambda  = [](auto&& x_) { return f(x_); };
   auto dfvLambda = [](auto&& x_) { return dfFail(x_); };
-  Ikarus::NonLinearOperator nonLinOp(linearAlgebraFunctions(fvLambda, dfvLambda), parameter(x));
+  Ikarus::NonLinearOperator nonLinOp(functions(fvLambda, dfvLambda), parameter(x));
 
   // Newton method test
   const double eps  = 1e-14;
   const int maxIter = 20;
 
   TestSuite t("checkNewtonRhapsonFailing");
   Ikarus::NewtonRaphson nr(nonLinOp);
@@ -113,15 +113,15 @@
 auto simple1DOperatorNewtonRhapsonTestWithParamter() {
   TestSuite t("simple1DOperatorNewtonRhapsonTestWithParamter");
   double x = 13;
 
   for (int i = 0; i < 3; ++i) {
     auto fvLambda  = [](auto&& x_, const int& i_) { return fp(x_, i_); };
     auto dfvLambda = [](auto&& x_, const int& i_) { return dfp(x_, i_); };
-    Ikarus::NonLinearOperator nonLinOp(linearAlgebraFunctions(fvLambda, dfvLambda), parameter(x, i));
+    Ikarus::NonLinearOperator nonLinOp(functions(fvLambda, dfvLambda), parameter(x, i));
 
     // Newton method test
     const double eps       = 1e-14;
     const int maxIter      = 20;
     const double xExpected = std::sqrt(4 + i * i) - i;
 
     Ikarus::NewtonRaphson nr(nonLinOp);
@@ -136,15 +136,15 @@
   Eigen::Vector3d b;
   b << 5, 7, 8;
   Eigen::Matrix3d A;
   A = Eigen::Matrix3d::Identity() * 13;
 
   auto fvLambda  = [&](auto&& x_) { return fv(x_, A, b); };
   auto dfvLambda = [&](auto&& x_) { return dfv(x_, A, b); };
-  auto nonLinOp  = Ikarus::NonLinearOperator(linearAlgebraFunctions(fvLambda, dfvLambda), parameter(x));
+  auto nonLinOp  = Ikarus::NonLinearOperator(functions(fvLambda, dfvLambda), parameter(x));
 
   // Newton method test
   const double eps  = 1e-14;
   const int maxIter = 20;
   Ikarus::NewtonRaphson nr(nonLinOp, [&](auto& r, auto& A_) { return A_.inverse() * r; });  // special linear solver
   return checkNewtonRhapson(nr, x, eps, maxIter, 1, (-A.ldlt().solve(b)).eval(), Eigen::Vector3d::Zero().eval());
 }
@@ -166,15 +166,15 @@
   b << 5, 7, 8;
   Eigen::MatrixXd A(3, 3);
   A = Eigen::MatrixXd::Identity(3, 3) * 13;
 
   auto fvLambda   = [&](auto&& x_) { return f2v(x_, A, b); };
   auto dfvLambda  = [&](auto&& x_) { return df2v(x_, A, b); };
   auto ddfvLambda = [&](auto&& x_) { return ddf2v(x_, A, b); };
-  auto nonLinOp   = Ikarus::NonLinearOperator(linearAlgebraFunctions(fvLambda, dfvLambda, ddfvLambda), parameter(x));
+  auto nonLinOp   = Ikarus::NonLinearOperator(functions(fvLambda, dfvLambda, ddfvLambda), parameter(x));
 
   t.check(checkGradient(nonLinOp, {.draw = false, .writeSlopeStatementIfFailed = false}));
 
   auto subOperator = nonLinOp.subOperator<1, 2>();
   // Newton method test find root of first derivative
   const double eps  = 1e-14;
   const int maxIter = 20;
@@ -222,15 +222,15 @@
     return df2vNL(xR, A, b);
   };
   auto ddfvLambda = [&](auto&& x_) {
     auto xR = x_.template cast<autodiff::dual2nd>().eval();
     return ddf2vNL(xR, A, b);
   };
 
-  auto nonLinOp = Ikarus::NonLinearOperator(linearAlgebraFunctions(fvLambda, dfvLambda, ddfvLambda), parameter(x));
+  auto nonLinOp = Ikarus::NonLinearOperator(functions(fvLambda, dfvLambda, ddfvLambda), parameter(x));
 
   t.check(checkGradient(nonLinOp, {.draw = false, .writeSlopeStatementIfFailed = false}));
   t.check(checkHessian(nonLinOp, {.draw = false, .writeSlopeStatementIfFailed = false}));
 
   auto subOperator = nonLinOp.subOperator<1, 2>();
 
   // Newton method test find root of first derivative
```

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testPathFollowing.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testPathFollowing.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -43,16 +43,15 @@
   double lambda = 0;
   Eigen::VectorXd D;
   D.setZero(2);
 
   auto fvLambda  = [&](auto&& D_, auto&& lambda_) { return residual(D_, lambda_); };
   auto dfvLambda = [&](auto&& D_, auto&& lambda_) { return stiffnessMatrix(D_, lambda_); };
 
-  auto nonLinOp
-      = Ikarus::NonLinearOperator(Ikarus::linearAlgebraFunctions(fvLambda, dfvLambda), Ikarus::parameter(D, lambda));
+  auto nonLinOp = Ikarus::NonLinearOperator(Ikarus::functions(fvLambda, dfvLambda), Ikarus::parameter(D, lambda));
 
   auto linSolver = Ikarus::ILinearSolver<double>(Ikarus::SolverTypeTag::d_LDLT);
 
   double stepSize = 0.1;
   int load_steps  = 50;
 
   auto pft = Ikarus::StandardArcLength{};  // Path following type
@@ -75,16 +74,15 @@
   double lambda = 0;
   Eigen::VectorXd D;
   D.setZero(2);
 
   auto fvLambda  = [&](auto&& D_, auto&& lambda_) { return residual(D_, lambda_); };
   auto dfvLambda = [&](auto&& D_, auto&& lambda_) { return stiffnessMatrix(D_, lambda_); };
 
-  auto nonLinOp
-      = Ikarus::NonLinearOperator(Ikarus::linearAlgebraFunctions(fvLambda, dfvLambda), Ikarus::parameter(D, lambda));
+  auto nonLinOp = Ikarus::NonLinearOperator(Ikarus::functions(fvLambda, dfvLambda), Ikarus::parameter(D, lambda));
 
   auto linSolver = Ikarus::ILinearSolver<double>(Ikarus::SolverTypeTag::d_LDLT);
 
   double stepSize = 0.1;
   int load_steps  = 50;
 
   auto nr                      = Ikarus::makeNewtonRaphsonWithSubsidiaryFunction(nonLinOp, std::move(linSolver));
@@ -102,16 +100,15 @@
   double lambda = 0;
   Eigen::VectorXd D;
   D.setZero(2);
 
   auto fvLambda  = [&](auto&& D_, auto&& lambda_) { return residual(D_, lambda_); };
   auto dfvLambda = [&](auto&& D_, auto&& lambda_) { return stiffnessMatrix(D_, lambda_); };
 
-  auto nonLinOp
-      = Ikarus::NonLinearOperator(Ikarus::linearAlgebraFunctions(fvLambda, dfvLambda), Ikarus::parameter(D, lambda));
+  auto nonLinOp = Ikarus::NonLinearOperator(Ikarus::functions(fvLambda, dfvLambda), Ikarus::parameter(D, lambda));
 
   auto linSolver = Ikarus::ILinearSolver<double>(Ikarus::SolverTypeTag::d_LDLT);
 
   double stepSize = 0.1;
   int load_steps  = 50;
 
   auto pft = Ikarus::LoadControlWithSubsidiaryFunction{};  // Path following type
@@ -133,16 +130,15 @@
   double lambda = 0;
   Eigen::VectorXd D;
   D.setZero(2);
 
   auto fvLambda  = [&](auto&& D_, auto&& lambda_) { return residual(D_, lambda_); };
   auto dfvLambda = [&](auto&& D_, auto&& lambda_) { return stiffnessMatrix(D_, lambda_); };
 
-  auto nonLinOp
-      = Ikarus::NonLinearOperator(Ikarus::linearAlgebraFunctions(fvLambda, dfvLambda), Ikarus::parameter(D, lambda));
+  auto nonLinOp = Ikarus::NonLinearOperator(Ikarus::functions(fvLambda, dfvLambda), Ikarus::parameter(D, lambda));
 
   auto linSolver = Ikarus::ILinearSolver<double>(Ikarus::SolverTypeTag::d_LDLT);
 
   double stepSize                    = 0.05;
   int load_steps                     = 30;
   std::vector<int> controlledIndices = {0};
```

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testPolyFit.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testPolyFit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testPythonConversion.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testPythonConversion.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230601114417/tests/src/testTrustRegion.cpp` & `pyikarus-0.3.3.dev20230601194812/tests/src/testTrustRegion.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
   TestSuite t("trustRegion1");
   Eigen::Vector<double, 1> x;
   x << 2;
 
   auto fvLambda   = [](auto&& xL) { return f(xL); };
   auto dfvLambda  = [](auto&& xL) { return df(xL); };
   auto ddfvLambda = [](auto&& xL) { return ddf(xL); };
-  Ikarus::NonLinearOperator nonLinOp(linearAlgebraFunctions(fvLambda, dfvLambda, ddfvLambda), parameter(x));
+  Ikarus::NonLinearOperator nonLinOp(functions(fvLambda, dfvLambda, ddfvLambda), parameter(x));
 
   Eigen::Vector<double, 1> xExpected;
   xExpected << 0;
 
   auto tr = Ikarus::makeTrustRegion(nonLinOp);
   tr->setup({.verbosity = 1, .Delta0 = 1});
   const auto solverInfo = tr->solve();
@@ -88,15 +88,15 @@
   TestSuite t("trustRegion2");
   Eigen::Vector2d x;
   x << 2, 3;
 
   auto fvLambda   = [](auto&& xL) { return rosenbrock(xL); };
   auto dfvLambda  = [](auto&& xL) { return rosenbrockdx(xL); };
   auto ddfvLambda = [](auto&& xL) { return rosenbrockddx(xL); };
-  Ikarus::NonLinearOperator nonLinOp(linearAlgebraFunctions(fvLambda, dfvLambda, ddfvLambda), parameter(x));
+  Ikarus::NonLinearOperator nonLinOp(functions(fvLambda, dfvLambda, ddfvLambda), parameter(x));
   const double eps   = 1e-10;
   const int maxIter_ = 30;
   Eigen::Vector2d xExpected;
   xExpected << a_, a_ * a_;
 
   Ikarus::TrustRegion tr(nonLinOp);
   tr.setup({.verbosity = 1, .maxiter = maxIter_, .grad_tol = eps, .Delta0 = 1});
@@ -144,15 +144,15 @@
     auto xR = xL.template cast<autodiff::dual>().eval();
     return df3(xR);
   };
   auto ddfvLambda = [](auto&& xL) {
     auto xR = xL.template cast<autodiff::dual2nd>().eval();
     return ddf3(xR);
   };
-  Ikarus::NonLinearOperator nonLinOp(linearAlgebraFunctions(fvLambda, dfvLambda, ddfvLambda), parameter(x));
+  Ikarus::NonLinearOperator nonLinOp(functions(fvLambda, dfvLambda, ddfvLambda), parameter(x));
   const double eps   = 1e-12;
   const int maxIter_ = 30;
   Eigen::Vector2d xExpected;
   xExpected << 2.3066301277034750861, -0.33230864873179355445;
 
   Ikarus::TrustRegion tr(nonLinOp);
   tr.setup({.verbosity = 1, .maxiter = maxIter_, .grad_tol = eps, .corr_tol = eps, .Delta0 = 1});
@@ -226,15 +226,15 @@
   auto d = Dune::UnitVector<double, 2>(Eigen::Vector2d::UnitX());
   d.update(Eigen::Vector<double, 1>::Ones());
   auto fvLambda = [](auto&& xL) { return f3R(xL); };
 
   auto dfvLambda  = [](auto&& xL) { return df3R(xL); };
   auto ddfvLambda = [](auto&& xL) { return ddf3R(xL); };
 
-  Ikarus::NonLinearOperator nonLinOp(linearAlgebraFunctions(fvLambda, dfvLambda, ddfvLambda), parameter(d));
+  Ikarus::NonLinearOperator nonLinOp(functions(fvLambda, dfvLambda, ddfvLambda), parameter(d));
   t.check(Dune::FloatCmp::eq(nonLinOp.value(), fvLambda(d))) << "Nonlinear operator and lambda have different value";
 
   t.check(isApproxSame(dfvLambda(d), nonLinOp.derivative(), 1e-15))
       << "Nonlinear operator derivative and lambda have different value";
   t.check(isApproxSame(ddfvLambda(d), nonLinOp.secondDerivative(), 1e-15))
       << "Nonlinear operator second derivative and lambda have different value";
 
@@ -404,15 +404,15 @@
   auto gred = dfvLambda(mT);
   t.check(10 == gred.size());
   auto ddfvLambda = [](auto&& xL) { return ddf3RBlocked(xL); };
   auto h          = ddfvLambda(mT);
   t.check(10 == h.rows());
   t.check(10 == h.cols());
 
-  Ikarus::NonLinearOperator nonLinOp(linearAlgebraFunctions(fvLambda, dfvLambda, ddfvLambda), parameter(mT));
+  Ikarus::NonLinearOperator nonLinOp(functions(fvLambda, dfvLambda, ddfvLambda), parameter(mT));
   t.check(Dune::FloatCmp::eq(nonLinOp.value(), fvLambda(mT)));
 
   t.check(isApproxSame(dfvLambda(mT), nonLinOp.derivative(), 1e-15));
   t.check(isApproxSame(ddfvLambda(mT), nonLinOp.secondDerivative(), 1e-15));
 
   Ikarus::TrustRegion tr3(nonLinOp);
   constexpr double tol = 1e-12;
```

