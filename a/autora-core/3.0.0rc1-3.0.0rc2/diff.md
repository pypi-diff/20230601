# Comparing `tmp/autora-core-3.0.0rc1.tar.gz` & `tmp/autora-core-3.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-core-3.0.0rc1.tar", last modified: Thu Jun  1 19:25:42 2023, max compression
+gzip compressed data, was "autora-core-3.0.0rc2.tar", last modified: Thu Jun  1 19:38:49 2023, max compression
```

## Comparing `autora-core-3.0.0rc1.tar` & `autora-core-3.0.0rc2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.211506 autora-core-3.0.0rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.211506 autora-core-3.0.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.211506 autora-core-3.0.0rc1/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/autora-core.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.211506 autora-core-3.0.0rc1/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.211506 autora-core-3.0.0rc1/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/runConfigurations/pytest.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/CONTRIBUTE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/docs/javascripts/
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/docs/javascripts/mathjax.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/docs/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/docs/pipeline/Experimentalist Pipeline Examples.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/mkdocs/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/mkdocs/base.yml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.207506 autora-core-3.0.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.207506 autora-core-3.0.0rc1/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/src/autora/experimentalist/
--rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/experimentalist/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/src/autora/experimentalist/pooler/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/experimentalist/pooler/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/experimentalist/pooler/random_pooler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/src/autora/experimentalist/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/experimentalist/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/experimentalist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/src/autora/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/utils/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/src/autora/variable/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/variable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/variable/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/src/autora_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-01 19:25:42.000000 autora-core-3.0.0rc1/src/autora_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 19:25:42.000000 autora-core-3.0.0rc1/src/autora_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:25:42.000000 autora-core-3.0.0rc1/src/autora_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-01 19:25:42.000000 autora-core-3.0.0rc1/src/autora_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 19:25:42.000000 autora-core-3.0.0rc1/src/autora_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/tests/test_experimentalist_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/tests/test_experimentalist_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.397503 autora-core-3.0.0rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.397503 autora-core-3.0.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/autora-core.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/runConfigurations/pytest.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/CONTRIBUTE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/docs/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/docs/pipeline/Experimentalist Pipeline Examples.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1476 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.397503 autora-core-3.0.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.397503 autora-core-3.0.0rc2/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora/experimentalist/
+-rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/experimentalist/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora/experimentalist/pooler/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/experimentalist/pooler/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/experimentalist/pooler/random_pooler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora/experimentalist/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/experimentalist/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/experimentalist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/utils/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/variable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/src/autora/variable/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/src/autora_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-01 19:38:49.000000 autora-core-3.0.0rc2/src/autora_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 19:38:49.000000 autora-core-3.0.0rc2/src/autora_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:38:49.000000 autora-core-3.0.0rc2/src/autora_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-01 19:38:49.000000 autora-core-3.0.0rc2/src/autora_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 19:38:49.000000 autora-core-3.0.0rc2/src/autora_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:38:49.401503 autora-core-3.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/tests/test_experimentalist_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-01 19:38:37.000000 autora-core-3.0.0rc2/tests/test_experimentalist_random.py
```

### Comparing `autora-core-3.0.0rc1/.github/pull_request_template.md` & `autora-core-3.0.0rc2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/.github/workflows/publish-package-pypi.yml` & `autora-core-3.0.0rc2/.github/workflows/publish-package-pypi.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/.github/workflows/test-pytest.yml` & `autora-core-3.0.0rc2/.github/workflows/test-pytest.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/.gitignore` & `autora-core-3.0.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/.idea/autora-core.iml` & `autora-core-3.0.0rc2/.idea/autora-core.iml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/.idea/inspectionProfiles/Project_Default.xml` & `autora-core-3.0.0rc2/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/.idea/runConfigurations/pytest.xml` & `autora-core-3.0.0rc2/.idea/runConfigurations/pytest.xml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/.pre-commit-config.yaml` & `autora-core-3.0.0rc2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/CONTRIBUTE.md` & `autora-core-3.0.0rc2/CONTRIBUTE.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/LICENSE.md` & `autora-core-3.0.0rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/PKG-INFO` & `autora-core-3.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-core
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `autora-core-3.0.0rc1/README.md` & `autora-core-3.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/docs/pipeline/Experimentalist Pipeline Examples.ipynb` & `autora-core-3.0.0rc2/docs/pipeline/Experimentalist Pipeline Examples.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/mkdocs/base.yml` & `autora-core-3.0.0rc2/mkdocs/base.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/pyproject.toml` & `autora-core-3.0.0rc2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,17 @@
 ]
 readme = "README.md"
 requires-python = ">=3.8,<4"
 dynamic = ["version"]
 
 dependencies = [
     "numpy",
+    "matplotlib",
+    "pandas",
+    "scikit-learn"
 ]
 
 
 [project.optional-dependencies]
 dev = [
     "autora-core[test]",
     "autora-core[build]",
```

### Comparing `autora-core-3.0.0rc1/src/autora/experimentalist/pipeline.py` & `autora-core-3.0.0rc2/src/autora/experimentalist/pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/src/autora/experimentalist/pooler/grid.py` & `autora-core-3.0.0rc2/src/autora/experimentalist/pooler/grid.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/src/autora/experimentalist/pooler/random_pooler.py` & `autora-core-3.0.0rc2/src/autora/experimentalist/pooler/random_pooler.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/src/autora/experimentalist/utils.py` & `autora-core-3.0.0rc2/src/autora/experimentalist/utils.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/src/autora/variable/__init__.py` & `autora-core-3.0.0rc2/src/autora/variable/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/src/autora/variable/time.py` & `autora-core-3.0.0rc2/src/autora/variable/time.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/src/autora_core.egg-info/PKG-INFO` & `autora-core-3.0.0rc2/src/autora_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.0.0rc1
+Version: 3.0.0rc2
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 Project-URL: homepage, http://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-core
 Project-URL: documentation, https://autoresearch.github.io/autora/
 Requires-Python: <4,>=3.8
 Description-Content-Type: text/markdown
```

### Comparing `autora-core-3.0.0rc1/src/autora_core.egg-info/SOURCES.txt` & `autora-core-3.0.0rc2/src/autora_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/tests/README.md` & `autora-core-3.0.0rc2/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/tests/test_experimentalist_pipeline.py` & `autora-core-3.0.0rc2/tests/test_experimentalist_pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0rc1/tests/test_experimentalist_random.py` & `autora-core-3.0.0rc2/tests/test_experimentalist_random.py`

 * *Files identical despite different names*

