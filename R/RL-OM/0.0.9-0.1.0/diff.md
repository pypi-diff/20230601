# Comparing `tmp/RL_OM-0.0.9.tar.gz` & `tmp/RL_OM-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.0.9.tar", last modified: Thu Jun  1 16:15:13 2023, max compression
+gzip compressed data, was "RL_OM-0.1.0.tar", last modified: Thu Jun  1 16:44:22 2023, max compression
```

## Comparing `RL_OM-0.0.9.tar` & `RL_OM-0.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.013062 RL_OM-0.0.9/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.9/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.9/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-01 16:15:13.012917 RL_OM-0.0.9/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.9/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.006193 RL_OM-0.0.9/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)       22 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)   131239 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.007566 RL_OM-0.0.9/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.008022 RL_OM-0.0.9/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     5364 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/benchmark_agents/eoq.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.008543 RL_OM-0.0.9/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.008945 RL_OM-0.0.9/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)      929 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/processors/eoq_preprocessors.py
--rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.009808 RL_OM-0.0.9/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.010678 RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.011558 RL_OM-0.0.9/RL_OM/agents/rl_agents/pre_specified_agents/
--rw-r--r--   0 magnus     (501) staff       (20)     5053 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)     5269 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    16656 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)     5082 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/sac_discrete.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.0.9/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.012383 RL_OM-0.0.9/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     3784 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/environments/data_generators.py
--rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/environments/feature_converters.py
--rw-r--r--   0 magnus     (501) staff       (20)    10928 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.012714 RL_OM-0.0.9/RL_OM/experiment_functions/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/experiment_functions/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     6834 2023-06-01 16:12:29.000000 RL_OM-0.0.9/RL_OM/experiment_functions/run_experiment.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:15:13.007402 RL_OM-0.0.9/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-01 16:15:12.000000 RL_OM-0.0.9/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-06-01 16:15:12.000000 RL_OM-0.0.9/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-06-01 16:15:12.000000 RL_OM-0.0.9/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2023-06-01 16:15:12.000000 RL_OM-0.0.9/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.9/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2023-06-01 16:15:12.000000 RL_OM-0.0.9/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-06-01 16:15:12.000000 RL_OM-0.0.9/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      989 2023-06-01 16:13:54.000000 RL_OM-0.0.9/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-06-01 16:15:13.013115 RL_OM-0.0.9/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.9/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.092641 RL_OM-0.1.0/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.1.0/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.1.0/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-01 16:44:22.092503 RL_OM-0.1.0/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.1.0/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.085722 RL_OM-0.1.0/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)   131239 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.086952 RL_OM-0.1.0/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.087206 RL_OM-0.1.0/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5364 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/benchmark_agents/eoq.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.087806 RL_OM-0.1.0/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.088282 RL_OM-0.1.0/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)      929 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/processors/eoq_preprocessors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4969 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.089241 RL_OM-0.1.0/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.090152 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14243 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13708 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19176 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19614 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19118 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.090971 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)     5053 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5269 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    16656 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)     5082 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14173 2023-05-29 08:25:22.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-29 08:25:22.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-29 08:25:22.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-29 08:25:22.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-29 08:25:22.000000 RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.091759 RL_OM-0.1.0/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3783 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)     3600 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/environments/data_generators.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1276 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/environments/feature_converters.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10928 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.092268 RL_OM-0.1.0/RL_OM/experiment_functions/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/experiment_functions/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     6834 2023-06-01 16:40:48.000000 RL_OM-0.1.0/RL_OM/experiment_functions/run_experiment.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-06-01 16:44:22.086804 RL_OM-0.1.0/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)     1788 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.1.0/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2023-06-01 16:44:22.000000 RL_OM-0.1.0/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      989 2023-06-01 16:43:27.000000 RL_OM-0.1.0/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2023-06-01 16:44:22.092695 RL_OM-0.1.0/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.1.0/setup.py
```

### Comparing `RL_OM-0.0.9/LICENSE` & `RL_OM-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/PKG-INFO` & `RL_OM-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.0.9
+Version: 0.1.0
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.9/RL_OM/_modidx.py` & `RL_OM-0.1.0/RL_OM/_modidx.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.1.0/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/networks/actors.py` & `RL_OM-0.1.0/RL_OM/agents/networks/actors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/networks/base.py` & `RL_OM-0.1.0/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/networks/critics.py` & `RL_OM-0.1.0/RL_OM/agents/networks/critics.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/processors/eoq_preprocessors.py` & `RL_OM-0.1.0/RL_OM/agents/processors/eoq_preprocessors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/processors/processors.py` & `RL_OM-0.1.0/RL_OM/agents/processors/processors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/sac_discrete.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/algorithms/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/pre_specified_agents/SAC_hybrid_naive.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/sac_discrete.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_discrete.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.1.0/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/environments/calculation_functions.py` & `RL_OM-0.1.0/RL_OM/environments/calculation_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
 
     fixed_ordering_cost_step = get_fixed_ordering_cost(self, order, positive_only = True)
 
     # todo: add variable ordering cost:
         # variable cost positive order ...
         # variable cost negative order would build on overage cost
 
-    self.inventory += action # first, the order will be added to inventory (meaning lead-time is 0)
+    self.inventory += order # first, the order will be added to inventory (meaning lead-time is 0)
 
     self.inventory = np.maximum(self.inventory, 0) # inventory cannot be negative
 
     self.inventory = np.minimum(self.inventory, self.inventory_cap) # inventory cannot be higher than inventory_cap
 
     self.inventory -= self.demand[self.period, :] # Then demand is subtracted from inventory
```

### Comparing `RL_OM-0.0.9/RL_OM/environments/data_generators.py` & `RL_OM-0.1.0/RL_OM/environments/data_generators.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/environments/feature_converters.py` & `RL_OM-0.1.0/RL_OM/environments/feature_converters.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.1.0/RL_OM/environments/multi_period_inventory.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM/experiment_functions/run_experiment.py` & `RL_OM-0.1.0/RL_OM/experiment_functions/run_experiment.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.1.0/RL_OM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.0.9
+Version: 0.1.0
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.9/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.1.0/RL_OM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.9/settings.ini` & `RL_OM-0.1.0/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.0.9
+version = 0.1.0
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.0.9/setup.py` & `RL_OM-0.1.0/setup.py`

 * *Files identical despite different names*

