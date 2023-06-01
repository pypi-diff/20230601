# Comparing `tmp/BAMT-1.1.40.tar.gz` & `tmp/bamt-1.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BAMT-1.1.40.tar", max compression
+gzip compressed data, was "bamt-1.1.41.tar", max compression
```

## Comparing `BAMT-1.1.40.tar` & `bamt-1.1.41.tar`

### file list

```diff
@@ -1,162 +1,161 @@
--rw-r--r--   0        0        0        0 2022-10-18 09:46:52.969462 BAMT-1.1.40/bamt/__init__.py
--rw-r--r--   0        0        0    14998 2023-04-10 14:01:43.784052 BAMT-1.1.40/bamt/builders.py
--rw-r--r--   0        0        0      688 2023-04-10 14:01:43.785048 BAMT-1.1.40/bamt/config.py
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.582873 BAMT-1.1.40/bamt/external/__init__.py
--rw-r--r--   0        0        0      154 2023-03-22 08:13:29.970622 BAMT-1.1.40/bamt/external/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      373 2022-12-24 09:53:39.265727 BAMT-1.1.40/bamt/external/libpgm/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0       82 2023-04-10 14:01:43.785048 BAMT-1.1.40/bamt/external/pyBN/__init__.py
--rw-r--r--   0        0        0      238 2023-03-27 20:03:35.633736 BAMT-1.1.40/bamt/external/pyBN/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0        0 2023-04-10 14:01:43.785048 BAMT-1.1.40/bamt/external/pyBN/classes/__init__.py
--rw-r--r--   0        0        0      167 2023-03-27 20:03:35.635733 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    12842 2023-03-27 20:03:35.673859 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/bayesnet.cpython-310.pyc
--rw-r--r--   0        0        0    10770 2023-03-27 08:04:03.587482 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/cliquetree.cpython-310.pyc
--rw-r--r--   0        0        0     4738 2023-03-27 08:04:03.584486 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/clustergraph.cpython-310.pyc
--rw-r--r--   0        0        0     5165 2023-03-27 08:04:03.681327 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/empiricaldistribution.cpython-310.pyc
--rw-r--r--   0        0        0    17971 2023-03-27 08:04:03.593487 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/factor.cpython-310.pyc
--rw-r--r--   0        0        0     4873 2023-03-27 08:04:03.590484 BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/factorization.cpython-310.pyc
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.588854 BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__init__.py
--rw-r--r--   0        0        0      174 2022-12-24 09:53:41.854845 BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5230 2022-12-24 09:53:41.861558 BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__pycache__/test_bayesnet.cpython-310.pyc
--rw-r--r--   0        0        0     6379 2022-12-24 09:53:41.867553 BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__pycache__/test_factor.cpython-310.pyc
--rw-r--r--   0        0        0     5520 2023-04-10 14:01:43.786046 BAMT-1.1.40/bamt/external/pyBN/classes/_tests/test_bayesnet.py
--rw-r--r--   0        0        0    11006 2023-04-10 14:01:43.787042 BAMT-1.1.40/bamt/external/pyBN/classes/bayesnet.py
--rw-r--r--   0        0        0      302 2023-03-27 08:04:03.623486 BAMT-1.1.40/bamt/external/pyBN/classification/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3370 2023-03-27 08:04:03.624483 BAMT-1.1.40/bamt/external/pyBN/classification/__pycache__/classification.cpython-310.pyc
--rw-r--r--   0        0        0     3432 2023-03-27 08:04:03.647079 BAMT-1.1.40/bamt/external/pyBN/classification/__pycache__/feature_selection.cpython-310.pyc
--rw-r--r--   0        0        0      335 2023-03-27 08:04:03.626130 BAMT-1.1.40/bamt/external/pyBN/inference/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      176 2022-12-24 09:53:41.870556 BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1060 2022-12-24 09:53:41.876256 BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_map_exact.cpython-310.pyc
--rw-r--r--   0        0        0     2776 2022-12-24 09:53:41.882205 BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_approx.cpython-310.pyc
--rw-r--r--   0        0        0     2251 2022-12-24 09:53:41.886925 BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_exact.cpython-310.pyc
--rw-r--r--   0        0        0      299 2023-03-27 08:04:03.628136 BAMT-1.1.40/bamt/external/pyBN/inference/map_exact/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2653 2023-03-27 08:04:03.630137 BAMT-1.1.40/bamt/external/pyBN/inference/map_exact/__pycache__/ilp_map.cpython-310.pyc
--rw-r--r--   0        0        0     1077 2023-03-27 08:04:03.631117 BAMT-1.1.40/bamt/external/pyBN/inference/map_exact/__pycache__/ve_map.cpython-310.pyc
--rw-r--r--   0        0        0      461 2023-03-27 08:04:03.632119 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2050 2023-03-27 08:04:03.634118 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/forward_sample.cpython-310.pyc
--rw-r--r--   0        0        0     1553 2023-03-27 08:04:03.639077 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/gibbs_sample.cpython-310.pyc
--rw-r--r--   0        0        0     1783 2023-03-27 08:04:03.641082 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/loopy_bp.cpython-310.pyc
--rw-r--r--   0        0        0     1613 2023-03-27 08:04:03.642078 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/lw_sample.cpython-310.pyc
--rw-r--r--   0        0        0      320 2023-03-27 08:04:03.643078 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_exact/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2054 2023-03-27 08:04:03.645083 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_exact/__pycache__/exact_bp.cpython-310.pyc
--rw-r--r--   0        0        0     1432 2023-03-27 08:04:03.646078 BAMT-1.1.40/bamt/external/pyBN/inference/marginal_exact/__pycache__/ve_marginal.cpython-310.pyc
--rw-r--r--   0        0        0      244 2023-03-27 08:04:03.695089 BAMT-1.1.40/bamt/external/pyBN/io/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5673 2023-03-27 08:04:03.697093 BAMT-1.1.40/bamt/external/pyBN/io/__pycache__/read.cpython-310.pyc
--rw-r--r--   0        0        0     1690 2023-03-27 08:04:03.699093 BAMT-1.1.40/bamt/external/pyBN/io/__pycache__/write.cpython-310.pyc
--rw-r--r--   0        0        0      169 2022-12-24 09:53:41.889932 BAMT-1.1.40/bamt/external/pyBN/io/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1451 2022-12-24 09:53:41.894772 BAMT-1.1.40/bamt/external/pyBN/io/_tests/__pycache__/test_reading.cpython-310.pyc
--rw-r--r--   0        0        0      888 2022-12-24 09:53:41.899461 BAMT-1.1.40/bamt/external/pyBN/io/_tests/__pycache__/test_writing.cpython-310.pyc
--rw-r--r--   0        0        0      271 2023-03-27 08:04:03.649082 BAMT-1.1.40/bamt/external/pyBN/learning/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      291 2023-03-27 08:04:03.650078 BAMT-1.1.40/bamt/external/pyBN/learning/parameter/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3832 2023-03-27 08:04:03.652079 BAMT-1.1.40/bamt/external/pyBN/learning/parameter/__pycache__/bayes.cpython-310.pyc
--rw-r--r--   0        0        0     5978 2023-03-27 08:04:03.654087 BAMT-1.1.40/bamt/external/pyBN/learning/parameter/__pycache__/mle.cpython-310.pyc
--rw-r--r--   0        0        0      185 2022-12-24 09:53:41.900463 BAMT-1.1.40/bamt/external/pyBN/learning/parameter/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      572 2023-03-27 08:04:03.655095 BAMT-1.1.40/bamt/external/pyBN/learning/structure/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3770 2023-03-27 08:04:03.694090 BAMT-1.1.40/bamt/external/pyBN/learning/structure/__pycache__/mdbn.cpython-310.pyc
--rw-r--r--   0        0        0      185 2022-12-24 09:53:41.902496 BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1821 2022-12-24 09:53:41.905088 BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_chow_liu.cpython-310.pyc
--rw-r--r--   0        0        0     2139 2022-12-24 09:53:41.908341 BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_grow_shrink.cpython-310.pyc
--rw-r--r--   0        0        0     1713 2022-12-24 09:53:41.910390 BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_orient_edges.cpython-310.pyc
--rw-r--r--   0        0        0     1744 2022-12-24 09:53:41.915718 BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_pc.cpython-310.pyc
--rw-r--r--   0        0        0      548 2023-03-27 08:04:03.657092 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     4331 2023-03-27 08:04:03.659096 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/fast_iamb.cpython-310.pyc
--rw-r--r--   0        0        0     4034 2023-03-27 08:04:03.660092 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/grow_shrink.cpython-310.pyc
--rw-r--r--   0        0        0     4359 2023-03-27 08:04:03.662095 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/iamb.cpython-310.pyc
--rw-r--r--   0        0        0     2892 2023-03-27 08:04:03.663691 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/lambda_iamb.cpython-310.pyc
--rw-r--r--   0        0        0     3783 2023-03-27 08:04:03.665697 BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/path_condition.cpython-310.pyc
--rw-r--r--   0        0        0      252 2023-03-27 08:04:03.666694 BAMT-1.1.40/bamt/external/pyBN/learning/structure/exact/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     1743 2023-03-27 08:04:03.668693 BAMT-1.1.40/bamt/external/pyBN/learning/structure/exact/__pycache__/gobnilp.cpython-310.pyc
--rw-r--r--   0        0        0      251 2023-03-27 08:04:03.669694 BAMT-1.1.40/bamt/external/pyBN/learning/structure/hybrid/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2480 2023-03-27 08:04:03.671004 BAMT-1.1.40/bamt/external/pyBN/learning/structure/hybrid/__pycache__/mmpc.cpython-310.pyc
--rw-r--r--   0        0        0      315 2023-03-27 08:04:03.672006 BAMT-1.1.40/bamt/external/pyBN/learning/structure/naive/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2312 2023-03-27 08:04:03.674010 BAMT-1.1.40/bamt/external/pyBN/learning/structure/naive/__pycache__/naive_bayes.cpython-310.pyc
--rw-r--r--   0        0        0      870 2023-03-27 08:04:03.675322 BAMT-1.1.40/bamt/external/pyBN/learning/structure/naive/__pycache__/TAN.cpython-310.pyc
--rw-r--r--   0        0        0      524 2023-03-27 08:04:03.676326 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     3803 2023-03-27 08:04:03.678326 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/bayes_scores.cpython-310.pyc
--rw-r--r--   0        0        0     6763 2023-03-27 08:04:03.683330 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/hill_climbing.cpython-310.pyc
--rw-r--r--   0        0        0     5042 2023-03-27 08:04:03.684326 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/info_scores.cpython-310.pyc
--rw-r--r--   0        0        0     6013 2023-03-27 08:04:03.687330 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/random_restarts.cpython-310.pyc
--rw-r--r--   0        0        0     4959 2023-03-27 08:04:03.689330 BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/tabu.cpython-310.pyc
--rw-r--r--   0        0        0      251 2023-03-27 08:04:03.691046 BAMT-1.1.40/bamt/external/pyBN/learning/structure/tree/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2067 2023-03-27 08:04:03.692088 BAMT-1.1.40/bamt/external/pyBN/learning/structure/tree/__pycache__/chow_liu.cpython-310.pyc
--rw-r--r--   0        0        0      217 2022-12-24 09:53:41.922124 BAMT-1.1.40/bamt/external/pyBN/plotting/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2504 2022-12-24 09:53:41.930964 BAMT-1.1.40/bamt/external/pyBN/plotting/__pycache__/plot.cpython-310.pyc
--rw-r--r--   0        0        0      208 2023-04-10 14:01:43.787042 BAMT-1.1.40/bamt/external/pyBN/utils/__init__.py
--rw-r--r--   0        0        0      362 2023-03-27 20:03:35.640736 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      948 2023-03-27 20:03:35.646737 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/class_equivalence.cpython-310.pyc
--rw-r--r--   0        0        0      840 2023-03-27 20:03:35.653137 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/data.cpython-310.pyc
--rw-r--r--   0        0        0     3156 2023-03-27 08:04:03.602487 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/discretize.cpython-310.pyc
--rw-r--r--   0        0        0     1274 2023-03-27 20:03:35.658779 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/graph.cpython-310.pyc
--rw-r--r--   0        0        0      973 2023-03-27 08:04:03.606486 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/hybrid_distance.cpython-310.pyc
--rw-r--r--   0        0        0     4392 2023-03-27 20:03:35.665794 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/independence_tests.cpython-310.pyc
--rw-r--r--   0        0        0     4723 2023-03-27 08:04:03.612483 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/markov_blanket.cpython-310.pyc
--rw-r--r--   0        0        0     4640 2023-03-27 08:04:03.615487 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/orient_edges.cpython-310.pyc
--rw-r--r--   0        0        0     3492 2023-03-27 08:04:03.617486 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/parameter_distance.cpython-310.pyc
--rw-r--r--   0        0        0     1943 2023-03-27 08:04:03.619487 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/random_sample.cpython-310.pyc
--rw-r--r--   0        0        0     2896 2023-03-27 08:04:03.621487 BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/structure_distance.cpython-310.pyc
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.702765 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__init__.py
--rw-r--r--   0        0        0      172 2022-12-24 09:53:42.684367 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2656 2022-12-24 09:53:42.690369 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_independence_tests.cpython-310.pyc
--rw-r--r--   0        0        0     1462 2022-12-24 09:53:42.696862 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_markov_blanket.cpython-310.pyc
--rw-r--r--   0        0        0     1700 2022-12-24 09:53:42.699046 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_orient_edges.cpython-310.pyc
--rw-r--r--   0        0        0     1483 2022-12-24 09:53:42.704515 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_random_sample.cpython-310.pyc
--rw-r--r--   0        0        0     1788 2023-04-10 14:01:43.787042 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_independence_tests.py
--rw-r--r--   0        0        0     1155 2023-04-10 14:01:43.788038 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_markov_blanket.py
--rw-r--r--   0        0        0     1205 2023-04-10 14:01:43.788038 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_orient_edges.py
--rw-r--r--   0        0        0      970 2023-04-10 14:01:43.788038 BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_random_sample.py
--rw-r--r--   0        0        0      907 2023-04-10 14:01:43.789035 BAMT-1.1.40/bamt/external/pyBN/utils/class_equivalence.py
--rw-r--r--   0        0        0      626 2023-04-10 14:01:43.789035 BAMT-1.1.40/bamt/external/pyBN/utils/data.py
--rw-r--r--   0        0        0     1386 2023-04-10 14:01:43.790031 BAMT-1.1.40/bamt/external/pyBN/utils/graph.py
--rw-r--r--   0        0        0     6222 2023-04-10 14:01:43.790031 BAMT-1.1.40/bamt/external/pyBN/utils/independence_tests.py
--rw-r--r--   0        0        0      979 2023-03-17 12:29:52.731831 BAMT-1.1.40/bamt/log.py
--rw-r--r--   0        0        0     1090 2022-08-01 09:44:45.658643 BAMT-1.1.40/bamt/logging.conf
--rw-r--r--   0        0        0    10778 2023-04-10 14:01:43.791028 BAMT-1.1.40/bamt/mi_entropy_gauss.py
--rw-r--r--   0        0        0      119 2023-04-10 14:01:43.791028 BAMT-1.1.40/bamt/networks/__init__.py
--rw-r--r--   0        0        0      229 2023-03-27 20:16:49.956781 BAMT-1.1.40/bamt/networks/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    26367 2023-03-31 13:44:44.700941 BAMT-1.1.40/bamt/networks/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     1115 2023-03-28 14:57:14.478682 BAMT-1.1.40/bamt/networks/__pycache__/hybrid_bn.cpython-310.pyc
--rw-r--r--   0        0        0    31404 2023-04-10 14:01:43.792025 BAMT-1.1.40/bamt/networks/base.py
--rw-r--r--   0        0        0     1704 2023-04-10 14:01:43.792025 BAMT-1.1.40/bamt/networks/big_brave_bn.py
--rw-r--r--   0        0        0      422 2023-04-10 14:01:43.792025 BAMT-1.1.40/bamt/networks/continuous_bn.py
--rw-r--r--   0        0        0      392 2023-04-10 14:01:43.792025 BAMT-1.1.40/bamt/networks/discrete_bn.py
--rw-r--r--   0        0        0      737 2023-04-10 14:01:43.793022 BAMT-1.1.40/bamt/networks/hybrid_bn.py
--rw-r--r--   0        0        0      223 2023-04-10 14:01:43.793022 BAMT-1.1.40/bamt/nodes/__init__.py
--rw-r--r--   0        0        0      324 2023-03-25 11:38:48.177276 BAMT-1.1.40/bamt/nodes/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2653 2023-03-31 13:44:42.957971 BAMT-1.1.40/bamt/nodes/__pycache__/base.cpython-310.pyc
--rw-r--r--   0        0        0     4702 2023-03-27 08:25:39.343392 BAMT-1.1.40/bamt/nodes/__pycache__/conditional_gaussian_node.cpython-310.pyc
--rw-r--r--   0        0        0     4717 2023-03-27 08:25:39.380393 BAMT-1.1.40/bamt/nodes/__pycache__/conditional_logit_node.cpython-310.pyc
--rw-r--r--   0        0        0     5041 2023-03-25 11:38:48.587289 BAMT-1.1.40/bamt/nodes/__pycache__/conditional_mixture_gaussian_node.cpython-310.pyc
--rw-r--r--   0        0        0     4095 2023-03-25 11:38:49.014930 BAMT-1.1.40/bamt/nodes/__pycache__/discrete_node.cpython-310.pyc
--rw-r--r--   0        0        0     3396 2023-03-27 08:25:39.477816 BAMT-1.1.40/bamt/nodes/__pycache__/gaussian_node.cpython-310.pyc
--rw-r--r--   0        0        0     3270 2023-03-27 08:25:39.475813 BAMT-1.1.40/bamt/nodes/__pycache__/logit_node.cpython-310.pyc
--rw-r--r--   0        0        0     3723 2023-03-25 11:38:49.780249 BAMT-1.1.40/bamt/nodes/__pycache__/mixture_gaussian_node.cpython-310.pyc
--rw-r--r--   0        0        0     1796 2023-03-25 11:16:57.986776 BAMT-1.1.40/bamt/nodes/__pycache__/schema.cpython-310.pyc
--rw-r--r--   0        0        0     2685 2023-04-10 14:01:43.793022 BAMT-1.1.40/bamt/nodes/base.py
--rw-r--r--   0        0        0     7951 2023-04-10 14:01:43.793022 BAMT-1.1.40/bamt/nodes/conditional_gaussian_node.py
--rw-r--r--   0        0        0     6920 2023-04-10 14:01:43.794018 BAMT-1.1.40/bamt/nodes/conditional_logit_node.py
--rw-r--r--   0        0        0     8119 2023-04-10 14:01:43.794018 BAMT-1.1.40/bamt/nodes/conditional_mixture_gaussian_node.py
--rw-r--r--   0        0        0     4064 2023-04-10 14:01:43.794018 BAMT-1.1.40/bamt/nodes/discrete_node.py
--rw-r--r--   0        0        0     4424 2023-04-10 14:01:43.795015 BAMT-1.1.40/bamt/nodes/gaussian_node.py
--rw-r--r--   0        0        0     4026 2023-04-10 14:01:43.795015 BAMT-1.1.40/bamt/nodes/logit_node.py
--rw-r--r--   0        0        0     5476 2023-04-10 14:01:43.795015 BAMT-1.1.40/bamt/nodes/mixture_gaussian_node.py
--rw-r--r--   0        0        0     1034 2023-04-10 14:01:43.795015 BAMT-1.1.40/bamt/nodes/schema.py
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.707748 BAMT-1.1.40/bamt/preprocess/__init__.py
--rw-r--r--   0        0        0      156 2023-03-22 08:13:30.026531 BAMT-1.1.40/bamt/preprocess/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     5287 2023-03-22 08:13:30.040531 BAMT-1.1.40/bamt/preprocess/__pycache__/discretization.cpython-310.pyc
--rw-r--r--   0        0        0     1292 2023-03-22 08:13:30.056531 BAMT-1.1.40/bamt/preprocess/__pycache__/graph.cpython-310.pyc
--rw-r--r--   0        0        0     1993 2023-03-22 08:13:30.051545 BAMT-1.1.40/bamt/preprocess/__pycache__/numpy_pandas.cpython-310.pyc
--rw-r--r--   0        0        0     5449 2023-03-17 12:29:52.733830 BAMT-1.1.40/bamt/preprocess/discretization.py
--rw-r--r--   0        0        0      871 2023-03-17 12:29:52.734830 BAMT-1.1.40/bamt/preprocess/graph.py
--rw-r--r--   0        0        0     1904 2023-03-17 12:29:52.734830 BAMT-1.1.40/bamt/preprocess/numpy_pandas.py
--rw-r--r--   0        0        0     4363 2023-03-17 12:29:52.735830 BAMT-1.1.40/bamt/preprocessors.py
--rw-r--r--   0        0        0    12521 2023-04-10 14:01:43.796011 BAMT-1.1.40/bamt/redef_HC.py
--rw-r--r--   0        0        0     6177 2023-04-10 14:01:43.797008 BAMT-1.1.40/bamt/redef_info_scores.py
--rw-r--r--   0        0        0        0 2022-07-18 14:22:44.709741 BAMT-1.1.40/bamt/utils/__init__.py
--rw-r--r--   0        0        0      151 2023-03-22 08:13:30.083531 BAMT-1.1.40/bamt/utils/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     2543 2023-03-27 08:04:04.969879 BAMT-1.1.40/bamt/utils/__pycache__/GraphUtils.cpython-310.pyc
--rw-r--r--   0        0        0     6440 2023-03-22 08:14:15.703888 BAMT-1.1.40/bamt/utils/__pycache__/MathUtils.cpython-310.pyc
--rw-r--r--   0        0        0     2412 2023-04-10 14:01:43.797008 BAMT-1.1.40/bamt/utils/GraphUtils.py
--rw-r--r--   0        0        0     7658 2023-03-17 12:29:52.737830 BAMT-1.1.40/bamt/utils/MathUtils.py
--rw-r--r--   0        0        0     1188 2023-04-20 12:46:05.088240 BAMT-1.1.40/pyproject.toml
--rw-r--r--   0        0        0     8820 2023-03-17 18:51:26.332933 BAMT-1.1.40/README.rst
--rw-r--r--   0        0        0     9963 2023-04-20 12:56:36.209555 BAMT-1.1.40/setup.py
--rw-r--r--   0        0        0     9711 2023-04-20 12:56:36.210555 BAMT-1.1.40/PKG-INFO
+-rw-r--r--   0        0        0        0 2022-10-18 09:46:52.969462 bamt-1.1.41/bamt/__init__.py
+-rw-r--r--   0        0        0    14998 2023-04-10 14:01:43.784052 bamt-1.1.41/bamt/builders.py
+-rw-r--r--   0        0        0      688 2023-04-10 14:01:43.785048 bamt-1.1.41/bamt/config.py
+-rw-r--r--   0        0        0        0 2022-07-18 14:22:44.582873 bamt-1.1.41/bamt/external/__init__.py
+-rw-r--r--   0        0        0      154 2023-03-22 08:13:29.970622 bamt-1.1.41/bamt/external/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      373 2022-12-24 09:53:39.265727 bamt-1.1.41/bamt/external/libpgm/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0       82 2023-04-10 14:01:43.785048 bamt-1.1.41/bamt/external/pyBN/__init__.py
+-rw-r--r--   0        0        0      238 2023-03-27 20:03:35.633736 bamt-1.1.41/bamt/external/pyBN/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2023-04-10 14:01:43.785048 bamt-1.1.41/bamt/external/pyBN/classes/__init__.py
+-rw-r--r--   0        0        0      167 2023-03-27 20:03:35.635733 bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    12842 2023-03-27 20:03:35.673859 bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/bayesnet.cpython-310.pyc
+-rw-r--r--   0        0        0    10770 2023-03-27 08:04:03.587482 bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/cliquetree.cpython-310.pyc
+-rw-r--r--   0        0        0     4738 2023-03-27 08:04:03.584486 bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/clustergraph.cpython-310.pyc
+-rw-r--r--   0        0        0     5165 2023-03-27 08:04:03.681327 bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/empiricaldistribution.cpython-310.pyc
+-rw-r--r--   0        0        0    17971 2023-03-27 08:04:03.593487 bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/factor.cpython-310.pyc
+-rw-r--r--   0        0        0     4873 2023-03-27 08:04:03.590484 bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/factorization.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2022-07-18 14:22:44.588854 bamt-1.1.41/bamt/external/pyBN/classes/_tests/__init__.py
+-rw-r--r--   0        0        0      174 2022-12-24 09:53:41.854845 bamt-1.1.41/bamt/external/pyBN/classes/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5230 2022-12-24 09:53:41.861558 bamt-1.1.41/bamt/external/pyBN/classes/_tests/__pycache__/test_bayesnet.cpython-310.pyc
+-rw-r--r--   0        0        0     6379 2022-12-24 09:53:41.867553 bamt-1.1.41/bamt/external/pyBN/classes/_tests/__pycache__/test_factor.cpython-310.pyc
+-rw-r--r--   0        0        0     5520 2023-04-10 14:01:43.786046 bamt-1.1.41/bamt/external/pyBN/classes/_tests/test_bayesnet.py
+-rw-r--r--   0        0        0    11006 2023-04-10 14:01:43.787042 bamt-1.1.41/bamt/external/pyBN/classes/bayesnet.py
+-rw-r--r--   0        0        0      302 2023-03-27 08:04:03.623486 bamt-1.1.41/bamt/external/pyBN/classification/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3370 2023-03-27 08:04:03.624483 bamt-1.1.41/bamt/external/pyBN/classification/__pycache__/classification.cpython-310.pyc
+-rw-r--r--   0        0        0     3432 2023-03-27 08:04:03.647079 bamt-1.1.41/bamt/external/pyBN/classification/__pycache__/feature_selection.cpython-310.pyc
+-rw-r--r--   0        0        0      335 2023-03-27 08:04:03.626130 bamt-1.1.41/bamt/external/pyBN/inference/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      176 2022-12-24 09:53:41.870556 bamt-1.1.41/bamt/external/pyBN/inference/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1060 2022-12-24 09:53:41.876256 bamt-1.1.41/bamt/external/pyBN/inference/_tests/__pycache__/test_map_exact.cpython-310.pyc
+-rw-r--r--   0        0        0     2776 2022-12-24 09:53:41.882205 bamt-1.1.41/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_approx.cpython-310.pyc
+-rw-r--r--   0        0        0     2251 2022-12-24 09:53:41.886925 bamt-1.1.41/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_exact.cpython-310.pyc
+-rw-r--r--   0        0        0      299 2023-03-27 08:04:03.628136 bamt-1.1.41/bamt/external/pyBN/inference/map_exact/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2653 2023-03-27 08:04:03.630137 bamt-1.1.41/bamt/external/pyBN/inference/map_exact/__pycache__/ilp_map.cpython-310.pyc
+-rw-r--r--   0        0        0     1077 2023-03-27 08:04:03.631117 bamt-1.1.41/bamt/external/pyBN/inference/map_exact/__pycache__/ve_map.cpython-310.pyc
+-rw-r--r--   0        0        0      461 2023-03-27 08:04:03.632119 bamt-1.1.41/bamt/external/pyBN/inference/marginal_approx/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2050 2023-03-27 08:04:03.634118 bamt-1.1.41/bamt/external/pyBN/inference/marginal_approx/__pycache__/forward_sample.cpython-310.pyc
+-rw-r--r--   0        0        0     1553 2023-03-27 08:04:03.639077 bamt-1.1.41/bamt/external/pyBN/inference/marginal_approx/__pycache__/gibbs_sample.cpython-310.pyc
+-rw-r--r--   0        0        0     1783 2023-03-27 08:04:03.641082 bamt-1.1.41/bamt/external/pyBN/inference/marginal_approx/__pycache__/loopy_bp.cpython-310.pyc
+-rw-r--r--   0        0        0     1613 2023-03-27 08:04:03.642078 bamt-1.1.41/bamt/external/pyBN/inference/marginal_approx/__pycache__/lw_sample.cpython-310.pyc
+-rw-r--r--   0        0        0      320 2023-03-27 08:04:03.643078 bamt-1.1.41/bamt/external/pyBN/inference/marginal_exact/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2054 2023-03-27 08:04:03.645083 bamt-1.1.41/bamt/external/pyBN/inference/marginal_exact/__pycache__/exact_bp.cpython-310.pyc
+-rw-r--r--   0        0        0     1432 2023-03-27 08:04:03.646078 bamt-1.1.41/bamt/external/pyBN/inference/marginal_exact/__pycache__/ve_marginal.cpython-310.pyc
+-rw-r--r--   0        0        0      244 2023-03-27 08:04:03.695089 bamt-1.1.41/bamt/external/pyBN/io/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5673 2023-03-27 08:04:03.697093 bamt-1.1.41/bamt/external/pyBN/io/__pycache__/read.cpython-310.pyc
+-rw-r--r--   0        0        0     1690 2023-03-27 08:04:03.699093 bamt-1.1.41/bamt/external/pyBN/io/__pycache__/write.cpython-310.pyc
+-rw-r--r--   0        0        0      169 2022-12-24 09:53:41.889932 bamt-1.1.41/bamt/external/pyBN/io/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1451 2022-12-24 09:53:41.894772 bamt-1.1.41/bamt/external/pyBN/io/_tests/__pycache__/test_reading.cpython-310.pyc
+-rw-r--r--   0        0        0      888 2022-12-24 09:53:41.899461 bamt-1.1.41/bamt/external/pyBN/io/_tests/__pycache__/test_writing.cpython-310.pyc
+-rw-r--r--   0        0        0      271 2023-03-27 08:04:03.649082 bamt-1.1.41/bamt/external/pyBN/learning/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      291 2023-03-27 08:04:03.650078 bamt-1.1.41/bamt/external/pyBN/learning/parameter/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3832 2023-03-27 08:04:03.652079 bamt-1.1.41/bamt/external/pyBN/learning/parameter/__pycache__/bayes.cpython-310.pyc
+-rw-r--r--   0        0        0     5978 2023-03-27 08:04:03.654087 bamt-1.1.41/bamt/external/pyBN/learning/parameter/__pycache__/mle.cpython-310.pyc
+-rw-r--r--   0        0        0      185 2022-12-24 09:53:41.900463 bamt-1.1.41/bamt/external/pyBN/learning/parameter/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      572 2023-03-27 08:04:03.655095 bamt-1.1.41/bamt/external/pyBN/learning/structure/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3770 2023-03-27 08:04:03.694090 bamt-1.1.41/bamt/external/pyBN/learning/structure/__pycache__/mdbn.cpython-310.pyc
+-rw-r--r--   0        0        0      185 2022-12-24 09:53:41.902496 bamt-1.1.41/bamt/external/pyBN/learning/structure/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1821 2022-12-24 09:53:41.905088 bamt-1.1.41/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_chow_liu.cpython-310.pyc
+-rw-r--r--   0        0        0     2139 2022-12-24 09:53:41.908341 bamt-1.1.41/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_grow_shrink.cpython-310.pyc
+-rw-r--r--   0        0        0     1713 2022-12-24 09:53:41.910390 bamt-1.1.41/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_orient_edges.cpython-310.pyc
+-rw-r--r--   0        0        0     1744 2022-12-24 09:53:41.915718 bamt-1.1.41/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_pc.cpython-310.pyc
+-rw-r--r--   0        0        0      548 2023-03-27 08:04:03.657092 bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     4331 2023-03-27 08:04:03.659096 bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/fast_iamb.cpython-310.pyc
+-rw-r--r--   0        0        0     4034 2023-03-27 08:04:03.660092 bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/grow_shrink.cpython-310.pyc
+-rw-r--r--   0        0        0     4359 2023-03-27 08:04:03.662095 bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/iamb.cpython-310.pyc
+-rw-r--r--   0        0        0     2892 2023-03-27 08:04:03.663691 bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/lambda_iamb.cpython-310.pyc
+-rw-r--r--   0        0        0     3783 2023-03-27 08:04:03.665697 bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/path_condition.cpython-310.pyc
+-rw-r--r--   0        0        0      252 2023-03-27 08:04:03.666694 bamt-1.1.41/bamt/external/pyBN/learning/structure/exact/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     1743 2023-03-27 08:04:03.668693 bamt-1.1.41/bamt/external/pyBN/learning/structure/exact/__pycache__/gobnilp.cpython-310.pyc
+-rw-r--r--   0        0        0      251 2023-03-27 08:04:03.669694 bamt-1.1.41/bamt/external/pyBN/learning/structure/hybrid/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2480 2023-03-27 08:04:03.671004 bamt-1.1.41/bamt/external/pyBN/learning/structure/hybrid/__pycache__/mmpc.cpython-310.pyc
+-rw-r--r--   0        0        0      315 2023-03-27 08:04:03.672006 bamt-1.1.41/bamt/external/pyBN/learning/structure/naive/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2312 2023-03-27 08:04:03.674010 bamt-1.1.41/bamt/external/pyBN/learning/structure/naive/__pycache__/naive_bayes.cpython-310.pyc
+-rw-r--r--   0        0        0      870 2023-03-27 08:04:03.675322 bamt-1.1.41/bamt/external/pyBN/learning/structure/naive/__pycache__/TAN.cpython-310.pyc
+-rw-r--r--   0        0        0      524 2023-03-27 08:04:03.676326 bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     3803 2023-03-27 08:04:03.678326 bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/bayes_scores.cpython-310.pyc
+-rw-r--r--   0        0        0     6763 2023-03-27 08:04:03.683330 bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/hill_climbing.cpython-310.pyc
+-rw-r--r--   0        0        0     5042 2023-03-27 08:04:03.684326 bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/info_scores.cpython-310.pyc
+-rw-r--r--   0        0        0     6013 2023-03-27 08:04:03.687330 bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/random_restarts.cpython-310.pyc
+-rw-r--r--   0        0        0     4959 2023-03-27 08:04:03.689330 bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/tabu.cpython-310.pyc
+-rw-r--r--   0        0        0      251 2023-03-27 08:04:03.691046 bamt-1.1.41/bamt/external/pyBN/learning/structure/tree/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2067 2023-03-27 08:04:03.692088 bamt-1.1.41/bamt/external/pyBN/learning/structure/tree/__pycache__/chow_liu.cpython-310.pyc
+-rw-r--r--   0        0        0      217 2022-12-24 09:53:41.922124 bamt-1.1.41/bamt/external/pyBN/plotting/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2504 2022-12-24 09:53:41.930964 bamt-1.1.41/bamt/external/pyBN/plotting/__pycache__/plot.cpython-310.pyc
+-rw-r--r--   0        0        0      208 2023-04-10 14:01:43.787042 bamt-1.1.41/bamt/external/pyBN/utils/__init__.py
+-rw-r--r--   0        0        0      362 2023-03-27 20:03:35.640736 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      948 2023-03-27 20:03:35.646737 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/class_equivalence.cpython-310.pyc
+-rw-r--r--   0        0        0      840 2023-03-27 20:03:35.653137 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0        0        0     3156 2023-03-27 08:04:03.602487 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/discretize.cpython-310.pyc
+-rw-r--r--   0        0        0     1274 2023-03-27 20:03:35.658779 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/graph.cpython-310.pyc
+-rw-r--r--   0        0        0      973 2023-03-27 08:04:03.606486 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/hybrid_distance.cpython-310.pyc
+-rw-r--r--   0        0        0     4392 2023-03-27 20:03:35.665794 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/independence_tests.cpython-310.pyc
+-rw-r--r--   0        0        0     4723 2023-03-27 08:04:03.612483 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/markov_blanket.cpython-310.pyc
+-rw-r--r--   0        0        0     4640 2023-03-27 08:04:03.615487 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/orient_edges.cpython-310.pyc
+-rw-r--r--   0        0        0     3492 2023-03-27 08:04:03.617486 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/parameter_distance.cpython-310.pyc
+-rw-r--r--   0        0        0     1943 2023-03-27 08:04:03.619487 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/random_sample.cpython-310.pyc
+-rw-r--r--   0        0        0     2896 2023-03-27 08:04:03.621487 bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/structure_distance.cpython-310.pyc
+-rw-r--r--   0        0        0        0 2022-07-18 14:22:44.702765 bamt-1.1.41/bamt/external/pyBN/utils/_tests/__init__.py
+-rw-r--r--   0        0        0      172 2022-12-24 09:53:42.684367 bamt-1.1.41/bamt/external/pyBN/utils/_tests/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2656 2022-12-24 09:53:42.690369 bamt-1.1.41/bamt/external/pyBN/utils/_tests/__pycache__/test_independence_tests.cpython-310.pyc
+-rw-r--r--   0        0        0     1462 2022-12-24 09:53:42.696862 bamt-1.1.41/bamt/external/pyBN/utils/_tests/__pycache__/test_markov_blanket.cpython-310.pyc
+-rw-r--r--   0        0        0     1700 2022-12-24 09:53:42.699046 bamt-1.1.41/bamt/external/pyBN/utils/_tests/__pycache__/test_orient_edges.cpython-310.pyc
+-rw-r--r--   0        0        0     1483 2022-12-24 09:53:42.704515 bamt-1.1.41/bamt/external/pyBN/utils/_tests/__pycache__/test_random_sample.cpython-310.pyc
+-rw-r--r--   0        0        0     1788 2023-04-10 14:01:43.787042 bamt-1.1.41/bamt/external/pyBN/utils/_tests/test_independence_tests.py
+-rw-r--r--   0        0        0     1155 2023-04-10 14:01:43.788038 bamt-1.1.41/bamt/external/pyBN/utils/_tests/test_markov_blanket.py
+-rw-r--r--   0        0        0     1205 2023-04-10 14:01:43.788038 bamt-1.1.41/bamt/external/pyBN/utils/_tests/test_orient_edges.py
+-rw-r--r--   0        0        0      970 2023-04-10 14:01:43.788038 bamt-1.1.41/bamt/external/pyBN/utils/_tests/test_random_sample.py
+-rw-r--r--   0        0        0      907 2023-04-10 14:01:43.789035 bamt-1.1.41/bamt/external/pyBN/utils/class_equivalence.py
+-rw-r--r--   0        0        0      626 2023-04-10 14:01:43.789035 bamt-1.1.41/bamt/external/pyBN/utils/data.py
+-rw-r--r--   0        0        0     1386 2023-04-10 14:01:43.790031 bamt-1.1.41/bamt/external/pyBN/utils/graph.py
+-rw-r--r--   0        0        0     6222 2023-04-10 14:01:43.790031 bamt-1.1.41/bamt/external/pyBN/utils/independence_tests.py
+-rw-r--r--   0        0        0      979 2023-03-17 12:29:52.731831 bamt-1.1.41/bamt/log.py
+-rw-r--r--   0        0        0     1090 2022-08-01 09:44:45.658643 bamt-1.1.41/bamt/logging.conf
+-rw-r--r--   0        0        0    10778 2023-04-10 14:01:43.791028 bamt-1.1.41/bamt/mi_entropy_gauss.py
+-rw-r--r--   0        0        0      119 2023-04-10 14:01:43.791028 bamt-1.1.41/bamt/networks/__init__.py
+-rw-r--r--   0        0        0      229 2023-03-27 20:16:49.956781 bamt-1.1.41/bamt/networks/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    26367 2023-03-31 13:44:44.700941 bamt-1.1.41/bamt/networks/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     1115 2023-03-28 14:57:14.478682 bamt-1.1.41/bamt/networks/__pycache__/hybrid_bn.cpython-310.pyc
+-rw-r--r--   0        0        0    31404 2023-04-10 14:01:43.792025 bamt-1.1.41/bamt/networks/base.py
+-rw-r--r--   0        0        0     1704 2023-04-10 14:01:43.792025 bamt-1.1.41/bamt/networks/big_brave_bn.py
+-rw-r--r--   0        0        0      422 2023-04-10 14:01:43.792025 bamt-1.1.41/bamt/networks/continuous_bn.py
+-rw-r--r--   0        0        0      392 2023-04-10 14:01:43.792025 bamt-1.1.41/bamt/networks/discrete_bn.py
+-rw-r--r--   0        0        0      737 2023-04-10 14:01:43.793022 bamt-1.1.41/bamt/networks/hybrid_bn.py
+-rw-r--r--   0        0        0      223 2023-04-10 14:01:43.793022 bamt-1.1.41/bamt/nodes/__init__.py
+-rw-r--r--   0        0        0      324 2023-03-25 11:38:48.177276 bamt-1.1.41/bamt/nodes/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2653 2023-03-31 13:44:42.957971 bamt-1.1.41/bamt/nodes/__pycache__/base.cpython-310.pyc
+-rw-r--r--   0        0        0     4702 2023-03-27 08:25:39.343392 bamt-1.1.41/bamt/nodes/__pycache__/conditional_gaussian_node.cpython-310.pyc
+-rw-r--r--   0        0        0     4717 2023-03-27 08:25:39.380393 bamt-1.1.41/bamt/nodes/__pycache__/conditional_logit_node.cpython-310.pyc
+-rw-r--r--   0        0        0     5041 2023-03-25 11:38:48.587289 bamt-1.1.41/bamt/nodes/__pycache__/conditional_mixture_gaussian_node.cpython-310.pyc
+-rw-r--r--   0        0        0     4095 2023-03-25 11:38:49.014930 bamt-1.1.41/bamt/nodes/__pycache__/discrete_node.cpython-310.pyc
+-rw-r--r--   0        0        0     3396 2023-03-27 08:25:39.477816 bamt-1.1.41/bamt/nodes/__pycache__/gaussian_node.cpython-310.pyc
+-rw-r--r--   0        0        0     3270 2023-03-27 08:25:39.475813 bamt-1.1.41/bamt/nodes/__pycache__/logit_node.cpython-310.pyc
+-rw-r--r--   0        0        0     3723 2023-03-25 11:38:49.780249 bamt-1.1.41/bamt/nodes/__pycache__/mixture_gaussian_node.cpython-310.pyc
+-rw-r--r--   0        0        0     1796 2023-03-25 11:16:57.986776 bamt-1.1.41/bamt/nodes/__pycache__/schema.cpython-310.pyc
+-rw-r--r--   0        0        0     2685 2023-04-10 14:01:43.793022 bamt-1.1.41/bamt/nodes/base.py
+-rw-r--r--   0        0        0     7951 2023-04-10 14:01:43.793022 bamt-1.1.41/bamt/nodes/conditional_gaussian_node.py
+-rw-r--r--   0        0        0     6920 2023-04-10 14:01:43.794018 bamt-1.1.41/bamt/nodes/conditional_logit_node.py
+-rw-r--r--   0        0        0     8119 2023-04-10 14:01:43.794018 bamt-1.1.41/bamt/nodes/conditional_mixture_gaussian_node.py
+-rw-r--r--   0        0        0     4064 2023-04-10 14:01:43.794018 bamt-1.1.41/bamt/nodes/discrete_node.py
+-rw-r--r--   0        0        0     4424 2023-04-10 14:01:43.795015 bamt-1.1.41/bamt/nodes/gaussian_node.py
+-rw-r--r--   0        0        0     4026 2023-04-10 14:01:43.795015 bamt-1.1.41/bamt/nodes/logit_node.py
+-rw-r--r--   0        0        0     5476 2023-04-10 14:01:43.795015 bamt-1.1.41/bamt/nodes/mixture_gaussian_node.py
+-rw-r--r--   0        0        0     1034 2023-04-10 14:01:43.795015 bamt-1.1.41/bamt/nodes/schema.py
+-rw-r--r--   0        0        0        0 2022-07-18 14:22:44.707748 bamt-1.1.41/bamt/preprocess/__init__.py
+-rw-r--r--   0        0        0      156 2023-03-22 08:13:30.026531 bamt-1.1.41/bamt/preprocess/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     5287 2023-03-22 08:13:30.040531 bamt-1.1.41/bamt/preprocess/__pycache__/discretization.cpython-310.pyc
+-rw-r--r--   0        0        0     1292 2023-03-22 08:13:30.056531 bamt-1.1.41/bamt/preprocess/__pycache__/graph.cpython-310.pyc
+-rw-r--r--   0        0        0     1993 2023-03-22 08:13:30.051545 bamt-1.1.41/bamt/preprocess/__pycache__/numpy_pandas.cpython-310.pyc
+-rw-r--r--   0        0        0     5449 2023-03-17 12:29:52.733830 bamt-1.1.41/bamt/preprocess/discretization.py
+-rw-r--r--   0        0        0      871 2023-03-17 12:29:52.734830 bamt-1.1.41/bamt/preprocess/graph.py
+-rw-r--r--   0        0        0     1904 2023-03-17 12:29:52.734830 bamt-1.1.41/bamt/preprocess/numpy_pandas.py
+-rw-r--r--   0        0        0     4363 2023-03-17 12:29:52.735830 bamt-1.1.41/bamt/preprocessors.py
+-rw-r--r--   0        0        0    12521 2023-04-10 14:01:43.796011 bamt-1.1.41/bamt/redef_HC.py
+-rw-r--r--   0        0        0     6177 2023-04-10 14:01:43.797008 bamt-1.1.41/bamt/redef_info_scores.py
+-rw-r--r--   0        0        0        0 2022-07-18 14:22:44.709741 bamt-1.1.41/bamt/utils/__init__.py
+-rw-r--r--   0        0        0      151 2023-03-22 08:13:30.083531 bamt-1.1.41/bamt/utils/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0     2543 2023-03-27 08:04:04.969879 bamt-1.1.41/bamt/utils/__pycache__/GraphUtils.cpython-310.pyc
+-rw-r--r--   0        0        0     6440 2023-03-22 08:14:15.703888 bamt-1.1.41/bamt/utils/__pycache__/MathUtils.cpython-310.pyc
+-rw-r--r--   0        0        0     2412 2023-04-10 14:01:43.797008 bamt-1.1.41/bamt/utils/GraphUtils.py
+-rw-r--r--   0        0        0     7658 2023-03-17 12:29:52.737830 bamt-1.1.41/bamt/utils/MathUtils.py
+-rw-r--r--   0        0        0     1151 2023-06-01 12:59:10.912215 bamt-1.1.41/pyproject.toml
+-rw-r--r--   0        0        0     8820 2023-03-17 18:51:26.332933 bamt-1.1.41/README.rst
+-rw-r--r--   0        0        0     9675 1970-01-01 00:00:00.000000 bamt-1.1.41/PKG-INFO
```

### Comparing `BAMT-1.1.40/bamt/builders.py` & `bamt-1.1.41/bamt/builders.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/config.py` & `bamt-1.1.41/bamt/config.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/bayesnet.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/bayesnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/cliquetree.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/cliquetree.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/clustergraph.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/clustergraph.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/empiricaldistribution.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/empiricaldistribution.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/factor.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/factor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classes/__pycache__/factorization.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/classes/__pycache__/factorization.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__pycache__/test_bayesnet.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/classes/_tests/__pycache__/test_bayesnet.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classes/_tests/__pycache__/test_factor.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/classes/_tests/__pycache__/test_factor.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classes/_tests/test_bayesnet.py` & `bamt-1.1.41/bamt/external/pyBN/classes/_tests/test_bayesnet.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classes/bayesnet.py` & `bamt-1.1.41/bamt/external/pyBN/classes/bayesnet.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classification/__pycache__/classification.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/classification/__pycache__/classification.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/classification/__pycache__/feature_selection.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/classification/__pycache__/feature_selection.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_map_exact.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/_tests/__pycache__/test_map_exact.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_approx.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_approx.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_exact.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/_tests/__pycache__/test_marginal_exact.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/map_exact/__pycache__/ilp_map.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/map_exact/__pycache__/ilp_map.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/map_exact/__pycache__/ve_map.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/map_exact/__pycache__/ve_map.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/forward_sample.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/marginal_approx/__pycache__/forward_sample.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/gibbs_sample.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/marginal_approx/__pycache__/gibbs_sample.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/loopy_bp.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/marginal_approx/__pycache__/loopy_bp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_approx/__pycache__/lw_sample.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/marginal_approx/__pycache__/lw_sample.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_exact/__pycache__/exact_bp.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/marginal_exact/__pycache__/exact_bp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/inference/marginal_exact/__pycache__/ve_marginal.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/inference/marginal_exact/__pycache__/ve_marginal.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/io/__pycache__/read.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/io/__pycache__/read.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/io/__pycache__/write.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/io/__pycache__/write.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/io/_tests/__pycache__/test_reading.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/io/_tests/__pycache__/test_reading.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/io/_tests/__pycache__/test_writing.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/io/_tests/__pycache__/test_writing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/parameter/__pycache__/bayes.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/parameter/__pycache__/bayes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/parameter/__pycache__/mle.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/parameter/__pycache__/mle.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/__pycache__/__init__.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/__pycache__/mdbn.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/__pycache__/mdbn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_chow_liu.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_chow_liu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_grow_shrink.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_grow_shrink.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_orient_edges.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_orient_edges.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_pc.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/_tests/__pycache__/test_pc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/__init__.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/fast_iamb.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/fast_iamb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/grow_shrink.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/grow_shrink.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/iamb.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/iamb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/lambda_iamb.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/lambda_iamb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/constraint/__pycache__/path_condition.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/constraint/__pycache__/path_condition.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/exact/__pycache__/gobnilp.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/exact/__pycache__/gobnilp.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/hybrid/__pycache__/mmpc.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/hybrid/__pycache__/mmpc.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/naive/__pycache__/naive_bayes.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/naive/__pycache__/naive_bayes.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/naive/__pycache__/TAN.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/naive/__pycache__/TAN.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/__init__.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/bayes_scores.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/bayes_scores.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/hill_climbing.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/hill_climbing.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/info_scores.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/info_scores.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/random_restarts.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/random_restarts.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/score/__pycache__/tabu.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/score/__pycache__/tabu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/learning/structure/tree/__pycache__/chow_liu.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/learning/structure/tree/__pycache__/chow_liu.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/plotting/__pycache__/plot.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/plotting/__pycache__/plot.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/class_equivalence.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/class_equivalence.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/data.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/discretize.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/discretize.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/graph.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/graph.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/hybrid_distance.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/hybrid_distance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/independence_tests.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/independence_tests.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/markov_blanket.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/markov_blanket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/orient_edges.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/orient_edges.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/parameter_distance.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/parameter_distance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/random_sample.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/random_sample.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/__pycache__/structure_distance.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/__pycache__/structure_distance.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_independence_tests.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/_tests/__pycache__/test_independence_tests.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_markov_blanket.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/_tests/__pycache__/test_markov_blanket.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_orient_edges.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/_tests/__pycache__/test_orient_edges.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/__pycache__/test_random_sample.cpython-310.pyc` & `bamt-1.1.41/bamt/external/pyBN/utils/_tests/__pycache__/test_random_sample.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_independence_tests.py` & `bamt-1.1.41/bamt/external/pyBN/utils/_tests/test_independence_tests.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_markov_blanket.py` & `bamt-1.1.41/bamt/external/pyBN/utils/_tests/test_markov_blanket.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_orient_edges.py` & `bamt-1.1.41/bamt/external/pyBN/utils/_tests/test_orient_edges.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/_tests/test_random_sample.py` & `bamt-1.1.41/bamt/external/pyBN/utils/_tests/test_random_sample.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/class_equivalence.py` & `bamt-1.1.41/bamt/external/pyBN/utils/class_equivalence.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/data.py` & `bamt-1.1.41/bamt/external/pyBN/utils/data.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/graph.py` & `bamt-1.1.41/bamt/external/pyBN/utils/graph.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/external/pyBN/utils/independence_tests.py` & `bamt-1.1.41/bamt/external/pyBN/utils/independence_tests.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/log.py` & `bamt-1.1.41/bamt/log.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/logging.conf` & `bamt-1.1.41/bamt/logging.conf`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/mi_entropy_gauss.py` & `bamt-1.1.41/bamt/mi_entropy_gauss.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/networks/__pycache__/base.cpython-310.pyc` & `bamt-1.1.41/bamt/networks/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/networks/__pycache__/hybrid_bn.cpython-310.pyc` & `bamt-1.1.41/bamt/networks/__pycache__/hybrid_bn.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/networks/base.py` & `bamt-1.1.41/bamt/networks/base.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/networks/big_brave_bn.py` & `bamt-1.1.41/bamt/networks/big_brave_bn.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/networks/hybrid_bn.py` & `bamt-1.1.41/bamt/networks/hybrid_bn.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/__pycache__/base.cpython-310.pyc` & `bamt-1.1.41/bamt/nodes/__pycache__/base.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/__pycache__/conditional_gaussian_node.cpython-310.pyc` & `bamt-1.1.41/bamt/nodes/__pycache__/conditional_gaussian_node.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/__pycache__/conditional_logit_node.cpython-310.pyc` & `bamt-1.1.41/bamt/nodes/__pycache__/conditional_logit_node.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/__pycache__/conditional_mixture_gaussian_node.cpython-310.pyc` & `bamt-1.1.41/bamt/nodes/__pycache__/conditional_mixture_gaussian_node.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/__pycache__/discrete_node.cpython-310.pyc` & `bamt-1.1.41/bamt/nodes/__pycache__/discrete_node.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/__pycache__/gaussian_node.cpython-310.pyc` & `bamt-1.1.41/bamt/nodes/__pycache__/gaussian_node.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/__pycache__/logit_node.cpython-310.pyc` & `bamt-1.1.41/bamt/nodes/__pycache__/logit_node.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/__pycache__/mixture_gaussian_node.cpython-310.pyc` & `bamt-1.1.41/bamt/nodes/__pycache__/mixture_gaussian_node.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/__pycache__/schema.cpython-310.pyc` & `bamt-1.1.41/bamt/nodes/__pycache__/schema.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/base.py` & `bamt-1.1.41/bamt/nodes/base.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/conditional_gaussian_node.py` & `bamt-1.1.41/bamt/nodes/conditional_gaussian_node.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/conditional_logit_node.py` & `bamt-1.1.41/bamt/nodes/conditional_logit_node.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/conditional_mixture_gaussian_node.py` & `bamt-1.1.41/bamt/nodes/conditional_mixture_gaussian_node.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/discrete_node.py` & `bamt-1.1.41/bamt/nodes/discrete_node.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/gaussian_node.py` & `bamt-1.1.41/bamt/nodes/gaussian_node.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/logit_node.py` & `bamt-1.1.41/bamt/nodes/logit_node.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/mixture_gaussian_node.py` & `bamt-1.1.41/bamt/nodes/mixture_gaussian_node.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/nodes/schema.py` & `bamt-1.1.41/bamt/nodes/schema.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/preprocess/__pycache__/discretization.cpython-310.pyc` & `bamt-1.1.41/bamt/preprocess/__pycache__/discretization.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/preprocess/__pycache__/graph.cpython-310.pyc` & `bamt-1.1.41/bamt/preprocess/__pycache__/graph.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/preprocess/__pycache__/numpy_pandas.cpython-310.pyc` & `bamt-1.1.41/bamt/preprocess/__pycache__/numpy_pandas.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/preprocess/discretization.py` & `bamt-1.1.41/bamt/preprocess/discretization.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/preprocess/graph.py` & `bamt-1.1.41/bamt/preprocess/graph.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/preprocess/numpy_pandas.py` & `bamt-1.1.41/bamt/preprocess/numpy_pandas.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/preprocessors.py` & `bamt-1.1.41/bamt/preprocessors.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/redef_HC.py` & `bamt-1.1.41/bamt/redef_HC.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/redef_info_scores.py` & `bamt-1.1.41/bamt/redef_info_scores.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/utils/__pycache__/GraphUtils.cpython-310.pyc` & `bamt-1.1.41/bamt/utils/__pycache__/GraphUtils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/utils/__pycache__/MathUtils.cpython-310.pyc` & `bamt-1.1.41/bamt/utils/__pycache__/MathUtils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/utils/GraphUtils.py` & `bamt-1.1.41/bamt/utils/GraphUtils.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/bamt/utils/MathUtils.py` & `bamt-1.1.41/bamt/utils/MathUtils.py`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/pyproject.toml` & `bamt-1.1.41/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "BAMT"
-version = "1.1.40"
+version = "1.1.41"
 description = "data modeling and analysis tool based on Bayesian networks"
 authors = ["Roman Netrogolov <romius2001@gmail.com>",
 	   "Irina Deeva <iriny.deeva@gmail.com>",
 	   "Karine Shakhkyan <kshahkyan@yandex.ru>",
 	   "Nikita Kovalev Yasen <Nikitoskova123@gmail.com>",
 	   "Anna Bubnova <banuba313@gmail.com>",
 	   "Yury Kaminsky <jkaminski@niuitmo.ru>"]
@@ -18,27 +18,27 @@
 
 packages = [
     { include = "bamt" }
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
-setuptools = "65.6.3"
 numpy = ">=1.24.2"
 matplotlib = "3.6.2"
 pandas = "1.5.2"
 pomegranate = "0.14.8"
 gmr = "1.6.2"
-scikit-learn = "1.2.0"
+scikit-learn = ">=0.24.0"
 scipy = "^1.8.0"
-pyvis = ">=0.2.1"
+pyvis = ">=0.3.2"
 missingno = "^0.5.1"
 pgmpy = "0.1.20"
-pyitlib = "0.2.2"
+pyitlib = "0.2.3"
+
+
 
 [tool.poetry.dev-dependencies]
 pytest = "7.1.3"
-catboost = "1.1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `BAMT-1.1.40/README.rst` & `bamt-1.1.41/README.rst`

 * *Files identical despite different names*

### Comparing `BAMT-1.1.40/setup.py` & `bamt-1.1.41/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,51 +1,239 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: bamt
+Version: 1.1.41
+Summary: data modeling and analysis tool based on Bayesian networks
+Home-page: https://github.com/ITMO-NSS-team/BAMT
+License: BSD-3-Clause
+Author: Roman Netrogolov
+Author-email: romius2001@gmail.com
+Requires-Python: >=3.9,<3.11
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Requires-Dist: gmr (==1.6.2)
+Requires-Dist: matplotlib (==3.6.2)
+Requires-Dist: missingno (>=0.5.1,<0.6.0)
+Requires-Dist: numpy (>=1.24.2)
+Requires-Dist: pandas (==1.5.2)
+Requires-Dist: pgmpy (==0.1.20)
+Requires-Dist: pomegranate (==0.14.8)
+Requires-Dist: pyitlib (==0.2.3)
+Requires-Dist: pyvis (>=0.3.2)
+Requires-Dist: scikit-learn (>=0.24.0)
+Requires-Dist: scipy (>=1.8.0,<2.0.0)
+Project-URL: Repository, https://github.com/ITMO-NSS-team/BAMT
+Description-Content-Type: text/x-rst
 
-packages = \
-['bamt',
- 'bamt.external',
- 'bamt.external.pyBN',
- 'bamt.external.pyBN.classes',
- 'bamt.external.pyBN.classes._tests',
- 'bamt.external.pyBN.utils',
- 'bamt.external.pyBN.utils._tests',
- 'bamt.networks',
- 'bamt.nodes',
- 'bamt.preprocess',
- 'bamt.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['gmr==1.6.2',
- 'matplotlib==3.6.2',
- 'missingno>=0.5.1,<0.6.0',
- 'numpy>=1.24.2',
- 'pandas==1.5.2',
- 'pgmpy==0.1.20',
- 'pomegranate==0.14.8',
- 'pyitlib==0.2.2',
- 'pyvis>=0.2.1',
- 'scikit-learn==1.2.0',
- 'scipy>=1.8.0,<2.0.0',
- 'setuptools==65.6.3']
-
-setup_kwargs = {
-    'name': 'bamt',
-    'version': '1.1.40',
-    'description': 'data modeling and analysis tool based on Bayesian networks',
-    'long_description': ".. image:: /docs/images/BAMT_white_bg.png\n   :align: center\n   :alt: BAMT framework logo\n\n.. start-badges\n.. list-table::\n   :stub-columns: 1\n\n   * - package\n     - | |pypi| |py_8| |py_9| |py_10|\n   * - tests\n     - | |Build| |coverage|\n   * - docs\n     - |docs|\n   * - license\n     - | |license|\n   * - stats\n     - | |downloads_stats| |downloads_monthly| |downloads_weekly|\n\nRepository of a data modeling and analysis tool based on Bayesian networks\n\nBAMT - Bayesian Analytical and Modelling Toolkit. This repository contains a data modeling and analysis tool based on Bayesian networks. It can be divided into two main parts - algorithms for constructing and training Bayesian networks on data and algorithms for applying Bayesian networks for filling gaps, generating synthetic data, assessing edges strength e.t.c.\n\n.. image:: docs/images/bamt_readme_scheme.png\n     :target: docs/images/bamt_readme_scheme.png\n     :align: center\n     :alt: bamt readme scheme\n\nInstallation\n^^^^^^^^^^^^\n\nBAMT package is available via PyPi:\n\n.. code-block:: bash\n\n   pip install bamt\n\nBAMT Features\n^^^^^^^^^^^^^\n\nThe following algorithms for Bayesian Networks learning are implemented:\n\n\n* Building the structure of a Bayesian network based on expert knowledge by directly specifying the structure of the network;\n* Building the structure of a Bayesian network on data using three algorithms - Hill Climbing, evolutionary and PC (evolutionary and PC are currently under development). For Hill Climbing, the following score functions are implemented - MI, K2, BIC, AIC. The algorithms work on both discrete and mixed data.\n* Learning the parameters of distributions in the nodes of the network based on Gaussian distribution and Mixture Gaussian distribution with automatic selection of the number of components.\n* Non-parametric learning of distributions at nodes using classification and regression models.\n* BigBraveBN - algorithm for structural learning of Bayesian networks with a large number of nodes. Tested on networks with up to 500 nodes.\n\nDifference from existing implementations:\n\n\n* Algorithms work on mixed data;\n* Structural learning implements score-functions for mixed data;\n* Parametric learning implements the use of a mixture of Gaussian distributions to approximate continuous distributions;\n* Non-parametric learning of distributions with various user-specified regression and classification models;\n* The algorithm for structural training of large Bayesian networks (> 10 nodes) is based on local training of small networks with their subsequent algorithmic connection.\n\n.. image:: img/BN_gif.gif\n     :target: img/BN_gif.gif\n     :align: center\n     :alt: bn example gif\n\nFor example, in terms of data analysis and modeling using Bayesian networks, a pipeline has been implemented to generate synthetic data by sampling from Bayesian networks.\n\n\n\n.. image:: img/synth_gen.png\n   :target: img/synth_gen.png\n   :align: center\n   :height: 300px\n   :width: 600px\n   :alt: synthetics generation\n\n\nHow to use\n^^^^^^^^^^\n\nThen the necessary classes are imported from the library:\n\n.. code-block:: python\n\n   import bamt.networks as Nets\n\nNext, a network instance is created and training (structure and parameters) is performed:\n\n.. code-block:: python\n\n   bn = Nets.HybridBN(has_logit=False, use_mixture=True)\n   bn.add_edges(discretized_data, scoring_function=('K2',K2Score))\n   bn.fit_parameters(data)\n\n\n\nExamples & Tutorials\n^^^^^^^^^^^^^^^^^^^^^^\n\nMore examples can be found in `tutorials <https://github.com/ITMO-NSS-team/BAMT/tree/master/tutorials>`__  and `Documentation <https://bamt.readthedocs.io/en/latest/examples/learn_save.html>`__.\n\nPublications about BAMT\n^^^^^^^^^^^^^^^^^^^^^^^\n\nWe have published several articles about BAMT:\n\n* `Advanced Approach for Distributions Parameters Learning in Bayesian Networks with Gaussian Mixture Models and Discriminative Models <https://www.mdpi.com/2227-7390/11/2/343>`__ (2023)\n* `BigBraveBN: algorithm of structural learning for bayesian networks with a large number of nodes <https://www.sciencedirect.com/science/article/pii/S1877050922016945>`__ (2022)\n* `MIxBN: Library for learning Bayesian networks from mixed data <https://www.sciencedirect.com/science/article/pii/S1877050921020925>`__ (2021)\n* `Oil and Gas Reservoirs Parameters Analysis Using Mixed Learning of Bayesian Networks <https://link.springer.com/chapter/10.1007/978-3-030-77961-0_33>`__ (2021)\n* `Bayesian Networks-based personal data synthesis <https://dl.acm.org/doi/abs/10.1145/3411170.3411243>`__ (2020)\n\n\nProject structure\n^^^^^^^^^^^^^^^^^\n\nThe latest stable version of the library is available in the master branch.\n\nIt includes the following modules and direcotries:\n\n* `bamt <https://github.com/ITMO-NSS-team/BAMT/tree/master/bamt>`__ - directory with the framework code:\n    * Preprocessing - module for data preprocessing\n    * Networks - module for building and training Bayesian networks\n    * Nodes - module for nodes support of Bayesian networks\n    * Utilities - module for mathematical and graph utilities\n* `data <https://github.com/ITMO-NSS-team/BAMT/tree/master/data>`__  - directory with data for experiments and tests\n* `tests <https://github.com/ITMO-NSS-team/BAMT/tree/master/tests>`__  - directory with unit and integration tests\n* `tutorials <https://github.com/ITMO-NSS-team/BAMT/tree/master/tutorials>`__  - directory with tutorials\n* `docs <https://github.com/ITMO-NSS-team/BAMT/tree/master/docs>`__ - directory with RTD documentation\n\nPreprocessing\n=============\n\nPreprocessor module allows user to transform data according pipeline (similar to pipeline in scikit-learn).\n\nNetworks\n========\n\nThree types of networks are implemented:\n\n* HybridBN - Bayesian network with mixed data\n* DiscreteBN - Bayesian network with discrete data\n* ContinuousBN - Bayesian network with continuous data\n\nThey are inherited from the abstract class BaseNetwork.\n\nNodes\n=====\n\nContains classes for nodes of Bayesian networks.\n\nUtilities\n=========\n\nUtilities module contains mathematical and graph utilities to support the main functionality of the library.\n\n\nWeb-BAMT\n^^^^^^^^\n\nA web interface for BAMT is currently under development.\nThe repository is available at `web-BAMT <https://github.com/aimclub/Web-BAMT>`__\n\nContacts\n^^^^^^^^\n\nIf you have questions or suggestions, you can contact us at the following address: ideeva@itmo.ru (Irina Deeva)\n\nOur resources:\n\n* `Natural Systems Simulation Team <https://itmo-nss-team.github.io/>`__\n* `NSS team Telegram channel <https://t.me/NSS_group>`__\n* `NSS lab YouTube channel <https://www.youtube.com/@nsslab/videos>`__\n\n.. |docs| image:: https://readthedocs.org/projects/bamt/badge/?version=latest\n    :target: https://bamt.readthedocs.io/en/latest/?badge=latest\n    :alt: Documentation Status\n\n.. |pypi| image:: https://badge.fury.io/py/bamt.svg\n    :target: https://badge.fury.io/py/bamt\n\n.. |py_10| image:: https://img.shields.io/badge/python_3.10-passing-success\n   :alt: Supported Python Versions\n   :target: https://img.shields.io/badge/python_3.10-passing-success\n\n.. |py_8| image:: https://img.shields.io/badge/python_3.8-passing-success\n   :alt: Supported Python Versions\n   :target: https://img.shields.io/badge/python_3.8-passing-success\n\n.. |py_9| image:: https://img.shields.io/badge/python_3.9-passing-success\n   :alt: Supported Python Versions\n   :target: https://img.shields.io/badge/python_3.9-passing-success\n\n.. |license| image:: https://img.shields.io/github/license/ITMO-NSS-team/BAMT\n   :alt: Supported Python Versions\n   :target: https://github.com/ITMO-NSS-team/BAMT/blob/master/LICENCE\n\n.. |downloads_stats| image:: https://static.pepy.tech/personalized-badge/bamt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads\n :target: https://pepy.tech/project/bamt\n\n.. |downloads_monthly| image:: https://static.pepy.tech/personalized-badge/bamt?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month\n :target: https://pepy.tech/project/bamt\n\n.. |downloads_weekly| image:: https://static.pepy.tech/personalized-badge/bamt?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week\n :target: https://pepy.tech/project/bamt\n\n.. |Build| image:: https://github.com/ITMO-NSS-team/BAMT/actions/workflows/bamtcodecov.yml/badge.svg\n   :target: https://github.com/ITMO-NSS-team/BAMT/actions/workflows/bamtcodecov.yml\n\n.. |coverage| image:: https://codecov.io/github/ITMO-NSS-team/BAMT/branch/master/graph/badge.svg?token=9ZX37JNIYZ\n   :target: https://codecov.io/github/ITMO-NSS-team/BAMT\n",
-    'author': 'Roman Netrogolov',
-    'author_email': 'romius2001@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/ITMO-NSS-team/BAMT',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<3.11',
-}
+.. image:: /docs/images/BAMT_white_bg.png
+   :align: center
+   :alt: BAMT framework logo
 
+.. start-badges
+.. list-table::
+   :stub-columns: 1
+
+   * - package
+     - | |pypi| |py_8| |py_9| |py_10|
+   * - tests
+     - | |Build| |coverage|
+   * - docs
+     - |docs|
+   * - license
+     - | |license|
+   * - stats
+     - | |downloads_stats| |downloads_monthly| |downloads_weekly|
+
+Repository of a data modeling and analysis tool based on Bayesian networks
+
+BAMT - Bayesian Analytical and Modelling Toolkit. This repository contains a data modeling and analysis tool based on Bayesian networks. It can be divided into two main parts - algorithms for constructing and training Bayesian networks on data and algorithms for applying Bayesian networks for filling gaps, generating synthetic data, assessing edges strength e.t.c.
+
+.. image:: docs/images/bamt_readme_scheme.png
+     :target: docs/images/bamt_readme_scheme.png
+     :align: center
+     :alt: bamt readme scheme
+
+Installation
+^^^^^^^^^^^^
+
+BAMT package is available via PyPi:
+
+.. code-block:: bash
+
+   pip install bamt
+
+BAMT Features
+^^^^^^^^^^^^^
+
+The following algorithms for Bayesian Networks learning are implemented:
+
+
+* Building the structure of a Bayesian network based on expert knowledge by directly specifying the structure of the network;
+* Building the structure of a Bayesian network on data using three algorithms - Hill Climbing, evolutionary and PC (evolutionary and PC are currently under development). For Hill Climbing, the following score functions are implemented - MI, K2, BIC, AIC. The algorithms work on both discrete and mixed data.
+* Learning the parameters of distributions in the nodes of the network based on Gaussian distribution and Mixture Gaussian distribution with automatic selection of the number of components.
+* Non-parametric learning of distributions at nodes using classification and regression models.
+* BigBraveBN - algorithm for structural learning of Bayesian networks with a large number of nodes. Tested on networks with up to 500 nodes.
+
+Difference from existing implementations:
+
+
+* Algorithms work on mixed data;
+* Structural learning implements score-functions for mixed data;
+* Parametric learning implements the use of a mixture of Gaussian distributions to approximate continuous distributions;
+* Non-parametric learning of distributions with various user-specified regression and classification models;
+* The algorithm for structural training of large Bayesian networks (> 10 nodes) is based on local training of small networks with their subsequent algorithmic connection.
+
+.. image:: img/BN_gif.gif
+     :target: img/BN_gif.gif
+     :align: center
+     :alt: bn example gif
+
+For example, in terms of data analysis and modeling using Bayesian networks, a pipeline has been implemented to generate synthetic data by sampling from Bayesian networks.
+
+
+
+.. image:: img/synth_gen.png
+   :target: img/synth_gen.png
+   :align: center
+   :height: 300px
+   :width: 600px
+   :alt: synthetics generation
+
+
+How to use
+^^^^^^^^^^
+
+Then the necessary classes are imported from the library:
+
+.. code-block:: python
+
+   import bamt.networks as Nets
+
+Next, a network instance is created and training (structure and parameters) is performed:
+
+.. code-block:: python
+
+   bn = Nets.HybridBN(has_logit=False, use_mixture=True)
+   bn.add_edges(discretized_data, scoring_function=('K2',K2Score))
+   bn.fit_parameters(data)
+
+
+
+Examples & Tutorials
+^^^^^^^^^^^^^^^^^^^^^^
+
+More examples can be found in `tutorials <https://github.com/ITMO-NSS-team/BAMT/tree/master/tutorials>`__  and `Documentation <https://bamt.readthedocs.io/en/latest/examples/learn_save.html>`__.
+
+Publications about BAMT
+^^^^^^^^^^^^^^^^^^^^^^^
+
+We have published several articles about BAMT:
+
+* `Advanced Approach for Distributions Parameters Learning in Bayesian Networks with Gaussian Mixture Models and Discriminative Models <https://www.mdpi.com/2227-7390/11/2/343>`__ (2023)
+* `BigBraveBN: algorithm of structural learning for bayesian networks with a large number of nodes <https://www.sciencedirect.com/science/article/pii/S1877050922016945>`__ (2022)
+* `MIxBN: Library for learning Bayesian networks from mixed data <https://www.sciencedirect.com/science/article/pii/S1877050921020925>`__ (2021)
+* `Oil and Gas Reservoirs Parameters Analysis Using Mixed Learning of Bayesian Networks <https://link.springer.com/chapter/10.1007/978-3-030-77961-0_33>`__ (2021)
+* `Bayesian Networks-based personal data synthesis <https://dl.acm.org/doi/abs/10.1145/3411170.3411243>`__ (2020)
+
+
+Project structure
+^^^^^^^^^^^^^^^^^
+
+The latest stable version of the library is available in the master branch.
+
+It includes the following modules and direcotries:
+
+* `bamt <https://github.com/ITMO-NSS-team/BAMT/tree/master/bamt>`__ - directory with the framework code:
+    * Preprocessing - module for data preprocessing
+    * Networks - module for building and training Bayesian networks
+    * Nodes - module for nodes support of Bayesian networks
+    * Utilities - module for mathematical and graph utilities
+* `data <https://github.com/ITMO-NSS-team/BAMT/tree/master/data>`__  - directory with data for experiments and tests
+* `tests <https://github.com/ITMO-NSS-team/BAMT/tree/master/tests>`__  - directory with unit and integration tests
+* `tutorials <https://github.com/ITMO-NSS-team/BAMT/tree/master/tutorials>`__  - directory with tutorials
+* `docs <https://github.com/ITMO-NSS-team/BAMT/tree/master/docs>`__ - directory with RTD documentation
+
+Preprocessing
+=============
+
+Preprocessor module allows user to transform data according pipeline (similar to pipeline in scikit-learn).
+
+Networks
+========
+
+Three types of networks are implemented:
+
+* HybridBN - Bayesian network with mixed data
+* DiscreteBN - Bayesian network with discrete data
+* ContinuousBN - Bayesian network with continuous data
+
+They are inherited from the abstract class BaseNetwork.
+
+Nodes
+=====
+
+Contains classes for nodes of Bayesian networks.
+
+Utilities
+=========
+
+Utilities module contains mathematical and graph utilities to support the main functionality of the library.
+
+
+Web-BAMT
+^^^^^^^^
+
+A web interface for BAMT is currently under development.
+The repository is available at `web-BAMT <https://github.com/aimclub/Web-BAMT>`__
+
+Contacts
+^^^^^^^^
+
+If you have questions or suggestions, you can contact us at the following address: ideeva@itmo.ru (Irina Deeva)
+
+Our resources:
+
+* `Natural Systems Simulation Team <https://itmo-nss-team.github.io/>`__
+* `NSS team Telegram channel <https://t.me/NSS_group>`__
+* `NSS lab YouTube channel <https://www.youtube.com/@nsslab/videos>`__
+
+.. |docs| image:: https://readthedocs.org/projects/bamt/badge/?version=latest
+    :target: https://bamt.readthedocs.io/en/latest/?badge=latest
+    :alt: Documentation Status
+
+.. |pypi| image:: https://badge.fury.io/py/bamt.svg
+    :target: https://badge.fury.io/py/bamt
+
+.. |py_10| image:: https://img.shields.io/badge/python_3.10-passing-success
+   :alt: Supported Python Versions
+   :target: https://img.shields.io/badge/python_3.10-passing-success
+
+.. |py_8| image:: https://img.shields.io/badge/python_3.8-passing-success
+   :alt: Supported Python Versions
+   :target: https://img.shields.io/badge/python_3.8-passing-success
+
+.. |py_9| image:: https://img.shields.io/badge/python_3.9-passing-success
+   :alt: Supported Python Versions
+   :target: https://img.shields.io/badge/python_3.9-passing-success
+
+.. |license| image:: https://img.shields.io/github/license/ITMO-NSS-team/BAMT
+   :alt: Supported Python Versions
+   :target: https://github.com/ITMO-NSS-team/BAMT/blob/master/LICENCE
+
+.. |downloads_stats| image:: https://static.pepy.tech/personalized-badge/bamt?period=total&units=international_system&left_color=grey&right_color=blue&left_text=downloads
+ :target: https://pepy.tech/project/bamt
+
+.. |downloads_monthly| image:: https://static.pepy.tech/personalized-badge/bamt?period=month&units=international_system&left_color=grey&right_color=blue&left_text=downloads/month
+ :target: https://pepy.tech/project/bamt
+
+.. |downloads_weekly| image:: https://static.pepy.tech/personalized-badge/bamt?period=week&units=international_system&left_color=grey&right_color=blue&left_text=downloads/week
+ :target: https://pepy.tech/project/bamt
+
+.. |Build| image:: https://github.com/ITMO-NSS-team/BAMT/actions/workflows/bamtcodecov.yml/badge.svg
+   :target: https://github.com/ITMO-NSS-team/BAMT/actions/workflows/bamtcodecov.yml
+
+.. |coverage| image:: https://codecov.io/github/ITMO-NSS-team/BAMT/branch/master/graph/badge.svg?token=9ZX37JNIYZ
+   :target: https://codecov.io/github/ITMO-NSS-team/BAMT
 
-setup(**setup_kwargs)
```

