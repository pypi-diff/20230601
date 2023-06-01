# Comparing `tmp/autora-core-3.0.0a7.tar.gz` & `tmp/autora-core-3.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-core-3.0.0a7.tar", last modified: Mon May  1 16:04:24 2023, max compression
+gzip compressed data, was "autora-core-3.0.0rc1.tar", last modified: Thu Jun  1 19:25:42 2023, max compression
```

## Comparing `autora-core-3.0.0a7.tar` & `autora-core-3.0.0rc1.tar`

### file list

```diff
@@ -1,101 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.665838 autora-core-3.0.0a7/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.github/workflows/test-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/autora-core.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/encodings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/other.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.idea/runConfigurations/
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/runConfigurations/pytest.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.vscode/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    19460 2023-05-01 16:04:24.665838 autora-core-3.0.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/conda/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/conda/autora/
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/conda/autora/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/conda/autora/run_test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/docs/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)   148488 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/cycle/simple_cycle_bms_model_poppernet.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/docs/experimentalists/
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/experimentalists/overview.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/docs/theorist/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.657837 autora-core-3.0.0a7/docs/theorist/bms/
--rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bms/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bms/search_space.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)  1572980 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bms/weber.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/docs/theorist/bsr/
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bsr/how_it_works.md
--rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bsr/img.png
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bsr/introduction.md
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bsr/meta_parameters.md
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/bsr/search_space.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/docs/theorist/darts/
--rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/darts/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)   796078 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/docs/theorist/darts/weber.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/mkdocs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/mkdocs/overrides/
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/mkdocs/overrides/main.html
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 16:04:24.665838 autora-core-3.0.0a7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.653837 autora-core-3.0.0a7/src/autora/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/cycle/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/cycle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20109 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/cycle/plot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/cycle/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/experimentalist/
--rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/experimentalist/pooler/
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/pooler/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/pooler/random_pooler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/experimentalist/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/assumption.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/dissimilarity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/model_disagreement.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/nearest_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/sampler/uncertainty.py
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/experimentalist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/synthetic/
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/synthetic/inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/theorist/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/theorist/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/utils/dictionary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.661838 autora-core-3.0.0a7/src/autora/variable/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/variable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/src/autora/variable/time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.665838 autora-core-3.0.0a7/src/autora_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19460 2023-05-01 16:04:24.000000 autora-core-3.0.0a7/src/autora_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-05-01 16:04:24.000000 autora-core-3.0.0a7/src/autora_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 16:04:24.000000 autora-core-3.0.0a7/src/autora_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-01 16:04:24.000000 autora-core-3.0.0a7/src/autora_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-01 16:04:24.000000 autora-core-3.0.0a7/src/autora_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 16:04:24.665838 autora-core-3.0.0a7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/tests/test_cycle_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/tests/test_experimentalist_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/tests/test_experimentalist_random.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-01 16:03:53.000000 autora-core-3.0.0a7/tests/test_synthetic_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.211506 autora-core-3.0.0rc1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.211506 autora-core-3.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.211506 autora-core-3.0.0rc1/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/autora-core.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.211506 autora-core-3.0.0rc1/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.211506 autora-core-3.0.0rc1/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/runConfigurations/pytest.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/CONTRIBUTE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/docs/javascripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/docs/javascripts/mathjax.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/docs/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)    10747 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/docs/pipeline/Experimentalist Pipeline Examples.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/mkdocs/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/mkdocs/base.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.207506 autora-core-3.0.0rc1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.207506 autora-core-3.0.0rc1/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/src/autora/experimentalist/
+-rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/experimentalist/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/src/autora/experimentalist/pooler/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/experimentalist/pooler/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/experimentalist/pooler/random_pooler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.215506 autora-core-3.0.0rc1/src/autora/experimentalist/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/experimentalist/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/experimentalist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/src/autora/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/utils/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/src/autora/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/variable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/src/autora/variable/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/src/autora_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-06-01 19:25:42.000000 autora-core-3.0.0rc1/src/autora_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-06-01 19:25:42.000000 autora-core-3.0.0rc1/src/autora_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 19:25:42.000000 autora-core-3.0.0rc1/src/autora_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-01 19:25:42.000000 autora-core-3.0.0rc1/src/autora_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-01 19:25:42.000000 autora-core-3.0.0rc1/src/autora_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 19:25:42.219506 autora-core-3.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/tests/test_experimentalist_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-01 19:25:26.000000 autora-core-3.0.0rc1/tests/test_experimentalist_random.py
```

### Comparing `autora-core-3.0.0a7/.github/pull_request_template.md` & `autora-core-3.0.0rc1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/.github/workflows/publish-package-pypi.yml` & `autora-core-3.0.0rc1/.github/workflows/publish-package-pypi.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/.github/workflows/test-pytest.yml` & `autora-core-3.0.0rc1/.github/workflows/test-pytest.yml`

 * *Files 17% similar despite different names*

```diff
@@ -21,9 +21,9 @@
     runs-on: ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v3
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: "pip"
-    - run: pip install ".[dev]"
+    - run: pip install ".[test]"
     - run: pytest --doctest-modules
```

### Comparing `autora-core-3.0.0a7/.gitignore` & `autora-core-3.0.0rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/.idea/autora-core.iml` & `autora-core-3.0.0rc1/.idea/autora-core.iml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/.idea/inspectionProfiles/Project_Default.xml` & `autora-core-3.0.0rc1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/.idea/runConfigurations/pytest.xml` & `autora-core-3.0.0rc1/.idea/runConfigurations/pytest.xml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/.pre-commit-config.yaml` & `autora-core-3.0.0rc1/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -23,10 +23,15 @@
     hooks:
       - id: mypy
         additional_dependencies: [types-requests,scipy,pytest]
         language_version: python3.8
         args:
           - "--namespace-packages"
           - "--explicit-package-bases"
-
+  - repo: https://github.com/srstevenson/nb-clean
+    rev: 2.4.0
+    hooks:
+      - id: nb-clean
+        args:
+          - --preserve-cell-outputs
 default_language_version:
   python: python3
```

### Comparing `autora-core-3.0.0a7/LICENSE.md` & `autora-core-3.0.0rc1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/pyproject.toml` & `autora-core-3.0.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,14 @@
 ]
 readme = "README.md"
 requires-python = ">=3.8,<4"
 dynamic = ["version"]
 
 dependencies = [
     "numpy",
-    "matplotlib",
-    "pandas",
-    "scikit-learn"
 ]
 
 
 [project.optional-dependencies]
 dev = [
     "autora-core[test]",
     "autora-core[build]",
@@ -57,15 +54,15 @@
 
 [[tool.mypy.overrides]]
 module = ["matplotlib.*", "sklearn.*", "pandas.*", "numpy.*"]
 ignore_missing_imports=true
 
 [project.urls]
 homepage = "http://www.empiricalresearch.ai"
-repository = "https://github.com/AutoResearch/autora-theorist-template"
+repository = "https://github.com/AutoResearch/autora-core"
 documentation = "https://autoresearch.github.io/autora/"
 
 
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
```

### Comparing `autora-core-3.0.0a7/src/autora/experimentalist/pipeline.py` & `autora-core-3.0.0rc1/src/autora/experimentalist/pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/src/autora/experimentalist/pooler/grid.py` & `autora-core-3.0.0rc1/src/autora/experimentalist/pooler/grid.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/src/autora/experimentalist/pooler/random_pooler.py` & `autora-core-3.0.0rc1/src/autora/experimentalist/pooler/random_pooler.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/src/autora/experimentalist/utils.py` & `autora-core-3.0.0rc1/src/autora/experimentalist/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,24 @@
         A simple range object can be converted into an array of dimension 2:
         >>> sequence_to_array(range(5)) # doctest: +NORMALIZE_WHITESPACE
         array([[0], [1], [2], [3], [4]])
 
         For mixed datatypes, the highest-level type common to all the inputs will be used, so
         consider using [_sequence_to_recarray][autora.experimentalist.utils._sequence_to_recarray]
         instead.
-        >>> sequence_to_array(zip(range(5), "abcde"))  # doctest: +NORMALIZE_WHITESPACE
-        array([['0', 'a'], ['1', 'b'], ['2', 'c'], ['3', 'd'], ['4', 'e']],  dtype='<U21')
+        >>> sequence_to_array(zip(range(5), "abcde"))  # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
+        array([['0', 'a'], ['1', 'b'], ['2', 'c'], ['3', 'd'], ['4', 'e']],  dtype='<U...')
 
         Single strings are broken into characters:
-        >>> sequence_to_array("abcde")  # doctest: +NORMALIZE_WHITESPACE
-        array([['a'], ['b'], ['c'], ['d'], ['e']], dtype='<U1')
+        >>> sequence_to_array("abcde")  # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
+        array([['a'], ['b'], ['c'], ['d'], ['e']], dtype='<U...')
 
         Multiple strings are treated as individual entries:
-        >>> sequence_to_array(["abc", "de"])  # doctest: +NORMALIZE_WHITESPACE
-        array([['abc'], ['de']], dtype='<U3')
+        >>> sequence_to_array(["abc", "de"])  # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
+        array([['abc'], ['de']], dtype='<U...')
 
     """
     deque = collections.deque(iterable)
     array = np.array(deque).reshape((len(deque), -1))
     return array
 
 
@@ -44,20 +44,20 @@
 
     See also: [array_to_sequence][autora.experimentalist.utils.array_to_sequence]
 
     Examples:
 
         A simple range object is converted into a recarray of dimension 2:
         >>> sequence_to_recarray(range(5)) # doctest: +NORMALIZE_WHITESPACE
-        rec.array([(0,), (1,), (2,), (3,), (4,)], dtype=[('f0', '<i8')])
+        rec.array([(0,), (1,), (2,), (3,), (4,)], dtype=[('f0', '<i...')])
 
         Mixed datatypes lead to multiple output types:
         >>> sequence_to_recarray(zip(range(5), "abcde"))  # doctest: +NORMALIZE_WHITESPACE
         rec.array([(0, 'a'), (1, 'b'), (2, 'c'), (3, 'd'), (4, 'e')],
-            dtype=[('f0', '<i8'), ('f1', '<U1')])
+            dtype=[('f0', '<i...'), ('f1', '<U1')])
 
         Single strings are broken into characters:
         >>> sequence_to_recarray("abcde")  # doctest: +NORMALIZE_WHITESPACE
         rec.array([('a',), ('b',), ('c',), ('d',), ('e',)], dtype=[('f0', '<U1')])
 
         Multiple strings are treated as individual entries:
         >>> sequence_to_recarray(["abc", "de"])  # doctest: +NORMALIZE_WHITESPACE
@@ -110,15 +110,15 @@
         >>> l0[2][1]
         5
 
         We can also use a record array:
         >>> a1 = np.rec.fromarrays([range(5), list("abcde")])
         >>> a1
         rec.array([(0, 'a'), (1, 'b'), (2, 'c'), (3, 'd'), (4, 'e')],
-                  dtype=[('f0', '<i8'), ('f1', '<U1')])
+                  dtype=[('f0', '<i...'), ('f1', '<U1')])
 
         This is converted into records:
         >>> l1 = list(array_to_sequence(a1))
         >>> l1
         [(0, 'a'), (1, 'b'), (2, 'c'), (3, 'd'), (4, 'e')]
 
         The elements of the list are numpy.records
```

### Comparing `autora-core-3.0.0a7/src/autora/variable/__init__.py` & `autora-core-3.0.0rc1/src/autora/variable/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/src/autora/variable/time.py` & `autora-core-3.0.0rc1/src/autora/variable/time.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/tests/README.md` & `autora-core-3.0.0rc1/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/tests/test_experimentalist_pipeline.py` & `autora-core-3.0.0rc1/tests/test_experimentalist_pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a7/tests/test_experimentalist_random.py` & `autora-core-3.0.0rc1/tests/test_experimentalist_random.py`

 * *Files identical despite different names*

