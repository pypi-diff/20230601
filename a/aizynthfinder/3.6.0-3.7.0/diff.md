# Comparing `tmp/aizynthfinder-3.6.0.tar.gz` & `tmp/aizynthfinder-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aizynthfinder-3.6.0.tar", max compression
+gzip compressed data, was "aizynthfinder-3.7.0.tar", max compression
```

## Comparing `aizynthfinder-3.6.0.tar` & `aizynthfinder-3.7.0.tar`

### file list

```diff
@@ -1,81 +1,80 @@
--rw-r--r--   0        0        0     1072 2022-11-28 08:29:07.879491 aizynthfinder-3.6.0/LICENSE
--rw-r--r--   0        0        0     6086 2022-11-28 14:09:20.574139 aizynthfinder-3.6.0/README.md
--rw-r--r--   0        0        0        0 2021-10-14 10:02:24.521574 aizynthfinder-3.6.0/aizynthfinder/__init__.py
--rw-r--r--   0        0        0    12162 2022-11-28 10:57:14.813425 aizynthfinder-3.6.0/aizynthfinder/aizynthfinder.py
--rw-r--r--   0        0        0      234 2021-10-14 10:02:24.522574 aizynthfinder-3.6.0/aizynthfinder/analysis/__init__.py
--rw-r--r--   0        0        0    14227 2022-11-28 10:57:14.814425 aizynthfinder-3.6.0/aizynthfinder/analysis/routes.py
--rw-r--r--   0        0        0     9428 2022-01-13 12:47:30.898828 aizynthfinder-3.6.0/aizynthfinder/analysis/tree_analysis.py
--rw-r--r--   0        0        0     4974 2022-07-06 09:18:55.584199 aizynthfinder-3.6.0/aizynthfinder/analysis/utils.py
--rw-r--r--   0        0        0      507 2022-07-06 09:25:30.213649 aizynthfinder-3.6.0/aizynthfinder/chem/__init__.py
--rw-r--r--   0        0        0    12519 2022-08-22 06:03:17.550805 aizynthfinder-3.6.0/aizynthfinder/chem/mol.py
--rw-r--r--   0        0        0    24480 2022-11-28 08:30:18.743844 aizynthfinder-3.6.0/aizynthfinder/chem/reaction.py
--rw-r--r--   0        0        0     5127 2022-08-22 06:03:17.552805 aizynthfinder-3.6.0/aizynthfinder/chem/serialization.py
--rw-r--r--   0        0        0        0 2021-10-14 10:02:24.525574 aizynthfinder-3.6.0/aizynthfinder/context/__init__.py
--rw-r--r--   0        0        0     4602 2021-10-14 10:02:24.526574 aizynthfinder-3.6.0/aizynthfinder/context/collection.py
--rw-r--r--   0        0        0     6141 2022-01-11 13:55:20.412035 aizynthfinder-3.6.0/aizynthfinder/context/config.py
--rw-r--r--   0        0        0      206 2021-10-14 10:02:24.526574 aizynthfinder-3.6.0/aizynthfinder/context/cost/__init__.py
--rw-r--r--   0        0        0     2626 2022-07-06 09:18:55.584199 aizynthfinder-3.6.0/aizynthfinder/context/cost/collection.py
--rw-r--r--   0        0        0     1318 2021-10-14 10:02:24.526574 aizynthfinder-3.6.0/aizynthfinder/context/cost/costs.py
--rw-r--r--   0        0        0      442 2022-10-04 07:54:11.339382 aizynthfinder-3.6.0/aizynthfinder/context/policy/__init__.py
--rw-r--r--   0        0        0     6498 2022-10-04 07:54:11.340382 aizynthfinder-3.6.0/aizynthfinder/context/policy/expansion_strategies.py
--rw-r--r--   0        0        0     5332 2022-07-19 11:12:37.035217 aizynthfinder-3.6.0/aizynthfinder/context/policy/filter_strategies.py
--rw-r--r--   0        0        0     7131 2022-02-07 10:02:49.210288 aizynthfinder-3.6.0/aizynthfinder/context/policy/policies.py
--rw-r--r--   0        0        0      535 2022-07-19 11:12:37.036217 aizynthfinder-3.6.0/aizynthfinder/context/policy/utils.py
--rw-r--r--   0        0        0      434 2021-10-14 10:02:24.527574 aizynthfinder-3.6.0/aizynthfinder/context/scoring/__init__.py
--rw-r--r--   0        0        0     3623 2021-10-14 10:02:24.527574 aizynthfinder-3.6.0/aizynthfinder/context/scoring/collection.py
--rw-r--r--   0        0        0    10858 2022-07-06 09:18:55.585199 aizynthfinder-3.6.0/aizynthfinder/context/scoring/scorers.py
--rw-r--r--   0        0        0      255 2021-10-14 10:02:24.527574 aizynthfinder-3.6.0/aizynthfinder/context/stock/__init__.py
--rw-r--r--   0        0        0     5498 2022-11-28 10:57:14.817425 aizynthfinder-3.6.0/aizynthfinder/context/stock/queries.py
--rw-r--r--   0        0        0    10537 2022-11-28 10:57:14.817425 aizynthfinder-3.6.0/aizynthfinder/context/stock/stock.py
--rw-r--r--   0        0        0     1446 2022-02-07 10:02:49.210288 aizynthfinder-3.6.0/aizynthfinder/data/default_training.yml
--rw-r--r--   0        0        0      487 2021-10-14 10:02:24.528574 aizynthfinder-3.6.0/aizynthfinder/data/logging.yml
--rw-r--r--   0        0        0      782 2022-02-07 10:02:49.211288 aizynthfinder-3.6.0/aizynthfinder/data/templates/reaction_tree.dot
--rw-r--r--   0        0        0     1265 2021-10-14 10:02:24.528574 aizynthfinder-3.6.0/aizynthfinder/data/templates/reaction_tree.thtml
--rw-r--r--   0        0        0      176 2021-10-14 10:02:24.528574 aizynthfinder-3.6.0/aizynthfinder/interfaces/__init__.py
--rw-r--r--   0        0        0    15064 2021-11-10 13:23:07.668021 aizynthfinder-3.6.0/aizynthfinder/interfaces/aizynthapp.py
--rw-r--r--   0        0        0     9759 2022-11-28 10:57:14.818425 aizynthfinder-3.6.0/aizynthfinder/interfaces/aizynthcli.py
--rw-r--r--   0        0        0       81 2021-10-14 10:02:24.529574 aizynthfinder-3.6.0/aizynthfinder/interfaces/gui/__init__.py
--rw-r--r--   0        0        0     4247 2022-11-28 10:57:14.818425 aizynthfinder-3.6.0/aizynthfinder/interfaces/gui/clustering.py
--rw-r--r--   0        0        0    14297 2022-11-28 10:57:14.819425 aizynthfinder-3.6.0/aizynthfinder/reactiontree.py
--rw-r--r--   0        0        0        0 2021-10-14 10:02:24.530574 aizynthfinder-3.6.0/aizynthfinder/search/__init__.py
--rw-r--r--   0        0        0     8186 2022-07-06 09:18:55.586199 aizynthfinder-3.6.0/aizynthfinder/search/andor_trees.py
--rw-r--r--   0        0        0      124 2022-07-06 09:18:55.586199 aizynthfinder-3.6.0/aizynthfinder/search/breadth_first/__init__.py
--rw-r--r--   0        0        0     7739 2022-07-06 09:18:55.586199 aizynthfinder-3.6.0/aizynthfinder/search/breadth_first/nodes.py
--rw-r--r--   0        0        0     5578 2022-07-06 09:18:55.587199 aizynthfinder-3.6.0/aizynthfinder/search/breadth_first/search_tree.py
--rw-r--r--   0        0        0      106 2022-07-06 09:18:55.587199 aizynthfinder-3.6.0/aizynthfinder/search/dfpn/__init__.py
--rw-r--r--   0        0        0    11071 2022-07-06 09:18:55.587199 aizynthfinder-3.6.0/aizynthfinder/search/dfpn/nodes.py
--rw-r--r--   0        0        0     4734 2022-07-06 09:18:55.588199 aizynthfinder-3.6.0/aizynthfinder/search/dfpn/search_tree.py
--rw-r--r--   0        0        0      211 2021-10-14 10:02:24.530574 aizynthfinder-3.6.0/aizynthfinder/search/mcts/__init__.py
--rw-r--r--   0        0        0    15856 2022-11-28 10:57:14.819425 aizynthfinder-3.6.0/aizynthfinder/search/mcts/node.py
--rw-r--r--   0        0        0     5593 2022-11-28 10:57:14.820425 aizynthfinder-3.6.0/aizynthfinder/search/mcts/search.py
--rw-r--r--   0        0        0     6490 2022-01-13 12:47:30.903828 aizynthfinder-3.6.0/aizynthfinder/search/mcts/state.py
--rw-r--r--   0        0        0     2582 2022-11-28 10:57:14.820425 aizynthfinder-3.6.0/aizynthfinder/search/mcts/utils.py
--rw-r--r--   0        0        0        0 2022-07-06 09:18:55.589199 aizynthfinder-3.6.0/aizynthfinder/search/retrostar/__init__.py
--rw-r--r--   0        0        0     2531 2022-07-06 09:18:55.615199 aizynthfinder-3.6.0/aizynthfinder/search/retrostar/cost.py
--rw-r--r--   0        0        0    11702 2022-07-06 09:18:55.615199 aizynthfinder-3.6.0/aizynthfinder/search/retrostar/nodes.py
--rw-r--r--   0        0        0     6521 2022-07-06 09:18:55.615199 aizynthfinder-3.6.0/aizynthfinder/search/retrostar/search_tree.py
--rw-r--r--   0        0        0        0 2021-10-14 10:02:24.531574 aizynthfinder-3.6.0/aizynthfinder/tools/__init__.py
--rw-r--r--   0        0        0      815 2022-08-22 06:03:17.556805 aizynthfinder-3.6.0/aizynthfinder/tools/cat_output.py
--rw-r--r--   0        0        0     3131 2022-11-28 14:22:42.883499 aizynthfinder-3.6.0/aizynthfinder/tools/download_public_data.py
--rw-r--r--   0        0        0     4677 2021-10-14 10:02:24.531574 aizynthfinder-3.6.0/aizynthfinder/tools/make_stock.py
--rw-r--r--   0        0        0        0 2021-10-14 10:02:24.531574 aizynthfinder-3.6.0/aizynthfinder/training/__init__.py
--rw-r--r--   0        0        0     8290 2022-11-28 10:57:14.821425 aizynthfinder-3.6.0/aizynthfinder/training/keras_models.py
--rw-r--r--   0        0        0     9204 2022-07-06 09:18:55.590199 aizynthfinder-3.6.0/aizynthfinder/training/make_false_products.py
--rw-r--r--   0        0        0     5300 2022-11-28 10:57:14.821425 aizynthfinder-3.6.0/aizynthfinder/training/preprocess_expansion.py
--rw-r--r--   0        0        0     2832 2022-11-28 10:57:14.821425 aizynthfinder-3.6.0/aizynthfinder/training/preprocess_filter.py
--rw-r--r--   0        0        0     2756 2022-11-28 10:57:14.821425 aizynthfinder-3.6.0/aizynthfinder/training/preprocess_recommender.py
--rw-r--r--   0        0        0     1085 2022-02-07 10:02:49.217288 aizynthfinder-3.6.0/aizynthfinder/training/training.py
--rw-r--r--   0        0        0     8760 2022-11-28 10:57:14.822425 aizynthfinder-3.6.0/aizynthfinder/training/utils.py
--rw-r--r--   0        0        0        0 2021-10-14 10:02:24.532574 aizynthfinder-3.6.0/aizynthfinder/utils/__init__.py
--rw-r--r--   0        0        0      914 2022-07-06 09:18:55.591199 aizynthfinder-3.6.0/aizynthfinder/utils/exceptions.py
--rw-r--r--   0        0        0     5095 2022-08-22 06:03:17.558805 aizynthfinder-3.6.0/aizynthfinder/utils/files.py
--rw-r--r--   0        0        0    16552 2022-11-28 10:57:14.822425 aizynthfinder-3.6.0/aizynthfinder/utils/image.py
--rw-r--r--   0        0        0     1502 2021-11-24 14:41:26.799625 aizynthfinder-3.6.0/aizynthfinder/utils/loading.py
--rw-r--r--   0        0        0     1799 2022-11-28 10:57:14.822425 aizynthfinder-3.6.0/aizynthfinder/utils/logging.py
--rw-r--r--   0        0        0    10038 2022-11-28 10:57:14.823425 aizynthfinder-3.6.0/aizynthfinder/utils/models.py
--rw-r--r--   0        0        0     1539 2022-11-28 10:57:14.825425 aizynthfinder-3.6.0/aizynthfinder/utils/mongo.py
--rw-r--r--   0        0        0      355 2021-10-14 10:02:24.533574 aizynthfinder-3.6.0/aizynthfinder/utils/paths.py
--rw-r--r--   0        0        0      631 2021-10-15 06:03:09.123498 aizynthfinder-3.6.0/aizynthfinder/utils/type_utils.py
--rw-r--r--   0        0        0     2321 2022-11-28 14:07:19.041627 aizynthfinder-3.6.0/pyproject.toml
--rw-r--r--   0        0        0     8707 2022-11-28 14:57:08.699113 aizynthfinder-3.6.0/setup.py
--rw-r--r--   0        0        0     7850 2022-11-28 14:57:08.699621 aizynthfinder-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/LICENSE
+-rw-r--r--   0        0        0     6086 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/__init__.py
+-rw-r--r--   0        0        0    12121 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/aizynthfinder.py
+-rw-r--r--   0        0        0      249 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/analysis/__init__.py
+-rw-r--r--   0        0        0    14215 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/analysis/routes.py
+-rw-r--r--   0        0        0     9407 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/analysis/tree_analysis.py
+-rw-r--r--   0        0        0     4917 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/analysis/utils.py
+-rw-r--r--   0        0        0      507 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/chem/__init__.py
+-rw-r--r--   0        0        0    12519 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/chem/mol.py
+-rw-r--r--   0        0        0    24481 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/chem/reaction.py
+-rw-r--r--   0        0        0     5128 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/chem/serialization.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/context/__init__.py
+-rw-r--r--   0        0        0     4565 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/context/collection.py
+-rw-r--r--   0        0        0     6705 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/context/config.py
+-rw-r--r--   0        0        0      206 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/context/cost/__init__.py
+-rw-r--r--   0        0        0     2618 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/context/cost/collection.py
+-rw-r--r--   0        0        0     1318 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/context/cost/costs.py
+-rw-r--r--   0        0        0      442 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/context/policy/__init__.py
+-rw-r--r--   0        0        0     6499 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/context/policy/expansion_strategies.py
+-rw-r--r--   0        0        0     5332 2023-06-01 12:50:10.920720 aizynthfinder-3.7.0/aizynthfinder/context/policy/filter_strategies.py
+-rw-r--r--   0        0        0     7132 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/context/policy/policies.py
+-rw-r--r--   0        0        0      535 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/context/policy/utils.py
+-rw-r--r--   0        0        0      434 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/context/scoring/__init__.py
+-rw-r--r--   0        0        0     3575 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/context/scoring/collection.py
+-rw-r--r--   0        0        0    10773 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/context/scoring/scorers.py
+-rw-r--r--   0        0        0      242 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/context/stock/__init__.py
+-rw-r--r--   0        0        0     5499 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/context/stock/queries.py
+-rw-r--r--   0        0        0    10538 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/context/stock/stock.py
+-rw-r--r--   0        0        0     1446 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/data/default_training.yml
+-rw-r--r--   0        0        0      487 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/data/logging.yml
+-rw-r--r--   0        0        0      782 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/data/templates/reaction_tree.dot
+-rw-r--r--   0        0        0     1265 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/data/templates/reaction_tree.thtml
+-rw-r--r--   0        0        0      176 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/interfaces/__init__.py
+-rw-r--r--   0        0        0    15064 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/interfaces/aizynthapp.py
+-rw-r--r--   0        0        0    11726 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/interfaces/aizynthcli.py
+-rw-r--r--   0        0        0       81 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/interfaces/gui/__init__.py
+-rw-r--r--   0        0        0     4248 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/interfaces/gui/clustering.py
+-rw-r--r--   0        0        0    14297 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/reactiontree.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/__init__.py
+-rw-r--r--   0        0        0     8187 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/andor_trees.py
+-rw-r--r--   0        0        0      124 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/breadth_first/__init__.py
+-rw-r--r--   0        0        0     7699 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/breadth_first/nodes.py
+-rw-r--r--   0        0        0     5579 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/breadth_first/search_tree.py
+-rw-r--r--   0        0        0      106 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/dfpn/__init__.py
+-rw-r--r--   0        0        0    11071 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/dfpn/nodes.py
+-rw-r--r--   0        0        0     4734 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/dfpn/search_tree.py
+-rw-r--r--   0        0        0      211 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/mcts/__init__.py
+-rw-r--r--   0        0        0    15801 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/mcts/node.py
+-rw-r--r--   0        0        0     5594 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/mcts/search.py
+-rw-r--r--   0        0        0     6466 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/mcts/state.py
+-rw-r--r--   0        0        0     2583 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/mcts/utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/retrostar/__init__.py
+-rw-r--r--   0        0        0     2532 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/retrostar/cost.py
+-rw-r--r--   0        0        0    11662 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/retrostar/nodes.py
+-rw-r--r--   0        0        0     6522 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/search/retrostar/search_tree.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/tools/__init__.py
+-rw-r--r--   0        0        0      815 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/tools/cat_output.py
+-rw-r--r--   0        0        0     3721 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/tools/download_public_data.py
+-rw-r--r--   0        0        0     4678 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/tools/make_stock.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/training/__init__.py
+-rw-r--r--   0        0        0     8540 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/training/keras_models.py
+-rw-r--r--   0        0        0     9199 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/training/make_false_products.py
+-rw-r--r--   0        0        0     5300 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/training/preprocess_expansion.py
+-rw-r--r--   0        0        0     2832 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/training/preprocess_filter.py
+-rw-r--r--   0        0        0     2756 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/training/preprocess_recommender.py
+-rw-r--r--   0        0        0     1085 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/training/training.py
+-rw-r--r--   0        0        0     8760 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/training/utils.py
+-rw-r--r--   0        0        0        0 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/utils/__init__.py
+-rw-r--r--   0        0        0      914 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/utils/exceptions.py
+-rw-r--r--   0        0        0     5235 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/utils/files.py
+-rw-r--r--   0        0        0    16521 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/utils/image.py
+-rw-r--r--   0        0        0     1503 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/utils/loading.py
+-rw-r--r--   0        0        0     1626 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/utils/logging.py
+-rw-r--r--   0        0        0    12001 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/utils/models.py
+-rw-r--r--   0        0        0     1539 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/utils/mongo.py
+-rw-r--r--   0        0        0      355 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/utils/paths.py
+-rw-r--r--   0        0        0      690 2023-06-01 12:50:10.924720 aizynthfinder-3.7.0/aizynthfinder/utils/type_utils.py
+-rw-r--r--   0        0        0     2367 2023-06-01 12:50:10.932720 aizynthfinder-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7888 1970-01-01 00:00:00.000000 aizynthfinder-3.7.0/PKG-INFO
```

### Comparing `aizynthfinder-3.6.0/LICENSE` & `aizynthfinder-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/README.md` & `aizynthfinder-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/aizynthfinder.py` & `aizynthfinder-3.7.0/aizynthfinder/aizynthfinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 """ Module containing a class that is the main interface the retrosynthesis tool.
 """
 from __future__ import annotations
+
 import time
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
 from tqdm import tqdm
 
-# This must be imported first to setup logging for rdkit, tensorflow etc
-from aizynthfinder.utils.logging import logger
-from aizynthfinder.utils.loading import load_dynamic_class
-from aizynthfinder.context.config import Configuration
-from aizynthfinder.search.mcts import MctsSearchTree
-from aizynthfinder.reactiontree import ReactionTreeFromExpansion
 from aizynthfinder.analysis import (
-    TreeAnalysis,
     RouteCollection,
     RouteSelectionArguments,
+    TreeAnalysis,
 )
-from aizynthfinder.chem import Molecule, TreeMolecule, FixedRetroReaction
+from aizynthfinder.chem import FixedRetroReaction, Molecule, TreeMolecule
+from aizynthfinder.context.config import Configuration
+from aizynthfinder.reactiontree import ReactionTreeFromExpansion
 from aizynthfinder.search.andor_trees import AndOrSearchTreeBase
+from aizynthfinder.search.mcts import MctsSearchTree
 from aizynthfinder.utils.exceptions import MoleculeException
+from aizynthfinder.utils.loading import load_dynamic_class
+
+# This must be imported first to setup logging for rdkit, tensorflow etc
+from aizynthfinder.utils.logging import logger
 
 if TYPE_CHECKING:
+    from aizynthfinder.chem import RetroReaction
     from aizynthfinder.utils.type_utils import (
-        StrDict,
-        Optional,
-        Union,
         Callable,
+        Dict,
         List,
+        Optional,
+        StrDict,
         Tuple,
-        Dict,
+        Union,
     )
-    from aizynthfinder.chem import RetroReaction
 
 
 class AiZynthFinder:
     """
     Public API to the aizynthfinder tool
 
     If instantiated with the path to a yaml file or dictionary of settings
@@ -226,25 +228,23 @@
         if show_progress:
             pbar.close()
         time_past = time.time() - time0
         self._logger.debug("Search completed")
         self.search_stats["time"] = time_past
         return time_past
 
-    def _setup_search_tree(self):
+    def _setup_search_tree(self) -> None:
         self._logger.debug("Defining tree root: %s" % self.target_smiles)
         if self.config.search_algorithm.lower() == "mcts":
             self.tree = MctsSearchTree(
                 root_smiles=self.target_smiles, config=self.config
             )
         else:
             cls = load_dynamic_class(self.config.search_algorithm)
-            self.tree: AndOrSearchTreeBase = cls(
-                root_smiles=self.target_smiles, config=self.config
-            )
+            self.tree = cls(root_smiles=self.target_smiles, config=self.config)
 
 
 class AiZynthExpander:
     """
     Public API to the AiZynthFinder expansion and filter policies
 
     If instantiated with the path to a yaml file or dictionary of settings
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/analysis/routes.py` & `aizynthfinder-3.7.0/aizynthfinder/analysis/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """ Module containing classes to store and manipulate collections of synthetic routes.
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 try:
     from route_distances.clustering import ClusteringHelper
     from route_distances.route_distances import route_distances_calculator
 except ImportError:
     pass
 
-from aizynthfinder.analysis.utils import (
-    CombinedReactionTrees,
-    RouteSelectionArguments,
-)
-from aizynthfinder.reactiontree import SUPPORT_DISTANCES, ReactionTree
-from aizynthfinder.search.mcts import MctsSearchTree, MctsNode
 from aizynthfinder.analysis import TreeAnalysis
+from aizynthfinder.analysis.utils import CombinedReactionTrees, RouteSelectionArguments
+from aizynthfinder.reactiontree import SUPPORT_DISTANCES, ReactionTree
+from aizynthfinder.search.mcts import MctsNode, MctsSearchTree
 
 if TYPE_CHECKING:
+    from aizynthfinder.context.scoring import Scorer
     from aizynthfinder.utils.type_utils import (
-        StrDict,
-        PilImage,
-        Optional,
         Any,
         Dict,
+        Optional,
+        PilImage,
         Sequence,
+        StrDict,
     )
-    from aizynthfinder.context.scoring import Scorer
 
 
 class RouteCollection:
     """
     Holds a collections of reaction routes.
 
     If can be the top scored nodes, their scores and
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/analysis/tree_analysis.py` & `aizynthfinder-3.7.0/aizynthfinder/analysis/tree_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 """ Module containing classes to perform analysis of the tree search results.
 """
 from __future__ import annotations
+
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
-from aizynthfinder.chem import (
-    FixedRetroReaction,
-    hash_reactions,
-)
-from aizynthfinder.context.scoring import (
-    StateScorer,
-)
 from aizynthfinder.analysis.utils import RouteSelectionArguments
+from aizynthfinder.chem import FixedRetroReaction, hash_reactions
+from aizynthfinder.context.scoring import StateScorer
 from aizynthfinder.reactiontree import ReactionTree
-from aizynthfinder.search.mcts import MctsSearchTree, MctsNode
 from aizynthfinder.search.andor_trees import AndOrSearchTreeBase
+from aizynthfinder.search.mcts import MctsNode, MctsSearchTree
 
 if TYPE_CHECKING:
+    from aizynthfinder.chem import RetroReaction
+    from aizynthfinder.context.scoring import Scorer
     from aizynthfinder.utils.type_utils import (
-        StrDict,
-        Union,
-        Tuple,
         Any,
         Iterable,
-        Sequence,
         List,
+        Sequence,
+        StrDict,
+        Tuple,
+        Union,
     )
-    from aizynthfinder.context.scoring import Scorer
-    from aizynthfinder.chem import RetroReaction
 
 
 class TreeAnalysis:
     """
     Class that encapsulate various analysis that can be
     performed on a search tree.
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/analysis/utils.py` & `aizynthfinder-3.7.0/aizynthfinder/analysis/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,25 @@
 """
 Helper routines and class for the `aizynthfinder.analysis` package.
 To avoid clutter in that package, larger utility algorithms are placed herein.
 """
 from __future__ import annotations
-from dataclasses import dataclass
+
 from collections import defaultdict
+from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 import networkx as nx
 
-from aizynthfinder.chem import (
-    Molecule,
-    UniqueMolecule,
-    FixedRetroReaction,
-)
-from aizynthfinder.utils.image import make_visjs_page
+from aizynthfinder.chem import FixedRetroReaction, Molecule, UniqueMolecule
 from aizynthfinder.reactiontree import ReactionTree
+from aizynthfinder.utils.image import make_visjs_page
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import (
-        Sequence,
-        Tuple,
-        StrDict,
-        FrameColors,
-    )
+    from aizynthfinder.utils.type_utils import FrameColors, Sequence, StrDict, Tuple
 
 
 @dataclass
 class RouteSelectionArguments:
     """
     Selection arguments for the tree analysis class
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/chem/mol.py` & `aizynthfinder-3.7.0/aizynthfinder/chem/mol.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 """ Module containing classes to deal with Molecules - mostly wrappers around rdkit routines.
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 import numpy as np
 from rdkit import Chem, DataStructs
 from rdkit.Chem import AllChem, Descriptors
 
 from aizynthfinder.utils.exceptions import MoleculeException
 
-
 if TYPE_CHECKING:
     from aizynthfinder.utils.type_utils import (
+        Callable,
         Dict,
+        List,
         Optional,
-        Union,
-        Tuple,
         RdMol,
         Sequence,
-        List,
-        Callable,
+        Tuple,
+        Union,
     )
 
 
 class Molecule:
     """
     A base class for molecules. Encapsulate an RDKit mol object and
     functions that can be applied to such a molecule.
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/chem/reaction.py` & `aizynthfinder-3.7.0/aizynthfinder/chem/reaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 """ Module containing classes to deal with Reactions.
 """
 from __future__ import annotations
-import hashlib
+
 import abc
+import hashlib
 from functools import partial
 from typing import TYPE_CHECKING
 
 import numpy as np
-from rdkit import Chem
-from rdkit.Chem import AllChem
-from rdkit.Chem.rdchem import ChiralType, BondDir, BondStereo
 from rdchiral import main as rdc
 from rdchiral.bonds import get_atoms_across_double_bonds
 from rdchiral.initialization import BondDirOpposite
+from rdkit import Chem
+from rdkit.Chem import AllChem
+from rdkit.Chem.rdchem import BondDir, BondStereo, ChiralType
 
+from aizynthfinder.chem.mol import Molecule, MoleculeException, TreeMolecule
 from aizynthfinder.utils.logging import logger
-from aizynthfinder.chem.mol import MoleculeException, Molecule, TreeMolecule
 
 if TYPE_CHECKING:
+    from aizynthfinder.chem.mol import UniqueMolecule
     from aizynthfinder.utils.type_utils import (
-        Optional,
-        Union,
-        Tuple,
+        Any,
+        Iterable,
         List,
+        Optional,
         RdReaction,
-        StrDict,
-        Iterable,
-        Any,
         Set,
+        StrDict,
+        Tuple,
+        Union,
     )
-    from aizynthfinder.chem.mol import UniqueMolecule
 
 
 class _ReactionInterfaceMixin:
     """
     Mixin class to define a common interface for all reaction class
 
     The methods `_products_getter` and `_reactants_getter` needs to be implemented by subclasses
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/chem/serialization.py` & `aizynthfinder-3.7.0/aizynthfinder/chem/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """ Module containing helper classes and routines for serialization.
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 import aizynthfinder.chem
 from aizynthfinder.utils.loading import load_dynamic_class
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import Optional, Sequence, Dict, Any, StrDict
     from aizynthfinder.chem import RetroReaction
+    from aizynthfinder.utils.type_utils import Any, Dict, Optional, Sequence, StrDict
 
 
 class MoleculeSerializer:
     """
     Utility class for serializing molecules
 
     The id of the molecule to be serialized can be obtained with:
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/collection.py` & `aizynthfinder-3.7.0/aizynthfinder/context/collection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """ Module containing a class that is the base class for all collection classes (stock, policies, scorers)
 """
 from __future__ import annotations
+
 import abc
 from typing import TYPE_CHECKING
 
 from aizynthfinder.utils.logging import logger
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import StrDict
-    from aizynthfinder.utils.type_utils import Any, List, Union
+    from aizynthfinder.utils.type_utils import Any, List, StrDict, Union
 
 
 class ContextCollection(abc.ABC):
     """
     Abstract base class for a collection of items
     that can be loaded and then (de-)selected.
 
@@ -30,15 +30,15 @@
 
 
     """
 
     _single_selection = False
     _collection_name = "collection"
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._items: StrDict = {}
         self._selection: List[str] = []
         self._logger = logger()
 
     def __delitem__(self, key: str) -> None:
         if key not in self._items:
             raise KeyError(
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/config.py` & `aizynthfinder-3.7.0/aizynthfinder/context/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """ Module containing a class for encapsulating the settings of the tree search
 """
 from __future__ import annotations
+
+import os
+import re
 from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 import yaml
 
-from aizynthfinder.utils.logging import logger
+from aizynthfinder.context.cost import MoleculeCost
 from aizynthfinder.context.policy import ExpansionPolicy, FilterPolicy
-from aizynthfinder.context.stock import Stock
 from aizynthfinder.context.scoring import ScorerCollection
-from aizynthfinder.context.cost import MoleculeCost
-
+from aizynthfinder.context.stock import Stock
+from aizynthfinder.utils.logging import logger
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import StrDict, Any, Dict, Union, Optional
+    from aizynthfinder.utils.type_utils import Any, Dict, Optional, StrDict, Union
 
 
 @dataclass
 class _PostprocessingConfiguration:
     min_routes: int = 5
     max_routes: int = 25
     all_routes: bool = False
@@ -103,20 +105,31 @@
 
     @classmethod
     def from_file(cls, filename: str) -> "Configuration":
         """
         Loads a configuration from a yaml file.
         The parameters not set in the yaml file are taken from the default values.
         The policies and stocks specified in the yaml file are directly loaded.
+        The parameters in the yaml file may also contain environment variables as
+        values.
 
         :param filename: the path to a yaml file
         :return: a Configuration object with settings from the yaml file
+        :raises:
+            ValueError: if parameter's value expects an environment variable that
+                does not exist in the current environment
         """
         with open(filename, "r") as fileobj:
-            _config = yaml.load(fileobj.read(), Loader=yaml.SafeLoader)
+            txt = fileobj.read()
+        environ_var = re.findall(r"\$\{.+?\}", txt)
+        for item in environ_var:
+            if item[2:-1] not in os.environ:
+                raise ValueError(f"'{item[2:-1]}' not in environment variables")
+            txt = txt.replace(item, os.environ[item[2:-1]])
+        _config = yaml.load(txt, Loader=yaml.SafeLoader)
         return Configuration.from_dict(_config)
 
     @property
     def properties(self) -> Dict[str, Union[int, float, str, bool]]:
         """Return the basic properties of the config as a dictionary"""
         dict_ = {}
         for item in dir(self):
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/cost/collection.py` & `aizynthfinder-3.7.0/aizynthfinder/context/cost/collection.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 """ Module containing classes to compute the molecule cost in some search algorithms
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 from aizynthfinder.context.collection import ContextCollection
-from aizynthfinder.utils.loading import load_dynamic_class
-from aizynthfinder.utils.exceptions import CostException
 from aizynthfinder.context.cost.costs import MoleculeCostCalculator, ZeroMoleculeCost
-from aizynthfinder.context.cost.costs import (
-    __name__ as costs_module,
-)
+from aizynthfinder.context.cost.costs import __name__ as costs_module
+from aizynthfinder.utils.exceptions import CostException
+from aizynthfinder.utils.loading import load_dynamic_class
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import Dict, Any
     from aizynthfinder.chem import Molecule
+    from aizynthfinder.utils.type_utils import Any, Dict
 
 
 class MoleculeCost(ContextCollection):
     """Collection of molecular cost objects"""
 
     _single_selection: bool = True
     _collection_name: str = "molecule cost"
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/cost/costs.py` & `aizynthfinder-3.7.0/aizynthfinder/context/cost/costs.py`

 * *Ordering differences only*

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """ Module containing classes that implements different cost calculators
 """
 from __future__ import annotations
+
 import abc
 from typing import TYPE_CHECKING
 
-
 if TYPE_CHECKING:
-    from aizynthfinder.context.config import Configuration
     from aizynthfinder.chem import Molecule
+    from aizynthfinder.context.config import Configuration
 
 
 class MoleculeCostCalculator(abc.ABC):
     """
     A base class for all molecule cost calculators.
 
     The cost can be computed by either calling the `calculate` method
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/policy/expansion_strategies.py` & `aizynthfinder-3.7.0/aizynthfinder/context/policy/expansion_strategies.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 """ Module containing classes that implements different expansion policy strategies
 """
 from __future__ import annotations
+
 import abc
 from typing import TYPE_CHECKING
 
 import numpy as np
 import pandas as pd
 
 from aizynthfinder.chem import TemplatedRetroReaction
-from aizynthfinder.utils.models import load_model
-from aizynthfinder.utils.logging import logger
 from aizynthfinder.context.policy.utils import _make_fingerprint
 from aizynthfinder.utils.exceptions import PolicyException
+from aizynthfinder.utils.logging import logger
+from aizynthfinder.utils.models import load_model
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import Any, Sequence, List, Tuple
-    from aizynthfinder.context.config import Configuration
     from aizynthfinder.chem import TreeMolecule
     from aizynthfinder.chem.reaction import RetroReaction
+    from aizynthfinder.context.config import Configuration
+    from aizynthfinder.utils.type_utils import Any, List, Sequence, Tuple
 
 
 class ExpansionStrategy(abc.ABC):
     """
     A base class for all expansion strategies.
 
     The strategy can be used by either calling the `get_actions` method
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/policy/filter_strategies.py` & `aizynthfinder-3.7.0/aizynthfinder/context/policy/filter_strategies.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """ Module containing classes that implements different filter policy strategies
 """
 from __future__ import annotations
+
 import abc
 from typing import TYPE_CHECKING
 
 import numpy as np
 
-from aizynthfinder.utils.models import load_model
-from aizynthfinder.utils.logging import logger
+from aizynthfinder.chem import TemplatedRetroReaction
 from aizynthfinder.context.policy.utils import _make_fingerprint
 from aizynthfinder.utils.exceptions import PolicyException, RejectionException
-from aizynthfinder.chem import TemplatedRetroReaction
-
+from aizynthfinder.utils.logging import logger
+from aizynthfinder.utils.models import load_model
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import Any, List, Tuple
-    from aizynthfinder.context.config import Configuration
     from aizynthfinder.chem.reaction import RetroReaction
+    from aizynthfinder.context.config import Configuration
+    from aizynthfinder.utils.type_utils import Any, List, Tuple
 
 
 class FilterStrategy(abc.ABC):
     """
     A base class for all filter strategies.
 
     The filter can be applied by either calling the `apply` method
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/policy/policies.py` & `aizynthfinder-3.7.0/aizynthfinder/context/policy/policies.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """ Module containing classes that interfaces neural network policies
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
-from aizynthfinder.utils.loading import load_dynamic_class
-from aizynthfinder.utils.exceptions import PolicyException
 from aizynthfinder.context.collection import ContextCollection
 from aizynthfinder.context.policy.expansion_strategies import (
     ExpansionStrategy,
     TemplateBasedExpansionStrategy,
 )
+from aizynthfinder.context.policy.expansion_strategies import (
+    __name__ as expansion_strategy_module,
+)
 from aizynthfinder.context.policy.filter_strategies import (
+    FILTER_STRATEGY_ALIAS,
     FilterStrategy,
     QuickKerasFilter,
-    FILTER_STRATEGY_ALIAS,
-)
-from aizynthfinder.context.policy.expansion_strategies import (
-    __name__ as expansion_strategy_module,
 )
 from aizynthfinder.context.policy.filter_strategies import (
     __name__ as filter_strategy_module,
 )
+from aizynthfinder.utils.exceptions import PolicyException
+from aizynthfinder.utils.loading import load_dynamic_class
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import Any, Sequence, List, Tuple
-    from aizynthfinder.context.config import Configuration
     from aizynthfinder.chem import TreeMolecule
     from aizynthfinder.chem.reaction import RetroReaction
+    from aizynthfinder.context.config import Configuration
+    from aizynthfinder.utils.type_utils import Any, List, Sequence, Tuple
 
 
 class ExpansionPolicy(ContextCollection):
     """
     An abstraction of an expansion policy.
 
     This policy provides actions that can be applied to a molecule
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/scoring/collection.py` & `aizynthfinder-3.7.0/aizynthfinder/context/scoring/collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,31 @@
 """ Module containing classes used to score the reaction routes.
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
-from aizynthfinder.search.mcts import MctsNode
-from aizynthfinder.reactiontree import ReactionTree
 from aizynthfinder.context.collection import ContextCollection
-from aizynthfinder.context.scoring.scorers import __name__ as scorers_module
 from aizynthfinder.context.scoring.scorers import (
+    AverageTemplateOccurrenceScorer,
+    NumberOfPrecursorsInStockScorer,
+    NumberOfPrecursorsScorer,
+    NumberOfReactionsScorer,
     Scorer,
     StateScorer,
-    NumberOfReactionsScorer,
-    NumberOfPrecursorsScorer,
-    NumberOfPrecursorsInStockScorer,
-    AverageTemplateOccurrenceScorer,
 )
+from aizynthfinder.context.scoring.scorers import __name__ as scorers_module
+from aizynthfinder.reactiontree import ReactionTree
+from aizynthfinder.search.mcts import MctsNode
 from aizynthfinder.utils.exceptions import ScorerException
 from aizynthfinder.utils.loading import load_dynamic_class
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import (
-        Union,
-        List,
-        Any,
-        Sequence,
-        TypeVar,
-    )
     from aizynthfinder.context.config import Configuration
+    from aizynthfinder.utils.type_utils import Any, List, Sequence, TypeVar, Union
 
     _Scoreable = TypeVar("_Scoreable", MctsNode, ReactionTree)
     _Scoreables = Sequence[_Scoreable]
     _ScorerItemType = Union[_Scoreables, _Scoreable]
 
 
 _SIMPLE_SCORERS = [
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/scoring/scorers.py` & `aizynthfinder-3.7.0/aizynthfinder/context/scoring/scorers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,26 @@
 """ Module containing classes used to score the reaction routes.
 """
 from __future__ import annotations
+
 import abc
 from collections import defaultdict
 from collections.abc import Sequence as SequenceAbc
 from typing import TYPE_CHECKING
 
-from aizynthfinder.search.mcts import MctsNode
-from aizynthfinder.reactiontree import ReactionTree
-from aizynthfinder.search.mcts import MctsState
 from aizynthfinder.chem import TreeMolecule
 from aizynthfinder.context.stock import StockException
+from aizynthfinder.reactiontree import ReactionTree
+from aizynthfinder.search.mcts import MctsNode, MctsState
 from aizynthfinder.utils.exceptions import ScorerException
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import (
-        Union,
-        Tuple,
-        Sequence,
-        Iterable,
-        TypeVar,
-    )
+    from aizynthfinder.chem import FixedRetroReaction, Molecule, RetroReaction
     from aizynthfinder.context.config import Configuration
-    from aizynthfinder.chem import Molecule, RetroReaction, FixedRetroReaction
+    from aizynthfinder.utils.type_utils import Iterable, Sequence, Tuple, TypeVar, Union
 
     _Scoreable = TypeVar("_Scoreable", MctsNode, ReactionTree)
     _Scoreables = Sequence[_Scoreable]
     _ScorerItemType = Union[_Scoreables, _Scoreable]
 
 
 class Scorer(abc.ABC):
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/stock/queries.py` & `aizynthfinder-3.7.0/aizynthfinder/context/stock/queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """ Module containing classes that interfaces different stocks query classes
 """
 from __future__ import annotations
+
 import os
 from typing import TYPE_CHECKING
 
 import pandas as pd
 
 from aizynthfinder.chem import Molecule
-from aizynthfinder.utils.mongo import get_mongo_client
 from aizynthfinder.utils.exceptions import StockException
+from aizynthfinder.utils.mongo import get_mongo_client
 
 if TYPE_CHECKING:
-    from pymongo.database import Database as MongoDatabase
     from pymongo.collection import Collection as MongoCollection
+    from pymongo.database import Database as MongoDatabase
 
     # pylint: disable=ungrouped-imports
-    from aizynthfinder.utils.type_utils import Set, Optional
+    from aizynthfinder.utils.type_utils import Optional, Set
 
 
 # pylint: disable=no-self-use
 class StockQueryMixin:
     """
     Mixin class for all query classes, providing a default interface
     to some methods that might not be possible to implement for each
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/context/stock/stock.py` & `aizynthfinder-3.7.0/aizynthfinder/context/stock/stock.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 """ Module containing classes that interfaces different stock classes
 """
 from __future__ import annotations
+
 import copy
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
 from aizynthfinder.chem import Molecule
 from aizynthfinder.context.collection import ContextCollection
-from aizynthfinder.utils.exceptions import StockException
-from aizynthfinder.utils.loading import load_dynamic_class
 from aizynthfinder.context.stock.queries import (
     InMemoryInchiKeyQuery,
     MongoDbInchiKeyQuery,
 )
+from aizynthfinder.utils.exceptions import StockException
+from aizynthfinder.utils.loading import load_dynamic_class
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import StrDict, Set, Union, Any, List
+    from aizynthfinder.utils.type_utils import Any, List, Set, StrDict, Union
 
 
 class Stock(ContextCollection):
     """
     A collection of molecules that are in stock
 
     A molecule can be queried on the stock with:
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/data/default_training.yml` & `aizynthfinder-3.7.0/aizynthfinder/data/default_training.yml`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/data/templates/reaction_tree.dot` & `aizynthfinder-3.7.0/aizynthfinder/data/templates/reaction_tree.dot`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/data/templates/reaction_tree.thtml` & `aizynthfinder-3.7.0/aizynthfinder/data/templates/reaction_tree.thtml`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/interfaces/aizynthapp.py` & `aizynthfinder-3.7.0/aizynthfinder/interfaces/aizynthapp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 """ Module containing classes and routines for the GUI interface
 """
-import tempfile
-import signal
-import subprocess
-import os
 import argparse
 import logging
+import os
+import signal
+import subprocess
+import tempfile
 from typing import TYPE_CHECKING
 
 import ipywidgets as widgets
 import jupytext
+from IPython.display import HTML, display
 from ipywidgets import (
+    BoundedFloatText,
+    BoundedIntText,
+    Button,
+    Checkbox,
+    Dropdown,
+    FloatText,
     HBox,
+    IntText,
     Label,
-    VBox,
-    Text,
     Output,
-    Checkbox,
-    IntText,
-    FloatText,
-    Button,
-    Dropdown,
-    BoundedIntText,
-    BoundedFloatText,
     SelectMultiple,
+    Text,
+    VBox,
 )
 from rdkit import Chem
-from IPython.display import display, HTML
 
 from aizynthfinder.aizynthfinder import AiZynthFinder
 from aizynthfinder.utils.logging import setup_logger
 
 if TYPE_CHECKING:
     from aizynthfinder.utils.type_utils import StrDict
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/interfaces/aizynthcli.py` & `aizynthfinder-3.7.0/aizynthfinder/interfaces/aizynthcli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 """ Module containing classes and routines for the CLI
 """
 from __future__ import annotations
+
 import argparse
+import importlib
 import json
-import os
 import logging
-import importlib
+import os
 import tempfile
 import time
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
 import pandas as pd
 
 from aizynthfinder.aizynthfinder import AiZynthFinder
+from aizynthfinder.chem import Molecule
 from aizynthfinder.utils.files import (
     cat_datafiles,
     save_datafile,
     split_file,
     start_processes,
 )
-from aizynthfinder.chem import Molecule
 from aizynthfinder.utils.logging import logger, setup_logger
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import StrDict, Callable, List, Optional
+    from aizynthfinder.utils.type_utils import (
+        Any,
+        Callable,
+        Dict,
+        List,
+        Optional,
+        StrDict,
+        Union,
+    )
 
     _PostProcessingJob = Callable[[AiZynthFinder], StrDict]
 
 
 def _do_clustering(
     finder: AiZynthFinder,
     results: StrDict,
@@ -102,14 +111,19 @@
         help="if provided, calculate route distances for clustering with this ML model",
     )
     parser.add_argument(
         "--post_processing",
         nargs="+",
         help="a number of modules that performs post-processing tasks",
     )
+    parser.add_argument(
+        "--checkpoint",
+        required=False,
+        help="the path to the checkpoint file",
+    )
     return parser.parse_args()
 
 
 def _load_postprocessing_jobs(modules: Optional[List[str]]) -> List[_PostProcessingJob]:
     jobs: List[_PostProcessingJob] = []
     for module_name in modules or []:
         try:
@@ -132,14 +146,33 @@
     else:
         if hasattr(module, "stock"):
             finder.stock.load(module.stock, "custom_stock")  # type: ignore
             stocks.append("custom_stock")
     finder.stock.select(stocks or finder.stock.items)
 
 
+def _load_checkpoint(
+    checkpoint: str,
+) -> Dict[str, List[Any]]:
+    if not os.path.exists(checkpoint):
+        return defaultdict(list)
+    with open(checkpoint) as json_file:
+        checkpoint_data = [json.loads(line) for line in json_file]
+
+    checkpoint_results = defaultdict(list)
+    if checkpoint_data:
+        checkpoint_results["processed_smiles"] = [
+            data["processed_smiles"] for data in checkpoint_data
+        ]
+        for data in checkpoint_data:
+            for key, value in data["results"].items():
+                checkpoint_results[key].append(value)
+    return checkpoint_results
+
+
 def _process_single_smiles(
     smiles: str,
     finder: AiZynthFinder,
     output_name: str,
     do_clustering: bool,
     route_distance_model: Optional[str],
     post_processing: List[_PostProcessingJob],
@@ -176,21 +209,35 @@
 def _process_multi_smiles(
     filename: str,
     finder: AiZynthFinder,
     output_name: str,
     do_clustering: bool,
     route_distance_model: Optional[str],
     post_processing: List[_PostProcessingJob],
+    checkpoint: Optional[str],
 ) -> None:
     output_name = output_name or "output.json.gz"
     with open(filename, "r") as fileobj:
         smiles = [line.strip() for line in fileobj.readlines()]
 
-    results = defaultdict(list)
+    checkpoint_data: StrDict = defaultdict(list)
+    if checkpoint:
+        checkpoint_data = _load_checkpoint(checkpoint)
+        start = len(checkpoint_data["processed_smiles"]) if checkpoint_data else 0
+        smiles = smiles[start:]
+
+    results: StrDict = defaultdict(list)
+    if checkpoint_data:
+        results = {
+            key: value
+            for key, value in checkpoint_data.items()
+            if key != "processed_smiles"
+        }
     for smi in smiles:
+        processed_results = {}
         finder.target_smiles = smi
         try:
             finder.prepare_tree()
         except ValueError as err:
             print(f"Failed to setup search for {smi} due to: '{str(err).lower()}'")
             continue
         search_time = finder.tree_search()
@@ -200,24 +247,38 @@
         solved_str = "is solved" if stats["is_solved"] else "is not solved"
         logger().info(f"Done with {smi} in {search_time:.3} s and {solved_str}")
         if do_clustering:
             _do_clustering(
                 finder, stats, detailed_results=True, model_path=route_distance_model
             )
         _do_post_processing(finder, stats, post_processing)
+
         for key, value in stats.items():
-            results[key].append(value)
-        results["stock_info"].append(finder.stock_info())
-        results["top_scores"].append(
-            ", ".join("%.4f" % score for score in finder.routes.scores)
+            processed_results[key] = value
+        processed_results["stock_info"] = finder.stock_info()
+        processed_results["top_scores"] = ", ".join(
+            "%.4f" % score for score in finder.routes.scores
         )
-        results["trees"].append(
-            finder.routes.dict_with_extra(include_metadata=True, include_scores=True)
+        processed_results["trees"] = finder.routes.dict_with_extra(
+            include_metadata=True, include_scores=True
         )
 
+        if checkpoint:
+            with open(checkpoint, "a") as checkpoint_file:
+                checkpoint_file.write(
+                    json.dumps({"processed_smiles": smi, "results": processed_results})
+                    + "\n"
+                )
+            logger().debug(
+                f"Results for processed smiles '{smi}' saved to {checkpoint}"
+            )
+
+        for key, value in processed_results.items():
+            results[key].append(value)
+
     data = pd.DataFrame.from_dict(results)
     save_datafile(data, output_name)
     logger().info(f"Output saved to {output_name}")
 
 
 def _multiprocess_smiles(args: argparse.Namespace) -> None:
     def create_cmd(index, filename):
@@ -285,22 +346,30 @@
 
     multi_smiles = os.path.exists(args.smiles)
 
     finder = AiZynthFinder(configfile=args.config)
     _select_stocks(finder, args)
     post_processing = _load_postprocessing_jobs(args.post_processing)
     finder.expansion_policy.select(args.policy or finder.expansion_policy.items[0])
-    finder.filter_policy.select(args.filter)
+    if args.filter:
+        finder.filter_policy.select(args.filter)
+    else:
+        finder.filter_policy.select_all()
 
-    func = _process_multi_smiles if multi_smiles else _process_single_smiles
-    func(
+    params = [
         args.smiles,
         finder,
         args.output,
         args.cluster,
         args.route_distance_model,
         post_processing,
-    )
+        args.checkpoint,
+    ]
+    if multi_smiles:
+        _process_multi_smiles(*params)
+    else:
+        params = params[:-1]
+        _process_single_smiles(*params)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/interfaces/gui/clustering.py` & `aizynthfinder-3.7.0/aizynthfinder/interfaces/gui/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 """ Module containing a GUI extension for clustering
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 import numpy as np
-from ipywidgets import Output, Label, BoundedIntText, Button, HBox, Tab
 from IPython.display import display
+from ipywidgets import BoundedIntText, Button, HBox, Label, Output, Tab
 
 try:
     import matplotlib.pylab as plt
-    from scipy.cluster.hierarchy import dendrogram
     from route_distances.clustering import ClusteringHelper
+    from scipy.cluster.hierarchy import dendrogram
 except ImportError:
     raise ImportError(
         "Clustering is not supported by this installation."
         " Please install aizynthfinder with extras dependencies."
     )
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/reactiontree.py` & `aizynthfinder-3.7.0/aizynthfinder/reactiontree.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 """ Module containing the implementation of a reaction tree or route and factory classes to make such trees """
 from __future__ import annotations
-import operator
-import json
+
 import abc
 import hashlib
+import json
+import operator
 from typing import TYPE_CHECKING
 
 import networkx as nx
 from networkx.algorithms.traversal.depth_first_search import dfs_tree
 
 try:
     from route_distances.route_distances import route_distances_calculator
 except ImportError:
     SUPPORT_DISTANCES = False
 else:
     SUPPORT_DISTANCES = True
 
 from aizynthfinder.chem import (
+    FixedRetroReaction,
     Molecule,
     UniqueMolecule,
-    FixedRetroReaction,
     none_molecule,
 )
 from aizynthfinder.utils.image import RouteImageFactory
 
-
 if TYPE_CHECKING:
+    from aizynthfinder.chem import RetroReaction
     from aizynthfinder.utils.type_utils import (
-        StrDict,
-        PilImage,
-        FrameColors,
-        Union,
-        Iterable,
         Any,
         Dict,
+        FrameColors,
+        Iterable,
         Optional,
+        PilImage,
+        StrDict,
+        Union,
     )
-    from aizynthfinder.chem import RetroReaction
 
 
 class ReactionTree:
     """
     Encapsulation of a bipartite reaction tree of a single route.
     The nodes consists of either FixedRetroReaction or UniqueMolecule objects.
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/andor_trees.py` & `aizynthfinder-3.7.0/aizynthfinder/search/andor_trees.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """ Module for base classes for AND/OR trees and some tree utility code """
 from __future__ import annotations
-import random
+
 import abc
+import random
 from typing import TYPE_CHECKING
 
 import networkx as nx
 
-from aizynthfinder.reactiontree import ReactionTree, ReactionTreeLoader
 from aizynthfinder.chem import UniqueMolecule
+from aizynthfinder.reactiontree import ReactionTree, ReactionTreeLoader
 
 if TYPE_CHECKING:
+    from aizynthfinder.chem import FixedRetroReaction
     from aizynthfinder.context.config import Configuration
     from aizynthfinder.context.stock import Stock
-    from aizynthfinder.chem import FixedRetroReaction
-    from aizynthfinder.utils.type_utils import StrDict, Any, List, Union, Optional
+    from aizynthfinder.utils.type_utils import Any, List, Optional, StrDict, Union
 
 
 class TreeNodeMixin:
     """A mixin class for node in a tree"""
 
     @property
     def prop(self) -> StrDict:
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/breadth_first/nodes.py` & `aizynthfinder-3.7.0/aizynthfinder/search/breadth_first/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 """ Module containing a classes representation various tree nodes
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 from aizynthfinder.chem import TreeMolecule
-from aizynthfinder.search.andor_trees import TreeNodeMixin
 from aizynthfinder.chem.serialization import deserialize_action, serialize_action
+from aizynthfinder.search.andor_trees import TreeNodeMixin
 
 if TYPE_CHECKING:
-    from aizynthfinder.context.config import Configuration
+    from aizynthfinder.chem import RetroReaction
     from aizynthfinder.chem.serialization import (
         MoleculeDeserializer,
         MoleculeSerializer,
     )
-    from aizynthfinder.utils.type_utils import (
-        StrDict,
-        Sequence,
-        Set,
-        List,
-    )
-    from aizynthfinder.chem import RetroReaction
+    from aizynthfinder.context.config import Configuration
+    from aizynthfinder.utils.type_utils import List, Sequence, Set, StrDict
 
 
 class MoleculeNode(TreeNodeMixin):
     """
     An OR node representing a molecule
 
     :ivar expandable: if True, this node is part of the frontier
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/breadth_first/search_tree.py` & `aizynthfinder-3.7.0/aizynthfinder/search/breadth_first/search_tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """ Module containing a class that holds the tree search
 """
 from __future__ import annotations
+
 import json
 from typing import TYPE_CHECKING
 
+from aizynthfinder.chem.serialization import MoleculeDeserializer, MoleculeSerializer
+from aizynthfinder.search.andor_trees import AndOrSearchTreeBase, SplitAndOrTree
 from aizynthfinder.search.breadth_first.nodes import MoleculeNode
 from aizynthfinder.utils.logging import logger
-from aizynthfinder.search.andor_trees import AndOrSearchTreeBase, SplitAndOrTree
-from aizynthfinder.chem.serialization import MoleculeDeserializer, MoleculeSerializer
 
 if TYPE_CHECKING:
+    from aizynthfinder.chem import RetroReaction
     from aizynthfinder.context.config import Configuration
     from aizynthfinder.reactiontree import ReactionTree
-    from aizynthfinder.chem import RetroReaction
-    from aizynthfinder.utils.type_utils import Optional, Sequence, List
+    from aizynthfinder.utils.type_utils import List, Optional, Sequence
 
 
 class SearchTree(AndOrSearchTreeBase):
     """
     Encapsulation of the a breadth-first exhaustive search algorithm
 
     :ivar config: settings of the tree search algorithm
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/dfpn/nodes.py` & `aizynthfinder-3.7.0/aizynthfinder/search/dfpn/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """ Module containing a classes representation various tree nodes
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from aizynthfinder.chem import TreeMolecule
 from aizynthfinder.search.andor_trees import TreeNodeMixin
 
-
 if TYPE_CHECKING:
-    from aizynthfinder.context.config import Configuration
-    from aizynthfinder.utils.type_utils import StrDict, Sequence, Set, List, Optional
     from aizynthfinder.chem import RetroReaction
+    from aizynthfinder.context.config import Configuration
     from aizynthfinder.search.dfpn import SearchTree
+    from aizynthfinder.utils.type_utils import List, Optional, Sequence, Set, StrDict
 
 BIG_INT = int(1e10)
 
 
 class _SuperNode(TreeNodeMixin):
     def __init__(self) -> None:
         # pylint: disable=invalid-name
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/dfpn/search_tree.py` & `aizynthfinder-3.7.0/aizynthfinder/search/dfpn/search_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """ Module containing a class that holds the tree search
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
+from aizynthfinder.reactiontree import ReactionTree
+from aizynthfinder.search.andor_trees import AndOrSearchTreeBase, SplitAndOrTree
 from aizynthfinder.search.dfpn.nodes import MoleculeNode, ReactionNode
 from aizynthfinder.utils.logging import logger
-from aizynthfinder.search.andor_trees import AndOrSearchTreeBase, SplitAndOrTree
-from aizynthfinder.reactiontree import ReactionTree
-
 
 if TYPE_CHECKING:
-    from aizynthfinder.search.andor_trees import TreeNodeMixin
-    from aizynthfinder.context.config import Configuration
     from aizynthfinder.chem import RetroReaction
-    from aizynthfinder.utils.type_utils import Optional, Sequence, List, Union
+    from aizynthfinder.context.config import Configuration
+    from aizynthfinder.search.andor_trees import TreeNodeMixin
+    from aizynthfinder.utils.type_utils import List, Optional, Sequence, Union
 
 
 class SearchTree(AndOrSearchTreeBase):
     """
     Encapsulation of the Depth-First Proof-Number (DFPN) search algorithm.
 
     This algorithm does not support:
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/mcts/node.py` & `aizynthfinder-3.7.0/aizynthfinder/search/mcts/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 """ Module containing a class that represents a node in the search tree.
 """
 from __future__ import annotations
-from typing import TYPE_CHECKING
+
 import random
+from typing import TYPE_CHECKING
 
 import numpy as np
 
-from aizynthfinder.chem import TreeMolecule
+from aizynthfinder.chem import TreeMolecule, deserialize_action, serialize_action
 from aizynthfinder.search.mcts.state import MctsState
 from aizynthfinder.search.mcts.utils import ReactionTreeFromSuperNode, route_to_node
-from aizynthfinder.utils.logging import logger
 from aizynthfinder.utils.exceptions import (
     NodeUnexpectedBehaviourException,
     RejectionException,
 )
-from aizynthfinder.chem import serialize_action, deserialize_action
+from aizynthfinder.utils.logging import logger
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import StrDict, List, Optional, Tuple
     from aizynthfinder.chem import (
         MoleculeDeserializer,
         MoleculeSerializer,
+        RetroReaction,
     )
     from aizynthfinder.context.config import Configuration
-    from aizynthfinder.search.mcts.search import MctsSearchTree
-    from aizynthfinder.chem import RetroReaction
     from aizynthfinder.reactiontree import ReactionTree
+    from aizynthfinder.search.mcts.search import MctsSearchTree
+    from aizynthfinder.utils.type_utils import List, Optional, StrDict, Tuple
 
 
 class MctsNode:
     """
     A node in the search tree.
 
     The children are instantiated lazily for efficiency: only when
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/mcts/search.py` & `aizynthfinder-3.7.0/aizynthfinder/search/mcts/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """ Module containing a class that holds the tree search
 """
 from __future__ import annotations
+
 import json
 from typing import TYPE_CHECKING
 
 import networkx as nx
 
+from aizynthfinder.chem import MoleculeDeserializer, MoleculeSerializer
 from aizynthfinder.search.mcts.node import MctsNode
-from aizynthfinder.chem import MoleculeSerializer, MoleculeDeserializer
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import Optional, List
     from aizynthfinder.context.config import Configuration
+    from aizynthfinder.utils.type_utils import List, Optional
 
 
 class MctsSearchTree:
     """
     Encapsulation of the search tree.
 
     :ivar root: the root node
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/mcts/state.py` & `aizynthfinder-3.7.0/aizynthfinder/search/mcts/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 """ Module contain a class that encapsulate the state of search tree node.
 """
 from __future__ import annotations
+
 import os
 from typing import TYPE_CHECKING
 
 import numpy as np
 from rdkit.Chem import Draw
 
 from aizynthfinder.chem import TreeMolecule
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import StrDict, Any, List, Optional, Sequence
-    from aizynthfinder.chem import (
-        MoleculeDeserializer,
-        MoleculeSerializer,
-    )
+    from aizynthfinder.chem import MoleculeDeserializer, MoleculeSerializer
     from aizynthfinder.context.config import Configuration
+    from aizynthfinder.utils.type_utils import Any, List, Optional, Sequence, StrDict
 
 os.environ["PYTHONHASHSEED"] = "42"
 
 
 class MctsState:
     """
     Encapsulation of the molecular state of a node.
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/mcts/utils.py` & `aizynthfinder-3.7.0/aizynthfinder/search/mcts/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """ Module containing utility routines for MCTS. This is not part of public interface """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 from aizynthfinder.reactiontree import ReactionTreeLoader
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import Tuple, List, Optional
-    from aizynthfinder.search.mcts import MctsNode
     from aizynthfinder.chem import RetroReaction
+    from aizynthfinder.search.mcts import MctsNode
+    from aizynthfinder.utils.type_utils import List, Optional, Tuple
 
 
 class ReactionTreeFromSuperNode(ReactionTreeLoader):
     """
     Creates a reaction tree object from MCTS-like nodes and reaction objects
     """
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/retrostar/cost.py` & `aizynthfinder-3.7.0/aizynthfinder/search/retrostar/cost.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """ Module containing Retro* cost model """
 from __future__ import annotations
-from typing import TYPE_CHECKING
+
 import pickle
+from typing import TYPE_CHECKING
 
 import numpy as np
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import Tuple, List
     from aizynthfinder.chem import Molecule
+    from aizynthfinder.utils.type_utils import List, Tuple
 
 
 class RetroStarCost:
     """
     Encapsulation of a the original Retro* molecular cost model
 
     Numpy implementation of original pytorch model
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/retrostar/nodes.py` & `aizynthfinder-3.7.0/aizynthfinder/search/retrostar/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 """ Module containing a classes representation various tree nodes
 """
 from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from aizynthfinder.chem import TreeMolecule
-from aizynthfinder.search.andor_trees import TreeNodeMixin
 from aizynthfinder.chem.serialization import deserialize_action, serialize_action
+from aizynthfinder.search.andor_trees import TreeNodeMixin
 
 if TYPE_CHECKING:
-    from aizynthfinder.context.config import Configuration
+    from aizynthfinder.chem import RetroReaction
     from aizynthfinder.chem.serialization import (
         MoleculeDeserializer,
         MoleculeSerializer,
     )
-    from aizynthfinder.utils.type_utils import (
-        StrDict,
-        Sequence,
-        Set,
-        List,
-    )
-    from aizynthfinder.chem import RetroReaction
+    from aizynthfinder.context.config import Configuration
+    from aizynthfinder.utils.type_utils import List, Sequence, Set, StrDict
 
 
 class MoleculeNode(TreeNodeMixin):
     """
     An OR node representing a molecule
 
     :ivar cost: the cost of synthesizing the molecule
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/search/retrostar/search_tree.py` & `aizynthfinder-3.7.0/aizynthfinder/search/retrostar/search_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """ Module containing a class that holds the tree search
 """
 from __future__ import annotations
+
 import json
 from typing import TYPE_CHECKING
 
 import numpy as np
 
-from aizynthfinder.search.retrostar.nodes import MoleculeNode
-from aizynthfinder.utils.logging import logger
-from aizynthfinder.search.andor_trees import AndOrSearchTreeBase, SplitAndOrTree
 from aizynthfinder.chem.serialization import MoleculeDeserializer, MoleculeSerializer
+from aizynthfinder.search.andor_trees import AndOrSearchTreeBase, SplitAndOrTree
+from aizynthfinder.search.retrostar.nodes import MoleculeNode
 from aizynthfinder.utils.exceptions import RejectionException
+from aizynthfinder.utils.logging import logger
 
 if TYPE_CHECKING:
+    from aizynthfinder.chem import RetroReaction
     from aizynthfinder.context.config import Configuration
     from aizynthfinder.reactiontree import ReactionTree
-    from aizynthfinder.chem import RetroReaction
-    from aizynthfinder.utils.type_utils import Optional, Sequence, List
+    from aizynthfinder.utils.type_utils import List, Optional, Sequence
 
 
 class SearchTree(AndOrSearchTreeBase):
     """
     Encapsulation of the Retro* search tree (an AND/OR tree).
 
     :ivar config: settings of the tree search algorithm
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/tools/cat_output.py` & `aizynthfinder-3.7.0/aizynthfinder/tools/cat_output.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/tools/make_stock.py` & `aizynthfinder-3.7.0/aizynthfinder/tools/make_stock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """ Module containing classes and routines for making stock input to the tree search.
 """
 from __future__ import annotations
+
 import argparse
 import importlib
 from typing import TYPE_CHECKING
 
 import pandas as pd
 
 from aizynthfinder.chem import Molecule, MoleculeException
 from aizynthfinder.context.stock import MongoDbInchiKeyQuery
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import List, Iterable
+    from aizynthfinder.utils.type_utils import Iterable, List
 
     _StrIterator = Iterable[str]
 
 
 def _get_arguments() -> argparse.Namespace:
     parser = argparse.ArgumentParser("smiles2stock")
     parser.add_argument(
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/training/keras_models.py` & `aizynthfinder-3.7.0/aizynthfinder/training/keras_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 """ Module containing classes and routines used in training of policies.
 """
 from __future__ import annotations
+
+import functools
 import os
 from typing import TYPE_CHECKING
 
 import numpy as np
-
-# pylint: disable=all
-from tensorflow.keras.layers import Dense, Dropout, Input, Dot
-from tensorflow.keras.models import Sequential, Model
-from tensorflow.keras.optimizers import Adam
-from tensorflow.keras.utils import Sequence
+from tensorflow.keras import regularizers
 from tensorflow.keras.callbacks import (
-    EarlyStopping,
     CSVLogger,
+    EarlyStopping,
     ModelCheckpoint,
     ReduceLROnPlateau,
 )
-from tensorflow.keras import regularizers
+
+# pylint: disable=all
+from tensorflow.keras.layers import Dense, Dot, Dropout, Input
+from tensorflow.keras.metrics import top_k_categorical_accuracy
+from tensorflow.keras.models import Model, Sequential
+from tensorflow.keras.optimizers import Adam
+from tensorflow.keras.utils import Sequence
 
 # pylint: enable=all
 try:
-    from sklearn.utils import shuffle
     from scipy import sparse
+    from sklearn.utils import shuffle
 except ImportError:
     raise ImportError(
         "Training is not supported by this installation."
         " Please install aizynthfinder with extras dependencies."
     )
 
-from aizynthfinder.utils.models import top10_acc, top50_acc
-
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import Tuple, List, Any
     from aizynthfinder.training.utils import Config
+    from aizynthfinder.utils.type_utils import Any, List, Tuple
+
+
+top10_acc = functools.partial(top_k_categorical_accuracy, k=10)
+top10_acc.__name__ = "top10_acc"  # type: ignore
+
+top50_acc = functools.partial(top_k_categorical_accuracy, k=50)
+top50_acc.__name__ = "top50_acc"  # type: ignore
 
 
 class _InMemorySequence(Sequence):  # pylint: disable=W0223
     def __init__(self, config: Config, dataset_label: str) -> None:
         self.batch_size = config["batch_size"]
         input_filename = config.filename(dataset_label + "_inputs")
         label_filename = config.filename(dataset_label + "_labels")
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/training/make_false_products.py` & `aizynthfinder-3.7.0/aizynthfinder/training/make_false_products.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """ Module routines for creating negative data for the training for filter policies
 """
 from __future__ import annotations
-import random
+
 import argparse
+import random
 from typing import TYPE_CHECKING
 
 import pandas as pd
 import tqdm
 
+# pylint: disable=all
+from tensorflow.keras.models import load_model as load_keras_model
+
+# pylint: enable=all
 import aizynthfinder.utils.logging  # pylint: disable=unused-import
-from aizynthfinder.chem import Molecule, Reaction, MoleculeException
+from aizynthfinder.chem import Molecule, MoleculeException, Reaction
 from aizynthfinder.training.utils import (
     Config,
     create_reactants_molecules,
-    reverse_template,
-    reaction_hash,
     reactants_to_fingerprint,
+    reaction_hash,
+    reverse_template,
     split_reaction_smiles,
 )
-from aizynthfinder.utils.models import CUSTOM_OBJECTS, load_keras_model
 
 if TYPE_CHECKING:
     from aizynthfinder.utils.type_utils import (
-        Iterable,
-        Optional,
-        Tuple,
         Any,
         Callable,
+        Iterable,
         List,
+        Optional,
         Sequence,
+        Tuple,
     )
 
     _DfGenerator = Iterable[Optional[pd.DataFrame]]
 
 
 class _ReactionException(Exception):
     pass
@@ -63,17 +67,15 @@
     to each row of reactants in the library in order to make new, false reactions.
 
     :param library: the reaction library
     :param config: the configuration
     :yield: a new DataFrame with a false reaction for each row if a match could be found, otherwise None
     """
 
-    model = load_keras_model(
-        config["negative_data"]["recommender_model"], custom_objects=CUSTOM_OBJECTS
-    )
+    model = load_keras_model(config["negative_data"]["recommender_model"])
     topn = config["negative_data"]["recommender_topn"]
 
     def prediction_sampler(row):
         fingerprint = reactants_to_fingerprint(
             [row[config["column_map"]["reactants"]]], config
         )
         fingerprint = fingerprint.reshape([1, config["fingerprint_len"]])
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/training/preprocess_expansion.py` & `aizynthfinder-3.7.0/aizynthfinder/training/preprocess_expansion.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/training/preprocess_filter.py` & `aizynthfinder-3.7.0/aizynthfinder/training/preprocess_filter.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/training/preprocess_recommender.py` & `aizynthfinder-3.7.0/aizynthfinder/training/preprocess_recommender.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/training/training.py` & `aizynthfinder-3.7.0/aizynthfinder/training/training.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/training/utils.py` & `aizynthfinder-3.7.0/aizynthfinder/training/utils.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/utils/exceptions.py` & `aizynthfinder-3.7.0/aizynthfinder/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `aizynthfinder-3.6.0/aizynthfinder/utils/files.py` & `aizynthfinder-3.7.0/aizynthfinder/utils/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Module containing routines to work with files and processes."""
 from __future__ import annotations
-import tempfile
+
+import gzip
+import json
 import subprocess
+import tempfile
 import time
 import warnings
-import json
-import gzip
 from pathlib import Path
 from typing import TYPE_CHECKING
 
-from deprecated import deprecated
-import more_itertools
 import pandas as pd
+from deprecated import deprecated
 
 from aizynthfinder.utils.logging import logger
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import List, Sequence, Any, Callable, Union
+    from aizynthfinder.utils.type_utils import Any, Callable, List, Sequence, Union
 
 
 def read_datafile(filename: Union[str, Path]) -> pd.DataFrame:
     """
     Read aizynth output from disc in either .hdf5 or .json format
 
     :param filename: the path to the data
@@ -82,15 +82,15 @@
     for filename in input_files[1:]:
         new_data = read_datafile(filename)
         if trees_name:
             trees.extend(new_data["trees"].values)
             new_data = new_data[columns]
         data = pd.concat([data, new_data])
 
-    save_datafile(data.reset_index(), output_name)
+    save_datafile(data.reset_index(drop=True), output_name)
     if trees_name:
         if not trees_name.endswith(".gz"):
             trees_name += ".gz"
         with gzip.open(trees_name, "wt", encoding="UTF-8") as fileobj:
             json.dump(trees, fileobj)
 
 
@@ -102,18 +102,22 @@
     :param nparts: the number of parts to create
     :return: list of filenames of the parts
     """
     with open(filename, "r") as fileobj:
         lines = fileobj.read().splitlines()
 
     filenames = []
-    for chunk in more_itertools.divide(nparts, lines):
+    batch_size, remainder = divmod(len(lines), nparts)
+    stop = 0
+    for part in range(1, nparts + 1):
+        start = stop
+        stop += batch_size + 1 if part <= remainder else batch_size
         filenames.append(tempfile.mktemp())
         with open(filenames[-1], "w") as fileobj:
-            fileobj.write("\n".join(chunk))
+            fileobj.write("\n".join(lines[start:stop]))
     return filenames
 
 
 def start_processes(
     inputs: Sequence[Any], log_prefix: str, cmd_callback: Callable, poll_freq: int = 5
 ) -> None:
     """
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/utils/image.py` & `aizynthfinder-3.7.0/aizynthfinder/utils/image.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 """ This module contains a collection of routines to produce pretty images
 """
 from __future__ import annotations
-import sys
+
+import atexit
 import io
-import subprocess
 import os
-import tempfile
-import atexit
 import shutil
+import subprocess
+import sys
+import tempfile
 from typing import TYPE_CHECKING
 
 from jinja2 import Template
 from PIL import Image, ImageDraw
-from rdkit.Chem import Draw
 from rdkit import Chem
+from rdkit.Chem import Draw
 
 from aizynthfinder.chem import Molecule
 from aizynthfinder.utils.paths import data_path
 
 if TYPE_CHECKING:
     import networkx as nx
 
+    from aizynthfinder.chem import FixedRetroReaction, RetroReaction, UniqueMolecule
+
     # pylint: disable=ungrouped-imports
     from aizynthfinder.utils.type_utils import (
-        Tuple,
         Any,
         Dict,
-        Union,
-        Sequence,
-        PilImage,
-        PilColor,
-        List,
         FrameColors,
+        List,
+        PilColor,
+        PilImage,
+        Sequence,
         StrDict,
-    )
-    from aizynthfinder.chem import (
-        UniqueMolecule,
-        RetroReaction,
-        FixedRetroReaction,
+        Tuple,
+        Union,
     )
 
 IMAGE_FOLDER = tempfile.mkdtemp()
 
 
 @atexit.register
 def _clean_up_images() -> None:
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/utils/loading.py` & `aizynthfinder-3.7.0/aizynthfinder/utils/loading.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """ Module containing routine to dynamically load a class from a specification """
 from __future__ import annotations
+
 import importlib
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from typing import Any
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/utils/logging.py` & `aizynthfinder-3.7.0/aizynthfinder/utils/logging.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,22 +11,14 @@
     import sklearn  # noqa
 except ImportError:
     pass
 from rdkit import RDLogger
 
 from aizynthfinder.utils.paths import data_path
 
-# Suppress tensforflow logging
-os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
-
-import tensorflow  # noqa
-
-tf_logger = tensorflow.get_logger()
-tf_logger.setLevel(logging.WARNING)
-
 # Suppress RDKit errors due to incomplete template (e.g. aromatic non-ring atoms)
 rd_logger = RDLogger.logger()
 rd_logger.setLevel(RDLogger.CRITICAL)
 
 
 def logger() -> logging.Logger:
     """
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/utils/models.py` & `aizynthfinder-3.7.0/aizynthfinder/utils/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,77 +1,87 @@
-""" Module containing helper routines for using Keras and Tensorflow models
+""" Module containing helper routines for using Keras, Tensorflow and Onnx models
 """
 from __future__ import annotations
+
 import functools
+import logging
 import os
 from typing import TYPE_CHECKING
 
 import numpy as np
+import onnxruntime
+import psutil
 import requests
-import tensorflow as tf
 
 try:
     import grpc
+    import tensorflow as tf
     from google.protobuf.json_format import MessageToDict
+
+    # pylint: disable=all
+    from tensorflow.keras.metrics import top_k_categorical_accuracy
+    from tensorflow.keras.models import load_model as load_keras_model
     from tensorflow_serving.apis import (
-        predict_pb2,
         get_model_metadata_pb2,
+        predict_pb2,
         prediction_service_pb2_grpc,
     )
 except ImportError:
     SUPPORT_EXTERNAL_APIS = False
 else:
     SUPPORT_EXTERNAL_APIS = True
 
-# pylint: disable=all
-from tensorflow.keras.metrics import top_k_categorical_accuracy
-from tensorflow.keras.models import load_model as load_keras_model
+
+from aizynthfinder.utils.exceptions import ExternalModelAPIError
 
 # pylint: enable=all
 from aizynthfinder.utils.logging import logger
-from aizynthfinder.utils.exceptions import ExternalModelAPIError
 
 if TYPE_CHECKING:
-    from aizynthfinder.utils.type_utils import Any, Union, Callable, List
+    from aizynthfinder.utils.type_utils import Any, Callable, List, Union
 
     _ModelInput = Union[np.ndarray, List[np.ndarray]]
 
-
-top10_acc = functools.partial(top_k_categorical_accuracy, k=10)
-top10_acc.__name__ = "top10_acc"  # type: ignore
-
-top50_acc = functools.partial(top_k_categorical_accuracy, k=50)
-top50_acc.__name__ = "top50_acc"  # type: ignore
-
-CUSTOM_OBJECTS = {"top10_acc": top10_acc, "top50_acc": top50_acc, "tf": tf}
-
 _logger = logger()
 
+# Suppress tensforflow logging
+os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
+
 TF_SERVING_HOST = os.environ.get("TF_SERVING_HOST")
 TF_SERVING_REST_PORT = os.environ.get("TF_SERVING_REST_PORT")
 TF_SERVING_GRPC_PORT = os.environ.get("TF_SERVING_GRPC_PORT")
 
 
 def load_model(
     source: str, key: str, use_remote_models: bool
-) -> Union["LocalKerasModel", "ExternalModelViaGRPC", "ExternalModelViaREST"]:
+) -> Union[
+    "LocalKerasModel", "LocalOnnxModel", "ExternalModelViaGRPC", "ExternalModelViaREST"
+]:
     """
     Load model from a configuration specification.
 
     If `use_remote_models` is True, tries to load:
       1. A Tensorflow server through gRPC
       2. A Tensorflow server through REST API
-      3. A local model
-    otherwise it just loads the local model
+      3. A local Keras model
+    otherwise it just loads the local model.
 
     :param source: if fallbacks to a local model, this is the filename
-    :param key: when connecting to Tensrflow server this is the model name
+    :param key: when connecting to Tensorflow server this is the model name
     :param use_remote_models: if True will try to connect to remote model server
     :return: a model object with a predict object
     """
+    if source.split(".")[-1] == "onnx":
+        return LocalOnnxModel(source)
+
+    if not SUPPORT_EXTERNAL_APIS:
+        raise ValueError(
+            "Tensorflow is not installed - this installation only supports ONNX models"
+        )
+
     if not use_remote_models:
         return LocalKerasModel(source)
 
     try:
         return ExternalModelViaGRPC(key)
     except ExternalModelAPIError:
         pass
@@ -91,15 +101,24 @@
     :ivar model: the compiled model
     :ivar output_size: the length of the output vector
 
     :param filename: the path to a Keras checkpoint file
     """
 
     def __init__(self, filename: str) -> None:
-        self.model = load_keras_model(filename, custom_objects=CUSTOM_OBJECTS)
+        top10_acc = functools.partial(top_k_categorical_accuracy, k=10)
+        top10_acc.__name__ = "top10_acc"  # type: ignore
+
+        top50_acc = functools.partial(top_k_categorical_accuracy, k=50)
+        top50_acc.__name__ = "top50_acc"  # type: ignore
+
+        self.model = load_keras_model(
+            filename,
+            custom_objects={"top10_acc": top10_acc, "top50_acc": top50_acc, "tf": tf},
+        )
         try:
             self._model_dimensions = int(self.model.input.shape[1])
         except AttributeError:
             self._model_dimensions = int(self.model.input[0].shape[1])
         self.output_size = int(self.model.output.shape[1])
 
     def __len__(self) -> int:
@@ -111,14 +130,57 @@
 
         :param args: the input vectors
         :return: the vector of the output layer
         """
         return self.model.predict(args, verbose=0)
 
 
+class LocalOnnxModel:
+    """
+    An Onnx model that is executed locally.
+
+    The size of the input vector can be determined with the len() method.
+
+    :ivar model: the compiled Onnx model
+    :ivar output_size: the length of the output vector
+
+    :param filename: the path to a Onnx model checkpoint file
+    """
+
+    def __init__(self, filename: str) -> None:
+        session_options = onnxruntime.SessionOptions()
+        session_options.intra_op_num_threads = _get_thread_count_per_core()
+
+        self.model = onnxruntime.InferenceSession(
+            filename, sess_options=session_options
+        )
+        self._model_inputs = self.model.get_inputs()
+        self._model_output = self.model.get_outputs()[0]
+        self._model_dimensions = int(self._model_inputs[0].shape[1])
+        self.output_size = int(self._model_output.shape[1])
+
+    def __len__(self) -> int:
+        return self._model_dimensions
+
+    def predict(self, *args: np.ndarray, **_: np.ndarray) -> np.ndarray:
+        """
+        Perform a prediction run on the onnx model.
+
+        :param args: the input vectors
+        :return: the vector of the output layer
+        """
+        return self.model.run(
+            [self._model_output.name],
+            {
+                model_input.name: input.astype(np.float32)
+                for model_input, input in zip(self._model_inputs, list(args))
+            },
+        )[0]
+
+
 def _log_and_reraise_exceptions(method: Callable) -> Callable:
     @functools.wraps(method)
     def wrapper(*args, **kwargs):
         try:
             return method(*args, **kwargs)
         except Exception as err:
             msg = "Error when requesting from tensorflow model API"
@@ -279,7 +341,11 @@
         if not TF_SERVING_HOST:
             _logger.warning(warning)
             raise ExternalModelAPIError(f"Host not set for model {name}")
         if not TF_SERVING_GRPC_PORT:
             _logger.warning(warning)
             raise ExternalModelAPIError(f"GRPC port not set for model {name}")
         return f"{TF_SERVING_HOST}:{TF_SERVING_GRPC_PORT}"
+
+
+def _get_thread_count_per_core() -> int:
+    return psutil.cpu_count() // psutil.cpu_count(logical=False)
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/utils/mongo.py` & `aizynthfinder-3.7.0/aizynthfinder/utils/mongo.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """ Module containing routines to obtain a MongoClient instance
 """
-from urllib.parse import urlencode
 from typing import Optional
+from urllib.parse import urlencode
 
 try:
     from pymongo import MongoClient
 except ImportError:
     MongoClient = None
     HAS_PYMONGO = False
 else:
```

### Comparing `aizynthfinder-3.6.0/aizynthfinder/utils/type_utils.py` & `aizynthfinder-3.7.0/aizynthfinder/utils/type_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,17 @@
 """ Module containing all types and type imports
 """
 # pylint: disable=unused-import
-from typing import (
-    Any,
-    Callable,  # noqa
-    Dict,
-    List,  # noqa
-    Iterable,  # noqa
-    Optional,
-    Sequence,  # noqa
-    Set,  # noqa
-    Tuple,
-    TypeVar,  # noqa
-    Union,
-)
+from typing import Callable  # noqa
+from typing import Iterable  # noqa
+from typing import List  # noqa
+from typing import Sequence  # noqa
+from typing import Set  # noqa
+from typing import TypeVar  # noqa
+from typing import Any, Dict, Optional, Tuple, Union
 
 from PIL.Image import Image
 from rdkit import Chem
 from rdkit.DataStructs.cDataStructs import ExplicitBitVect
 
 StrDict = Dict[str, Any]
 RdMol = Chem.rdchem.Mol
```

### Comparing `aizynthfinder-3.6.0/pyproject.toml` & `aizynthfinder-3.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 [tool.poetry]
 name = "aizynthfinder"
-version = "3.6.0"
+version = "3.7.0"
 description = "Retrosynthetic route finding using neural network guided Monte-Carlo tree search"
 authors = ["Molecular AI group <samuel.genheden@astrazeneca.com>"]
 license = "MIT"
 include = ["aizynthfinder/data/*.yml", "aizynthfinder/data/templates/*"]
 readme = "README.md"
 homepage = "https://github.com/MolecularAI/aizynthfinder/"
 repository = "https://github.com/MolecularAI/aizynthfinder/"
 documentation = "https://molecularai.github.io/aizynthfinder/"
 
 [tool.pytest.ini_options]
 mccabe-complexity = 9
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length = 120
-max-args = 6
+max-args = 7
 max-attributes = 20
 min-public-methods = 0
 disable = "W3101, R0022, W1201, W1203, R0401, W0707, W0221, W0603, R0801, R1735, W1514, C0209, W0237, R1732, W0602, R0914, typecheck"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.10"
 ipywidgets = "^7.5.1"
 jinja2 = "^3.0.0"
 jupyter = "^1.0.0"
 jupytext = "^1.3.3"
 networkx = "^2.4"
-more-itertools = "^8.2.0"
 deprecated = "^1.2.10"
 pandas = "^1.0.0"
 pillow = "^9.0.0"
 requests = "^2.23.0"
 rdchiral = "^1.0.0"
 rdkit = "^2022.3.3"
 tables = "^3.6.1"
-tensorflow = "^2.8.0"
 tqdm = "^4.42.1"
+onnxruntime = "^1.14.0"
+tensorflow = {version = "^2.8.0", optional=true}
 grpcio = {version = "^1.24.0", optional=true}
 tensorflow-serving-api = {version = "^2.1.0", optional=true}
 pymongo = {version = "^3.10.1", optional=true}
 route-distances = {version = "^1.1.0", optional=true}
 scipy = {version = "^1.0", optional=true}
 matplotlib = {version = "^3.0.0", optional=true}
 timeout-decorator = {version = "^0.5.0", optional=true}
@@ -51,19 +51,20 @@
 pytest = "^6.2.2"
 pytest-black = "^0.3.12"
 pytest-cov = "^2.11.0"
 pytest-datadir = "^1.3.1"
 pytest-mock = "^3.5.0"
 pytest-mccabe = "^2.0.0"
 sphinx = "^4.0.0"
-mypy = "^0.800"
-pylint = "^2.7.0"
+mypy = "^1.0.0"
+pylint = "^2.16.0"
 
 [tool.poetry.extras]
-all = ["grpcio", "tensorflow-serving-api", "pymongo", "route-distances", "scipy", "matplotlib", "timeout-decorator"]
+all = ["pymongo", "route-distances", "scipy", "matplotlib", "timeout-decorator"]
+tf = ["tensorflow", "grpcio", "tensorflow-serving-api"]
 
 [tool.poetry.scripts]
 aizynthapp = "aizynthfinder.interfaces.aizynthapp:main"
 aizynthcli = "aizynthfinder.interfaces.aizynthcli:main"
 cat_aizynth_output = "aizynthfinder.tools.cat_output:main"
 download_public_data = "aizynthfinder.tools.download_public_data:main"
 smiles2stock = "aizynthfinder.tools.make_stock:main"
```

### Comparing `aizynthfinder-3.6.0/setup.py` & `aizynthfinder-3.7.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,80 +1,183 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: aizynthfinder
+Version: 3.7.0
+Summary: Retrosynthetic route finding using neural network guided Monte-Carlo tree search
+Home-page: https://github.com/MolecularAI/aizynthfinder/
+License: MIT
+Author: Molecular AI group
+Author-email: samuel.genheden@astrazeneca.com
+Requires-Python: >=3.8,<3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: all
+Provides-Extra: tf
+Requires-Dist: deprecated (>=1.2.10,<2.0.0)
+Requires-Dist: grpcio (>=1.24.0,<2.0.0) ; extra == "tf"
+Requires-Dist: ipywidgets (>=7.5.1,<8.0.0)
+Requires-Dist: jinja2 (>=3.0.0,<4.0.0)
+Requires-Dist: jupyter (>=1.0.0,<2.0.0)
+Requires-Dist: jupytext (>=1.3.3,<2.0.0)
+Requires-Dist: matplotlib (>=3.0.0,<4.0.0) ; extra == "all"
+Requires-Dist: networkx (>=2.4,<3.0)
+Requires-Dist: onnxruntime (>=1.14.0,<2.0.0)
+Requires-Dist: pandas (>=1.0.0,<2.0.0)
+Requires-Dist: pillow (>=9.0.0,<10.0.0)
+Requires-Dist: pymongo (>=3.10.1,<4.0.0) ; extra == "all"
+Requires-Dist: rdchiral (>=1.0.0,<2.0.0)
+Requires-Dist: rdkit (>=2022.3.3,<2023.0.0)
+Requires-Dist: requests (>=2.23.0,<3.0.0)
+Requires-Dist: route-distances (>=1.1.0,<2.0.0) ; extra == "all"
+Requires-Dist: scipy (>=1.0,<2.0) ; extra == "all"
+Requires-Dist: tables (>=3.6.1,<4.0.0)
+Requires-Dist: tensorflow (>=2.8.0,<3.0.0) ; extra == "tf"
+Requires-Dist: tensorflow-serving-api (>=2.1.0,<3.0.0) ; extra == "tf"
+Requires-Dist: timeout-decorator (>=0.5.0,<0.6.0) ; extra == "all"
+Requires-Dist: tqdm (>=4.42.1,<5.0.0)
+Project-URL: Documentation, https://molecularai.github.io/aizynthfinder/
+Project-URL: Repository, https://github.com/MolecularAI/aizynthfinder/
+Description-Content-Type: text/markdown
 
-packages = \
-['aizynthfinder',
- 'aizynthfinder.analysis',
- 'aizynthfinder.chem',
- 'aizynthfinder.context',
- 'aizynthfinder.context.cost',
- 'aizynthfinder.context.policy',
- 'aizynthfinder.context.scoring',
- 'aizynthfinder.context.stock',
- 'aizynthfinder.interfaces',
- 'aizynthfinder.interfaces.gui',
- 'aizynthfinder.search',
- 'aizynthfinder.search.breadth_first',
- 'aizynthfinder.search.dfpn',
- 'aizynthfinder.search.mcts',
- 'aizynthfinder.search.retrostar',
- 'aizynthfinder.tools',
- 'aizynthfinder.training',
- 'aizynthfinder.utils']
-
-package_data = \
-{'': ['*'], 'aizynthfinder': ['data/*', 'data/templates/*']}
-
-install_requires = \
-['deprecated>=1.2.10,<2.0.0',
- 'ipywidgets>=7.5.1,<8.0.0',
- 'jinja2>=3.0.0,<4.0.0',
- 'jupyter>=1.0.0,<2.0.0',
- 'jupytext>=1.3.3,<2.0.0',
- 'more-itertools>=8.2.0,<9.0.0',
- 'networkx>=2.4,<3.0',
- 'pandas>=1.0.0,<2.0.0',
- 'pillow>=9.0.0,<10.0.0',
- 'rdchiral>=1.0.0,<2.0.0',
- 'rdkit>=2022.3.3,<2023.0.0',
- 'requests>=2.23.0,<3.0.0',
- 'tables>=3.6.1,<4.0.0',
- 'tensorflow>=2.8.0,<3.0.0',
- 'tqdm>=4.42.1,<5.0.0']
-
-extras_require = \
-{'all': ['grpcio>=1.24.0,<2.0.0',
-         'tensorflow-serving-api>=2.1.0,<3.0.0',
-         'pymongo>=3.10.1,<4.0.0',
-         'route-distances>=1.1.0,<2.0.0',
-         'scipy>=1.0,<2.0',
-         'matplotlib>=3.0.0,<4.0.0',
-         'timeout-decorator>=0.5.0,<0.6.0']}
-
-entry_points = \
-{'console_scripts': ['aizynthapp = aizynthfinder.interfaces.aizynthapp:main',
-                     'aizynthcli = aizynthfinder.interfaces.aizynthcli:main',
-                     'cat_aizynth_output = aizynthfinder.tools.cat_output:main',
-                     'download_public_data = '
-                     'aizynthfinder.tools.download_public_data:main',
-                     'smiles2stock = aizynthfinder.tools.make_stock:main']}
-
-setup_kwargs = {
-    'name': 'aizynthfinder',
-    'version': '3.6.0',
-    'description': 'Retrosynthetic route finding using neural network guided Monte-Carlo tree search',
-    'long_description': '# AiZynthFinder \n\n[![License](https://img.shields.io/github/license/MolecularAI/aizynthfinder)](https://github.com/MolecularAI/aizynthfinder/blob/master/LICENSE)\n[![Tests](https://github.com/MolecularAI/aizynthfinder/workflows/tests/badge.svg)](https://github.com/MolecularAI/aizynthfinder/actions?workflow=tests)\n[![codecov](https://codecov.io/gh/MolecularAI/aizynthfinder/branch/master/graph/badge.svg)](https://codecov.io/gh/MolecularAI/aizynthfinder)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black) \n[![version](https://img.shields.io/github/v/release/MolecularAI/aizynthfinder)](https://github.com/MolecularAI/aizynthfinder/releases)\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MolecularAI/aizynthfinder/blob/master/contrib/notebook.ipynb)\n\n\nAiZynthFinder is a tool for retrosynthetic planning. The algorithm is based on a Monte Carlo tree search that recursively breaks down a molecule to purchasable precursors. The tree search is guided by a policy that suggests possible precursors by utilizing a neural network trained on a library of known reaction templates.\n\nAn introduction video can be found here: [https://youtu.be/r9Dsxm-mcgA](https://youtu.be/r9Dsxm-mcgA)\n\n## Prerequisites\n\nBefore you begin, ensure you have met the following requirements:\n\n* Linux, Windows or macOS platforms are supported - as long as the dependencies are supported on these platforms.\n\n* You have installed [anaconda](https://www.anaconda.com/) or [miniconda](https://docs.conda.io/en/latest/miniconda.html) with python 3.8 - 3.9\n\nThe tool has been developed on a Linux platform, but the software has been tested on Windows 10 and macOS Catalina.\n\n\n## Installation\n\n### For end-users\n\nFirst time, execute the following command in a console or an Anaconda prompt\n\n    conda create "python>=3.8,<3.10" -n aizynth-env\n    \nTo install, activate the environment and install the package using pypi\n\n    conda activate aizynth-env\n    python -m pip install aizynthfinder[all]\n\nfor a smaller package, without all the functionality, you can also type\n\n    python -m pip install aizynthfinder\n\n### For developers\n\nFirst clone the repository using Git.\n\nThen execute the following commands in the root of the repository \n\n    conda env create -f env-dev.yml\n    conda activate aizynth-dev\n    poetry install -E all\n    \nthe `aizynthfinder` package is now installed in editable mode.\n\n## Usage\n\nThe tool will install the ``aizynthcli`` and ``aizynthapp`` tools\nas interfaces to the algorithm:\n\n```\naizynthcli --config config.yml --smiles smiles.txt\naizynthapp --config config.yml\n```\n\nConsult the documentation [here](https://molecularai.github.io/aizynthfinder/) for more information.\n\nTo use the tool you need\n\n    1. A stock file\n    2. A trained rollout policy network (including the Keras model and the list of unique templates)\n    3. A trained filer policy network (optional)\n\nSuch files can be downloaded from [figshare](https://figshare.com/articles/AiZynthFinder_a_fast_robust_and_flexible_open-source_software_for_retrosynthetic_planning/12334577) and [here](https://figshare.com/articles/dataset/A_quick_policy_to_filter_reactions_based_on_feasibility_in_AI-guided_retrosynthetic_planning/13280507) or they can be downloaded automatically using\n\n```\ndownload_public_data my_folder\n```\n\nwhere ``my_folder`` is the folder that you want download to.\nThis will create a ``config.yml`` file that you can use with either ``aizynthcli`` or ``aizynthapp``.\n\n## Development\n\n### Testing\n\nTests uses the ``pytest`` package, and is installed by `poetry`\n\nRun the tests using:\n\n    pytest -v\n\nThe full command run on the CI server is available through an `invoke` command\n\n    invoke full-tests\n    \n ### Documentation generation\n\nThe documentation is generated by Sphinx from hand-written tutorials and docstrings\n\nThe HTML documentation can be generated by\n\n    invoke build-docs\n\n## Contributing\n\nWe welcome contributions, in the form of issues or pull requests.\n\nIf you have a question or want to report a bug, please submit an issue.\n\n\nTo contribute with code to the project, follow these steps:\n\n1. Fork this repository.\n2. Create a branch: `git checkout -b <branch_name>`.\n3. Make your changes and commit them: `git commit -m \'<commit_message>\'`\n4. Push to the remote branch: `git push`\n5. Create the pull request.\n\nPlease use ``black`` package for formatting, and follow ``pep8`` style guide.\n\n\n## Contributors\n\n* [@SGenheden](https://www.github.com/SGenheden)\n* [@EBjerrum](https://www.github.com/EBjerrum)\n* [@A-Thakkar](https://www.github.com/A-Thakkar)\n* [@benteb](https://www.github.com/benteb)\n\nThe contributors have limited time for support questions, but please do not hesitate to submit an issue (see above).\n\n## License\n\nThe software is licensed under the MIT license (see LICENSE file), and is free and provided as-is.\n\n## References\n\n1. Thakkar A, Kogej T, Reymond J-L, et al (2019) Datasets and their influence on the development of computer assisted synthesis planning tools in the pharmaceutical domain. Chem Sci. https://doi.org/10.1039/C9SC04944D\n2. Genheden S, Thakkar A, Chadimova V, et al (2020) AiZynthFinder: a fast, robust and flexible open-source software for retrosynthetic planning. J. Cheminf. https://jcheminf.biomedcentral.com/articles/10.1186/s13321-020-00472-1\n3. Genheden S, Engkvist O, Bjerrum E (2020) A Quick Policy to Filter Reactions Based on Feasibility in AI-Guided Retrosynthetic Planning. ChemRxiv. Preprint. https://doi.org/10.26434/chemrxiv.13280495.v1 \n4. Genheden S, Engkvist O, Bjerrum E (2021) Clustering of synthetic routes using tree edit distance. J. Chem. Inf. Model. 61:3899–3907 [https://doi.org/10.1021/acs.jcim.1c00232](https://doi.org/10.1021/acs.jcim.1c00232)\n5. Genheden S, Engkvist O, Bjerrum E (2022) Fast prediction of distances between synthetic routes with deep learning. Mach. Learn. Sci. Technol. 3:015018 [https://doi.org/10.1088/2632-2153/ac4a91](https://doi.org/10.1088/2632-2153/ac4a91) \n',
-    'author': 'Molecular AI group',
-    'author_email': 'samuel.genheden@astrazeneca.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/MolecularAI/aizynthfinder/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<3.10',
-}
+# AiZynthFinder 
 
+[![License](https://img.shields.io/github/license/MolecularAI/aizynthfinder)](https://github.com/MolecularAI/aizynthfinder/blob/master/LICENSE)
+[![Tests](https://github.com/MolecularAI/aizynthfinder/workflows/tests/badge.svg)](https://github.com/MolecularAI/aizynthfinder/actions?workflow=tests)
+[![codecov](https://codecov.io/gh/MolecularAI/aizynthfinder/branch/master/graph/badge.svg)](https://codecov.io/gh/MolecularAI/aizynthfinder)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black) 
+[![version](https://img.shields.io/github/v/release/MolecularAI/aizynthfinder)](https://github.com/MolecularAI/aizynthfinder/releases)
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/MolecularAI/aizynthfinder/blob/master/contrib/notebook.ipynb)
+
+
+AiZynthFinder is a tool for retrosynthetic planning. The algorithm is based on a Monte Carlo tree search that recursively breaks down a molecule to purchasable precursors. The tree search is guided by a policy that suggests possible precursors by utilizing a neural network trained on a library of known reaction templates.
+
+An introduction video can be found here: [https://youtu.be/r9Dsxm-mcgA](https://youtu.be/r9Dsxm-mcgA)
+
+## Prerequisites
+
+Before you begin, ensure you have met the following requirements:
+
+* Linux, Windows or macOS platforms are supported - as long as the dependencies are supported on these platforms.
+
+* You have installed [anaconda](https://www.anaconda.com/) or [miniconda](https://docs.conda.io/en/latest/miniconda.html) with python 3.8 - 3.9
+
+The tool has been developed on a Linux platform, but the software has been tested on Windows 10 and macOS Catalina.
+
+
+## Installation
+
+### For end-users
+
+First time, execute the following command in a console or an Anaconda prompt
+
+    conda create "python>=3.8,<3.10" -n aizynth-env
+    
+To install, activate the environment and install the package using pypi
+
+    conda activate aizynth-env
+    python -m pip install aizynthfinder[all]
+
+for a smaller package, without all the functionality, you can also type
+
+    python -m pip install aizynthfinder
+
+### For developers
+
+First clone the repository using Git.
+
+Then execute the following commands in the root of the repository 
+
+    conda env create -f env-dev.yml
+    conda activate aizynth-dev
+    poetry install -E all
+    
+the `aizynthfinder` package is now installed in editable mode.
+
+## Usage
+
+The tool will install the ``aizynthcli`` and ``aizynthapp`` tools
+as interfaces to the algorithm:
+
+```
+aizynthcli --config config.yml --smiles smiles.txt
+aizynthapp --config config.yml
+```
+
+Consult the documentation [here](https://molecularai.github.io/aizynthfinder/) for more information.
+
+To use the tool you need
+
+    1. A stock file
+    2. A trained rollout policy network (including the Keras model and the list of unique templates)
+    3. A trained filer policy network (optional)
+
+Such files can be downloaded from [figshare](https://figshare.com/articles/AiZynthFinder_a_fast_robust_and_flexible_open-source_software_for_retrosynthetic_planning/12334577) and [here](https://figshare.com/articles/dataset/A_quick_policy_to_filter_reactions_based_on_feasibility_in_AI-guided_retrosynthetic_planning/13280507) or they can be downloaded automatically using
+
+```
+download_public_data my_folder
+```
+
+where ``my_folder`` is the folder that you want download to.
+This will create a ``config.yml`` file that you can use with either ``aizynthcli`` or ``aizynthapp``.
+
+## Development
+
+### Testing
+
+Tests uses the ``pytest`` package, and is installed by `poetry`
+
+Run the tests using:
+
+    pytest -v
+
+The full command run on the CI server is available through an `invoke` command
+
+    invoke full-tests
+    
+ ### Documentation generation
+
+The documentation is generated by Sphinx from hand-written tutorials and docstrings
+
+The HTML documentation can be generated by
+
+    invoke build-docs
+
+## Contributing
+
+We welcome contributions, in the form of issues or pull requests.
+
+If you have a question or want to report a bug, please submit an issue.
+
+
+To contribute with code to the project, follow these steps:
+
+1. Fork this repository.
+2. Create a branch: `git checkout -b <branch_name>`.
+3. Make your changes and commit them: `git commit -m '<commit_message>'`
+4. Push to the remote branch: `git push`
+5. Create the pull request.
+
+Please use ``black`` package for formatting, and follow ``pep8`` style guide.
+
+
+## Contributors
+
+* [@SGenheden](https://www.github.com/SGenheden)
+* [@EBjerrum](https://www.github.com/EBjerrum)
+* [@A-Thakkar](https://www.github.com/A-Thakkar)
+* [@benteb](https://www.github.com/benteb)
+
+The contributors have limited time for support questions, but please do not hesitate to submit an issue (see above).
+
+## License
+
+The software is licensed under the MIT license (see LICENSE file), and is free and provided as-is.
+
+## References
+
+1. Thakkar A, Kogej T, Reymond J-L, et al (2019) Datasets and their influence on the development of computer assisted synthesis planning tools in the pharmaceutical domain. Chem Sci. https://doi.org/10.1039/C9SC04944D
+2. Genheden S, Thakkar A, Chadimova V, et al (2020) AiZynthFinder: a fast, robust and flexible open-source software for retrosynthetic planning. J. Cheminf. https://jcheminf.biomedcentral.com/articles/10.1186/s13321-020-00472-1
+3. Genheden S, Engkvist O, Bjerrum E (2020) A Quick Policy to Filter Reactions Based on Feasibility in AI-Guided Retrosynthetic Planning. ChemRxiv. Preprint. https://doi.org/10.26434/chemrxiv.13280495.v1 
+4. Genheden S, Engkvist O, Bjerrum E (2021) Clustering of synthetic routes using tree edit distance. J. Chem. Inf. Model. 61:3899–3907 [https://doi.org/10.1021/acs.jcim.1c00232](https://doi.org/10.1021/acs.jcim.1c00232)
+5. Genheden S, Engkvist O, Bjerrum E (2022) Fast prediction of distances between synthetic routes with deep learning. Mach. Learn. Sci. Technol. 3:015018 [https://doi.org/10.1088/2632-2153/ac4a91](https://doi.org/10.1088/2632-2153/ac4a91) 
 
-setup(**setup_kwargs)
```

