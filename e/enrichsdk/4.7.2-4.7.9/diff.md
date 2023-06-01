# Comparing `tmp/enrichsdk-4.7.2.tar.gz` & `tmp/enrichsdk-4.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enrichsdk-4.7.2.tar", last modified: Mon Apr 17 03:51:59 2023, max compression
+gzip compressed data, was "enrichsdk-4.7.9.tar", last modified: Thu Jun  1 06:42:46 2023, max compression
```

## Comparing `enrichsdk-4.7.2.tar` & `enrichsdk-4.7.9.tar`

### file list

```diff
@@ -1,329 +1,334 @@
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      806 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/LICENSE
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      203 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/MANIFEST.in
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3298 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/PKG-INFO
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2182 2023-01-17 09:28:06.000000 enrichsdk-4.7.2/README.rst
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1676 2023-04-13 06:33:53.000000 enrichsdk-4.7.2/enrichsdk/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/api/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6446 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/api/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6001 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/api/draw.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       35 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      369 2023-01-10 11:58:12.000000 enrichsdk-4.7.2/enrichsdk/app/bases/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      456 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/forms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2875 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/models.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9438 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    17335 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    19428 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       92 2022-11-14 13:05:48.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns_helper.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14153 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3129 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14043 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    16391 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    31979 2023-02-27 08:21:08.000000 enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/views.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      272 2023-02-17 05:17:51.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      300 2023-04-13 04:01:12.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button_function.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      212 2023-03-10 06:57:41.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      389 2023-04-05 10:39:21.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_search.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1091 2023-02-17 05:17:51.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      694 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      771 2023-02-17 05:17:51.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2475 2023-02-17 05:17:51.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6992 2023-04-15 03:35:02.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3730 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4104 2023-04-14 03:48:35.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1387 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1591 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4433 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7312 2023-04-13 05:31:25.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8014 2023-03-10 06:57:41.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7251 2023-03-10 06:57:41.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3137 2023-04-13 13:27:08.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2980 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      214 2023-01-17 09:28:06.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/help.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3417 2023-02-17 05:17:51.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1529 2023-01-17 08:20:08.000000 enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      130 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/forms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/models.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2324 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      119 2022-11-23 04:27:41.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/helper.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2224 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10036 2023-04-13 18:17:15.000000 enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/views.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3186 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/utils.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/app/widget/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/widget/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      635 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/widget/basewidget.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5121 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/widget/customcomponent.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3327 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/app/widget/customwidget.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/commands/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      176 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    11330 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/config.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1431 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/decorators.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3025 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/helper.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2232 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6436 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/commands/run.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       45 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       82 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      227 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    25017 2023-02-14 06:43:41.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/anonymizer.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7017 2023-02-07 10:54:16.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/changepoints.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5845 2023-01-10 09:26:26.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/llmtextgen.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7224 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/profilespec.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-16 05:19:04.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/syndata.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3068 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/timeseries_forecasting.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2717 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/catalog.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26236 2023-01-03 13:19:44.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/logprocessor.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      747 2023-04-05 10:39:21.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/anomalies/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33176 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/anomalies/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/changepoints/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33192 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/changepoints/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/classifier/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33641 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/classifier/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/data_quality/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    18378 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/data_quality/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/feature_compute/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4667 2023-04-04 16:04:30.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1615 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    29587 2023-04-04 16:04:30.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1743 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/fileops/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      238 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/fileops/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5046 2023-04-04 16:04:30.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/fileops/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/inmemory_query_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23726 2023-04-04 16:04:30.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/metrics/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    17600 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/metrics/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/notebook_executor/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      946 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/notebook_executor/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5391 2023-04-04 16:04:30.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/observability/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    33314 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/observability/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/synthetic_data_generator/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    26037 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/timeseries_forecaster/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    25318 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      391 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.095734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/fileops/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      769 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/fileops/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2309 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/fileops/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsink/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      452 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsink/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7845 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsink/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsource/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      514 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsource/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5451 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsource/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/pqexport/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/pqexport/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9384 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/pqexport/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/sqlexport/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1450 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/sqlexport/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14007 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/sqlexport/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesink/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1187 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesink/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     9446 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesink/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesource/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1581 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesource/README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8317 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesource/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/core/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3428 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/frames.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    41276 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/core/mixins.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    52640 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/core/node.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3691 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/patch.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7222 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/render.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1292 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/core/res.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    32053 2023-04-05 10:39:21.000000 enrichsdk-4.7.2/enrichsdk/core/run.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14634 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/sdk.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6898 2023-03-09 06:57:39.000000 enrichsdk-4.7.2/enrichsdk/core/state.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/core/widgets.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/datasets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/datasets/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    36181 2023-02-21 05:43:43.000000 enrichsdk-4.7.2/enrichsdk/datasets/discover.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    18149 2023-03-01 13:54:44.000000 enrichsdk-4.7.2/enrichsdk/datasets/doodle.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1389 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/datasets/generators.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/extractors/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1703 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/extractors/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/feature_compute/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    13231 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/feature_compute/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/featurestore/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4502 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/featurestore/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10432 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/featurestore/schema.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/lib/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23696 2023-04-13 03:39:51.000000 enrichsdk-4.7.2/enrichsdk/lib/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4945 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/lib/context.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5827 2023-02-26 08:39:33.000000 enrichsdk-4.7.2/enrichsdk/lib/customer.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2069 2023-03-09 06:57:39.000000 enrichsdk-4.7.2/enrichsdk/lib/exceptions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2903 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/enrichsdk/lib/integration.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      983 2023-01-10 09:26:26.000000 enrichsdk-4.7.2/enrichsdk/lib/misc.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/lib/permissions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1212 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/lib/renderlib.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1357 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/lib/resources.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/notebook/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8611 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/notebook/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/notebook/utils.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/package/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    86072 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/package/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4194 2023-02-01 09:43:30.000000 enrichsdk-4.7.2/enrichsdk/package/lib.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1629 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/package/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    14964 2023-01-03 13:19:44.000000 enrichsdk-4.7.2/enrichsdk/package/misc.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    23959 2023-03-09 06:57:39.000000 enrichsdk-4.7.2/enrichsdk/package/mock.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4322 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/package/validators.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.099734 enrichsdk-4.7.2/enrichsdk/policy/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7529 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/policy/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1608 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/policy/sdk.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/quality/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2476 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5666 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/base.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      925 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/exceptions.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4371 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/expectations.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5157 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/reconciliation.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4884 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/quality/transforms.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/realtime/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      283 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2401 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/db.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      824 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/log.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5122 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/messaging.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4056 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/spark.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4869 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/transforms.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3173 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/realtime/workflow.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/render/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10751 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/render/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/scripts/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/scripts/__init__.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     4372 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/scripts/enrichcmd.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)    44398 2023-04-05 10:51:48.000000 enrichsdk-4.7.2/enrichsdk/scripts/enrichpkg.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/services/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1800 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/services/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/tasks/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10443 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/tasks/__init__.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/tasks/dummy_task/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1839 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/tasks/dummy_task/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     8046 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/tasks/sdk.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/templates/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       42 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/LICENSE.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/MANIFEST.in.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      370 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/README.md.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      383 2023-01-02 14:59:19.000000 enrichsdk-4.7.2/enrichsdk/templates/README_PIPELINE.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       53 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/README_TASK.md
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/templates/airflow/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1476 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/airflow/contrib-pipeline-v1.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/templates/appstore2.0/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3669 2023-01-17 08:20:08.000000 enrichsdk-4.7.2/enrichsdk/templates/appstore2.0/index.html.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.103734 enrichsdk-4.7.2/enrichsdk/templates/assets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4444 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/assets/datasets.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1340 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/config.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/dashboard/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      180 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/apps.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/catalog.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      235 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/custom.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3455 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/persona.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      685 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/tasks.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/dashboard/templates/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5168 2021-09-14 02:19:33.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/templates/complex_result.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2405 2022-03-28 06:32:35.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/templates/index.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1273 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/urls.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4684 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/dashboard/views.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/datasets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      311 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/datasets/manifest.json.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5999 2022-08-02 10:38:39.000000 enrichsdk-4.7.2/enrichsdk/templates/datasets.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      315 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/enrich.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.087734 enrichsdk-4.7.2/enrichsdk/templates/fixtures/
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/fixtures/configs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      419 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/fixtures/configs/1.json
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      421 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/fixtures/configs/2.json
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      854 2022-06-16 09:58:20.000000 enrichsdk-4.7.2/enrichsdk/templates/helloworld.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1180 2022-04-26 06:44:46.000000 enrichsdk-4.7.2/enrichsdk/templates/iris.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      231 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/manifest.json.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/metrics/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    12277 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/metrics/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1266 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/metrics/profilespec.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1248 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/pipelineconf.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1257 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/pipelinepyconf.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/prefect/
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     2693 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/prefect/default.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      916 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/pyscript.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     5053 2021-09-21 13:30:07.000000 enrichsdk-4.7.2/enrichsdk/templates/query.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      225 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/repo.init.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/root.README.md
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      286 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/root.enrich.json.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2599 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/rscript.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       22 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/setup.cfg.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      623 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/setup.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4378 2023-01-26 11:14:36.000000 enrichsdk-4.7.2/enrichsdk/templates/simpletransform.node.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3328 2023-02-07 03:49:08.000000 enrichsdk-4.7.2/enrichsdk/templates/singlepageapp.py.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/spark/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2273 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/README.md
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/spark/configs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/configs/etl_config.json
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1444 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/enrich.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1267 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/logging.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4288 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/spark.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/spark/jobs/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3468 2022-12-08 14:18:41.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/jobs/run_spark.py
--rwxrwxr-x   0 pingali   (1000) pingali   (1000)     1287 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/spark/run.sh
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      682 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/taskconf.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1921 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/tasklib.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     2172 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/test_module.py.template
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     7964 2022-06-27 05:08:43.000000 enrichsdk-4.7.2/enrichsdk/templates/transform.node.template
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/templates/widgets/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3056 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/barchart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1101 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/chart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       28 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/footer.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/fullpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      139 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/gridelement.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       95 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/header.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1561 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/heatmap.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      548 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/hero.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1830 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/linechart.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      373 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/mediumpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      219 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/multicolumn_list.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       74 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/nextrow.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/sectionfooter.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      111 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/sectionheader.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      312 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/shortpanel.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      436 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/table.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       54 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/text.html
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      466 2021-09-12 13:54:25.000000 enrichsdk-4.7.2/enrichsdk/templates/widgets/trophy.html
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/enrichsdk/utils/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     4402 2023-03-27 07:17:21.000000 enrichsdk-4.7.2/enrichsdk/utils/__init__.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3002 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/utils/excel.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     6555 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/utils/redis.py
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:42.000000 enrichsdk-4.7.2/enrichsdk/utils/sample.py
-drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-04-17 03:51:59.091734 enrichsdk-4.7.2/enrichsdk.egg-info/
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3298 2023-04-17 03:51:58.000000 enrichsdk-4.7.2/enrichsdk.egg-info/PKG-INFO
--rw-rw-r--   0 pingali   (1000) pingali   (1000)    10897 2023-04-17 03:51:59.000000 enrichsdk-4.7.2/enrichsdk.egg-info/SOURCES.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2023-04-17 03:51:58.000000 enrichsdk-4.7.2/enrichsdk.egg-info/dependency_links.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       64 2023-04-17 03:51:58.000000 enrichsdk-4.7.2/enrichsdk.egg-info/entry_points.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2021-09-12 14:22:47.000000 enrichsdk-4.7.2/enrichsdk.egg-info/not-zip-safe
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      953 2023-04-17 03:51:58.000000 enrichsdk-4.7.2/enrichsdk.egg-info/requires.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)       10 2023-04-17 03:51:58.000000 enrichsdk-4.7.2/enrichsdk.egg-info/top_level.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     1391 2023-03-08 02:41:34.000000 enrichsdk-4.7.2/requirements.txt
--rw-rw-r--   0 pingali   (1000) pingali   (1000)      116 2023-04-17 03:51:59.107734 enrichsdk-4.7.2/setup.cfg
--rw-rw-r--   0 pingali   (1000) pingali   (1000)     3013 2023-04-13 06:33:53.000000 enrichsdk-4.7.2/setup.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      806 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/LICENSE
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      203 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/MANIFEST.in
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3562 2023-06-01 06:42:46.959321 enrichsdk-4.7.9/PKG-INFO
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2342 2023-05-23 17:29:05.000000 enrichsdk-4.7.9/README.rst
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.931320 enrichsdk-4.7.9/enrichsdk/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1676 2023-06-01 06:40:48.000000 enrichsdk-4.7.9/enrichsdk/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.931320 enrichsdk-4.7.9/enrichsdk/api/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6446 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/api/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6001 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/api/draw.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.931320 enrichsdk-4.7.9/enrichsdk/app/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       35 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/app/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.931320 enrichsdk-4.7.9/enrichsdk/app/bases/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      369 2023-01-10 11:58:12.000000 enrichsdk-4.7.9/enrichsdk/app/bases/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.931320 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      456 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/forms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2875 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/models.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.927320 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.927320 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.931320 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9434 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    17331 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    19424 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       92 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns_helper.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14149 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3125 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14039 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    16381 2023-06-01 04:13:26.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    31961 2023-05-24 11:09:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/views.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.927320 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.927320 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.931320 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.931320 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      272 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      300 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button_function.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       21 2023-05-12 09:38:40.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_donothing.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      468 2023-05-30 06:46:23.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      389 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_search.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1091 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      694 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      771 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2469 2023-06-01 04:13:26.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7369 2023-05-02 06:27:30.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3740 2023-05-14 15:19:15.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4963 2023-05-15 10:25:46.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1397 2023-05-14 15:19:41.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1601 2023-05-14 15:02:24.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4443 2023-05-14 15:19:54.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7244 2023-05-14 15:10:44.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8024 2023-05-14 15:20:08.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7261 2023-05-14 15:11:01.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3147 2023-05-14 15:02:07.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2985 2023-05-14 15:20:20.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      214 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/help.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3423 2023-05-14 15:20:27.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1529 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      183 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      130 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/forms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/models.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.927320 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/templates/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.927320 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/templates/enrichapp/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2320 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      119 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/helper.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2220 2023-05-01 12:58:05.000000 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10025 2023-05-09 15:38:31.000000 enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/views.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3352 2023-05-02 10:46:19.000000 enrichsdk-4.7.9/enrichsdk/app/utils.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/app/widget/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/app/widget/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      635 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/app/widget/basewidget.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5121 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/app/widget/customcomponent.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3327 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/app/widget/customwidget.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/commands/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      176 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/commands/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11171 2023-05-30 15:32:53.000000 enrichsdk-4.7.9/enrichsdk/commands/config.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1431 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/commands/decorators.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3025 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/commands/helper.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2232 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/commands/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6436 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/commands/run.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       45 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       82 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      227 2023-03-08 02:41:34.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    25017 2023-02-14 06:43:41.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/anonymizer.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7017 2023-02-07 10:54:16.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/changepoints.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5845 2023-01-10 09:26:26.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/llmtextgen.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7224 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/profilespec.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-16 05:19:04.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/syndata.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3068 2023-03-08 02:41:34.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/timeseries_forecasting.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2717 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/catalog.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26236 2023-01-03 13:19:44.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/logprocessor.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      880 2023-05-30 13:50:35.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/anomalies/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33176 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/anomalies/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/changepoints/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33192 2023-05-23 11:51:26.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/changepoints/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/classifier/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33641 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/classifier/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/data_quality/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    18378 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/data_quality/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/data_sanitizer/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    21225 2023-05-24 03:24:06.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/data_sanitizer/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/feature_compute/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4667 2023-04-04 16:04:30.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/filebased_query_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1615 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    29587 2023-04-04 16:04:30.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1743 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/fileops/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      238 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/fileops/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5046 2023-04-04 16:04:30.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/fileops/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/inmemory_query_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23726 2023-04-04 16:04:30.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.935320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/metrics/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    17300 2023-05-29 12:15:00.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/metrics/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/notebook_executor/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      946 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/notebook_executor/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5391 2023-04-04 16:04:30.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/observability/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    33314 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/observability/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/synthetic_data_generator/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    26037 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/timeseries_forecaster/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    25318 2023-04-05 10:51:48.000000 enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/transforms/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      469 2023-05-30 13:50:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/transforms/fileops/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      769 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/fileops/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2309 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/fileops/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/transforms/jsonsink/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      452 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/jsonsink/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7845 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/jsonsink/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/transforms/jsonsource/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      514 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/jsonsource/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5451 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/jsonsource/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/transforms/pqexport/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/pqexport/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9384 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/pqexport/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/transforms/sqlexport/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1450 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/sqlexport/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14007 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/sqlexport/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/transforms/tablesink/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1187 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/tablesink/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     9446 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/tablesink/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/contrib/transforms/tablesource/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1581 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/tablesource/README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8317 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/contrib/transforms/tablesource/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/core/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      909 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/core/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3428 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/core/frames.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    41276 2023-03-08 02:41:34.000000 enrichsdk-4.7.9/enrichsdk/core/mixins.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    52640 2023-03-08 02:41:34.000000 enrichsdk-4.7.9/enrichsdk/core/node.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3691 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/core/patch.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7222 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/core/render.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1292 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/core/res.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    32053 2023-04-05 10:39:21.000000 enrichsdk-4.7.9/enrichsdk/core/run.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14634 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/core/sdk.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6898 2023-03-09 06:57:39.000000 enrichsdk-4.7.9/enrichsdk/core/state.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/core/widgets.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/datasets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/datasets/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    37013 2023-05-06 11:02:09.000000 enrichsdk-4.7.9/enrichsdk/datasets/discover.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    18153 2023-05-29 06:02:24.000000 enrichsdk-4.7.9/enrichsdk/datasets/doodle.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1389 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/datasets/generators.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/extractors/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1703 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/extractors/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/feature_compute/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    13231 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/feature_compute/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/featurestore/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4502 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/featurestore/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10432 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/featurestore/schema.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/hedwig/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10907 2023-05-05 12:48:49.000000 enrichsdk-4.7.9/enrichsdk/hedwig/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/lib/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23696 2023-04-13 03:39:51.000000 enrichsdk-4.7.9/enrichsdk/lib/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4945 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/lib/context.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5827 2023-02-26 08:39:33.000000 enrichsdk-4.7.9/enrichsdk/lib/customer.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2069 2023-03-09 06:57:39.000000 enrichsdk-4.7.9/enrichsdk/lib/exceptions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2903 2023-03-08 02:41:34.000000 enrichsdk-4.7.9/enrichsdk/lib/integration.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      983 2023-01-10 09:26:26.000000 enrichsdk-4.7.9/enrichsdk/lib/misc.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      552 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/lib/permissions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1212 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/lib/renderlib.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1357 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/lib/resources.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.939320 enrichsdk-4.7.9/enrichsdk/notebook/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8611 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/notebook/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/notebook/utils.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.943321 enrichsdk-4.7.9/enrichsdk/package/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    86268 2023-05-29 05:29:42.000000 enrichsdk-4.7.9/enrichsdk/package/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4194 2023-02-01 09:43:30.000000 enrichsdk-4.7.9/enrichsdk/package/lib.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1629 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/package/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    14964 2023-01-03 13:19:44.000000 enrichsdk-4.7.9/enrichsdk/package/misc.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    23740 2023-05-30 15:32:23.000000 enrichsdk-4.7.9/enrichsdk/package/mock.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4322 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/package/validators.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.943321 enrichsdk-4.7.9/enrichsdk/policy/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7529 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/policy/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1608 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/policy/sdk.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.943321 enrichsdk-4.7.9/enrichsdk/quality/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2476 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/quality/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5666 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/quality/base.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      925 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/quality/exceptions.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4371 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/quality/expectations.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5157 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/quality/reconciliation.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4884 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/quality/transforms.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.943321 enrichsdk-4.7.9/enrichsdk/realtime/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      283 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/realtime/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2401 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/realtime/db.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      824 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/realtime/log.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5122 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/realtime/messaging.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4056 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/realtime/spark.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4869 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/realtime/transforms.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3173 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/realtime/workflow.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.943321 enrichsdk-4.7.9/enrichsdk/render/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10751 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/render/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.943321 enrichsdk-4.7.9/enrichsdk/scripts/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/scripts/__init__.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     4372 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/scripts/enrichcmd.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)    44415 2023-05-29 05:29:42.000000 enrichsdk-4.7.9/enrichsdk/scripts/enrichpkg.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.943321 enrichsdk-4.7.9/enrichsdk/services/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1800 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/services/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.943321 enrichsdk-4.7.9/enrichsdk/tasks/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    10443 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/tasks/__init__.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.943321 enrichsdk-4.7.9/enrichsdk/tasks/dummy_task/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1839 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/tasks/dummy_task/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     8046 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/tasks/sdk.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.951321 enrichsdk-4.7.9/enrichsdk/templates/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       42 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/LICENSE.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/MANIFEST.in.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      370 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/README.md.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      383 2023-01-02 14:59:19.000000 enrichsdk-4.7.9/enrichsdk/templates/README_PIPELINE.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       53 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/README_TASK.md
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.951321 enrichsdk-4.7.9/enrichsdk/templates/airflow/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1476 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/airflow/contrib-pipeline-v1.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.951321 enrichsdk-4.7.9/enrichsdk/templates/appstore2.0/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3669 2023-01-17 08:20:08.000000 enrichsdk-4.7.9/enrichsdk/templates/appstore2.0/index.html.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.951321 enrichsdk-4.7.9/enrichsdk/templates/assets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4444 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/assets/datasets.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1340 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/config.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.951321 enrichsdk-4.7.9/enrichsdk/templates/dashboard/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      180 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/dashboard/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/dashboard/apps.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      189 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/dashboard/catalog.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      235 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/dashboard/custom.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3455 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/dashboard/persona.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      685 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/dashboard/tasks.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.951321 enrichsdk-4.7.9/enrichsdk/templates/dashboard/templates/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5168 2021-09-14 02:19:33.000000 enrichsdk-4.7.9/enrichsdk/templates/dashboard/templates/complex_result.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2405 2022-03-28 06:32:35.000000 enrichsdk-4.7.9/enrichsdk/templates/dashboard/templates/index.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1273 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/dashboard/urls.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4684 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/dashboard/views.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/enrichsdk/templates/datasets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      311 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/datasets/manifest.json.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5999 2022-08-02 10:38:39.000000 enrichsdk-4.7.9/enrichsdk/templates/datasets.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      315 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/enrich.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.927320 enrichsdk-4.7.9/enrichsdk/templates/fixtures/
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/enrichsdk/templates/fixtures/configs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      419 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/fixtures/configs/1.json
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      421 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/fixtures/configs/2.json
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      854 2022-06-16 09:58:20.000000 enrichsdk-4.7.9/enrichsdk/templates/helloworld.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1180 2022-04-26 06:44:46.000000 enrichsdk-4.7.9/enrichsdk/templates/iris.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      231 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/manifest.json.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/enrichsdk/templates/metrics/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    12277 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/metrics/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1266 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/metrics/profilespec.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1248 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/pipelineconf.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1257 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/pipelinepyconf.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/enrichsdk/templates/prefect/
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     2693 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/prefect/default.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      916 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/pyscript.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     5053 2021-09-21 13:30:07.000000 enrichsdk-4.7.9/enrichsdk/templates/query.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      225 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/repo.init.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/root.README.md
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      286 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/root.enrich.json.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2599 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/rscript.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       22 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/setup.cfg.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      623 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/setup.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4378 2023-01-26 11:14:36.000000 enrichsdk-4.7.9/enrichsdk/templates/simpletransform.node.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3328 2023-02-07 03:49:08.000000 enrichsdk-4.7.9/enrichsdk/templates/singlepageapp.py.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/enrichsdk/templates/spark/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2273 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/spark/README.md
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/enrichsdk/templates/spark/configs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       27 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/spark/configs/etl_config.json
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/enrichsdk/templates/spark/dependencies/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        0 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/spark/dependencies/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1444 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/spark/dependencies/enrich.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1267 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/spark/dependencies/logging.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4288 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/spark/dependencies/spark.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/enrichsdk/templates/spark/jobs/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3468 2022-12-08 14:18:41.000000 enrichsdk-4.7.9/enrichsdk/templates/spark/jobs/run_spark.py
+-rwxrwxr-x   0 pingali   (1000) pingali   (1000)     1287 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/spark/run.sh
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      682 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/taskconf.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1921 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/tasklib.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     2172 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/test_module.py.template
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     7964 2022-06-27 05:08:43.000000 enrichsdk-4.7.9/enrichsdk/templates/transform.node.template
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/enrichsdk/templates/widgets/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3056 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/barchart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1101 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/chart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       28 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/footer.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      384 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/fullpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      139 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/gridelement.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       95 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/header.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1561 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/heatmap.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      548 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/hero.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1830 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/linechart.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      373 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/mediumpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      219 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/multicolumn_list.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       74 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/nextrow.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       70 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/sectionfooter.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      111 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/sectionheader.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      312 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/shortpanel.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      436 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/table.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       54 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/text.html
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      466 2021-09-12 13:54:25.000000 enrichsdk-4.7.9/enrichsdk/templates/widgets/trophy.html
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.955321 enrichsdk-4.7.9/enrichsdk/utils/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     4507 2023-05-30 14:02:13.000000 enrichsdk-4.7.9/enrichsdk/utils/__init__.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3002 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/utils/excel.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     6555 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/utils/redis.py
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1294 2022-12-08 14:18:42.000000 enrichsdk-4.7.9/enrichsdk/utils/sample.py
+drwxrwxr-x   0 pingali   (1000) pingali   (1000)        0 2023-06-01 06:42:46.931320 enrichsdk-4.7.9/enrichsdk.egg-info/
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3562 2023-06-01 06:42:46.000000 enrichsdk-4.7.9/enrichsdk.egg-info/PKG-INFO
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)    11069 2023-06-01 06:42:46.000000 enrichsdk-4.7.9/enrichsdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2023-06-01 06:42:46.000000 enrichsdk-4.7.9/enrichsdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       64 2023-06-01 06:42:46.000000 enrichsdk-4.7.9/enrichsdk.egg-info/entry_points.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)        1 2021-09-12 14:22:47.000000 enrichsdk-4.7.9/enrichsdk.egg-info/not-zip-safe
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      960 2023-06-01 06:42:46.000000 enrichsdk-4.7.9/enrichsdk.egg-info/requires.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)       10 2023-06-01 06:42:46.000000 enrichsdk-4.7.9/enrichsdk.egg-info/top_level.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     1391 2023-03-08 02:41:34.000000 enrichsdk-4.7.9/requirements.txt
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)      116 2023-06-01 06:42:46.959321 enrichsdk-4.7.9/setup.cfg
+-rw-rw-r--   0 pingali   (1000) pingali   (1000)     3092 2023-06-01 06:40:48.000000 enrichsdk-4.7.9/setup.py
```

### Comparing `enrichsdk-4.7.2/LICENSE` & `enrichsdk-4.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/PKG-INFO` & `enrichsdk-4.7.9/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: enrichsdk
-Version: 4.7.2
+Version: 4.7.9
 Summary: Enrich Developer Kit
 Home-page: http://github.com/pingali/scribble-enrichsdk
 Author: Venkata Pingali
 Author-email: pingali@scribbledata.io
 License: All rights reserved
 Description: ==========
         Enrich SDK
@@ -95,11 +95,24 @@
              git push origin
         
         5. Install at customer::
         
              cd scribble-deploy
              fab install_enrichsdk:role=demo
         
+        6. Known issues
+        
+           The package dependencies are a jungle.Problematic packages include:
+        
+           boto3
+           botocore
+           aiobotocore
+           jupyter-events
+           nbconvert
+        
+        
+        
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `enrichsdk-4.7.2/README.rst` & `enrichsdk-4.7.9/README.rst`

 * *Files 19% similar despite different names*

```diff
@@ -86,7 +86,20 @@
 
      git push origin
 
 5. Install at customer::
 
      cd scribble-deploy
      fab install_enrichsdk:role=demo
+
+6. Known issues
+
+   The package dependencies are a jungle.Problematic packages include:
+
+   boto3
+   botocore
+   aiobotocore
+   jupyter-events
+   nbconvert
+
+
+
```

### Comparing `enrichsdk-4.7.2/enrichsdk/__init__.py` & `enrichsdk-4.7.9/enrichsdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 |_____|_| |_|_|  |_|\___|_| |_| |____/|____/|_|\_\
 
 </pre>
 
 """
 import os
 
-VERSION = "4.7.2"
+VERSION = "4.7.9"
 
 
 def _get_git_revision(path):
     revision_file = os.path.join(path, "refs", "heads", "master")
     if os.path.exists(revision_file):
         with open(revision_file) as fh:
             return fh.read().strip()[:7]
```

### Comparing `enrichsdk-4.7.2/enrichsdk/api/__init__.py` & `enrichsdk-4.7.9/enrichsdk/api/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/api/draw.py` & `enrichsdk-4.7.9/enrichsdk/api/draw.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/models.py` & `enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/models.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_add.html`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 {% with knowledge=spec.name|add:' '|add:app.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
 {% block nav_index%}
 <!--Header tab name-->
-    {% with nav_data="usecases" %}{{ block.super }}{% endwith %}
+    {% with nav_data="apps" %}{{ block.super }}{% endwith %}
 {% endblock %}
 <!--============================= Help Content =============================== -->
 {% block help %}
 {% include 'sharedapp/partials/help.html' with app=app spec=spec extra="This page allows you to store the configuration" %}
 {{block.super}}
 {% endblock %}
 <!--============================= Help Content End =============================== -->
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
    2. Usecases
    3. {{usecase.org.name}}
    4. {{spec.name}}
    5. Configurations
    6. Add
 {% with tags=spec.tags|join:" " %} {% with knowledge=spec.name|add:' '|add:
 app.name|add:' '|add:tags %}{{ block.super }}{% endwith %} {% endwith %} {%
-endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="usecases" %}{
+endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="apps" %}{
 { block.super }}{% endwith %} {% endblock %}  {% block help %} {% include
 'sharedapp/partials/help.html' with app=app spec=spec extra="This page allows
 you to store the configuration" %} {{block.super}} {% endblock %}  {% block
 content %}
 {% if 'icon' in spec %}  {% else %}  {% endif %}
 **** {% translate 'Complete the New Configuration' %} ****
 App: {% translate spec.name %} | Type: {{app.verbose_name}}
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_index.html`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 {% with knowledge=spec.name|add:' '|add:app.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
 {% block nav_index%}
 <!--Header tab name-->
-    {% with nav_data="usecases" %}{{ block.super }}{% endwith %}
+    {% with nav_data="apps" %}{{ block.super }}{% endwith %}
 {% endblock %}
 <!--============================= Help Content =============================== -->
 {% block help %}
 {% include 'sharedapp/partials/help.html' with app=app spec=spec %}
 {{block.super}}
 {% endblock %}
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
    1. Enrich
    2. Usecases
    3. {{usecase.org.name}}
    4. {{spec.name}}
    5. Configurations
 {% with tags=spec.tags|join:" " %} {% with knowledge=spec.name|add:' '|add:
 app.name|add:' '|add:tags %}{{ block.super }}{% endwith %} {% endwith %} {%
-endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="usecases" %}{
+endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="apps" %}{
 { block.super }}{% endwith %} {% endblock %}  {% block help %} {% include
 'sharedapp/partials/help.html' with app=app spec=spec %} {{block.super}} {%
 endblock %} {% block customhead %} {% endblock %} {% block content %}
 {% if 'icon' in spec %}  {% else %}  {% endif %}
 **** {% translate spec.name %} ****
 Type: {{app.verbose_name}} {% with spec.app.spec.configuration as conf %} {% if
 conf.workflows == 'on' %} | Workflows: enabled {% endif %} {% if conf.pipeline
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_columns.html`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 {% with knowledge=spec.name|add:' '|add:app.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
 {% block nav_index%}
 <!--Header tab name-->
-    {% with nav_data="usecases" %}{{ block.super }}{% endwith %}
+    {% with nav_data="apps" %}{{ block.super }}{% endwith %}
 {% endblock %}
 <!--============================= Help Content =============================== -->
 {% block help %}
 {% include 'sharedapp/partials/help.html' with app=app spec=spec extra="This page allows you to complete the configuration" %}
 {{block.super}}
 {% endblock %}
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
    2. Usecases
    3. {{usecase.org.name}}
    4. {{spec.name}}
    5. Configurations
    6. Specify
 {% with tags=spec.tags|join:" " %} {% with knowledge=spec.name|add:' '|add:
 app.name|add:' '|add:tags %}{{ block.super }}{% endwith %} {% endwith %} {%
-endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="usecases" %}{
+endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="apps" %}{
 { block.super }}{% endwith %} {% endblock %}  {% block help %} {% include
 'sharedapp/partials/help.html' with app=app spec=spec extra="This page allows
 you to complete the configuration" %} {{block.super}} {% endblock %} {% block
 customhead %} {% endblock %}  {% block content %}
 {% if 'icon' in spec %}  {% else %}  {% endif %}
 **** {% translate 'Select Parameters for the New Configuration' %} ****
 App: {% translate spec.name %} | Type: {{app.verbose_name}}
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 {% with knowledge=spec.name|add:' '|add:app.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
 {% block nav_index%}
 <!--Header tab name-->
-    {% with nav_data="usecases" %}{{ block.super }}{% endwith %}
+    {% with nav_data="apps" %}{{ block.super }}{% endwith %}
 {% endblock %}
 <!--============================= Help Content =============================== -->
 {% block help %}
 {% include 'sharedapp/partials/help.html' with app=app spec=spec extra="This page helps you select a dataset for defining a configuration" %}
 {{block.super}}
 {% endblock %}
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
    2. Usecases
    3. {{usecase.org.name}}
    4. {{spec.name}}
    5. Configurations
    6. Select Dataset
 {% with tags=spec.tags|join:" " %} {% with knowledge=spec.name|add:' '|add:
 app.name|add:' '|add:tags %}{{ block.super }}{% endwith %} {% endwith %} {%
-endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="usecases" %}{
+endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="apps" %}{
 { block.super }}{% endwith %} {% endblock %}  {% block help %} {% include
 'sharedapp/partials/help.html' with app=app spec=spec extra="This page helps
 you select a dataset for defining a configuration" %} {{block.super}} {%
 endblock %} {% block customhead %} {% endblock %}  {% block content %}
 {% if 'icon' in spec %}  {% else %}  {% endif %}
 **** {% translate 'Select a Dataset for New Configuration' %} ****
 App: {% translate spec.name %} | Type: {{app.verbose_name}}
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 {% with knowledge=spec.name|add:' '|add:app.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
 {% block nav_index%}
 <!--Header tab name-->
-    {% with nav_data="usecases" %}{{ block.super }}{% endwith %}
+    {% with nav_data="apps" %}{{ block.super }}{% endwith %}
 {% endblock %}
 <!--============================= Help Content =============================== -->
 {% block help %}
 {% include 'sharedapp/partials/help.html' with app=app spec=spec extra="This page shows the details of one run of the pipeline" %}
 {{block.super}}
 {% endblock %}
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
    2. Usecases
    3. {{usecase.org.name}}
    4. {{spec.name}}
    5. Results
    6. Detail
 {% with tags=spec.tags|join:" " %} {% with knowledge=spec.name|add:' '|add:
 app.name|add:' '|add:tags %}{{ block.super }}{% endwith %} {% endwith %} {%
-endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="usecases" %}{
+endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="apps" %}{
 { block.super }}{% endwith %} {% endblock %}  {% block help %} {% include
 'sharedapp/partials/help.html' with app=app spec=spec extra="This page shows
 the details of one run of the pipeline" %} {{block.super}} {% endblock %} {%
 block customhead %} {% endblock %}  {% block content %}
 {% if 'icon' in spec %}  {% else %}  {% endif %}
 **** {% translate 'Results for' %} {% translate name %} ****
 App: {% translate spec.name %} | Type: {{app.verbose_name}}
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 {% with knowledge=spec.name|add:' '|add:app.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
 {% block nav_index%}
 <!--Header tab name-->
-    {% with nav_data="usecases" %}{{ block.super }}{% endwith %}
+    {% with nav_data="apps" %}{{ block.super }}{% endwith %}
 {% endblock %}
 <!--============================= Help Content =============================== -->
 {% block help %}
 {% include 'sharedapp/partials/help.html' with app=app spec=spec extra="This page shows the available results of pipeline execution" %}
 {{block.super}}
 {% endblock %}
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
    1. Enrich
    2. Usecases
    3. {{usecase.org.name}}
    4. {{spec.name}}
    5. Results
 {% with tags=spec.tags|join:" " %} {% with knowledge=spec.name|add:' '|add:
 app.name|add:' '|add:tags %}{{ block.super }}{% endwith %} {% endwith %} {%
-endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="usecases" %}{
+endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="apps" %}{
 { block.super }}{% endwith %} {% endblock %}  {% block help %} {% include
 'sharedapp/partials/help.html' with app=app spec=spec extra="This page shows
 the available results of pipeline execution" %} {{block.super}} {% endblock %}
 {% block customhead %} {% endblock %}  {% block content %}
 {% if 'icon' in spec %}  {% else %}  {% endif %}
 **** {% translate spec.name %} ****
 Type: {{app.verbose_name}}
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 {% with knowledge=spec.name|add:' '|add:app.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
 {% block nav_index%}
 <!--Header tab name-->
-    {% with nav_data="usecases" %}{{ block.super }}{% endwith %}
+    {% with nav_data="apps" %}{{ block.super }}{% endwith %}
 {% endblock %}
 <!--============================= Help Content =============================== -->
 {% block help %}
 <div id="page_help_content" style="visibility: hidden">
   {% translate 'Trigger workflows for' %} {{app.name}}
 </div>
 {{block.super}}
@@ -247,15 +247,15 @@
 
 <script>
   $(document).ready(function(){
 
       var record = {{data|prettify|safe}};
       $(".actionbtn").on("click", function(){
 	  var btn = $(this);
-          var cookie = getCookie('csrftoken');
+          var cookie = '{{csrf_token}}';
 
 	  var description = $("#description").val();
 
 	  if (description.length == 0){
 	      $('#description').css("border-color", "red");
 	      $("#description").focus();
 	      return;
```

#### html2text {}

```diff
@@ -4,15 +4,15 @@
    1. Enrich
    2. Usecases
    3. {{usecase.org.name}}
    4. {{spec.name}}
    5. Workflow
 {% with tags=spec.tags|join:" " %} {% with knowledge=spec.name|add:' '|add:
 app.name|add:' '|add:tags %}{{ block.super }}{% endwith %} {% endwith %} {%
-endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="usecases" %}{
+endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="apps" %}{
 { block.super }}{% endwith %} {% endblock %}  {% block help %}
 {% translate 'Trigger workflows for' %} {{app.name}}
 {{block.super}} {% endblock %} {% block customhead %} {% endblock %}  {% block
 content %}
 {% if 'icon' in spec %}  {% else %}  {% endif %}
 **** {% translate app.verbose_name %} - {% translate 'Trigger Workflow/Sharing'
 %} ****
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/policyapp/views.py` & `enrichsdk-4.7.9/enrichsdk/app/bases/policyapp/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,24 +86,24 @@
     def get_model(self, spec, name):
 
         from enrichapp.dashboard.globalapp import lib as globallib
 
         if (('models' in spec) and (name in spec['models'])):
             return spec['models'][name]
 
-        return globallib.get_model(f"app_policy")
+        return globallib.get_model(name)
 
     def get_form(self, spec, name):
 
         from enrichapp.dashboard.globalapp import lib as globallib
 
         if (('forms' in spec) and (name in spec['forms'])):
             return spec['forms'][name]
 
-        return globallib.get_form(f"app_policy")
+        return globallib.get_form(name)
 
     def validate_spec(self, spec):
 
         fill_action_gaps(spec, context={ })
 
         errors = default_validate_spec(spec)
         if len(errors) > 0:
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 <script>
   $(document).on('click','.{{widget.id}}_workflowtarget',function(){
       
       var obj = $(this);
       var row = obj.data("row");
       var actionid = obj.data('actionid');
-      var cookie = getCookie('csrftoken');
+      var cookie = '{{csrf_token}}';
       
       var data = {
 	  "actionid": actionid,
 	  "message": "{{content.message}}",
 	  "data": JSON.stringify(row)
       };
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html`

 * *Files 3% similar despite different names*

```diff
@@ -11,24 +11,33 @@
       <li class="breadcrumb-item"><a href="{% url 'dashboard:home' %}">Enrich</a></li>
       <li class="breadcrumb-item"><a href="{% url 'dashboard:index' %}">Usecases</a></li>
       <li class="breadcrumb-item"><a href="{% url 'dashboard:usecase_detail' usecase.org.name %}">{{usecase.org.name}}</a></li>
       <li class="breadcrumb-item active"><a href="{% url basenamespace|add:':index' %}">{{spec.name}}</a></li>
       {% if data.breadcrumb %}
       <li class="breadcrumb-item active">{{data.breadcrumb}}</a></li>
       {% endif %}
+      {% if data.breadcrumbs %}
+      {% for breadcrumb in data.breadcrumbs %}
+      {% if 'url' in breadcrumb %}
+      <li class="breadcrumb-item"><a href="{{breadcrumb.url}}">{{breadcrumb.name}}</a></li>
+      {% else %}
+      <li class="breadcrumb-item active">{{breadcrumb.name}}</a></li>
+      {% endif %}
+      {% endfor %}
+      {% endif %}
     </ol>
 </div>
 {% with tags=spec.tags|join:" " %}
 {% with knowledge=spec.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
 {% block nav_index %}
 <!--Header tab name-->
-    {% with nav_data="usecases" %}{{ block.super }}{% endwith %}
+    {% with nav_data="apps" %}{{ block.super }}{% endwith %}
 {% endblock %}
 <!--============================= Help Content =============================== -->
 
 {% block help %}
 {% include 'sharedapp/partials/help.html' with spec=spec app=app %}
 {{block.super}}
 {% endblock %}
@@ -147,15 +156,17 @@
           <div class="sidebar-wrapper">
             <div class="sticky-top">
               <div class="sidebar-inside">
                 <ul class="nav-menu-list">
                   {% for target in data.sidebar_targets %}
                   <li class="nav-menu-item">
                       {% if target.link %}
-                        <a href="{{target.link}}" class="nav-menu-box">
+                      <a href="{{target.link}}"
+			 target="{{target.target}}"
+			 class="nav-menu-box">
                           <div class="nav-menu-icon">
                                 {% include 'sharedapp/partials/sidebar_menu_icon.html' with target=target %}
                             <span>{% translate target.label %}</span>
                           </div>
                         </a>
                       {% else %}
                         <a href="{% url basenamespace|add:':index' %}?{{target.params|get_encoded_dict}}" class="nav-menu-box">
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html`

 * *Files 1% similar despite different names*

```diff
@@ -77,17 +77,17 @@
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapseresults_{{widget.id}}" aria-expanded="true">
         <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
         <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
       </div>
       <div class="accor-right">
         <div class="block-filter-left">
           <ul class="cp-text-list d-flex align-items-center">
-            <li><b>{% translate widget.name %}</b></li>
+            <li><b>{% translate widget.name|safe %}</b></li>
           </ul>
-            <p>{% translate widget.description %}</p>
+            <p>{% translate widget.description|safe %}</p>
         </div>
       </div>
     </div>
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-end">
             {% include 'sharedapp/components/share_menu_action.html' %}
     </div>
   </div>
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_form.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 {% load staticfiles %}
 {% load i18n %}
 {% load fontawesome %}
+{% load dashboard_tags %}
 
 <style>
   .spinner-border{
       width: 4.375rem;
       height: 4.375rem;
       position: fixed;
       z-index: 999;
@@ -30,63 +31,84 @@
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapseresults" aria-expanded="true">
         <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
         <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
       </div>
       <div class="accor-right">
         <div class="block-filter-left">
           <ul class="cp-text-list d-flex align-items-center">
-            <li><b>{% translate widget.name %}</b></li>
+            <li><b>{% translate widget.name|safe %}</b></li>
           </ul>
-            <p>{% translate widget.description %}</p>
+            <p>{% translate widget.description|safe %}</p>
         </div>
       </div>
     </div>
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-center align-block-filter-option">
     </div>
   </div>
   <div id="collapseresults" class="crc-body accordion-collapse collapse show">
     <div class="cp-body">
       <div class="row mb-30">
 	{% if widget.method %}
 	<form class="uniForm"  method="{{widget.method}}" id="form{{widget.id}}">
         {% else %}
 	<form class="uniForm"  method="GET" id="form{{widget.id}}">
-        {% endif %}
-	  {% if widget.method == "POST" %}
+          {% endif %}
+	  {% if widget.method.lower == "post" %}
 	  {% csrf_token %}
 	  {% endif %}
 	  {% for name, value in widget.hidden_vars.items %}
 	  <input name="{{name}}" value="{{value}}" type="hidden"></input>
 	  {% endfor %}
           <ul class="v-line-text-list d-flex flex-wrap">
 	    {% for element in widget.elements %}
 	    {% if element.type == "select" %}
             <div class="v-box p-2">
               <h4>{{element.label}}</h4>
               <div class="column">
 	        <div class="form-group">
+
                   <span class="multiselect-native-select">
                     <select class="selectpicker form-control" id="{{element.id}}" name="{{element.id}}" data-live-search-placeholder="Search" data-live-search="true" data-container="body" data-size="5">
+		      {% if element.choices|get_class == "dict" %}
+                      {% for label,value in element.choices.items %}
+                      <option value="{{value}}" title="{{value}}" {% if element.selected_choice == value %}selected{% endif%}>{{label|safe}}</option>
+                      {% endfor %}
+		      {% else %}
                       {% for choice in element.choices %}
                       <option value="{{choice}}" title="{{choice}}" {% if element.selected_choice == choice %}selected{% endif%}>{{choice}}</option>
                       {% endfor %}
+		      {% endif %}
                     </select>
                   </span>
 	        </div>
               </div>
             </div>
 	    {% elif element.type == "input" %}
             <div class="v-box p-2">
               <h4>{{element.label}}</h4>
               <div class="column">
                 <div class="form-group" id="single-text-{{widget.id}}">
                   <input type="text" class="form-control" id="{{element.name}}" name="{{element.name}}" value="{{element.value}}" placeholder="{{element.placeholder}}" required >
                 </div>
               </div>
             </div>
+	    {% elif element.type == "textarea" %}
+            <div class="v-box p-2">
+              <h4>{{element.label}}</h4>
+	      <div class="column">
+		<div class="form-group d-flex">
+		  <textarea class="{{element.class}}"
+			    id="{{ element.id }}"
+			    name="{{ element.id }}"
+			    rows="{{ element.rows }}"
+			    cols="{{ element.cols }}"
+			    placeholder="{{ element.placeholder }}" required>{{element.value}}</textarea>
+		</div>
+	      </div>
+	    </div>
 	    {% endif %}
 	    {% endfor %}
             <div class="v-box p-2 mt-3">
               <div class="column">
 		<div class="form-group d-flex" id="formsubmitdiv">
 		  <button name="submit" id="submit" value="show" type="submit" class="btn btn-default" data-toggle="tooltip" data-placement="bottom"><img src="{% static 'gui2/appstore2/images/play.svg' %}" alt="" />{% if 'submit' in widget %}{{widget.submit}}{% else %}Show{% endif %}</button>
 		  <div class="spinner-border" role="status" id="spinner">
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_image.html`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,17 @@
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapseresults_{{widget.id}}" aria-expanded="true">
         <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
         <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
       </div>
       <div class="accor-right">
         <div class="block-filter-left">
           <ul class="cp-text-list d-flex align-items-center">
-            <li><b>{% translate widget.name %}</b></li>
+            <li><b>{% translate widget.name|safe %}</b></li>
           </ul>
-            <p>{% translate widget.description %}</p>
+            <p>{% translate widget.description|safe %}</p>
         </div>
       </div>
     </div>
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-center align-block-filter-option">
     </div>
   </div>
   <div id="collapseresults_{{widget.id}}" class="crc-body accordion-collapse collapse show">
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_key_value_pairs.html`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapseresults" aria-expanded="true">
         <img class="expand-open" src="{% static 'gui2/appstore2/images/new-caret-icon-1.svg' %}" alt="" />
         <img class="expand-add" src="{% static 'gui2/appstore2/images/expand-add.svg' %}" alt="" />
       </div>
       <div class="accor-right">
         <div class="block-filter-left">
           <ul class="cp-text-list d-flex align-items-center">
-            <li><b>{% translate widget.name %}</b></li>
+            <li><b>{% translate widget.name|safe %}</b></li>
           </ul>
           <p>{% translate widget.description %}</p>
         </div>
       </div>
     </div>
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-center align-block-filter-option">
     </div>
@@ -29,15 +29,15 @@
   <div id="collapseresults" class="crc-body accordion-collapse collapse show">
     <div class="bw-body p-0">
       <ul class="v-line-text-list d-flex flex-wrap">
 	{% for k, v in widget.details.items %}
         <li>
           <div class="v-line-box">
             <h4>{% translate k %}</h4>
-            <p>{{v}}</p>
+            <p>{{v|safe}}</p>
           </div>
         </li>
 	{% endfor %}
       </ul>
     </div>
   </div>
 </div>
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_linechart.html`

 * *Files 2% similar despite different names*

```diff
@@ -93,17 +93,17 @@
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapseresults_{{widget.id}}" aria-expanded="true">
         <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
         <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
       </div>
       <div class="accor-right">
         <div class="block-filter-left">
           <ul class="cp-text-list d-flex align-items-center">
-            <li><b>{% translate widget.name %}</b></li>
+            <li><b>{% translate widget.name|safe %}</b></li>
           </ul>
-            <p>{% translate widget.description %}</p>
+            <p>{% translate widget.description|safe %}</p>
         </div>
       </div>
     </div>
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-end align-block-filter-option">
       {% for k,values in widget.header_components.items %}
       {% for v in  values %}
       <div class="cp-download">
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table.html`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapsetable_{{widget.id}}" aria-expanded="true">
         <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
         <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
       </div>
       <div class="accor-right">
         <div class="block-filter-left">
           <ul class="cp-text-list d-flex align-items-center">
-            <li><b>{% translate widget.name %}</b></li>
+            <li><b>{% translate widget.name|safe %}</b></li>
             <li>{%  if widget.results_count %} {{ widget.results_count }} {% else %} {{ widget.rows | length }} {% endif %} {% translate 'results' %}</li>
           </ul>
-         <p>{% translate widget.description %}</p>
+         <p>{% translate widget.description|safe %}</p>
         </div>
       </div>
     </div>
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-end">
         {% for k,values in widget.header_components.items %}
         {% for v in  values %}
         {% include 'sharedapp/components/'|add:v.template|add:'.html' with content=v widget=widget %}
@@ -77,25 +77,25 @@
 
                     </tr>
                   </thead>
                   <tbody>
                         {% for row in widget.rows %}
                         <tr>
                             {% for col in widget.columns %}
-                                {%  if 'ACTION_' in col %}
-                                        {% for k,v in  row.items %}
-                                            {% if 'ACTION_' in k %}
-                                                <td>
-                                                    {% include 'sharedapp/components/'|add:v.template|add:'.html' with content=v %}
-                                                </td>
-                                            {% endif %}
-                                        {% endfor %}
-                                {% else %}
-                                    <td class="{{widget.td_class}}">{{row|get_item:col|safe}}</td>
-                                {% endif %}
+                              {%  if 'ACTION_' in col %}
+                                 {% for k,v in  row.items %}
+                                     {% if 'ACTION_' in k %}
+                                     <td>
+                                     {% include 'sharedapp/components/'|add:v.template|add:'.html' with content=v %}
+                                     </td>
+                                    {% endif %}
+                                 {% endfor %}
+                              {% else %}
+                              <td class="{{widget.td_class}}">{{row|get_item:col|safe}}</td>
+                              {% endif %}
 
                             {% endfor %}
                         </tr>
                         {% endfor %}
                   </tbody>
               </table>
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_filters.html`

 * *Files 1% similar despite different names*

```diff
@@ -14,18 +14,18 @@
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapsetable_{{widget.id}}" aria-expanded="true">
         <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
         <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
       </div>
       <div class="accor-right">
         <div class="block-filter-left">
           <ul class="cp-text-list d-flex align-items-center">
-            <li><b>{% translate widget.name %}</b></li>
+            <li><b>{% translate widget.name|safe %}</b></li>
             <li>{%  if widget.results_count %} {{ widget.results_count }} {% else %} {{ widget.rows | length }} {% endif %} {% translate 'results' %}</li>
           </ul>
-          <p>{% translate widget.description %}</p>
+          <p>{% translate widget.description|safe %}</p>
         </div>
       </div>
     </div>
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-end">
         {% for k,values in widget.header_components.items %}
               {% for v in  values %}
                   <div class="cp-download">
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_table_with_search.html`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapsetable_{{widget.id}}" aria-expanded="true">
         <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
         <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
       </div>
       <div class="accor-right">
         <div class="block-filter-left">
           <ul class="cp-text-list d-flex align-items-center">
-            <li><b>{% translate widget.name %}</b></li>
+            <li><b>{% translate widget.name|safe %}</b></li>
             <li>{%  if widget.results_count %} {{ widget.results_count }} {% else %} {{ widget.rows | length }} {% endif %} {% translate 'results' %}</li>
           </ul>
-        <p>{% translate widget.description %}</p>
+        <p>{% translate widget.description|safe %}</p>
         </div>
       </div>
     </div>
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-end">
         {% for k,values in widget.header_components.items %}
               {% for v in  values %}
                   <div class="cp-download">
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_text.html`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapseresults_{{widget.id}}" aria-expanded="true">
         <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
         <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
       </div>
       <div class="accor-right">
         <div class="block-filter-left">
           <ul class="cp-text-list d-flex align-items-center">
-            <li><b>{% translate widget.name %}</b></li>
+            <li><b>{% translate widget.name|safe %}</b></li>
           </ul>
-            <p>{% translate widget.description %}</p>
+            <p>{% translate widget.description|safe %}</p>
         </div>
       </div>
     </div>
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-end align-block-filter-option">
       {% for k,values in widget.header_components.items %}
       {% for v in  values %}
       {% include 'sharedapp/components/'|add:v.template|add:'.html' with content=v widget=widget %}
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_widget_with_config.html`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
       <div class="code-panel-head d-flex align-items-center">
          <div class="cph-left d-flex align-items-center flex-wrap" style="width: auto;">
             <div class="cph-icon"  data-bs-toggle="collapse" data-bs-target="#collapsetable_{{widget.id}}" aria-expanded="true">
                <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
                <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
             </div>
                 <div class="accor-right">
-                    <div class="title" id="codeblockTitle_{{widget.id}}">{% translate widget.name %}</div>
+                    <div class="title" id="codeblockTitle_{{widget.id}}">{% translate widget.name|safe %}</div>
                 </div>
             </div>
          <div class="cph-right d-flex align-items-center flex-wrap ms-auto" style="width: auto;">
              {% for k,values in widget.header_components.items %}
                   {% for v in  values %}
                         {% include 'sharedapp/components/'|add:v.template|add:'.html' with content=v %}
                   {% endfor %}
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 {% load staticfiles %} {% load dashboard_tags %} {% load i18n %}
 gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
 gui2/appstore2/images/expand-add.svg' %} alt="" />
-{% translate widget.name %}
+{% translate widget.name|safe %}
 {% for k,values in widget.header_components.items %} {% for v in values %} {%
 include 'sharedapp/components/'|add:v.template|add:'.html' with content=v %} {%
 endfor %} {% endfor %}
 gui2/appstore2/images/get-app.svg' %} alt="" />
 gui2/appstore2/images/copy-icon.svg' %} alt="">
 {{widget.info|safe}}
 {% csrf_token %}
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/share.html`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       <div class="crc-head-icon"  data-bs-toggle="collapse" data-bs-target="#collapsetable_{{widget.id}}" aria-expanded="true">
         <img class="expand-open" src={% static 'gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
         <img class="expand-add" src={% static 'gui2/appstore2/images/expand-add.svg' %} alt="" />
       </div>
       <div class="accor-right">
         <div class="block-filter-left">
           <ul class="cp-text-list d-flex align-items-center">
-            <li><b>{% translate widget.name %}</b></li>
+            <li><b>{% translate widget.name|safe %}</b></li>
           </ul>
         </div>
       </div>
     </div>
     <div class="block-filter-option ms-auto d-flex align-items-center justify-content-end">
     </div>
   </div>
@@ -65,8 +65,8 @@
 <div class="mt-4"></div>
 
 <script>
 function getContent(){
     var value = $("#messagediv").html()
     document.getElementById("message").value = value;
 };
-</script>
+</script>
```

#### html2text {}

```diff
@@ -1,15 +1,16 @@
 {% load staticfiles %} {% load dashboard_tags %} {% load i18n %}
 gui2/appstore2/images/new-caret-icon-1.svg' %} alt="" />
 gui2/appstore2/images/expand-add.svg' %} alt="" />
-    * {% translate widget.name %}
+    * {% translate widget.name|safe %}
 {% csrf_token %}
 Emails [{{widget.shareparams.emails|join:','}}] Enter a list of emails
 separated by comma
 Hi!
 
 Please check the following Search_Results. You can explore and download the
 search results from the given url.
 
 -{{widget.shareparams.user}}
 Doubleclick to edit the message to be sent
  {% translate 'Send' %}
+
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/sidebar_menu_icon.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/generic.html`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 {% with knowledge=spec.name|add:' '|add:app.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
 {% block nav_index%}
 <!--Header tab name-->
-    {% with nav_data="usecases" %}{{ block.super }}{% endwith %}
+    {% with nav_data="apps" %}{{ block.super }}{% endwith %}
 {% endblock %}
 <!--============================= Help Content =============================== -->
 {% block help %}
 <div id="page_help_content" style="visibility: hidden">
   Show {{app.name}} configurations
 </div>
 {{block.super}}
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 %} {% load static %}  {% block breadcrumbs %}
    1. Enrich
    2. Usecases
    3. {{usecase.org.name}}
    4. {{spec.name}}
 {% with tags=spec.tags|join:" " %} {% with knowledge=spec.name|add:' '|add:
 app.name|add:' '|add:tags %}{{ block.super }}{% endwith %} {% endwith %} {%
-endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="usecases" %}{
+endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="apps" %}{
 { block.super }}{% endwith %} {% endblock %}  {% block help %}
 Show {{app.name}} configurations
 {{block.super}} {% endblock %}  {% block content %}
 {% fontawesome_icon app.icon %}
 {% block page_header %}
 ****** {{app.verbose_name}} ******
 {{spec.name}}: {{spec.description}}
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html` & `enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/templates/enrichapp/singlepageapp/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 {% with knowledge=spec.name|add:' '|add:app.name|add:' '|add:tags %}{{ block.super }}{% endwith %}
 {% endwith %}
 
 {% endblock breadcrumbs %}
 <!-- ============================= Address Bar End =============================== -->
 {% block nav_index%}
 <!--Header tab name-->
-    {% with nav_data="usecases" %}{{ block.super }}{% endwith %}
+    {% with nav_data="apps" %}{{ block.super }}{% endwith %}
 {% endblock %}
 <!--============================= Help Content =============================== -->
 {% block help %}
 {% include 'sharedapp/partials/help.html' with app=app spec=spec %}
 {{block.super}}
 {% endblock %}
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
 %} {% load static %}  {% block breadcrumbs %}
    1. Enrich
    2. Usecases
    3. {{usecase.org.name}}
    4. {{spec.name}}
 {% with tags=spec.tags|join:" " %} {% with knowledge=spec.name|add:' '|add:
 app.name|add:' '|add:tags %}{{ block.super }}{% endwith %} {% endwith %} {%
-endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="usecases" %}{
+endblock breadcrumbs %}  {% block nav_index%}  {% with nav_data="apps" %}{
 { block.super }}{% endwith %} {% endblock %}  {% block help %} {% include
 'sharedapp/partials/help.html' with app=app spec=spec %} {{block.super}} {%
 endblock %}  {% block content %}
 {% fontawesome_icon app.icon %}
 ****** {{app.verbose_name}} ******
 {{spec.name}}: {{spec.description}}
 {% include 'dashboard/_appusers.html' with usecase=usecase spec=spec %}
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/bases/singlepageapp/views.py` & `enrichsdk-4.7.9/enrichsdk/app/bases/singlepageapp/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,24 +74,24 @@
     def get_model(self, spec, name):
 
         from enrichapp.dashboard.globalapp import lib as globallib
 
         if (('models' in spec) and (name in spec['models'])):
             return spec['models'][name]
 
-        raise Exception("Not implemented")
+        return globallib.get_model(name)
 
     def get_form(self, spec, name):
 
         from enrichapp.dashboard.globalapp import lib as globallib
 
         if (('forms' in spec) and (name in spec['forms'])):
             return spec['forms'][name]
 
-        raise Exception("Not implemented")
+        return globallib.get_form(name)
 
     def validate_spec(self, spec):
 
         fill_action_gaps(spec, context={ })
 
         errors = default_validate_spec(spec)
         if len(errors) > 0:
@@ -132,15 +132,15 @@
         return ['Email']
 
     def take_action(self, request, spec, data, target):
 
         r = resolve(request.path)
 
         detailurl = request.build_absolute_uri(reverse(r.namespace + ":index")) + "?" + request.GET.urlencode()
-    
+
         try:
             if target.nature == "Email":
 
                 """{
                     "emails": [
                        "pingali@scribbledata.io"
                      ]
@@ -158,19 +158,19 @@
                 if len(fullname) == 0:
                     fullname = user.username
 
                 sender = fullname + "<" + get_default_from_email() +">"
                 receivers = policy['emails']
                 subject = f"{spec['name']} - Sharing Observation"
                 content = f"<p>{data['message']}</p>"
-                content += f"<p>You can find the full details at <a href='{detailurl}'>{spec['name']}</a> app"
+                content += f"<p>You can find the full details at <a href='{detailurl}'>{spec['name']}</a> app."
                 if (('data' in data) and (len(data) > 0)):
                     content += "Here is quick context:</p>"
-                    content += data['data']
-                
+                    content += "<p>" + data['data'] + "</p>"
+
                 msg = MIMEMultipart()
                 msg.attach(MIMEText(content, "html"))
                 send_html_email(content=content,
                                 sender=sender,
                                 receivers=receivers,
                                 subject=subject)
 
@@ -229,15 +229,15 @@
             })
 
         return status
 
 
     ################################################################
     # Data Access
-    ################################################################    
+    ################################################################
     def get_fs_handle(self, cred):
         """
         Get s3/gcs filesystem handle..
         """
         cred = get_credentials_by_name(cred)
         nature = cred['nature']
         if nature not in ['s3', 'gcs']:
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/utils.py` & `enrichsdk-4.7.9/enrichsdk/app/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 """
 Utilities meant for the dashboard apps
 """
 import sys
 import inspect
 import copy
+import random
+import string
 from ..lib.customer import find_usecase
 from django.apps import AppConfig
 
 def get_default_configuration():
     """
     Default description for any app
     """
@@ -124,19 +126,23 @@
     def is_enabled(self):
         return self.enable
 
     def __str__(self):
         return f"{self.name}: {self.verbose_name}"
 
 ##################################################
-# App helpers 
+# App helpers
 ##################################################
 def generate_id(name):
-    return "".join([c if c.isalnum() else "_" for c in name]).lower()
+    if len(name) > 0:
+        return "".join([c if c.isalnum() else "_" for c in name]).lower()
+    else:
+        chars = string.ascii_uppercase + string.digits
+        return ''.join(random.choices(chars, k=10))
 
 def clean_and_validate_widgets(widgets):
 
     for w in widgets:
         if 'id' not in w:
             w['id'] = generate_id(w['name'])
 
-    
+
```

### Comparing `enrichsdk-4.7.2/enrichsdk/app/widget/basewidget.py` & `enrichsdk-4.7.9/enrichsdk/app/widget/basewidget.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/app/widget/customcomponent.py` & `enrichsdk-4.7.9/enrichsdk/app/widget/customcomponent.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/app/widget/customwidget.py` & `enrichsdk-4.7.9/enrichsdk/app/widget/customwidget.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/commands/config.py` & `enrichsdk-4.7.9/enrichsdk/commands/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,27 +6,21 @@
 import platform
 import distro
 import getpass
 import logging
 from collections import OrderedDict
 import logging
 
+from enrichsdk.utils import SafeEncoder
+
 from . import log
 
 logger = logging.getLogger("app")
 
 
-class CustomEncoder(json.JSONEncoder):
-    def default(self, obj):
-        if isinstance(obj, datetime):
-            return obj.isoformat()
-        else:
-            return super().default(obj)
-
-
 #######################################################
 # Config object to handle a number of helper functions
 #######################################################
 class Config(object):
     """
     Context object having a number of capabilities including
     log management, files and path management, credentials
@@ -314,17 +308,17 @@
                 ("notes", self.state["notes"]),
                 ("log", os.path.relpath(self.log, self.rundir)),
             ]
         )
 
         if not self.readonly:
             with open(self.metadata, "w") as fd:
-                json.dump(metadata, fd, indent=4, cls=CustomEncoder)
+                json.dump(metadata, fd, indent=4, cls=SafeEncoder)
         elif self.show_metadata:
-            print(json.dumps(metadata, indent=4, cls=CustomEncoder), file=sys.stderr)
+            print(json.dumps(metadata, indent=4, cls=SafeEncoder), file=sys.stderr)
 
         if self.debug:
             logger.debug("Dumped execution metadata")
 
     # Logging start and end
     def start_run(self, cmd):
```

### Comparing `enrichsdk-4.7.2/enrichsdk/commands/decorators.py` & `enrichsdk-4.7.9/enrichsdk/commands/decorators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/commands/helper.py` & `enrichsdk-4.7.9/enrichsdk/commands/helper.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/commands/log.py` & `enrichsdk-4.7.9/enrichsdk/commands/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/commands/run.py` & `enrichsdk-4.7.9/enrichsdk/commands/run.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/anonymizer.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/anonymizer.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/changepoints.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/changepoints.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/llmtextgen.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/llmtextgen.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/profilespec.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/profilespec.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/assets/timeseries_forecasting.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/assets/timeseries_forecasting.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/catalog.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/catalog.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/logprocessor.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/logprocessor.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,22 +7,27 @@
     "MetricsBase",
     "AnomaliesBase",
     "SyntheticDataGeneratorBase",
     "DataObserverBase",
     "ChangePointDetectorBase",
     "TimeSeriesForecasterBase",
     "ClassifierBase",
+    'DataSanitizerBase',
+    'CustomEncoder'
 ]
 
+from enrichsdk.utils import SafeEncoder as CustomEncoder
+
 from .fileops import *
 from .filebased_query_executor import *
 from .inmemory_query_executor import *
 from .notebook_executor import *
 from .feature_compute import *
 from .metrics import *
 from .anomalies import *
 from .changepoints import *
 from .classifier import *
 from .timeseries_forecaster import *
 from .synthetic_data_generator import *
 from .observability import *
 from .data_quality import *
+from .data_sanitizer import *
```

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/anomalies/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/anomalies/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/changepoints/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/changepoints/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/classifier/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/classifier/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/data_quality/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/data_quality/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/feature_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/fileops/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/metrics/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/metrics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import logging
 from sqlalchemy import create_engine, text as satext
 from functools import partial
 
 logger = logging.getLogger("app")
 
 from enrichsdk.contrib.lib.assets import profilespec
-from enrichsdk.utils import get_lineage_of_query
+from enrichsdk.utils import get_lineage_of_query, get_yesterday, get_today
 from enrichsdk.lib.exceptions import NoDataFound
 
 
 def note(df, title):
     msg = title + "\n"
     msg += "--------" + "\n"
     msg += "Timestamp: " + str(datetime.now()) + "\n"
@@ -44,30 +44,14 @@
     if isinstance(df, pd.DataFrame):
         msg += "\nDtypes" + "\n"
         msg += df.dtypes.to_string() + "\n"
     msg += "------" + "\n"
     return msg
 
 
-class CustomEncoder(json.JSONEncoder):
-    def default(self, obj):
-        try:
-            return super().default(obj)
-        except:
-            return str(obj)
-
-
-def get_yesterday():
-    yesterday = date.today() + timedelta(days=-1)
-    return yesterday.isoformat()
-
-
-def get_today():
-    return date.today().isoformat()
-
 
 class MetricsBase(Compute):
     """
     Compute metrics as input for the anomaly/other computation
 
     Features of transform baseclass include:
```

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/notebook_executor/README.md` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/notebook_executor/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/notebook_executor/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/observability/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/observability/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/synthetic_data_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/lib/transforms/timeseries_forecaster/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/fileops/README.md` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/fileops/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/fileops/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/fileops/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsink/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/jsonsink/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsource/README.md` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/jsonsource/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/jsonsource/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/jsonsource/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/pqexport/README.md` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/pqexport/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/pqexport/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/pqexport/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/sqlexport/README.md` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/sqlexport/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/sqlexport/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/sqlexport/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesink/README.md` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/tablesink/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesink/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/tablesink/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesource/README.md` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/tablesource/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/contrib/transforms/tablesource/__init__.py` & `enrichsdk-4.7.9/enrichsdk/contrib/transforms/tablesource/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/__init__.py` & `enrichsdk-4.7.9/enrichsdk/core/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/frames.py` & `enrichsdk-4.7.9/enrichsdk/core/frames.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/mixins.py` & `enrichsdk-4.7.9/enrichsdk/core/mixins.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/node.py` & `enrichsdk-4.7.9/enrichsdk/core/node.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/patch.py` & `enrichsdk-4.7.9/enrichsdk/core/patch.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/render.py` & `enrichsdk-4.7.9/enrichsdk/core/render.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/res.py` & `enrichsdk-4.7.9/enrichsdk/core/res.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/run.py` & `enrichsdk-4.7.9/enrichsdk/core/run.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/sdk.py` & `enrichsdk-4.7.9/enrichsdk/core/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/state.py` & `enrichsdk-4.7.9/enrichsdk/core/state.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/core/widgets.py` & `enrichsdk-4.7.9/enrichsdk/core/widgets.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/datasets/__init__.py` & `enrichsdk-4.7.9/enrichsdk/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/datasets/discover.py` & `enrichsdk-4.7.9/enrichsdk/datasets/discover.py`

 * *Files 8% similar despite different names*

```diff
@@ -476,32 +476,55 @@
         Args:
             filename (str): A file that belongs to this dataset
             safe (bool): Whether file is trusted
             fd (object): File descriptor for s3/gcs/other non-filesystems
             nrows (int): Number of rows to sample
         """
 
+        skiprows = None
+        filesize = 0 # unknown
         if fd is None:
             # Text formats..
             if filename.split(".")[-1].lower() in ["csv", "tsv"]:
                 fd = open(filename)
             else:
                 fd = open(filename, "rb")
+            filesize = os.path.getsize(filename)
 
         # Read the file
         if filename.lower().endswith(".csv"):
-            df = pd.read_csv(fd, nrows=nrows)
+            if filesize > 10**9 : # 1GB
+                skiprows=lambda i: i % 100 != 0
+            df = pd.read_csv(fd, nrows=nrows, skiprows=skiprows)
         elif filename.lower().endswith(".csv.gz"):
-            df = pd.read_csv(fd, nrows=nrows, compression="gzip", error_bad_lines=False, encoding=encoding)
+            if filesize > 10**8 : # 100MB
+                skiprows=lambda i: i % 100 != 0
+            df = pd.read_csv(fd, nrows=nrows,
+                             compression="gzip",
+                             error_bad_lines=False,
+                             encoding=encoding,
+                             skiprows=skiprows)
         elif filename.lower().endswith(".tsv.gz"):
+            if filesize > 10**8 : # 100MB
+                skiprows=lambda i: i % 100 != 0
             df = pd.read_csv(
-                fd, nrows=nrows, sep="\t", compression="gzip", error_bad_lines=False, encoding=encoding
+                fd, nrows=nrows, sep="\t",
+                compression="gzip",
+                error_bad_lines=False,
+                encoding=encoding,
+                skiprows=skiprows
             )
         elif filename.lower().endswith(".tsv"):
-            df = pd.read_csv(fd, nrows=nrows, sep="\t", encoding=encoding)
+            if filesize > 10**9 : # 1GB
+                skiprows=lambda i: i % 100 != 0
+            df = pd.read_csv(fd,
+                             nrows=nrows,
+                             sep="\t",
+                             encoding=encoding,
+                             skiprows=skiprows)
         elif filename.lower().endswith(".pq") or filename.lower().endswith(
             ".pq.sample"
         ):
             df = pd.read_parquet(fd)
             if nrows is not None:
                 df = df.head(nrows)
         else:
```

### Comparing `enrichsdk-4.7.2/enrichsdk/datasets/doodle.py` & `enrichsdk-4.7.9/enrichsdk/datasets/doodle.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,15 @@
     ####################################################
     def get_performance(self, pid):
         status, result = self.access_server("/api/v1/performance",
                                             params={
                                                 'pid': str(pid)
                                             })
         if status >= 300:
-            raise Exception(f"Could obtain performance data")
+            raise Exception(f"Could not obtain performance data")
 
         return result
 
     ####################################################
     # Read source
     ####################################################
     def compute_source_paths(self, source, start, end):
```

### Comparing `enrichsdk-4.7.2/enrichsdk/datasets/generators.py` & `enrichsdk-4.7.9/enrichsdk/datasets/generators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/extractors/__init__.py` & `enrichsdk-4.7.9/enrichsdk/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/feature_compute/__init__.py` & `enrichsdk-4.7.9/enrichsdk/feature_compute/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/featurestore/__init__.py` & `enrichsdk-4.7.9/enrichsdk/featurestore/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/featurestore/schema.py` & `enrichsdk-4.7.9/enrichsdk/featurestore/schema.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/lib/__init__.py` & `enrichsdk-4.7.9/enrichsdk/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/lib/context.py` & `enrichsdk-4.7.9/enrichsdk/lib/context.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/lib/customer.py` & `enrichsdk-4.7.9/enrichsdk/lib/customer.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/lib/exceptions.py` & `enrichsdk-4.7.9/enrichsdk/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/lib/integration.py` & `enrichsdk-4.7.9/enrichsdk/lib/integration.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/lib/misc.py` & `enrichsdk-4.7.9/enrichsdk/lib/misc.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/lib/permissions.py` & `enrichsdk-4.7.9/enrichsdk/lib/permissions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/lib/renderlib.py` & `enrichsdk-4.7.9/enrichsdk/lib/renderlib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/lib/resources.py` & `enrichsdk-4.7.9/enrichsdk/lib/resources.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/notebook/__init__.py` & `enrichsdk-4.7.9/enrichsdk/notebook/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/package/__init__.py` & `enrichsdk-4.7.9/enrichsdk/package/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,31 +485,35 @@
 
     try:
         os.makedirs(target)
     except:
         pass
 
     defaults = load_enrichjson_defaults(target, usecase=False)
-
+    defaults.update({
+        'transform_name': "TransformName",
+        "transform_description": "Transform description"
+    })
     transform_root = get_template_path("metrics")
 
     context = {}
 
     # First copy the py files
     files = glob2.glob(transform_root + "/**")
     for f in files:
-        if f.endswith("~") or f == "__pycache__":
+        if f.endswith("~") or f.endswith("__pycache__"):
             continue
         content = open(f).read()
         variables = get_variables(f)
 
         for v in variables:
             context[v] = prompt(
                 "> " + v + ": ",
                 default=defaults.get(v, ""))
+
         basename = os.path.basename(f)
 
         # Write a local copy
         write_rendered_file(f, target, basename, context)
         print(greenbg(basename))
 
 
@@ -1288,14 +1292,16 @@
 export DJANGO_UWSGI_MODE="production"
 export EMAIL_HOST="email-smtp.us-east-1.amazonaws.com"
 export EMAIL_HOST_USER="AKIAZYH5XXX"
 export EMAIL_HOST_PASSWORD="BJGTIp88VjXXX"
 export EMAIL_PORT=587
 export EMAIL_USE_TLS="TRUE"
 
+# Suppress any python warnings
+export PYTHONWARNINGS=ignore
 
 """
     return djangoenv
 
 def get_sample_versionmap():
     versionmap = """\
 [
```

### Comparing `enrichsdk-4.7.2/enrichsdk/package/lib.py` & `enrichsdk-4.7.9/enrichsdk/package/lib.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/package/log.py` & `enrichsdk-4.7.9/enrichsdk/package/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/package/misc.py` & `enrichsdk-4.7.9/enrichsdk/package/misc.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/package/mock.py` & `enrichsdk-4.7.9/enrichsdk/package/mock.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,24 +16,15 @@
 
 from ..core.state import EnrichStateBase
 from ..core.frames import PandasDataFrame, DictDataFrame
 from ..lib import read_siteconf, read_versionmap
 from ..lib.context import Context
 import logging
 
-
-class CustomEncoder(json.JSONEncoder):
-    def default(self, obj):
-        try:
-            if "DataFrame" in obj.__class__.__name__:
-                return "<dataframe>"
-            return super().default(obj)
-        except:
-            return str(obj)
-
+from enrichsdk.utils import SafeEncoder
 
 logger = logging.getLogger("app")
 
 
 class MockRun(object):
     def __init__(self, *args, **kwargs):
         self.state = kwargs.pop("state")
@@ -636,15 +627,15 @@
                 "pid": self.state.pid,
                 "frames": self.state.state,
                 "expectations": self.state.expectations,
                 "accesses": self.accessed_files,
                 "dataset_accesses": self.state.dataset_accesses,
                 "versionmap": self.versionmap,
             },
-            cls=CustomEncoder,
+            cls=SafeEncoder,
             indent=4,
         )
 
         path = os.path.join(self.statedir, "metadata.json")
         with open(path, "w") as fd:
             fd.write(metadata)
```

### Comparing `enrichsdk-4.7.2/enrichsdk/package/validators.py` & `enrichsdk-4.7.9/enrichsdk/package/validators.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/policy/__init__.py` & `enrichsdk-4.7.9/enrichsdk/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/policy/sdk.py` & `enrichsdk-4.7.9/enrichsdk/policy/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/quality/__init__.py` & `enrichsdk-4.7.9/enrichsdk/quality/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/quality/base.py` & `enrichsdk-4.7.9/enrichsdk/quality/base.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/quality/exceptions.py` & `enrichsdk-4.7.9/enrichsdk/quality/exceptions.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/quality/expectations.py` & `enrichsdk-4.7.9/enrichsdk/quality/expectations.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/quality/reconciliation.py` & `enrichsdk-4.7.9/enrichsdk/quality/reconciliation.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/quality/transforms.py` & `enrichsdk-4.7.9/enrichsdk/quality/transforms.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/realtime/db.py` & `enrichsdk-4.7.9/enrichsdk/realtime/db.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/realtime/log.py` & `enrichsdk-4.7.9/enrichsdk/realtime/log.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/realtime/messaging.py` & `enrichsdk-4.7.9/enrichsdk/realtime/messaging.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/realtime/spark.py` & `enrichsdk-4.7.9/enrichsdk/realtime/spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/realtime/transforms.py` & `enrichsdk-4.7.9/enrichsdk/realtime/transforms.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/realtime/workflow.py` & `enrichsdk-4.7.9/enrichsdk/realtime/workflow.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/render/__init__.py` & `enrichsdk-4.7.9/enrichsdk/render/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/scripts/enrichcmd.py` & `enrichsdk-4.7.9/enrichsdk/scripts/enrichcmd.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/scripts/enrichpkg.py` & `enrichsdk-4.7.9/enrichsdk/scripts/enrichpkg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/usr/bin/env python3
 
+
 # Core
 import os
 import sys
 import pip
 import base64
 import subprocess
 import textwrap
 import json
 import imp
 import yaml
 import traceback
 import pkg_resources
 import logging, traceback
 import pyfiglet
+import warnings
 
 # thirdparty
 import click
 from pythonjsonlogger import jsonlogger
 from prompt_toolkit import prompt
 
 # Disable warnings
```

### Comparing `enrichsdk-4.7.2/enrichsdk/services/__init__.py` & `enrichsdk-4.7.9/enrichsdk/services/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/tasks/__init__.py` & `enrichsdk-4.7.9/enrichsdk/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/tasks/dummy_task/__init__.py` & `enrichsdk-4.7.9/enrichsdk/tasks/dummy_task/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/tasks/sdk.py` & `enrichsdk-4.7.9/enrichsdk/tasks/sdk.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/airflow/contrib-pipeline-v1.py` & `enrichsdk-4.7.9/enrichsdk/templates/airflow/contrib-pipeline-v1.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/appstore2.0/index.html.template` & `enrichsdk-4.7.9/enrichsdk/templates/appstore2.0/index.html.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/assets/datasets.py` & `enrichsdk-4.7.9/enrichsdk/templates/assets/datasets.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/config.json.template` & `enrichsdk-4.7.9/enrichsdk/templates/config.json.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/dashboard/persona.py` & `enrichsdk-4.7.9/enrichsdk/templates/dashboard/persona.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/dashboard/tasks.py` & `enrichsdk-4.7.9/enrichsdk/templates/dashboard/tasks.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/dashboard/templates/complex_result.html` & `enrichsdk-4.7.9/enrichsdk/templates/dashboard/templates/complex_result.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/dashboard/templates/index.html` & `enrichsdk-4.7.9/enrichsdk/templates/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/dashboard/urls.py` & `enrichsdk-4.7.9/enrichsdk/templates/dashboard/urls.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/dashboard/views.py` & `enrichsdk-4.7.9/enrichsdk/templates/dashboard/views.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/datasets.py.template` & `enrichsdk-4.7.9/enrichsdk/templates/datasets.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/helloworld.node.template` & `enrichsdk-4.7.9/enrichsdk/templates/helloworld.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/iris.node.template` & `enrichsdk-4.7.9/enrichsdk/templates/iris.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/metrics/__init__.py` & `enrichsdk-4.7.9/enrichsdk/templates/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/metrics/profilespec.py` & `enrichsdk-4.7.9/enrichsdk/templates/metrics/profilespec.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/pipelineconf.template` & `enrichsdk-4.7.9/enrichsdk/templates/pipelineconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/pipelinepyconf.template` & `enrichsdk-4.7.9/enrichsdk/templates/pipelinepyconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/prefect/default.py` & `enrichsdk-4.7.9/enrichsdk/templates/prefect/default.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/pyscript.template` & `enrichsdk-4.7.9/enrichsdk/templates/pyscript.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/query.node.template` & `enrichsdk-4.7.9/enrichsdk/templates/query.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/rscript.template` & `enrichsdk-4.7.9/enrichsdk/templates/rscript.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/setup.py.template` & `enrichsdk-4.7.9/enrichsdk/templates/setup.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/simpletransform.node.template` & `enrichsdk-4.7.9/enrichsdk/templates/simpletransform.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/singlepageapp.py.template` & `enrichsdk-4.7.9/enrichsdk/templates/singlepageapp.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/spark/README.md` & `enrichsdk-4.7.9/enrichsdk/templates/spark/README.md`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/enrich.py` & `enrichsdk-4.7.9/enrichsdk/templates/spark/dependencies/enrich.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/logging.py` & `enrichsdk-4.7.9/enrichsdk/templates/spark/dependencies/logging.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/spark/dependencies/spark.py` & `enrichsdk-4.7.9/enrichsdk/templates/spark/dependencies/spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/spark/jobs/run_spark.py` & `enrichsdk-4.7.9/enrichsdk/templates/spark/jobs/run_spark.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/spark/run.sh` & `enrichsdk-4.7.9/enrichsdk/templates/spark/run.sh`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/taskconf.template` & `enrichsdk-4.7.9/enrichsdk/templates/taskconf.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/tasklib.template` & `enrichsdk-4.7.9/enrichsdk/templates/tasklib.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/test_module.py.template` & `enrichsdk-4.7.9/enrichsdk/templates/test_module.py.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/transform.node.template` & `enrichsdk-4.7.9/enrichsdk/templates/transform.node.template`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/widgets/barchart.html` & `enrichsdk-4.7.9/enrichsdk/templates/widgets/barchart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/widgets/chart.html` & `enrichsdk-4.7.9/enrichsdk/templates/widgets/chart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/widgets/heatmap.html` & `enrichsdk-4.7.9/enrichsdk/templates/widgets/heatmap.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/widgets/hero.html` & `enrichsdk-4.7.9/enrichsdk/templates/widgets/hero.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/templates/widgets/linechart.html` & `enrichsdk-4.7.9/enrichsdk/templates/widgets/linechart.html`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/utils/__init__.py` & `enrichsdk-4.7.9/enrichsdk/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -154,7 +154,11 @@
 def get_tomorrow():
     tomorrow = date.today() + timedelta(days=1)
     return tomorrow.isoformat()
 
 def get_today():
     return date.today().isoformat()
 
+def get_daybefore():
+    daybefore = date.today() + timedelta(days=-2)
+    return daybefore.isoformat()
+
```

### Comparing `enrichsdk-4.7.2/enrichsdk/utils/excel.py` & `enrichsdk-4.7.9/enrichsdk/utils/excel.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/utils/redis.py` & `enrichsdk-4.7.9/enrichsdk/utils/redis.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk/utils/sample.py` & `enrichsdk-4.7.9/enrichsdk/utils/sample.py`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/enrichsdk.egg-info/PKG-INFO` & `enrichsdk-4.7.9/enrichsdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: enrichsdk
-Version: 4.7.2
+Version: 4.7.9
 Summary: Enrich Developer Kit
 Home-page: http://github.com/pingali/scribble-enrichsdk
 Author: Venkata Pingali
 Author-email: pingali@scribbledata.io
 License: All rights reserved
 Description: ==========
         Enrich SDK
@@ -95,11 +95,24 @@
              git push origin
         
         5. Install at customer::
         
              cd scribble-deploy
              fab install_enrichsdk:role=demo
         
+        6. Known issues
+        
+           The package dependencies are a jungle.Problematic packages include:
+        
+           boto3
+           botocore
+           aiobotocore
+           jupyter-events
+           nbconvert
+        
+        
+        
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `enrichsdk-4.7.2/enrichsdk.egg-info/SOURCES.txt` & `enrichsdk-4.7.9/enrichsdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/policy_select_dataset.html
 enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_detail.html
 enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/result_index.html
 enrichsdk/app/bases/policyapp/templates/enrichapp/policyapp/workflow_index.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/generic_index.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_button_function.html
+enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_donothing.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_icon.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/action_search.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/dropdown.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/notes.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/query_box.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/components/share_menu_action.html
 enrichsdk/app/bases/sharedapp/templates/sharedapp/partials/full_width_areachart.html
@@ -80,14 +81,15 @@
 enrichsdk/contrib/lib/assets/syndata.py
 enrichsdk/contrib/lib/assets/timeseries_forecasting.py
 enrichsdk/contrib/lib/transforms/__init__.py
 enrichsdk/contrib/lib/transforms/anomalies/__init__.py
 enrichsdk/contrib/lib/transforms/changepoints/__init__.py
 enrichsdk/contrib/lib/transforms/classifier/__init__.py
 enrichsdk/contrib/lib/transforms/data_quality/__init__.py
+enrichsdk/contrib/lib/transforms/data_sanitizer/__init__.py
 enrichsdk/contrib/lib/transforms/feature_compute/__init__.py
 enrichsdk/contrib/lib/transforms/filebased_query_executor/README.md
 enrichsdk/contrib/lib/transforms/filebased_query_executor/__init__.py
 enrichsdk/contrib/lib/transforms/filebased_query_executor/lib.py
 enrichsdk/contrib/lib/transforms/fileops/README.md
 enrichsdk/contrib/lib/transforms/fileops/__init__.py
 enrichsdk/contrib/lib/transforms/inmemory_query_executor/__init__.py
@@ -127,14 +129,15 @@
 enrichsdk/datasets/discover.py
 enrichsdk/datasets/doodle.py
 enrichsdk/datasets/generators.py
 enrichsdk/extractors/__init__.py
 enrichsdk/feature_compute/__init__.py
 enrichsdk/featurestore/__init__.py
 enrichsdk/featurestore/schema.py
+enrichsdk/hedwig/__init__.py
 enrichsdk/lib/__init__.py
 enrichsdk/lib/context.py
 enrichsdk/lib/customer.py
 enrichsdk/lib/exceptions.py
 enrichsdk/lib/integration.py
 enrichsdk/lib/misc.py
 enrichsdk/lib/permissions.py
```

### Comparing `enrichsdk-4.7.2/enrichsdk.egg-info/requires.txt` & `enrichsdk-4.7.9/enrichsdk.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 Jinja2==3.0.3
 Markdown>=2.9.10
 aiobotocore<=1.2.2,>=1.2.1
 aioitertools==0.8.0
-boto3==1.21.0
 botocore<=1.24.21,>=1.19.51
 click>=7.1.2
 colored==1.3.5
 coverage==5.5
 cryptography
 cytoolz>=0.9.0.1
 distributed==2.30.1
@@ -15,40 +14,42 @@
 flake8
 fsspec<=0.8.7,>=0.8.5
 gcsfs==0.6.0
 gitpython
 glob2==0.7
 google-cloud-logging
 great-expectations
+httpx
 humanize==0.5.1
 idna==2.8
 imblearn==0.0
 jsonschema>=3.2.0
-jupyter-core>=4.7.2
+jupyter-core>=4.12.0
 kafka-python==2.0.2
 logstash_formatter
 nbformat>=5.1.2
+numpy<=1.23.0
 openai
 pandas<1.5,>=1.3.5
 papermill>=2.3.4
 plotly>=4.0.0
 prefect<0.15.11,>=0.15.7
 pretty-html-table
 prompt-toolkit<3.1.0,>3.0.1
-prophet==1.1.2
+prophet==1.1.3
 pyarrow>=0.9.0
 pyfiglet
 pyhive
 pykafka
 pykafka==2.8.0
 pymongo
 pytest-cov
-pytest>=4.7.2
+pytest>=4.7.9
 python-dateutil>=2.8.1
-python-json-logger==0.1.8
+python-json-logger==2.0.4
 pytz>=2020.1
 raven==6.6.0
 redis
 requests-oauthlib==0.8.0
 requests==2.26.0
 ruptures
 s3fs<=0.5.2,>=0.5.1
```

### Comparing `enrichsdk-4.7.2/requirements.txt` & `enrichsdk-4.7.9/requirements.txt`

 * *Files identical despite different names*

### Comparing `enrichsdk-4.7.2/setup.py` & `enrichsdk-4.7.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("enrichsdk/__init__.py", "rb") as f:
     version = str(
         ast.literal_eval(_version_re.search(f.read().decode("utf-8")).group(1))
     )
 
 setup(
     name="enrichsdk",
-    version="4.7.2",
+    version="4.7.9",
     description="Enrich Developer Kit",
     long_description=readme,
     url="http://github.com/pingali/scribble-enrichsdk",
     author="Venkata Pingali",
     author_email="pingali@scribbledata.io",
     license="All rights reserved",
     scripts=[],
@@ -31,26 +31,29 @@
     install_requires=[
         "ruptures",
         "wheel",
         "click>=7.1.2",
         "aioitertools==0.8.0",
 
         "glob2==0.7",
+        "httpx",
         "requests==2.26.0",
         "requests-oauthlib==0.8.0",
-        "pytest>=4.7.2",
+        "pytest>=4.7.9",
         "pandas>=1.3.5,<1.5",
         "distributed==2.30.1",
         "idna==2.8",
         "coverage==5.5",
         "flake8",
         "raven==6.6.0",
-        "python-json-logger==0.1.8",
+        "python-json-logger==2.0.4",
         "python-dateutil>=2.8.1",
 
+        # numpy/statsmodels issues
+        "numpy<=1.23.0",
 
         # Celery breaks without these..
         # https://github.com/celery/celery/issues/7607
         "s3fs>=0.5.1,<=0.5.2",
         "fsspec>=0.8.5,<=0.8.7",
 
         "botocore>=1.19.51,<=1.24.21",
@@ -71,15 +74,15 @@
         "scipy<=1.10.0",
         "seaborn",
         #"flask_cors",
         #'moto>=1.3.14',
         "prefect>=0.15.7,<0.15.11",
         "distro>=1.4.0",
         "gcsfs==0.6.0",
-        "jupyter-core>=4.7.2",
+        "jupyter-core>=4.12.0",
         "nbformat>=5.1.2",
         "tzlocal>=2.0.0",
         "texttable",
         "pykafka",
         "redis",
         "gitpython",
         "logstash_formatter",
@@ -98,21 +101,21 @@
         "pymongo",
         "great-expectations",
         "openai",
         "pretty-html-table",
 
         # prophet dependencies
         "plotly>=4.0.0",
-        "prophet==1.1.2",
+        "prophet==1.1.3",
 
         # classification
         "imblearn==0.0",
 
         # Boto
-        "boto3==1.21.0"
+        #"boto3==1.16.0"
     ],
     entry_points={
         "console_scripts": [
             "enrichpkg=enrichsdk.scripts.enrichpkg:main",
         ],
     },
     classifiers=[
```

