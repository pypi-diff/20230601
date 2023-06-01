# Comparing `tmp/pyikarus-0.3.3.dev20230523103500.tar.gz` & `tmp/pyikarus-0.3.3.dev20230601114417.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyikarus-0.3.3.dev20230523103500.tar", last modified: Tue May 23 10:35:00 2023, max compression
+gzip compressed data, was "pyikarus-0.3.3.dev20230601114417.tar", last modified: Thu Jun  1 11:44:17 2023, max compression
```

## Comparing `pyikarus-0.3.3.dev20230523103500.tar` & `pyikarus-0.3.3.dev20230601114417.tar`

### file list

```diff
@@ -1,331 +1,331 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.859768 pyikarus-0.3.3.dev20230523103500/
--rw-r--r--   0 root         (0) root         (0)      312 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.bettercodehub.yml
--rw-r--r--   0 root         (0) root         (0)     1300 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.clang-format
--rw-r--r--   0 root         (0) root         (0)     1017 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.cmake-format
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.779763 pyikarus-0.3.3.dev20230523103500/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.795764 pyikarus-0.3.3.dev20230523103500/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)      460 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 root         (0) root         (0)      615 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.799764 pyikarus-0.3.3.dev20230523103500/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/codespell.yml
--rw-r--r--   0 root         (0) root         (0)     1034 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/createDockerContainer.yml
--rw-r--r--   0 root         (0) root         (0)     5615 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/createRelease.yml
--rw-r--r--   0 root         (0) root         (0)     1834 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/debian-coverage.yml
--rw-r--r--   0 root         (0) root         (0)     2612 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/debian.yml
--rw-r--r--   0 root         (0) root         (0)     2042 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/ghpages.yml
--rw-r--r--   0 root         (0) root         (0)     1712 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/releasePythonPackage.yml
--rw-r--r--   0 root         (0) root         (0)      314 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/reuseLint.yml
--rw-r--r--   0 root         (0) root         (0)     3045 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/runExamples.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.799764 pyikarus-0.3.3.dev20230523103500/.github/workflows/scripts/
--rw-r--r--   0 root         (0) root         (0)     3071 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/scripts/release.py
--rw-r--r--   0 root         (0) root         (0)     1331 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.github/workflows/style.yml
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.799764 pyikarus-0.3.3.dev20230523103500/.reuse/
--rw-r--r--   0 root         (0) root         (0)      661 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/.reuse/dep5
--rw-r--r--   0 root         (0) root         (0)     3440 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)     1251 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5335 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/CODE_OF_CONDUCT.md
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/LICENSE.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.799764 pyikarus-0.3.3.dev20230523103500/LICENSES/
--rw-r--r--   0 root         (0) root         (0)    18375 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/LICENSES/CC-BY-SA-4.0.txt
--rw-r--r--   0 root         (0) root         (0)     7048 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/LICENSES/CC0-1.0.txt
--rw-r--r--   0 root         (0) root         (0)    42098 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/LICENSES/LGPL-3.0-or-later.txt
--rw-r--r--   0 root         (0) root         (0)     1078 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/LICENSES/MIT.txt
--rw-r--r--   0 root         (0) root         (0)    16727 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/LICENSES/MPL-2.0.txt
--rw-r--r--   0 root         (0) root         (0)     3732 2023-05-23 10:35:00.855767 pyikarus-0.3.3.dev20230523103500/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3321 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.803764 pyikarus-0.3.3.dev20230523103500/cmake/
--rw-r--r--   0 root         (0) root         (0)      184 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/cmake/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      973 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/cmake/CPM.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.803764 pyikarus-0.3.3.dev20230523103500/cmake/FormatTarget/
--rw-r--r--   0 root         (0) root         (0)     1875 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/cmake/FormatTarget/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.803764 pyikarus-0.3.3.dev20230523103500/cmake/modules/
--rw-r--r--   0 root         (0) root         (0)      715 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/cmake/modules/AddAutoDiffFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      683 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/cmake/modules/AddEigenFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      740 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/cmake/modules/AddMatplotppFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      691 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/cmake/modules/AddSpdlogFlags.cmake
--rw-r--r--   0 root         (0) root         (0)      325 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/cmake/modules/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      379 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/cmake/modules/IkarusMacros.cmake
--rw-r--r--   0 root         (0) root         (0)     2040 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/cmake/tools.cmake
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/codecov.yml
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/codespellignore
--rw-r--r--   0 root         (0) root         (0)     1588 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/config.h.cmake
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.807764 pyikarus-0.3.3.dev20230523103500/docs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.807764 pyikarus-0.3.3.dev20230523103500/docs/BuildLocally/
--rw-r--r--   0 root         (0) root         (0)      439 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/BuildLocally/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      333 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.807764 pyikarus-0.3.3.dev20230523103500/docs/__pycache__/
--rw-r--r--   0 root         (0) root         (0)     1136 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/__pycache__/mkdocs-macros.cpython-39.pyc
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
--rw-r--r--   0 root         (0) root         (0)     6961 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/literature.bib
--rw-r--r--   0 root         (0) root         (0)      117 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/literature.bib.license
--rw-r--r--   0 root         (0) root         (0)     1271 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/mkdocs-macros.py
--rw-r--r--   0 root         (0) root         (0)      395 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/mkdocs.insiders.yml
--rw-r--r--   0 root         (0) root         (0)     5042 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/mkdocs.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.783763 pyikarus-0.3.3.dev20230523103500/docs/overrides/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.807764 pyikarus-0.3.3.dev20230523103500/docs/overrides/partials/
--rw-r--r--   0 root         (0) root         (0)     1732 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/overrides/partials/comments.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.807764 pyikarus-0.3.3.dev20230523103500/docs/website/
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/.meta.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.811765 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/
--rw-r--r--   0 root         (0) root         (0)     4710 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/assembler.md
--rw-r--r--   0 root         (0) root         (0)     6387 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/controlRoutines.md
--rw-r--r--   0 root         (0) root         (0)     2024 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/dirichletBCs.md
--rw-r--r--   0 root         (0) root         (0)     3237 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/feRequirements.md
--rw-r--r--   0 root         (0) root         (0)     8524 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/finiteElements.md
--rw-r--r--   0 root         (0) root         (0)     2745 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/grids.md
--rw-r--r--   0 root         (0) root         (0)     4121 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/index.md
--rw-r--r--   0 root         (0) root         (0)     4932 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/localBasis.md
--rw-r--r--   0 root         (0) root         (0)    44213 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/localFunctions.md
--rw-r--r--   0 root         (0) root         (0)     3978 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/manifolds.md
--rw-r--r--   0 root         (0) root         (0)     2590 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/nonlinearOperator.md
--rw-r--r--   0 root         (0) root         (0)     3086 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/observer.md
--rw-r--r--   0 root         (0) root         (0)     5211 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/solvers.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.811765 pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/
--rw-r--r--   0 root         (0) root         (0)     6655 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/cantileverBeam.md
--rw-r--r--   0 root         (0) root         (0)     7251 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/computePi.md
--rw-r--r--   0 root         (0) root         (0)     5439 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/cooksMembrane.md
--rw-r--r--   0 root         (0) root         (0)     7055 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/incompressibleRubberBlock.md
--rw-r--r--   0 root         (0) root         (0)     2164 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/index.md
--rw-r--r--   0 root         (0) root         (0)     7702 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/kirchhoffPlate.md
--rw-r--r--   0 root         (0) root         (0)     5114 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/newtonRaphsonMethod.md
--rw-r--r--   0 root         (0) root         (0)     6200 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/nonLinearElasticity.md
--rw-r--r--   0 root         (0) root         (0)     4071 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/vonMisesTruss.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.815765 pyikarus-0.3.3.dev20230523103500/docs/website/03_contribution/
--rw-r--r--   0 root         (0) root         (0)     2439 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/03_contribution/buildDocumentationLocally.md
--rw-r--r--   0 root         (0) root         (0)     1002 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/03_contribution/codeStyle.md
--rw-r--r--   0 root         (0) root         (0)     2415 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/03_contribution/howToEdit.md
--rw-r--r--   0 root         (0) root         (0)     1696 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/03_contribution/openTask.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.815765 pyikarus-0.3.3.dev20230523103500/docs/website/04_blog/
--rw-r--r--   0 root         (0) root         (0)      274 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/04_blog/.authors.yml
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/04_blog/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.815765 pyikarus-0.3.3.dev20230523103500/docs/website/04_blog/posts/
--rw-r--r--   0 root         (0) root         (0)     7731 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/04_blog/posts/v0.3.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.815765 pyikarus-0.3.3.dev20230523103500/docs/website/05_cppReferences/
--rw-r--r--   0 root         (0) root         (0)     2324 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/05_cppReferences/cppRef.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.815765 pyikarus-0.3.3.dev20230523103500/docs/website/99_Literature/
--rw-r--r--   0 root         (0) root         (0)      169 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/99_Literature/99_Literature.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.815765 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.819765 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/
--rw-r--r--   0 root         (0) root         (0)    52795 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
--rw-r--r--   0 root         (0) root         (0)    46250 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/CMakeOutput.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
--rw-r--r--   0 root         (0) root         (0)     2852 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/ClionFooter.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
--rw-r--r--   0 root         (0) root         (0)    17924 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
--rw-r--r--   0 root         (0) root         (0)     9455 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.819765 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/
--rw-r--r--   0 root         (0) root         (0)    35234 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
--rw-r--r--   0 root         (0) root         (0)    62184 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
--rw-r--r--   0 root         (0) root         (0)     2281 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
--rw-r--r--   0 root         (0) root         (0)    40033 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
--rw-r--r--   0 root         (0) root         (0)    25505 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
--rw-r--r--   0 root         (0) root         (0)     8101 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/logo_blue.svg
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/logo_blue.svg.license
--rw-r--r--   0 root         (0) root         (0)     8255 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/logo_white.svg
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/logo_white.svg.license
--rw-r--r--   0 root         (0) root         (0)     4364 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/download.md
--rw-r--r--   0 root         (0) root         (0)      244 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/gallery.md
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/index.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.819765 pyikarus-0.3.3.dev20230523103500/docs/website/javascripts/
--rw-r--r--   0 root         (0) root         (0)      486 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/javascripts/mathjax.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.823765 pyikarus-0.3.3.dev20230523103500/docs/website/stylesheets/
--rw-r--r--   0 root         (0) root         (0)      302 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/docs/website/stylesheets/extra.css
--rw-r--r--   0 root         (0) root         (0)      504 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/dune.module
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.823765 pyikarus-0.3.3.dev20230523103500/ikarus/
--rw-r--r--   0 root         (0) root         (0)      743 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.823765 pyikarus-0.3.3.dev20230523103500/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      268 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    12924 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/assembler/simpleAssemblers.hh
--rw-r--r--   0 root         (0) root         (0)    10714 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/assembler/simpleAssemblers.inl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.823765 pyikarus-0.3.3.dev20230523103500/ikarus/controlRoutines/
--rw-r--r--   0 root         (0) root         (0)      239 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/controlRoutines/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2575 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/controlRoutines/loadControl.hh
--rw-r--r--   0 root         (0) root         (0)     2970 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/controlRoutines/pathFollowingTechnique.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.823765 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      349 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/fEparameter.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.823765 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feBases/
--rw-r--r--   0 root         (0) root         (0)      282 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feBases/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2942 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feBases/autodiffFE.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feBases/powerBasisFE.hh
--rw-r--r--   0 root         (0) root         (0)     1827 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feBases/scalarFE.hh
--rw-r--r--   0 root         (0) root         (0)     9346 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feRequirements.hh
--rw-r--r--   0 root         (0) root         (0)     1338 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feTraits.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.827766 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/
--rw-r--r--   0 root         (0) root         (0)      345 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)    19446 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
--rw-r--r--   0 root         (0) root         (0)    12479 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.827766 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/
--rw-r--r--   0 root         (0) root         (0)      397 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5699 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/interface.hh
--rw-r--r--   0 root         (0) root         (0)     2718 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
--rw-r--r--   0 root         (0) root         (0)     4635 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/neohooke.hh
--rw-r--r--   0 root         (0) root         (0)     3809 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/strainConversions.hh
--rw-r--r--   0 root         (0) root         (0)     5734 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/svk.hh
--rw-r--r--   0 root         (0) root         (0)      473 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/tags.hh
--rw-r--r--   0 root         (0) root         (0)     8008 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
--rw-r--r--   0 root         (0) root         (0)     1196 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials.hh
--rw-r--r--   0 root         (0) root         (0)     9574 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/nonLinearElastic.hh
--rw-r--r--   0 root         (0) root         (0)    12655 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/physicsHelper.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.827766 pyikarus-0.3.3.dev20230523103500/ikarus/io/
--rw-r--r--   0 root         (0) root         (0)      258 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/io/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     2351 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/io/resultEvaluators.hh
--rw-r--r--   0 root         (0) root         (0)     3829 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/io/resultFunction.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.831766 pyikarus-0.3.3.dev20230523103500/ikarus/linearAlgebra/
--rw-r--r--   0 root         (0) root         (0)      301 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/linearAlgebra/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6735 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/linearAlgebra/dirichletValues.hh
--rw-r--r--   0 root         (0) root         (0)     7789 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/linearAlgebra/nonLinearOperator.hh
--rw-r--r--   0 root         (0) root         (0)    12303 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/linearAlgebra/truncatedConjugateGradient.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.831766 pyikarus-0.3.3.dev20230523103500/ikarus/python/
--rw-r--r--   0 root         (0) root         (0)      294 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.831766 pyikarus-0.3.3.dev20230523103500/ikarus/python/assembler/
--rw-r--r--   0 root         (0) root         (0)      249 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     6752 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/assembler/flatAssembler.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.831766 pyikarus-0.3.3.dev20230523103500/ikarus/python/basis/
--rw-r--r--   0 root         (0) root         (0)      237 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/basis/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1469 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/basis/basis.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.831766 pyikarus-0.3.3.dev20230523103500/ikarus/python/dirichletValues/
--rw-r--r--   0 root         (0) root         (0)      257 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/dirichletValues/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     4169 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/dirichletValues/dirichletValues.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.831766 pyikarus-0.3.3.dev20230523103500/ikarus/python/finiteElements/
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/finiteElements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5220 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/finiteElements/linearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.831766 pyikarus-0.3.3.dev20230523103500/ikarus/python/finiteElements/materials/
--rw-r--r--   0 root         (0) root         (0)      268 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/finiteElements/materials/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     9949 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/finiteElements/materials/material.hh
--rw-r--r--   0 root         (0) root         (0)     5518 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/finiteElements/nonLinearElastic.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.831766 pyikarus-0.3.3.dev20230523103500/ikarus/python/test/
--rw-r--r--   0 root         (0) root         (0)      511 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/test/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3830 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/test/linearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)     4481 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/test/nonLinearElasticTest.py
--rw-r--r--   0 root         (0) root         (0)      862 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/test/setpath.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.835766 pyikarus-0.3.3.dev20230523103500/ikarus/python/utils/
--rw-r--r--   0 root         (0) root         (0)      245 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1185 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/python/utils/boundarypatch.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.835766 pyikarus-0.3.3.dev20230523103500/ikarus/solver/
--rw-r--r--   0 root         (0) root         (0)      211 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/solver/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.835766 pyikarus-0.3.3.dev20230523103500/ikarus/solver/linearSolver/
--rw-r--r--   0 root         (0) root         (0)      244 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/solver/linearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     8891 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/solver/linearSolver/linearSolver.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.835766 pyikarus-0.3.3.dev20230523103500/ikarus/solver/nonLinearSolver/
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/solver/nonLinearSolver/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     5406 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/solver/nonLinearSolver/newtonRaphson.hh
--rw-r--r--   0 root         (0) root         (0)     8297 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
--rw-r--r--   0 root         (0) root         (0)    18574 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/solver/nonLinearSolver/trustRegion.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.843767 pyikarus-0.3.3.dev20230523103500/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      712 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1741 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/algorithms.hh
--rw-r--r--   0 root         (0) root         (0)      878 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/autodiffHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1469 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/basis.hh
--rw-r--r--   0 root         (0) root         (0)     6930 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/concepts.hh
--rw-r--r--   0 root         (0) root         (0)      499 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/defaultFunctions.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.843767 pyikarus-0.3.3.dev20230523103500/ikarus/utils/drawing/
--rw-r--r--   0 root         (0) root         (0)      262 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/drawing/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1654 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/drawing/griddrawer.hh
--rw-r--r--   0 root         (0) root         (0)      544 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/drawing/matplotHelper.cpp
--rw-r--r--   0 root         (0) root         (0)      703 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/drawing/matplotHelper.hh
--rw-r--r--   0 root         (0) root         (0)     2484 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/duneUtilities.hh
--rw-r--r--   0 root         (0) root         (0)     2347 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/eigenDuneTransformations.hh
--rw-r--r--   0 root         (0) root         (0)      682 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/eigenSparseAddon.hh
--rw-r--r--   0 root         (0) root         (0)     1367 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/findLineSegment.cpp
--rw-r--r--   0 root         (0) root         (0)      724 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/findLineSegment.hh
--rw-r--r--   0 root         (0) root         (0)     3611 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/flatPreBasis.hh
--rw-r--r--   0 root         (0) root         (0)     2171 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/functionSanityChecks.cpp
--rw-r--r--   0 root         (0) root         (0)     6359 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/functionSanityChecks.hh
--rw-r--r--   0 root         (0) root         (0)     3152 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/init.hh
--rw-r--r--   0 root         (0) root         (0)    15244 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/linearAlgebraHelper.hh
--rw-r--r--   0 root         (0) root         (0)     1711 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/makeEnum.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.843767 pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/
--rw-r--r--   0 root         (0) root         (0)      450 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1554 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/controlLogger.hh
--rw-r--r--   0 root         (0) root         (0)     2307 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/controlVTKWriter.hh
--rw-r--r--   0 root         (0) root         (0)      905 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/genericControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1053 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/gridDrawerObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1132 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/loadControlObserver.hh
--rw-r--r--   0 root         (0) root         (0)     1985 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/nonLinearSolverLogger.hh
--rw-r--r--   0 root         (0) root         (0)     5497 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/observer.hh
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/observerMessages.hh
--rw-r--r--   0 root         (0) root         (0)     4159 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/pathFollowingFunctions.hh
--rw-r--r--   0 root         (0) root         (0)     1131 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/polyfit.cpp
--rw-r--r--   0 root         (0) root         (0)      570 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/polyfit.hh
--rw-r--r--   0 root         (0) root         (0)    10054 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/tensorUtils.hh
--rw-r--r--   0 root         (0) root         (0)    15044 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/ikarus/utils/traits.hh
--rw-r--r--   0 root         (0) root         (0)      432 2023-05-23 10:34:51.000000 pyikarus-0.3.3.dev20230523103500/ikarus.pc.in
--rw-r--r--   0 root         (0) root         (0)      196 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/iwyu.imp
--rw-r--r--   0 root         (0) root         (0)      422 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.843767 pyikarus-0.3.3.dev20230523103500/python/
--rw-r--r--   0 root         (0) root         (0)      423 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.847767 pyikarus-0.3.3.dev20230523103500/python/ikarus/
--rw-r--r--   0 root         (0) root         (0)      500 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      603 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5650 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/_ikarus.cc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.847767 pyikarus-0.3.3.dev20230523103500/python/ikarus/assembler/
--rw-r--r--   0 root         (0) root         (0)      167 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/assembler/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     1628 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/assembler/__init__.py
--rw-r--r--   0 root         (0) root         (0)      790 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/basis.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/dirichletValues.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.847767 pyikarus-0.3.3.dev20230523103500/python/ikarus/finite_elements/
--rw-r--r--   0 root         (0) root         (0)      173 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/finite_elements/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3119 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/finite_elements/__init__.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/generator.py
--rw-r--r--   0 root         (0) root         (0)     1052 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/materials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.847767 pyikarus-0.3.3.dev20230523103500/python/ikarus/utils/
--rw-r--r--   0 root         (0) root         (0)      163 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/utils/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)      768 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/ikarus/utils/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.847767 pyikarus-0.3.3.dev20230523103500/python/pyikarus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3732 2023-05-23 10:35:00.000000 pyikarus-0.3.3.dev20230523103500/python/pyikarus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10022 2023-05-23 10:35:00.000000 pyikarus-0.3.3.dev20230523103500/python/pyikarus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 10:35:00.000000 pyikarus-0.3.3.dev20230523103500/python/pyikarus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      119 2023-05-23 10:35:00.000000 pyikarus-0.3.3.dev20230523103500/python/pyikarus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-23 10:35:00.000000 pyikarus-0.3.3.dev20230523103500/python/pyikarus.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      632 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/python/setup.py.in
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.847767 pyikarus-0.3.3.dev20230523103500/sandbox/
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/sandbox/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.851767 pyikarus-0.3.3.dev20230523103500/sandbox/src/
--rw-r--r--   0 root         (0) root         (0)     1220 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/sandbox/src/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.851767 pyikarus-0.3.3.dev20230523103500/sandbox/src/auxiliaryFiles/
--rw-r--r--   0 root         (0) root         (0)   674469 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/sandbox/src/auxiliaryFiles/circle.msh
--rw-r--r--   0 root         (0) root         (0)      320 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/sandbox/src/sandbox.cpp
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 10:35:00.859768 pyikarus-0.3.3.dev20230523103500/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1080 2023-05-23 10:35:00.000000 pyikarus-0.3.3.dev20230523103500/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.851767 pyikarus-0.3.3.dev20230523103500/tests/
--rw-r--r--   0 root         (0) root         (0)      150 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/CMakeLists.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.855767 pyikarus-0.3.3.dev20230523103500/tests/src/
--rw-r--r--   0 root         (0) root         (0)     1408 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/CMakeLists.txt
--rw-r--r--   0 root         (0) root         (0)     3907 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/assemblerTest.cpp
--rw-r--r--   0 root         (0) root         (0)     9842 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/common.hh
--rw-r--r--   0 root         (0) root         (0)     2639 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/dependenciesTest.cpp
--rw-r--r--   0 root         (0) root         (0)     6520 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/dirichletValueTest.cpp
--rw-r--r--   0 root         (0) root         (0)     4594 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/easTest.hh
--rw-r--r--   0 root         (0) root         (0)     1473 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/enhancedAssumedStrainsTest.cpp
--rw-r--r--   0 root         (0) root         (0)      608 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/factories.hh
--rw-r--r--   0 root         (0) root         (0)     1870 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/functionTraitsTest.cpp
--rw-r--r--   0 root         (0) root         (0)     2661 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/linearElasticityTest.cpp
--rw-r--r--   0 root         (0) root         (0)     2378 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/manifoldsTest.cpp
--rw-r--r--   0 root         (0) root         (0)     7961 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/materialTest.cpp
--rw-r--r--   0 root         (0) root         (0)     9330 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/nonLinearElasticityTest.hh
--rw-r--r--   0 root         (0) root         (0)      724 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/nonLinearElasticityTestNeoHooke.cpp
--rw-r--r--   0 root         (0) root         (0)      829 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/nonLinearElasticityTestSVK.cpp
--rw-r--r--   0 root         (0) root         (0)     9936 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/nonLinearOperatorTest.cpp
--rw-r--r--   0 root         (0) root         (0)     6327 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/pathFollowingTest.cpp
--rw-r--r--   0 root         (0) root         (0)     1651 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/polyFitTest.cpp
--rw-r--r--   0 root         (0) root         (0)      695 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/pythonConversionTest.cpp
--rw-r--r--   0 root         (0) root         (0)     1292 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/testAutodiffHelper.cpp
--rw-r--r--   0 root         (0) root         (0)     6143 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/testFEElement.hh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 10:35:00.855767 pyikarus-0.3.3.dev20230523103500/tests/src/testFiles/
--rw-r--r--   0 root         (0) root         (0)     9028 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/testFiles/unstructuredQuadscoarse.msh
--rw-r--r--   0 root         (0) root         (0)      395 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/testFiles/unstructuredTest.geo
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/testFiles/unstructuredTest.msh
--rw-r--r--   0 root         (0) root         (0)      546 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/testFiles/unstructuredTest2.geo
--rw-r--r--   0 root         (0) root         (0)    11431 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/testFiles/unstructuredTrianglesfine.msh
--rw-r--r--   0 root         (0) root         (0)     1114 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/testHelpers.hh
--rw-r--r--   0 root         (0) root         (0)    17595 2023-05-23 10:34:52.000000 pyikarus-0.3.3.dev20230523103500/tests/src/trustRegionTest.cpp
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.967877 pyikarus-0.3.3.dev20230601114417/
+-rw-r--r--   0 root         (0) root         (0)      312 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.bettercodehub.yml
+-rw-r--r--   0 root         (0) root         (0)     1300 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.clang-format
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.cmake-format
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.911876 pyikarus-0.3.3.dev20230601114417/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.919876 pyikarus-0.3.3.dev20230601114417/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)      460 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      615 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/codespell.yml
+-rw-r--r--   0 root         (0) root         (0)     1034 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/createDockerContainer.yml
+-rw-r--r--   0 root         (0) root         (0)     5615 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/createRelease.yml
+-rw-r--r--   0 root         (0) root         (0)     1834 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/debian-coverage.yml
+-rw-r--r--   0 root         (0) root         (0)     2612 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/debian.yml
+-rw-r--r--   0 root         (0) root         (0)     2042 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/ghpages.yml
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/releasePythonPackage.yml
+-rw-r--r--   0 root         (0) root         (0)      314 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/reuseLint.yml
+-rw-r--r--   0 root         (0) root         (0)     3335 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/runExamples.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/.github/workflows/scripts/
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/scripts/release.py
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.github/workflows/style.yml
+-rw-r--r--   0 root         (0) root         (0)      482 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/.reuse/
+-rw-r--r--   0 root         (0) root         (0)      661 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/.reuse/dep5
+-rw-r--r--   0 root         (0) root         (0)     3707 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5335 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/CODE_OF_CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)      784 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/LICENSES/
+-rw-r--r--   0 root         (0) root         (0)    18375 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSES/CC-BY-SA-4.0.txt
+-rw-r--r--   0 root         (0) root         (0)     7048 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSES/CC0-1.0.txt
+-rw-r--r--   0 root         (0) root         (0)    42098 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSES/LGPL-3.0-or-later.txt
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSES/MIT.txt
+-rw-r--r--   0 root         (0) root         (0)    16727 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/LICENSES/MPL-2.0.txt
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-06-01 11:44:17.967877 pyikarus-0.3.3.dev20230601114417/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3321 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/cmake/
+-rw-r--r--   0 root         (0) root         (0)      184 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      973 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/CPM.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.923876 pyikarus-0.3.3.dev20230601114417/cmake/FormatTarget/
+-rw-r--r--   0 root         (0) root         (0)     1807 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/FormatTarget/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/cmake/modules/
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/AddAutoDiffFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      683 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/AddEigenFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/AddMatplotppFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/AddSpdlogFlags.cmake
+-rw-r--r--   0 root         (0) root         (0)      325 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      379 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/modules/IkarusMacros.cmake
+-rw-r--r--   0 root         (0) root         (0)     2040 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/cmake/tools.cmake
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/codecov.yml
+-rw-r--r--   0 root         (0) root         (0)      121 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/codespellignore
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/config.h.cmake
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/docs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/docs/BuildLocally/
+-rw-r--r--   0 root         (0) root         (0)      439 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/BuildLocally/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/docs/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     1136 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/__pycache__/mkdocs-macros.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/__pycache__/mkdocs-macros.cpython-39.pyc.license
+-rw-r--r--   0 root         (0) root         (0)     6961 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/literature.bib
+-rw-r--r--   0 root         (0) root         (0)      117 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/literature.bib.license
+-rw-r--r--   0 root         (0) root         (0)     1271 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/mkdocs-macros.py
+-rw-r--r--   0 root         (0) root         (0)      398 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/mkdocs.insiders.yml
+-rw-r--r--   0 root         (0) root         (0)     5042 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/mkdocs.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.911876 pyikarus-0.3.3.dev20230601114417/docs/overrides/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/docs/overrides/partials/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/overrides/partials/comments.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.927876 pyikarus-0.3.3.dev20230601114417/docs/website/
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/.meta.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/
+-rw-r--r--   0 root         (0) root         (0)     4710 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/assembler.md
+-rw-r--r--   0 root         (0) root         (0)     6387 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/controlRoutines.md
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/dirichletBCs.md
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/feRequirements.md
+-rw-r--r--   0 root         (0) root         (0)    12894 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/finiteElements.md
+-rw-r--r--   0 root         (0) root         (0)     2745 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/grids.md
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/index.md
+-rw-r--r--   0 root         (0) root         (0)     4932 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/localBasis.md
+-rw-r--r--   0 root         (0) root         (0)    44213 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/localFunctions.md
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/manifolds.md
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/nonlinearOperator.md
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/observer.md
+-rw-r--r--   0 root         (0) root         (0)     5211 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/solvers.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/
+-rw-r--r--   0 root         (0) root         (0)     6655 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/cantileverBeam.md
+-rw-r--r--   0 root         (0) root         (0)     7251 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/computePi.md
+-rw-r--r--   0 root         (0) root         (0)     5439 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/cooksMembrane.md
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/incompressibleRubberBlock.md
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/index.md
+-rw-r--r--   0 root         (0) root         (0)     7774 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/kirchhoffPlate.md
+-rw-r--r--   0 root         (0) root         (0)     5114 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/newtonRaphsonMethod.md
+-rw-r--r--   0 root         (0) root         (0)     6177 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/nonLinearElasticity.md
+-rw-r--r--   0 root         (0) root         (0)     4179 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/vonMisesTruss.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/buildDocumentationLocally.md
+-rw-r--r--   0 root         (0) root         (0)     1002 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/codeStyle.md
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/howToEdit.md
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/openTask.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/.authors.yml
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/posts/
+-rw-r--r--   0 root         (0) root         (0)     7731 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/posts/v0.3.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/05_cppReferences/
+-rw-r--r--   0 root         (0) root         (0)     2324 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/05_cppReferences/cppRef.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.931876 pyikarus-0.3.3.dev20230601114417/docs/website/99_Literature/
+-rw-r--r--   0 root         (0) root         (0)      169 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/99_Literature/99_Literature.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.935876 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.935876 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/
+-rw-r--r--   0 root         (0) root         (0)    52795 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)    46250 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CMakeOutput.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CMakeOutput.png.license
+-rw-r--r--   0 root         (0) root         (0)     2852 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ClionFooter.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ClionFooter.png.license
+-rw-r--r--   0 root         (0) root         (0)    17924 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/DockerWslSettings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/DockerWslSettings.png.license
+-rw-r--r--   0 root         (0) root         (0)     9455 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png.license
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/
+-rw-r--r--   0 root         (0) root         (0)    35234 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png.license
+-rw-r--r--   0 root         (0) root         (0)    62184 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png.license
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png.license
+-rw-r--r--   0 root         (0) root         (0)    40033 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png.license
+-rw-r--r--   0 root         (0) root         (0)    25505 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png.license
+-rw-r--r--   0 root         (0) root         (0)     8101 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_blue.svg
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_blue.svg.license
+-rw-r--r--   0 root         (0) root         (0)     8255 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_white.svg
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_white.svg.license
+-rw-r--r--   0 root         (0) root         (0)     4364 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/download.md
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/gallery.md
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/index.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/docs/website/javascripts/
+-rw-r--r--   0 root         (0) root         (0)      486 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/javascripts/mathjax.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/docs/website/stylesheets/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/docs/website/stylesheets/extra.css
+-rw-r--r--   0 root         (0) root         (0)      504 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/dune.module
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      743 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    12924 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/assembler/simpleAssemblers.hh
+-rw-r--r--   0 root         (0) root         (0)    10714 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/assembler/simpleAssemblers.inl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/
+-rw-r--r--   0 root         (0) root         (0)      239 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2575 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/loadControl.hh
+-rw-r--r--   0 root         (0) root         (0)     2970 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/pathFollowingTechnique.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/fEparameter.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.939876 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/
+-rw-r--r--   0 root         (0) root         (0)      282 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5311 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/autodiffFE.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/powerBasisFE.hh
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/scalarFE.hh
+-rw-r--r--   0 root         (0) root         (0)     9346 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feRequirements.hh
+-rw-r--r--   0 root         (0) root         (0)     1338 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feTraits.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/
+-rw-r--r--   0 root         (0) root         (0)      345 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)    21360 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh
+-rw-r--r--   0 root         (0) root         (0)    13674 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/
+-rw-r--r--   0 root         (0) root         (0)      397 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5699 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/interface.hh
+-rw-r--r--   0 root         (0) root         (0)     2718 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/linearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/neohooke.hh
+-rw-r--r--   0 root         (0) root         (0)     3809 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/strainConversions.hh
+-rw-r--r--   0 root         (0) root         (0)     5734 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/svk.hh
+-rw-r--r--   0 root         (0) root         (0)      473 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/tags.hh
+-rw-r--r--   0 root         (0) root         (0)     8008 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/vanishingStress.hh
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials.hh
+-rw-r--r--   0 root         (0) root         (0)    15536 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/nonLinearElastic.hh
+-rw-r--r--   0 root         (0) root         (0)    12678 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/physicsHelper.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/io/
+-rw-r--r--   0 root         (0) root         (0)      258 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/io/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/io/resultEvaluators.hh
+-rw-r--r--   0 root         (0) root         (0)     3829 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/io/resultFunction.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6735 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/dirichletValues.hh
+-rw-r--r--   0 root         (0) root         (0)     7789 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/nonLinearOperator.hh
+-rw-r--r--   0 root         (0) root         (0)    12303 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/truncatedConjugateGradient.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/python/
+-rw-r--r--   0 root         (0) root         (0)      294 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/python/assembler/
+-rw-r--r--   0 root         (0) root         (0)      249 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     6752 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/assembler/flatAssembler.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/python/basis/
+-rw-r--r--   0 root         (0) root         (0)      237 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/basis/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/basis/basis.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.943877 pyikarus-0.3.3.dev20230601114417/ikarus/python/dirichletValues/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/dirichletValues/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     4169 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/dirichletValues/dirichletValues.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/
+-rw-r--r--   0 root         (0) root         (0)      303 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5220 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/linearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/materials/
+-rw-r--r--   0 root         (0) root         (0)      268 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/materials/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     9949 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/materials/material.hh
+-rw-r--r--   0 root         (0) root         (0)     5207 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/nonLinearElastic.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/python/test/
+-rw-r--r--   0 root         (0) root         (0)      511 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/test/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/test/linearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)     4340 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/test/nonLinearElasticTest.py
+-rw-r--r--   0 root         (0) root         (0)      862 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/test/setpath.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/python/utils/
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/python/utils/boundarypatch.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/solver/
+-rw-r--r--   0 root         (0) root         (0)      211 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/solver/linearSolver/
+-rw-r--r--   0 root         (0) root         (0)      244 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/linearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     8891 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/linearSolver/linearSolver.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.947877 pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     5406 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/newtonRaphson.hh
+-rw-r--r--   0 root         (0) root         (0)     8297 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh
+-rw-r--r--   0 root         (0) root         (0)    18574 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/trustRegion.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.951877 pyikarus-0.3.3.dev20230601114417/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      712 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/algorithms.hh
+-rw-r--r--   0 root         (0) root         (0)      878 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/autodiffHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1469 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/basis.hh
+-rw-r--r--   0 root         (0) root         (0)     6930 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/concepts.hh
+-rw-r--r--   0 root         (0) root         (0)      499 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/defaultFunctions.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.955877 pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/
+-rw-r--r--   0 root         (0) root         (0)      262 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1654 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/griddrawer.hh
+-rw-r--r--   0 root         (0) root         (0)      544 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/matplotHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)      703 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/matplotHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     2484 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/duneUtilities.hh
+-rw-r--r--   0 root         (0) root         (0)     2347 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/eigenDuneTransformations.hh
+-rw-r--r--   0 root         (0) root         (0)      682 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/eigenSparseAddon.hh
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/findLineSegment.cpp
+-rw-r--r--   0 root         (0) root         (0)      724 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/findLineSegment.hh
+-rw-r--r--   0 root         (0) root         (0)     3611 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/flatPreBasis.hh
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/functionSanityChecks.cpp
+-rw-r--r--   0 root         (0) root         (0)     6359 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/functionSanityChecks.hh
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/init.hh
+-rw-r--r--   0 root         (0) root         (0)    15244 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/linearAlgebraHelper.hh
+-rw-r--r--   0 root         (0) root         (0)     1711 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/makeEnum.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.955877 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/
+-rw-r--r--   0 root         (0) root         (0)      450 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/controlLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     2307 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/controlVTKWriter.hh
+-rw-r--r--   0 root         (0) root         (0)      905 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/genericControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/gridDrawerObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/loadControlObserver.hh
+-rw-r--r--   0 root         (0) root         (0)     1985 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/nonLinearSolverLogger.hh
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/observer.hh
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/observerMessages.hh
+-rw-r--r--   0 root         (0) root         (0)     4159 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/pathFollowingFunctions.hh
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/polyfit.cpp
+-rw-r--r--   0 root         (0) root         (0)      570 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/polyfit.hh
+-rw-r--r--   0 root         (0) root         (0)    10054 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/tensorUtils.hh
+-rw-r--r--   0 root         (0) root         (0)    15149 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus/utils/traits.hh
+-rw-r--r--   0 root         (0) root         (0)      432 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/ikarus.pc.in
+-rw-r--r--   0 root         (0) root         (0)      196 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/iwyu.imp
+-rw-r--r--   0 root         (0) root         (0)      422 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.955877 pyikarus-0.3.3.dev20230601114417/python/
+-rw-r--r--   0 root         (0) root         (0)      423 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/python/ikarus/
+-rw-r--r--   0 root         (0) root         (0)      500 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      603 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5650 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/_ikarus.cc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/python/ikarus/assembler/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/assembler/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     1628 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/assembler/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      790 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/basis.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/dirichletValues.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/python/ikarus/finite_elements/
+-rw-r--r--   0 root         (0) root         (0)      173 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/finite_elements/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/finite_elements/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/generator.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/materials.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/python/ikarus/utils/
+-rw-r--r--   0 root         (0) root         (0)      163 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/utils/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)      768 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/ikarus/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3732 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10030 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      119 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      632 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/python/setup.py.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/sandbox/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/sandbox/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/sandbox/src/
+-rw-r--r--   0 root         (0) root         (0)     1220 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/sandbox/src/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/sandbox/src/auxiliaryFiles/
+-rw-r--r--   0 root         (0) root         (0)   674469 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/sandbox/src/auxiliaryFiles/circle.msh
+-rw-r--r--   0 root         (0) root         (0)      320 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/sandbox/src/sandbox.cpp
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-01 11:44:17.967877 pyikarus-0.3.3.dev20230601114417/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-06-01 11:44:17.000000 pyikarus-0.3.3.dev20230601114417/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.959877 pyikarus-0.3.3.dev20230601114417/tests/
+-rw-r--r--   0 root         (0) root         (0)      150 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/CMakeLists.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.963877 pyikarus-0.3.3.dev20230601114417/tests/src/
+-rw-r--r--   0 root         (0) root         (0)     1408 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/CMakeLists.txt
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testAssembler.cpp
+-rw-r--r--   0 root         (0) root         (0)     1292 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testAutodiffHelper.cpp
+-rw-r--r--   0 root         (0) root         (0)    14291 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testCommon.hh
+-rw-r--r--   0 root         (0) root         (0)     2639 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testDependencies.cpp
+-rw-r--r--   0 root         (0) root         (0)     6520 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testDirichletValue.cpp
+-rw-r--r--   0 root         (0) root         (0)     4795 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testEAS.hh
+-rw-r--r--   0 root         (0) root         (0)     1600 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testEnhancedAssumedStrains.cpp
+-rw-r--r--   0 root         (0) root         (0)     5818 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFEElement.hh
+-rw-r--r--   0 root         (0) root         (0)      571 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFactories.hh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-01 11:44:17.967877 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/
+-rw-r--r--   0 root         (0) root         (0)     9028 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredQuadscoarse.msh
+-rw-r--r--   0 root         (0) root         (0)      395 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTest.geo
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTest.msh
+-rw-r--r--   0 root         (0) root         (0)      546 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTest2.geo
+-rw-r--r--   0 root         (0) root         (0)    11431 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTrianglesfine.msh
+-rw-r--r--   0 root         (0) root         (0)     1870 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testFunctionTraits.cpp
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testHelpers.hh
+-rw-r--r--   0 root         (0) root         (0)     3190 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testLinearElasticity.cpp
+-rw-r--r--   0 root         (0) root         (0)     2278 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testManifolds.cpp
+-rw-r--r--   0 root         (0) root         (0)     7962 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testMaterial.cpp
+-rw-r--r--   0 root         (0) root         (0)    15896 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearElasticity.hh
+-rw-r--r--   0 root         (0) root         (0)      669 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearElasticityNeoHooke.cpp
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearElasticitySVK.cpp
+-rw-r--r--   0 root         (0) root         (0)     9937 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearOperator.cpp
+-rw-r--r--   0 root         (0) root         (0)     6327 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testPathFollowing.cpp
+-rw-r--r--   0 root         (0) root         (0)     1651 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testPolyFit.cpp
+-rw-r--r--   0 root         (0) root         (0)      696 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testPythonConversion.cpp
+-rw-r--r--   0 root         (0) root         (0)    17596 2023-06-01 11:44:09.000000 pyikarus-0.3.3.dev20230601114417/tests/src/testTrustRegion.cpp
```

### Comparing `pyikarus-0.3.3.dev20230523103500/.clang-format` & `pyikarus-0.3.3.dev20230601114417/.clang-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.cmake-format` & `pyikarus-0.3.3.dev20230601114417/.cmake-format`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.github/ISSUE_TEMPLATE/feature_request.md` & `pyikarus-0.3.3.dev20230601114417/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.github/workflows/createDockerContainer.yml` & `pyikarus-0.3.3.dev20230601114417/.github/workflows/createDockerContainer.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.github/workflows/createRelease.yml` & `pyikarus-0.3.3.dev20230601114417/.github/workflows/createRelease.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.github/workflows/debian-coverage.yml` & `pyikarus-0.3.3.dev20230601114417/.github/workflows/debian-coverage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.github/workflows/debian.yml` & `pyikarus-0.3.3.dev20230601114417/.github/workflows/debian.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.github/workflows/ghpages.yml` & `pyikarus-0.3.3.dev20230601114417/.github/workflows/ghpages.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.github/workflows/releasePythonPackage.yml` & `pyikarus-0.3.3.dev20230601114417/.github/workflows/releasePythonPackage.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.github/workflows/runExamples.yml` & `pyikarus-0.3.3.dev20230601114417/.github/workflows/runExamples.yml`

 * *Files 6% similar despite different names*

```diff
@@ -54,15 +54,21 @@
 
       - name: Clone examples
         run: |
           git clone https://github.com/ikarus-project/ikarus-examples.git
       - name: Checkout branch if it exists
         working-directory: ./ikarus-examples
         continue-on-error: true
+        if: ${{ github.event_name == 'push' }}
         run: git checkout ${{ github.ref_name }}
+      - name: Checkout branch if it exists
+        working-directory: ./ikarus-examples
+        continue-on-error: true
+        if: ${{ github.event_name == 'pull_request' }}
+        run: git checkout ${{ github.event.pull_request.head.ref }}
       - name: Compile all examples
         working-directory: ./ikarus-examples
         run: |
           mkdir cmake-build-${{ matrix.config.config }}
           cd cmake-build-${{ matrix.config.config }}
           cmake ../  -DCMAKE_BUILD_TYPE=${{ matrix.config.config }} -G "Unix Makefiles" -DCMAKE_C_COMPILER=${{ matrix.config.compilerC }} -DCMAKE_CXX_COMPILER=${{ matrix.config.compilerCxx }}
           for i in $( find ../src -maxdepth 1 -name 'iks*'| sed -e 's/\(.cpp\)*$//g' | sed "s|../src/||" ); do cmake --build . --parallel 2 --target "$i"; done;
```

### Comparing `pyikarus-0.3.3.dev20230523103500/.github/workflows/scripts/release.py` & `pyikarus-0.3.3.dev20230601114417/.github/workflows/scripts/release.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.github/workflows/style.yml` & `pyikarus-0.3.3.dev20230601114417/.github/workflows/style.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/.reuse/dep5` & `pyikarus-0.3.3.dev20230601114417/.reuse/dep5`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/CHANGELOG.md` & `pyikarus-0.3.3.dev20230601114417/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,18 +6,20 @@
 # Master (becomes Release v0.4)
 - Add CODE_OF_CONDUCT.md file
 - Refactored Cmake and directory structure  ([#146](https://github.com/ikarus-project/ikarus/pull/146))
 - Added comment section to blog post ([511d83](https://github.com/ikarus-project/ikarus/commit/511d83f9e7c474c9b320db5bc9367114ebe2825d))
 - Updated license information ([#138](https://github.com/ikarus-project/ikarus/pull/138))
 - Added detailed documentation for ikarus-examples ([#140](https://github.com/ikarus-project/ikarus/pull/140))
 - Added computation of Cauchy stress in linear elasticity ([#137](https://github.com/ikarus-project/ikarus/pull/137))
-- Added greeting and init function for reasonable default, e.g. log also to file ([#147](https://github.com/ikarus-project/ikarus/pull/147))
+- Added greeting and init function for a reasonable default, e.g., log also to file ([#147](https://github.com/ikarus-project/ikarus/pull/147))
 - Added an interface for the material library ([#154](https://github.com/ikarus-project/ikarus/pull/154))
 - Added a wrapper for flat and blocked basis ([#157](https://github.com/ikarus-project/ikarus/pull/157))
 - Added basic python bindings and infrastructure. Ikarus can now be downloaded via `pip install pyikarus` ([#157](https://github.com/ikarus-project/ikarus/pull/152))
+- Added result evaluators to post-process desired results ([#165](https://github.com/ikarus-project/ikarus/pull/165))
+- Added explicit calculation of scalars, vectors, and matrices for `NonLinearElastic` ([#160](https://github.com/ikarus-project/ikarus/pull/160))
 
 ## Release v0.3 (Prometheus)
 
 - Added codespell workflow (CI checks now for grammar and typos in comments and variable names) [#70](https://github.com/ikarus-project/ikarus/pull/70)
 - Added `EnhancedAssumedStrains` to decorate a linear-elastic element with various EAS methods [#74](https://github.com/ikarus-project/ikarus/pull/74)
 - Added the ability for the linear solver to accept matrix-valued rhs [#76](https://github.com/ikarus-project/ikarus/pull/76)
 - Added a path-following technique, such that a scalar subsidiary equation, for example, for `Arc length method`,  can be implemented independently [#80](https://github.com/ikarus-project/ikarus/pull/80)
```

### Comparing `pyikarus-0.3.3.dev20230523103500/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601114417/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/CODE_OF_CONDUCT.md` & `pyikarus-0.3.3.dev20230601114417/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/LICENSE.md` & `pyikarus-0.3.3.dev20230601114417/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/LICENSES/CC-BY-SA-4.0.txt` & `pyikarus-0.3.3.dev20230601114417/LICENSES/CC-BY-SA-4.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/LICENSES/CC0-1.0.txt` & `pyikarus-0.3.3.dev20230601114417/LICENSES/CC0-1.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/LICENSES/LGPL-3.0-or-later.txt` & `pyikarus-0.3.3.dev20230601114417/LICENSES/LGPL-3.0-or-later.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/LICENSES/MIT.txt` & `pyikarus-0.3.3.dev20230601114417/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/LICENSES/MPL-2.0.txt` & `pyikarus-0.3.3.dev20230601114417/LICENSES/MPL-2.0.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/PKG-INFO` & `pyikarus-0.3.3.dev20230601114417/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230523103500
+Version: 0.3.3.dev20230601114417
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
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230523103500 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230601114417 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [![Debian](https://github.com/
 ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://
 github.com/ikarus-project/ikarus/actions/workflows/debian.yml) [![codecov]
```

### Comparing `pyikarus-0.3.3.dev20230523103500/README.md` & `pyikarus-0.3.3.dev20230601114417/README.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/cmake/CPM.cmake` & `pyikarus-0.3.3.dev20230601114417/cmake/CPM.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/cmake/FormatTarget/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601114417/cmake/FormatTarget/CMakeLists.txt`

 * *Files 7% similar despite different names*

```diff
@@ -14,16 +14,14 @@
   )
 endif()
 
 if(ADD_CODESPELLTARGET)
   find_package(Python)
   if(Python_FOUND)
     message("Adding codespell targets")
-    message("${CMAKE_SOURCE_DIR}")
-    message(${CMAKE_SOURCE_DIR})
     set(CODESPELLCOMAND
         codespell
         -c
         -s
         -I
         codespellignore
         -S
```

### Comparing `pyikarus-0.3.3.dev20230523103500/cmake/modules/AddAutoDiffFlags.cmake` & `pyikarus-0.3.3.dev20230601114417/cmake/modules/AddAutoDiffFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/cmake/modules/AddEigenFlags.cmake` & `pyikarus-0.3.3.dev20230601114417/cmake/modules/AddEigenFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/cmake/modules/AddMatplotppFlags.cmake` & `pyikarus-0.3.3.dev20230601114417/cmake/modules/AddMatplotppFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/cmake/modules/AddSpdlogFlags.cmake` & `pyikarus-0.3.3.dev20230601114417/cmake/modules/AddSpdlogFlags.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/cmake/tools.cmake` & `pyikarus-0.3.3.dev20230601114417/cmake/tools.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/config.h.cmake` & `pyikarus-0.3.3.dev20230601114417/config.h.cmake`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/__pycache__/mkdocs-macros.cpython-39.pyc` & `pyikarus-0.3.3.dev20230601114417/docs/__pycache__/mkdocs-macros.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/literature.bib` & `pyikarus-0.3.3.dev20230601114417/docs/literature.bib`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/mkdocs-macros.py` & `pyikarus-0.3.3.dev20230601114417/docs/mkdocs-macros.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/mkdocs.yml` & `pyikarus-0.3.3.dev20230601114417/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/overrides/partials/comments.html` & `pyikarus-0.3.3.dev20230601114417/docs/overrides/partials/comments.html`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/assembler.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/assembler.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/controlRoutines.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/controlRoutines.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/dirichletBCs.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/dirichletBCs.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/feRequirements.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/feRequirements.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/finiteElements.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/finiteElements.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+---
+status: new
+---
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Finite elements
 
@@ -10,26 +13,37 @@
 The first one is to provide an evaluation of the scalars, vectors, and matrices. 
 These are associated with an algebraic representation of discrete energies, weak forms, or bilinear forms.
 These algebraic objects are usually constructed using some combination of [local functions](localFunctions.md) and 
 parameters stemming from the underlying physical problem, e.g., load factor, Young's modulus, or viscosity.
 
 The second task of finite elements is to evaluate derived results in the element parameter space, e.g., stresses or geometric quantities.
 This leads to the following interface for the finite elements:
+
 ## Interface
-Local functions provide the following interface
+
+Finite elements should have non-template and non-virtual (considering non-virtual interface idiom (NVI) for the latter) interface methods.
+This is because these methods are usually used to assemble quantities.
+These functions are `calculateScalar`, `calculateVector` and `calculateMatrix`. These are public methods.
+Such an interface is provided by the local functions are shown below:
+
 ```cpp
-ScalarType evaluateScalar(const FErequirements& req);
-void evaluateVector(const FErequirements& req, VectorType& b);
-void evaluateMatrix(const FErequirements& req, MatrixType& A);
+ScalarType calculateScalar(const FErequirements& req);
+void calculateVector(const FErequirements& req, VectorType& b);
+void calculateMatrix(const FErequirements& req, MatrixType& A);
 void calculateLocalSystem(const FErequirements& req, MatrixType& A, VectorType& b);
 void calculateAt(const Resultrequirements& req, const Eigen::Vector<double, Traits::mydim>& local,
                      ResultTypeMap<ScalarType>& result);
 void globalFlatIndices(std::vector<GlobalIndex>& indices);
 ```
 
+Since we would also like to use `autodiff` for our element, we have their protected implementations.
+These methods are templates to allow double or `autodiff` scalar types.
+These methods are `calculateScalarImpl`, `calculateVectorImpl` and `calculateMatrixImpl`.
+`calculateScalar`, `calculateVector` and `calculateMatrix` simply forward to these implementation functions.
+
 Please refer to the [FE requirements](feRequirements.md) to learn more about the finite element requirements and result requirements. 
 The first four methods receive an object of type `FErequirements`. This object is responsible for passing different types of information needed for the local evaluation of the local linear algebra objects.
 The first method, `evaluateScalar`, simply returns by value because it is cheaper to return a `double`, for example when evaluating energy.
 The other methods, `evaluateVector`, `evaluateMatrix`, and `calculateLocalSystem`, receive one or two additional output arguments where the results are to be written.
 This interface is needed to circumvent the dynamic memory allocation, that is required if these methods return by value.
 
 The method `calculateAt` is responsible for evaluating several results, and it receives the `ResultRequirements` object.
@@ -62,23 +76,67 @@
     Thus, the maximum size of `result` is limited to a 3x3 matrix. This is used to circumvent dynamic memory allocations again.
 
 
 The last method is the `globalFlatIndices`. It is used to write a finite element's global indices to the output parameter `indices`.
 This information originates from a `basis` object. See existing implementations for details.
 
 ## Linear and Non-linear Elasticity
-* To be added
+
+`LinearElastic` and `NonLinearElastic` classes are designed in a generic way.
+This means that they could be directly used for any $n$-dimensional finite element in the geometrically linear and non-linear cases.
+They inherit from the class `PowerBasisFE`, which helps to arrange the nodal degrees of freedom in a `FlatInterleaved` format.
+Refer DUNE[@sander2020dune] for more details. The constructor for both classes of elements has the following signature:
+```cpp
+template <typename VolumeLoad = LoadDefault, typename NeumannBoundaryLoad = LoadDefault>
+LinearElastic(const Basis& globalBasis, const typename LocalView::Element& element, double emod, double nu,
+                  VolumeLoad p_volumeLoad = {}, const BoundaryPatch<GridView>* p_neumannBoundary = nullptr,
+                  NeumannBoundaryLoad p_neumannBoundaryLoad = {}) {}
+```
+```cpp
+template <typename VolumeLoad = LoadDefault, typename NeumannBoundaryLoad = LoadDefault>
+NonLinearElastic(const Basis& globalBasis, const typename LocalView::Element& element, const Material& p_mat,
+                 VolumeLoad p_volumeLoad = {}, const BoundaryPatch<GridView>* p_neumannBoundary = nullptr,
+                 NeumannBoundaryLoad p_neumannBoundaryLoad = {})
+```
+
+The first argument defines the basis function used to interpolate the solution field, while the second argument points to the `gridElement` itself.
+The next set of arguments are related to the material law to be used.
+For the geometrically linear case, the Young's modulus and the Poisson's ratio are passed, and a `planeStress` material model is assumed.
+For the geometrically non-linear case, the material model is to be passed as an argument.
+This could be for instance, the St. Venant-Kirchhoff material law or the Neo-Hookean material law.
+`volumeLoad` and `neumannBoundaryLoad` are optional parameters that could be passed as per the use case.
+It is necessary to note that a `neumannBoundary` must be defined if a `neumannBoundaryLoad` is to be applied.
+Member functions are defined as per the [interface](finiteElements.md#interface) mentioned above.
+Two member functions are written such that the stiffness matrices and load vectors can also be obtained by automatic differentiation.
+These functions are `protected`. They are:
+```cpp
+calculateScalarImpl(const FERequirementType& par, const Eigen::VectorX<ScalarType>& dx)
+calculateVectorImpl(const FERequirementType& par, const Eigen::VectorX<ScalarType>& dx, Eigen::VectorX<ScalarType>& force)
+```
+`getStrainFunction(const FERequirementType& par, const Eigen::VectorX<ScalarType>& dx)` is used to get the desired strain measure.
+It can be used to toggle between the geometrically linear and non-linear cases.
+`LinearStrains` are used for the geometrically linear case, while `GreenLagrangianStrains` are used for the non-linear case.
+These strain measures are defined as expressions in `dune-localfefunctions`. Refer to [Expressions](localFunctions.md#expressions) for more details.
+The strain-displacement operators are obtained by evaluating the derivative of the strain measure with respect to the nodal degrees of freedom.
+This is then used to evaluate the stiffness matrix.
+For more details on derivatives w.r.t. coefficients, refer [here](localFunctions.md#derivatives-wrt-coefficients).
+Finally, the `calculateAt()` function evaluates the `linearStress` and `PK2Stress` (the second Piola-Kirchhoff stress tensor) as per the `ResultRequirementsType`.
+An implementation for a push forward operation to evaluate the `cauchyStress` is an open task.
+Refer to [open tasks](../03_contribution/openTask.md#finite-elements) for more details.
 
 ## Enhanced Assumed Strain Elements
+
 The Enhanced Assumed Strain (EAS) elements are a class of finite elements that helps to avoid the locking phenomenon.
-They are obtained by re-parametrizing the Hu-Washizu principle and enforcing an orthogonality condition. 
-This results in an extension of the standard pure displacement formulation with an enhanced strain field ($\tilde\epsilon$) 
-as an additional independent variable.The locking characteristics of the pure displacement formulations can be eliminated with an appropriate choice of ansatz space for $\tilde\epsilon$. For further theoretical aspects, the readers are referred to [@simo_class_1990] 
-and [@andelfinger_eas-elements_1993]. The EAS formulation is currently implemented for the linear-elastic case, but 
-it could be extended to the non-linear regime. The currently implemented EAS elements are the following:
+They are obtained by re-parametrizing the Hu-Washizu principle and enforcing an orthogonality condition.
+This results in an extension of the standard pure displacement formulation with an enhanced strain field ($\tilde\epsilon$).
+($\tilde\epsilon$) is as an additional independent variable.
+The locking characteristics of the pure displacement formulations can be eliminated with an appropriate choice of ansatz space for $\tilde\epsilon$.
+For further theoretical aspects, the readers are referred to [@simo_class_1990] and [@andelfinger_eas-elements_1993].
+The EAS formulation is currently implemented for the linear-elastic case, but it could be extended to the non-linear regime.
+The currently implemented EAS elements are the following:
 
 * Q1E4
 * Q1E5
 * Q1E7
 * H1E9
 * H1E21
```

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/grids.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/grids.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/index.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/localBasis.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/localBasis.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/localFunctions.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/localFunctions.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/manifolds.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/manifolds.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/nonlinearOperator.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/nonlinearOperator.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/observer.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/observer.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/01_framework/solvers.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/01_framework/solvers.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/cantileverBeam.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/cantileverBeam.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/computePi.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/computePi.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/cooksMembrane.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/cooksMembrane.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/incompressibleRubberBlock.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/incompressibleRubberBlock.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+---
+status: new
+---
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Deformation of an incompressible rubber block
 
@@ -12,19 +15,19 @@
 for such a system is defined in the `Solid struct` by the function
 `calculateScalarImpl(const FERequirementType &par, const Eigen::VectorX<ScalarType> &dx)`. 
 This function uses the principles of automatic differentiation to provide the stiffness matrix and
 other necessary quantities to perform a static structural analysis.
 
 ## Code highlights
 
-The `struct` named `Solid` is created such that it inherits from `AutoDiffFE`. It is constructed as shown below:
+The `struct` named `Solid` is created which is not inherited from any class. It is constructed as shown below:
 ```cpp
 Solid(const Basis &basis, const typename LocalView::Element &element, double emod, double nu)
-    : BaseAD(basis.flat(), element), emod_{emod}, nu_{nu} {
-  this->localView().bind(element);
+    : localView_{basis.flat().localView()}, emod_{emod}, nu_{nu} {
+  localView_.bind(element);
   mu_       = emod_ / (2 * (1 + nu_));
   lambdaMat = convertLameConstants({.emodul = emod_, .nu = nu_}).toLamesFirstParameter();
 }
 ```
 It takes a reference to the basis function (`&basis`), the element (`&element`), and the material parameters, namely Young's modulus 
 (`emod`) and Poisson's ratio (`nu`), as arguments during construction. The function `convertLameConstants()` is a helper function
 to switch between the Lame parameters.
@@ -62,15 +65,21 @@
 ```
 A linear Lagrangian basis is opted for the displacements and a constant basis for the pressure degrees of freedom using the
 `composite` basis feature from Dune, as shown below:
 ```cpp
 auto basis = Ikarus::makeBasis(
 gridView, composite(power<2>(lagrange<1>()), lagrange<0>()));
 ```
-Here, `#!cpp power<2>` is used to approximate the displacement field in both $x$ and $y$ directions. 
+Here, `#!cpp power<2>` is used to approximate the displacement field in both $x$ and $y$ directions.
+A vector of `Solid` finite elements that are decorated by `AutoDiffFE` are then constructed as shown below:
+```cpp
+std::vector<AutoDiffFE<Solid<decltype(basis)>>> fes;
+for (auto &ele : elements(gridView))
+  fes.emplace_back(basis, ele, Emod, nu);
+```
 The displacement degrees of freedom at position $y=0$ are fixed using the following snippet:
 ```cpp
 auto basisP = std::make_shared<const decltype(basis)>(basis);
 Ikarus::DirichletValues dirichletValues(basisP->flat());
 dirichletValues.fixDOFs([](auto &basis_, auto &dirichletFlags) {
   Dune::Functions::forEachBoundaryDOF(subspaceBasis(basis_, _0),
                    [&](auto &&localIndex, auto &&localView, auto &&intersection) {
```

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/index.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/kirchhoffPlate.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/kirchhoffPlate.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+---
+status: new
+---
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Plate subjected to a surface load
 
@@ -10,21 +13,22 @@
 Kirchhoff-type plate element is implemented in `iks004_kirchhoffPlate.cpp` using the automatic differentiation
 technique as commented before. The basis used for discretization is a NURBS basis from the `dune-iga` module.
 The problem is solved, and convergence plots are created by comparing the solutions to the available analytical solutions for the
 simply supported case.
 
 ## Code highlights
 
-Similar to the `struct` named `Solid` in `iks003_incompressible_LinearElasticity.cpp`, here a `struct` named `KirchhoffPlate` 
-is created such that it inherits from `AutoDiffFE`. It is constructed as shown below:
+Similar to the `struct` named `Solid` in `iks003_incompressible_LinearElasticity.cpp`, here a `struct` named `KirchhoffPlate` is created.
+It inherits from `ScalarFieldFE` and it must be decorated with `AutoDiffFE` as well to compute the required matrices and vectors.
+It is constructed as shown below:
+
 ```cpp
 KirchhoffPlate(const Basis &basis, const typename LocalView::Element &element, double p_Emodul, double p_nu,
                double p_thickness)
     : BaseDisp(basis.flat(), element),
-      BaseAD(basis.flat(), element),
       Emodul{p_Emodul},
       nu{p_nu},
       thickness{p_thickness} {
   this->localView().bind(element);
   geometry_.emplace(this->localView().element().geometry());
 }
 ```
@@ -116,15 +120,14 @@
 ```
 The $L^2$-error is calculated by using 
 $$
 L^2\textrm{-error} = \sqrt{\sum_{ele} \int_{\Omega_{ele}} \left( w_{analytical}-w_{FE} \right)^2}
 $$ 
 as shown below: 
 ```cpp
-
 double l2_error = 0.0;
 for (auto &ele : elements(gridView)) {
   localView.bind(ele);
   localw.bind(ele);
   localwAna.bind(ele);
   const auto geo   = localView.element().geometry();
   const auto &rule = Dune::QuadratureRules<double, 2>::rule(ele.type(), 2 * localView.tree().finiteElement().localBasis().order());
```

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/newtonRaphsonMethod.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/newtonRaphsonMethod.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/nonLinearElasticity.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/nonLinearElasticity.md`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 };
 
 auto matParameter = Ikarus::toLamesFirstParameterAndShearModulus({.emodul = 1000, .nu = 0.3});
 
 Ikarus::StVenantKirchhoff matSVK(matParameter);
 auto reducedMat = planeStress(matSVK);
 
-std::vector<Ikarus::NonLinearElastic<typename decltype(basis)::element_type, decltype(reducedMat)>>> fes;
+std::vector<Ikarus::NonLinearElastic<decltype(basis), decltype(reducedMat)>>> fes;
 for (auto &element : elements(gridView))
   fes.emplace_back(*basis, element, reducedMat, &neumannBoundary, neumannBoundaryLoad, volumeLoad);
 ```
 The functors `volumeLoad` and `neumannBoundaryLoad` are used to obtain the external volume and surface loads acting on a particular position.
 We use a Saint Venant–Kirchhoff material model, which we transform to a plane stress material law for our two-dimensional simulation.
 The line $y=0$ is clamped by applying the Dirichlet boundary condition expressed below:
 ```cpp
```

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/02_examples/vonMisesTruss.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/02_examples/vonMisesTruss.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+---
+status: new
+---
 <!--
 SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 SPDX-License-Identifier: CC-BY-SA-4.0
 -->
 
 # Von Mises truss calculation  
 
@@ -9,18 +12,20 @@
 
 `iks007_vonMisesTruss.cpp` utilizes the tools and features mentioned in the previous examples to solve the 
 standard Von-Mises truss example found in literature (refer to Section 2[@misesTruss1923]).
 
 
 ## Code highlights
 
-The struct named `Truss` is created such that it inherits from `AutoDiffFE`. It is constructed as shown below:
+The struct named `Truss` is created such that it inherits from `PowerBasisFE`.
+It must be decorated with `AutoDiffFE` as well to compute the stiffness matrix and load vectors during construction.
+It is constructed as shown below:
 ```cpp
 Truss(const Basis &basis, const typename LocalView::Element &element, double p_EA)
-    : BaseDisp(basis.flat(), element), BaseAD(basis.flat(), element), EA{p_EA} {
+    : BaseDisp(basis.flat(), element), EA{p_EA} {
   this->localView().bind(element);
 }
 ```
 It takes a reference to the basis function (`&basis`), the element (`&element`), and the axial stiffness of the 
 truss structure (`p_EA`) as arguments during construction.
 
 `ScalarType calculateScalarImpl(const FERequirementType &par, const Eigen::VectorX<ScalarType> &dx)` is
```

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/03_contribution/buildDocumentationLocally.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/buildDocumentationLocally.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/03_contribution/codeStyle.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/codeStyle.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/03_contribution/howToEdit.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/howToEdit.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/03_contribution/openTask.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/03_contribution/openTask.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 ### Finite element helper
 * Implement a default mass matrix
 
 ### Finite elements
 * Nonlinear Reissner-Mindlin shell [@muller2022consistent]
 * Kirchhoff-Love shell
 * 3D-Beam
-* Implement forces and stiffness matrix of `NonLinearElastic`
 * Standard beam and plate formulations
+* Add calculation of different stress measures (push-forward or pull-back of PK2 stresses or similar)
 
 ### Further addons
 * [Muesli](https://materials.imdea.org/muesli/)
 
 [^KLNote]: This is usually needed for a Kirchhoff-Love shell implementation, see [@kiendlKLshell].
 
 !!! note  "Code style"
```

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/04_blog/posts/v0.3.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/04_blog/posts/v0.3.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/05_cppReferences/cppRef.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/05_cppReferences/cppRef.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CLionToolchainSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/CMakeOutput.png` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/CMakeOutput.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/ClionFooter.png` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ClionFooter.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/DockerWslSettings.png` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/DockerWslSettings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/Installation/ReloadCmakeProject.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/CmakeOptions.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/buildMessages.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/localSite.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/portBindings.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/builddocumentationlocally/servicesDocker.png`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/logo_blue.svg` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_blue.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/auxiliaryImages/logo_white.svg` & `pyikarus-0.3.3.dev20230601114417/docs/website/auxiliaryImages/logo_white.svg`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/download.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/download.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/docs/website/index.md` & `pyikarus-0.3.3.dev20230601114417/docs/website/index.md`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601114417/ikarus/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/assembler/simpleAssemblers.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/assembler/simpleAssemblers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/assembler/simpleAssemblers.inl` & `pyikarus-0.3.3.dev20230601114417/ikarus/assembler/simpleAssemblers.inl`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/controlRoutines/loadControl.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/loadControl.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/controlRoutines/pathFollowingTechnique.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/controlRoutines/pathFollowingTechnique.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feBases/powerBasisFE.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/powerBasisFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feBases/scalarFE.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feBases/scalarFE.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feRequirements.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feRequirements.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/feTraits.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/feTraits.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 
-#include <functional>
-#include <optional>
-
-#include <dune/fufem/boundarypatch.hh>
 #include <dune/localfefunctions/meta.hh>
 
 #include <ikarus/finiteElements/feRequirements.hh>
 #include <ikarus/utils/eigenDuneTransformations.hh>
 
 namespace Ikarus {
 
@@ -241,208 +237,240 @@
     }
 
     std::shared_ptr<Geometry> geometry;
     Eigen::Matrix<double, 6, 6> T0InverseTransformed;
   };
 
   template <typename Geometry>
-  using EAS2DVariant = std::variant<EASQ1E4<Geometry>, EASQ1E5<Geometry>, EASQ1E7<Geometry>>;
+  using EAS2DVariant = std::variant<std::monostate, EASQ1E4<Geometry>, EASQ1E5<Geometry>, EASQ1E7<Geometry>>;
   template <typename Geometry>
-  using EAS3DVariant = std::variant<EASH1E9<Geometry>, EASH1E21<Geometry>>;
+  using EAS3DVariant = std::variant<std::monostate, EASH1E9<Geometry>, EASH1E21<Geometry>>;
 
   template <typename DisplacementBasedElement>
   class EnhancedAssumedStrains : public DisplacementBasedElement {
   public:
     using FERequirementType      = typename DisplacementBasedElement::FERequirementType;
     using ResultRequirementsType = typename DisplacementBasedElement::ResultRequirementsType;
     using LocalView              = typename DisplacementBasedElement::LocalView;
     using GridView               = typename DisplacementBasedElement::GridView;
     using Traits                 = typename DisplacementBasedElement::Traits;
     using DisplacementBasedElement::localView;
 
+    // Disabling this forwarding constructor if the argument provided is EnhancedAssumedStrains itself, to forward the
+    // calls to the implicit copy constructor
     template <typename... Args>
-    explicit EnhancedAssumedStrains(Args&&... args) : DisplacementBasedElement(std::forward<Args>(args)...) {
-      setEASType(0);
-    }
+    requires(not std::is_same_v<std::remove_cvref_t<std::tuple_element_t<0, std::tuple<Args...>>>,
+                                EnhancedAssumedStrains>) explicit EnhancedAssumedStrains(Args&&... args)
+        : DisplacementBasedElement(std::forward<Args>(args)...) {}
 
-    double calculateScalar(const FERequirementType& par) const {
-      if (onlyDisplacementBase) return DisplacementBasedElement::calculateScalar(par);
+    inline double calculateScalar(const FERequirementType& par) const {
+      if (isDisplacementBased()) return DisplacementBasedElement::calculateScalar(par);
       DUNE_THROW(Dune::NotImplemented,
                  "EAS element do not support any scalar calculations, i.e. they are not derivable from a potential");
-      return 0.0;
     }
 
-    void calculateVector(const FERequirementType& par, typename Traits::VectorType& g) const {
-      DisplacementBasedElement::calculateVector(par, g);
-      using namespace Dune;
-
-      if (onlyDisplacementBase) return;
-
-      const auto& d       = par.getGlobalSolution(Ikarus::FESolutions::displacement);
-      auto strainFunction = DisplacementBasedElement::getStrainFunction(par);
-      Eigen::VectorXd disp(localView().size());
-      const auto& numNodes = DisplacementBasedElement::numberOfNodes;
-
-      for (auto i = 0U; i < numNodes; ++i)
-        for (auto k2 = 0U; k2 < Traits::mydim; ++k2)
-          disp[i * Traits::mydim + k2] = d[localView().index(localView().tree().child(k2).localIndex(i))[0]];
+    bool isDisplacementBased() const { return std::holds_alternative<std::monostate>(easVariant_); }
 
-      using namespace Dune::DerivativeDirections;
-
-      auto C         = DisplacementBasedElement::getMaterialTangentFunction(par);
-      const auto geo = localView().element().geometry();
+    inline void calculateVector(const FERequirementType& par, typename Traits::template VectorType<> force) const {
+      calculateVectorImpl<double>(par, force);
+    }
 
-      // Internal forces from enhanced strains
-      std::visit(
+    const auto& easVariant() const { return easVariant_; }
+    auto getNumberOfEASParameters() const {
+      return std::visit(
           [&]<typename EAST>(const EAST& easFunction) {
-            constexpr int enhancedStrainSize = EAST::enhancedStrainSize;
-            Eigen::Matrix<double, enhancedStrainSize, enhancedStrainSize> D;
-            calculateDAndLMatrix(easFunction, par, D, L);
-
-            const auto alpha = (-D.inverse() * L * disp).eval();
-
-            for (const auto& [gpIndex, gp] : strainFunction.viewOverIntegrationPoints()) {
-              const auto M            = easFunction.calcM(gp.position());
-              const double intElement = geo.integrationElement(gp.position()) * gp.weight();
-              const auto CEval        = C(gpIndex);
-              auto stresses           = (CEval * M * alpha).eval();
-              for (size_t i = 0; i < numNodes; ++i) {
-                const auto bopI = strainFunction.evaluateDerivative(gpIndex, wrt(coeff(i)), on(gridElement));
-                g.template segment<Traits::mydim>(Traits::mydim * i) += bopI.transpose() * stresses * intElement;
-              }
-            }
+            if constexpr (std::is_same_v<std::monostate, EAST>)
+              return 0;
+            else
+              return EAST::enhancedStrainSize;
           },
           easVariant_);
     }
 
-    auto& easVariant() { return easVariant_; }
-
-    void calculateMatrix(const FERequirementType& par, typename Traits::MatrixType& K) const {
+    void calculateMatrix(const FERequirementType& par, typename Traits::template MatrixType<> K) const {
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
 
-      /// fill h with displacement-based stiffness.
+      /// fill K with displacement-based stiffness.
       /// It is assumed to be assembled block-wise on element level.
       /// This means the displacements x,y,z of node I are grouped together.
       DisplacementBasedElement::calculateMatrix(par, K);
 
-      if (onlyDisplacementBase) return;
-
-      auto strainFunction  = DisplacementBasedElement::getStrainFunction(par);
-      const auto& numNodes = DisplacementBasedElement::numberOfNodes;
-      assert(((numNodes == 4 and Traits::mydim == 2) or (numNodes == 8 and Traits::mydim == 3))
-             && "EAS only supported for Q1 or H1 elements");
+      if (isDisplacementBased()) return;
 
       std::visit(
           [&]<typename EAST>(const EAST& easFunction) {
-            constexpr int enhancedStrainSize = EAST::enhancedStrainSize;
-            Eigen::Matrix<double, enhancedStrainSize, enhancedStrainSize> D;
-            calculateDAndLMatrix(easFunction, par, D, L);
+            if constexpr (not std::is_same_v<std::monostate, EAST>) {
+              constexpr int enhancedStrainSize = EAST::enhancedStrainSize;
+              Eigen::Matrix<double, enhancedStrainSize, enhancedStrainSize> D;
+              calculateDAndLMatrix(easFunction, par, D, L);
 
-            K.template triangularView<Eigen::Upper>() -= L.transpose() * D.inverse() * L;
-            K.template triangularView<Eigen::StrictlyLower>() = K.transpose();
+              K.template triangularView<Eigen::Upper>() -= L.transpose() * D.inverse() * L;
+              K.template triangularView<Eigen::StrictlyLower>() = K.transpose();
+            }
           },
           easVariant_);
     }
 
     void calculateAt(const ResultRequirementsType& req, const Dune::FieldVector<double, Traits::mydim>& local,
                      ResultTypeMap<double>& result) const {
       using namespace Dune::Indices;
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
 
       DisplacementBasedElement::calculateAt(req, local, result);
 
-      if (onlyDisplacementBase) return;
+      if (isDisplacementBased()) return;
 
       const auto& d        = req.getGlobalSolution(Ikarus::FESolutions::displacement);
       const auto C         = DisplacementBasedElement::getMaterialTangentFunction(req.getFERequirements());
       const auto& numNodes = DisplacementBasedElement::numberOfNodes;
 
       Eigen::VectorXd disp(localView().size());
       for (auto i = 0U; i < numNodes; ++i)
         for (auto k2 = 0U; k2 < Traits::mydim; ++k2)
           disp[i * Traits::mydim + k2] = d[localView().index(localView().tree().child(k2).localIndex(i))[0]];
 
-      assert(((numNodes == 4 and Traits::mydim == 2) or (numNodes == 8 and Traits::mydim == 3))
-             && "EAS only supported for Q1 or H1 elements");
-
       std::visit(
           [&]<typename EAST>(const EAST& easFunction) {
-            constexpr int enhancedStrainSize = EAST::enhancedStrainSize;
-            Eigen::Matrix<double, enhancedStrainSize, enhancedStrainSize> D;
-            calculateDAndLMatrix(easFunction, req.getFERequirements(), D, L);
-            const auto alpha = (-D.inverse() * L * disp).eval();
-            const auto M     = easFunction.calcM(local);
-            const auto CEval = C(local);
-            auto easStress   = (CEval * M * alpha).eval();
-            typename ResultTypeMap<double>::ResultArray resultVector;
-            if (req.isResultRequested(ResultType::linearStress)) {
-              resultVector.resize(3, 1);
-              resultVector = result.getResult(ResultType::linearStress) + easStress;
-              result.insertOrAssignResult(ResultType::linearStress, resultVector);
+            if constexpr (not std::is_same_v<std::monostate, EAST>) {
+              constexpr int enhancedStrainSize = EAST::enhancedStrainSize;
+              Eigen::Matrix<double, enhancedStrainSize, enhancedStrainSize> D;
+              calculateDAndLMatrix(easFunction, req.getFERequirements(), D, L);
+              const auto alpha = (-D.inverse() * L * disp).eval();
+              const auto M     = easFunction.calcM(local);
+              const auto CEval = C(local);
+              auto easStress   = (CEval * M * alpha).eval();
+              typename ResultTypeMap<double>::ResultArray resultVector;
+              if (req.isResultRequested(ResultType::linearStress)) {
+                resultVector.resize(3, 1);
+                resultVector = result.getResult(ResultType::linearStress) + easStress;
+                result.insertOrAssignResult(ResultType::linearStress, resultVector);
+              }
             }
           },
           easVariant_);
     }
 
-    void setEASType(int numberOfEASParameters) {
+    void setEASType(int numberOfEASParameters_) {
+      const auto& numNodes = DisplacementBasedElement::numberOfNodes;
+      if (not((numNodes == 4 and Traits::mydim == 2) or (numNodes == 8 and Traits::mydim == 3))
+          and (not isDisplacementBased()))
+        DUNE_THROW(Dune::NotImplemented, "EAS only supported for Q1 or H1 elements");
+
       if constexpr (Traits::mydim == 2) {
-        switch (numberOfEASParameters) {
+        switch (numberOfEASParameters_) {
           case 0:
-            onlyDisplacementBase = true;
+            easVariant_ = std::monostate();
             break;
           case 4:
-            easVariant_          = EASQ1E4(localView().element().geometry());
-            onlyDisplacementBase = false;
+            easVariant_ = EASQ1E4(localView().element().geometry());
             break;
           case 5:
-            easVariant_          = EASQ1E5(localView().element().geometry());
-            onlyDisplacementBase = false;
+            easVariant_ = EASQ1E5(localView().element().geometry());
             break;
           case 7:
-            easVariant_          = EASQ1E7(localView().element().geometry());
-            onlyDisplacementBase = false;
+            easVariant_ = EASQ1E7(localView().element().geometry());
             break;
           default:
             DUNE_THROW(Dune::NotImplemented, "The given EAS parameters are not available for the 2D case.");
             break;
         }
       } else if constexpr (Traits::mydim == 3) {
-        switch (numberOfEASParameters) {
+        switch (numberOfEASParameters_) {
           case 0:
-            onlyDisplacementBase = true;
+            easVariant_ = std::monostate();
             break;
           case 9:
-            easVariant_          = EASH1E9(localView().element().geometry());
-            onlyDisplacementBase = false;
+            easVariant_ = EASH1E9(localView().element().geometry());
             break;
           case 21:
-            easVariant_          = EASH1E21(localView().element().geometry());
-            onlyDisplacementBase = false;
+            easVariant_ = EASH1E21(localView().element().geometry());
             break;
           default:
             DUNE_THROW(Dune::NotImplemented, "The given EAS parameters are not available for the 3D case.");
             break;
         }
       }
     }
 
+  protected:
+    template <typename ScalarType>
+    inline ScalarType calculateScalarImpl(const FERequirementType& par,
+                                          const std::optional<const Eigen::VectorX<ScalarType>>& dx
+                                          = std::nullopt) const {
+      if (isDisplacementBased()) return DisplacementBasedElement::template calculateScalarImpl<ScalarType>(par, dx);
+      DUNE_THROW(Dune::NotImplemented,
+                 "EAS element do not support any scalar calculations, i.e. they are not derivable from a potential");
+    }
+
+    template <typename ScalarType>
+    void calculateVectorImpl(const FERequirementType& par, typename Traits::template VectorType<ScalarType> force,
+                             const std::optional<const Eigen::VectorX<ScalarType>>& dx = std::nullopt) const {
+      DisplacementBasedElement::calculateVectorImpl(par, force, dx);
+      if (isDisplacementBased()) return;
+      using namespace Dune;
+      const auto& d       = par.getGlobalSolution(Ikarus::FESolutions::displacement);
+      auto strainFunction = DisplacementBasedElement::getStrainFunction(par, dx);
+      Eigen::VectorX<ScalarType> disp(localView().size());
+      const auto& numNodes = DisplacementBasedElement::numberOfNodes;
+
+      // FIXME this should not be needed in the future strainFunction should be able to hand out this vector
+      if (dx)
+        for (auto i = 0U; i < numNodes; ++i)
+          for (auto k2 = 0U; k2 < Traits::mydim; ++k2)
+            disp[i * Traits::mydim + k2] = dx.value()[i * Traits::mydim + k2]
+                                           + d[localView().index(localView().tree().child(k2).localIndex(i))[0]];
+      else
+        for (auto i = 0U; i < numNodes; ++i)
+          for (auto k2 = 0U; k2 < Traits::mydim; ++k2)
+            disp[i * Traits::mydim + k2] = d[localView().index(localView().tree().child(k2).localIndex(i))[0]];
+
+      using namespace Dune::DerivativeDirections;
+
+      auto C         = DisplacementBasedElement::getMaterialTangentFunction(par);
+      const auto geo = localView().element().geometry();
+
+      // Internal forces from enhanced strains
+      std::visit(
+          [&]<typename EAST>(const EAST& easFunction) {
+            if constexpr (not std::is_same_v<std::monostate, EAST>) {
+              constexpr int enhancedStrainSize = EAST::enhancedStrainSize;
+              Eigen::Matrix<double, enhancedStrainSize, enhancedStrainSize> D;
+              calculateDAndLMatrix(easFunction, par, D, L);
+
+              const auto alpha = (-D.inverse() * L * disp).eval();
+
+              for (const auto& [gpIndex, gp] : strainFunction.viewOverIntegrationPoints()) {
+                const auto M            = easFunction.calcM(gp.position());
+                const double intElement = geo.integrationElement(gp.position()) * gp.weight();
+                const auto CEval        = C(gpIndex);
+                auto stresses           = (CEval * M * alpha).eval();
+                for (size_t i = 0; i < numNodes; ++i) {
+                  const auto bopI = strainFunction.evaluateDerivative(gpIndex, wrt(coeff(i)), on(gridElement));
+                  force.template segment<Traits::mydim>(Traits::mydim * i) += bopI.transpose() * stresses * intElement;
+                }
+              }
+            }
+          },
+          easVariant_);
+    }
+
   private:
     using EAS2DVariantImpl = EAS2DVariant<typename LocalView::Element::Geometry>;
     using EAS3DVariantImpl = EAS3DVariant<typename LocalView::Element::Geometry>;
     std::conditional_t<Traits::mydim == 2, EAS2DVariantImpl, EAS3DVariantImpl> easVariant_;
     mutable Eigen::MatrixXd L;
-    bool onlyDisplacementBase{false};
     template <int enhancedStrainSize>
     void calculateDAndLMatrix(const auto& easFunction, const auto& par,
                               Eigen::Matrix<double, enhancedStrainSize, enhancedStrainSize>& DMat,
                               Eigen::MatrixXd& LMat) const {
       using namespace Dune;
       using namespace Dune::DerivativeDirections;
+
       auto strainFunction = DisplacementBasedElement::getStrainFunction(par);
       const auto C        = DisplacementBasedElement::getMaterialTangentFunction(par);
       const auto geo      = localView().element().geometry();
       const auto numNodes = DisplacementBasedElement::numberOfNodes;
       DMat.setZero();
       LMat.setZero(enhancedStrainSize, localView().size());
       for (const auto& [gpIndex, gp] : strainFunction.viewOverIntegrationPoints()) {
```

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/linearElastic.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/linearElastic.hh`

 * *Files 12% similar despite different names*

```diff
@@ -1,142 +1,215 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
-#include <concepts>
-#include <iosfwd>
-#include <optional>
-#include <type_traits>
 
 #include <dune/common/classname.hh>
 #include <dune/fufem/boundarypatch.hh>
 #include <dune/geometry/quadraturerules.hh>
 #include <dune/geometry/type.hh>
 #include <dune/localfefunctions/expressions/linearStrainsExpr.hh>
 #include <dune/localfefunctions/impl/standardLocalFunction.hh>
 #include <dune/localfefunctions/manifolds/realTuple.hh>
 
 #include <autodiff/forward/dual.hpp>
 #include <autodiff/forward/dual/eigen.hpp>
 
-#include <ikarus/finiteElements/feBases/autodiffFE.hh>
 #include <ikarus/finiteElements/feBases/powerBasisFE.hh>
 #include <ikarus/finiteElements/feRequirements.hh>
 #include <ikarus/finiteElements/feTraits.hh>
 #include <ikarus/finiteElements/mechanics/materials.hh>
 #include <ikarus/finiteElements/physicsHelper.hh>
 #include <ikarus/utils/defaultFunctions.hh>
 #include <ikarus/utils/eigenDuneTransformations.hh>
 #include <ikarus/utils/linearAlgebraHelper.hh>
 
 namespace Ikarus {
 
-  template <typename Basis_, typename FErequirements_ = FErequirements<>, bool useEigenRef = false>
+  template <typename Basis_, typename FERequirements_ = FErequirements<>, bool useEigenRef = false>
   class LinearElastic : public PowerBasisFE<typename Basis_::FlatBasis> {
   public:
     using Basis                  = Basis_;
     using FlatBasis              = typename Basis::FlatBasis;
     using BaseDisp               = PowerBasisFE<FlatBasis>;  // Handles globalIndices function
-    using FERequirementType      = FErequirements_;
+    using FERequirementType      = FERequirements_;
     using ResultRequirementsType = ResultRequirements<FERequirementType>;
     using LocalView              = typename FlatBasis::LocalView;
     using Element                = typename LocalView::Element;
     using GridView               = typename FlatBasis::GridView;
 
     using Traits = TraitsFromLocalView<LocalView, useEigenRef>;
 
-    static constexpr int mydim = Traits::mydim;
+    static constexpr int myDim = Traits::mydim;
 
     template <typename VolumeLoad = LoadDefault, typename NeumannBoundaryLoad = LoadDefault>
     LinearElastic(const Basis& globalBasis, const typename LocalView::Element& element, double emod, double nu,
                   VolumeLoad p_volumeLoad = {}, const BoundaryPatch<GridView>* p_neumannBoundary = nullptr,
                   NeumannBoundaryLoad p_neumannBoundaryLoad = {})
         : BaseDisp(globalBasis.flat(), element), neumannBoundary{p_neumannBoundary}, emod_{emod}, nu_{nu} {
       this->localView().bind(element);
       auto& first_child = this->localView().tree().child(0);
       const auto& fe    = first_child.finiteElement();
       numberOfNodes     = fe.size();
       dispAtNodes.resize(fe.size());
       const int order = 2 * (this->localView().tree().child(0).finiteElement().localBasis().order());
       localBasis      = Dune::CachedLocalBasis(this->localView().tree().child(0).finiteElement().localBasis());
-      localBasis.bind(Dune::QuadratureRules<double, Traits::mydim>::rule(this->localView().element().type(), order),
+      localBasis.bind(Dune::QuadratureRules<double, myDim>::rule(this->localView().element().type(), order),
                       Dune::bindDerivatives(0, 1));
 
       if constexpr (!std::is_same_v<VolumeLoad, LoadDefault>) volumeLoad = p_volumeLoad;
       if constexpr (!std::is_same_v<NeumannBoundaryLoad, LoadDefault>) neumannBoundaryLoad = p_neumannBoundaryLoad;
 
       assert(((not p_neumannBoundary and not neumannBoundaryLoad) or (p_neumannBoundary and neumannBoundaryLoad))
              && "If you pass a Neumann boundary you should also pass the function for the Neumann load!");
     }
 
   public:
-    //    const auto& localView() const { return localView(); }
-
-    auto getDisplacementFunction(const FERequirementType& par) const {
+    template <typename ScalarType>
+    auto getDisplacementFunction(const FERequirementType& par,
+                                 const std::optional<const Eigen::VectorX<ScalarType>>& dx = std::nullopt) const {
       const auto& d = par.getGlobalSolution(Ikarus::FESolutions::displacement);
 
-      for (auto i = 0U; i < dispAtNodes.size(); ++i)
-        for (auto k2 = 0U; k2 < mydim; ++k2)
-          dispAtNodes[i][k2] = d[this->localView().index(this->localView().tree().child(k2).localIndex(i))[0]];
+      Dune::BlockVector<Dune::RealTuple<ScalarType, Traits::dimension>> disp(dispAtNodes.size());
+      if (dx) {
+        for (auto i = 0U; i < disp.size(); ++i)
+          for (auto k2 = 0U; k2 < myDim; ++k2)
+            disp[i][k2] = dx.value()[i * myDim + k2]
+                          + d[this->localView().index(this->localView().tree().child(k2).localIndex(i))[0]];
+      } else
+        for (auto i = 0U; i < disp.size(); ++i)
+          for (auto k2 = 0U; k2 < myDim; ++k2)
+            disp[i][k2] = d[this->localView().index(this->localView().tree().child(k2).localIndex(i))[0]];
+
       auto geo = std::make_shared<const typename GridView::GridView::template Codim<0>::Entity::Geometry>(
           this->localView().element().geometry());
-      Dune::StandardLocalFunction uFunction(localBasis, dispAtNodes, geo);
+      Dune::StandardLocalFunction uFunction(localBasis, disp, geo);
 
       return uFunction;
     }
 
-    auto getStrainFunction(const FERequirementType& par) const { return linearStrains(getDisplacementFunction(par)); }
+    template <class ScalarType = double>
+    auto getStrainFunction(const FERequirementType& par,
+                           const std::optional<const Eigen::VectorX<ScalarType>>& dx = std::nullopt) const {
+      return linearStrains(getDisplacementFunction(par, dx));
+    }
 
     auto getMaterialTangent() const {
-      if constexpr (mydim == 2)
+      if constexpr (myDim == 2)
         return planeStressLinearElasticMaterialTangent(emod_, nu_);
-      else if constexpr (mydim == 3)
+      else if constexpr (myDim == 3)
         return linearElasticMaterialTangent3D(emod_, nu_);
     }
 
     auto getMaterialTangentFunction([[maybe_unused]] const FERequirementType& par) const {
       return [&]([[maybe_unused]] auto gp) { return getMaterialTangent(); };
     }
 
-    double calculateScalar(const FERequirementType& par) const {
-      const auto u       = getDisplacementFunction(par);
-      const auto eps     = getStrainFunction(par);
+    inline double calculateScalar(const FERequirementType& par) const { return calculateScalarImpl<double>(par); }
+
+    inline void calculateVector(const FERequirementType& par, typename Traits::template VectorType<> force) const {
+      calculateVectorImpl<double>(par, force);
+    }
+
+    void calculateMatrix(const FERequirementType& par, typename Traits::template MatrixType<> K) const {
+      const auto eps = getStrainFunction(par);
+      using namespace Dune::DerivativeDirections;
+      using namespace Dune;
+
+      const auto C   = getMaterialTangent();
+      const auto geo = this->localView().element().geometry();
+
+      for (const auto& [gpIndex, gp] : eps.viewOverIntegrationPoints()) {
+        const double intElement = geo.integrationElement(gp.position()) * gp.weight();
+        for (size_t i = 0; i < numberOfNodes; ++i) {
+          const auto bopI = eps.evaluateDerivative(gpIndex, wrt(coeff(i)), on(gridElement));
+          for (size_t j = 0; j < numberOfNodes; ++j) {
+            const auto bopJ = eps.evaluateDerivative(gpIndex, wrt(coeff(j)), on(gridElement));
+            K.template block<myDim, myDim>(i * myDim, j * myDim) += bopI.transpose() * C * bopJ * intElement;
+          }
+        }
+      }
+    }
+
+    void calculateAt(const ResultRequirementsType& req, const Dune::FieldVector<double, Traits::mydim>& local,
+                     ResultTypeMap<double>& result) const {
+      using namespace Dune::Indices;
+      using namespace Dune::DerivativeDirections;
+      using namespace Dune;
+
+      const auto eps = getStrainFunction(req.getFERequirements());
+      const auto C   = getMaterialTangent();
+      auto epsVoigt  = eps.evaluate(local, on(gridElement));
+
+      auto cauchyStress = (C * epsVoigt).eval();
+
+      typename ResultTypeMap<double>::ResultArray resultVector;
+      if (req.isResultRequested(ResultType::linearStress)) {
+        resultVector.resize(3, 1);
+        resultVector = cauchyStress;
+        result.insertOrAssignResult(ResultType::linearStress, resultVector);
+      }
+    }
+
+    Dune::CachedLocalBasis<
+        std::remove_cvref_t<decltype(std::declval<LocalView>().tree().child(0).finiteElement().localBasis())>>
+        localBasis;
+    std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
+                                                          const double&)>
+        volumeLoad;
+    std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
+                                                          const double&)>
+        neumannBoundaryLoad;
+    const BoundaryPatch<GridView>* neumannBoundary;
+    mutable Dune::BlockVector<Dune::RealTuple<double, Traits::dimension>> dispAtNodes;
+    double emod_;
+    double nu_;
+    size_t numberOfNodes{0};
+
+  protected:
+    template <typename ScalarType>
+    auto calculateScalarImpl(const FERequirementType& par, const std::optional<const Eigen::VectorX<ScalarType>>& dx
+                                                           = std::nullopt) const -> ScalarType {
+      const auto u       = getDisplacementFunction(par, dx);
+      const auto eps     = getStrainFunction(par, dx);
       const auto& lambda = par.getParameter(Ikarus::FEParameter::loadfactor);
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
+
       const auto C = getMaterialTangent();
 
-      const auto geo = this->localView().element().geometry();
-      double energy  = 0.0;
+      const auto geo    = this->localView().element().geometry();
+      ScalarType energy = 0.0;
       for (const auto& [gpIndex, gp] : eps.viewOverIntegrationPoints()) {
         const auto EVoigt = eps.evaluate(gpIndex, on(gridElement));
 
         energy += (0.5 * EVoigt.dot(C * EVoigt)) * geo.integrationElement(gp.position()) * gp.weight();
       }
+
       // External forces volume forces over the domain
       if (volumeLoad) {
         for (const auto& [gpIndex, gp] : eps.viewOverIntegrationPoints()) {
           const auto uVal                              = u.evaluate(gpIndex);
-          Eigen::Vector<double, Traits::worlddim> fext = volumeLoad(toEigen(gp.position()), lambda);
+          Eigen::Vector<double, Traits::worlddim> fext = volumeLoad(toEigen(geo.global(gp.position())), lambda);
           energy -= uVal.dot(fext) * geo.integrationElement(gp.position()) * gp.weight();
         }
       }
 
       // line or surface loads, i.e. neumann boundary
-      if (not neumannBoundary) return energy;
+      if (not neumannBoundary and not neumannBoundaryLoad) return energy;
 
       auto element = this->localView().element();
       for (auto&& intersection : intersections(neumannBoundary->gridView(), element)) {
         if (not neumannBoundary->contains(intersection)) continue;
 
-        const auto& quadLine = Dune::QuadratureRules<double, mydim - 1>::rule(intersection.type(), u.order());
+        const auto& quadLine = Dune::QuadratureRules<double, myDim - 1>::rule(intersection.type(), u.order());
 
         for (const auto& curQuad : quadLine) {
           // Local position of the quadrature point
-          const Dune::FieldVector<double, mydim>& quadPos = intersection.geometryInInside().global(curQuad.position());
+          const Dune::FieldVector<double, myDim>& quadPos = intersection.geometryInInside().global(curQuad.position());
 
           const double integrationElement = intersection.geometry().integrationElement(curQuad.position());
 
           // The value of the local function
           const auto uVal = u.evaluate(quadPos);
 
           // Value of the Neumann data at the current position
@@ -144,125 +217,71 @@
 
           energy -= neumannValue.dot(uVal) * curQuad.weight() * integrationElement;
         }
       }
       return energy;
     }
 
-    void calculateMatrix(const FERequirementType& par, typename Traits::MatrixType K) const {
-      const auto eps = getStrainFunction(par);
-      using namespace Dune::DerivativeDirections;
-      using namespace Dune;
-
-      const auto C   = getMaterialTangent();
-      const auto geo = this->localView().element().geometry();
-
-      for (const auto& [gpIndex, gp] : eps.viewOverIntegrationPoints()) {
-        const double intElement = geo.integrationElement(gp.position()) * gp.weight();
-        for (size_t i = 0; i < numberOfNodes; ++i) {
-          const auto bopI = eps.evaluateDerivative(gpIndex, wrt(coeff(i)), on(gridElement));
-          for (size_t j = 0; j < numberOfNodes; ++j) {
-            const auto bopJ = eps.evaluateDerivative(gpIndex, wrt(coeff(j)), on(gridElement));
-            K.template block<mydim, mydim>(i * mydim, j * mydim) += bopI.transpose() * C * bopJ * intElement;
-          }
-        }
-      }
-    }
-
-    void calculateAt(const ResultRequirementsType& req, const Dune::FieldVector<double, Traits::mydim>& local,
-                     ResultTypeMap<double>& result) const {
-      using namespace Dune::Indices;
-      using namespace Dune::DerivativeDirections;
-      using namespace Dune;
-
-      const auto eps = getStrainFunction(req.getFERequirements());
-      const auto C   = getMaterialTangent();
-      auto epsVoigt  = eps.evaluate(local, on(gridElement));
-
-      auto cauchyStress = (C * epsVoigt).eval();
-
-      typename ResultTypeMap<double>::ResultArray resultVector;
-      if (req.isResultRequested(ResultType::linearStress)) {
-        resultVector.resize(3, 1);
-        resultVector = cauchyStress;
-        result.insertOrAssignResult(ResultType::linearStress, resultVector);
-      }
-    }
-
-    void calculateVector(const FERequirementType& par, typename Traits::VectorType force) const {
+    template <typename ScalarType>
+    void calculateVectorImpl(const FERequirementType& par, typename Traits::template VectorType<ScalarType> force,
+                             const std::optional<const Eigen::VectorX<ScalarType>>& dx = std::nullopt) const {
       const auto& lambda = par.getParameter(Ikarus::FEParameter::loadfactor);
-      const auto eps     = getStrainFunction(par);
+      const auto eps     = getStrainFunction(par, dx);
       using namespace Dune::DerivativeDirections;
       using namespace Dune;
 
       const auto C   = getMaterialTangent();
       const auto geo = this->localView().element().geometry();
 
       // Internal forces
       for (const auto& [gpIndex, gp] : eps.viewOverIntegrationPoints()) {
         const double intElement = geo.integrationElement(gp.position()) * gp.weight();
         auto stresses           = (C * eps.evaluate(gpIndex, on(gridElement))).eval();
         for (size_t i = 0; i < numberOfNodes; ++i) {
           const auto bopI = eps.evaluateDerivative(gpIndex, wrt(coeff(i)), on(gridElement));
-          force.template segment<mydim>(mydim * i) += bopI.transpose() * stresses * intElement;
+          force.template segment<myDim>(myDim * i) += bopI.transpose() * stresses * intElement;
         }
       }
 
       // External forces volume forces over the domain
       if (volumeLoad) {
-        const auto u = getDisplacementFunction(par);
+        const auto u = getDisplacementFunction(par, dx);
         for (const auto& [gpIndex, gp] : u.viewOverIntegrationPoints()) {
-          Eigen::Vector<double, Traits::worlddim> fext = volumeLoad(toEigen(gp.position()), lambda);
+          Eigen::Vector<double, Traits::worlddim> fext = volumeLoad(toEigen(geo.global(gp.position())), lambda);
           for (size_t i = 0; i < numberOfNodes; ++i) {
             const auto udCi = u.evaluateDerivative(gpIndex, wrt(coeff(i)));
-            force.template segment<mydim>(mydim * i)
+            force.template segment<myDim>(myDim * i)
                 -= udCi * fext * geo.integrationElement(gp.position()) * gp.weight();
           }
         }
       }
 
       // External forces, boundary forces, i.e. at the Neumann boundary
       if (not neumannBoundary) return;
 
-      const auto u = getDisplacementFunction(par);
+      const auto u = getDisplacementFunction(par, dx);
       auto element = this->localView().element();
       for (auto&& intersection : intersections(neumannBoundary->gridView(), element)) {
         if (not neumannBoundary->contains(intersection)) continue;
 
         // Integration rule along the boundary
-        const auto& quadLine = Dune::QuadratureRules<double, mydim - 1>::rule(intersection.type(), u.order());
+        const auto& quadLine = Dune::QuadratureRules<double, myDim - 1>::rule(intersection.type(), u.order());
 
         for (const auto& curQuad : quadLine) {
-          const Dune::FieldVector<double, mydim>& quadPos = intersection.geometryInInside().global(curQuad.position());
+          const Dune::FieldVector<double, myDim>& quadPos = intersection.geometryInInside().global(curQuad.position());
 
           const double integrationElement = intersection.geometry().integrationElement(curQuad.position());
 
           // The value of the local function wrt the i-th coef
           for (size_t i = 0; i < numberOfNodes; ++i) {
             const auto udCi = u.evaluateDerivative(quadPos, wrt(coeff(i)));
 
             // Value of the Neumann data at the current position
             auto neumannValue
                 = neumannBoundaryLoad(toEigen(intersection.geometry().global(curQuad.position())), lambda);
-            force.template segment<mydim>(mydim * i) -= udCi * neumannValue * curQuad.weight() * integrationElement;
+            force.template segment<myDim>(myDim * i) -= udCi * neumannValue * curQuad.weight() * integrationElement;
           }
         }
       }
     }
-
-    Dune::CachedLocalBasis<
-        std::remove_cvref_t<decltype(std::declval<LocalView>().tree().child(0).finiteElement().localBasis())>>
-        localBasis;
-    std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
-                                                          const double&)>
-        volumeLoad;
-    std::function<Eigen::Vector<double, Traits::worlddim>(const Eigen::Vector<double, Traits::worlddim>&,
-                                                          const double&)>
-        neumannBoundaryLoad;
-    const BoundaryPatch<GridView>* neumannBoundary;
-    mutable Dune::BlockVector<Dune::RealTuple<double, Traits::dimension>> dispAtNodes;
-    double emod_;
-    double nu_;
-    size_t numberOfNodes{0};
   };
-
 }  // namespace Ikarus
```

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/interface.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/interface.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/linearElasticity.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/linearElasticity.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/neohooke.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/neohooke.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/strainConversions.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/strainConversions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/svk.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/svk.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials/vanishingStress.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials/vanishingStress.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/mechanics/materials.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/mechanics/materials.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/finiteElements/physicsHelper.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/finiteElements/physicsHelper.hh`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,20 @@
     /** \brief Dimension of the geometry */
     static constexpr int mydim = GridEntity::mydimension;
 
     /** \brief Dimension of the grid */
     static constexpr int dimension = GridEntity::dimension;
 
     /** \brief Type of the internal forces */
-    using VectorType = std::conditional_t<useRef, Eigen::Ref<Eigen::VectorXd>, Eigen::VectorXd&>;
+    template <typename ScalarType = double>
+    using VectorType = std::conditional_t<useRef, Eigen::Ref<Eigen::VectorX<ScalarType>>, Eigen::VectorX<ScalarType>&>;
 
     /** \brief Type of the stiffness matrix */
-    using MatrixType = std::conditional_t<useRef, Eigen::Ref<Eigen::MatrixXd>, Eigen::MatrixXd&>;
-
-    /** \brief Type of the stiffness matrix */
-    using ScalarType = typename GridEntity::Geometry::ctype;
+    template <typename ScalarType = double>
+    using MatrixType = std::conditional_t<useRef, Eigen::Ref<Eigen::MatrixX<ScalarType>>, Eigen::MatrixX<ScalarType>&>;
   };
 
   /// see https://en.wikipedia.org/wiki/Lam%C3%A9_parameters
   struct YoungsModulusAndPoissonsRatio {
     double emodul;
     double nu;
   };
```

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/io/resultEvaluators.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/io/resultEvaluators.hh`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 
-#include <dune/common/power.hh>
+#include <dune/common/math.hh>
 
 #include <ikarus/finiteElements/feRequirements.hh>
 
 namespace Dune {
   // Forward declaration
   template <typename ScalarType, int size>
   class FieldVector;
```

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/io/resultFunction.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/io/resultFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/linearAlgebra/dirichletValues.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/linearAlgebra/nonLinearOperator.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/nonLinearOperator.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/linearAlgebra/truncatedConjugateGradient.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/linearAlgebra/truncatedConjugateGradient.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/python/assembler/flatAssembler.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/python/assembler/flatAssembler.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/python/basis/basis.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/python/basis/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/python/dirichletValues/dirichletValues.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/python/dirichletValues/dirichletValues.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/python/finiteElements/linearElastic.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/linearElastic.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/python/finiteElements/materials/material.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/materials/material.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/python/finiteElements/nonLinearElastic.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/python/finiteElements/nonLinearElastic.hh`

 * *Files 6% similar despite different names*

```diff
@@ -32,28 +32,25 @@
     using Material       = typename NonLinearElastic::Material;
 
     cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, const Material& mat) {
               return new NonLinearElastic(basis, element, mat);
             }),
             pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>());
 
-    cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, const Material& mat,
-                              const std::function<Eigen::Vector<double, Traits::worlddim>(
-                                  Eigen::Vector<double, Traits::worlddim>, const double&)>
-                                  volumeLoad) { return new NonLinearElastic(basis, element, mat, volumeLoad); }),
+    using LoadFunction = std::function<Eigen::Vector<double, Traits::worlddim>(Eigen::Vector<double, Traits::worlddim>,
+                                                                               const double&)>;
+
+    cls.def(pybind11::init(
+                [](const GlobalBasis& basis, const Element& element, const Material& mat,
+                   const LoadFunction volumeLoad) { return new NonLinearElastic(basis, element, mat, volumeLoad); }),
             pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>());
 
     cls.def(pybind11::init([](const GlobalBasis& basis, const Element& element, const Material& mat,
-                              const std::function<Eigen::Vector<double, Traits::worlddim>(
-                                  Eigen::Vector<double, Traits::worlddim>, const double&)>
-                                  volumeLoad,
-                              const BoundaryPatch<GridView>& bp,
-                              const std::function<Eigen::Vector<double, Traits::worlddim>(
-                                  Eigen::Vector<double, Traits::worlddim>, const double&)>
-                                  neumannBoundaryLoad) {
+                              const LoadFunction volumeLoad, const BoundaryPatch<GridView>& bp,
+                              const LoadFunction neumannBoundaryLoad) {
               return new NonLinearElastic(basis, element, mat, volumeLoad, &bp, neumannBoundaryLoad);
             }),
             pybind11::keep_alive<1, 2>(), pybind11::keep_alive<1, 3>(), pybind11::keep_alive<1, 7>());
 
     pybind11::module scopedf = pybind11::module::import("dune.functions");
 
     typedef Dune::Python::LocalViewWrapper<FlatBasis> LocalViewWrapper;
```

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/python/test/linearElasticTest.py` & `pyikarus-0.3.3.dev20230601114417/ikarus/python/test/linearElasticTest.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/python/test/nonLinearElasticTest.py` & `pyikarus-0.3.3.dev20230601114417/ikarus/python/test/nonLinearElasticTest.py`

 * *Files 7% similar despite different names*

```diff
@@ -108,31 +108,27 @@
         reqL.addAffordance(iks.MatrixAffordances.stiffness)
         reqL.insertParameter(iks.FEParameter.loadfactor, lambdaLoad)
 
         dBig = assembler.createFullVector(dRedInput)
         reqL.insertGlobalSolution(iks.FESolutions.displacement, dBig)
         return assembler.getReducedMatrix(reqL).todense()
 
-    print("energy(dRed):", energy(dRed))
-    print("energyafer")
     resultd = minimize(energy, x0=dRed, options={"disp": True}, tol=1e-14)
     resultd2 = minimize(
         energy, x0=dRed, jac=gradient, options={"disp": True}, tol=1e-14
     )
     resultd3 = minimize(
         energy,
         method="trust-constr",
         x0=dRed,
         jac=gradient,
         hess=hess,
         options={"disp": True},
     )
-    resultd4 = sp.optimize.root(
-        gradient, jac=hess, x0=dRed, options={"disp": True}, tol=1e-10
-    )
-    # print(assembler.createFullVector(resultd.g))
+    resultd4 = sp.optimize.root(        gradient, jac=hess, x0=dRed, tol=1e-10    )
+
     np.set_printoptions(precision=3)
 
     assert np.allclose(resultd.x, resultd2.x, atol=1e-6)
     assert np.allclose(resultd3.x, resultd4.x)
     assert np.all(abs(resultd3.grad) < 1e-8)
     assert np.all(abs(resultd4.fun) < 1e-8)
```

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/python/test/setpath.py.in` & `pyikarus-0.3.3.dev20230601114417/ikarus/python/test/setpath.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/python/utils/boundarypatch.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/python/utils/boundarypatch.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/solver/linearSolver/linearSolver.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/solver/linearSolver/linearSolver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/solver/nonLinearSolver/newtonRaphson.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/newtonRaphson.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/newtonRaphsonWithScalarSubsidiaryFunction.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/solver/nonLinearSolver/trustRegion.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/solver/nonLinearSolver/trustRegion.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/algorithms.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/algorithms.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/autodiffHelper.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/autodiffHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/basis.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/basis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/concepts.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/concepts.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/drawing/griddrawer.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/griddrawer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/drawing/matplotHelper.cpp` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/matplotHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/drawing/matplotHelper.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/drawing/matplotHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/duneUtilities.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/duneUtilities.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/eigenDuneTransformations.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/eigenDuneTransformations.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/eigenSparseAddon.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/eigenSparseAddon.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/findLineSegment.cpp` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/findLineSegment.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/findLineSegment.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/findLineSegment.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/flatPreBasis.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/flatPreBasis.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/functionSanityChecks.cpp` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/functionSanityChecks.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/functionSanityChecks.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/functionSanityChecks.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/init.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/init.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/linearAlgebraHelper.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/linearAlgebraHelper.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/makeEnum.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/makeEnum.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/controlLogger.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/controlLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/controlVTKWriter.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/controlVTKWriter.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/genericControlObserver.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/genericControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/gridDrawerObserver.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/gridDrawerObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/loadControlObserver.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/loadControlObserver.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/nonLinearSolverLogger.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/nonLinearSolverLogger.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/observer/observer.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/observer/observer.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/pathFollowingFunctions.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/pathFollowingFunctions.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/polyfit.cpp` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/polyfit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/polyfit.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/polyfit.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/tensorUtils.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/tensorUtils.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/ikarus/utils/traits.hh` & `pyikarus-0.3.3.dev20230601114417/ikarus/utils/traits.hh`

 * *Files 0% similar despite different names*

```diff
@@ -399,8 +399,13 @@
   /**
    * \brief Specialization for lambdas using std::void_t to allow a specialization of the original template
    *        The lambda is forwarded using lambdas operator() to the general function traits
    */
   template <typename T>
   struct FunctionTraits<T, Dune::void_t<decltype(&T::operator())>> : public FunctionTraits<decltype(&T::operator())> {};
 
+  template <typename T = void>
+  struct DummyFalse {
+    static constexpr bool value = false;
+  };
+
 }  // namespace Ikarus::Std
```

### Comparing `pyikarus-0.3.3.dev20230523103500/python/ikarus/__init__.py` & `pyikarus-0.3.3.dev20230601114417/python/ikarus/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/python/ikarus/_ikarus.cc` & `pyikarus-0.3.3.dev20230601114417/python/ikarus/_ikarus.cc`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/python/ikarus/assembler/__init__.py` & `pyikarus-0.3.3.dev20230601114417/python/ikarus/assembler/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/python/ikarus/basis.py` & `pyikarus-0.3.3.dev20230601114417/python/ikarus/basis.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/python/ikarus/dirichletValues.py` & `pyikarus-0.3.3.dev20230601114417/python/ikarus/dirichletValues.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/python/ikarus/finite_elements/__init__.py` & `pyikarus-0.3.3.dev20230601114417/python/ikarus/finite_elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/python/ikarus/generator.py` & `pyikarus-0.3.3.dev20230601114417/python/ikarus/generator.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/python/ikarus/materials.py` & `pyikarus-0.3.3.dev20230601114417/python/ikarus/materials.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/python/ikarus/utils/__init__.py` & `pyikarus-0.3.3.dev20230601114417/python/ikarus/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/python/pyikarus.egg-info/PKG-INFO` & `pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyikarus
-Version: 0.3.3.dev20230523103500
+Version: 0.3.3.dev20230601114417
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
-Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230523103500 Home-
+Metadata-Version: 2.1 Name: pyikarus Version: 0.3.3.dev20230601114417 Home-
 page: Author: mueller@ibb.uni-stuttgart.de Author-email: mueller@ibb.uni-
 stuttgart.de Classifier: Programming Language :: C++ Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License (GPL) Requires-Python: >=3.4 Description-Content-Type: text/
 markdown License-File: LICENSE.md  # Ikarus [![Debian](https://github.com/
 ikarus-project/ikarus/actions/workflows/debian.yml/badge.svg)](https://
 github.com/ikarus-project/ikarus/actions/workflows/debian.yml) [![codecov]
```

### Comparing `pyikarus-0.3.3.dev20230523103500/python/pyikarus.egg-info/SOURCES.txt` & `pyikarus-0.3.3.dev20230601114417/python/pyikarus.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -233,34 +233,34 @@
 python/pyikarus.egg-info/top_level.txt
 sandbox/CMakeLists.txt
 sandbox/src/CMakeLists.txt
 sandbox/src/sandbox.cpp
 sandbox/src/auxiliaryFiles/circle.msh
 tests/CMakeLists.txt
 tests/src/CMakeLists.txt
-tests/src/assemblerTest.cpp
-tests/src/common.hh
-tests/src/dependenciesTest.cpp
-tests/src/dirichletValueTest.cpp
-tests/src/easTest.hh
-tests/src/enhancedAssumedStrainsTest.cpp
-tests/src/factories.hh
-tests/src/functionTraitsTest.cpp
-tests/src/linearElasticityTest.cpp
-tests/src/manifoldsTest.cpp
-tests/src/materialTest.cpp
-tests/src/nonLinearElasticityTest.hh
-tests/src/nonLinearElasticityTestNeoHooke.cpp
-tests/src/nonLinearElasticityTestSVK.cpp
-tests/src/nonLinearOperatorTest.cpp
-tests/src/pathFollowingTest.cpp
-tests/src/polyFitTest.cpp
-tests/src/pythonConversionTest.cpp
+tests/src/testAssembler.cpp
 tests/src/testAutodiffHelper.cpp
+tests/src/testCommon.hh
+tests/src/testDependencies.cpp
+tests/src/testDirichletValue.cpp
+tests/src/testEAS.hh
+tests/src/testEnhancedAssumedStrains.cpp
 tests/src/testFEElement.hh
+tests/src/testFactories.hh
+tests/src/testFunctionTraits.cpp
 tests/src/testHelpers.hh
-tests/src/trustRegionTest.cpp
+tests/src/testLinearElasticity.cpp
+tests/src/testManifolds.cpp
+tests/src/testMaterial.cpp
+tests/src/testNonLinearElasticity.hh
+tests/src/testNonLinearElasticityNeoHooke.cpp
+tests/src/testNonLinearElasticitySVK.cpp
+tests/src/testNonLinearOperator.cpp
+tests/src/testPathFollowing.cpp
+tests/src/testPolyFit.cpp
+tests/src/testPythonConversion.cpp
+tests/src/testTrustRegion.cpp
 tests/src/testFiles/unstructuredQuadscoarse.msh
 tests/src/testFiles/unstructuredTest.geo
 tests/src/testFiles/unstructuredTest.msh
 tests/src/testFiles/unstructuredTest2.geo
 tests/src/testFiles/unstructuredTrianglesfine.msh
```

### Comparing `pyikarus-0.3.3.dev20230523103500/python/setup.py.in` & `pyikarus-0.3.3.dev20230601114417/python/setup.py.in`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/sandbox/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601114417/sandbox/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/sandbox/src/auxiliaryFiles/circle.msh` & `pyikarus-0.3.3.dev20230601114417/sandbox/src/auxiliaryFiles/circle.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/setup.py` & `pyikarus-0.3.3.dev20230601114417/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # build _ikarus
 # cd /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env pip install twine scikit-build
 # git config --global --add safe.directory /tmp/Ikarus
 # /dune/dune-common/build-cmake/run-in-dune-env python setup.py sdist
 # /dune/dune-common/build-cmake/run-in-dune-env python -m twine upload dist/* --verbose
 
-ikarusVersion = "0.3.3.dev20230523103500"
+ikarusVersion = "0.3.3.dev20230601114417"
 duneVersion = "2.9.0"
 
 metadata = metaData(duneVersion)[1]
 metadata["version"] = ikarusVersion
 
 # refactor since ikarus pypi package already exists
 metadata["name"] = "pyikarus"
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/CMakeLists.txt` & `pyikarus-0.3.3.dev20230601114417/tests/src/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/assemblerTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testAssembler.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/common.hh` & `pyikarus-0.3.3.dev20230601114417/tests/src/testCommon.hh`

 * *Files 23% similar despite different names*

```diff
@@ -3,18 +3,23 @@
 
 #pragma once
 
 #include <vector>
 
 #include <dune/alugrid/grid.hh>
 #include <dune/common/test/testsuite.hh>
+#include <dune/fufem/boundarypatch.hh>
 #include <dune/functions/functionspacebases/lagrangedgbasis.hh>
+#include <dune/grid/uggrid.hh>
 #include <dune/grid/yaspgrid.hh>
 #include <dune/iga/nurbsgrid.hh>
+#include <dune/localfefunctions/cachedlocalBasis/cachedlocalBasis.hh>
 
+#include <ikarus/finiteElements/feBases/autodiffFE.hh>
+#include <ikarus/finiteElements/feBases/powerBasisFE.hh>
 #include <ikarus/finiteElements/feRequirements.hh>
 #include <ikarus/utils/duneUtilities.hh>
 #include <ikarus/utils/eigenDuneTransformations.hh>
 #include <ikarus/utils/functionSanityChecks.hh>
 #include <ikarus/utils/linearAlgebraHelper.hh>
 
 namespace Grids {
@@ -73,36 +78,74 @@
   static void construct(std::vector<Dune::FieldVector<double, size>>& values, const int corners = 10) {
     values.resize(corners);
     std::generate(values.begin(), values.end(),
                   []() { return Ikarus::createRandomVector<Dune::FieldVector<double, size>>(); });
   }
 };
 
+enum class CornerDistortionFlag { unDistorted, fixedDistorted, randomlyDistorted };
+
 // Corner factory for element with codim==0, e.g. no surfaces in 3D
 template <int gridDim>
 struct ValidCornerFactory {
   static void construct(std::vector<Dune::FieldVector<double, gridDim>>& values, const Dune::GeometryType& type,
-                        const bool& isRandomlyDistorted) {
+                        const CornerDistortionFlag& distortionFlag) {
     const auto& refElement = Dune::ReferenceElements<double, gridDim>::general(type);
 
     const auto numberOfVertices = refElement.size(gridDim);
 
     values.resize(numberOfVertices);
     for (int i = 0; i < numberOfVertices; ++i)
       values[i] = refElement.position(i, gridDim);
 
-    /// perturb corner values slightly
-    if (isRandomlyDistorted) {
+    /// Perturbation of the corner values
+    if (distortionFlag == CornerDistortionFlag::unDistorted)
+      return;
+    else if (distortionFlag == CornerDistortionFlag::fixedDistorted) {
+      if (not((gridDim == 2) and (numberOfVertices == 4)))
+        DUNE_THROW(Dune::NotImplemented, "Fixed distortion is only implemented for a 2D 4-node element (Q1)");
+      std::vector<Dune::FieldVector<double, gridDim>> randomnessOnNodes;
+      randomnessOnNodes.push_back({-0.2, -0.05});
+      randomnessOnNodes.push_back({-0.15, 0.05});
+      randomnessOnNodes.push_back({0.15, 0.15});
+      randomnessOnNodes.push_back({-0.05, -0.1});
+      for (long i = 0; i < 4; ++i)
+        values[i] += randomnessOnNodes[i];
+    } else if (distortionFlag == CornerDistortionFlag::randomlyDistorted) {
       std::transform(values.begin(), values.end(), values.begin(), [](const auto& vec) {
         return vec + Ikarus::createRandomVector<Dune::FieldVector<double, gridDim>>(-0.2, 0.2);
       });
-    }
+    } else
+      DUNE_THROW(Dune::IOError, "Incorrect CornerDistortionFlag entered");
   }
 };
 
+template <int gridDim>
+auto createUGGridFromCorners(const CornerDistortionFlag& distortionFlag) {
+  using Grid = Dune::UGGrid<gridDim>;
+
+  std::vector<Dune::FieldVector<double, gridDim>> corners;
+
+  const int numberOfVertices = Dune::power(2, gridDim);
+  ValidCornerFactory<gridDim>::construct(corners, Dune::GeometryTypes::cube(gridDim), distortionFlag);
+
+  std::vector<unsigned int> vertexArrangment;
+  vertexArrangment.resize(numberOfVertices);
+  std::iota(vertexArrangment.begin(), vertexArrangment.end(), 0);
+
+  Dune::GridFactory<Grid> gridFactory;
+  for (auto& corner : corners) {
+    gridFactory.insertVertex(corner);
+  }
+  gridFactory.insertElement(Dune::GeometryTypes::cube(gridDim), vertexArrangment);
+
+  std::unique_ptr<Grid> grid = gridFactory.createGrid();
+  return grid;
+}
+
 template <typename Ele>
 struct ElementTest {};
 
 template <typename NonLinearOperator>
 [[nodiscard]] auto checkGradientOfElement(NonLinearOperator& nonLinearOperator,
                                           const std::string& messageIfFailed = "") {
   Dune::TestSuite t("Check gradient");
@@ -196,7 +239,70 @@
           = Dune::FloatCmp::eq<double, Dune::FloatCmp::CmpStyle::absolute>(FEStressComponent, expectedStressComponent);
       t.check(isStressCorrect) << "Stress component " << voigtIndex << " at node " << c << " is not correctly computed"
                                << messageIfFailed;
     }
   }
   return t;
 }
+
+template <typename NonLinearOperator, typename FiniteElement,
+          typename FERequirementType = FiniteElement::FERequirementType>
+[[nodiscard]] auto checkFEByAutoDiff(NonLinearOperator&, FiniteElement& fe, FERequirementType req,
+                                     const std::string& messageIfFailed = "") {
+  Dune::TestSuite t("Check calculateScalarImpl() and calculateVectorImpl() by Automatic Differentiation");
+  auto& basis           = fe.localView().globalBasis();
+  auto nDOF             = basis.size();
+  using AutoDiffBasedFE = Ikarus::AutoDiffFE<FiniteElement, FERequirementType, false, true>;
+  AutoDiffBasedFE feAutoDiff(fe);
+
+  const double tol = 1e-10;
+
+  Eigen::MatrixXd K, KAutoDiff;
+  K.setZero(nDOF, nDOF);
+  KAutoDiff.setZero(nDOF, nDOF);
+
+  fe.calculateMatrix(req, K);
+  feAutoDiff.calculateMatrix(req, KAutoDiff);
+
+  if constexpr (requires { feAutoDiff.getFE().getNumberOfEASParameters(); }) {
+    t.check(fe.getNumberOfEASParameters() == feAutoDiff.getFE().getNumberOfEASParameters())
+        << "Number of EAS parameters for FE(" << fe.getNumberOfEASParameters()
+        << ") and number of EAS parameters for AutodiffFE(" << feAutoDiff.getFE().getNumberOfEASParameters()
+        << ") are not equal";
+  }
+
+  t.check(K.isApprox(KAutoDiff, tol),
+          "Mismatch between the stiffness matrices obtained from explicit implementation and the one based on "
+          "automatic differentiation")
+      << messageIfFailed << "\nKAutoDiff:\n"
+      << KAutoDiff << "\nK:\n"
+      << K;
+
+  try {
+    Eigen::VectorXd R, RAutoDiff;
+    R.setZero(nDOF);
+    RAutoDiff.setZero(nDOF);
+
+    fe.calculateVector(req, R);
+    feAutoDiff.calculateVector(req, RAutoDiff);
+    t.check(R.isApprox(RAutoDiff, tol),
+            "Mismatch between the residual vectors obtained from explicit implementation and the one based on "
+            "automatic differentiation")
+        << messageIfFailed << "\nRAutoDiff:\n"
+        << RAutoDiff << "\nR:\n"
+        << R;
+  } catch (const Dune::NotImplemented&) {
+    /// calculateVector not checked since the element throws a Dune::NotImplemented
+  }
+
+  try {
+    auto energy         = fe.calculateScalar(req);
+    auto energyAutoDiff = feAutoDiff.calculateScalar(req);
+    t.check(Dune::FloatCmp::eq(energy, energyAutoDiff, tol),
+            "Mismatch between the energies obtained from explicit implementation and the one based on "
+            "automatic differentiation")
+        << messageIfFailed;
+  } catch (const Dune::NotImplemented&) {
+  }
+
+  return t;
+}
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/dependenciesTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testDependencies.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/dirichletValueTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testDirichletValue.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/easTest.hh` & `pyikarus-0.3.3.dev20230601114417/tests/src/testEAS.hh`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 
-#include "common.hh"
+#include "testCommon.hh"
 
 #include <variant>
 
 #include <ikarus/finiteElements/mechanics/enhancedAssumedStrains.hh>
+
 template <typename DisplacementBasedElement>
 struct ElementTest<Ikarus::EnhancedAssumedStrains<DisplacementBasedElement>> {
   [[nodiscard]] static auto test() {
-    auto easFunctor = [](auto& nonLinOp, auto& fe) {
+    auto easFunctor = [](auto& nonLinOp, auto& fe, auto& req) {
       const auto& localView = fe.localView();
       const auto& element   = localView.element();
       constexpr int gridDim = std::remove_cvref_t<decltype(element)>::dimension;
 
       Dune::TestSuite t("EAS specific test");
 
       auto subOp = nonLinOp.template subOperator<1, 2>();
@@ -33,14 +34,15 @@
         auto messageIfFailed = "The numbers of EAS parameters are " + std::to_string(numberOfEASParameter) + ".";
         if (numberOfEASParameter == 0) {
           nonLinOp.updateAll();
           t.subTest(checkGradientOfElement(nonLinOp, messageIfFailed));
           t.subTest(checkHessianOfElement(nonLinOp, messageIfFailed));
         }
         t.subTest(checkJacobianOfElement(subOp, messageIfFailed));
+        t.subTest(checkFEByAutoDiff(nonLinOp, fe, req, messageIfFailed));
 
         auto stiffnessMatrix = subOp.derivative();
 
         Eigen::SelfAdjointEigenSolver<Eigen::MatrixXd> es(stiffnessMatrix);
         newEigenValues = es.eigenvalues();
 
         t.check((newEigenValues.array() < 1e-6 * newEigenValues.norm()).count() == 3 * gridDim - 3,
@@ -64,25 +66,27 @@
         auto rule       = Dune::QuadratureRules<double, gridDim>::rule(localView.element().type(), order);
 
         if (numberOfEASParameter > 0) {
           auto easVariantCopy    = fe.easVariant();  // This only test if the variant has a copy assignment operator
           const auto& easVariant = fe.easVariant();
           std::visit(
               [&]<typename EAS>(const EAS& easFunction) {
-                typename EAS::MType MIntegrated;
-                MIntegrated.setZero();
-                for (const auto& gp : rule) {
-                  const auto M = easFunction.calcM(gp.position());
-
-                  const double detJ = element.geometry().integrationElement(gp.position());
-                  MIntegrated += M * detJ * gp.weight();
+                if constexpr (not std::is_same_v<std::monostate, EAS>) {
+                  typename EAS::MType MIntegrated;
+                  MIntegrated.setZero();
+                  for (const auto& gp : rule) {
+                    const auto M = easFunction.calcM(gp.position());
+
+                    const double detJ = element.geometry().integrationElement(gp.position());
+                    MIntegrated += M * detJ * gp.weight();
+                  }
+                  t.check(MIntegrated.isZero())
+                      << "Orthogonality condition check: The M matrix of the EAS method should be "
+                         "zero, integrated over the domain.";
                 }
-                t.check(MIntegrated.isZero())
-                    << "Orthogonality condition check: The M matrix of the EAS method should be "
-                       "zero, integrated over the domain.";
               },
               easVariant);
           try {
             auto requirements = Ikarus::FErequirements();
             fe.calculateScalar(requirements);
             t.check(false) << "fe.calculateScalar should have failed for numberOfEASParameter > 0";
           } catch (const Dune::NotImplemented&) {
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/enhancedAssumedStrainsTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testEnhancedAssumedStrains.cpp`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #include <config.h>
 
-#include "easTest.hh"
+#include "testEAS.hh"
 #include "testFEElement.hh"
 
 #include <dune/common/test/testsuite.hh>
 #include <dune/functions/functionspacebases/basistags.hh>
 #include <dune/functions/functionspacebases/lagrangebasis.hh>
 #include <dune/functions/functionspacebases/powerbasis.hh>
 
@@ -16,24 +16,26 @@
 #include <ikarus/utils/init.hh>
 
 using Dune::TestSuite;
 
 template <typename Basis>
 using EASElement = Ikarus::EnhancedAssumedStrains<Ikarus::LinearElastic<Basis>>;
 
-template <typename Basis>
-using LinearElasticElement = Ikarus::LinearElastic<Basis>;
-
 int main(int argc, char** argv) {
   Ikarus::init(argc, argv);
   TestSuite t("EAS");
 
   using namespace Dune::Functions::BasisFactory;
   auto firstOrderLagrangePrePower2Basis = power<2>(lagrange<1>(), FlatInterleaved());
   auto firstOrderLagrangePrePower3Basis = power<3>(lagrange<1>(), FlatInterleaved());
+  const auto randomlyDistorted          = CornerDistortionFlag::randomlyDistorted;
+  const auto unDistorted                = CornerDistortionFlag::unDistorted;
 
-  t.subTest(testFEElement<EASElement, 2>(firstOrderLagrangePrePower2Basis, "EAS", true, checkJacobianFunctor));
-  t.subTest(testFEElement<EASElement, 3>(firstOrderLagrangePrePower3Basis, "EAS", true, checkJacobianFunctor));
-  t.subTest(testFEElement<EASElement, 2>(firstOrderLagrangePrePower2Basis, "EAS", false, checkCauchyStressFunctor));
+  t.subTest(
+      testFEElement<EASElement, 2>(firstOrderLagrangePrePower2Basis, "EAS", randomlyDistorted, checkJacobianFunctor));
+  t.subTest(
+      testFEElement<EASElement, 3>(firstOrderLagrangePrePower3Basis, "EAS", randomlyDistorted, checkJacobianFunctor));
+  t.subTest(
+      testFEElement<EASElement, 2>(firstOrderLagrangePrePower2Basis, "EAS", unDistorted, checkCauchyStressFunctor));
 
   return t.exit();
 }
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/functionTraitsTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testFunctionTraits.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/linearElasticityTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testLinearElasticity.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 
 #include <config.h>
 
 #include "testFEElement.hh"
 
 #include <dune/common/test/testsuite.hh>
 #include <dune/functions/functionspacebases/basistags.hh>
-#include <dune/functions/functionspacebases/compositebasis.hh>
 #include <dune/functions/functionspacebases/lagrangebasis.hh>
 #include <dune/functions/functionspacebases/powerbasis.hh>
 
 #include <ikarus/finiteElements/mechanics/linearElastic.hh>
-#include <ikarus/utils/flatPreBasis.hh>
 #include <ikarus/utils/init.hh>
 
 using Dune::TestSuite;
 
 template <typename Basis>
 using LinearElasticElement = Ikarus::LinearElastic<Basis>;
 
@@ -26,22 +24,29 @@
 
   using namespace Dune::Functions::BasisFactory;
   auto firstOrderLagrangePrePower2Basis         = power<2>(lagrange<1>(), FlatInterleaved());
   auto secondOrderLagrangePrePower2Basis        = power<2>(lagrange<2>(), FlatInterleaved());
   auto firstOrderLagrangePrePower3Basis         = power<3>(lagrange<1>(), FlatInterleaved());
   auto secondOrderLagrangePrePower3Basis        = power<3>(lagrange<2>(), FlatInterleaved());
   auto secondOrderLagrangePrePower3BasisBlocked = power<3>(lagrange<2>());
+  const auto randomlyDistorted                  = CornerDistortionFlag::randomlyDistorted;
+  const auto unDistorted                        = CornerDistortionFlag::unDistorted;
 
-  t.subTest(testFEElement<LinearElasticElement, 2>(firstOrderLagrangePrePower2Basis, "LinearElastic", true,
-                                                   checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor));
-  t.subTest(testFEElement<LinearElasticElement, 2>(secondOrderLagrangePrePower2Basis, "LinearElastic", true,
-                                                   checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor));
-  t.subTest(testFEElement<LinearElasticElement, 3>(firstOrderLagrangePrePower3Basis, "LinearElastic", true,
-                                                   checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor));
-  t.subTest(testFEElement<LinearElasticElement, 3>(secondOrderLagrangePrePower3Basis, "LinearElastic", true,
-                                                   checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor));
-  t.subTest(testFEElement<LinearElasticElement, 3>(secondOrderLagrangePrePower3BasisBlocked, "LinearElastic", true,
-                                                   checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor));
-  t.subTest(testFEElement<LinearElasticElement, 2>(firstOrderLagrangePrePower2Basis, "LinearElastic", false,
+  t.subTest(testFEElement<LinearElasticElement, 2>(firstOrderLagrangePrePower2Basis, "LinearElastic", randomlyDistorted,
+                                                   checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor,
+                                                   checkFEByAutoDiffFunctor));
+  t.subTest(testFEElement<LinearElasticElement, 2>(secondOrderLagrangePrePower2Basis, "LinearElastic",
+                                                   randomlyDistorted, checkGradientFunctor, checkHessianFunctor,
+                                                   checkJacobianFunctor, checkFEByAutoDiffFunctor));
+  t.subTest(testFEElement<LinearElasticElement, 3>(firstOrderLagrangePrePower3Basis, "LinearElastic", randomlyDistorted,
+                                                   checkGradientFunctor, checkHessianFunctor, checkJacobianFunctor,
+                                                   checkFEByAutoDiffFunctor));
+  t.subTest(testFEElement<LinearElasticElement, 3>(secondOrderLagrangePrePower3Basis, "LinearElastic",
+                                                   randomlyDistorted, checkGradientFunctor, checkHessianFunctor,
+                                                   checkJacobianFunctor, checkFEByAutoDiffFunctor));
+  t.subTest(testFEElement<LinearElasticElement, 3>(secondOrderLagrangePrePower3BasisBlocked, "LinearElastic",
+                                                   randomlyDistorted, checkGradientFunctor, checkHessianFunctor,
+                                                   checkJacobianFunctor, checkFEByAutoDiffFunctor));
+  t.subTest(testFEElement<LinearElasticElement, 2>(firstOrderLagrangePrePower2Basis, "LinearElastic", unDistorted,
                                                    checkCauchyStressFunctor));
   return t.exit();
 }
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/manifoldsTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testManifolds.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -2,25 +2,21 @@
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #include <config.h>
 
 #include "testHelpers.hh"
 
 #include <array>
-#include <fstream>
-#include <unordered_set>
-#include <vector>
 
 #include <dune/common/test/testsuite.hh>
 #include <dune/localfefunctions/manifolds/realTuple.hh>
 #include <dune/localfefunctions/manifolds/unitVector.hh>
 
 #include <Eigen/Core>
 
-#include <ikarus/utils/algorithms.hh>
 #include <ikarus/utils/init.hh>
 
 using Dune::TestSuite;
 
 static constexpr double tol = 1e-15;
 
 auto testUnitVector() {
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/materialTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testMaterial.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 #include <Eigen/Eigenvalues>
 
 #include <ikarus/finiteElements/mechanics/materials.hh>
 #include <ikarus/finiteElements/physicsHelper.hh>
 #include <ikarus/linearAlgebra/nonLinearOperator.hh>
 #include <ikarus/utils/functionSanityChecks.hh>
 #include <ikarus/utils/init.hh>
+
 using namespace Ikarus;
 using Dune::TestSuite;
 
 template <StrainTags strainTag, typename MaterialImpl>
 auto testMaterialWithStrain(const MaterialImpl& mat, const double tol = 1e-14) {
   TestSuite t(mat.name() + " InputStrainMeasure: " + toString(strainTag));
   std::cout << "Test: " << t.name() << " started\n";
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/nonLinearElasticityTestNeoHooke.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearElasticityNeoHooke.cpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 //
 #include <config.h>
 
-#include "common.hh"
-#include "nonLinearElasticityTest.hh"
-#include "testHelpers.hh"
+#include "testNonLinearElasticity.hh"
 
 using Dune::TestSuite;
 
 int main(int argc, char** argv) {
   Ikarus::init(argc, argv);
   TestSuite t;
 
   auto matParameter = Ikarus::toLamesFirstParameterAndShearModulus({.emodul = 1000, .nu = 0.3});
 
   Ikarus::NeoHooke matNH(matParameter);
 
   t.subTest(NonLinearElasticityLoadControlNRandTR<Grids::Alu>(matNH));
-  //  t.subTest(NonLinearElasticityLoadControlNRandTR<Grids::Yasp>(matNH));
-  //  t.subTest(NonLinearElasticityLoadControlNRandTR<Grids::Iga>(matNH));
+  t.subTest(NonLinearElasticityLoadControlNRandTR<Grids::Yasp>(matNH));
+  t.subTest(NonLinearElasticityLoadControlNRandTR<Grids::Iga>(matNH));
   return t.exit();
 }
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/nonLinearOperatorTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testNonLinearOperator.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #include <Eigen/Core>
 
 #include <ikarus/linearAlgebra/nonLinearOperator.hh>
 #include <ikarus/solver/nonLinearSolver/newtonRaphson.hh>
 #include <ikarus/utils/functionSanityChecks.hh>
 #include <ikarus/utils/init.hh>
 #include <ikarus/utils/observer/nonLinearSolverLogger.hh>
+
 using namespace Ikarus;
 using Dune::TestSuite;
 
 template <typename SolutionType, typename SolutionTypeExpected, typename NewtonRhapson>
 auto checkNewtonRhapson(NewtonRhapson& nr, SolutionType& x, double tolerance, int maxIter, int iterExpected,
                         const SolutionTypeExpected& xExpected, const auto& x_Predictor) {
   TestSuite t("checkNewtonRhapson");
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/pathFollowingTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testPathFollowing.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/polyFitTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testPolyFit.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/pythonConversionTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testPythonConversion.cpp`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
+
 #include <config.h>
 
 #include <dune/common/test/testsuite.hh>
 
 #include <ikarus/utils/duneUtilities.hh>
 #include <ikarus/utils/init.hh>
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/testAutodiffHelper.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testAutodiffHelper.cpp`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/testFEElement.hh` & `pyikarus-0.3.3.dev20230601114417/tests/src/testFEElement.hh`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,42 @@
 // SPDX-FileCopyrightText: 2022 The Ikarus Developers mueller@ibb.uni-stuttgart.de
 // SPDX-License-Identifier: LGPL-3.0-or-later
 
 #pragma once
 
-#include "common.hh"
+#include "testCommon.hh"
 
 #include <dune/common/bitsetvector.hh>
 #include <dune/fufem/boundarypatch.hh>
 #include <dune/grid/uggrid.hh>
 
-#include "ikarus/io/resultFunction.hh"
 #include <ikarus/assembler/simpleAssemblers.hh>
 #include <ikarus/finiteElements/feRequirements.hh>
+#include <ikarus/io/resultFunction.hh>
 #include <ikarus/linearAlgebra/dirichletValues.hh>
 #include <ikarus/linearAlgebra/nonLinearOperator.hh>
 #include <ikarus/utils/basis.hh>
 
 /** These tests test your element on some gridElement with some basis
  *
  * @tparam FEElementTemplate The element as template template parameter. The template needs to be the globalBasis
  * @tparam gridDim The dimension of the grid element the finite element should be tested
  * @tparam PreBasis The preBasis you want to test the element with
  * @tparam F A variadic number of the test functor you want to be checked, they need to accept a non-linear operator and
  * the finite element
  */
 template <template <typename> typename FEElementTemplate, int gridDim, typename PreBasis, typename... F>
-auto testFEElement(const PreBasis& preBasis, const std::string& elementName, const bool& isRandomlyDistorted,
+auto testFEElement(const PreBasis& preBasis, const std::string& elementName, const CornerDistortionFlag& distortionFlag,
                    F&&... f) {
   Dune::TestSuite t(std::string("testFEElement ") + elementName + " on grid element with dimension "
                     + std::to_string(gridDim));
 
   auto fTuple = std::forward_as_tuple(f...);
 
-  using Grid = Dune::UGGrid<gridDim>;
-
-  std::vector<Dune::FieldVector<double, gridDim>> corners;
-
-  const int numberOfVertices = Dune::power(2, gridDim);
-  ValidCornerFactory<gridDim>::construct(corners, Dune::GeometryTypes::cube(gridDim), isRandomlyDistorted);
-
-  std::vector<unsigned int> vertexArrangment;
-  vertexArrangment.resize(numberOfVertices);
-  std::iota(vertexArrangment.begin(), vertexArrangment.end(), 0);
-
-  Dune::GridFactory<Grid> gridFactory;
-  for (auto& corner : corners) {
-    gridFactory.insertVertex(corner);
-  }
-  gridFactory.insertElement(Dune::GeometryTypes::cube(gridDim), vertexArrangment);
-
-  std::unique_ptr<Grid> grid = gridFactory.createGrid();
+  auto grid = createUGGridFromCorners<gridDim>(distortionFlag);
 
   auto gridView = grid->leafGridView();
   using namespace Ikarus;
 
   using namespace Dune::Functions::BasisFactory;
   auto basis     = Ikarus::makeBasis(gridView, preBasis);
   auto flatBasis = basis.flat();
@@ -119,32 +102,39 @@
     return sparseAssembler.getMatrix(requirements);
   };
   auto nonLinOp = Ikarus::NonLinearOperator(linearAlgebraFunctions(fvLambda, dfvLambda, ddfvLambda), parameter(d));
 
   // execute all passed functions
   nonLinOp.updateAll();
   Dune::Hybrid::forEach(Dune::Hybrid::integralRange(Dune::index_constant<sizeof...(F)>()),
-                        [&](auto i) { t.subTest(std::get<i.value>(fTuple)(nonLinOp, fe)); });
+                        [&](auto i) { t.subTest(std::get<i.value>(fTuple)(nonLinOp, fe, requirements)); });
 
   // check if element has a test functor, if yes we execute it
   if constexpr (requires { ElementTest<FEElementType>::test(); }) {
     auto testFunctor = ElementTest<FEElementType>::test();
-    t.subTest(testFunctor(nonLinOp, fe));
+    t.subTest(testFunctor(nonLinOp, fe, requirements));
   } else
     spdlog::info("No element test functor found for {}", Dune::className<FEElementType>());
 
   // Trying to instantiate the Result Evaluator
   if constexpr (gridDim == 2) {
     auto resReq         = Ikarus::ResultRequirements(requirements).addResultRequest(ResultType::PK2Stress);
     auto resultFunction = std::make_shared<ResultFunction<FEElementType>>(&fes, resReq);
   }
 
   return t;
 }
 
-auto checkGradientFunctor = [](auto& nonLinOp, [[maybe_unused]] auto& fe) { return checkGradientOfElement(nonLinOp); };
-auto checkHessianFunctor  = [](auto& nonLinOp, [[maybe_unused]] auto& fe) { return checkHessianOfElement(nonLinOp); };
-auto checkJacobianFunctor = [](auto& nonLinOp, [[maybe_unused]] auto& fe) {
+auto checkGradientFunctor = [](auto& nonLinOp, [[maybe_unused]] auto& fe, [[maybe_unused]] auto& req) {
+  return checkGradientOfElement(nonLinOp);
+};
+auto checkHessianFunctor = [](auto& nonLinOp, [[maybe_unused]] auto& fe, [[maybe_unused]] auto& req) {
+  return checkHessianOfElement(nonLinOp);
+};
+auto checkJacobianFunctor = [](auto& nonLinOp, [[maybe_unused]] auto& fe, [[maybe_unused]] auto& req) {
   auto subOperator = nonLinOp.template subOperator<1, 2>();
   return checkJacobianOfElement(subOperator);
 };
-auto checkCauchyStressFunctor = [](auto& nonLinOp, auto& fe) { return checkCauchyStressOf2DElement(nonLinOp, fe); };
+auto checkCauchyStressFunctor
+    = [](auto& nonLinOp, auto& fe, [[maybe_unused]] auto& req) { return checkCauchyStressOf2DElement(nonLinOp, fe); };
+auto checkFEByAutoDiffFunctor
+    = [](auto& nonLinOp, auto& fe, auto& req) { return checkFEByAutoDiff(nonLinOp, fe, req); };
```

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/testFiles/unstructuredQuadscoarse.msh` & `pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredQuadscoarse.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/testFiles/unstructuredTest2.geo` & `pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTest2.geo`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/testFiles/unstructuredTrianglesfine.msh` & `pyikarus-0.3.3.dev20230601114417/tests/src/testFiles/unstructuredTrianglesfine.msh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/testHelpers.hh` & `pyikarus-0.3.3.dev20230601114417/tests/src/testHelpers.hh`

 * *Files identical despite different names*

### Comparing `pyikarus-0.3.3.dev20230523103500/tests/src/trustRegionTest.cpp` & `pyikarus-0.3.3.dev20230601114417/tests/src/testTrustRegion.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 #include <dune/common/tuplevector.hh>
 #include <dune/localfefunctions/manifolds/realTuple.hh>
 #include <dune/localfefunctions/manifolds/unitVector.hh>
 
 #include <ikarus/linearAlgebra/nonLinearOperator.hh>
 #include <ikarus/solver/nonLinearSolver/trustRegion.hh>
 #include <ikarus/utils/init.hh>
+
 using namespace Ikarus;
 using Dune::TestSuite;
 
 auto f(const Eigen::Vector<double, 1>& x) { return 0.5 * x[0] * x[0]; }
 auto df(const Eigen::Vector<double, 1>& x) {
   Eigen::Vector<double, 1> r;
   r[0] = x[0];
```

