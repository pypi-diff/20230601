# Comparing `tmp/vectice-23.2.3.1.tar.gz` & `tmp/vectice-23.2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectice-23.2.3.1.tar", last modified: Wed May 17 08:31:51 2023, max compression
+gzip compressed data, was "vectice-23.2.4.0.tar", last modified: Thu Jun  1 08:01:23 2023, max compression
```

## Comparing `vectice-23.2.3.1.tar` & `vectice-23.2.4.0.tar`

### file list

```diff
@@ -1,125 +1,127 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.381728 vectice-23.2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 08:31:38.000000 vectice-23.2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-17 08:31:51.381728 vectice-23.2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 08:31:38.000000 vectice-23.2.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-17 08:31:38.000000 vectice-23.2.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-17 08:31:51.381728 vectice-23.2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-17 08:31:38.000000 vectice-23.2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.361728 vectice-23.2.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.365728 vectice-23.2.3.1/src/vectice/
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.369728 vectice-23.2.3.1/src/vectice/api/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8534 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    22851 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/gql_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/gql_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/gql_code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/gql_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/gql_feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/gql_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/gql_user_workspace_api.py
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/http_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/http_error_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8956 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/iteration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.373728 vectice-23.2.3.1/src/vectice/api/json/
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/artifact_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/code_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/dataset_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/dataset_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/model_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/model_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/model_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/paged_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/property.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/public_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/user_and_workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/user_declared_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/json_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/rest_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/step.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/api/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.377728 vectice-23.2.3.1/src/vectice/models/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/attachment_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    13240 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/git_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10686 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/iteration.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/phase.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/project.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.377728 vectice-23.2.3.1/src/vectice/models/representation/
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/representation/dataset_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/representation/dataset_version_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/representation/model_representation.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/representation/model_version_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.377728 vectice-23.2.3.1/src/vectice/models/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7294 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/bigquery_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/description.py
--rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/file_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     6082 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/gcs_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.377728 vectice-23.2.3.1/src/vectice/models/resource/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/metadata/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/metadata/column_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/metadata/dataframe_column_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/metadata/db_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/metadata/files_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/metadata/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6703 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/resource/s3_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    30039 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/step.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/step_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/step_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/step_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/step_number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/step_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/models/workspace.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.381728 vectice-23.2.3.1/src/vectice/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/utils/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/utils/automatic_link_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/utils/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9469 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/utils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/utils/instance_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/utils/last_assets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/utils/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-17 08:31:38.000000 vectice-23.2.3.1/src/vectice/utils/vectice_ids_regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 08:31:51.365728 vectice-23.2.3.1/src/vectice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-17 08:31:51.000000 vectice-23.2.3.1/src/vectice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-05-17 08:31:51.000000 vectice-23.2.3.1/src/vectice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 08:31:51.000000 vectice-23.2.3.1/src/vectice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-17 08:31:51.000000 vectice-23.2.3.1/src/vectice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-17 08:31:51.000000 vectice-23.2.3.1/src/vectice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.726807 vectice-23.2.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-01 08:01:12.000000 vectice-23.2.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-01 08:01:23.730807 vectice-23.2.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 08:01:12.000000 vectice-23.2.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-01 08:01:12.000000 vectice-23.2.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-01 08:01:23.730807 vectice-23.2.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-01 08:01:12.000000 vectice-23.2.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.710807 vectice-23.2.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.710807 vectice-23.2.4.0/src/vectice/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.714807 vectice-23.2.4.0/src/vectice/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18521 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/gql_user_workspace_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/http_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/http_error_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8954 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/iteration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.722807 vectice-23.2.4.0/src/vectice/api/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/artifact_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/code_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/dataset_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1428 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/dataset_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/entity_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/model_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/model_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/model_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/paged_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/public_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/user_and_workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/user_declared_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/json_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8182 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/rest_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6142 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2514 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/api/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25210 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.722807 vectice-23.2.4.0/src/vectice/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/attachment_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14035 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6202 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/git_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10769 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/iteration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/phase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.726807 vectice-23.2.4.0/src/vectice/models/representation/
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/representation/dataset_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/representation/dataset_version_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/representation/model_representation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/representation/model_version_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.726807 vectice-23.2.4.0/src/vectice/models/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7267 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/bigquery_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5615 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/file_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5583 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/gcs_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.726807 vectice-23.2.4.0/src/vectice/models/resource/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/column_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5515 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/dataframe_column_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/db_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/files_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/metadata/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/resource/s3_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30033 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step_number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/step_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/models/workspace.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.726807 vectice-23.2.4.0/src/vectice/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/automatic_link_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5811 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/instance_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/last_assets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-01 08:01:12.000000 vectice-23.2.4.0/src/vectice/utils/vectice_ids_regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 08:01:23.714807 vectice-23.2.4.0/src/vectice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-01 08:01:23.000000 vectice-23.2.4.0/src/vectice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4047 2023-06-01 08:01:23.000000 vectice-23.2.4.0/src/vectice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 08:01:23.000000 vectice-23.2.4.0/src/vectice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-01 08:01:23.000000 vectice-23.2.4.0/src/vectice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 08:01:23.000000 vectice-23.2.4.0/src/vectice.egg-info/top_level.txt
```

### Comparing `vectice-23.2.3.1/LICENSE` & `vectice-23.2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/PKG-INFO` & `vectice-23.2.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.3.1
+Version: 23.2.4.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
 Platform: MacOS X
 Platform: Windows
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `vectice-23.2.3.1/setup.py` & `vectice-23.2.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         "rich",
         "urllib3",
         "gql[requests]",
         "GitPython",
         "packaging",
         "Pillow",
         "pandas",
+        "typing-extensions==4.6.2",
     ],
     extras_require={
         "dev": [
             "black",
             "gitpython",
             "mypy",
             "ruff",
@@ -81,15 +82,15 @@
         "gcs": ["google-cloud-storage>=1.17.0", "google-cloud-bigquery"],
         "s3": ["boto3"],
     },
     classifiers=[
         "Topic :: Internet",
         "Topic :: Scientific/Engineering :: Artificial Intelligence",
         "Topic :: Software Development :: Libraries :: Python Modules",
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

### Comparing `vectice-23.2.3.1/src/vectice/__init__.py` & `vectice-23.2.4.0/src/vectice/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/__init__.py` & `vectice-23.2.4.0/src/vectice/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/_auth.py` & `vectice-23.2.4.0/src/vectice/api/_auth.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from base64 import b64decode
 from datetime import datetime
 
 import requests
 import urllib3
 
 from vectice.__version__ import __vectice_version__, __version__
-from vectice.api._utils import read_env
 
 DEFAULT_API_ENDPOINT = "https://app.vectice.com"
 
 
 def default_http_headers() -> dict[str, str]:
     return {"Vectice-SDK-Version": __version__, "Vectice-Version": __vectice_version__}
 
@@ -36,57 +35,25 @@
 
 _logger = logging.getLogger(__name__)
 
 
 class Auth:  # nosec B107
     def __init__(
         self,
-        api_endpoint: str | None = None,
-        api_token: str | None = None,
-        token: str | None = None,
-        auto_connect=True,
-        allow_self_certificate=True,
+        api_endpoint: str,
+        api_token: str,
     ):
         self._default_request_headers: dict[str, str] = default_http_headers()
-        self._API_TOKEN = None
-        root_endpoint = format_url(self._get_endpoint(api_endpoint))
-        if api_token is not None:
-            self._API_TOKEN = api_token
-        else:
-            env_value = read_env("VECTICE_API_TOKEN")[0]
-            if env_value is not None:
-                self._API_TOKEN = env_value
-        if not self._API_TOKEN:
-            raise ValueError(
-                f"You must provide the api_token. You can generate them by going to the page {root_endpoint}/account/api-keys"
-            )
-        self._API_BASE_URL = root_endpoint
-        self.verify_certificate = not allow_self_certificate
-        if allow_self_certificate:
-            urllib3.disable_warnings()
-        self._jwt = None
-        self._jwt_expiration = None
-        if token:
-            self._token = token
-        elif auto_connect:
-            self._refresh_token()
-        self.vectice_path: str | None = None
-
-    def _get_endpoint(self, api_endpoint: str | None = None) -> str:
-        endpoint_env, endpoint = None, None
-        if api_endpoint is not None:
-            endpoint = api_endpoint
-        else:
-            endpoint_env = read_env("VECTICE_API_ENDPOINT")[0]
-        if endpoint_env is not None:
-            endpoint = endpoint_env
-        if not endpoint:
-            _logger.debug(f"no VECTICE_API_ENDPOINT provided. Using default endpoint {DEFAULT_API_ENDPOINT}")
-            endpoint = DEFAULT_API_ENDPOINT
-        return endpoint
+        self._API_TOKEN = api_token
+        self._API_BASE_URL = format_url(api_endpoint)
+        self.verify_certificate = False
+        self._jwt: str | None = None
+        self._jwt_expiration: int | None = None
+        urllib3.disable_warnings()
+        self._refresh_token()
 
     @property
     def _token(self) -> str | None:
         if self._jwt_expiration is None:
             return None
         # Refresh token 1 min before expiration
         if datetime.now().timestamp() >= self._jwt_expiration - 60:
@@ -120,17 +87,14 @@
 
     @staticmethod
     def _get_jwt_expiration(jwt: str) -> int:
         jwt_payload = jwt.split(".")[1]
         jwt_payload_with_padding = f"{jwt_payload}{'=' * (4 - len(jwt_payload) % 4)}"
         return int(json.loads(b64decode(jwt_payload_with_padding))["exp"])
 
-    def connect(self) -> None:
-        self._refresh_token()
-
     @property
     def api_base_url(self) -> str:
         return self._API_BASE_URL
 
     @property
     def http_headers(self) -> dict[str, str]:
         # ensure token is up to date
```

### Comparing `vectice-23.2.3.1/src/vectice/api/attachment.py` & `vectice-23.2.4.0/src/vectice/api/attachment.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,42 +49,42 @@
     ) -> tuple[str, str | None]:
         if isinstance(version, ModelVersionOutput):
             return self._generate_model_url_and_id(version)
 
         return self._generate_dataset_url_and_id(version)
 
     @staticmethod
-    def _build_url(project_id: str | int, version: str, type: str) -> str:
-        return f"/metadata/project/{project_id}/entityfiles/{type}/{version}"
+    def _build_url(project_id: str | int, version: str, file_type: str) -> str:
+        return f"/metadata/project/{project_id}/entityfiles/{file_type}/{version}"
 
     def post_attachment(
         self, files: list[tuple[str, tuple[str, BinaryIO]]], version: ModelVersionOutput | DatasetVersionOutput
     ) -> list[dict]:
         entity_files = []
-        url, repr = self._generate_version_url_and_id(version)
+        url, asset_repr = self._generate_version_url_and_id(version)
         if len(files) == 1:
             filename = files[0][1][0]
             try:
                 response = self._post_attachments(url, files)
                 if response:
                     entity_files.append(response.json())
-                _logger.debug(f"Attachment with name: {filename} successfully attached to {repr}.")
+                _logger.debug(f"Attachment with name: {filename} successfully attached to {asset_repr}.")
             except HttpError as e:
                 self._handle_http_error(e, version, filename)
         elif len(files) > 1:
             for file in files:
                 try:
                     response = self._post_attachments(url, [file])
                     if response:
                         entity_files.append(response.json())
                 except HttpError as e:
                     self._handle_http_error(e, version, file[1][0])
 
                 filenames = ", ".join([f[1][0] for f in files])
-                _logger.debug(f"Attachments with names: {filenames} successfully attached to {repr}.")
+                _logger.debug(f"Attachments with names: {filenames} successfully attached to {asset_repr}.")
         return entity_files
 
     def post_model_predictor(self, model_type: str, model_content: BytesIO, model_version: ModelVersionOutput) -> None:
         url, model_repr = self._generate_model_url_and_id(model_version)
         url += f"?modelFramework={model_type}"
         attachment = ("file", ("model_pickle", model_content))
         self._post_attachments(url, [attachment])
@@ -129,15 +129,15 @@
                 f"/metadata/project/{project_id}/entityfiles/codeversion/{code_version_id}/{file_id}"
             )
         except HttpError as e:
             self._handle_code_version_error(e, code_version_id)
 
     def list_attachments(self, version: ModelVersionOutput | DatasetVersionOutput) -> PagedResponse[AttachmentOutput]:
         try:
-            url, repr = self._generate_version_url_and_id(version)
+            url, _ = self._generate_version_url_and_id(version)
             if url is None:
                 raise InvalidReferenceError(MODEL_VERSION, version.id)
             attachments = self._list_attachments(url)
         except HttpError as e:
             self._handle_http_error(e, version)
         return PagedResponse(
             item_cls=AttachmentOutput,
@@ -159,31 +159,14 @@
         return PagedResponse(
             item_cls=AttachmentOutput,
             total=len(attachments),
             page={},
             items=attachments,
         )
 
-    def list_object_attachments(
-        self, project_id: str, code_version_id: int | None = None, phase_id: str | None = None
-    ) -> PagedResponse[AttachmentOutput]:
-        parent_object, object_id = self._identify_object(code_version_id, phase_id)
-        try:
-            attachments = self._list_attachments(
-                f"/metadata/project/{project_id}/entityfiles/{parent_object}/{object_id}"
-            )
-        except HttpError as e:
-            self._httpErrorHandler.handle_get_http_error(e, parent_object, object_id)
-        return PagedResponse(
-            item_cls=AttachmentOutput,
-            total=len(attachments),
-            page={},
-            items=attachments,
-        )
-
     def _handle_http_error(
         self,
         error: HttpError,
         version: ModelVersionOutput | DatasetVersionOutput | ModelVersionRepresentation | DatasetVersionRepresentation,
         file: str | None = None,
     ) -> NoReturn:
         ref_type = (
```

### Comparing `vectice-23.2.3.1/src/vectice/api/client.py` & `vectice-23.2.4.0/src/vectice/api/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 from vectice.__version__ import __version__
 from vectice.api._auth import Auth
 from vectice.api.attachment import AttachmentApi
 from vectice.api.compatibility import CompatibilityApi
 from vectice.api.gql_code import GqlCodeApi
 from vectice.api.gql_code_version import GqlCodeVersionApi
 from vectice.api.gql_dataset import GqlDatasetApi
+from vectice.api.gql_entity_file import GqlEntityFileApi
 from vectice.api.gql_feature_flag import GqlFeatureFlagApi
 from vectice.api.gql_model import GqlModelApi
 from vectice.api.gql_user_workspace_api import UserAndDefaultWorkspaceApi
 from vectice.api.http_error_handlers import MissingReferenceError, VecticeException
 from vectice.api.iteration import IterationApi
 from vectice.api.json import (
     ArtifactName,
     CodeInput,
     CodeVersionCreateBody,
     ModelRegisterInput,
     ModelRegisterOutput,
     ModelType,
     ModelVersionOutput,
     ModelVersionStatus,
-    Page,
     PagedResponse,
     PropertyInput,
     StepOutput,
 )
 from vectice.api.json.dataset_register import DatasetRegisterInput, DatasetRegisterOutput
 from vectice.api.json.dataset_representation import DatasetRepresentationOutput
 from vectice.api.json.dataset_version import DatasetVersionOutput
@@ -68,82 +68,27 @@
 
 
 DISABLED_FEATURE_FLAG_MESSAGE = (
     "This '{}' feature is not enabled. Please contact your Account Manager for Beta program access."
 )
 
 
-def _auth_success_message(workspace: WorkspaceOutput, project: ProjectOutput | None) -> str:
-    if workspace and project:
-        return f"Successfully authenticated. You'll be working on Project: '{project.name}', part of Workspace: '{workspace.name}'"
-    return f"Successfully authenticated. Your current Workspace: '{workspace.name}'"
-
-
 class Client:
     """Low level Vectice API client."""
 
     def __init__(
         self,
-        workspace: str | None = None,
-        project: str | None = None,
-        token: str | None = None,
-        api_endpoint: str | None = None,
-        auto_connect=True,
-        allow_self_certificate=True,
+        token: str,
+        api_endpoint: str,
     ):
-        self.auth = Auth(
-            api_endpoint=api_endpoint,
-            api_token=token,
-            auto_connect=auto_connect,
-            allow_self_certificate=allow_self_certificate,
-        )
+        self.auth = Auth(api_endpoint=api_endpoint, api_token=token)
         transport = RequestsHTTPTransport(url=self.auth.api_base_url + "/graphql", verify=self.auth.verify_certificate)
         logging.getLogger("gql.transport.requests").setLevel("WARNING")
         self._gql_client = GQLClient(transport=transport)
         self._logger = logging.getLogger(self.__class__.__name__)
-        self._workspace: WorkspaceOutput | None = None
-        self._project: ProjectOutput | None = None
-
-        if auto_connect:
-            if workspace and project:
-                self._project = self.get_project(project, workspace)
-                self._workspace = self._project.workspace
-                is_vectice_id = re.search(WORKSPACE_VID_REG, workspace)
-                if (not is_vectice_id and workspace != self._workspace.name) or (
-                    is_vectice_id and workspace != self._workspace.id
-                ):
-                    raise ValueError(
-                        f"Inconsistency in configuration: Project {project} does not belong to Workspace {workspace}"
-                    )
-            elif workspace:
-                self._workspace = self.get_workspace(workspace)
-            elif project:
-                self._project = self.get_project(project)
-                self._workspace = self._project.workspace
-
-            if self._workspace:
-                _logger.debug(_auth_success_message(workspace=self._workspace, project=self._project))
-
-    @property
-    def workspace(self) -> WorkspaceOutput | None:
-        """The workspace object.
-
-        Returns:
-            The workspace object.
-        """
-        return self._workspace
-
-    @property
-    def project(self) -> ProjectOutput | None:
-        """The project object.
-
-        Returns:
-            The project object.
-        """
-        return self._project
 
     @property
     def version_api(self) -> str:
         return __version__
 
     @property
     def version_backend(self) -> str:
@@ -155,32 +100,24 @@
 
     def check_compatibility(self) -> CompatibilityOutput:
         return CompatibilityApi(self.auth).check_version()
 
     def list_projects(
         self,
         workspace: str,
-        search: str | None = None,
-        page_index: int | None = Page.index,
-        page_size: int | None = Page.size,
-    ) -> list[ProjectOutput]:
+    ) -> PagedResponse[ProjectOutput]:
         """List the projects in a workspace.
 
         Parameters:
-            workspace: The workspace name or id.
-            search: A text to search for.
-            page_index: The index of the page.
-            page_size: The size of the page.
+            workspace: The workspace id.
 
         Returns:
             The workspace's projects.
         """
-        if not re.search(WORKSPACE_VID_REG, workspace):
-            workspace = WorkspaceApi(self._gql_client, self.auth).get_workspace(workspace).id
-        return ProjectApi(self._gql_client, self.auth).list_projects(workspace, search, page_index, page_size)
+        return ProjectApi(self._gql_client, self.auth).list_projects(workspace)
 
     def get_project(self, project: str, workspace: str | None = None) -> ProjectOutput:
         """Get a project.
 
         Parameters:
             project: The project name or vectice id.
             workspace: The workspace name or id.
@@ -199,28 +136,21 @@
             workspace: The workspace name or id.
 
         Returns:
             The workspace JSON structure.
         """
         return WorkspaceApi(self._gql_client, self.auth).get_workspace(workspace)
 
-    def list_workspaces(
-        self, search: str | None = None, page_index: int = 1, page_size: int = 100
-    ) -> list[WorkspaceOutput]:
+    def list_workspaces(self) -> PagedResponse[WorkspaceOutput]:
         """List the workspaces.
 
-        Parameters:
-            search: A text to search for.
-            page_index: The index of the page.
-            page_size: The size of the page.
-
         Returns:
             The workspaces.
         """
-        return WorkspaceApi(self._gql_client, self.auth).list_workspaces(search, page_index, page_size)
+        return WorkspaceApi(self._gql_client, self.auth).list_workspaces()
 
     def create_code_attachments(self, files: list[tuple[str, tuple[str, str]]], code_version_id: int, project_id: str):
         """Create an attachment.
 
         Parameters:
             files: The paths to the files to attach.
             code_version_id: The code version id to attach files to.
@@ -293,38 +223,14 @@
             version: The version to list attachments from.
 
         Returns:
             The attachments of an artifact.
         """
         return AttachmentApi(self.auth).list_attachments(version)
 
-    def list_code_attachments(self, code_version_id: int, project_id: str) -> PagedResponse[AttachmentOutput]:
-        """List the attachments of a code version.
-
-        Parameters:
-            code_version_id: The id of the code version to list attachments from.
-            project_id: The id of the project the code version belongs to.
-
-        Returns:
-            A list of attachments that belong to the code version.
-        """
-        return AttachmentApi(self.auth).list_object_attachments(project_id, code_version_id=code_version_id)
-
-    def list_phase_attachments(self, phase_id: str, project_id: str) -> PagedResponse[AttachmentOutput]:
-        """List the attachments of a phase.
-
-        Parameters:
-            phase_id: The id of the phase the attachments belongs to.
-            project_id: The id of the project the attachments belongs to.
-
-        Returns:
-            An attachment.
-        """
-        return AttachmentApi(self.auth).list_object_attachments(project_id, phase_id=phase_id)
-
     def get_code_version_attachment(self, code_version_id: int, project_id: str, file_id: int) -> Response:
         """Get the attachment of a code version.
 
         Parameters:
             code_version_id: The code version id to list attachments from.
             project_id: The project id the code version belongs to.
             file_id: The file id attached to the code version.
@@ -347,19 +253,16 @@
 
     def get_full_phase(self, phase: str) -> PhaseOutput:
         return PhaseApi(self._gql_client, self.auth).get_phase(phase=phase, full=True)
 
     def get_step_by_name(self, step_reference: str, iteration_id: str) -> StepOutput:
         return StepApi(self._gql_client, self.auth).get_step(step_reference, iteration_id)
 
-    def list_steps(
-        self,
-        iteration_id: str,
-    ) -> list[StepOutput]:
-        return StepApi(self._gql_client, self.auth).list_steps(iteration_id)
+    def list_steps(self, iteration_id: str, populate: bool = True) -> PagedResponse[StepOutput]:
+        return StepApi(self._gql_client, self.auth).list_steps(iteration_id, populate)
 
     def add_iteration_step_artifact(self, step_id: int, step_artifacts: IterationStepArtifactInput) -> StepOutput:
         return StepApi(self._gql_client, self.auth).add_iteration_step_artifact(step_artifacts, step_id)
 
     def update_iteration_step_artifact(
         self,
         step_id: int,
@@ -468,29 +371,14 @@
             f"name='{dataset_register_input.name}', "
             f"id={data['datasetVersion']['vecticeId']}, "
             f"version='{data['datasetVersion']['name']}', "
             f"type={dataset_register_input.type})."
         )
         return data
 
-    def get_project_and_workspace_references(self, project: str | None = None, workspace: str | None = None):
-        if project is None and self.project is not None:
-            project = self.project.id
-        if workspace is None and self.workspace is not None:
-            workspace = self.workspace.id
-        return project, workspace
-
-    def get_project_and_workspace_references_or_raise_error(
-        self, project: str | None = None, workspace: str | None = None
-    ) -> tuple[str, str | None]:
-        project, workspace = self.get_project_and_workspace_references(project, workspace)
-        if project is None:
-            raise MissingReferenceError("project")
-        return project, workspace
-
     @staticmethod
     def _get_model_name(library: str, technique: str, name: str | None = None) -> str:
         return name if name else f"{library} {technique} model"
 
     def register_model(
         self,
         model: Model,
@@ -549,12 +437,15 @@
         return GqlCodeApi(self._gql_client, self.auth).get_code(code, project_id)
 
     def get_code_version(self, code_version: str | int, code_id: int | None = None):
         if code_id is None:
             raise MissingReferenceError("code")
         return GqlCodeVersionApi(self._gql_client, self.auth).get_code_version(code_version, code_id)
 
+    def get_entity_file_by_id(self, id: int):
+        return GqlEntityFileApi(self._gql_client, self.auth).get_entity_file_by_id(id)
+
     def is_feature_flag_enabled(self, code: str) -> bool:
         enabled = GqlFeatureFlagApi(self._gql_client, self.auth).is_feature_flag_enabled(code)
         if enabled is False:
             _logger.info(DISABLED_FEATURE_FLAG_MESSAGE.format(code))
         return enabled
```

### Comparing `vectice-23.2.3.1/src/vectice/api/gql_api.py` & `vectice-23.2.4.0/src/vectice/api/gql_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     StepOutput,
     UserActivity,
     UserAndDefaultWorkspaceOutput,
     WorkspaceOutput,
 )
 from vectice.api.json.dataset_representation import DatasetRepresentationOutput
 from vectice.api.json.dataset_version_representation import DatasetVersionRepresentationOutput
+from vectice.api.json.entity_file import EntityFileOutput
 from vectice.api.json.model_representation import ModelRepresentationOutput
 from vectice.api.json.model_version_representation import ModelVersionRepresentationOutput
 
 if TYPE_CHECKING:
     from gql import Client
 
     from vectice.api._auth import Auth
@@ -70,14 +71,15 @@
             "Phase": PhaseOutput,
             "IterationStep": StepOutput,
             "Iteration": IterationOutput,
             "DatasetRegisterResultOutput": DatasetRegisterOutput,
             "ModelRegisterResultOutput": ModelRegisterOutput,
             "DataSet": DatasetRepresentationOutput,
             "DataSetVersion": DatasetVersionRepresentationOutput,
+            "EntityFile": EntityFileOutput,
             "Model": ModelRepresentationOutput,
             "ModelVersion": ModelVersionRepresentationOutput,
             "UserActivity": UserActivity,
             "Code": CodeOutput,
             "CodeVersion": CodeVersionOutput,
             "PublicConfigOutput": PublicConfigOutput,
             "UserAndDefaultWorkspaceOutput": UserAndDefaultWorkspaceOutput,
```

### Comparing `vectice-23.2.3.1/src/vectice/api/gql_code.py` & `vectice-23.2.4.0/src/vectice/api/gql_code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/gql_code_version.py` & `vectice-23.2.4.0/src/vectice/api/gql_code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/gql_dataset.py` & `vectice-23.2.4.0/src/vectice/api/gql_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/gql_feature_flag.py` & `vectice-23.2.4.0/src/vectice/api/gql_feature_flag.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
             keyword_arguments=kw,
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
             return response["isFeatureFlagEnabled"]  # type: ignore[no-any-return]
         except TransportQueryError:
-            return False
+            return True
```

### Comparing `vectice-23.2.3.1/src/vectice/api/gql_model.py` & `vectice-23.2.4.0/src/vectice/api/gql_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/gql_user_workspace_api.py` & `vectice-23.2.4.0/src/vectice/api/gql_user_workspace_api.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/http_error.py` & `vectice-23.2.4.0/src/vectice/api/http_error.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/http_error_handlers.py` & `vectice-23.2.4.0/src/vectice/api/http_error_handlers.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/iteration.py` & `vectice-23.2.4.0/src/vectice/api/iteration.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import TYPE_CHECKING
 
 from gql import gql
 from gql.transport.exceptions import TransportQueryError
 
 from vectice.api.gql_api import GqlApi, Parser
 from vectice.api.json.paged_response import PagedResponse
-from vectice.utils.api_utils import INDEX_ORDERED_DESC, PAGINATE_OUTPUT, get_phase_input
+from vectice.utils.api_utils import INDEX_ORDERED_DESC, PAGINATE_OUTPUT, get_page_input
 
 if TYPE_CHECKING:
     from vectice.api.json.iteration import IterationInput, IterationOutput
 
 _logger = logging.getLogger(__name__)
 
 _RETURNS_LIST = """vecticeId
@@ -135,15 +135,15 @@
         gql_query = "getIterationList"
         alias_filter = {"phaseId": parent_id, "onlyMine": only_mine}
         variable_types = "$filters:IterationFiltersInput!,$order:ListOrderInput,$page:PageInput"
         kw = "filters:$filters,order:$order,page:$page"
         variables = {
             "filters": alias_filter,
             "order": INDEX_ORDERED_DESC,
-            "page": get_phase_input(),
+            "page": get_page_input(),
         }
         query = GqlApi.build_query(
             gql_query=gql_query,
             variable_types=variable_types,
             returns=_RETURNS_PAGE,
             keyword_arguments=kw,
         )
```

### Comparing `vectice-23.2.3.1/src/vectice/api/json/__init__.py` & `vectice-23.2.4.0/src/vectice/api/json/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/artifact_version.py` & `vectice-23.2.4.0/src/vectice/api/json/artifact_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/code.py` & `vectice-23.2.4.0/src/vectice/api/json/code.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/code_version.py` & `vectice-23.2.4.0/src/vectice/api/json/code_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/dataset_register.py` & `vectice-23.2.4.0/src/vectice/api/json/dataset_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/dataset_representation.py` & `vectice-23.2.4.0/src/vectice/api/json/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/dataset_version.py` & `vectice-23.2.4.0/src/vectice/api/json/dataset_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/dataset_version_representation.py` & `vectice-23.2.4.0/src/vectice/api/json/dataset_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/files_metadata.py` & `vectice-23.2.4.0/src/vectice/api/json/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/iteration.py` & `vectice-23.2.4.0/src/vectice/api/json/iteration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/last_assets.py` & `vectice-23.2.4.0/src/vectice/api/json/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/metric.py` & `vectice-23.2.4.0/src/vectice/api/json/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/model.py` & `vectice-23.2.4.0/src/vectice/api/json/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/model_register.py` & `vectice-23.2.4.0/src/vectice/api/json/model_register.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/model_representation.py` & `vectice-23.2.4.0/src/vectice/api/json/model_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/model_version.py` & `vectice-23.2.4.0/src/vectice/api/json/model_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/model_version_representation.py` & `vectice-23.2.4.0/src/vectice/api/json/model_version_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/paged_response.py` & `vectice-23.2.4.0/src/vectice/api/json/paged_response.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/phase.py` & `vectice-23.2.4.0/src/vectice/api/json/phase.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/project.py` & `vectice-23.2.4.0/src/vectice/api/json/project.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/property.py` & `vectice-23.2.4.0/src/vectice/api/json/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/public_config.py` & `vectice-23.2.4.0/src/vectice/api/json/public_config.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/json/step.py` & `vectice-23.2.4.0/src/vectice/api/json/step.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,18 @@
         return str(self["description"])
 
     @property
     def slug(self) -> str:
         return str(self["slug"])
 
     @property
+    def artifacts_count(self) -> int:
+        return int(self["artifactsCount"])
+
+    @property
     def artifacts(self) -> list[IterationStepArtifact]:
         # TODO: refactor to break cyclic import
         from vectice.api.json.iteration import IterationStepArtifact
 
         return [IterationStepArtifact(artifact) for artifact in self["artifacts"]]
 
     @property
```

### Comparing `vectice-23.2.3.1/src/vectice/api/json/workspace.py` & `vectice-23.2.4.0/src/vectice/api/json/workspace.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/last_assets.py` & `vectice-23.2.4.0/src/vectice/api/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/phase.py` & `vectice-23.2.4.0/src/vectice/api/phase.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 from typing import TYPE_CHECKING
 
 from gql import gql
 from gql.transport.exceptions import TransportQueryError
 
 from vectice.api.gql_api import GqlApi, Parser
-from vectice.utils.api_utils import INDEX_ORDERED, PAGINATE_OUTPUT, get_phase_input
+from vectice.utils.api_utils import INDEX_ORDERED, PAGINATE_OUTPUT, get_page_input
 from vectice.utils.vectice_ids_regex import PHASE_VID_REG
 
 if TYPE_CHECKING:
     from vectice.api.json.paged_response import PagedResponse
     from vectice.api.json.phase import PhaseOutput
     from vectice.api.json.step import StepOutput
 
@@ -79,15 +79,15 @@
         variable_types = "$filters:PhaseFiltersInput!,$order:ListOrderInput,$page:PageInput"
         kw = "filters:$filters,order:$order,page:$page"
         variables = {
             "filters": {
                 "parentId": parent_id,
             },
             "order": INDEX_ORDERED,
-            "page": get_phase_input(),
+            "page": get_page_input(),
         }
         query = GqlApi.build_query(
             gql_query=gql_query, variable_types=variable_types, returns=_RETURNS_PAGE, keyword_arguments=kw
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
```

### Comparing `vectice-23.2.3.1/src/vectice/api/rest_api.py` & `vectice-23.2.4.0/src/vectice/api/rest_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,43 +59,43 @@
     def __init__(self, auth: Auth):
         self.auth = auth
         self.api_base_url = self.auth.api_base_url
         self.verify_certificate = self.auth.verify_certificate
         self._httpErrorHandler = ClientErrorHandler()
 
     def get(self, path: str) -> dict[str, Any]:
-        headers = {**self.auth.http_headers, "Content-Type": "application/json"}
+        headers = self._add_json_response_to_headers()
         log_request("GET", path, headers)
         response = requests.get(  # noqa: S113
             url=self.api_base_url + path, headers=headers, verify=self.verify_certificate
         )
         return self._response(self.api_base_url + path, headers, response, "GET")
 
     def post(self, path: str, payload: Any = None) -> JsonObject:
-        headers = {**self.auth.http_headers, "Content-Type": "application/json"}
+        headers = self._add_json_response_to_headers()
         cleaned_payload: Any = self._clean_dict(payload) if isinstance(payload, dict) else payload
         data = VecticeEncoder(indent=1).encode(cleaned_payload)
         log_request("POST", path, headers, data)
         response = requests.post(  # noqa: S113
             url=self.api_base_url + path, headers=headers, data=data, verify=self.verify_certificate
         )
         return self._response(self.api_base_url + path, headers, response, "POST", data)
 
     def put(self, path: str, payload: Any = None) -> JsonObject:
-        headers = {**self.auth.http_headers, "Content-Type": "application/json"}
+        headers = self._add_json_response_to_headers()
         cleaned_payload: Any = self._clean_dict(payload) if isinstance(payload, dict) else payload
         data = VecticeEncoder(indent=1).encode(cleaned_payload)
         log_request("PUT", path, headers, data)
         response = requests.put(  # noqa: S113
             url=self.auth.api_base_url + path, headers=headers, data=data, verify=self.verify_certificate
         )
         return self._response(self.auth.api_base_url + path, headers, response, "PUT", payload)
 
     def delete(self, path: str, payload: Any = None) -> JsonObject:
-        headers = {**self.auth.http_headers, "Content-Type": "application/json"}
+        headers = self._add_json_response_to_headers()
         if payload is None:
             data = None
         else:
             cleaned_payload: Any = self._clean_dict(payload) if isinstance(payload, dict) else payload
             data = VecticeEncoder(indent=1).encode(cleaned_payload)
         log_request("DELETE", path, headers, data)
         response = requests.delete(  # noqa: S113
@@ -136,21 +136,24 @@
 
     def _delete_attachment(self, path: str) -> Response | None:
         headers = self.auth.http_headers
         response = requests.delete(url=self.api_base_url + path, headers=headers)  # noqa: S113
         return self._attachment_response(self.api_base_url + path, headers, response, "DELETE")
 
     def _list_attachments(self, path: str) -> Sequence[dict]:
-        headers = {**self.auth.http_headers, "Content-Type": "application/json"}
+        headers = self._add_json_response_to_headers()
         response = requests.get(  # noqa: S113
             url=self.api_base_url + path, headers=headers, verify=self.verify_certificate
         )
         self._attachment_response(self.api_base_url + path, headers, response, "GET")
         return cast(Sequence[Dict], response.json())
 
+    def _add_json_response_to_headers(self) -> dict[str, str]:
+        return {**self.auth.http_headers, "Content-Type": "application/json"}
+
     @classmethod
     def raise_status(cls, path: str, response: Response, method: str, payload: Any | None = None) -> None:
         if not (200 <= response.status_code < 300):
             reason = response.text
             if not isinstance(payload, str):
                 json = VecticeEncoder(indent=4, sort_keys=True).encode(payload) if payload is not None else None
             else:
```

### Comparing `vectice-23.2.3.1/src/vectice/api/step.py` & `vectice-23.2.4.0/src/vectice/api/step.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from __future__ import annotations
 
 import logging
 from typing import TYPE_CHECKING
 
 from gql import gql
 
-from vectice.utils.api_utils import INDEX_ORDERED
+from vectice.utils.api_utils import INDEX_ORDERED, PAGINATE_OUTPUT, get_page_input
 
 if TYPE_CHECKING:
     from vectice.api.json import IterationStepArtifactInput, StepOutput
 
 from gql.transport.exceptions import TransportQueryError
 
 from vectice.api.gql_api import GqlApi, Parser
+from vectice.api.json.paged_response import PagedResponse
 from vectice.api.json.step import StepType
 
 _logger = logging.getLogger(__name__)
 
+_RETURNS_WITH_LIST = """
+                    index
+                    description
+                    slug
+                    artifactsCount
+                    __typename
+
+            """
+
 _RETURNS_WITH_STEPS = """
-                items {
                     id
                     index
                     name
                     completed
                     description
                     stepType
                     slug
@@ -34,17 +43,18 @@
                                 datasetVersion {
                                     vecticeId
                                 }
                                 text
                                 type
                     }
                     __typename
-                }
+
             """
 
+
 _RETURNS = """
                 id
                 index
                 name
                 completed
                 description
                 stepType
@@ -61,30 +71,35 @@
                                 type
                     }
                 __typename
             """
 
 
 class StepApi(GqlApi):
-    def list_steps(self, iteration_id: str) -> list[StepOutput]:
+    def list_steps(self, iteration_id: str, populate=True) -> PagedResponse[StepOutput]:
         gql_query = "getIterationStepList"
-        variable_types = "$parentId:VecticeId!,$order:ListOrderInput"
-        variables = {"parentId": iteration_id, "order": INDEX_ORDERED}
-        kw = "parentId:$parentId,order:$order"
+        variable_types = "$parentId:VecticeId!,$order:ListOrderInput,$page:PageInput"
+        kw = "parentId:$parentId,order:$order,page:$page"
+        variables = {
+            "parentId": iteration_id,
+            "order": INDEX_ORDERED,
+            "page": get_page_input() if not populate else get_page_input(1, 100),
+        }
+        _returns = _RETURNS_WITH_STEPS if populate is True else _RETURNS_WITH_LIST
         query = GqlApi.build_query(
             gql_query=gql_query,
             variable_types=variable_types,
-            returns=_RETURNS_WITH_STEPS,
+            returns=PAGINATE_OUTPUT.format(_returns),
             keyword_arguments=kw,
             query=True,
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
-            step_output: list[StepOutput] = Parser().parse_list(response[gql_query]["items"])
+            step_output: PagedResponse[StepOutput] = Parser().parse_paged_response(response[gql_query])
             return step_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "iteration", iteration_id)
 
     def add_iteration_step_artifact(self, data: IterationStepArtifactInput, step_id: int) -> StepOutput:
         gql_query = "addIterationStepArtifact"
         variable_types = "$id:Float!,$data:IterationStepArtifactInput!"
```

### Comparing `vectice-23.2.3.1/src/vectice/api/version.py` & `vectice-23.2.4.0/src/vectice/api/version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/api/workspace.py` & `vectice-23.2.4.0/src/vectice/api/workspace.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from __future__ import annotations
 
 import re
 from typing import TYPE_CHECKING
 
 from gql import gql
 
+from vectice.api.json.paged_response import PagedResponse
+from vectice.utils.api_utils import PAGINATE_OUTPUT, get_page_input
 from vectice.utils.vectice_ids_regex import WORKSPACE_VID_REG
 
 if TYPE_CHECKING:
     from vectice.api.json import WorkspaceOutput
 
 from gql.transport.exceptions import TransportQueryError
 
@@ -17,14 +19,16 @@
 _RETURNS = """
             name
             description
             vecticeId
             __typename
 """
 
+_RETURNS_PAGE = PAGINATE_OUTPUT.format(_RETURNS)
+
 
 class WorkspaceApi(GqlApi):
     def get_workspace(self, workspace: str) -> WorkspaceOutput:
         search_vectice_id = re.search(WORKSPACE_VID_REG, workspace)
         if search_vectice_id:
             gql_query = "getWorkspaceById"
             variable_types = "$workspaceId:VecticeId!"
@@ -42,36 +46,26 @@
         try:
             response = self.execute(query_built, variables)
             workspace_output: WorkspaceOutput = Parser().parse_item(response[gql_query])
             return workspace_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "workspace", workspace)
 
-    def list_workspaces(self, search: str | None, page_index: int, page_size: int) -> list[WorkspaceOutput]:
+    def list_workspaces(self) -> PagedResponse[WorkspaceOutput]:
         gql_query = "getUserWorkspaceList"
-        page = {
-            "index": page_index,
-            "size": page_size,
-        }
-        filters = {
-            "searchFilter": {"search": search if search is not None else "", "fields": "name"},
-        }
-        variable_types = "$page: PageInput!,$filters:WorkspaceListFiltersInput!"
-        variables = {"page": page, "filters": filters}
-        kw = "page:$page,filters:$filters"
-        returns = f"""items{{
-                    {_RETURNS}
-        }}"""
+        variable_types = "$page: PageInput!"
+        variables = {"page": get_page_input()}
+        kw = "page:$page"
         query = GqlApi.build_query(
             gql_query=gql_query,
             variable_types=variable_types,
-            returns=returns,
+            returns=_RETURNS_PAGE,
             keyword_arguments=kw,
             query=True,
         )
         query_built = gql(query)
         try:
             response = self.execute(query_built, variables)
-            workspace_output: list[WorkspaceOutput] = Parser().parse(response["getUserWorkspaceList"]["items"])  # type: ignore[assignment]
+            workspace_output: PagedResponse[WorkspaceOutput] = Parser().parse_paged_response(response[gql_query])
             return workspace_output
         except TransportQueryError as e:
             self._error_handler.handle_post_gql_error(e, "workspaces", "list")
```

### Comparing `vectice-23.2.3.1/src/vectice/connection.py` & `vectice-23.2.4.0/src/vectice/connection.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 import os
 import re
 from contextlib import suppress
 from pathlib import Path
 from textwrap import dedent
+from typing import overload
 
 import dotenv
 from rich.table import Table
 
 from vectice.api import Client
 from vectice.api.http_error_handlers import InvalidIdError
 from vectice.api.json.iteration import IterationOutput
@@ -23,29 +24,30 @@
 from vectice.models.representation.dataset_representation import DatasetRepresentation
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.representation.model_representation import ModelRepresentation
 from vectice.models.representation.model_version_representation import ModelVersionRepresentation
 from vectice.models.workspace import Workspace
 from vectice.utils.common_utils import _temp_print, hide_logs
 from vectice.utils.configuration import Configuration
+from vectice.utils.deprecation import deprecate
 from vectice.utils.last_assets import _connection_logging, _get_last_assets, _get_last_user_and_default_workspace
 from vectice.utils.logging_utils import CONNECTION_PROJECT_LOGGING, CONNECTION_WORKSPACE_LOGGING, format_description
 from vectice.utils.vectice_ids_regex import (
     DATASET_VERSION_VID_REG,
     DATASET_VID_REG,
     ITERATION_VID_REG,
     MODEL_VERSION_VID_REG,
     MODEL_VID_REG,
     PHASE_VID_REG,
     PROJECT_VID_REG,
     WORKSPACE_VID_REG,
 )
 
 _logger = logging.getLogger(__name__)
-DEFAULT_API_ENDPOINT = "https://app.vectice.com"
+DEFAULT_HOST = "https://app.vectice.com"
 CAN_NOT_BE_EMPTY_ERROR_MESSAGE = "%s can not be empty."
 
 
 class Connection:
     """Connect to the Vectice backend (application).
 
     The Connection class encapsulates a connection to the Vectice App.
@@ -88,53 +90,39 @@
         ".vectice",
         str(Path.home() / ".vectice"),
         ".env",
         str(Path.home() / ".env"),
         "/etc/vectice/api.cfg",
     ]
 
-    def __init__(
-        self,
-        api_token: str,
-        host: str,
-        workspace: str | None = None,
-        project: str | None = None,
-    ):
+    def __init__(self, api_token: str, host: str):
         """Initialize a connection.
 
         Parameters:
             api_token: Your private api token.
             host: The address of the Vectice application.
-            workspace: The workspace you want to work in.
-            project: The project you want to work in.
 
         Raises:
             RuntimeError: When the API and backend versions are incompatible.
         """
         logging.getLogger("Client").propagate = True
-        self._client = Client(
-            workspace=workspace,
-            project=project,
-            token=api_token,
-            api_endpoint=host,
-            auto_connect=True,
-            allow_self_certificate=True,
-        )
+        self._workspace: Workspace | None = None
+        self._client = Client(token=api_token, api_endpoint=host)
         compatibility = self._client.check_compatibility()
         if compatibility.status != "OK":
             if compatibility.status == "Error":
                 _logger.error(f"compatibility error: {compatibility.message}")
                 raise RuntimeError(f"compatibility error: {compatibility.message}")
             else:
                 _logger.warning(f"compatibility warning: {compatibility.message}")
 
     def __repr__(self) -> str:
         return (
             "Connection("
-            + f"workspace={self._client.workspace.name if self._client.workspace else 'None'}, "
+            + f"workspace={self._workspace.name if self._workspace else 'None'}, "
             + f"host={self._client.auth.api_base_url}, "
         )
 
     @property
     def version_api(self) -> str:
         return self._client.version_api
 
@@ -147,17 +135,15 @@
 
         Parameters:
             workspace: The id or the name of the desired workspace.
 
         Returns:
             The desired workspace.
         """
-        output = self._client.get_workspace(workspace)
-        result = Workspace(output.id, output.name, output.description)
-        result.__post_init__(self._client, self)
+        result = self._get_workspace_from_str(workspace)
         logging_output = dedent(
             f"""
                         Workspace {result.name!r} successfully retrieved."
 
                         For quick access to the workspace in the Vectice web app, visit:
                         {self._client.auth._API_BASE_URL}/browse/workspace/{result.id}"""
         ).lstrip()
@@ -234,24 +220,24 @@
             project: The id of the desired project.
 
         Returns:
             The desired project.
         """
         if not re.search(PROJECT_VID_REG, project):
             raise InvalidIdError("project", project)
-        output = self._client.get_project(project)
+        output = self._get_project_from_str(project)
         logging_output = dedent(
             f"""
                 Project {output.name!r} successfully retrieved."
 
                 For quick access to the Project in the Vectice web app, visit:
                 {self._client.auth._API_BASE_URL}/browse/project/{output.id}"""
         ).lstrip()
         _logger.info(logging_output)
-        return self._build_project_from_output(output)
+        return output
 
     def phase(self, phase: str) -> Phase:
         """Get a phase.
 
         Parameters:
             phase: The id of the desired phase.
 
@@ -385,30 +371,26 @@
     def list_workspaces(self) -> None:
         """Prints a list of workspaces in a tabular format, limited to the first 10 items. A link is provided to view the remaining workspaces.
 
         Returns:
             None
         """
         workspace_outputs = self._client.list_workspaces()
-        user_name, _ = _get_last_user_and_default_workspace(self._client)
 
         rich_table = Table(expand=True, show_edge=False)
-
         rich_table.add_column("workspace id", justify="left", no_wrap=True, min_width=4, max_width=10)
         rich_table.add_column("name", justify="left", no_wrap=True, max_width=20)
         rich_table.add_column("description", justify="left", no_wrap=True, max_width=50)
 
-        for count, workspace in enumerate(workspace_outputs, 1):
-            if count > 10:
-                break
+        for workspace in workspace_outputs.list:
             rich_table.add_row(str(workspace.id), workspace.name, format_description(workspace.description))
 
         description = dedent(
             f"""
-        There are {len(workspace_outputs)} workspaces and a maximum of 10 workspaces are displayed in the table below:"""
+        There are {workspace_outputs.total} workspaces and a maximum of 10 workspaces are displayed in the table below:"""
         ).lstrip()
         tips = dedent(
             """
         To access your personal workspace, use \033[1mconnection\033[0m.my_workspace
         To access a specific workspace, use \033[1mconnection\033[0m.workspace(Workspace ID)"""
         ).lstrip()
         link = dedent(
@@ -425,15 +407,15 @@
     def workspaces(self) -> list[Workspace] | None:
         """List the workspaces to which this connection has access.
 
         Returns:
             The workspaces to which this connection has access.
         """
         _, default_workspace_id = _get_last_user_and_default_workspace(self._client)
-        outputs = self._client.list_workspaces()
+        outputs = self._client.list_workspaces().list
         results: list[Workspace] = []
         for output in outputs:
             workspace = Workspace(id=output.id, name=output.name, description=output.description)
             workspace.__post_init__(self._client, self)
             if output.id == default_workspace_id:
                 results.insert(0, workspace)
                 continue
@@ -461,22 +443,44 @@
         """
         target_types = [activity for activity in ActivityTargetType]
         asset = _get_last_assets(target_types, self._client, _logger)
         if not asset or not asset.get("workspace"):
             raise ValueError("Workspace with activity not found.")
         return self.workspace(asset["workspace"]["vecticeId"])
 
+    @overload
+    @staticmethod
+    def connect(  # type: ignore[misc]
+        api_token: str | None = None,
+        host: str | None = None,
+        config: str | None = None,
+        workspace: str | None = None,
+        project: None = None,
+    ) -> Connection | Workspace | Project:
+        ...
+
+    @overload
+    @staticmethod
+    def connect(
+        api_token: str | None = None,
+        host: str | None = None,
+        config: str | None = None,
+        workspace: str | None = None,
+        project: str = "",
+    ) -> Project:
+        ...
+
     @staticmethod
     def connect(
         api_token: str | None = None,
         host: str | None = None,
         config: str | None = None,
         workspace: str | None = None,
         project: str | None = None,
-    ) -> Connection | Workspace | Project | None:
+    ) -> Connection | Workspace | Project:
         """Method to connect to the Vectice backend (application).
 
         Authentication credentials are retrieved, in order, from:
 
         1. keyword arguments
         2. configuration file (`config` parameter)
         3. environment variables
@@ -492,64 +496,72 @@
         webapp when creating an API token.
 
         Parameters:
             api_token: The api token provided by the Vectice webapp.
             host: The backend host to which the client will connect.
                 If not found, the default endpoint https://app.vectice.com is used.
             config: A JSON config file containing keys VECTICE_API_TOKEN and
-                VECTICE_API_ENDPOINT as well as optionally WORKSPACE and PROJECT.
+                VECTICE_HOST as well as optionally WORKSPACE and PROJECT.
             workspace: The name or id of an optional workspace to return.
             project: The name or id of an optional project to return.
 
         Raises:
             ValueError: When a project is specified without a workspace.
 
         Returns:
             A Connection, Workspace, or Project.
         """
         host = host or Connection._get_host(config)
         api_token = api_token or Connection._get_api_token(host, config)
-        workspace = workspace or Connection._get_workspace(config)
-        project = project or Connection._get_project(config)
-        connection = Connection(api_token=api_token, host=host, workspace=workspace, project=project)
+        workspace = workspace or Connection._get_config_workspace(config)
+        project = project or Connection._get_config_project(config)
+        connection = Connection(api_token=api_token, host=host)
         user_name, workspace_id = _get_last_user_and_default_workspace(connection._client)
         url = connection._client.auth.api_base_url
-        if workspace and not project:
-            return connection.get_workspace(workspace, user_name, url)
-        if workspace and project:
-            return connection.get_project(workspace, project, user_name, url)
+        if workspace:
+            return connection._log_workspace_or_project(workspace, project, user_name, url)
         _connection_logging(_logger, user_name, url, workspace_id)
         return connection
 
     @staticmethod
     def _get_host(config: str | None) -> str:
         try:
-            return Connection._get_config_item("VECTICE_API_ENDPOINT", config)
+            return Connection._get_config_item("VECTICE_HOST", config)
         except ValueError:
-            _logger.debug(f"No VECTICE_API_ENDPOINT provided. Using default endpoint {DEFAULT_API_ENDPOINT}")
-            return DEFAULT_API_ENDPOINT
+            # To remove in 23.3.1.0
+            try:
+                host = Connection._get_config_item("VECTICE_API_ENDPOINT", config)
+                _logger.warning(
+                    "VECTICE_API_ENDPOINT is deprecated and will be removed in 23.3.1.0, please use VECTICE_HOST instead."
+                )
+                return host
+            except ValueError:
+                pass
+
+            _logger.debug(f"No VECTICE_HOST provided. Using default host {DEFAULT_HOST}")
+            return DEFAULT_HOST
 
     @staticmethod
-    def _get_api_token(host: str | None, config: str | None) -> str:
+    def _get_api_token(host: str, config: str | None) -> str:
         try:
             return Connection._get_config_item("VECTICE_API_TOKEN", config)
         except ValueError as error:
             raise ValueError(
                 f"You must provide the api_token. You can generate them by going to the page {host}/account/api-keys"
             ) from error
 
     @staticmethod
-    def _get_workspace(config) -> str | None:
+    def _get_config_workspace(config) -> str | None:
         try:
             return Connection._get_config_item("WORKSPACE", config)
         except ValueError:
             return None
 
     @staticmethod
-    def _get_project(config) -> str | None:
+    def _get_config_project(config) -> str | None:
         try:
             return str(Connection._get_config_item("PROJECT", config))
         except ValueError:
             return None
 
     @staticmethod
     def _get_config_item(item_name: str, config_path: str | None) -> str:
@@ -569,29 +581,97 @@
             with hide_logs("dotenv"):
                 item = dotenv.get_key(path, item_name)
             if item:
                 _logger.debug(f"Found {item_name} in {path}")
                 return item
         raise ValueError(f"Could not find {item_name} in user configuration")
 
-    def get_workspace(self, workspace: str, user_name: str, host: str) -> Workspace:
-        workspace_output: Workspace = self.workspace(workspace)
+    def _log_workspace_or_project(
+        self, workspace: str, project: str | None, user_name: str, host: str
+    ) -> Workspace | Project:
+        workspace_output: Workspace = self._get_workspace_from_str(workspace)
+        if project:
+            project_obj = self._log_project(workspace_output, project, user_name, host)
+            self._workspace = project_obj.workspace
+            _logger.debug(
+                f"Successfully authenticated. You'll be working on Project: {project_obj.name!r}, part of Workspace: {project_obj.workspace.name!r}"
+            )
+            return project_obj
+
+        workspace_obj = self._log_workspace(workspace_output, user_name, host)
+        self._workspace = workspace_obj
+        _logger.debug(f"Successfully authenticated. Your current Workspace: {workspace_output.name!r}")
+        return workspace_obj
+
+    def _log_workspace(self, workspace_output: Workspace, user_name: str, host: str) -> Workspace:
         _logger.info(
             CONNECTION_WORKSPACE_LOGGING.format(
                 user=user_name, workspace_name=workspace_output.name, url=host, workspace_id=workspace_output.id
             )
         )
         return workspace_output
 
-    def get_project(self, workspace: str, project: str, user_name: str, host: str) -> Project:
-        workspace_output = self.workspace(workspace)
-        project_output: Project = workspace_output.project(project)
+    def _log_project(self, workspace_output: Workspace, project: str, user_name: str, host: str) -> Project:
+        project_output = self._get_project_from_str(project, workspace_output.id)
+
         _logger.info(
             CONNECTION_PROJECT_LOGGING.format(
                 user=user_name,
                 project_name=project_output.name,
                 url=host,
                 workspace_id=workspace_output.id,
                 project_id=project_output.id,
             )
         )
         return project_output
+
+    def _get_workspace_from_str(self, workspace: str) -> Workspace:
+        return self._build_workspace_from_output(self._client.get_workspace(workspace))
+
+    def _get_project_from_str(self, project: str, workspace: str | None = None) -> Project:
+        return self._build_project_from_output(self._client.get_project(project, workspace))
+
+    @staticmethod
+    @deprecate(
+        reason="Use _get_config_workspace(...) method instead.",
+        warn_at="23.2.4.0",
+        fail_at="23.2.5.0",
+        remove_at="23.2.6.0",
+    )
+    def _get_workspace(config) -> str | None:
+        try:
+            return Connection._get_config_item("WORKSPACE", config)
+        except ValueError:
+            return None
+
+    @staticmethod
+    @deprecate(
+        reason="Use _get_config_project(...) method instead.",
+        warn_at="23.2.4.0",
+        fail_at="23.2.5.0",
+        remove_at="23.2.6.0",
+    )
+    def _get_project(config) -> str | None:
+        try:
+            return str(Connection._get_config_item("PROJECT", config))
+        except ValueError:
+            return None
+
+    @deprecate(
+        reason="Use workspace(...) method instead.",
+        warn_at="23.2.4.0",
+        fail_at="23.2.5.0",
+        remove_at="23.2.6.0",
+    )
+    def get_workspace(self, workspace: str, user_name: str, host: str) -> Workspace:
+        workspace_output: Workspace = self._get_workspace_from_str(workspace)
+        return self._log_workspace(workspace_output, user_name, host)
+
+    @deprecate(
+        reason="Use project(...) method instead.",
+        warn_at="23.2.4.0",
+        fail_at="23.2.5.0",
+        remove_at="23.2.6.0",
+    )
+    def get_project(self, workspace: str, project: str, user_name: str, host: str) -> Project:
+        workspace_output: Workspace = self._get_workspace_from_str(workspace)
+        return self._log_project(workspace_output, project, user_name, host)
```

### Comparing `vectice-23.2.3.1/src/vectice/models/__init__.py` & `vectice-23.2.4.0/src/vectice/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/attachment_container.py` & `vectice-23.2.4.0/src/vectice/models/attachment_container.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/dataset.py` & `vectice-23.2.4.0/src/vectice/models/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime
 from typing import Union
 
+from typing_extensions import get_args
+
 from vectice.models.property import Property
 from vectice.models.representation.dataset_representation import DatasetRepresentation
 from vectice.models.representation.dataset_version_representation import DatasetVersionRepresentation
 from vectice.models.resource.base import Resource
 from vectice.models.resource.bigquery_resource import BigQueryResource
 from vectice.models.resource.metadata.base import DatasetSourceUsage, DatasetType
 
@@ -22,15 +24,15 @@
         self,
         type: DatasetType,
         name: str | None = None,
         resource: Resource | None = None,
         training_resource: Resource | None = None,
         testing_resource: Resource | None = None,
         validation_resource: Resource | None = None,
-        derived_from: list[TBaseDerivedFrom | Dataset] | None = None,
+        derived_from: list[TBaseDerivedFrom | Dataset] | TBaseDerivedFrom | Dataset | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
         attachments: str | list[str] | None = None,
     ):
         """Initialize a dataset.
 
         Users should not instantiate a dataset directly but rather use the provided static methods
         [`origin()`][vectice.models.dataset.Dataset.origin],
@@ -113,15 +115,15 @@
             attachments=attachments,
         )
 
     @staticmethod
     def clean(
         resource: Resource,
         name: str | None = None,
-        derived_from: list[str | Dataset | DatasetRepresentation | DatasetVersionRepresentation] | None = None,
+        derived_from: list[TBaseDerivedFrom | Dataset] | TBaseDerivedFrom | Dataset | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
         attachments: str | list[str] | None = None,
     ) -> Dataset:
         """Create a clean dataset.
 
         Examples:
             ```python
@@ -153,14 +155,15 @@
     def modeling(
         training_resource: Resource,
         testing_resource: Resource,
         validation_resource: Resource | None = None,
         name: str | None = None,
         properties: dict[str, str | int] | list[Property] | Property | None = None,
         attachments: str | list[str] | None = None,
+        derived_from: list[TBaseDerivedFrom | Dataset] | TBaseDerivedFrom | Dataset | None = None,
     ) -> Dataset:
         """Create a modeling dataset.
 
         Examples:
             ```python
             from vectice import Dataset, FileResource
 
@@ -175,23 +178,25 @@
         Parameters:
             training_resource: The resource for the training set (for modeling datasets).
             testing_resource: The resource for the testing set (for modeling datasets).
             validation_resource: The resource for the validation set (optional, for modeling datasets).
             name: The name of the dataset.
             properties: A dict, for example `{"folds": 32}`.
             attachments: Path of a file that will be attached to the step along with the dataset.
+            derived_from: A list of datasets (or ids) from which this dataset is derived.
         """
         return Dataset(
             type=DatasetType.MODELING,
             name=name,
             training_resource=training_resource,
             testing_resource=testing_resource,
             validation_resource=validation_resource,
             properties=properties,
             attachments=attachments,
+            derived_from=derived_from,
         )
 
     def __repr__(self):
         return f"Dataset(name={self.name!r}, type={self.type!r})"
 
     @property
     def type(self) -> DatasetType:
@@ -327,25 +332,39 @@
         return properties
 
 
 TDerivedFrom = Union[TBaseDerivedFrom, Dataset]
 
 
 def _get_derived_from(
-    derived_from: list[TDerivedFrom] | None,
+    derived_from: list[TDerivedFrom] | TDerivedFrom | None,
 ) -> list[str]:
     derived_from_ids: list[str] = []
-    for df in derived_from or []:
+    formatted_df = _format_derived_from(derived_from)
+    for df in formatted_df or []:
         if isinstance(df, Dataset):
             if df.latest_version_id is None:
                 raise ValueError(
                     f"Dataset {df.name!r} does not have a version id. "
                     "Was it registered in Vectice (assigned to a step)?"
                 )
             derived_from_ids.append(df.latest_version_id)
         elif isinstance(df, DatasetRepresentation):
             derived_from_ids.append(df.version.id)
         elif isinstance(df, DatasetVersionRepresentation):
             derived_from_ids.append(df.id)
         else:
             derived_from_ids.append(df)
     return derived_from_ids
+
+
+def _format_derived_from(derived_from: list[TDerivedFrom] | TDerivedFrom | None) -> list[TDerivedFrom]:
+    if derived_from is None:
+        return []
+
+    formatted_derived_from = derived_from if isinstance(derived_from, list) else [derived_from]
+
+    for df in formatted_derived_from:
+        if not isinstance(df, get_args(TDerivedFrom)):
+            raise ValueError("Invalid derived_from parameter")
+
+    return formatted_derived_from
```

### Comparing `vectice-23.2.3.1/src/vectice/models/git_version.py` & `vectice-23.2.4.0/src/vectice/models/git_version.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/iteration.py` & `vectice-23.2.4.0/src/vectice/models/iteration.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from vectice.api.http_error_handlers import NoStepsInPhaseError, VecticeException
 from vectice.api.json.iteration import (
     IterationInput,
     IterationStatus,
 )
 from vectice.utils.common_utils import _check_read_only, _get_step_type, _temp_print
-from vectice.utils.last_assets import _get_last_user_and_default_workspace
+from vectice.utils.logging_utils import get_iteration_status
 
 if TYPE_CHECKING:
     from vectice import Connection
     from vectice.api import Client
     from vectice.models import Phase, Project, Step, Workspace
     from vectice.models.model import Model
 
@@ -140,15 +140,15 @@
             )
             return step_object
         raise AttributeError(f"The attribute '{item}' does not exist.")
 
     def __setattr__(self, attr_name, attr_value):
         if hasattr(self, "_steps") and attr_name in super().__getattribute__("_steps"):
             if self._status in {IterationStatus.Abandoned, IterationStatus.Completed}:
-                raise VecticeException(f"The Iteration is {self._status.name} and is read-only!")
+                raise VecticeException(f"The Iteration is {self.status} and is read-only!")
             self._steps[attr_name] = self._steps[attr_name]._step_factory_and_update(value=attr_value)
         elif hasattr(self, "__dict__") and attr_name not in self.__slots__:
             raise AttributeError(f"The attribute '{attr_name}' does not exist.")
         else:
             super().__setattr__(attr_name, attr_value)
 
     @property
@@ -176,14 +176,23 @@
 
         Returns:
             The iteration's index.
         """
         return self._index
 
     @property
+    def status(self) -> str:
+        """The iteration's status.
+
+        Returns:
+            The iteration's status.
+        """
+        return get_iteration_status(self._status)
+
+    @property
     def completed(self) -> bool:
         """Whether this iteration is completed.
 
         Returns:
             Whether the iteration is completed.
         """
         return self._status is IterationStatus.Completed
@@ -222,39 +231,34 @@
                 index=item.index,
                 slug=item.slug,
                 description=item.description,
                 completed=item.completed or None,
                 artifacts=item.artifacts,
                 step_type=item.step_type,
             )
-            for item in steps_output
+            for item in steps_output.list
         ]
 
     def list_steps(self) -> None:
-        """Prints a list of steps belonging to the iteration in a tabular format, limited to the first 10 items. A link is provided to view the remaining steps.
+        """Prints a list of steps belonging to the iteration in a tabular format, limited to the first 10 steps. A link is provided to view the remaining steps.
 
         Returns:
             None
         """
-        steps_output = self._client.list_steps(self.id)
-        user_name, _ = _get_last_user_and_default_workspace(self._client)
+        steps_output = self._client.list_steps(self.id, populate=False)
 
         rich_table = Table(expand=True, show_edge=False)
 
-        rich_table.add_column("index", justify="left", no_wrap=True, min_width=5, max_width=5)
-        rich_table.add_column("shortcut", justify="left", no_wrap=True, min_width=5, max_width=20)
-        rich_table.add_column("artifacts", justify="left", no_wrap=True, min_width=5, max_width=15)
-
-        for count, step in enumerate(steps_output, 1):
-            if count > 10:
-                break
-            number_of_artifacts = len(step.artifacts)
-            rich_table.add_row(str(count), step.slug, str(number_of_artifacts))
-
-        description = f"""There are {len(steps_output)} steps in Iteration '{self.index!r}' and a maximum of 10 steps are displayed in the table below:"""
+        rich_table.add_column("Shortcut", justify="left", no_wrap=True, min_width=5, max_width=20)
+        rich_table.add_column("Registered items (count)", justify="left", no_wrap=True, min_width=5, max_width=15)
+        rich_table.add_column("Description", justify="left", no_wrap=True, min_width=5, max_width=35)
+
+        for step in steps_output.list:
+            rich_table.add_row(step.slug, str(step.artifacts_count), step.description)
+        description = f"""There are {steps_output.total} steps in Iteration '{self.index!r}' and a maximum of 10 steps are displayed in the table below:"""
         tips = dedent(
             """
         To access a specific step, use the step shortcut \033[1iiteration\033[0m.step_my_step_name
         The step reference is referred to as shortcut"""
         ).lstrip()
         link = dedent(
             f"""
@@ -268,33 +272,34 @@
         _temp_print(link)
 
     def cancel(self) -> None:
         """Cancel the iteration by abandoning all unfinished steps."""
         iteration_input = IterationInput(status=IterationStatus.Abandoned.name)
         self._client.update_iteration(self.id, iteration_input)
         self._status = IterationStatus.Abandoned
-        _logger.info(f"Iteration with index {self.index} canceled.")
+        _logger.info(f"Iteration with index {self.index} cancelled.")
 
     def complete(self) -> None:
         """Mark the iteration as completed."""
         if self._status is IterationStatus.Abandoned:
-            raise VecticeException("The iteration is canceled and cannot be completed.")
+            raise VecticeException("The iteration is cancelled and cannot be completed.")
         iteration_input = IterationInput(status=IterationStatus.Completed.name)
         self._client.update_iteration(self.id, iteration_input)
         self._status = IterationStatus.Completed
         logging_output = dedent(
             f"""
                         Iteration with index {self.index} completed.
 
                         For quick access to the Iteration in the Vectice web app, visit:
                         {self._client.auth._API_BASE_URL}/browse/iteration/{self.id}"""
         ).lstrip()
         _logger.info(logging_output)
 
     def delete(self) -> None:
+        """Permanently deletes the iteration."""
         self._client.delete_iteration(self.id)
         _logger.info(f"Iteration with index {self.index} was deleted.")
 
     @property
     def connection(self) -> Connection:
         """The connection to which this iteration belongs.
```

### Comparing `vectice-23.2.3.1/src/vectice/models/metric.py` & `vectice-23.2.4.0/src/vectice/models/metric.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/model.py` & `vectice-23.2.4.0/src/vectice/models/model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/phase.py` & `vectice-23.2.4.0/src/vectice/models/phase.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 from rich.table import Table
 
 from vectice.api.http_error_handlers import InvalidReferenceError
 from vectice.api.json.phase import PhaseStatus
 from vectice.models.iteration import Iteration
 from vectice.utils.common_utils import _temp_print
+from vectice.utils.deprecation import deprecate
 from vectice.utils.last_assets import _get_last_user_and_default_workspace
 from vectice.utils.logging_utils import format_description, get_iteration_status
 from vectice.utils.vectice_ids_regex import ITERATION_VID_REG
 
 if TYPE_CHECKING:
     from vectice import Connection
     from vectice.api import Client
@@ -166,14 +167,20 @@
 
         Returns:
             A dictionary containing the `name`, `id`, and `index` items.
         """
         return {"name": self.name, "id": self.id, "index": self.index}
 
     @property
+    @deprecate(
+        reason="Use list_iterations() instead.",
+        warn_at="23.2.3.0",
+        fail_at="23.2.5.0",
+        remove_at="23.2.6.0",
+    )
     def iterations(self) -> list[Iteration]:
         """The phase's iterations.
 
         Returns:
             The phase's iterations.
         """
         iteration_outputs = self._client.list_iterations(self.id)
@@ -209,17 +216,26 @@
         # For quick access to the list of iterations in the Vectice web app, visit:
         # {self._client.auth._API_BASE_URL}/phase/{self.id}/iterations?w={self.workspace.id}"""
         ).lstrip()
         _temp_print(description)
         _temp_print(table=rich_table)
         _temp_print(link)
 
+    @deprecate(
+        reason="This method is deprecated, to get your list of steps use the list_steps() of the iteration object.",
+        warn_at="23.2.4.0",
+        fail_at="23.2.5.0",
+        remove_at="23.2.6.0",
+    )
     def list_steps(self) -> None:
         """Prints a list of step definitions belonging to the phase in a tabular format, limited to the first 10 items. A link is provided to view the remaining step definitions.
 
+        > **Deprecated** <br>
+        > To get your list of steps use the list_steps() of the iteration object.
+
         Returns:
             None
         """
         steps_output = self._client.list_step_definitions(self.id)
         user_name, _ = _get_last_user_and_default_workspace(self._client)
 
         rich_table = Table(expand=True, show_edge=False)
```

### Comparing `vectice-23.2.3.1/src/vectice/models/project.py` & `vectice-23.2.4.0/src/vectice/models/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,20 +166,20 @@
 
         Returns:
             None
         """
         phase_outputs = self._client.list_phases(project=self.id)
         rich_table = Table(expand=True, show_edge=False)
 
-        rich_table.add_column("phase id", justify="left", no_wrap=True, min_width=3, max_width=5)
-        rich_table.add_column("name", justify="left", no_wrap=True, min_width=5, max_width=10)
-        rich_table.add_column("owner", justify="left", no_wrap=True, min_width=4, max_width=4)
-        rich_table.add_column("status", justify="left", no_wrap=True, min_width=4, max_width=4)
-        rich_table.add_column("iterations", justify="left", no_wrap=True, min_width=4, max_width=4)
-        rich_table.add_column("steps", justify="left", no_wrap=True, max_width=10)
+        rich_table.add_column("Phase id", justify="left", no_wrap=True, min_width=3, max_width=5)
+        rich_table.add_column("Name", justify="left", no_wrap=True, min_width=5, max_width=10)
+        rich_table.add_column("Owner", justify="left", no_wrap=True, min_width=4, max_width=4)
+        rich_table.add_column("Status", justify="left", no_wrap=True, min_width=4, max_width=4)
+        rich_table.add_column("Iterations", justify="left", no_wrap=True, min_width=4, max_width=4)
+        rich_table.add_column("Steps", justify="left", no_wrap=True, max_width=10)
 
         for phase in phase_outputs.list:
             phase_owner = phase["owner"]["name"] if phase.get("owner") else "Unassigned"
             phase_status = get_phase_status(phase.status)
             rich_table.add_row(
                 phase.id,
                 phase.name,
```

### Comparing `vectice-23.2.3.1/src/vectice/models/property.py` & `vectice-23.2.4.0/src/vectice/models/property.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/representation/dataset_representation.py` & `vectice-23.2.4.0/src/vectice/models/representation/dataset_representation.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/__init__.py` & `vectice-23.2.4.0/src/vectice/models/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/base.py` & `vectice-23.2.4.0/src/vectice/models/resource/base.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,16 +4,14 @@
 from typing import TYPE_CHECKING
 
 from pandas import DataFrame
 
 from vectice.models.resource.metadata.base import DatasetSourceOrigin, Metadata
 
 if TYPE_CHECKING:
-    from google.cloud.bigquery import Table
-
     from vectice.models.resource.metadata.base import DatasetSourceUsage
 
 
 class Resource(metaclass=ABCMeta):
     """Base class for resources.
 
     Use Resource subclasses to assign datasets to steps.  The
@@ -60,47 +58,47 @@
             [DBMetadata][vectice.models.resource.metadata.DBMetadata] for data stored in a database.
     """
 
     # origin must be a string because users can subclass resources
     # and set a custom origin
     _origin: str = DatasetSourceOrigin.OTHER.value
 
+    _files_limit = 5000
+
     @abstractmethod
     def __init__(self, paths: list[str] | str, dataframes: DataFrame | list[DataFrame] | None = None):
         """Initialize a resource."""
         self._metadata: Metadata | None = None
-        self._data: dict[str, bytes] | dict[str, bytes | None] | dict[
-            str, tuple[Table | None, DataFrame | None]
-        ] | None = None
+        self._data: dict | None = None
 
         self._paths = paths if isinstance(paths, list) else [paths]
 
         self._dataframes = dataframes if isinstance(dataframes, list) or dataframes is None else [dataframes]
         if self._dataframes is not None:
             for dataframe in self._dataframes:
                 if dataframe is not None and not isinstance(dataframe, DataFrame):
                     raise ValueError(
                         f"Argument 'dataframe' of type '{type(dataframe)}' is invalid, only pandas DataFrame is supported."
                     )
 
     @property
-    def data(self) -> dict[str, bytes] | dict[str, bytes | None] | dict[str, tuple[Table | None, DataFrame | None]]:
+    def data(self) -> dict:
         """The resource's data.
 
         Returns:
             The resource's data.
         """
         if self._data is None:
             self._data = self._fetch_data()
         return self._data
 
     @abstractmethod
     def _fetch_data(
         self,
-    ) -> dict[str, bytes] | dict[str, bytes | None] | dict[str, tuple[Table | None, DataFrame | None]]:
+    ) -> dict:
         pass
 
     @abstractmethod
     def _build_metadata(self) -> Metadata:
         pass
 
     @property
```

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/bigquery_resource.py` & `vectice-23.2.4.0/src/vectice/models/resource/bigquery_resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                 df_index += 1
             return tables_dict, df_index
         except Forbidden:
             _logger.warning(f"Failed to list tables for dataset {path}")
             return {}, 0
 
     def _build_metadata(self) -> DBMetadata:
-        tables_metadata: dict[str, tuple[Table | None, DataFrame | None]] = self.data  # type:ignore[assignment]
+        tables_metadata: dict[str, tuple[Table | None, DataFrame | None]] = self.data
         dbs: list[MetadataDB] = []
         for table_name, [table_metadata, dataframe] in tables_metadata.items():
             columns: list[DBColumn] = []
             size = None
             rows_number = None
             updated_date = None
             created_date = None
```

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/description.py` & `vectice-23.2.4.0/src/vectice/models/resource/description.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/file_resource.py` & `vectice-23.2.4.0/src/vectice/models/resource/file_resource.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/gcs_resource.py` & `vectice-23.2.4.0/src/vectice/models/resource/gcs_resource.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 from __future__ import annotations
 
+import logging
 import re
 from typing import TYPE_CHECKING
 
 from pandas import DataFrame
 
 from vectice.models.resource.base import Resource
 from vectice.models.resource.metadata import DatasetSourceOrigin
 from vectice.models.resource.metadata.files_metadata import File, FilesMetadata
 
 if TYPE_CHECKING:
-    from google.cloud.storage import Blob, Bucket, Client
+    from google.cloud.storage import Blob, Client
 
 GS_URI_REG = r"(gs:\/\/)([^\/]+)\/(.+)"
 
+_logger = logging.getLogger(__name__)
+
 
 class GCSResource(Resource):
     """GCS resource reference wrapper.
 
     This resource wraps GCS uris references such as file folders that you have stored in Google Cloud
     Storage with optional metadata and versioning. You assign it to a step.
 
@@ -39,15 +42,15 @@
         gcs_client: Client | None = None,
     ):
         """Initialize a GCS resource.
 
         Parameters:
             uris: The uris of the referenced resources. Should follow the pattern 'gs://<bucket_name>/<file_path_inside_bucket>'
             dataframes (Optional): The pandas dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats.
-            gcs_client (Optional): The `google.cloud.storage.Client` to optionally retrieve file size, creation date and updated date (used for auto-versioning).
+            gcs_client (Optional): The `google.cloud.storage.Client` to optionally retrieve file size, creation date and updated date (used for auto-versioning) up to 5000 files.
         """
         super().__init__(paths=uris, dataframes=dataframes)
         self.gcs_client = gcs_client
 
         for uri in self._paths:
             if not re.search(GS_URI_REG, uri):
                 raise ValueError(
@@ -57,15 +60,15 @@
     def _fetch_data(self) -> dict[str, bytes | None]:
         datas = {}
         for uri in self._paths:
             bucket_name, path = self._get_bucket_and_path_from_uri(uri)
             blobs = self._get_blobs(bucket_name, path)
             if blobs is not None:
                 for blob in blobs:
-                    datas[f"{bucket_name}/{path}"] = blob.download_as_bytes() if blob else None
+                    datas[f"{bucket_name}/{path}"] = blob
         return datas
 
     def _build_metadata(self) -> FilesMetadata:
         files = []
         size: int | None = None
         df_index = 0
         for uri in self._paths:
@@ -97,44 +100,32 @@
         metadata = FilesMetadata(
             size=size,
             origin=self._origin,
             files=files,
         )
         return metadata
 
-    def _get_blobs(self, bucket_name, path: str) -> list[Blob] | None:
-        from google.cloud import storage
-
+    def _get_blobs(self, bucket_name: str, path: str) -> list[Blob] | None:
         if self.gcs_client is None:
             return None
 
-        bucket: Bucket = storage.Bucket(self.gcs_client, name=bucket_name)
-        blob = self._recurse_blob(bucket, path)
-        return self._get_children_blobs(self.gcs_client, bucket_name, blob)
-
-    def _recurse_blob(self, bucket: Bucket, path: str) -> Blob:
-        blob = bucket.get_blob(blob_name=path)
-        if blob is None:
-            if path.endswith("/"):
-                raise NoSuchGCSResourceError(bucket.name, path)
-            return self._recurse_blob(bucket, f"{path}/")
-        return blob
-
-    def _get_children_blobs(self, gcs_client: Client, bucket_name: str, blob: Blob) -> list[Blob]:
-        path: str = blob.name
-        if path.endswith("/"):
-            all_blobs: list[Blob] = []
-            blobs: list[Blob] = gcs_client.list_blobs(bucket_or_name=bucket_name, prefix=path)
-            for bl in blobs:
-                if bl.name.endswith("/") is False:
-                    bl.reload()
-                    all_blobs.append(bl)
-            return all_blobs
-        blob.reload()
-        return [blob]
+        blobs_list = list(
+            filter(
+                lambda bl: bl.name.endswith("/") is False,
+                self.gcs_client.list_blobs(
+                    bucket_or_name=bucket_name, prefix=path, max_results=(self._files_limit + 2)
+                ),  # +2 for base directory and to check if more files than limit
+            )
+        )
+
+        if len(blobs_list) > self._files_limit:
+            _logger.warning(f"Only first {self._files_limit} files metadata were used.")
+            blobs_list.pop()
+
+        return blobs_list
 
     def _build_file_from_blob(self, blob: Blob, uri: str, dataframe: DataFrame | None = None) -> File:
         return File(
             name=blob.name,
             size=blob.size,
             fingerprint=blob.md5_hash,
             created_date=blob.time_created.isoformat(),
```

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/metadata/__init__.py` & `vectice-23.2.4.0/src/vectice/models/resource/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/metadata/base.py` & `vectice-23.2.4.0/src/vectice/models/resource/metadata/base.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/metadata/dataframe_column_parser.py` & `vectice-23.2.4.0/src/vectice/models/resource/metadata/dataframe_column_parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 from __future__ import annotations
 
 import logging
 
 import pandas as pd
 from pandas import DataFrame, Series, api
 
-from vectice.models.resource.metadata.column_metadata import Column, ColumnCategoryType, StatValue
-
-# mypy: ignore-errors
+from vectice.models.resource.metadata.column_metadata import (
+    BooleanStat,
+    Column,
+    ColumnCategoryType,
+    DateStat,
+    MostCommon,
+    NumericalStat,
+    Quantiles,
+    TextStat,
+)
 
 _logger = logging.getLogger(__name__)
 
 
-def capture_columns(init_columns: list[Column] | None, dataframe: DataFrame | None) -> dict:
+def capture_columns(init_columns: list[Column] | None, dataframe: DataFrame | None) -> list:
     init_columns = init_columns if init_columns is not None else []
     if dataframe is None:
         return [column.asdict() for column in init_columns]
 
     columns: list[Column] = []
     column_names_with_types = dataframe.dtypes.astype(str).to_dict()
     for idx, (name, d_type) in enumerate(column_names_with_types.items()):
@@ -32,128 +39,127 @@
                 category_type=category_type,
             )
         )
 
     return [column.asdict() for column in columns]
 
 
-def capture_column_stats(series: Series) -> tuple[str | None, list[StatValue] | None]:
+def capture_column_stats(
+    series: Series,
+) -> tuple[ColumnCategoryType | None, TextStat | BooleanStat | NumericalStat | DateStat | None]:
     if api.types.is_bool_dtype(series):
         return ColumnCategoryType.BOOLEAN, compute_boolean_column_statistics(series)
     elif api.types.is_numeric_dtype(series):
         return ColumnCategoryType.NUMERICAL, compute_numeric_column_statistics(series)
     elif api.types.is_datetime64_any_dtype(series) | (series.dtypes == "dbdate"):
         return ColumnCategoryType.DATE, compute_date_column_statistics(series)
-    elif api.types.is_string_dtype(series):
+    elif api.types.is_string_dtype(series) | api.types.is_categorical_dtype(series):
         return ColumnCategoryType.TEXT, compute_string_column_statistics(series)
     return None, None
 
 
-def compute_boolean_column_statistics(series: Series) -> list[StatValue]:
+def compute_boolean_column_statistics(series: Series) -> BooleanStat:
     """Parse a dataframe series and return statistics about it.
 
     The computed statistics are:
-    - the series count (size)
-    - the top value
-    - the frequence of the value
+    - The percentage of True
+    - The percentage of False
+    - The count missing value in %
     Parameters:
         series: The pandas series to get information from.
 
     Returns:
-        A list of StatValue.
+        A BooleanStat object containing the above statistics.
     """
-    value_counts = series.value_counts()
-    count = series.count()
-    top = value_counts.idxmax()
-    freq = value_counts.max()
-    return [
-        StatValue(key="count", value=int(count)),
-        StatValue(key="top", value=float(top) if isinstance(top, float) else int(top)),
-        StatValue(key="freq", value=float(freq) if isinstance(freq, float) else int(freq)),
-    ]
+    value_counts = series.value_counts(dropna=False)
+    value_counts = value_counts / value_counts.sum()
+    missing = series.isnull().sum() / len(series)
+
+    return BooleanStat(true=float(value_counts[True]), false=float(value_counts[False]), missing=float(missing))
 
 
-def compute_numeric_column_statistics(series: Series) -> list[StatValue]:
+def compute_numeric_column_statistics(series: Series) -> NumericalStat:
     """Parse a dataframe series and return statistics about it.
 
     The computed statistics are:
-    - the series count (size)
     - the mean
-    - the median
-    - the variance
     - the standard deviation
     - the min value
     - the 25% percentiles
     - the 50% percentiles
     - the 75% percentiles
     - the max value
+    - the count missing value in %
     Parameters:
         series: The pandas series to get information from.
 
     Returns:
-        A list of StatValue.
+        A NumericalStat object containing the above statistics.
     """
-    var = series.var()
-    med = series.median()
-    stats = [
-        StatValue("median", float(med) if isinstance(med, float) else int(med)),
-        StatValue("variance", float(var) if isinstance(var, float) else int(var)),
-    ]
-    stats.extend(
-        [
-            StatValue(str(name), float(value) if isinstance(value, float) else int(value))
-            for name, value in series.describe().items()
-        ]
+    mean = series.mean()
+    std = series.std()
+    min = series.min()
+    q25 = series.quantile(0.25)
+    q50 = series.quantile(0.5)
+    q75 = series.quantile(0.75)
+    max = series.max()
+    missing = series.isnull().sum() / len(series)
+
+    return NumericalStat(
+        mean=float(mean),
+        std_deviation=float(std),
+        quantiles=Quantiles(q_min=float(min), q25=float(q25), q50=float(q50), q75=float(q75), q_max=float(max)),
+        missing=float(missing),
     )
-    return stats
 
 
-def compute_string_column_statistics(series: Series) -> list[StatValue]:
+def compute_string_column_statistics(series: Series) -> TextStat:
     """Parse a dataframe series and return statistics about it.
 
     The computed statistics are:
-    - the null count
-    - the series count (size)
     - the unique number of value
-    - the most frequent value (top)
-    - the frequency of the top value
+    - the top 3 most common values with their percentages
+    - the count missing value in %
     Parameters:
         series: The pandas series to get information from.
 
     Returns:
-        A list of StatValue.
+        A TextStat object containing the above statistics.
     """
-    stats = [StatValue("null", int(series.isna().sum()))]
-    for name, value in series.describe(include="all").items():
-        stats.extend([StatValue(str(name), int(value) if isinstance(value, (int, float)) else str(value))])
-
-    return stats
+    missing = series.isnull().sum() / len(series)
+    unique = len(series.unique())
+    value_counts: Series[float] = series.value_counts() / series.value_counts(dropna=False).sum()
+
+    size = 3 if unique >= 3 else unique
+    value_counts = value_counts.nlargest(size)
+
+    return TextStat(
+        unique=float(unique),
+        missing=float(missing),
+        most_commons=[MostCommon(str(i), float(value_counts[i])) for i in value_counts.index],
+    )
 
 
-def compute_date_column_statistics(series: Series) -> list[StatValue]:
+def compute_date_column_statistics(series: Series) -> DateStat:
     """Parse a dataframe series and return statistics about it.
 
     The computed statistics are:
-    - the min value
+    - the first date
     - the mean
-    - max value
-    - the null count
+    - the median
+    - the last date
+    - the count missing value in %
     Parameters:
         series: The pandas series to get information from.
 
     Returns:
-        A list of StatValue.
+        A DateStat object containing the above statistics.
     """
     # Convert to datetime since mean is not supported for non datetime pandas object such as dbdates
     series = pd.to_datetime(series)
-    min = series.min().date()
-    mean = series.mean().date()
-    median = series.median().date()
-    max = series.max().date()
-
-    return [
-        StatValue("null", int(series.isna().sum())),
-        StatValue(key="min", value=str(min)),
-        StatValue(key="mean", value=str(mean)),
-        StatValue(key="median", value=str(median)),
-        StatValue(key="max", value=str(max)),
-    ]
+    min = series.min().isoformat()
+    mean = series.mean().isoformat()
+    median = series.median().isoformat()
+    max = series.max().isoformat()
+    missing = series.isnull().sum() / len(series)
+
+    return DateStat(missing=float(missing), minimum=str(min), mean=str(mean), median=str(median), maximum=str(max))
```

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/metadata/db_metadata.py` & `vectice-23.2.4.0/src/vectice/models/resource/metadata/db_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/metadata/files_metadata.py` & `vectice-23.2.4.0/src/vectice/models/resource/metadata/files_metadata.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/metadata/source.py` & `vectice-23.2.4.0/src/vectice/models/resource/metadata/source.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/resource/s3_resource.py` & `vectice-23.2.4.0/src/vectice/models/resource/s3_resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import logging
 import re
 from typing import TYPE_CHECKING
 
 from pandas import DataFrame
 
 from vectice.models.resource.base import Resource
 from vectice.models.resource.metadata.base import DatasetSourceOrigin
@@ -13,14 +14,17 @@
     from mypy_boto3_s3 import Client
     from mypy_boto3_s3.type_defs import ListObjectsV2OutputTypeDef, ObjectTypeDef
 
 
 S3_URI_REG = r"(s3:\/\/)([^\/]+)\/(.+)"
 
 
+_logger = logging.getLogger(__name__)
+
+
 class S3Resource(Resource):
     """AWS S3resource reference wrapper.
 
     This resource wraps AWS S3 uris references such as file folders that you have stored in AWS S3
     with optional metadata and versioning. You assign it to a step.
 
     ```python
@@ -41,62 +45,57 @@
         s3_client: Client | None = None,
     ):
         """Initialize an S3 resource.
 
         Parameters:
             uris: The uris of the resources to get. Should follow the pattern 's3://<bucket_name>/<file_path_inside_bucket>'
             dataframes (Optional): The pandas dataframes allowing vectice to optionally compute more metadata about this resource such as columns stats.
-            s3_client (Optional): The Amazon s3 client to optionally retrieve file size, creation date and updated date (used for auto-versioning).
+            s3_client (Optional): The Amazon s3 client to optionally retrieve file size, creation date and updated date (used for auto-versioning) up to 5000 files.
         """
         super().__init__(paths=uris, dataframes=dataframes)
         self.s3_client = s3_client
 
         for uri in self._paths:
             if not re.search(S3_URI_REG, uri):
                 raise ValueError(
                     f"Uri '{uri}' is not following the right pattern 's3://<bucket_name>/<file_path_inside_bucket>'"
                 )
 
-    def _fetch_data(self) -> dict[str, bytes | None]:
-        datas = {}
+    def _fetch_data(self) -> dict[str, ObjectTypeDef | None]:
+        datas: dict[str, ObjectTypeDef | None] = {}
         if self.s3_client:
-            s3_objects_list = self._get_s3_objects_list(self.s3_client)
-            for bucket_name, s3_objects in s3_objects_list:
-                for s3_object in s3_objects["Contents"]:
-                    object_path = s3_object["Key"]
-                    data = self._get_aws_data(self.s3_client, bucket_name, object_path)
-                    datas[f"{bucket_name}/{object_path}"] = data
+            for bucket_name, s3_objects_list in self._get_s3_objects_list(self.s3_client):
+                for s3_objects in s3_objects_list:
+                    for s3_object in s3_objects["Contents"]:
+                        object_path = s3_object["Key"]
+                        datas[f"{bucket_name}/{object_path}"] = s3_object
         else:
             for path in self._paths:
                 datas[path] = None
 
         return datas
 
-    def _get_aws_data(self, s3_client: Client, bucket_name: str, object_path: str):
-        data_response = s3_client.get_object(Bucket=bucket_name, Key=object_path)
-        return data_response["Body"].read()
-
     def _build_metadata(self) -> FilesMetadata:
         size = None
         files = []
         df_index = 0
         if self.s3_client:
-            s3_objects_list = self._get_s3_objects_list(self.s3_client)
-            for bucket_name, s3_objects in s3_objects_list:
-                if s3_objects["KeyCount"] == 0:
-                    raise NoSuchS3ResourceError(bucket_name, s3_objects["Prefix"])
-                s3_object = s3_objects["Contents"]
-                new_files, total_size, new_df_index = self._build_files_list_with_size(
-                    index=df_index, bucket_name=bucket_name, s3_object=s3_object
-                )
-                if size is None:
-                    size = 0
-                size += total_size
-                files.extend(new_files)
-                df_index += new_df_index
+            for bucket_name, s3_objects_list in self._get_s3_objects_list(self.s3_client):
+                for s3_objects in s3_objects_list:
+                    if s3_objects["KeyCount"] == 0:
+                        raise NoSuchS3ResourceError(bucket_name, s3_objects["Prefix"])
+                    s3_object = s3_objects["Contents"]
+                    new_files, total_size, new_df_index = self._build_files_list_with_size(
+                        index=df_index, bucket_name=bucket_name, s3_object=s3_object
+                    )
+                    if size is None:
+                        size = 0
+                    size += total_size
+                    files.extend(new_files)
+                    df_index += new_df_index
         else:
             for index, uri in enumerate(self._paths):
                 dataframe = (
                     self._dataframes[index] if self._dataframes is not None and len(self._dataframes) > index else None
                 )
                 _, path = self._get_bucket_and_path_from_uri(uri)
                 file = File(name=path, uri=uri, dataframe=dataframe)
@@ -134,20 +133,42 @@
                 dataframe=dataframe,
             )
             total_size += size
             files.append(file)
             df_index += 1
         return files, total_size, df_index
 
-    def _get_s3_objects_list(self, s3_client: Client) -> list[tuple[str, ListObjectsV2OutputTypeDef]]:
+    def _get_s3_objects_list(self, s3_client: Client) -> list[tuple[str, list[ListObjectsV2OutputTypeDef]]]:
         return list(map(lambda uri: self._get_s3_objects(s3_client, uri), self._paths))
 
-    def _get_s3_objects(self, s3_client: Client, uri: str) -> tuple[str, ListObjectsV2OutputTypeDef]:
+    def _get_s3_objects(self, s3_client: Client, uri: str) -> tuple[str, list[ListObjectsV2OutputTypeDef]]:
         bucket_name, path = self._get_bucket_and_path_from_uri(uri)
-        return bucket_name, s3_client.list_objects_v2(Bucket=bucket_name, Prefix=path)
+        results: list[ListObjectsV2OutputTypeDef] = []
+        next_token: str | None = ""
+        base_kwargs = {
+            "Bucket": bucket_name,
+            "Prefix": path,
+        }
+        count = 0
+        while next_token is not None:
+            kwargs = base_kwargs.copy()
+            if next_token != "":
+                kwargs.update({"ContinuationToken": next_token})
+
+            result = s3_client.list_objects_v2(**kwargs)  # type: ignore[arg-type]
+            count += result["KeyCount"]
+            if count >= self._files_limit:
+                _logger.warning(f"Only first {self._files_limit} files metadata were used.")
+                next_token = None
+            else:
+                next_token = result.get("NextContinuationToken")
+
+            results.append(result)
+
+        return bucket_name, results
 
     def _get_bucket_and_path_from_uri(self, uri: str) -> tuple[str, str]:
         match = re.search(S3_URI_REG, uri)
         if match is not None:
             _, bucket_name, path = match.groups()
             return bucket_name, path
```

### Comparing `vectice-23.2.3.1/src/vectice/models/step.py` & `vectice-23.2.4.0/src/vectice/models/step.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
         self._artifacts = artifacts or []
         self._slug = slug
         self._type: StepType = step_type
         self._model: Model | None = None
 
         self._iteration_read_only = self._iteration._status in {IterationStatus.Completed, IterationStatus.Abandoned}
         if self._iteration_read_only:
-            _logger.debug(f"Step {self.name}, iteration is {self._iteration._status.name} and is read-only!")
+            _logger.debug(f"Step {self.name}, iteration is {self._iteration.status} and is read-only!")
 
     def __repr__(self):
         return f"Step(name={self.name!r}, slug={self.slug!r}, id={self.id!r})"
 
     def __eq__(self, other: object):
         if not isinstance(other, Step):
             return NotImplemented
```

### Comparing `vectice-23.2.3.1/src/vectice/models/step_dataset.py` & `vectice-23.2.4.0/src/vectice/models/step_dataset.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/step_image.py` & `vectice-23.2.4.0/src/vectice/models/step_image.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/step_model.py` & `vectice-23.2.4.0/src/vectice/models/step_model.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/step_number.py` & `vectice-23.2.4.0/src/vectice/models/step_number.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/step_string.py` & `vectice-23.2.4.0/src/vectice/models/step_string.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/models/workspace.py` & `vectice-23.2.4.0/src/vectice/models/workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 from textwrap import dedent
 from typing import TYPE_CHECKING
 
 from rich.table import Table
 
 from vectice.models.project import Project
 from vectice.utils.common_utils import _temp_print
-from vectice.utils.last_assets import _get_last_user_and_default_workspace
 from vectice.utils.logging_utils import format_description
 
 if TYPE_CHECKING:
     from vectice import Connection
     from vectice.api import Client
 
 
@@ -129,46 +128,42 @@
 
         Returns:
             The project.
         """
         item = self._client.get_project(project, self.name)
         logging_output = dedent(
             f"""
-                Project '{item.name!r}' successfully retrieved."
+                Project {item.name!r} successfully retrieved."
 
-                For quick access to the Dataset in the Vectice web app, visit:
+                For quick access to the Project in the Vectice web app, visit:
                 {self._client.auth._API_BASE_URL}/browse/project/{item.id}"""
         ).lstrip()
         _logger.info(logging_output)
         project_object = Project(item.id, self, item.name, item.description)
         return project_object
 
     def list_projects(self) -> None:
         """Prints a list of projects belonging to the workspace in a tabular format, limited to the first 10 items. A link is provided to view the remaining projects.
 
         Returns:
             None
         """
-        project_outputs = self.projects
-        user_name, _ = _get_last_user_and_default_workspace(self._client)
-
+        project_outputs = self._client.list_projects(self.id)
         rich_table = Table(expand=True, show_edge=False)
 
-        rich_table.add_column("project id", justify="left", no_wrap=True, min_width=4, max_width=10)
-        rich_table.add_column("name", justify="left", no_wrap=True, max_width=15)
-        rich_table.add_column("description", justify="left", no_wrap=True, max_width=50)
-
-        for count, project in enumerate(project_outputs, 1):
-            if count > 10:
-                break
+        rich_table.add_column("Project id", justify="left", no_wrap=True, min_width=4, max_width=10)
+        rich_table.add_column("Name", justify="left", no_wrap=True, max_width=15)
+        rich_table.add_column("Description", justify="left", no_wrap=True, max_width=50)
+
+        for project in project_outputs.list:
             rich_table.add_row(project.id, project.name, format_description(project.description))
 
         description = dedent(
             f"""
-        There are {len(project_outputs)} projects in the workspace {self.name!r} and a maximum of 10 projects are displayed in the table below:
+        There are {project_outputs.total} projects in the workspace {self.name!r} and a maximum of 10 projects are displayed in the table below:
         """
         ).lstrip()
         tips = dedent(
             """
         To access a specific project, use \033[1mworkspace\033[0m.project(Project ID)"""
         ).lstrip()
         link = dedent(
@@ -186,15 +181,15 @@
     def projects(self) -> list[Project]:
         """List projects.
 
         Returns:
             A list of projects in this workspace.
         """
         response = self._client.list_projects(self.id)
-        return [Project(item.id, self, item.name, item.description) for item in response]
+        return [Project(item.id, self, item.name, item.description) for item in response.list]
 
     @property
     def connection(self) -> Connection:
         """The Connection to which this workspace belongs.
 
         Returns:
             The Connection to which this workspace belongs.
```

### Comparing `vectice-23.2.3.1/src/vectice/utils/automatic_link_utils.py` & `vectice-23.2.4.0/src/vectice/utils/automatic_link_utils.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/utils/common_utils.py` & `vectice-23.2.4.0/src/vectice/utils/common_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from __future__ import annotations
 
 import logging
 import os
+import re
 from contextlib import contextmanager
 from io import BytesIO, IOBase
 from pathlib import Path
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Dict, Union
 
+from gql.transport.exceptions import TransportQueryError
 from PIL import Image, UnidentifiedImageError
 from rich.console import Console
 from rich.table import Table
 
 from vectice.api.json.iteration import IterationStatus, IterationStepArtifact
 from vectice.api.json.step import StepType
 
@@ -26,28 +28,28 @@
         logging.getLogger(package).setLevel(logging.ERROR)
         yield
     finally:
         logging.getLogger(package).setLevel(old_level)
 
 
 def _check_read_only(iteration: Iteration):
-    """Check if an iteration is completed or canceled.
+    """Check if an iteration is completed or cancelled.
 
     Refreshing the iteration is necessary because in a Jupyter notebook
     its status could have changed on the backend.
 
     Parameters:
         iteration: The iteration to check.
 
     Raises:
-        RuntimeError: When the iteration is read-only (completed or canceled).
+        RuntimeError: When the iteration is read-only (completed or cancelled).
     """
     refresh_iteration = iteration._phase.iteration(iteration.index)
     if refresh_iteration._status in {IterationStatus.Completed, IterationStatus.Abandoned}:
-        raise RuntimeError(f"The Iteration is {refresh_iteration._status.name} and is read-only.")
+        raise RuntimeError(f"The Iteration is {refresh_iteration.status} and is read-only.")
 
 
 def _get_step_type(
     id: int,
     iteration: Iteration,
     name: str,
     index: int,
@@ -87,33 +89,37 @@
         artifact = artifacts[len(artifacts) - 1]
         if step_type is StepType.StepNumber:
             number = _get_number(artifact.text) if artifact.text else None
             return StepNumber(step, number)
         if step_type is StepType.StepString:
             return StepString(step, str(artifact.text))
         if step_type is StepType.StepImage:
-            image = _get_image_info(iteration, artifacts) if artifacts else None
+            image = _get_image_info(iteration, artifact)
+            if image is None:
+                return step
             return StepImage(step, image=image)
         if step_type is StepType.StepDataset:
             dataset_version = artifact
             return StepDataset(step, dataset_version=dataset_version)
         if step_type is StepType.StepModel:
             model_version = artifact
             return StepModel(step, model_version=model_version)
     return step
 
 
-def _get_image_info(iteration: Iteration, artifacts: list[IterationStepArtifact]):
-    artifacts = [image for image in artifacts if image.type.value == "EntityFile"]
-    artifact = artifacts[len(artifacts) - 1] if len(artifacts) >= 1 else None
-    attachments = iteration._client.list_phase_attachments(iteration.phase.id, iteration.project.id)
-    if not artifact:
+def _get_image_info(iteration: Iteration, artifact: IterationStepArtifact):
+    ef_id = artifact.entity_file_id
+    if ef_id is None:
+        return None
+
+    try:
+        image = iteration._client.get_entity_file_by_id(ef_id)
+        return image.file_name
+    except TransportQueryError:
         return None
-    image = next(img for img in attachments.list if img.fileId == artifact.entity_file_id)
-    return image.fileName
 
 
 def _check_image_path(path: str) -> bool:
     try:
         check_path = Path(path).exists()
     except OSError:
         return False
@@ -159,7 +165,19 @@
     console = Console(width=120)
     if string:
         print(string)
         print()
     if table:
         console.print(table)
         print()
+
+
+def _convert_keys_to_camel_case(input_dict: Dict[str, Any]) -> Dict[str, Union[Any, Dict[str, Any]]]:
+    camel_case_dict: Dict[str, Union[Any, Dict[str, Any]]] = {}
+
+    for key, value in input_dict.items():
+        camel_case_key = re.sub(r"_([a-z])", lambda match: match.group(1).upper(), key)
+        if isinstance(value, dict):
+            value = _convert_keys_to_camel_case(value)
+        camel_case_dict[camel_case_key] = value
+
+    return camel_case_dict
```

### Comparing `vectice-23.2.3.1/src/vectice/utils/configuration.py` & `vectice-23.2.4.0/src/vectice/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/utils/deprecation.py` & `vectice-23.2.4.0/src/vectice/utils/deprecation.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from functools import wraps
 from typing import Any, Callable
 
 from packaging.version import Version
 
 from vectice.__version__ import __version__
 
-CURRENT_VERSION = Version(__version__)
+CURRENT_VERSION = Version(Version(__version__).base_version)
 _WARN_DEPR_REMOVAL = os.getenv("VECTICE_WARN_DEPR_REMOVAL", "0") == "1"
 
 
 class DeprecationError(BaseException):
     """An exception raised when a deprecated object is used."""
```

### Comparing `vectice-23.2.3.1/src/vectice/utils/last_assets.py` & `vectice-23.2.4.0/src/vectice/utils/last_assets.py`

 * *Files identical despite different names*

### Comparing `vectice-23.2.3.1/src/vectice/utils/logging_utils.py` & `vectice-23.2.4.0/src/vectice/utils/logging_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,26 +132,26 @@
 
 def format_description(description: str | None) -> str | None:
     if not description:
         return None
     return description
 
 
-def get_iteration_status(status: IterationStatus, starred: bool | None) -> str:
+def get_iteration_status(status: IterationStatus, starred: bool | None = None) -> str:
     verbose_dict: dict[str, str | None] = defaultdict(lambda: None)
     verbose_dict["NotStarted"] = "Not Started"
     verbose_dict["InProgress"] = "In Progress"
-    verbose_dict["Abandoned"] = "Abandoned"
+    verbose_dict["Abandoned"] = "Cancelled"
     verbose_dict["Completed"] = "Completed"
     verbose_dict["InReview"] = "In Review"
 
     status_value = verbose_dict[status.value]
     if status_value is None:
         raise ValueError("Iteration status unknown")
-    if starred:
+    if starred is True:
         return status_value + " (*)"
     return status_value
 
 
 def get_phase_status(status: PhaseStatus) -> str:
     verbose_dict: dict[str, str | None] = defaultdict(lambda: None)
     verbose_dict["NotStarted"] = "Not Started"
```

### Comparing `vectice-23.2.3.1/src/vectice.egg-info/PKG-INFO` & `vectice-23.2.4.0/src/vectice.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: vectice
-Version: 23.2.3.1
+Version: 23.2.4.0
 Summary: Vectice Python library
 Home-page: https://www.vectice.com
 Author: Vectice Inc.
 Author-email: sdk@vectice.com
 License: Apache License 2.0
 Keywords: Vectice,Client,API,Adapter
 Platform: Linux
 Platform: MacOS X
 Platform: Windows
 Classifier: Topic :: Internet
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `vectice-23.2.3.1/src/vectice.egg-info/SOURCES.txt` & `vectice-23.2.4.0/src/vectice.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 src/vectice/api/attachment.py
 src/vectice/api/client.py
 src/vectice/api/compatibility.py
 src/vectice/api/gql_api.py
 src/vectice/api/gql_code.py
 src/vectice/api/gql_code_version.py
 src/vectice/api/gql_dataset.py
+src/vectice/api/gql_entity_file.py
 src/vectice/api/gql_feature_flag.py
 src/vectice/api/gql_model.py
 src/vectice/api/gql_user_workspace_api.py
 src/vectice/api/http_error.py
 src/vectice/api/http_error_handlers.py
 src/vectice/api/iteration.py
 src/vectice/api/json_object.py
@@ -42,14 +43,15 @@
 src/vectice/api/json/code.py
 src/vectice/api/json/code_version.py
 src/vectice/api/json/compatibility.py
 src/vectice/api/json/dataset_register.py
 src/vectice/api/json/dataset_representation.py
 src/vectice/api/json/dataset_version.py
 src/vectice/api/json/dataset_version_representation.py
+src/vectice/api/json/entity_file.py
 src/vectice/api/json/files_metadata.py
 src/vectice/api/json/iteration.py
 src/vectice/api/json/last_assets.py
 src/vectice/api/json/metric.py
 src/vectice/api/json/model.py
 src/vectice/api/json/model_register.py
 src/vectice/api/json/model_representation.py
```

### Comparing `vectice-23.2.3.1/src/vectice.egg-info/requires.txt` & `vectice-23.2.4.0/src/vectice.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 rich
 urllib3
 gql[requests]
 GitPython
 packaging
 Pillow
 pandas
+typing-extensions==4.6.2
 
 [dev]
 black
 gitpython
 mypy
 ruff
 types-requests
```

