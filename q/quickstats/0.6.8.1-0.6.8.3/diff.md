# Comparing `tmp/quickstats-0.6.8.1.tar.gz` & `tmp/quickstats-0.6.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quickstats-0.6.8.1.tar", last modified: Mon May 22 12:55:36 2023, max compression
+gzip compressed data, was "quickstats-0.6.8.3.tar", last modified: Wed May 31 23:19:43 2023, max compression
```

## Comparing `quickstats-0.6.8.1.tar` & `quickstats-0.6.8.3.tar`

### file list

```diff
@@ -1,239 +1,241 @@
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:36.000000 quickstats-0.6.8.1/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-05-22 12:55:36.000000 quickstats-0.6.8.1/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/README.md
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:01.000000 quickstats-0.6.8.1/bin/
--rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.1/bin/quickstats
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:01.000000 quickstats-0.6.8.1/quickstats/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-05-20 03:49:33.000000 quickstats-0.6.8.1/quickstats/_version.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:03.000000 quickstats-0.6.8.1/quickstats/analysis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.1/quickstats/analysis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.1/quickstats/analysis/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.1/quickstats/analysis/analysis_path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.1/quickstats/analysis/config_format_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.1/quickstats/analysis/data_loading.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/analysis/data_preprocessing.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.1/quickstats/analysis/event_categorization.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/analysis/multi_class_boundary_tree.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.1/quickstats/analysis/ntuple_conversion_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31665 2023-05-20 03:35:44.000000 quickstats-0.6.8.1/quickstats/analysis/ntuple_process_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8856 2023-05-20 03:36:01.000000 quickstats-0.6.8.1/quickstats/analysis/sample_poly_param_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:04.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    29550 2023-05-20 03:37:08.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/base_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/gaussian_shape_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/normalization_systematics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11815 2023-05-20 03:31:54.000000 quickstats-0.6.8.1/quickstats/analysis/systematics/systematics_evaluation_tool.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:06.000000 quickstats-0.6.8.1/quickstats/clis/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.1/quickstats/clis/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    33847 2023-04-21 13:37:08.000000 quickstats-0.6.8.1/quickstats/clis/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.1/quickstats/clis/inspect_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.1/quickstats/clis/inspect_ws.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-05-03 13:28:30.000000 quickstats-0.6.8.1/quickstats/clis/likelihood_fit.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/clis/likelihood_scan.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/clis/limit_setting.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.8.1/quickstats/clis/processor_cli.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15178 2023-05-11 20:21:35.000000 quickstats-0.6.8.1/quickstats/clis/workspace_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:09.000000 quickstats-0.6.8.1/quickstats/components/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/components/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-21 14:45:07.000000 quickstats-0.6.8.1/quickstats/components/analysis_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13082 2023-05-21 14:42:47.000000 quickstats-0.6.8.1/quickstats/components/analysis_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8656 2023-04-05 18:11:38.000000 quickstats-0.6.8.1/quickstats/components/asimov_generator.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.1/quickstats/components/asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.1/quickstats/components/basics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    31924 2023-05-20 02:58:35.000000 quickstats-0.6.8.1/quickstats/components/extended_minimizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    97245 2023-05-20 03:03:07.000000 quickstats-0.6.8.1/quickstats/components/extended_model.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5539 2023-05-20 03:03:29.000000 quickstats-0.6.8.1/quickstats/components/extended_rfile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15647 2023-05-20 13:23:46.000000 quickstats-0.6.8.1/quickstats/components/likelihood.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:10.000000 quickstats-0.6.8.1/quickstats/components/modelling/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.1/quickstats/components/modelling/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.1/quickstats/components/modelling/component_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.1/quickstats/components/modelling/data_modelling.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.1/quickstats/components/modelling/model_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.1/quickstats/components/modelling/parameter_templates.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.1/quickstats/components/modelling/pdf_fit_tool.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.1/quickstats/components/modelling/tree_data_source.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.8.1/quickstats/components/nuisance_parameter_harmonizer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16921 2023-03-08 10:24:33.000000 quickstats-0.6.8.1/quickstats/components/nuisance_parameter_pull.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:11.000000 quickstats-0.6.8.1/quickstats/components/processors/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.1/quickstats/components/processors/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:15.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/auxiliary.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_as_numpy.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2660 2023-05-21 22:51:18.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_base_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_declare.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      821 2023-05-21 21:47:11.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      937 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_export.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_filter.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_global_variables.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_helper_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_hybrid_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_if_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_if_not_defined.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_load_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_load_macro.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_max.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_mean.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_min.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_nested_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_rdf_action.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_redefine.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1657 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_report.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_safe_alias.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_safe_define.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2204 2022-11-10 10:03:00.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_save.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      654 2022-07-19 21:53:28.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_save_frame.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_stat.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_sum.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_treename.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8316 2023-05-21 20:31:48.000000 quickstats-0.6.8.1/quickstats/components/processors/builtin_methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.1/quickstats/components/processors/roo_config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6646 2023-05-20 03:08:06.000000 quickstats-0.6.8.1/quickstats/components/processors/roo_processor.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.1/quickstats/components/pvalue_toys.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3519 2023-05-20 03:04:57.000000 quickstats-0.6.8.1/quickstats/components/roo_inspector.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.1/quickstats/components/root_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.1/quickstats/components/toy_limit_calculator.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:19.000000 quickstats-0.6.8.1/quickstats/components/workspaces/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.1/quickstats/components/workspaces/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.1/quickstats/components/workspaces/asimov_handler.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.1/quickstats/components/workspaces/core_argument_sets.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.1/quickstats/components/workspaces/sample.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.1/quickstats/components/workspaces/settings.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.1/quickstats/components/workspaces/systematic.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.1/quickstats/components/workspaces/systematics_domain.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    53138 2023-05-20 03:11:16.000000 quickstats-0.6.8.1/quickstats/components/workspaces/ws_comparer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.1/quickstats/components/workspaces/ws_decomposer.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.1/quickstats/components/workspaces/ws_modifier_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_base.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_builder_v1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_builder_v2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    45866 2023-05-20 03:21:08.000000 quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_combiner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    48960 2023-05-20 03:23:15.000000 quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_modifier.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:20.000000 quickstats-0.6.8.1/quickstats/concurrent/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      228 2022-03-27 20:47:33.000000 quickstats-0.6.8.1/quickstats/concurrent/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2654 2023-05-20 03:24:10.000000 quickstats-0.6.8.1/quickstats/concurrent/abstract_runner.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.1/quickstats/concurrent/logging.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5884 2023-05-20 03:24:25.000000 quickstats-0.6.8.1/quickstats/concurrent/parameterised_asymptotic_cls.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10316 2023-05-20 03:24:47.000000 quickstats-0.6.8.1/quickstats/concurrent/parameterised_likelihood.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3983 2022-09-20 17:52:34.000000 quickstats-0.6.8.1/quickstats/concurrent/parameterised_runner.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:22.000000 quickstats-0.6.8.1/quickstats/core/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/core/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/core/abstract_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.1/quickstats/core/configs.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/core/configurable_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/core/dataclass_object.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.1/quickstats/core/decorators.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2201 2023-03-30 08:35:19.000000 quickstats-0.6.8.1/quickstats/core/enums.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.1/quickstats/core/methods.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.1/quickstats/core/path_manager.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.1/quickstats/core/virtual_trees.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:22.000000 quickstats-0.6.8.1/quickstats/interface/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2022-01-31 04:51:23.000000 quickstats-0.6.8.1/quickstats/interface/__init__.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:22.000000 quickstats-0.6.8.1/quickstats/interface/cppyy/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-31 03:26:35.000000 quickstats-0.6.8.1/quickstats/interface/cppyy/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.1/quickstats/interface/cppyy/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12040 2023-05-21 22:08:49.000000 quickstats-0.6.8.1/quickstats/interface/cppyy/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/interface/cppyy/vectorize.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:25.000000 quickstats-0.6.8.1/quickstats/interface/root/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.1/quickstats/interface/root/RooAbsData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.1/quickstats/interface/root/RooAbsPdf.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.1/quickstats/interface/root/RooArgSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.1/quickstats/interface/root/RooCategory.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.1/quickstats/interface/root/RooDataSet.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.1/quickstats/interface/root/RooMsgService.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.1/quickstats/interface/root/RooRealVar.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.1/quickstats/interface/root/TArrayData.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.1/quickstats/interface/root/TF1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.1/quickstats/interface/root/TFile.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.1/quickstats/interface/root/TH1.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.1/quickstats/interface/root/TH2.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.1/quickstats/interface/root/TObject.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.1/quickstats/interface/root/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.1/quickstats/interface/root/helper.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.1/quickstats/interface/root/inspection.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.1/quickstats/interface/root/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.1/quickstats/interface/root/macros.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-02-24 22:56:11.000000 quickstats-0.6.8.1/quickstats/interface/root/roofit_extension.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:01.000000 quickstats-0.6.8.1/quickstats/macros/
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:25.000000 quickstats-0.6.8.1/quickstats/macros/AsymptoticCLsTool/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:25.000000 quickstats-0.6.8.1/quickstats/macros/FlexibleInterpVarMkII/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:26.000000 quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/RooFitExt.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:26.000000 quickstats-0.6.8.1/quickstats/macros/ResponseFunction/
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.1/quickstats/macros/ResponseFunction/ResponseFunction.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:26.000000 quickstats-0.6.8.1/quickstats/macros/RooTwoSidedCBShape/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:27.000000 quickstats-0.6.8.1/quickstats/maths/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.1/quickstats/maths/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1130 2023-03-10 17:21:22.000000 quickstats-0.6.8.1/quickstats/maths/interpolation.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.1/quickstats/maths/numerics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    24166 2023-05-20 11:38:14.000000 quickstats-0.6.8.1/quickstats/maths/statistics.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.1/quickstats/maths/statistics_jitted.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.1/quickstats/maths/symbolics.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:27.000000 quickstats-0.6.8.1/quickstats/parsers/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.1/quickstats/parsers/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.1/quickstats/parsers/config_parser.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15875 2023-04-11 14:45:10.000000 quickstats-0.6.8.1/quickstats/parsers/param_parser.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:33.000000 quickstats-0.6.8.1/quickstats/plots/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.1/quickstats/plots/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12818 2023-04-27 22:46:00.000000 quickstats-0.6.8.1/quickstats/plots/abstract_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.1/quickstats/plots/bidirectional_bar_chart.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.1/quickstats/plots/collective_data_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.1/quickstats/plots/color_schemes.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.1/quickstats/plots/core.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.1/quickstats/plots/correlation_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5968 2023-03-22 14:09:34.000000 quickstats-0.6.8.1/quickstats/plots/general_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.1/quickstats/plots/general_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.1/quickstats/plots/histo_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.1/quickstats/plots/hypotest_inverter_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5749 2023-04-06 23:36:13.000000 quickstats-0.6.8.1/quickstats/plots/likelihood_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9916 2023-04-10 17:13:17.000000 quickstats-0.6.8.1/quickstats/plots/likelihood_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.1/quickstats/plots/likelihood_scan_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    26316 2023-04-17 19:54:51.000000 quickstats-0.6.8.1/quickstats/plots/np_ranking_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.1/quickstats/plots/pdf_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.1/quickstats/plots/sample_purity_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.1/quickstats/plots/score_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.1/quickstats/plots/stat_plot_config.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.8.1/quickstats/plots/template.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.1/quickstats/plots/test_statistic_distribution_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.1/quickstats/plots/upper_limit_1D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-04-14 12:19:16.000000 quickstats-0.6.8.1/quickstats/plots/upper_limit_2D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.1/quickstats/plots/upper_limit_3D_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.8.1/quickstats/plots/upper_limit_benchmark_plot.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    28679 2023-05-20 03:29:27.000000 quickstats-0.6.8.1/quickstats/plots/variable_distribution_plot.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:34.000000 quickstats-0.6.8.1/quickstats/resources/
--rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.1/quickstats/resources/default_workspace_extensions.json
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.1/quickstats/root_checker.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:34.000000 quickstats-0.6.8.1/quickstats/stylesheets/
--rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.1/quickstats/stylesheets/quick_default.mplstyle
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:36.000000 quickstats-0.6.8.1/quickstats/utils/
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.1/quickstats/utils/__init__.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    10897 2023-03-07 15:00:08.000000 quickstats-0.6.8.1/quickstats/utils/common_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.1/quickstats/utils/condor_tasks.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    16140 2023-03-25 23:04:40.000000 quickstats-0.6.8.1/quickstats/utils/data_conversion.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.1/quickstats/utils/hep_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     6634 2023-05-20 02:56:51.000000 quickstats-0.6.8.1/quickstats/utils/io.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.1/quickstats/utils/process_tools.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    26227 2023-05-20 21:07:10.000000 quickstats-0.6.8.1/quickstats/utils/roofit_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.1/quickstats/utils/roostats_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-05-20 03:26:53.000000 quickstats-0.6.8.1/quickstats/utils/root_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1347 2023-05-21 21:45:53.000000 quickstats-0.6.8.1/quickstats/utils/string_utils.py
--rw-r--r--   0 chlcheng (124202) zp        (1307)    15011 2023-03-14 18:38:57.000000 quickstats-0.6.8.1/quickstats/utils/xml_tools.py
-drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-22 12:55:02.000000 quickstats-0.6.8.1/quickstats.egg-info/
--rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-05-22 12:54:53.000000 quickstats-0.6.8.1/quickstats.egg-info/PKG-INFO
--rw-r--r--   0 chlcheng (124202) zp        (1307)     8968 2023-05-22 12:54:54.000000 quickstats-0.6.8.1/quickstats.egg-info/SOURCES.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-05-22 12:54:53.000000 quickstats-0.6.8.1/quickstats.egg-info/dependency_links.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-05-22 12:54:53.000000 quickstats-0.6.8.1/quickstats.egg-info/requires.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-05-22 12:54:53.000000 quickstats-0.6.8.1/quickstats.egg-info/top_level.txt
--rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-05-22 12:55:36.000000 quickstats-0.6.8.1/setup.cfg
--rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.1/setup.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3567 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/README.md
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:41.000000 quickstats-0.6.8.3/bin/
+-rwxr-xr-x   0 chlcheng (124202) zp        (1307)     1651 2023-05-11 20:22:22.000000 quickstats-0.6.8.3/bin/quickstats
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:41.000000 quickstats-0.6.8.3/quickstats/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      626 2023-05-31 15:23:38.000000 quickstats-0.6.8.3/quickstats/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       24 2023-05-31 20:15:22.000000 quickstats-0.6.8.3/quickstats/_version.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/analysis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      428 2023-02-08 03:42:01.000000 quickstats-0.6.8.3/quickstats/analysis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-02-08 08:27:54.000000 quickstats-0.6.8.3/quickstats/analysis/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4191 2023-02-08 05:24:19.000000 quickstats-0.6.8.3/quickstats/analysis/analysis_path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22807 2023-03-14 14:12:10.000000 quickstats-0.6.8.3/quickstats/analysis/config_format_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    41649 2023-05-20 03:33:19.000000 quickstats-0.6.8.3/quickstats/analysis/data_loading.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1303 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/quickstats/analysis/data_preprocessing.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    85935 2023-05-20 03:34:59.000000 quickstats-0.6.8.3/quickstats/analysis/event_categorization.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8060 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/quickstats/analysis/multi_class_boundary_tree.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9286 2023-05-20 03:35:21.000000 quickstats-0.6.8.3/quickstats/analysis/ntuple_conversion_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31665 2023-05-20 03:35:44.000000 quickstats-0.6.8.3/quickstats/analysis/ntuple_process_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8856 2023-05-20 03:36:01.000000 quickstats-0.6.8.3/quickstats/analysis/sample_poly_param_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      241 2023-03-07 22:17:53.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29550 2023-05-20 03:37:08.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/base_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9774 2023-04-03 12:27:59.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/gaussian_shape_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6796 2023-03-14 18:47:57.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/normalization_systematics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11815 2023-05-20 03:31:54.000000 quickstats-0.6.8.3/quickstats/analysis/systematics/systematics_evaluation_tool.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/clis/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-05-17 11:53:22.000000 quickstats-0.6.8.3/quickstats/clis/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    35299 2023-05-31 19:41:46.000000 quickstats-0.6.8.3/quickstats/clis/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2174 2023-02-14 22:30:46.000000 quickstats-0.6.8.3/quickstats/clis/inspect_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2573 2023-02-14 22:27:47.000000 quickstats-0.6.8.3/quickstats/clis/inspect_ws.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16785 2023-05-03 13:28:30.000000 quickstats-0.6.8.3/quickstats/clis/likelihood_fit.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7818 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/quickstats/clis/likelihood_scan.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8575 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/quickstats/clis/limit_setting.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1327 2023-02-14 22:29:19.000000 quickstats-0.6.8.3/quickstats/clis/processor_cli.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15178 2023-05-11 20:21:35.000000 quickstats-0.6.8.3/quickstats/clis/workspace_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/components/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      849 2023-05-30 19:49:31.000000 quickstats-0.6.8.3/quickstats/components/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3152 2023-05-27 07:22:07.000000 quickstats-0.6.8.3/quickstats/components/analysis_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13395 2023-05-27 02:29:45.000000 quickstats-0.6.8.3/quickstats/components/analysis_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8656 2023-04-05 18:11:38.000000 quickstats-0.6.8.3/quickstats/components/asimov_generator.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    30804 2023-05-20 02:55:29.000000 quickstats-0.6.8.3/quickstats/components/asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2464 2023-01-04 09:02:54.000000 quickstats-0.6.8.3/quickstats/components/basics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    31916 2023-05-31 14:47:47.000000 quickstats-0.6.8.3/quickstats/components/extended_minimizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    98139 2023-05-31 20:12:21.000000 quickstats-0.6.8.3/quickstats/components/extended_model.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5539 2023-05-20 03:03:29.000000 quickstats-0.6.8.3/quickstats/components/extended_rfile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15647 2023-05-25 18:13:48.000000 quickstats-0.6.8.3/quickstats/components/likelihood.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/components/modelling/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      207 2022-09-18 16:06:32.000000 quickstats-0.6.8.3/quickstats/components/modelling/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2520 2022-09-18 05:43:28.000000 quickstats-0.6.8.3/quickstats/components/modelling/component_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20157 2023-05-20 03:06:27.000000 quickstats-0.6.8.3/quickstats/components/modelling/data_modelling.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      767 2022-09-18 12:07:18.000000 quickstats-0.6.8.3/quickstats/components/modelling/model_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4562 2022-09-18 16:32:35.000000 quickstats-0.6.8.3/quickstats/components/modelling/parameter_templates.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5578 2023-05-20 03:07:18.000000 quickstats-0.6.8.3/quickstats/components/modelling/pdf_fit_tool.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3532 2023-05-20 03:07:28.000000 quickstats-0.6.8.3/quickstats/components/modelling/tree_data_source.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10839 2022-04-07 03:18:15.000000 quickstats-0.6.8.3/quickstats/components/nuisance_parameter_harmonizer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    17291 2023-05-31 18:05:59.000000 quickstats-0.6.8.3/quickstats/components/nuisance_parameter_pull.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12390 2023-05-31 15:55:13.000000 quickstats-0.6.8.3/quickstats/components/nuisance_parameter_ranking.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/components/processors/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      205 2022-07-19 21:07:01.000000 quickstats-0.6.8.3/quickstats/components/processors/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2066 2023-05-19 15:52:58.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      111 2022-07-21 18:27:25.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/auxiliary.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1072 2023-03-05 12:07:49.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1082 2022-07-19 21:51:30.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_as_numpy.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2660 2023-05-21 22:51:18.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_base_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      784 2023-05-21 22:53:11.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_declare.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      870 2023-05-23 18:53:54.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      937 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_export.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1164 2022-07-21 15:20:21.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_filter.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1076 2022-08-29 06:56:49.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_global_variables.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      506 2022-07-19 21:00:22.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_helper_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      586 2022-07-19 21:52:08.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_hybrid_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      697 2022-07-21 18:29:41.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_if_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      704 2022-07-21 18:48:13.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_if_not_defined.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-19 21:50:41.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_load_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1121 2023-05-21 22:55:55.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_load_macro.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:20.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_max.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      142 2022-07-19 20:41:10.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_mean.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:40:51.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_min.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      636 2022-07-21 18:30:05.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_nested_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      462 2022-07-19 20:22:13.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_rdf_action.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2022-07-19 20:28:28.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_redefine.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1677 2023-05-22 21:51:19.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_report.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1382 2023-03-05 12:11:04.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_safe_alias.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      454 2022-07-19 20:28:24.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_safe_define.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2204 2022-11-10 10:03:00.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_save.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      654 2022-07-19 21:53:28.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_save_frame.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1194 2022-07-19 21:50:00.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_stat.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      140 2022-07-19 20:39:49.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_sum.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      523 2022-07-19 21:54:23.000000 quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_treename.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8953 2023-05-28 22:27:10.000000 quickstats-0.6.8.3/quickstats/components/processors/builtin_methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6504 2023-05-21 22:51:45.000000 quickstats-0.6.8.3/quickstats/components/processors/roo_config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6646 2023-05-20 03:08:06.000000 quickstats-0.6.8.3/quickstats/components/processors/roo_processor.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5397 2021-09-16 21:06:55.000000 quickstats-0.6.8.3/quickstats/components/pvalue_toys.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3519 2023-05-20 03:04:57.000000 quickstats-0.6.8.3/quickstats/components/roo_inspector.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3083 2023-05-20 03:04:47.000000 quickstats-0.6.8.3/quickstats/components/root_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    21336 2023-05-20 03:06:10.000000 quickstats-0.6.8.3/quickstats/components/toy_limit_calculator.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/components/workspaces/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      591 2023-05-11 12:58:08.000000 quickstats-0.6.8.3/quickstats/components/workspaces/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9877 2023-05-20 03:10:01.000000 quickstats-0.6.8.3/quickstats/components/workspaces/asimov_handler.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1727 2023-05-20 03:10:09.000000 quickstats-0.6.8.3/quickstats/components/workspaces/core_argument_sets.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1997 2023-01-09 17:03:21.000000 quickstats-0.6.8.3/quickstats/components/workspaces/sample.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1991 2023-03-11 17:09:50.000000 quickstats-0.6.8.3/quickstats/components/workspaces/settings.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8295 2023-05-20 03:10:27.000000 quickstats-0.6.8.3/quickstats/components/workspaces/systematic.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2303 2023-01-08 18:43:45.000000 quickstats-0.6.8.3/quickstats/components/workspaces/systematics_domain.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    53138 2023-05-20 03:11:16.000000 quickstats-0.6.8.3/quickstats/components/workspaces/ws_comparer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     8837 2023-05-20 03:11:35.000000 quickstats-0.6.8.3/quickstats/components/workspaces/ws_decomposer.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1756 2022-04-20 13:20:42.000000 quickstats-0.6.8.3/quickstats/components/workspaces/ws_modifier_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10859 2023-05-20 03:12:06.000000 quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_base.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    87030 2023-05-20 03:16:06.000000 quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_builder_v1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    76213 2023-05-20 03:19:36.000000 quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_builder_v2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    45866 2023-05-20 03:21:08.000000 quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_combiner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    48960 2023-05-20 03:23:15.000000 quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_modifier.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/concurrent/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      306 2023-05-31 15:27:50.000000 quickstats-0.6.8.3/quickstats/concurrent/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3064 2023-05-31 15:10:38.000000 quickstats-0.6.8.3/quickstats/concurrent/abstract_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      627 2022-05-16 01:31:37.000000 quickstats-0.6.8.3/quickstats/concurrent/logging.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5239 2023-05-31 16:02:49.000000 quickstats-0.6.8.3/quickstats/concurrent/nuisance_parameter_ranking_runner.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5891 2023-05-31 15:28:21.000000 quickstats-0.6.8.3/quickstats/concurrent/parameterised_asymptotic_cls.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10275 2023-05-31 15:28:38.000000 quickstats-0.6.8.3/quickstats/concurrent/parameterised_likelihood.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3963 2023-05-31 15:27:15.000000 quickstats-0.6.8.3/quickstats/concurrent/parameterised_runner.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/core/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      398 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/core/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      811 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/core/abstract_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    20587 2023-05-20 03:28:17.000000 quickstats-0.6.8.3/quickstats/core/configs.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2198 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/core/configurable_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      541 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/core/dataclass_object.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      971 2023-05-20 03:27:42.000000 quickstats-0.6.8.3/quickstats/core/decorators.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2296 2023-05-23 21:10:32.000000 quickstats-0.6.8.3/quickstats/core/enums.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6651 2023-02-14 22:36:19.000000 quickstats-0.6.8.3/quickstats/core/methods.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9057 2023-02-08 05:24:13.000000 quickstats-0.6.8.3/quickstats/core/path_manager.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2952 2022-07-21 15:05:33.000000 quickstats-0.6.8.3/quickstats/core/virtual_trees.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/interface/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       66 2023-05-31 15:27:05.000000 quickstats-0.6.8.3/quickstats/interface/__init__.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:42.000000 quickstats-0.6.8.3/quickstats/interface/cppyy/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2023-05-31 20:08:24.000000 quickstats-0.6.8.3/quickstats/interface/cppyy/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      513 2022-01-31 03:37:54.000000 quickstats-0.6.8.3/quickstats/interface/cppyy/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12546 2023-05-28 20:56:33.000000 quickstats-0.6.8.3/quickstats/interface/cppyy/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4433 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/interface/cppyy/vectorize.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/interface/root/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      621 2022-09-16 14:23:50.000000 quickstats-0.6.8.3/quickstats/interface/root/RooAbsData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9855 2023-05-20 12:12:25.000000 quickstats-0.6.8.3/quickstats/interface/root/RooAbsPdf.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      420 2022-08-23 02:59:13.000000 quickstats-0.6.8.3/quickstats/interface/root/RooArgSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1182 2023-03-12 16:17:52.000000 quickstats-0.6.8.3/quickstats/interface/root/RooCategory.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    44679 2023-05-20 12:08:58.000000 quickstats-0.6.8.3/quickstats/interface/root/RooDataSet.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      588 2022-08-23 03:02:49.000000 quickstats-0.6.8.3/quickstats/interface/root/RooMsgService.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5451 2023-05-11 15:17:32.000000 quickstats-0.6.8.3/quickstats/interface/root/RooRealVar.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      130 2022-01-25 17:28:15.000000 quickstats-0.6.8.3/quickstats/interface/root/TArrayData.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      983 2023-01-04 09:02:55.000000 quickstats-0.6.8.3/quickstats/interface/root/TF1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1995 2023-02-28 09:57:47.000000 quickstats-0.6.8.3/quickstats/interface/root/TFile.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13146 2023-05-20 12:06:46.000000 quickstats-0.6.8.3/quickstats/interface/root/TH1.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5707 2023-05-03 13:36:36.000000 quickstats-0.6.8.3/quickstats/interface/root/TH2.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      571 2022-08-23 03:14:20.000000 quickstats-0.6.8.3/quickstats/interface/root/TObject.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      856 2023-03-12 13:27:02.000000 quickstats-0.6.8.3/quickstats/interface/root/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1069 2022-08-23 02:53:43.000000 quickstats-0.6.8.3/quickstats/interface/root/helper.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-03-24 19:40:20.000000 quickstats-0.6.8.3/quickstats/interface/root/inspection.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      235 2022-08-23 02:57:43.000000 quickstats-0.6.8.3/quickstats/interface/root/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    19576 2023-05-11 13:39:17.000000 quickstats-0.6.8.3/quickstats/interface/root/macros.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5637 2023-05-27 06:13:47.000000 quickstats-0.6.8.3/quickstats/interface/root/roofit_extension.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:41.000000 quickstats-0.6.8.3/quickstats/macros/
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/macros/AsymptoticCLsTool/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     7083 2021-08-19 17:39:48.000000 quickstats-0.6.8.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1511 2021-06-11 19:36:10.000000 quickstats-0.6.8.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/macros/FlexibleInterpVarMkII/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12372 2022-03-27 23:04:56.000000 quickstats-0.6.8.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2498 2022-03-27 22:34:26.000000 quickstats-0.6.8.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1231 2022-05-07 02:55:05.000000 quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10322 2022-05-11 00:00:32.000000 quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/RooFitExt.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3429 2022-05-10 23:59:25.000000 quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/RooFitExt.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/macros/ResponseFunction/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13755 2023-04-25 19:09:18.000000 quickstats-0.6.8.3/quickstats/macros/ResponseFunction/ResponseFunction.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2982 2023-04-25 19:07:54.000000 quickstats-0.6.8.3/quickstats/macros/ResponseFunction/ResponseFunction.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/macros/RooTwoSidedCBShape/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3689 2022-03-24 20:47:13.000000 quickstats-0.6.8.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1358 2021-03-16 05:44:03.000000 quickstats-0.6.8.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/maths/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2022-02-07 21:49:51.000000 quickstats-0.6.8.3/quickstats/maths/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1130 2023-03-10 17:21:22.000000 quickstats-0.6.8.3/quickstats/maths/interpolation.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5548 2023-03-30 08:30:53.000000 quickstats-0.6.8.3/quickstats/maths/numerics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    24166 2023-05-20 11:38:14.000000 quickstats-0.6.8.3/quickstats/maths/statistics.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3506 2023-05-15 01:04:06.000000 quickstats-0.6.8.3/quickstats/maths/statistics_jitted.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      613 2022-09-23 13:42:24.000000 quickstats-0.6.8.3/quickstats/maths/symbolics.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/parsers/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      113 2022-04-20 10:58:59.000000 quickstats-0.6.8.3/quickstats/parsers/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      337 2022-04-20 10:57:08.000000 quickstats-0.6.8.3/quickstats/parsers/config_parser.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15883 2023-05-31 15:27:08.000000 quickstats-0.6.8.3/quickstats/parsers/param_parser.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/plots/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1441 2023-03-29 12:38:13.000000 quickstats-0.6.8.3/quickstats/plots/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12818 2023-04-27 22:46:00.000000 quickstats-0.6.8.3/quickstats/plots/abstract_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    14145 2023-03-29 14:21:34.000000 quickstats-0.6.8.3/quickstats/plots/bidirectional_bar_chart.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1634 2022-09-07 04:28:06.000000 quickstats-0.6.8.3/quickstats/plots/collective_data_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     2750 2023-04-01 10:15:48.000000 quickstats-0.6.8.3/quickstats/plots/color_schemes.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5180 2023-05-17 15:59:58.000000 quickstats-0.6.8.3/quickstats/plots/core.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4007 2023-05-17 16:00:48.000000 quickstats-0.6.8.3/quickstats/plots/correlation_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5968 2023-03-22 14:09:34.000000 quickstats-0.6.8.3/quickstats/plots/general_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    22775 2022-09-07 07:18:02.000000 quickstats-0.6.8.3/quickstats/plots/general_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     3731 2022-09-09 08:30:51.000000 quickstats-0.6.8.3/quickstats/plots/histo_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6100 2023-03-21 16:34:42.000000 quickstats-0.6.8.3/quickstats/plots/hypotest_inverter_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5834 2023-05-25 20:07:07.000000 quickstats-0.6.8.3/quickstats/plots/likelihood_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9916 2023-04-10 17:13:17.000000 quickstats-0.6.8.3/quickstats/plots/likelihood_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      219 2021-04-19 13:56:55.000000 quickstats-0.6.8.3/quickstats/plots/likelihood_scan_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    29009 2023-05-31 19:45:49.000000 quickstats-0.6.8.3/quickstats/plots/np_ranking_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    25696 2023-04-18 01:26:39.000000 quickstats-0.6.8.3/quickstats/plots/pdf_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5059 2023-02-06 09:15:46.000000 quickstats-0.6.8.3/quickstats/plots/sample_purity_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10293 2023-03-27 13:06:51.000000 quickstats-0.6.8.3/quickstats/plots/score_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4123 2023-01-04 09:02:56.000000 quickstats-0.6.8.3/quickstats/plots/stat_plot_config.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    18642 2023-04-02 13:33:12.000000 quickstats-0.6.8.3/quickstats/plots/template.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13688 2022-07-29 18:50:11.000000 quickstats-0.6.8.3/quickstats/plots/test_statistic_distribution_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    11061 2023-01-04 09:02:56.000000 quickstats-0.6.8.3/quickstats/plots/upper_limit_1D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12201 2023-04-14 12:19:16.000000 quickstats-0.6.8.3/quickstats/plots/upper_limit_2D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    13186 2022-08-18 13:35:04.000000 quickstats-0.6.8.3/quickstats/plots/upper_limit_3D_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     5069 2022-08-24 13:05:29.000000 quickstats-0.6.8.3/quickstats/plots/upper_limit_benchmark_plot.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    28679 2023-05-20 03:29:27.000000 quickstats-0.6.8.3/quickstats/plots/variable_distribution_plot.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/resources/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       90 2023-03-20 15:25:27.000000 quickstats-0.6.8.3/quickstats/resources/default_workspace_extensions.json
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4530 2022-04-08 03:20:04.000000 quickstats-0.6.8.3/quickstats/root_checker.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/stylesheets/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      379 2021-10-20 08:52:20.000000 quickstats-0.6.8.3/quickstats/stylesheets/quick_default.mplstyle
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/quickstats/utils/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-11-16 06:49:21.000000 quickstats-0.6.8.3/quickstats/utils/__init__.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    10949 2023-05-27 07:03:50.000000 quickstats-0.6.8.3/quickstats/utils/common_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        0 2021-09-21 13:14:14.000000 quickstats-0.6.8.3/quickstats/utils/condor_tasks.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    16140 2023-03-25 23:04:40.000000 quickstats-0.6.8.3/quickstats/utils/data_conversion.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1187 2022-08-27 16:49:16.000000 quickstats-0.6.8.3/quickstats/utils/hep_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     6812 2023-05-31 13:27:25.000000 quickstats-0.6.8.3/quickstats/utils/io.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)      335 2021-05-17 13:11:29.000000 quickstats-0.6.8.3/quickstats/utils/process_tools.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    26227 2023-05-20 21:07:10.000000 quickstats-0.6.8.3/quickstats/utils/roofit_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9267 2021-11-23 21:10:48.000000 quickstats-0.6.8.3/quickstats/utils/roostats_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    12379 2023-05-20 03:26:53.000000 quickstats-0.6.8.3/quickstats/utils/root_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1347 2023-05-21 21:45:53.000000 quickstats-0.6.8.3/quickstats/utils/string_utils.py
+-rw-r--r--   0 chlcheng (124202) zp        (1307)    15011 2023-03-14 18:38:57.000000 quickstats-0.6.8.3/quickstats/utils/xml_tools.py
+drwxr-xr-x   0 chlcheng (124202) zp        (1307)        0 2023-05-31 23:19:41.000000 quickstats-0.6.8.3/quickstats.egg-info/
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     4011 2023-05-31 23:19:40.000000 quickstats-0.6.8.3/quickstats.egg-info/PKG-INFO
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     9079 2023-05-31 23:19:41.000000 quickstats-0.6.8.3/quickstats.egg-info/SOURCES.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)        1 2023-05-31 23:19:40.000000 quickstats-0.6.8.3/quickstats.egg-info/dependency_links.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       39 2023-05-31 23:19:40.000000 quickstats-0.6.8.3/quickstats.egg-info/requires.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       11 2023-05-31 23:19:40.000000 quickstats-0.6.8.3/quickstats.egg-info/top_level.txt
+-rw-r--r--   0 chlcheng (124202) zp        (1307)       38 2023-05-31 23:19:43.000000 quickstats-0.6.8.3/setup.cfg
+-rw-r--r--   0 chlcheng (124202) zp        (1307)     1687 2023-01-04 09:02:56.000000 quickstats-0.6.8.3/setup.py
```

### Comparing `quickstats-0.6.8.1/PKG-INFO` & `quickstats-0.6.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.1
+Version: 0.6.8.3
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.1/README.md` & `quickstats-0.6.8.3/README.md`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/bin/quickstats` & `quickstats-0.6.8.3/bin/quickstats`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/__init__.py` & `quickstats-0.6.8.3/quickstats/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/analysis_base.py` & `quickstats-0.6.8.3/quickstats/analysis/analysis_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/analysis_path_manager.py` & `quickstats-0.6.8.3/quickstats/analysis/analysis_path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/config_format_templates.py` & `quickstats-0.6.8.3/quickstats/analysis/config_format_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/data_loading.py` & `quickstats-0.6.8.3/quickstats/analysis/data_loading.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/data_preprocessing.py` & `quickstats-0.6.8.3/quickstats/analysis/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/event_categorization.py` & `quickstats-0.6.8.3/quickstats/analysis/event_categorization.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/multi_class_boundary_tree.py` & `quickstats-0.6.8.3/quickstats/analysis/multi_class_boundary_tree.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/ntuple_conversion_tool.py` & `quickstats-0.6.8.3/quickstats/analysis/ntuple_conversion_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/ntuple_process_tool.py` & `quickstats-0.6.8.3/quickstats/analysis/ntuple_process_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/sample_poly_param_tool.py` & `quickstats-0.6.8.3/quickstats/analysis/sample_poly_param_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/systematics/base_systematics.py` & `quickstats-0.6.8.3/quickstats/analysis/systematics/base_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/systematics/gaussian_shape_systematics.py` & `quickstats-0.6.8.3/quickstats/analysis/systematics/gaussian_shape_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/systematics/normalization_systematics.py` & `quickstats-0.6.8.3/quickstats/analysis/systematics/normalization_systematics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/analysis/systematics/systematics_evaluation_tool.py` & `quickstats-0.6.8.3/quickstats/analysis/systematics/systematics_evaluation_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/clis/core.py` & `quickstats-0.6.8.3/quickstats/clis/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,53 +6,51 @@
     def type_cast_value(self, ctx, value):
         try:
             return [i.strip() for i in value.split(",")]
         except:
             raise click.BadParameter(value)
 
 @click.command(name='run_pulls')
-@click.option('-i', '--input_file', required=True, 
+@click.option('-i', '--input_file', 'filename', required=True, 
               help='Path to the input workspace file')
-@click.option('-x', '--poi', required=True,
-              help='POIs to measure')
+@click.option('-x', '--poi', 'poi_name', default=None,
+              help='POI to measure NP impact on')
 @click.option('-o', '--outdir', default="pulls", show_default=True,
               help='Output directory')
-@click.option('-w', '--workspace', default=None, 
+@click.option('-w', '--workspace', 'ws_name', default=None, 
               help='Name of workspace. Auto-detect by default.')
-@click.option('-m', '--model_config', default=None, 
+@click.option('-m', '--model_config', 'mc_name', default=None, 
               help='Name of model config. Auto-detect by default.')
-@click.option('-d', '--data', default='combData', show_default=True,
+@click.option('-d', '--data', 'data_name', default='combData', show_default=True,
               help='Name of dataset')
-@click.option('-p', '--parameter', default='', show_default=True,
-              help='Nuisance parameter(s) to run pulls on.'+\
+@click.option('--filter', 'filter_expr', default=None, show_default=True,
+              help='Filter nuisance parameter(s) to run pulls and impacts on.'+\
                    'Multiple parameters are separated by commas.'+\
-                   'Wildcards are accepted. All NPs are run by default.')
-@click.option('-r', '--profile', default=None, show_default=True,
+                   'Wildcards are accepted. All NPs are included by default.')
+@click.option('-r', '--profile', 'profile_param', default=None, show_default=True,
               help='Parameters to profile')
-@click.option('-f', '--fix', default=None, show_default=True,
+@click.option('-f', '--fix', 'fix_param', default=None, show_default=True,
               help='Parameters to fix')
-@click.option('-s', '--snapshot', default="nominalNuis", show_default=True,
+@click.option('-s', '--snapshot', 'snapshot_name', default=None, show_default=True,
               help='Name of initial snapshot')
 @click.option('-t', '--minimizer_type', default="Minuit2", show_default=True,
               help='Minimizer type')
 @click.option('-a', '--minimizer_algo', default="Migrad", show_default=True,
               help='Minimizer algorithm')
 @click.option('-c', '--num_cpu', type=int, default=1, show_default=True,
               help='Number of CPUs to use per parameter')
-@click.option('--binned/--unbinned', default=True, show_default=True,
+@click.option('--binned/--unbinned', 'binned_likelihood', default=True, show_default=True,
               help='Binned likelihood')
 @click.option('-q', '--precision', type=float, default=0.001, show_default=True,
               help='Precision for scan')
 @click.option('-e', '--eps', type=float, default=1.0, show_default=True,
               help='Convergence criterium')
-@click.option('--retry', type=int, default=0, show_default=True,
+@click.option('--retry', type=int, default=2, show_default=True,
               help='Maximum number of retries upon a failed fit')
-@click.option('-l', '--log_level', default="INFO", show_default=True,
-              help='Log level')
-@click.option('--print_level', type=int, default=1, show_default=True,
+@click.option('--print_level', type=int, default=-1, show_default=True,
               help='Minimizer print level')
 @click.option('--strategy', type=int, default=1, show_default=True,
               help='Default strategy')
 @click.option('--fix-cache/--no-fix-cache', default=True, show_default=True,
               help='Fix StarMomentMorph cache')
 @click.option('--fix-multi/--no-fix-multi', default=True, show_default=True,
               help='Fix MultiPdf level 2')
@@ -71,24 +69,45 @@
                    'density at the bin centre')
 @click.option('--parallel', type=int, default=-1, show_default=True,
               help='\b\n Parallelize job across the N workers.'
                    '\b\n Case  0: Jobs are run sequentially (for debugging).'
                    '\b\n Case -1: Jobs are run across N_CPU workers.')
 @click.option('--cache/--no-cache', default=True, show_default=True,
               help='Cache existing result')
-@click.option('--exclude', default="", show_default=True,
-              help='Exclude NPs (wildcard is accepted)')
+@click.option('--exclude', 'exclude_expr', default=None, show_default=True,
+              help='Exclude NPs to run pulls and impacts on. '+\
+                   'Multiple parameters are separated by commas.'+\
+                   'Wildcards are accepted.')
+@click.option('--save_log/--skip_log', default=True, show_default=True,
+              help='Save log file.')
 @click.option('--constrained_only/--any_nuis', default=True, show_default=True,
               help='Whether to include constrained nuisance parameters only')
+@click.option('--version', type=click.Choice(['1', '2']), default='2', show_default=True,
+              help='Version of tool to use (Choose between 1 and 2).')
+@click.option('-v', '--verbosity', default='INFO', show_default=True,
+              type=click.Choice(["DEBUG", "INFO", "WARNING", "ERROR"], case_sensitive=False),
+              help='Verbosity level.')
 def run_pulls(**kwargs):
     """
     Tool for computing NP pulls and impacts
     """
-    from quickstats.components import NuisanceParameterPull
-    NuisanceParameterPull().run_pulls(**kwargs)
+    version = kwargs.pop('version')
+    if version == '1':
+        from quickstats.components import NuisanceParameterPull
+        NuisanceParameterPull().run_pulls(**kwargs)
+    elif version == '2':
+        from quickstats.concurrent import NuisanceParameterRankingRunner
+        init_kwargs = {}
+        for key in ['filename', 'filter_expr', 'exclude_expr', 'poi_name',
+                    'data_name', 'cache', 'outdir', 'constrained_only',
+                    'save_log', 'parallel', 'verbosity']:
+            init_kwargs[key] = kwargs.pop(key)
+        init_kwargs['config'] = kwargs
+        runner = NuisanceParameterRankingRunner(**init_kwargs)
+        runner.run()
     
 @click.command(name='plot_pulls')
 @click.option('-i', '--inputdir', required=True, help='Path to directory containing pull results')
 @click.option('-p', '--poi', default=None, help='Parameter of interest for plotting impact')
 @click.option('-n', '--n_rank', type=int, default=None, help='Total number of NP to rank')
 @click.option('-m', '--rank_per_plot', type=int, default=20, show_default=True,
               help='Number of NP to show in a single plot')
@@ -150,21 +169,24 @@
 @click.option('-o', '--outname', default='ranking', show_default=True,
               help='Output file name prefix')
 @click.option('--style', default='default', show_default=True,
               help='Plotting style. Built-in styles are "default" and "trex".'+\
                    'Specify path to yaml file to set custom plotting style.')
 @click.option('--fix_axis_scale/--free_axis_scale', default=True, show_default=True,
               help='Fix the axis scale across all ranking plots')
+@click.option('--version', type=click.Choice(['1', '2']), default='2', show_default=True,
+              help='Version of tool to use (Choose between 1 and 2).')
 def plot_pulls(**kwargs):
     """
     Tool for plotting NP pulls and impact rankings
     """    
     from quickstats.plots.np_ranking_plot import NPRankingPlot
     inputdir, poi = kwargs.pop('inputdir'), kwargs.pop('poi')
-    ranking_plot = NPRankingPlot(inputdir, poi)
+    version = kwargs.pop('version')
+    ranking_plot = NPRankingPlot(inputdir, poi, version=version)
     ranking_plot.plot(**kwargs)
 
 @click.command(name='cls_limit')
 @click.option('-i', '--input_file', 'filename', required=True, 
               help='Path to the input workspace file')
 @click.option('-p', '--poi', 'poi_name', default=None, show_default=True,
               help='POI to scan. If not specified, the first POI from the workspace is used.')
```

### Comparing `quickstats-0.6.8.1/quickstats/clis/inspect_rfile.py` & `quickstats-0.6.8.3/quickstats/clis/inspect_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/clis/inspect_ws.py` & `quickstats-0.6.8.3/quickstats/clis/inspect_ws.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/clis/likelihood_fit.py` & `quickstats-0.6.8.3/quickstats/clis/likelihood_fit.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/clis/likelihood_scan.py` & `quickstats-0.6.8.3/quickstats/clis/likelihood_scan.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/clis/limit_setting.py` & `quickstats-0.6.8.3/quickstats/clis/limit_setting.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/clis/processor_cli.py` & `quickstats-0.6.8.3/quickstats/clis/processor_cli.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/clis/workspace_tools.py` & `quickstats-0.6.8.3/quickstats/clis/workspace_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/analysis_base.py` & `quickstats-0.6.8.3/quickstats/components/analysis_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from quickstats.utils.common_utils import combine_dict
 
 class AnalysisBase(Likelihood, AsimovGenerator):
     def __init__(self, filename:str, poi_name:Optional[Union[str, List[str]]]=None,
                  data_name:str='combData', 
                  config:Optional[Union[Dict, str]]=None,
                  verbosity:Optional[Union[int, str]]="INFO", **kwargs):
-        config = combine_dict(config, kwargs)
+        config = combine_dict(kwargs, config)
         super().__init__(filename=filename,
                          poi_name=poi_name,
                          data_name=data_name,
                          config=config,
                          verbosity=verbosity)
         
     def plot_fit_summary(self, uncond_fit:bool=True, cond_fit:bool=True,
```

### Comparing `quickstats-0.6.8.1/quickstats/components/analysis_object.py` & `quickstats-0.6.8.3/quickstats/components/analysis_object.py`

 * *Files 3% similar despite different names*

```diff
@@ -81,21 +81,24 @@
         floating_aux_vars = [v.GetName() for v in aux_vars if not v.isConstant()]
         if len(floating_aux_vars) > 0:
             self.stdout.warning("The following auxiliary variables (variables that are not "
                                 "part of the POIs, observables, nuisance parameters and global "
                                 f"observables) are floating: {','.join(floating_aux_vars)}. If this is "
                                 "not intended, please make sure to fix them before fitting.", "red")            
     
-    def preset_parameters(self):
-        ROOT.RooStats.SetAllConstant(self.model.global_observables, True)
-        #ROOT.RooStats.SetAllConstant(self.model.nuisance_parameters, False)
-        ROOT.RooStats.SetAllConstant(self.model.pois, True)
-        self.stdout.info("Preset POIs as constant parameters.")
-        #self.stdout.info("INFO: Preset nuisance parameters as floating parameters.")
-        self.stdout.info("Preset global observables as constant parameters.")
+    def preset_parameters(self, fix_pois:bool=True, fix_globs:bool=True, float_nuis:bool=False):
+        if fix_pois:
+            ROOT.RooStats.SetAllConstant(self.model.pois, True)
+            self.stdout.info("Preset POIs as constant parameters.")
+        if fix_globs:
+            ROOT.RooStats.SetAllConstant(self.model.global_observables, True)
+            self.stdout.info("Preset global observables as constant parameters.")
+        if float_nuis:
+            ROOT.RooStats.SetAllConstant(self.model.nuisance_parameters, False)
+            self.stdout.info("INFO: Preset nuisance parameters as floating parameters.")
     
     @property
     def use_blind_range(self):
         return self._use_blind_range
     
     @property
     def minimizer_options(self):
@@ -229,16 +232,20 @@
     def unset_blind_range(self):
         self.minimizer.nll = None
         self.minimizer.nll_commands.pop("RangeWithName", None)
         self.minimizer.nll_commands.pop("SplitRange", None)
         self.stdout.info("Blind range removed from list of  NLL commands. NLL is reset.")
         self._use_blind_range = False
                 
-    def restore_snapshot(self):
+    def restore_prefit_snapshot(self):
         self.load_snapshot(self.kCurrentSnapshotName)
+        
+    def restore_init_snapshot(self):
+        self.load_snapshot(self.kInitialSnapshotName)
+        self.save_snapshot(self.kCurrentSnapshotName)
     
     def get_variables(self, variable_type:Union[str, WSArgument], sort:bool=True):
         return self.model.get_variables(variable_type, sort=sort)
     
     def save_snapshot(self, snapshot_name:Optional[str]=None, 
                       variables:Optional[Union[ROOT.RooArgSet, str, WSArgument]]=None):
         self.model.save_snapshot(snapshot_name, variables=variables)
```

### Comparing `quickstats-0.6.8.1/quickstats/components/asimov_generator.py` & `quickstats-0.6.8.3/quickstats/components/asimov_generator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/asymptotic_cls.py` & `quickstats-0.6.8.3/quickstats/components/asymptotic_cls.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/basics.py` & `quickstats-0.6.8.3/quickstats/components/basics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/extended_minimizer.py` & `quickstats-0.6.8.3/quickstats/components/extended_minimizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -169,15 +169,14 @@
         #self.nll = self.pdf.createNLL(self.data, nll_command_list)
         for command in nll_commands:
             if command.GetName() == "RangeWithName":
                 range_name = command.getString(0)
                 self.stdout.info(f"Using the range \"{range_name}\" for NLL calculation")
         if dataset is None:
             dataset = self.data
-        
         if quickstats.root_version >= (6, 26, 0):
             self._bug_fix_create_nll(dataset, nll_commands)
             nll = self.pdf.createNLL(dataset, *nll_commands)
         else:
             if len(nll_commands) <= 6:
                 nll = self.pdf.createNLL(dataset, *nll_commands)
             # bug: can't have more than 6 arguments
@@ -518,15 +517,15 @@
             eps = 0.001 * tol
             precision = 5.0*eps / (n_sigma**2)
         
         temp_options = {**scan_options}
         snapshot = self.cond_set.snapshot()
         for i in range(max_iter):
             self.stdout.info(f'{front_str} Parameter {par.GetName()} {n_sigma}sigma '
-                             f'iteration {i + 1}: start {val_guess} (MLE{val_guess - val_mle})', bare=True)
+                             f'iteration {i + 1}: start {val_guess} (MLE {val_guess - val_mle})', bare=True)
             val_pre = val_guess
             
             poi_set = ROOT.RooArgSet(par).snapshot()
             poi_set.first().setVal(val_guess)
             
             scan_options['reuse_nll'] = 1
             scan_options['scan']      = 0
```

### Comparing `quickstats-0.6.8.1/quickstats/components/extended_model.py` & `quickstats-0.6.8.3/quickstats/components/extended_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 ##################################################################################################
 import os
 import sys
 import copy
 import math
 import uuid
 import fnmatch
-from typing import List, Optional, Union, Dict, Set, Tuple
+from typing import List, Optional, Union, Dict, Set, Tuple, Sequence
 
 import numpy as np
 
 import ROOT
 from ROOT.RooPrintable import (kName, kClassName, kValue, kArgs, kExtras, kAddress,
                                kTitle, kCollectionHeader, kSingleLine)
 
 import quickstats
 from quickstats import semistaticmethod, AbstractObject
 from quickstats.maths.numerics import is_integer, pretty_value, get_bins_given_edges, array_issubset
 from quickstats.utils.root_utils import load_macro
 from quickstats.utils.common_utils import str_list_filter
 from quickstats.utils.roofit_utils import (get_variable_attributes, variable_collection_to_dataframe,
                                            get_relevant_components)
-from quickstats.utils.string_utils import split_str
+from quickstats.utils.string_utils import split_str, remove_whitespace
 from quickstats.interface.root import TH1, RooDataSet, RooArgSet, RooMsgService, RooAbsPdf
 from quickstats.interface.root import roofit_extension as rf_ext
 from quickstats.interface.root.roofit_extension import get_str_data
 from quickstats.components.basics import WSArgument, SetValueMode
 from .extended_minimizer import ExtendedMinimizer
 
 class ExtendedModel(AbstractObject):
@@ -114,19 +114,14 @@
         return self._observables
     @property
     def category(self):
         return self._category
     @property
     def floating_auxiliary_variables(self):
         return self._floating_auxiliary_variables
-    """
-    @property
-    def data_cat(self):
-        return self._data_cat
-    """
     @property
     def initial_snapshots(self):
         return self._initial_snapshots
     
     @initial_snapshots.setter
     def initial_snapshots(self, val):
         if val is None:
@@ -341,166 +336,185 @@
                           
         # Load snapshots
         self.load_snapshots(self.initial_snapshots)
         
         RooMsgService.remove_topics()
         return None
                 
-    def set_parameters_with_expression(self, param_expr:Optional[str]=None,
+    def set_parameters_with_expression(self, param_setup_expr:Optional[str]=None,
                                        source:Optional["ROOT.RooArgSet"]=None,
                                        mode:Union[str, SetValueMode]=SetValueMode.UNCHANGED):
         if source is None:
             source = self.workspace.allVars()
-        param_dict = self.parse_param_expr(param_expr)
-        parameters = self._set_parameters(source, param_dict, mode=mode)
+        param_setup = self.parse_param_setup(param_setup_expr)
+        parameters = self._set_parameters(source, param_setup, mode=mode)
         if not parameters:
             self.stdout.warning("No parameters are modified from the given fix / profile expression", "red")
         return parameters
         
-    def fix_parameters(self, param_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
-        return self.set_parameters_with_expression(param_expr, source, mode=SetValueMode.FIX)
+    def fix_parameters(self, param_setup_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
+        return self.set_parameters_with_expression(param_setup_expr, source, mode=SetValueMode.FIX)
     
-    def profile_parameters(self, param_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
-        return self.set_parameters_with_expression(param_expr, source, mode=SetValueMode.FREE)
+    def profile_parameters(self, param_setup_expr:Optional[str]=None, source:Optional["ROOT.RooArgSet"]=None):
+        return self.set_parameters_with_expression(param_setup_expr, source, mode=SetValueMode.FREE)
     
-    def _set_parameters(self, source:"ROOT.RooArgSet", param_dict:Dict, 
+    def _set_parameters(self, source:"ROOT.RooArgSet", param_setup:Dict, 
                         mode:Union[str, SetValueMode]=SetValueMode.UNCHANGED):
         selected_parameters = []
         source_names = [param.GetName() for param in source]
-        for name in param_dict:
+        for param_name in param_setup:
             # resolve variable set
-            if name.startswith("<") and name.endswith(">"):
-                selected_params = self.get_variables(name.strip("<>"))
+            if param_name.startswith("<") and param_name.endswith(">"):
+                selected_params = self.get_variables(param_name.strip("<>"))
             else:
-                selected_params = [sname for sname in source_names if fnmatch.fnmatch(sname, name)]
+                selected_params = [sname for sname in source_names if fnmatch.fnmatch(sname, param_name)]
             if not selected_params:
                 # check the possibility that the parameter is not a variable
-                param = self.workspace.obj(name)
+                param = self.workspace.obj(param_name)
                 if param:
                     selected_params = [param]
                 else:
-                    self.stdout.warning(f'Parameter "{name}" does not exist. No modification will be made.', "red")
+                    self.stdout.warning(f'Parameter "{param_name}" does not exist. No modification will be made.', "red")
             for param in selected_params:
                 if isinstance(param, str):
                     param = source[param]
-                self._set_parameter(param, param_dict[name], mode=mode)
+                self._set_parameter(param, param_setup[param_name], mode=mode)
                 selected_parameters.append(param)
         return selected_parameters
 
-    def _set_parameter(self, param:"ROOT.RooRealVar", value:Union[float, int, List, Tuple], 
+    def _set_parameter(self, param:"ROOT.RooRealVar", value:Union[float, int, Sequence], 
                        mode:Union[str, SetValueMode]=SetValueMode.UNCHANGED):
         mode = SetValueMode.parse(mode)
         name = param.GetName()
+        # for non-variable objects, only fix or free them
         if not isinstance(param, ROOT.RooRealVar):
             if mode == SetValueMode.FIX:
                 param.setConstant(1)
-                self.stdout.info(f"Fixed object \"{name}\" as constant.")
+                self.stdout.info(f'Fixed object "{name}" as constant.')
             elif mode == SetValueMode.FREE:
                 param.setConstant(0)
-                self.stdout.info(f"Float object \"{name}\".")
+                self.stdout.info(f'Float object "{name}".')
             return None
         old_value = param.getVal()
-        new_value = old_value
+        setup = {
+            'value': old_value,
+            'vmin' : None,
+            'vmax' : None,
+            'error': None
+        }
+        # set parameter range first
         if isinstance(value, (float, int)):
-            new_value = value
+            setup['value'] = value
         elif isinstance(value, (list, tuple)):
-            if len(value) == 3:
-                new_value = value[0]
-                v_min, v_max = value[1], value[2]
-            elif len(value) == 2:
-                v_min, v_max = value[0], value[1]
+            nargs = len(value)
+            if nargs == 4:
+                setup['value'], setup['vmin'], setup['vmax'], setup['error'] = value
+            elif nargs == 3:
+                setup['value'], setup['vmin'], setup['vmax'] = value
+            elif nargs == 2:
+                setup['vmin'], setup['vmax'] = value
+            elif nargs == 1:
+                setup['value'] = value
             else:
-                raise ValueError('invalid expression for profiling parameter: {}'.format(value))
-            if new_value is None:
-                new_value = old_value
-            # set range
-            if (v_min is not None) and (v_max is not None):
-                if (new_value < v_min) or (new_value > v_max):
-                    new_value = (v_min + v_max)/2
-                param.setRange(v_min, v_max)
-            elif (v_min is not None):
-                if (new_value < v_min):
-                    new_value = v_min
-                # lower bound is zero, if original value is negative, will flip to positive value
-                if (v_min == 0) and (old_value < 0):
-                    new_value = abs(old_value)
-                param.setMin(v_min)
-            elif (v_max is not None):
-                if (new_value > v_max):
-                    new_value = v_max
-                if (v_max == 0) and (old_value > 0):
-                    new_value = -abs(old_value)
-                param.setMax(v_max)
-        if new_value != old_value:
-            param.setVal(new_value)
+                raise ValueError(f'invalid parameter setup: {value}')
+        if setup['value'] is None:
+            setup['value'] = old_value
+        # set range
+        if (setup['vmin'] is not None) and (setup['vmax'] is not None):
+            if (setup['value'] < setup['vmin']) or (setup['value'] > setup['vmax']):
+                setup['value'] = (setup['vmax'] + setup['vmin']) / 2
+            param.setRange(setup['vmin'], setup['vmax'])
+        elif (setup['vmin'] is not None):
+            if (setup['value'] < setup['vmin']):
+                setup['value'] = setup['vmin']
+            # lower bound is zero, if original value is negative, will flip to positive value
+            if (setup['vmin'] == 0) and (old_value < 0):
+                setup['value'] = abs(old_value)
+            param.setMin(setup['vmin'])
+        elif (setup['vmax'] is not None):
+            if (setup['value'] > setup['vmax']):
+                setup['value'] = setup['vmax']
+             # upper bound is zero, if original value is positive, will flip to negative value
+            if (setup['vmax'] == 0) and (old_value > 0):
+                setup['value'] = -abs(old_value)
+            param.setMax(setup['vmax'])
+        # set parameter value
+        if setup['value'] != old_value:
+            param.setVal(setup['value'])
+        # set error value
+        if setup['error'] is not None:
+            param.setError(setup['error'])
+            error_str = f'+/- {param.getError()} '
+        else:
+            error_str = ''
+            
         if mode == SetValueMode.FIX:
             param.setConstant(1)
-            self.stdout.info(f"Fixed parameter \"{name}\" at value {param.getVal()} "
-                             f"[{param.getMin()}, {param.getMax()}]")
+            self.stdout.info(f'Fixed parameter "{name}" at value {param.getVal()} {error_str}'
+                             f'[{param.getMin()}, {param.getMax()}]')
         elif mode == SetValueMode.FREE:
             param.setConstant(0)
-            self.stdout.info(f"Float parameter \"{name}\" at value {param.getVal()} "
-                             f"[{param.getMin()}, {param.getMax()}]")
+            self.stdout.info(f'Float parameter "{name}" at value {param.getVal()}  {error_str}'
+                             f'[{param.getMin()}, {param.getMax()}]')
         else:
             state_str = "C" if param.isConstant() else "F"
-            self.stdout.info(f"Set parameter \"{name}\" at value {param.getVal()} "
-                             f"[{param.getMin()}, {param.getMax()}] {state_str}")
+            self.stdout.info(f'Set parameter "{name}" at value {param.getVal()}  {error_str}'
+                             f'[{param.getMin()}, {param.getMax()}] {state_str}')
 
+    # deprecated
     def set_parameter_defaults(self, source:"ROOT.RooArgSet", value:float=None, error:float=None,
                                constant:bool=None, remove_range:bool=None, target:List[str]=None):
         for param in source:
             if (not target) or (param.GetName() in target):
                 if remove_range:
                     param.removeRange()            
                 if value is not None:
                     param.setVal(value)
                 if error is not None:
                     param.setError(error)
                 if constant is not None:
                     param.setConstant(constant)
-    
-    @staticmethod
-    def parse_param_expr(param_expr:str=None):
-        param_dict = {}
-        # if parameter expression is not empty string or None
-        if param_expr: 
-            if isinstance(param_expr, str):
-                param_dict = ExtendedModel.parse_param_str(param_expr)
-            elif isinstance(param_expr, dict):
-                param_dict = param_dict
-            else:
-                raise ValueError(f'invalid format for parameter expression: {param_expr}')
-        elif param_expr is None:
-        # if param_expr is None, all parameters will be parsed as None by default
-            param_dict = {param.GetName():None for param in source}
-        return param_dict
 
     @staticmethod
-    def parse_param_str(param_str):
+    def parse_param_setup(param_setup_expr:str):
         '''
-        Example: "param_1,param_2=0.5,param_3=-1,param_4=1,param_5=_0_100,param_6=__100,param_7=_0_"
+        `param_setup` should have the format "<param_name>=<nominal_value>_<min_value>_<max_value>_<error_value>"
+        Examples: 
+            "param_1,param_2=0.5,param_3=-1,param_4=1,param_5=_0_100,param_6=__100,param_7=_0_"
         '''
-        param_str = param_str.replace(' ', '')
-        param_list = split_str(param_str, sep=',', remove_empty=True)
-        param_dict = {}
-        for param_expr in param_list:
+        param_setup_expr = remove_whitespace(param_setup_expr)
+        param_expr_list  = split_str(param_setup_expr, sep=',', remove_empty=True)
+        param_setup = {}
+        for param_expr in param_expr_list:
             expr = param_expr.split('=')
             # case only parameter name is given
             if len(expr) == 1:
-                param_dict[expr[0]] = None
+                param_setup[expr[0]] = None
             # case both parameter name and value is given
             elif len(expr) == 2:
                 param_name = expr[0]
                 param_values = [float(v) if v else None for v in split_str(expr[1], sep="_")]
                 if len(param_values) == 1:
                     param_values = param_values[0]
-                param_dict[param_name] = param_values
+                param_setup[param_name] = param_values
             else:
-                raise ValueError(f'invalid parameter expression: {param}')
-        return param_dict
+                raise ValueError(f'invalid parameter setup expression: {param_setup_expr}')
+        return param_setup
+    
+    def get_var(self, name:str):
+        variable = self.workspace.var(name)
+        if not variable:
+            raise ValueError(f'Variable "{name}" not found in the workspace')
+        return variable
+            
+    def get_obj(self, name:str):
+        obj = self.workspace.obj(name)
+        if not obj:
+            raise ValueError(f'Object "{name}" not found in the workspace')
+        return obj
     
     @staticmethod
     def randomize_globs(pdf:ROOT.RooAbsPdf, globs:ROOT.RooArgSet, seed:int):
         """Randomize values of global observables (for generating pseudo-experiments)
         """
         # set random seed for reproducible result
         if seed >= 0:
@@ -525,18 +539,18 @@
             return rf_ext.pair_constraints_base_component(constraint_pdfs, self.nuisance_parameters,
                                                           self.global_observables, fmt=fmt,
                                                           sort=sort, to_str=to_str)
         return rf_ext.pair_constraints(constraint_pdfs, self.nuisance_parameters,
                                        self.global_observables, fmt=fmt,
                                        sort=sort, to_str=to_str)
     
-    def get_constrained_nuisance_parameters(self):
+    def get_constrained_nuisance_parameters(self, fmt:str='list'):
         """Get the list of constrained nuisance parameters instances
         """
-        _, constrained_nuis, _ = self.pair_constraints()
+        _, constrained_nuis, _ = self.pair_constraints(fmt=fmt)
         return constrained_nuis
     
     def get_unconstrained_nuisance_parameters(self, constrained_nuis=None):
         """Get the list of unconstrained nuisance parameters instances
         """
         # do not re-isolate constrained nuisance parameters
         if constrained_nuis is None:
@@ -609,14 +623,15 @@
                 constraint_type = 'unknown'
                 # Loop over global observables to match nuisance parameter and
                 # global observable in case of a constrained nuisance parameter
                 found_global_observable = ROOT.kFALSE
                 for glob_obs in self.global_observables:
                     if constraint.dependsOn(glob_obs):
                         found_global_observable = ROOT.kTRUE
+                        nuip_nom = glob_obs.getVal()
                         # find constraint width in case of a Gaussian
                         if constraint.IsA() == ROOT.RooGaussian.Class():
                             found_gaussian_constraint = ROOT.kTRUE
                             constraint_type = 'gaus'
                             old_sigma_value = 1.0
                             found_sigma = ROOT.kFALSE
                             for server in constraint.servers():
```

### Comparing `quickstats-0.6.8.1/quickstats/components/extended_rfile.py` & `quickstats-0.6.8.3/quickstats/components/extended_rfile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/likelihood.py` & `quickstats-0.6.8.3/quickstats/components/likelihood.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/modelling/component_source.py` & `quickstats-0.6.8.3/quickstats/components/modelling/component_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/modelling/data_modelling.py` & `quickstats-0.6.8.3/quickstats/components/modelling/data_modelling.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/modelling/model_source.py` & `quickstats-0.6.8.3/quickstats/components/modelling/model_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/modelling/parameter_templates.py` & `quickstats-0.6.8.3/quickstats/components/modelling/parameter_templates.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/modelling/pdf_fit_tool.py` & `quickstats-0.6.8.3/quickstats/components/modelling/pdf_fit_tool.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/modelling/tree_data_source.py` & `quickstats-0.6.8.3/quickstats/components/modelling/tree_data_source.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/nuisance_parameter_harmonizer.py` & `quickstats-0.6.8.3/quickstats/components/nuisance_parameter_harmonizer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/nuisance_parameter_pull.py` & `quickstats-0.6.8.3/quickstats/components/nuisance_parameter_pull.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from itertools import repeat
 from typing import List, Optional
 
 import numpy as np
 
 from quickstats.components import ExtendedModel, ExtendedMinimizer
 from quickstats.utils import root_utils, common_utils, string_utils
+from quickstats.utils.io import VerbosePrint
 
 import ROOT
 
 class NuisanceParameterPull(object):
     @property
     def model(self):
         return self._model
@@ -71,83 +72,85 @@
         minimizer.minimize(**minimizer_options)
         for poi in pois:
             poi_values.append(poi.getVal())
         elapsed_time = time.time() - start_time
         return poi_values, elapsed_time
 
     @staticmethod
-    def _run_pulls(input_file:str, data:str, snapshot:str, nuis_name:str, poi_name:str, 
-                   fix_param:Optional[str]=None, profile_param:Optional[str]=None, binned:bool=True,
-                   workspace:Optional[str]=None, model_config:Optional[str]=None,
+    def _run_pulls(filename:str, data_name:str, snapshot_name:str, nuis_name:str, poi_name:str, 
+                   fix_param:Optional[str]=None, profile_param:Optional[str]=None,
+                   binned_likelihood:bool=True, ws_name:Optional[str]=None, mc_name:Optional[str]=None,
                    minimizer_type:str='Minuit2', minimizer_algo:str='Migrad', 
                    precision:float=0.001, eps:float=1.0, retry:int=0, strategy:int=0, print_level:int=1,
                    num_cpu:int=1, offset:bool=True, optimize:int=2, eigen:bool=False,
                    fix_cache:bool=True, fix_multi:bool=True, max_calls:int=-1, 
                    max_iters:int=-1, batch_mode:bool=False, int_bin_precision:float=-1.,
                    outdir:str='pulls', cache=True, logfile_path=None,
-                   minimizer_cls=None, **kwargs):
+                   minimizer_cls=None, verbosity:str="INFO", **kwargs):
+        stdout = VerbosePrint(verbosity)
         # create output directory if not exists
         if not os.path.exists(outdir):
             os.makedirs(outdir, exist_ok=True)        
         outname_root = os.path.join(outdir, nuis_name + '.root')
         outname_json = os.path.join(outdir, nuis_name + '.json')
         #checkpointing:
         if (os.path.exists(outname_root) and os.path.exists(outname_json)) and cache:
-            print('INFO: Jobs already finished for the NP: {}. Skipping.'.format(nuis_name))
+            stdout.info('Jobs already finished for the NP: {}. Skipping.'.format(nuis_name))
             return None
         else:
-            print('INFO: Evaluating pulls for the NP: {}'.format(nuis_name))
+            stdout.info('Evaluating pulls for the NP: {}'.format(nuis_name))
         if logfile_path is not None:
             common_utils.redirect_stdout(logfile_path)
         start_time = time.time()
         # load model
-        model = ExtendedModel(fname=input_file, ws_name=workspace,
-                              mc_name=model_config, data_name=data, 
-                              snapshot_name=snapshot, binned_likelihood=binned,
-                              fix_cache=fix_cache, fix_multi=fix_multi)
+        model = ExtendedModel(fname=filename, ws_name=ws_name,
+                              mc_name=mc_name, data_name=data_name, 
+                              snapshot_name=snapshot_name, binned_likelihood=binned_likelihood,
+                              fix_cache=fix_cache, fix_multi=fix_multi,
+                              verbosity=verbosity)
         if fix_param:
             model.fix_parameters(fix_param)
             
         # by default fix all POIs before floating
         model.set_parameter_defaults(model.pois, error=0.15, constant=1, remove_range=True)
         for param in model.pois:
             extra_str = 'Fixing' if param.isConstant() else 'Set'
-            print('INFO: {} POI {} at value {}'.format(extra_str, param.GetName(), param.getVal()))
+            stdout.info('{} POI {} at value {}'.format(extra_str, param.GetName(), param.getVal()))
         
         # collect pois
         rank_pois = model.profile_parameters(poi_name)
         model.set_parameter_defaults(rank_pois, error=0.15)     
         
         # profile pois
         if profile_param:
-            print('INFO: Profiling POIs')
+            stdout.info('Profiling POIs')
             profile_pois = model.profile_parameters(profile_param)
         
         buffer_time = time.time()
     
         nuip = model.workspace.var(nuis_name)
         if not nuip:
             raise ValueError('Nuisance parameter "{}" does not exist'.format(parameter))
         nuip_name = nuip.GetName()
         nuip.setConstant(0)
-        print('INFO: Computing error for parameter "{}" at {}'.format(nuip.GetName(), nuip.getVal()))
+        stdout.info('Computing error for parameter "{}" at {}'.format(nuip.GetName(), nuip.getVal()))
         
-        print("INFO: Making ExtendedMinimizer for unconditional fit")
+        stdout.info('Making ExtendedMinimizer for unconditional fit')
         if minimizer_cls is None:
             minimizer_cls = ExtendedMinimizer
         minimizer = minimizer_cls("minimizer", model.pdf, model.data, workspace=model.workspace)
-        print("INFO: Starting minimization")
+        stdout.info('Starting minimization')
         nll_commands = [ROOT.RooFit.NumCPU(num_cpu, 3),
                         #ROOT.RooFit.Constrain(model.nuisance_parameters),
                         ROOT.RooFit.GlobalObservables(model.global_observables), 
                         ROOT.RooFit.Offset(offset)]
         if hasattr(ROOT.RooFit, "BatchMode"):
             nll_commands.append(ROOT.RooFit.BatchMode(batch_mode))
         if hasattr(ROOT.RooFit, "IntegrateBins"):
-            nll_commands.append(ROOT.RooFit.IntegrateBins(int_bin_precision))            
+            nll_commands.append(ROOT.RooFit.IntegrateBins(int_bin_precision))
 
         minimize_options = {
             'minimizer_type'   : minimizer_type,
             'minimizer_algo'   : minimizer_algo,
             'strategy' : strategy,
             'optimize'         : optimize,
             'precision'        : precision,
@@ -157,88 +160,89 @@
             'max_iters'        : max_iters,
         }
 
         minimizer.minimize(nll_commands=nll_commands,
                            scan=1, scan_set=ROOT.RooArgSet(nuip),
                            **minimize_options)
         unconditional_time = time.time() - buffer_time
-        print("INFO: Fitting time: {:.3f} s".format(unconditional_time))
+        stdout.info('Fitting time: {:.3f} s'.format(unconditional_time))
         pois_hat = []
         for rank_poi in rank_pois:
             name = rank_poi.GetName()
             value = rank_poi.getVal()
             pois_hat.append(value)
             print(f'\t{name} = {value}')
         
         model.workspace.saveSnapshot('tmp_snapshot', model.pdf.getParameters(model.data))
-        print('INFO: Made unconditional snapshot with name tmp_snapshot')
+        stdout.info('Made unconditional snapshot with name tmp_snapshot')
         
         # find prefit variation
         buffer_time = time.time()
         
         nuip_hat = nuip.getVal()
         nuip_errup = nuip.getErrorHi()
         nuip_errdown = nuip.getErrorLo()
 
         all_constraints = model.get_all_constraints()
         prefit_variation, constraint_type, nuip_nom = model.inspect_constrained_nuisance_parameter(nuip, all_constraints)
         if not constraint_type:
-            print('INFO: Not a constrained parameter. No prefit impact can be determined. Use postfit impact instead.')
+            stdout.info('Not a constrained parameter. No prefit impact can be determined. Use postfit impact instead.')
         prefit_uncertainty_time = time.time() - buffer_time
-        print('INFO: Time to find prefit variation: {:.3f} s'.format(prefit_uncertainty_time))
+        stdout.info('Time to find prefit variation: {:.3f} s'.format(prefit_uncertainty_time))
         
         if rank_pois:
             new_minimizer_options = {
                 'nll_commands': nll_commands,
                 'reuse_nll'   : 1,
                 **minimize_options
             }
             # fix theta at the MLE value +/- postfit uncertainty and minimize again to estimate the change in the POI
-            print('INFO: Evaluating effect of moving {} up by {} + {}'.format(nuip_name, nuip_hat, nuip_errup))
+            stdout.info('Evaluating effect of moving {} up by {} + {}'.format(nuip_name, nuip_hat, nuip_errup))
             pois_up, postfit_up_impact_time = NuisanceParameterPull.evaluate_impact(model, minimizer,
                                                 nuip, nuip_hat + abs(nuip_errup), rank_pois,
                                                 new_minimizer_options,  'tmp_snapshot')
-            print('INFO: Time to find postfit up impact: {:.3f} s'.format(postfit_up_impact_time))
+            stdout.info('Time to find postfit up impact: {:.3f} s'.format(postfit_up_impact_time))
             
-            print('INFO: Evaluating effect of moving {} down by {} - {}'.format(nuip_name, nuip_hat, nuip_errup))
+            stdout.info('Evaluating effect of moving {} down by {} - {}'.format(nuip_name, nuip_hat, nuip_errup))
             pois_down, postfit_down_impact_time = NuisanceParameterPull.evaluate_impact(model, minimizer,
                                                     nuip, nuip_hat - abs(nuip_errdown), rank_pois,
                                                     new_minimizer_options,  'tmp_snapshot')
-            print('INFO: Time to find postfit down impact: {:.3f} s'.format(postfit_down_impact_time))
+            stdout.info('Time to find postfit down impact: {:.3f} s'.format(postfit_down_impact_time))
             
             # fix theta at the MLE value +/- prefit uncertainty and minimize again to estimate the change in the POI
             
             if constraint_type:
-                print('INFO: Evaluating effect of moving {} up by {} + {}'.format(nuip_name, nuip_hat, prefit_variation))
+                stdout.info('Evaluating effect of moving {} up by {} + {}'.format(nuip_name, nuip_hat, prefit_variation))
                 pois_nom_up, prefit_up_impact_time = NuisanceParameterPull.evaluate_impact(model, minimizer,
                                                         nuip, nuip_hat + prefit_variation, rank_pois,
                                                         new_minimizer_options,  'tmp_snapshot')
-                print('INFO: Time to find prefit up impact: {:.3f} s'.format(prefit_up_impact_time))      
+                stdout.info('Time to find prefit up impact: {:.3f} s'.format(prefit_up_impact_time))      
                 
-                print('INFO: Evaluating effect of moving {} down by {} - {}'.format(nuip_name, nuip_hat, prefit_variation))
+                stdout.info('Evaluating effect of moving {} down by {} - {}'.format(nuip_name, nuip_hat, prefit_variation))
                 pois_nom_down, prefit_down_impact_time = NuisanceParameterPull.evaluate_impact(model, minimizer,
                                                             nuip, nuip_hat - prefit_variation, rank_pois,
                                                             new_minimizer_options,  'tmp_snapshot')
-                print('INFO: Time to find prefit down impact: {:.3f} s'.format(prefit_up_impact_time))
+                stdout.info('Time to find prefit down impact: {:.3f} s'.format(prefit_up_impact_time))
             else:
-                print('WARNING: Prefit impact not estimated, instead postfit impact is cloned')
+                stdout.warning('Prefit impact not estimated, instead postfit impact is cloned')
                 pois_nom_up = [i for i in pois_up]
                 pois_nom_down = [i for i in pois_down]
         else:
             pois_up, pois_down, pois_nom_up, pois_nom_down = [], [], [], []
         
         end_time = time.time()
-        print('\nINFO: Time to perform all fits: {:.3f} s'.format(end_time-start_time))
-        print('INFO: Unconditional minimum of NP {}: {} + {} - {}'.format(nuis_name, nuip_hat, 
+        stdout.info(bare=True)
+        stdout.info('Time to perform all fits: {:.3f} s'.format(end_time-start_time))
+        stdout.info('Unconditional minimum of NP {}: {} + {} - {}'.format(nuis_name, nuip_hat, 
               abs(nuip_errup), abs(nuip_errdown)))
-        print('INFO: Prefit uncertainy of NP {}: {} +/- {}'.format(nuis_name, nuip_hat, prefit_variation))
+        stdout.info('Prefit uncertainy of NP {}: {} +/- {}'.format(nuis_name, nuip_hat, prefit_variation))
         for i, rank_poi in enumerate(rank_pois):
-            print('INFO: Unconditional minimum of POI {}: {}'.format(rank_poi.GetName(), pois_hat[i]))
-            print('INFO: POI when varying NP up by 1 sigma postfit (prefit): {} ({})'.format(pois_up[i], pois_nom_up[i]))
-            print('INFO: POI when varying NP down by 1 sigma postfit (prefit): {} ({})'.format(pois_down[i], pois_nom_down[i]))
+            stdout.info('Unconditional minimum of POI {}: {}'.format(rank_poi.GetName(), pois_hat[i]))
+            stdout.info('POI when varying NP up by 1 sigma postfit (prefit): {} ({})'.format(pois_up[i], pois_nom_up[i]))
+            stdout.info('POI when varying NP down by 1 sigma postfit (prefit): {} ({})'.format(pois_down[i], pois_nom_down[i]))
             
         # store result in root file
         outname_root = os.path.join(outdir, nuis_name + '.root')
         
         result = {}
         result['nuis'] = {  'nuisance'   : nuis_name,
                             'nuis_nom'   : nuip_nom,
@@ -261,75 +265,76 @@
             buffer = {'{}_{}'.format(k, kk): vv for kk,vv in v.items()}
             result_for_root.update(buffer)
         r_file = ROOT.TFile(outname_root, "RECREATE")
         r_tree = ROOT.TTree("result", "result")
         root_utils.fill_branch(r_tree, result_for_root)
         r_file.Write()
         r_file.Close()
-        print('INFO: Saved output to {}'.format(outname_root))
+        stdout.info('Saved output to {}'.format(outname_root))
         outname_json = os.path.join(outdir, nuis_name + '.json')
         json.dump(result, open(outname_json, 'w'), indent=2)
         
         if logfile_path is not None:
             common_utils.restore_stdout()
 
     @common_utils.timer
-    def run_pulls(self, input_file:str='workspace.root', data:str='combData', poi:str='', 
-                  snapshot:str='nominalNuis', outdir:str='output', profile:Optional[str]=None,
-                  fix:Optional[str]=None, workspace:Optional[str]=None, model_config:Optional[str]=None,
-                  minimizer_type:str='Minuit2', minimizer_algo:str='Migrad', num_cpu:int=1, 
-                  binned:bool=1, precision:float=0.001, eps:float=1.0, retry:int=0, log_level:str='INFO',
+    def run_pulls(self, filename:str, data_name:str='combData', poi_name:str='', 
+                  snapshot_name:Optional[str]=None, outdir:str='output', profile_param:Optional[str]=None,
+                  fix_param:Optional[str]=None, ws_name:Optional[str]=None, mc_name:Optional[str]=None,
+                  minimizer_type:str='Minuit2', minimizer_algo:str='Migrad', num_cpu:int=1, save_log:bool=True,
+                  binned_likelihood:bool=True, precision:float=0.001, eps:float=1.0, retry:int=0, verbosity:str='INFO',
                   eigen:bool=False, strategy:int=0, print_level:int=1, fix_cache:bool=True, fix_multi:bool=True,
-                  offset:bool=True, optimize:int=2, parameter:str="", max_calls:int=-1, max_iters:int=-1,
+                  offset:bool=True, optimize:int=2, filter_expr:Optional[str]=None, max_calls:int=-1, max_iters:int=-1,
                   batch_mode:bool=False, int_bin_precision:float=-1.,parallel:int=0, cache:bool=True,
-                  exclude:str='', constrained_only:bool=True, minimizer_cls=None, **kwargs):
-        
+                  exclude_expr:Optional[str]=None, constrained_only:bool=True, minimizer_cls=None, **kwargs):
+        if poi_name is None:
+            poi_name = ''
         # configure default minimizer options
         ExtendedMinimizer._configure_default_minimizer_options(minimizer_type, minimizer_algo,
-            strategy, debug_mode=(log_level=="DEBUG"))
+            strategy, debug_mode=(verbosity=="DEBUG"))
         
-        model = ExtendedModel(input_file, workspace, model_config, data_name=data, verbosity="WARNING")
+        model = ExtendedModel(filename, ws_name, mc_name, data_name=data_name, verbosity="WARNING")
         # include constrained NPs only
         if constrained_only:
             nuis_list = [np.GetName() for np in model.get_variables("constrained_nuisance_parameter")]
         # include all NPs
         else:
             nuis_list = [np.GetName() for np in model.get_variables("nuisance_parameter")]
-        include_patterns = string_utils.split_str(parameter, sep=',', remove_empty=True)
-        if parameter:
+        if filter_expr:
             nuis_to_include = []
+            include_patterns = string_utils.split_str(filter_expr, sep=',', remove_empty=True)
             for nuis_name in nuis_list:
                 # filter out nuisance parameters
                 if any(fnmatch.fnmatch(nuis_name, include_pattern) for include_pattern in include_patterns):
                     nuis_to_include.append(nuis_name)
         else:
             nuis_to_include = nuis_list
-        exclude_patterns =  string_utils.split_str(exclude, sep=',', remove_empty=True)
         nuis_to_exclude = []
-        if exclude_patterns:
+        if exclude_expr is not None:
+            exclude_patterns =  string_utils.split_str(exclude_expr, sep=',', remove_empty=True)
             for nuis_name in nuis_list:
                 if any(fnmatch.fnmatch(nuis_name, exclude_pattern) for exclude_pattern in exclude_patterns):
                     nuis_to_exclude.append(nuis_name)
         nuis_names = sorted(list(set(nuis_to_include) - set(nuis_to_exclude)))
         
-        if log_level == 'INFO':
+        if save_log:
             logfile_paths = [os.path.join(outdir, '{}.log'.format(nuis_name)) for nuis_name in nuis_names]
         else:
             logfile_paths = [None]*len(nuis_names)
             
 
-        arguments = (repeat(input_file), repeat(data), repeat(snapshot), nuis_names, 
-                     repeat(poi), repeat(fix), repeat(profile), repeat(binned),
-                     repeat(workspace), repeat(model_config), repeat(minimizer_type), 
+        arguments = (repeat(filename), repeat(data_name), repeat(snapshot_name), nuis_names, 
+                     repeat(poi_name), repeat(fix_param), repeat(profile_param), repeat(binned_likelihood),
+                     repeat(ws_name), repeat(mc_name), repeat(minimizer_type), 
                      repeat(minimizer_algo), repeat(precision), repeat(eps), repeat(retry),
                      repeat(strategy), repeat(print_level), repeat(num_cpu), repeat(offset),
                      repeat(optimize), repeat(eigen), repeat(fix_cache), repeat(fix_multi),
                      repeat(max_calls), repeat(max_iters), repeat(batch_mode),
                      repeat(int_bin_precision), repeat(outdir), repeat(cache), logfile_paths,
-                     repeat(minimizer_cls))
+                     repeat(minimizer_cls), repeat(verbosity))
         common_utils.execute_multi_tasks(self._run_pulls, *arguments, parallel=parallel)
 
         
     @staticmethod
     def parse_root_result(fname):
         import uproot
         with uproot.open(fname) as file:
```

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/__init__.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_alias.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_as_numpy.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_as_numpy.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_base_action.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_base_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_declare.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_declare.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_define.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_define.py`

 * *Files 19% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class RooProcDefine(RooProcRDFAction):
     
     def __init__(self, name:str, expression:str):
         super().__init__(name=name, expression=expression)
         
     @classmethod
     def parse(cls, main_text:str, block_text:Optional[str]=None):
+        main_text = re.sub(' +', ' ', main_text)
         result = re.search(r"^\s*(\w+)\s*=(.*)", main_text)
         if not result:
             raise RuntimeError(f"invalid expression {main_text}")
         name = result.group(1)
         expression = result.group(2)
         return cls(name=name, expression=expression)
```

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_export.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_export.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_filter.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_filter.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_global_variables.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_global_variables.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_hybrid_action.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_hybrid_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_if_defined.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_if_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_if_not_defined.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_if_not_defined.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_load_frame.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_load_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_load_macro.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_load_macro.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_nested_action.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_nested_action.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_report.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_report.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,13 +31,13 @@
             data['pass'] = report.GetPass()
             data['efficiency'] = report.GetEff()
             cumulative_eff *= data['efficiency']/100
             data['cumulative_efficiency'] = cumulative_eff*100
             result.append(data)
         df = pd.DataFrame(result)
         if int(display):
-            processor.stdout.info(df)
+            processor.stdout.info(f'Cutflow Table\n{df}')
         if filename is not None:
             self.makedirs(filename)
             processor.stdout.info(f'INFO: Writing cutflow report to "{filename}".')
             df.to_csv(filename, index=False)
         return rdf, processor
```

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_safe_alias.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_safe_alias.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_save.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_save.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_save_frame.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_save_frame.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_stat.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_stat.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/actions/rooproc_treename.py` & `quickstats-0.6.8.3/quickstats/components/processors/actions/rooproc_treename.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/roo_config_parser.py` & `quickstats-0.6.8.3/quickstats/components/processors/roo_config_parser.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/processors/roo_processor.py` & `quickstats-0.6.8.3/quickstats/components/processors/roo_processor.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/pvalue_toys.py` & `quickstats-0.6.8.3/quickstats/components/pvalue_toys.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/roo_inspector.py` & `quickstats-0.6.8.3/quickstats/components/roo_inspector.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/root_object.py` & `quickstats-0.6.8.3/quickstats/components/root_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/toy_limit_calculator.py` & `quickstats-0.6.8.3/quickstats/components/toy_limit_calculator.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/__init__.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/asimov_handler.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/asimov_handler.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/core_argument_sets.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/core_argument_sets.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/sample.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/sample.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/settings.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/settings.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/systematic.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/systematic.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/systematics_domain.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/systematics_domain.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/ws_comparer.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/ws_comparer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/ws_decomposer.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/ws_decomposer.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/ws_modifier_config.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/ws_modifier_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_base.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_base.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_builder_v1.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_builder_v1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_builder_v2.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_builder_v2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_combiner.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_combiner.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/components/workspaces/xml_ws_modifier.py` & `quickstats-0.6.8.3/quickstats/components/workspaces/xml_ws_modifier.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/concurrent/abstract_runner.py` & `quickstats-0.6.8.3/quickstats/concurrent/abstract_runner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 import os
-import sys
-import time
 from typing import Optional, Union, Dict, List, Any
-from quickstats import semistaticmethod, AbstractObject
+from quickstats import semistaticmethod, AbstractObject, Timer
 from quickstats.concurrent.logging import standard_log
 from quickstats.utils.common_utils import execute_multi_tasks, is_valid_file
 
 class AbstractRunner(AbstractObject):
     
     @property
     def config(self):
@@ -37,43 +35,56 @@
     
     @semistaticmethod
     def _cached_return(self, outname:str):
         raise NotImplementedError
         
     def _end_of_instance_cleanup(self):
         pass
+    
+    def get_instance_outpath(self, kwargs:Dict):
+        outpath = kwargs.get("outname", None)
+        return outpath
+    
+    def get_instance_logpath(self, kwargs:Dict):
+        outpath = self.get_instance_outpath(kwargs)
+        if outpath:
+            return os.path.splitext(outpath)[0] + ".log"
+        return None
         
     def run_instance(self, kwargs:Dict[str, Any]):
         self._prerun_instance(**kwargs)
-        outname = kwargs.get("outname", None)
+        outpath = self.get_instance_outpath(kwargs)
         
-        if outname and (self.config['cache'] and os.path.exists(outname) and is_valid_file(outname)):
-            self.stdout.info(f"Cached output from {outname}")
-            return self._cached_return(outname)
-        
-        log_path = kwargs.get("log_path", None)
-        if (outname and self.config['save_log']) and (not log_path):
-            log_path = os.path.splitext(outname)[0] + ".log"
-        if self.config['save_log']:
-            with standard_log(log_path) as logger:
+        if outpath and (self.config['cache'] and os.path.exists(outpath) and is_valid_file(outpath)):
+            self.stdout.info(f"Cached output from {outpath}")
+            return self._cached_return(outpath)
+        
+        logpath = self.get_instance_logpath(kwargs)
+        if logpath and self.config['save_log']:
+            with standard_log(logpath) as logger:
                 result = self._run_instance(**kwargs)
         else:
             result = self._run_instance(**kwargs)
             
         self._end_of_instance_cleanup()
         
         return result
         
     def run_batch(self, argument_list, auxiliary_args:Optional[Dict]=None):
         parallel = self.config['parallel']
-        t0 = time.time()
-        self._prerun_batch()
-        raw_result = execute_multi_tasks(self.run_instance, argument_list, parallel=parallel)
-        results = self.postprocess(raw_result, auxiliary_args)
-        t1 = time.time()
-        dt = t1 - t0        
+        with Timer() as t:
+            self._prerun_batch()
+            raw_result = execute_multi_tasks(self.run_instance, argument_list, parallel=parallel)
+            results = self.postprocess(raw_result, auxiliary_args)        
         if self.config['timed']:
-            self.stdout.info('All jobs have finished. Total time taken: {:.3f} s'.format(dt))
+            self.stdout.info(f'All jobs have finished. Total time taken: {t.interval:.3f} s')
         return results
     
+    def run(self):
+        argument_list, auxiliary_args = self.prepare_task_inputs()
+        return self.run_batch(argument_list, auxiliary_args=auxiliary_args)
+    
+    def prepare_task_inputs(self):
+        raise NotImplementedError
+    
     def postprocess(self, raw_result, auxiliary_args:Optional[Dict]=None):
         return raw_result
```

### Comparing `quickstats-0.6.8.1/quickstats/concurrent/logging.py` & `quickstats-0.6.8.3/quickstats/concurrent/logging.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/concurrent/parameterised_asymptotic_cls.py` & `quickstats-0.6.8.3/quickstats/concurrent/parameterised_asymptotic_cls.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import os
 import sys
 import copy
 import json
 from typing import Optional, Union, Dict, List, Any
 from itertools import repeat
 
-import pandas as pd
-
 from quickstats import semistaticmethod
 from quickstats.parsers import ParamParser
 from quickstats.concurrent import ParameterisedRunner
-from quickstats.components import AsymptoticCLs
 from quickstats.utils.common_utils import batch_makedirs, json_load
+from quickstats.components import AsymptoticCLs
 
 class ParameterisedAsymptoticCLs(ParameterisedRunner):
     def __init__(self, input_path:str, config:Optional[Dict]=None,
                  file_expr:Optional[str]=None, param_expr:Optional[str]=None,
                  filter_expr:Optional[str]=None, exclude_expr:Optional[str]=None,
                  outdir:str="output", cachedir:str="cache", outname:str="limits.json",
                  save_summary:bool=False, cache:bool=True,
@@ -128,14 +126,15 @@
                 if params:
                     param_str = "("+ParamParser.val_encode_parameters(params)+")"
                 else:
                     param_str = ""                
                 raise RuntimeError(f'Job failed for the input "{filename}" {param_str}. '
                                    'Please check the log file for more details.')
             final_result.append({**params, **limit})
+        import pandas as pd
         final_result = pd.DataFrame(final_result).to_dict('list')
         
         outdir     = self.attributes['outdir']
         outname    = self.attributes['outname']
         
         if outname is not None:
             outpath = os.path.join(outdir, outname)
```

### Comparing `quickstats-0.6.8.1/quickstats/concurrent/parameterised_likelihood.py` & `quickstats-0.6.8.3/quickstats/concurrent/parameterised_likelihood.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import os
 import sys
 import copy
 import json
 from typing import Optional, Union, Dict, List, Any
 from itertools import repeat
 
-import pandas as pd
-
 import ROOT
 from quickstats import semistaticmethod
 from quickstats.parsers import ParamParser
 from quickstats.concurrent import ParameterisedRunner
-from quickstats.components import Likelihood
 from quickstats.utils.common_utils import batch_makedirs
 from quickstats.maths.numerics import pretty_value
+from quickstats.components import Likelihood
 
 class ParameterisedLikelihood(ParameterisedRunner):
     def __init__(self, input_file:str, param_expr:str,
                  filter_expr:Optional[str]=None, exclude_expr:Optional[str]=None,
                  data_name:str="combData", uncond_snapshot:Optional[str]=None,
                  config:Optional[Dict]=None, outdir:str="output", cachedir:str="cache",
                  outname:str="{poi_names}.json", cache:bool=True,
@@ -38,16 +36,16 @@
             'cachedir': cachedir,
             'outname': outname
         }
         
         self.attributes['poi_names'] = ParamParser._get_param_str_attributes(param_expr)
 
     def _prerun_batch(self):
-        self.stdout.info("TIPS: When running likelihood scan on an Asimov dataset, remember to restore the global "
-                         "observables to their Asimov values by loading the appropriate snapshot.", bare=True)
+        self.stdout.tips("When running likelihood scan on an Asimov dataset, remember to restore the global "
+                         "observables to their Asimov values by loading the appropriate snapshot.")
         outdir = self.attributes['outdir']
         cache_dir = self.get_cache_dir()
         batch_makedirs([outdir, cache_dir])
     
     @semistaticmethod
     def _prerun_instance(self, filename:str, mode:int, poi_val:Optional[Union[float, Dict[str, float]]]=None, **kwargs):
         if mode == 2:
@@ -105,15 +103,15 @@
             fit_result = likelihood.nll_fit(poi_val, mode=mode, do_minos=do_minos,
                                             snapshot_name=snapshot_name)
             # save results
             if outname is not None:
                 with open(outname, 'w') as outfile:
                     json.dump(fit_result, outfile)
                     outfile.truncate()
-                print('INFO: Saved NLL result to {}'.format(outname))
+                self.stdout.info(f'Saved NLL result to {outname}')
             result = self._process_result(fit_result)
             return result
         except Exception as e:
             sys.stdout.write(f"{e}\n")
             return None
         
     def get_cache_dir(self):
```

### Comparing `quickstats-0.6.8.1/quickstats/concurrent/parameterised_runner.py` & `quickstats-0.6.8.3/quickstats/concurrent/parameterised_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Optional, List, Dict, Union, Tuple
 import os
 
-from quickstats.concurrent import AbstractRunner
+from . import AbstractRunner
 from quickstats.parsers import ParamParser
 from quickstats.utils.common_utils import combine_dict
 
 class ParameterisedRunner(AbstractRunner):
     
     @property
     def parser(self):
```

### Comparing `quickstats-0.6.8.1/quickstats/core/abstract_object.py` & `quickstats-0.6.8.3/quickstats/core/abstract_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/core/configs.py` & `quickstats-0.6.8.3/quickstats/core/configs.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/core/configurable_object.py` & `quickstats-0.6.8.3/quickstats/core/configurable_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/core/dataclass_object.py` & `quickstats-0.6.8.3/quickstats/core/dataclass_object.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/core/decorators.py` & `quickstats-0.6.8.3/quickstats/core/decorators.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/core/enums.py` & `quickstats-0.6.8.3/quickstats/core/enums.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,20 @@
     def parse(cls, expr:str):
         if expr is None:
             return None
         elif isinstance(expr, cls):
             return expr
         elif isinstance(expr, int):
             return cls(expr)
+        if not isinstance(expr, str):
+            raise RuntimeError(f'invalid expression: {expr}')
         _expr = expr.strip().lower()
         members = cls.get_members_map()
         if _expr in members:
-            return cls(members[_expr])
+            return members[_expr]
         else:
             # check aliases
             aliases = cls.get_aliases_map()
             if _expr in aliases:
                 return cls(cls.parse(aliases[_expr]))
         cls.on_parse_exception(expr)
```

### Comparing `quickstats-0.6.8.1/quickstats/core/methods.py` & `quickstats-0.6.8.3/quickstats/core/methods.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/core/path_manager.py` & `quickstats-0.6.8.3/quickstats/core/path_manager.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/core/virtual_trees.py` & `quickstats-0.6.8.3/quickstats/core/virtual_trees.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/cppyy/core.py` & `quickstats-0.6.8.3/quickstats/interface/cppyy/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/cppyy/macros.py` & `quickstats-0.6.8.3/quickstats/interface/cppyy/macros.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,38 +159,47 @@
     #include "xgboost/c_api.h"
     #include <vector>
     #include <string>
     #include <iostream>
     namespace XGBoostUtils{
         class XGBoostHandle {
             public:
-                XGBoostHandle(const std::string &model_path, bool multithread=false){
+                XGBoostHandle(const std::string &model_path, const bool &multithread=false, 
+                              const bool &use_best_ntree_limit=false){
                     // load xgboost model
                     m_booster = std::unique_ptr<BoosterHandle>(new BoosterHandle());
                     XGBoosterCreate(0, 0, m_booster.get());
                     auto status = XGBoosterLoadModel(*m_booster.get(), model_path.c_str());
                     if (status != 0)
                         throw std::runtime_error(((std::string)"failed to load xgboost model from " + model_path).c_str());
                     // control multithreading
                     if (!multithread)
                         XGBoosterSetParam(*m_booster.get(), "nthread", "1");
+                    if (use_best_ntree_limit){
+                        const char* out;
+                        int success;
+                        XGBoosterGetAttr(*m_booster.get(), "best_iteration", &out, &success);
+                        m_bst_ntree_limit = atoi(out);
+                    }
+                    else
+                        m_bst_ntree_limit = 0;
                 }
                 
                 std::vector<float> getWeightsFromDMatrix(std::vector<float> &vars, const int &size=1){
                     const int nvars = vars.size();
                     std::vector<float> weights = getWeightsFromDMatrix(vars.data(), nvars, size);
                     return weights;
                 }
                 
                 std::vector<float> getWeightsFromDMatrix(float* vars, const int nvars, const int &size=1){
                     DMatrixHandle dmat;
                     XGDMatrixCreateFromMat(vars, size, nvars, -1, &dmat);
                     bst_ulong out_len;
                     const float *f;
-                    XGBoosterPredict(*m_booster.get(), dmat, 0, 0, 1, &out_len, &f);
+                    XGBoosterPredict(*m_booster.get(), dmat, 0, m_bst_ntree_limit, 0, &out_len, &f);
                     XGDMatrixFree(dmat);
                     std::vector<float> weights(size);
                     weights.assign(f, f + size);
                     return weights;
                 }
                 
                 std::vector<float> getWeightsFromDense(std::vector<float> &vars, const int &size=1){
@@ -215,14 +224,15 @@
                                               &out_shape, &out_len, &f);
                     std::vector<float> weights(size);
                     weights.assign(f, f + size);
                     return weights;
                 }
             private:
                 std::unique_ptr<BoosterHandle> m_booster;
+                unsigned m_bst_ntree_limit;
         };
         
         std::vector<float> getXGBoostWeightsFromDMatrix(XGBoostHandle & handle, std::vector<float> &vars, const int &size=1){
             std::vector<float> result = handle.getWeightsFromDMatrix(vars, size);
             return result;
         }
```

### Comparing `quickstats-0.6.8.1/quickstats/interface/cppyy/vectorize.py` & `quickstats-0.6.8.3/quickstats/interface/cppyy/vectorize.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/RooAbsData.py` & `quickstats-0.6.8.3/quickstats/interface/root/RooAbsData.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/RooAbsPdf.py` & `quickstats-0.6.8.3/quickstats/interface/root/RooAbsPdf.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/RooCategory.py` & `quickstats-0.6.8.3/quickstats/interface/root/RooCategory.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/RooDataSet.py` & `quickstats-0.6.8.3/quickstats/interface/root/RooDataSet.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/RooMsgService.py` & `quickstats-0.6.8.3/quickstats/interface/root/RooMsgService.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/RooRealVar.py` & `quickstats-0.6.8.3/quickstats/interface/root/RooRealVar.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/TF1.py` & `quickstats-0.6.8.3/quickstats/interface/root/TF1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/TFile.py` & `quickstats-0.6.8.3/quickstats/interface/root/TFile.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/TH1.py` & `quickstats-0.6.8.3/quickstats/interface/root/TH1.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/TH2.py` & `quickstats-0.6.8.3/quickstats/interface/root/TH2.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/TObject.py` & `quickstats-0.6.8.3/quickstats/interface/root/TObject.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/__init__.py` & `quickstats-0.6.8.3/quickstats/interface/root/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/helper.py` & `quickstats-0.6.8.3/quickstats/interface/root/helper.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/inspection.py` & `quickstats-0.6.8.3/quickstats/interface/root/inspection.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/macros.py` & `quickstats-0.6.8.3/quickstats/interface/root/macros.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/interface/root/roofit_extension.py` & `quickstats-0.6.8.3/quickstats/interface/root/roofit_extension.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,16 @@
     return result
 
 
 def convert_argsets(*argsets, fmt:str="argset", to_str:bool=False):
     if to_str and (fmt == "argset"):
         raise ValueError("argset format does not support to_str")
     if fmt == "argset":
-        return argsets
+        import ROOT
+        return [ROOT.RooArgSet(argset) for argset in argsets]
     elif fmt in ["list", "dict"]:
         results = []
         if to_str:
             for argset in argsets:
                 results.append([i.GetName() for i in argset])
         else:
             for argset in argsets:
```

### Comparing `quickstats-0.6.8.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx` & `quickstats-0.6.8.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h` & `quickstats-0.6.8.3/quickstats/macros/AsymptoticCLsTool/AsymptoticCLsTool.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx` & `quickstats-0.6.8.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h` & `quickstats-0.6.8.3/quickstats/macros/FlexibleInterpVarMkII/FlexibleInterpVarMkII.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx` & `quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/QuickStatsCore.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/RooFitExt.cxx` & `quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/RooFitExt.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/macros/QuickStatsCore/RooFitExt.h` & `quickstats-0.6.8.3/quickstats/macros/QuickStatsCore/RooFitExt.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/macros/ResponseFunction/ResponseFunction.cxx` & `quickstats-0.6.8.3/quickstats/macros/ResponseFunction/ResponseFunction.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/macros/ResponseFunction/ResponseFunction.h` & `quickstats-0.6.8.3/quickstats/macros/ResponseFunction/ResponseFunction.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx` & `quickstats-0.6.8.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.cxx`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h` & `quickstats-0.6.8.3/quickstats/macros/RooTwoSidedCBShape/RooTwoSidedCBShape.h`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/maths/interpolation.py` & `quickstats-0.6.8.3/quickstats/maths/interpolation.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/maths/numerics.py` & `quickstats-0.6.8.3/quickstats/maths/numerics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/maths/statistics.py` & `quickstats-0.6.8.3/quickstats/maths/statistics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/maths/statistics_jitted.py` & `quickstats-0.6.8.3/quickstats/maths/statistics_jitted.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/maths/symbolics.py` & `quickstats-0.6.8.3/quickstats/maths/symbolics.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/parsers/param_parser.py` & `quickstats-0.6.8.3/quickstats/parsers/param_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import copy
 import glob
 import fnmatch
 import itertools
 from functools import partial
 
 import numpy as np
-import pandas as pd
 
 from quickstats import semistaticmethod, DescriptiveEnum
 from quickstats.maths.numerics import pretty_float, str_encode_value, str_decode_value, to_string, to_rounded_float
 from quickstats.utils.string_utils import remove_whitespace, split_str
 
 signature_regex = {
     'F': r"\d+[.]?\d*",
@@ -219,14 +218,15 @@
             combinations = [np.array(param_values[param_name]) for param_name in param_names]
             # take care of rounding errors and negative zeros
             combinations = [(arr.round(decimals=8) + 0.0) if arr[0] is not None else arr for arr in combinations]
             # take care of duplicate ploints
             combinations = [np.unique(arr) for arr in combinations]
             combinations = itertools.product(*combinations)
             all_combinations.extend(list(combinations))
+        import pandas as pd
         all_combinations = pd.unique(all_combinations)
         for combination in all_combinations:
             param_point = {k:v for k,v in zip(param_names, combination)}
             param_points.append(param_point)
         return param_points
     
     @staticmethod
```

### Comparing `quickstats-0.6.8.1/quickstats/plots/__init__.py` & `quickstats-0.6.8.3/quickstats/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/abstract_plot.py` & `quickstats-0.6.8.3/quickstats/plots/abstract_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/bidirectional_bar_chart.py` & `quickstats-0.6.8.3/quickstats/plots/bidirectional_bar_chart.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/collective_data_plot.py` & `quickstats-0.6.8.3/quickstats/plots/collective_data_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/color_schemes.py` & `quickstats-0.6.8.3/quickstats/plots/color_schemes.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/core.py` & `quickstats-0.6.8.3/quickstats/plots/core.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/correlation_plot.py` & `quickstats-0.6.8.3/quickstats/plots/correlation_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/general_1D_plot.py` & `quickstats-0.6.8.3/quickstats/plots/general_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/general_distribution_plot.py` & `quickstats-0.6.8.3/quickstats/plots/general_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/histo_1D_plot.py` & `quickstats-0.6.8.3/quickstats/plots/histo_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/hypotest_inverter_plot.py` & `quickstats-0.6.8.3/quickstats/plots/hypotest_inverter_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/likelihood_1D_plot.py` & `quickstats-0.6.8.3/quickstats/plots/likelihood_1D_plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,16 +11,18 @@
     STYLES = {
         'annotation':{
             'fontsize': 20
         }
     }
     
     CONFIG = {
+        #'sigma_values': (0.99, 3.84),
         'sigma_values': (1, 4),
         'sigma_pos': 0.93,
+        #'sigma_names': ('68% CL', '95% CL'),
         'sigma_names': ('1 $\sigma$', '2 $\sigma$'),
         'sigma_line_styles':{
             'color': 'gray',
             'linestyle': '--'
         },
         'sigma_interval_styles':{
             'loc': (0.2, 0.4),
```

### Comparing `quickstats-0.6.8.1/quickstats/plots/likelihood_2D_plot.py` & `quickstats-0.6.8.3/quickstats/plots/likelihood_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/np_ranking_plot.py` & `quickstats-0.6.8.3/quickstats/plots/np_ranking_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import click
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 import matplotlib.transforms as transforms
 from matplotlib.patches import Rectangle
 from matplotlib.backends.backend_pdf import PdfPages
+from quickstats import AbstractObject, semistaticmethod
 from quickstats.utils.process_tools import parallel_run
 from quickstats.plots.template import draw_analysis_label, format_axis_ticks, parse_transform, draw_hatches, \
                                       draw_sigma_bands, draw_sigma_lines, get_box_dimension, draw_text, centralize_axis
 from quickstats.maths.numerics import ceildiv
 from quickstats.utils.common_utils import json_load
 
 BASE_STYLE = {
@@ -143,66 +144,109 @@
         'color': "#6495ED",
         'alpha': 0.6,
         'hatch': None,
         'fill': True,
     }, **BASE_STYLE
 }
 
-class NPRankingPlot:
-    def __init__(self, input_dir:str=None, poi:Optional[str]=None):
+class NPRankingPlot(AbstractObject):
+    def __init__(self, input_dir:str=None, poi:Optional[str]=None,
+                 version:int=1, verbosity:Optional[Union[int, str]]=None):
         self._data = None
+        self._version = version
         if input_dir is not None:
             self.load(input_dir, poi=poi)
         
     @property
     def data(self):
         return self._data
     
-    @staticmethod
-    def _extract_pull_result(file:str, poi:str=None):
-        with open(file, 'r') as infile:
-                data = json_load(infile)
+    @property
+    def version(self):
+        return self._version
+    
+    @semistaticmethod
+    def _extract_pull_result(self, filename:str, poi:str=None, version:int=1):
+        with open(filename, 'r') as file:
+                data = json_load(file)
         result = {}
-        nuis_data = data['nuis']
-        result['nuis_label']  = nuis_data['nuisance']
-        result['nuis_val']    = nuis_data['nuis_hat'] - nuis_data['nuis_nom']
-        result['nuis_up']     = nuis_data['nuis_hi']
-        result['nuis_down']   = nuis_data['nuis_lo']
-        result['nuis_prefit'] = nuis_data['nuis_prefit']
-        if poi:
-            poi_data = data['pois'].get(poi, None)
-            if not poi_data:
-                raise ValueError("No impact evaluated for the POI \"{}\" in the file {}".format(poi, file))
-            result['poi_hat']      = poi_data['hat']
-            result['impact_postfit_up']    = poi_data['up'] 
-            result['impact_postfit_down']  = poi_data['down'] 
-            result['impact_prefit_up']   = poi_data['up_nom'] 
-            result['impact_prefit_down'] = poi_data['down_nom']
+        version = int(version)
+        if version == 1:
+            nuis_data = data['nuis']
+            result['nuis_label']  = nuis_data['nuisance']
+            result['nuis_val']    = nuis_data['nuis_hat'] - nuis_data['nuis_nom']
+            result['nuis_up']     = nuis_data['nuis_hi']
+            result['nuis_down']   = nuis_data['nuis_lo']
+            result['nuis_prefit'] = nuis_data['nuis_prefit']
+            if poi:
+                poi_data = data['pois'].get(poi, None)
+                if not poi_data:
+                    raise ValueError("No impact evaluated for the POI \"{}\" in the file {}".format(poi, file))
+                result['poi_hat']      = poi_data['hat']
+                result['impact_postfit_up']    = poi_data['up'] 
+                result['impact_postfit_down']  = poi_data['down'] 
+                result['impact_prefit_up']   = poi_data['up_nom'] 
+                result['impact_prefit_down'] = poi_data['down_nom']
+        else:
+            nuis_data = data['nuis']
+            nuis_name = nuis_data['name']
+            result['nuis_label']  = nuis_name
+            result['nuis_val']    = nuis_data['theta_hat'] - nuis_data['theta_0']
+            result['nuis_up']     = nuis_data['theta_errhi']
+            result['nuis_down']   = nuis_data['theta_errlo']
+            result['nuis_prefit'] = nuis_data['theta_errprefit']
+            if data['fit_status']['uncond_fit'] < 0:
+                
+                self.stdout.warning(f'Unconditional fit failed during the evaluation of pulls for the NP "{nuis_name}".')
+            if poi:
+                poi_data = data['poi']
+                if poi_data['name'] != poi:
+                    raise ValueError(f'No impact evaluated for the POI "{poi}" in the file {filename}')
+                result['poi_hat']             = poi_data['mu_hat']
+                result['impact_postfit_up']   = poi_data['up'] 
+                result['impact_postfit_down'] = poi_data['down']
+                result['impact_prefit_up']    = poi_data['up_nom'] 
+                result['impact_prefit_down']  = poi_data['down_nom']
+                if data['fit_status']['sigma_up_postfit'] < 0:
+                    self.stdout.warning(f'Fit failed during the evaluation of postfit +1 sigma impact for the '
+                                        f'NP "{nuis_name}" on the POI "{poi}".')
+                if data['fit_status']['sigma_down_postfit'] < 0:
+                    self.stdout.warning(f'Fit failed during the evaluation of postfit -1 sigma impact for the '
+                                        f'NP "{nuis_name}" on the POI "{poi}".')
+                if data['fit_status']['sigma_up_prefit'] < 0:
+                    self.stdout.warning(f'Fit failed during the evaluation of prefit +1 sigma impact for the '
+                                        f'NP "{nuis_name}" on the POI "{poi}".')
+                if data['fit_status']['sigma_down_prefit'] < 0:
+                    self.stdout.warning(f'Fit failed during the evaluation of prefit -1 sigma impact for the '
+                                        f'NP "{nuis_name}" on the POI "{poi}".')
         return result
     
-    @staticmethod
-    def extract_pull_results(input_dir:str, poi:str=None):
+    @semistaticmethod
+    def extract_pull_results(self, input_dir:str, poi:str=None, version:int=1):
         if not os.path.exists(input_dir):
             raise FileNotFoundError('input directory {} does not exist'.format(input_dir))
         if not os.path.isdir(input_dir):
-            raise ValueError('{} is not a directory'.format(input_dir))
+            raise ValueError(f'{input_dir} is not a directory')
         input_files = glob.glob(os.path.join(input_dir, "*.json"))
-        data = parallel_run(NPRankingPlot._extract_pull_result, input_files, repeat(poi))
-        df = pd.DataFrame(data)
+        pull_results = []
+        for input_file in input_files:
+            result = self._extract_pull_result(input_file, poi, version)
+            pull_results.append(result)
+        df = pd.DataFrame(pull_results)
         if poi:
             df['impact_postfit_up']   -= df['poi_hat']
             df['impact_postfit_down'] -= df['poi_hat']
             df['impact_prefit_up']    -= df['poi_hat']
             df['impact_prefit_down']  -= df['poi_hat']
             df['impact_postfit_total'] = abs(df['impact_postfit_up']) + abs(df['impact_postfit_down'])
             df['impact_prefit_total']  = abs(df['impact_prefit_up']) + abs(df['impact_prefit_down'])
         return df
     
     def load(self, input_dir:str, poi:Optional[str]=None):
-        self._data = self.extract_pull_results(input_dir, poi=poi)
+        self._data = self.extract_pull_results(input_dir, poi=poi, version=self.version)
         
     @staticmethod
     def get_processed_data(df, num=None, threshold=None, ranking=True):
         processed_df = df.copy()
         if 'impact_postfit_total' in processed_df:
             if ranking:
                 processed_df.sort_values('impact_postfit_total', ascending=False, inplace=True)
```

### Comparing `quickstats-0.6.8.1/quickstats/plots/pdf_distribution_plot.py` & `quickstats-0.6.8.3/quickstats/plots/pdf_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/sample_purity_plot.py` & `quickstats-0.6.8.3/quickstats/plots/sample_purity_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/score_distribution_plot.py` & `quickstats-0.6.8.3/quickstats/plots/score_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/stat_plot_config.py` & `quickstats-0.6.8.3/quickstats/plots/stat_plot_config.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/template.py` & `quickstats-0.6.8.3/quickstats/plots/template.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/test_statistic_distribution_plot.py` & `quickstats-0.6.8.3/quickstats/plots/test_statistic_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/upper_limit_1D_plot.py` & `quickstats-0.6.8.3/quickstats/plots/upper_limit_1D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/upper_limit_2D_plot.py` & `quickstats-0.6.8.3/quickstats/plots/upper_limit_2D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/upper_limit_3D_plot.py` & `quickstats-0.6.8.3/quickstats/plots/upper_limit_3D_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/upper_limit_benchmark_plot.py` & `quickstats-0.6.8.3/quickstats/plots/upper_limit_benchmark_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/plots/variable_distribution_plot.py` & `quickstats-0.6.8.3/quickstats/plots/variable_distribution_plot.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/root_checker.py` & `quickstats-0.6.8.3/quickstats/root_checker.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/utils/common_utils.py` & `quickstats-0.6.8.3/quickstats/utils/common_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,18 @@
         if isinstance(d.get(k, None), collections.Mapping) and isinstance(v, collections.Mapping):
             d[k] = update_nested_dict(d[k], v)
         else:
             d[k] = v
     return d
 
 def combine_dict(d:Dict, u:Optional[Dict]=None):
-    d_copy = copy.deepcopy(d)
+    if d is None:
+        d_copy = {}
+    else:
+        d_copy = copy.deepcopy(d)
     if u is None:
         return d_copy
     else:
         u_copy = copy.deepcopy(u)
         return update_nested_dict(d_copy, u_copy)
     
 def str_list_filter(source:List[str], patterns:List[str], inclusive:bool=True):
```

### Comparing `quickstats-0.6.8.1/quickstats/utils/data_conversion.py` & `quickstats-0.6.8.3/quickstats/utils/data_conversion.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/utils/hep_utils.py` & `quickstats-0.6.8.3/quickstats/utils/hep_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/utils/io.py` & `quickstats-0.6.8.3/quickstats/utils/io.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,14 +57,15 @@
 getProcesses = True
 
 @total_ordering
 class Verbosity(Enum):
     
     CRITICAL = (50, 'CRITICAL')
     ERROR = (40, 'ERROR')
+    TIPS = (35, 'TIPS')
     WARNING = (30, 'WARNING')
     INFO = (20, 'INFO')
     DEBUG = (10, 'DEBUG')
     NOTSET = (0, 'NOTSET')
     
     def __new__(cls, value:int, levelname:str=""):
         obj = object.__new__(cls)
@@ -119,27 +120,30 @@
                  msecfmt:Optional[str]=None,
                  datefmt:Optional[str]=None):
         self.verbosity = verbosity
         self.set_format(fmt)
         self.set_timefmt(datefmt, msecfmt)
         self._name = name
         
-    def info(self, text:str, color=None, bare:bool=False):
+    def tips(self, text:str='', color=None, bare:bool=False):
+        self.__call__(text, Verbosity.TIPS, color=color, bare=bare)
+        
+    def info(self, text:str='', color=None, bare:bool=False):
         self.__call__(text, Verbosity.INFO, color=color, bare=bare)
         
-    def warning(self, text:str, color=None, bare:bool=False):
+    def warning(self, text:str='', color=None, bare:bool=False):
         self.__call__(text, Verbosity.WARNING, color=color, bare=bare)
         
-    def error(self, text:str, color=None, bare:bool=False):
+    def error(self, text:str='', color=None, bare:bool=False):
         self.__call__(text, Verbosity.ERROR, color=color, bare=bare)
         
-    def critical(self, text:str, color=None, bare:bool=False):
+    def critical(self, text:str='', color=None, bare:bool=False):
         self.__call__(text, Verbosity.CRITICAL, color=color, bare=bare)
 
-    def debug(self, text:str, color=None, bare:bool=False):
+    def debug(self, text:str='', color=None, bare:bool=False):
         self.__call__(text, Verbosity.DEBUG, color=color, bare=bare)
         
     def set_format(self, fmt:Optional[str]=None):
         if fmt is None:
             fmt = self.DEFAULT_FORMAT
         self._formatter = logging.Formatter(fmt)
```

### Comparing `quickstats-0.6.8.1/quickstats/utils/roofit_utils.py` & `quickstats-0.6.8.3/quickstats/utils/roofit_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/utils/roostats_utils.py` & `quickstats-0.6.8.3/quickstats/utils/roostats_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/utils/root_utils.py` & `quickstats-0.6.8.3/quickstats/utils/root_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/utils/string_utils.py` & `quickstats-0.6.8.3/quickstats/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats/utils/xml_tools.py` & `quickstats-0.6.8.3/quickstats/utils/xml_tools.py`

 * *Files identical despite different names*

### Comparing `quickstats-0.6.8.1/quickstats.egg-info/PKG-INFO` & `quickstats-0.6.8.3/quickstats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quickstats
-Version: 0.6.8.1
+Version: 0.6.8.3
 Summary: A tool for quick statistical analysis for HEP experiments
 Author: Alkaid Cheng
 Author-email: chi.lung.cheng@cern.ch
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `quickstats-0.6.8.1/quickstats.egg-info/SOURCES.txt` & `quickstats-0.6.8.3/quickstats.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 quickstats/components/basics.py
 quickstats/components/extended_minimizer.py
 quickstats/components/extended_model.py
 quickstats/components/extended_rfile.py
 quickstats/components/likelihood.py
 quickstats/components/nuisance_parameter_harmonizer.py
 quickstats/components/nuisance_parameter_pull.py
+quickstats/components/nuisance_parameter_ranking.py
 quickstats/components/pvalue_toys.py
 quickstats/components/roo_inspector.py
 quickstats/components/root_object.py
 quickstats/components/toy_limit_calculator.py
 quickstats/components/modelling/__init__.py
 quickstats/components/modelling/component_source.py
 quickstats/components/modelling/data_modelling.py
@@ -105,14 +106,15 @@
 quickstats/components/workspaces/xml_ws_builder_v1.py
 quickstats/components/workspaces/xml_ws_builder_v2.py
 quickstats/components/workspaces/xml_ws_combiner.py
 quickstats/components/workspaces/xml_ws_modifier.py
 quickstats/concurrent/__init__.py
 quickstats/concurrent/abstract_runner.py
 quickstats/concurrent/logging.py
+quickstats/concurrent/nuisance_parameter_ranking_runner.py
 quickstats/concurrent/parameterised_asymptotic_cls.py
 quickstats/concurrent/parameterised_likelihood.py
 quickstats/concurrent/parameterised_runner.py
 quickstats/core/__init__.py
 quickstats/core/abstract_object.py
 quickstats/core/configs.py
 quickstats/core/configurable_object.py
```

### Comparing `quickstats-0.6.8.1/setup.py` & `quickstats-0.6.8.3/setup.py`

 * *Files identical despite different names*

