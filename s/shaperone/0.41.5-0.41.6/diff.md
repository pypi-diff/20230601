# Comparing `tmp/shaperone-0.41.5.tar.gz` & `tmp/shaperone-0.41.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shaperone-0.41.5.tar", last modified: Wed May 24 16:00:48 2023, max compression
+gzip compressed data, was "shaperone-0.41.6.tar", last modified: Thu Jun  1 11:27:02 2023, max compression
```

## Comparing `shaperone-0.41.5.tar` & `shaperone-0.41.6.tar`

### file list

```diff
@@ -1,123 +1,123 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.730425 shaperone-0.41.5/
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-24 16:00:33.000000 shaperone-0.41.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-05-24 16:00:33.000000 shaperone-0.41.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-24 16:00:48.730425 shaperone-0.41.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      631 2023-05-24 16:00:33.000000 shaperone-0.41.5/README.md
--rw-r--r--   0 runner    (1001) docker     (122)      115 2023-05-24 16:00:34.000000 shaperone-0.41.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-24 16:00:48.730425 shaperone-0.41.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)    11869 2023-05-24 16:00:34.000000 shaperone-0.41.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.694424 shaperone-0.41.5/shaperone/
--rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32344 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/_explanation.py
--rw-r--r--   0 runner    (1001) docker     (122)     8707 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/_serializable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.698425 shaperone-0.41.5/shaperone/actions/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      210 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/actions/_action.py
--rw-r--r--   0 runner    (1001) docker     (122)     3636 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/actions/_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.702425 shaperone-0.41.5/shaperone/benchmark/
--rw-r--r--   0 runner    (1001) docker     (122)      214 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/_compute.py
--rw-r--r--   0 runner    (1001) docker     (122)     8099 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/_explanation_error.py
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/_result.py
--rw-r--r--   0 runner    (1001) docker     (122)    13399 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/_sequential.py
--rw-r--r--   0 runner    (1001) docker     (122)    14182 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/experiments.py
--rw-r--r--   0 runner    (1001) docker     (122)     4243 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/framework.py
--rw-r--r--   0 runner    (1001) docker     (122)    18601 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/measures.py
--rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/methods.py
--rw-r--r--   0 runner    (1001) docker     (122)    31376 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)     6513 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (122)    23812 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/benchmark/plots.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.706425 shaperone-0.41.5/shaperone/cext/
--rw-r--r--   0 runner    (1001) docker     (122)    25873 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/cext/_cext.cc
--rw-r--r--   0 runner    (1001) docker     (122)    58256 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/cext/tree_shap.h
--rw-r--r--   0 runner    (1001) docker     (122)     9316 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.710425 shaperone-0.41.5/shaperone/explainers/
--rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8939 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_additive.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.710425 shaperone-0.41.5/shaperone/explainers/_deep/
--rw-r--r--   0 runner    (1001) docker     (122)     6730 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_deep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16170 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_deep/deep_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (122)    35006 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_deep/deep_tf.py
--rw-r--r--   0 runner    (1001) docker     (122)    16264 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_exact.py
--rw-r--r--   0 runner    (1001) docker     (122)    23234 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_explainer.py
--rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_gpu_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    27238 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_gradient.py
--rw-r--r--   0 runner    (1001) docker     (122)    31017 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_kernel.py
--rw-r--r--   0 runner    (1001) docker     (122)    19121 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_linear.py
--rw-r--r--   0 runner    (1001) docker     (122)    31746 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_partition.py
--rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_permutation.py
--rw-r--r--   0 runner    (1001) docker     (122)     9255 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_sampling.py
--rw-r--r--   0 runner    (1001) docker     (122)    93670 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/mimic.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.714425 shaperone-0.41.5/shaperone/explainers/other/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      512 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/_coefficent.py
--rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/_lime.py
--rw-r--r--   0 runner    (1001) docker     (122)    11413 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/_maple.py
--rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/_random.py
--rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/other/_treegain.py
--rw-r--r--   0 runner    (1001) docker     (122)    20310 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/pytree.py
--rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/explainers/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      443 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/links.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.718425 shaperone-0.41.5/shaperone/maskers/
--rw-r--r--   0 runner    (1001) docker     (122)      283 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5213 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_composite.py
--rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_fixed.py
--rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_fixed_composite.py
--rw-r--r--   0 runner    (1001) docker     (122)     9543 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_image.py
--rw-r--r--   0 runner    (1001) docker     (122)      753 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_masker.py
--rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_output_composite.py
--rw-r--r--   0 runner    (1001) docker     (122)    14131 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_tabular.py
--rw-r--r--   0 runner    (1001) docker     (122)    21556 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/maskers/_text.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.718425 shaperone-0.41.5/shaperone/models/
--rw-r--r--   0 runner    (1001) docker     (122)      202 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/_model.py
--rw-r--r--   0 runner    (1001) docker     (122)    18717 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/_teacher_forcing.py
--rw-r--r--   0 runner    (1001) docker     (122)     9978 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/_text_generation.py
--rw-r--r--   0 runner    (1001) docker     (122)    10116 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/_topk_lm.py
--rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/models/_transformers_pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.726425 shaperone-0.41.5/shaperone/plots/
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    17309 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_bar.py
--rw-r--r--   0 runner    (1001) docker     (122)    41107 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_beeswarm.py
--rw-r--r--   0 runner    (1001) docker     (122)     9455 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (122)    26022 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_decision.py
--rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_embedding.py
--rw-r--r--   0 runner    (1001) docker     (122)    19463 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_force.py
--rw-r--r--   0 runner    (1001) docker     (122)    14797 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_force_matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_group_difference.py
--rw-r--r--   0 runner    (1001) docker     (122)     6502 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_heatmap.py
--rw-r--r--   0 runner    (1001) docker     (122)    25135 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_image.py
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_labels.py
--rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (122)     9521 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_partial_dependence.py
--rw-r--r--   0 runner    (1001) docker     (122)    33020 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_scatter.py
--rw-r--r--   0 runner    (1001) docker     (122)    59166 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_text.py
--rw-r--r--   0 runner    (1001) docker     (122)     7616 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    23943 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_violin.py
--rw-r--r--   0 runner    (1001) docker     (122)    26592 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/_waterfall.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.726425 shaperone-0.41.5/shaperone/plots/colors/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    36754 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/colors/_colorconv.py
--rw-r--r--   0 runner    (1001) docker     (122)     5096 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/colors/_colors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.726425 shaperone-0.41.5/shaperone/plots/resources/
--rw-r--r--   0 runner    (1001) docker     (122)   370829 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/resources/bundle.js
--rw-r--r--   0 runner    (1001) docker     (122)      570 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/plots/resources/logoSmallGray.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.730425 shaperone-0.41.5/shaperone/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      449 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8513 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_clustering.py
--rw-r--r--   0 runner    (1001) docker     (122)      591 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    10645 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_general.py
--rw-r--r--   0 runner    (1001) docker     (122)     2576 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_keras.py
--rw-r--r--   0 runner    (1001) docker     (122)     7329 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_legacy.py
--rw-r--r--   0 runner    (1001) docker     (122)    21361 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_masked_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/_show_progress.py
--rw-r--r--   0 runner    (1001) docker     (122)     5416 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (122)     6494 2023-05-24 16:00:34.000000 shaperone-0.41.5/shaperone/utils/transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-24 16:00:48.698425 shaperone-0.41.5/shaperone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1113 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      514 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-24 16:00:48.000000 shaperone-0.41.5/shaperone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.370183 shaperone-0.41.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-06-01 11:26:50.000000 shaperone-0.41.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-06-01 11:26:50.000000 shaperone-0.41.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-06-01 11:27:02.370183 shaperone-0.41.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1313 2023-06-01 11:26:50.000000 shaperone-0.41.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      115 2023-06-01 11:26:52.000000 shaperone-0.41.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-01 11:27:02.370183 shaperone-0.41.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)    11378 2023-06-01 11:26:52.000000 shaperone-0.41.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.358183 shaperone-0.41.6/shaperone/
+-rw-r--r--   0 runner    (1001) docker     (122)     3259 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32344 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/_explanation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8707 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/_serializable.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.358183 shaperone-0.41.6/shaperone/actions/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      210 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/actions/_action.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3636 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/actions/_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.362183 shaperone-0.41.6/shaperone/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (122)      214 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      289 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/_compute.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8099 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/_explanation_error.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1074 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13399 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/_sequential.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14182 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/experiments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4243 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/framework.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18601 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/measures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4287 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/methods.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31376 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6513 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23812 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/benchmark/plots.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.362183 shaperone-0.41.6/shaperone/cext/
+-rw-r--r--   0 runner    (1001) docker     (122)    25873 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/cext/_cext.cc
+-rw-r--r--   0 runner    (1001) docker     (122)    58256 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/cext/tree_shap.h
+-rw-r--r--   0 runner    (1001) docker     (122)     9316 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.362183 shaperone-0.41.6/shaperone/explainers/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8939 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_additive.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.362183 shaperone-0.41.6/shaperone/explainers/_deep/
+-rw-r--r--   0 runner    (1001) docker     (122)     6730 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_deep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16170 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_deep/deep_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35006 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_deep/deep_tf.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16294 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_exact.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23234 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_explainer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9330 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_gpu_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27238 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_gradient.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31017 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19121 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_linear.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31761 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_partition.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10941 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_permutation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9255 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93670 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5009 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/mimic.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.362183 shaperone-0.41.6/shaperone/explainers/other/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/other/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      512 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/other/_coefficent.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2528 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/other/_lime.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11413 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/other/_maple.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3344 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/other/_random.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1283 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/other/_treegain.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20310 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/pytree.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2774 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/explainers/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      503 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/links.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.366183 shaperone-0.41.6/shaperone/maskers/
+-rw-r--r--   0 runner    (1001) docker     (122)      283 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/maskers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5213 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/maskers/_composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1008 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/maskers/_fixed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2416 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/maskers/_fixed_composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9558 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/maskers/_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      753 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/maskers/_masker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/maskers/_output_composite.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14161 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/maskers/_tabular.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21556 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/maskers/_text.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.366183 shaperone-0.41.6/shaperone/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1498 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/models/_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18717 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/models/_teacher_forcing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9978 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/models/_text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10116 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/models/_topk_lm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1623 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/models/_transformers_pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.370183 shaperone-0.41.6/shaperone/plots/
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17309 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_bar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41107 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_beeswarm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9455 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26022 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_decision.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2813 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19463 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_force.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14797 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_force_matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3121 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_group_difference.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6502 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25135 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_image.py
+-rw-r--r--   0 runner    (1001) docker     (122)      608 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2825 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9521 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_partial_dependence.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33020 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    59166 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_text.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7616 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23943 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_violin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26592 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/_waterfall.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.370183 shaperone-0.41.6/shaperone/plots/colors/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36754 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/colors/_colorconv.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5096 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/colors/_colors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.370183 shaperone-0.41.6/shaperone/plots/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)   370829 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/resources/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (122)      570 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/plots/resources/logoSmallGray.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.370183 shaperone-0.41.6/shaperone/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      449 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8592 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/utils/_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (122)      591 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/utils/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10645 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/utils/_general.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2576 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/utils/_keras.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7329 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/utils/_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21421 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/utils/_masked_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1227 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/utils/_show_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5416 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6494 2023-06-01 11:26:52.000000 shaperone-0.41.6/shaperone/utils/transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-01 11:27:02.358183 shaperone-0.41.6/shaperone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      800 2023-06-01 11:27:02.000000 shaperone-0.41.6/shaperone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3268 2023-06-01 11:27:02.000000 shaperone-0.41.6/shaperone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 11:27:02.000000 shaperone-0.41.6/shaperone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-01 11:27:02.000000 shaperone-0.41.6/shaperone.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      514 2023-06-01 11:27:02.000000 shaperone-0.41.6/shaperone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-06-01 11:27:02.000000 shaperone-0.41.6/shaperone.egg-info/top_level.txt
```

### Comparing `shaperone-0.41.5/LICENSE` & `shaperone-0.41.6/LICENSE`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/setup.py` & `shaperone-0.41.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -200,22 +200,16 @@
     }
     extras_require['test'] = tests_require
     extras_require['all'] = list(set(i for val in extras_require.values() for i in val))
 
     setup(
         name='shaperone',
         version=find_version("shaperone", "__init__.py"),
-        description='A unified approach to explain the output of any machine learning model.',
-        long_description="SHAP (SHapley Additive exPlanations) is a unified approach to explain "
-                         "the output of " + \
-                         "any machine learning model. SHAP connects game theory with local "
-                         "explanations, uniting " + \
-                         "several previous methods and representing the only possible consistent "
-                         "and locally accurate " + \
-                         "additive feature attribution method based on expectations.",
+        description='Shaperone is a fork of the SHAP library, fixing open issues to improve usability.',
+        long_description="",
         long_description_content_type="text/markdown",
         url='http://github.com/slundberg/shap',
         author='Scott Lundberg',
         author_email='slund1@cs.washington.edu',
         license='MIT',
         packages=[
             'shaperone', 'shaperone.explainers', 'shaperone.explainers.other', 'shaperone.explainers._deep',
```

### Comparing `shaperone-0.41.5/shaperone/__init__.py` & `shaperone-0.41.6/shaperone/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # flake8: noqa
 
 import warnings
 import sys
 
-__version__ = '0.41.5'
+__version__ = '0.41.6'
 
 # check python version
 if (sys.version_info < (3, 0)):
     warnings.warn("As of version 0.29.0 shaperone only supports Python 3 (not 2)!")
 
 from ._explanation import Explanation, Cohorts
```

### Comparing `shaperone-0.41.5/shaperone/_explanation.py` & `shaperone-0.41.6/shaperone/_explanation.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/_serializable.py` & `shaperone-0.41.6/shaperone/_serializable.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/actions/_optimizer.py` & `shaperone-0.41.6/shaperone/actions/_optimizer.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/benchmark/_explanation_error.py` & `shaperone-0.41.6/shaperone/benchmark/_explanation_error.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/benchmark/_result.py` & `shaperone-0.41.6/shaperone/benchmark/_result.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/benchmark/_sequential.py` & `shaperone-0.41.6/shaperone/benchmark/_sequential.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/benchmark/experiments.py` & `shaperone-0.41.6/shaperone/benchmark/experiments.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/benchmark/framework.py` & `shaperone-0.41.6/shaperone/benchmark/framework.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/benchmark/measures.py` & `shaperone-0.41.6/shaperone/benchmark/measures.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/benchmark/methods.py` & `shaperone-0.41.6/shaperone/benchmark/methods.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/benchmark/metrics.py` & `shaperone-0.41.6/shaperone/benchmark/metrics.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/benchmark/models.py` & `shaperone-0.41.6/shaperone/benchmark/models.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/benchmark/plots.py` & `shaperone-0.41.6/shaperone/benchmark/plots.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/cext/_cext.cc` & `shaperone-0.41.6/shaperone/cext/_cext.cc`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/cext/tree_shap.h` & `shaperone-0.41.6/shaperone/cext/tree_shap.h`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/datasets.py` & `shaperone-0.41.6/shaperone/datasets.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_additive.py` & `shaperone-0.41.6/shaperone/explainers/_additive.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_deep/__init__.py` & `shaperone-0.41.6/shaperone/explainers/_deep/__init__.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_deep/deep_pytorch.py` & `shaperone-0.41.6/shaperone/explainers/_deep/deep_pytorch.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_deep/deep_tf.py` & `shaperone-0.41.6/shaperone/explainers/_deep/deep_tf.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_exact.py` & `shaperone-0.41.6/shaperone/explainers/_exact.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
             "values": row_values,
             "expected_values": outputs[0],
             "mask_shapes": fm.mask_shapes,
             "main_effects": main_effect_values if main_effects else None,
             "clustering": getattr(self.masker, "clustering", None)
         }
 
-@jit
+@jit(nopython=True)
 def _compute_grey_code_row_values(row_values, mask, inds, outputs, shapley_coeff, extended_delta_indexes, noop_code):
     set_size = 0
     M = len(inds)
     for i in range(2**M):
 
         # update the mask
         delta_ind = extended_delta_indexes[i]
@@ -197,15 +197,15 @@
         out = outputs[i]
         for j in inds:
             if mask[j]:
                 row_values[j] += out * on_coeff
             else:
                 row_values[j] -= out * off_coeff
 
-@jit
+@jit(nopython=True)
 def _compute_grey_code_row_values_st(row_values, mask, inds, outputs, shapley_coeff, extended_delta_indexes, noop_code):
     set_size = 0
     M = len(inds)
     for i in range(2**M):
 
         # update the mask
         delta_ind = extended_delta_indexes[i]
```

### Comparing `shaperone-0.41.5/shaperone/explainers/_explainer.py` & `shaperone-0.41.6/shaperone/explainers/_explainer.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_gpu_tree.py` & `shaperone-0.41.6/shaperone/explainers/_gpu_tree.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_gradient.py` & `shaperone-0.41.6/shaperone/explainers/_gradient.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_kernel.py` & `shaperone-0.41.6/shaperone/explainers/_kernel.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_linear.py` & `shaperone-0.41.6/shaperone/explainers/_linear.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_partition.py` & `shaperone-0.41.6/shaperone/explainers/_partition.py`

 * *Files 0% similar despite different names*

```diff
@@ -668,15 +668,15 @@
     elif output_indexes.startswith("min("):
         return int(output_indexes[4:-1])
     elif output_indexes.startswith("max(abs("):
         return int(output_indexes[8:-2])
     elif not isinstance(output_indexes, str):
         return len(output_indexes)
 
-@jit
+@jit(nopython=True)
 def lower_credit(i, value, M, values, clustering):
     if i < M:
         values[i] += value
         return
     li = int(clustering[i-M,0])
     ri = int(clustering[i-M,1])
     group_size = int(clustering[i-M,3])
```

### Comparing `shaperone-0.41.5/shaperone/explainers/_permutation.py` & `shaperone-0.41.6/shaperone/explainers/_permutation.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_sampling.py` & `shaperone-0.41.6/shaperone/explainers/_sampling.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/_tree.py` & `shaperone-0.41.6/shaperone/explainers/_tree.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/mimic.py` & `shaperone-0.41.6/shaperone/explainers/mimic.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/other/_coefficent.py` & `shaperone-0.41.6/shaperone/explainers/other/_coefficent.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/other/_lime.py` & `shaperone-0.41.6/shaperone/explainers/other/_lime.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/other/_maple.py` & `shaperone-0.41.6/shaperone/explainers/other/_maple.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/other/_random.py` & `shaperone-0.41.6/shaperone/explainers/other/_random.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/other/_treegain.py` & `shaperone-0.41.6/shaperone/explainers/other/_treegain.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/pytree.py` & `shaperone-0.41.6/shaperone/explainers/pytree.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/explainers/tf_utils.py` & `shaperone-0.41.6/shaperone/explainers/tf_utils.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/maskers/_composite.py` & `shaperone-0.41.6/shaperone/maskers/_composite.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/maskers/_fixed.py` & `shaperone-0.41.6/shaperone/maskers/_fixed.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/maskers/_fixed_composite.py` & `shaperone-0.41.6/shaperone/maskers/_fixed_composite.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/maskers/_image.py` & `shaperone-0.41.6/shaperone/maskers/_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -167,15 +167,15 @@
 
         kwargs = super().load(in_file, instantiate=False)
         with Deserializer(in_file, "shaperone.maskers.Image", min_version=0, max_version=0) as s:
             kwargs["mask_value"] = s.load("mask_value")
             kwargs["shape"] = s.load("shape")
         return kwargs
 
-@jit
+@jit(nopython=True)
 def _jit_build_partition_tree(xmin, xmax, ymin, ymax, zmin, zmax, total_ywidth, total_zwidth, M, clustering, q):
     """ This partitions an image into a herarchical clustering based on axis-aligned splits.
     """
 
     # heapq.heappush(q, (0, xmin, xmax, ymin, ymax, zmin, zmax, -1, False))
 
     # q.put((0, xmin, xmax, ymin, ymax, zmin, zmax, -1, False))
```

### Comparing `shaperone-0.41.5/shaperone/maskers/_masker.py` & `shaperone-0.41.6/shaperone/maskers/_masker.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/maskers/_output_composite.py` & `shaperone-0.41.6/shaperone/maskers/_output_composite.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/maskers/_tabular.py` & `shaperone-0.41.6/shaperone/maskers/_tabular.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,26 +178,26 @@
         kwargs = super().load(in_file, instantiate=False)
         with Deserializer(in_file, "shaperone.maskers.Tabular", min_version=0, max_version=0) as s:
             kwargs["data"] = s.load("data")
             kwargs["max_samples"] = s.load("max_samples")
             kwargs["clustering"] = s.load("clustering")
         return kwargs
 
-@jit
+@jit(nopython=True)
 def _single_delta_mask(dind, masked_inputs, last_mask, data, x, noop_code):
     if dind == noop_code:
         pass
     elif last_mask[dind]:
         masked_inputs[:, dind] = data[:, dind]
         last_mask[dind] = False
     else:
         masked_inputs[:, dind] = x[dind]
         last_mask[dind] = True
 
-@jit
+@jit(nopython=True)
 def _delta_masking(masks, x, curr_delta_inds, varying_rows_out,
                    masked_inputs_tmp, last_mask, data, variants, masked_inputs_out, noop_code):
     """ Implements the special (high speed) delta masking API that only flips the positions we need to.
 
     Note that we attempt to avoid doing any allocation inside this function for speed reasons.
     """
```

### Comparing `shaperone-0.41.5/shaperone/maskers/_text.py` & `shaperone-0.41.6/shaperone/maskers/_text.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/models/_model.py` & `shaperone-0.41.6/shaperone/models/_model.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/models/_teacher_forcing.py` & `shaperone-0.41.6/shaperone/models/_teacher_forcing.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/models/_text_generation.py` & `shaperone-0.41.6/shaperone/models/_text_generation.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/models/_topk_lm.py` & `shaperone-0.41.6/shaperone/models/_topk_lm.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/models/_transformers_pipeline.py` & `shaperone-0.41.6/shaperone/models/_transformers_pipeline.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/__init__.py` & `shaperone-0.41.6/shaperone/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_bar.py` & `shaperone-0.41.6/shaperone/plots/_bar.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_beeswarm.py` & `shaperone-0.41.6/shaperone/plots/_beeswarm.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_benchmark.py` & `shaperone-0.41.6/shaperone/plots/_benchmark.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_decision.py` & `shaperone-0.41.6/shaperone/plots/_decision.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_embedding.py` & `shaperone-0.41.6/shaperone/plots/_embedding.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_force.py` & `shaperone-0.41.6/shaperone/plots/_force.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_force_matplotlib.py` & `shaperone-0.41.6/shaperone/plots/_force_matplotlib.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_group_difference.py` & `shaperone-0.41.6/shaperone/plots/_group_difference.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_heatmap.py` & `shaperone-0.41.6/shaperone/plots/_heatmap.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_image.py` & `shaperone-0.41.6/shaperone/plots/_image.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_labels.py` & `shaperone-0.41.6/shaperone/plots/_labels.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_monitoring.py` & `shaperone-0.41.6/shaperone/plots/_monitoring.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_partial_dependence.py` & `shaperone-0.41.6/shaperone/plots/_partial_dependence.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_scatter.py` & `shaperone-0.41.6/shaperone/plots/_scatter.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_text.py` & `shaperone-0.41.6/shaperone/plots/_text.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_utils.py` & `shaperone-0.41.6/shaperone/plots/_utils.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_violin.py` & `shaperone-0.41.6/shaperone/plots/_violin.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/_waterfall.py` & `shaperone-0.41.6/shaperone/plots/_waterfall.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/colors/_colorconv.py` & `shaperone-0.41.6/shaperone/plots/colors/_colorconv.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/colors/_colors.py` & `shaperone-0.41.6/shaperone/plots/colors/_colors.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/resources/bundle.js` & `shaperone-0.41.6/shaperone/plots/resources/bundle.js`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/plots/resources/logoSmallGray.png` & `shaperone-0.41.6/shaperone/plots/resources/logoSmallGray.png`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/utils/_clustering.py` & `shaperone-0.41.6/shaperone/utils/_clustering.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 
     partition_tree: np.array
         The partition tree we should follow.
     """
     M = len(index_mask)
     #switch = np.random.randn(M) < 0
     _pt_shuffle_rec(partition_tree.shape[0]-1, indexes, index_mask, partition_tree, M, 0)
-@jit
+
+@jit(nopython=True)
 def _pt_shuffle_rec(i, indexes, index_mask, partition_tree, M, pos):
     if i < 0:
         # see if we should include this index in the ordering
         if index_mask[i + M]: 
             indexes[pos] = i + M
             return pos + 1
         else:
@@ -46,38 +47,41 @@
         pos = _pt_shuffle_rec(left, indexes, index_mask, partition_tree, M, pos)
         pos = _pt_shuffle_rec(right, indexes, index_mask, partition_tree, M, pos)
     else:
         pos = _pt_shuffle_rec(right, indexes, index_mask, partition_tree, M, pos)
         pos = _pt_shuffle_rec(left, indexes, index_mask, partition_tree, M, pos)
     return pos
 
-@jit
+@jit(nopython=True)
 def delta_minimization_order(all_masks, max_swap_size=100, num_passes=2):
     order = np.arange(len(all_masks))
     for _ in range(num_passes):
         for length in list(range(2, max_swap_size)): 
             for i in range(1, len(order)-length):
                 if _reverse_window_score_gain(all_masks, order, i, length) > 0:
                     _reverse_window(order, i, length)
     return order
-@jit
+
+@jit(nopython=True)
 def _reverse_window(order, start, length):
     for i in range(length // 2):
         tmp = order[start + i]
         order[start + i] = order[start + length - i - 1]
         order[start + length - i - 1] = tmp
-@jit
+
+@jit(nopython=True)
 def _reverse_window_score_gain(masks, order, start, length):
     forward_score = _mask_delta_score(masks[order[start - 1]], masks[order[start]]) + \
                     _mask_delta_score(masks[order[start + length-1]], masks[order[start + length]])
     reverse_score = _mask_delta_score(masks[order[start - 1]], masks[order[start + length-1]]) + \
                     _mask_delta_score(masks[order[start]], masks[order[start + length]])
     
     return forward_score - reverse_score
-@jit
+
+@jit(nopython=True)
 def _mask_delta_score(m1, m2):
     return (m1 ^ m2).sum()
 
 
 def hclust_ordering(X, metric="sqeuclidean", anchor_first=False):
     """ A leaf ordering is under-defined, this picks the ordering that keeps nearby samples similar.
     """
```

### Comparing `shaperone-0.41.5/shaperone/utils/_exceptions.py` & `shaperone-0.41.6/shaperone/utils/_exceptions.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/utils/_general.py` & `shaperone-0.41.6/shaperone/utils/_general.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/utils/_keras.py` & `shaperone-0.41.6/shaperone/utils/_keras.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/utils/_legacy.py` & `shaperone-0.41.6/shaperone/utils/_legacy.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/utils/_masked_model.py` & `shaperone-0.41.6/shaperone/utils/_masked_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 
 def _build_fixed_output(averaged_outs, last_outs, outputs, batch_positions, varying_rows, num_varying_rows, link, linearizing_weights):
     if len(last_outs.shape) == 1:
         _build_fixed_single_output(averaged_outs, last_outs, outputs, batch_positions, varying_rows, num_varying_rows, link, linearizing_weights)
     else:
         _build_fixed_multi_output(averaged_outs, last_outs, outputs, batch_positions, varying_rows, num_varying_rows, link, linearizing_weights)
 
-@jit # we can't use this when using a custom link function...
+@jit(nopython=True) # we can't use this when using a custom link function...
 def _build_fixed_single_output(averaged_outs, last_outs, outputs, batch_positions, varying_rows, num_varying_rows, link, linearizing_weights):
     # here we can assume that the outputs will always be the same size, and we need
     # to carry over evaluation outputs
     sample_count = last_outs.shape[0]
     # if linearizing_weights is not None:
     #     averaged_outs[0] = np.mean(linearizing_weights * link(last_outs))
     # else:
@@ -377,15 +377,15 @@
             if linearizing_weights is not None:
                 averaged_outs[i] = np.mean(linearizing_weights * link(last_outs))
             else:
                 averaged_outs[i] = link(np.mean(last_outs))
         else:
             averaged_outs[i] = averaged_outs[i-1]
 
-@jit
+@jit(nopython=True)
 def _build_fixed_multi_output(averaged_outs, last_outs, outputs, batch_positions, varying_rows, num_varying_rows, link, linearizing_weights):
     # here we can assume that the outputs will always be the same size, and we need
     # to carry over evaluation outputs
     sample_count = last_outs.shape[0]
     for i in range(0, len(averaged_outs)):
         if batch_positions[i] < batch_positions[i+1]:
             if num_varying_rows[i] == sample_count:
@@ -420,26 +420,26 @@
     mask_matrix = scipy.sparse.csr_matrix(
         (np.ones(len(indices), dtype=bool), indices, indptr),
         shape=(2 * M - 1, M)
     )
 
     return mask_matrix
 
-@jit
+@jit(nopython=True)
 def _init_masks(cluster_matrix, M, indices_row_pos, indptr):
     pos = 0
     for i in range(2 * M - 1):
         if i < M:
             pos += 1
         else:
             pos += int(cluster_matrix[i-M, 3])
         indptr[i+1] = pos
         indices_row_pos[i] = indptr[i]
 
-@jit
+@jit(nopython=True)
 def _rec_fill_masks(cluster_matrix, indices_row_pos, indptr, indices, M, ind):
     pos = indices_row_pos[ind]
 
     if ind < M:
         indices[pos] = ind
         return
```

### Comparing `shaperone-0.41.5/shaperone/utils/_show_progress.py` & `shaperone-0.41.6/shaperone/utils/_show_progress.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/utils/image.py` & `shaperone-0.41.6/shaperone/utils/image.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone/utils/transformers.py` & `shaperone-0.41.6/shaperone/utils/transformers.py`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone.egg-info/SOURCES.txt` & `shaperone-0.41.6/shaperone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shaperone-0.41.5/shaperone.egg-info/requires.txt` & `shaperone-0.41.6/shaperone.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -5,33 +5,33 @@
 tqdm>4.25.0
 packaging>20.9
 slicer==0.0.7
 numba
 cloudpickle
 
 [all]
-pytest-cov
-torch
-opencv-python
+transformers
 lime
+pytest-mpl
+sphinx
+sphinx_rtd_theme
 pytest
-lightgbm
 pyod
-sphinx
-matplotlib
+torch
+sentencepiece
 pyspark
+opencv-python
+matplotlib
 nbsphinx
-sentencepiece
-sphinx_rtd_theme
-transformers
-pytest-mpl
-ipython
 catboost
+lightgbm
+ipython
 xgboost
 numpydoc
+pytest-cov
 
 [docs]
 matplotlib
 ipython
 numpydoc
 sphinx_rtd_theme
 sphinx
```

